# Comparing `tmp/hmeg-0.1.1.tar.gz` & `tmp/hmeg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmeg-0.1.1.tar", max compression
+gzip compressed data, was "hmeg-0.1.2.tar", max compression
```

## Comparing `hmeg-0.1.1.tar` & `hmeg-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,76 @@
--rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.1/LICENSE
--rw-r--r--   0        0        0     4392 2024-03-30 12:01:08.301249 hmeg-0.1.1/README.md
--rw-r--r--   0        0        0      137 2024-03-30 12:13:29.628059 hmeg-0.1.1/hmeg/__init__.py
--rw-r--r--   0        0        0     2345 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/entities.py
--rw-r--r--   0        0        0     1534 2024-03-30 12:01:08.301249 hmeg-0.1.1/hmeg/exercise_generator.py
--rw-r--r--   0        0        0      178 2024-03-21 21:48:31.789981 hmeg-0.1.1/hmeg/inflections.py
--rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/ab.toml
--rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/cd.toml
--rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/efg.toml
--rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/h.toml
--rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/ikl.toml
--rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/mn.toml
--rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/opr.toml
--rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/stu.toml
--rw-r--r--   0        0        0     2146 2024-03-30 08:41:48.508255 hmeg-0.1.1/hmeg/miniphrase/wy.toml
--rw-r--r--   0        0        0      905 2024-03-30 12:17:59.185087 hmeg-0.1.1/hmeg/registry.py
--rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.1/hmeg/topics/1_basic_present_tense.toml
--rw-r--r--   0        0        0      296 2024-03-10 07:44:10.147484 hmeg-0.1.1/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
--rw-r--r--   0        0        0      325 2024-03-24 12:49:15.051567 hmeg-0.1.1/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
--rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.1/hmeg/topics/1_i_want_to.toml
--rw-r--r--   0        0        0      415 2024-03-10 07:44:10.147484 hmeg-0.1.1/hmeg/topics/1_negative_sentenses.toml
--rw-r--r--   0        0        0      233 2024-03-10 07:44:10.151485 hmeg-0.1.1/hmeg/topics/1_past_tense.toml
--rw-r--r--   0        0        0      161 2024-03-10 07:44:10.151485 hmeg-0.1.1/hmeg/topics/1_please_give_me.toml
--rw-r--r--   0        0        0      224 2024-03-24 12:49:15.051567 hmeg-0.1.1/hmeg/topics/1_this_is.toml
--rw-r--r--   0        0        0      165 2024-03-10 07:44:10.151485 hmeg-0.1.1/hmeg/topics/1_topic_subject_particle.toml
--rw-r--r--   0        0        0      327 2024-03-10 07:44:10.151485 hmeg-0.1.1/hmeg/topics/1_what_do_you_want_to_do.toml
--rw-r--r--   0        0        0      230 2024-03-14 13:30:47.048412 hmeg-0.1.1/hmeg/topics/2_and_and_then_therefore_so.toml
--rw-r--r--   0        0        0      154 2024-03-14 13:33:59.925728 hmeg-0.1.1/hmeg/topics/2_and_with.toml
--rw-r--r--   0        0        0      288 2024-03-14 13:39:48.992097 hmeg-0.1.1/hmeg/topics/2_but_however.toml
--rw-r--r--   0        0        0      250 2024-03-14 13:49:14.375934 hmeg-0.1.1/hmeg/topics/2_can_cannot.toml
--rw-r--r--   0        0        0      152 2024-03-15 14:01:09.329766 hmeg-0.1.1/hmeg/topics/2_dont_do_it.toml
--rw-r--r--   0        0        0      242 2024-03-14 13:27:05.334892 hmeg-0.1.1/hmeg/topics/2_future_tense.toml
--rw-r--r--   0        0        0      281 2024-03-21 21:46:08.368116 hmeg-0.1.1/hmeg/topics/2_have_to_should_must.toml
--rw-r--r--   0        0        0      185 2024-03-15 13:48:12.447505 hmeg-0.1.1/hmeg/topics/2_if_in_case.toml
--rw-r--r--   0        0        0      138 2024-03-15 13:50:12.715855 hmeg-0.1.1/hmeg/topics/2_imperative.toml
--rw-r--r--   0        0        0      183 2024-03-15 13:59:28.597472 hmeg-0.1.1/hmeg/topics/2_particles_for_method_way.toml
--rw-r--r--   0        0        0      158 2024-03-15 13:51:16.464040 hmeg-0.1.1/hmeg/topics/2_please_do_it_for_me.toml
--rw-r--r--   0        0        0      251 2024-03-14 13:46:29.870818 hmeg-0.1.1/hmeg/topics/2_present_progressive.toml
--rw-r--r--   0        0        0      294 2024-03-14 13:51:21.940821 hmeg-0.1.1/hmeg/topics/2_to_be_good_poor_at.toml
--rw-r--r--   0        0        0      288 2024-03-14 13:56:35.319010 hmeg-0.1.1/hmeg/topics/2_to_like.toml
--rw-r--r--   0        0        0      354 2024-03-10 07:43:30.163214 hmeg-0.1.1/hmeg/topics/9_while.toml
--rw-r--r--   0        0        0     4926 2024-03-30 12:19:52.689521 hmeg-0.1.1/hmeg/utils.py
--rw-r--r--   0        0        0     3943 2024-03-30 12:01:08.301249 hmeg-0.1.1/hmeg/vocabs/minilex.toml
--rw-r--r--   0        0        0     3663 2024-03-30 12:19:37.741464 hmeg-0.1.1/hmeg/vocabulary.py
--rw-r--r--   0        0        0      483 2024-03-30 12:21:50.805971 hmeg-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 hmeg-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-01 07:41:02.775209 hmeg-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4437 2024-04-06 02:54:50.998893 hmeg-0.1.2/README.md
+-rw-r--r--   0        0        0      137 2024-03-31 04:16:50.659172 hmeg-0.1.2/hmeg/__init__.py
+-rw-r--r--   0        0        0     2345 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/entities.py
+-rw-r--r--   0        0        0     1566 2024-04-04 12:43:38.812500 hmeg-0.1.2/hmeg/exercise_generator.py
+-rw-r--r--   0        0        0     1500 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/ab.toml
+-rw-r--r--   0        0        0     1782 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/cd.toml
+-rw-r--r--   0        0        0     1897 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/efg.toml
+-rw-r--r--   0        0        0     1384 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/h.toml
+-rw-r--r--   0        0        0     1631 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/ikl.toml
+-rw-r--r--   0        0        0     1809 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/mn.toml
+-rw-r--r--   0        0        0     1216 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/opr.toml
+-rw-r--r--   0        0        0     3075 2024-03-30 08:41:48.508255 hmeg-0.1.2/hmeg/miniphrase/stu.toml
+-rw-r--r--   0        0        0     2146 2024-04-01 23:25:07.107024 hmeg-0.1.2/hmeg/miniphrase/wy.toml
+-rw-r--r--   0        0        0     1682 2024-04-02 00:34:59.871652 hmeg-0.1.2/hmeg/registry.py
+-rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_basic_present_tense.toml
+-rw-r--r--   0        0        0      296 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_from_a_to_b_from_c_until_d.toml
+-rw-r--r--   0        0        0      325 2024-03-24 12:49:15.051567 hmeg-0.1.2/hmeg/topics/1_have_dont_have_there_is_there_isnt.toml
+-rw-r--r--   0        0        0      290 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_i_want_to.toml
+-rw-r--r--   0        0        0      415 2024-03-10 07:44:10.147484 hmeg-0.1.2/hmeg/topics/1_negative_sentenses.toml
+-rw-r--r--   0        0        0      233 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_past_tense.toml
+-rw-r--r--   0        0        0      161 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_please_give_me.toml
+-rw-r--r--   0        0        0      224 2024-03-24 12:49:15.051567 hmeg-0.1.2/hmeg/topics/1_this_is.toml
+-rw-r--r--   0        0        0      165 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_topic_subject_particle.toml
+-rw-r--r--   0        0        0      327 2024-03-10 07:44:10.151485 hmeg-0.1.2/hmeg/topics/1_what_do_you_want_to_do.toml
+-rw-r--r--   0        0        0      230 2024-03-14 13:30:47.048412 hmeg-0.1.2/hmeg/topics/2_and_and_then_therefore_so.toml
+-rw-r--r--   0        0        0      154 2024-03-14 13:33:59.925728 hmeg-0.1.2/hmeg/topics/2_and_with.toml
+-rw-r--r--   0        0        0      288 2024-03-14 13:39:48.992097 hmeg-0.1.2/hmeg/topics/2_but_however.toml
+-rw-r--r--   0        0        0      250 2024-03-14 13:49:14.375934 hmeg-0.1.2/hmeg/topics/2_can_cannot.toml
+-rw-r--r--   0        0        0      152 2024-03-15 14:01:09.329766 hmeg-0.1.2/hmeg/topics/2_dont_do_it.toml
+-rw-r--r--   0        0        0      242 2024-03-14 13:27:05.334892 hmeg-0.1.2/hmeg/topics/2_future_tense.toml
+-rw-r--r--   0        0        0      281 2024-03-21 21:46:08.368116 hmeg-0.1.2/hmeg/topics/2_have_to_should_must.toml
+-rw-r--r--   0        0        0      185 2024-03-15 13:48:12.447505 hmeg-0.1.2/hmeg/topics/2_if_in_case.toml
+-rw-r--r--   0        0        0      138 2024-03-15 13:50:12.715855 hmeg-0.1.2/hmeg/topics/2_imperative.toml
+-rw-r--r--   0        0        0      183 2024-03-15 13:59:28.597472 hmeg-0.1.2/hmeg/topics/2_particles_for_method_way.toml
+-rw-r--r--   0        0        0      173 2024-04-02 00:34:59.871652 hmeg-0.1.2/hmeg/topics/2_please_do_it_for_me.toml
+-rw-r--r--   0        0        0      251 2024-03-14 13:46:29.870818 hmeg-0.1.2/hmeg/topics/2_present_progressive.toml
+-rw-r--r--   0        0        0      294 2024-03-14 13:51:21.940821 hmeg-0.1.2/hmeg/topics/2_to_be_good_poor_at.toml
+-rw-r--r--   0        0        0      288 2024-03-14 13:56:35.319010 hmeg-0.1.2/hmeg/topics/2_to_like.toml
+-rw-r--r--   0        0        0      152 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_after_ing.toml
+-rw-r--r--   0        0        0      209 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_approximately_about.toml
+-rw-r--r--   0        0        0      156 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_before_ing.toml
+-rw-r--r--   0        0        0      167 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_but_still_nevertheless.toml
+-rw-r--r--   0        0        0      166 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_even_if_even_though.toml
+-rw-r--r--   0        0        0      284 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_in_front_of_behind.toml
+-rw-r--r--   0        0        0      215 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_in_order_to_for_the_sake_of.toml
+-rw-r--r--   0        0        0      204 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_linking_verbs_고.toml
+-rw-r--r--   0        0        0      165 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_linking_verbs_여서.toml
+-rw-r--r--   0        0        0      256 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_linking_words_는데.toml
+-rw-r--r--   0        0        0      339 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_maybe_i_might.toml
+-rw-r--r--   0        0        0      289 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_nothing_but_only.toml
+-rw-r--r--   0        0        0      241 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_shall_we_i_wonder.toml
+-rw-r--r--   0        0        0      198 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_to_look_like_seem_like.toml
+-rw-r--r--   0        0        0      166 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_too_much_very.toml
+-rw-r--r--   0        0        0      159 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_verb_ending_네요.toml
+-rw-r--r--   0        0        0      371 2024-04-05 00:05:12.018851 hmeg-0.1.2/hmeg/topics/3_well_then_in_that_case.toml
+-rw-r--r--   0        0        0      284 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_among_between.toml
+-rw-r--r--   0        0        0      168 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_do_you_want_to.toml
+-rw-r--r--   0        0        0      511 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_i_think_past_future.toml
+-rw-r--r--   0        0        0      293 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_it_cant_be.toml
+-rw-r--r--   0        0        0      439 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_it_is_ok_to.toml
+-rw-r--r--   0        0        0      281 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_less_not_completely.toml
+-rw-r--r--   0        0        0      314 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_most_best.toml
+-rw-r--r--   0        0        0      190 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_much_more_much_less.toml
+-rw-r--r--   0        0        0      343 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_the_more_the_more.toml
+-rw-r--r--   0        0        0      224 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_to_become_adj.toml
+-rw-r--r--   0        0        0      371 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_to_gradually_get_to_do.toml
+-rw-r--r--   0        0        0      339 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_to_try_doing_something.toml
+-rw-r--r--   0        0        0      247 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_verb_ending_지_죠.toml
+-rw-r--r--   0        0        0      413 2024-04-06 02:54:50.998893 hmeg-0.1.2/hmeg/topics/4_you_should_not.toml
+-rw-r--r--   0        0        0      354 2024-03-10 07:43:30.163214 hmeg-0.1.2/hmeg/topics/9_while.toml
+-rw-r--r--   0        0        0     3195 2024-04-01 23:25:07.107024 hmeg-0.1.2/hmeg/utils.py
+-rw-r--r--   0        0        0     3943 2024-03-30 12:01:08.301249 hmeg-0.1.2/hmeg/vocabs/minilex.toml
+-rw-r--r--   0        0        0     4953 2024-04-01 23:25:07.107024 hmeg-0.1.2/hmeg/vocabulary.py
+-rw-r--r--   0        0        0      482 2024-04-06 02:56:59.567357 hmeg-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 hmeg-0.1.2/PKG-INFO
```

### Comparing `hmeg-0.1.1/LICENSE` & `hmeg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/README.md` & `hmeg-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 ```
 
 * Run with custom topic and number of exercises
 ```bash
 python hmeg_cli.py run -n 15 -t "Have, Don’t have, There is, There isn’t / 있어요, 없어요"
 ```
 
+* You can use partial name of the topic. In that case all topics, that contain the specified string will be used.
+```bash
+python hmeg_cli.py run -n 15 -t "있어요, 없어요"
+python hmeg_cli.py run -n 15 -t "there is"
+```
+
 * List available topics described in the specified configuration file (optional)
 ```bash
 python hmeg_cli.py list -c hmeg.conf
 ```
 
 * Print help for the arguments or specific command
 
@@ -46,27 +52,26 @@
 python hmeg_cli.py run --help
 python hmeg_cli.py list --help
 ```
 
 ## Python code
 
 ```python
-from hmeg import utils, Vocabulary, ExerciseGenerator
+from hmeg import utils, ExerciseGenerator, load_minilex
+
 
-topics_folder = "hmeg/topics/"  # folder containing description of exercises for different grammar topics.
-vocab_file = "hmeg/vocabs/minilex.toml"  # file with vocabulary for generation of exercises.
 num_exercises = 10  # number of randomly generated exercises for selected topic
 
-utils.register_grammar_topics(topics_folder)
-vocab = Vocabulary.load(vocab_file)
+utils.register_grammar_topics()
+vocab = load_minilex()  # load words from the Minilex.
 
 exercises = ExerciseGenerator.generate_exercises(
     topic_name="While / -(으)면서", num=num_exercises, vocab=vocab
 )
-print(exercises)
+print("\n".join(exercises))
 ```
 
 # Format of exercises and vocabulary
 
 The library supports extensible and configurable templates for generation of exercises
 as well as customizable vocabulary.
