# Comparing `tmp/aicsshparam-0.1.7.tar.gz` & `tmp/aicsshparam-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicsshparam-0.1.7.tar", last modified: Tue Jul 18 17:32:51 2023, max compression
+gzip compressed data, was "aicsshparam-0.1.9.tar", last modified: Fri Mar 15 17:09:11 2024, max compression
```

## Comparing `aicsshparam-0.1.7.tar` & `aicsshparam-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/aicsshparam/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/aicsshparam/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/shparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/shtools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/aicsshparam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)   621959 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/logo.gif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/pc12.png
--rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/table1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/table2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:09:11.272457 aicsshparam-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-15 17:09:11.272457 aicsshparam-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:09:11.268457 aicsshparam-0.1.9/aicsshparam/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/aicsshparam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:09:11.272457 aicsshparam-0.1.9/aicsshparam/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/aicsshparam/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/aicsshparam/shparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19075 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/aicsshparam/shtools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:09:11.272457 aicsshparam-0.1.9/aicsshparam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-15 17:09:11.000000 aicsshparam-0.1.9/aicsshparam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-15 17:09:11.000000 aicsshparam-0.1.9/aicsshparam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:09:11.000000 aicsshparam-0.1.9/aicsshparam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:09:11.000000 aicsshparam-0.1.9/aicsshparam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-15 17:09:11.000000 aicsshparam-0.1.9/aicsshparam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-15 17:09:11.000000 aicsshparam-0.1.9/aicsshparam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:09:11.272457 aicsshparam-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   621959 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/logo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/pc12.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25314 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/table1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/docs/table2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-15 17:09:11.272457 aicsshparam-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-15 17:09:05.000000 aicsshparam-0.1.9/setup.py
```

### Comparing `aicsshparam-0.1.7/CONTRIBUTING.md` & `aicsshparam-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/LICENSE` & `aicsshparam-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/PKG-INFO` & `aicsshparam-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: aicsshparam
-Version: 0.1.7
+Version: 0.1.9
 Summary: Spherical harmonics parametrization for 3D starlike shapes
 Home-page: https://github.com/AllenCell/aics-shparam
 Author: Matheus Viana
 Author-email: matheus.viana@alleninstitute.org
 License: Allen Institute Software License
 Keywords: aicsshparam
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
@@ -73,23 +72,24 @@
         image=img,
         angle=360 * np.random.rand()
     ).squeeze()
     return label, img
 
 # Compute spherical harmonics coefficients of shape and store them
 # in a pandas dataframe.
-df_coeffs = pd.DataFrame([])
+df_coeffs = []
 for i in range(30):
     # Get a random shape
     label, img = get_random_3d_shape()
     # Parameterize with L=4, which corresponds to50 coefficients
     # in total
     (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
     coeffs.update({'label': label})
-    df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
+    df_coeffs.append(coeffs)
+df_coeffs = pd.DataFrame(df_coeffs)
 
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_coeffs)
 ```
 
 ![Coefficients dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table1.jpg?raw=true)
```

### Comparing `aicsshparam-0.1.7/README.md` & `aicsshparam-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,24 @@
         image=img,
         angle=360 * np.random.rand()
     ).squeeze()
     return label, img
 
 # Compute spherical harmonics coefficients of shape and store them
 # in a pandas dataframe.
-df_coeffs = pd.DataFrame([])
+df_coeffs = []
 for i in range(30):
     # Get a random shape
     label, img = get_random_3d_shape()
     # Parameterize with L=4, which corresponds to50 coefficients
     # in total
     (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
     coeffs.update({'label': label})
-    df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
+    df_coeffs.append(coeffs)
+df_coeffs = pd.DataFrame(df_coeffs)
 
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_coeffs)
 ```
 
 ![Coefficients dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table1.jpg?raw=true)
```

