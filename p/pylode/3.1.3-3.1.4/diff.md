# Comparing `tmp/pylode-3.1.3.tar.gz` & `tmp/pylode-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylode-3.1.3.tar", max compression
+gzip compressed data, was "pylode-3.1.4.tar", max compression
```

## Comparing `pylode-3.1.3.tar` & `pylode-3.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1524 2024-03-18 09:35:48.457001 pylode-3.1.3/LICENSE
--rw-r--r--   0        0        0    11982 2024-03-18 09:35:48.457001 pylode-3.1.3/README.rst
--rw-r--r--   0        0        0      190 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/__init__.py
--rw-r--r--   0        0        0       72 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/__main__.py
--rw-r--r--   0        0        0     2201 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/cli.py
--rw-r--r--   0        0        0       89 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/__init__.py
--rw-r--r--   0        0        0    24998 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/ontpub.py
--rw-r--r--   0        0        0       29 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/__init__.py
--rw-r--r--   0        0        0      165 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/__init__.py
--rw-r--r--   0        0        0     1702 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/example.py
--rw-r--r--   0        0        0     2018 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/heading.py
--rw-r--r--   0        0        0      395 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/link.py
--rw-r--r--   0        0        0     1237 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/preamble.py
--rw-r--r--   0        0        0     8584 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/properties_table.py
--rw-r--r--   0        0        0      258 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/component/tooltip.py
--rw-r--r--   0        0        0      981 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/dataset.py
--rw-r--r--   0        0        0      200 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/fragment.py
--rw-r--r--   0        0        0    42490 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/html.py
--rw-r--r--   0        0        0     9821 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/loader.py
--rw-r--r--   0        0        0     5758 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/model.py
--rw-r--r--   0        0        0     1019 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/namespace.py
--rw-r--r--   0        0        0    37284 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/query/__init__.py
--rw-r--r--   0        0        0     2768 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/query/common.py
--rw-r--r--   0        0        0    10101 2024-03-18 09:35:48.521002 pylode-3.1.3/pylode/profiles/supermodel/query/property_shape.py
--rw-r--r--   0        0        0      110 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/profiles/supermodel/random.py
--rw-r--r--   0        0        0       17 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/profiles/supermodel/state.py
--rw-r--r--   0        0        0    25010 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/profiles/vocpub.py
--rw-r--r--   0        0        0     5079 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/pylode.css
--rw-r--r--   0        0        0    47847 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/dcterms-mod.ttl
--rw-r--r--   0        0        0     3593 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/licenses.ttl
--rw-r--r--   0        0        0     1702 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/ontdoc.ttl
--rw-r--r--   0        0        0    23997 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/owl.ttl
--rw-r--r--   0        0        0   112669 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/prov.ttl
--rw-r--r--   0        0        0     6004 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/rdf.ttl
--rw-r--r--   0        0        0     3816 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/rdfs-mod.ttl
--rw-r--r--   0        0        0   565104 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/sdo-mod.ttl
--rw-r--r--   0        0        0    16123 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/skos.ttl
--rw-r--r--   0        0        0    10983 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf/void.ttl
--rw-r--r--   0        0        0     3044 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/rdf_elements.py
--rw-r--r--   0        0        0    29020 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/static/asciidoc.css
--rw-r--r--   0        0        0      801 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/static/hierarchy.css
--rw-r--r--   0        0        0     1228 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/static/hierarchy.js
--rw-r--r--   0        0        0     2046 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/static/property-table-row.js
--rw-r--r--   0        0        0      601 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/static/pylode.css
--rw-r--r--   0        0        0    32772 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/utils.py
--rw-r--r--   0        0        0       22 2024-03-18 09:35:48.525002 pylode-3.1.3/pylode/version.py
--rw-r--r--   0        0        0      639 2024-03-18 09:36:06.333229 pylode-3.1.3/pyproject.toml
--rw-r--r--   0        0        0    12674 1970-01-01 00:00:00.000000 pylode-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-04-06 06:34:08.738093 pylode-3.1.4/LICENSE
+-rw-r--r--   0        0        0    12021 2024-04-06 06:34:08.738093 pylode-3.1.4/README.rst
+-rw-r--r--   0        0        0      190 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/__main__.py
+-rw-r--r--   0        0        0     2201 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/cli.py
+-rw-r--r--   0        0        0       89 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/__init__.py
+-rw-r--r--   0        0        0    24998 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/ontpub.py
+-rw-r--r--   0        0        0       29 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/example.py
+-rw-r--r--   0        0        0     2018 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/heading.py
+-rw-r--r--   0        0        0      395 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/link.py
+-rw-r--r--   0        0        0     1237 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/preamble.py
+-rw-r--r--   0        0        0     8584 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/properties_table.py
+-rw-r--r--   0        0        0      258 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/component/tooltip.py
+-rw-r--r--   0        0        0      981 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/dataset.py
+-rw-r--r--   0        0        0      200 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/fragment.py
+-rw-r--r--   0        0        0    42490 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/html.py
+-rw-r--r--   0        0        0     9821 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/loader.py
+-rw-r--r--   0        0        0     5758 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/model.py
+-rw-r--r--   0        0        0     1019 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/namespace.py
+-rw-r--r--   0        0        0    37284 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/query/__init__.py
+-rw-r--r--   0        0        0     2768 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/query/common.py
+-rw-r--r--   0        0        0    10101 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/query/property_shape.py
+-rw-r--r--   0        0        0      110 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/random.py
+-rw-r--r--   0        0        0       17 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/supermodel/state.py
+-rw-r--r--   0        0        0    25010 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/profiles/vocpub.py
+-rw-r--r--   0        0        0     5079 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/pylode.css
+-rw-r--r--   0        0        0    47847 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/rdf/dcterms-mod.ttl
+-rw-r--r--   0        0        0     3593 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/rdf/licenses.ttl
+-rw-r--r--   0        0        0     1702 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/rdf/ontdoc.ttl
+-rw-r--r--   0        0        0    23997 2024-04-06 06:34:08.806093 pylode-3.1.4/pylode/rdf/owl.ttl
+-rw-r--r--   0        0        0   112669 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf/prov.ttl
+-rw-r--r--   0        0        0     6004 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf/rdf.ttl
+-rw-r--r--   0        0        0     3816 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf/rdfs-mod.ttl
+-rw-r--r--   0        0        0   565104 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf/sdo-mod.ttl
+-rw-r--r--   0        0        0    16123 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf/skos.ttl
+-rw-r--r--   0        0        0    10983 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf/void.ttl
+-rw-r--r--   0        0        0     3044 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/rdf_elements.py
+-rw-r--r--   0        0        0    29020 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/static/asciidoc.css
+-rw-r--r--   0        0        0      801 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/static/hierarchy.css
+-rw-r--r--   0        0        0     1228 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/static/hierarchy.js
+-rw-r--r--   0        0        0     2046 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/static/property-table-row.js
+-rw-r--r--   0        0        0      601 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/static/pylode.css
+-rw-r--r--   0        0        0    32891 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/utils.py
+-rw-r--r--   0        0        0       22 2024-04-06 06:34:08.810093 pylode-3.1.4/pylode/version.py
+-rw-r--r--   0        0        0      639 2024-04-06 06:34:24.874175 pylode-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0    12713 1970-01-01 00:00:00.000000 pylode-3.1.4/PKG-INFO
```

### Comparing `pylode-3.1.3/LICENSE` & `pylode-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/README.rst` & `pylode-3.1.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -280,19 +280,20 @@
 Release Schedule
 ----------------
 
 .. csv-table:: **pyLODE Release Schedule**
    :header: "Version", "Date", "Description"
    :widths: 15, 10, 30
 
