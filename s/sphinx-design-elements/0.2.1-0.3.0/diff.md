# Comparing `tmp/sphinx-design-elements-0.2.1.tar.gz` & `tmp/sphinx-design-elements-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-design-elements-0.2.1.tar", last modified: Tue Aug  8 00:46:38 2023, max compression
+gzip compressed data, was "sphinx-design-elements-0.3.0.tar", last modified: Sat Apr  6 16:27:47 2024, max compression
```

## Comparing `sphinx-design-elements-0.2.1.tar` & `sphinx-design-elements-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,62 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.616178 sphinx-design-elements-0.2.1/
--rw-r--r--   0 amo        (501) staff       (20)      468 2023-08-08 00:46:07.000000 sphinx-design-elements-0.2.1/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.2.1/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      139 2023-08-08 00:45:53.000000 sphinx-design-elements-0.2.1/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     5285 2023-08-08 00:46:38.615921 sphinx-design-elements-0.2.1/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     2144 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.1/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.605888 sphinx-design-elements-0.2.1/docs/
--rw-r--r--   0 amo        (501) staff       (20)      258 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.1/docs/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)      468 2023-08-08 00:46:07.000000 sphinx-design-elements-0.2.1/docs/changes.md
--rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.1/docs/css_classes.md
--rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.1/docs/dropdown-group.md
--rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx-design-elements-0.2.1/docs/get_started.md
--rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.1/docs/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)     3566 2023-08-07 22:11:04.000000 sphinx-design-elements-0.2.1/docs/index.md
--rw-r--r--   0 amo        (501) staff       (20)     2943 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.1/docs/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.2.1/docs/project.md
--rw-r--r--   0 amo        (501) staff       (20)     2144 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.1/docs/readme.md
--rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx-design-elements-0.2.1/docs/sandbox.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.606462 sphinx-design-elements-0.2.1/docs/snippets/
--rw-r--r--   0 amo        (501) staff       (20)       73 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.1/docs/snippets/index.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.608335 sphinx-design-elements-0.2.1/docs/snippets/myst/
--rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.1/docs/snippets/myst/dropdown-group.md
--rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.1/docs/snippets/myst/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.2.1/docs/snippets/myst/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.2.1/docs/snippets/myst/tag.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.610486 sphinx-design-elements-0.2.1/docs/snippets/rst/
--rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.1/docs/snippets/rst/dropdown-group.rst
--rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.1/docs/snippets/rst/gridtable.rst
--rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.2.1/docs/snippets/rst/infocard.rst
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.2.1/docs/snippets/rst/tag.rst
--rw-r--r--   0 amo        (501) staff       (20)     2832 2023-07-19 19:40:43.000000 sphinx-design-elements-0.2.1/docs/tag.md
--rw-r--r--   0 amo        (501) staff       (20)     4939 2023-08-08 00:45:53.000000 sphinx-design-elements-0.2.1/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-08-08 00:46:38.616259 sphinx-design-elements-0.2.1/setup.cfg
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.613111 sphinx-design-elements-0.2.1/sphinx_design_elements/
--rw-r--r--   0 amo        (501) staff       (20)      433 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.615357 sphinx-design-elements-0.2.1/sphinx_design_elements/compiled/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/compiled/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      879 2023-08-08 00:45:53.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/compiled/addon.js
--rw-r--r--   0 amo        (501) staff       (20)      965 2023-08-08 00:31:45.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/compiled/style.css
--rw-r--r--   0 amo        (501) staff       (20)      263 2023-08-08 00:45:53.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/dropdown_group.py
--rw-r--r--   0 amo        (501) staff       (20)     2742 2023-08-08 00:45:53.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/extension.py
--rw-r--r--   0 amo        (501) staff       (20)     4960 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/gridtable.py
--rw-r--r--   0 amo        (501) staff       (20)     3751 2023-07-19 17:40:51.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/infocard.py
--rw-r--r--   0 amo        (501) staff       (20)     2006 2023-07-18 22:13:22.000000 sphinx-design-elements-0.2.1/sphinx_design_elements/tag.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-08 00:46:38.614570 sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     5285 2023-08-08 00:46:38.000000 sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     1102 2023-08-08 00:46:38.000000 sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-08-08 00:46:38.000000 sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)      300 2023-08-08 00:46:38.000000 sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       29 2023-08-08 00:46:38.000000 sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.184218 sphinx-design-elements-0.3.0/
+-rw-r--r--   0 amo        (501) staff       (20)      702 2024-04-06 16:25:38.000000 sphinx-design-elements-0.3.0/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.3.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      139 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.0/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     8082 2024-04-06 16:27:47.183787 sphinx-design-elements-0.3.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3069 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.164605 sphinx-design-elements-0.3.0/docs/
+-rw-r--r--   0 amo        (501) staff       (20)      772 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.0/docs/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)      702 2024-04-06 16:25:38.000000 sphinx-design-elements-0.3.0/docs/changes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.0/docs/css_classes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.0/docs/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx-design-elements-0.3.0/docs/get_started.md
+-rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.3.0/docs/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)    33174 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/hyper.md
+-rw-r--r--   0 amo        (501) staff       (20)     3835 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/index.md
+-rw-r--r--   0 amo        (501) staff       (20)     2145 2024-04-06 16:09:47.000000 sphinx-design-elements-0.3.0/docs/info.md
+-rw-r--r--   0 amo        (501) staff       (20)     2996 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/docs/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.3.0/docs/project.md
+-rw-r--r--   0 amo        (501) staff       (20)     3069 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/docs/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx-design-elements-0.3.0/docs/sandbox.md
+-rw-r--r--   0 amo        (501) staff       (20)    12371 2024-04-06 16:14:56.000000 sphinx-design-elements-0.3.0/docs/shield.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.165063 sphinx-design-elements-0.3.0/docs/snippets/
+-rw-r--r--   0 amo        (501) staff       (20)       73 2024-03-24 17:03:31.000000 sphinx-design-elements-0.3.0/docs/snippets/index.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.168316 sphinx-design-elements-0.3.0/docs/snippets/myst/
+-rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)      643 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/hyper.md
+-rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      177 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/shield.md
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.0/docs/snippets/myst/tag.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.171068 sphinx-design-elements-0.3.0/docs/snippets/rst/
+-rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/dropdown-group.rst
+-rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/gridtable.rst
+-rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/infocard.rst
+-rw-r--r--   0 amo        (501) staff       (20)      201 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/shield.rst
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.3.0/docs/snippets/rst/tag.rst
+-rw-r--r--   0 amo        (501) staff       (20)     2822 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/docs/tag.md
+-rw-r--r--   0 amo        (501) staff       (20)     5928 2024-04-06 16:24:49.000000 sphinx-design-elements-0.3.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-06 16:27:47.184304 sphinx-design-elements-0.3.0/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.176599 sphinx-design-elements-0.3.0/sphinx_design_elements/
+-rw-r--r--   0 amo        (501) staff       (20)      434 2024-03-07 23:44:18.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.179273 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      879 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/addon.js
+-rw-r--r--   0 amo        (501) staff       (20)     1431 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/style.css
+-rw-r--r--   0 amo        (501) staff       (20)      263 2023-08-08 00:45:53.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/dropdown_group.py
+-rw-r--r--   0 amo        (501) staff       (20)     2849 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/extension.py
+-rw-r--r--   0 amo        (501) staff       (20)     5218 2024-03-24 11:42:42.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/gridtable.py
+-rw-r--r--   0 amo        (501) staff       (20)    13371 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/hyper.py
+-rw-r--r--   0 amo        (501) staff       (20)     3751 2024-03-20 22:48:06.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/infocard.py
+-rw-r--r--   0 amo        (501) staff       (20)     4004 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/shield.py
+-rw-r--r--   0 amo        (501) staff       (20)     2006 2024-03-07 23:25:56.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/tag.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.180364 sphinx-design-elements-0.3.0/sphinx_design_elements/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4565 2024-04-06 16:12:43.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/util/directive.py
+-rw-r--r--   0 amo        (501) staff       (20)     4469 2024-04-06 16:14:54.000000 sphinx-design-elements-0.3.0/sphinx_design_elements/util/role.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-06 16:27:47.180961 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     8082 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     1412 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)      331 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       29 2024-04-06 16:27:47.000000 sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/top_level.txt
```

### Comparing `sphinx-design-elements-0.2.1/LICENSE` & `sphinx-design-elements-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/PKG-INFO` & `sphinx-design-elements-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.2.1
+Version: 0.3.0
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
@@ -25,62 +25,104 @@
         FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: changelog, https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md
 Project-URL: documentation, https://sphinx-design-elements.readthedocs.io/
 Project-URL: homepage, https://sphinx-design-elements.readthedocs.io/
 Project-URL: repository, https://github.com/panodata/sphinx-design-elements
