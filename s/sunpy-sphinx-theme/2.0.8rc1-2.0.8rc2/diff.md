# Comparing `tmp/sunpy-sphinx-theme-2.0.8rc1.tar.gz` & `tmp/sunpy-sphinx-theme-2.0.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunpy-sphinx-theme-2.0.8rc1.tar", last modified: Sat Apr  6 14:08:46 2024, max compression
+gzip compressed data, was "sunpy-sphinx-theme-2.0.8rc2.tar", last modified: Sat Apr  6 20:02:53 2024, max compression
```

## Comparing `sunpy-sphinx-theme-2.0.8rc1.tar` & `sunpy-sphinx-theme-2.0.8rc2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.620936 sunpy-sphinx-theme-2.0.8rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/.rtd-environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/.stylelintrc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 14:08:46.620936 sunpy-sphinx-theme-2.0.8rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 14:08:46.620936 sunpy-sphinx-theme-2.0.8rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.612936 sunpy-sphinx-theme-2.0.8rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.612936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/footer-links.html
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   187674 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-06 14:08:35.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:08:46.616936 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 14:08:46.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-06 14:08:46.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:08:46.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 14:08:46.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 14:08:46.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 14:08:46.000000 sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.689839 sunpy-sphinx-theme-2.0.8rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/.stylelintrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 20:02:53.689839 sunpy-sphinx-theme-2.0.8rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 20:02:53.689839 sunpy-sphinx-theme-2.0.8rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.681840 sunpy-sphinx-theme-2.0.8rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.681840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.681840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/footer-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   187674 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-06 20:02:42.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:02:53.685840 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 20:02:53.000000 sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/top_level.txt
```

### Comparing `sunpy-sphinx-theme-2.0.8rc1/LICENSE.md` & `sunpy-sphinx-theme-2.0.8rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/PKG-INFO` & `sunpy-sphinx-theme-2.0.8rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-sphinx-theme
-Version: 2.0.8rc1
+Version: 2.0.8rc2
 Summary: The sphinx theme for the SunPy website and documentation.
 Author: The SunPy Developers
 License: BSD 2-Clause License
         
         Copyright (c) 2018-2023, The SunPy Developers
         All rights reserved.
```

### Comparing `sunpy-sphinx-theme-2.0.8rc1/README.md` & `sunpy-sphinx-theme-2.0.8rc2/README.md`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/pyproject.toml` & `sunpy-sphinx-theme-2.0.8rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/__init__.py` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,28 +138,32 @@
     app.add_css_file("sunpy_style.css", priority=600)
 
     app.connect("builder-inited", update_config)
     app.connect("html-page-context", update_html_context)
 
     # Conditionally include goat counter js
     # We can't do this in update_config as that causes the scripts to be duplicated.
+    # Also in here none of the theme defaults have be applied by `update_config`
+    # TODO: Improve this mess
     theme_options = utils.get_theme_options_dict(app)
-    if theme_options.get("goatcounter_analytics_url"):
-        root_domain = (
-            theme_options.get("sst_site_root", "https://sunpy.org").removeprefix("https://").removeprefix("http://")
-        )
+    # We want to default to the sunpy goat counter only if the sst_site_root is sunpy.org
+    root_domain = theme_options.get("sst_site_root", "https://sunpy.org")
+    sunpy_goat_url = "https://sunpy.goatcounter.com/count"
+    default_goat_url = sunpy_goat_url if root_domain == "https://sunpy.org" else None
+    if primary_goat_url := theme_options.get("goatcounter_analytics_url", default_goat_url):
+        root_domain = root_domain.removeprefix("https://").removeprefix("http://")
         default_endpoint = theme_options.get("goatcounter_non_domain_endpoint", False)
         if default_endpoint is False:
             default_endpoint = ""
         app.add_js_file(
             None,
             body=f"""
             var endpoint = '{default_endpoint}';
             if (location.hostname.endsWith('{root_domain}')) {{
-                endpoint = '{theme_options["goatcounter_analytics_url"]}'
+                endpoint = '{primary_goat_url}'
             }}
 
             window.goatcounter = {{
                 endpoint: endpoint,
                 path: function(p) {{ return location.host + p }}
             }}
             """,
```

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/conf.py` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/conf.py`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/built-with.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar-logo.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_center.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/navbar_start.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/components/sst-sidebar-nav.html`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/favicon-32.ico`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/numfocus-logo.svg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy-bg.jpg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon.svg`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/img/sunpy_icon_128x128.png`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/static/sunpy_style.css`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme/theme/sunpy/theme.conf` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme/theme/sunpy/theme.conf`

 * *Files identical despite different names*

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/PKG-INFO` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpy-sphinx-theme
-Version: 2.0.8rc1
+Version: 2.0.8rc2
 Summary: The sphinx theme for the SunPy website and documentation.
 Author: The SunPy Developers
 License: BSD 2-Clause License
         
         Copyright (c) 2018-2023, The SunPy Developers
         All rights reserved.
```

### Comparing `sunpy-sphinx-theme-2.0.8rc1/src/sunpy_sphinx_theme.egg-info/SOURCES.txt` & `sunpy-sphinx-theme-2.0.8rc2/src/sunpy_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

