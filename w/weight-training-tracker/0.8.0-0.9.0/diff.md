# Comparing `tmp/weight_training_tracker-0.8.0.tar.gz` & `tmp/weight_training_tracker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weight_training_tracker-0.8.0.tar", last modified: Sat Mar  9 02:01:23 2024, max compression
+gzip compressed data, was "weight_training_tracker-0.9.0.tar", last modified: Thu Mar 14 01:27:24 2024, max compression
```

## Comparing `weight_training_tracker-0.8.0.tar` & `weight_training_tracker-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-09 02:01:23.849016 weight_training_tracker-0.8.0/
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      163 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/AUTHORS.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)     3725 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       89 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/HISTORY.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      262 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/MANIFEST.in
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)     1325 2024-03-09 02:01:23.849016 weight_training_tracker-0.8.0/PKG-INFO
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      423 2024-02-12 02:04:34.000000 weight_training_tracker-0.8.0/README.rst
-drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-09 02:01:23.839016 weight_training_tracker-0.8.0/docs/
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      624 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/Makefile
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       28 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/authors.rst
--rwxrwxr-x   0 sundaram  (1000) sundaram  (1000)     4998 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/conf.py
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       33 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/contributing.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       28 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/history.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      320 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/index.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)     1254 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/installation.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      821 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/make.bat
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       27 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/readme.rst
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      101 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/docs/usage.rst
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)      344 2024-02-12 02:01:08.000000 weight_training_tracker-0.8.0/pyproject.toml
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      395 2024-03-09 02:01:23.849016 weight_training_tracker-0.8.0/setup.cfg
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)     1571 2024-03-09 02:01:18.000000 weight_training_tracker-0.8.0/setup.py
-drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-09 02:01:23.839016 weight_training_tracker-0.8.0/tests/
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       53 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/tests/__init__.py
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      964 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/tests/test_weight_training_tracker.py
-drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-09 02:01:23.849016 weight_training_tracker-0.8.0/weight_training_tracker/
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      148 2024-02-12 02:04:20.000000 weight_training_tracker-0.8.0/weight_training_tracker/__init__.py
-drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-09 02:01:23.849016 weight_training_tracker-0.8.0/weight_training_tracker/conf/
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)    15888 2024-03-08 01:05:08.000000 weight_training_tracker-0.8.0/weight_training_tracker/conf/config.yaml
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)      598 2024-02-12 02:01:08.000000 weight_training_tracker-0.8.0/weight_training_tracker/console_helper.py
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)      530 2024-02-12 02:31:36.000000 weight_training_tracker-0.8.0/weight_training_tracker/constants.py
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)     7373 2024-02-12 02:01:08.000000 weight_training_tracker-0.8.0/weight_training_tracker/file_utils.py
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)    30379 2024-03-09 01:58:32.000000 weight_training_tracker-0.8.0/weight_training_tracker/main.py
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)     3150 2024-02-12 02:01:08.000000 weight_training_tracker-0.8.0/weight_training_tracker/system_caller.py
-drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-09 02:01:23.849016 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/
--rw-r--r--   0 sundaram  (1000) sundaram  (1000)     1325 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      915 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)        1 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       78 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/entry_points.txt
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)        1 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/not-zip-safe
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       51 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/requires.txt
--rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       24 2024-03-09 02:01:23.000000 weight_training_tracker-0.8.0/weight_training_tracker.egg-info/top_level.txt
+drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      163 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/AUTHORS.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)     3725 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       89 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/HISTORY.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      262 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/MANIFEST.in
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)     1325 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/PKG-INFO
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      423 2024-02-12 02:04:34.000000 weight_training_tracker-0.9.0/README.rst
+drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/docs/
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      624 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/Makefile
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       28 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/authors.rst
+-rwxrwxr-x   0 sundaram  (1000) sundaram  (1000)     4998 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/conf.py
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       33 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/contributing.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       28 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/history.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      320 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/index.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)     1254 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/installation.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      821 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/make.bat
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       27 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/readme.rst
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      101 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/docs/usage.rst
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)      344 2024-02-12 02:01:08.000000 weight_training_tracker-0.9.0/pyproject.toml
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      395 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/setup.cfg
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)     1571 2024-03-13 21:30:18.000000 weight_training_tracker-0.9.0/setup.py
+drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/tests/
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       53 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/tests/__init__.py
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      964 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/tests/test_weight_training_tracker.py
+drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/weight_training_tracker/
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      148 2024-02-12 02:04:20.000000 weight_training_tracker-0.9.0/weight_training_tracker/__init__.py
+drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/weight_training_tracker/conf/
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)    15888 2024-03-11 23:42:31.000000 weight_training_tracker-0.9.0/weight_training_tracker/conf/config.yaml
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)      598 2024-02-12 02:01:08.000000 weight_training_tracker-0.9.0/weight_training_tracker/console_helper.py
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)      530 2024-02-12 02:31:36.000000 weight_training_tracker-0.9.0/weight_training_tracker/constants.py
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)     7373 2024-02-12 02:01:08.000000 weight_training_tracker-0.9.0/weight_training_tracker/file_utils.py
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)    31297 2024-03-13 21:29:13.000000 weight_training_tracker-0.9.0/weight_training_tracker/main.py
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)     3150 2024-02-12 02:01:08.000000 weight_training_tracker-0.9.0/weight_training_tracker/system_caller.py
+drwxrwxr-x   0 sundaram  (1000) sundaram  (1000)        0 2024-03-14 01:27:24.898833 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/
+-rw-r--r--   0 sundaram  (1000) sundaram  (1000)     1325 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)      915 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)        1 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       78 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/entry_points.txt
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)        1 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/not-zip-safe
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       51 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/requires.txt
+-rw-rw-r--   0 sundaram  (1000) sundaram  (1000)       24 2024-03-14 01:27:24.000000 weight_training_tracker-0.9.0/weight_training_tracker.egg-info/top_level.txt
```

### Comparing `weight_training_tracker-0.8.0/CONTRIBUTING.rst` & `weight_training_tracker-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/PKG-INFO` & `weight_training_tracker-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weight_training_tracker
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple CLI-based app for tracking weight training.
 Home-page: https://github.com/jai-python3/weight-training-tracker
 Author: Jaideep Sundaram
 Author-email: jai.python3@gmail.com
 Keywords: weight-training-tracker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `weight_training_tracker-0.8.0/docs/Makefile` & `weight_training_tracker-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/docs/conf.py` & `weight_training_tracker-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/docs/installation.rst` & `weight_training_tracker-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/docs/make.bat` & `weight_training_tracker-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/setup.py` & `weight_training_tracker-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords='weight-training-tracker',
     name='weight_training_tracker',
     packages=find_packages(include=['weight_training_tracker', 'weight_training_tracker.*']),
     package_data={"weight_training_tracker": ["conf/config.yaml"]},
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/jai-python3/weight-training-tracker',
-    version='0.8.0',
+    version='0.9.0',
     zip_safe=False,
 )
```

