# Comparing `tmp/efootprint-1.3.2.tar.gz` & `tmp/efootprint-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efootprint-1.3.2.tar", max compression
+gzip compressed data, was "efootprint-2.0.0.tar", max compression
```

## Comparing `efootprint-1.3.2.tar` & `efootprint-2.0.0.tar`

### file list

```diff
@@ -1,54 +1,63 @@
--rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-1.3.2/LICENSE
--rw-r--r--   0        0        0     3456 2024-03-20 20:43:07.972219 efootprint-1.3.2/README.md
--rw-r--r--   0        0        0        0 2024-03-20 20:43:08.661396 efootprint-1.3.2/efootprint/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-1.3.2/efootprint/abstract_modeling_classes/__init__.py
--rw-r--r--   0        0        0    11880 2024-03-20 18:43:51.365759 efootprint-1.3.2/efootprint/abstract_modeling_classes/explainable_object_base_class.py
--rw-r--r--   0        0        0     2240 2024-03-08 17:07:16.555575 efootprint-1.3.2/efootprint/abstract_modeling_classes/explainable_object_dict.py
--rw-r--r--   0        0        0    12607 2024-03-08 17:07:16.560057 efootprint-1.3.2/efootprint/abstract_modeling_classes/explainable_objects.py
--rw-r--r--   0        0        0    17405 2024-03-20 20:43:08.668865 efootprint-1.3.2/efootprint/abstract_modeling_classes/modeling_object.py
--rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-1.3.2/efootprint/abstract_modeling_classes/source_objects.py
--rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-1.3.2/efootprint/api_utils/__init__.py
--rw-r--r--   0        0        0     5639 2024-03-20 18:43:51.368997 efootprint-1.3.2/efootprint/api_utils/json_to_system.py
--rw-r--r--   0        0        0     1358 2024-03-20 20:43:08.679663 efootprint-1.3.2/efootprint/api_utils/system_to_json.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-1.3.2/efootprint/builders/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-1.3.2/efootprint/builders/hardware/__init__.py
--rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-1.3.2/efootprint/builders/hardware/devices_defaults.py
--rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-1.3.2/efootprint/builders/hardware/network_defaults.py
--rw-r--r--   0        0        0     8980 2024-03-04 16:55:02.041839 efootprint-1.3.2/efootprint/builders/hardware/servers_boaviztapi.py
--rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-1.3.2/efootprint/builders/hardware/servers_defaults.py
--rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-1.3.2/efootprint/builders/hardware/storage_defaults.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-1.3.2/efootprint/constants/__init__.py
--rw-r--r--   0        0        0     4182 2024-03-15 15:47:43.137993 efootprint-1.3.2/efootprint/constants/countries.py
--rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-1.3.2/efootprint/constants/custom_units.txt
--rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-1.3.2/efootprint/constants/files.py
--rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-1.3.2/efootprint/constants/sources.py
--rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-1.3.2/efootprint/constants/units.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-1.3.2/efootprint/core/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-1.3.2/efootprint/core/hardware/__init__.py
--rw-r--r--   0        0        0     6034 2024-03-15 15:47:43.140928 efootprint-1.3.2/efootprint/core/hardware/device_population.py
--rw-r--r--   0        0        0     5707 2024-03-15 15:47:43.144566 efootprint-1.3.2/efootprint/core/hardware/hardware_base_classes.py
--rw-r--r--   0        0        0     3367 2024-03-15 15:47:43.146858 efootprint-1.3.2/efootprint/core/hardware/network.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-1.3.2/efootprint/core/hardware/servers/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-1.3.2/efootprint/core/hardware/servers/autoscaling.py
--rw-r--r--   0        0        0     3766 2024-03-04 16:55:01.236244 efootprint-1.3.2/efootprint/core/hardware/servers/on_premise.py
--rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-1.3.2/efootprint/core/hardware/servers/server_base_class.py
--rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-1.3.2/efootprint/core/hardware/servers/serverless.py
--rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-1.3.2/efootprint/core/hardware/storage.py
--rw-r--r--   0        0        0     5388 2024-03-15 15:47:43.150188 efootprint-1.3.2/efootprint/core/service.py
--rw-r--r--   0        0        0    10031 2024-03-15 15:47:43.152518 efootprint-1.3.2/efootprint/core/system.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-1.3.2/efootprint/core/usage/__init__.py
--rw-r--r--   0        0        0     3890 2024-03-15 15:47:43.155499 efootprint-1.3.2/efootprint/core/usage/usage_pattern.py
--rw-r--r--   0        0        0     7069 2024-03-15 15:47:43.160015 efootprint-1.3.2/efootprint/core/usage/user_journey.py
--rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-1.3.2/efootprint/logger.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-1.3.2/efootprint/utils/__init__.py
--rw-r--r--   0        0        0     3055 2024-03-15 15:47:43.162389 efootprint-1.3.2/efootprint/utils/calculus_graph.py
--rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-1.3.2/efootprint/utils/dev_utils/README.md
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-1.3.2/efootprint/utils/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-1.3.2/efootprint/utils/dev_utils/page_weights.py
--rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-1.3.2/efootprint/utils/dev_utils/selenium_screenshot.py
--rw-r--r--   0        0        0     1407 2024-03-20 20:43:08.683131 efootprint-1.3.2/efootprint/utils/graph_tools.py
--rw-r--r--   0        0        0     2357 2024-03-20 20:43:08.691495 efootprint-1.3.2/efootprint/utils/object_relationships_graphs.py
--rw-r--r--   0        0        0     7596 2024-03-15 15:47:43.172640 efootprint-1.3.2/efootprint/utils/plot_emission_diffs.py
--rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-1.3.2/efootprint/utils/tools.py
--rw-r--r--   0        0        0     1258 2024-03-20 20:43:08.711273 efootprint-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.0.0/efootprint/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.0.0/efootprint/abstract_modeling_classes/__init__.py
+-rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_base_class.py
+-rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_dict.py
+-rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_objects.py
+-rw-r--r--   0        0        0    17405 2024-04-06 12:40:52.176669 efootprint-2.0.0/efootprint/abstract_modeling_classes/modeling_object.py
+-rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.0.0/efootprint/abstract_modeling_classes/source_objects.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.0.0/efootprint/api_utils/__init__.py
+-rw-r--r--   0        0        0     5499 2024-04-06 16:25:45.616333 efootprint-2.0.0/efootprint/api_utils/json_to_system.py
+-rw-r--r--   0        0        0     1306 2024-04-06 16:25:45.620494 efootprint-2.0.0/efootprint/api_utils/system_to_json.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.0.0/efootprint/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.0.0/efootprint/builders/hardware/__init__.py
+-rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.0.0/efootprint/builders/hardware/devices_defaults.py
+-rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.0.0/efootprint/builders/hardware/network_defaults.py
+-rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.0.0/efootprint/builders/hardware/servers_boaviztapi.py
+-rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.0.0/efootprint/builders/hardware/servers_defaults.py
+-rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.0.0/efootprint/builders/hardware/storage_defaults.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:25:45.621704 efootprint-2.0.0/efootprint/builders/usage/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-06 16:25:45.623649 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-06 16:25:45.624639 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-06 17:04:29.583138 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
+-rw-r--r--   0        0        0     3888 2024-04-06 17:04:45.906689 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
+-rw-r--r--   0        0        0     1827 2024-04-06 16:46:25.107263 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
+-rw-r--r--   0        0        0    67861 2024-04-06 16:25:45.634291 efootprint-2.0.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.0.0/efootprint/constants/__init__.py
+-rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.0.0/efootprint/constants/countries.py
+-rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.0.0/efootprint/constants/custom_units.txt
+-rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.0.0/efootprint/constants/files.py
+-rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.0.0/efootprint/constants/sources.py
+-rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.0.0/efootprint/constants/units.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.0.0/efootprint/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.0.0/efootprint/core/hardware/__init__.py
+-rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.0.0/efootprint/core/hardware/device_population.py
+-rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.0.0/efootprint/core/hardware/hardware_base_classes.py
+-rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.0.0/efootprint/core/hardware/network.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.0.0/efootprint/core/hardware/servers/__init__.py
+-rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.0.0/efootprint/core/hardware/servers/autoscaling.py
+-rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.0.0/efootprint/core/hardware/servers/on_premise.py
+-rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.0.0/efootprint/core/hardware/servers/server_base_class.py
+-rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.0.0/efootprint/core/hardware/servers/serverless.py
+-rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.0.0/efootprint/core/hardware/storage.py
+-rw-r--r--   0        0        0     5312 2024-04-06 16:25:45.643459 efootprint-2.0.0/efootprint/core/service.py
+-rw-r--r--   0        0        0    10359 2024-04-06 16:25:45.650082 efootprint-2.0.0/efootprint/core/system.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.0.0/efootprint/core/usage/__init__.py
+-rw-r--r--   0        0        0     3995 2024-04-06 16:25:45.651955 efootprint-2.0.0/efootprint/core/usage/job.py
+-rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.0.0/efootprint/core/usage/usage_pattern.py
+-rw-r--r--   0        0        0     2723 2024-04-06 16:25:45.657976 efootprint-2.0.0/efootprint/core/usage/user_journey.py
+-rw-r--r--   0        0        0     1510 2024-04-06 16:25:45.660815 efootprint-2.0.0/efootprint/core/usage/user_journey_step.py
+-rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.0.0/efootprint/logger.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.0.0/efootprint/utils/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.0.0/efootprint/utils/calculus_graph.py
+-rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.0.0/efootprint/utils/dev_utils/README.md
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.0.0/efootprint/utils/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.0.0/efootprint/utils/dev_utils/page_weights.py
+-rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.0.0/efootprint/utils/dev_utils/selenium_screenshot.py
+-rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.0.0/efootprint/utils/graph_tools.py
+-rw-r--r--   0        0        0     2390 2024-04-06 16:50:31.330325 efootprint-2.0.0/efootprint/utils/object_relationships_graphs.py
+-rw-r--r--   0        0        0     7612 2024-04-06 16:26:15.688584 efootprint-2.0.0/efootprint/utils/plot_emission_diffs.py
+-rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.0.0/efootprint/utils/tools.py
+-rw-r--r--   0        0        0     1258 2024-04-06 17:10:56.033814 efootprint-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.0.0/PKG-INFO
```

### Comparing `efootprint-1.3.2/LICENSE` & `efootprint-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/README.md` & `efootprint-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/abstract_modeling_classes/explainable_object_base_class.py` & `efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/abstract_modeling_classes/explainable_object_dict.py` & `efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_object_dict.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/abstract_modeling_classes/explainable_objects.py` & `efootprint-2.0.0/efootprint/abstract_modeling_classes/explainable_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/abstract_modeling_classes/modeling_object.py` & `efootprint-2.0.0/efootprint/abstract_modeling_classes/modeling_object.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/abstract_modeling_classes/source_objects.py` & `efootprint-2.0.0/efootprint/abstract_modeling_classes/source_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/api_utils/json_to_system.py` & `efootprint-2.0.0/efootprint/api_utils/json_to_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from efootprint.abstract_modeling_classes.explainable_objects import ExplainableQuantity, ExplainableHourlyUsage
 from efootprint.abstract_modeling_classes.source_objects import SourceObject
