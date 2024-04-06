# Comparing `tmp/botsonrails-0.1.0.tar.gz` & `tmp/botsonrails-0.1.2.tar.gz`

## Comparing `botsonrails-0.1.0.tar` & `botsonrails-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 botsonrails-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/NLX.iml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/__about__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/__init__.py
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/decorators.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/nodes.py
--rw-r--r--   0        0        0    40015 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/rails.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/stores.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/types.py
--rw-r--r--   0        0        0    16382 2020-02-02 00:00:00.000000 botsonrails-0.1.0/BotsOnRails/utils.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/about.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/index.md
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/loops.md
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/node_syntax.md
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/quickstart.md
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/resumable_workflows.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/validation.md
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/test.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/content_moderation/.gitignore
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/content_moderation/credentials.json.env
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/content_moderation/main.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/content_moderation/requirements.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/.gitignore
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/Digraph.gv
--rw-r--r--   0        0        0    25814 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/Digraph.gv.pdf
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/credentials.json.env
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/display.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/main.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/models.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/requirements.txt
--rw-r--r--   0        0        0   120592 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/docs/airbnb/Airbnb-COI.pdf
--rw-r--r--   0        0        0   116806 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/docs/palantir/Palantir-COI.pdf
--rw-r--r--   0        0        0   114125 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/llamaindex/docs/toast/Toast-COI.pdf
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/.gitignore
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/Digraph.gv
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/Digraph.gv.pdf
--rw-r--r--   0        0        0     9782 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/agent.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/credentials.json.sample
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/requirements.txt
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 botsonrails-0.1.0/docs/examples/marvin/sample_doc.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_cycle_validations.py
--rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_for_each_router.py
--rw-r--r--   0        0        0    13385 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_function_type_checking.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_node_routers.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_resumable_execution.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_tree_execution.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_tree_utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_tree_utils.py
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_tree_validations.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/test_tree_visualizations.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/fixtures/tmp/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/fixtures/visualizations/graphviz_visual.dot
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/fixtures/visualizations/graphviz_visual.dot.pdf
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/fixtures/visualizations/test_nx_visualization.png
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 botsonrails-0.1.0/tests/fixtures/visualizations/tree_dump.json
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 botsonrails-0.1.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 botsonrails-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 botsonrails-0.1.0/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 botsonrails-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 botsonrails-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.gitattributes
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 botsonrails-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/NLX.iml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/__about__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/__init__.py
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/decorators.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/nodes.py
+-rw-r--r--   0        0        0    40015 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/rails.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/stores.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/types.py
+-rw-r--r--   0        0        0    18971 2020-02-02 00:00:00.000000 botsonrails-0.1.2/BotsOnRails/utils.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/about.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/loops.md
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/node_syntax.md
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/quickstart.md
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/resumable_workflows.md
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/validation.md
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/test.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/content_moderation/.gitignore
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/content_moderation/credentials.json.env
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/content_moderation/main.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/content_moderation/requirements.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/.gitignore
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/Digraph.gv
+-rw-r--r--   0        0        0    25814 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/Digraph.gv.pdf
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/credentials.json.env
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/display.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/main.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/models.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/requirements.txt
+-rw-r--r--   0        0        0   120592 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/docs/airbnb/Airbnb-COI.pdf
+-rw-r--r--   0        0        0   116806 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/docs/palantir/Palantir-COI.pdf
+-rw-r--r--   0        0        0   114125 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/llamaindex/docs/toast/Toast-COI.pdf
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/.gitignore
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/Digraph.gv
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/Digraph.gv.pdf
+-rw-r--r--   0        0        0     9782 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/agent.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/credentials.json.sample
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/requirements.txt
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 botsonrails-0.1.2/docs/examples/marvin/sample_doc.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_cycle_validations.py
+-rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_for_each_router.py
+-rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_function_type_checking.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_node_routers.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_resumable_execution.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_tree_execution.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_tree_utilities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_tree_utils.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_tree_validations.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/test_tree_visualizations.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/fixtures/tmp/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/fixtures/visualizations/graphviz_visual.dot
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/fixtures/visualizations/graphviz_visual.dot.pdf
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/fixtures/visualizations/test_nx_visualization.png
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 botsonrails-0.1.2/tests/fixtures/visualizations/tree_dump.json
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 botsonrails-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 botsonrails-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 botsonrails-0.1.2/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 botsonrails-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 botsonrails-0.1.2/PKG-INFO
```

### Comparing `botsonrails-0.1.0/.github/workflows/ci.yaml` & `botsonrails-0.1.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/BotsOnRails/decorators.py` & `botsonrails-0.1.2/BotsOnRails/decorators.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/BotsOnRails/nodes.py` & `botsonrails-0.1.2/BotsOnRails/nodes.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/BotsOnRails/rails.py` & `botsonrails-0.1.2/BotsOnRails/rails.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/BotsOnRails/stores.py` & `botsonrails-0.1.2/BotsOnRails/stores.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/BotsOnRails/utils.py` & `botsonrails-0.1.2/BotsOnRails/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -353,7 +353,73 @@
         path.pop()
 
     visited = set()
     dfs(root_node_id, [], None, visited)
 
     cycle_tuples = [(cycle[0], cycle[-1]) for cycle in cycles]
     return cycle_tuples, for_each_paths
