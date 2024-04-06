# Comparing `tmp/wwpdb.utils.db-0.30.tar.gz` & `tmp/wwpdb.utils.db-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.db-0.30.tar", last modified: Sat Sep  2 11:43:14 2023, max compression
+gzip compressed data, was "wwpdb.utils.db-0.31.tar", last modified: Sat Apr  6 20:51:15 2024, max compression
```

## Comparing `wwpdb.utils.db-0.30.tar` & `wwpdb.utils.db-0.31.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-09-02 11:43:14.268747 wwpdb.utils.db-0.30/
--rw-r--r--   0 vsts      (1001) docker     (999)      719 2023-09-02 11:43:14.268747 wwpdb.utils.db-0.30/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (999)      212 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/README.md
--rw-r--r--   0 vsts      (1001) docker     (999)      108 2023-09-02 11:43:14.268747 wwpdb.utils.db-0.30/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (999)     2165 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-09-02 11:43:14.256747 wwpdb.utils.db-0.30/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (999)       65 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-09-02 11:43:14.256747 wwpdb.utils.db-0.30/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (999)       65 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-09-02 11:43:14.268747 wwpdb.utils.db-0.30/wwpdb/utils/db/
--rw-r--r--   0 vsts      (1001) docker     (999)   237963 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/BirdSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)   154030 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/ChemCompSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)     4802 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/DBLoadUtil.py
--rw-r--r--   0 vsts      (1001) docker     (999)   260559 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/DaInternalSchemaDef.py
--rwxr-xr-x   0 vsts      (1001) docker     (999)    22118 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/DbLoadingApi.py
--rw-r--r--   0 vsts      (1001) docker     (999)     7042 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MessageSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)     8889 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MyConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (999)    19146 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (999)    30645 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MyDbSqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (999)    17636 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (999)    23832 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MyQueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (999)     4815 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (999)   606730 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/PdbDistroSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)  3724930 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/PdbxSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)    12178 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (999)   150992 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/PrdChemCompSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)    15722 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/SchemaDefBase.py
--rw-r--r--   0 vsts      (1001) docker     (999)    26185 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (999)     7057 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/SqlLoader.py
--rw-r--r--   0 vsts      (1001) docker     (999)    12147 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistory.py
--rw-r--r--   0 vsts      (1001) docker     (999)     6744 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistoryExec.py
--rw-r--r--   0 vsts      (1001) docker     (999)     8873 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistorySchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)    32566 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistoryUtils.py
--rw-r--r--   0 vsts      (1001) docker     (999)     1829 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/StatusLoadWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (999)    27651 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/WorkflowSchemaDef.py
--rw-r--r--   0 vsts      (1001) docker     (999)      154 2023-09-02 11:41:57.000000 wwpdb.utils.db-0.30/wwpdb/utils/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-09-02 11:43:14.256747 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (999)      719 2023-09-02 11:43:14.000000 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (999)     1177 2023-09-02 11:43:14.000000 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (999)        1 2023-09-02 11:43:14.000000 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (999)        1 2023-09-02 11:42:56.000000 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (999)      139 2023-09-02 11:43:14.000000 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (999)        6 2023-09-02 11:43:14.000000 wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.157198 wwpdb.utils.db-0.31/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-06 20:51:15.157198 wwpdb.utils.db-0.31/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      212 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-06 20:51:15.157198 wwpdb.utils.db-0.31/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2165 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.141197 wwpdb.utils.db-0.31/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.145197 wwpdb.utils.db-0.31/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.153198 wwpdb.utils.db-0.31/wwpdb/utils/db/
+-rw-r--r--   0 vsts      (1001) docker     (127)   237963 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/BirdSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   166675 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/ChemCompSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4802 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/DBLoadUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   260559 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/DaInternalSchemaDef.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    22118 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/DbLoadingApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7042 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MessageSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8889 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19146 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30645 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbSqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17636 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23832 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MyQueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4815 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   606730 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PdbDistroSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  3724930 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12178 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   150992 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/PrdChemCompSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26185 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7057 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/SqlLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12147 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6744 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8873 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistorySchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32566 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1829 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/StatusLoadWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27651 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/WorkflowSchemaDef.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-06 20:49:46.000000 wwpdb.utils.db-0.31/wwpdb/utils/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:51:15.153198 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1026 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1177 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 20:50:54.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      139 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-06 20:51:15.000000 wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.db-0.30/setup.py` & `wwpdb.utils.db-0.31/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/BirdSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/BirdSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/ChemCompSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/PrdChemCompSchemaDef.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 ##
-# File:    ChemCompSchemaDef.py
-# Author:  J. Westbrook
-# Date:    12-Jan-2013
+# File:    PrdChemCompSchemaDef.py
+# Author:  E. Peisach
+# Date:    18-Mar-2022
 # Version: 0.001 Initial version
 #
 # Updates:
-#    5-Dec-2016 jdw add program and program version to pdbx_chem_comp_identifier table
 ##
 """
-Database schema defintions for chemical component definitions.
+Database schema defintions for Bird PRD/FAMILY reference data.
 
 """
 __docformat__ = "restructuredtext en"
-__author__    = "John Westbrook"
-__email__     = "jwest@rcsb.rutgers.edu"
+__author__    = "Ezra Peisach"
+__email__     = "ezra.peisach@rcsb.org"
 __license__   = "Creative Commons Attribution 3.0 Unported"
 __version__   = "V0.001"
 
 import sys
 from wwpdb.utils.db.SchemaDefBase import SchemaDefBase
 
 
