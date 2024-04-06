# Comparing `tmp/modern-greek-inflexion-2.0.0.tar.gz` & `tmp/modern-greek-inflexion-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modern-greek-inflexion-2.0.0.tar", last modified: Mon Feb 26 21:51:19 2024, max compression
+gzip compressed data, was "modern-greek-inflexion-2.0.1.tar", last modified: Sat Apr  6 16:58:09 2024, max compression
```

## Comparing `modern-greek-inflexion-2.0.0.tar` & `modern-greek-inflexion-2.0.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.337762 modern-greek-inflexion-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-02-26 21:51:19.333762 modern-greek-inflexion-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-26 21:51:19.337762 modern-greek-inflexion-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.281762 modern-greek-inflexion-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.285762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.285762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.285762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/all/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/all/create_all_adj.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/all/create_all_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.285762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.285762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adverb/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adverb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.285762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/article/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/article/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.289762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38618 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/create_noun_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/create_noun_decl.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.289762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/create_num_decl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/create_num_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.289762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/create_pron_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/create_pron_decl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.289762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/adj.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/adv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/article.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.325762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle
--rw-r--r--   0 runner    (1001) docker     (127) 29309847 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/el_GR.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   347390 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/noun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/numerals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/pronouns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    33523 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/verb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.329762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.329762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.329762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.329762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.329762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.329762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17592 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.333762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.333762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.333762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.333762 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-02-26 21:51:19.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-02-26 21:51:19.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 21:51:19.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 21:51:19.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-26 21:51:19.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-26 21:51:19.000000 modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:19.333762 modern-greek-inflexion-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:51:10.000000 modern-greek-inflexion-2.0.0/test/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-06 16:58:09.512697 modern-greek-inflexion-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.452697 modern-greek-inflexion-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.456697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.460697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.460697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/all/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/all/create_all_adj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/all/create_all_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.460697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.460697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adverb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adverb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.460697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/article/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/article/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.460697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38618 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/create_noun_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28125 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/create_noun_decl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.464697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/create_num_decl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/create_num_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.464697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/create_pron_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/create_pron_decl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.464697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/adj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/adv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/article.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.500697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle
+-rw-r--r--   0 runner    (1001) docker     (127) 29309847 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/el_GR.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   347390 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/noun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/numerals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/pronouns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33523 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/verb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.500697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.504697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.504697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.504697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.504697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.504697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17592 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-06 16:58:09.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-06 16:58:09.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:58:09.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:58:09.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 16:58:09.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 16:58:09.000000 modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:09.508697 modern-greek-inflexion-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:04.000000 modern-greek-inflexion-2.0.1/test/test_case.py
```

### Comparing `modern-greek-inflexion-2.0.0/LICENSE` & `modern-greek-inflexion-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/PKG-INFO` & `modern-greek-inflexion-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-greek-inflexion
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python 3 library for creating inflected forms given basic forms of Modern Greek words
 Home-page: https://github.com/PicusZeus/modern-greek-inflexion
 Author: Krzysztof H
 Author-email: krzysztof.hilman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -43,27 +43,28 @@
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install modern-greek-inflexion.
 
 ```bash
 pip install modern-greek-inflexion
 ```
 
 ## Usage
