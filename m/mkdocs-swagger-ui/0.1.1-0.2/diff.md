# Comparing `tmp/mkdocs-swagger-ui-0.1.1.tar.gz` & `tmp/mkdocs-swagger-ui-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-swagger-ui-0.1.1.tar", last modified: Wed Feb 28 21:24:36 2024, max compression
+gzip compressed data, was "mkdocs-swagger-ui-0.2.tar", last modified: Fri Apr  5 22:02:59 2024, max compression
```

## Comparing `mkdocs-swagger-ui-0.1.1.tar` & `mkdocs-swagger-ui-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-02-28 21:24:36.423142 mkdocs-swagger-ui-0.1.1/
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1068 2024-02-28 21:15:53.000000 mkdocs-swagger-ui-0.1.1/LICENSE
--rw-r--r--   0 byrne.reese   (502) staff       (20)     3148 2024-02-28 21:24:36.423012 mkdocs-swagger-ui-0.1.1/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)     2202 2024-02-28 21:15:53.000000 mkdocs-swagger-ui-0.1.1/README.md
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-02-28 21:24:36.422644 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/
--rw-r--r--   0 byrne.reese   (502) staff       (20)     3148 2024-02-28 21:24:36.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)      346 2024-02-28 21:24:36.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/SOURCES.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2024-02-28 21:24:36.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/dependency_links.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       78 2024-02-28 21:24:36.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/entry_points.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       37 2024-02-28 21:24:36.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/requires.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       25 2024-02-28 21:24:36.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/top_level.txt
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-02-28 21:24:36.422846 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui_plugin/
--rw-r--r--   0 byrne.reese   (502) staff       (20)        0 2024-02-28 21:15:53.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui_plugin/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     2355 2024-02-28 21:22:46.000000 mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui_plugin/plugin.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)       38 2024-02-28 21:24:36.423179 mkdocs-swagger-ui-0.1.1/setup.cfg
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1436 2024-02-28 21:23:56.000000 mkdocs-swagger-ui-0.1.1/setup.py
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-04-05 22:02:59.990405 mkdocs-swagger-ui-0.2/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     1068 2024-02-28 21:15:53.000000 mkdocs-swagger-ui-0.2/LICENSE
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     3146 2024-04-05 22:02:59.990278 mkdocs-swagger-ui-0.2/PKG-INFO
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     2202 2024-02-28 21:15:53.000000 mkdocs-swagger-ui-0.2/README.md
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-04-05 22:02:59.989841 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     3146 2024-04-05 22:02:59.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/PKG-INFO
+-rw-r--r--   0 byrne.reese   (502) staff       (20)      346 2024-04-05 22:02:59.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2024-04-05 22:02:59.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       78 2024-04-05 22:02:59.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/entry_points.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       37 2024-04-05 22:02:59.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/requires.txt
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       25 2024-04-05 22:02:59.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/top_level.txt
+drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-04-05 22:02:59.990095 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui_plugin/
+-rw-r--r--   0 byrne.reese   (502) staff       (20)        0 2024-02-28 21:15:53.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui_plugin/__init__.py
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     2525 2024-04-05 21:53:56.000000 mkdocs-swagger-ui-0.2/mkdocs_swagger_ui_plugin/plugin.py
+-rw-r--r--   0 byrne.reese   (502) staff       (20)       38 2024-04-05 22:02:59.990449 mkdocs-swagger-ui-0.2/setup.cfg
+-rw-r--r--   0 byrne.reese   (502) staff       (20)     1434 2024-04-05 21:57:55.000000 mkdocs-swagger-ui-0.2/setup.py
```

### Comparing `mkdocs-swagger-ui-0.1.1/LICENSE` & `mkdocs-swagger-ui-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-swagger-ui-0.1.1/PKG-INFO` & `mkdocs-swagger-ui-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-swagger-ui
-Version: 0.1.1
+Version: 0.2
 Summary: An MkDocs plugin to generate a markdown file containing an API reference built using Swagger UI from a base OAS3 specification.
 Home-page: https://github.com/byrnereese/mkdocs-swagger-ui
 Author: Byrne Reese
 Author-email: byrne@majordojo.com
 License: MIT
 Keywords: mkdocs swagger api documentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-swagger-ui-0.1.1/README.md` & `mkdocs-swagger-ui-0.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui.egg-info/PKG-INFO` & `mkdocs-swagger-ui-0.2/mkdocs_swagger_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-swagger-ui
-Version: 0.1.1
+Version: 0.2
 Summary: An MkDocs plugin to generate a markdown file containing an API reference built using Swagger UI from a base OAS3 specification.
 Home-page: https://github.com/byrnereese/mkdocs-swagger-ui
 Author: Byrne Reese
 Author-email: byrne@majordojo.com
 License: MIT
 Keywords: mkdocs swagger api documentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-swagger-ui-0.1.1/mkdocs_swagger_ui_plugin/plugin.py` & `mkdocs-swagger-ui-0.2/mkdocs_swagger_ui_plugin/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,25 +32,28 @@
     def __init__(self):
         self.enabled = True
         self.total_time = 0
 
     def generate_page_contents(self):
         spec_url    = self.config['spec_url']
         tmpl_url    = self.config['template']
+        cur_dir     = os.path.dirname(__file__)
         print("INFO     -  Generating swagger-ui for spec: " + spec_url)
         print("DEBUG    -  template: " + tmpl_url)
+        print("DEBUG    -  directory: " + cur_dir)
         env = Environment(
-            loader=FileSystemLoader('tmpl'),
+            loader=FileSystemLoader(['tmpl',os.path.join(cur_dir,'tmpl')]),
             autoescape=select_autoescape(['html', 'xml'])
         )
         md = markdown.Markdown()
         env.filters['markdown'] = lambda text: Markup(md.convert(text))
   
         template = env.get_template( tmpl_url )
         tmpl_out = template.render( spec=spec_url )
+        print("DEBUG    - " + tmpl_out)
         return tmpl_out
     
     def on_config(self, config):
         print("INFO     -  swagger-ui plugin ENABLED")
 
     def on_page_read_source(self, page, config):
         index_path = os.path.join(config['docs_dir'], self.config['outfile'])
```

### Comparing `mkdocs-swagger-ui-0.1.1/setup.py` & `mkdocs-swagger-ui-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mkdocs-swagger-ui',
-    version='0.1.1',
+    version='0.2',
     description='An MkDocs plugin to generate a markdown file containing an API reference built using Swagger UI from a base OAS3 specification.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='mkdocs swagger api documentation',
     url='https://github.com/byrnereese/mkdocs-swagger-ui',
     author='Byrne Reese',
     author_email='byrne@majordojo.com',
```