+
+
+from typing import Union, Optional, get_args, get_origin
+
+
+def is_union_type(target_type) -> bool:
+    origin = get_origin(target_type)
+    return origin is Union
+
+def is_optional_type(target_type) -> bool:
+    origin = get_origin(target_type)
+    return origin is Optional
+
+def check_union_or_optional_overlaps(input_type, output_type):
+    """
+    Check if two typing annotations (input and output) are potentially compatible.
+
+    This function considers Union types and Optional types. If either the input or output
+    is a Union type, it checks for any overlap between the allowed types. If either is an
+    Optional type, it checks compatibility with the non-None type.
+
+    Args:
+        input_type: The input typing annotation.
+        output_type: The output typing annotation.
+
+    Returns:
+        bool: True if the input and output types are potentially compatible, False otherwise.
+
+    Examples:
+        >>> check_union_or_optional_overlaps(str, Optional[str])
+        True
+        >>> check_union_or_optional_overlaps(int, Union[None, str, int])
+        True
+        >>> check_union_or_optional_overlaps(float, Union[str, int])
+        False
+        >>> check_union_or_optional_overlaps(Union[str, int], Union[int, float])
+        True
+        >>> check_union_or_optional_overlaps(Optional[str], int)
+        False
+    """
+    # Check if either input or output is a Union type
+    input_origin = get_origin(input_type)
+    output_origin = get_origin(output_type)
+
+    if input_origin is Union or output_origin is Union:
+        # If both are Union types, check if there's any overlap
+        if input_origin is Union and output_origin is Union:
+            input_args = get_args(input_type)
+            output_args = get_args(output_type)
+            return any(arg in output_args for arg in input_args)
+
+        # If only one is a Union type, check if the other is in the Union
+        if input_origin is Union:
+            return output_type in get_args(input_type)
+        else:
+            return input_type in get_args(output_type)
+
+    # Check if either input or output is an Optional type
+    if input_origin is Union and type(None) in get_args(input_type):
+        return check_union_or_optional_overlaps(get_args(input_type)[0], output_type)
+
+    if output_origin is Union and type(None) in get_args(output_type):
+        return check_union_or_optional_overlaps(input_type, get_args(output_type)[0])
+
+    # If neither is a Union or Optional, check for equality
+    return input_type == output_type
```

### Comparing `botsonrails-0.1.0/docs/about.md` & `botsonrails-0.1.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/index.md` & `botsonrails-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/loops.md` & `botsonrails-0.1.2/docs/loops.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/node_syntax.md` & `botsonrails-0.1.2/docs/node_syntax.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/quickstart.md` & `botsonrails-0.1.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/resumable_workflows.md` & `botsonrails-0.1.2/docs/resumable_workflows.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/validation.md` & `botsonrails-0.1.2/docs/validation.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/test.py` & `botsonrails-0.1.2/docs/examples/test.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/content_moderation/main.py` & `botsonrails-0.1.2/docs/examples/content_moderation/main.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/Digraph.gv` & `botsonrails-0.1.2/docs/examples/llamaindex/Digraph.gv`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/Digraph.gv.pdf` & `botsonrails-0.1.2/docs/examples/llamaindex/Digraph.gv.pdf`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/display.py` & `botsonrails-0.1.2/docs/examples/llamaindex/display.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/main.py` & `botsonrails-0.1.2/docs/examples/llamaindex/main.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/models.py` & `botsonrails-0.1.2/docs/examples/llamaindex/models.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/docs/airbnb/Airbnb-COI.pdf` & `botsonrails-0.1.2/docs/examples/llamaindex/docs/airbnb/Airbnb-COI.pdf`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/docs/palantir/Palantir-COI.pdf` & `botsonrails-0.1.2/docs/examples/llamaindex/docs/palantir/Palantir-COI.pdf`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/llamaindex/docs/toast/Toast-COI.pdf` & `botsonrails-0.1.2/docs/examples/llamaindex/docs/toast/Toast-COI.pdf`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/marvin/Digraph.gv` & `botsonrails-0.1.2/docs/examples/marvin/Digraph.gv`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/marvin/Digraph.gv.pdf` & `botsonrails-0.1.2/docs/examples/marvin/Digraph.gv.pdf`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/marvin/agent.py` & `botsonrails-0.1.2/docs/examples/marvin/agent.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/docs/examples/marvin/sample_doc.txt` & `botsonrails-0.1.2/docs/examples/marvin/sample_doc.txt`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_cycle_validations.py` & `botsonrails-0.1.2/tests/test_cycle_validations.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_for_each_router.py` & `botsonrails-0.1.2/tests/test_for_each_router.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_function_type_checking.py` & `botsonrails-0.1.2/tests/test_function_type_checking.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 from typing import Tuple, Optional, List, Union, NoReturn, Dict, Callable
 
 from BotsOnRails.decorators import step_decorator_for_path
 from BotsOnRails.rails import ExecutionPath