-from efootprint.utils.tools import time_it
 from efootprint.abstract_modeling_classes.explainable_object_base_class import ExplainableObject, Source
 from efootprint.abstract_modeling_classes.explainable_object_dict import ExplainableObjectDict
 from efootprint.constants.units import u
 from efootprint.core.service import Service
 from efootprint.core.system import System
 from efootprint.core.hardware.storage import Storage
 from efootprint.core.hardware.servers.autoscaling import Autoscaling
 from efootprint.core.hardware.servers.serverless import Serverless
 from efootprint.core.hardware.servers.on_premise import OnPremise
 from efootprint.core.hardware.hardware_base_classes import Hardware
 from efootprint.core.usage.usage_pattern import UsagePattern
-from efootprint.core.usage.user_journey import UserJourney, UserJourneyStep
+from efootprint.core.usage.user_journey import UserJourney
+from efootprint.core.usage.job import Job
+from efootprint.core.usage.user_journey_step import UserJourneyStep
 from efootprint.core.hardware.network import Network
 from efootprint.core.hardware.device_population import DevicePopulation
 from efootprint.constants.countries import Country
 
 import pytz
 import json
 
@@ -41,15 +42,14 @@
     elif "zone" in input_dict.keys():
         output = SourceObject(
             pytz.timezone(input_dict["zone"]), source, input_dict["label"])
 
     return output
 
 
