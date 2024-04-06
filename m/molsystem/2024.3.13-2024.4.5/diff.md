# Comparing `tmp/molsystem-2024.3.13.tar.gz` & `tmp/molsystem-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molsystem-2024.3.13.tar", last modified: Wed Mar 13 19:24:05 2024, max compression
+gzip compressed data, was "molsystem-2024.4.5.tar", last modified: Sat Apr  6 01:37:10 2024, max compression
```

## Comparing `molsystem-2024.3.13.tar` & `molsystem-2024.4.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.791486 molsystem-2024.3.13/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-13 19:23:51.000000 molsystem-2024.3.13/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-03-13 19:23:51.000000 molsystem-2024.3.13/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-13 19:23:51.000000 molsystem-2024.3.13/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-13 19:23:51.000000 molsystem-2024.3.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-13 19:23:51.000000 molsystem-2024.3.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-03-13 19:24:05.791486 molsystem-2024.3.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-13 19:23:51.000000 molsystem-2024.3.13/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.771485 molsystem-2024.3.13/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.775485 molsystem-2024.3.13/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.775485 molsystem-2024.3.13/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.775485 molsystem-2024.3.13/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.775485 molsystem-2024.3.13/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.775485 molsystem-2024.3.13/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-13 19:23:51.000000 molsystem-2024.3.13/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.791486 molsystem-2024.3.13/molsystem/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-13 19:24:05.791486 molsystem-2024.3.13/molsystem/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    63857 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    38909 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/cif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/cms_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/configuration_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.783486 molsystem-2024.3.13/molsystem/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/data/standard_properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/frozencolumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/molfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/openbabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/pubchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/rdkit_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    42049 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    36183 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/system_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/system_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-03-13 19:23:51.000000 molsystem-2024.3.13/molsystem/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.791486 molsystem-2024.3.13/molsystem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-03-13 19:24:05.000000 molsystem-2024.3.13/molsystem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-13 19:24:05.000000 molsystem-2024.3.13/molsystem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:24:05.000000 molsystem-2024.3.13/molsystem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-13 19:24:05.000000 molsystem-2024.3.13/molsystem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-13 19:24:05.000000 molsystem-2024.3.13/molsystem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-13 19:24:05.791486 molsystem-2024.3.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-13 19:23:51.000000 molsystem-2024.3.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.787485 molsystem-2024.3.13/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:24:05.787485 molsystem-2024.3.13/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   269083 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/1n9v.cif
--rw-r--r--   0 runner    (1001) docker     (127)  1055288 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/aa-variants-v1.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/acy.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)   117392 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/aminoacids.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/benzene.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/hoh.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/polyethylene.cif
--rw-r--r--   0 runner    (1001) docker     (127)    71597 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/spacegroup_names.json
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/data/trigonal.cif
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_angiotensin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_cif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_configuration_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_molfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_openbabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_property_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_pubchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_rdkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_system_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-13 19:23:51.000000 molsystem-2024.3.13/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-03-13 19:23:51.000000 molsystem-2024.3.13/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-06 01:36:58.000000 molsystem-2024.4.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-06 01:36:58.000000 molsystem-2024.4.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-06 01:36:58.000000 molsystem-2024.4.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 01:36:58.000000 molsystem-2024.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-06 01:36:58.000000 molsystem-2024.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-06 01:37:10.694393 molsystem-2024.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-06 01:36:58.000000 molsystem-2024.4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.678393 molsystem-2024.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.678393 molsystem-2024.4.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.678393 molsystem-2024.4.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.682393 molsystem-2024.4.5/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.682393 molsystem-2024.4.5/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.682393 molsystem-2024.4.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-06 01:36:58.000000 molsystem-2024.4.5/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/molsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 01:37:10.694393 molsystem-2024.4.5/molsystem/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69805 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38956 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/cms_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/configuration_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.686393 molsystem-2024.4.5/molsystem/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/data/standard_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/frozencolumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/molfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/rdkit_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47649 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36917 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/system_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/system_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-04-06 01:36:58.000000 molsystem-2024.4.5/molsystem/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/molsystem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 01:37:10.000000 molsystem-2024.4.5/molsystem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-06 01:37:10.694393 molsystem-2024.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-06 01:36:58.000000 molsystem-2024.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.690393 molsystem-2024.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:37:10.694393 molsystem-2024.4.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   269083 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/1n9v.cif
+-rw-r--r--   0 runner    (1001) docker     (127)  1055288 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/aa-variants-v1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/acy.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)   117392 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/aminoacids.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/benzene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/hoh.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/polyethylene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    71597 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/spacegroup_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/data/trigonal.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_angiotensin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_configuration_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_molfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_property_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_system_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-06 01:36:58.000000 molsystem-2024.4.5/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-04-06 01:36:58.000000 molsystem-2024.4.5/versioneer.py
```

### Comparing `molsystem-2024.3.13/CONTRIBUTING.rst` & `molsystem-2024.4.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/HISTORY.rst` & `molsystem-2024.4.5/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2023.4.6 -- Added gradients
+    * Added gradient on atoms as a separate table alongside atoms, so they take no space
+      unless actually used.
+      
 2024.3.13 -- Handle uppercase X, Y, Z in strings for symmetry operators
     * the Crystallographic Open Database CIF files seems to use upper case X, Y, Z in
       explicit symmetry operators. These need to be lowercased in the code.
 
 2023.12.5 -- Bugfixes for symmetry
     * Fixed issue #72, where symmetry was not correctly handled for trigonal and
       hexagonal cells where atoms had coordinates of 1/3 or 2/3.
```

### Comparing `molsystem-2024.3.13/LICENSE` & `molsystem-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/PKG-INFO` & `molsystem-2024.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2024.3.13
+Version: 2024.4.5
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -113,14 +113,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.4.6 -- Added gradients
+    * Added gradient on atoms as a separate table alongside atoms, so they take no space
+      unless actually used.
+      
 2024.3.13 -- Handle uppercase X, Y, Z in strings for symmetry operators
     * the Crystallographic Open Database CIF files seems to use upper case X, Y, Z in
       explicit symmetry operators. These need to be lowercased in the code.
 
 2023.12.5 -- Bugfixes for symmetry
     * Fixed issue #72, where symmetry was not correctly handled for trigonal and
       hexagonal cells where atoms had coordinates of 1/3 or 2/3.
```

### Comparing `molsystem-2024.3.13/README.rst` & `molsystem-2024.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/Makefile` & `molsystem-2024.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/_static/SEAMM inverted.png` & `molsystem-2024.4.5/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/_static/SEAMM logo.png` & `molsystem-2024.4.5/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/_static/molssi_main_logo.png` & `molsystem-2024.4.5/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/_static/molssi_main_logo_inverted_white.png` & `molsystem-2024.4.5/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/_static/molssi_square.png` & `molsystem-2024.4.5/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/_static/nsf.png` & `molsystem-2024.4.5/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/conf.py` & `molsystem-2024.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/developer_guide/installation.rst` & `molsystem-2024.4.5/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/getting_started/index.rst` & `molsystem-2024.4.5/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/index.rst` & `molsystem-2024.4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/make.bat` & `molsystem-2024.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/docs/user_guide/index.rst` & `molsystem-2024.4.5/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/__init__.py` & `molsystem-2024.4.5/molsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/align.py` & `molsystem-2024.4.5/molsystem/align.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/atoms.py` & `molsystem-2024.4.5/molsystem/atoms.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         self._system = None
 
         self._atomset = self._configuration.atomset
 
         self._atom_table = _Table(self.system_db, "atom")
         self._coordinates_table = _Table(self.system_db, "coordinates")
         self._velocities_table = _Table(self.system_db, "velocities")
+        self._gradients_table = _Table(self.system_db, "gradients")
 
         super().__init__(self._system_db, "atom")
 
     def __enter__(self) -> Any:
         """Copy the tables to a backup for a 'with' statement."""
         self.system_db["atomset_atom"].__enter__()
         self.system_db["atom"].__enter__()
@@ -66,14 +67,16 @@
         """Allow deletion of keys"""
         if key in self._atom_table.attributes:
             del self._atom_table[key]
         elif key in self._coordinates_table.attributes:
             del self._coordinates_table[key]
         elif key in self._velocities_table.attributes:
             del self._velocities_table[key]
+        elif key in self._gradients_table.attributes:
+            del self._gradients_table[key]
 
     def __iter__(self) -> iter:
         """Allow iteration over the object"""
         return iter([*self.attributes.keys()])
 
     def __len__(self) -> int:
         """The len() command"""
@@ -180,28 +183,32 @@
     def atom_generators(self):
         """The symmetry operations that create the symmetric atoms."""
         return self.configuration.symmetry.atom_generators
 
     @property
     def attributes(self) -> Dict[str, Any]:
         """The definitions of the attributes.
-        Combine the attributes of the atom, coordinates, and velocities tables to
-        make it look like a single larger table.
+        Combine the attributes of the atom, coordinates, velocities, and gradients
+        tables to make it look like a single larger table.
         """
 
         result = self._atom_table.attributes
 
         for key, value in self._coordinates_table.attributes.items():
             if key != "atom":  # atom key links the tables together, so ignore
                 result[key] = value
 
         for key, value in self._velocities_table.attributes.items():
             if key != "atom":  # atom key links the tables together, so ignore
                 result[key] = value
 
+        for key, value in self._gradients_table.attributes.items():
+            if key != "atom":  # atom key links the tables together, so ignore
+                result[key] = value
+
         return result
 
     @property
     def configuration(self):
         """Return the configuration."""
         return self._configuration
 
@@ -222,23 +229,46 @@
 
     @property
     def db(self):
         """The database connection."""
         return self.system_db.db
 
     @property