-class ChemCompSchemaDef(SchemaDefBase):
-    """ A data class containing schema definitions chemical component definitions.
+class PrdChemCompSchemaDef(SchemaDefBase):
+    """ A data class containing schema definitions for deposition related messages.
     """
-    _databaseName="compv4"
-    _schemaDefDict ={
+    _databaseName = "prdccv4"
+    _schemaDefDict = {
         'CHEM_COMP': {'ATTRIBUTES': {'COMPONENT_ID': 'Component_ID',
                                      'FORMULA': 'formula',
                                      'FORMULA_WEIGHT': 'formula_weight',
                                      'ID': 'id',
                                      'MODEL_DETAILS': 'model_details',
                                      'MODEL_ERF': 'model_erf',
                                      'MODEL_SOURCE': 'model_source',
@@ -436,21 +435,18 @@
                                           'MODEL_CARTN_Z': 'model_Cartn_z',
                                           'MODEL_CARTN_Z_ESD': 'model_Cartn_z_esd',
                                           'PARTIAL_CHARGE': 'partial_charge',
                                           'PDBX_ALIGN': 'pdbx_align',
                                           'PDBX_ALT_ATOM_ID': 'pdbx_alt_atom_id',
                                           'PDBX_ALT_COMP_ID': 'pdbx_alt_comp_id',
                                           'PDBX_AROMATIC_FLAG': 'pdbx_aromatic_flag',
-                                          'PDBX_BACKBONE_ATOM_FLAG': 'pdbx_backbone_atom_flag',
-                                          'PDBX_C_TERMINAL_ATOM_FLAG': 'pdbx_c_terminal_atom_flag',
                                           'PDBX_LEAVING_ATOM_FLAG': 'pdbx_leaving_atom_flag',
                                           'PDBX_MODEL_CARTN_X_IDEAL': 'pdbx_model_Cartn_x_ideal',
                                           'PDBX_MODEL_CARTN_Y_IDEAL': 'pdbx_model_Cartn_y_ideal',
                                           'PDBX_MODEL_CARTN_Z_IDEAL': 'pdbx_model_Cartn_z_ideal',
-                                          'PDBX_N_TERMINAL_ATOM_FLAG': 'pdbx_n_terminal_atom_flag',
                                           'PDBX_ORDINAL': 'pdbx_ordinal',
                                           'PDBX_STEREO_CONFIG': 'pdbx_stereo_config',
                                           'PDBX_STND_ATOM_ID': 'pdbx_stnd_atom_id',
                                           'SUBSTRUCT_CODE': 'substruct_code',
                                           'TYPE_SYMBOL': 'type_symbol'},
                            'ATTRIBUTE_INFO': {'ALT_ATOM_ID': {'NULLABLE': True,
                                                               'ORDER': 3,
@@ -544,26 +540,14 @@
                                                                    'WIDTH': 10},
                                               'PDBX_AROMATIC_FLAG': {'NULLABLE': True,
                                                                      'ORDER': 23,
                                                                      'PRECISION': 0,
                                                                      'PRIMARY_KEY': False,
                                                                      'SQL_TYPE': 'VARCHAR',
                                                                      'WIDTH': 10},
-                                              'PDBX_BACKBONE_ATOM_FLAG': {'NULLABLE': True,
-                                                                          'ORDER': 26,
-                                                                          'PRECISION': 0,
-                                                                          'PRIMARY_KEY': False,
-                                                                          'SQL_TYPE': 'VARCHAR',
-                                                                          'WIDTH': 10},
-                                              'PDBX_C_TERMINAL_ATOM_FLAG': {'NULLABLE': True,
-                                                                            'ORDER': 28,
-                                                                            'PRECISION': 0,
-                                                                            'PRIMARY_KEY': False,
-                                                                            'SQL_TYPE': 'VARCHAR',
-                                                                            'WIDTH': 10},
                                               'PDBX_LEAVING_ATOM_FLAG': {'NULLABLE': True,
                                                                          'ORDER': 24,
                                                                          'PRECISION': 0,
                                                                          'PRIMARY_KEY': False,
                                                                          'SQL_TYPE': 'VARCHAR',
                                                                          'WIDTH': 10},
                                               'PDBX_MODEL_CARTN_X_IDEAL': {'NULLABLE': True,
@@ -580,20 +564,14 @@
                                                                            'WIDTH': 10},
                                               'PDBX_MODEL_CARTN_Z_IDEAL': {'NULLABLE': True,
                                                                            'ORDER': 21,
                                                                            'PRECISION': 6,
                                                                            'PRIMARY_KEY': False,
                                                                            'SQL_TYPE': 'FLOAT',
                                                                            'WIDTH': 10},
-                                              'PDBX_N_TERMINAL_ATOM_FLAG': {'NULLABLE': True,
-                                                                            'ORDER': 27,
-                                                                            'PRECISION': 0,
-                                                                            'PRIMARY_KEY': False,
-                                                                            'SQL_TYPE': 'VARCHAR',
-                                                                            'WIDTH': 10},
                                               'PDBX_ORDINAL': {'NULLABLE': True,
                                                                'ORDER': 16,
                                                                'PRECISION': 0,
                                                                'PRIMARY_KEY': False,
                                                                'SQL_TYPE': 'INT',
                                                                'WIDTH': 10},
                                               'PDBX_STEREO_CONFIG': {'NULLABLE': True,
@@ -632,22 +610,14 @@
                                              'MODEL_CARTN_Z': ('chem_comp_atom', 'model_Cartn_z', None, None),
                                              'MODEL_CARTN_Z_ESD': ('chem_comp_atom', 'model_Cartn_z_esd', None, None),
                                              'PARTIAL_CHARGE': ('chem_comp_atom', 'partial_charge', None, None),
                                              'PDBX_ALIGN': ('chem_comp_atom', 'pdbx_align', None, None),
                                              'PDBX_ALT_ATOM_ID': ('chem_comp_atom', 'pdbx_alt_atom_id', None, None),
                                              'PDBX_ALT_COMP_ID': ('chem_comp_atom', 'pdbx_alt_comp_id', None, None),
                                              'PDBX_AROMATIC_FLAG': ('chem_comp_atom', 'pdbx_aromatic_flag', None, None),
-                                             'PDBX_BACKBONE_ATOM_FLAG': ('chem_comp_atom',
-                                                                         'pdbx_backbone_atom_flag',
-                                                                         None,
-                                                                         None),
-                                             'PDBX_C_TERMINAL_ATOM_FLAG': ('chem_comp_atom',
-                                                                           'pdbx_c_terminal_atom_flag',
-                                                                           None,
-                                                                           None),
                                              'PDBX_LEAVING_ATOM_FLAG': ('chem_comp_atom',
                                                                         'pdbx_leaving_atom_flag',
                                                                         None,
                                                                         None),
                                              'PDBX_MODEL_CARTN_X_IDEAL': ('chem_comp_atom',
                                                                           'pdbx_model_Cartn_x_ideal',
                                                                           None,
@@ -656,18 +626,14 @@
                                                                           'pdbx_model_Cartn_y_ideal',
                                                                           None,
                                                                           None),
                                              'PDBX_MODEL_CARTN_Z_IDEAL': ('chem_comp_atom',
                                                                           'pdbx_model_Cartn_z_ideal',
                                                                           None,
                                                                           None),
-                                             'PDBX_N_TERMINAL_ATOM_FLAG': ('chem_comp_atom',
-                                                                           'pdbx_n_terminal_atom_flag',
-                                                                           None,
-                                                                           None),
                                              'PDBX_ORDINAL': ('chem_comp_atom', 'pdbx_ordinal', None, None),
                                              'PDBX_STEREO_CONFIG': ('chem_comp_atom', 'pdbx_stereo_config', None, None),
                                              'PDBX_STND_ATOM_ID': ('chem_comp_atom', 'pdbx_stnd_atom_id', None, None),
                                              'SUBSTRUCT_CODE': ('chem_comp_atom', 'substruct_code', None, None),
                                              'TYPE_SYMBOL': ('chem_comp_atom', 'type_symbol', None, None)},
                            'INDICES': {'p1': {'ATTRIBUTES': ('COMPONENT_ID', 'COMP_ID', 'ATOM_ID'), 'TYPE': 'UNIQUE'},
                                        's1': {'ATTRIBUTES': ('COMPONENT_ID',), 'TYPE': 'SEARCH'}},
@@ -1793,40 +1759,44 @@
                                     'INDICES': {'p1': {'ATTRIBUTES': ('COMPONENT_ID', 'ORDINAL', 'COMP_ID'), 'TYPE': 'UNIQUE'},
                                                 's1': {'ATTRIBUTES': ('COMPONENT_ID',), 'TYPE': 'SEARCH'}},
                                     'MAP_MERGE_INDICES': {'pdbx_chem_comp_synonyms': {'ATTRIBUTES': ('ordinal', 'comp_id'),
                                                                                       'TYPE': 'EQUI-JOIN'}},
                                     'TABLE_DELETE_ATTRIBUTE': 'COMPONENT_ID',
                                     'TABLE_ID': 'PDBX_CHEM_COMP_SYNONYMS',
                                     'TABLE_NAME': 'pdbx_chem_comp_synonyms',
-                                    'TABLE_TYPE': 'transactional'}}
-    
+                                    'TABLE_TYPE': 'transactional'}
+    }
 
-    def __init__(self,verbose=True,log=sys.stderr):
-        super(ChemCompSchemaDef,self).__init__(databaseName=ChemCompSchemaDef._databaseName,schemaDefDict=ChemCompSchemaDef._schemaDefDict,
-                                           verbose=verbose,log=log)
 
 
+    def __init__(self,verbose=True,log=sys.stderr):
+        super(PrdChemCompSchemaDef,self).__init__(databaseName=PrdChemCompSchemaDef._databaseName,schemaDefDict=PrdChemCompSchemaDef._schemaDefDict,
+                                                  verbose=verbose,log=log)
+        
+
 if __name__ == "__main__":
-    sd=ChemCompSchemaDef()
-    tableIdList=sd.getTableIdList()
+    bsd = PrdChemCompSchemaDef()
+    tableIdList = bsd.getTableIdList()
 
     for tableId in tableIdList:
-        aIdL=sd.getAttributeIdList(tableId)
-        tObj=sd.getTable(tableId)
+        aIdL=bsd.getAttributeIdList(tableId)
+        tObj=bsd.getTable(tableId)
         attributeIdList=tObj.getAttributeIdList()
-        attributeNameList=tObj.getAttributeNameList()
+        attributeNameList=tObj.getAttributeNameList()        
         sys.stdout.write("Ordered attribute Id   list %s\n" % (str(attributeIdList)))
-        sys.stdout.write("Ordered attribute name list %s\n" % (str(attributeNameList)))
+        sys.stdout.write("Ordered attribute name list %s\n" % (str(attributeNameList)))        
         #
         mAL=tObj.getMapAttributeNameList()
         sys.stdout.write("Ordered mapped attribute name list %s\n" % (str(mAL)))
 
         mAL=tObj.getMapAttributeIdList()
-        sys.stdout.write("Ordered mapped attribute id   list %s\n" % (str(mAL)))
+        sys.stdout.write("Ordered mapped attribute id   list %s\n" % (str(mAL)))        
 
         cL=tObj.getMapInstanceCategoryList()
         sys.stdout.write("Mapped category list %s\n" % (str(cL)))
         for c in cL:
             aL=tObj.getMapInstanceAttributeList(c)
             sys.stdout.write("Mapped attribute list in %s :  %s\n" % (c,str(aL)))
+            
 
 
+
```

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/DBLoadUtil.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/DBLoadUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/DaInternalSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/DaInternalSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/DbLoadingApi.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/DbLoadingApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MessageSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MessageSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MyConnectionBase.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MyConnectionBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MyDbAdapter.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MyDbSqlGen.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbSqlGen.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MyDbUtil.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MyQueryDirectives.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MyQueryDirectives.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/MysqlSchemaImporter.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/PdbDistroSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/PdbDistroSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/PdbxSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/PdbxSchemaMapReader.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/PrdChemCompSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/ChemCompSchemaDef.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 ##
-# File:    PrdChemCompSchemaDef.py
-# Author:  E. Peisach
-# Date:    18-Mar-2022
+# File:    ChemCompSchemaDef.py
+# Author:  J. Westbrook
+# Date:    12-Jan-2013
 # Version: 0.001 Initial version
 #
 # Updates:
+#    5-Dec-2016 jdw add program and program version to pdbx_chem_comp_identifier table
 ##
 """