-   **3.1.3**, **18 March 2024**, "Relax rdflib version constraint"
-   **3.1.2**, **18 March 2024**, "Relax httpx version constraint"
-   **3.1.1**, **19 February 2024**, "Fix release"
-   **3.1.0**, **19 February 2024**, "Add supermodel mode - supports documenting profiles and modules"
-   **3.0.5**, **27 April 2023**, "Minor patching"
+   3.1.4, 6 April 2024, "Fix load_ontology function's detection of data input"
+   3.1.3, 18 March 2024, "Relax rdflib version constraint"
+   3.1.2, 18 March 2024, "Relax httpx version constraint"
+   3.1.1, 19 February 2024, "Fix release"
+   3.1.0, 19 February 2024, "Add supermodel mode - supports documenting profiles and modules"
+   3.0.5, 27 April 2023, "Minor patching"
    3.0.4, 24 May 2022, "Use of Poetry"
    3.0.2, 24 May 2022, "Support for preformatted skos:example literals"
    3.0.1, 6 Jan 2022, "Direct HTML generation using dominate; easier to maintain and extend"
    2.13.2, 21 December 2021, "Updated RDFlib to 6.1.1, improved test to properly use pytest"
    2.10.0, 24 May 2021, "Update Windows EXE build process, simplified versioning"
    2.9.1, 28 Apr 2021, "Support for ASCIIDOC format (OntDoc profile only)"
    2.8.11, 28 Apr 2021, "Further changes for PyPI only"
