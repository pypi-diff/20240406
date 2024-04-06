# Comparing `tmp/seacrowd-0.0.1.tar.gz` & `tmp/seacrowd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seacrowd-0.0.1.tar", last modified: Thu Apr  4 08:03:02 2024, max compression
+gzip compressed data, was "seacrowd-0.0.2.tar", last modified: Sat Apr  6 05:07:40 2024, max compression
```

## Comparing `seacrowd-0.0.1.tar` & `seacrowd-0.0.2.tar`

### file list

```diff
@@ -1,979 +1,980 @@
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.937176 seacrowd-0.0.1/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.1/LICENSE
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-04 08:03:02.933293 seacrowd-0.0.1/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.1/README.md
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:53.953556 seacrowd-0.0.1/seacrowd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       58 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.042715 seacrowd-0.0.1/seacrowd/sea_datasets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.064381 seacrowd-0.0.1/seacrowd/sea_datasets/abui_wordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/abui_wordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.090358 seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.119828 seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.167677 seacrowd-0.0.1/seacrowd/sea_datasets/ara_close/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ara_close/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ara_close/ara_close.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.194428 seacrowd-0.0.1/seacrowd/sea_datasets/asr_sindodusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/asr_sindodusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.220667 seacrowd-0.0.1/seacrowd/sea_datasets/asr_smaldusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/asr_smaldusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.255397 seacrowd-0.0.1/seacrowd/sea_datasets/asr_stidusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/asr_stidusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.277462 seacrowd-0.0.1/seacrowd/sea_datasets/audio_keyword_spotting/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.297603 seacrowd-0.0.1/seacrowd/sea_datasets/aya_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/aya_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.342658 seacrowd-0.0.1/seacrowd/sea_datasets/barasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/barasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/barasa/barasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.368575 seacrowd-0.0.1/seacrowd/sea_datasets/beaye_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/beaye_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.390528 seacrowd-0.0.1/seacrowd/sea_datasets/belebele/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/belebele/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8594 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/belebele/belebele.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.416755 seacrowd-0.0.1/seacrowd/sea_datasets/bible_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bible_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.458461 seacrowd-0.0.1/seacrowd/sea_datasets/bible_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bible_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.480029 seacrowd-0.0.1/seacrowd/sea_datasets/bible_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bible_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.509603 seacrowd-0.0.1/seacrowd/sea_datasets/bioner_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bioner_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bioner_id/bioner_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.542657 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_captioning/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_captioning/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.571341 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_lm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_lm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.596352 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_speech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_speech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.625521 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_vist/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_vist/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.653695 seacrowd-0.0.1/seacrowd/sea_datasets/burapha_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/burapha_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/burapha_th/burapha_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.674643 seacrowd-0.0.1/seacrowd/sea_datasets/burmese_romanize/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/burmese_romanize/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.695008 seacrowd-0.0.1/seacrowd/sea_datasets/casa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/casa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/casa/casa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.721295 seacrowd-0.0.1/seacrowd/sea_datasets/cc100/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cc100/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cc100/cc100.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.747490 seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_doc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.774624 seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_sent/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.796605 seacrowd-0.0.1/seacrowd/sea_datasets/cebuaner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cebuaner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cebuaner/cebuaner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.822153 seacrowd-0.0.1/seacrowd/sea_datasets/coco_35l/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/coco_35l/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9814 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/coco_35l/coco_35l.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.849829 seacrowd-0.0.1/seacrowd/sea_datasets/cod/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cod/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cod/cod.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.872795 seacrowd-0.0.1/seacrowd/sea_datasets/code_mixed_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.892556 seacrowd-0.0.1/seacrowd/sea_datasets/codeswitch_reddit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.914607 seacrowd-0.0.1/seacrowd/sea_datasets/commonvoice_120/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/commonvoice_120/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.961465 seacrowd-0.0.1/seacrowd/sea_datasets/copal/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/copal/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/copal/copal.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:54.982378 seacrowd-0.0.1/seacrowd/sea_datasets/covost2/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/covost2/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/covost2/covost2.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.008150 seacrowd-0.0.1/seacrowd/sea_datasets/creole_rc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.1/seacrowd/sea_datasets/creole_rc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/creole_rc/creole_rc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.040150 seacrowd-0.0.1/seacrowd/sea_datasets/crosssum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/crosssum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/crosssum/crosssum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.060066 seacrowd-0.0.1/seacrowd/sea_datasets/cub_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cub_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.086610 seacrowd-0.0.1/seacrowd/sea_datasets/culturax/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/culturax/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/culturax/culturax.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.111439 seacrowd-0.0.1/seacrowd/sea_datasets/cvss/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cvss/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/cvss/cvss.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.144259 seacrowd-0.0.1/seacrowd/sea_datasets/dengue_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/dengue_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4761 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.168660 seacrowd-0.0.1/seacrowd/sea_datasets/emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emot/emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.188755 seacrowd-0.0.1/seacrowd/sea_datasets/emotcmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emotcmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emotcmt/emotcmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.243887 seacrowd-0.0.1/seacrowd/sea_datasets/emotes_3k/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emotes_3k/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.262483 seacrowd-0.0.1/seacrowd/sea_datasets/emotion_id_opinion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.283239 seacrowd-0.0.1/seacrowd/sea_datasets/etos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/etos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/etos/etos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.304594 seacrowd-0.0.1/seacrowd/sea_datasets/facqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/facqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/facqa/facqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.329229 seacrowd-0.0.1/seacrowd/sea_datasets/facqa/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/facqa/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.351738 seacrowd-0.0.1/seacrowd/sea_datasets/fakenews_ph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/fakenews_ph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.371821 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_gay_lang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.392134 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.413539 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_slang_norm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.436432 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_words_aoa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.456478 seacrowd-0.0.1/seacrowd/sea_datasets/filwordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filwordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/filwordnet/filwordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.476503 seacrowd-0.0.1/seacrowd/sea_datasets/fleurs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/fleurs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13189 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/fleurs/fleurs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.501438 seacrowd-0.0.1/seacrowd/sea_datasets/flores200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/flores200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/flores200/flores200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.524887 seacrowd-0.0.1/seacrowd/sea_datasets/fsl_105/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/fsl_105/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/fsl_105/fsl_105.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.552068 seacrowd-0.0.1/seacrowd/sea_datasets/gatitos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/gatitos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/gatitos/gatitos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.578257 seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_newsclass/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.598947 seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.624699 seacrowd-0.0.1/seacrowd/sea_datasets/globalwoz/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/globalwoz/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/globalwoz/globalwoz.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.663956 seacrowd-0.0.1/seacrowd/sea_datasets/glotstorybook/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/glotstorybook/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.682642 seacrowd-0.0.1/seacrowd/sea_datasets/hoasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/hoasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/hoasa/hoasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.701299 seacrowd-0.0.1/seacrowd/sea_datasets/iapp_squad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/iapp_squad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.731232 seacrowd-0.0.1/seacrowd/sea_datasets/iatf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/iatf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/iatf/iatf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.759808 seacrowd-0.0.1/seacrowd/sea_datasets/icon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/icon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/icon/icon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.779583 seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive/id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.798974 seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive_news_comment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.823656 seacrowd-0.0.1/seacrowd/sea_datasets/id_am2ico/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_am2ico/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.856893 seacrowd-0.0.1/seacrowd/sea_datasets/id_clickbait/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_clickbait/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.876526 seacrowd-0.0.1/seacrowd/sea_datasets/id_coreference_resolution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.899237 seacrowd-0.0.1/seacrowd/sea_datasets/id_frog_story/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_frog_story/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.925423 seacrowd-0.0.1/seacrowd/sea_datasets/id_google_play_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_google_play_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.952511 seacrowd-0.0.1/seacrowd/sea_datasets/id_hatespeech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_hatespeech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.974618 seacrowd-0.0.1/seacrowd/sea_datasets/id_hoax_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_hoax_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:55.995452 seacrowd-0.0.1/seacrowd/sea_datasets/id_hsd_nofaaulia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.024615 seacrowd-0.0.1/seacrowd/sea_datasets/id_msvd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_msvd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5035 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_msvd/id_msvd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.043537 seacrowd-0.0.1/seacrowd/sea_datasets/id_multilabel_hs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.066028 seacrowd-0.0.1/seacrowd/sea_datasets/id_panl_bppt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_panl_bppt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.086013 seacrowd-0.0.1/seacrowd/sea_datasets/id_qqp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_qqp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_qqp/id_qqp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.105952 seacrowd-0.0.1/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.132582 seacrowd-0.0.1/seacrowd/sea_datasets/id_sentiment_analysis/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.158165 seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.178169 seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.198789 seacrowd-0.0.1/seacrowd/sea_datasets/id_stance/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_stance/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_stance/id_stance.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.228937 seacrowd-0.0.1/seacrowd/sea_datasets/id_sts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_sts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_sts/id_sts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.249127 seacrowd-0.0.1/seacrowd/sea_datasets/id_vaccines_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.268301 seacrowd-0.0.1/seacrowd/sea_datasets/id_wiki_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.287653 seacrowd-0.0.1/seacrowd/sea_datasets/id_wsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_wsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/id_wsd/id_wsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.315573 seacrowd-0.0.1/seacrowd/sea_datasets/identic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/identic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/identic/identic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.352028 seacrowd-0.0.1/seacrowd/sea_datasets/identifikasi_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.373590 seacrowd-0.0.1/seacrowd/sea_datasets/idk_mrc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/idk_mrc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.394831 seacrowd-0.0.1/seacrowd/sea_datasets/idn_tagged_corpus_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.421499 seacrowd-0.0.1/seacrowd/sea_datasets/ijelid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ijelid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ijelid/ijelid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.452574 seacrowd-0.0.1/seacrowd/sea_datasets/imdb_jv/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/imdb_jv/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.472078 seacrowd-0.0.1/seacrowd/sea_datasets/indo4b/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo4b/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo4b/indo4b.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.497242 seacrowd-0.0.1/seacrowd/sea_datasets/indo4b_plus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo4b_plus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.528736 seacrowd-0.0.1/seacrowd/sea_datasets/indo_general_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.550188 seacrowd-0.0.1/seacrowd/sea_datasets/indo_law/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_law/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_law/indo_law.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.580249 seacrowd-0.0.1/seacrowd/sea_datasets/indo_puisi/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_puisi/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.605360 seacrowd-0.0.1/seacrowd/sea_datasets/indo_religious_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.631770 seacrowd-0.0.1/seacrowd/sea_datasets/indo_story_cloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_story_cloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.654836 seacrowd-0.0.1/seacrowd/sea_datasets/indocamrest/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocamrest/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocamrest/indocamrest.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.674202 seacrowd-0.0.1/seacrowd/sea_datasets/indocollex/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocollex/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocollex/indocollex.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.693370 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/indocoref.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.742867 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/file_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.764821 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ner_ugm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.786893 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_nerui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_nerui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.818521 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ntp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ntp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.844727 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.870793 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_tweet_ordering/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.891272 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_gsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.931182 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_pud/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.956925 seacrowd-0.0.1/seacrowd/sea_datasets/indoler/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indoler/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indoler/indoler.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:56.977164 seacrowd-0.0.1/seacrowd/sea_datasets/indommlu/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indommlu/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indommlu/indommlu.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.006238 seacrowd-0.0.1/seacrowd/sea_datasets/indoner_tourism/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indoner_tourism/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.026131 seacrowd-0.0.1/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.056358 seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.076166 seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_news_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4543 2024-04-04 06:00:47.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.095352 seacrowd-0.0.1/seacrowd/sea_datasets/indonesiannmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesiannmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.119193 seacrowd-0.0.1/seacrowd/sea_datasets/indonglish/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonglish/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonglish/indonglish.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.146039 seacrowd-0.0.1/seacrowd/sea_datasets/indonli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonli/indonli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.166742 seacrowd-0.0.1/seacrowd/sea_datasets/indonlu_nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.185498 seacrowd-0.0.1/seacrowd/sea_datasets/indoqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indoqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indoqa/indoqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.203970 seacrowd-0.0.1/seacrowd/sea_datasets/indosmd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indosmd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indosmd/indosmd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.236024 seacrowd-0.0.1/seacrowd/sea_datasets/indosum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indosum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indosum/indosum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.262868 seacrowd-0.0.1/seacrowd/sea_datasets/indotacos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indotacos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indotacos/indotacos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.282762 seacrowd-0.0.1/seacrowd/sea_datasets/indowiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indowiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indowiki/indowiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.304745 seacrowd-0.0.1/seacrowd/sea_datasets/indqner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indqner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indqner/indqner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.333221 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_digit_cdsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.353613 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.374086 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.397777 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.431332 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.462423 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.490440 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.510653 seacrowd-0.0.1/seacrowd/sea_datasets/inset_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/inset_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.530732 seacrowd-0.0.1/seacrowd/sea_datasets/jadi_ide/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/jadi_ide/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.560718 seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.585337 seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.602477 seacrowd-0.0.1/seacrowd/sea_datasets/kamus_alay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kamus_alay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.621999 seacrowd-0.0.1/seacrowd/sea_datasets/karonese_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/karonese_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.646803 seacrowd-0.0.1/seacrowd/sea_datasets/kawat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kawat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kawat/kawat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.667012 seacrowd-0.0.1/seacrowd/sea_datasets/kde4/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kde4/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kde4/kde4.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.689136 seacrowd-0.0.1/seacrowd/sea_datasets/keps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/keps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/keps/keps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.714060 seacrowd-0.0.1/seacrowd/sea_datasets/kheng_info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kheng_info/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kheng_info/kheng_info.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.736143 seacrowd-0.0.1/seacrowd/sea_datasets/khmer_alt_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.754633 seacrowd-0.0.1/seacrowd/sea_datasets/khpos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/khpos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/khpos/khpos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.776464 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.796043 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.825575 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_nllb/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_nllb/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.852121 seacrowd-0.0.1/seacrowd/sea_datasets/korpus_nusantara/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/korpus_nusantara/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.871658 seacrowd-0.0.1/seacrowd/sea_datasets/lazada_review_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.891963 seacrowd-0.0.1/seacrowd/sea_datasets/librivox_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/librivox_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.918173 seacrowd-0.0.1/seacrowd/sea_datasets/limesoda/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/limesoda/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/limesoda/limesoda.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.949328 seacrowd-0.0.1/seacrowd/sea_datasets/liputan6/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/liputan6/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/liputan6/liputan6.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.975980 seacrowd-0.0.1/seacrowd/sea_datasets/local_id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/local_id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:57.996003 seacrowd-0.0.1/seacrowd/sea_datasets/lr_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/lr_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/lr_sum/lr_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.034011 seacrowd-0.0.1/seacrowd/sea_datasets/m3exam/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/m3exam/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/m3exam/m3exam.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.055420 seacrowd-0.0.1/seacrowd/sea_datasets/mabl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mabl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mabl/mabl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.077860 seacrowd-0.0.1/seacrowd/sea_datasets/malaysia_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/malaysia_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.097140 seacrowd-0.0.1/seacrowd/sea_datasets/malindo_morph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/malindo_morph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.129182 seacrowd-0.0.1/seacrowd/sea_datasets/malindo_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/malindo_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.160166 seacrowd-0.0.1/seacrowd/sea_datasets/massive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/massive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.1/seacrowd/sea_datasets/massive/massive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.184098 seacrowd-0.0.1/seacrowd/sea_datasets/mc4_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mc4_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5495 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.202939 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_brunei/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_brunei/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.255672 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sabah/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sabah/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.282807 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sarawak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sarawak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.312269 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_standard_lisan/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.360078 seacrowd-0.0.1/seacrowd/sea_datasets/memolon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/memolon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5545 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/memolon/memolon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.388325 seacrowd-0.0.1/seacrowd/sea_datasets/minangnlp_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/minangnlp_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.432762 seacrowd-0.0.1/seacrowd/sea_datasets/miracl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/miracl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13102 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/miracl/miracl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.451760 seacrowd-0.0.1/seacrowd/sea_datasets/mkqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mkqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mkqa/mkqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.480296 seacrowd-0.0.1/seacrowd/sea_datasets/mlqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mlqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9809 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mlqa/mlqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.514242 seacrowd-0.0.1/seacrowd/sea_datasets/mozilla_pontoon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.552188 seacrowd-0.0.1/seacrowd/sea_datasets/mswc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mswc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mswc/mswc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.594217 seacrowd-0.0.1/seacrowd/sea_datasets/mtop_intent_classification/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mtop_intent_classification/labels.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5622 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.640597 seacrowd-0.0.1/seacrowd/sea_datasets/multilexnorm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/multilexnorm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.670387 seacrowd-0.0.1/seacrowd/sea_datasets/my_paraphrase/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/my_paraphrase/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8184 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.689663 seacrowd-0.0.1/seacrowd/sea_datasets/myanmar_rakhine_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.714089 seacrowd-0.0.1/seacrowd/sea_datasets/mypos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mypos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mypos/mypos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.737695 seacrowd-0.0.1/seacrowd/sea_datasets/mysentence/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mysentence/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/mysentence/mysentence.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.756010 seacrowd-0.0.1/seacrowd/sea_datasets/myxnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/myxnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/myxnli/myxnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.774873 seacrowd-0.0.1/seacrowd/sea_datasets/nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nergrit/nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.812676 seacrowd-0.0.1/seacrowd/sea_datasets/nerp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nerp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nerp/nerp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.837181 seacrowd-0.0.1/seacrowd/sea_datasets/netifier/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/netifier/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/netifier/netifier.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.859408 seacrowd-0.0.1/seacrowd/sea_datasets/news_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/news_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/news_en_id/news_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.877744 seacrowd-0.0.1/seacrowd/sea_datasets/newsph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/newsph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/newsph/newsph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.895633 seacrowd-0.0.1/seacrowd/sea_datasets/nllb_seed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nllb_seed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.922150 seacrowd-0.0.1/seacrowd/sea_datasets/ntrex_128/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ntrex_128/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.949079 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.977091 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_rhetoric/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:58.998014 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_topic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.037235 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.058443 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.078304 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.106246 seacrowd-0.0.1/seacrowd/sea_datasets/nusax_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusax_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.134635 seacrowd-0.0.1/seacrowd/sea_datasets/nusax_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusax_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.155755 seacrowd-0.0.1/seacrowd/sea_datasets/oil/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/oil/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/oil/oil.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.176369 seacrowd-0.0.1/seacrowd/sea_datasets/ojw/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ojw/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ojw/ojw.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.196912 seacrowd-0.0.1/seacrowd/sea_datasets/openlid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/openlid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/openlid/openlid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.219384 seacrowd-0.0.1/seacrowd/sea_datasets/openslr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/openslr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/openslr/openslr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.254189 seacrowd-0.0.1/seacrowd/sea_datasets/orchid_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/orchid_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.274861 seacrowd-0.0.1/seacrowd/sea_datasets/oscar_2201/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/oscar_2201/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.292771 seacrowd-0.0.1/seacrowd/sea_datasets/palito/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/palito/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/palito/palito.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.328608 seacrowd-0.0.1/seacrowd/sea_datasets/paracotta_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/paracotta_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.348900 seacrowd-0.0.1/seacrowd/sea_datasets/parallel_id_nyo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.368025 seacrowd-0.0.1/seacrowd/sea_datasets/parallel_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/parallel_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.389927 seacrowd-0.0.1/seacrowd/sea_datasets/ph_fake_news_corpus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4311 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.422599 seacrowd-0.0.1/seacrowd/sea_datasets/pho_ner_covid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/pho_ner_covid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.1/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.454680 seacrowd-0.0.1/seacrowd/sea_datasets/phomt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/phomt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/phomt/phomt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.475359 seacrowd-0.0.1/seacrowd/sea_datasets/phost/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/phost/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/phost/phost.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.495525 seacrowd-0.0.1/seacrowd/sea_datasets/posp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/posp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/posp/posp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.518716 seacrowd-0.0.1/seacrowd/sea_datasets/postag_su/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/postag_su/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/postag_su/postag_su.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.544247 seacrowd-0.0.1/seacrowd/sea_datasets/prdect_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/prdect_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/prdect_id/prdect_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.564833 seacrowd-0.0.1/seacrowd/sea_datasets/qasina/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/qasina/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/qasina/qasina.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.584740 seacrowd-0.0.1/seacrowd/sea_datasets/roots_vi_ted/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/roots_vi_ted/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.603340 seacrowd-0.0.1/seacrowd/sea_datasets/sampiran/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sampiran/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sampiran/sampiran.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.625774 seacrowd-0.0.1/seacrowd/sea_datasets/sap_wat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sap_wat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7061 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sap_wat/sap_wat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.647469 seacrowd-0.0.1/seacrowd/sea_datasets/sarawak_malay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sarawak_malay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.668872 seacrowd-0.0.1/seacrowd/sea_datasets/scb_mt_en_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.686561 seacrowd-0.0.1/seacrowd/sea_datasets/sea_bench/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sea_bench/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sea_bench/sea_bench.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.707576 seacrowd-0.0.1/seacrowd/sea_datasets/sea_madlad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sea_madlad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.731584 seacrowd-0.0.1/seacrowd/sea_datasets/sea_wiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sea_wiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.751628 seacrowd-0.0.1/seacrowd/sea_datasets/seaeval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/seaeval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/seaeval/seaeval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.772292 seacrowd-0.0.1/seacrowd/sea_datasets/seahorse/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/seahorse/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/seahorse/seahorse.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.794366 seacrowd-0.0.1/seacrowd/sea_datasets/sentiment_nathasa_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.820845 seacrowd-0.0.1/seacrowd/sea_datasets/shopee_reviews_tagalog/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.850671 seacrowd-0.0.1/seacrowd/sea_datasets/singgalang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/singgalang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/singgalang/singgalang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.870777 seacrowd-0.0.1/seacrowd/sea_datasets/smsa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/smsa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/smsa/smsa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.911651 seacrowd-0.0.1/seacrowd/sea_datasets/snli_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/snli_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/snli_indo/snli_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.938806 seacrowd-0.0.1/seacrowd/sea_datasets/spamid_pair/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/spamid_pair/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.962635 seacrowd-0.0.1/seacrowd/sea_datasets/squad_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/squad_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/squad_id/squad_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:02:59.988170 seacrowd-0.0.1/seacrowd/sea_datasets/stb_ext/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/stb_ext/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/stb_ext/stb_ext.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.020813 seacrowd-0.0.1/seacrowd/sea_datasets/stif_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/stif_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.039312 seacrowd-0.0.1/seacrowd/sea_datasets/struct_amb_ind/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/struct_amb_ind/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.057278 seacrowd-0.0.1/seacrowd/sea_datasets/su_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/su_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/su_emot/su_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.075978 seacrowd-0.0.1/seacrowd/sea_datasets/su_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/su_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.094959 seacrowd-0.0.1/seacrowd/sea_datasets/su_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/su_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.115182 seacrowd-0.0.1/seacrowd/sea_datasets/talpco/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/talpco/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/talpco/talpco.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.136780 seacrowd-0.0.1/seacrowd/sea_datasets/tatabahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tatabahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.156105 seacrowd-0.0.1/seacrowd/sea_datasets/tatoeba/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tatoeba/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tatoeba/tatoeba.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.176616 seacrowd-0.0.1/seacrowd/sea_datasets/tcope/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tcope/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tcope/tcope.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.196976 seacrowd-0.0.1/seacrowd/sea_datasets/ted_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ted_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.228914 seacrowd-0.0.1/seacrowd/sea_datasets/term_a/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/term_a/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/term_a/term_a.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.248216 seacrowd-0.0.1/seacrowd/sea_datasets/tgl_profanity/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tgl_profanity/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.272861 seacrowd-0.0.1/seacrowd/sea_datasets/tha_lao_embassy_parcor/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.292923 seacrowd-0.0.1/seacrowd/sea_datasets/thai_alpaca/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_alpaca/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.311323 seacrowd-0.0.1/seacrowd/sea_datasets/thai_constitution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_constitution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.333344 seacrowd-0.0.1/seacrowd/sea_datasets/thai_databricks_dolly/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.351846 seacrowd-0.0.1/seacrowd/sea_datasets/thai_depression/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_depression/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_depression/thai_depression.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.369546 seacrowd-0.0.1/seacrowd/sea_datasets/thai_gpteacher/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_gpteacher/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.391512 seacrowd-0.0.1/seacrowd/sea_datasets/thai_hh_rlhf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.408848 seacrowd-0.0.1/seacrowd/sea_datasets/thai_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_sum/thai_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.438557 seacrowd-0.0.1/seacrowd/sea_datasets/thai_toxicity_tweet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.462386 seacrowd-0.0.1/seacrowd/sea_datasets/tico_19/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tico_19/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tico_19/tico_19.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.482589 seacrowd-0.0.1/seacrowd/sea_datasets/titml_idn/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/titml_idn/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/titml_idn/titml_idn.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.507682 seacrowd-0.0.1/seacrowd/sea_datasets/tlunified_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tlunified_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.528878 seacrowd-0.0.1/seacrowd/sea_datasets/toxicity_200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/toxicity_200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.552682 seacrowd-0.0.1/seacrowd/sea_datasets/tydiqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tydiqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23855 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/tydiqa/tydiqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.578162 seacrowd-0.0.1/seacrowd/sea_datasets/typhoon_yolanda_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.598314 seacrowd-0.0.1/seacrowd/sea_datasets/ucla_phonetic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ucla_phonetic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.624426 seacrowd-0.0.1/seacrowd/sea_datasets/ud_id_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ud_id_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.645496 seacrowd-0.0.1/seacrowd/sea_datasets/ud_jv_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ud_jv_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.665617 seacrowd-0.0.1/seacrowd/sea_datasets/udhr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/udhr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/udhr/udhr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.685785 seacrowd-0.0.1/seacrowd/sea_datasets/udhr_lid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/udhr_lid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.706147 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vicov19qa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.726574 seacrowd-0.0.1/seacrowd/sea_datasets/uit_victsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_victsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.744623 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vihsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vihsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.763819 seacrowd-0.0.1/seacrowd/sea_datasets/uit_viic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_viic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_viic/uit_viic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.783854 seacrowd-0.0.1/seacrowd/sea_datasets/uit_viocd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_viocd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.802926 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vion/uit_vion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.829270 seacrowd-0.0.1/seacrowd/sea_datasets/uit_visd4sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_visd4sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7018 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.857501 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsfc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsfc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.878449 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsmec/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsmec/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.897912 seacrowd-0.0.1/seacrowd/sea_datasets/unimorph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/unimorph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/unimorph/unimorph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.922085 seacrowd-0.0.1/seacrowd/sea_datasets/unimorph_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/unimorph_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.943159 seacrowd-0.0.1/seacrowd/sea_datasets/vi_pubmed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vi_pubmed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.962455 seacrowd-0.0.1/seacrowd/sea_datasets/vihealthqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vihealthqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.979400 seacrowd-0.0.1/seacrowd/sea_datasets/visobert/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/visobert/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/visobert/visobert.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:00.998565 seacrowd-0.0.1/seacrowd/sea_datasets/vispamreviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vispamreviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.019050 seacrowd-0.0.1/seacrowd/sea_datasets/vistec_tp_th_21/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.037261 seacrowd-0.0.1/seacrowd/sea_datasets/vitext2sql/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vitext2sql/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.065207 seacrowd-0.0.1/seacrowd/sea_datasets/vivos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vivos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vivos/vivos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.089928 seacrowd-0.0.1/seacrowd/sea_datasets/vivqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vivqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vivqa/vivqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.115353 seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.139083 seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.183246 seacrowd-0.0.1/seacrowd/sea_datasets/vndt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vndt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vndt/utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/vndt/vndt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.221349 seacrowd-0.0.1/seacrowd/sea_datasets/voxlingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/voxlingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/voxlingua/voxlingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.269537 seacrowd-0.0.1/seacrowd/sea_datasets/weathub/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/weathub/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/weathub/weathub.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.319488 seacrowd-0.0.1/seacrowd/sea_datasets/wikiann/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikiann/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikiann/wikiann.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.351435 seacrowd-0.0.1/seacrowd/sea_datasets/wikilingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikilingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikilingua/wikilingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.408349 seacrowd-0.0.1/seacrowd/sea_datasets/wikimatrix/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikimatrix/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.448286 seacrowd-0.0.1/seacrowd/sea_datasets/wikitext_tl_39/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.532182 seacrowd-0.0.1/seacrowd/sea_datasets/wili_2018/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wili_2018/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wili_2018/wili_2018.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.562536 seacrowd-0.0.1/seacrowd/sea_datasets/wisesight_thai_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.625214 seacrowd-0.0.1/seacrowd/sea_datasets/wit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wit/wit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.664349 seacrowd-0.0.1/seacrowd/sea_datasets/wongnai_reviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wongnai_reviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.715807 seacrowd-0.0.1/seacrowd/sea_datasets/wrete/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wrete/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/wrete/wrete.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.817766 seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.869404 seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/x_fact.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:01.971759 seacrowd-0.0.1/seacrowd/sea_datasets/xcopa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xcopa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xcopa/xcopa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.047742 seacrowd-0.0.1/seacrowd/sea_datasets/xl_jailbreak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xl_jailbreak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.116936 seacrowd-0.0.1/seacrowd/sea_datasets/xl_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xl_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xl_sum/xl_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.195197 seacrowd-0.0.1/seacrowd/sea_datasets/xm3600/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xm3600/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8217 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xm3600/xm3600.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.269255 seacrowd-0.0.1/seacrowd/sea_datasets/xnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xnli/xnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.322855 seacrowd-0.0.1/seacrowd/sea_datasets/xpersona_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xpersona_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.360414 seacrowd-0.0.1/seacrowd/sea_datasets/xquad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xquad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xquad/xquad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.385686 seacrowd-0.0.1/seacrowd/sea_datasets/xsid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xsid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xsid/xsid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.423311 seacrowd-0.0.1/seacrowd/sea_datasets/xstorycloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xstorycloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.451545 seacrowd-0.0.1/seacrowd/sea_datasets/yunshan_cup_2020/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.509600 seacrowd-0.0.1/seacrowd/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/common_parser.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/configs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/constants.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.847164 seacrowd-0.0.1/seacrowd/utils/schemas/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/image_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/imqa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/kb.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/pairs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/pairs_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/qa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/self_supervised_pretraining.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/seq_label.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/speech_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/speech_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/speech_to_speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/text_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/text_to_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/tod.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/tree.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.1/seacrowd/utils/schemas/video.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.915983 seacrowd-0.0.1/seacrowd.egg-info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-04 08:02:51.000000 seacrowd-0.0.1/seacrowd.egg-info/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31251 2024-04-04 08:02:52.000000 seacrowd-0.0.1/seacrowd.egg-info/SOURCES.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 08:02:51.000000 seacrowd-0.0.1/seacrowd.egg-info/dependency_links.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-04 08:02:51.000000 seacrowd-0.0.1/seacrowd.egg-info/requires.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-04 08:02:51.000000 seacrowd-0.0.1/seacrowd.egg-info/top_level.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      666 2024-04-04 08:03:02.947620 seacrowd-0.0.1/setup.cfg
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-04 06:00:52.000000 seacrowd-0.0.1/setup.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 08:03:02.890336 seacrowd-0.0.1/tests/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.1/tests/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.1/tests/test_seacrowd.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.1/tests/test_seacrowd_source_only.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.962531 seacrowd-0.0.2/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.2/LICENSE
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-06 05:07:40.958015 seacrowd-0.0.2/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.2/README.md
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.103721 seacrowd-0.0.2/seacrowd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       58 2024-04-06 05:03:12.000000 seacrowd-0.0.2/seacrowd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-04 14:04:10.000000 seacrowd-0.0.2/seacrowd/config_helper.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.192981 seacrowd-0.0.2/seacrowd/sea_datasets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.219051 seacrowd-0.0.2/seacrowd/sea_datasets/abui_wordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/abui_wordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.240911 seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.267536 seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.294487 seacrowd-0.0.2/seacrowd/sea_datasets/ara_close/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ara_close/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ara_close/ara_close.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.316531 seacrowd-0.0.2/seacrowd/sea_datasets/asr_sindodusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/asr_sindodusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.346063 seacrowd-0.0.2/seacrowd/sea_datasets/asr_smaldusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/asr_smaldusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.373031 seacrowd-0.0.2/seacrowd/sea_datasets/asr_stidusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/asr_stidusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.394778 seacrowd-0.0.2/seacrowd/sea_datasets/audio_keyword_spotting/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.424540 seacrowd-0.0.2/seacrowd/sea_datasets/aya_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/aya_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.449233 seacrowd-0.0.2/seacrowd/sea_datasets/barasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/barasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/barasa/barasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.475561 seacrowd-0.0.2/seacrowd/sea_datasets/beaye_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/beaye_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.502969 seacrowd-0.0.2/seacrowd/sea_datasets/belebele/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/belebele/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-04 09:36:40.000000 seacrowd-0.0.2/seacrowd/sea_datasets/belebele/belebele.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.525890 seacrowd-0.0.2/seacrowd/sea_datasets/bible_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bible_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.556581 seacrowd-0.0.2/seacrowd/sea_datasets/bible_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bible_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.582471 seacrowd-0.0.2/seacrowd/sea_datasets/bible_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bible_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.606265 seacrowd-0.0.2/seacrowd/sea_datasets/bioner_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bioner_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bioner_id/bioner_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.630241 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_captioning/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_captioning/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.653928 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_lm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_lm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.681771 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_speech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_speech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.705767 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_vist/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_vist/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.739122 seacrowd-0.0.2/seacrowd/sea_datasets/burapha_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/burapha_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/burapha_th/burapha_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.761890 seacrowd-0.0.2/seacrowd/sea_datasets/burmese_romanize/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/burmese_romanize/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-04 09:37:19.000000 seacrowd-0.0.2/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.781070 seacrowd-0.0.2/seacrowd/sea_datasets/casa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/casa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/casa/casa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.803653 seacrowd-0.0.2/seacrowd/sea_datasets/cc100/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cc100/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cc100/cc100.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.832621 seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_doc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.866944 seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_sent/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.893607 seacrowd-0.0.2/seacrowd/sea_datasets/cebuaner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cebuaner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cebuaner/cebuaner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.926926 seacrowd-0.0.2/seacrowd/sea_datasets/coco_35l/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/coco_35l/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-04 09:37:44.000000 seacrowd-0.0.2/seacrowd/sea_datasets/coco_35l/coco_35l.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.952984 seacrowd-0.0.2/seacrowd/sea_datasets/cod/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cod/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cod/cod.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.973621 seacrowd-0.0.2/seacrowd/sea_datasets/code_mixed_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:32.995289 seacrowd-0.0.2/seacrowd/sea_datasets/codeswitch_reddit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.026071 seacrowd-0.0.2/seacrowd/sea_datasets/commonvoice_120/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/commonvoice_120/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.059337 seacrowd-0.0.2/seacrowd/sea_datasets/copal/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/copal/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/copal/copal.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.091085 seacrowd-0.0.2/seacrowd/sea_datasets/covost2/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/covost2/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/covost2/covost2.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.140318 seacrowd-0.0.2/seacrowd/sea_datasets/creole_rc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.2/seacrowd/sea_datasets/creole_rc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/creole_rc/creole_rc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.174560 seacrowd-0.0.2/seacrowd/sea_datasets/crosssum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/crosssum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/crosssum/crosssum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.212524 seacrowd-0.0.2/seacrowd/sea_datasets/cub_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cub_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.254944 seacrowd-0.0.2/seacrowd/sea_datasets/culturax/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/culturax/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/culturax/culturax.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.288981 seacrowd-0.0.2/seacrowd/sea_datasets/cvss/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cvss/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/cvss/cvss.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.322670 seacrowd-0.0.2/seacrowd/sea_datasets/dengue_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/dengue_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-04 09:38:19.000000 seacrowd-0.0.2/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.356710 seacrowd-0.0.2/seacrowd/sea_datasets/emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emot/emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.388142 seacrowd-0.0.2/seacrowd/sea_datasets/emotcmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emotcmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emotcmt/emotcmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.414976 seacrowd-0.0.2/seacrowd/sea_datasets/emotes_3k/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emotes_3k/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.447222 seacrowd-0.0.2/seacrowd/sea_datasets/emotion_id_opinion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.475961 seacrowd-0.0.2/seacrowd/sea_datasets/etos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/etos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/etos/etos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.503269 seacrowd-0.0.2/seacrowd/sea_datasets/facqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/facqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/facqa/facqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.535424 seacrowd-0.0.2/seacrowd/sea_datasets/facqa/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/facqa/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.563217 seacrowd-0.0.2/seacrowd/sea_datasets/fakenews_ph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/fakenews_ph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.590434 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_gay_lang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.621091 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.647588 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_slang_norm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.676543 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_words_aoa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.706627 seacrowd-0.0.2/seacrowd/sea_datasets/filwordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filwordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/filwordnet/filwordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.739412 seacrowd-0.0.2/seacrowd/sea_datasets/fleurs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/fleurs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13189 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/fleurs/fleurs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.767404 seacrowd-0.0.2/seacrowd/sea_datasets/flores200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/flores200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/flores200/flores200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.789922 seacrowd-0.0.2/seacrowd/sea_datasets/fsl_105/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/fsl_105/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6753 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/fsl_105/fsl_105.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.812711 seacrowd-0.0.2/seacrowd/sea_datasets/gatitos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/gatitos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/gatitos/gatitos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.851977 seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_newsclass/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.876145 seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.898546 seacrowd-0.0.2/seacrowd/sea_datasets/globalwoz/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/globalwoz/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/globalwoz/globalwoz.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.926295 seacrowd-0.0.2/seacrowd/sea_datasets/glotstorybook/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/glotstorybook/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.951104 seacrowd-0.0.2/seacrowd/sea_datasets/hoasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/hoasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/hoasa/hoasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.973400 seacrowd-0.0.2/seacrowd/sea_datasets/iapp_squad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/iapp_squad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:33.994771 seacrowd-0.0.2/seacrowd/sea_datasets/iatf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/iatf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/iatf/iatf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.019442 seacrowd-0.0.2/seacrowd/sea_datasets/icon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/icon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/icon/icon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.048303 seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive/id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.079931 seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive_news_comment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.105075 seacrowd-0.0.2/seacrowd/sea_datasets/id_am2ico/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_am2ico/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.138007 seacrowd-0.0.2/seacrowd/sea_datasets/id_clickbait/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_clickbait/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.166694 seacrowd-0.0.2/seacrowd/sea_datasets/id_coreference_resolution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.189515 seacrowd-0.0.2/seacrowd/sea_datasets/id_frog_story/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_frog_story/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.209238 seacrowd-0.0.2/seacrowd/sea_datasets/id_google_play_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_google_play_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.232381 seacrowd-0.0.2/seacrowd/sea_datasets/id_hatespeech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_hatespeech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.253583 seacrowd-0.0.2/seacrowd/sea_datasets/id_hoax_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_hoax_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.276952 seacrowd-0.0.2/seacrowd/sea_datasets/id_hsd_nofaaulia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.299701 seacrowd-0.0.2/seacrowd/sea_datasets/id_msvd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_msvd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-04 09:39:30.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_msvd/id_msvd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.324874 seacrowd-0.0.2/seacrowd/sea_datasets/id_multilabel_hs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.349011 seacrowd-0.0.2/seacrowd/sea_datasets/id_panl_bppt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_panl_bppt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.372928 seacrowd-0.0.2/seacrowd/sea_datasets/id_qqp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_qqp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_qqp/id_qqp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.394799 seacrowd-0.0.2/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.419319 seacrowd-0.0.2/seacrowd/sea_datasets/id_sentiment_analysis/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.443285 seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.472869 seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.494640 seacrowd-0.0.2/seacrowd/sea_datasets/id_stance/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_stance/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_stance/id_stance.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.516585 seacrowd-0.0.2/seacrowd/sea_datasets/id_sts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_sts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_sts/id_sts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.543012 seacrowd-0.0.2/seacrowd/sea_datasets/id_vaccines_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.565811 seacrowd-0.0.2/seacrowd/sea_datasets/id_wiki_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.589242 seacrowd-0.0.2/seacrowd/sea_datasets/id_wsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_wsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/id_wsd/id_wsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.612780 seacrowd-0.0.2/seacrowd/sea_datasets/identic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/identic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/identic/identic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.641774 seacrowd-0.0.2/seacrowd/sea_datasets/identifikasi_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.665407 seacrowd-0.0.2/seacrowd/sea_datasets/idk_mrc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/idk_mrc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.688669 seacrowd-0.0.2/seacrowd/sea_datasets/idn_tagged_corpus_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.709289 seacrowd-0.0.2/seacrowd/sea_datasets/ijelid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ijelid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ijelid/ijelid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.734451 seacrowd-0.0.2/seacrowd/sea_datasets/imdb_jv/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/imdb_jv/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.759152 seacrowd-0.0.2/seacrowd/sea_datasets/indo4b/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo4b/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo4b/indo4b.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.785625 seacrowd-0.0.2/seacrowd/sea_datasets/indo4b_plus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo4b_plus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.813502 seacrowd-0.0.2/seacrowd/sea_datasets/indo_general_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.844179 seacrowd-0.0.2/seacrowd/sea_datasets/indo_law/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_law/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_law/indo_law.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.865473 seacrowd-0.0.2/seacrowd/sea_datasets/indo_puisi/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_puisi/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.887519 seacrowd-0.0.2/seacrowd/sea_datasets/indo_religious_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.915465 seacrowd-0.0.2/seacrowd/sea_datasets/indo_story_cloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_story_cloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.943477 seacrowd-0.0.2/seacrowd/sea_datasets/indocamrest/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocamrest/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocamrest/indocamrest.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.966307 seacrowd-0.0.2/seacrowd/sea_datasets/indocollex/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocollex/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocollex/indocollex.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:34.993021 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/indocoref.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.042549 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/file_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.073712 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ner_ugm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.096116 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_nerui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_nerui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.118073 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ntp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ntp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.140533 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.175130 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_tweet_ordering/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.197261 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_gsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.219666 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_pud/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.251855 seacrowd-0.0.2/seacrowd/sea_datasets/indoler/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indoler/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indoler/indoler.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.279550 seacrowd-0.0.2/seacrowd/sea_datasets/indommlu/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indommlu/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-04 09:44:25.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indommlu/indommlu.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.307778 seacrowd-0.0.2/seacrowd/sea_datasets/indoner_tourism/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indoner_tourism/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.347239 seacrowd-0.0.2/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.377567 seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.400330 seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_news_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-04 09:51:18.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.422520 seacrowd-0.0.2/seacrowd/sea_datasets/indonesiannmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesiannmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.454650 seacrowd-0.0.2/seacrowd/sea_datasets/indonglish/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonglish/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonglish/indonglish.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.487530 seacrowd-0.0.2/seacrowd/sea_datasets/indonli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonli/indonli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.510716 seacrowd-0.0.2/seacrowd/sea_datasets/indonlu_nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.535920 seacrowd-0.0.2/seacrowd/sea_datasets/indoqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indoqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indoqa/indoqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.564299 seacrowd-0.0.2/seacrowd/sea_datasets/indosmd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indosmd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indosmd/indosmd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.589868 seacrowd-0.0.2/seacrowd/sea_datasets/indosum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indosum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indosum/indosum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.611605 seacrowd-0.0.2/seacrowd/sea_datasets/indotacos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indotacos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indotacos/indotacos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.633358 seacrowd-0.0.2/seacrowd/sea_datasets/indowiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indowiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indowiki/indowiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.661842 seacrowd-0.0.2/seacrowd/sea_datasets/indqner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indqner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indqner/indqner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.718196 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_digit_cdsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.752405 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.796352 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.834077 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.862751 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.886147 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.912684 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.950720 seacrowd-0.0.2/seacrowd/sea_datasets/inset_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/inset_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:35.977439 seacrowd-0.0.2/seacrowd/sea_datasets/jadi_ide/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/jadi_ide/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.002358 seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.024547 seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.048310 seacrowd-0.0.2/seacrowd/sea_datasets/kamus_alay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kamus_alay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.079956 seacrowd-0.0.2/seacrowd/sea_datasets/karonese_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/karonese_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.100305 seacrowd-0.0.2/seacrowd/sea_datasets/kawat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kawat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kawat/kawat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.121186 seacrowd-0.0.2/seacrowd/sea_datasets/kde4/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kde4/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kde4/kde4.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.142526 seacrowd-0.0.2/seacrowd/sea_datasets/keps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/keps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/keps/keps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.172326 seacrowd-0.0.2/seacrowd/sea_datasets/kheng_info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kheng_info/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kheng_info/kheng_info.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.195704 seacrowd-0.0.2/seacrowd/sea_datasets/khmer_alt_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.218217 seacrowd-0.0.2/seacrowd/sea_datasets/khpos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/khpos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/khpos/khpos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.240761 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.263532 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.284333 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_nllb/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_nllb/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.320579 seacrowd-0.0.2/seacrowd/sea_datasets/korpus_nusantara/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/korpus_nusantara/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.344660 seacrowd-0.0.2/seacrowd/sea_datasets/lazada_review_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.366862 seacrowd-0.0.2/seacrowd/sea_datasets/librivox_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/librivox_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.390709 seacrowd-0.0.2/seacrowd/sea_datasets/limesoda/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/limesoda/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/limesoda/limesoda.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.413251 seacrowd-0.0.2/seacrowd/sea_datasets/liputan6/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/liputan6/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/liputan6/liputan6.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.436018 seacrowd-0.0.2/seacrowd/sea_datasets/local_id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/local_id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.463301 seacrowd-0.0.2/seacrowd/sea_datasets/lr_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/lr_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/lr_sum/lr_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.490934 seacrowd-0.0.2/seacrowd/sea_datasets/m3exam/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/m3exam/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/m3exam/m3exam.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.514642 seacrowd-0.0.2/seacrowd/sea_datasets/mabl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mabl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mabl/mabl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.537666 seacrowd-0.0.2/seacrowd/sea_datasets/malaysia_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/malaysia_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.564544 seacrowd-0.0.2/seacrowd/sea_datasets/malindo_morph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/malindo_morph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.595045 seacrowd-0.0.2/seacrowd/sea_datasets/malindo_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/malindo_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.620391 seacrowd-0.0.2/seacrowd/sea_datasets/massive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/massive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.2/seacrowd/sea_datasets/massive/massive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.642803 seacrowd-0.0.2/seacrowd/sea_datasets/mc4_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mc4_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-04 09:54:18.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.673685 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_brunei/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_brunei/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.697056 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sabah/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sabah/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.718980 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sarawak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sarawak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.750759 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_standard_lisan/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.772805 seacrowd-0.0.2/seacrowd/sea_datasets/memolon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/memolon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-04 09:56:41.000000 seacrowd-0.0.2/seacrowd/sea_datasets/memolon/memolon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.792621 seacrowd-0.0.2/seacrowd/sea_datasets/minangnlp_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/minangnlp_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.814691 seacrowd-0.0.2/seacrowd/sea_datasets/miracl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/miracl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-04 09:57:37.000000 seacrowd-0.0.2/seacrowd/sea_datasets/miracl/miracl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.835409 seacrowd-0.0.2/seacrowd/sea_datasets/mkqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mkqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mkqa/mkqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.862165 seacrowd-0.0.2/seacrowd/sea_datasets/mlqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mlqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-04 09:58:31.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mlqa/mlqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.883785 seacrowd-0.0.2/seacrowd/sea_datasets/mozilla_pontoon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.907717 seacrowd-0.0.2/seacrowd/sea_datasets/mswc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mswc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mswc/mswc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.945178 seacrowd-0.0.2/seacrowd/sea_datasets/mtop_intent_classification/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mtop_intent_classification/labels.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-04 10:05:24.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.975311 seacrowd-0.0.2/seacrowd/sea_datasets/multilexnorm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/multilexnorm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:36.995630 seacrowd-0.0.2/seacrowd/sea_datasets/my_paraphrase/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/my_paraphrase/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-04 10:20:55.000000 seacrowd-0.0.2/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.017041 seacrowd-0.0.2/seacrowd/sea_datasets/myanmar_rakhine_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.041308 seacrowd-0.0.2/seacrowd/sea_datasets/mypos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mypos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mypos/mypos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.064019 seacrowd-0.0.2/seacrowd/sea_datasets/mysentence/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mysentence/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/mysentence/mysentence.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.090341 seacrowd-0.0.2/seacrowd/sea_datasets/myxnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/myxnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/myxnli/myxnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.113711 seacrowd-0.0.2/seacrowd/sea_datasets/nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nergrit/nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.141011 seacrowd-0.0.2/seacrowd/sea_datasets/nerp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nerp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nerp/nerp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.168852 seacrowd-0.0.2/seacrowd/sea_datasets/netifier/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/netifier/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/netifier/netifier.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.202428 seacrowd-0.0.2/seacrowd/sea_datasets/news_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/news_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/news_en_id/news_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.223545 seacrowd-0.0.2/seacrowd/sea_datasets/newsph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/newsph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/newsph/newsph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.251434 seacrowd-0.0.2/seacrowd/sea_datasets/nllb_seed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nllb_seed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.275443 seacrowd-0.0.2/seacrowd/sea_datasets/ntrex_128/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ntrex_128/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.301843 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.327690 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_rhetoric/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.350556 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_topic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.384569 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.413818 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.442210 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.465762 seacrowd-0.0.2/seacrowd/sea_datasets/nusax_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusax_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.488904 seacrowd-0.0.2/seacrowd/sea_datasets/nusax_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusax_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.511957 seacrowd-0.0.2/seacrowd/sea_datasets/oil/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/oil/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/oil/oil.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.534615 seacrowd-0.0.2/seacrowd/sea_datasets/ojw/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ojw/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ojw/ojw.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.558355 seacrowd-0.0.2/seacrowd/sea_datasets/openlid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/openlid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/openlid/openlid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.580807 seacrowd-0.0.2/seacrowd/sea_datasets/openslr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/openslr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/openslr/openslr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.603626 seacrowd-0.0.2/seacrowd/sea_datasets/orchid_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/orchid_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.633901 seacrowd-0.0.2/seacrowd/sea_datasets/oscar_2201/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/oscar_2201/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.658667 seacrowd-0.0.2/seacrowd/sea_datasets/palito/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/palito/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/palito/palito.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.685310 seacrowd-0.0.2/seacrowd/sea_datasets/paracotta_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/paracotta_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.707530 seacrowd-0.0.2/seacrowd/sea_datasets/parallel_id_nyo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.752677 seacrowd-0.0.2/seacrowd/sea_datasets/parallel_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/parallel_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.774557 seacrowd-0.0.2/seacrowd/sea_datasets/ph_fake_news_corpus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-04 10:21:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.796223 seacrowd-0.0.2/seacrowd/sea_datasets/pho_ner_covid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/pho_ner_covid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.2/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.825955 seacrowd-0.0.2/seacrowd/sea_datasets/phomt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/phomt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/phomt/phomt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.849596 seacrowd-0.0.2/seacrowd/sea_datasets/phost/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/phost/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/phost/phost.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.875467 seacrowd-0.0.2/seacrowd/sea_datasets/posp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/posp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/posp/posp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.898055 seacrowd-0.0.2/seacrowd/sea_datasets/postag_su/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/postag_su/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/postag_su/postag_su.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.921152 seacrowd-0.0.2/seacrowd/sea_datasets/prdect_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/prdect_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/prdect_id/prdect_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.942481 seacrowd-0.0.2/seacrowd/sea_datasets/qasina/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/qasina/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/qasina/qasina.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.970233 seacrowd-0.0.2/seacrowd/sea_datasets/roots_vi_ted/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/roots_vi_ted/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:37.992376 seacrowd-0.0.2/seacrowd/sea_datasets/sampiran/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sampiran/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sampiran/sampiran.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.018399 seacrowd-0.0.2/seacrowd/sea_datasets/sap_wat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sap_wat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-04 10:22:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sap_wat/sap_wat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.054935 seacrowd-0.0.2/seacrowd/sea_datasets/sarawak_malay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sarawak_malay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.081763 seacrowd-0.0.2/seacrowd/sea_datasets/scb_mt_en_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.119507 seacrowd-0.0.2/seacrowd/sea_datasets/sea_bench/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sea_bench/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sea_bench/sea_bench.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.149331 seacrowd-0.0.2/seacrowd/sea_datasets/sea_madlad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sea_madlad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.186473 seacrowd-0.0.2/seacrowd/sea_datasets/sea_wiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sea_wiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.214202 seacrowd-0.0.2/seacrowd/sea_datasets/seaeval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/seaeval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/seaeval/seaeval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.245627 seacrowd-0.0.2/seacrowd/sea_datasets/seahorse/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/seahorse/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/seahorse/seahorse.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.298627 seacrowd-0.0.2/seacrowd/sea_datasets/sentiment_nathasa_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.336240 seacrowd-0.0.2/seacrowd/sea_datasets/shopee_reviews_tagalog/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.363060 seacrowd-0.0.2/seacrowd/sea_datasets/singgalang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/singgalang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/singgalang/singgalang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.384404 seacrowd-0.0.2/seacrowd/sea_datasets/smsa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/smsa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/smsa/smsa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.409155 seacrowd-0.0.2/seacrowd/sea_datasets/snli_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/snli_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/snli_indo/snli_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.438976 seacrowd-0.0.2/seacrowd/sea_datasets/spamid_pair/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/spamid_pair/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.468049 seacrowd-0.0.2/seacrowd/sea_datasets/squad_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/squad_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/squad_id/squad_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.500906 seacrowd-0.0.2/seacrowd/sea_datasets/stb_ext/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/stb_ext/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/stb_ext/stb_ext.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.530113 seacrowd-0.0.2/seacrowd/sea_datasets/stif_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/stif_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.560850 seacrowd-0.0.2/seacrowd/sea_datasets/struct_amb_ind/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/struct_amb_ind/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.585378 seacrowd-0.0.2/seacrowd/sea_datasets/su_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/su_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/su_emot/su_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.617750 seacrowd-0.0.2/seacrowd/sea_datasets/su_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/su_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.644823 seacrowd-0.0.2/seacrowd/sea_datasets/su_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/su_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.683417 seacrowd-0.0.2/seacrowd/sea_datasets/talpco/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/talpco/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/talpco/talpco.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.706463 seacrowd-0.0.2/seacrowd/sea_datasets/tatabahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tatabahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.732089 seacrowd-0.0.2/seacrowd/sea_datasets/tatoeba/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tatoeba/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tatoeba/tatoeba.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.757078 seacrowd-0.0.2/seacrowd/sea_datasets/tcope/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tcope/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tcope/tcope.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.777798 seacrowd-0.0.2/seacrowd/sea_datasets/ted_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ted_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.800390 seacrowd-0.0.2/seacrowd/sea_datasets/term_a/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/term_a/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/term_a/term_a.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.823535 seacrowd-0.0.2/seacrowd/sea_datasets/tgl_profanity/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tgl_profanity/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.847761 seacrowd-0.0.2/seacrowd/sea_datasets/tha_lao_embassy_parcor/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.881696 seacrowd-0.0.2/seacrowd/sea_datasets/thai_alpaca/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_alpaca/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.909890 seacrowd-0.0.2/seacrowd/sea_datasets/thai_constitution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_constitution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.936052 seacrowd-0.0.2/seacrowd/sea_datasets/thai_databricks_dolly/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:38.959196 seacrowd-0.0.2/seacrowd/sea_datasets/thai_depression/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_depression/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_depression/thai_depression.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.004980 seacrowd-0.0.2/seacrowd/sea_datasets/thai_gpteacher/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_gpteacher/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.040243 seacrowd-0.0.2/seacrowd/sea_datasets/thai_hh_rlhf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.062829 seacrowd-0.0.2/seacrowd/sea_datasets/thai_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_sum/thai_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.085999 seacrowd-0.0.2/seacrowd/sea_datasets/thai_toxicity_tweet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.110271 seacrowd-0.0.2/seacrowd/sea_datasets/tico_19/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tico_19/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tico_19/tico_19.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.147761 seacrowd-0.0.2/seacrowd/sea_datasets/titml_idn/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/titml_idn/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/titml_idn/titml_idn.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.202973 seacrowd-0.0.2/seacrowd/sea_datasets/tlunified_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tlunified_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.230781 seacrowd-0.0.2/seacrowd/sea_datasets/toxicity_200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/toxicity_200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.259963 seacrowd-0.0.2/seacrowd/sea_datasets/tydiqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tydiqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-04 10:25:46.000000 seacrowd-0.0.2/seacrowd/sea_datasets/tydiqa/tydiqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.290234 seacrowd-0.0.2/seacrowd/sea_datasets/typhoon_yolanda_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.313258 seacrowd-0.0.2/seacrowd/sea_datasets/ucla_phonetic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ucla_phonetic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.335784 seacrowd-0.0.2/seacrowd/sea_datasets/ud_id_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ud_id_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.363752 seacrowd-0.0.2/seacrowd/sea_datasets/ud_jv_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ud_jv_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.390393 seacrowd-0.0.2/seacrowd/sea_datasets/udhr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/udhr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/udhr/udhr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.413571 seacrowd-0.0.2/seacrowd/sea_datasets/udhr_lid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/udhr_lid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.436785 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vicov19qa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.474098 seacrowd-0.0.2/seacrowd/sea_datasets/uit_victsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_victsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.496062 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vihsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vihsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.525137 seacrowd-0.0.2/seacrowd/sea_datasets/uit_viic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_viic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_viic/uit_viic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.549692 seacrowd-0.0.2/seacrowd/sea_datasets/uit_viocd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_viocd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.576223 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vion/uit_vion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.598019 seacrowd-0.0.2/seacrowd/sea_datasets/uit_visd4sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_visd4sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-04 10:27:09.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.634870 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsfc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsfc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.660931 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsmec/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsmec/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.682709 seacrowd-0.0.2/seacrowd/sea_datasets/unimorph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/unimorph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/unimorph/unimorph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.709779 seacrowd-0.0.2/seacrowd/sea_datasets/unimorph_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/unimorph_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.740141 seacrowd-0.0.2/seacrowd/sea_datasets/vi_pubmed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vi_pubmed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.764598 seacrowd-0.0.2/seacrowd/sea_datasets/vihealthqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vihealthqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.794136 seacrowd-0.0.2/seacrowd/sea_datasets/visobert/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/visobert/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/visobert/visobert.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.815354 seacrowd-0.0.2/seacrowd/sea_datasets/vispamreviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vispamreviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.837497 seacrowd-0.0.2/seacrowd/sea_datasets/vistec_tp_th_21/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.871281 seacrowd-0.0.2/seacrowd/sea_datasets/vitext2sql/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vitext2sql/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.893784 seacrowd-0.0.2/seacrowd/sea_datasets/vivos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vivos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vivos/vivos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.917116 seacrowd-0.0.2/seacrowd/sea_datasets/vivqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vivqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vivqa/vivqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.937289 seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.960665 seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:39.994943 seacrowd-0.0.2/seacrowd/sea_datasets/vndt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vndt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vndt/utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/vndt/vndt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.021098 seacrowd-0.0.2/seacrowd/sea_datasets/voxlingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/voxlingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/voxlingua/voxlingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.044125 seacrowd-0.0.2/seacrowd/sea_datasets/weathub/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/weathub/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/weathub/weathub.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.066950 seacrowd-0.0.2/seacrowd/sea_datasets/wikiann/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikiann/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikiann/wikiann.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.090136 seacrowd-0.0.2/seacrowd/sea_datasets/wikilingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikilingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikilingua/wikilingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.116641 seacrowd-0.0.2/seacrowd/sea_datasets/wikimatrix/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikimatrix/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.137120 seacrowd-0.0.2/seacrowd/sea_datasets/wikitext_tl_39/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.165316 seacrowd-0.0.2/seacrowd/sea_datasets/wili_2018/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wili_2018/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wili_2018/wili_2018.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.197048 seacrowd-0.0.2/seacrowd/sea_datasets/wisesight_thai_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.218685 seacrowd-0.0.2/seacrowd/sea_datasets/wit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wit/wit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.242721 seacrowd-0.0.2/seacrowd/sea_datasets/wongnai_reviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wongnai_reviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.271693 seacrowd-0.0.2/seacrowd/sea_datasets/wrete/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wrete/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/wrete/wrete.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.297855 seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.324774 seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/x_fact.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.348824 seacrowd-0.0.2/seacrowd/sea_datasets/xcopa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xcopa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xcopa/xcopa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.374379 seacrowd-0.0.2/seacrowd/sea_datasets/xl_jailbreak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xl_jailbreak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.397597 seacrowd-0.0.2/seacrowd/sea_datasets/xl_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xl_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xl_sum/xl_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.420732 seacrowd-0.0.2/seacrowd/sea_datasets/xm3600/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xm3600/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 10:28:01.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xm3600/xm3600.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.442869 seacrowd-0.0.2/seacrowd/sea_datasets/xnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xnli/xnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.490824 seacrowd-0.0.2/seacrowd/sea_datasets/xpersona_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xpersona_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.514428 seacrowd-0.0.2/seacrowd/sea_datasets/xquad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xquad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xquad/xquad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.536596 seacrowd-0.0.2/seacrowd/sea_datasets/xsid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xsid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xsid/xsid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.560612 seacrowd-0.0.2/seacrowd/sea_datasets/xstorycloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xstorycloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.583076 seacrowd-0.0.2/seacrowd/sea_datasets/yunshan_cup_2020/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.641775 seacrowd-0.0.2/seacrowd/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/common_parser.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/configs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/constants.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.889725 seacrowd-0.0.2/seacrowd/utils/schemas/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/image_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/imqa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/kb.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/pairs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/pairs_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/qa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/self_supervised_pretraining.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/seq_label.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/speech_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/speech_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/speech_to_speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/text_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/text_to_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/tod.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/tree.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.2/seacrowd/utils/schemas/video.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.941498 seacrowd-0.0.2/seacrowd.egg-info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-06 05:07:29.000000 seacrowd-0.0.2/seacrowd.egg-info/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31277 2024-04-06 05:07:30.000000 seacrowd-0.0.2/seacrowd.egg-info/SOURCES.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-06 05:07:29.000000 seacrowd-0.0.2/seacrowd.egg-info/dependency_links.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-06 05:07:29.000000 seacrowd-0.0.2/seacrowd.egg-info/requires.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-06 05:07:29.000000 seacrowd-0.0.2/seacrowd.egg-info/top_level.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      666 2024-04-06 05:07:40.974003 seacrowd-0.0.2/setup.cfg
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-04 06:00:52.000000 seacrowd-0.0.2/setup.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-06 05:07:40.925925 seacrowd-0.0.2/tests/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.2/tests/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.2/tests/test_seacrowd.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.2/tests/test_seacrowd_source_only.py
```

### Comparing `seacrowd-0.0.1/LICENSE` & `seacrowd-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/PKG-INFO` & `seacrowd-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.1
+Version: 0.0.2
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.1/README.md` & `seacrowd-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ara_close/ara_close.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ara_close/ara_close.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/aya_dataset/aya_dataset.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/aya_dataset/aya_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/barasa/barasa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/barasa/barasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/belebele/belebele.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/belebele/belebele.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 _SEACROWD_VERSION = "1.0.0"
 
 _SOURCE_NAMES = ["ceb_Latn", "ilo_Latn", "ind_Latn", "jav_Latn", "kac_Latn", "khm_Khmr", "lao_Laoo", "mya_Mymr", "shn_Mymr", "sun_Latn", "tgl_Latn", "tha_Thai", "vie_Latn", "war_Latn", "zsm_Latn"]
 _LANGUAGES = [source.split("_")[0] for source in _SOURCE_NAMES]
 
 _DEFAULT_LANG = "zsm"
 