-@time_it
 def json_to_system(system_dict):
     class_obj_dict = {}
     flat_obj_dict = {}
 
     for class_key in system_dict.keys():
         if class_key not in class_obj_dict.keys():
             class_obj_dict[class_key] = {}
@@ -82,18 +82,14 @@
                         if type(elt) == str and elt in flat_obj_dict.keys():
                             output_val.append(flat_obj_dict[elt])
                             flat_obj_dict[elt].add_obj_to_modeling_obj_containers(mod_obj)
                     mod_obj.__dict__[attr_key] = output_val
             mod_obj.__dict__["dont_handle_input_updates"] = False
             mod_obj.__dict__["init_has_passed"] = True
 
-    for class_key in ["UserJourneyStep", "UserJourney"]:
-        for mod_obj_key, mod_obj in class_obj_dict[class_key].items():
-            mod_obj.compute_calculated_attributes()
-
     for mod_obj_key, mod_obj in class_obj_dict["DevicePopulation"].items():
         mod_obj.user_journey_freq_per_up = ExplainableObjectDict()
         mod_obj.nb_user_journeys_in_parallel_during_usage_per_up = ExplainableObjectDict()
         mod_obj.utc_time_intervals_per_up = ExplainableObjectDict()
 
     for mod_obj_key, mod_obj in class_obj_dict["System"].items():
         mod_obj.launch_attributes_computation_chain()
