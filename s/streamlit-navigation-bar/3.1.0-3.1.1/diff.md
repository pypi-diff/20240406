# Comparing `tmp/streamlit-navigation-bar-3.1.0.tar.gz` & `tmp/streamlit-navigation-bar-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-navigation-bar-3.1.0.tar", last modified: Sat Apr  6 14:38:44 2024, max compression
+gzip compressed data, was "streamlit-navigation-bar-3.1.1.tar", last modified: Sat Apr  6 16:45:11 2024, max compression
```

## Comparing `streamlit-navigation-bar-3.1.0.tar` & `streamlit-navigation-bar-3.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.297266 streamlit-navigation-bar-3.1.0/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.1.0/LICENSE
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.1.0/MANIFEST.in
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13454 2024-04-06 14:38:44.296967 streamlit-navigation-bar-3.1.0/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    12937 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.0/README.md
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-06 14:38:44.297322 streamlit-navigation-bar-3.1.0/setup.cfg
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1024 2024-04-06 14:35:00.000000 streamlit-navigation-bar-3.1.0/setup.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.294396 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    17097 2024-04-06 14:38:25.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/__init__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8452 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/errors.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/example.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.292319 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.295588 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.296690 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/index.html
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/match_navbar.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.295432 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13454 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/requires.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/top_level.txt
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.630179 streamlit-navigation-bar-3.1.1/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.1.1/LICENSE
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.1.1/MANIFEST.in
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13521 2024-04-06 16:45:11.630022 streamlit-navigation-bar-3.1.1/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13004 2024-04-06 16:17:40.000000 streamlit-navigation-bar-3.1.1/README.md
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-06 16:45:11.630222 streamlit-navigation-bar-3.1.1/setup.cfg
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1024 2024-04-06 16:42:42.000000 streamlit-navigation-bar-3.1.1/setup.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.627717 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    17101 2024-04-06 16:44:33.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/__init__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8452 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/errors.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/example.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.625796 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.628676 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.629751 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/index.html
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/match_navbar.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.628546 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13521 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/requires.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/top_level.txt
```

### Comparing `streamlit-navigation-bar-3.1.0/LICENSE` & `streamlit-navigation-bar-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/PKG-INFO` & `streamlit-navigation-bar-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.1.0
+Version: 3.1.1
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -304,21 +304,25 @@
     "active": {
         "color": "var(--text-color)",
         "background-color": "white",
         "font-weight": "normal",
         "padding": "14px",
     }
 }
+options = {
+    "show_menu": False,
+    "show_sidebar": False,
+}
 
 page = st_navbar(
     pages,
     logo_path=logo_path,
     urls=urls,
     styles=styles,
-    options=False,
+    options=options,
 )
 
 functions = {
     "Home": pg.show_home,
     "Install": pg.show_install,
     "User Guide": pg.show_user_guide,
     "API": pg.show_api,
```

### Comparing `streamlit-navigation-bar-3.1.0/README.md` & `streamlit-navigation-bar-3.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -289,21 +289,25 @@
     "active": {
         "color": "var(--text-color)",
         "background-color": "white",
         "font-weight": "normal",
         "padding": "14px",
     }
 }
+options = {
+    "show_menu": False,
+    "show_sidebar": False,
+}
 
 page = st_navbar(
     pages,
     logo_path=logo_path,
     urls=urls,
     styles=styles,
-    options=False,
+    options=options,
 )
 
 functions = {
     "Home": pg.show_home,
     "Install": pg.show_install,
     "User Guide": pg.show_user_guide,
     "API": pg.show_api,
```

### Comparing `streamlit-navigation-bar-3.1.0/setup.py` & `streamlit-navigation-bar-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="streamlit-navigation-bar",
-    version="3.1.0",
+    version="3.1.1",
     author="Gabriel Tem Pass",
     author_email="redo_hint_0x@icloud.com",
     description="A component that allows you to place a navigation bar in your Streamlit app.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gabrieltempass/streamlit-navigation-bar",
     packages=[
```

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/__init__.py` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     container : DeltaGenerator
         A container object. ``st.markdown`` can be added to this container
         using either the ``"with"`` notation or by calling methods directly on
         the returned object.
     """
     if use_padding:
         # The position of the body will be 6rem from the top.
-        margin_bottom = "-6rem"
+        margin_bottom = "-5.875rem"
     else:
         # The position of the body will be right below the navbar.
         margin_bottom = "-9rem"
 
     html = (
         f"""
         <style>
```

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/errors.py` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/example.py` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/index.html` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/match_navbar.py` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/match_navbar.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/PKG-INFO` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.1.0
+Version: 3.1.1
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -304,21 +304,25 @@
     "active": {
         "color": "var(--text-color)",
         "background-color": "white",
         "font-weight": "normal",
         "padding": "14px",
     }
 }
+options = {
+    "show_menu": False,
+    "show_sidebar": False,
+}
 
 page = st_navbar(
     pages,
     logo_path=logo_path,
     urls=urls,
     styles=styles,
-    options=False,
+    options=options,
 )
 
 functions = {
     "Home": pg.show_home,
     "Install": pg.show_install,
     "User Guide": pg.show_user_guide,
     "API": pg.show_api,
```

### Comparing `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/SOURCES.txt` & `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