+    def gradients(self):
+        """The gradients as list of lists."""
+        return self.get_gradients()
+
+    @gradients.setter
+    def gradients(self, xyz):
+        """The gradients as list of lists."""
+        return self.set_gradients(xyz)
+
+    @property
     def group(self):
         """The space or point group of the configuration."""
         return self.configuration.symmetry.group
 
     @group.setter
     def group(self, value):
         self.configuration.symmetry.group = value
 
     @property
+    def have_gradients(self):
+        """Whether there are any gradients for this configuration."""
+        sql = (
+            "SELECT COUNT(*)"
+            " FROM atomset_atom AS aa, gradients AS ve "
+            "WHERE aa.atomset = ?"
+            "  AND ve.atom = aa.atom AND ve.configuration = ?"
+        )
+        parameters = [self.atomset, self.configuration.id]
+        self.cursor.execute(sql, parameters)
+        return self.cursor.fetchone()[0] > 0
+
+    @property
     def have_velocities(self):
         """Whether there are any velocities for this configuration."""
         sql = (
             "SELECT COUNT(*)"
             " FROM atomset_atom AS aa, velocities AS ve "
             "WHERE aa.atomset = ?"
             "  AND ve.atom = aa.atom AND ve.configuration = ?"
@@ -472,14 +502,24 @@
         for column in self._velocities_table.attributes:
             if column != "id" and column in kwargs:
                 data[column] = kwargs.pop(column)
                 have_velocities = True
         if have_velocities:
             self._velocities_table.append(n=n_rows, **data)
 
+        # And gradients table
+        data = {"configuration": configuration, "atom": ids}
+        have_gradients = False
+        for column in self._gradients_table.attributes:
+            if column != "id" and column in kwargs:
+                data[column] = kwargs.pop(column)
+                have_gradients = True
+        if have_gradients:
+            self._gradients_table.append(n=n_rows, **data)
+
         # And to the atomset
         table = _Table(self.system_db, "atomset_atom")
         table.append(atomset=self.atomset, atom=ids)
 
         self.configuration.symmetry.reset_atoms()
 
         return ids
@@ -493,124 +533,115 @@
             Added selection criteria for the SQL, one word at a time.
 
         Returns
         -------
         sqlite3.Cursor
             A cursor that returns sqlite3.Row objects for the atoms.
         """
-        if self.have_velocities:
-            columns = self._columns(velocities=True)
-            column_defs = ", ".join(columns)
-
-            # What tables are requested in the extra arguments?
-            tables = set()
-            if len(args) > 0:
-                atom_columns = [*self._atom_table.attributes]
-                coordinates_columns = [*self._coordinates_table.attributes]
-                velocities_columns = [*self._velocities_table.attributes]
-                for col, op, value in grouped(args, 3):
-                    if "." in col:
-                        tables.add(col.split(".")[0])
-                    elif col in atom_columns:
-                        tables.add("at")
-                    elif col in coordinates_columns:
-                        tables.add("co")
-                    elif col in velocities_columns:
+        have_velocities = self.have_velocities
+        have_gradients = self.have_gradients
+        columns = self._columns(velocities=have_velocities, gradients=have_gradients)
+        column_defs = ", ".join(columns)
+
+        # What tables are requested in the extra arguments?
+        tables = set()
+        if len(args) == 0:
+            tables.add("at")
+            tables.add("co")
+            if have_velocities:
+                tables.add("ve")
+            if have_gradients:
+                tables.add("gr")
+        else:
+            atom_columns = [*self._atom_table.attributes]
+            coordinates_columns = [*self._coordinates_table.attributes]
+            velocities_columns = [*self._velocities_table.attributes]
+            gradients_columns = [*self._gradients_table.attributes]
+            for col, op, value in grouped(args, 3):
+                if "." in col:
+                    tables.add(col.split(".")[0])
+                elif col in atom_columns:
+                    tables.add("at")
+                elif col in coordinates_columns:
+                    tables.add("co")
+                elif col in velocities_columns:
+                    if have_velocities:
                         tables.add("ve")
                     else:
-                        raise ValueError(f"Column '{col}' is not available")
-
-            # Build the query based on the tables needed
-            sql = (
-                f"SELECT {column_defs}"
-                " FROM atomset_atom AS aa, atom AS at, coordinates AS co, "
-                "      velocities AS ve "
-                "WHERE aa.atomset = ?"
-                "  AND at.id = aa.atom"
-                "  AND co.atom = at.id AND co.configuration = ?"
-                "  AND ve.atom = at.id AND ve.configuration = ?"
-            )
-            parameters = [self.atomset, self.configuration.id, self.configuration.id]
-
-            # And any extra selection criteria
-            if len(args) > 0:
-                for col, op, value in grouped(args, 3):
-                    if op == "==":
-                        op = "="
-                    sql += f' AND "{col}" {op} ?'
-                    parameters.append(value)
-        else:
-            columns = self._columns(velocities=False)
-            column_defs = ", ".join(columns)
-
-            # What tables are requested in the extra arguments?
-            tables = set()
-            if len(args) > 0:
-                atom_columns = [*self._atom_table.attributes]
-                coordinates_columns = [*self._coordinates_table.attributes]
-                velocities_columns = [*self._velocities_table.attributes]
-                for col, op, value in grouped(args, 3):
-                    if "." in col:
-                        tables.add(col.split(".")[0])
-                    elif col in atom_columns:
-                        tables.add("at")
-                    elif col in coordinates_columns:
-                        tables.add("co")
-                    elif col in velocities_columns:
                         raise ValueError(
                             "Query for atom has velocities, but the atoms don't"
                         )
+                elif col in gradients_columns:
+                    if have_gradients:
+                        tables.add("gr")
                     else:
-                        raise ValueError(f"Column '{col}' is not available")
+                        raise ValueError(
+                            "Query for atom has gradients, but the atoms don't"
+                        )
+                else:
+                    raise ValueError(f"Column '{col}' is not available")
 
-            # Build the query based on the tables needed
-            sql = (
-                f"SELECT {column_defs}"
-                " FROM atomset_atom AS aa, atom AS at, coordinates AS co "
-                "WHERE aa.atomset = ?"
-                "  AND at.id = aa.atom"
-                "  AND co.atom = at.id AND co.configuration = ?"
-            )
-            parameters = [self.atomset, self.configuration.id]
+        # Build the query based on the tables needed
+        from_string = ["atomset_atom AS aa", "atom AS at", "coordinates AS co"]
+        if "ve" in tables:
+            from_string.append("velocities AS ve")
+        if "gr" in tables:
+            from_string.append("gradients AS gr")
+        from_string = ", ".join(from_string)
+
+        sql = (
+            f"SELECT {column_defs}\n"
+            f" FROM {from_string}\n"
+            "WHERE aa.atomset = ?\n"
+            "  AND at.id = aa.atom\n"
+            "  AND co.atom = at.id AND co.configuration = ?"
+        )
+        parameters = [self.atomset, self.configuration.id]
+        if "ve" in tables:
+            sql += "\n  AND ve.atom = at.id AND ve.configuration = ?"
+            parameters.append(self.configuration.id)
+        if "gr" in tables:
+            sql += "\n  AND gr.atom = at.id AND gr.configuration = ?"
+            parameters.append(self.configuration.id)
 
-            # And any extra selection criteria
-            if len(args) > 0:
-                for col, op, value in grouped(args, 3):
-                    if op == "==":
-                        op = "="
-                    sql += f' AND "{col}" {op} ?'
-                    parameters.append(value)
+        # And any extra selection criteria
+        if len(args) > 0:
+            for col, op, value in grouped(args, 3):
+                if op == "==":
+                    op = "="
+                sql += f'\n AND "{col}" {op} ?'
+                parameters.append(value)
 
         logger.debug("atoms query:")
         logger.debug(sql)
         logger.debug(parameters)
         logger.debug("---")
 
         return self.db.execute(sql, parameters)
 
     def diff(self, other):
         """Difference between these atoms and another
 
-        Currently ignores velocities. Not sure what we want to do....
+        Currently ignores velocities and gradients. Not sure what we want to do....
 
         Parameters
         ----------
         other : _Atoms
             The other atoms to diff against
 
         Result
         ------
         result : Dict
             The differences, described in a dictionary
         """
         result = {}
 
         # Check the columns
-        columns = self._columns(velocities=False)
-        other_columns = other._columns(velocities=False)
+        columns = self._columns(velocities=False, gradients=False)
+        other_columns = other._columns(velocities=False, gradients=False)
 
         column_defs = ", ".join(columns)
         other_column_defs = ", ".join(other_columns)
 
         if columns == other_columns:
             column_def = column_defs
         else:
@@ -1148,14 +1179,66 @@
         symmetry = self.configuration.symmetry
         if asymmetric or symmetry.n_symops == 1:
             return data
 
         # Expand to the asymmetric atoms
         return [data[i] for i in symmetry.atom_to_asymmetric_atom]
 
+    def get_gradients(
+        self,
+        fractionals=True,
+        as_array=False,
+    ):
+        """Return the gradients.
+
+        Symmetry is not supported, because it makes no (little?) sense for gradients.
+
+        Parameters
+        ----------
+        fractionals : bool = True
+            Return the gradients as fractional gradients for periodic
+            systems. Non-periodic systems always use Cartesian gradients.
+        as_array : bool = False
+            Whether to return the results as a np array or as a list of
+            lists (the default).
+
+        Returns
+        -------
+        abc : [N][float*3]
+            The gradients, either Cartesian or fractional
+        """
+        gxs = self.get_column_data("gx")
+        gys = self.get_column_data("gy")
+        gzs = self.get_column_data("gz")
+        xyz = [[gx, gy, gz] for gx, gy, gz in zip(gxs, gys, gzs)]
+
+        periodicity = self.configuration.periodicity
+        if periodicity == 0:
+            if as_array:
+                return np.array(xyz)
+            else:
+                return xyz
+
+        cell = self.configuration.cell
+
+        if fractionals:
+            if self.configuration.coordinate_system == "Cartesian":
+                return cell.to_fractionals(xyz, as_array=as_array)
+            elif as_array:
+                return np.array(xyz)
+            else:
+                return xyz
+        else:
+            if self.configuration.coordinate_system == "fractional":
+                return cell.to_cartesians(xyz, as_array=as_array)
+            elif as_array:
+                return np.array(xyz)
+            else:
+                return xyz
+
     def get_velocities(
         self,
         fractionals=True,
         as_array=False,
     ):
         """Return the velocities.
 
@@ -1272,14 +1355,85 @@
                     xs.append(x)
                     ys.append(y)
                     zs.append(z)
         x_column[0:] = xs
         y_column[0:] = ys
         z_column[0:] = zs
 
+    def set_gradients(self, gxyz, fractionals=False):
+        """Set the gradients to new values.
+
+        Parameters
+        ----------
+        fractionals : bool = False
+            The gradients are fractional gradients for periodic
+            systems. Ignored for non-periodic systems.
+
+        Returns
+        -------
+        None
+        """
+        if self.n_symops > 1:
+            raise RuntimeError("Can't handle gradients with symmetry.")
+
+        as_array = isinstance(gxyz, np.ndarray)
+
+        gxs = []
+        gys = []
+        gzs = []
+
+        periodicity = self.configuration.periodicity
+        coordinate_system = self.configuration.coordinate_system
+        if (
+            periodicity == 0
+            or (coordinate_system == "Cartesian" and not fractionals)
+            or (coordinate_system == "fractional" and fractionals)
+        ):
+            if as_array:
+                for gx, gy, gz in gxyz.tolist():
+                    gxs.append(gx)
+                    gys.append(gy)
+                    gzs.append(gz)
+            else:
+                for gx, gy, gz in gxyz:
+                    gxs.append(gx)
+                    gys.append(gy)
+                    gzs.append(gz)
+        else:
+            cell = self.configuration.cell
+            if coordinate_system == "fractional":
+                # Convert gradients to fractionals
+                for gx, gy, gz in cell.to_fractionals(gxyz):
+                    gxs.append(gx)
+                    gys.append(gy)
+                    gzs.append(gz)
+            else:
+                for gx, gy, gz in cell.to_cartesians(gxyz):
+                    gxs.append(gx)
+                    gys.append(gy)
+                    gzs.append(gz)
+
+        gx_column = self.get_column("gx")
+        if len(gx_column) == 0:
+            # No gradients in the database, so need to add rather than setFormatter
+            self._gradients_table.append(
+                n=len(gxs),
+                gx=gxs,
+                gy=gys,
+                gz=gzs,
+                atom=self.ids,
+                configuration=self.configuration.id,
+            )
+        else:
+            gy_column = self.get_column("gy")
+            gz_column = self.get_column("gz")
+            gx_column[0:] = gxs
+            gy_column[0:] = gys
+            gz_column[0:] = gzs
+
     def set_velocities(self, vxyz, fractionals=False):
         """Set the velocities to new values.
 
         Parameters
         ----------
         fractionals : bool = False
             The velocities are fractional velocities for periodic
@@ -1387,14 +1541,26 @@
                 "        atomset_atom as aa"
                 "  WHERE ve.atom = at.id"
                 f"   AND ve.configuration = {self.configuration.id}"
                 "    AND at.id = aa.atom"
                 f"   AND aa.atomset = {self.atomset}"
             )
             return _Column(self._velocities_table, key, sql=sql)
+        elif key in self._gradients_table.attributes:
+            sql = (
+                f'SELECT gr.rowid, gr."{key}"'
+                "   FROM atom as at,"
+                "        gradients as gr,"
+                "        atomset_atom as aa"
+                "  WHERE gr.atom = at.id"
+                f"   AND gr.configuration = {self.configuration.id}"
+                "    AND at.id = aa.atom"
+                f"   AND aa.atomset = {self.atomset}"
+            )
+            return _Column(self._gradients_table, key, sql=sql)
         else:
             raise KeyError(f"'{key}' not in atoms")
 
     def get_column_data(self, key: str) -> Any:
         """Return a column of data from the table.
 
         Parameters
@@ -1434,14 +1600,26 @@
                 "        atomset_atom as aa"
                 "  WHERE ve.atom = at.id"
                 f"   AND ve.configuration = {self.configuration.id}"
                 "    AND at.id = aa.atom"
                 f"   AND aa.atomset = {self.atomset}"
             )
             return [row[0] for row in self.db.execute(sql)]