```

### Comparing `efootprint-1.3.2/efootprint/api_utils/system_to_json.py` & `efootprint-2.0.0/efootprint/api_utils/system_to_json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from efootprint.utils.tools import time_it
 from efootprint.abstract_modeling_classes.modeling_object import ModelingObject
 
 import json
 
 
 def recursively_write_json_dict(output_dict, mod_obj, save_calculated_attributes=True):
     mod_obj_class = mod_obj.class_as_simple_str
@@ -16,15 +15,14 @@
             elif type(value) == list and len(value) > 0 and issubclass(type(value[0]), ModelingObject):
                 for mod_obj_elt in value:
                     recursively_write_json_dict(output_dict, mod_obj_elt, save_calculated_attributes)
 
     return output_dict
 
 
-@time_it
 def system_to_json(input_system, save_calculated_attributes, output_filepath=None):
     output_dict = {}
     recursively_write_json_dict(output_dict, input_system, save_calculated_attributes)
 
     if output_filepath is not None:
         with open(output_filepath, "w") as file:
             file.write(json.dumps(output_dict, indent=4))
```

### Comparing `efootprint-1.3.2/efootprint/builders/hardware/devices_defaults.py` & `efootprint-2.0.0/efootprint/builders/hardware/devices_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/builders/hardware/network_defaults.py` & `efootprint-2.0.0/efootprint/builders/hardware/network_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/builders/hardware/servers_boaviztapi.py` & `efootprint-2.0.0/efootprint/builders/hardware/servers_boaviztapi.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/builders/hardware/servers_defaults.py` & `efootprint-2.0.0/efootprint/builders/hardware/servers_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/builders/hardware/storage_defaults.py` & `efootprint-2.0.0/efootprint/builders/hardware/storage_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/constants/countries.py` & `efootprint-2.0.0/efootprint/constants/countries.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/constants/sources.py` & `efootprint-2.0.0/efootprint/constants/sources.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/device_population.py` & `efootprint-2.0.0/efootprint/core/hardware/device_population.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/hardware_base_classes.py` & `efootprint-2.0.0/efootprint/core/hardware/hardware_base_classes.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/network.py` & `efootprint-2.0.0/efootprint/core/hardware/network.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/servers/autoscaling.py` & `efootprint-2.0.0/efootprint/core/hardware/servers/autoscaling.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/servers/on_premise.py` & `efootprint-2.0.0/efootprint/core/hardware/servers/on_premise.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/servers/server_base_class.py` & `efootprint-2.0.0/efootprint/core/hardware/servers/server_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/servers/serverless.py` & `efootprint-2.0.0/efootprint/core/hardware/servers/serverless.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/hardware/storage.py` & `efootprint-2.0.0/efootprint/core/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/core/service.py` & `efootprint-2.0.0/efootprint/core/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,36 +41,36 @@
         return ["hour_by_hour_ram_need", "hour_by_hour_cpu_need", "storage_needed"]
 
     @property
     def modeling_objects_whose_attributes_depend_directly_on_me(self) -> List[ModelingObject]:
         return [self.server, self.storage]
 
     @property
