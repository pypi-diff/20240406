# Comparing `tmp/hesmapy-23.12.1.tar.gz` & `tmp/hesmapy-24.4.1.tar.gz`

## Comparing `hesmapy-23.12.1.tar` & `hesmapy-24.4.1.tar`

### file list

```diff
@@ -1,25 +1,37 @@
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hesmapy-23.12.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 hesmapy-23.12.1/SCHEMA.md
--rw-r--r--   0        0        0    32879 2020-02-02 00:00:00.000000 hesmapy-23.12.1/examples/hydro/hydro_1d.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/base.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/hydro/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/hydro/hydro1d.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/hydro/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/utils/__init__.py
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/utils/plot_utils.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/utils/writer_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/writers/__init__.py
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 hesmapy-23.12.1/src/hesmapy/writers/hydro1d.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 hesmapy-23.12.1/tests/test_hydro1d.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 hesmapy-23.12.1/tests/test_hydro_utils.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 hesmapy-23.12.1/tests/test_loader.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 hesmapy-23.12.1/tests/test_writer_utils.py
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 hesmapy-23.12.1/tests/test_writers_hydro1d.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 hesmapy-23.12.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 hesmapy-23.12.1/LICENSE
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hesmapy-23.12.1/README.md
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 hesmapy-23.12.1/pyproject.toml
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 hesmapy-23.12.1/PKG-INFO
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hesmapy-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 hesmapy-24.4.1/SCHEMA.md
+-rw-r--r--   0        0        0    32879 2020-02-02 00:00:00.000000 hesmapy-24.4.1/examples/hydro/hydro_1d.json
+-rw-r--r--   0        0        0   183168 2020-02-02 00:00:00.000000 hesmapy-24.4.1/examples/rt/rt_lightcurve.json
+-rw-r--r--   0        0        0    80948 2020-02-02 00:00:00.000000 hesmapy-24.4.1/examples/rt/rt_spectrum.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/base.py
+-rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/constants.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/json_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/hydro/__init__.py
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/hydro/hydro1d.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/hydro/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/rt/__init__.py
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/rt/lightcurves.py
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/rt/spectra.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/utils/__init__.py
+-rw-r--r--   0        0        0    14704 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/utils/plot_utils.py
+-rw-r--r--   0        0        0    14126 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/utils/writer_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/writers/__init__.py
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/writers/hydro1d.py
+-rw-r--r--   0        0        0    12172 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/writers/rt_lightcurve.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 hesmapy-24.4.1/src/hesmapy/writers/rt_spectrum.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_hydro1d.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_hydro_utils.py
+-rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_loader.py
+-rw-r--r--   0        0        0    10059 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_rt_lightcurve.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_rt_spectrum.py
+-rw-r--r--   0        0        0    26208 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_writer_utils.py
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_writers_hydro1d.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_writers_rt_lightcurve.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 hesmapy-24.4.1/tests/test_writers_rt_spectrum.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 hesmapy-24.4.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 hesmapy-24.4.1/LICENSE
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hesmapy-24.4.1/README.md
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 hesmapy-24.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hesmapy-24.4.1/PKG-INFO
```

### Comparing `hesmapy-23.12.1/examples/hydro/hydro_1d.json` & `hesmapy-24.4.1/examples/hydro/hydro_1d.json`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/src/hesmapy/hydro/hydro1d.py` & `hesmapy-24.4.1/src/hesmapy/hydro/hydro1d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,95 +1,25 @@
-import json
-from jsonschema import ValidationError, validate
 import plotly.graph_objects as go
 import pandas as pd
+
+from hesmapy.json_base import HesmaBaseJSONFile
 from hesmapy.utils.plot_utils import (
     add_timestep_slider,
     plot_hydro_traces,
     add_log_axis_buttons,
     plot_abundance_traces,
 )
 from hesmapy.hydro.utils import normalize_hydro1d_data, get_abundance_data
-from hesmapy.constants import HYDRO1D_JSON_SCHEMA
+from hesmapy.constants import HYDRO1D_JSON_SCHEMA, ARB_UNIT_STRING
 
 
-class Hydro1D:
+class Hydro1D(HesmaBaseJSONFile):
     def __init__(self, path) -> None:
         self.schema = HYDRO1D_JSON_SCHEMA
