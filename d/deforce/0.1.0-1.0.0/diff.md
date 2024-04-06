# Comparing `tmp/deforce-0.1.0.tar.gz` & `tmp/deforce-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deforce-0.1.0.tar", last modified: Sat Apr  6 10:50:50 2024, max compression
+gzip compressed data, was "deforce-1.0.0.tar", last modified: Sat Apr  6 15:43:02 2024, max compression
```

## Comparing `deforce-0.1.0.tar` & `deforce-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:50:50.996038 deforce-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-06 10:48:36.000000 deforce-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 10:48:36.000000 deforce-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-06 10:48:36.000000 deforce-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-06 10:50:50.996038 deforce-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-06 10:48:36.000000 deforce-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:50:50.988038 deforce-0.1.0/deforce/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:50:50.992038 deforce-0.1.0/deforce/model/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23575 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/model/base_cfn_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/model/base_cfn_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16326 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/model/dfo_cfn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/model/gd_cfn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:50:50.992038 deforce-0.1.0/deforce/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/toolkit/activators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/toolkit/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/toolkit/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/toolkit/scalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-06 10:48:36.000000 deforce-0.1.0/deforce/toolkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:50:50.992038 deforce-0.1.0/deforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-06 10:50:50.000000 deforce-0.1.0/deforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 10:50:50.000000 deforce-0.1.0/deforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:50:50.000000 deforce-0.1.0/deforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 10:50:50.000000 deforce-0.1.0/deforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 10:50:50.000000 deforce-0.1.0/deforce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:50:50.996038 deforce-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-06 10:48:36.000000 deforce-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:50:50.992038 deforce-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-06 10:48:36.000000 deforce-0.1.0/tests/test_CfnClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-06 10:48:36.000000 deforce-0.1.0/tests/test_CfnRegressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-06 10:48:36.000000 deforce-0.1.0/tests/test_DfoCfnClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-06 10:48:36.000000 deforce-0.1.0/tests/test_DfoCfnRegressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:02.045580 deforce-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-06 15:40:54.000000 deforce-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-06 15:40:54.000000 deforce-1.0.0/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 15:40:54.000000 deforce-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-06 15:40:54.000000 deforce-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-06 15:43:02.041580 deforce-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-06 15:40:54.000000 deforce-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:02.037580 deforce-1.0.0/deforce/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:02.041580 deforce-1.0.0/deforce/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23498 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/model/base_cfn_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/model/base_cfn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/model/dfo_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/model/dfo_tune_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18596 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/model/gd_cfn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:02.041580 deforce-1.0.0/deforce/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/toolkit/activators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/toolkit/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/toolkit/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/toolkit/scalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-06 15:40:54.000000 deforce-1.0.0/deforce/toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:02.041580 deforce-1.0.0/deforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-06 15:43:02.000000 deforce-1.0.0/deforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-06 15:43:02.000000 deforce-1.0.0/deforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:43:02.000000 deforce-1.0.0/deforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 15:43:02.000000 deforce-1.0.0/deforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 15:43:02.000000 deforce-1.0.0/deforce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:43:02.045580 deforce-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-06 15:40:54.000000 deforce-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:02.041580 deforce-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-06 15:40:54.000000 deforce-1.0.0/tests/test_CfnClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-06 15:40:54.000000 deforce-1.0.0/tests/test_CfnRegressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-06 15:40:54.000000 deforce-1.0.0/tests/test_DfoCfnClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-06 15:40:54.000000 deforce-1.0.0/tests/test_DfoCfnRegressor.py
```

### Comparing `deforce-0.1.0/CODE_OF_CONDUCT.md` & `deforce-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/LICENSE` & `deforce-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/PKG-INFO` & `deforce-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deforce
-Version: 0.1.0
+Version: 1.0.0
 Summary: deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks
 Home-page: https://github.com/thieu1995/deforce
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://deforce.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/deforce
@@ -51,57 +51,67 @@
 Requires-Dist: flake8>=4.0.1; extra == "dev"
 
 
 ## deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.0-yellow.svg)](https://github.com/thieu1995/deforce/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/deforce/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/deforce) 
 [![PyPI version](https://badge.fury.io/py/deforce.svg)](https://badge.fury.io/py/deforce)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/deforce.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/deforce.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/deforce.svg)
 [![Downloads](https://pepy.tech/badge/deforce)](https://pepy.tech/project/deforce)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/deforce/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/deforce/actions/workflows/publish-package.yaml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/deforce.svg)
 [![Documentation Status](https://readthedocs.org/projects/deforce/badge/?version=latest)](https://deforce.readthedocs.io/en/latest/?badge=latest)
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/deforce.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
-[![DOI](https://zenodo.org/badge/676088001.svg)](https://zenodo.org/doi/10.5281/zenodo.10251021)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10935437.svg)](https://doi.org/10.5281/zenodo.10935437)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-
-deforce (DErivative Free Optimization foR Cascade forward nEural networks) is a Python library that implements variants and the traditional version of Cascade Forward Neural Networks. These include Derivative Free-optimized CFN models (such as GA, PSO, WOA, TLO, DE, ...) and Gradient Descent-optimized CFN models (such as SGD, Adam, Adelta, Adagrad, ...). It provides a comprehensive list of optimizers for training CFN models and is also compatible with the Scikit-Learn library. With deforce, 
-you can perform searches and hyperparameter tuning using the features provided by the Scikit-Learn library.
+`deforce` (DErivative Free Optimization foR Cascade forward nEural networks) is a Python library that implements 
+variants and the traditional version of Cascade Forward Neural Networks. These include Derivative Free-optimized CFN 
+models (such as genetic algorithm, particle swarm optimization, whale optimization algorithm, teaching learning 
+optimization, differential evolution, ...) and Gradient Descent-optimized CFN models (such as stochastic gradient 
+descent, Adam optimizer, Adelta optimizer, ...). It provides a comprehensive list of optimizers for training CFN 
+models and is also compatible with the Scikit-Learn library. With deforce, you can perform searches and 
+hyperparameter tuning for traditional CFN networks using the features provided by the Scikit-Learn library.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Provided Estimator**: CfnRegressor, CfnClassifier, DfoCfnRegressor, DfoCfnClassifier
+* **Provided Estimator**: `CfnRegressor`, `CfnClassifier`, `DfoCfnRegressor`, `DfoCfnClassifier`, `DfoTuneCfn`
 * **Total DFO-based CFN Regressor**: > 200 Models 
 * **Total DFO-based CFN Classifier**: > 200 Models
 * **Total GD-based CFN Regressor**: 12 Models
 * **Total GD-based CFN Classifier**: 12 Models
 * **Supported performance metrics**: >= 67 (47 regressions and 20 classifications)
-* **Supported objective functions (as fitness functions or loss functions)**: >= 67 (47 regressions and 20 classifications)
+* **Supported objective functions**: >= 67 (47 regressions and 20 classifications)
 * **Documentation:** https://deforce.readthedocs.io
 * **Python versions:** >= 3.8.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, torch, skorch
 
 
 # Citation Request 
 
-If you want to understand how Metaheuristic is applied to CFNN, you need to read the paper 
-titled **"Optimization of neural-network model using a meta-heuristic algorithm for the estimation of dynamic Poisson’s ratio of selected rock types"**. 
+If you want to understand how to use Derivative Free-optimized Cascade Forward Neural Network, you 
+need to read the paper titled **"Optimization of neural-network model using a meta-heuristic algorithm for the estimation of dynamic Poisson’s ratio of selected rock types"**. 
 The paper can be accessed at the following [link](https://doi.org/10.1038%2Fs41598-023-38163-0)
 
-
 Please include these citations if you plan to use this library:
 
-```code
+```bibtex
+@software{thieu_deforce_2024,
+  author = {Van Thieu, Nguyen},
+  title = {{deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks}},
+  url = {https://github.com/thieu1995/deforce},
+  doi = {10.5281/zenodo.10935437},
+  year = {2024}
+}
 
 @article{van2023mealpy,
   title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
   author={Van Thieu, Nguyen and Mirjalili, Seyedali},
   journal={Journal of Systems Architecture},
   year={2023},
   publisher={Elsevier},
@@ -113,165 +123,75 @@
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
   pages={129034},
   year={2023},
   publisher={Elsevier}
 }
-
-@article{thieu2019efficient,
-  title={Efficient time-series forecasting using neural network and opposition-based coral reefs optimization},
-  author={Thieu Nguyen, Tu Nguyen and Nguyen, Binh Minh and Nguyen, Giang},
-  journal={International Journal of Computational Intelligence Systems},
-  volume={12},
-  number={2},
-  pages={1144--1161},
-  year={2019}
-}
-
 ```
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/deforce):
 ```sh 
-$ pip install deforce==0.1.0
-```
-
-* Install directly from source code
-```sh 
-$ git clone https://github.com/thieu1995/deforce.git
-$ cd deforce
-$ python setup.py install
+$ pip install deforce
 ```
 
-* In case, you want to install the development version from Github:
-```sh 
-$ pip install git+https://github.com/thieu1995/deforce 
-```
-
-After installation, you can import deforce as any other Python module:
+After installation, check the installed version by:
 
 ```sh
 $ python
 >>> import deforce
 >>> deforce.__version__
 ```
 
 ### Examples
 
-Please check all use cases and examples in folder [examples](examples).
+Please check [documentation website](https://deforce.readthedocs.io/) and [examples folder](examples).
 
-1) deforce provides this useful classes
+1) `deforce` provides this useful classes
 
 ```python
 from deforce import DataTransformer, Data
 from deforce import CfnRegressor, CfnClassifier
 from deforce import DfoCfnRegressor, DfoCfnClassifier
 ```
 
-2) What you can do with `DataTransformer` class
-
-We provide many scaler classes that you can select and make a combination of transforming your data via 
-DataTransformer class. For example: 
-
-2.1) I want to scale data by `Loge` and then `Sqrt` and then `MinMax`:
-
-```python
-from deforce import DataTransformer
-import pandas as pd
-from sklearn.model_selection import train_test_split
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-X_train, y_train, X_test, y_test = train_test_split(X, y, test_size=0.2)
-
-dt = DataTransformer(scaling_methods=("loge", "sqrt", "minmax"))
-X_train_scaled = dt.fit_transform(X_train)
-X_test_scaled = dt.transform(X_test)
-```
-
-2.2) I want to scale data by `YeoJohnson` and then `Standard`:
-
-```python
-from deforce import DataTransformer
-import pandas as pd
-from sklearn.model_selection import train_test_split
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-X_train, y_train, X_test, y_test = train_test_split(X, y, test_size=0.2)
-
-dt = DataTransformer(scaling_methods=("yeo-johnson", "standard"))
-X_train_scaled = dt.fit_transform(X_train)
-X_test_scaled = dt.transform(X_test)
-```
-
-3) What can you do with `Data` class
-+ You can load your dataset into Data class
-+ You can split dataset to train and test set
-+ You can scale dataset without using DataTransformer class
-+ You can scale labels using LabelEncoder
-
-```python
-from deforce import Data
-import pandas as pd
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-
-data = Data(X, y, name="position_salaries")
-
-#### Split dataset into train and test set
-data.split_train_test(test_size=0.2, shuffle=True, random_state=100, inplace=True)
-
-#### Feature Scaling
-data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard", "sqrt", "minmax"))
-data.X_test = scaler_X.transform(data.X_test)
-
-data.y_train, scaler_y = data.encode_label(data.y_train)  # This is for classification problem only
-data.y_test = scaler_y.transform(data.y_test)
-```
-
-4) What can you do with all model classes
-+ Define the model 
-+ Use provides functions to train, predict, and evaluate model
+2) What can you do with all `model` classes
 
 ```python
 from deforce import CfnRegressor, CfnClassifier, DfoCfnRegressor, DfoCfnClassifier
 
 ## Use standard CFN model for regression problem
 regressor = CfnRegressor(hidden_size=50, act1_name="tanh", act2_name="sigmoid", obj_name="MSE",
-                         max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False)
+                         max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False, seed=42)
 
 ## Use standard CFN model for classification problem 
 classifier = CfnClassifier(hidden_size=50, act1_name="tanh", act2_name="sigmoid", obj_name="NLLL",
-                           max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False)
+                           max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False, seed=42)
 
 ## Use Metaheuristic-optimized CFN model for regression problem
 print(DfoCfnClassifier.SUPPORTED_OPTIMIZERS)
 print(DfoCfnClassifier.SUPPORTED_REG_OBJECTIVES)
 
 opt_paras = {"name": "WOA", "epoch": 100, "pop_size": 30}
 regressor = DfoCfnRegressor(hidden_size=50, act1_name="tanh", act2_name="sigmoid",
-                            obj_name="MSE", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
+                            obj_name="MSE", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
 
 ## Use Metaheuristic-optimized CFN model for classification problem
 print(DfoCfnClassifier.SUPPORTED_OPTIMIZERS)
 print(DfoCfnClassifier.SUPPORTED_CLS_OBJECTIVES)
 
 opt_paras = {"name": "WOA", "epoch": 100, "pop_size": 30}
 classifier = DfoCfnClassifier(hidden_size=50, act1_name="tanh", act2_name="softmax",
-                              obj_name="CEL", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
+                              obj_name="CEL", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
 ```
 
-5) What can you do with model object
+3) After you define the `model`, do something with it
++ Use provides functions to train, predict, and evaluate model
 
 ```python
 from deforce import CfnRegressor, Data
 
 data = Data()  # Assumption that you have provide this object like above
 
 model = CfnRegressor(hidden_size=50, act1_name="tanh", act2_name="sigmoid", obj_name="MSE",
@@ -302,30 +222,7 @@
 
 ## Save model
 model.save_model(save_path="history", filename="traditional_CFN.pkl")
 
 ## Load model 
 trained_model = CfnRegressor.load_model(load_path="history", filename="traditional_CFN.pkl")
 ```
-
-# Support (questions, problems)
-
-### Official Links 
-
-* Official source code repo: https://github.com/thieu1995/deforce
-* Official document: https://metapeceptron.readthedocs.io/
-* Download releases: https://pypi.org/project/deforce/
-* Issue tracker: https://github.com/thieu1995/deforce/issues
-* Notable changes log: https://github.com/thieu1995/deforce/blob/master/ChangeLog.md
-* Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
-
-* This project also related to our another projects which are "optimization" and "machine learning", check it here:
-    * https://github.com/thieu1995/mealpy
-    * https://github.com/thieu1995/metaheuristics
-    * https://github.com/thieu1995/opfunu
-    * https://github.com/thieu1995/enoppy
-    * https://github.com/thieu1995/permetrics
-    * https://github.com/thieu1995/MetaCluster
-    * https://github.com/thieu1995/pfevaluator
-    * https://github.com/thieu1995/IntelELM
-    * https://github.com/thieu1995/reflame
-    * https://github.com/aiir-team
```

### Comparing `deforce-0.1.0/README.md` & `deforce-1.0.0/deforce.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,117 @@
+Metadata-Version: 2.1
+Name: deforce
+Version: 1.0.0
+Summary: deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks
+Home-page: https://github.com/thieu1995/deforce
+Author: Thieu
+Author-email: nguyenthieu2102@gmail.com
+License: GPLv3
+Project-URL: Documentation, https://deforce.readthedocs.io/
+Project-URL: Source Code, https://github.com/thieu1995/deforce
+Project-URL: Bug Tracker, https://github.com/thieu1995/deforce/issues
+Project-URL: Change Log, https://github.com/thieu1995/deforce/blob/main/ChangeLog.md
+Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
+Keywords: Cascade Forward Neural Networks,machine learning,artificial intelligence,deep learning,neural networks,single hidden layer network,cascade forward networks,random projection,CFN,CFNN,feed-forward neural network,artificial neural network,classification,regression,supervised learning,online learning,generalization,optimization algorithms,Kernel CFN,Cross-validationGenetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,metaheuristic,metaheuristic algorithms,nature-inspired computing,nature-inspired algorithms,swarm-based computation,metaheuristic-based cascade forward neural networks,metaheuristic-optimized CFN,derivative free-based cascade forward neural networks,derivative free-optimized CFNN,gradient descent-based optimized cascade forward neural network,GD-based CFNN,Performance analysis,Intelligent optimization,Simulations
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Benchmark
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.17.1
+Requires-Dist: scipy>=1.8.1
+Requires-Dist: scikit-learn>=1.2.0
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: mealpy>=3.0.1
+Requires-Dist: permetrics>=2.0.0
+Requires-Dist: torch>=2.0.0
+Requires-Dist: skorch>=0.13.0
+Provides-Extra: dev
+Requires-Dist: pytest>=7.0; extra == "dev"
+Requires-Dist: pytest-cov==4.0.0; extra == "dev"
+Requires-Dist: flake8>=4.0.1; extra == "dev"
+
 
 ## deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.0-yellow.svg)](https://github.com/thieu1995/deforce/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/deforce/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/deforce) 
 [![PyPI version](https://badge.fury.io/py/deforce.svg)](https://badge.fury.io/py/deforce)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/deforce.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/deforce.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/deforce.svg)
 [![Downloads](https://pepy.tech/badge/deforce)](https://pepy.tech/project/deforce)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/deforce/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/deforce/actions/workflows/publish-package.yaml)
 ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/deforce.svg)
 [![Documentation Status](https://readthedocs.org/projects/deforce/badge/?version=latest)](https://deforce.readthedocs.io/en/latest/?badge=latest)
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/deforce.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
-[![DOI](https://zenodo.org/badge/676088001.svg)](https://zenodo.org/doi/10.5281/zenodo.10251021)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10935437.svg)](https://doi.org/10.5281/zenodo.10935437)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-
-deforce (DErivative Free Optimization foR Cascade forward nEural networks) is a Python library that implements variants and the traditional version of Cascade Forward Neural Networks. These include Derivative Free-optimized CFN models (such as GA, PSO, WOA, TLO, DE, ...) and Gradient Descent-optimized CFN models (such as SGD, Adam, Adelta, Adagrad, ...). It provides a comprehensive list of optimizers for training CFN models and is also compatible with the Scikit-Learn library. With deforce, 
-you can perform searches and hyperparameter tuning using the features provided by the Scikit-Learn library.
+`deforce` (DErivative Free Optimization foR Cascade forward nEural networks) is a Python library that implements 
+variants and the traditional version of Cascade Forward Neural Networks. These include Derivative Free-optimized CFN 
+models (such as genetic algorithm, particle swarm optimization, whale optimization algorithm, teaching learning 
+optimization, differential evolution, ...) and Gradient Descent-optimized CFN models (such as stochastic gradient 
+descent, Adam optimizer, Adelta optimizer, ...). It provides a comprehensive list of optimizers for training CFN 
+models and is also compatible with the Scikit-Learn library. With deforce, you can perform searches and 
+hyperparameter tuning for traditional CFN networks using the features provided by the Scikit-Learn library.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Provided Estimator**: CfnRegressor, CfnClassifier, DfoCfnRegressor, DfoCfnClassifier
+* **Provided Estimator**: `CfnRegressor`, `CfnClassifier`, `DfoCfnRegressor`, `DfoCfnClassifier`, `DfoTuneCfn`
 * **Total DFO-based CFN Regressor**: > 200 Models 
 * **Total DFO-based CFN Classifier**: > 200 Models
 * **Total GD-based CFN Regressor**: 12 Models
 * **Total GD-based CFN Classifier**: 12 Models
 * **Supported performance metrics**: >= 67 (47 regressions and 20 classifications)
-* **Supported objective functions (as fitness functions or loss functions)**: >= 67 (47 regressions and 20 classifications)
+* **Supported objective functions**: >= 67 (47 regressions and 20 classifications)
 * **Documentation:** https://deforce.readthedocs.io
 * **Python versions:** >= 3.8.x
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, torch, skorch
 
 
 # Citation Request 
 
-If you want to understand how Metaheuristic is applied to CFNN, you need to read the paper 
-titled **"Optimization of neural-network model using a meta-heuristic algorithm for the estimation of dynamic Poisson’s ratio of selected rock types"**. 
+If you want to understand how to use Derivative Free-optimized Cascade Forward Neural Network, you 
+need to read the paper titled **"Optimization of neural-network model using a meta-heuristic algorithm for the estimation of dynamic Poisson’s ratio of selected rock types"**. 
 The paper can be accessed at the following [link](https://doi.org/10.1038%2Fs41598-023-38163-0)
 
-
 Please include these citations if you plan to use this library:
 
-```code
+```bibtex
+@software{thieu_deforce_2024,
+  author = {Van Thieu, Nguyen},
+  title = {{deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks}},
+  url = {https://github.com/thieu1995/deforce},
+  doi = {10.5281/zenodo.10935437},
+  year = {2024}
+}
 
 @article{van2023mealpy,
   title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
   author={Van Thieu, Nguyen and Mirjalili, Seyedali},
   journal={Journal of Systems Architecture},
   year={2023},
   publisher={Elsevier},
@@ -61,165 +123,75 @@
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
   pages={129034},
   year={2023},
   publisher={Elsevier}
 }
-
-@article{thieu2019efficient,
-  title={Efficient time-series forecasting using neural network and opposition-based coral reefs optimization},
-  author={Thieu Nguyen, Tu Nguyen and Nguyen, Binh Minh and Nguyen, Giang},
-  journal={International Journal of Computational Intelligence Systems},
-  volume={12},
-  number={2},
-  pages={1144--1161},
-  year={2019}
-}
-
 ```
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/deforce):
 ```sh 
-$ pip install deforce==0.1.0
+$ pip install deforce
 ```
 
-* Install directly from source code
-```sh 
-$ git clone https://github.com/thieu1995/deforce.git
-$ cd deforce
-$ python setup.py install
-```
-
-* In case, you want to install the development version from Github:
-```sh 
-$ pip install git+https://github.com/thieu1995/deforce 
-```
-
-After installation, you can import deforce as any other Python module:
+After installation, check the installed version by:
 
 ```sh
 $ python
 >>> import deforce
 >>> deforce.__version__
 ```
 
 ### Examples
 
-Please check all use cases and examples in folder [examples](examples).
+Please check [documentation website](https://deforce.readthedocs.io/) and [examples folder](examples).
 
-1) deforce provides this useful classes
+1) `deforce` provides this useful classes
 
 ```python
 from deforce import DataTransformer, Data
 from deforce import CfnRegressor, CfnClassifier
 from deforce import DfoCfnRegressor, DfoCfnClassifier
 ```
 
-2) What you can do with `DataTransformer` class
-
-We provide many scaler classes that you can select and make a combination of transforming your data via 
-DataTransformer class. For example: 
-
-2.1) I want to scale data by `Loge` and then `Sqrt` and then `MinMax`:
-
-```python
-from deforce import DataTransformer
-import pandas as pd
-from sklearn.model_selection import train_test_split
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-X_train, y_train, X_test, y_test = train_test_split(X, y, test_size=0.2)
-
-dt = DataTransformer(scaling_methods=("loge", "sqrt", "minmax"))
-X_train_scaled = dt.fit_transform(X_train)
-X_test_scaled = dt.transform(X_test)
-```
-
-2.2) I want to scale data by `YeoJohnson` and then `Standard`:
-
-```python
-from deforce import DataTransformer
-import pandas as pd
-from sklearn.model_selection import train_test_split
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-X_train, y_train, X_test, y_test = train_test_split(X, y, test_size=0.2)
-
-dt = DataTransformer(scaling_methods=("yeo-johnson", "standard"))
-X_train_scaled = dt.fit_transform(X_train)
-X_test_scaled = dt.transform(X_test)
-```
-
-3) What can you do with `Data` class
-+ You can load your dataset into Data class
-+ You can split dataset to train and test set
-+ You can scale dataset without using DataTransformer class
-+ You can scale labels using LabelEncoder
-
-```python
-from deforce import Data
-import pandas as pd
-
-dataset = pd.read_csv('Position_Salaries.csv')
-X = dataset.iloc[:, 1:5].values
-y = dataset.iloc[:, 5].values
-
-data = Data(X, y, name="position_salaries")
-
-#### Split dataset into train and test set
-data.split_train_test(test_size=0.2, shuffle=True, random_state=100, inplace=True)
-
-#### Feature Scaling
-data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard", "sqrt", "minmax"))
-data.X_test = scaler_X.transform(data.X_test)
-
-data.y_train, scaler_y = data.encode_label(data.y_train)  # This is for classification problem only
-data.y_test = scaler_y.transform(data.y_test)
-```
-
-4) What can you do with all model classes
-+ Define the model 
-+ Use provides functions to train, predict, and evaluate model
+2) What can you do with all `model` classes
 
 ```python
 from deforce import CfnRegressor, CfnClassifier, DfoCfnRegressor, DfoCfnClassifier
 
 ## Use standard CFN model for regression problem
 regressor = CfnRegressor(hidden_size=50, act1_name="tanh", act2_name="sigmoid", obj_name="MSE",
-                         max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False)
+                         max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False, seed=42)
 
 ## Use standard CFN model for classification problem 
 classifier = CfnClassifier(hidden_size=50, act1_name="tanh", act2_name="sigmoid", obj_name="NLLL",
-                           max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False)
+                           max_epochs=1000, batch_size=32, optimizer="SGD", optimizer_paras=None, verbose=False, seed=42)
 
 ## Use Metaheuristic-optimized CFN model for regression problem
 print(DfoCfnClassifier.SUPPORTED_OPTIMIZERS)
 print(DfoCfnClassifier.SUPPORTED_REG_OBJECTIVES)
 
 opt_paras = {"name": "WOA", "epoch": 100, "pop_size": 30}
 regressor = DfoCfnRegressor(hidden_size=50, act1_name="tanh", act2_name="sigmoid",
-                            obj_name="MSE", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
+                            obj_name="MSE", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
 
 ## Use Metaheuristic-optimized CFN model for classification problem
 print(DfoCfnClassifier.SUPPORTED_OPTIMIZERS)
 print(DfoCfnClassifier.SUPPORTED_CLS_OBJECTIVES)
 
 opt_paras = {"name": "WOA", "epoch": 100, "pop_size": 30}
 classifier = DfoCfnClassifier(hidden_size=50, act1_name="tanh", act2_name="softmax",
-                              obj_name="CEL", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True)
+                              obj_name="CEL", optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
 ```
 
-5) What can you do with model object
+3) After you define the `model`, do something with it
++ Use provides functions to train, predict, and evaluate model
 
 ```python
 from deforce import CfnRegressor, Data
 
 data = Data()  # Assumption that you have provide this object like above
 
 model = CfnRegressor(hidden_size=50, act1_name="tanh", act2_name="sigmoid", obj_name="MSE",
@@ -250,30 +222,7 @@
 
 ## Save model
 model.save_model(save_path="history", filename="traditional_CFN.pkl")
 
 ## Load model 
 trained_model = CfnRegressor.load_model(load_path="history", filename="traditional_CFN.pkl")
 ```
-
-# Support (questions, problems)
-
-### Official Links 
-
-* Official source code repo: https://github.com/thieu1995/deforce
-* Official document: https://metapeceptron.readthedocs.io/
-* Download releases: https://pypi.org/project/deforce/
-* Issue tracker: https://github.com/thieu1995/deforce/issues
-* Notable changes log: https://github.com/thieu1995/deforce/blob/master/ChangeLog.md
-* Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
-
-* This project also related to our another projects which are "optimization" and "machine learning", check it here:
-    * https://github.com/thieu1995/mealpy
-    * https://github.com/thieu1995/metaheuristics
-    * https://github.com/thieu1995/opfunu
-    * https://github.com/thieu1995/enoppy
-    * https://github.com/thieu1995/permetrics
-    * https://github.com/thieu1995/MetaCluster
-    * https://github.com/thieu1995/pfevaluator
-    * https://github.com/thieu1995/IntelELM
-    * https://github.com/thieu1995/reflame
-    * https://github.com/aiir-team
```

### Comparing `deforce-0.1.0/deforce/model/base_cfn_numpy.py` & `deforce-1.0.0/deforce/model/base_cfn_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,19 +280,19 @@
         """
         pred = self.network.predict(X)
         if return_prob:
             return pred
         return self.obj_scaler.inverse_transform(pred)
 
     def __evaluate_reg(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
-        rm = RegressionMetric(y_true=y_true, y_pred=y_pred, decimal=8)
+        rm = RegressionMetric(y_true=y_true, y_pred=y_pred)
         return rm.get_metrics_by_list_names(list_metrics)
 
     def __evaluate_cls(self, y_true, y_pred, list_metrics=("AS", "RS")):
-        cm = ClassificationMetric(y_true, y_pred, decimal=8)
+        cm = ClassificationMetric(y_true, y_pred)
         return cm.get_metrics_by_list_names(list_metrics)
 
     def __score_reg(self, X, y, method="RMSE"):
         """Return the metric of the prediction.
 
         Parameters
         ----------
@@ -309,15 +309,15 @@
         Returns
         -------
         result : float
             The result of selected metric
         """
         method = self._check_method(method, list(self.SUPPORTED_REG_METRICS.keys()))
         y_pred = self.network.predict(X)
-        return RegressionMetric(y, y_pred, decimal=6).get_metric_by_name(method)[method]
+        return RegressionMetric(y, y_pred).get_metric_by_name(method)[method]
 
     def __scores_reg(self, X, y, list_methods=("MSE", "MAE")):
         """Return the list of metrics of the prediction.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
@@ -332,15 +332,15 @@
 
         Returns
         -------
         results : dict
             The results of the list metrics
         """
         y_pred = self.network.predict(X)
-        rm = RegressionMetric(y_true=y, y_pred=y_pred, decimal=6)
+        rm = RegressionMetric(y_true=y, y_pred=y_pred)
         return rm.get_metrics_by_list_names(list_methods)
 
     def __score_cls(self, X, y, method="AS"):
         """
         Return the metric on the given test data and labels.
 
         In multi-label classification, this is the subset accuracy which is a harsh metric
@@ -364,15 +364,15 @@
         """
         method = self._check_method(method, list(self.SUPPORTED_CLS_METRICS.keys()))
         return_prob = False
         if self.n_labels > 2:
             if method in self.CLS_OBJ_LOSSES:
                 return_prob = True
         y_pred = self.predict(X, return_prob=return_prob)
-        cm = ClassificationMetric(y_true=y, y_pred=y_pred, decimal=6)
+        cm = ClassificationMetric(y_true=y, y_pred=y_pred)
         return cm.get_metric_by_name(method)[method]
 
     def __scores_cls(self, X, y, list_methods=("AS", "RS")):
         """
         Return the list of metrics on the given test data and labels.
 
         In multi-label classification, this is the subset accuracy which is a harsh metric
@@ -398,18 +398,18 @@
         list_scores = list((set(self.SUPPORTED_CLS_METRICS.keys()) - set(self.CLS_OBJ_LOSSES)) & set(list_methods))
         t1 = {}
         if len(list_errors) > 0:
             return_prob = False
             if self.n_labels > 2:
                 return_prob = True
             y_pred = self.predict(X, return_prob=return_prob)
-            cm = ClassificationMetric(y, y_pred, decimal=6)
+            cm = ClassificationMetric(y, y_pred)
             t1 = cm.get_metrics_by_list_names(list_errors)
         y_pred = self.predict(X, return_prob=False)
-        cm = ClassificationMetric(y, y_pred, decimal=6)
+        cm = ClassificationMetric(y, y_pred)
         t2 = cm.get_metrics_by_list_names(list_scores)
         return {**t2, **t1}
 
     def evaluate(self, y_true, y_pred, list_metrics=None):
         """Return the list of performance metrics of the prediction.
 
         Parameters
```

### Comparing `deforce-0.1.0/deforce/model/base_cfn_torch.py` & `deforce-1.0.0/deforce/model/base_cfn_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,19 +157,19 @@
         X = torch.tensor(X, dtype=torch.float32)
         if return_prob:
             return self.network.predict_proba(X)
         else:
             return self.network.predict(X)
 
     def __evaluate_reg(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
-        rm = RegressionMetric(y_true=y_true, y_pred=y_pred, decimal=8)
+        rm = RegressionMetric(y_true=y_true, y_pred=y_pred)
         return rm.get_metrics_by_list_names(list_metrics)
 
     def __evaluate_cls(self, y_true, y_pred, list_metrics=("AS", "RS")):
-        cm = ClassificationMetric(y_true, y_pred, decimal=8)
+        cm = ClassificationMetric(y_true, y_pred)
         return cm.get_metrics_by_list_names(list_metrics)
 
     def __score_reg(self, X, y, method="RMSE"):
         """Return the metric of the prediction.
 
         Parameters
         ----------
@@ -186,15 +186,15 @@
         Returns
         -------
         result : float
             The result of selected metric
         """
         method = self._check_method(method, list(self.SUPPORTED_REG_METRICS.keys()))
         y_pred = self.network.predict(X)
-        return RegressionMetric(y, y_pred, decimal=6).get_metric_by_name(method)[method]
+        return RegressionMetric(y, y_pred).get_metric_by_name(method)[method]
 
     def __scores_reg(self, X, y, list_methods=("MSE", "MAE")):
         """Return the list of metrics of the prediction.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
@@ -209,15 +209,15 @@
 
         Returns
         -------
         results : dict
             The results of the list metrics
         """
         y_pred = self.network.predict(X)
-        rm = RegressionMetric(y_true=y, y_pred=y_pred, decimal=6)
+        rm = RegressionMetric(y_true=y, y_pred=y_pred)
         return rm.get_metrics_by_list_names(list_methods)
 
     def __score_cls(self, X, y, method="AS"):
         """
         Return the metric on the given test data and labels.
 
         In multi-label classification, this is the subset accuracy which is a harsh metric
@@ -241,15 +241,15 @@
         """
         method = self._check_method(method, list(self.SUPPORTED_CLS_METRICS.keys()))
         return_prob = False
         if self.n_labels > 2:
             if method in self.CLS_OBJ_LOSSES:
                 return_prob = True
         y_pred = self.predict(X, return_prob=return_prob)
-        cm = ClassificationMetric(y_true=y, y_pred=y_pred, decimal=6)
+        cm = ClassificationMetric(y_true=y, y_pred=y_pred)
         return cm.get_metric_by_name(method)[method]
 
     def __scores_cls(self, X, y, list_methods=("AS", "RS")):
         """
         Return the list of metrics on the given test data and labels.
 
         In multi-label classification, this is the subset accuracy which is a harsh metric
@@ -275,18 +275,18 @@
         list_scores = list((set(self.SUPPORTED_CLS_METRICS.keys()) - set(self.CLS_OBJ_LOSSES)) & set(list_methods))
         t1 = {}
         if len(list_errors) > 0:
             return_prob = False
             if self.n_labels > 2:
                 return_prob = True
             y_pred = self.predict(X, return_prob=return_prob)
-            cm = ClassificationMetric(y, y_pred, decimal=6)
+            cm = ClassificationMetric(y, y_pred)
             t1 = cm.get_metrics_by_list_names(list_errors)
         y_pred = self.predict(X, return_prob=False)
-        cm = ClassificationMetric(y, y_pred, decimal=6)
+        cm = ClassificationMetric(y, y_pred)
         t2 = cm.get_metrics_by_list_names(list_scores)
         return {**t2, **t1}
 
     def evaluate(self, y_true, y_pred, list_metrics=None):
         """Return the list of performance metrics of the prediction.
 
         Parameters
```

### Comparing `deforce-0.1.0/deforce/model/dfo_cfn.py` & `deforce-1.0.0/deforce/model/dfo_cfn.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         Returns
         -------
         result: float
             The fitness value
         """
         self.network.update_weights_from_solution(solution)
         y_pred = self.network.predict(self.X_temp)
-        loss_train = RegressionMetric(self.y_temp, y_pred, decimal=6).get_metric_by_name(self.obj_name)[self.obj_name]
+        loss_train = RegressionMetric(self.y_temp, y_pred).get_metric_by_name(self.obj_name)[self.obj_name]
         return loss_train
 
     def score(self, X, y, method="RMSE"):
         """Return the metric of the prediction.
 
         Parameters
         ----------
@@ -289,15 +289,15 @@
         -------
         result: float
             The fitness value
         """
         self.network.update_weights_from_solution(solution)
         y_pred = self.predict(self.X_temp, return_prob=self.return_prob)
         y1 = self.obj_scaler.inverse_transform(self.y_temp)
-        loss_train = ClassificationMetric(y1, y_pred, decimal=6).get_metric_by_name(self.obj_name)[self.obj_name]
+        loss_train = ClassificationMetric(y1, y_pred).get_metric_by_name(self.obj_name)[self.obj_name]
         return loss_train
 
     def score(self, X, y, method="AS"):
         """
         Return the metric on the given test data and labels.
 
         In multi-label classification, this is the subset accuracy which is a harsh metric
```

### Comparing `deforce-0.1.0/deforce/model/gd_cfn.py` & `deforce-1.0.0/deforce/model/gd_cfn.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/deforce/toolkit/activators.py` & `deforce-1.0.0/deforce/toolkit/activators.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/deforce/toolkit/metrics.py` & `deforce-1.0.0/deforce/toolkit/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 from permetrics.regression import RegressionMetric
 from permetrics.classification import ClassificationMetric
 
 
 def get_metrics(problem, y_true, y_pred, metrics=None, testcase="test"):
     if problem == "regression":
         evaluator = RegressionMetric(y_true, y_pred)
-        paras = [{"decimal": 4}, ] * len(metrics)
     else:
         evaluator = ClassificationMetric(y_true, y_pred)
-        paras = [{"average": "weighted"}, ] * len(metrics)
     if type(metrics) is dict:
         result = evaluator.get_metrics_by_dict(metrics)
     elif type(metrics) in (tuple, list):
-        result = evaluator.get_metrics_by_list_names(metrics, paras)
+        result = evaluator.get_metrics_by_list_names(metrics)
     else:
         raise ValueError("metrics parameter should be a list or dict")
     final_result = {}
     for key, value in result.items():
         if testcase is None or testcase == "":
             final_result[f"{key}"] = value
         else:
```

### Comparing `deforce-0.1.0/deforce/toolkit/preprocessor.py` & `deforce-1.0.0/deforce/toolkit/preprocessor.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/deforce/toolkit/scalers.py` & `deforce-1.0.0/deforce/toolkit/scalers.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/deforce/toolkit/validators.py` & `deforce-1.0.0/deforce/toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/setup.py` & `deforce-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="deforce",
-    version="0.1.0",
+    version="1.0.0",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="deforce: Derivative-Free Algorithms for Optimizing Cascade Forward Neural Networks",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["Cascade Forward Neural Networks", "machine learning", "artificial intelligence",
               "deep learning", "neural networks", "single hidden layer network", "cascade forward networks",
```

### Comparing `deforce-0.1.0/tests/test_CfnClassifier.py` & `deforce-1.0.0/tests/test_CfnClassifier.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/tests/test_CfnRegressor.py` & `deforce-1.0.0/tests/test_CfnRegressor.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/tests/test_DfoCfnClassifier.py` & `deforce-1.0.0/tests/test_DfoCfnClassifier.py`

 * *Files identical despite different names*

### Comparing `deforce-0.1.0/tests/test_DfoCfnRegressor.py` & `deforce-1.0.0/tests/test_DfoCfnRegressor.py`

 * *Files identical despite different names*