+_LOCAL = False
+
 def config_constructor(belebele_subset: str, schema: str, version: str) -> SEACrowdConfig:
     lang = _LANGUAGES[_SOURCE_NAMES.index(belebele_subset)]
     return SEACrowdConfig(
         name="belebele_{belebele_subset}_{schema}".format(belebele_subset=belebele_subset.lower(), schema=schema),
         version=version,
         description="belebele {lang} {schema} schema".format(lang=lang, schema=schema),
         schema=schema,
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bible_en_id/bible_en_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bible_en_id/bible_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bible_su_id/bible_su_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bible_su_id/bible_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bioner_id/bioner_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bioner_id/bioner_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bloom_lm/bloom_lm.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bloom_lm/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bloom_speech/bloom_speech.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bloom_speech/bloom_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/bloom_vist/bloom_vist.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/bloom_vist/bloom_vist.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/burapha_th/burapha_th.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/burapha_th/burapha_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 _LICENSE = Licenses.CC_BY_NC_SA_4_0.value
 _URLS = "http://www.nlpresearch-ucsy.edu.mm/NLP_UCSY/myanmaroma.zip"
 
 _SUPPORTED_TASKS = [Tasks.TRANSLITERATION]
 _SOURCE_VERSION = "1.0.0"
 _SEACROWD_VERSION = "1.0.0"
 
+_LOCAL = False
+
 
 class BurmeseRomanizeDataset(datasets.GeneratorBasedBuilder):
     """Romanization of names in Burmese script"""
 
     SOURCE_VERSION = datasets.Version(_SOURCE_VERSION)
     SEACROWD_VERSION = datasets.Version(_SEACROWD_VERSION)
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/casa/casa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/casa/casa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cc100/cc100.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cebuaner/cebuaner.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cebuaner/cebuaner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/coco_35l/coco_35l.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/coco_35l/coco_35l.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
 _SOURCE_VERSION = "1.0.0"
 
 _SEACROWD_VERSION = "1.0.0"
 
 _LANGUAGES = {"fil": "fil", "ind": "id", "tha": "th", "vie": "vi"}
 
+_LOCAL = False
+
 class Coco35LDataset(datasets.GeneratorBasedBuilder):
     """
     COCO-35L is a machine-generated image caption dataset, constructed by translating COCO Captions (Chen et al., 2015) to the other 34 languages using Google’s machine translation API.
     """
 
     SOURCE_VERSION = datasets.Version(_SOURCE_VERSION)
     SEACROWD_VERSION = datasets.Version(_SEACROWD_VERSION)
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cod/cod.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cod/cod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/copal/copal.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/copal/copal.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/covost2/covost2.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/covost2/covost2.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/creole_rc/creole_rc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/creole_rc/creole_rc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/crosssum/crosssum.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/crosssum/crosssum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/culturax/culturax.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/culturax/culturax.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/cvss/cvss.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/cvss/cvss.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 _LICENSE = Licenses.UNKNOWN.value
 
 _SUPPORTED_TASKS = [Tasks.DOMAIN_KNOWLEDGE_MULTICLASSIFICATION]
 
 _SOURCE_VERSION = "1.0.0"
 _SEACROWD_VERSION = "1.0.0"
 
+_LOCAL = False
+
 
 class DengueFilipinoDataset(datasets.GeneratorBasedBuilder):
     """Dengue Dataset Low-Resource Multi-label Text Classification Dataset in Filipino"""
 
     BUILDER_CONFIGS = [
         SEACrowdConfig(
             name=f"{_DATASETNAME}_source",
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/emot/emot.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/emot/emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/emotcmt/emotcmt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/emotcmt/emotcmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/emotes_3k/emotes_3k.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/emotes_3k/emotes_3k.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/etos/etos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/etos/etos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/facqa/facqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/facqa/facqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/facqa/utils/facqa_utils.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/facqa/utils/facqa_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/filwordnet/filwordnet.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/filwordnet/filwordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/fleurs/fleurs.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/fleurs/fleurs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/flores200/flores200.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/flores200/flores200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/fsl_105/fsl_105.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/fsl_105/fsl_105.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/gatitos/gatitos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/gatitos/gatitos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/globalwoz/globalwoz.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/globalwoz/globalwoz.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/glotstorybook/glotstorybook.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/glotstorybook/glotstorybook.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/hoasa/hoasa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/hoasa/hoasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/iapp_squad/iapp_squad.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/iapp_squad/iapp_squad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/iatf/iatf.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/iatf/iatf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/icon/icon.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/icon/icon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive/id_abusive.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive/id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_am2ico/id_am2ico.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_am2ico/id_am2ico.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_clickbait/id_clickbait.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_clickbait/id_clickbait.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_frog_story/id_frog_story.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_frog_story/id_frog_story.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_msvd/id_msvd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_msvd/id_msvd.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 _LICENSE = Licenses.MIT.value
 _URLS = {"text": "https://raw.githubusercontent.com/willyfh/msvd-indonesian/main/data/MSVD-indonesian.txt", "video": "https://www.cs.utexas.edu/users/ml/clamp/videoDescription/YouTubeClips.tar"}
 
 _SUPPORTED_TASKS = [Tasks.VIDEO_TO_TEXT_RETRIEVAL]
 _SOURCE_VERSION = "1.0.0"
 _SEACROWD_VERSION = "1.0.0"
 
+_LOCAL = False
+
 
 class IdMsvdDataset(datasets.GeneratorBasedBuilder):
     """MSVD dataset with Indonesian translation."""
 
     SOURCE_VERSION = datasets.Version(_SOURCE_VERSION)
     SEACROWD_VERSION = datasets.Version(_SEACROWD_VERSION)
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_qqp/id_qqp.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_qqp/id_qqp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_stance/id_stance.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_stance/id_stance.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_sts/id_sts.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_sts/id_sts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/id_wsd/id_wsd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/id_wsd/id_wsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/identic/identic.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/identic/identic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/idk_mrc/idk_mrc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/idk_mrc/idk_mrc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ijelid/ijelid.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ijelid/ijelid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/imdb_jv/imdb_jv.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/imdb_jv/imdb_jv.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo4b/indo4b.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo4b/indo4b.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo_law/indo_law.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo_law/indo_law.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo_puisi/indo_puisi.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo_puisi/indo_puisi.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indocamrest/indocamrest.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indocamrest/indocamrest.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indocollex/indocollex.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indocollex/indocollex.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/indocoref.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/indocoref.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/feature_utils.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/file_utils.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indoler/indoler.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indoler/indoler.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indommlu/indommlu.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indommlu/indommlu.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         ),
     ]
     for lang in _LANGUAGES:
         lang_config = SEACrowdConfig(
             name=f"{_DATASETNAME}_{lang}_seacrowd_qa",
             version=SEACROWD_VERSION,
             description=f"{_DATASETNAME} {lang} SEACrowd schema",
-            schema=f"seacrowd_{lang}_qa",
+            schema=f"seacrowd_qa",
             subset_id=_DATASETNAME,
         )
         BUILDER_CONFIGS.append(lang_config)
 
     DEFAULT_CONFIG_NAME = f"{_DATASETNAME}_source"
 
     def _info(self) -> datasets.DatasetInfo:
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
   year      = {2020},
   howpublished = {Online},
   url       = {https://github.com/andreaschandra/indonesian-news},
   note      = {Accessed: 2024-02-13},
 }
 """
 
+_LANGUAGES = ["ind"]
+
 _DATASETNAME = "indonesian_news_dataset"
 
 _DESCRIPTION = """An imbalanced dataset to classify Indonesian News articles.
 The dataset contains 5 class labels: bola, news, bisnis, tekno, and otomotif.
 The dataset comprises of around 6k train and 2.5k test examples, with the more prevalent classes
 (bola and news) having roughly 10x the number of train and test examples than the least prevalent class (otomotif).
 """
@@ -40,14 +42,16 @@
 
 _SOURCE_VERSION = "1.0.0"
 
 _SEACROWD_VERSION = "1.0.0"
 
 _TAGS = ["bola", "news", "bisnis", "tekno", "otomotif"]
 
+_LOCAL = False
+
 
 class IndonesianNewsDataset(datasets.GeneratorBasedBuilder):
     """The dataset contains 5 Indonesian News articles with imbalanced classes"""
 
     SOURCE_VERSION = datasets.Version(_SOURCE_VERSION)
     SEACROWD_VERSION = datasets.Version(_SEACROWD_VERSION)
     SEACROWD_SCHEMA_NAME = "text"
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonglish/indonglish.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonglish/indonglish.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonli/indonli.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonli/indonli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indoqa/indoqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indoqa/indoqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indosmd/indosmd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indosmd/indosmd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indosum/indosum.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indosum/indosum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indotacos/indotacos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indotacos/indotacos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indowiki/indowiki.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indowiki/indowiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indqner/indqner.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indqner/indqner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/jadi_ide/jadi_ide.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/jadi_ide/jadi_ide.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kamus_alay/kamus_alay.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kamus_alay/kamus_alay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kawat/kawat.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kawat/kawat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kde4/kde4.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kde4/kde4.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/keps/keps.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/keps/keps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kheng_info/kheng_info.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kheng_info/kheng_info.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/khpos/khpos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/khpos/khpos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc/kopi_cc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc/kopi_cc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/limesoda/limesoda.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/limesoda/limesoda.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/liputan6/liputan6.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/liputan6/liputan6.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/lr_sum/lr_sum.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/lr_sum/lr_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/m3exam/m3exam.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/m3exam/m3exam.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mabl/mabl.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mabl/mabl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/malindo_morph/malindo_morph.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/malindo_morph/malindo_morph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/massive/massive.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/massive/massive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mc4_indo/mc4_indo.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mc4_indo/mc4_indo.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 _CONFIGS = {"full": {"train": 1016, "validation": 8}}
 # The entire dataset is 150 Gigs. You can adjust the number of "parquet" files you want to download here
 # _CONFIGS = {
 #     "full": {"train": 1, "validation": 1}
 # }
 
+_LOCAL = False
 
 _SUPPORTED_TASKS = [Tasks.SELF_SUPERVISED_PRETRAINING]
 _SOURCE_VERSION = "1.0.0"
 _SEACROWD_VERSION = "1.0.0"
 
 
 class MC4Indo(datasets.GeneratorBasedBuilder):
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/memolon/memolon.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/memolon/memolon.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,24 @@
 _LICENSE = Licenses.MIT.value
 
 _URLS = {
     _DATASETNAME: "https://zenodo.org/record/3756607/files/MTL_grouped.zip?download=1",
 }
 
 _SOURCE_VERSION = "1.0.0"
+_SEACROWD_VERSION = "1.0.0"
 
 _LANGUAGES = ["ceb", "tgl", "ind", "sun", "jav", "zsm", "vie", "tha", "mya"]
 
 _LANGUAGE_MAP = {"ceb": "Cebuano", "tgl": "Tagalog", "ind": "Indonesian", "sun": "Sundanese", "jav": "Javanese", "zsm": "Malay", "vie": "Vietnamese", "tha": "Thai", "mya": "Burmese"}
 
 _SUPPORTED_TASKS = [Tasks.EMOTION_CLASSIFICATION]
 
+_LOCAL = False
+
 
 def seacrowd_config_constructor(lang: str, schema: str, version: str) -> SEACrowdConfig:
     if lang not in _LANGUAGE_MAP:
         raise ValueError(f"Invalid lang {lang}")
 
     if schema != "source" and schema != "seacrowd_text_multi":
         raise ValueError(f"Invalid schema: {schema}")
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/miracl/miracl.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/miracl/miracl.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,19 @@
 
 _SUPPORTED_TASKS = [Tasks.TEXT_RETRIEVAL]  # example: [Tasks.TRANSLATION, Tasks.NAMED_ENTITY_RECOGNITION, Tasks.RELATION_EXTRACTION]
 
 _SOURCE_VERSION = "1.0.0"
 
 _SEACROWD_VERSION = "1.0.0"
 
+_LOCAL = False
+
 
 def load_topic(fn):
+
     qid2topic = {}
     with open(fn, encoding="utf-8") as f:
         for line in f:
             qid, topic = line.strip().split('\t')
             qid2topic[qid] = topic
     return qid2topic
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mkqa/mkqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mkqa/mkqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mlqa/mlqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mlqa/mlqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 _TRANSLATE_TEST_URL = "mlqa-translate-test.tar.gz"
 _TRANSLATE_TRAIN_URL = "mlqa-translate-train.tar.gz"
 _SUPPORTED_TASKS = [Tasks.QUESTION_ANSWERING]
 
 _SOURCE_VERSION = "1.0.0"
 _SEACROWD_VERSION = "1.0.0"
 
+_LOCAL = False
+
 
 class MLQADataset(datasets.GeneratorBasedBuilder):
     """
     MLQA (MultiLingual Question Answering) is a benchmark dataset for evaluating cross-lingual question answering performance.
     MLQA consists of over 5K extractive QA instances (12K in English) in SQuAD format in seven languages - English, Arabic,
     German, Spanish, Hindi, Vietnamese and Simplified Chinese. MLQA is highly parallel, with QA instances parallel between
     4 different languages on average.
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mswc/mswc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mswc/mswc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mtop_intent_classification/labels.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mtop_intent_classification/labels.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,24 +63,24 @@
 
     BUILDER_CONFIGS = [
         SEACrowdConfig(
             name=f"{_DATASETNAME}_{subset}_source",
             version=datasets.Version(_SOURCE_VERSION),
             description=f"{_DATASETNAME} source schema for {subset} subset",
             schema="source",
-            subset_id=subset,
+            subset_id=f"{_DATASETNAME}_{subset}",
         )
         for subset in SUBSETS
     ] + [
         SEACrowdConfig(
             name=f"{_DATASETNAME}_{subset}_seacrowd_text",
             version=datasets.Version(_SEACROWD_VERSION),
             description=f"{_DATASETNAME} SEACrowd schema for {subset} subset",
             schema="seacrowd_text",
-            subset_id=subset,
+            subset_id=f"{_DATASETNAME}_{subset}",
         )
         for subset in SUBSETS
     ]
 
     DEFAULT_CONFIG_NAME = f"{_DATASETNAME}_domain_source"
 
     def _info(self) -> datasets.DatasetInfo:
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/multilexnorm/multilexnorm.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/multilexnorm/multilexnorm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,50 +70,50 @@
     SEACROWD_SCHEMA_NAME = "t2t"
 
     BUILDER_CONFIGS = [
         SEACrowdConfig(
             name=f"{_DATASETNAME}_source",  # source
             version=SOURCE_VERSION,
             description=f"{_DATASETNAME} source schema",
-            schema="paraphrase_source",
+            schema="source",
             subset_id=f"{_DATASETNAME}_paraphrase",
         ),
         SEACrowdConfig(
             name=f"{_DATASETNAME}_seacrowd_{SEACROWD_SCHEMA_NAME}",  # schema
             version=SEACROWD_VERSION,
             description=f"{_DATASETNAME} SEACrowd schema",
-            schema=f"seacrowd_paraphrase_{SEACROWD_SCHEMA_NAME}",
+            schema=f"seacrowd_{SEACROWD_SCHEMA_NAME}",
             subset_id=f"{_DATASETNAME}_paraphrase",
         ),
         SEACrowdConfig(
             name=f"{_DATASETNAME}_non_paraphrase_source",  # source
             version=SEACROWD_VERSION,
             description=f"{_DATASETNAME} SEACrowd schema",
-            schema="non_paraphrase_source",
+            schema="source",
             subset_id=f"{_DATASETNAME}_non_paraphrase",
         ),
         SEACrowdConfig(
             name=f"{_DATASETNAME}_non_paraphrase_seacrowd_{SEACROWD_SCHEMA_NAME}",  # schema
             version=SEACROWD_VERSION,
             description=f"{_DATASETNAME} SEACrowd schema",
-            schema=f"seacrowd_non_paraphrase_{SEACROWD_SCHEMA_NAME}",
+            schema=f"seacrowd_{SEACROWD_SCHEMA_NAME}",
             subset_id=f"{_DATASETNAME}_non_paraphrase",
         ),
         SEACrowdConfig(
             name=f"{_DATASETNAME}_all_source",  # source
             version=SOURCE_VERSION,
             description=f"{_DATASETNAME} source schema",
-            schema="all_source",
+            schema="source",
             subset_id=f"{_DATASETNAME}_all",
         ),
         SEACrowdConfig(
             name=f"{_DATASETNAME}_all_seacrowd_{SEACROWD_SCHEMA_NAME}",  # schema
             version=SEACROWD_VERSION,
             description=f"{_DATASETNAME} SEACrowd schema",
-            schema=f"seacrowd_all_{SEACROWD_SCHEMA_NAME}",
+            schema=f"seacrowd_{SEACROWD_SCHEMA_NAME}",
             subset_id=f"{_DATASETNAME}_all",
         ),
     ]
 
     DEFAULT_CONFIG_NAME = f"{_DATASETNAME}_seacrowd_{SEACROWD_SCHEMA_NAME}"
 
     def _info(self) -> datasets.DatasetInfo:
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mypos/mypos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mypos/mypos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/mysentence/mysentence.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/mysentence/mysentence.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/myxnli/myxnli.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/myxnli/myxnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nergrit/nergrit.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nergrit/nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nerp/nerp.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nerp/nerp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/netifier/netifier.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/netifier/netifier.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/news_en_id/news_en_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/news_en_id/news_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/newsph/newsph.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/newsph/newsph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nllb_seed/nllb_seed.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nllb_seed/nllb_seed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ntrex_128/ntrex_128.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ntrex_128/ntrex_128.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusax_mt/nusax_mt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusax_mt/nusax_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/nusax_senti/nusax_senti.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/nusax_senti/nusax_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/oil/oil.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/oil/oil.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ojw/ojw.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ojw/ojw.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/openlid/openlid.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/openlid/openlid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/openslr/openslr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/openslr/openslr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/orchid_pos/orchid_pos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/orchid_pos/orchid_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/oscar_2201/oscar_2201.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/oscar_2201/oscar_2201.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/palito/palito.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/palito/palito.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/paracotta_id/paracotta_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/paracotta_id/paracotta_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 _HOMEPAGE = "https://github.com/aaroncarlfernandez/Philippine-Fake-News-Corpus"
 _LICENSE = Licenses.UNKNOWN.value
 _URL = "https://github.com/aaroncarlfernandez/Philippine-Fake-News-Corpus/raw/master/Philippine%20Fake%20News%20Corpus.zip/"
 
 _SUPPORTED_TASKS = [Tasks.FACT_CHECKING]
 _SOURCE_VERSION = "1.0.0"
+_SEACROWD_VERSION = "1.0.0"
 
 
 class PhilippineFakeNewsDataset(datasets.GeneratorBasedBuilder):
     """
     Dataset of English news articles from the Philippines manually annotated as "credible" or
     "non-credible" based on source.
     """
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/phomt/phomt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/phomt/phomt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/phost/phost.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/phost/phost.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/posp/posp.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/posp/posp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/postag_su/postag_su.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/postag_su/postag_su.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/prdect_id/prdect_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/prdect_id/prdect_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/qasina/qasina.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/qasina/qasina.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sampiran/sampiran.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sampiran/sampiran.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sap_wat/sap_wat.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sap_wat/sap_wat.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 ]
 
 _SOURCE_VERSION = "1.0.0"
 _SEACROWD_VERSION = "1.0.0"
 
 _SUBSET = ["id", "ms", "th", "vi"]
 
