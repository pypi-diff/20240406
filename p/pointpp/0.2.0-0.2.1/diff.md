# Comparing `tmp/pointpp-0.2.0.tar.gz` & `tmp/pointpp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointpp-0.2.0.tar", last modified: Wed Feb  1 14:45:59 2023, max compression
+gzip compressed data, was "pointpp-0.2.1.tar", last modified: Sat Apr  6 18:56:42 2024, max compression
```

## Comparing `pointpp-0.2.0.tar` & `pointpp-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 thomasn  (43954) thomasn  (43954)        0 2023-02-01 14:45:59.739954 pointpp-0.2.0/
--rw-rw-r--   0 thomasn  (43954) thomasn  (43954)     1469 2017-05-16 07:29:38.000000 pointpp-0.2.0/LICENSE
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)      838 2023-02-01 14:45:59.739954 pointpp-0.2.0/PKG-INFO
--rw-rw-r--   0 thomasn  (43954) thomasn  (43954)     1250 2017-10-23 07:46:24.000000 pointpp-0.2.0/README.rst
-drwxr-xr-x   0 thomasn  (43954) thomasn  (43954)        0 2023-02-01 14:45:59.739954 pointpp-0.2.0/pointpp/
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)      229 2023-02-01 14:42:47.000000 pointpp-0.2.0/pointpp/__init__.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)    11945 2023-02-01 14:43:06.000000 pointpp-0.2.0/pointpp/__main__.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)     2637 2023-02-01 14:44:12.000000 pointpp-0.2.0/pointpp/gen.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)    35273 2022-10-16 16:48:00.000000 pointpp-0.2.0/pointpp/method.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)      446 2020-07-11 14:50:03.000000 pointpp-0.2.0/pointpp/metric.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)     3727 2023-02-01 14:44:30.000000 pointpp-0.2.0/pointpp/radpro.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)     1437 2021-07-10 15:45:29.000000 pointpp-0.2.0/pointpp/solver.py
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)      598 2020-07-11 16:08:49.000000 pointpp-0.2.0/pointpp/util.py
-drwxr-xr-x   0 thomasn  (43954) thomasn  (43954)        0 2023-02-01 14:45:59.739954 pointpp-0.2.0/pointpp.egg-info/
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)      838 2023-02-01 14:45:59.000000 pointpp-0.2.0/pointpp.egg-info/PKG-INFO
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)      358 2023-02-01 14:45:59.000000 pointpp-0.2.0/pointpp.egg-info/SOURCES.txt
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)        1 2023-02-01 14:45:59.000000 pointpp-0.2.0/pointpp.egg-info/dependency_links.txt
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)       69 2023-02-01 14:45:59.000000 pointpp-0.2.0/pointpp.egg-info/entry_points.txt
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)       98 2023-02-01 14:45:59.000000 pointpp-0.2.0/pointpp.egg-info/requires.txt
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)        8 2023-02-01 14:45:59.000000 pointpp-0.2.0/pointpp.egg-info/top_level.txt
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)       38 2023-02-01 14:45:59.739954 pointpp-0.2.0/setup.cfg
--rw-r--r--   0 thomasn  (43954) thomasn  (43954)     2447 2023-01-27 10:10:04.000000 pointpp-0.2.0/setup.py
+drwxrwxr-x   0 thomasn  (43954) thomasn  (43954)        0 2024-04-06 18:56:42.224765 pointpp-0.2.1/
+-rw-rw-r--   0 thomasn  (43954) thomasn  (43954)     1469 2017-05-16 07:29:38.000000 pointpp-0.2.1/LICENSE
+-rw-rw-r--   0 thomasn  (43954) thomasn  (43954)      866 2024-04-06 18:56:42.224765 pointpp-0.2.1/PKG-INFO
+-rw-rw-r--   0 thomasn  (43954) thomasn  (43954)     1250 2017-10-23 07:46:24.000000 pointpp-0.2.1/README.rst
+drwxrwxr-x   0 thomasn  (43954) thomasn  (43954)        0 2024-04-06 18:56:42.224765 pointpp-0.2.1/pointpp/
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)      229 2024-04-06 18:55:25.000000 pointpp-0.2.1/pointpp/__init__.py
+-rw-rw-r--   0 thomasn  (43954) thomasn  (43954)    12014 2024-03-23 08:15:09.000000 pointpp-0.2.1/pointpp/__main__.py
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)     2637 2023-02-01 14:44:12.000000 pointpp-0.2.1/pointpp/gen.py
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)    35273 2022-10-16 16:48:00.000000 pointpp-0.2.1/pointpp/method.py
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)      446 2020-07-11 14:50:03.000000 pointpp-0.2.1/pointpp/metric.py
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)     3727 2023-02-01 14:44:30.000000 pointpp-0.2.1/pointpp/radpro.py
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)     1437 2021-07-10 15:45:29.000000 pointpp-0.2.1/pointpp/solver.py
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)      598 2020-07-11 16:08:49.000000 pointpp-0.2.1/pointpp/util.py
+drwxrwxr-x   0 thomasn  (43954) thomasn  (43954)        0 2024-04-06 18:56:42.224765 pointpp-0.2.1/pointpp.egg-info/
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)      866 2024-04-06 18:56:42.000000 pointpp-0.2.1/pointpp.egg-info/PKG-INFO
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)      358 2024-04-06 18:56:42.000000 pointpp-0.2.1/pointpp.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)        1 2024-04-06 18:56:42.000000 pointpp-0.2.1/pointpp.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)       70 2024-04-06 18:56:42.000000 pointpp-0.2.1/pointpp.egg-info/entry_points.txt
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)       98 2024-04-06 18:56:42.000000 pointpp-0.2.1/pointpp.egg-info/requires.txt
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)        8 2024-04-06 18:56:42.000000 pointpp-0.2.1/pointpp.egg-info/top_level.txt
+-rw-rw-r--   0 thomasn  (43954) thomasn  (43954)       38 2024-04-06 18:56:42.224765 pointpp-0.2.1/setup.cfg
+-rw-r--r--   0 thomasn  (43954) thomasn  (43954)     2447 2023-01-27 10:10:04.000000 pointpp-0.2.1/setup.py
```

### Comparing `pointpp-0.2.0/LICENSE` & `pointpp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/PKG-INFO` & `pointpp-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: pointpp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Program to post-process verif files
 Home-page: https://github.com/tnipen/pointpp
 Author: Thomas Nipen
 Author-email: thomas.nipen@met.no
 License: BSD-3
 Keywords: meteorology post-processing weather prediction
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: test
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `pointpp-0.2.0/README.rst` & `pointpp-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/pointpp/__main__.py` & `pointpp-0.2.1/pointpp/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,25 +45,27 @@
         sys.exit(1)
     args = parser.parse_args()
 
     # Evaluation dataset
     input = verif.input.get_input(args.file)
     eobs = input.obs
     efcst = input.fcst
+    etimes = input.times
 
     if eobs is None:
         pointpp.util.error("No observations available")
 
     # Training dataset
     if args.file_training is not None:
         input_training = verif.input.get_input(args.file_training)
     else:
         input_training = input
     tobs = input_training.obs
     tfcst = input_training.fcst
+    ttimes = input_training.times
 
     if args.dates is not None:
         dates = [verif.util.unixtime_to_date(d) for d in input_training.times]
         Idates = [i for i in range(tobs.shape[0]) if dates[i] in args.dates]
         print("Reducing dates: %d to %d" % (tobs.shape[0], len(Idates)))
         tobs = tobs[Idates, :, :]
         tfcst = tfcst[Idates, :, :]
@@ -106,21 +108,21 @@
 
 
     if args.ofile is not None:
         """ Create output """
         shutil.copyfile(args.file, args.ofile)
 
         fid = netCDF4.Dataset(args.ofile, 'a')
-        efcst2, eobs2 = calibrate(tobs, tfcst, eobs, efcst, args.method, method, args.leadtime_dependent, args.location_dependent)
+        efcst2, eobs2 = calibrate(tobs, tfcst, etimes, eobs, efcst, e2t_loc, args.method, method, args.leadtime_dependent, args.location_dependent)
         fid.variables["fcst"][:] = efcst2
 
         if "quantile" in fid.variables:
             for i in range(len(fid.variables["quantile"])):
                 curr = input.quantile_scores[..., i]
-                efcst2, _ = calibrate(tobs, tfcst, eobs, curr, args.method, method, args.leadtime_dependent, args.location_dependent)
+                efcst2, _ = calibrate(tobs, tfcst, etimes, eobs, curr, e2t_loc, args.method, method, args.leadtime_dependent, args.location_dependent)
                 fid.variables["x"][:, :, :, i] = efcst2
 
         if eobs2 is not None:
             fid.variables["obs"][:] = eobs2
         print("Writing")
         fid.close()
 
@@ -184,15 +186,15 @@
         if header is not None:
             file.write("%s\n" % header)
         for i in range(len(x)):
             file.write("%f %f\n" % (x[i], y[i]))
         file.close()
 
 
-def calibrate(tobs, tfcst, eobs, efcst, method_name, method, leadtime_dependent, location_dependent):
+def calibrate(tobs, tfcst, etimes, eobs, efcst, e2t_loc, method_name, method, leadtime_dependent, location_dependent):
     D = eobs.shape[0]
     LT = eobs.shape[1]
     LOC = eobs.shape[2]
 
     eobs2 = None
     if method_name == "pers" or method_name == "fpers":
         """ Persistence methods should always be location and date dependent """
@@ -201,29 +203,28 @@
             for j in e2t_loc:
                 #pointpp.util.progress_bar(i * LOC + j, D * LOC)
                 jt = e2t_loc[j]
                 efcst2 [i, :, j] = method.calibrate(tobs[i, :, jt], tfcst[i, :, jt], efcst[i, :, j])
     elif method_name == "clim":
         """ Climatology methods should always be location, leadtime, and month dependent """
         efcst2 = np.nan * np.zeros(eobs.shape)
-        all_months = np.array([verif.util.unixtime_to_date(t) // 100 % 100 for t in input.times])
-        months = np.unique(np.sort([verif.util.unixtime_to_date(t) // 100 % 100 for t in input.times]))
+        all_months = np.array([verif.util.unixtime_to_date(t) // 100 % 100 for t in etimes])
+        months = np.unique(np.sort([verif.util.unixtime_to_date(t) // 100 % 100 for t in etimes]))
         for i in range(len(months)):
             month = months[i]
             I = np.where(all_months == month)[0]
             for i in range(LT):
-                for j in e2t_loc:
-                    jt = e2t_loc[j]
+                for j, jt in enumerate(e2t_loc):
                     tmp = method.calibrate(tobs[I, i, jt].flatten(), tfcst[I, i, jt].flatten(), efcst[I, i, j].flatten())
                     efcst2[I, i, j] = tmp
     elif method_name == "anomaly":
         efcst2 = np.nan * np.zeros(eobs.shape)
         eobs2 = np.nan * np.zeros(eobs.shape)
-        all_months = np.array([verif.util.unixtime_to_date(t) // 100 % 100 for t in input.times])
-        months = np.unique(np.sort([verif.util.unixtime_to_date(t) // 100 % 100 for t in input.times]))
+        all_months = np.array([verif.util.unixtime_to_date(t) // 100 % 100 for t in etimes])
+        months = np.unique(np.sort([verif.util.unixtime_to_date(t) // 100 % 100 for t in etimes]))
         for i in range(len(months)):
             month = months[i]
             I = np.where(all_months == month)[0]
             for j in e2t_loc:
                 jt = e2t_loc[j]
                 mean_obs = np.nanmean(tobs[I, :, jt])
                 mean_fcst = np.nanmean(tfcst[I, :, jt])
```

### Comparing `pointpp-0.2.0/pointpp/gen.py` & `pointpp-0.2.1/pointpp/gen.py`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/pointpp/method.py` & `pointpp-0.2.1/pointpp/method.py`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/pointpp/radpro.py` & `pointpp-0.2.1/pointpp/radpro.py`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/pointpp/solver.py` & `pointpp-0.2.1/pointpp/solver.py`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/pointpp/util.py` & `pointpp-0.2.1/pointpp/util.py`

 * *Files identical despite different names*

### Comparing `pointpp-0.2.0/pointpp.egg-info/PKG-INFO` & `pointpp-0.2.1/pointpp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: pointpp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Program to post-process verif files
 Home-page: https://github.com/tnipen/pointpp
 Author: Thomas Nipen
 Author-email: thomas.nipen@met.no
 License: BSD-3
 Keywords: meteorology post-processing weather prediction
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: test
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `pointpp-0.2.0/setup.py` & `pointpp-0.2.1/setup.py`

 * *Files identical despite different names*