-    def uj_steps(self):
+    def jobs(self):
         return self.modeling_obj_containers
 
     @property
     def usage_patterns(self):
-        return list(set(sum([uj_step.usage_patterns for uj_step in self.uj_steps], start=[])))
+        return list(set(sum([job.usage_patterns for job in self.jobs], start=[])))
 
     @property
     def systems(self) -> List:
         return list(set(sum([up.systems for up in self.usage_patterns], start=[])))
 
     def update_storage_needed(self):
         if len(self.usage_patterns) == 0:
             self.storage_needed = ExplainableQuantity(
                 0 * u.TB / u.year,
                 f"No storage for {self.name} because no associated user journey steps with usage pattern")
         else:
             storage_needs = 0
-            for uj_step in self.uj_steps:
-                uj_step_up = uj_step.usage_patterns
-                if len(uj_step_up) > 0:
-                    storage_needs += uj_step.data_upload * sum(up.user_journey_freq for up in uj_step_up)
+            for job in self.jobs:
+                job_up = job.usage_patterns
+                if len(job_up) > 0:
+                    storage_needs += job.data_upload * sum(up.user_journey_freq for up in job_up)
 
             self.storage_needed = storage_needs.to(u.TB / u.year).set_label(
                 f"Storage needed for {self.name}")
 
     def compute_hour_by_hour_resource_need(self, resource):
         resource_unit = u(self.resources_unit_dict[resource])
         one_user_journey = ExplainableQuantity(1 * u.user_journey, "One user journey")
@@ -81,27 +81,27 @@
                     f"{self.name} is installed on {self.server.name} but unused, so it consumes "
                     f"{base_resource_consumption.value} of {resource} for nothing.")
             return ExplainableHourlyUsage(
                 [0 * resource_unit] * 24,
                 f"No {resource} need for {self.name} because no associated user journey steps with usage pattern")
         else:
             hour_by_hour_resource_needs = 0
-            for uj_step in self.uj_steps:
-                for usage_pattern in uj_step.usage_patterns:
+            for job in self.jobs:
+                for usage_pattern in job.usage_patterns:
                     average_uj_resource_needed_for_up = (
-                        getattr(uj_step, f"{resource}_needed") * uj_step.request_duration /
+                        getattr(job, f"{resource}_needed") * job.request_duration /
                         (usage_pattern.user_journey.duration * one_user_journey)).to(
                         resource_unit / u.user_journey).set_label(
-                        f"Average {resource} needed over {usage_pattern.name} to process {uj_step.name}")
+                        f"Average {resource} needed over {usage_pattern.name} to process {job.name}")
 
                     hour_by_hour_resource_needs += (
                             (average_uj_resource_needed_for_up * usage_pattern.nb_user_journeys_in_parallel_during_usage)
                             * usage_pattern.utc_time_intervals)
 
             return hour_by_hour_resource_needs.set_label(
                 f"{self.name} hour by hour {resource} need")
 
     def update_hour_by_hour_ram_need(self):
