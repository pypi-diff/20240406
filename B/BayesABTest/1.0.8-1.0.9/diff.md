# Comparing `tmp/BayesABTest-1.0.8.tar.gz` & `tmp/BayesABTest-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BayesABTest-1.0.8.tar", last modified: Tue Mar 29 20:28:45 2022, max compression
+gzip compressed data, was "BayesABTest-1.0.9.tar", last modified: Sat Apr  6 00:38:53 2024, max compression
```

## Comparing `BayesABTest-1.0.8.tar` & `BayesABTest-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bakermoran   (501) staff       (20)        0 2022-03-29 20:28:45.844922 BayesABTest-1.0.8/
-drwxr-xr-x   0 bakermoran   (501) staff       (20)        0 2022-03-29 20:28:45.842472 BayesABTest-1.0.8/BayesABTest/
--rw-r--r--   0 bakermoran   (501) staff       (20)      375 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/__init__.py
--rw-r--r--   0 bakermoran   (501) staff       (20)     6587 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/_ab_test_model_loss_func.py
--rw-r--r--   0 bakermoran   (501) staff       (20)    12217 2022-03-29 20:25:45.000000 BayesABTest-1.0.8/BayesABTest/_ab_test_model_plotting.py
--rw-r--r--   0 bakermoran   (501) staff       (20)     4067 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/_ab_test_model_sampling.py
--rw-r--r--   0 bakermoran   (501) staff       (20)     1371 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/_ab_test_model_utils.py
--rw-r--r--   0 bakermoran   (501) staff       (20)     6524 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/_posterior_distribution.py
--rw-r--r--   0 bakermoran   (501) staff       (20)    10294 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/_prior_distribution.py
--rw-r--r--   0 bakermoran   (501) staff       (20)     4580 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/ab_test_dist_explorer.py
--rw-r--r--   0 bakermoran   (501) staff       (20)    15252 2022-03-29 20:18:03.000000 BayesABTest-1.0.8/BayesABTest/ab_test_model.py
-drwxr-xr-x   0 bakermoran   (501) staff       (20)        0 2022-03-29 20:28:45.844635 BayesABTest-1.0.8/BayesABTest.egg-info/
--rw-r--r--   0 bakermoran   (501) staff       (20)     3455 2022-03-29 20:28:45.000000 BayesABTest-1.0.8/BayesABTest.egg-info/PKG-INFO
--rw-r--r--   0 bakermoran   (501) staff       (20)      528 2022-03-29 20:28:45.000000 BayesABTest-1.0.8/BayesABTest.egg-info/SOURCES.txt
--rw-r--r--   0 bakermoran   (501) staff       (20)        1 2022-03-29 20:28:45.000000 BayesABTest-1.0.8/BayesABTest.egg-info/dependency_links.txt
--rw-r--r--   0 bakermoran   (501) staff       (20)       62 2022-03-29 20:28:45.000000 BayesABTest-1.0.8/BayesABTest.egg-info/requires.txt
--rw-r--r--   0 bakermoran   (501) staff       (20)       12 2022-03-29 20:28:45.000000 BayesABTest-1.0.8/BayesABTest.egg-info/top_level.txt
--rw-r--r--   0 bakermoran   (501) staff       (20)     1068 2021-07-08 14:45:02.000000 BayesABTest-1.0.8/LICENSE
--rw-r--r--   0 bakermoran   (501) staff       (20)     3455 2022-03-29 20:28:45.845090 BayesABTest-1.0.8/PKG-INFO
--rw-r--r--   0 bakermoran   (501) staff       (20)     2677 2022-03-29 20:27:23.000000 BayesABTest-1.0.8/README.md
--rw-r--r--   0 bakermoran   (501) staff       (20)       79 2022-03-29 20:28:45.845576 BayesABTest-1.0.8/setup.cfg
--rw-r--r--   0 bakermoran   (501) staff       (20)     1305 2022-03-29 20:27:18.000000 BayesABTest-1.0.8/setup.py
+drwxr-xr-x   0 bakermoran   (501) staff       (20)        0 2024-04-06 00:38:53.516791 BayesABTest-1.0.9/
+drwxr-xr-x   0 bakermoran   (501) staff       (20)        0 2024-04-06 00:38:53.515063 BayesABTest-1.0.9/BayesABTest/
+-rw-r--r--   0 bakermoran   (501) staff       (20)      375 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/__init__.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)     6587 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/_ab_test_model_loss_func.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)    12217 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/_ab_test_model_plotting.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)     4067 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/_ab_test_model_sampling.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)     1371 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/_ab_test_model_utils.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)     6524 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/_posterior_distribution.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)    10294 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/_prior_distribution.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)     4580 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/ab_test_dist_explorer.py
+-rw-r--r--   0 bakermoran   (501) staff       (20)    15252 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/BayesABTest/ab_test_model.py
+drwxr-xr-x   0 bakermoran   (501) staff       (20)        0 2024-04-06 00:38:53.516346 BayesABTest-1.0.9/BayesABTest.egg-info/
+-rw-r--r--   0 bakermoran   (501) staff       (20)     3587 2024-04-06 00:38:53.000000 BayesABTest-1.0.9/BayesABTest.egg-info/PKG-INFO
+-rw-r--r--   0 bakermoran   (501) staff       (20)      528 2024-04-06 00:38:53.000000 BayesABTest-1.0.9/BayesABTest.egg-info/SOURCES.txt
+-rw-r--r--   0 bakermoran   (501) staff       (20)        1 2024-04-06 00:38:53.000000 BayesABTest-1.0.9/BayesABTest.egg-info/dependency_links.txt
+-rw-r--r--   0 bakermoran   (501) staff       (20)       67 2024-04-06 00:38:53.000000 BayesABTest-1.0.9/BayesABTest.egg-info/requires.txt
+-rw-r--r--   0 bakermoran   (501) staff       (20)       12 2024-04-06 00:38:53.000000 BayesABTest-1.0.9/BayesABTest.egg-info/top_level.txt
+-rw-r--r--   0 bakermoran   (501) staff       (20)     1068 2023-10-26 21:07:26.000000 BayesABTest-1.0.9/LICENSE
+-rw-r--r--   0 bakermoran   (501) staff       (20)     3587 2024-04-06 00:38:53.516704 BayesABTest-1.0.9/PKG-INFO
+-rw-r--r--   0 bakermoran   (501) staff       (20)     2702 2024-04-06 00:36:14.000000 BayesABTest-1.0.9/README.md
+-rw-r--r--   0 bakermoran   (501) staff       (20)       79 2024-04-06 00:38:53.517051 BayesABTest-1.0.9/setup.cfg
+-rw-r--r--   0 bakermoran   (501) staff       (20)     1311 2024-04-06 00:35:24.000000 BayesABTest-1.0.9/setup.py
```

### Comparing `BayesABTest-1.0.8/BayesABTest/_ab_test_model_loss_func.py` & `BayesABTest-1.0.9/BayesABTest/_ab_test_model_loss_func.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/_ab_test_model_plotting.py` & `BayesABTest-1.0.9/BayesABTest/_ab_test_model_plotting.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/_ab_test_model_sampling.py` & `BayesABTest-1.0.9/BayesABTest/_ab_test_model_sampling.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/_ab_test_model_utils.py` & `BayesABTest-1.0.9/BayesABTest/_ab_test_model_utils.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/_posterior_distribution.py` & `BayesABTest-1.0.9/BayesABTest/_posterior_distribution.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/_prior_distribution.py` & `BayesABTest-1.0.9/BayesABTest/_prior_distribution.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/ab_test_dist_explorer.py` & `BayesABTest-1.0.9/BayesABTest/ab_test_dist_explorer.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest/ab_test_model.py` & `BayesABTest-1.0.9/BayesABTest/ab_test_model.py`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/BayesABTest.egg-info/PKG-INFO` & `BayesABTest-1.0.9/BayesABTest.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: BayesABTest
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for running AB tests in a Bayesian framework.
 Home-page: https://github.com/bakermoran/BayesABTest
+Download-URL: https://github.com/bakermoran/BayesABTest/archive/v1.0.9-alpha.tar.gz
 Author: Baker Moran
 Author-email: bamoran99@gmail.com
 License: MIT
-Download-URL: https://github.com/bakermoran/BayesABTest/archive/v1.0.8-alpha.tar.gz
 Keywords: AB Test,Bayes,Bayesian Statistics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy<1.24.0,>=1.21.0
+Requires-Dist: pandas<1.5.0
+Requires-Dist: matplotlib<4.0.0
+Requires-Dist: seaborn<0.11.0
 
 # Bayesian AB Test Report Builder
 
 ![Build Status](https://github.com/bakermoran/BayesABTest/workflows/Build%20Status/badge.svg?branch=main)
 [![PyPI version](https://badge.fury.io/py/BayesABTest.svg)](https://badge.fury.io/py/BayesABTest)
 
 > **Baker Moran**
@@ -30,23 +33,23 @@
 
 ### Example Output for a conversion rate test
 
 ![alt text](docs/package_documentation/img/one_var_continuous.png "Conversion Rate Example")
 
 ## Installation
 
-* Install via pip (or specify pip3)
+- Install via pip (or specify pip3)
 
-    ```bash
-    pip install BayesABTest
-    ```
+  ```bash
+  pip install BayesABTest
+  ```
 
   OR
 
-* Download files from [PyPi](https://pypi.org/project/BayesABTest/#files) and install
+- Download files from [PyPi](https://pypi.org/project/BayesABTest/#files) and install
 
 ## Package Functions and Classes
 
 ### [ab_test_model](docs/package_documentation/ab_test_model.md)
 
 Class implementing out of the box AB testing functionality. Simple, easy to use AB testing with many different prior function types, all in one clean interface.
 
@@ -62,25 +65,24 @@
 
 ### Acknowledgements
 
 There is a lot of documentation out there about a Bayesian framework of A/B testing. Some of the specific articles are listed below. Most of the work I came across was written in R, and I set out to create a Python implementation. The visuals were inspired by a standard template we use at Root, first written by <https://github.com/zachurchill-root>.
 
 Articles Reference:
 
-* <https://www.countbayesie.com/blog/2015/4/25/bayesian-ab-testing>
-* <https://medium.com/convoy-tech/the-power-of-bayesian-a-b-testing-f859d2219d5>
-* <https://cdn2.hubspot.net/hubfs/310840/VWO_SmartStats_technical_whitepaper.pdf>
+- <https://www.countbayesie.com/blog/2015/4/25/bayesian-ab-testing>
+- <https://medium.com/convoy-tech/the-power-of-bayesian-a-b-testing-f859d2219d5>
+- <https://cdn2.hubspot.net/hubfs/310840/VWO_SmartStats_technical_whitepaper.pdf>
 
 ### Version History
 
-* `0.1.0-prealpha` - *12/02/2019*
-* `1.0.0-alpha` - *12/27/2019*
-* `1.0.1-alpha` - *01/02/2020*
-* `1.0.2-alpha` - *06/17/2020*
-* `1.0.3-alpha` - *06/17/2020*
-* `1.0.4-alpha` - *06/22/2020*
-* `1.0.5-alpha` - *06/22/2020*
-* `1.0.6-alpha` - *06/22/2020*
-* `1.0.7-alpha` - *07/09/2021*
-* `1.0.8-alpha` - *03/29/2022*
-
-
+- `0.1.0-prealpha` - _12/02/2019_
+- `1.0.0-alpha` - _12/27/2019_
+- `1.0.1-alpha` - _01/02/2020_
+- `1.0.2-alpha` - _06/17/2020_
+- `1.0.3-alpha` - _06/17/2020_
+- `1.0.4-alpha` - _06/22/2020_
+- `1.0.5-alpha` - _06/22/2020_
+- `1.0.6-alpha` - _06/22/2020_
+- `1.0.7-alpha` - _07/09/2021_
+- `1.0.8-alpha` - _03/29/2022_
+- `1.0.9-alpha` - _03/29/2022_
```

