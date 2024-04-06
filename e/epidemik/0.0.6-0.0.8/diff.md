# Comparing `tmp/epidemik-0.0.6.tar.gz` & `tmp/epidemik-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.6.tar", last modified: Sat Apr  6 18:50:26 2024, max compression
+gzip compressed data, was "epidemik-0.0.8.tar", last modified: Sat Apr  6 19:02:47 2024, max compression
```

## Comparing `epidemik-0.0.6.tar` & `epidemik-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.595429 epidemik-0.0.6/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.6/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:50:26.595218 epidemik-0.0.6/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.6/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 18:50:09.000000 epidemik-0.0.6/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 18:50:26.595473 epidemik-0.0.6/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.593719 epidemik-0.0.6/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.594447 epidemik-0.0.6/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    19363 2024-04-06 18:03:54.000000 epidemik-0.0.6/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5961 2024-04-06 18:47:57.000000 epidemik-0.0.6/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)       96 2024-04-06 18:50:11.000000 epidemik-0.0.6/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.595029 epidemik-0.0.6/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.034559 epidemik-0.0.8/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.8/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 19:02:47.034380 epidemik-0.0.8/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.8/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 19:02:36.000000 epidemik-0.0.8/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 19:02:47.034602 epidemik-0.0.8/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.032836 epidemik-0.0.8/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.033600 epidemik-0.0.8/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    17749 2024-04-06 18:55:08.000000 epidemik-0.0.8/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.8/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      289 2024-04-06 19:02:32.000000 epidemik-0.0.8/src/epidemik/__init__.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.034227 epidemik-0.0.8/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/top_level.txt
```

### Comparing `epidemik-0.0.6/LICENSE` & `epidemik-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.6/PKG-INFO` & `epidemik-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.6
+Version: 0.0.8
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epidemik-0.0.6/pyproject.toml` & `epidemik-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epidemik"
-version = "0.0.6"
+version = "0.0.8"
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
 description = "A pakage to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `epidemik-0.0.6/src/epidemik/EpiModel.py` & `epidemik-0.0.8/src/epidemik/EpiModel.py`

 * *Files 14% similar despite different names*

```diff
@@ -561,67 +561,7 @@
     def __getitem__(self, key):
         if key in self.values_.columns:
             return self.values_[key]
         elif key in self.values_ages_.columns:
             return self.values_ages_[key]
         else:
             return None
-
-if __name__ == '__main__':
-    SIR = EpiModel()
-
-    beta = 0.3
-    mu = 0.1
-
-    SIR.add_interaction('S', 'I', 'I', rate=beta)
-    SIR.add_spontaneous('I', 'R', rate=mu)
-
-    SIR.single_step(S=10000, I=10, R=0)
-
-    for i in range(10):
-        temp = dict(SIR.values_.iloc[-1].to_dict())
-        SIR.single_step(**temp)
-
-    SIR.values_
-
-    exit()
-    Nk_uk = pd.read_csv("data/United Kingdom-2020.csv", index_col=0)
-    Nk_ke = pd.read_csv("data/Kenya-2020.csv", index_col=0)
-
-    contacts_uk = pd.read_excel("data/MUestimates_all_locations_2.xlsx", sheet_name="United Kingdom of Great Britain", header=None)
-    contacts_ke = pd.read_excel("data/MUestimates_all_locations_1.xlsx", sheet_name="Kenya")
-
-    beta = 0.05
-    mu = 0.1
-
-    SIR_uk = EpiModel()
-    SIR_uk.add_interaction('S', 'I', 'I', beta)
-    SIR_uk.add_spontaneous('I', 'R', mu)
-
-
-    SIR_ke = EpiModel()
-    SIR_ke.add_interaction('S', 'I', 'I', beta)
-    SIR_ke.add_spontaneous('I', 'R', mu)
-
-    N_uk = int(Nk_uk.sum())
-    N_ke = int(Nk_ke.sum())
-
-
-    SIR_uk.add_age_structure(contacts_uk, Nk_uk)
-    SIR_ke.add_age_structure(contacts_ke, Nk_ke)
-
-    SIR_uk.integrate(100, S=N_uk*.99, I=N_uk*.01, R=0)
-    SIR_ke.integrate(100, S=N_ke*.99, I=N_ke*.01, R=0)
-
-    fig, ax = plt.subplots(1)
-    SIR_uk.draw_model(ax)
-    fig.savefig('SIR_model.png', dpi=300, facecolor='white')
-
-    fig, ax = plt.subplots(1)
-
-    (SIR_uk['I']*100/N_uk).plot(ax=ax)
-    (SIR_ke['I']*100/N_ke).plot(ax=ax)
-    ax.legend(['UK', 'Kenya'])
-    ax.set_xlabel('Time')
-    ax.set_ylabel('Population (%)')
-
-    fig.savefig('SIR_age.png', dpi=300, facecolor='white')
```

### Comparing `epidemik-0.0.6/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.8/src/epidemik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.6
+Version: 0.0.8
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