### Comparing `weight_training_tracker-0.8.0/tests/test_weight_training_tracker.py` & `weight_training_tracker-0.9.0/tests/test_weight_training_tracker.py`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker/conf/config.yaml` & `weight_training_tracker-0.9.0/weight_training_tracker/conf/config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -49,54 +49,55 @@
           equipment: "dumbbells; bench 45 degrees"
           alternating_sides: true
           body_position: seated
         - name: "Seated Hammer Curls"
           equipment: "dumbbells; bench 45 degrees"
           alternating_sides: true
           body_position: seated
-        - name: "Bicep Throwbacks"
+        - name: "Dumbbell Curl - rest arm on upper part of inclined bench"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: standing
         - name: "Reverse Grip Dumbbell Bicep Curls"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: standing
         - name: "EZ bar Bicep Curl"
           equipment: "EZ barbell"
           alternating_sides: false
           body_position: standing
-        - name: "EZ bar Bicep Spider Curls"
-          equipment: "EZ barbell"
-          alternating_sides: false
-          body_position: leaning with chest on top of inclined bench
         - name: "Reverse Grip EZ bar Bicep Curl"
           equipment: "EZ barbell"
           alternating_sides: false
           body_position: standing
-        - name: "Dumbbell Curl - rest arm on upper part of inclined bench"
-          equipment: "dumbbells"
-          alternating_sides: true
-          body_position: standing
         - name: "Dumbbell Bicep Spider Curls"
           equipment: "dumbbells"