```

### Comparing `pylode-3.1.3/pylode/cli.py` & `pylode-3.1.4/pylode/cli.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/ontpub.py` & `pylode-3.1.4/pylode/profiles/ontpub.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/component/example.py` & `pylode-3.1.4/pylode/profiles/supermodel/component/example.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/component/heading.py` & `pylode-3.1.4/pylode/profiles/supermodel/component/heading.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/component/preamble.py` & `pylode-3.1.4/pylode/profiles/supermodel/component/preamble.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/component/properties_table.py` & `pylode-3.1.4/pylode/profiles/supermodel/component/properties_table.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/dataset.py` & `pylode-3.1.4/pylode/profiles/supermodel/dataset.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/html.py` & `pylode-3.1.4/pylode/profiles/supermodel/html.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/loader.py` & `pylode-3.1.4/pylode/profiles/supermodel/loader.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/model.py` & `pylode-3.1.4/pylode/profiles/supermodel/model.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/namespace.py` & `pylode-3.1.4/pylode/profiles/supermodel/namespace.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/query/__init__.py` & `pylode-3.1.4/pylode/profiles/supermodel/query/__init__.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/query/common.py` & `pylode-3.1.4/pylode/profiles/supermodel/query/common.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/supermodel/query/property_shape.py` & `pylode-3.1.4/pylode/profiles/supermodel/query/property_shape.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/profiles/vocpub.py` & `pylode-3.1.4/pylode/profiles/vocpub.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/pylode.css` & `pylode-3.1.4/pylode/pylode.css`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/dcterms-mod.ttl` & `pylode-3.1.4/pylode/rdf/dcterms-mod.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/licenses.ttl` & `pylode-3.1.4/pylode/rdf/licenses.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/ontdoc.ttl` & `pylode-3.1.4/pylode/rdf/ontdoc.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/owl.ttl` & `pylode-3.1.4/pylode/rdf/owl.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/prov.ttl` & `pylode-3.1.4/pylode/rdf/prov.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/rdf.ttl` & `pylode-3.1.4/pylode/rdf/rdf.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/rdfs-mod.ttl` & `pylode-3.1.4/pylode/rdf/rdfs-mod.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/sdo-mod.ttl` & `pylode-3.1.4/pylode/rdf/sdo-mod.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/skos.ttl` & `pylode-3.1.4/pylode/rdf/skos.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf/void.ttl` & `pylode-3.1.4/pylode/rdf/void.ttl`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/rdf_elements.py` & `pylode-3.1.4/pylode/rdf_elements.py`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/static/asciidoc.css` & `pylode-3.1.4/pylode/static/asciidoc.css`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/static/hierarchy.css` & `pylode-3.1.4/pylode/static/hierarchy.css`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/static/hierarchy.js` & `pylode-3.1.4/pylode/static/hierarchy.js`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/static/property-table-row.js` & `pylode-3.1.4/pylode/static/property-table-row.js`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/static/pylode.css` & `pylode-3.1.4/pylode/static/pylode.css`

 * *Files identical despite different names*