-Keywords: extension,material design,sphinx,web components
+Keywords: authoring,badge,css,design,documentation,dropdown,extension,flexbox,grid,layout,markdown,material design,myst,responsive html,restructuredtext,shield,sphinx,sphinx design,table,tag,web components
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
+Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Documentation
+Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Education
+Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sphinx<7.2
+Requires-Dist: sphinx-design<1
 Provides-Extra: develop
+Requires-Dist: black<25; extra == "develop"
+Requires-Dist: mypy<1.10; extra == "develop"
+Requires-Dist: poethepoet<0.26; extra == "develop"
+Requires-Dist: pyproject-fmt<1.8; extra == "develop"
+Requires-Dist: ruff<0.4; extra == "develop"
+Requires-Dist: types-docutils==0.20.0.3; extra == "develop"
+Requires-Dist: validate-pyproject<0.17; extra == "develop"
 Provides-Extra: docs
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: myst-parser[linkify]<3,>=0.18; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
 Provides-Extra: release
+Requires-Dist: build<2; extra == "release"
+Requires-Dist: keyring; extra == "release"
+Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest<9; extra == "test"
+Requires-Dist: pytest-cov<6; extra == "test"
+Requires-Dist: pytest-regressions<3; extra == "test"
+Requires-Dist: sphinx_pytest<0.3; extra == "test"
 
 # sphinx-design-elements
 
 » [Documentation]
 | [Changelog]
 | [PyPI]
 | [Issues]
 | [Source code]
 | [License]
 
-[![CI][gha-badge]][gha-link]
-[![Coverage Status][codecov-badge]][codecov-link]
-[![PyPI][pypi-badge]][pypi-link]
+[![CI][badge-tests]][project-tests]
+[![Coverage Status][badge-coverage]][project-codecov]
+[![License][badge-license]][project-license]
+[![Downloads per month][badge-downloads-per-month]][project-downloads]
+
+[![Supported Python versions][badge-python-versions]][project-pypi]
+[![Status][badge-status]][project-pypi]
+[![Package version][badge-package-version]][project-pypi]
 
 
 ## About
 