+          alternating_sides: true
+          body_position: leaning with chest on top of inclined bench
+        - name: "EZ bar Bicep Spider Curls"
+          equipment: "EZ barbell"
           alternating_sides: false
           body_position: leaning with chest on top of inclined bench
         - name: "Bench Dumbbell Curl - rest chest on upper part of inclined bench"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: standing
         - name: "Master Bicep Curl"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: standing
         - name: "Supinate Curl - all weight on one side"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: standing
+        - name: "Bicep Throwbacks"
+          equipment: "dumbbells"
+          alternating_sides: true
+          body_position: standing
+
     "Triceps":
       exercises:
         - name: "Bench Dips Tricep Extensions"
           equipment: "bench"
           alternating_sides: false
           body_position: standing
         - name: "Bent Over Single Arm Tricep Kickback"
@@ -107,26 +108,26 @@
           equipment: "dumbbells"
           alternating_sides: true
           body_position: lying on bench
         - name: "EZ Bar Skull Crusher Tricep Extensions"
           equipment: "EZ barbell"
           alternating_sides: false
           body_position: lying on bench
+        - name: "EZ Bar Overhead Tricep Extensions"
+          equipment: "EZ barbell"
+          alternating_sides: false
+          body_position: standing
         - name: "Dumbbell Skull Crusher Tricep Extensions"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: lying on bench
         - name: "Overhead Tricep Extensions"
           equipment: "dumbbells"
           alternating_sides: true
           body_position: standing
-        - name: "EZ Bar Overhead Tricep Extensions"
-          equipment: "EZ barbell"
-          alternating_sides: false
-          body_position: standing
     "Back: Reverse Flies":
       exercises:
         - name: "Single Arm Neutral Grip Standing Reverse Flies"
           equipment: "bench"
           alternating_sides: true
           body_position: standing
           instructions:
```

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker/console_helper.py` & `weight_training_tracker-0.9.0/weight_training_tracker/console_helper.py`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker/constants.py` & `weight_training_tracker-0.9.0/weight_training_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker/file_utils.py` & `weight_training_tracker-0.9.0/weight_training_tracker/file_utils.py`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker/main.py` & `weight_training_tracker-0.9.0/weight_training_tracker/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self.verbose = kwargs.get("verbose", constants.DEFAULT_VERBOSE)
 
         logging.info(f"Will load contents of the workout file '{self.config_file}'")
         self.config = yaml.safe_load(Path(self.config_file).read_text())
 
         self._load_functions()
 
+        self.workout_file_created_during_current_session = False
         self.is_file_backed_up = False
         self.current_option_number = 0
         self.selection_lookup = {}
 
 
         self._workout_session_start_time = None
         self._workout_session_end_time = None
@@ -748,54 +749,61 @@
                 pathlib.Path(outdir).mkdir(parents=True, exist_ok=True)
                 logging.info(f"Created directory '{outdir}'")
             outfile = os.path.join(outdir, f"{current_date}.yaml")
         else:
             outfile = self.outfile
 
         if os.path.exists(outfile):
-            if not self.is_file_backed_up:
-                timestamp = datetime.now().strftime("%Y-%m-%d-%H%M%S")
-                bakfile = f"{outfile}.{timestamp}.bak"
-                logging.info(f"Backing up '{outfile}' to '{bakfile}'")
-                os.rename(outfile, bakfile)
-                self.is_file_backed_up = True
+            if self.workout_file_created_during_current_session:
+                logging.info(f"Will not backup the workout file '{outfile}' as it was created during the current session")
+            else:
+                if not self.is_file_backed_up:
+                    timestamp = datetime.now().strftime("%Y-%m-%d-%H%M%S")
+                    bakfile = f"{outfile}.{timestamp}.bak"
+                    logging.info(f"Backing up '{outfile}' to '{bakfile}'")
+                    os.rename(outfile, bakfile)
+                    self.is_file_backed_up = True
 
         # Save the workout session to the workout file
         # Write the Python dictionary to a YAML file
         with open(outfile, "w") as file:
             documents = yaml.dump(self.config["current_workout"], file)
 
+        # The current workout file has just been created during this session.
+        self.workout_file_created_during_current_session = True
+
         console.print(f"Saved workout session to '{outfile}'")
         logging.info(f"Saved workout session to '{outfile}'")
 
     def _sleep_or_interrupt(self, timeout: int) -> None:
         print(f"Get ready to start in {timeout} seconds.")
         print("Press Enter to start immediately.")
         try:
             # Wait for the specified time or until Enter key is pressed
             rlist, _, _ = select.select([sys.stdin], [], [], timeout)
             if rlist:
                 # Enter key pressed, interrupt the sleep
                 sys.stdin.readline()
                 # print("Pause interrupted by user.")
+                print("Okay, starting in 3 seconds.")
+                time.sleep(3)
             else:
                 # print("Break over.")
                 pass
         except KeyboardInterrupt:
             # Handle Ctrl+C gracefully
             print("\nPause interrupted by user (Ctrl+C).")
 
     def _start_set_timer(self, seconds_per_set: int = None) -> float:
         if seconds_per_set is None:
             seconds_per_set = self.config["seconds_per_set"]
 
-
         f = Figlet(font='big')
 
-        print(colored(f.renderText('Start'), 'green'))
+        print(colored(f.renderText('S T A R T'), 'yellow'))
 
         print("\nStarted the timer for the set.")
         print("Press [Enter] to stop the timer.")
 
         start_time = time.time()
         elapsed_time = 0
 
@@ -824,26 +832,34 @@
     def _load_previous_workout_details(self) -> None:
         indir = self.config["workout_file"]["outdir"]
         if not os.path.exists(indir):
             logging.info(f"workflow files directory '{indir}' does not exist - so unable to load any previous workout details")
             return
 
         files = os.listdir(indir)
-        files = [os.path.join(indir, f) for f in files if f.endswith(".yaml")]
+        files = [os.path.join(indir, f) for f in files if f.endswith(".yaml") or f.endswith(".bak")]
         if len(files) == 0:
             logging.info(f"No workout files found in '{indir}'")
             return
 
         files.sort(reverse=True)
 
         for f in files:
 
             print(f"Processing workout file '{f}'")
 
-            timestamp = os.path.splitext(os.path.basename(f))[0]
+            timestamp = None
+
+            if f.endswith(".bak"):
+                # Example backup file: 2024-03-12.yaml.2024-03-12-090032.bak
+                timestamp = os.path.basename(f).split(".")[0]
+            elif f.endswith(".yaml"):
+                timestamp = os.path.splitext(os.path.basename(f))[0]
+            else:
+                logging.warning(f"Skipping file '{f}' as it does not have a '.yaml' or '.bak' extension")
 
             # Calculate number of days ago the workout was done
             date = datetime.strptime(timestamp, "%Y-%m-%d")
             days_ago = (datetime.now() - date).days
 
             logging.info(f"Will load contents of workout file '{f}'")
             config = yaml.safe_load(Path(f).read_text())
```

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker/system_caller.py` & `weight_training_tracker-0.9.0/weight_training_tracker/system_caller.py`

 * *Files identical despite different names*

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker.egg-info/PKG-INFO` & `weight_training_tracker-0.9.0/weight_training_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weight_training_tracker
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple CLI-based app for tracking weight training.
 Home-page: https://github.com/jai-python3/weight-training-tracker
 Author: Jaideep Sundaram
 Author-email: jai.python3@gmail.com
 Keywords: weight-training-tracker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `weight_training_tracker-0.8.0/weight_training_tracker.egg-info/SOURCES.txt` & `weight_training_tracker-0.9.0/weight_training_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