### Comparing `pylode-3.1.3/pylode/utils.py` & `pylode-3.1.4/pylode/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,25 +238,33 @@
 
     pl = {}
     for prop in PROPS:
         pl[prop] = _get_prop_label(prop, back_onts)
     return pl
 
 
+def _is_file(filepath: str) -> bool:
+    try:
+        if Path(filepath).is_file():
+            return True
+        return False
+    except:
+        return False
+
+
 def load_ontology(ontology: Union[Graph, Path, str]) -> Graph:
     """Loads and ontology into an RDFLib Graph.
 
     Can handle string data, file path, URL or Graph input"""
     try:
         # try URL
         if isinstance(ontology, str) and ontology.startswith("http"):
             return Graph().parse(location=ontology)
         elif isinstance(ontology, str):
-            # see if it's a file path
-            if Path(ontology).is_file():
+            if _is_file(ontology):
                 return Graph().parse(ontology)
             else:  # it's data
                 if ontology.startswith("[") or ontology.startswith("{"):
                     input_format = "json-ld"
                 elif (
                     ontology.startswith("<?xml")
                     or ontology.startswith("<!--")
```

### Comparing `pylode-3.1.3/pyproject.toml` & `pylode-3.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylode"
-version = "3.1.3"
+version = "3.1.4"
 description = "An OWL ontology documentation tool using Python, based on LODE."
 authors = ["Nicholas Car <nick@kurrawong.net>"]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rdflib = ">=6.0.0,<8.0.0"
```

### Comparing `pylode-3.1.3/PKG-INFO` & `pylode-3.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylode
-Version: 3.1.3
+Version: 3.1.4
 Summary: An OWL ontology documentation tool using Python, based on LODE.
 Author: Nicholas Car
 Author-email: nick@kurrawong.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -299,19 +299,20 @@
 Release Schedule
 ----------------
 
 .. csv-table:: **pyLODE Release Schedule**
    :header: "Version", "Date", "Description"
    :widths: 15, 10, 30
 
-   **3.1.3**, **18 March 2024**, "Relax rdflib version constraint"
-   **3.1.2**, **18 March 2024**, "Relax httpx version constraint"
-   **3.1.1**, **19 February 2024**, "Fix release"
-   **3.1.0**, **19 February 2024**, "Add supermodel mode - supports documenting profiles and modules"
-   **3.0.5**, **27 April 2023**, "Minor patching"
+   3.1.4, 6 April 2024, "Fix load_ontology function's detection of data input"
+   3.1.3, 18 March 2024, "Relax rdflib version constraint"
+   3.1.2, 18 March 2024, "Relax httpx version constraint"
+   3.1.1, 19 February 2024, "Fix release"
+   3.1.0, 19 February 2024, "Add supermodel mode - supports documenting profiles and modules"
+   3.0.5, 27 April 2023, "Minor patching"
    3.0.4, 24 May 2022, "Use of Poetry"
    3.0.2, 24 May 2022, "Support for preformatted skos:example literals"
    3.0.1, 6 Jan 2022, "Direct HTML generation using dominate; easier to maintain and extend"
    2.13.2, 21 December 2021, "Updated RDFlib to 6.1.1, improved test to properly use pytest"
    2.10.0, 24 May 2021, "Update Windows EXE build process, simplified versioning"
    2.9.1, 28 Apr 2021, "Support for ASCIIDOC format (OntDoc profile only)"
    2.8.11, 28 Apr 2021, "Further changes for PyPI only"
```