### Comparing `BayesABTest-1.0.8/BayesABTest.egg-info/SOURCES.txt` & `BayesABTest-1.0.9/BayesABTest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/LICENSE` & `BayesABTest-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BayesABTest-1.0.8/PKG-INFO` & `BayesABTest-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: BayesABTest
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for running AB tests in a Bayesian framework.
 Home-page: https://github.com/bakermoran/BayesABTest
+Download-URL: https://github.com/bakermoran/BayesABTest/archive/v1.0.9-alpha.tar.gz
 Author: Baker Moran
 Author-email: bamoran99@gmail.com
 License: MIT
-Download-URL: https://github.com/bakermoran/BayesABTest/archive/v1.0.8-alpha.tar.gz
 Keywords: AB Test,Bayes,Bayesian Statistics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy<1.24.0,>=1.21.0
+Requires-Dist: pandas<1.5.0
+Requires-Dist: matplotlib<4.0.0
+Requires-Dist: seaborn<0.11.0
 
 # Bayesian AB Test Report Builder
 
 ![Build Status](https://github.com/bakermoran/BayesABTest/workflows/Build%20Status/badge.svg?branch=main)
 [![PyPI version](https://badge.fury.io/py/BayesABTest.svg)](https://badge.fury.io/py/BayesABTest)
 
 > **Baker Moran**
@@ -30,23 +33,23 @@
 
 ### Example Output for a conversion rate test
 
 ![alt text](docs/package_documentation/img/one_var_continuous.png "Conversion Rate Example")
 
 ## Installation
 
-* Install via pip (or specify pip3)
+- Install via pip (or specify pip3)
 
-    ```bash
-    pip install BayesABTest
-    ```
+  ```bash
+  pip install BayesABTest
+  ```
 
   OR
 
-* Download files from [PyPi](https://pypi.org/project/BayesABTest/#files) and install
+- Download files from [PyPi](https://pypi.org/project/BayesABTest/#files) and install
 
 ## Package Functions and Classes
 
 ### [ab_test_model](docs/package_documentation/ab_test_model.md)
 
 Class implementing out of the box AB testing functionality. Simple, easy to use AB testing with many different prior function types, all in one clean interface.
 
@@ -62,25 +65,24 @@
 
 ### Acknowledgements
 
 There is a lot of documentation out there about a Bayesian framework of A/B testing. Some of the specific articles are listed below. Most of the work I came across was written in R, and I set out to create a Python implementation. The visuals were inspired by a standard template we use at Root, first written by <https://github.com/zachurchill-root>.
 
 Articles Reference:
 
-* <https://www.countbayesie.com/blog/2015/4/25/bayesian-ab-testing>
-* <https://medium.com/convoy-tech/the-power-of-bayesian-a-b-testing-f859d2219d5>
-* <https://cdn2.hubspot.net/hubfs/310840/VWO_SmartStats_technical_whitepaper.pdf>
+- <https://www.countbayesie.com/blog/2015/4/25/bayesian-ab-testing>
+- <https://medium.com/convoy-tech/the-power-of-bayesian-a-b-testing-f859d2219d5>
+- <https://cdn2.hubspot.net/hubfs/310840/VWO_SmartStats_technical_whitepaper.pdf>
 
 ### Version History
 
-* `0.1.0-prealpha` - *12/02/2019*
-* `1.0.0-alpha` - *12/27/2019*
-* `1.0.1-alpha` - *01/02/2020*
-* `1.0.2-alpha` - *06/17/2020*
-* `1.0.3-alpha` - *06/17/2020*
-* `1.0.4-alpha` - *06/22/2020*
-* `1.0.5-alpha` - *06/22/2020*
-* `1.0.6-alpha` - *06/22/2020*
-* `1.0.7-alpha` - *07/09/2021*
-* `1.0.8-alpha` - *03/29/2022*
-
-
+- `0.1.0-prealpha` - _12/02/2019_
+- `1.0.0-alpha` - _12/27/2019_
+- `1.0.1-alpha` - _01/02/2020_
+- `1.0.2-alpha` - _06/17/2020_
+- `1.0.3-alpha` - _06/17/2020_
+- `1.0.4-alpha` - _06/22/2020_
+- `1.0.5-alpha` - _06/22/2020_
+- `1.0.6-alpha` - _06/22/2020_
+- `1.0.7-alpha` - _07/09/2021_
+- `1.0.8-alpha` - _03/29/2022_
+- `1.0.9-alpha` - _03/29/2022_
```

### Comparing `BayesABTest-1.0.8/README.md` & `BayesABTest-1.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 ### Example Output for a conversion rate test
 
 ![alt text](docs/package_documentation/img/one_var_continuous.png "Conversion Rate Example")
 
 ## Installation
 
-* Install via pip (or specify pip3)
+- Install via pip (or specify pip3)
 
-    ```bash
-    pip install BayesABTest
-    ```
+  ```bash
+  pip install BayesABTest
+  ```
 
   OR
 
-* Download files from [PyPi](https://pypi.org/project/BayesABTest/#files) and install
+- Download files from [PyPi](https://pypi.org/project/BayesABTest/#files) and install
 
 ## Package Functions and Classes
 
 ### [ab_test_model](docs/package_documentation/ab_test_model.md)
 
 Class implementing out of the box AB testing functionality. Simple, easy to use AB testing with many different prior function types, all in one clean interface.
 
@@ -41,23 +41,24 @@
 
 ### Acknowledgements
 
 There is a lot of documentation out there about a Bayesian framework of A/B testing. Some of the specific articles are listed below. Most of the work I came across was written in R, and I set out to create a Python implementation. The visuals were inspired by a standard template we use at Root, first written by <https://github.com/zachurchill-root>.
 
 Articles Reference:
 
-* <https://www.countbayesie.com/blog/2015/4/25/bayesian-ab-testing>
-* <https://medium.com/convoy-tech/the-power-of-bayesian-a-b-testing-f859d2219d5>
-* <https://cdn2.hubspot.net/hubfs/310840/VWO_SmartStats_technical_whitepaper.pdf>
+- <https://www.countbayesie.com/blog/2015/4/25/bayesian-ab-testing>
+- <https://medium.com/convoy-tech/the-power-of-bayesian-a-b-testing-f859d2219d5>
+- <https://cdn2.hubspot.net/hubfs/310840/VWO_SmartStats_technical_whitepaper.pdf>
 
 ### Version History
 
-* `0.1.0-prealpha` - *12/02/2019*
-* `1.0.0-alpha` - *12/27/2019*
-* `1.0.1-alpha` - *01/02/2020*
-* `1.0.2-alpha` - *06/17/2020*
-* `1.0.3-alpha` - *06/17/2020*
-* `1.0.4-alpha` - *06/22/2020*
-* `1.0.5-alpha` - *06/22/2020*
-* `1.0.6-alpha` - *06/22/2020*
-* `1.0.7-alpha` - *07/09/2021*
-* `1.0.8-alpha` - *03/29/2022*
+- `0.1.0-prealpha` - _12/02/2019_
+- `1.0.0-alpha` - _12/27/2019_
+- `1.0.1-alpha` - _01/02/2020_
+- `1.0.2-alpha` - _06/17/2020_
+- `1.0.3-alpha` - _06/17/2020_
+- `1.0.4-alpha` - _06/22/2020_
+- `1.0.5-alpha` - _06/22/2020_
+- `1.0.6-alpha` - _06/22/2020_
+- `1.0.7-alpha` - _07/09/2021_
+- `1.0.8-alpha` - _03/29/2022_
+- `1.0.9-alpha` - _03/29/2022_
```

### Comparing `BayesABTest-1.0.8/setup.py` & `BayesABTest-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BayesABTest',
-    version='1.0.8',
+    version='1.0.9',
     author='Baker Moran',
     author_email='bamoran99@gmail.com',
     license='MIT',
     description='A package for running AB tests in a Bayesian framework.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['AB Test', 'Bayes', 'Bayesian Statistics'],
     url='https://github.com/bakermoran/BayesABTest',
-    download_url='https://github.com/bakermoran/BayesABTest/archive/v1.0.8-alpha.tar.gz',
+    download_url='https://github.com/bakermoran/BayesABTest/archive/v1.0.9-alpha.tar.gz',
     packages=['BayesABTest'],
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=[
-        'numpy==1.19.5',
-        'pandas==1.1.5',
-        'matplotlib==3.3.4',
-        'seaborn==0.10.1'
+        'numpy>=1.21.0,<1.24.0',
+        'pandas<1.5.0',
+        'matplotlib<4.0.0',
+        'seaborn<0.11.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Mathematics',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9'
     ],
 )
```