+        elif key in self._gradients_table.attributes:
+            sql = (
+                f'SELECT gr."{key}"'
+                "   FROM atom as at,"
+                "        gradients as gr,"
+                "        atomset_atom as aa"
+                "  WHERE gr.atom = at.id"
+                f"   AND gr.configuration = {self.configuration.id}"
+                "    AND at.id = aa.atom"
+                f"   AND aa.atomset = {self.atomset}"
+            )
+            return [row[0] for row in self.db.execute(sql)]
         else:
             raise KeyError(f"'{key}' not in atoms")
 
     def _get_n_rows(self, **kwargs):
         """Get the total number of rows represented in the arguments."""
         n_rows = None
 
@@ -1497,16 +1675,16 @@
         atoms : [int]
             The list of atoms to delete, or 'all' or '*'
 
         Returns
         -------
         None
         """
-        # Delete the listed atoms, which will cascade to delete coordinates and
-        # velocities
+        # Delete the listed atoms, which will cascade to delete coordinates,
+        # velocities, and gradients
         if atoms == "all" or atoms == "*":
             sql = """
             DELETE FROM atom
              WHERE id IN (SELECT atom FROM atomset_atom WHERE atomset = ?)
             """
             parameters = (self.atomset,)
             self.db.execute(sql, parameters)
@@ -1530,28 +1708,33 @@
 
         columns = [x[0] for x in rows.description[1:]]
 
         df = pandas.DataFrame.from_dict(data, orient="index", columns=columns)
 
         return df
 
-    def _columns(self, velocities=True):
-        """The list of columns across the atom, coordinates and velocities tables.
+    def _columns(self, velocities=True, gradients=True):
+        """The list of columns across the atom, coordinates, velocities, and gradients
+        tables.
 
-        Uses 'at', 'co', and 've' as the shorthand for the full table names.
+        Uses 'at', 'co', 've', and 'gr' as the shorthand for the full table names.
         """
         atom_columns = [*self._atom_table.attributes]
         coordinates_columns = [*self._coordinates_table.attributes]
         coordinates_columns.remove("atom")
         columns = [f'at."{x}"' for x in atom_columns]
         columns += [f'co."{x}"' for x in coordinates_columns]
         if velocities:
             velocities_columns = [*self._velocities_table.attributes]
             velocities_columns.remove("atom")
             columns += [f've."{x}"' for x in velocities_columns]
+        if gradients:
+            gradients_columns = [*self._gradients_table.attributes]
+            gradients_columns.remove("atom")
+            columns += [f'gr."{x}"' for x in gradients_columns]
 
         return columns
 
 
 class _SubsetAtoms(_Atoms):
     """The atoms in a subset.
 
@@ -1721,59 +1904,51 @@
             Added selection criteria for the SQL, one word at a time.
 
         Returns
         -------
         sqlite3.Cursor
             A cursor that returns sqlite3.Row objects for the atoms.
         """
-        if self.have_velocities:
-            columns = self._columns()
-            column_defs = ", ".join(columns)
-
-            sql = f"""
-            SELECT {column_defs}
-              FROM atom as at, coordinates as co, velocities as ve, subset_atom as sa
-             WHERE co.atom = at.id
-               AND co.configuration = ?
-               AND ve.atom = at.id
-               AND ve.configuration = ?
-               AND at.id = sa.atom
-               AND sa.subset = ?
-            """
+        have_velocities = self.have_velocities
+        have_gradients = self.have_gradients
+        columns = self._columns(velocities=have_velocities, gradients=have_gradients)
+        column_defs = ", ".join(columns)
 
-            parameters = [self.configuration.id, self.configuration.id, self.subset_id]
-            if len(args) > 0:
-                for col, op, value in grouped(args, 3):
-                    if op == "==":
-                        op = "="
-                    sql += f' AND "{col}" {op} ?'
-                    parameters.append(value)
-        else:
-            columns = self._columns(velocities=False)
-            column_defs = ", ".join(columns)
-
-            sql = f"""
-            SELECT {column_defs}
-              FROM atom as at, coordinates as co, subset_atom as sa
-             WHERE co.atom = at.id
-               AND co.configuration = ?
-               AND at.id = sa.atom
-               AND sa.subset = ?
-            """
+        from_string = ["atom as at", "coordinates as co", "subset_atom as sa"]
+        if have_velocities:
+            from_string.append("velocities AS ve")
+        if have_gradients:
+            from_string.append("gradients AS gr")
+        from_string = ", ".join(from_string)
+
+        sql = f"""
+        SELECT {column_defs}
+          FROM {from_string}
+         WHERE co.atom = at.id
+           AND co.configuration = ?
+           AND at.id = sa.atom
+           AND sa.subset = ?
+        """
+        parameters = [self.configuration.id, self.subset_id]
+        if have_velocities:
+            sql += "\n  AND ve.atom = at.id AND ve.configuration = ?"
+            parameters.append(self.configuration.id)
+        if have_gradients:
+            sql += "\n  AND gr.atom = at.id AND gr.configuration = ?"
+            parameters.append(self.configuration.id)
 