+_LOCAL = False
+
 class SapWatDataset(datasets.GeneratorBasedBuilder):
     """SAP WAT is a software documentation dataset for machine translation. The current language scope is English to Hindi, 
     Indonesian, Japanese, Korean, Malay, Thai, Vietnamese, Simplified Chinese and Traditional Chinese. Here, we only consider 
     EN-ID, EN-TH, EN-MS, EN-VI"""
 
     BUILDER_CONFIGS = [
         SEACrowdConfig(
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sea_bench/sea_bench.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sea_bench/sea_bench.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sea_madlad/sea_madlad.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sea_madlad/sea_madlad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sea_wiki/sea_wiki.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sea_wiki/sea_wiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/seaeval/seaeval.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/seaeval/seaeval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/seahorse/seahorse.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/seahorse/seahorse.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/singgalang/singgalang.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/singgalang/singgalang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/smsa/smsa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/smsa/smsa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/snli_indo/snli_indo.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/snli_indo/snli_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/spamid_pair/spamid_pair.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/spamid_pair/spamid_pair.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/squad_id/squad_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/squad_id/squad_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/stb_ext/stb_ext.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/stb_ext/stb_ext.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/su_emot/su_emot.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/su_emot/su_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/su_id_asr/su_id_asr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/su_id_asr/su_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/su_id_tts/su_id_tts.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/su_id_tts/su_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/talpco/talpco.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/talpco/talpco.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tatabahasa/tatabahasa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tatabahasa/tatabahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tatoeba/tatoeba.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tatoeba/tatoeba.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tcope/tcope.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tcope/tcope.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ted_en_id/ted_en_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ted_en_id/ted_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/term_a/term_a.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/term_a/term_a.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_constitution/thai_constitution.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_constitution/thai_constitution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_depression/thai_depression.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_depression/thai_depression.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_sum/thai_sum.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_sum/thai_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tico_19/tico_19.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tico_19/tico_19.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/titml_idn/titml_idn.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/titml_idn/titml_idn.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/toxicity_200/toxicity_200.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/toxicity_200/toxicity_200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/tydiqa/tydiqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/tydiqa/tydiqa.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
 _HOMEPAGE = "https://github.com/google-research-datasets/tydiqa"
 _LICENSE = Licenses.APACHE_2_0.value
 _HF_URL = "https://huggingface.co/datasets/tydiqa"
 _SUPPORTED_TASKS = [Tasks.QUESTION_ANSWERING]
 _LANGUAGES = ["ind", "tha"]
 _LOCAL = False
+_SOURCE_VERSION = "1.0.0"
 _SOURCE_VERSION_P = "1.0.0"
 _SOURCE_VERSION_S = "1.1.0"
 _SEACROWD_VERSION = "1.0.0"
 
 _URL = "https://storage.googleapis.com/tydiqa/"
 _PRIMARY_URLS = {
     "train": _URL + "v1.0/tydiqa-v1.0-train.jsonl.gz",
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/udhr/udhr.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/udhr/udhr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/udhr_lid/udhr_lid.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/udhr_lid/udhr_lid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_victsd/uit_victsd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_victsd/uit_victsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_viic/uit_viic.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_viic/uit_viic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_viocd/uit_viocd.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_viocd/uit_viocd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_vion/uit_vion.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_vion/uit_vion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 _SUPPORTED_TASKS = [Tasks.SPAN_BASED_ABSA]
 
 _SOURCE_VERSION = "1.0.0"
 
 _SEACROWD_VERSION = "1.0.0"
 
+_LOCAL = False
+
 
 def construct_label_classes():
     IOB_tag = ["I", "O", "B"]
     aspects = ["SCREEN", "CAMERA", "FEATURES", "BATTERY", "PERFORMANCE", "STORAGE", "DESIGN", "PRICE", "GENERAL", "SER&ACC"]
     ratings = ["POSITIVE", "NEUTRAL", "NEGATIVE"]
     label_classes = []
     for iob in IOB_tag:
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/unimorph/unimorph.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/unimorph/unimorph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/unimorph_id/unimorph_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/unimorph_id/unimorph_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vihealthqa/vihealthqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vihealthqa/vihealthqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/visobert/visobert.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/visobert/visobert.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vispamreviews/vispamreviews.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vispamreviews/vispamreviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vitext2sql/vitext2sql.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vitext2sql/vitext2sql.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vivos/vivos.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vivos/vivos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vivqa/vivqa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vivqa/vivqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vndt/utils.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vndt/utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/vndt/vndt.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/vndt/vndt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/voxlingua/voxlingua.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/voxlingua/voxlingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/weathub/weathub.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/weathub/weathub.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wikiann/wikiann.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wikiann/wikiann.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wikilingua/wikilingua.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wikilingua/wikilingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wikimatrix/wikimatrix.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wikimatrix/wikimatrix.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wili_2018/wili_2018.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wili_2018/wili_2018.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wit/wit.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wit/wit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/wrete/wrete.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/wrete/wrete.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/x_fact/x_fact.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/x_fact/x_fact.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xcopa/xcopa.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xcopa/xcopa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xl_sum/xl_sum.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xl_sum/xl_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xm3600/xm3600.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xm3600/xm3600.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 _SOURCE_VERSION = "1.0.0"
 
 _SEACROWD_VERSION = "1.0.0"
 
 _LANGUAGES = ["fil", "id", "th", "vi"]
 
+_LOCAL = False
+
 
 class XM3600Dataset(datasets.GeneratorBasedBuilder):
     """
     Crossmodal-3600 dataset (XM3600 in short), a geographically-diverse set of 3600 images annotated with
     human-generated reference captions in 36 languages. The images were selected from across the world,
     covering regions where the languages are spoken, and annotated with captions that achieve consistency in
     terms of style across all languages, while avoiding annotation artifacts due to direct translation.
```

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xnli/xnli.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xnli/xnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xpersona_id/xpersona_id.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xpersona_id/xpersona_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xquad/xquad.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xquad/xquad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xsid/xsid.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xsid/xsid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/xstorycloze/xstorycloze.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/xstorycloze/xstorycloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py` & `seacrowd-0.0.2/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/common_parser.py` & `seacrowd-0.0.2/seacrowd/utils/common_parser.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/constants.py` & `seacrowd-0.0.2/seacrowd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/__init__.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/imqa.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/imqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/kb.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/kb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/pairs.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/pairs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/qa.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/seq_label.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/seq_label.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/speech.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/speech_multilabel.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/speech_multilabel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/speech_to_speech.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/speech_to_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/tod.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/tod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/tree.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/tree.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd/utils/schemas/video.py` & `seacrowd-0.0.2/seacrowd/utils/schemas/video.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/seacrowd.egg-info/PKG-INFO` & `seacrowd-0.0.2/seacrowd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.1
+Version: 0.0.2
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.1/seacrowd.egg-info/SOURCES.txt` & `seacrowd-0.0.2/seacrowd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 seacrowd/__init__.py
+seacrowd/config_helper.py
 seacrowd.egg-info/PKG-INFO
 seacrowd.egg-info/SOURCES.txt
 seacrowd.egg-info/dependency_links.txt
 seacrowd.egg-info/requires.txt
 seacrowd.egg-info/top_level.txt
 seacrowd/sea_datasets/__init__.py
 seacrowd/sea_datasets/abui_wordnet/__init__.py
```

### Comparing `seacrowd-0.0.1/setup.cfg` & `seacrowd-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/tests/test_seacrowd.py` & `seacrowd-0.0.2/tests/test_seacrowd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.1/tests/test_seacrowd_source_only.py` & `seacrowd-0.0.2/tests/test_seacrowd_source_only.py`

 * *Files identical despite different names*