-            self.hour_by_hour_ram_need = self.compute_hour_by_hour_resource_need("ram")
+        self.hour_by_hour_ram_need = self.compute_hour_by_hour_resource_need("ram")
 
     def update_hour_by_hour_cpu_need(self):
-            self.hour_by_hour_cpu_need = self.compute_hour_by_hour_resource_need("cpu")
+        self.hour_by_hour_cpu_need = self.compute_hour_by_hour_resource_need("cpu")
```

### Comparing `efootprint-1.3.2/efootprint/core/system.py` & `efootprint-2.0.0/efootprint/core/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from efootprint.constants.units import u
 from efootprint.core.hardware.network import Network
 from efootprint.core.hardware.device_population import DevicePopulation
 from efootprint.core.hardware.servers.server_base_class import Server
 from efootprint.core.hardware.storage import Storage
 from efootprint.core.service import Service
 from efootprint.core.usage.usage_pattern import UsagePattern
+from efootprint.core.usage.user_journey import UserJourney
 from efootprint.abstract_modeling_classes.explainable_objects import ExplainableQuantity
 from efootprint.utils.plot_emission_diffs import EmissionPlotter
 from efootprint.utils.tools import format_co2_amount, display_co2_amount
 
 from typing import Dict, List, Set
 import plotly.express as px
 import plotly
@@ -27,66 +28,74 @@
         self.previous_total_energy_footprints = None
         self.previous_total_fabrication_footprints = None
         self.all_changes = []
         self.initial_total_energy_footprints = None
         self.initial_total_fabrication_footprints = None
 
     @property
+    def user_journeys(self) -> List[UserJourney]:
+        output_set = set()
+        for usage_pattern in self.usage_patterns:
+            output_set.update({usage_pattern.user_journey})
+
+        return list(output_set)
+
+    @property
     def modeling_objects_whose_attributes_depend_directly_on_me(self):
-        return self.usage_patterns
+        return self.user_journeys
 
     @property
     def systems(self) -> List:
         return []
 
     def after_init(self):
         self.init_has_passed = True
         self.launch_attributes_computation_chain()
         self.initial_total_energy_footprints = self.total_energy_footprints
         self.initial_total_fabrication_footprints = self.total_fabrication_footprints
 
     @property
-    def servers(self) -> Set[Server]:
+    def servers(self) -> List[Server]:
         output_set = set()
         for usage_pattern in self.usage_patterns:
             output_set.update(usage_pattern.user_journey.servers)
 
-        return output_set
+        return list(output_set)
 
     @property
-    def storages(self) -> Set[Storage]:
+    def storages(self) -> List[Storage]:
         output_set = set()
         for usage_pattern in self.usage_patterns:
             output_set.update(usage_pattern.user_journey.storages)
 
-        return output_set
+        return list(output_set)
 
     @property
-    def services(self) -> Set[Service]:
+    def services(self) -> List[Service]:
         output_set = set()
         for usage_pattern in self.usage_patterns:
             output_set.update(usage_pattern.user_journey.services)
 
-        return output_set
+        return list(output_set)
 
     @property
-    def device_populations(self) -> Set[DevicePopulation]:
+    def device_populations(self) -> List[DevicePopulation]:
         output_set = set()
         for usage_pattern in self.usage_patterns:
             output_set.update({usage_pattern.device_population})
 
-        return output_set
+        return list(output_set)
 
     @property