-A collection of composite web elements based on components from [sphinx-design].
+A collection of composite and convenience web elements based on components
+from [sphinx-design].
 
 
 ## Setup
 
 Install the package using `pip install sphinx-design-elements`, and add the
 extension to the list of `extensions` within your Sphinx configuration file
 `conf.py`.
@@ -88,42 +130,51 @@
 ```python
 extensions = [
     "sphinx_design",
     "sphinx_design_elements",
 ]
 ```
 
-## Comparison to sphinx-design
+## Development
 
-This package uses low-level components of [sphinx-design], in order to build more
-high-level elements on top.
+In order to learn how to set up a development sandbox, please visit the
+[development documentation].
 
 
-## Development
+## Comparison to sphinx-design
+
+[sphinx-design-elements] uses low-level components of [sphinx-design],
+in order to build more high-level elements on top.
 
-In order to learn how to set up the project in development mode, please visit the
-[development documentation].
 
 ## Acknowledgements
 
-Kudos to [Chris Sewell] and all contributors for conceiving and maintaining
-[MyST Parser] and [sphinx-design].
+Kudos to [Chris Sewell], [Chris Holdgraf], and all contributors for conceiving
+and maintaining [MyST Parser] and [sphinx-design].
 
 
 
-[Changelog]: https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md
+[Changelog]: https://github.com/pyveci/sphinx-design-elements/blob/main/CHANGES.md
+[Chris Holdgraf]: https://github.com/choldgraf
 [Chris Sewell]: https://github.com/chrisjsewell
 [development documentation]: https://sphinx-design-elements.readthedocs.io/en/latest/sandbox.html
 [Documentation]: https://sphinx-design-elements.readthedocs.io/
-[Issues]: https://github.com/panodata/sphinx-design-elements/issues
-[License]: https://github.com/panodata/sphinx-design-elements/blob/main/LICENSE
+[Issues]: https://github.com/pyveci/sphinx-design-elements/issues
+[License]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
 [MyST Parser]: https://myst-parser.readthedocs.io/
 [PyPI]: https://pypi.org/project/sphinx-design-elements/
-[Source code]: https://github.com/panodata/sphinx-design-elements
+[Source code]: https://github.com/pyveci/sphinx-design-elements
 [sphinx-design]: https://sphinx-design.readthedocs.io/
+[sphinx-design-elements]: https://sphinx-design-elements.readthedocs.io/
 
