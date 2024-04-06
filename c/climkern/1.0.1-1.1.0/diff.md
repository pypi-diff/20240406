# Comparing `tmp/climkern-1.0.1.tar.gz` & `tmp/climkern-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climkern-1.0.1.tar", last modified: Mon Dec 18 18:14:10 2023, max compression
+gzip compressed data, was "climkern-1.1.0.tar", last modified: Sat Apr  6 17:15:25 2024, max compression
```

## Comparing `climkern-1.0.1.tar` & `climkern-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2023-12-18 18:14:10.246389 climkern-1.0.1/
--rw-rw-r--   0 janoski  (10306) janoski  (10306)     1067 2023-01-11 20:51:22.000000 climkern-1.0.1/LICENSE
--rw-r--r--   0 janoski  (10306) janoski  (10306)     8459 2023-12-18 18:14:10.246389 climkern-1.0.1/PKG-INFO
--rw-rw-r--   0 janoski  (10306) janoski  (10306)     8012 2023-12-07 21:32:59.000000 climkern-1.0.1/README.md
-drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2023-12-18 18:14:10.244389 climkern-1.0.1/climkern/
--rw-rw-r--   0 janoski  (10306) janoski  (10306)      421 2023-12-07 18:33:51.000000 climkern-1.0.1/climkern/__init__.py
--rw-rw-r--   0 janoski  (10306) janoski  (10306)      494 2023-11-30 20:13:15.000000 climkern-1.0.1/climkern/__main__.py
--rw-rw-r--   0 janoski  (10306) janoski  (10306)      635 2023-11-30 19:57:38.000000 climkern-1.0.1/climkern/download.py
--rw-rw-r--   0 janoski  (10306) janoski  (10306)    47532 2023-12-18 17:16:19.000000 climkern-1.0.1/climkern/frontend.py
--rw-rw-r--   0 janoski  (10306) janoski  (10306)     9391 2023-11-29 20:25:05.000000 climkern-1.0.1/climkern/util.py
-drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2023-12-18 18:14:10.245389 climkern-1.0.1/climkern.egg-info/
--rw-r--r--   0 janoski  (10306) janoski  (10306)     8459 2023-12-18 18:14:10.000000 climkern-1.0.1/climkern.egg-info/PKG-INFO
--rw-rw-r--   0 janoski  (10306) janoski  (10306)      301 2023-12-18 18:14:10.000000 climkern-1.0.1/climkern.egg-info/SOURCES.txt
--rw-rw-r--   0 janoski  (10306) janoski  (10306)        1 2023-12-18 18:14:10.000000 climkern-1.0.1/climkern.egg-info/dependency_links.txt
--rw-rw-r--   0 janoski  (10306) janoski  (10306)      102 2023-12-18 18:14:10.000000 climkern-1.0.1/climkern.egg-info/requires.txt
--rw-rw-r--   0 janoski  (10306) janoski  (10306)        9 2023-12-18 18:14:10.000000 climkern-1.0.1/climkern.egg-info/top_level.txt
--rw-rw-r--   0 janoski  (10306) janoski  (10306)       81 2023-01-11 20:46:12.000000 climkern-1.0.1/pyproject.toml
--rw-rw-r--   0 janoski  (10306) janoski  (10306)       38 2023-12-18 18:14:10.246389 climkern-1.0.1/setup.cfg
--rw-rw-r--   0 janoski  (10306) janoski  (10306)      746 2023-12-18 18:12:52.000000 climkern-1.0.1/setup.py
+drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2024-04-06 17:15:25.232181 climkern-1.1.0/
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)     1067 2023-01-11 20:51:22.000000 climkern-1.1.0/LICENSE
+-rw-r--r--   0 janoski  (10306) janoski  (10306)     9404 2024-04-06 17:15:25.231181 climkern-1.1.0/PKG-INFO
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)     8830 2024-04-06 17:14:18.000000 climkern-1.1.0/README.md
+drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2024-04-06 17:15:25.229181 climkern-1.1.0/climkern/
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)      660 2024-03-22 20:18:38.000000 climkern-1.1.0/climkern/__init__.py
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)      497 2024-03-22 20:18:38.000000 climkern-1.1.0/climkern/__main__.py
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)      596 2024-03-23 18:34:04.000000 climkern-1.1.0/climkern/download.py
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)    47574 2024-03-22 20:18:38.000000 climkern-1.1.0/climkern/frontend.py
+drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2024-04-06 17:15:25.230181 climkern-1.1.0/climkern/tests/
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)      433 2024-03-22 20:18:38.000000 climkern-1.1.0/climkern/tests/conftest.py
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)     1217 2024-03-22 20:18:38.000000 climkern-1.1.0/climkern/tests/test_frontend.py
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)     9461 2024-04-06 15:56:39.000000 climkern-1.1.0/climkern/util.py
+drwxrwxr-x   0 janoski  (10306) janoski  (10306)        0 2024-04-06 17:15:25.230181 climkern-1.1.0/climkern.egg-info/
+-rw-r--r--   0 janoski  (10306) janoski  (10306)     9404 2024-04-06 17:15:25.000000 climkern-1.1.0/climkern.egg-info/PKG-INFO
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)      360 2024-04-06 17:15:25.000000 climkern-1.1.0/climkern.egg-info/SOURCES.txt
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)        1 2024-04-06 17:15:25.000000 climkern-1.1.0/climkern.egg-info/dependency_links.txt
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)      149 2024-04-06 17:15:25.000000 climkern-1.1.0/climkern.egg-info/requires.txt
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)        9 2024-04-06 17:15:25.000000 climkern-1.1.0/climkern.egg-info/top_level.txt
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)     1729 2024-04-06 17:14:22.000000 climkern-1.1.0/pyproject.toml
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)       38 2024-04-06 17:15:25.232181 climkern-1.1.0/setup.cfg
+-rw-rw-r--   0 janoski  (10306) janoski  (10306)       38 2024-04-06 17:14:25.000000 climkern-1.1.0/setup.py
```

### Comparing `climkern-1.0.1/LICENSE` & `climkern-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climkern-1.0.1/PKG-INFO` & `climkern-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 Metadata-Version: 2.1
 Name: climkern
-Version: 1.0.1
-Author: Ty Janoski
-Author-email: tjanoski@ccny.cuny.edu
+Version: 1.1.0
+Author-email: Ty Janoski <tyfolino@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray>=0.16.2
 Requires-Dist: cf-xarray>=0.5.1
 Requires-Dist: cftime
 Requires-Dist: xesmf>=0.7.1
-Requires-Dist: esmpy
 Requires-Dist: importlib_resources
 Requires-Dist: pooch
 Requires-Dist: tqdm
 Requires-Dist: plac
 Requires-Dist: netCDF4