### Comparing `aicsshparam-0.1.7/aicsshparam/shparam.py` & `aicsshparam-0.1.9/aicsshparam/shparam.py`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/aicsshparam/shtools.py` & `aicsshparam-0.1.9/aicsshparam/shtools.py`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/aicsshparam.egg-info/PKG-INFO` & `aicsshparam-0.1.9/aicsshparam.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: aicsshparam
-Version: 0.1.7
+Version: 0.1.9
 Summary: Spherical harmonics parametrization for 3D starlike shapes
 Home-page: https://github.com/AllenCell/aics-shparam
 Author: Matheus Viana
 Author-email: matheus.viana@alleninstitute.org
 License: Allen Institute Software License
 Keywords: aicsshparam
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
@@ -73,23 +72,24 @@
         image=img,
         angle=360 * np.random.rand()
     ).squeeze()
     return label, img
 
 # Compute spherical harmonics coefficients of shape and store them
 # in a pandas dataframe.
-df_coeffs = pd.DataFrame([])
+df_coeffs = []
 for i in range(30):
     # Get a random shape
     label, img = get_random_3d_shape()
     # Parameterize with L=4, which corresponds to50 coefficients
     # in total
     (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
     coeffs.update({'label': label})
-    df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
+    df_coeffs.append(coeffs)
+df_coeffs = pd.DataFrame(df_coeffs)
 
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_coeffs)
 ```
 
 ![Coefficients dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table1.jpg?raw=true)
```

### Comparing `aicsshparam-0.1.7/aicsshparam.egg-info/SOURCES.txt` & `aicsshparam-0.1.9/aicsshparam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/Makefile` & `aicsshparam-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/conf.py` & `aicsshparam-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/installation.rst` & `aicsshparam-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/logo.gif` & `aicsshparam-0.1.9/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/make.bat` & `aicsshparam-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/pc12.png` & `aicsshparam-0.1.9/docs/pc12.png`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/table1.jpg` & `aicsshparam-0.1.9/docs/table1.jpg`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/docs/table2.jpg` & `aicsshparam-0.1.9/docs/table2.jpg`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.7/setup.py` & `aicsshparam-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,45 +9,44 @@
     readme = readme_file.read()
 
 setup_requirements = [
     "pytest-runner>=5.2",
 ]
 
 test_requirements = [
-    "black>=22.10.0",
-#    "codecov>=2.1.4",
-    "flake8>=3.8.3",
-    "flake8-debugger>=3.2.1",
-    "pytest>=5.4.3",
-    "pytest-cov>=2.9.0",
-    "pytest-raises>=0.11",
+    "black",
+    "flake8",
+    "flake8-debugger",
+    "pytest",
+    "pytest-cov",
+    "pytest-raises",
 ]
 
 dev_requirements = [
     *setup_requirements,
     *test_requirements,
-    "bump2version>=1.0.1",
-    "coverage>=5.1",
-    "ipython>=7.15.0",
-    "m2r2>=0.2.7",
-    "pytest-runner>=5.2",
-    "sphinx>=7.0.1",
-    "furo>=2023.5.20",
-    "tox>=3.15.2",
-    "twine>=3.1.1",
-    "wheel>=0.34.2",
+    "bump2version",
+    "coverage",
+    "ipython",
+    "m2r2",
+    "pytest-runner",
+    "sphinx",
+    "furo",
+    "tox",
+    "twine",
+    "wheel",
 ]
 
 requirements = [
-    'numpy>=1.18.1',
-    'scipy>=1.4.1',
-    'scikit-image>=0.16.2',
-    'scikit-learn>=0.22.1',
-    'vtk>=9.0.1',
-    'pyshtools>=4.9.1'
+    'numpy',
+    'scipy',
+    'scikit-image',
+    'scikit-learn',
+    'vtk',
+    'pyshtools==4.10.4',#4.11+ seems to be broken with Python3.9+
 ]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [
@@ -56,34 +55,33 @@
     ]
 }
 
 setup(
     author="Matheus Viana",
     author_email="matheus.viana@alleninstitute.org",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
-        "Intended Audience :: Developers",
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Science/Research",
         "License :: Free for non-commercial use",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3 :: Only"
     ],
     description="Spherical harmonics parametrization for 3D starlike shapes",
     install_requires=requirements,
     license="Allen Institute Software License",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="aicsshparam",
     name="aicsshparam",
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*"]),
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     setup_requires=setup_requirements,
     test_suite="aicsshparam/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCell/aics-shparam",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.1.7",
+    version="0.1.9",
     zip_safe=False,
 )
```