-            parameters = [self.configuration.id, self.subset_id]
-            if len(args) > 0:
-                for col, op, value in grouped(args, 3):
-                    if op == "==":
-                        op = "="
-                    sql += f' AND "{col}" {op} ?'
-                    parameters.append(value)
+        if len(args) > 0:
+            for col, op, value in grouped(args, 3):
+                if op == "==":
+                    op = "="
+                sql += f'\n AND "{col}" {op} ?'
+                parameters.append(value)
 
-            if self.template.is_full and self.template_order:
-                sql += "ORDER BY sa.templateatom"
+        if self.template.is_full and self.template_order:
+            sql += "\nORDER BY sa.templateatom"
 
         return self.db.execute(sql, parameters)
 
     def get_n_atoms(self, *args):
         """Return the number of atoms meeting the criteria.
 
         Parameters
```

### Comparing `molsystem-2024.3.13/molsystem/bonds.py` & `molsystem-2024.4.5/molsystem/bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/cell.py` & `molsystem-2024.4.5/molsystem/cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/cif.py` & `molsystem-2024.4.5/molsystem/cif.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             volume = cell.volume
             spgname = symmetry.group
             if spgname == "":
                 pass
             elif symmetry.n_symops == 1:
                 lines.append("_space_group_name_H-M_full   'P 1'")
             else:
-                spgname_system = symmetry.spacegroup_names_to_system[spgname]
+                spgname_system = symmetry.spacegroup_names_to_system()[spgname]
                 lines.append(f"_space_group_{spgname_system}       '{spgname}'")
                 hall = symmetry.hall_symbol
                 lines.append(f"_symmetry_space_group_name_Hall '{hall}'")
                 it_number = symmetry.IT_number
                 lines.append(f"_space_group_IT_number          {it_number}")
             lines.append(f"_cell_length_a   {a}")
             lines.append(f"_cell_length_b   {b}")
@@ -281,25 +281,26 @@
                 self.symmetry.symops = data_block[symdata]
                 used_symops = True
             elif "_symmetry_equiv" + dot + "pos_as_xyz" in data_block:
                 symdata = "_symmetry_equiv" + dot + "pos_as_xyz"
                 self.symmetry.symops = data_block[symdata]
                 used_symops = True
             else:
+                found = False
                 for section in (
                     "_space_group" + dot + "name_Hall",
                     "_space_group" + dot + "name_H-M_full",
                     "_space_group" + dot + "name_H-M_alt",
                     "_symmetry" + dot + "space_group_name_Hall",
                     "_symmetry" + dot + "space_group_name_H-M",
                 ):
                     if section in data_block:
+                        found = True
                         self.symmetry.group = data_block[section]
-                        break
-                else:
+                if not found:
                     raise RuntimeError(
                         "CIF file does not contain required symmetry information. "
                         "Neither "
                         "'_symmetry_equiv" + dot + "pos_as_xyz' or "
                         "'_space_group_symop" + dot + "operation_xyz' or "
                         "_symmetry" + dot + "space_group_name_Hall  or "
                         "_symmetry" + dot + "space_group_name_H-M "
```

### Comparing `molsystem-2024.3.13/molsystem/cms_schema.py` & `molsystem-2024.4.5/molsystem/cms_schema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/column.py` & `molsystem-2024.4.5/molsystem/column.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/configuration.py` & `molsystem-2024.4.5/molsystem/configuration.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/configuration_properties.py` & `molsystem-2024.4.5/molsystem/configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/data/standard_properties.csv` & `molsystem-2024.4.5/molsystem/data/standard_properties.csv`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/elements.py` & `molsystem-2024.4.5/molsystem/elements.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/frozencolumn.py` & `molsystem-2024.4.5/molsystem/frozencolumn.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/inchi.py` & `molsystem-2024.4.5/molsystem/inchi.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/molfile.py` & `molsystem-2024.4.5/molsystem/molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/openbabel.py` & `molsystem-2024.4.5/molsystem/openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/pdb.py` & `molsystem-2024.4.5/molsystem/pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/properties.py` & `molsystem-2024.4.5/molsystem/properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/pubchem.py` & `molsystem-2024.4.5/molsystem/pubchem.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/qcschema.py` & `molsystem-2024.4.5/molsystem/qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/rdkit_.py` & `molsystem-2024.4.5/molsystem/rdkit_.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/smiles.py` & `molsystem-2024.4.5/molsystem/smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/subset.py` & `molsystem-2024.4.5/molsystem/subset.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/subsets.py` & `molsystem-2024.4.5/molsystem/subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/symmetry.py` & `molsystem-2024.4.5/molsystem/symmetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 
 import numpy as np
 import spglib
 
 logger = logging.getLogger(__name__)
 # logger.setLevel("INFO")
+logger.setLevel("WARNING")
 
 
 class _Symmetry(object):
     """A class to handle point and space group symmetry."""
 
     spgno_to_hall = None
     spgname_to_hall = None
@@ -43,14 +44,345 @@
         self._atom_to_asymmetric_atom = None  # The asymmetric atom for each atom
         self._bond_to_asymmetric_bond = None  # The asymmetric bond for each bond
         self._bond_atoms = None  # The pair of symmetric atoms in each bond
         self._bond_offsets = None  # The triplet of cell offsets for each bond
 
         super().__init__()
 
+    @staticmethod
+    def filter_atoms(atoms, coordinates, group=None, sym_ops=None, operators=None):
+        """Check and filter the atoms in a periodic system.
+
+        There is an issue with some CIF files, notably those from the Cambridge
+        structural database, where there are atoms in the asymmetric unit that
+        are duplicates. It appears that the CIF file is written with entire molecules
+        in some cases. So if the molecule is on a symmetry element, the atoms that are
+        related by symmetry are explicitly in the file.
+
+        To handle this we need to check for duplicates and remove them. Not a bad check
+        to have, anyway.
+
+        Parameters
+        ----------
+        atoms : str or int
+            The atomic symbols or numbers of the atoms.
+        coordinates : array_like
+            The coordinates of the atoms.
+        group : str
+            The space group symbol.
+        sym_ops : array_like
+            The symmetry operations as strings.
+        operators : array_like
+            The symmetry operators.
+        """
+        if group is not None:
+            # Get the symmetry operators
+            if sym_ops is not None or operators is not None:
+                raise RuntimeError(
+                    "Cannot specify both group and sym_ops or operators."
+                )
+            operators = _Symmetry.get_operators(group)
+        elif sym_ops is not None:
+            if operators is not None or group is not None:
+                raise RuntimeError(
+                    "Cannot specify both sym_ops and group or operators."
+                )
+            operators = _Symmetry.get_operators(sym_ops)
+        elif operators is not None:
+            if sym_ops is not None or group is not None:
+                raise RuntimeError(
+                    "Cannot specify both operators and group or sym_ops."
+                )
+        else:
+            raise RuntimeError("Must specify either group or sym_ops or operators.")
+
+        self = _Symmetry()
+
+        symbols = self.configuration.atoms.asymmetric_symbols
+        n_atoms = self.configuration.n_asymmetric_atoms
+        logger.info(f"Expanding {n_atoms} asymmetric atoms to full cell.")
+        if n_atoms == 0:
+            self._atom_generators = None
+            self._symop_to_atom = None
+        self._atom_generators = []  # Symmetry ops that create the symmetric atoms
+        self._symop_to_atom = []  # The symmetry atom resulting from symmetry ops
+        if self.configuration.periodicity == 3:
+            if len(operators) == 1:
+                # P1 is a special case. Nothing to do.
+                self._atom_generators = [[0] for i in range(n_atoms)]
+                self._symop_to_atom = [[i] for i in range(n_atoms)]
+                self._atom_to_asymmetric_atom = [*range(n_atoms)]
+            else:
+                uvw0 = self.configuration.atoms.get_coordinates(
+                    as_array=True, asymmetric=True
+                )
+                if uvw0.shape[0] != n_atoms:
+                    raise RuntimeError(
+                        f"Mismatch of number of atoms in symmetry: {uvw0.shape[0]} != "
+                        f"{n_atoms}"
+                    )
+                logger.debug(
+                    f"""
+{n_atoms=}
+{uvw0.shape=}"
+Original coordinates
+{uvw0}
+                    """
+                )
+
+                uvw = np.ndarray((n_atoms, 4))
+                uvw[:, 0:3] = uvw0[:, :]
+                logger.debug(f"\nExpanded coordinates\n{uvw}")
+                uvw[:, 3] = 1
+                # logger.debug(self.symops)
+                logger.debug(f"\n{operators.shape=}")
+                # logger.debug(operators)
+                # logger.debug(f"{uvw.shape=}")
+                # logger.debug("Expanded coordinates")
+                # logger.debug(uvw)
+                xformed = np.einsum("ijk,lk", operators, uvw)
+                logger.debug(f"\n{xformed.shape=}\n{xformed}")
+
+                # For comparison, bring all atoms into the cell [0..1)
+                tmp = xformed - np.floor(xformed)
+
+                logger.debug(f"\ntmp = Transformed and floored coordinates\n{tmp}")
+
+                # Keep track of atoms and coordinates found so can check for duplicates
+                found = {}
+
+                n_sym_atoms = 0
+                n_asymmetric_atoms = 0
+                for i in range(n_atoms):
+                    values, I1, I2 = np.unique(
+                        np.round(tmp[:, :3, i], 4),
+                        axis=0,
+                        return_index=True,
+                        return_inverse=True,
+                    )
+                    # pprint.pprint(np.round(tmp[:, :3, i], 4).tolist())
+                    logger.debug(
+                        f"""
+{i=}: {symbols[i]}
+{np.round(tmp[:, :3, i], 4)}
+nvalues
+{values}
+I1
+{I1}
+I2
+{I2}
+                        """
+                    )
+                    # Check for duplicates
+                    if tuple(values[0]) in found:
+                        if found[tuple(values[0])] != symbols[i]:
+                            raise RuntimeError(
+                                "Duplicate atoms with different symbols: "
+                                f"{symbols[i]} != {found[tuple(values[0])]} at "
+                                f"{values[0]}"
+                            )
+                        else:
+                            # Same element, so ignore
+                            logger.debug("\nDuplicate atom, ignoring")
+                            continue
+
+                    for value in values:
+                        found[tuple(value)] = symbols[i]
+
+                    n_asymmetric_atoms += 1
+                    I2 += n_sym_atoms
+                    self._atom_generators.append(I1.tolist())
+                    self._symop_to_atom.append(I2.tolist())
+                    n_sym_atoms += I1.shape[0]
+                tmp = []
+                for i, generators in enumerate(self._atom_generators):
+                    tmp.extend([i] * len(generators))
+                self._atom_to_asymmetric_atom = tmp
+                logger.info(f"{n_asymmetric_atoms=} {n_sym_atoms=}")
+
+    @staticmethod
+    def get_operators(self, value, periodicity=3):
+        """Get the symmetry operators as 4x4 matrices.
+
+        Parameters
+        ----------
+        value : str or [str]
+            The symmetry group or space group, or symmetry operators as strings.
+        periodicity : int
+            The periodicity of the structure. 3 for 3D, 2 for 2D, 1 for 1D, or 0.
+
+        Returns
+        -------
+        operators : np.ndarray
+            The symmetry operators as 4x4 matrices.
+        """
+        if isinstance(value, str):
+            if value == "":
+                raise RuntimeError("No group specified.")
+            if self.periodicity == 0:
+                if value != "C1":
+                    raise NotImplementedError("Point groups not implemented yet!")
+                W4 = [[1, 0, 0], [0, 1, 0], [0, 0, 1]]
+
+                W4s = []
+                W4s.append(W4)
+                operators = np.array(W4s, dtype=float)
+            else:
+                # Get the 4x4 augmented matrices
+                hall = _Symmetry.to_hall(value)
+                value = _Symmetry.hall_to_spacegroup_name(hall)
+                data = spglib.get_symmetry_from_database(hall)
+                W4s = []
+                for W, w in zip(
+                    data["rotations"].tolist(), data["translations"].tolist()
+                ):
+                    W4 = []
+                    for Wrow, w_i in zip(W, w):
+                        W4.append([*Wrow, w_i])
+                    W4.append([0, 0, 0, 1])
+                    W4s.append(W4)
+                operators = np.array(W4s, dtype=float)
+        elif isinstance(value, list):
+            W4s = []
+            operators = np.array(W4s, dtype=float)
+        return operators
+
+    @staticmethod
+    def hall_to_spacegroup_name(hall):
+        """Return the International name including setting for a hall number."""
+        if _Symmetry.hall_to_spgname is None:
+            _Symmetry.spgname_to_hall = None
+            _Symmetry.spacegroup_names_to_hall()
+        return _Symmetry.hall_to_spgname[hall]
+
+    @staticmethod
+    def spacegroup_names_to_hall():
+        """Dictionary of Hall number for spacegroup names."""
+        if _Symmetry.spgname_to_hall is None:
+            system_name = {
+                "international_full": "name_H-M_full",
+                "international": "name_H-M_alt",
+                "international_short": "name_H-M_short",
+                "hall_symbol": "name_Hall",
+            }
+            # Initialize the symmetry data
+            _Symmetry.spgname_to_hall = {}
+            _Symmetry.hall_to_spgname = {}
+            _Symmetry.hall_to_hall_symbol = {}
+            _Symmetry.hall_to_IT_number = {}
+            if _Symmetry.spgname_to_system is None:
+                _Symmetry.spgname_to_system = {}
+            for hall in range(1, 530):
+                data = spglib.get_spacegroup_type(hall)
+                # pws pprint.pprint(data)
+                choice = data["choice"]
+                _Symmetry.hall_to_hall_symbol[hall] = data["hall_symbol"]
+                _Symmetry.hall_to_IT_number[hall] = data["number"]
+
+                # Handle Hall to spacegroup using the full H-M name
+                key = "international_full"
+                name = data[key]
+
+                # Default setting if there are multiple, leave unadorned
+                if choice in ("2", "b", "b1", "H"):
+                    if (
+                        hall in _Symmetry.hall_to_spgname
+                        and name != _Symmetry.hall_to_spgname[hall]
+                    ):
+                        raise RuntimeError(
+                            f"{hall=} {key} --> {name} exists: "
+                            f"{_Symmetry.hall_to_spgname[hall]}"
+                        )
+                    else:
+                        _Symmetry.hall_to_spgname[hall] = name
+                else:
+                    # Add other settings to the spacegroup name
+                    if choice != "":
+                        name += f" :{choice}"
+                    if hall not in _Symmetry.hall_to_spgname:
+                        # pws if choice != "":
+                        # pws print(f"{hall} = {name}   QQQQQQQQQQQQQQQQQQQQQQ")
+                        _Symmetry.hall_to_spgname[hall] = name
+
+                # Now handle all the rest
+                for key in (
+                    "international_full",
+                    "international",
+                    "international_short",
+                    "hall_symbol",
+                ):
+                    name = data[key]
+
+                    # SPGLib encodes the international name: 'C 2/c = B 2/n 1 1',
+                    if key == "international":
+                        name = name.split("=")[0].strip()
+
+                    # Default setting if there are multiple, leave unadorned
+                    if choice in ("2", "b", "b1", "H"):
+                        _Symmetry.spgname_to_hall[name] = hall
+                        _Symmetry.spgname_to_system[name] = system_name[key]
+                        for txt in ("_", " "):
+                            tmp = name.replace(txt, "")
+                            _Symmetry.spgname_to_hall[tmp] = hall
+                            _Symmetry.spgname_to_system[tmp] = system_name[key]
+                            if tmp[-2:] == ":H":
+                                tmp = tmp[:-2].strip()
+                                _Symmetry.spgname_to_hall[tmp] = hall
+                                _Symmetry.spgname_to_system[tmp] = system_name[key]
+
+                    if key in ("international", "international_short") and choice != "":
+                        name += f" :{choice}"
+
+                    _Symmetry.spgname_to_hall[name] = hall
+                    _Symmetry.spgname_to_system[name] = system_name[key]
+                    for txt in ("_", " "):
+                        tmp = name.replace(txt, "")
+                        _Symmetry.spgname_to_hall[tmp] = hall
+                        _Symmetry.spgname_to_system[tmp] = system_name[key]
+                        if tmp[-2:] == ":H":
+                            tmp = tmp[:-2].strip()
+                            _Symmetry.spgname_to_hall[tmp] = hall
+                            _Symmetry.spgname_to_system[tmp] = system_name[key]
+        return _Symmetry.spgname_to_hall
+
+    @staticmethod
+    def spacegroup_numbers_to_hall():
+        """List of the Hall spacegroup names for the IT number."""
+        if _Symmetry.spgno_to_hall is None:
+            # Initialize the symmetry data
+            _Symmetry.spgno_to_hall = {}
+            if _Symmetry.spgname_to_system is None:
+                _Symmetry.spgname_to_system = {}
+            for hall in range(1, 530):
+                data = spglib.get_spacegroup_type(hall)
+                spgno = int(data["number"])
+                if spgno not in _Symmetry.spgno_to_hall:
+                    _Symmetry.spgno_to_hall[spgno] = hall
+                    _Symmetry.spgname_to_system[spgno] = "Int_Tables_number"
+                    _Symmetry.spgname_to_system[str(spgno)] = "Int_Tables_number"
+
+        return _Symmetry.spgno_to_hall
+
+    @staticmethod
+    def to_hall(name):
+        """Hall number given full spacegroup name or number."""
+        if isinstance(name, int):
+            return _Symmetry.spacegroup_numbers_to_hall()[name]
+        return _Symmetry.spacegroup_names_to_hall()[name]
+
+    @staticmethod
+    def spacegroup_names_to_system():
+        """Dictionary of system (name_Hall, name_H-M_full,...) for spacegroup names."""
+        if _Symmetry.spgname_to_hall is None:
+            _Symmetry.spacegroup_names_to_hall()
+        if _Symmetry.spgno_to_hall is None:
+            _Symmetry.spacegroup_numbers_to_hall()
+
+        return _Symmetry.spgname_to_system
+
     @property
     def configuration(self):
         """Return the configuration."""
         return self._configuration
 
     @property
     def cursor(self):
@@ -326,201 +658,14 @@
         return self._system
 
     @property
     def system_db(self):
         """Return the SystemDB object that contains this cell."""
         return self._system_db
 
-    @property
-    def spacegroup_numbers_to_hall(self):
-        """List of the Hall spacegroup names for the IT number."""
-        if _Symmetry.spgno_to_hall is None:
-            # Initialize the symmetry data
-            _Symmetry.spgno_to_hall = {}
-            if _Symmetry.spgname_to_system is None:
-                _Symmetry.spgname_to_system = {}
-            for hall in range(1, 530):
-                data = spglib.get_spacegroup_type(hall)
-                spgno = int(data["number"])
-                if spgno not in _Symmetry.spgno_to_hall:
-                    _Symmetry.spgno_to_hall[spgno] = hall
-                    _Symmetry.spgname_to_system[spgno] = "Int_Tables_number"
-                    _Symmetry.spgname_to_system[str(spgno)] = "Int_Tables_number"
-
-        return _Symmetry.spgno_to_hall
-
-    @property
-    def spacegroup_names_to_hall(self):
-        """Dictionary of Hall number for spacegroup names."""
-        if _Symmetry.spgname_to_hall is None:
-            system_name = {
-                "international_full": "name_H-M_full",
-                "international": "name_H-M_alt",
-                "international_short": "name_H-M_short",
-                "hall_symbol": "name_Hall",
-            }
-            # Initialize the symmetry data
-            _Symmetry.spgname_to_hall = {}
-            _Symmetry.hall_to_spgname = {}
-            _Symmetry.hall_to_hall_symbol = {}
-            _Symmetry.hall_to_IT_number = {}
-            if _Symmetry.spgname_to_system is None:
-                _Symmetry.spgname_to_system = {}
-            for hall in range(1, 530):
-                data = spglib.get_spacegroup_type(hall)
-                # pws pprint.pprint(data)
-                choice = data["choice"]
-                _Symmetry.hall_to_hall_symbol[hall] = data["hall_symbol"]
-                _Symmetry.hall_to_IT_number[hall] = data["number"]
-
-                # Handle Hall to spacegroup using the full H-M name
-                key = "international_full"
-                name = data[key]
-
-                # Default setting if there are multiple, leave unadorned
-                if choice in ("2", "b", "b1", "H"):
-                    if (
-                        hall in _Symmetry.hall_to_spgname
-                        and name != _Symmetry.hall_to_spgname[hall]
-                    ):
-                        raise RuntimeError(
-                            f"{hall=} {key} --> {name} exists: "
-                            f"{_Symmetry.hall_to_spgname[hall]}"
-                        )
-                    else:
-                        _Symmetry.hall_to_spgname[hall] = name
-                else:
-                    # Add other settings to the spacegroup name
-                    if choice != "":
-                        name += f" :{choice}"
-                    if hall not in _Symmetry.hall_to_spgname:
-                        # pws if choice != "":
-                        # pws print(f"{hall} = {name}   QQQQQQQQQQQQQQQQQQQQQQ")
-                        _Symmetry.hall_to_spgname[hall] = name
-
-                # Now handle all the rest
-                for key in (
-                    "international_full",
-                    "international",
-                    "international_short",
-                    "hall_symbol",
-                ):
-                    name = data[key]
-
-                    # SPGLib encodes the international name: 'C 2/c = B 2/n 1 1',
-                    if key == "international":
-                        name = name.split("=")[0].strip()
-
-                    # Default setting if there are multiple, leave unadorned
-                    if choice in ("2", "b", "b1", "H"):
-                        _Symmetry.spgname_to_hall[name] = hall
-                        _Symmetry.spgname_to_system[name] = system_name[key]
-                        for txt in ("_", " "):
-                            tmp = name.replace(txt, "")
-                            _Symmetry.spgname_to_hall[tmp] = hall
-                            _Symmetry.spgname_to_system[tmp] = system_name[key]
-                            if tmp[-2:] == ":H":
-                                tmp = tmp[:-2].strip()
-                                _Symmetry.spgname_to_hall[tmp] = hall
-                                _Symmetry.spgname_to_system[tmp] = system_name[key]
-
-                    if key in ("international", "international_short") and choice != "":
-                        name += f" :{choice}"
-
-                    _Symmetry.spgname_to_hall[name] = hall
-                    _Symmetry.spgname_to_system[name] = system_name[key]
-                    for txt in ("_", " "):
-                        tmp = name.replace(txt, "")
-                        _Symmetry.spgname_to_hall[tmp] = hall
-                        _Symmetry.spgname_to_system[tmp] = system_name[key]
-                        if tmp[-2:] == ":H":
-                            tmp = tmp[:-2].strip()
-                            _Symmetry.spgname_to_hall[tmp] = hall
-                            _Symmetry.spgname_to_system[tmp] = system_name[key]
-        return _Symmetry.spgname_to_hall
-
-    def old_spacegroup_names_to_hall(self):
-        """Dictionary of Hall number for spacegroup names."""
-        if _Symmetry.spgname_to_hall is None:
-            system_name = {
-                "international_full": "name_H-M_full",
-                "international": "name_H-M_alt",
-                "international_short": "name_H-M_short",
-                "hall_symbol": "name_Hall",
-            }
-            # Initialize the symmetry data
-            _Symmetry.spgname_to_hall = {}
-            _Symmetry.hall_to_spgname = {}
-            _Symmetry.hall_to_hall_symbol = {}
-            _Symmetry.hall_to_IT_number = {}
-            if _Symmetry.spgname_to_system is None:
-                _Symmetry.spgname_to_system = {}
-            for hall in range(1, 530):
-                data = spglib.get_spacegroup_type(hall)
-                choice = data["choice"]
-                _Symmetry.hall_to_hall_symbol[hall] = data["hall_symbol"]
-                _Symmetry.hall_to_IT_number[hall] = data["number"]
-                for key in (
-                    "international_full",
-                    "international",
-                    "international_short",
-                    "hall_symbol",
-                ):
-                    name = data[key]
-                    if "international" in key and choice in ("2",):
-                        if (
-                            name in _Symmetry.spgname_to_hall
-                            and hall != _Symmetry.spgname_to_hall[name]
-                        ):
-                            raise RuntimeError(
-                                f"{hall=} {key} --> {name} exists: "
-                                f"{_Symmetry.spgname_to_hall[name]}"
-                            )
-                        if key == "international":
-                            _Symmetry.hall_to_spgname[hall] = name
-                        _Symmetry.spgname_to_hall[name] = hall
-                        _Symmetry.spgname_to_system[name] = system_name[key]
-                        for txt in ("_", " "):
-                            tmp = name.replace(txt, "")
-                            _Symmetry.spgname_to_hall[tmp] = hall
-                            _Symmetry.spgname_to_system[tmp] = system_name[key]
-                    if choice != "":
-                        name += f" :{choice}"
-                    if (
-                        name in _Symmetry.spgname_to_hall
-                        and hall != _Symmetry.spgname_to_hall[name]
-                    ):
-                        raise RuntimeError(
-                            f"{hall=} {key} --> {name} exists: "
-                            f"{_Symmetry.spgname_to_hall[name]}"
-                        )
-                    if key == "international" and hall not in _Symmetry.spgname_to_hall:
-                        _Symmetry.hall_to_spgname[hall] = name
-                    _Symmetry.spgname_to_hall[name] = hall
-                    _Symmetry.spgname_to_system[name] = system_name[key]
-                    for txt in ("_", " "):
-                        tmp = name.replace(txt, "")
-                        _Symmetry.spgname_to_hall[tmp] = hall
-                        _Symmetry.spgname_to_system[tmp] = system_name[key]
-                        if tmp[-2:] == ":H":
-                            tmp = tmp[:-2].strip()
-                            _Symmetry.spgname_to_hall[tmp] = hall
-                            _Symmetry.spgname_to_system[tmp] = system_name[key]
-        return _Symmetry.spgname_to_hall
-
-    @property
-    def spacegroup_names_to_system(self):
-        """Dictionary of system (name_Hall, name_H-M_full,...) for spacegroup names."""
-        if _Symmetry.spgname_to_hall is None:
-            self.spacegroup_names_to_hall
-        if _Symmetry.spgno_to_hall is None:
-            self.spacegroup_numbers_to_hall
-
-        return _Symmetry.spgname_to_system
-
     def find_spacegroup_from_operators(self):
         """Find the spacegroup from the symmetry operators."""
         if self.configuration.periodicity > 0:
             # Treat P1 as special to avoid bug in spglib...
             if self.n_symops == 1:
                 hall_number = 1
                 international_number = 1
@@ -544,21 +689,14 @@
                             f"{international_number}."
                         )
                     if all(abs(data["origin_shift"]) < 0.001):
                         break
                     hall_number += 1
             return self.hall_to_spacegroup_name(hall_number)
 
-    def hall_to_spacegroup_name(self, hall):
-        """Return the International name including setting for a hall number."""
-        if _Symmetry.hall_to_spgname is None:
-            _Symmetry.spgname_to_hall = None
-            self.spacegroup_names_to_hall
-        return _Symmetry.hall_to_spgname[hall]
-
     def reset_atoms(self):
         """The atoms have changed, so need to recalculate the symmetric atoms."""
         self._operators = None
         self._atom_generators = None
         self._atom_to_asymmetric_atom = None
         self._symop_to_atom = None
 
@@ -588,23 +726,23 @@
             else:
                 raise NotImplementedError("symmetrize_atomic_scalar for molecules!")
 
         if self.n_symops == 1:
             return v_sym, None
 
         v_in = np.array(v_sym)
-        print(f"{v_in=}")
+        # print(f"{v_in=}")
         generators = self.atom_generators
         v = np.ndarray((len(generators),), dtype=float)
         delta = np.zeros_like(v_in)
         start = 0
         for asym_atom, ops in enumerate(generators):
-            print(f"{asym_atom=} {ops}")
+            # print(f"{asym_atom=} {ops}")
             n = len(ops)
-            print(f"{n=}")
+            # print(f"{n=}")
             v[asym_atom] = np.average(v_in[start : start + n], axis=0)
             delta[start : start + n] = v_in[start : start + n] - v[asym_atom]
             start += n
 
         if isinstance(v_sym, np.ndarray):
             return v, delta
         else:
@@ -708,20 +846,14 @@
         else:
             if fractionals:
                 return uvw.round(8).tolist(), delta.round(8).tolist()
             else:
                 tmp = self.configuration.cell.to_cartesians(uvw, as_array=True)
                 return tmp.round(8).tolist(), delta.round(8).tolist()
 
-    def to_hall(self, name):
-        """Hall number given full spacegroup name or number."""
-        if isinstance(name, int):
-            return self.spacegroup_numbers_to_hall[name]
-        return self.spacegroup_names_to_hall[name]
-
     def update_group(self, value):
         if self.configuration.periodicity == 0:
             if value != "C1":
                 raise NotImplementedError("Point groups not implemented yet!")
         self.db.execute(
             'UPDATE symmetry SET "group" = ? WHERE id = ?', (value, self.id)
         )
@@ -735,96 +867,128 @@
         else:
             v = np.array([0.0, 0.0, 0.0, 0.0])
         v[0:3] = vector
         xformed = np.einsum("ij,j", sym_mat, v)
         return xformed[0:3]
 
     def _expand(self):
-        """Setup the information for going from asymmetric cell to full cell."""
+        """Setup the information for going from asymmetric cell to full cell.
+
+        There is an issue with some CIF files, notably those from the Cambridge
+        structural database, where there are atoms in the asymmetric unit that
+        are duplicates. It appears that the CIF file is written with entire molecules
+        in some cases. So if the molecule is on a symmetry element, the atoms that are
+        related by symmetry are explicitly in the file.
+
+        To handle this we need to check for duplicates and remove them. Not a bad check
+        to have, anyway.
+        """
         operators = self.symmetry_matrices
 
+        symbols = self.configuration.atoms.asymmetric_symbols
         n_atoms = self.configuration.n_asymmetric_atoms
+        logger.info(f"Expanding {n_atoms} asymmetric atoms to full cell.")
         if n_atoms == 0:
             self._atom_generators = None
             self._symop_to_atom = None
         self._atom_generators = []  # Symmetry ops that create the symmetric atoms
         self._symop_to_atom = []  # The symmetry atom resulting from symmetry ops
         if self.configuration.periodicity == 3:
             if len(operators) == 1:
-                # P1 is a special case. Nothing to do!
+                # P1 is a special case. Nothing to do.
                 self._atom_generators = [[0] for i in range(n_atoms)]
                 self._symop_to_atom = [[i] for i in range(n_atoms)]
                 self._atom_to_asymmetric_atom = [*range(n_atoms)]
             else:
                 uvw0 = self.configuration.atoms.get_coordinates(
                     as_array=True, asymmetric=True
                 )
                 if uvw0.shape[0] != n_atoms:
                     raise RuntimeError(
                         f"Mismatch of number of atoms in symmetry: {uvw0.shape[0]} != "
                         f"{n_atoms}"
                     )
-                logger.debug("Original coordinates")
-                logger.debug(uvw0)
-                logger.debug(f"{uvw0.shape=}")
+                logger.debug(
+                    f"""
+{n_atoms=}
+{uvw0.shape=}"
+Original coordinates
+{uvw0}
+                    """
+                )
 
-                logger.debug(f"{n_atoms=}")
                 uvw = np.ndarray((n_atoms, 4))
-                logger.debug(f"{uvw.shape=}")
                 uvw[:, 0:3] = uvw0[:, :]
-                logger.debug("Expanded coordinates")
-                logger.debug(uvw)
+                logger.debug(f"\nExpanded coordinates\n{uvw}")
                 uvw[:, 3] = 1
                 # logger.debug(self.symops)
-                logger.debug(f"{operators.shape=}")
+                logger.debug(f"\n{operators.shape=}")
                 # logger.debug(operators)
-                logger.debug(f"{uvw.shape=}")
-                logger.debug("Expanded coordinates")
-                logger.debug(uvw)
+                # logger.debug(f"{uvw.shape=}")
+                # logger.debug("Expanded coordinates")
+                # logger.debug(uvw)
                 xformed = np.einsum("ijk,lk", operators, uvw)
-                logger.debug(f"{xformed.shape=}")
-                # logger.debug(xformed)
+                logger.debug(f"\n{xformed.shape=}\n{xformed}")
 
                 # For comparison, bring all atoms into the cell [0..1)
                 tmp = xformed - np.floor(xformed)
 
-                logger.debug("tmp")
-                logger.debug(tmp)
+                logger.debug(f"\ntmp = Transformed and floored coordinates\n{tmp}")
+
+                # Keep track of atoms and coordinates found so can check for duplicates
+                found = {}
 
                 n_sym_atoms = 0
+                n_asymmetric_atoms = 0
                 for i in range(n_atoms):
                     values, I1, I2 = np.unique(
                         np.round(tmp[:, :3, i], 4),
                         axis=0,
                         return_index=True,
                         return_inverse=True,
                     )
-                    logger.debug(f"{i=}")
                     # pprint.pprint(np.round(tmp[:, :3, i], 4).tolist())
-                    logger.debug("values")
-                    # pprint.pprint(values.tolist())
-                    logger.debug(values)
-                    logger.debug("I1")
-                    logger.debug(I1)
-                    logger.debug("I2")
-                    logger.debug(I2)
+                    logger.debug(
+                        f"""
+{i=}: {symbols[i]}
+{np.round(tmp[:, :3, i], 4)}
+nvalues
+{values}
+I1
+{I1}
+I2
+{I2}
+                        """
+                    )
+                    # Check for duplicates
+                    if tuple(values[0]) in found:
+                        if found[tuple(values[0])] != symbols[i]:
+                            raise RuntimeError(
+                                "Duplicate atoms with different symbols: "
+                                f"{symbols[i]} != {found[tuple(values[0])]} at "
+                                f"{values[0]}"
+                            )
+                        else:
+                            # Same element, so ignore
+                            logger.debug("\nDuplicate atom, ignoring")
+                            continue
+
+                    for value in values:
+                        found[tuple(value)] = symbols[i]
+
+                    n_asymmetric_atoms += 1
                     I2 += n_sym_atoms
                     self._atom_generators.append(I1.tolist())
                     self._symop_to_atom.append(I2.tolist())
                     n_sym_atoms += I1.shape[0]
                 tmp = []
                 for i, generators in enumerate(self._atom_generators):
                     tmp.extend([i] * len(generators))
                 self._atom_to_asymmetric_atom = tmp
-        else:
-            if len(operators) == 1:
-                # P1 is a special case. Nothing to do!
-                self._atom_generators = [[0] for i in range(n_atoms)]
-                self._symop_to_atom = [[i] for i in range(n_atoms)]
-                self._atom_to_asymmetric_atom = [*range(n_atoms)]
+                logger.info(f"{n_asymmetric_atoms=} {n_sym_atoms=}")
 
     def _expand_bonds(self):
         """Expand the list of asymmetric bonds to the full list.
 
         Keep track of the following:
 
             1. bond_to_asymmetric_bond: the asymmetric bond index for each bond