```

### Comparing `hmeg-0.1.1/hmeg/entities.py` & `hmeg-0.1.2/hmeg/entities.py`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/exercise_generator.py` & `hmeg-0.1.2/hmeg/exercise_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         The results are represented as templates with placeholders for nouns, verbs, ....
 
         See also: `apply_vocabulary`
         """
         vocab = vocab or Vocabulary.load(DEFAULT_VOCABULARY_FILE)
 
         if topic_name not in GrammarRegistry.topics:
-            raise RuntimeError(f"Requested an unregistered topic: {topic_name}. Please check the topics' folder.")
+            raise RuntimeError(f"Requested an unregistered topic: {topic_name}. Please run `python hmeg_cli.py list` to see the existing topics.")
 
         templates = []
         for exercise_type in GrammarRegistry.topics[topic_name].exercises:
             cur_grammar = CFG.fromstring(exercise_type)
             templates.extend(generate(cur_grammar, n=num))
 
         res = []
```

### Comparing `hmeg-0.1.1/hmeg/miniphrase/ab.toml` & `hmeg-0.1.2/hmeg/miniphrase/ab.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/cd.toml` & `hmeg-0.1.2/hmeg/miniphrase/cd.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/efg.toml` & `hmeg-0.1.2/hmeg/miniphrase/efg.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/h.toml` & `hmeg-0.1.2/hmeg/miniphrase/h.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/ikl.toml` & `hmeg-0.1.2/hmeg/miniphrase/ikl.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/mn.toml` & `hmeg-0.1.2/hmeg/miniphrase/mn.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/opr.toml` & `hmeg-0.1.2/hmeg/miniphrase/opr.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/stu.toml` & `hmeg-0.1.2/hmeg/miniphrase/stu.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/hmeg/miniphrase/wy.toml` & `hmeg-0.1.2/hmeg/miniphrase/wy.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """,
     """
     S -> P 'wants him to do it.'
     P -> 'He' | 'She' | 'It'
     """,
     """
     S -> 'Which way should' P 'go?'
-    P -> 'I' | 'He' | 'She' | 'It' | 'They'
+    P -> 'I' | 'he' | 'she' | 'it' | 'they'
     """,
     """
     S -> 'Can you tell me the way to the {place}?\t' R
     R -> 'Straight on' | 'Go down the street and turn' RL
     RL -> 'right' | 'left'
     """,
     """
```

### Comparing `hmeg-0.1.1/hmeg/vocabs/minilex.toml` & `hmeg-0.1.2/hmeg/vocabs/minilex.toml`

 * *Files identical despite different names*

### Comparing `hmeg-0.1.1/PKG-INFO` & `hmeg-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: hmeg
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generator of exercises for practicing speaking for language learning.
 Home-page: https://github.com/yurytsoy/hmeg
 License: MIT
 Author: Yury Choi
 Author-email: yurytsoy@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.6.0,<0.7.0)
 Requires-Dist: inflect (>=7.0.0,<8.0.0)
 Requires-Dist: mlconjug3 (>=3.11.0,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
@@ -51,14 +53,20 @@
 ```
 
 * Run with custom topic and number of exercises
 ```bash
 python hmeg_cli.py run -n 15 -t "Have, Don’t have, There is, There isn’t / 있어요, 없어요"
 ```
 
+* You can use partial name of the topic. In that case all topics, that contain the specified string will be used.
+```bash
+python hmeg_cli.py run -n 15 -t "있어요, 없어요"
+python hmeg_cli.py run -n 15 -t "there is"
+```
+
 * List available topics described in the specified configuration file (optional)
 ```bash
 python hmeg_cli.py list -c hmeg.conf
 ```
 
 * Print help for the arguments or specific command
 
@@ -67,27 +75,26 @@
 python hmeg_cli.py run --help
 python hmeg_cli.py list --help
 ```
 
 ## Python code
 
 ```python
-from hmeg import utils, Vocabulary, ExerciseGenerator
+from hmeg import utils, ExerciseGenerator, load_minilex
+
 
-topics_folder = "hmeg/topics/"  # folder containing description of exercises for different grammar topics.
-vocab_file = "hmeg/vocabs/minilex.toml"  # file with vocabulary for generation of exercises.
 num_exercises = 10  # number of randomly generated exercises for selected topic
 
-utils.register_grammar_topics(topics_folder)
-vocab = Vocabulary.load(vocab_file)
+utils.register_grammar_topics()
+vocab = load_minilex()  # load words from the Minilex.
 
 exercises = ExerciseGenerator.generate_exercises(
     topic_name="While / -(으)면서", num=num_exercises, vocab=vocab
 )
-print(exercises)
+print("\n".join(exercises))
 ```
 
 # Format of exercises and vocabulary
 
 The library supports extensible and configurable templates for generation of exercises
 as well as customizable vocabulary.
```