-You can read the docs [here](https://github.com/PicusZeus/modern-greek-inflexion.git)
+You can read the docs [here](https://modern-greek-inflexion.readthedocs.io/en/latest/)
 
 ## Unittests
 run 
 >python -m unittest
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
  * 1.0.4 Added logic for multiple root formation in verbs on -άρω (σοκάρω, σοκαρίζω, σοκαρίσω), now the app will try to create also imperfect forms with a root on 'ιζ'. The Experiment with extending the core language check corpus failed miserably, as all the corpora I tried (even these from the EU) are unfortunately full of typos and orthographic errors, which, when used, introduced into the app huge problems. Next time I will try to use some NLTK magic and frequency lists to try them again.
  * 1.0.3 The problem with verbs with prefix para fixed by adding a flag to verb.create_all_forms para. If there is possibility, that there are two different verbs (like παραβλέπω/παραβλέψω and παραβλέπω/παραδώ), you have to set flag para to True. Fixed issue with non existent imper aor sg of compound verbs with βαίνω (like παρεμβαίνω).
  * 1.0.2 Updated list of irregular past passive participles, deleted most of them as they're not needed anymore and in places they would cause incorrect participle formation.
  * 1.0.1 Project is mature enough, some issue with dependency accentuation module fixed.
```

### Comparing `modern-greek-inflexion-2.0.0/README.md` & `modern-greek-inflexion-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install modern-greek-inflexion.
 
 ```bash
 pip install modern-greek-inflexion
 ```
 
 ## Usage
-You can read the docs [here](https://github.com/PicusZeus/modern-greek-inflexion.git)
+You can read the docs [here](https://modern-greek-inflexion.readthedocs.io/en/latest/)
 
 ## Unittests
 run 
 >python -m unittest
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
  * 1.0.4 Added logic for multiple root formation in verbs on -άρω (σοκάρω, σοκαρίζω, σοκαρίσω), now the app will try to create also imperfect forms with a root on 'ιζ'. The Experiment with extending the core language check corpus failed miserably, as all the corpora I tried (even these from the EU) are unfortunately full of typos and orthographic errors, which, when used, introduced into the app huge problems. Next time I will try to use some NLTK magic and frequency lists to try them again.
  * 1.0.3 The problem with verbs with prefix para fixed by adding a flag to verb.create_all_forms para. If there is possibility, that there are two different verbs (like παραβλέπω/παραβλέψω and παραβλέπω/παραδώ), you have to set flag para to True. Fixed issue with non existent imper aor sg of compound verbs with βαίνω (like παρεμβαίνω).
  * 1.0.2 Updated list of irregular past passive participles, deleted most of them as they're not needed anymore and in places they would cause incorrect participle formation.
  * 1.0.1 Project is mature enough, some issue with dependency accentuation module fixed.
```

### Comparing `modern-greek-inflexion-2.0.0/setup.cfg` & `modern-greek-inflexion-2.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modern-greek-inflexion
-version = 2.0.0
+version = 2.0.1
 description = Python 3 library for creating inflected forms given basic forms of Modern Greek words
 long_description_content_type = text/markdown
 long_description = file: README.md
 license = MIT
 url = https://github.com/PicusZeus/modern-greek-inflexion
 author = Krzysztof H
 author_email = krzysztof.hilman@gmail.com
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from modern_greek_inflexion.adjective.basic.create_basic_adj import create_all_basic_forms
 from .all.create_all_adj import create_all_adj_forms
 from ..exceptions import NotInGreekException
 from modern_greek_inflexion.verb.helpers import merging_all_dictionaries
 from modern_greek_accentuation.accentuation import convert_to_monotonic
 
-from ..resources.typing import adjective_basic_forms, declension_forms_type
+from ..resources.typing import adj_basic_forms_type, genders_declensions_type, adj_declension_degree_type
 from ..resources.variables import ADJ, ADVERB, COMP, COMP_ADV, ADV, COMPARATIVE, ADVERB_COMPARATIVE, SUPERL, SUPERL_ADV
 from modern_greek_inflexion.resources import greek_pattern
 
 
 class Adjective:
     """
     This class can be used to create adjective forms, all or only in certain degree, you can do it by instantiating the class with a single basic form (nom sg masc), you can also add already prepared basic forms.
@@ -17,31 +17,31 @@
     :type adj: str
     :param aklito: If you know the noun is indeclinable, set it to True
     :type aklito: bool, optional
     :param basic_forms: a dictionary with the following shape ``{ADJ: "masc/fem/neut", COMPARATIVE: "parathetiko,alt_parathetiko/uperthetiko,alt_uperthetiko, ADVERB: "adverb,alt_adverb", ADVERB_COMPARATIVE: "adverb_parathetiko,alt_adverb_parathetiko/adverb_uperthetiko,alt_adverb_uperthetiko"}``
     :type basic_forms: dict, optional
     """
 
-    def __init__(self, adj: str, aklito: bool = False, basic_forms: dict = None):
+    def __init__(self, adj: str, aklito: bool = False, basic_forms: adj_basic_forms_type = None):
 
         self.adjective = adj
         adj = convert_to_monotonic(adj, one_syllable_rule=False)
 
         if not greek_pattern.match(adj):
             raise NotInGreekException
         if basic_forms:
             self.basic_forms = basic_forms
         else:
             self.basic_forms = create_all_basic_forms(adj, aklito)
 
     @staticmethod
-    def _adj(basic: str, adverb: str) -> tuple[declension_forms_type, set[str]]:
+    def _adj(basic: str, adverb: str) -> tuple[adj_declension_degree_type, set[str]]:
         """
         :param basic: "masc/fem/neut"
-        :param adverb: "adverb,alt_adverb
+        :param adverb: set adverb, alt_adverb
         :return: two element tuple, the first is a dictionary with all inflexion adjective forms with the following
         structure:{SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, the second one is a set containing adverbs
         """
         forms, alternative_forms = create_all_adj_forms(basic)
 
         if alternative_forms:
             adj = merging_all_dictionaries(forms, alternative_forms)
@@ -51,25 +51,25 @@
         if adverb:
             adv = set(adverb.split(','))
         else:
             adv = set()
 
         return adj, adv
 
-    def positive_degree(self) -> {ADJ: declension_forms_type, ADV: set[str]}:
+    def positive_degree(self) -> {ADJ: adj_declension_degree_type, ADV: set[str]}:
         """
         Creates positive degree forms
 
         :return: A dictionary of adjective forms in positive degree with the following shape: ``{ADJ: {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, ADV: set(forms)}``
         :rtype: dict
         """
         adj, adv = self._adj(self.basic_forms[ADJ], self.basic_forms[ADVERB])
         return {ADJ: adj, ADV: adv}
 
-    def _comp_degree(self, bas_compars: str) -> tuple[declension_forms_type, set[str]]:
+    def _comp_degree(self, bas_compars: str) -> tuple[adj_declension_degree_type, set[str]]:
         """
         Creates comparative degree forms
 
         :param bas_compars: adj: masc nom sg form (`ωραιότερος`)
         :return: two element tuple, the first is a dictionary with all inflexion adjective forms with the following
         structure:{SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, the second one is a set containing adverbs
         """
@@ -82,46 +82,47 @@
             all_compars.append(adj)
 
             all_adverbs.update(adv)
         all_comp_forms = merging_all_dictionaries(*all_compars)
 
         return all_comp_forms, all_adverbs
 
-    def comparative_degree(self) -> {COMP: declension_forms_type, COMP_ADV: set[str]}:
+    def comparative_degree(self) -> {COMP: adj_declension_degree_type, COMP_ADV: set[str]}:
         """
         Creates comparative degree forms
 
         :return: A dictionary of adjective forms in the comparative degree with the following shape: ``COMP: {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, COMP_ADV: set(forms)``
         :rtype: dict
         """
         basic_compar = self.basic_forms[COMPARATIVE]
         if basic_compar:
             compars, superlatives = basic_compar.split('/')
             advs_compar, advs_superlative = self.basic_forms[ADVERB_COMPARATIVE].split('/')
             if compars != '-':
                 comparative_forms, comparative_adv = self._comp_degree(compars)
                 return {COMP: comparative_forms, COMP_ADV: set(advs_compar.split(','))}
 
-    def superlative_degree(self) -> {SUPERL: declension_forms_type, SUPERL_ADV: set[str]}:
+    def superlative_degree(self) -> {SUPERL: adj_declension_degree_type, SUPERL_ADV: set[str]}:
+
         """
         Create superlative degree forms
 
         :return: A dictionary of adjective forms in the superlative degree with the following shape ``SUPERL: {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, SUPERL_ADV: set(forms)}``
         :rtype: dict
         """
         basic_compar = self.basic_forms[COMPARATIVE]
         if basic_compar:
             compars, superlatives = basic_compar.split('/')
             advs_compar, advs_superlative = self.basic_forms[ADVERB_COMPARATIVE].split('/')
             if superlatives != '-':
                 comparative_forms, comparative_adv = self._comp_degree(superlatives)
                 return {SUPERL: comparative_forms, SUPERL_ADV: set(advs_superlative.split(','))}
 
-    def all(self) -> {ADJ: declension_forms_type, ADV: set[str], COMP: declension_forms_type, COMP_ADV: set[str],
-                      SUPERL: declension_forms_type, SUPERL_ADV: set[str]}:
+    def all(self) -> {ADJ: adj_declension_degree_type, ADV: set[str], COMP: adj_declension_degree_type, COMP_ADV: set[str],
+                      SUPERL: adj_declension_degree_type, SUPERL_ADV: set[str]}:
         """
         Create all forms from a basic adjective form
 
         :return: a dictionary with the following shape ``{ADJ: {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, ADV: set(forms), COMP: {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, COMP_ADV: set(forms), SUPERL: {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}, SUPERL_ADV: set(forms)}``
         :rtype: dict
         """
         _all = {}
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/_helpers.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from modern_greek_accentuation._helpers import AccentType
 
 from modern_greek_accentuation.accentuation import put_accent, where_is_accent
 from modern_greek_accentuation.syllabify import count_syllables
 
 from modern_greek_inflexion.resources import PENULTIMATE
-from modern_greek_inflexion.resources.typing import declension_forms_type
+from modern_greek_inflexion.resources.typing import genders_declensions_type
 
 
-def put_accent_on_all_forms(forms: declension_forms_type, accent: AccentType) -> dict:
+def put_accent_on_all_forms(forms: genders_declensions_type, accent: AccentType) -> dict:
     """
     Put stress on all adjective forms
     :param forms: Dictionary {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}
     :param accent: Accent name
     :return: Dictionary {SG: {MASC: {NOM: set(forms), ...}, ...}, ...}
     """
     for num in forms.keys():
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/all/create_all_adj.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/all/create_all_adj.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 from modern_greek_inflexion.adjective.all.create_all_alt import alternative_forms_r, alternative_forms_ios, \
     alternative_forms_us, alternative_fem_os, alternative_forms_kxth, alternative_forms_modern_3rd, \
     alternative_forms_onas, alternative_forms_tis, alternative_forms_wn, alternative_forms_us2, alternative_forms_ou
 from modern_greek_inflexion.adjective._helpers import put_accent_on_all_forms, put_accent_on_unaccented_forms
 from modern_greek_inflexion.resources import greek_corpus
 from modern_greek_inflexion.resources.adj import adj_basic_template
-from modern_greek_inflexion.resources.typing import declension_forms_type
+from modern_greek_inflexion.resources.typing import genders_declensions_type, adj_declension_degree_type
 from modern_greek_inflexion.resources.variables import SG, PL, FEM, MASC, NEUT, NOM, GEN, ACC, VOC, ANTEPENULTIMATE, \
     ULTIMATE, PENULTIMATE
 
 """
 example
 adj = {'adj': 'ωμός/ωμή/ωμό', 'comparative': 'ωμότερος/ωμότατος', 'adverb': 'ωμά',
 'adverb_comparative': 'ωμότερα/ωμότατα'}
 """
 
 
-def create_all_adj_forms(adj: str) -> tuple[declension_forms_type, declension_forms_type | None]:
+def create_all_adj_forms(adj: str) -> tuple[adj_declension_degree_type, adj_declension_degree_type | None]:
     """
     :param adj: expects masc, fem and neut forms divided with slash / (eg 'ωραίος/ωραία/ωραίο). If feminine doesn't exist, it should be replaced with dash '-'.
     :return: two element tuple, first is a dictionary with all primary forms (forms[number][gender][case], the second
     one is a dictionary with alternative forms, if exists it has the same structure as the first dictionary
     """
     forms = deepcopy(adj_basic_template)
     fem_alt = None
@@ -768,15 +768,15 @@
             for gender in forms[number].keys():
                 for case in forms[number][gender].keys():
                     forms[number][gender][case] = masc
 
         return forms, None
 
 
-def create_all_comparative_forms(comp_or_super: str) -> declension_forms_type:
+def create_all_comparative_forms(comp_or_super: str) -> genders_declensions_type:
     """
     :param comp_or_super: one form ending in os
     :return: all forms in a dict
     """
 
     if comp_or_super[-2:] in ['ών', 'ων']:
         accent = where_is_accent(comp_or_super)
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/all/create_all_alt.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/all/create_all_alt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from copy import deepcopy
 
 from modern_greek_accentuation.accentuation import put_accent, put_accent_on_the_penultimate, put_accent_on_the_ultimate
 from modern_greek_inflexion.adjective._helpers import put_accent_on_all_forms
 from modern_greek_inflexion.resources import greek_corpus
-from modern_greek_inflexion.resources.typing import declension_forms_type
+from modern_greek_inflexion.resources.typing import genders_declensions_type, adj_declension_degree_type
 from modern_greek_inflexion.resources.variables import SG, FEM, NOM, ACC, GEN, VOC, NEUT, MASC, PL, ULTIMATE
 from modern_greek_accentuation._helpers import AccentType
 from modern_greek_inflexion.resources.adj import adj_basic_template_alt
 
 
-def alternative_forms_r(fem: str, accent: AccentType) -> declension_forms_type:
+def alternative_forms_r(fem: str, accent: AccentType) -> adj_declension_degree_type:
     """
 
     :param fem: feminine nom sg
     :param accent: accent type
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
@@ -24,15 +24,15 @@
         alt_forms[SG][FEM][ACC] = alt_form
         alt_forms[SG][FEM][GEN] = alt_form + 'ς'
         alt_forms[SG][FEM][VOC] = alt_form
 
     return alt_forms
 
 
-def alternative_forms_ios(adj: str) -> declension_forms_type:
+def alternative_forms_ios(adj: str) -> adj_declension_degree_type:
     """
     Alternatives for adjective that ends on 'ιος'
     :param adj: adj: str "masc/fem/neut"
     :return: dictionary {gender: number: case: {forms}}
     """
     masc, fem, neut = adj.split('/')
     alt_forms = deepcopy(adj_basic_template_alt)
@@ -56,15 +56,15 @@
         if fem_nom + 'ν' not in greek_corpus:
             alt_forms[SG][FEM][ACC] = fem_nom
         alt_forms[SG][FEM][VOC] = fem_nom
 
     return alt_forms
 
 
-def alternative_forms_us(adj: str) -> declension_forms_type:
+def alternative_forms_us(adj: str) -> adj_declension_degree_type:
 
     """
     Alternatives for the υς, ια, υ type
     :param adj: str "masc/fem/neut"
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
@@ -110,15 +110,15 @@
         alt_forms[PL][FEM][GEN] = fem[:-2] + 'ειών'
 
     if masc.endswith('πολύς') or masc.endswith('μέγας'):
         alt_forms.pop(PL)
     return alt_forms
 
 
-def alternative_forms_us2(adj: str) -> declension_forms_type:
+def alternative_forms_us2(adj: str) -> adj_declension_degree_type:
     """
     Alternatives for the υς, ια, υ, only gen έος
     :param adj: str "masc/fem/neut"
     :return: dictionary {gender: number: case: {forms}}
     """
     #
 
@@ -129,17 +129,18 @@
     if masc:
         alt_forms[SG][MASC][GEN] = masc[:-2] + 'έος'
         alt_forms[SG][NEUT][GEN] = masc[:-2] + 'έος'
 
     return alt_forms
 
 
-def alternative_fem_os(fem_os: str, accent: AccentType) -> declension_forms_type:
+def alternative_fem_os(fem_os: str, accent: AccentType) -> adj_declension_degree_type:
     """
     Alternative for feminine forms on -ος
+
     :param fem_os: nom sg
     :param accent: accent name
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
 
     alt_forms[SG][FEM][NOM] = fem_os
@@ -151,18 +152,19 @@
     alt_forms[PL][FEM][ACC] = fem_os[:-2] + 'ους'
     alt_forms[PL][FEM][GEN] = fem_os[:-2] + 'ων'
     alt_forms[PL][FEM][VOC] = fem_os[:-2] + 'οι'
 
     return put_accent_on_all_forms(alt_forms, accent)
 
 
-def alternative_forms_kxth(fem: str, accent: AccentType) -> declension_forms_type:
+def alternative_forms_kxth(fem: str, accent: AccentType) -> adj_declension_degree_type:
 
     """
     Alternatives feminine for adj with stem ending on κ, χ, θ (ια)
+
     :param fem: singular nominative
     :param accent:
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
 
     alt_form = fem[:-1] + 'ια'
@@ -175,17 +177,18 @@
         alt_forms[SG][FEM][ACC] = alt_form
         alt_forms[SG][FEM][GEN] = alt_form + 'ς'
         alt_forms[SG][FEM][VOC] = alt_form
 
     return alt_forms
 
 
-def alternative_forms_modern_3rd(adj: str) -> declension_forms_type:
+def alternative_forms_modern_3rd(adj: str) -> adj_declension_degree_type:
     """
     Alternatives for 3rd declension adjectives
+
     :param adj: str "masc/fem/neut"
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
     masc, fem, neut = adj.split('/')
 
     stem = neut + 'τ'
@@ -197,15 +200,15 @@
         alt_forms[SG][FEM][GEN] = fem[:-1] + 'ης'
     if fem + 'ν' in greek_corpus:
         alt_forms[SG][FEM][ACC] = fem + 'ν'
 
     return alt_forms
 
 
-def alternative_forms_wn(adj: str) -> declension_forms_type:
+def alternative_forms_wn(adj: str) -> adj_declension_degree_type:
     """
     Alternatives for adj/participles on ων, ουσα, ον
     :param adj: str "masc/fem/neut"
     :return: dictionary {gender: number: case: {forms}}
     """
     #
     alt_forms = deepcopy(adj_basic_template_alt)
@@ -241,15 +244,15 @@
         alt_forms[PL][FEM][ACC] = fem[:-1] + 'ες'
         alt_forms[PL][FEM][GEN] = put_accent_on_the_ultimate(fem[:-1] + 'ων')
         alt_forms[PL][FEM][VOC] = fem[:-1] + 'ες'
 
     return alt_forms
 
 
-def alternative_forms_tis(adj: str, stem: str) -> declension_forms_type:
+def alternative_forms_tis(adj: str, stem: str) -> adj_declension_degree_type:
     """
     Alternative forms for adjectives on ις, ις, ι
     :param adj: str "masc/fem/neut"
     :param stem: stem visible in gen, and plural
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
@@ -262,15 +265,15 @@
     alt_forms[PL][MASC][GEN] = gen_pl
     alt_forms[PL][FEM][GEN] = gen_pl
     alt_forms[PL][NEUT][GEN] = gen_pl
 
     return alt_forms
 
 
-def alternative_forms_onas(adj: str) -> declension_forms_type:
+def alternative_forms_onas(adj: str) -> adj_declension_degree_type:
     """
     Alternatives for adj on ωνας
     :param adj: str "masc/fem/neut"
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
 
@@ -288,15 +291,15 @@
     if fem:
         alt_forms[SG][MASC][NOM] = fem
         alt_forms[SG][MASC][VOC] = fem
 
     return alt_forms
 
 
-def alternative_forms_ou(fem: str) -> declension_forms_type:
+def alternative_forms_ou(fem: str) -> adj_declension_degree_type:
     """
     Alternatives for feminine on ου
     :param fem: nom sg
     :return: dictionary {gender: number: case: {forms}}
     """
     alt_forms = deepcopy(adj_basic_template_alt)
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 from modern_greek_accentuation.accentuation import is_accented, where_is_accent, put_accent, count_syllables, \
     put_accent_on_the_antepenultimate, put_accent_on_the_penultimate, remove_all_diacritics, put_accent_on_the_ultimate
 from modern_greek_accentuation.resources import vowels
 from modern_greek_accentuation.syllabify import modern_greek_syllabify
 from modern_greek_inflexion.exceptions import NotLegalAdjectiveException
 from modern_greek_inflexion.resources import greek_corpus
-from modern_greek_inflexion.resources.typing import adjective_basic_forms
+from modern_greek_inflexion.resources.typing import adj_basic_forms_type
 from modern_greek_inflexion.resources.variables import (ADJ, ADVERB, ADVERB_COMPARATIVE, COMPARATIVE, INCORRECT_ACCENT,
                                                         ULTIMATE,
                                                         ANTEPENULTIMATE, PENULTIMATE, ADJ_FEM_OS_ONLY, ADJ_FEM_OS_ALSO)
 from modern_greek_inflexion.resources.adj import irregular_comparatives, irregular_comparative_adverbs, \
     adj_grammar_lists
 
 
-def create_all_basic_forms(adj: str, aklito: bool = False) -> adjective_basic_forms:
+def create_all_basic_forms(adj: str, aklito: bool = False) -> adj_basic_forms_type:
     """
     :param aklito: if relevant, boolean
     :param adj: masc nom sg form (`ωραίος`)
     :return: dictionary with keys:
          {ADJ: "masc/fem/neut",
          COMPARATIVE: "parathetiko,alt_parathetiko/uperthetiko,alt_uperthetiko,
          ADVERB: "adverb,alt_adverb",
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/adverb/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/adverb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .. import adjective
 from ..adjective import Adjective
 from ..resources import greek_pattern
 from ..resources.adv import irregular_adv
 from modern_greek_inflexion.resources.variables import ADV, COMP_ADV, ADJ, COMP, SUPERL, SUPERL_ADV
 from ..exceptions import NotInGreekException
-from ..resources.typing import declension_forms_type
+from ..resources.typing import genders_declensions_type, adj_declension_degree_type
 
 
 class Adverb:
     """
     This class can be used to create adverb forms
 
     :param adverb: an adverb form
@@ -18,16 +18,16 @@
 
     def __init__(self, adverb: str):
 
         if not greek_pattern.match(adverb):
             raise NotInGreekException
         self.adverb = adverb
 
-    def all(self) -> {ADV: set[str], COMP_ADV: set[str], SUPERL_ADV: set[str], SUPERL: declension_forms_type,
-                      COMP: declension_forms_type}:
+    def all(self) -> {ADV: set[str], COMP_ADV: set[str], SUPERL_ADV: set[str], SUPERL: adj_declension_degree_type,
+                      COMP: adj_declension_degree_type}:
         """
         If an adverb is creates comparative and superlative degree, or even if it creates adjectival forms in comparative and superlative degree, they will be found in the resulting dictionary.
 
         :return: A dictionary always with an ADV key, and if it's an adverb that creates comparative or/and superlative degree, there are also additional forms under COMP_ADV, SUPERL_ADV, COMP, SUPERL keys.
         :rtype: dict
         """
         if self.adverb in irregular_adv:
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/article/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/article/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from modern_greek_accentuation.accentuation import convert_to_monotonic
 
 from ..resources.article import definite_article, indefinite_article
-from ..resources.typing import declension_forms_type
+from ..resources.typing import genders_declensions_type, adj_declension_degree_type
 
 
 class Article:
     """
     This class creates article, it is an overkill, since it returns already created inflected forms, but added
     for the sake of completion of the API. Instantiate it with one of the articles (has to be nominative singular masculine)
 
@@ -13,15 +13,15 @@
     :type article: str
     """
     def __init__(self, article: str):
 
         article = convert_to_monotonic(article)
         self.article = article
 
-    def all(self) -> declension_forms_type:
+    def all(self) -> adj_declension_degree_type:
         """
         It returns a dictionary with inflected article forms
 
         :return: A dictionary of the folloing shape ``{SG: {MASC: {NOM: set(forms), ...}, ...}, ...}``
         :rtype: dict
         """
         if self.article not in ['ο', 'ένας']:
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from .create_noun_basic import create_all_basic_forms
 from .create_noun_decl import create_all_noun_forms
 from modern_greek_inflexion.verb.helpers import merging_all_dictionaries
 from modern_greek_accentuation.accentuation import convert_to_monotonic
-from ..resources.typing import genderType, noun_basic_forms, declension_forms_type
+from ..resources.typing import genderType, noun_basic_forms, genders_declensions_type
 
 
 class Noun:
     """
     This class can be used to create noun inflected forms.
 
     :param noun: A noun in nom sg, or, if it's an only plural noun, then in nom pl
@@ -32,15 +32,15 @@
         self.noun = convert_to_monotonic(noun, one_syllable_rule=False)
         self.proper_name = proper_name
         if not basic_forms:
             self.basic_forms = create_all_basic_forms(noun, gender=gender, proper_name=proper_name, aklito=aklito)
         else:
             self.basic_forms = basic_forms
 
-    def all(self) -> declension_forms_type:
+    def all(self) -> genders_declensions_type:
 
         """
         Create all the inflected forms as a dictionary
 
         :return: A dictionary with the following shape: ``{SG: {MASC: {NOM: set(forms), ...}, ...}``
         :rtype: dict
         """
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/create_noun_basic.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/create_noun_basic.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/noun/create_noun_decl.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/noun/create_noun_decl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from modern_greek_accentuation.accentuation import where_is_accent, put_accent, count_syllables, remove_all_diacritics
 from modern_greek_accentuation.resources import vowels
 from ..resources import greek_corpus
-from ..resources.typing import declension_forms_type, genderBasicType
+from ..resources.typing import genders_declensions_type, genderBasicType
 from ..resources.variables import *
 from ..resources.noun import irregular_gen_sg, irregular_voc_sg, noun_grammar_lists
 
 
 def create_all_noun_forms(nom_sg: str, gen_sg: str, nom_pl: str, genders: list[genderBasicType],
-                          proper_name: bool = False) -> declension_forms_type:
+                          proper_name: bool = False) -> genders_declensions_type:
     """
     :param nom_sg: nominative singular
     :param gen_sg: genitive singular
     :param nom_pl: nominative plural
     :param genders: a list with gender variables (FEM, MASC, NEUT)
     :param proper_name: flag useful for creation of vocatives in proper names
     :return: A dictionary {MASC: {SG: {NOM: str, ...}, ...}, ...}
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..adjective import Adjective
 from ..noun import Noun
 from ..resources import greek_pattern
 from ..resources.numerals import cardinal_irregulars
 from ..resources.variables import ADJ, ADV
 from modern_greek_accentuation.accentuation import convert_to_monotonic
 from ..exceptions import NotInGreekException
-from ..resources.typing import declension_forms_type
+from ..resources.typing import genders_declensions_type
 
 
 class Numeral:
     """
     This class can be used to create inflected forms of numerals. Most numerals behave like adjectives, but there are also ones, that can be viewed as nouns, because of that you should supply this info during instantiation, but you can also hope that it will be correctly guessed by algorithm.
 
     :param numeral: nominative singular or plural
@@ -26,16 +26,16 @@
 
         numeral = convert_to_monotonic(numeral, one_syllable_rule=False)
         if not greek_pattern.match(numeral):
             raise NotInGreekException
         self.numeral = numeral
         self.pos = pos
 
-    def all(self) -> {ADJ: declension_forms_type, ADV: set[str], COMP: declension_forms_type, COMP_ADV: set[str],
-                      SUPERL: declension_forms_type, SUPERL_ADV: set[str]} | declension_forms_type:
+    def all(self) -> {ADJ: genders_declensions_type, ADV: set[str], COMP: genders_declensions_type, COMP_ADV: set[str],
+                      SUPERL: genders_declensions_type, SUPERL_ADV: set[str]} | genders_declensions_type:
         """
         This method will create all the inflected forms.
 
         :return: If numeral is of noun type it returns a dictionary of the following shape ``{SG: {MASC: {NOM: set(forms), ...}, ...}``, but if the numeral is of adjective type it returns a dictionary of this shape ''{ADJ: {SG: {MASC: {NOM: set(forms), ...}, ...}}''
         "rtype: dict
         """
         if self.pos == ADJ:
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/create_num_decl.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/create_num_decl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import copy
 
 from modern_greek_accentuation.accentuation import put_accent_on_the_penultimate, where_is_accent, \
     put_accent_on_the_ultimate
 from ..adjective import create_all_adj_forms
 from ..resources.adj import adj_basic_template
-from ..resources.typing import declension_forms_type
+from ..resources.typing import genders_declensions_type
 from ..resources.variables import SG, PL, NOM, GEN, ACC, VOC, FEM, MASC, NEUT, ANTEPENULTIMATE, ULTIMATE
 from ..resources import greek_corpus
 
 
-def create_all_num_adj_forms(num_base_forms: str, cardinal: bool = False) -> declension_forms_type:
+def create_all_num_adj_forms(num_base_forms: str, cardinal: bool = False) -> genders_declensions_type:
     """
     :param cardinal: boolean
     :param num_base_forms: str "masc/fem/neut"
     :return: a dictionary of forms {SG: {MASC: {NOM: set(forms), ...}, ...}
     """
     if cardinal:
         all_forms = create_all_adj_forms(num_base_forms)
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/numeral/create_num_list.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/numeral/create_num_list.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from .create_pron_basic import create_basic_forms
 from .create_pron_decl import create_all_pron_forms
 from modern_greek_accentuation.accentuation import convert_to_monotonic
 
-from ..resources.typing import declension_forms_type
+from ..resources.typing import genders_declensions_type
 
 
 class Pronoun:
     """
     This class can be used to create pronouns
 
     :param pronoun: Has to be nominative singular masculine, if it's an adjectival pronoun, otherwise, if adverbial, there is only one form.
     :type pronoun: str
     :param strong: Applicable only for personal pronouns, which can be strong or weak, defaults to True.
     :type strong: bool, optional
     """
     def __init__(self, pronoun: str, strong: bool = True):
 
-        pron = convert_to_monotonic(pronoun, one_syllable_rule=False)
+        pronoun = convert_to_monotonic(pronoun, one_syllable_rule=False)
         self.pronoun = pronoun
         self.strong = strong
 
-    def all(self) -> declension_forms_type:
+    def all(self) -> genders_declensions_type:
         """
         This method should be used to generate all the inflected forms
 
         :return: A dictionary with the following shape ``{SG: {MASC: {NOM: set(forms), ...}, ...}``. If the pronoun is adverbial, the shape is the same, but the values of grammatical variables are all 'nd': ``{'nd': {'nd': {'nd': {'πού'}}}}``
         :rtype: dict
         """
         bas_form = create_basic_forms(self.pronoun)
+
         return create_all_pron_forms(bas_form, strong=self.strong)
+
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/create_pron_basic.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/create_pron_basic.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/pronoun/create_pron_decl.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/pronoun/create_pron_decl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from modern_greek_accentuation.accentuation import put_accent, where_is_accent
 
 from ..adjective import create_all_adj_forms
 from modern_greek_inflexion.verb.helpers import merging_all_dictionaries
 from ..resources.pronouns import *
 from ..resources import greek_corpus
-from ..resources.typing import declension_forms_type
+from ..resources.typing import genders_declensions_type
 from ..resources.variables import MASC, FEM, NEUT, SG, PL, ACC, NOM, GEN, VOC, ND
 
 
-def remove_vocatives(forms: declension_forms_type) -> declension_forms_type:
+def remove_vocatives(forms: genders_declensions_type) -> genders_declensions_type:
     """
     Removes vocatives, if a pronoun doesn't actually create vocatives
     :param forms: A dictionary {SG: {MASC: {NOM: set(forms), ...}, ...}
     :return: A dictionary {SG: {MASC: {NOM: set(forms), ...}, ...}
     """
     for number in forms:
         for gender in forms[number]:
             for case in forms[number][gender]:
 
                 if case == VOC:
                     forms[number][gender][case] = ''
     return forms
 
 
-def create_all_pron_forms(bas_forms: str, strong: bool = True) -> declension_forms_type:
+def create_all_pron_forms(bas_forms: str, strong: bool = True) -> genders_declensions_type:
     """
 
     :param bas_forms: str "masc/fem/neut"
     :param strong: if false, creates week pronouns
     :return: A dictionary {SG: {MASC: {NOM: set(forms), ...}, ...}
     """
     # forms: dic FEM, MASC, neut', if not inflected forms is a string
@@ -236,20 +236,20 @@
                 forms = ESU_STRONG
             else:
                 forms = ESU_WEAK
 
         elif masc == 'αλλήλων':
             forms = {PL: {
                 MASC: {
-                    GEN: 'αλλήλων',
-                    ACC: 'αλλήλους'
+                    GEN: {'αλλήλων'},
+                    ACC: {'αλλήλους'}
                 },
                 FEM: {
-                    GEN: 'αλλήλων',
-                    ACC: 'αλλήλες'
+                    GEN: {'αλλήλων'},
+                    ACC: {'αλλήλες'}
                 },
             }}
             return forms
 
         elif masc in ['όπερ', 'τουθόπερ', 'ό']:
 
             forms = {SG: {
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/adj.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/adj.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/article.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/article.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/el_GR.pickle` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/el_GR.pickle`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/noun.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/noun.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/numerals.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/numerals.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/prefixes.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/prefixes.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/pronouns.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/pronouns.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/typing.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/typing.py`

 * *Files 24% similar despite different names*

```diff
@@ -87,23 +87,32 @@
 
 
 class Tenses(Enum):
     FIN = FIN
     PAST = PAST
 
 
+cases_type = {NOM: set[str], VOC: set[str], ACC: set[str], GEN: set[str]}
+
+# adjective, pronouns itp
+
+genders_adj_type = {MASC: cases_type, FEM: cases_type, NEUT: cases_type}
+
+adj_declension_degree_type = {SG: genders_adj_type, PL: genders_adj_type}
+
+adj_basic_forms_type = {ADJ: str, COMPARATIVE: str, ADVERB: str, ADVERB_COMPARATIVE: str}
+
+
 tenseType = NewType("tenseType", Tenses)
 
 cases = {NOM: set[str], VOC: set[str], ACC: set[str], GEN: set[str]}
 
 numbers = {SG: cases, PL: cases}
 
-declension_forms_type = {FEM: numbers, MASC: numbers, NEUT: numbers}
-
-adjective_basic_forms = {ADJ: str, COMPARATIVE: str, ADVERB: str, ADVERB_COMPARATIVE: str}
+genders_declensions_type = {FEM: numbers, MASC: numbers, NEUT: numbers}
 
 noun_basic_forms = {NOM_SG: str, GEN_SG: str, NOM_PL: str, GENDERS: list[genderType], PROPER_NAME: bool}
 
 recognized_conjugation_type = {ASPECT: aspectType, VOICE: voiceType, TENSE: tenseType,
                                ROOT: str, CONJUGATION_IND: str, CONJUGATION_IMP: str, CONJUGATION_PART: str}
 
 basic_forms_type = {ACT_PRES_PARTICIPLE: set[str],
@@ -121,31 +130,11 @@
 
 personal_forms_type = {SG: {PRI: set[str], SEC: set[str], TER: set[str]},
                        PL: {PRI: set[str], SEC: set[str], TER: set[str]}}
 
 voice_forms_imp_type = {ACTIVE: {IND: personal_forms_type, IMP: personal_forms_type}, PASSIVE: {IND: personal_forms_type, IMP: personal_forms_type}}
 voice_forms_type = {ACTIVE: {IND: personal_forms_type}, PASSIVE: {IND: personal_forms_type}}
 
-participles_type = {ARCH_ACT_PRES_PARTICIPLE: declension_forms_type, PASSIVE_PERFECT_PARTICIPLE: declension_forms_type, PASS_PRES_PARTICIPLE: declension_forms_type, ACTIVE_AORIST_PARTICIPLE: declension_forms_type, PASSIVE_AORIST_PARTICIPLE: declension_forms_type, ACT_PRES_PARTICIPLE: set[str]}
-
+participles_type = {ARCH_ACT_PRES_PARTICIPLE: genders_declensions_type, PASSIVE_PERFECT_PARTICIPLE: genders_declensions_type, PASS_PRES_PARTICIPLE: genders_declensions_type, ACTIVE_AORIST_PARTICIPLE: genders_declensions_type, PASSIVE_AORIST_PARTICIPLE: genders_declensions_type, ACT_PRES_PARTICIPLE: set[str]}
 
 
-# adjective_type = dict[]
 
-# ADJ: masc, fem, neut
-# forms as a
-# string
-# divided
-# with / ('ωραίος/ωραία/ωραίο') if alternatives, they are added and
-# separated
-# with a coma
-# COMPARATIVE:
-# if exists in form parathetiko + ',' + alt_parathetiko + '/' + uperthetiko + ',' + alt_uperthetiko with
-# form
-# only in masc
-# sing
-# nom
-# ADVERB: adverb
-# form,
-# if alternatives, then separated with coma
-# ADVERB_COMPARATIVE:
-# if exists, adverb_parathetiko + ',' + alt_adverb_parathetiko + '/' + adverb_uperthetiko + ',' + alt_adverb_uperthetiko
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/variables.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/variables.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/resources/verb.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/resources/verb.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/__init__.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     create_all_past_personal_forms
 from modern_greek_inflexion.adjective.all.create_all_adj import create_all_adj_forms
 from modern_greek_inflexion.verb.helpers import merging_all_dictionaries, dict_of_dicts_merge
 
 from modern_greek_inflexion.verb.create.forms.basic.create_basic_all_forms import create_all_basic_forms
 from modern_greek_accentuation.accentuation import convert_to_monotonic
 from ..resources.typing import basic_forms_type, voice_forms_imp_type, voice_forms_type, participles_type, \
-    declension_forms_type
+    genders_declensions_type
 from ..resources.variables import *
 from modern_greek_inflexion.resources import greek_pattern
 from modern_greek_inflexion.exceptions import NotInGreekException
 
 
 class Verb:
     """
@@ -174,15 +174,15 @@
                     else:
                         res = merging_all_dictionaries(res[0], res[0])
                     participles_of_type.append(res)
 
                 participles[participle_type] = merging_all_dictionaries(*participles_of_type)
         return participles
 
-    def all(self) -> {PRESENT: voice_forms_imp_type, CONJUNCTIVE: voice_forms_imp_type, PARATATIKOS: voice_forms_type, AORIST: voice_forms_type, ARCH_ACT_PRES_PARTICIPLE: declension_forms_type, PASSIVE_PERFECT_PARTICIPLE: declension_forms_type, PASS_PRES_PARTICIPLE: declension_forms_type, ACTIVE_AORIST_PARTICIPLE: declension_forms_type, PASSIVE_AORIST_PARTICIPLE: declension_forms_type, ACT_PRES_PARTICIPLE: set[str]}:
+    def all(self) -> {PRESENT: voice_forms_imp_type, CONJUNCTIVE: voice_forms_imp_type, PARATATIKOS: voice_forms_type, AORIST: voice_forms_type, ARCH_ACT_PRES_PARTICIPLE: genders_declensions_type, PASSIVE_PERFECT_PARTICIPLE: genders_declensions_type, PASS_PRES_PARTICIPLE: genders_declensions_type, ACTIVE_AORIST_PARTICIPLE: genders_declensions_type, PASSIVE_AORIST_PARTICIPLE: genders_declensions_type, ACT_PRES_PARTICIPLE: set[str]}:
         """
         This method will create all inflected forms
 
         :return: A dictionary with personal forms and with participles
         :rtype: dict
         """
         result = self.create_imperfect_forms()
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/helpers.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/helpers.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/PKG-INFO` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-greek-inflexion
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python 3 library for creating inflected forms given basic forms of Modern Greek words
 Home-page: https://github.com/PicusZeus/modern-greek-inflexion
 Author: Krzysztof H
 Author-email: krzysztof.hilman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -43,27 +43,28 @@
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install modern-greek-inflexion.
 
 ```bash
 pip install modern-greek-inflexion
 ```
 
 ## Usage
-You can read the docs [here](https://github.com/PicusZeus/modern-greek-inflexion.git)
+You can read the docs [here](https://modern-greek-inflexion.readthedocs.io/en/latest/)
 
 ## Unittests
 run 
 >python -m unittest
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
  * 1.0.4 Added logic for multiple root formation in verbs on -άρω (σοκάρω, σοκαρίζω, σοκαρίσω), now the app will try to create also imperfect forms with a root on 'ιζ'. The Experiment with extending the core language check corpus failed miserably, as all the corpora I tried (even these from the EU) are unfortunately full of typos and orthographic errors, which, when used, introduced into the app huge problems. Next time I will try to use some NLTK magic and frequency lists to try them again.
  * 1.0.3 The problem with verbs with prefix para fixed by adding a flag to verb.create_all_forms para. If there is possibility, that there are two different verbs (like παραβλέπω/παραβλέψω and παραβλέπω/παραδώ), you have to set flag para to True. Fixed issue with non existent imper aor sg of compound verbs with βαίνω (like παρεμβαίνω).
  * 1.0.2 Updated list of irregular past passive participles, deleted most of them as they're not needed anymore and in places they would cause incorrect participle formation.
  * 1.0.1 Project is mature enough, some issue with dependency accentuation module fixed.
```

### Comparing `modern-greek-inflexion-2.0.0/src/modern_greek_inflexion.egg-info/SOURCES.txt` & `modern-greek-inflexion-2.0.1/src/modern_greek_inflexion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