-    def networks(self) -> Set[Network]:
+    def networks(self) -> List[Network]:
         output_set = set()
         for usage_pattern in self.usage_patterns:
             output_set.update({usage_pattern.network})
 
-        return output_set
+        return list(output_set)
 
     def get_storage_by_name(self, storage_name) -> Storage:
         for storage in self.storages:
             if storage.name == storage_name:
                 return storage
 
     def get_server_by_name(self, server_name) -> Server:
```

### Comparing `efootprint-1.3.2/efootprint/core/usage/usage_pattern.py` & `efootprint-2.0.0/efootprint/core/usage/usage_pattern.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/logger.py` & `efootprint-2.0.0/efootprint/logger.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/utils/calculus_graph.py` & `efootprint-2.0.0/efootprint/utils/calculus_graph.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/utils/dev_utils/selenium_screenshot.py` & `efootprint-2.0.0/efootprint/utils/dev_utils/selenium_screenshot.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/utils/graph_tools.py` & `efootprint-2.0.0/efootprint/utils/graph_tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/efootprint/utils/object_relationships_graphs.py` & `efootprint-2.0.0/efootprint/utils/object_relationships_graphs.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 COLOR_MAP = {
     "Autoscaling": "red",
     "OnPremise": "red",
     "Serverless": "red",
     "Hardware": "red",
     "Storage": "red",
-    "Service": "deepskyblue",
-    "UsagePattern": "blueviolet",
+    "Service": "gold",
+    "UsagePattern": "mediumblue",
     "DevicePopulation": "red",
-    "UserJourney": "gold",
-    "UserJourneyStep": "gold",
+    "UserJourney": "dodgerblue",
+    "UserJourneyStep": "deepskyblue",
     "TimeIntervals": "gold",
+    "Job": "palegoldenrod"
 }
 
 USAGE_PATTERN_VIEW_CLASSES_TO_IGNORE = [
     "System", "Network", "Hardware", "Country"]
 SERVICES_VIEW_CLASSES_TO_IGNORE = [
     "System", "UsagePattern", "TimeIntervals", "Network", "Server", "Storage", "Hardware", "DevicePopulation"]
 SERVICES_AND_INFRA_VIEW_CLASSES_TO_IGNORE = [
```

### Comparing `efootprint-1.3.2/efootprint/utils/plot_emission_diffs.py` & `efootprint-2.0.0/efootprint/utils/plot_emission_diffs.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             if rounded_total__new - rounded_total__old > 0:
                 plus_sign = "+"
             subtitle_text = f"From {rounded_total__old} to {rounded_total__new} {unit}s of CO2 emissions in" \
                             f" {self.timespan.value} " \
                             f"({plus_sign}{int(100 * (rounded_total__new - rounded_total__old) / rounded_total__old)}%)"
         else:
             subtitle_text = f"{rounded_total__new} {unit}s of CO2 emissions in {self.timespan.value}"
-        subtitle_text.replace("in 1 year", "per year")
+        subtitle_text = subtitle_text.replace("in 1 year", "per year")
 
         self.ax.text(
             0.5, 1.1, subtitle_text,
             transform=self.ax.transAxes, fontsize=16, va="top", ha="center")
 
     def plot_emission_diffs(self):
         for i, (input_dict_old, input_dict_new) in enumerate(
```

### Comparing `efootprint-1.3.2/efootprint/utils/tools.py` & `efootprint-2.0.0/efootprint/utils/tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-1.3.2/pyproject.toml` & `efootprint-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "efootprint"
-version = "1.3.2"
+version = "2.0.0"
 description = "Digital service environmental footprint model"
 authors = ["Vincent Villet for Publicis Sapient"]
 readme = "README.md"
 include = ["efootprint/constants/custom_units.txt"]
 
 [tool.black]
 line-length = 120
```

### Comparing `efootprint-1.3.2/PKG-INFO` & `efootprint-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efootprint
-Version: 1.3.2
+Version: 2.0.0
 Summary: Digital service environmental footprint model
 Author: Vincent Villet for Publicis Sapient
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