-
-        self.path = path
-        self.data = self._load_data()
-
-        # Naively assume that the data is valid
-        self.valid = True
-
-        self.models = []
-        self.multi_model = self._multiple_models()
-
-        self.valid = self._validate_data()
-
-    def _multiple_models(self) -> bool:
-        # This is a hacky way to deal with multiple models and individual
-        # models at the same time
-        if isinstance(self.data, dict):
-            self.models = list(self.data.keys())
-        elif isinstance(self.data, list):
-            for item in self.data:
-                if isinstance(item, dict):
-                    self.models.append(list(item.keys())[0])
-                else:
-                    self.valid = False
-                    break
-            else:
-                # Put all data in a single dict so we don't have to deal with
-                # with a list of dicts
-                data = {}
-                for i, item in enumerate(self.data):
-                    modelname = self.models[i]
-                    # Avoid duplicate keys
-                    if modelname in data:
-                        modelname = f"{modelname}_{i}"
-                    data[modelname] = item[self.models[i]]
-                    self.models[i] = modelname
-                self.data = data
-        else:
-            # This collects all the edge cases I can't think of
-            self.models = []
-            self.valid = False
-        return len(self.models) > 1
-
-    def _load_data(self) -> dict:
-        with open(self.path) as f:
-            try:
-                data = json.load(f)
-            except json.decoder.JSONDecodeError:
-                raise IOError("Invalid JSON file")
-        return data
-
-    def _validate_data(self) -> bool:
-        for model in self.models:
-            try:
-                validate(self.data[model], schema=self.schema)
-            except ValidationError:
-                return False
-
-        # TODO: Check if all data has the same length
-        return True
-
-    def _get_model(self, model: str | int = None) -> str:
-        if model is None:
-            model = self.models[0]
-        elif isinstance(model, int):
-            assert model < len(self.models), "Invalid model index"
-            model = self.models[model]
-        elif isinstance(model, str):
-            assert model in self.models, "Invalid model name"
-        else:
-            raise TypeError("Invalid model type")
-        return model
+        super().__init__(path)
 
     def get_unique_times(self, model: str | int = None) -> list:
         """
         Get the unique time steps for a model.
         Returns an empty list if the data is invalid
 
         Parameters
@@ -158,45 +88,45 @@
             raise NotImplementedError("Getting units of invalid data not implemented")
 
         model = self._get_model(model=model)
 
         radius_unit = (
             self.data[model]["units"]["radius"]
             if "radius" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         density_unit = (
             self.data[model]["units"]["density"]
             if "density" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         pressure_unit = (
             self.data[model]["units"]["pressure"]
             if "pressure" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         temperature_unit = (
             self.data[model]["units"]["temperature"]
             if "temperature" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         mass_unit = (
             self.data[model]["units"]["mass"]
             if "mass" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         velocity_unit = (
             self.data[model]["units"]["velocity"]
             if "velocity" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         time_unit = (
             self.data[model]["units"]["time"]
             if "time" in self.data[model]["units"]
-            else "(arb. units)"
+            else ARB_UNIT_STRING
         )
         units = {
             "radius": radius_unit,
             "density": density_unit,
             "pressure": pressure_unit,
             "temperature": temperature_unit,
             "mass": mass_unit,
```

### Comparing `hesmapy-23.12.1/src/hesmapy/hydro/utils.py` & `hesmapy-24.4.1/src/hesmapy/hydro/utils.py`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/src/hesmapy/writers/hydro1d.py` & `hesmapy-24.4.1/src/hesmapy/writers/hydro1d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import json
 import pandas as pd
 import numpy as np
 
 from hesmapy.utils.writer_utils import (
+    _check_data_dataframe,
+    _check_data_dict,
     _check_sources,
-    _check_units,
+    _check_hydro1d_units,
     _check_model_names,
     _check_numpy_array,
     _hydro1d_dataframe_to_json_dict,
 )
 from hesmapy.constants import HYDRO1D_ABUNDANCE_REGEX
 
 
@@ -57,29 +59,19 @@
     the HESMA scheme will be written to the JSON file.
 
     """
 
     if os.path.exists(path) and not overwrite:
         raise IOError(f"File {path} already exists")
 
-    if isinstance(data, pd.DataFrame):
-        data = [data]
-    elif isinstance(data, list):
-        if not all(isinstance(df, pd.DataFrame) for df in data):
-            raise TypeError("data must be a DataFrame or a list of DataFrames")
-    else:
-        raise TypeError("data must be a DataFrame or a list of DataFrames")
-
-    for i, df in enumerate(data):
-        if not all(col in df.columns for col in ["time", "density", "radius"]):
-            raise ValueError(f"DataFrame {i} does not contain the necessary columns")
+    data = _check_data_dataframe(data, columns=["time", "density", "radius"])
 
     model_names = _check_model_names(model_names, len(data))
     sources = _check_sources(sources)
-    units = _check_units(units)
+    units = _check_hydro1d_units(units)
 
     hydro = {}
 
     for i, df in enumerate(data):
         data_dict = _hydro1d_dataframe_to_json_dict(df, model_names[i], sources, units)
         hydro[model_names[i]] = data_dict[model_names[i]]
 
@@ -132,21 +124,15 @@
     - density
     - radius
     Other columns are optional. Only columns compliant with
     the HESMA scheme will be written to the JSON file.
 
     """
 
-    if isinstance(data, dict):
-        data = [data]
-    elif isinstance(data, list):
-        if not all(isinstance(df, dict) for df in data):
-            raise TypeError("data must be a dict or a list of dicts")
-    else:
-        raise TypeError("data must be a dict or a list of dicts")
+    data = _check_data_dict(data)
 
     data_dfs = []
     for i, df in enumerate(data):
         data_dfs.append(pd.DataFrame(df))
 
     write_hydro1d_from_dataframe(
         data_dfs,
@@ -173,15 +159,15 @@
     units: dict = None,
     overwrite: bool = False,
     create_path: bool = True,
     **kwargs,
 ) -> None:
     """
     Write a 1D Hydrodynamical model to a JSON file