+from BotsOnRails.utils import check_union_or_optional_overlaps
 
 
 class TestTypeChecking(unittest.TestCase):
     def test_simple_types(self):
         tree = ExecutionPath()
         node = step_decorator_for_path(tree)
 
@@ -409,10 +410,17 @@
             if isinstance(x, dict):
                 return sum(x["numbers"])
             return 0
 
         tree.compile(type_checking=True)
         assert tree.run() == 6
 
+    def test_check_union_or_optional_overlaps(self):
+        assert check_union_or_optional_overlaps(str, Optional[str]) == True
+        assert check_union_or_optional_overlaps(int, Union[None, str, int]) == True
+        assert check_union_or_optional_overlaps(float, Union[str, int]) == False
+        assert check_union_or_optional_overlaps(Union[str, int], Union[int, float]) == True
+        assert check_union_or_optional_overlaps(Optional[str], int) == False
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `botsonrails-0.1.0/tests/test_node_routers.py` & `botsonrails-0.1.2/tests/test_node_routers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import unittest
-from typing import NoReturn
-
-from BotsOnRails.decorators import step_decorator_for_path
-from BotsOnRails.rails import ExecutionPath
-
-
-class TestNodeRouting(unittest.TestCase):
-    def test_dict_router(self):
-        tree = ExecutionPath()
-        node = step_decorator_for_path(tree)
-
-        @node(next_step={"valid": "handle_valid", "invalid": "handle_invalid"}, path_start=True)
-        def wrapped_dict_routing(input_str: str, **kwargs) -> str:
-            return input_str
-
-        @node()
-        def handle_valid(input: str, **kwargs):
-            return "Congrats!"
-
-        @node()
-        def handle_invalid(input: str, **kwargs):
-            return "Aww, too bad"
-
-        tree.compile()
-
-        print("Result:")
-        print(tree.run('valid'))
-
-        assert tree.run('valid') == "Congrats!"
-        assert tree.run('invalid') == "Aww, too bad"
-
-    def test_functional_router(self):
-
-        tree = ExecutionPath()
-        node = step_decorator_for_path(tree)
-
-        def route_function(input: int) -> str:
-            if input % 3 == 0:
-                return 'comedy_comes_in_threes'
-            return 'boring_boring'
-
-        @node(
-            path_start=True,
-            next_step=route_function,
-            func_router_possible_next_step_names=[
-                'boring_boring',
-                'comedy_comes_in_threes'
-            ]
-        )
-        def start_node(input: int, **kwargs) -> int:
-            """
-            Where we just want an initial router, we can pass through the input value to the output. You could
-            also process the input here too, of course.
-            """
-            return input
-
-        @node()
-        def boring_boring(input: int, **kwargs) -> str:
-            return "Have I told you about the benefits of a high fiber diet?"
-
-        @node()
-        def comedy_comes_in_threes(value: int, **kwargs) -> NoReturn:
-            return f"Did I tell you the one about the {value} that walked into a bar?"
-
-        tree.compile(type_checking=True)
-        assert tree.run(4) == 'Have I told you about the benefits of a high fiber diet?'
-        assert tree.run(3) == 'Did I tell you the one about the 3 that walked into a bar?'
-
-    def test_functional_routing_with_no_annot(self):
-        """
-        Where we use a functional router, we require you provide a list of possible outputs so we can
-        produce a visualization showing the possible execution pathway.
-        """
-        tree = ExecutionPath()
-        node = step_decorator_for_path(tree)
-
-        def route_function(input: int) -> str:
-            if input % 3 == 0:
-                return 'comedy_comes_in_threes'
-            return 'boring_boring'
-
-        # Leave off the func_router_possible_next_step_names
-        @node(
-            path_start=True,
-            next_step=route_function
-        )
-        def start_node(input: int, **kwargs) -> int:
-            return input
-
-        @node()
-        def boring_boring(input: int, **kwargs) -> str:
-            return "Have I told you about the benefits of a high fiber diet?"
-
-        @node()
-        def comedy_comes_in_threes(value: int, **kwargs) -> NoReturn:
-            return f"Did I tell you the one about the {value} that walked into a bar?"
-
-        with self.assertRaises(ValueError):
-            tree.compile(type_checking=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from typing import NoReturn
+
+from BotsOnRails.decorators import step_decorator_for_path
+from BotsOnRails.rails import ExecutionPath
+
+
+class TestNodeRouting(unittest.TestCase):
+    def test_dict_router(self):
+        tree = ExecutionPath()
+        node = step_decorator_for_path(tree)
+
+        @node(next_step={"valid": "handle_valid", "invalid": "handle_invalid"}, path_start=True)
+        def wrapped_dict_routing(input_str: str, **kwargs) -> str:
+            return input_str
+
+        @node()
+        def handle_valid(input: str, **kwargs):
+            return "Congrats!"
+
+        @node()
+        def handle_invalid(input: str, **kwargs):
+            return "Aww, too bad"
+
+        tree.compile()
+
+        print("Result:")
+        print(tree.run('valid'))
+
+        assert tree.run('valid') == "Congrats!"
+        assert tree.run('invalid') == "Aww, too bad"
+
+    def test_functional_router(self):
+
+        tree = ExecutionPath()
+        node = step_decorator_for_path(tree)
+
+        def route_function(input: int) -> str:
+            if input % 3 == 0:
+                return 'comedy_comes_in_threes'
+            return 'boring_boring'
+
+        @node(
+            path_start=True,
+            next_step=route_function,
+            func_router_possible_next_step_names=[
+                'boring_boring',
+                'comedy_comes_in_threes'
+            ]
+        )
+        def start_node(input: int, **kwargs) -> int:
+            """
+            Where we just want an initial router, we can pass through the input value to the output. You could
+            also process the input here too, of course.
+            """
+            return input
+
+        @node()
+        def boring_boring(input: int, **kwargs) -> str:
+            return "Have I told you about the benefits of a high fiber diet?"
+
+        @node()
+        def comedy_comes_in_threes(value: int, **kwargs) -> NoReturn:
+            return f"Did I tell you the one about the {value} that walked into a bar?"
+
+        tree.compile(type_checking=True)
+        assert tree.run(4) == 'Have I told you about the benefits of a high fiber diet?'
+        assert tree.run(3) == 'Did I tell you the one about the 3 that walked into a bar?'
+
+    def test_functional_routing_with_no_annot(self):
+        """
+        Where we use a functional router, we require you provide a list of possible outputs so we can
+        produce a visualization showing the possible execution pathway.
+        """
+        tree = ExecutionPath()
+        node = step_decorator_for_path(tree)
+
+        def route_function(input: int) -> str:
+            if input % 3 == 0:
+                return 'comedy_comes_in_threes'
+            return 'boring_boring'
+
+        # Leave off the func_router_possible_next_step_names
+        @node(
+            path_start=True,
+            next_step=route_function
+        )
+        def start_node(input: int, **kwargs) -> int:
+            return input
+
+        @node()
+        def boring_boring(input: int, **kwargs) -> str:
+            return "Have I told you about the benefits of a high fiber diet?"
+
+        @node()
+        def comedy_comes_in_threes(value: int, **kwargs) -> NoReturn:
+            return f"Did I tell you the one about the {value} that walked into a bar?"
+
+        with self.assertRaises(ValueError):
+            tree.compile(type_checking=True)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `botsonrails-0.1.0/tests/test_resumable_execution.py` & `botsonrails-0.1.2/tests/test_resumable_execution.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_tree_execution.py` & `botsonrails-0.1.2/tests/test_tree_execution.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_tree_utilities.py` & `botsonrails-0.1.2/tests/test_tree_utilities.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_tree_validations.py` & `botsonrails-0.1.2/tests/test_tree_validations.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/test_tree_visualizations.py` & `botsonrails-0.1.2/tests/test_tree_visualizations.py`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/fixtures/visualizations/graphviz_visual.dot.pdf` & `botsonrails-0.1.2/tests/fixtures/visualizations/graphviz_visual.dot.pdf`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/tests/fixtures/visualizations/test_nx_visualization.png` & `botsonrails-0.1.2/tests/fixtures/visualizations/test_nx_visualization.png`

 * *Files 1% similar despite different names*

#### sng

```diff
@@ -2,15 +2,15 @@
 IHDR {
     width: 1066; height: 1066; bitdepth: 8;
     using color alpha;
 }
 pHYs {xpixels: 3937; ypixels: 3937; per: meter;}  # (100 dpi)
 tEXt {
     keyword: "Software";
-    text: "Matplotlib version3.8.3, https://matplotlib.org/";
+    text: "Matplotlib version3.8.4, https://matplotlib.org/";
 }
 IMAGE {
     pixels hex
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff
```

### Comparing `botsonrails-0.1.0/tests/fixtures/visualizations/tree_dump.json` & `botsonrails-0.1.2/tests/fixtures/visualizations/tree_dump.json`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/.gitignore` & `botsonrails-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/LICENSE.txt` & `botsonrails-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/README.md` & `botsonrails-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/pyproject.toml` & `botsonrails-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `botsonrails-0.1.0/PKG-INFO` & `botsonrails-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: BotsOnRails
-Version: 0.1.0
+Version: 0.1.2
 Summary: BotsOnRails makes it easy to write LLM-controlled programs without outsourcing all of the logic and decisions to stochastic models. It facilitates the seamless integration of function-based nodes into an execution tree, enabling conditional and sequential task execution tailored to complex, resumable processing flows.
 Project-URL: Documentation, https://github.com/JSv4/BotsOnRails#readme
 Project-URL: Issues, https://github.com/JSv4/BotsOnRails/issues
 Project-URL: Source, https://github.com/JSv4/BotsOnRails
 Author-email: JSv4 <scrudato@umich.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
```