```

### Comparing `molsystem-2024.3.13/molsystem/system.py` & `molsystem-2024.4.5/molsystem/system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/system_db.py` & `molsystem-2024.4.5/molsystem/system_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -966,14 +966,29 @@
                 "CREATE INDEX 'idx_velocities_atom' ON velocities (\"atom\")"
             )
             self.db.execute(
                 "CREATE INDEX idx_velocities_atom_configuration "
                 "    ON velocities(atom, configuration)"
             )
 
+            # Keep the gradients separate from coordinates to keep the size down
+            table = self["gradients"]
+            table.add_attribute(
+                "configuration", coltype="int", references="configuration"
+            )
+            table.add_attribute("atom", coltype="int", references="atom")
+            table.add_attribute("gx", coltype="float")
+            table.add_attribute("gy", coltype="float")
+            table.add_attribute("gz", coltype="float")
+            self.db.execute("CREATE INDEX 'idx_gradients_atom' ON gradients (\"atom\")")
+            self.db.execute(
+                "CREATE INDEX idx_gradients_atom_configuration "
+                "    ON gradients(atom, configuration)"
+            )
+
             # The definition of the subsets -- templates
             table = self["template"]
             table.add_attribute("id", coltype="int", pk=True)
             table.add_attribute("name", coltype="str")
             table.add_attribute("canonical_smiles", coltype="str")
             table.add_attribute("category", coltype="str", default="general")
             table.add_attribute(
```

### Comparing `molsystem-2024.3.13/molsystem/system_properties.py` & `molsystem-2024.4.5/molsystem/system_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/table.py` & `molsystem-2024.4.5/molsystem/table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/template.py` & `molsystem-2024.4.5/molsystem/template.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/templates.py` & `molsystem-2024.4.5/molsystem/templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem/topology.py` & `molsystem-2024.4.5/molsystem/topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/molsystem.egg-info/PKG-INFO` & `molsystem-2024.4.5/molsystem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2024.3.13
+Version: 2024.4.5
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -113,14 +113,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.4.6 -- Added gradients
+    * Added gradient on atoms as a separate table alongside atoms, so they take no space
+      unless actually used.
+      
 2024.3.13 -- Handle uppercase X, Y, Z in strings for symmetry operators
     * the Crystallographic Open Database CIF files seems to use upper case X, Y, Z in
       explicit symmetry operators. These need to be lowercased in the code.
 
 2023.12.5 -- Bugfixes for symmetry
     * Fixed issue #72, where symmetry was not correctly handled for trigonal and
       hexagonal cells where atoms had coordinates of 1/3 or 2/3.
```

### Comparing `molsystem-2024.3.13/molsystem.egg-info/SOURCES.txt` & `molsystem-2024.4.5/molsystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/setup.py` & `molsystem-2024.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/conftest.py` & `molsystem-2024.4.5/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,14 +318,17 @@
     configuration.periodicity = 3
     configuration.coordinate_system = "fractional"
     configuration.cell.parameters = [3.03, 3.03, 3.03, 90, 90, 90]
     configuration.atoms.append(
         x=[0.0, 0.5],
         y=[0.0, 0.5],
         z=[0.0, 0.5],
+        gx=[0.0, 0.02],
+        gy=[0.01, -0.02],
+        gz=[-0.01, 0.01],
         vx=[0.0, 0.02],
         vy=[0.01, -0.02],
         vz=[-0.01, 0.01],
         symbol="V",
     )
     return configuration
```

### Comparing `molsystem-2024.3.13/tests/data/1n9v.cif` & `molsystem-2024.4.5/tests/data/1n9v.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/aa-variants-v1.cif` & `molsystem-2024.4.5/tests/data/aa-variants-v1.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/acy.mmcif` & `molsystem-2024.4.5/tests/data/acy.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/aminoacids.mmcif` & `molsystem-2024.4.5/tests/data/aminoacids.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/benzene.cif` & `molsystem-2024.4.5/tests/data/benzene.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/hoh.mmcif` & `molsystem-2024.4.5/tests/data/hoh.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/polyethylene.cif` & `molsystem-2024.4.5/tests/data/polyethylene.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/spacegroup_names.json` & `molsystem-2024.4.5/tests/data/spacegroup_names.json`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/data/trigonal.cif` & `molsystem-2024.4.5/tests/data/trigonal.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_angiotensin.py` & `molsystem-2024.4.5/tests/test_angiotensin.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_atoms.py` & `molsystem-2024.4.5/tests/test_atoms.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,28 @@
     """Simplest test that we can make an Atoms object"""
     atoms = configuration.atoms
     assert str(type(atoms)) == "<class 'molsystem.atoms._Atoms'>"
 
 
 def test_keys(atoms):
     """Test the default keys in an Atoms object"""
-    result = ["atno", "configuration", "id", "vx", "vy", "vz", "x", "y", "z"]
+    result = [
+        "atno",
+        "configuration",
+        "gx",
+        "gy",
+        "gz",
+        "id",
+        "vx",
+        "vy",
+        "vz",
+        "x",
+        "y",
+        "z",
+    ]
 
     if sorted([*atoms.keys()]) != result:
         print(sorted([*atoms.keys()]))
     assert sorted([*atoms.keys()]) == result
 
 
 def test_n_atoms_empty(atoms):
@@ -76,44 +89,93 @@
     assert atoms.n_atoms == 0
     assert atoms.configuration.version == 0
     assert str(e.value) == "'\"bad\" is not an attribute of the atoms.'"
 
 
 def test_add_attribute(atoms):
     """Test adding an attribute"""
-    result = ["atno", "configuration", "id", "name", "vx", "vy", "vz", "x", "y", "z"]
+    result = [
+        "atno",
+        "configuration",
+        "gx",
+        "gy",
+        "gz",
+        "id",
+        "name",
+        "vx",
+        "vy",
+        "vz",
+        "x",
+        "y",
+        "z",
+    ]
     with atoms as tmp:
         tmp.add_attribute("name")
     assert sorted([*atoms.keys()]) == result
 
 
 def test_add_duplicate_attribute(atoms):
     """Test duplicate adding an attribute"""
-    result = ["atno", "configuration", "id", "name", "vx", "vy", "vz", "x", "y", "z"]
+    result = [
+        "atno",
+        "configuration",
+        "gx",
+        "gy",
+        "gz",
+        "id",
+        "name",
+        "vx",
+        "vy",
+        "vz",
+        "x",
+        "y",
+        "z",
+    ]
     with atoms as tmp:
         tmp.add_attribute("name")
     with pytest.raises(RuntimeError) as e:
         with atoms as tmp:
             ver = tmp.configuration.version
             tmp.add_attribute("name")
     assert sorted([*atoms.keys()]) == result
     assert ver == 1
     assert atoms.configuration.version == 1
     assert str(e.value) == "_Table attribute 'name' is already defined!"
 
 
 def test_add_coordinates_attribute(atoms):
     """Test adding an attribute"""
-    result = ["atno", "configuration", "id", "spin", "vx", "vy", "vz", "x", "y", "z"]
+    correct = [
+        "atno",
+        "configuration",
+        "gx",
+        "gy",
+        "gz",
+        "id",
+        "spin",
+        "vx",
+        "vy",
+        "vz",
+        "x",
+        "y",
+        "z",
+    ]
     with atoms as tmp:
         tmp.add_attribute("spin", configuration_dependent=True)
-    assert sorted([*atoms.keys()]) == result
+    result = sorted([*atoms.keys()])
+    if result != correct:
+        print(result)
+    assert result == correct
+
     del atoms["spin"]
-    result.remove("spin")
-    assert sorted([*atoms.keys()]) == result
+    correct.remove("spin")
+    result = sorted([*atoms.keys()])
+    if result != correct:
+        print(result)
+    assert result == correct
 
 
 def test_add_attribute_with_values(atoms):
     """Test adding several atoms"""
     with atoms as tmp:
         tmp.append(x=x, y=y, z=z, atno=atno)
         tmp.add_attribute("name", values=["H1", "O", "H2"])
@@ -182,14 +244,17 @@
 
 def test_deleting_column(atoms):
     """Test deleting a column"""
     with atoms as tmp:
         del tmp["atno"]
     assert sorted([*atoms.keys()]) == [
         "configuration",
+        "gx",
+        "gy",
+        "gz",
         "id",
         "vx",
         "vy",
         "vz",
         "x",
         "y",
         "z",
@@ -515,7 +580,56 @@
     vxs = [0.0, 0.02]
     vys = [0.01, -0.02]
     vzs = [-0.01, 0.01]
     vxyz0 = [[vx * 3.03, vy * 3.03, vz * 3.03] for vx, vy, vz in zip(vxs, vys, vzs)]
 
     vxyz = configuration.atoms.get_velocities(fractionals=False)
     assert np.allclose(vxyz, vxyz0)
+
+
+def test_have_gradients(AceticAcid):
+    """Test whether there are gradients."""
+    assert not AceticAcid.atoms.have_gradients
+
+
+def test_set_gradients(AceticAcid):
+    """Test setting gradients."""
+    configuration = AceticAcid
+
+    xs = [1.08, 0.58, 0.72, 0.71, 0.57, -0.13, 0.98, 2.17]
+    ys = [0.02, 3.14, -0.67, -0.31, 1.39, 1.71, 2.30, 0.02]
+    zs = [-0.02, 0.28, -0.79, 0.95, -0.32, -1.26, 0.59, -0.03]
+    gxyz0 = [[x, y, z] for x, y, z in zip(xs, ys, zs)]
+
+    configuration.atoms.set_gradients(gxyz0)
+
+    gxyz = configuration.atoms.gradients
+    if not np.allclose(gxyz, gxyz0):
+        print(gxyz)
+        print(" != ", gxyz0)
+    assert np.allclose(gxyz, gxyz0)
+
+
+def test_periodic_gradients(vanadium):
+    """Test getting gradients."""
+    configuration = vanadium
+
+    gxs = [0.0, 0.02]
+    gys = [0.01, -0.02]
+    gzs = [-0.01, 0.01]
+    gxyz0 = [[gx, gy, gz] for gx, gy, gz in zip(gxs, gys, gzs)]
+
+    gxyz = configuration.atoms.gradients
+    assert np.allclose(gxyz, gxyz0)
+
+
+def test_periodic_gradients_cartesians(vanadium):
+    """Test getting gradients in Cartesian gradients."""
+    configuration = vanadium
+
+    gxs = [0.0, 0.02]
+    gys = [0.01, -0.02]
+    gzs = [-0.01, 0.01]
+    gxyz0 = [[gx * 3.03, gy * 3.03, gz * 3.03] for gx, gy, gz in zip(gxs, gys, gzs)]
+
+    gxyz = configuration.atoms.get_gradients(fractionals=False)
+    assert np.allclose(gxyz, gxyz0)
```

### Comparing `molsystem-2024.3.13/tests/test_bonds.py` & `molsystem-2024.4.5/tests/test_bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_cell.py` & `molsystem-2024.4.5/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_cif.py` & `molsystem-2024.4.5/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_configuration_properties.py` & `molsystem-2024.4.5/tests/test_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_configurations.py` & `molsystem-2024.4.5/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_inchi.py` & `molsystem-2024.4.5/tests/test_inchi.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_molfile.py` & `molsystem-2024.4.5/tests/test_molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_openbabel.py` & `molsystem-2024.4.5/tests/test_openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_pdb.py` & `molsystem-2024.4.5/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_properties.py` & `molsystem-2024.4.5/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_property_timings.py` & `molsystem-2024.4.5/tests/test_property_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_pubchem.py` & `molsystem-2024.4.5/tests/test_pubchem.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_qcschema.py` & `molsystem-2024.4.5/tests/test_qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_rdkit.py` & `molsystem-2024.4.5/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_smiles.py` & `molsystem-2024.4.5/tests/test_smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_subsets.py` & `molsystem-2024.4.5/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_symmetry.py` & `molsystem-2024.4.5/tests/test_symmetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 def test_spacegroup_names(symmetry):
     """Test the correspondance of spacegroup names and Hall numbers."""
     path = Path(__file__).parent / "data" / "spacegroup_names.json"
     with path.open() as fd:
         correct = json.load(fd)
-    answer = symmetry.spacegroup_names_to_hall
+    answer = symmetry.spacegroup_names_to_hall()
     if answer != correct:
         print(json.dumps(answer, indent=3))
     assert answer == correct
 
 
 def test_spacegroup(symmetry):
     """Handling of a spacegroup."""
```

### Comparing `molsystem-2024.3.13/tests/test_system.py` & `molsystem-2024.4.5/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_system_db.py` & `molsystem-2024.4.5/tests/test_system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_table.py` & `molsystem-2024.4.5/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_templates.py` & `molsystem-2024.4.5/tests/test_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             47.549,
             46.757,
             47.703,
             44.09,
         ],
     }
     for column in gly.atoms:
-        if column in ("vx", "vy", "vz"):
+        if column in ("gx", "gy", "gz", "vx", "vy", "vz"):
             continue
         result = gly.atoms.get_column_data(column)
         if column not in answer:
             print(f"'{column}': {result}")
         assert column in answer
         if result != answer[column]:
             print(f"'{column}': {result}")
```

### Comparing `molsystem-2024.3.13/tests/test_timings.py` & `molsystem-2024.4.5/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/tests/test_topology.py` & `molsystem-2024.4.5/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.3.13/versioneer.py` & `molsystem-2024.4.5/versioneer.py`

 * *Files identical despite different names*