-    compatible with the HESMA scheme from a dict.
+    compatible with the HESMA scheme from numpy arrays.
 
     Parameters
     ----------
     radius : np.ndarray | list[np.ndarray]
         Radius of the model cells.
     density : np.ndarray | list[np.ndarray]
         Density of the model cells.
@@ -259,17 +245,17 @@
         if len(time) != len(radius):
             raise ValueError(
                 "time must be a float or an array with the same length as"
                 " the number of models"
             )
 
     data_dfs = []
-    for i, df in enumerate(radius):
+    for i, r in enumerate(radius):
         data = {
-            "radius": radius[i],
+            "radius": r,
             "density": density[i],
             "time": time[i],
         }
         if pressure is not None:
             data["pressure"] = pressure[i]
         if temperature is not None:
             data["temperature"] = temperature[i]
@@ -277,16 +263,15 @@
             data["mass"] = mass[i]
         if velocity is not None:
             data["velocity"] = velocity[i]
         if abundances is not None:
             for key in abundances.keys():
                 data[key] = abundances[key][i]
 
-        df = pd.DataFrame(data)
-        data_dfs.append(pd.DataFrame(df))
+        data_dfs.append(pd.DataFrame(data))
 
     write_hydro1d_from_dataframe(
         data_dfs,
         path,
         model_names=model_names,
         sources=sources,
         units=units,
```

### Comparing `hesmapy-23.12.1/tests/test_hydro1d.py` & `hesmapy-24.4.1/tests/test_hydro1d.py`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/tests/test_hydro_utils.py` & `hesmapy-24.4.1/tests/test_hydro_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         self.assertEqual(normalization_factors["temperature"], 2)
         self.assertEqual(normalization_factors["mass"], 2)
         self.assertEqual(normalization_factors["velocity"], 2)
 
     def test_get_abundance_data(self):
         data = pd.DataFrame(self.valid_data["model"]["data"])
         abundances = get_abundance_data(data, 1)
-        print(abundances)
         self.assertEqual(abundances["xC12"].iloc[1], 0.9)
 
     def test_get_abundance_data_empty(self):
         data = pd.DataFrame(self.valid_data_empty_abundances["model"]["data"])
         abundances = get_abundance_data(data, 1)
         self.assertEqual(abundances.empty, True)
```

### Comparing `hesmapy-23.12.1/tests/test_writers_hydro1d.py` & `hesmapy-24.4.1/tests/test_writers_hydro1d.py`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/.gitignore` & `hesmapy-24.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/LICENSE` & `hesmapy-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/pyproject.toml` & `hesmapy-24.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hesmapy-23.12.1/PKG-INFO` & `hesmapy-24.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hesmapy
-Version: 23.12.1
+Version: 24.4.1
 Summary: HESMA file format reader and writer
 Project-URL: Homepage, https://github.com/alexhls/hesmapy
 Project-URL: Bug Tracker, https://github.com/alexhls/hesmapy/issues
 Author-email: Alexander Holas <alex.holas@gmx.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # Hesmapy
 
 ![PyPI - Version](https://img.shields.io/pypi/v/hesmapy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/hesmapy)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10404977.svg)](https://doi.org/10.5281/zenodo.10404977)
 
 HESMA Python - Tools for reading HESMA models
 
 ## Documentation
 Full documentation can be found [here](https://alexhls.github.io/hesmapy/).
 
 ## Installation
@@ -63,12 +64,48 @@
 ```
 model.plot(show_plot=True)
 ```
 Model files can be written by providing either a ``pd.DataFrame``, ``dict`` or several ``np.ndarray``.
 See the documentation for more details.
 
 ### RT
-*(Not yet implemented)*
+
+#### Lightcurves
+This module contains the tools for lightcurves and data derived from them. See below for some basic usage examples.
+
+Loading models:
+```python
+import hesmapy.base as hp
+model = hp.load_rt_lightcurve("examples/rt/rt_lightcurve.json")
+```
+Get the data from a model as a ``pd.DataFrame``:
+```python
+df = model.get_data()
+```
+Plot a model:
+```
+model.plot(show_plot=True)
+```
+
+#### Spectra
+This module contains the tools for spectra(l timeseries). See below for some basic usage examples.
+
+Loading models:
+```python
+import hesmapy.base as hp
+model = hp.load_rt_spectrum("examples/rt/rt_spectrum.json")
+```
+Get the data from a model as a list of ``pd.DataFrame`` (one for each timestep):
+```python
+dfs = model.get_data()
+```
+Plot a model:
+```
+model.plot(show_plot=True)``````
+
+
+Model files can be written by providing either a ``pd.DataFrame``, ``dict`` or several ``np.ndarray``.
+See the documentation for more details.
 
 ### Tracer
 *(Not yet implemented)*
```