-Database schema defintions for Bird PRD/FAMILY reference data.
+Database schema defintions for chemical component definitions.
 
 """
 __docformat__ = "restructuredtext en"
-__author__    = "Ezra Peisach"
-__email__     = "ezra.peisach@rcsb.org"
+__author__    = "John Westbrook"
+__email__     = "jwest@rcsb.rutgers.edu"
 __license__   = "Creative Commons Attribution 3.0 Unported"
 __version__   = "V0.001"
 
 import sys
 from wwpdb.utils.db.SchemaDefBase import SchemaDefBase
 
 
-class PrdChemCompSchemaDef(SchemaDefBase):
-    """ A data class containing schema definitions for deposition related messages.
+class ChemCompSchemaDef(SchemaDefBase):
+    """ A data class containing schema definitions chemical component definitions.
     """
-    _databaseName = "prdccv4"
+    _databaseName="compv4"
     _schemaDefDict = {
         'CHEM_COMP': {'ATTRIBUTES': {'COMPONENT_ID': 'Component_ID',
                                      'FORMULA': 'formula',
                                      'FORMULA_WEIGHT': 'formula_weight',
                                      'ID': 'id',
                                      'MODEL_DETAILS': 'model_details',
                                      'MODEL_ERF': 'model_erf',
@@ -48,14 +49,15 @@
                                      'PDBX_IDEAL_COORDINATES_MISSING_FLAG': 'pdbx_ideal_coordinates_missing_flag',
                                      'PDBX_INITIAL_DATE': 'pdbx_initial_date',
                                      'PDBX_MODEL_COORDINATES_DB_CODE': 'pdbx_model_coordinates_db_code',
                                      'PDBX_MODEL_COORDINATES_DETAILS': 'pdbx_model_coordinates_details',
                                      'PDBX_MODEL_COORDINATES_MISSING_FLAG': 'pdbx_model_coordinates_missing_flag',
                                      'PDBX_MODIFICATION_DETAILS': 'pdbx_modification_details',
                                      'PDBX_MODIFIED_DATE': 'pdbx_modified_date',
+                                     'PDBX_PCM': 'pdbx_pcm',
                                      'PDBX_PROCESSING_SITE': 'pdbx_processing_site',
                                      'PDBX_RELEASE_STATUS': 'pdbx_release_status',
                                      'PDBX_REPLACED_BY': 'pdbx_replaced_by',
                                      'PDBX_REPLACES': 'pdbx_replaces',
                                      'PDBX_SUBCOMPONENT_LIST': 'pdbx_subcomponent_list',
                                      'PDBX_SYNONYMS': 'pdbx_synonyms',
                                      'PDBX_TYPE': 'pdbx_type',
@@ -184,21 +186,21 @@
                                          'PDBX_IDEAL_COORDINATES_MISSING_FLAG': {'NULLABLE': True,
                                                                                  'ORDER': 29,
                                                                                  'PRECISION': 0,
                                                                                  'PRIMARY_KEY': False,
                                                                                  'SQL_TYPE': 'VARCHAR',
                                                                                  'WIDTH': 10},
                                          'PDBX_INITIAL_DATE': {'NULLABLE': True,
-                                                               'ORDER': 35,
+                                                               'ORDER': 36,
                                                                'PRECISION': 0,
                                                                'PRIMARY_KEY': False,
                                                                'SQL_TYPE': 'DATETIME',
                                                                'WIDTH': 15},
                                          'PDBX_MODEL_COORDINATES_DB_CODE': {'NULLABLE': True,
-                                                                            'ORDER': 31,
+                                                                            'ORDER': 32,
                                                                             'PRECISION': 0,
                                                                             'PRIMARY_KEY': False,
                                                                             'SQL_TYPE': 'VARCHAR',
                                                                             'WIDTH': 30},
                                          'PDBX_MODEL_COORDINATES_DETAILS': {'NULLABLE': True,
                                                                             'ORDER': 27,
                                                                             'PRECISION': 0,
@@ -214,27 +216,33 @@
                                          'PDBX_MODIFICATION_DETAILS': {'NULLABLE': True,
                                                                        'ORDER': 20,
                                                                        'PRECISION': 0,
                                                                        'PRIMARY_KEY': False,
                                                                        'SQL_TYPE': 'VARCHAR',
                                                                        'WIDTH': 80},
                                          'PDBX_MODIFIED_DATE': {'NULLABLE': True,
-                                                                'ORDER': 36,
+                                                                'ORDER': 37,
                                                                 'PRECISION': 0,
                                                                 'PRIMARY_KEY': False,
                                                                 'SQL_TYPE': 'DATETIME',
                                                                 'WIDTH': 15},
+                                         'PDBX_PCM': {'NULLABLE': True,
+                                                      'ORDER': 31,
+                                                      'PRECISION': 0,
+                                                      'PRIMARY_KEY': False,
+                                                      'SQL_TYPE': 'VARCHAR',
+                                                      'WIDTH': 10},
                                          'PDBX_PROCESSING_SITE': {'NULLABLE': True,
-                                                                  'ORDER': 34,
+                                                                  'ORDER': 35,
                                                                   'PRECISION': 0,
                                                                   'PRIMARY_KEY': False,
                                                                   'SQL_TYPE': 'VARCHAR',
                                                                   'WIDTH': 10},
                                          'PDBX_RELEASE_STATUS': {'NULLABLE': True,
-                                                                 'ORDER': 33,
+                                                                 'ORDER': 34,
                                                                  'PRECISION': 0,
                                                                  'PRIMARY_KEY': False,
                                                                  'SQL_TYPE': 'VARCHAR',
                                                                  'WIDTH': 8},
                                          'PDBX_REPLACED_BY': {'NULLABLE': True,
                                                               'ORDER': 24,
                                                               'PRECISION': 0,
@@ -244,15 +252,15 @@
                                          'PDBX_REPLACES': {'NULLABLE': True,
                                                            'ORDER': 25,
                                                            'PRECISION': 0,
                                                            'PRIMARY_KEY': False,
                                                            'SQL_TYPE': 'VARCHAR',
                                                            'WIDTH': 80},
                                          'PDBX_SUBCOMPONENT_LIST': {'NULLABLE': True,
-                                                                    'ORDER': 32,
+                                                                    'ORDER': 33,
                                                                     'PRECISION': 0,
                                                                     'PRIMARY_KEY': False,
                                                                     'SQL_TYPE': 'VARCHAR',
                                                                     'WIDTH': 80},
                                          'PDBX_SYNONYMS': {'NULLABLE': True,
                                                            'ORDER': 19,
                                                            'PRECISION': 0,
@@ -315,14 +323,15 @@
                                                                            None),
                                         'PDBX_MODEL_COORDINATES_MISSING_FLAG': ('chem_comp',
                                                                                 'pdbx_model_coordinates_missing_flag',
                                                                                 None,
                                                                                 None),
                                         'PDBX_MODIFICATION_DETAILS': ('chem_comp', 'pdbx_modification_details', None, None),
                                         'PDBX_MODIFIED_DATE': ('chem_comp', 'pdbx_modified_date', None, None),
+                                        'PDBX_PCM': ('chem_comp', 'pdbx_pcm', None, None),
                                         'PDBX_PROCESSING_SITE': ('chem_comp', 'pdbx_processing_site', None, None),
                                         'PDBX_RELEASE_STATUS': ('chem_comp', 'pdbx_release_status', None, None),
                                         'PDBX_REPLACED_BY': ('chem_comp', 'pdbx_replaced_by', None, None),
                                         'PDBX_REPLACES': ('chem_comp', 'pdbx_replaces', None, None),
                                         'PDBX_SUBCOMPONENT_LIST': ('chem_comp', 'pdbx_subcomponent_list', None, None),
                                         'PDBX_SYNONYMS': ('chem_comp', 'pdbx_synonyms', None, None),
                                         'PDBX_TYPE': ('chem_comp', 'pdbx_type', None, None),
@@ -435,18 +444,21 @@
                                           'MODEL_CARTN_Z': 'model_Cartn_z',
                                           'MODEL_CARTN_Z_ESD': 'model_Cartn_z_esd',
                                           'PARTIAL_CHARGE': 'partial_charge',
                                           'PDBX_ALIGN': 'pdbx_align',
                                           'PDBX_ALT_ATOM_ID': 'pdbx_alt_atom_id',
                                           'PDBX_ALT_COMP_ID': 'pdbx_alt_comp_id',
                                           'PDBX_AROMATIC_FLAG': 'pdbx_aromatic_flag',
+                                          'PDBX_BACKBONE_ATOM_FLAG': 'pdbx_backbone_atom_flag',
+                                          'PDBX_C_TERMINAL_ATOM_FLAG': 'pdbx_c_terminal_atom_flag',
                                           'PDBX_LEAVING_ATOM_FLAG': 'pdbx_leaving_atom_flag',
                                           'PDBX_MODEL_CARTN_X_IDEAL': 'pdbx_model_Cartn_x_ideal',
                                           'PDBX_MODEL_CARTN_Y_IDEAL': 'pdbx_model_Cartn_y_ideal',
                                           'PDBX_MODEL_CARTN_Z_IDEAL': 'pdbx_model_Cartn_z_ideal',
+                                          'PDBX_N_TERMINAL_ATOM_FLAG': 'pdbx_n_terminal_atom_flag',
                                           'PDBX_ORDINAL': 'pdbx_ordinal',
                                           'PDBX_STEREO_CONFIG': 'pdbx_stereo_config',
                                           'PDBX_STND_ATOM_ID': 'pdbx_stnd_atom_id',
                                           'SUBSTRUCT_CODE': 'substruct_code',
                                           'TYPE_SYMBOL': 'type_symbol'},
                            'ATTRIBUTE_INFO': {'ALT_ATOM_ID': {'NULLABLE': True,
                                                               'ORDER': 3,
@@ -540,14 +552,26 @@
                                                                    'WIDTH': 10},
                                               'PDBX_AROMATIC_FLAG': {'NULLABLE': True,
                                                                      'ORDER': 23,
                                                                      'PRECISION': 0,
                                                                      'PRIMARY_KEY': False,
                                                                      'SQL_TYPE': 'VARCHAR',
                                                                      'WIDTH': 10},
+                                              'PDBX_BACKBONE_ATOM_FLAG': {'NULLABLE': True,
+                                                                          'ORDER': 26,
+                                                                          'PRECISION': 0,
+                                                                          'PRIMARY_KEY': False,
+                                                                          'SQL_TYPE': 'VARCHAR',
+                                                                          'WIDTH': 10},
+                                              'PDBX_C_TERMINAL_ATOM_FLAG': {'NULLABLE': True,
+                                                                            'ORDER': 28,
+                                                                            'PRECISION': 0,
+                                                                            'PRIMARY_KEY': False,
+                                                                            'SQL_TYPE': 'VARCHAR',
+                                                                            'WIDTH': 10},
                                               'PDBX_LEAVING_ATOM_FLAG': {'NULLABLE': True,
                                                                          'ORDER': 24,
                                                                          'PRECISION': 0,
                                                                          'PRIMARY_KEY': False,
                                                                          'SQL_TYPE': 'VARCHAR',
                                                                          'WIDTH': 10},
                                               'PDBX_MODEL_CARTN_X_IDEAL': {'NULLABLE': True,
@@ -564,14 +588,20 @@
                                                                            'WIDTH': 10},
                                               'PDBX_MODEL_CARTN_Z_IDEAL': {'NULLABLE': True,
                                                                            'ORDER': 21,
                                                                            'PRECISION': 6,
                                                                            'PRIMARY_KEY': False,
                                                                            'SQL_TYPE': 'FLOAT',
                                                                            'WIDTH': 10},
+                                              'PDBX_N_TERMINAL_ATOM_FLAG': {'NULLABLE': True,
+                                                                            'ORDER': 27,
+                                                                            'PRECISION': 0,
+                                                                            'PRIMARY_KEY': False,
+                                                                            'SQL_TYPE': 'VARCHAR',
+                                                                            'WIDTH': 10},
                                               'PDBX_ORDINAL': {'NULLABLE': True,
                                                                'ORDER': 16,
                                                                'PRECISION': 0,
                                                                'PRIMARY_KEY': False,
                                                                'SQL_TYPE': 'INT',
                                                                'WIDTH': 10},
                                               'PDBX_STEREO_CONFIG': {'NULLABLE': True,
@@ -610,14 +640,22 @@
                                              'MODEL_CARTN_Z': ('chem_comp_atom', 'model_Cartn_z', None, None),
                                              'MODEL_CARTN_Z_ESD': ('chem_comp_atom', 'model_Cartn_z_esd', None, None),
                                              'PARTIAL_CHARGE': ('chem_comp_atom', 'partial_charge', None, None),
                                              'PDBX_ALIGN': ('chem_comp_atom', 'pdbx_align', None, None),
                                              'PDBX_ALT_ATOM_ID': ('chem_comp_atom', 'pdbx_alt_atom_id', None, None),
                                              'PDBX_ALT_COMP_ID': ('chem_comp_atom', 'pdbx_alt_comp_id', None, None),
                                              'PDBX_AROMATIC_FLAG': ('chem_comp_atom', 'pdbx_aromatic_flag', None, None),
+                                             'PDBX_BACKBONE_ATOM_FLAG': ('chem_comp_atom',
+                                                                         'pdbx_backbone_atom_flag',
+                                                                         None,
+                                                                         None),
+                                             'PDBX_C_TERMINAL_ATOM_FLAG': ('chem_comp_atom',
+                                                                           'pdbx_c_terminal_atom_flag',
+                                                                           None,
+                                                                           None),
                                              'PDBX_LEAVING_ATOM_FLAG': ('chem_comp_atom',
                                                                         'pdbx_leaving_atom_flag',
                                                                         None,
                                                                         None),
                                              'PDBX_MODEL_CARTN_X_IDEAL': ('chem_comp_atom',
                                                                           'pdbx_model_Cartn_x_ideal',
                                                                           None,
@@ -626,14 +664,18 @@
                                                                           'pdbx_model_Cartn_y_ideal',
                                                                           None,
                                                                           None),
                                              'PDBX_MODEL_CARTN_Z_IDEAL': ('chem_comp_atom',
                                                                           'pdbx_model_Cartn_z_ideal',
                                                                           None,
                                                                           None),
+                                             'PDBX_N_TERMINAL_ATOM_FLAG': ('chem_comp_atom',
+                                                                           'pdbx_n_terminal_atom_flag',
+                                                                           None,
+                                                                           None),
                                              'PDBX_ORDINAL': ('chem_comp_atom', 'pdbx_ordinal', None, None),
                                              'PDBX_STEREO_CONFIG': ('chem_comp_atom', 'pdbx_stereo_config', None, None),
                                              'PDBX_STND_ATOM_ID': ('chem_comp_atom', 'pdbx_stnd_atom_id', None, None),
                                              'SUBSTRUCT_CODE': ('chem_comp_atom', 'substruct_code', None, None),
                                              'TYPE_SYMBOL': ('chem_comp_atom', 'type_symbol', None, None)},
                            'INDICES': {'p1': {'ATTRIBUTES': ('COMPONENT_ID', 'COMP_ID', 'ATOM_ID'), 'TYPE': 'UNIQUE'},
                                        's1': {'ATTRIBUTES': ('COMPONENT_ID',), 'TYPE': 'SEARCH'}},
@@ -1644,14 +1686,146 @@
                                               's1': {'ATTRIBUTES': ('COMPONENT_ID',), 'TYPE': 'SEARCH'}},
                                   'MAP_MERGE_INDICES': {'pdbx_chem_comp_import': {'ATTRIBUTES': ('comp_id',),
                                                                                   'TYPE': 'EQUI-JOIN'}},
                                   'TABLE_DELETE_ATTRIBUTE': 'COMPONENT_ID',
                                   'TABLE_ID': 'PDBX_CHEM_COMP_IMPORT',
                                   'TABLE_NAME': 'pdbx_chem_comp_import',
                                   'TABLE_TYPE': 'transactional'},
+        'PDBX_CHEM_COMP_PCM': {'ATTRIBUTES': {'CATEGORY': 'category',
+                                              'COMPONENT_ID': 'Component_ID',
+                                              'COMP_ID': 'comp_id',
+                                              'COMP_ID_LINKING_ATOM': 'comp_id_linking_atom',
+                                              'FIRST_INSTANCE_MODEL_DB_CODE': 'first_instance_model_db_code',
+                                              'MODIFIED_RESIDUE_ID': 'modified_residue_id',
+                                              'MODIFIED_RESIDUE_ID_LINKING_ATOM': 'modified_residue_id_linking_atom',
+                                              'PCM_ID': 'pcm_id',
+                                              'POLYPEPTIDE_POSITION': 'polypeptide_position',
+                                              'POSITION': 'position',
+                                              'TYPE': 'type',
+                                              'UNIPROT_GENERIC_PTM_ACCESSION': 'uniprot_generic_ptm_accession',
+                                              'UNIPROT_SPECIFIC_PTM_ACCESSION': 'uniprot_specific_ptm_accession'},
+                               'ATTRIBUTE_INFO': {'CATEGORY': {'NULLABLE': True,
+                                                               'ORDER': 6,
+                                                               'PRECISION': 0,
+                                                               'PRIMARY_KEY': False,
+                                                               'SQL_TYPE': 'VARCHAR',
+                                                               'WIDTH': 80},
+                                                  'COMPONENT_ID': {'NULLABLE': False,
+                                                                   'ORDER': 1,
+                                                                   'PRECISION': 0,
+                                                                   'PRIMARY_KEY': True,
+                                                                   'SQL_TYPE': 'VARCHAR',
+                                                                   'WIDTH': 10},
+                                                  'COMP_ID': {'NULLABLE': True,
+                                                              'ORDER': 3,
+                                                              'PRECISION': 0,
+                                                              'PRIMARY_KEY': False,
+                                                              'SQL_TYPE': 'VARCHAR',
+                                                              'WIDTH': 10},
+                                                  'COMP_ID_LINKING_ATOM': {'NULLABLE': True,
+                                                                           'ORDER': 9,
+                                                                           'PRECISION': 0,
+                                                                           'PRIMARY_KEY': False,
+                                                                           'SQL_TYPE': 'VARCHAR',
+                                                                           'WIDTH': 6},
+                                                  'FIRST_INSTANCE_MODEL_DB_CODE': {'NULLABLE': True,
+                                                                                   'ORDER': 13,
+                                                                                   'PRECISION': 0,
+                                                                                   'PRIMARY_KEY': False,
+                                                                                   'SQL_TYPE': 'VARCHAR',
+                                                                                   'WIDTH': 20},
+                                                  'MODIFIED_RESIDUE_ID': {'NULLABLE': True,
+                                                                          'ORDER': 4,
+                                                                          'PRECISION': 0,
+                                                                          'PRIMARY_KEY': False,
+                                                                          'SQL_TYPE': 'VARCHAR',
+                                                                          'WIDTH': 10},
+                                                  'MODIFIED_RESIDUE_ID_LINKING_ATOM': {'NULLABLE': True,
+                                                                                       'ORDER': 10,
+                                                                                       'PRECISION': 0,
+                                                                                       'PRIMARY_KEY': False,
+                                                                                       'SQL_TYPE': 'VARCHAR',
+                                                                                       'WIDTH': 6},
+                                                  'PCM_ID': {'NULLABLE': False,
+                                                             'ORDER': 2,
+                                                             'PRECISION': 0,
+                                                             'PRIMARY_KEY': True,
+                                                             'SQL_TYPE': 'INT',
+                                                             'WIDTH': 10},
+                                                  'POLYPEPTIDE_POSITION': {'NULLABLE': True,
+                                                                           'ORDER': 8,
+                                                                           'PRECISION': 0,
+                                                                           'PRIMARY_KEY': False,
+                                                                           'SQL_TYPE': 'VARCHAR',
+                                                                           'WIDTH': 80},
+                                                  'POSITION': {'NULLABLE': True,
+                                                               'ORDER': 7,
+                                                               'PRECISION': 0,
+                                                               'PRIMARY_KEY': False,
+                                                               'SQL_TYPE': 'VARCHAR',
+                                                               'WIDTH': 80},
+                                                  'TYPE': {'NULLABLE': True,
+                                                           'ORDER': 5,
+                                                           'PRECISION': 0,
+                                                           'PRIMARY_KEY': False,
+                                                           'SQL_TYPE': 'VARCHAR',
+                                                           'WIDTH': 80},
+                                                  'UNIPROT_GENERIC_PTM_ACCESSION': {'NULLABLE': True,
+                                                                                    'ORDER': 12,
+                                                                                    'PRECISION': 0,
+                                                                                    'PRIMARY_KEY': False,
+                                                                                    'SQL_TYPE': 'VARCHAR',
+                                                                                    'WIDTH': 20},
+                                                  'UNIPROT_SPECIFIC_PTM_ACCESSION': {'NULLABLE': True,
+                                                                                     'ORDER': 11,
+                                                                                     'PRECISION': 0,
+                                                                                     'PRIMARY_KEY': False,
+                                                                                     'SQL_TYPE': 'VARCHAR',
+                                                                                     'WIDTH': 20}},
+                               'ATTRIBUTE_MAP': {'CATEGORY': ('pdbx_chem_comp_pcm', 'category', None, None),
+                                                 'COMPONENT_ID': (None, None, 'datablockid()', None),
+                                                 'COMP_ID': ('pdbx_chem_comp_pcm', 'comp_id', None, None),
+                                                 'COMP_ID_LINKING_ATOM': ('pdbx_chem_comp_pcm',
+                                                                          'comp_id_linking_atom',
+                                                                          None,
+                                                                          None),
+                                                 'FIRST_INSTANCE_MODEL_DB_CODE': ('pdbx_chem_comp_pcm',
+                                                                                  'first_instance_model_db_code',
+                                                                                  None,
+                                                                                  None),
+                                                 'MODIFIED_RESIDUE_ID': ('pdbx_chem_comp_pcm',
+                                                                         'modified_residue_id',
+                                                                         None,
+                                                                         None),
+                                                 'MODIFIED_RESIDUE_ID_LINKING_ATOM': ('pdbx_chem_comp_pcm',
+                                                                                      'modified_residue_id_linking_atom',
+                                                                                      None,
+                                                                                      None),
+                                                 'PCM_ID': ('pdbx_chem_comp_pcm', 'pcm_id', None, None),
+                                                 'POLYPEPTIDE_POSITION': ('pdbx_chem_comp_pcm',
+                                                                          'polypeptide_position',
+                                                                          None,
+                                                                          None),
+                                                 'POSITION': ('pdbx_chem_comp_pcm', 'position', None, None),
+                                                 'TYPE': ('pdbx_chem_comp_pcm', 'type', None, None),
+                                                 'UNIPROT_GENERIC_PTM_ACCESSION': ('pdbx_chem_comp_pcm',
+                                                                                   'uniprot_generic_ptm_accession',
+                                                                                   None,
+                                                                                   None),
+                                                 'UNIPROT_SPECIFIC_PTM_ACCESSION': ('pdbx_chem_comp_pcm',
+                                                                                    'uniprot_specific_ptm_accession',
+                                                                                    None,
+                                                                                    None)},
+                               'INDICES': {'p1': {'ATTRIBUTES': ('COMPONENT_ID', 'PCM_ID'), 'TYPE': 'UNIQUE'},
+                                           's1': {'ATTRIBUTES': ('COMPONENT_ID',), 'TYPE': 'SEARCH'}},
+                               'MAP_MERGE_INDICES': {'pdbx_chem_comp_pcm': {'ATTRIBUTES': ('pcm_id',), 'TYPE': 'EQUI-JOIN'}},
+                               'TABLE_DELETE_ATTRIBUTE': 'COMPONENT_ID',
+                               'TABLE_ID': 'PDBX_CHEM_COMP_PCM',
+                               'TABLE_NAME': 'pdbx_chem_comp_pcm',
+                               'TABLE_TYPE': 'transactional'},
         'PDBX_CHEM_COMP_RELATED': {'ATTRIBUTES': {'COMPONENT_ID': 'Component_ID',
                                                   'COMP_ID': 'comp_id',
                                                   'DETAILS': 'details',
                                                   'RELATED_COMP_ID': 'related_comp_id',
                                                   'RELATIONSHIP_TYPE': 'relationship_type'},
                                    'ATTRIBUTE_INFO': {'COMPONENT_ID': {'NULLABLE': False,
                                                                        'ORDER': 1,
@@ -1759,44 +1933,40 @@
                                     'INDICES': {'p1': {'ATTRIBUTES': ('COMPONENT_ID', 'ORDINAL', 'COMP_ID'), 'TYPE': 'UNIQUE'},
                                                 's1': {'ATTRIBUTES': ('COMPONENT_ID',), 'TYPE': 'SEARCH'}},
                                     'MAP_MERGE_INDICES': {'pdbx_chem_comp_synonyms': {'ATTRIBUTES': ('ordinal', 'comp_id'),
                                                                                       'TYPE': 'EQUI-JOIN'}},
                                     'TABLE_DELETE_ATTRIBUTE': 'COMPONENT_ID',
                                     'TABLE_ID': 'PDBX_CHEM_COMP_SYNONYMS',
                                     'TABLE_NAME': 'pdbx_chem_comp_synonyms',
-                                    'TABLE_TYPE': 'transactional'}
-    }
-
-
+                                    'TABLE_TYPE': 'transactional'}}
+    
 
     def __init__(self,verbose=True,log=sys.stderr):
-        super(PrdChemCompSchemaDef,self).__init__(databaseName=PrdChemCompSchemaDef._databaseName,schemaDefDict=PrdChemCompSchemaDef._schemaDefDict,
-                                                  verbose=verbose,log=log)
-        
+        super(ChemCompSchemaDef,self).__init__(databaseName=ChemCompSchemaDef._databaseName,schemaDefDict=ChemCompSchemaDef._schemaDefDict,
+                                               verbose=verbose,log=log)
+
 
 if __name__ == "__main__":
-    bsd = PrdChemCompSchemaDef()
-    tableIdList = bsd.getTableIdList()
+    sd=ChemCompSchemaDef()
+    tableIdList=sd.getTableIdList()
 
     for tableId in tableIdList:
-        aIdL=bsd.getAttributeIdList(tableId)
-        tObj=bsd.getTable(tableId)
+        aIdL=sd.getAttributeIdList(tableId)
+        tObj=sd.getTable(tableId)
         attributeIdList=tObj.getAttributeIdList()
-        attributeNameList=tObj.getAttributeNameList()        
+        attributeNameList=tObj.getAttributeNameList()
         sys.stdout.write("Ordered attribute Id   list %s\n" % (str(attributeIdList)))
-        sys.stdout.write("Ordered attribute name list %s\n" % (str(attributeNameList)))        
+        sys.stdout.write("Ordered attribute name list %s\n" % (str(attributeNameList)))
         #
         mAL=tObj.getMapAttributeNameList()
         sys.stdout.write("Ordered mapped attribute name list %s\n" % (str(mAL)))
 
         mAL=tObj.getMapAttributeIdList()
-        sys.stdout.write("Ordered mapped attribute id   list %s\n" % (str(mAL)))        
+        sys.stdout.write("Ordered mapped attribute id   list %s\n" % (str(mAL)))
 
         cL=tObj.getMapInstanceCategoryList()
         sys.stdout.write("Mapped category list %s\n" % (str(cL)))
         for c in cL:
             aL=tObj.getMapInstanceAttributeList(c)
             sys.stdout.write("Mapped attribute list in %s :  %s\n" % (c,str(aL)))
-            
 
 
-
```

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/SchemaDefBase.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/SchemaDefLoader.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/SqlLoader.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/SqlLoader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistory.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistoryExec.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistorySchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistorySchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/StatusHistoryUtils.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusHistoryUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/StatusLoadWrapper.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/StatusLoadWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb/utils/db/WorkflowSchemaDef.py` & `wwpdb.utils.db-0.31/wwpdb/utils/db/WorkflowSchemaDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.db-0.30/wwpdb.utils.db.egg-info/SOURCES.txt` & `wwpdb.utils.db-0.31/wwpdb.utils.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