+Requires-Dist: esmpy
+Provides-Extra: test
+Requires-Dist: pytest<8,>=7; extra == "test"
+Provides-Extra: lint
+Requires-Dist: precommit>=2.20.0; extra == "lint"
 
 # ClimKern: a Python package for calculating radiative feedbacks
 
 [![DOI](https://zenodo.org/badge/588323813.svg)](https://zenodo.org/doi/10.5281/zenodo.10291284)
 
 ## Citation
 If you use this package or any part of this code, please cite it! Until we have a paper prepared, please cite this package at software.
 
-Janoski, T. P., & Mitevski, I. (2023, December 7). ClimKern (Version 1.0.0). Retrieved from https://pypi.org/project/climkern/1.0.0/. <https://doi.org/10.5281/zenodo.10291284>.
+Janoski, T. P., & Mitevski, I. (2024, April 6). ClimKern (Version 1.1.0). Retrieved from https://pypi.org/project/climkern/1.1.0/. <https://doi.org/10.5281/zenodo.10291284>.
 
 ## Overview
 
 The radiative kernel technique outlined in [Soden & Held (2006)](https://journals.ametsoc.org/view/journals/clim/19/14/jcli3799.1.xml) and [Soden et al. (2008)](https://journals.ametsoc.org/view/journals/clim/21/14/2007jcli2110.1.xml) is commonly used to calculate climate feedbacks. The "kernels" refer to datasets containing the radiative sensitivities of TOA (or surface) radiation to changes in fields such as temperature, specific humidity, and surface albedo; they are typically computed using offline radiative transfer calculations.
 
 ClimKern
 * standardizes the assumptions used in producing radiative feedbacks using kernels
 * simplifies the calculations by giving users access to functions tailored for climate model output
 * provides access to a repository of **12 different radiative kernels** to quantify interkernel spread
 
+The below information is meant to be a quickstart guide, but all functions and capabilities can be found at ClimKern's [documentation site](https://tyfolino.github.io/climkern/).
+
 ## Installation
 
-ClimKern is built on the architecture of Xarray and requires several other packages for compatibility with climate model output. The easiest method to install is to create a new conda environment with prerequisite packages using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) or [mamba](https://mamba-framework.readthedocs.io/en/latest/installation_guide.html):  
-`conda create -n ck_env python=3.9 esmpy xarray xesmf cftime pooch tqdm importlib-resources plac netcdf4 -c conda-forge`  
-or  
-`mamba create -n ck_env python=3.9 esmpy xarray xesmf cftime pooch tqdm importlib-resources plac netcdf4 -c conda-forge` 
-<br></br>Then, activate the environment:  
-`conda activate ck_env`  
-or  
-`mamba activate ck_env` 
-<br></br>
-Finally, install ClimKern with [pip](https://pip.pypa.io/en/stable/#):  
-`pip install -i https://test.pypi.org/simple/ climkern`
-<br></br>
-Once installed, ClimKern requires kernels found on [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10223376). These kernels (and tutorial data) are stored separately because of PyPI size limitations. You can download the kernels easily using the download script included in the package.  
+ClimKern is built on the Xarray architecture and requires several other packages for
+regridding and climate model output compatibility. The easiest method is to create a
+new conda environment using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) or [mamba](https://mamba-framework.readthedocs.io/en/latest/installation_guide.html):
+
+`conda create -n ck_env python=3.10 esmpy -c conda-forge`
+
+A conda environment is necessary because [ESMPy](https://earthsystemmodeling.org/esmpy/), which is required for regridding kernels, is unavailable via `pip`.
+
+Next, activate the new environment:
+
+`conda activate ck_env`
+
+Finally, install ClimKern with [pip](https://pip.pypa.io/en/stable/#):
+
+`pip install climkern`
+
+Once installed, ClimKern requires kernels found on [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10223376). These kernels (and tutorial data) are stored separately because of PyPI size limitations. You can download the kernels easily using the download script included in the package:  
+
 `python -m climkern download`
 
+Note: The kernels & tutorial data are approximately 5.5 GB.
+
+<i>Optional</i>:
+
+You can test your installation via pytest.
+
+```
+pip install pytest
+pytest -v --pyargs climkern
+```
+
+All three tests should pass.
+
 ## Basic tutorial
 ### Temperature, water vapor, and surface albedo feedbacks
 
-This brief tutorial will cover the basics of using ClimKern before more complete documentation can be written (I'm only one person, here!). We start by importing ClimKern and accessing our tutorial data:
+This brief tutorial will cover the basics of using ClimKern. Please check the [documentation](https://tyfolino.github.io/climkern/) for a more complete list of available functions. We start by importing ClimKern and accessing our tutorial data:
 ```python
 import climkern as ck
 
 ctrl,pert = ck.tutorial_data('ctrl'),ck.tutorial_data('pert')
 ```
 
 These datasets have all the necessary variables for computing feedbacks. Let's start with temperature feedbacks.
@@ -145,17 +168,26 @@
     val=(ck.spat_avg(cld_lw)/dTS_glob_avg).mean()))
 ```
 Expected result:
 >`The global average SW cloud feedback is 0.48 W/m^2/K.`
 >
 >`The global average LW cloud feedback is 0.02 W/m^2/K.`
 
+## Troubleshooting
+
+If you are having issues downloading dependencies with `pip`, you can also try adding them to your conda environment with `conda`, i.e.:
+
+`conda install xesmf -c conda-forge`
+
+If you are having trouble downloading the  kernels and tutorial data using the package's download function, you can also download the data directly from the [Zenodo repository](https://zenodo.org/doi/10.5281/zenodo.10223376) and put it in the climkern/data directory located wherever your conda/mamba environments are stored.
+
 ## Other features & coming soon
 ClimKern has several other useful features:
 - Four different methods for calculating water vapor feedbacks.
 - The ability to calculate the "relative humidity" version of all feedbacks following [Held & Shell (2012)](https://journals.ametsoc.org/view/journals/clim/25/8/jcli-d-11-00721.1.xml) and [Zelinka et al. (2020)](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019GL085782).
 - Functions to calculate stratospheric temperature and water vapor feedbacks.
 
-We are continuously updating the package and are working on improved documentation. For now, we recommend exploring the other functions by referencing the package with a "?" in a Jupyter notebook.
+We are continuously updating the package. Please check out the [GitHub issues page](https://github.com/tyfolino/climkern/issues) for this repository for plans for new features.
 
 ## Want to help? Get involved!
-Our hope is that this package will be useful to the climate science community and we appreciate any contributions our fellow scientists and programmers can offer. For more information and to get involved, email Ty at <tjanoski@ccny.cuny.edu>. 
+
+We deeply appreciate contributions from other scientists and programmers and are happy to attribute credit accordingly. If you wish to contribute, please create a fork or branch from the `dev` channel (<b>not</b> `main`) and submit a pull request when you are done with your changes.
```

### Comparing `climkern-1.0.1/README.md` & `climkern-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,66 @@
 # ClimKern: a Python package for calculating radiative feedbacks
 
 [![DOI](https://zenodo.org/badge/588323813.svg)](https://zenodo.org/doi/10.5281/zenodo.10291284)
 
 ## Citation
 If you use this package or any part of this code, please cite it! Until we have a paper prepared, please cite this package at software.
 
-Janoski, T. P., & Mitevski, I. (2023, December 7). ClimKern (Version 1.0.0). Retrieved from https://pypi.org/project/climkern/1.0.0/. <https://doi.org/10.5281/zenodo.10291284>.
+Janoski, T. P., & Mitevski, I. (2024, April 6). ClimKern (Version 1.1.0). Retrieved from https://pypi.org/project/climkern/1.1.0/. <https://doi.org/10.5281/zenodo.10291284>.
 
 ## Overview
 
 The radiative kernel technique outlined in [Soden & Held (2006)](https://journals.ametsoc.org/view/journals/clim/19/14/jcli3799.1.xml) and [Soden et al. (2008)](https://journals.ametsoc.org/view/journals/clim/21/14/2007jcli2110.1.xml) is commonly used to calculate climate feedbacks. The "kernels" refer to datasets containing the radiative sensitivities of TOA (or surface) radiation to changes in fields such as temperature, specific humidity, and surface albedo; they are typically computed using offline radiative transfer calculations.
 
 ClimKern
 * standardizes the assumptions used in producing radiative feedbacks using kernels
 * simplifies the calculations by giving users access to functions tailored for climate model output
 * provides access to a repository of **12 different radiative kernels** to quantify interkernel spread
 
+The below information is meant to be a quickstart guide, but all functions and capabilities can be found at ClimKern's [documentation site](https://tyfolino.github.io/climkern/).
+
 ## Installation
 
-ClimKern is built on the architecture of Xarray and requires several other packages for compatibility with climate model output. The easiest method to install is to create a new conda environment with prerequisite packages using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) or [mamba](https://mamba-framework.readthedocs.io/en/latest/installation_guide.html):  
-`conda create -n ck_env python=3.9 esmpy xarray xesmf cftime pooch tqdm importlib-resources plac netcdf4 -c conda-forge`  
-or  
-`mamba create -n ck_env python=3.9 esmpy xarray xesmf cftime pooch tqdm importlib-resources plac netcdf4 -c conda-forge` 
-<br></br>Then, activate the environment:  
-`conda activate ck_env`  
-or  
-`mamba activate ck_env` 
-<br></br>
-Finally, install ClimKern with [pip](https://pip.pypa.io/en/stable/#):  
-`pip install -i https://test.pypi.org/simple/ climkern`
-<br></br>
-Once installed, ClimKern requires kernels found on [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10223376). These kernels (and tutorial data) are stored separately because of PyPI size limitations. You can download the kernels easily using the download script included in the package.  
+ClimKern is built on the Xarray architecture and requires several other packages for
+regridding and climate model output compatibility. The easiest method is to create a
+new conda environment using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) or [mamba](https://mamba-framework.readthedocs.io/en/latest/installation_guide.html):
+
+`conda create -n ck_env python=3.10 esmpy -c conda-forge`
+
+A conda environment is necessary because [ESMPy](https://earthsystemmodeling.org/esmpy/), which is required for regridding kernels, is unavailable via `pip`.
+
+Next, activate the new environment:
+
+`conda activate ck_env`
+
+Finally, install ClimKern with [pip](https://pip.pypa.io/en/stable/#):
+
+`pip install climkern`
+
+Once installed, ClimKern requires kernels found on [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10223376). These kernels (and tutorial data) are stored separately because of PyPI size limitations. You can download the kernels easily using the download script included in the package:  
+
 `python -m climkern download`
 
+Note: The kernels & tutorial data are approximately 5.5 GB.
+
+<i>Optional</i>:
+
+You can test your installation via pytest.
+
+```
+pip install pytest
+pytest -v --pyargs climkern
+```
+
+All three tests should pass.
+
 ## Basic tutorial
 ### Temperature, water vapor, and surface albedo feedbacks
 
-This brief tutorial will cover the basics of using ClimKern before more complete documentation can be written (I'm only one person, here!). We start by importing ClimKern and accessing our tutorial data:
+This brief tutorial will cover the basics of using ClimKern. Please check the [documentation](https://tyfolino.github.io/climkern/) for a more complete list of available functions. We start by importing ClimKern and accessing our tutorial data:
 ```python
 import climkern as ck
 
 ctrl,pert = ck.tutorial_data('ctrl'),ck.tutorial_data('pert')
 ```
 
 These datasets have all the necessary variables for computing feedbacks. Let's start with temperature feedbacks.
@@ -126,17 +146,26 @@
     val=(ck.spat_avg(cld_lw)/dTS_glob_avg).mean()))
 ```
 Expected result:
 >`The global average SW cloud feedback is 0.48 W/m^2/K.`
 >
 >`The global average LW cloud feedback is 0.02 W/m^2/K.`
 
+## Troubleshooting
+
+If you are having issues downloading dependencies with `pip`, you can also try adding them to your conda environment with `conda`, i.e.:
+
+`conda install xesmf -c conda-forge`
+
+If you are having trouble downloading the  kernels and tutorial data using the package's download function, you can also download the data directly from the [Zenodo repository](https://zenodo.org/doi/10.5281/zenodo.10223376) and put it in the climkern/data directory located wherever your conda/mamba environments are stored.
+
 ## Other features & coming soon
 ClimKern has several other useful features:
 - Four different methods for calculating water vapor feedbacks.
 - The ability to calculate the "relative humidity" version of all feedbacks following [Held & Shell (2012)](https://journals.ametsoc.org/view/journals/clim/25/8/jcli-d-11-00721.1.xml) and [Zelinka et al. (2020)](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019GL085782).
 - Functions to calculate stratospheric temperature and water vapor feedbacks.
 
-We are continuously updating the package and are working on improved documentation. For now, we recommend exploring the other functions by referencing the package with a "?" in a Jupyter notebook.
+We are continuously updating the package. Please check out the [GitHub issues page](https://github.com/tyfolino/climkern/issues) for this repository for plans for new features.
 
 ## Want to help? Get involved!
-Our hope is that this package will be useful to the climate science community and we appreciate any contributions our fellow scientists and programmers can offer. For more information and to get involved, email Ty at <tjanoski@ccny.cuny.edu>. 
+
+We deeply appreciate contributions from other scientists and programmers and are happy to attribute credit accordingly. If you wish to contribute, please create a fork or branch from the `dev` channel (<b>not</b> `main`) and submit a pull request when you are done with your changes.
```

### Comparing `climkern-1.0.1/climkern/frontend.py` & `climkern-1.1.0/climkern/frontend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 # import required packages
-import xarray as xr
-import xesmf as xe
 import warnings
+
 import numpy as np
+import xarray as xr
+import xesmf as xe
 from importlib_resources import files
+from xarray import DataArray
 
 # import functions from util.py
-from climkern.util import *
+# from climkern.util import *
+from .util import *
 
 # change warning format
 warnings.formatwarning = custom_formatwarning
 
 # Apply warning filter to prevent xarray renaming warming
 # Ideally, this will be removed in the future
-warnings.filterwarnings('ignore','.*does not create an index anymore.*')
+warnings.filterwarnings("ignore", ".*does not create an index anymore.*")
+
 
-def calc_alb_feedback(ctrl_rsus,ctrl_rsds,pert_rsus,pert_rsds,kern='GFDL',
-                      sky="all-sky"):
+# def calc_alb_feedback(ctrl_rsus,ctrl_rsds,pert_rsus,pert_rsds,kern='GFDL',
+#                       sky="all-sky"):
+def calc_alb_feedback(
+    ctrl_rsus: DataArray,
+    ctrl_rsds: DataArray,
+    pert_rsus: DataArray,
+    pert_rsds: DataArray,
+    kern: str = "GFDL",
+    sky: str = "all-sky",
+) -> DataArray:
     """
     Calculate the radiative perturbation (W/m^2) from changes in surface
     albedo using user-specified radiative kernel. Horizontal resolution
     is kept at input data's resolution.
-    
+
     Parameters
     ----------
     ctrl_rsus : xarray DataArray
         DataArray containing the upwelling SW radiation at the surface in the
         control simulation. Must be 3D with coordinates of time, latitude, and
         longitude with units of W/m^2.
-        
+
     ctrl_rsds : xarray DataArray
         DataArray containing the downwelling SW radiation at the surface in
         the control simulation. Must be 3D with coordinates of time, latitude,
         and longitude with units of W/m^2.
-        
+
     pert_rsus : xarray DataArray
         DataArray containing the upwelling SW radiation at the surface in the
         perturbed simulation. Must be 3D with coordinates of time, latitude,
         and longitude with units of W/m^2.
-        
+
     pert_rsds : xarray DataArray
         DataArray containing the downwelling SW radiation at the surface in
-        the perturbed simulation. Must be 3D with coordinates of time, 
+        the perturbed simulation. Must be 3D with coordinates of time,
         latitude, and longitude with units of W/m^2.
 
     kern : string, optional
         String specifying the name of the desired kernel. Defaults to "GFDL".
 
     sky : string, optional
         String, either "all-sky" or "clear-sky", specifying whether to
@@ -55,89 +67,105 @@
     -------
     alb_feedback : xarray DataArray
         3D DataArray containing radiative perturbations at TOA caused by
         changes in surface albedo with coordinates of time, latitude, and
         longitude.
     """
     # get correct key for all-sky or clear-sky
-    alb_key = 'sw_a' if check_sky(sky)=='all-sky' else 'swclr_a'
+    alb_key = "sw_a" if check_sky(sky) == "all-sky" else "swclr_a"
 
     # check input coordinates
-    for d in [ctrl_rsus,ctrl_rsds,pert_rsus,pert_rsds]:
+    for d in [ctrl_rsus, ctrl_rsds, pert_rsus, pert_rsds]:
         d = check_coords(d)
 
     # calculate albedo and create control climatology
-    ctrl_alb_clim = make_clim(get_albedo(ctrl_rsus,ctrl_rsds))
+    ctrl_alb_clim = make_clim(get_albedo(ctrl_rsus, ctrl_rsds))
     pert_alb = get_albedo(pert_rsus, pert_rsds)
-        
+
     # tile climatology and take difference
-    ctrl_alb_clim_tiled = tile_data(ctrl_alb_clim,pert_alb)
+    ctrl_alb_clim_tiled = tile_data(ctrl_alb_clim, pert_alb)
     diff_alb = pert_alb - ctrl_alb_clim_tiled
-    
+
     # read in and regrid surface albedo kernel
     kernel = get_kern(kern)
-    regridder = xe.Regridder(kernel[alb_key],diff_alb,method='bilinear',
-                             reuse_weights=False,periodic=True,
-                            extrap_method='nearest_s2d')
-    kernel = tile_data(regridder(kernel[alb_key]),diff_alb)
-    
+    regridder = xe.Regridder(
+        kernel[alb_key],
+        diff_alb,
+        method="bilinear",
+        reuse_weights=False,
+        periodic=True,
+        extrap_method="nearest_s2d",
+    )
+    kernel = tile_data(regridder(kernel[alb_key]), diff_alb)
+
     # calculate feedbacks
     # the 100 is to convert albedo to percent
     alb_feedback = diff_alb * kernel * 100
     return alb_feedback
 
-def calc_T_feedbacks(ctrl_ta,ctrl_ts,ctrl_ps,pert_ta,pert_ts,pert_ps,
-                     pert_trop=None,kern='GFDL',sky='all-sky',fixRH=False):
+
+def calc_T_feedbacks(
+    ctrl_ta,
+    ctrl_ts,
+    ctrl_ps,
+    pert_ta,
+    pert_ts,
+    pert_ps,
+    pert_trop=None,
+    kern="GFDL",
+    sky="all-sky",
+    fixRH=False,
+):
     """
     Calculate the raditive pertubations (W/m^2) at the TOA from changes in
     surface skin and air temperature using user-specified kernel. Horizontal
     resolution is kept at input data's resolution.
-    
+
     Parameters
     ----------
     ctrl_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the
         control simulation. 4D with coordinates of time, latitude, longitude,
         and pressure level and units of K.
-        
+
     ctrl_ts : xarray DataArray
-        DataArray containing surface skin temperature in the control 
+        DataArray containing surface skin temperature in the control
         simulation. 3D with coordinates of time, latitude, and longitude
         and units of K.
-        
+
     ctrl_ps : xarray DataArray
-        DataArray containing surface pressure in the control simulation. 3D 
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        DataArray containing surface pressure in the control simulation. 3D
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the
-        perturbed simulation. 4D with coordinates of time, latitude, 
+        perturbed simulation. 4D with coordinates of time, latitude,
         longitude, and pressure level and units of K.
-        
+
     pert_ts : xarray DataArray
-        DataArray containing surface skin temperature in the perturbed 
+        DataArray containing surface skin temperature in the perturbed
         simulation. 3D with coordinates of time, latitude, and longitude
         and units of K.
-        
+
     pert_ps : xarray DataArray
         DataArray containing surface pressure in the perturbed simulation. 3D
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_trop : xarray DataArray, optional
         DataArray containing tropopause pressure in the perturbed simulation.
         3D with coordinates of time, latitude, and longitude and units of Pa
         or hPa. If not provided, ClimKern will assume a tropopause height of
         300 hPa at the equator, linearly decreasing with the cosine of
         latitude to 100 hPa at the poles.
 
     kern : string, optional
         String specifying the name of the desired kernel. Defaults to "GFDL".
-        
+
     sky : string, optional
         String, either "all-sky" or "clear-sky", specifying whether to
         calculate the all-sky or clear-sky feedbacks. Defaults to "all-sky".
 
     fixRH : boolean, optional
         Specifies whether to calculate alternative Planck and lapse rate
         feedbacks using relative humidity as a state variable, as outlined
@@ -145,133 +173,148 @@
 
     Returns
     -------
     lr_feedback : xarray DataArray
         3D DataArray containing radiative perturbations at TOA caused by
         changes in tropospheric lapse rate with coordinates of time, latitude,
         and longitude.
-        
+
     planck_feedback : xarray DataArray
         3D DataArray containing radiative perturbations at TOA caused by
-        vertically-uniform temperature change with coordinates of time, 
+        vertically-uniform temperature change with coordinates of time,
         latitude, and longitude.
     """
     # get correct keys for all-sky or clear-sky
-    t_key = 'lw_t' if check_sky(sky)=='all-sky' else 'lwclr_t'
-    ts_key = 'lw_ts' if sky=='all-sky' else 'lwclr_ts'
+    t_key = "lw_t" if check_sky(sky) == "all-sky" else "lwclr_t"
+    ts_key = "lw_ts" if sky == "all-sky" else "lwclr_ts"
 
     # if using RH as a state variable, read in water vapor kernels too
-    if(fixRH==True):
-        qlw_key = 'lw_q' if sky=='all-sky' else 'lwclr_q'
-        qsw_key = 'sw_q' if sky=='all-sky' else 'swclr_q'
+    if fixRH is True:
+        qlw_key = "lw_q" if sky == "all-sky" else "lwclr_q"
+        qsw_key = "sw_q" if sky == "all-sky" else "swclr_q"
 
     # check input coordinates
-    for d in [ctrl_ta,pert_ta]:
-        d = check_coords(d,ndim=4)
-    for d in [ctrl_ts,ctrl_ps,pert_ts,pert_ps]:
+    for d in [ctrl_ta, pert_ta]:
+        d = check_coords(d, ndim=4)
+    for d in [ctrl_ts, ctrl_ps, pert_ts, pert_ps]:
         d = check_coords(d)
 
     # check input units
-    ctrl_ta = check_var_units(check_plev_units(ctrl_ta),'T')
-    pert_ta = check_var_units(check_plev_units(pert_ta),'T')
-    ctrl_ts = check_var_units(ctrl_ts,'T')
-    pert_ts = check_var_units(pert_ts,'T')
-    ctrl_ps = check_pres_units(ctrl_ps,"ctrl PS")
-    pert_ps = check_pres_units(pert_ps,"pert PS")
+    ctrl_ta = check_var_units(check_plev_units(ctrl_ta), "T")
+    pert_ta = check_var_units(check_plev_units(pert_ta), "T")
+    ctrl_ts = check_var_units(ctrl_ts, "T")
+    pert_ts = check_var_units(pert_ts, "T")
+    ctrl_ps = check_pres_units(ctrl_ps, "ctrl PS")
+    pert_ps = check_pres_units(pert_ps, "pert PS")
 
     # check tropopause units if provided by user, else create dummy tropopause
-    if(type(pert_trop) == type(None)):
+    if type(pert_trop) == type(None):
         pert_trop = make_tropo(ctrl_ps)
     else:
         pert_trop = check_coords(pert_trop)
-        pert_trop = check_pres_units(pert_trop,"pert tropopause")
+        pert_trop = check_pres_units(pert_trop, "pert tropopause")
 
     # mask values below the surface & make climatology
     ctrl_ps_clim = make_clim(ctrl_ps)
     ctrl_ta_clim = make_clim(ctrl_ta)
     ctrl_ta_clim = ctrl_ta_clim.where(ctrl_ta_clim.plev < ctrl_ps_clim)
     ctrl_ts_clim = make_clim(ctrl_ts)
-    
+
     # calculate change in air and surface skin temperature
-    diff_ta = (pert_ta - tile_data(ctrl_ta_clim,pert_ta))
-    diff_ts = pert_ts - tile_data(ctrl_ts_clim,pert_ts)
-    
+    diff_ta = pert_ta - tile_data(ctrl_ta_clim, pert_ta)
+    diff_ts = pert_ts - tile_data(ctrl_ts_clim, pert_ts)
+
     # read in and regrid temperature kernel
     kernel = check_plev(get_kern(kern))
-    regridder = xe.Regridder(kernel[t_key],diff_ts,method='bilinear',
-                             reuse_weights=False,periodic=True,
-                            extrap_method='nearest_s2d')
-    ta_kernel = tile_data(regridder(kernel[t_key]),diff_ta)
-    ts_kernel = tile_data(regridder(kernel[ts_key],skipna=True),diff_ta)
+    regridder = xe.Regridder(
+        kernel[t_key],
+        diff_ts,
+        method="bilinear",
+        reuse_weights=False,
+        periodic=True,
+        extrap_method="nearest_s2d",
+    )
+    ta_kernel = tile_data(regridder(kernel[t_key]), diff_ta)
+    ts_kernel = tile_data(regridder(kernel[ts_key], skipna=True), diff_ta)
 
     # repeat process for water vapor kernels if using RH
-    if(fixRH==True):
-        qlw_kernel = tile_data(regridder(kernel[qlw_key]),diff_ta)
-        qsw_kernel = tile_data(regridder(kernel[qsw_key]),diff_ta)
+    if fixRH is True:
+        qlw_kernel = tile_data(regridder(kernel[qlw_key]), diff_ta)
+        qsw_kernel = tile_data(regridder(kernel[qsw_key]), diff_ta)
         # overwrite ta_kernel to include q kernel
         ta_kernel = ta_kernel + qlw_kernel + qsw_kernel
 
     # regrid temperature differences to kernel pressure levels
     # we have to extrapolate in case the lowest model plev is above the
     # kernel's.
-    
-    diff_ta = diff_ta.interp_like(ta_kernel,kwargs={
-        "fill_value": "extrapolate"})
+
+    diff_ta = diff_ta.interp_like(ta_kernel, kwargs={"fill_value": "extrapolate"})
 
     # use get_dp in climkern.util to calculate layer thickness
-    dp = get_dp(diff_ta,pert_ps,pert_trop,layer='troposphere')
-    
+    dp = get_dp(diff_ta, pert_ps, pert_trop, layer="troposphere")
+
     # calculate feedbacks
     # for lapse rate, use the deviation of the air temperature response
     # from vertically uniform warming
-    lr_feedback = ((ta_kernel * (diff_ta - diff_ts).fillna(0)) * dp/10000
-                  ).sum(dim='plev',min_count=1)
-    
-    # for planck, assume vertically uniform warming and 
-    # account for surface temperature change
-    planck_feedback = ((ts_kernel * diff_ts) + (ta_kernel * xr.broadcast(
-        diff_ts,diff_ta)[0].fillna(0) * dp/10000).sum(dim='plev',min_count=1))
-       
-    return(lr_feedback,planck_feedback)
-
+    lr_feedback = ((ta_kernel * (diff_ta - diff_ts).fillna(0)) * dp / 10000).sum(
+        dim="plev", min_count=1
+    )
 
-def calc_q_feedbacks(ctrl_q,ctrl_ta,ctrl_ps,pert_q,pert_ps,pert_trop=None,
-                     kern='GFDL',sky='all-sky',method='pendergrass'):
+    # for planck, assume vertically uniform warming and
+    # account for surface temperature change
+    planck_feedback = (ts_kernel * diff_ts) + (
+        ta_kernel * xr.broadcast(diff_ts, diff_ta)[0].fillna(0) * dp / 10000
+    ).sum(dim="plev", min_count=1)
+
+    return (lr_feedback, planck_feedback)
+
+
+def calc_q_feedbacks(
+    ctrl_q,
+    ctrl_ta,
+    ctrl_ps,
+    pert_q,
+    pert_ps,
+    pert_trop=None,
+    kern="GFDL",
+    sky="all-sky",
+    method="pendergrass",
+):
     """
-    Calculate the raditive pertubations (W/m^2), LW & SW, at the TOA from 
+    Calculate the raditive pertubations (W/m^2), LW & SW, at the TOA from
     changes in specific humidity using user-specified kernel. Horizontal
     resolution is kept at input data's resolution.
-    
+
     Parameters
     ----------
     ctrl_q : xarray DataArray
         DataArray containing specific humidity on pressure levels in the
         control simulation. 4D with coordinates of time, latitude, longitude,
         and pressure level and units of "1", "kg/kg", or "g/kg".
 
     ctrl_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the
         control simulation. 4D with coordinates of time, latitude, longitude,
         and pressure level and units of K.
-        
+
     ctrl_ps : xarray DataArray
-        DataArray containing surface pressure in the control simulation. 3D 
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        DataArray containing surface pressure in the control simulation. 3D
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_q : xarray DataArray
         DataArray containing specific humidity on pressure levels in the
-        perturbed simulation. 4D with coordinates of time, latitude, 
+        perturbed simulation. 4D with coordinates of time, latitude,
         longitude, and pressure level and units of "1", "kg/kg", or "g/kg".
-        
+
     pert_ps : xarray DataArray
         DataArray containing surface pressure in the perturbed simulation. 3D
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_trop : xarray DataArray, optional
         DataArray containing tropopause pressure in the perturbed simulation.
         3D with coordinates of time, latitude, and longitude and units of Pa
         or hPa. If not provided, ClimKern will assume a tropopause height of
         300 hPa at the equator, linearly decreasing with the cosine of
         latitude to 100 hPa at the poles.
 
@@ -281,253 +324,265 @@
     sky : string, optional
         String, either "all-sky" or "clear-sky", specifying whether to
         calculate the all-sky or clear-sky feedbacks. Defaults to "all-sky".
 
     method : string, optional
         Specifies the method to use to calculate the specific humidity
         feedback. Options are "pendergrass" (default), "kramer", "zelinka",
-        and "linear". 
+        and "linear".
 
     Returns
     -------
     lw_q_feedback : xarray DataArray
         3D DataArray containing LW radiative perturbations at TOA caused by
         changes in specific humidity with coordinates of time, latitude,
         and longitude.
-        
+
     sw_q_feedback : xarray DataArray
         3D DataArray containing SW radiative perturbations at TOA caused by
         changes in specific humidity with coordinates of time, latitude,
         and longitude.
     """
     # get correct keys for all-sky or clear-sky
-    qlw_key = 'lw_q' if check_sky(sky)=='all-sky' else 'lwclr_q'
-    qsw_key = 'sw_q' if sky=='all-sky' else 'swclr_q'
+    qlw_key = "lw_q" if check_sky(sky) == "all-sky" else "lwclr_q"
+    qsw_key = "sw_q" if sky == "all-sky" else "swclr_q"
 
     # check input coordinates
-    for d in [ctrl_q,ctrl_ta,pert_q]:
-        d = check_coords(d,ndim=4)
-    for d in [ctrl_ps,pert_ps]:
+    for d in [ctrl_q, ctrl_ta, pert_q]:
+        d = check_coords(d, ndim=4)
+    for d in [ctrl_ps, pert_ps]:
         d = check_coords(d)
 
     # check input units
-    ctrl_ta = check_var_units(check_plev_units(ctrl_ta),'T')
-    ctrl_q = check_var_units(check_plev_units(ctrl_q),'q')
-    pert_q = check_var_units(check_plev_units(pert_q),'q')
-    ctrl_ps = check_pres_units(ctrl_ps,"ctrl PS")
-    pert_ps = check_pres_units(pert_ps,"pert PS")
+    ctrl_ta = check_var_units(check_plev_units(ctrl_ta), "T")
+    ctrl_q = check_var_units(check_plev_units(ctrl_q), "q")
+    pert_q = check_var_units(check_plev_units(pert_q), "q")
+    ctrl_ps = check_pres_units(ctrl_ps, "ctrl PS")
+    pert_ps = check_pres_units(pert_ps, "pert PS")
 
     # check tropopause units if provided by user, else create dummy tropopause
-    if(type(pert_trop) == type(None)):
+    if type(pert_trop) == type(None):
         pert_trop = make_tropo(ctrl_ps)
     else:
         pert_trop = check_coords(pert_trop)
-        pert_trop = check_pres_units(pert_trop,"pert tropopause")
-    
+        pert_trop = check_pres_units(pert_trop, "pert tropopause")
+
     # mask values below the surface & make climatology
     ctrl_ps_clim = make_clim(ctrl_ps)
     ctrl_q_clim = make_clim(ctrl_q)
-    ctrl_q_clim = ctrl_q_clim.where(ctrl_q_clim.plev<ctrl_ps_clim)
+    ctrl_q_clim = ctrl_q_clim.where(ctrl_q_clim.plev < ctrl_ps_clim)
     ctrl_ta_clim = make_clim(ctrl_ta)
-    ctrl_ta_clim = ctrl_ta_clim.where(ctrl_ta_clim.plev<ctrl_ps_clim)
+    ctrl_ta_clim = ctrl_ta_clim.where(ctrl_ta_clim.plev < ctrl_ps_clim)
 
-    # if q has units of unity or kg/kg, we will have to 
+    # if q has units of unity or kg/kg, we will have to
     # multiply by 1000 later on to make it g/kg
-    if(ctrl_q.units in ['1','kg/kg']):
+    if ctrl_q.units in ["1", "kg/kg"]:
         conv_factor = 1000
-    elif(ctrl_q.units in ['g/kg']):
+    elif ctrl_q.units in ["g/kg"]:
         conv_factor = 1
     else:
         warnings.warn("Cannot determine units of q. Assuming kg/kg.")
         conv_factor = 1000
 
     # tile control climatology to match length of pert simulation time dim
-    ctrl_q_clim_tiled = tile_data(ctrl_q_clim,pert_q)
+    ctrl_q_clim_tiled = tile_data(ctrl_q_clim, pert_q)
 
     # calculate specific humidity response using user-specified method
-    if(method=='pendergrass'):
-        diff_q = (pert_q - ctrl_q_clim_tiled)/ctrl_q_clim_tiled
-    elif(method=='linear'):
+    if method == "pendergrass":
+        diff_q = (pert_q - ctrl_q_clim_tiled) / ctrl_q_clim_tiled
+    elif method == "linear":
         diff_q = pert_q - ctrl_q_clim_tiled
-    elif(method in ['kramer','zelinka']):
-        diff_q = np.log(pert_q.where(pert_q>0)) - np.log(
-            ctrl_q_clim_tiled.where(ctrl_q_clim_tiled>0))
+    elif method in ["kramer", "zelinka"]:
+        diff_q = np.log(pert_q.where(pert_q > 0)) - np.log(
+            ctrl_q_clim_tiled.where(ctrl_q_clim_tiled > 0)
+        )
     else:
-        raise ValueError(
-            "Please select a valid choice for the method argument.")
-    
+        raise ValueError("Please select a valid choice for the method argument.")
+
     # read in and regrid water vapor kernel
     kernel = check_plev(get_kern(kern))
-    regridder = xe.Regridder(kernel[qlw_key],diff_q,method='bilinear',
-                             extrap_method="nearest_s2d",
-                             reuse_weights=False,periodic=True)
+    regridder = xe.Regridder(
+        kernel[qlw_key],
+        diff_q,
+        method="bilinear",
+        extrap_method="nearest_s2d",
+        reuse_weights=False,
+        periodic=True,
+    )
 
-    qlw_kernel = tile_data(regridder(kernel[qlw_key],skipna=True),diff_q)
-    qsw_kernel = tile_data(regridder(kernel[qsw_key],skipna=True),diff_q)  
+    qlw_kernel = tile_data(regridder(kernel[qlw_key], skipna=True), diff_q)
+    qsw_kernel = tile_data(regridder(kernel[qsw_key], skipna=True), diff_q)
 
     # regrid T/q to kernel pressure levels
     # we have to extrapolate in case the lowest model plev is above the
     # kernel's.
-    kwargs = {'fill_value':'extrapolate'}
-    diff_q = diff_q.interp_like(qlw_kernel,kwargs=kwargs)
-    ctrl_q_clim = ctrl_q_clim.interp(plev=qlw_kernel.plev,kwargs=kwargs)
-    ctrl_q_clim.plev.attrs['units'] = ctrl_q.plev.units
-    ctrl_ta_clim = ctrl_ta_clim.interp(plev=qlw_kernel.plev,kwargs=kwargs)
-    ctrl_ta_clim.plev.attrs['units'] = ctrl_ta.plev.units
+    kwargs = {"fill_value": "extrapolate"}
+    diff_q = diff_q.interp_like(qlw_kernel, kwargs=kwargs)
+    ctrl_q_clim = ctrl_q_clim.interp(plev=qlw_kernel.plev, kwargs=kwargs)
+    ctrl_q_clim.plev.attrs["units"] = ctrl_q.plev.units
+    ctrl_ta_clim = ctrl_ta_clim.interp(plev=qlw_kernel.plev, kwargs=kwargs)
+    ctrl_ta_clim.plev.attrs["units"] = ctrl_ta.plev.units
 
     # create the normalization factor, which corresponds to the increase
     # in specific humidity for a 1K increate in temperature
-    norm = tile_data(calc_q_norm(ctrl_ta_clim,ctrl_q_clim,method=method),
-                     diff_q)
-    
+    norm = tile_data(calc_q_norm(ctrl_ta_clim, ctrl_q_clim, method=method), diff_q)
+
     # use get_dp in climkern.util to calculate layer thickness
-    dp = get_dp(diff_q,pert_ps,pert_trop,layer='troposphere')
-                    
+    dp = get_dp(diff_q, pert_ps, pert_trop, layer="troposphere")
+
     # calculate feedbacks
-    qlw_feedback = (qlw_kernel/norm * diff_q * conv_factor * dp/10000).sum(
-        dim='plev',min_count=1)
-    qsw_feedback = (qsw_kernel/norm * diff_q * conv_factor * dp/10000).sum(
-        dim='plev',min_count=1).fillna(0)
+    qlw_feedback = (qlw_kernel / norm * diff_q * conv_factor * dp / 10000).sum(
+        dim="plev", min_count=1
+    ).drop_vars("units")
+    qsw_feedback = (
+        (qsw_kernel / norm * diff_q * conv_factor * dp / 10000)
+        .sum(dim="plev", min_count=1)
+        .fillna(0)
+    ).drop_vars("units")
 
     # one complication: CloudSat needs to be masked so we don't fill the NaNs
     # with zeros
-    if(kern=='CloudSat'):
-        qsw_feedback = qsw_feedback.where(qsw_kernel.sum(
-            dim='plev',min_count=1).notnull())
-    
-    return(qlw_feedback,qsw_feedback)
+    if kern == "CloudSat":
+        qsw_feedback = qsw_feedback.where(
+            qsw_kernel.sum(dim="plev", min_count=1).notnull()
+        )
+
+    return (qlw_feedback, qsw_feedback)
 
-def calc_dCRE_SW(ctrl_FSNT,pert_FSNT,ctrl_FSNTC,pert_FSNTC):
+
+def calc_dCRE_SW(ctrl_FSNT, pert_FSNT, ctrl_FSNTC, pert_FSNTC):
     """
     Calculate the change in the SW cloud radiative effect at the TOA.
 
     Parameters
     ----------
     ctrl_FSNT : xarray DataArray
         Three-dimensional DataArray containing the all-sky net shortwave flux
         at the top-of-atmosphere in the control simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards/incoming.
-        
+
     pert_FSNT : xarray DataArray
         Three-dimensional DataArray containing the all-sky net shortwave flux
         at the top-of-atmosphere in the perturbed simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards/incoming.
 
     ctrl_FSNTC : xarray DataArray
-        Three-dimensional DataArray containing the clear-sky net shortwave 
+        Three-dimensional DataArray containing the clear-sky net shortwave
         flux at the top-of-atmosphere in the control simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards/incoming.
-        
+
     pert_FSNTC : xarray DataArray
-        Three-dimensional DataArray containing the clear-sky net shortwave 
+        Three-dimensional DataArray containing the clear-sky net shortwave
         flux at the top-of-atmosphere in the perturbed simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards/incoming.
-    
+
 
     Returns
     -------
     dCRE_SW : xarray DataArray
         Three-dimensional DataArray containing the change in shortwave cloud
-        radiative effect at the top-of-atmosphere with coords of time, lat, 
+        radiative effect at the top-of-atmosphere with coords of time, lat,
         and lon and units of Wm^-2. positive = downwards.
     """
     # double check the signs of SW fluxes
     sw_coeff = -1 if ctrl_FSNT.mean() < 0 else 1
 
     ctrl_CRE_SW = sw_coeff * (ctrl_FSNT - ctrl_FSNTC)
     pert_CRE_SW = sw_coeff * (pert_FSNT - pert_FSNTC)
 
-    return(pert_CRE_SW - ctrl_CRE_SW)
+    return pert_CRE_SW - ctrl_CRE_SW
+
 
-def calc_dCRE_LW(ctrl_FLNT,pert_FLNT,ctrl_FLNTC,pert_FLNTC):
+def calc_dCRE_LW(ctrl_FLNT, pert_FLNT, ctrl_FLNTC, pert_FLNTC):
     """
     Calculate the change in the LW cloud radiative effect at the TOA.
 
     Parameters
     ----------
     ctrl_FLNT : xarray DataArray
         Three-dimensional DataArray containing the all-sky net longwave flux
         at the top-of-atmosphere in the control simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards.
-        
+
     pert_FLNT : xarray DataArray
         Three-dimensional DataArray containing the all-sky net longwave flux
         at the top-of-atmosphere in the perturbed simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards.
 
     ctrl_FLNTC : xarray DataArray
         Three-dimensional DataArray containing the clear-sky net longwave flux
         at the top-of-atmosphere in the control simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards.
-        
+
     pert_FLNTC : xarray DataArray
         Three-dimensional DataArray containing the clear-sky net longwave flux
         at the top-of-atmosphere in the perturbed simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards.
-    
+
 
     Returns
     -------
     dCRE_LW : xarray DataArray
         Three-dimensional DataArray containing the change in longwave cloud
-        radiative effect at the top-of-atmosphere with coords of time, lat, 
+        radiative effect at the top-of-atmosphere with coords of time, lat,
         and lon and units of Wm^-2. positive = downwards.
     """
     # double check the signs of LW/SW fluxes
     lw_coeff = -1 if ctrl_FLNT.mean() > 0 else 1
 
     ctrl_CRE_LW = lw_coeff * (ctrl_FLNT - ctrl_FLNTC)
     pert_CRE_LW = lw_coeff * (pert_FLNT - pert_FLNTC)
 
-    return(pert_CRE_LW - ctrl_CRE_LW)
+    return pert_CRE_LW - ctrl_CRE_LW
+
 
-def calc_cloud_LW(t_as,t_cs,q_lwas,q_lwcs,dCRE_lw,IRF_lwas,IRF_lwcs):
+def calc_cloud_LW(t_as, t_cs, q_lwas, q_lwcs, dCRE_lw, IRF_lwas, IRF_lwcs):
     """
     Calculate the radiative perturbation from the longwave cloud feedback
     using the adjustment method outlined in Soden et al. (2008).
 
     Parameters
     ----------
     t_as : xarray DataArray
-        DataArray containing the vertically integrated all-sky radiative 
-        perturbation at the TOA from the total temperature feedback. The 
+        DataArray containing the vertically integrated all-sky radiative
+        perturbation at the TOA from the total temperature feedback. The
         total temperature feedback is the sum of the Planck and lapse rate
         feedbacks. Should have dims of lat, lon, and time.
 
     t_cs : xarray DataArray
-        DataArray containing the vertically integrated clear-sky radiative 
-        perturbation at the TOA from the total temperature feedback. The 
+        DataArray containing the vertically integrated clear-sky radiative
+        perturbation at the TOA from the total temperature feedback. The
         total temperature feedback is the sum of the Planck and lapse rate
         feedbacks. Should have dims of lat, lon, and time.
 
     q_lwas : xarray DataArray
         DataArray containing the vertically integrated LW all-sky radiative
-        perturbation at the TOA from the water vapor feedback. Should have 
+        perturbation at the TOA from the water vapor feedback. Should have
         coords of lat, lon, and time.
 
     q_lwcs : xarray DataArray
         DataArray containing the vertically integrated LW clear-sky radiative
-        perturbation at the TOA from the water vapor feedback. Should have 
+        perturbation at the TOA from the water vapor feedback. Should have
         coords of lat, lon, and time.
 
     dCRE_lw : xarray DataArray
-        DataArray containing the change in LW cloud radiative effect at the 
-        TOA with coords of time, lat, and lon and units of Wm^-2. positive 
+        DataArray containing the change in LW cloud radiative effect at the
+        TOA with coords of time, lat, and lon and units of Wm^-2. positive
         = downwards.
 
     IRF_lwas : xarray DataArray
-        DataArray containing the LW all-sky instantaneous radiative forcing 
+        DataArray containing the LW all-sky instantaneous radiative forcing
         in units of Wm^-2 with coords of lat, lon, and time.
 
     IRF_lwcs : xarray DataArray
         DataArray containing the LW clear-sky instantaneous radiative forcing
         in units of Wm^-2 with coords of lat, lon, and time.
 
     Returns
@@ -547,54 +602,55 @@
     # first double check that the LW IRF is positive
     irf_coeff = -1 if IRF_lwcs.mean() < 0 else 1
     dIRF_lw = irf_coeff * (IRF_lwcs - IRF_lwas)
 
     # calculate longwave cloud feedback
     lw_cld_feedback = dCRE_lw + dt + dq_lw + dIRF_lw
 
-    return(lw_cld_feedback)
+    return lw_cld_feedback
 
-def calc_cloud_SW(alb_as,alb_cs,q_swas,q_swcs,dCRE_sw,IRF_swas,IRF_swcs):
+
+def calc_cloud_SW(alb_as, alb_cs, q_swas, q_swcs, dCRE_sw, IRF_swas, IRF_swcs):
     """
     Calculate the radiative perturbation from the shortwave cloud feedback
     using the adjustment method outlined in Soden et al. (2008).
 
     Parameters
     ----------
     alb_as : xarray DataArray
         DataArray containing the all-sky radiative perturbation at the TOA
-        from the surface albedo feedback. Should have coords of lat, lon, and 
+        from the surface albedo feedback. Should have coords of lat, lon, and
         time.
 
     alb_cs : xarray DataArray
         DataArray containing the clear-sky radiative perturbation at the TOA
-        from the surface albedo feedback. Should have coords of lat, lon, and 
+        from the surface albedo feedback. Should have coords of lat, lon, and
         time.
 
     q_swas : xarray DataArray
-        DataArray containing the vertically integrated all-sky LW radiative 
-        perturbation at the TOA from the shortwave water vapor feedback. 
+        DataArray containing the vertically integrated all-sky LW radiative
+        perturbation at the TOA from the shortwave water vapor feedback.
         Should have coords of lat, lon, and time.
 
     q_swcs : xarray DataArray
-        DataArray containing the vertically integrated clear-sky LW radiative 
-        perturbation at the TOA from the shortwave water vapor feedback. 
+        DataArray containing the vertically integrated clear-sky LW radiative
+        perturbation at the TOA from the shortwave water vapor feedback.
         Should have coords of lat, lon, and time.
 
     dCRE_sw : xarray DataArray
         Three-dimensional DataArray containing the change in shortwave cloud
-        radiative effect at the top-of-atmosphere with coords of time, lat, 
+        radiative effect at the top-of-atmosphere with coords of time, lat,
         and lon and units of Wm^-2. positive = downwards.
 
     IRF_swas : xarray DataArray
-        The shortwave all-sky instantaneous radiative forcing in units of 
+        The shortwave all-sky instantaneous radiative forcing in units of
         Wm^-2 with coords of lat, lon, and time.
 
     IRF_swcs : xarray DataArray
-        The shortwave clear-sky instantaneous radiative forcing in units of 
+        The shortwave clear-sky instantaneous radiative forcing in units of
         Wm^-2 with coords of lat, lon, and time.
 
     Returns
     -------
     sw_cld_feedback : xarray DataArray
         Three-dimensional DataArray containing the TOA radiative perturbation
         from the shortwave cloud feedback.
@@ -603,22 +659,23 @@
     # water vapor cloud masking term
     dq_sw = q_swcs - q_swas
 
     # surface albedo cloud masking term
     dalb = alb_cs - alb_as
 
     # IRF cloud masking term
-    dIRF_sw = (IRF_swcs - IRF_swas)
+    dIRF_sw = IRF_swcs - IRF_swas
 
     # calculate longwave cloud feedback
     sw_cld_feedback = dCRE_sw + dalb + dq_sw + dIRF_sw
 
-    return(sw_cld_feedback)
+    return sw_cld_feedback
+
 
-def calc_cloud_LW_res(ctrl_FLNT,pert_FLNT,RF_lw,t_lw,q_lw):
+def calc_cloud_LW_res(ctrl_FLNT, pert_FLNT, RF_lw, t_lw, q_lw):
     """
     Calculate the radiative perturbation from the shortwave cloud feedback
     using the residual method outlined in Soden & Held (2006).
 
     Parameters
     ----------
     ctrl_FLNT : xarray DataArray
@@ -628,47 +685,48 @@
         oriented such that positive = downwards.
 
     pert_FLNT : xarray DataArray
         Three-dimensional DataArray containing the all-sky net longwave flux
         at the top-of-atmosphere in the perturbed simulation
         with coords of time, lat, and lon and units of Wm^-2. It should be
         oriented such that positive = downwards.
-        
+
     RF_lw : xarray DataArray
         The longwave all-sky radiative forcing in units of Wm^-2
         with coords of lat, lon, and time. This is usually the stratosphere-
         adjusted RF.
 
     t_lw : xarray DataArray
-        DataArray containing the vertically integrated all-sky radiative 
-        perturbation at the TOA from the total temperature feedback. The 
+        DataArray containing the vertically integrated all-sky radiative
+        perturbation at the TOA from the total temperature feedback. The
         total temperature feedback is the sum of the Planck and lapse rate
         feedbacks. Should have dims of lat, lon, and time.
 
     q_lw : xarray DataArray
         DataArray containing the vertically integrated LW all-sky radiative
-        perturbation at the TOA from the water vapor feedback. Should have 
+        perturbation at the TOA from the water vapor feedback. Should have
         coords of lat, lon, and time.
-        
+
     Returns
     -------
     lw_cld_feedback : xarray DataArray
         Three-dimensional DataArray containing the TOA radiative perturbation
         from the longwave cloud feedback.
     """
     # Calculate ΔR as the difference in net longwave flux
     # double check that sign is correct first, though
     lw_coeff = 1 if ctrl_FLNT.mean() < 0 else -1
     dR_lw = lw_coeff * (pert_FLNT - ctrl_FLNT)
 
     irf_coeff = -1 if RF_lw.mean() < 0 else 1
     lw_cld_feedback = dR_lw - (irf_coeff * RF_lw) - t_lw - q_lw
-    return(lw_cld_feedback)
+    return lw_cld_feedback
+
 
-def calc_cloud_SW_res(ctrl_FSNT,pert_FSNT,RF_sw,q_sw,alb_sw):
+def calc_cloud_SW_res(ctrl_FSNT, pert_FSNT, RF_sw, q_sw, alb_sw):
     """
     Calculate the radiative perturbation from the shortwave cloud feedback
     using the residual method outlined in Soden & Held (2006).
 
     Parameters
     ----------
     ctrl_FSNT : xarray DataArray
@@ -685,155 +743,171 @@
 
     RF_sw : xarray DataArray
         The shortwave all-sky radiative forcing in units of Wm^-2
         with coords of lat, lon, and time. This is usually the stratosphere-
         adjusted RF.
 
     q_sw : xarray DataArray
-        DataArray containing the vertically integrated all-sky LW radiative 
-        perturbation at the TOA from the shortwave water vapor feedback. 
+        DataArray containing the vertically integrated all-sky LW radiative
+        perturbation at the TOA from the shortwave water vapor feedback.
         Should have coords of lat, lon, and time.
 
     alb_sw : xarray DataArray
         DataArray containing the all-sky radiative perturbation at the TOA
-        from the surface albedo feedback. Should have coords of lat, lon, and 
+        from the surface albedo feedback. Should have coords of lat, lon, and
         time.
-        
+
     Returns
     -------
     sw_cld_feedback : xarray DataArray
         Three-dimensional DataArray containing the TOA radiative perturbation
         from the shortwave cloud feedback.
     """
     # Calculate ΔR as the difference in net shortwave flux
     dR_sw = pert_FSNT - ctrl_FSNT
 
     sw_cld_feedback = dR_sw - RF_sw - q_sw - alb_sw
-    return(sw_cld_feedback)
+    return sw_cld_feedback
 
-def calc_strato_T(ctrl_ta,pert_ta,pert_ps,pert_trop=None,kern='GFDL',
-                  sky='all-sky'):
+
+def calc_strato_T(
+    ctrl_ta, pert_ta, pert_ps, pert_trop=None, kern="GFDL", sky="all-sky"
+):
     """
     Calculate the raditive pertubations (W/m^2) at the TOA from changes in
     statosphere air temperature using user-specified kernel. Horizontal
     resolution is kept at input data's resolution.
-    
+
     Parameters
     ----------
     ctrl_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the
         control simulation. 4D with coordinates of time, latitude, longitude,
         and pressure level and units of K.
-        
+
     pert_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the
-        perturbed simulation. 4D with coordinates of time, latitude, 
+        perturbed simulation. 4D with coordinates of time, latitude,
         longitude, and pressure level and units of K.
-        
+
     pert_ps : xarray DataArray
         DataArray containing surface pressure in the perturbed simulation. 3D
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_trop : xarray DataArray, optional
         DataArray containing tropopause pressure in the perturbed simulation.
         3D with coordinates of time, latitude, and longitude and units of Pa
         or hPa. If not provided, ClimKern will assume a tropopause height of
         300 hPa at the equator, linearly decreasing with the cosine of
         latitude to 100 hPa at the poles.
 
     kern : string, optional
         String specifying the name of the desired kernel. Defaults to "GFDL".
-        
+
     sky : string, optional
         String, either "all-sky" or "clear-sky", specifying whether to
         calculate the all-sky or clear-sky feedbacks. Defaults to "all-sky".
 
     Returns
     -------
     T_feedback : xarray DataArray
-        3D DataArray containing the vertically integrated radiative 
-        perturbations caused by changes in stratospheric temperature. 
+        3D DataArray containing the vertically integrated radiative
+        perturbations caused by changes in stratospheric temperature.
         Has coordinates of time, lat, and lon.
     """
     # get correct keys for all-sky or clear-sky
-    t_key = 'lw_t' if check_sky(sky)=='all-sky' else 'lwclr_t'
+    t_key = "lw_t" if check_sky(sky) == "all-sky" else "lwclr_t"
 
     # check input coordinates
-    for d in [ctrl_ta,pert_ta]:
-        d = check_coords(d,ndim=4)
-    pert_ps = check_coords(pert_ps,ndim=3)
+    for d in [ctrl_ta, pert_ta]:
+        d = check_coords(d, ndim=4)
+    pert_ps = check_coords(pert_ps, ndim=3)
 
     # check input units
-    ctrl_ta = check_var_units(check_plev_units(ctrl_ta),'T')
-    pert_ta = check_var_units(check_plev_units(pert_ta),'T')
-    pert_ps = check_pres_units(pert_ps,"pert PS")
+    ctrl_ta = check_var_units(check_plev_units(ctrl_ta), "T")
+    pert_ta = check_var_units(check_plev_units(pert_ta), "T")
+    pert_ps = check_pres_units(pert_ps, "pert PS")
 
     # check tropopause units if provided by user, else create dummy tropopause
-    if(type(pert_trop) == type(None)):
+    if type(pert_trop) == type(None):
         pert_trop = make_tropo(pert_ps)
     else:
         pert_trop = check_coords(pert_trop)
-        pert_trop = check_pres_units(pert_trop,"pert tropopause")
+        pert_trop = check_pres_units(pert_trop, "pert tropopause")
 
     # make climatology
     ctrl_ta_clim = make_clim(ctrl_ta)
-    
+
     # calculate change in air temperature
-    diff_ta = (pert_ta - tile_data(ctrl_ta_clim,pert_ta))
-    
+    diff_ta = pert_ta - tile_data(ctrl_ta_clim, pert_ta)
+
     # read in and regrid temperature kernel
     kernel = check_plev(get_kern(kern))
-    regridder = xe.Regridder(kernel[t_key],diff_ta,method='bilinear',
-                             reuse_weights=False,periodic=True,
-                            extrap_method='nearest_s2d')
-    ta_kernel = tile_data(regridder(kernel[t_key]),diff_ta)
+    regridder = xe.Regridder(
+        kernel[t_key],
+        diff_ta,
+        method="bilinear",
+        reuse_weights=False,
+        periodic=True,
+        extrap_method="nearest_s2d",
+    )
+    ta_kernel = tile_data(regridder(kernel[t_key]), diff_ta)
 
     # regrid diff_ta to kernel pressure levels
-    diff_ta = diff_ta.interp_like(ta_kernel,kwargs={
-        "fill_value": "extrapolate"})
-    
+    diff_ta = diff_ta.interp_like(ta_kernel, kwargs={"fill_value": "extrapolate"})
+
     # use get_function in climkern.util to calculate layer thickness
-    dp = get_dp(diff_ta,pert_ps,pert_trop,layer='stratosphere')
+    dp = get_dp(diff_ta, pert_ps, pert_trop, layer="stratosphere")
 
     # calculate total temperature feedback
-    T_feedback = ((ta_kernel * diff_ta.fillna(0)) * dp/10000
-                  ).sum(dim='plev',min_count=1)
-       
-    return(T_feedback)
-
-def calc_strato_q(ctrl_q,ctrl_ta,pert_q,pert_ps,pert_trop=None,
-                     kern='GFDL',sky='all-sky',method='pendergrass'):
+    T_feedback = ((ta_kernel * diff_ta.fillna(0)) * dp / 10000).sum(
+        dim="plev", min_count=1
+    )
+
+    return T_feedback
+
+
+def calc_strato_q(
+    ctrl_q,
+    ctrl_ta,
+    pert_q,
+    pert_ps,
+    pert_trop=None,
+    kern="GFDL",
+    sky="all-sky",
+    method="pendergrass",
+):
     """
-    Calculate the raditive pertubations (W/m^2), LW & SW, at the TOA from 
+    Calculate the raditive pertubations (W/m^2), LW & SW, at the TOA from
     changes in stratospheric specific humidity using user-specified kernel.
     Horizontal resolution is kept at input data's resolution.
 
     Parameters
     ----------
     ctrl_q : xarray DataArray
         DataArray containing specific humidity on pressure levels in the
         control simulation. 4D with coordinates of time, latitude, longitude,
         and pressure level and units of "1", "kg/kg", or "g/kg".
 
     ctrl_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the
         control simulation. 4D with coordinates of time, latitude, longitude,
         and pressure level and units of K.
-        
+
     pert_q : xarray DataArray
         DataArray containing specific humidity on pressure levels in the
-        perturbed simulation. 4D with coordinates of time, latitude, 
+        perturbed simulation. 4D with coordinates of time, latitude,
         longitude, and pressure level and units of "1", "kg/kg", or "g/kg".
-        
+
     pert_ps : xarray DataArray
         DataArray containing surface pressure in the perturbed simulation. 3D
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_trop : xarray DataArray, optional
         DataArray containing tropopause pressure in the perturbed simulation.
         3D with coordinates of time, latitude, and longitude and units of Pa
         or hPa. If not provided, ClimKern will assume a tropopause height of
         300 hPa at the equator, linearly decreasing with the cosine of
         latitude to 100 hPa at the poles.
 
@@ -843,152 +917,170 @@
     sky : string, optional
         String, either "all-sky" or "clear-sky", specifying whether to
         calculate the all-sky or clear-sky feedbacks. Defaults to "all-sky".
 
     method : string, optional
         Specifies the method to use to calculate the specific humidity
         feedback. Options are "pendergrass" (default), "kramer", "zelinka",
-        and "linear". 
+        and "linear".
 
     Returns
     -------
     lw_q_feedback : xarray DataArray
         3D DataArray containing the vertically integrated radiative
         perturbations from changes in specific humidity in the stratosphere
         (longwave). Has coordinates of time, lat, and lon.
-        
+
     sw_q_feedback : xarray DataArray
-        3D DataArray containing the vertically integrated radiative 
+        3D DataArray containing the vertically integrated radiative
         perturbations from changes in specific humidity in the stratosphere
         (shortwave). Has coordinates of time, lat, and lon.
     """
     # get correct keys for all-sky or clear-sky
-    qlw_key = 'lw_q' if check_sky(sky)=='all-sky' else 'lwclr_q'
-    qsw_key = 'sw_q' if sky=='all-sky' else 'swclr_q'
+    qlw_key = "lw_q" if check_sky(sky) == "all-sky" else "lwclr_q"
+    qsw_key = "sw_q" if sky == "all-sky" else "swclr_q"
 
     # check input coordinates
-    for d in [ctrl_q,ctrl_ta,pert_q]:
-        d = check_coords(d,ndim=4)
+    for d in [ctrl_q, ctrl_ta, pert_q]:
+        d = check_coords(d, ndim=4)
     for d in [pert_ps]:
         d = check_coords(d)
 
     # check input units
-    ctrl_ta = check_var_units(check_plev_units(ctrl_ta),'T')
-    ctrl_q = check_var_units(check_plev_units(ctrl_q),'q')
-    pert_q = check_var_units(check_plev_units(pert_q),'q')
-    pert_ps = check_pres_units(pert_ps,"pert PS")
+    ctrl_ta = check_var_units(check_plev_units(ctrl_ta), "T")
+    ctrl_q = check_var_units(check_plev_units(ctrl_q), "q")
+    pert_q = check_var_units(check_plev_units(pert_q), "q")
+    pert_ps = check_pres_units(pert_ps, "pert PS")
 
     # check tropopause units if provided by user, else create dummy tropopause
-    if(type(pert_trop) == type(None)):
-        pert_trop = make_tropo(ctrl_ps)
+    if type(pert_trop) == type(None):
+        pert_trop = make_tropo(pert_ps)
     else:
         pert_trop = check_coords(pert_trop)
-        pert_trop = check_pres_units(pert_trop,"pert tropopause")
-    
+        pert_trop = check_pres_units(pert_trop, "pert tropopause")
+
     # make climatology
     ctrl_q_clim = make_clim(ctrl_q)
     ctrl_ta_clim = make_clim(ctrl_ta)
 
-    # if q has units of unity or kg/kg, we will have to 
+    # if q has units of unity or kg/kg, we will have to
     # multiply by 1000 later on to make it g/kg
-    if(ctrl_q.units in ['1','kg/kg']):
+    if ctrl_q.units in ["1", "kg/kg"]:
         conv_factor = 1000
-    elif(ctrl_q.units in ['g/kg']):
+    elif ctrl_q.units in ["g/kg"]:
         conv_factor = 1
     else:
         warnings.warn("Cannot determine units of q. Assuming kg/kg.")
         conv_factor = 1000
 
     # tile control climatology to match length of pert simulation time dim
-    ctrl_q_clim_tiled = tile_data(ctrl_q_clim,pert_q)
-    
-    if(method=='pendergrass'):
-        diff_q = (pert_q - ctrl_q_clim_tiled)/ctrl_q_clim_tiled
-    elif(method=='linear'):
+    ctrl_q_clim_tiled = tile_data(ctrl_q_clim, pert_q)
+
+    if method == "pendergrass":
+        diff_q = (pert_q - ctrl_q_clim_tiled) / ctrl_q_clim_tiled
+    elif method == "linear":
         diff_q = pert_q - ctrl_q_clim_tiled
-    elif(method in ['kramer','zelinka']):
+    elif method in ["kramer", "zelinka"]:
         diff_q = np.log(pert_q) - np.log(ctrl_q_clim_tiled)
     else:
-        raise ValueError(
-            "Please select a valid choice for the method argument.")
-    
+        raise ValueError("Please select a valid choice for the method argument.")
+
     # read in and regrid water vapor kernel
     kernel = check_plev(get_kern(kern))
-    regridder = xe.Regridder(kernel[qlw_key],diff_q,method='bilinear',
-                             extrap_method="nearest_s2d",
-                             reuse_weights=False,periodic=True)
+    regridder = xe.Regridder(
+        kernel[qlw_key],
+        diff_q,
+        method="bilinear",
+        extrap_method="nearest_s2d",
+        reuse_weights=False,
+        periodic=True,
+    )
 
-    qlw_kernel = tile_data(regridder(kernel[qlw_key],skipna=True),diff_q)
-    qsw_kernel = tile_data(regridder(kernel[qsw_key],skipna=True),diff_q)  
+    qlw_kernel = tile_data(regridder(kernel[qlw_key], skipna=True), diff_q)
+    qsw_kernel = tile_data(regridder(kernel[qsw_key], skipna=True), diff_q)
 
     # regrid diff_q, ctrl_q_clim, and ctrl_ta_clim to kernel pressure levels
-    kwargs = {'fill_value':'extrapolate'}
-    diff_q = diff_q.interp_like(qlw_kernel,kwargs=kwargs)
-    ctrl_q_clim = ctrl_q_clim.interp(plev=qlw_kernel.plev,kwargs=kwargs)
-    ctrl_q_clim.plev.attrs['units'] = ctrl_q.plev.units
-    ctrl_ta_clim = ctrl_ta_clim.interp(plev=qlw_kernel.plev,kwargs=kwargs)
-    ctrl_ta_clim.plev.attrs['units'] = ctrl_ta.plev.units
+    kwargs = {"fill_value": "extrapolate"}
+    diff_q = diff_q.interp_like(qlw_kernel, kwargs=kwargs)
+    ctrl_q_clim = ctrl_q_clim.interp(plev=qlw_kernel.plev, kwargs=kwargs)
+    ctrl_q_clim.plev.attrs["units"] = ctrl_q.plev.units
+    ctrl_ta_clim = ctrl_ta_clim.interp(plev=qlw_kernel.plev, kwargs=kwargs)
+    ctrl_ta_clim.plev.attrs["units"] = ctrl_ta.plev.units
 
     # create the normalization factor, which corresponds to the increase
     # in specific humidity for a 1K increate in temperature
-    norm = tile_data(calc_q_norm(ctrl_ta_clim,ctrl_q_clim,method=method),
-                     diff_q)
-    
+    norm = tile_data(calc_q_norm(ctrl_ta_clim, ctrl_q_clim, method=method), diff_q)
+
     # use get_function in climkern.util to calculate layer thickness
-    dp = get_dp(diff_q,pert_ps,pert_trop,layer='stratosphere')
-                    
+    dp = get_dp(diff_q, pert_ps, pert_trop, layer="stratosphere")
+
     # calculate feedbacks
-    qlw_feedback = (qlw_kernel/norm * diff_q * conv_factor * dp/10000).sum(
-        dim='plev',min_count=1)
-    qsw_feedback = (qsw_kernel/norm * diff_q * conv_factor * dp/10000).sum(
-        dim='plev',min_count=1).fillna(0)
+    qlw_feedback = (qlw_kernel / norm * diff_q * conv_factor * dp / 10000).sum(
+        dim="plev", min_count=1
+    )
+    qsw_feedback = (
+        (qsw_kernel / norm * diff_q * conv_factor * dp / 10000)
+        .sum(dim="plev", min_count=1)
+        .fillna(0)
+    )
 
     # one complication: CloudSat needs to be masked so we don't fill the NaNs
     # with zeros
-    if(kern=='CloudSat'):
-        qsw_feedback = qsw_feedback.where(qsw_kernel.sum(
-            dim='plev',min_count=1).notnull())
-    
-    return(qlw_feedback,qsw_feedback)
-
-def calc_RH_feedback(ctrl_q,ctrl_ta,ctrl_ps,pert_q,pert_ta,pert_ps,
-                     pert_trop=None,kern='GFDL',sky='all-sky',
-                     method='pendergrass'):
+    if kern == "CloudSat":
+        qsw_feedback = qsw_feedback.where(
+            qsw_kernel.sum(dim="plev", min_count=1).notnull()
+        )
+
+    return (qlw_feedback, qsw_feedback)
+
+
+def calc_RH_feedback(
+    ctrl_q,
+    ctrl_ta,
+    ctrl_ps,
+    pert_q,
+    pert_ta,
+    pert_ps,
+    pert_trop=None,
+    kern="GFDL",
+    sky="all-sky",
+    method="pendergrass",
+):
     """
     Calculate the TOA radiative perturbations from changes in relative
-    humidity following Held & Shell (2012). Horizontal resolution is 
+    humidity following Held & Shell (2012). Horizontal resolution is
     kept at input data's resolution.
-    
+
     Parameters
     ----------
     ctrl_q : xarray DataArray
-        DataArray containing specific humidity on pressure levels in the 
+        DataArray containing specific humidity on pressure levels in the
         control simulation. Must be 4D with coords of time, lat, lon, and plev
         with units of either "1", "kg/kg", or "g/kg".
 
     ctrl_ta : xarray DataArray
         DataArray containing air temperature on pressure levels in the control
-        simulation. Must be 4D with coords of time, lat, lon, and plev with 
+        simulation. Must be 4D with coords of time, lat, lon, and plev with
         units "K".
-        
+
     ctrl_ps : xarray DataArray
-        DataArray containing surface pressure in the control simulation. 3D 
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        DataArray containing surface pressure in the control simulation. 3D
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_q : xarray DataArray
         DataArray containing specific humidity on pressure levels in the
-        perturbed simulation. 4D with coordinates of time, latitude, 
+        perturbed simulation. 4D with coordinates of time, latitude,
         longitude, and pressure level and units of "1", "kg/kg", or "g/kg".
-        
+
     pert_ps : xarray DataArray
         DataArray containing surface pressure in the perturbed simulation. 3D
-        with coordinates of time, latitude, and longitude and units of Pa or 
+        with coordinates of time, latitude, and longitude and units of Pa or
         hPa.
-        
+
     pert_trop : xarray DataArray, optional
         DataArray containing tropopause pressure in the perturbed simulation.
         3D with coordinates of time, latitude, and longitude and units of Pa
         or hPa. If not provided, ClimKern will assume a tropopause height of
         300 hPa at the equator, linearly decreasing with the cosine of
         latitude to 100 hPa at the poles.
 
@@ -998,170 +1090,178 @@
     sky : string, optional
         String, either "all-sky" or "clear-sky", specifying whether to
         calculate the all-sky or clear-sky feedbacks. Defaults to "all-sky".
 
     method : string, optional
         Specifies the method to use to calculate the specific humidity
         feedback. Options are "pendergrass" (default), "kramer", "zelinka",
-        and "linear". 
+        and "linear".
 
     Returns
     -------
     RH_feedback : xarray DataArray
-        3D DataArray containing the vertically integrated radiative 
+        3D DataArray containing the vertically integrated radiative
         perturbations from changes in relative humidity (LW+SW).
         Has coordinates of time, lat, and lon.
     """
     # get correct keys for all-sky or clear-sky
-    qlw_key = 'lw_q' if check_sky(sky)=='all-sky' else 'lwclr_q'
-    qsw_key = 'sw_q' if sky=='all-sky' else 'swclr_q'
+    qlw_key = "lw_q" if check_sky(sky) == "all-sky" else "lwclr_q"
+    qsw_key = "sw_q" if sky == "all-sky" else "swclr_q"
 
     # check input coordinates
-    for d in [ctrl_q,ctrl_ta,pert_q,pert_ta]:
-        d = check_coords(d,ndim=4)
-    for d in [ctrl_ps,pert_ps]:
+    for d in [ctrl_q, ctrl_ta, pert_q, pert_ta]:
+        d = check_coords(d, ndim=4)
+    for d in [ctrl_ps, pert_ps]:
         d = check_coords(d)
 
     # check input units
-    ctrl_ta = check_var_units(check_plev_units(ctrl_ta),'T')
-    pert_ta = check_var_units(check_plev_units(pert_ta),'T')
-    ctrl_q = check_var_units(check_plev_units(ctrl_q),'q')
-    pert_q = check_var_units(check_plev_units(pert_q),'q')
-    ctrl_ps = check_pres_units(ctrl_ps,"ctrl PS")
-    pert_ps = check_pres_units(pert_ps,"pert PS")
+    ctrl_ta = check_var_units(check_plev_units(ctrl_ta), "T")
+    pert_ta = check_var_units(check_plev_units(pert_ta), "T")
+    ctrl_q = check_var_units(check_plev_units(ctrl_q), "q")
+    pert_q = check_var_units(check_plev_units(pert_q), "q")
+    ctrl_ps = check_pres_units(ctrl_ps, "ctrl PS")
+    pert_ps = check_pres_units(pert_ps, "pert PS")
 
     # check tropopause units if provided by user, else create dummy tropopause
-    if(type(pert_trop) == type(None)):
+    if type(pert_trop) == type(None):
         pert_trop = make_tropo(ctrl_ps)
     else:
         pert_trop = check_coords(pert_trop)
-        pert_trop = check_pres_units(pert_trop,"pert tropopause")
-    
+        pert_trop = check_pres_units(pert_trop, "pert tropopause")
+
     # make climatology
     ctrl_ps_clim = make_clim(ctrl_ps)
     ctrl_q_clim = make_clim(ctrl_q)
-    ctrl_q_clim = ctrl_q_clim.where(ctrl_q_clim.plev<ctrl_ps_clim)
+    ctrl_q_clim = ctrl_q_clim.where(ctrl_q_clim.plev < ctrl_ps_clim)
     ctrl_ta_clim = make_clim(ctrl_ta)
-    ctrl_ta_clim = ctrl_ta_clim.where(ctrl_ta_clim.plev<ctrl_ps_clim)
+    ctrl_ta_clim = ctrl_ta_clim.where(ctrl_ta_clim.plev < ctrl_ps_clim)
 
-    # if q has units of unity or kg/kg, we will have to 
+    # if q has units of unity or kg/kg, we will have to
     # multiply by 1000 later on to make it g/kg
-    if(ctrl_q.units in ['1','kg/kg']):
+    if ctrl_q.units in ["1", "kg/kg"]:
         conv_factor = 1000
-    elif(ctrl_q.units in ['g/kg']):
+    elif ctrl_q.units in ["g/kg"]:
         conv_factor = 1
     else:
         warnings.warn("Cannot determine units of q. Assuming kg/kg.")
         conv_factor = 1000
 
     # tile control climatology to match length of pert simulation time dim
-    ctrl_q_clim_tiled = tile_data(ctrl_q_clim,pert_q)
-    
-    if(method=='pendergrass'):
-        diff_q = (pert_q - ctrl_q_clim_tiled)/ctrl_q_clim_tiled
-    elif(method=='linear'):
+    ctrl_q_clim_tiled = tile_data(ctrl_q_clim, pert_q)
+
+    if method == "pendergrass":
+        diff_q = (pert_q - ctrl_q_clim_tiled) / ctrl_q_clim_tiled
+    elif method == "linear":
         diff_q = pert_q - ctrl_q_clim_tiled
-    elif(method in ['kramer','zelinka']):
+    elif method in ["kramer", "zelinka"]:
         diff_q = np.log(pert_q) - np.log(ctrl_q_clim_tiled)
     else:
-        raise ValueError(
-            "Please select a valid choice for the method argument.")
+        raise ValueError("Please select a valid choice for the method argument.")
 
     # for the RH feedback, we also need the T response
-    diff_ta = pert_ta - tile_data(ctrl_ta_clim,pert_ta)
-    
+    diff_ta = pert_ta - tile_data(ctrl_ta_clim, pert_ta)
+
     # read in and regrid water vapor kernel
     kernel = check_plev(get_kern(kern))
-    regridder = xe.Regridder(kernel[qlw_key],diff_q,method='bilinear',
-                             extrap_method="nearest_s2d",
-                             reuse_weights=False,periodic=True)
+    regridder = xe.Regridder(
+        kernel[qlw_key],
+        diff_q,
+        method="bilinear",
+        extrap_method="nearest_s2d",
+        reuse_weights=False,
+        periodic=True,
+    )
     q_kernel = kernel[qlw_key] + kernel[qsw_key]
-    q_kernel = tile_data(regridder(q_kernel,skipna=True),diff_q)
+    q_kernel = tile_data(regridder(q_kernel, skipna=True), diff_q)
 
     # regrid diff_q, ctrl_q_clim, and ctrl_ta_clim to kernel pressure levels
-    kwargs = {'fill_value':'extrapolate'}
-    diff_q = diff_q.interp_like(q_kernel,kwargs=kwargs)
-    diff_ta = diff_ta.interp_like(q_kernel,kwargs=kwargs)
-    ctrl_q_clim = ctrl_q_clim.interp(plev=q_kernel.plev,kwargs=kwargs)
-    ctrl_q_clim.plev.attrs['units'] = ctrl_q.plev.units
-    ctrl_ta_clim = ctrl_ta_clim.interp(plev=q_kernel.plev,kwargs=kwargs)
-    ctrl_ta_clim.plev.attrs['units'] = ctrl_ta.plev.units
+    kwargs = {"fill_value": "extrapolate"}
+    diff_q = diff_q.interp_like(q_kernel, kwargs=kwargs)
+    diff_ta = diff_ta.interp_like(q_kernel, kwargs=kwargs)
+    ctrl_q_clim = ctrl_q_clim.interp(plev=q_kernel.plev, kwargs=kwargs)
+    ctrl_q_clim.plev.attrs["units"] = ctrl_q.plev.units
+    ctrl_ta_clim = ctrl_ta_clim.interp(plev=q_kernel.plev, kwargs=kwargs)
+    ctrl_ta_clim.plev.attrs["units"] = ctrl_ta.plev.units
 
     # create the normalization factor, which corresponds to the increase
     # in specific humidity for a 1K increate in temperature
-    norm = tile_data(calc_q_norm(ctrl_ta_clim,ctrl_q_clim,method=method),
-                     diff_q)
-    
+    norm = tile_data(calc_q_norm(ctrl_ta_clim, ctrl_q_clim, method=method), diff_q)
+
     # use get_dp in climkern.util to calculate layer thickness
-    dp = get_dp(diff_q,pert_ps,pert_trop,layer='troposphere')
+    dp = get_dp(diff_q, pert_ps, pert_trop, layer="troposphere")
 
     # calculate RH_feedback
-    RH_feedback = ((q_kernel/norm * diff_q * conv_factor * dp/10000)
-                   - (q_kernel * diff_ta * dp/10000)).sum(
-        dim='plev',min_count=1).fillna(0)
+    RH_feedback = (
+        (
+            (q_kernel / norm * diff_q * conv_factor * dp / 10000)
+            - (q_kernel * diff_ta * dp / 10000)
+        )
+        .sum(dim="plev", min_count=1)
+        .fillna(0)
+    )
 
     # one complication: CloudSat needs to be masked so we don't fill the NaNs
     # with zeros
-    if(kern=='CloudSat'):
-        RH_feedback = RH_feedback.where(q_kernel.sum(
-            dim='plev',min_count=1).notnull())
-    
-    return(RH_feedback)
+    if kern == "CloudSat":
+        RH_feedback = RH_feedback.where(q_kernel.sum(dim="plev", min_count=1).notnull())
+
+    return RH_feedback
+
 
 def tutorial_data(label):
     """
     Retrieve tutorial data which should be located in the package's
     "data" folder.
 
     Parameters
     ----------
     name : string
-        Specifies which data to access. Choices are "ctrl", "pert", "IRF", or 
+        Specifies which data to access. Choices are "ctrl", "pert", "IRF", or
         "adjRF" for the 1xCO2, 2xCO2, instantaneous radiative forcing, and
         stratosphere-adjusted radiative forcing, respectively.
 
     Returns
     -------
     data : xarray Dataset
         Requested tutorial dataset.
     """
-    if label not in ['ctrl','pert','IRF','adjRF']:
-        raise ValueError('Invalid data name. See docstring for options.')
-    path = 'data/tutorial_data/'+ label + ".nc"
-    data = xr.open_dataset(files('climkern').joinpath(path))
+    if label not in ["ctrl", "pert", "IRF", "adjRF"]:
+        raise ValueError("Invalid data name. See docstring for options.")
+    path = "data/tutorial_data/" + label + ".nc"
+    data = xr.open_dataset(files("climkern").joinpath(path))
     return data
 
-def spat_avg(data,lat_bound_s=-90,lat_bound_n=90):
+
+def spat_avg(data, lat_bound_s=-90, lat_bound_n=90):
     """
     Compute the spatial average while weighting for cos(latitude), optionally
     specifying latitudinal boundaries.
 
     Parameters
     ----------
     data : Xarray DataArray
         3D input data over which to compute the spatial average.
 
     lat_bound_s : float, optional
-        Latitude of the southern boundary of the area over which to average. 
+        Latitude of the southern boundary of the area over which to average.
         Defaults to -90 to compute a global average.
 
     lat_bound_n : float, optional
-        Latitude of the northern boundary of the area over which to average. 
-        Defaults to 90 to compute a global average.   
+        Latitude of the northern boundary of the area over which to average.
+        Defaults to 90 to compute a global average.
 
     Returns
     -------
     avg : Xarray DataArray
         New spatially averaged DataArray with latitude and longitude
         coordinates now removed.
     """
     # check coords, constrain area of interest, and take zonal mean
-    data = check_coords(data).sel(lat=slice(lat_bound_s,lat_bound_n)).mean(
-        dim='lon')
+    data = check_coords(data).sel(lat=slice(lat_bound_s, lat_bound_n)).mean(dim="lon")
     # compute weights
-    weights = np.cos(np.deg2rad(data.lat))/np.cos(np.deg2rad(data.lat)).sum()
+    weights = np.cos(np.deg2rad(data.lat)) / np.cos(np.deg2rad(data.lat)).sum()
 
     # compute average
-    avg = (data * weights).sum(dim='lat')
+    avg = (data * weights).sum(dim="lat")
 
     # return avg
-    return(avg)
+    return avg
```

### Comparing `climkern-1.0.1/climkern/util.py` & `climkern-1.1.0/climkern/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,276 +1,309 @@
-import xarray as xr
-import cf_xarray as cfxr
-import xesmf as xe
-from importlib_resources import files
 import warnings
+
 import numpy as np
+import xarray as xr
+from importlib_resources import files
+
 
 # monkey patch Python warnings format function
-def custom_formatwarning(msg,cat,*args,**kwargs):
-    return(str(cat.__name__) + ': ' + str(msg) + '\n')
+def custom_formatwarning(msg, cat, *args, **kwargs):
+    return str(cat.__name__) + ": " + str(msg) + "\n"
+
+
 warnings.formatwarning = custom_formatwarning
 
 # filter out warnings from xarray when using the rename function
 # ideally, this can be removed in the future
-warnings.filterwarnings('ignore','.*does not create an index anymore.*')
+warnings.filterwarnings("ignore", ".*does not create an index anymore.*")
 
-def get_dp(ds_4D,ps,tropo,layer='troposphere'):
+
+def get_dp(ds_4D, ps, tropo, layer="troposphere"):
     """Calculate layer thickness using model pressure levels, surface
     pressure, and tropopause pressure. Also specify the layer as either
-    'troposphere' or 'stratosphere'."""
+    'troposphere' or 'stratosphere'.
+    """
     # construct a 4D DataArray corresponding to layer thickness
     # for vertical integration later
     # this is achieved by finding the midpoints between pressure levels
     # and bounding that array with surface pressure below
     # and TOA (p=0) above
-    aligned = xr.align(ds_4D.plev[1:],ds_4D.plev[:-1],join='override')
-    mids = xr.broadcast((aligned[0] + aligned[1])/2,ps)[0]
-    ps_expand = ps.expand_dims(dim={"plev":[ds_4D.plev[0]]},axis=1)
-    
+    aligned = xr.align(ds_4D.plev[1:], ds_4D.plev[:-1], join="override")
+    mids = xr.broadcast((aligned[0] + aligned[1]) / 2, ps)[0]
+    ps_expand = ps.expand_dims(dim={"plev": [ds_4D.plev[0]]}, axis=1)
+
     TOA = xr.zeros_like(ps_expand)
-    TOA['plev']=ps_expand.plev*0
+    TOA["plev"] = ps_expand.plev * 0
 
     # this if/else statement accounts for potentially
     # reversed pressure axis direction
-    if(ds_4D.plev[0] > ds_4D.plev[-1]):
-        ilevs = xr.concat([ps_expand,mids,TOA],dim='plev')
+    if ds_4D.plev[0] > ds_4D.plev[-1]:
+        ilevs = xr.concat([ps_expand, mids, TOA], dim="plev")
         sign_change = -1
     else:
-        ilevs = xr.concat([TOA,mids,ps_expand],dim='plev')
+        ilevs = xr.concat([TOA, mids, ps_expand], dim="plev")
         sign_change = 1
 
-    if(layer=='troposphere'):
+    if layer == "troposphere":
         # make points above tropopause equal to tropopause height
         # make points below surface pressure equal to surface pressure
-        ilevs = ilevs.where(ilevs>tropo,tropo).where(ilevs<ps,ps)
-    elif(layer=='stratosphere'):
+        ilevs = ilevs.where(ilevs > tropo, tropo).where(ilevs < ps, ps)
+    elif layer == "stratosphere":
         # make points below tropopause equal to tropopause height
-        ilevs = ilevs.where(ilevs<tropo,tropo)
+        ilevs = ilevs.where(ilevs < tropo, tropo)
 
-    # get the layer thickness by taking finite difference 
+    # get the layer thickness by taking finite difference
     # along pressure axis
-    dp = sign_change * ilevs.diff(dim='plev',label='lower')
+    dp = sign_change * ilevs.diff(dim="plev", label="lower")
 
     # override pressure axis so xarray doesn't throw a fit
-    dp['plev'] = ds_4D.plev
+    dp["plev"] = ds_4D.plev
 
     # return dp
-    return(dp)
+    return dp
 
-def check_var_units(da,var):
+
+def check_var_units(da, var):
     """Check to see if the xarray DataArray has a units attribute."""
-    if('units' not in da.attrs):
-        if(var=='q'):
-            warnings.warn('No units found for input q. Assuming kg/kg.')
-            return(da.assign_attrs({'units':'kg/kg'}))
-        elif(var=='T'):
-            warnings.warn('No units found for input T. Assuming K.')
-            return(da.assign_attrs({'units':'K'}))
+    if "units" not in da.attrs:
+        if var == "q":
+            warnings.warn("No units found for input q. Assuming kg/kg.")
+            return da.assign_attrs({"units": "kg/kg"})
+        elif var == "T":
+            warnings.warn("No units found for input T. Assuming K.")
+            return da.assign_attrs({"units": "K"})
     else:
-        return(da)
+        return da
+
+
+def make_tropo(da):
+    """Use the a DataArray containing model lat and lon to make a makeshift
+    tropopause.
+    """
+    tropo = (3e4 - 2e4 * np.cos(np.deg2rad(da.lat))).broadcast_like(da)
+    return tropo
 
-def make_tropo(PS):
-    """Use the surface pressure DataArray to make a makeshift tropopause."""
-    tropo = (3e4 - 2e4*np.cos(np.deg2rad(PS.lat))).broadcast_like(PS)
-    return(tropo)
 
 def check_plev_units(da):
-    if('units' not in da.plev.attrs):
-        warnings.warn(
-            'No units found for input vertical coordinate. Assuming Pa.')
-        plev = da.plev.assign_attrs({'units':'Pa'})
-        return(da.assign_coords({'plev':plev}))
-    elif(da.plev.units in ['hPa','mb','millibars']):
-        da['plev'] = da.plev * 100
-        da.plev.attrs['units'] = 'Pa'
-        return(da)
+    if "units" not in da.plev.attrs:
+        warnings.warn("No units found for input vertical coordinate. Assuming Pa.")
+        plev = da.plev.assign_attrs({"units": "Pa"})
+        return da.assign_coords({"plev": plev})
+    elif da.plev.units in ["hPa", "mb", "millibars"]:
+        da["plev"] = da.plev * 100
+        da.plev.attrs["units"] = "Pa"
+        return da
     else:
-        return(da)
+        return da
 
-def check_pres_units(da,var_name):
-    if('units' not in da.attrs):
-        warnings.warn("Could not determine units of " + var_name +
-                      ". Assuming Pa.")
-        da.assign_attrs({'units':'Pa'})
-    elif(da.units in ['hPa','mb','millibars']):
+
+def check_pres_units(da, var_name):
+    if "units" not in da.attrs:
+        warnings.warn("Could not determine units of " + var_name + ". Assuming Pa.")
+        da.assign_attrs({"units": "Pa"})
+    elif da.units in ["hPa", "mb", "millibars"]:
         da = da * 100
-        da.attrs['units'] = 'Pa'
-        return(da)
+        da.attrs["units"] = "Pa"
+        return da
     else:
-        return(da)
+        return da
+
 
-def tile_data(to_tile,new_shape):
-    """tile dataset along time axis to match another dataset"""
+def tile_data(to_tile, new_shape):
+    """Tile dataset along time axis to match another dataset."""
     # new_shape = _check_time(new_shape)
-    if(len(new_shape.time) % 12 != 0):
-        raise ValueError('dataset time dimension must be divisible by 12')
-    tiled = xr.concat([to_tile for i in range(
-        int(len(new_shape.time)/12))],dim='time')
-    tiled['time'] = new_shape.time
-    return(tiled)
-
-def get_kern(name,loc='TOA'):
-    """read in kernel from local directory"""
-    path = 'data/kernels/'+name + '/' +loc + '_' + str(name) + "_Kerns.nc"
+    if len(new_shape.time) % 12 != 0:
+        raise ValueError("dataset time dimension must be divisible by 12")
+    tiled = xr.concat(
+        [to_tile for i in range(int(len(new_shape.time) / 12))], dim="time"
+    )
+    tiled["time"] = new_shape.time
+    return tiled
+
+
+def get_kern(name, loc="TOA"):
+    """Read in kernel from local directory."""
+    path = "data/kernels/" + name + "/" + loc + "_" + str(name) + "_Kerns.nc"
     try:
-        data = xr.open_dataset(files('climkern').joinpath(path))
-    except(ValueError):
-        data = xr.open_dataset(files('climkern').joinpath(
-            path),decode_times=False)
+        data = xr.open_dataset(files("climkern").joinpath(path))
+    except ValueError:
+        data = xr.open_dataset(files("climkern").joinpath(path), decode_times=False)
     return check_coords(data)
 
+
 def make_clim(da):
     "Produce monthly climatology of model field."
-    # da = _check_time(da)
     try:
-        clim = da.groupby(da.time.dt.month).mean(
-            dim='time',skipna=True).rename(
-            {'month':'time'})
-    except(TypeError):
-        # TypeError if time is not datetime object
+        clim = (
+            da.groupby(da.time.dt.month)
+            .mean(dim="time", skipna=True)
+            .rename({"month": "time"})
+        )
+    except AttributeError:
+        # AttributeError if time is not datetime object
         clim = da
     return clim
 
-def get_albedo(SWup,SWdown):
+
+def get_albedo(SWup, SWdown):
     """Calculate the surface albedo as the ratio of upward to
-    downward sfc shortwave."""
+    downward sfc shortwave.
+    """
     # avoid dividing by 0 and assign 0 to those grid boxes
-    # SWup = _check_time(SWup)
-    # SWdown = _check_time(SWdown)
-    return (SWup/SWdown.where(SWdown>0)).fillna(0)
+    return (SWup / SWdown.where(SWdown > 0)).fillna(0)
+
 
 def check_plev(kern):
     """Make sure the vertical pressure units of the kernel are in Pa."""
-    if(kern.plev.units != 'Pa'):
-        kern['plev'] = kern.plev*100
-        kern.plev.attrs['units'] = 'Pa'
+    if kern.plev.units != "Pa":
+        kern["plev"] = kern.plev * 100
+        kern.plev.attrs["units"] = "Pa"
     else:
         pass
-    return(kern)
+    return kern
+
 
 def __calc_qs__(temp):
-    """Calculate either the saturated specific humidity
-    given temperature and pressure."""
-    if(temp.plev.units=='Pa'):
-        pres = temp.plev/100
-    elif(temp.plev.units in ['hPa','millibars']):
+    """Calculate the saturated specific humidity
+    given temperature and pressure.
+    """
+    if temp.plev.units == "Pa":
+        pres = temp.plev / 100
+    elif temp.plev.units in ["hPa", "millibars"]:
         pres = temp.plev
     else:
-        warnings.warn('Cannot determine units of pressure \
-        coordinate. Assuming units are Pa.')
-        pres = temp.plev/100
+        warnings.warn(
+            "Cannot determine units of pressure \
+        coordinate. Assuming units are Pa."
+        )
+        pres = temp.plev / 100
 
-    if(temp.units=='K'):
+    if temp.units == "K":
         temp_c = temp - 273.15
         temp_c.attrs = temp.attrs
-        temp_c['units'] = 'C'
-    elif(temp.units=='C'):
+        temp_c["units"] = "C"
+    elif temp.units == "C":
         temp_c = temp
     else:
-        warnings.warn('Warning: Cannot determine units of temperature. \
-        Assuming Kelvin.')
+        warnings.warn(
+            "Warning: Cannot determine units of temperature. \
+        Assuming Kelvin."
+        )
         temp_c = temp - 273.15
         temp_c.attrs = temp.attrs
-        temp_c['units'] = 'C'
+        temp_c["units"] = "C"
 
     # Buck 1981 equation for saturated vapor pressure
-    esl = (1.0007 + 3.46e-6 * pres) * 6.1121 * np.exp(
-        (17.502 * temp_c)/(240.97+temp_c))
-    esi = (1.0003 + 4.18e-6 * pres) * 6.1115 * np.exp(
-        (22.452*temp_c)/(272.55 + temp_c))
+    esl = (
+        (1.0007 + 3.46e-6 * pres)
+        * 6.1121
+        * np.exp((17.502 * temp_c) / (240.97 + temp_c))
+    )
+    esi = (
+        (1.0003 + 4.18e-6 * pres)
+        * 6.1115
+        * np.exp((22.452 * temp_c) / (272.55 + temp_c))
+    )
 
     # conversion from vapor pressure to mixing ratio
     wsl = 0.622 * esl / (pres - esl)
     wsi = 0.622 * esi / (pres - esi)
 
     # use liquid water w when temp is above freezing
-    ws = xr.where(temp_c>0,wsl,wsi)
+    ws = xr.where(temp_c > 0, wsl, wsi)
 
     # convert to specific humidity
-    qs = ws / (1+ws)
-    qs['units'] = 'kg/kg'
-    return(qs)
+    qs = ws / (1 + ws)
+    qs["units"] = "kg/kg"
+    return qs
 
-def calc_q_norm(ctrl_ta,ctrl_q,method):
+
+def calc_q_norm(ctrl_ta, ctrl_q, method):
     """Calculate the change in specific humidity for 1K warming
-    assuming fixed relative humidity."""
-    if(ctrl_q.units=='g/kg'):
-        ctrl_q = ctrl_q/1000
+    assuming fixed relative humidity.
+    """
+    if ctrl_q.units == "g/kg":
+        ctrl_q = ctrl_q / 1000
 
     # get saturated specific humidity from control air temps
     qs0 = __calc_qs__(ctrl_ta)
 
     # RH = specific humidity / sat. specific humidity
     RH = ctrl_q / qs0
 
     # make a DataArray for the temperature plus 1K
     ta1K = ctrl_ta + 1
     ta1K.attrs = ctrl_ta.attrs
     qs1K = __calc_qs__(ta1K)
 
-    if(method=='linear'):
+    if method == "linear":
         # get the new specific humidity using the same RH
         q1K = qs1K * RH
-        q1K['units'] = 'kg/kg'
-    
+        q1K["units"] = "kg/kg"
+
         # take the difference
         dq1K = 1000 * (q1K - ctrl_q)
-        return(dq1K)
-        
-    elif(method in ['pendergrass','kramer']):
+        return dq1K
+
+    elif method in ["pendergrass", "kramer"]:
         dqsdT = qs1K - qs0
         dqdT = RH * dqsdT
 
         dlogqdT = 1000 * (dqdT / ctrl_q)
-        return(dlogqdT)
-        
-    elif(method=='zelinka'):
-        dlogqdT = 1000 * (np.log(qs1K.where(qs1K>0)) - np.log(
-            qs0.where(qs0>0)))
-        return(dlogqdT)
-        
+        return dlogqdT
+
+    elif method == "zelinka":
+        dlogqdT = 1000 * (np.log(qs1K.where(qs1K > 0)) - np.log(qs0.where(qs0 > 0)))
+        return dlogqdT
+
+
 def check_sky(sky):
-    """Make sure the sky argument is either all-sky or clear-sky"""
-    if(sky not in ['all-sky','clear-sky']):
-        raise ValueError(
-            'The sky argument must either be all-sky or clear-sky.')
+    """Make sure the sky argument is either all-sky or clear-sky."""
+    if sky not in ["all-sky", "clear-sky"]:
+        raise ValueError("The sky argument must either be all-sky or clear-sky.")
     else:
-        return(sky)
+        return sky
+
 
-def check_coords(ds,ndim=3):
+def check_coords(ds, ndim=3):
     """Universal function to check that dataset coordinates are in line with
-    what the package requires."""
+    what the package requires.
+    """
     # time
-    if('time' in ds.dims):
+    if "time" in ds.dims:
         pass
-    elif('month' in ds.dims):
-        ds = ds.rename({'month':'time'})
+    elif "month" in ds.dims:
+        ds = ds.rename({"month": "time"})
     else:
         raise AttributeError(
-            'There is no \'time\' or \'month\' dimension in\
-        one of the input DataArrays. Please rename your time dimension(s).')
+            "There is no 'time' or 'month' dimension in\
+        one of the input DataArrays. Please rename your time dimension(s)."
+        )
 
     # lat and lon
-    if('lat' not in ds.dims and 'latitude' not in ds.dims):
+    if "lat" not in ds.dims and "latitude" not in ds.dims:
         raise AttributeError(
-            'There is no \'lat\' or \'latitude\' dimension in\
-        one of the input DataArrays. Please rename your lat dimension(s).')
+            "There is no 'lat' or 'latitude' dimension in\
+        one of the input DataArrays. Please rename your lat dimension(s)."
+        )
 
-    if('lon' not in ds.dims and 'longitude' not in ds.dims):
+    if "lon" not in ds.dims and "longitude" not in ds.dims:
         raise AttributeError(
-            'There is no \'lon\' or \'longitude\' dimension in\
-        one of the input DataArrays. Please rename your lat dimension(s).')
+            "There is no 'lon' or 'longitude' dimension in\
+        one of the input DataArrays. Please rename your lat dimension(s)."
+        )
 
-    if(ndim==4):
-        if('plev' in ds.dims):
+    if ndim == 4:
+        if "plev" in ds.dims:
             pass
         else:
             bool = False
-            for n in ['lev','player','level']:
-                if(n in ds.dims):
-                    ds = ds.rename({n:'plev'})
+            for n in ["lev", "player", "level"]:
+                if n in ds.dims:
+                    ds = ds.rename({n: "plev"})
                     bool = True
-            if(bool == False):
-                raise AttributeError('Cannot find the name of the pressure\
-                coordinate. Please rename it to \'plev\'.')
-    return(ds)
+            if bool is False:
+                raise AttributeError(
+                    "Cannot find the name of the pressure\
+                coordinate. Please rename it to 'plev'."
+                )
+    return ds
```

### Comparing `climkern-1.0.1/climkern.egg-info/PKG-INFO` & `climkern-1.1.0/climkern.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 Metadata-Version: 2.1
 Name: climkern
-Version: 1.0.1
-Author: Ty Janoski
-Author-email: tjanoski@ccny.cuny.edu
+Version: 1.1.0
+Author-email: Ty Janoski <tyfolino@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xarray>=0.16.2
 Requires-Dist: cf-xarray>=0.5.1
 Requires-Dist: cftime
 Requires-Dist: xesmf>=0.7.1
-Requires-Dist: esmpy
 Requires-Dist: importlib_resources
 Requires-Dist: pooch
 Requires-Dist: tqdm
 Requires-Dist: plac
 Requires-Dist: netCDF4
+Requires-Dist: esmpy
+Provides-Extra: test
+Requires-Dist: pytest<8,>=7; extra == "test"
+Provides-Extra: lint
+Requires-Dist: precommit>=2.20.0; extra == "lint"
 
 # ClimKern: a Python package for calculating radiative feedbacks
 
 [![DOI](https://zenodo.org/badge/588323813.svg)](https://zenodo.org/doi/10.5281/zenodo.10291284)
 
 ## Citation
 If you use this package or any part of this code, please cite it! Until we have a paper prepared, please cite this package at software.
 
-Janoski, T. P., & Mitevski, I. (2023, December 7). ClimKern (Version 1.0.0). Retrieved from https://pypi.org/project/climkern/1.0.0/. <https://doi.org/10.5281/zenodo.10291284>.
+Janoski, T. P., & Mitevski, I. (2024, April 6). ClimKern (Version 1.1.0). Retrieved from https://pypi.org/project/climkern/1.1.0/. <https://doi.org/10.5281/zenodo.10291284>.
 
 ## Overview
 
 The radiative kernel technique outlined in [Soden & Held (2006)](https://journals.ametsoc.org/view/journals/clim/19/14/jcli3799.1.xml) and [Soden et al. (2008)](https://journals.ametsoc.org/view/journals/clim/21/14/2007jcli2110.1.xml) is commonly used to calculate climate feedbacks. The "kernels" refer to datasets containing the radiative sensitivities of TOA (or surface) radiation to changes in fields such as temperature, specific humidity, and surface albedo; they are typically computed using offline radiative transfer calculations.
 
 ClimKern
 * standardizes the assumptions used in producing radiative feedbacks using kernels
 * simplifies the calculations by giving users access to functions tailored for climate model output
 * provides access to a repository of **12 different radiative kernels** to quantify interkernel spread
 
+The below information is meant to be a quickstart guide, but all functions and capabilities can be found at ClimKern's [documentation site](https://tyfolino.github.io/climkern/).
+
 ## Installation
 
-ClimKern is built on the architecture of Xarray and requires several other packages for compatibility with climate model output. The easiest method to install is to create a new conda environment with prerequisite packages using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) or [mamba](https://mamba-framework.readthedocs.io/en/latest/installation_guide.html):  
-`conda create -n ck_env python=3.9 esmpy xarray xesmf cftime pooch tqdm importlib-resources plac netcdf4 -c conda-forge`  
-or  
-`mamba create -n ck_env python=3.9 esmpy xarray xesmf cftime pooch tqdm importlib-resources plac netcdf4 -c conda-forge` 
-<br></br>Then, activate the environment:  
-`conda activate ck_env`  
-or  
-`mamba activate ck_env` 
-<br></br>
-Finally, install ClimKern with [pip](https://pip.pypa.io/en/stable/#):  
-`pip install -i https://test.pypi.org/simple/ climkern`
-<br></br>
-Once installed, ClimKern requires kernels found on [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10223376). These kernels (and tutorial data) are stored separately because of PyPI size limitations. You can download the kernels easily using the download script included in the package.  
+ClimKern is built on the Xarray architecture and requires several other packages for
+regridding and climate model output compatibility. The easiest method is to create a
+new conda environment using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) or [mamba](https://mamba-framework.readthedocs.io/en/latest/installation_guide.html):
+
+`conda create -n ck_env python=3.10 esmpy -c conda-forge`
+
+A conda environment is necessary because [ESMPy](https://earthsystemmodeling.org/esmpy/), which is required for regridding kernels, is unavailable via `pip`.
+
+Next, activate the new environment:
+
+`conda activate ck_env`
+
+Finally, install ClimKern with [pip](https://pip.pypa.io/en/stable/#):
+
+`pip install climkern`
+
+Once installed, ClimKern requires kernels found on [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10223376). These kernels (and tutorial data) are stored separately because of PyPI size limitations. You can download the kernels easily using the download script included in the package:  
+
 `python -m climkern download`
 
+Note: The kernels & tutorial data are approximately 5.5 GB.
+
+<i>Optional</i>:
+
+You can test your installation via pytest.
+
+```
+pip install pytest
+pytest -v --pyargs climkern
+```
+
+All three tests should pass.
+
 ## Basic tutorial
 ### Temperature, water vapor, and surface albedo feedbacks
 
-This brief tutorial will cover the basics of using ClimKern before more complete documentation can be written (I'm only one person, here!). We start by importing ClimKern and accessing our tutorial data:
+This brief tutorial will cover the basics of using ClimKern. Please check the [documentation](https://tyfolino.github.io/climkern/) for a more complete list of available functions. We start by importing ClimKern and accessing our tutorial data:
 ```python
 import climkern as ck
 
 ctrl,pert = ck.tutorial_data('ctrl'),ck.tutorial_data('pert')
 ```
 
 These datasets have all the necessary variables for computing feedbacks. Let's start with temperature feedbacks.
@@ -145,17 +168,26 @@
     val=(ck.spat_avg(cld_lw)/dTS_glob_avg).mean()))
 ```
 Expected result:
 >`The global average SW cloud feedback is 0.48 W/m^2/K.`
 >
 >`The global average LW cloud feedback is 0.02 W/m^2/K.`
 
+## Troubleshooting
+
+If you are having issues downloading dependencies with `pip`, you can also try adding them to your conda environment with `conda`, i.e.:
+
+`conda install xesmf -c conda-forge`
+
+If you are having trouble downloading the  kernels and tutorial data using the package's download function, you can also download the data directly from the [Zenodo repository](https://zenodo.org/doi/10.5281/zenodo.10223376) and put it in the climkern/data directory located wherever your conda/mamba environments are stored.
+
 ## Other features & coming soon
 ClimKern has several other useful features:
 - Four different methods for calculating water vapor feedbacks.
 - The ability to calculate the "relative humidity" version of all feedbacks following [Held & Shell (2012)](https://journals.ametsoc.org/view/journals/clim/25/8/jcli-d-11-00721.1.xml) and [Zelinka et al. (2020)](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019GL085782).
 - Functions to calculate stratospheric temperature and water vapor feedbacks.
 
-We are continuously updating the package and are working on improved documentation. For now, we recommend exploring the other functions by referencing the package with a "?" in a Jupyter notebook.
+We are continuously updating the package. Please check out the [GitHub issues page](https://github.com/tyfolino/climkern/issues) for this repository for plans for new features.
 
 ## Want to help? Get involved!
-Our hope is that this package will be useful to the climate science community and we appreciate any contributions our fellow scientists and programmers can offer. For more information and to get involved, email Ty at <tjanoski@ccny.cuny.edu>. 
+
+We deeply appreciate contributions from other scientists and programmers and are happy to attribute credit accordingly. If you wish to contribute, please create a fork or branch from the `dev` channel (<b>not</b> `main`) and submit a pull request when you are done with your changes.
```

