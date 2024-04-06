# Comparing `tmp/treat-sim-1.0.0.tar.gz` & `tmp/treat-sim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat-sim-1.0.0.tar", last modified: Wed Jun 28 14:46:40 2023, max compression
+gzip compressed data, was "treat-sim-1.1.0.tar", last modified: Sat Apr  6 15:43:35 2024, max compression
```

## Comparing `treat-sim-1.0.0.tar` & `treat-sim-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-28 14:46:40.523695 treat-sim-1.0.0/
--rw-rw-r--   0 tom       (1001) tom       (1001)       52 2022-10-25 08:21:31.000000 treat-sim-1.0.0/MANIFEST.in
--rw-rw-r--   0 tom       (1001) tom       (1001)     1844 2023-06-28 14:46:40.523695 treat-sim-1.0.0/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)     1266 2022-10-25 08:21:31.000000 treat-sim-1.0.0/README.md
--rw-rw-r--   0 tom       (1001) tom       (1001)       82 2023-06-28 13:53:35.000000 treat-sim-1.0.0/requirements.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       38 2023-06-28 14:46:40.523695 treat-sim-1.0.0/setup.cfg
--rw-rw-r--   0 tom       (1001) tom       (1001)     1817 2022-10-25 08:21:31.000000 treat-sim-1.0.0/setup.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-28 14:46:40.523695 treat-sim-1.0.0/treat_sim/
--rw-rw-r--   0 tom       (1001) tom       (1001)       45 2023-06-28 14:43:14.000000 treat-sim-1.0.0/treat_sim/__init__.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-28 14:46:40.523695 treat-sim-1.0.0/treat_sim/data/
--rw-rw-r--   0 tom       (1001) tom       (1001)      381 2022-10-25 08:21:31.000000 treat-sim-1.0.0/treat_sim/data/ed_arrivals.csv
--rw-rw-r--   0 tom       (1001) tom       (1001)     5895 2022-10-25 08:21:31.000000 treat-sim-1.0.0/treat_sim/distributions.py
--rw-rw-r--   0 tom       (1001) tom       (1001)    38255 2023-06-28 14:32:50.000000 treat-sim-1.0.0/treat_sim/model.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2023-06-28 14:46:40.523695 treat-sim-1.0.0/treat_sim.egg-info/
--rw-rw-r--   0 tom       (1001) tom       (1001)     1844 2023-06-28 14:46:40.000000 treat-sim-1.0.0/treat_sim.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)      310 2023-06-28 14:46:40.000000 treat-sim-1.0.0/treat_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-06-28 14:46:40.000000 treat-sim-1.0.0/treat_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       72 2023-06-28 14:46:40.000000 treat-sim-1.0.0/treat_sim.egg-info/requires.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       10 2023-06-28 14:46:40.000000 treat-sim-1.0.0/treat_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 15:43:31.000000 treat-sim-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 15:43:31.000000 treat-sim-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-06 15:43:35.280857 treat-sim-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-06 15:43:31.000000 treat-sim-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-06 15:43:31.000000 treat-sim-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:43:35.280857 treat-sim-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-06 15:43:31.000000 treat-sim-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/treat_sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/treat_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/data/ed_arrivals.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-04-06 15:43:31.000000 treat-sim-1.1.0/treat_sim/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:35.280857 treat-sim-1.1.0/treat_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 15:43:35.000000 treat-sim-1.1.0/treat_sim.egg-info/top_level.txt
```

### Comparing `treat-sim-1.0.0/setup.py` & `treat-sim-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,21 +32,22 @@
     author_email="forecast-tools@gmail.com",
     license="The MIT License (MIT)",
     license_files=('LICENSE', ),
     description="A free and open implementation of the Treatment Centre Model from Nelson (2013)",
     # read in from readme.md and will appear on PyPi
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/TomMonks/treatment-centre-sim",
+    url="https://github.com/pythonhealthdatascience/stars-treat-sim",
     packages=setuptools.find_packages(),
     # if true look in MANIFEST.in for data files to include
     include_package_data=True,
     # these are for documentation 
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8.12',
     install_requires=requirements,
 )
```

### Comparing `treat-sim-1.0.0/treat_sim/distributions.py` & `treat-sim-1.1.0/treat_sim/distributions.py`

 * *Files identical despite different names*

### Comparing `treat-sim-1.0.0/treat_sim/model.py` & `treat-sim-1.1.0/treat_sim/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,17 +297,19 @@
         self.n_cubicles_2 = n_cubicles_2
 
     def init_sampling(self):
         '''
         Create the distributions used by the model and initialise 
         the random seeds of each.
         '''
-        # create random number streams
-        rng_streams = np.random.default_rng(self.random_number_set)
-        self.seeds = rng_streams.integers(0, 999999999, size=N_STREAMS)
+        # MODIFICATION. Better method for producing n non-overlapping streams
+        seed_sequence = np.random.SeedSequence(self.random_number_set)
+    
+        # Generate n high quality child seeds
+        self.seeds = seed_sequence.spawn(N_STREAMS)
 
         # create distributions
         
         # Triage duration
         self.triage_dist = Exponential(self.triage_mean, 
                                        random_seed=self.seeds[0])
```