-[gha-badge]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml/badge.svg
-[gha-link]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml
-[codecov-badge]: https://codecov.io/gh/panodata/sphinx-design-elements/branch/main/graph/badge.svg
-[codecov-link]: https://codecov.io/gh/panodata/sphinx-design-elements
-[pypi-badge]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
-[pypi-link]: https://pypi.org/project/sphinx-design-elements
+[badge-coverage]: https://codecov.io/gh/pyveci/sphinx-design-elements/branch/main/graph/badge.svg
+[badge-downloads-per-month]: https://pepy.tech/badge/sphinx-design-elements/month
+[badge-license]: https://img.shields.io/github/license/pyveci/sphinx-design-elements.svg
+[badge-package-version]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
+[badge-python-versions]: https://img.shields.io/pypi/pyversions/sphinx-design-elements.svg
+[badge-status]: https://img.shields.io/pypi/status/sphinx-design-elements.svg
+[badge-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml/badge.svg
+[project-codecov]: https://codecov.io/gh/pyveci/sphinx-design-elements
+[project-downloads]: https://pepy.tech/project/sphinx-design-elements/
+[project-license]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[project-pypi]: https://pypi.org/project/sphinx-design-elements
+[project-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml
```

### Comparing `sphinx-design-elements-0.2.1/README.md` & `sphinx-design-elements-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 » [Documentation]
 | [Changelog]
 | [PyPI]
 | [Issues]
 | [Source code]
 | [License]
 
-[![CI][gha-badge]][gha-link]
-[![Coverage Status][codecov-badge]][codecov-link]
-[![PyPI][pypi-badge]][pypi-link]
+[![CI][badge-tests]][project-tests]
+[![Coverage Status][badge-coverage]][project-codecov]
+[![License][badge-license]][project-license]
+[![Downloads per month][badge-downloads-per-month]][project-downloads]
+
+[![Supported Python versions][badge-python-versions]][project-pypi]
+[![Status][badge-status]][project-pypi]
+[![Package version][badge-package-version]][project-pypi]
 
 
 ## About
 
-A collection of composite web elements based on components from [sphinx-design].
+A collection of composite and convenience web elements based on components
+from [sphinx-design].
 
 
 ## Setup
 
 Install the package using `pip install sphinx-design-elements`, and add the
 extension to the list of `extensions` within your Sphinx configuration file
 `conf.py`.
@@ -26,42 +32,51 @@
 ```python
 extensions = [
     "sphinx_design",
     "sphinx_design_elements",
 ]
 ```
 
-## Comparison to sphinx-design
+## Development
 
-This package uses low-level components of [sphinx-design], in order to build more
-high-level elements on top.
+In order to learn how to set up a development sandbox, please visit the
+[development documentation].
 
 
-## Development
+## Comparison to sphinx-design
+
+[sphinx-design-elements] uses low-level components of [sphinx-design],
+in order to build more high-level elements on top.
 
-In order to learn how to set up the project in development mode, please visit the
-[development documentation].
 
 ## Acknowledgements
 
-Kudos to [Chris Sewell] and all contributors for conceiving and maintaining
-[MyST Parser] and [sphinx-design].
+Kudos to [Chris Sewell], [Chris Holdgraf], and all contributors for conceiving
+and maintaining [MyST Parser] and [sphinx-design].
 
 
 
-[Changelog]: https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md
+[Changelog]: https://github.com/pyveci/sphinx-design-elements/blob/main/CHANGES.md
+[Chris Holdgraf]: https://github.com/choldgraf
 [Chris Sewell]: https://github.com/chrisjsewell
 [development documentation]: https://sphinx-design-elements.readthedocs.io/en/latest/sandbox.html
 [Documentation]: https://sphinx-design-elements.readthedocs.io/
-[Issues]: https://github.com/panodata/sphinx-design-elements/issues
-[License]: https://github.com/panodata/sphinx-design-elements/blob/main/LICENSE
+[Issues]: https://github.com/pyveci/sphinx-design-elements/issues
+[License]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
 [MyST Parser]: https://myst-parser.readthedocs.io/
 [PyPI]: https://pypi.org/project/sphinx-design-elements/
-[Source code]: https://github.com/panodata/sphinx-design-elements
+[Source code]: https://github.com/pyveci/sphinx-design-elements
 [sphinx-design]: https://sphinx-design.readthedocs.io/
+[sphinx-design-elements]: https://sphinx-design-elements.readthedocs.io/
 
-[gha-badge]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml/badge.svg
-[gha-link]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml
-[codecov-badge]: https://codecov.io/gh/panodata/sphinx-design-elements/branch/main/graph/badge.svg
-[codecov-link]: https://codecov.io/gh/panodata/sphinx-design-elements
-[pypi-badge]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
-[pypi-link]: https://pypi.org/project/sphinx-design-elements
+[badge-coverage]: https://codecov.io/gh/pyveci/sphinx-design-elements/branch/main/graph/badge.svg
+[badge-downloads-per-month]: https://pepy.tech/badge/sphinx-design-elements/month
+[badge-license]: https://img.shields.io/github/license/pyveci/sphinx-design-elements.svg
+[badge-package-version]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
+[badge-python-versions]: https://img.shields.io/pypi/pyversions/sphinx-design-elements.svg
+[badge-status]: https://img.shields.io/pypi/status/sphinx-design-elements.svg
+[badge-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml/badge.svg
+[project-codecov]: https://codecov.io/gh/pyveci/sphinx-design-elements
+[project-downloads]: https://pepy.tech/project/sphinx-design-elements/
+[project-license]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[project-pypi]: https://pypi.org/project/sphinx-design-elements
+[project-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml
```

### Comparing `sphinx-design-elements-0.2.1/docs/css_classes.md` & `sphinx-design-elements-0.3.0/docs/css_classes.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/docs/dropdown-group.md` & `sphinx-design-elements-0.3.0/docs/dropdown-group.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/docs/get_started.md` & `sphinx-design-elements-0.3.0/docs/get_started.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/docs/gridtable.md` & `sphinx-design-elements-0.3.0/docs/gridtable.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/docs/index.md` & `sphinx-design-elements-0.3.0/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -69,20 +69,22 @@
 
 ```{toctree}
 :caption: Directives
 :hidden:
 
 gridtable
 infocard
+shield
 ```
 
 ```{toctree}
 :caption: Roles
 :hidden:
 
+hyper
 tag
 ```
 
 ```{toctree}
 :caption: Styling
 :hidden:
 
@@ -114,14 +116,28 @@
 :::{grid-item-card} {octicon}`note` Info card
 :link: infocard
 :link-type: doc
 
 Composite info card container element, to be used as a grid item.
 :::
 
+:::{grid-item-card} {octicon}`shield` Shield
+:link: shield
+:link-type: doc
+
+Badge generator for Shields\.io, with optional target linking.
+:::
+
+:::{grid-item-card} {octicon}`shield` Hyper
+:link: hyper
+:link-type: doc
+
+A versatile hyperlink generator.
+:::
+
 :::{grid-item-card} {octicon}`tag` Special badges
 :link: tag
 :link-type: doc
 
 Special {tags}`tag-like, badges` and other components.
 :::
```

### Comparing `sphinx-design-elements-0.2.1/docs/infocard.md` & `sphinx-design-elements-0.3.0/docs/infocard.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,17 @@
 ```
 ```{literalinclude} ./snippets/rst/infocard.rst
 :language: rst
 ```
 ````
 
 
-## More examples
+## Variants
+
+A few more variants how to change the visual appearance.
 
 :::::{info-card}
 
 ::::{grid-item}
 :columns: 8
 :class: sd-align-major-spaced
 #### Curated picture of the day
```

### Comparing `sphinx-design-elements-0.2.1/docs/readme.md` & `sphinx-design-elements-0.3.0/docs/readme.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 » [Documentation]
 | [Changelog]
 | [PyPI]
 | [Issues]
 | [Source code]
 | [License]
 
-[![CI][gha-badge]][gha-link]
-[![Coverage Status][codecov-badge]][codecov-link]
-[![PyPI][pypi-badge]][pypi-link]
+[![CI][badge-tests]][project-tests]
+[![Coverage Status][badge-coverage]][project-codecov]
+[![License][badge-license]][project-license]
+[![Downloads per month][badge-downloads-per-month]][project-downloads]
+
+[![Supported Python versions][badge-python-versions]][project-pypi]
+[![Status][badge-status]][project-pypi]
+[![Package version][badge-package-version]][project-pypi]
 
 
 ## About
 
-A collection of composite web elements based on components from [sphinx-design].
+A collection of composite and convenience web elements based on components
+from [sphinx-design].
 
 
 ## Setup
 
 Install the package using `pip install sphinx-design-elements`, and add the
 extension to the list of `extensions` within your Sphinx configuration file
 `conf.py`.
@@ -26,42 +32,51 @@
 ```python
 extensions = [
     "sphinx_design",
     "sphinx_design_elements",
 ]
 ```
 
-## Comparison to sphinx-design
+## Development
 
-This package uses low-level components of [sphinx-design], in order to build more
-high-level elements on top.
+In order to learn how to set up a development sandbox, please visit the
+[development documentation].
 
 
-## Development
+## Comparison to sphinx-design
+
+[sphinx-design-elements] uses low-level components of [sphinx-design],
+in order to build more high-level elements on top.
 
-In order to learn how to set up the project in development mode, please visit the
-[development documentation].
 
 ## Acknowledgements
 
-Kudos to [Chris Sewell] and all contributors for conceiving and maintaining
-[MyST Parser] and [sphinx-design].
+Kudos to [Chris Sewell], [Chris Holdgraf], and all contributors for conceiving
+and maintaining [MyST Parser] and [sphinx-design].
 
 
 
-[Changelog]: https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md
+[Changelog]: https://github.com/pyveci/sphinx-design-elements/blob/main/CHANGES.md
+[Chris Holdgraf]: https://github.com/choldgraf
 [Chris Sewell]: https://github.com/chrisjsewell
 [development documentation]: https://sphinx-design-elements.readthedocs.io/en/latest/sandbox.html
 [Documentation]: https://sphinx-design-elements.readthedocs.io/
-[Issues]: https://github.com/panodata/sphinx-design-elements/issues
-[License]: https://github.com/panodata/sphinx-design-elements/blob/main/LICENSE
+[Issues]: https://github.com/pyveci/sphinx-design-elements/issues
+[License]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
 [MyST Parser]: https://myst-parser.readthedocs.io/
 [PyPI]: https://pypi.org/project/sphinx-design-elements/
-[Source code]: https://github.com/panodata/sphinx-design-elements
+[Source code]: https://github.com/pyveci/sphinx-design-elements
 [sphinx-design]: https://sphinx-design.readthedocs.io/
+[sphinx-design-elements]: https://sphinx-design-elements.readthedocs.io/
 
-[gha-badge]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml/badge.svg
-[gha-link]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml
-[codecov-badge]: https://codecov.io/gh/panodata/sphinx-design-elements/branch/main/graph/badge.svg
-[codecov-link]: https://codecov.io/gh/panodata/sphinx-design-elements
-[pypi-badge]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
-[pypi-link]: https://pypi.org/project/sphinx-design-elements
+[badge-coverage]: https://codecov.io/gh/pyveci/sphinx-design-elements/branch/main/graph/badge.svg
+[badge-downloads-per-month]: https://pepy.tech/badge/sphinx-design-elements/month
+[badge-license]: https://img.shields.io/github/license/pyveci/sphinx-design-elements.svg
+[badge-package-version]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
+[badge-python-versions]: https://img.shields.io/pypi/pyversions/sphinx-design-elements.svg
+[badge-status]: https://img.shields.io/pypi/status/sphinx-design-elements.svg
+[badge-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml/badge.svg
+[project-codecov]: https://codecov.io/gh/pyveci/sphinx-design-elements
+[project-downloads]: https://pepy.tech/project/sphinx-design-elements/
+[project-license]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[project-pypi]: https://pypi.org/project/sphinx-design-elements
+[project-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml
```

### Comparing `sphinx-design-elements-0.2.1/docs/sandbox.md` & `sphinx-design-elements-0.3.0/docs/sandbox.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/docs/snippets/rst/infocard.rst` & `sphinx-design-elements-0.3.0/docs/snippets/rst/infocard.rst`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/docs/tag.md` & `sphinx-design-elements-0.3.0/docs/tag.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 (tag-role)=
 
-# `tag(s)` role
+# Tag
 
 
 ## About
 
 The `tag` and `tags` roles are shortcuts to the `bdg` badge roles of
 [sphinx{design}](inv:sd#index), see [](inv:sd#badges).
```

### Comparing `sphinx-design-elements-0.2.1/pyproject.toml` & `sphinx-design-elements-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -10,79 +10,114 @@
 default-tag = "0.0.0"
 
 [project]
 name = "sphinx-design-elements"
 description = "A collection of composite web elements based on components from sphinx-design."
 readme = "README.md"
 keywords = [
+  "authoring",
+  "badge",
+  "css",
+  "design",
+  "documentation",
+  "dropdown",
   "extension",
+  "flexbox",
+  "grid",
+  "layout",
+  "markdown",
   "material design",
+  "myst",
+  "responsive html",
+  "restructuredtext",
+  "shield",
   "sphinx",
+  "sphinx design",
+  "table",
+  "tag",
   "web components",
 ]
 license = { file = "LICENSE" }
 authors = [
   { name = "Andreas Motl", email = "andreas.motl@panodata.org" },
 ]
 requires-python = ">=3.7"
 classifiers = [
   "Development Status :: 4 - Beta",
+  "Environment :: Plugins",
+  "Environment :: Web Environment",
+  "Framework :: Sphinx",
   "Framework :: Sphinx :: Extension",
+  "Intended Audience :: Customer Service",
   "Intended Audience :: Developers",
   "Intended Audience :: Education",
+  "Intended Audience :: End Users/Desktop",
+  "Intended Audience :: Information Technology",
+  "Intended Audience :: Manufacturing",
   "Intended Audience :: Science/Research",
+  "Intended Audience :: System Administrators",
+  "Intended Audience :: Telecommunications Industry",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Documentation",
+  "Topic :: Documentation :: Sphinx",
   "Topic :: Education",
+  "Topic :: File Formats",
   "Topic :: Scientific/Engineering",
+  "Topic :: Software Development :: Bug Tracking",
+  "Topic :: Software Development :: Code Generators",
+  "Topic :: Software Development :: Documentation",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Widget Sets",
   "Topic :: Text Processing",
   "Topic :: Text Processing :: Markup",
   "Topic :: Text Processing :: Markup :: HTML",
   "Topic :: Text Processing :: Markup :: Markdown",
   "Topic :: Text Processing :: Markup :: reStructuredText",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
+  "sphinx<7.2",
   "sphinx-design<1",
 ]
 [project.optional-dependencies]
 develop = [
-  "black<24",
-  "docutils-stubs",
-  "mypy==1.4.1",
-  "poethepoet<0.22",
-  "pyproject-fmt<0.14",
-  "ruff==0.0.282",
-  "validate-pyproject<0.14",
+  "black<25",
+  "mypy<1.10",
+  "poethepoet<0.26",
+  "pyproject-fmt<1.8",
+  "ruff<0.4",
+  "types-docutils==0.20.0.3",
+  "validate-pyproject<0.17",
 ]
 docs = [
   "furo",
   "myst-parser[linkify]<3,>=0.18",
   "sphinx-autobuild",
   "sphinx-copybutton",
 ]
 release = [
-  "build<1",
+  "build<2",
   "keyring",
-  "twine<5",
+  "twine<6",
 ]
 test = [
-  "pytest<8",
-  "pytest-cov<5",
+  "pytest<9",
+  "pytest-cov<6",
   "pytest-regressions<3",
+  "sphinx_pytest<0.3",
 ]
 [project.urls]
 changelog = "https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md"
 documentation = "https://sphinx-design-elements.readthedocs.io/"
 homepage = "https://sphinx-design-elements.readthedocs.io/"
 repository = "https://github.com/panodata/sphinx-design-elements"
 
@@ -101,15 +136,14 @@
 show_missing = true
 
 [tool.mypy]
 packages = ["sphinx_design_elements"]
 exclude = [
 ]
 check_untyped_defs = true
-#ignore_missing_imports = true
 implicit_optional = true
 install_types = true
 no_implicit_optional = true
 non_interactive = true
 show_error_codes = true
 strict_equality = true
 warn_unused_ignores = true
@@ -132,15 +166,15 @@
 xfail_strict = true
 markers = [
 ]
 
 [tool.ruff]
 line-length = 120
 
-select = [
+lint.select = [
   # Bandit
   "S",
   # Bugbear
   "B",
   # Builtins
   "A",
   # comprehensions
@@ -160,27 +194,27 @@
   "W",
   # Pyflakes
   "F",
   # return
   "RET",
 ]
 
-extend-ignore = [
+lint.extend-ignore = [
   # zip() without an explicit strict= parameter
   "B905",
   # df is a bad variable name. Be kinder to your future self.
   "PD901",
   # Unnecessary variable assignment before `return` statement
   "RET504",
   # Unnecessary `elif` after `return` statement
   "RET505",
 ]
 
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101"]  # Allow use of `assert`, and `print`.
 "docs/conf.py" = ["ERA001"]  # Allow commented-out code (ERA001).
 
 [tool.setuptools.packages.find]
 namespaces = false
 
 
@@ -195,27 +229,27 @@
   "test",
 ]
 
 docs-autobuild = [
   { cmd = "sphinx-autobuild --open-browser --watch sphinx_design_elements docs docs/_build" }
 ]
 docs-html = [
-  { cmd = "sphinx-build docs docs/_build" }
+  { cmd = "sphinx-build -W --keep-going docs docs/_build" }
 ]
 
 format = [
   { cmd = "black ." },
   # Configure Ruff not to auto-fix (remove!):
   # unused imports (F401), unused variables (F841), `print` statements (T201), and commented-out code (ERA001).
-  { cmd = "ruff --fix --ignore=ERA --ignore=F401 --ignore=F841 --ignore=T20 --ignore=ERA001 ." },
-  { cmd = "pyproject-fmt pyproject.toml" },
+  { cmd = "ruff check --fix --ignore=ERA --ignore=F401 --ignore=F841 --ignore=T20 --ignore=ERA001 ." },
+  { cmd = "pyproject-fmt --keep-full-version pyproject.toml" },
 ]
 
 lint = [
-  { cmd = "ruff ." },
+  { cmd = "ruff check ." },
   { cmd = "black --check ." },
   { cmd = "validate-pyproject pyproject.toml" },
   { cmd = "mypy" },
 ]
 
 release = [
   { cmd = "python -m build" },
```

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements/compiled/addon.js` & `sphinx-design-elements-0.3.0/sphinx_design_elements/compiled/addon.js`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements/extension.py` & `sphinx-design-elements-0.3.0/sphinx_design_elements/extension.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx_design.extension import depart_container, visit_container
 
 from . import compiled as static_module
 from .dropdown_group import setup_dropdown_group
 from .gridtable import setup_gridtable
+from .hyper import setup_hyper
 from .infocard import setup_infocard
+from .shield import setup_shield
 from .tag import setup_tags
 
 
 def setup_extension(app: Sphinx) -> None:
     """
     Set up the sphinx extension.
     """
@@ -22,18 +24,20 @@
     app.connect("builder-inited", add_assets)
     app.connect("env-updated", update_asset_links)
 
     # Override container html visitors, to stop the default behaviour
     # of adding the `container` class to all `nodes.container`.
     app.add_node(nodes.container, override=True, html=(visit_container, depart_container))
 
+    setup_dropdown_group(app)
     setup_gridtable(app)
+    setup_hyper(app)
     setup_infocard(app)
+    setup_shield(app)
     setup_tags(app)
-    setup_dropdown_group(app)
 
 
 def add_assets(app: Sphinx):
     """
     Copy JS and CSS assets to the build directory.
     """
```

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements/gridtable.py` & `sphinx-design-elements-0.3.0/sphinx_design_elements/gridtable.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,19 +42,19 @@
     the maintenance nightmares of tables.
     """
 
     has_content = True
     required_arguments = 0
     optional_arguments = 1
     option_spec = {
-        "widths": widths_option,
+        "item-outline": directives.flag,
         "outline": directives.flag,
         "row-class": directives.class_option,
         "row-outline": directives.flag,
-        "item-outline": directives.flag,
+        "widths": widths_option,
     }
 
     def run(self) -> List[nodes.Node]:
         self.state_machine.document.attributes["widths"] = self.options.get("widths", [])
         self.state_machine.document.attributes["row-class"] = self.options.get("row-class", [])
         if "row-outline" in self.options:
             self.state_machine.document.attributes["row-outline"] = None
@@ -116,15 +116,21 @@
     The "item" (cell) element of the `TableDirective`.
 
     It is intended to be used nested within a `RowDirective`.
     """
 
     has_content = True
     option_spec = {
+        "child-align": directives.unchanged,
+        "child-direction": directives.unchanged,
+        "class": directives.class_option,
+        "columns": directives.unchanged,
+        "margin": directives.unchanged,
         "outline": directives.flag,
+        "padding": directives.unchanged,
     }
 
     def run(self) -> List[nodes.Node]:
         if "item-outline" in self.state_machine.document.attributes:
             self.options["outline"] = None
 
         column = create_component(
```

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements/infocard.py` & `sphinx-design-elements-0.3.0/sphinx_design_elements/infocard.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements/tag.py` & `sphinx-design-elements-0.3.0/sphinx_design_elements/tag.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/PKG-INFO` & `sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.2.1
+Version: 0.3.0
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
@@ -25,62 +25,104 @@
         FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: changelog, https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md
 Project-URL: documentation, https://sphinx-design-elements.readthedocs.io/
 Project-URL: homepage, https://sphinx-design-elements.readthedocs.io/
 Project-URL: repository, https://github.com/panodata/sphinx-design-elements
-Keywords: extension,material design,sphinx,web components
+Keywords: authoring,badge,css,design,documentation,dropdown,extension,flexbox,grid,layout,markdown,material design,myst,responsive html,restructuredtext,shield,sphinx,sphinx design,table,tag,web components
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
+Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Documentation
+Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Education
+Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sphinx<7.2
+Requires-Dist: sphinx-design<1
 Provides-Extra: develop
+Requires-Dist: black<25; extra == "develop"
+Requires-Dist: mypy<1.10; extra == "develop"
+Requires-Dist: poethepoet<0.26; extra == "develop"
+Requires-Dist: pyproject-fmt<1.8; extra == "develop"
+Requires-Dist: ruff<0.4; extra == "develop"
+Requires-Dist: types-docutils==0.20.0.3; extra == "develop"
+Requires-Dist: validate-pyproject<0.17; extra == "develop"
 Provides-Extra: docs
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: myst-parser[linkify]<3,>=0.18; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
 Provides-Extra: release
+Requires-Dist: build<2; extra == "release"
+Requires-Dist: keyring; extra == "release"
+Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest<9; extra == "test"
+Requires-Dist: pytest-cov<6; extra == "test"
+Requires-Dist: pytest-regressions<3; extra == "test"
+Requires-Dist: sphinx_pytest<0.3; extra == "test"
 
 # sphinx-design-elements
 
 » [Documentation]
 | [Changelog]
 | [PyPI]
 | [Issues]
 | [Source code]
 | [License]
 
-[![CI][gha-badge]][gha-link]
-[![Coverage Status][codecov-badge]][codecov-link]
-[![PyPI][pypi-badge]][pypi-link]
+[![CI][badge-tests]][project-tests]
+[![Coverage Status][badge-coverage]][project-codecov]
+[![License][badge-license]][project-license]
+[![Downloads per month][badge-downloads-per-month]][project-downloads]
+
+[![Supported Python versions][badge-python-versions]][project-pypi]
+[![Status][badge-status]][project-pypi]
+[![Package version][badge-package-version]][project-pypi]
 
 
 ## About
 
-A collection of composite web elements based on components from [sphinx-design].
+A collection of composite and convenience web elements based on components
+from [sphinx-design].
 
 
 ## Setup
 
 Install the package using `pip install sphinx-design-elements`, and add the
 extension to the list of `extensions` within your Sphinx configuration file
 `conf.py`.
@@ -88,42 +130,51 @@
 ```python
 extensions = [
     "sphinx_design",
     "sphinx_design_elements",
 ]
 ```
 
-## Comparison to sphinx-design
+## Development
 
-This package uses low-level components of [sphinx-design], in order to build more
-high-level elements on top.
+In order to learn how to set up a development sandbox, please visit the
+[development documentation].
 
 
-## Development
+## Comparison to sphinx-design
+
+[sphinx-design-elements] uses low-level components of [sphinx-design],
+in order to build more high-level elements on top.
 
-In order to learn how to set up the project in development mode, please visit the
-[development documentation].
 
 ## Acknowledgements
 
-Kudos to [Chris Sewell] and all contributors for conceiving and maintaining
-[MyST Parser] and [sphinx-design].
+Kudos to [Chris Sewell], [Chris Holdgraf], and all contributors for conceiving
+and maintaining [MyST Parser] and [sphinx-design].
 
 
 
-[Changelog]: https://github.com/panodata/sphinx-design-elements/blob/main/CHANGES.md
+[Changelog]: https://github.com/pyveci/sphinx-design-elements/blob/main/CHANGES.md
+[Chris Holdgraf]: https://github.com/choldgraf
 [Chris Sewell]: https://github.com/chrisjsewell
 [development documentation]: https://sphinx-design-elements.readthedocs.io/en/latest/sandbox.html
 [Documentation]: https://sphinx-design-elements.readthedocs.io/
-[Issues]: https://github.com/panodata/sphinx-design-elements/issues
-[License]: https://github.com/panodata/sphinx-design-elements/blob/main/LICENSE
+[Issues]: https://github.com/pyveci/sphinx-design-elements/issues
+[License]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
 [MyST Parser]: https://myst-parser.readthedocs.io/
 [PyPI]: https://pypi.org/project/sphinx-design-elements/
-[Source code]: https://github.com/panodata/sphinx-design-elements
+[Source code]: https://github.com/pyveci/sphinx-design-elements
 [sphinx-design]: https://sphinx-design.readthedocs.io/
+[sphinx-design-elements]: https://sphinx-design-elements.readthedocs.io/
 
-[gha-badge]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml/badge.svg
-[gha-link]: https://github.com/panodata/sphinx-design-elements/actions/workflows/main.yml
-[codecov-badge]: https://codecov.io/gh/panodata/sphinx-design-elements/branch/main/graph/badge.svg
-[codecov-link]: https://codecov.io/gh/panodata/sphinx-design-elements
-[pypi-badge]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
-[pypi-link]: https://pypi.org/project/sphinx-design-elements
+[badge-coverage]: https://codecov.io/gh/pyveci/sphinx-design-elements/branch/main/graph/badge.svg
+[badge-downloads-per-month]: https://pepy.tech/badge/sphinx-design-elements/month
+[badge-license]: https://img.shields.io/github/license/pyveci/sphinx-design-elements.svg
+[badge-package-version]: https://img.shields.io/pypi/v/sphinx-design-elements.svg
+[badge-python-versions]: https://img.shields.io/pypi/pyversions/sphinx-design-elements.svg
+[badge-status]: https://img.shields.io/pypi/status/sphinx-design-elements.svg
+[badge-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml/badge.svg
+[project-codecov]: https://codecov.io/gh/pyveci/sphinx-design-elements
+[project-downloads]: https://pepy.tech/project/sphinx-design-elements/
+[project-license]: https://github.com/pyveci/sphinx-design-elements/blob/main/LICENSE
+[project-pypi]: https://pypi.org/project/sphinx-design-elements
+[project-tests]: https://github.com/pyveci/sphinx-design-elements/actions/workflows/main.yml
```

### Comparing `sphinx-design-elements-0.2.1/sphinx_design_elements.egg-info/SOURCES.txt` & `sphinx-design-elements-0.3.0/sphinx_design_elements.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,36 +5,47 @@
 pyproject.toml
 docs/backlog.md
 docs/changes.md
 docs/css_classes.md
 docs/dropdown-group.md
 docs/get_started.md
 docs/gridtable.md
+docs/hyper.md
 docs/index.md
+docs/info.md
 docs/infocard.md
 docs/project.md
 docs/readme.md
 docs/sandbox.md
+docs/shield.md
 docs/tag.md
 docs/snippets/index.md
 docs/snippets/myst/dropdown-group.md
 docs/snippets/myst/gridtable.md
+docs/snippets/myst/hyper.md
 docs/snippets/myst/infocard.md
+docs/snippets/myst/shield.md
 docs/snippets/myst/tag.md
 docs/snippets/rst/dropdown-group.rst
 docs/snippets/rst/gridtable.rst
 docs/snippets/rst/infocard.rst
+docs/snippets/rst/shield.rst
 docs/snippets/rst/tag.rst
 sphinx_design_elements/__init__.py
 sphinx_design_elements/dropdown_group.py
 sphinx_design_elements/extension.py
 sphinx_design_elements/gridtable.py
+sphinx_design_elements/hyper.py
 sphinx_design_elements/infocard.py
+sphinx_design_elements/shield.py
 sphinx_design_elements/tag.py
 sphinx_design_elements.egg-info/PKG-INFO
 sphinx_design_elements.egg-info/SOURCES.txt
 sphinx_design_elements.egg-info/dependency_links.txt
 sphinx_design_elements.egg-info/requires.txt
 sphinx_design_elements.egg-info/top_level.txt
 sphinx_design_elements/compiled/__init__.py
 sphinx_design_elements/compiled/addon.js
-sphinx_design_elements/compiled/style.css
+sphinx_design_elements/compiled/style.css
+sphinx_design_elements/util/__init__.py
+sphinx_design_elements/util/directive.py
+sphinx_design_elements/util/role.py
```

