# Comparing `tmp/streamlit-navigation-bar-3.0.3.tar.gz` & `tmp/streamlit-navigation-bar-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-navigation-bar-3.0.3.tar", last modified: Thu Apr  4 18:55:07 2024, max compression
+gzip compressed data, was "streamlit-navigation-bar-3.1.0.tar", last modified: Sat Apr  6 14:38:44 2024, max compression
```

## Comparing `streamlit-navigation-bar-3.0.3.tar` & `streamlit-navigation-bar-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.705165 streamlit-navigation-bar-3.0.3/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.0.3/LICENSE
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.0.3/MANIFEST.in
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13156 2024-04-04 18:55:07.704875 streamlit-navigation-bar-3.0.3/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    12639 2024-04-04 18:38:25.000000 streamlit-navigation-bar-3.0.3/README.md
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-04 18:55:07.705275 streamlit-navigation-bar-3.0.3/setup.cfg
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1024 2024-04-04 18:37:38.000000 streamlit-navigation-bar-3.0.3/setup.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.701203 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    15968 2024-03-31 21:52:11.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/__init__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8403 2024-03-21 18:46:33.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/errors.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/example.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.698053 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.702850 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.703605 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1147 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css
--rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-03-27 13:32:37.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/index.html
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/match_navbar.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-04 18:55:07.702652 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13156 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/requires.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-04 18:55:07.000000 streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/top_level.txt
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.297266 streamlit-navigation-bar-3.1.0/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.1.0/LICENSE
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.1.0/MANIFEST.in
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13454 2024-04-06 14:38:44.296967 streamlit-navigation-bar-3.1.0/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    12937 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.0/README.md
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-06 14:38:44.297322 streamlit-navigation-bar-3.1.0/setup.cfg
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1024 2024-04-06 14:35:00.000000 streamlit-navigation-bar-3.1.0/setup.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.294396 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    17097 2024-04-06 14:38:25.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/__init__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8452 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/errors.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/example.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.292319 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.295588 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.296690 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/index.html
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/match_navbar.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 14:38:44.295432 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13454 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/requires.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-06 14:38:44.000000 streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/top_level.txt
```

### Comparing `streamlit-navigation-bar-3.0.3/LICENSE` & `streamlit-navigation-bar-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.3/PKG-INFO` & `streamlit-navigation-bar-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.0.3
+Version: 3.1.0
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,16 +76,16 @@
 by ``"hover"`` (if they are set to ``True`` in *options*). Currently,
 ``"hover"`` only accepts two CSS properties, they are: ``"color"`` and
 ``"background-color"``.
 
 **options** : `bool` or `dict of {str : bool}`, `default=True`</br>
 Customize the navbar with options that can be toggled on or off. It accepts a
 dictionary with the option name as the key and a boolean as the value. The
-available options are: ``"show_menu"``, ``"show_sidebar"`` and
-``"fix_shadow"``. Check the notes section for a description of each one.
+available options are: ``"show_menu"``, ``"show_sidebar"``, ``"fix_shadow"``
+and ``"use_padding"``. Check the notes section for a description of each one.
 
 It is also possible to toggle all options to the same state. Simply pass
 ``True`` to *options*, which is the parameter default value, or ``False``.
 
 **adjust** : `bool`, `default=True`</br>
 When set to ``True`` (default), it overrides some Streamlit behaviors and makes
 a series of CSS adjustments to display the navbar correctly.
@@ -187,18 +187,18 @@
 However, the ``"img"`` tag is unique to the logo, just as ``"span"`` is to the
 page names.
 
 ### Maximum width
 
 A fundamental CSS property to adjust is the ``"max-width"`` for the ``"div"``
 tag. Because it controls how much space the page names have between them. The
-default value is ``"700px"``, which works well in most cases. But if the navbar
-has a large number of pages, or longer names, it might be necessary to increase
-the maximum width. Conversely, whenever the navbar has few pages or short
-names, this value may need to be reduced.
+default value is ``"43.75rem"``, which works well in most cases. But if the
+navbar has a large number of pages, or longer names, it might be necessary to
+increase the maximum width. Conversely, whenever the navbar has few pages or
+short names, this value may need to be reduced.
 
 ### Options
 
 The available options and their descriptions are:
 
 `"show_menu"`</br>
 Show Streamlit's menu button in the navbar.
@@ -213,14 +213,20 @@
 It is useful when the navbar and the sidebar have the same background color,
 which they do by default, because the shadow makes it possible to differentiate
 between the two elements.
 
 When set to ``False``, it assumes Streamlit's default behavior, where it
 applies the shadow only when the window width is below a certain threshold.
 
+`"use_padding"`</br>
+Position the body of the app, in the y axis of the window, 6rem from the top
+(if the navbar has a default height). This is the default style used by
+Streamlit. When set to ``False``, it removes this padding and positions the
+body right below the navbar.
+
 ## Examples
 
 A basic example:
 ``` python
 import streamlit as st
 from streamlit_navigation_bar import st_navbar
```

### Comparing `streamlit-navigation-bar-3.0.3/README.md` & `streamlit-navigation-bar-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 by ``"hover"`` (if they are set to ``True`` in *options*). Currently,
 ``"hover"`` only accepts two CSS properties, they are: ``"color"`` and
 ``"background-color"``.
 
 **options** : `bool` or `dict of {str : bool}`, `default=True`</br>
 Customize the navbar with options that can be toggled on or off. It accepts a
 dictionary with the option name as the key and a boolean as the value. The
-available options are: ``"show_menu"``, ``"show_sidebar"`` and
-``"fix_shadow"``. Check the notes section for a description of each one.
+available options are: ``"show_menu"``, ``"show_sidebar"``, ``"fix_shadow"``
+and ``"use_padding"``. Check the notes section for a description of each one.
 
 It is also possible to toggle all options to the same state. Simply pass
 ``True`` to *options*, which is the parameter default value, or ``False``.
 
 **adjust** : `bool`, `default=True`</br>
 When set to ``True`` (default), it overrides some Streamlit behaviors and makes
 a series of CSS adjustments to display the navbar correctly.
@@ -172,18 +172,18 @@
 However, the ``"img"`` tag is unique to the logo, just as ``"span"`` is to the
 page names.
 
 ### Maximum width
 
 A fundamental CSS property to adjust is the ``"max-width"`` for the ``"div"``
 tag. Because it controls how much space the page names have between them. The
-default value is ``"700px"``, which works well in most cases. But if the navbar
-has a large number of pages, or longer names, it might be necessary to increase
-the maximum width. Conversely, whenever the navbar has few pages or short
-names, this value may need to be reduced.
+default value is ``"43.75rem"``, which works well in most cases. But if the
+navbar has a large number of pages, or longer names, it might be necessary to
+increase the maximum width. Conversely, whenever the navbar has few pages or
+short names, this value may need to be reduced.
 
 ### Options
 
 The available options and their descriptions are:
 
 `"show_menu"`</br>
 Show Streamlit's menu button in the navbar.
@@ -198,14 +198,20 @@
 It is useful when the navbar and the sidebar have the same background color,
 which they do by default, because the shadow makes it possible to differentiate
 between the two elements.
 
 When set to ``False``, it assumes Streamlit's default behavior, where it
 applies the shadow only when the window width is below a certain threshold.
 
+`"use_padding"`</br>
+Position the body of the app, in the y axis of the window, 6rem from the top
+(if the navbar has a default height). This is the default style used by
+Streamlit. When set to ``False``, it removes this padding and positions the
+body right below the navbar.
+
 ## Examples
 
 A basic example:
 ``` python
 import streamlit as st
 from streamlit_navigation_bar import st_navbar
```

### Comparing `streamlit-navigation-bar-3.0.3/setup.py` & `streamlit-navigation-bar-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="streamlit-navigation-bar",
-    version="3.0.3",
+    version="3.1.0",
     author="Gabriel Tem Pass",
     author_email="redo_hint_0x@icloud.com",
     description="A component that allows you to place a navigation bar in your Streamlit app.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gabrieltempass/streamlit-navigation-bar",
     packages=[
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/__init__.py` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 
 
 def _prepare_options(options):
     """Build dict with given options, state and defaults where omitted."""
     available = {
         "show_menu": True,
         "show_sidebar": True,
-        "fixed_shadow": True,
+        "fix_shadow": True,
+        "use_padding": True,
     }
     for option in available:
         if isinstance(options, dict) and option in options:
             available[option] = options[option]
         elif isinstance(options, bool) and not options:
             available[option] = options
     return available
@@ -82,46 +83,62 @@
 
 def load_env(path):
     """Load the Jinja environment from a given absolute path."""
     loader = FileSystemLoader(path)
     return Environment(loader=loader, trim_blocks=True, lstrip_blocks=True)
 
 
-def stylized_container(key):
+def position_body(key, use_padding):
     """
-    Add a spaceless container to the app.
+    Add a stylized container to the app that adjusts the position of the body.
 
-    Insert a container into the app, which receives an iframe that does not
-    render anything. Style this container using CSS and a unique key to remove
-    the space added by Streamlit.
+    Insert a container into the app, to add an ``st.markdown``, using either
+    the "with" notation or by calling the method directly on the returned
+    object.
+
+    This container serves to position the body of the app in the y axis of the
+    window. Which can be the same as the default in Streamlit (6rem from the
+    top), or right below the navbar.
+
+    It does so by having a unique CSS selector, and being inserted in a <div>
+    palced immediately before the <div> of the body of the app. Then, it styles
+    the margin-bottom property and moves the body to the desired position.
 
     Parameters
     ----------
     key : str, int or None
         A key associated with this container. This needs to be unique since all
         styles will be applied to the container with this key.
 
     Returns
     -------
     container : DeltaGenerator
-        A container object. Elements can be added to this container using
-        either the "with" notation or by calling methods directly on the
-        returned object.
+        A container object. ``st.markdown`` can be added to this container
+        using either the ``"with"`` notation or by calling methods directly on
+        the returned object.
     """
+    if use_padding:
+        # The position of the body will be 6rem from the top.
+        margin_bottom = "-6rem"
+    else:
+        # The position of the body will be right below the navbar.
+        margin_bottom = "-9rem"
+
     html = (
         f"""
         <style>
-            div[data-testid='stVerticalBlock']:has(
+            div[data-testid="stVerticalBlockBorderWrapper"]:has(
+                div[data-testid="stVerticalBlock"]
                 > div.element-container
                 > div.stMarkdown
                 > div[data-testid='stMarkdownContainer']
                 > p
                 > span.{key}
-            ) > div:first-child {{
-                margin-bottom: -1rem;
+            ) {{
+                margin-bottom: {margin_bottom};
             }}
         </style>
         <span class='{key}'></span>
         """
     )
     container = st.container()
     container.markdown(html, unsafe_allow_html=True)
@@ -151,21 +168,21 @@
 
         The available HTML tags are: ``"nav"``, ``"div"``, ``"ul"``, ``"li"``,
         ``"a"``, ``"img"`` and ``"span"``.
 
         The available pseudo-classes are: ``"active"`` and ``"hover"``, which
         direct the styling to the ``"span"`` tag. The menu and sidebar buttons
         are only styled by ``"hover"`` (if they are set to ``True`` in
-        `options`). Currently, ``"hover"`` only accepts two CSS properties, they
-        are: ``"color"`` and ``"background-color"``.
+        `options`). Currently, ``"hover"`` only accepts two CSS properties,
+        they are: ``"color"`` and ``"background-color"``.
     options : bool or dict of {str : bool}
         Customize the navbar with options that can be toggled on or off. It
         accepts a dictionary with the option name as the key and a boolean as
         the value. The available options are: ``"show_menu"``,
-        ``"show_sidebar"`` and ``"fix_shadow"``.
+        ``"show_sidebar"``, ``"fix_shadow"`` and ``"use_padding"``.
 
         It is also possible to toggle all options to the same state. Simply
         pass ``True`` or ``False`` to `options`.
     key : str, int or None
         A key associated with the container that adjusts the CSS. This needs to
         be unique since all styles will be applied to the container with this
         key.
@@ -212,15 +229,15 @@
     template = env.get_template("options.css")
     css = template.render(
         ui=ui,
         options=options,
         margin=margin,
         key=key,
     )
-    with stylized_container(key):
+    with position_body(key, options["use_padding"]):
         _adjust(css)
 
 
 # A placeholder object to implement the default rules for selected
 sentinel = object()
 
 
@@ -284,16 +301,16 @@
         are only styled by ``"hover"`` (if they are set to ``True`` in
         `options`). Currently, ``"hover"`` only accepts two CSS properties,
         they are: ``"color"`` and ``"background-color"``.
     options : bool or dict of {str : bool}, default=True
         Customize the navbar with options that can be toggled on or off. It
         accepts a dictionary with the option name as the key and a boolean as
         the value. The available options are: ``"show_menu"``,
-        ``"show_sidebar"`` and ``"fix_shadow"``. Check the notes section for a
-        description of each one.
+        ``"show_sidebar"``, ``"fix_shadow"`` and ``"use_padding"``. Check the
+        notes section for a description of each one.
 
         It is also possible to toggle all options to the same state. Simply
         pass ``True`` to `options`, which is the parameter default value, or
         ``False``.
     adjust : bool, default=True
         When set to ``True`` (default), it overrides some Streamlit behaviors
         and makes a series of CSS adjustments to display the navbar correctly.
@@ -385,15 +402,15 @@
     However, the ``"img"`` tag is unique to the logo, just as ``"span"`` is to
     the page names.
 
     **Maximum width**
 
     A fundamental CSS property to adjust is the ``"max-width"`` for the
     ``"div"`` tag. Because it controls how much space the page names have
-    between them. The default value is ``"700px"``, which works well
+    between them. The default value is ``"43.75rem"``, which works well
     in most cases. But if the navbar has a large number of pages, or longer
     names, it might be necessary to increase the maximum width. Conversely,
     whenever the navbar has few pages or short names, this value may need to
     be reduced.
 
     **Options**
 
@@ -410,14 +427,19 @@
         width. It is useful when the navbar and the sidebar have the same
         background color, which they do by default, because the shadow makes it
         possible to differentiate between the two elements.
 
         When set to ``False``, it assumes Streamlit's default behavior, where
         it applies the shadow only when the window width is below a certain
         threshold.
+    "use_padding"
+        Position the body of the app, in the y axis of the window, 6rem from
+        the top (if the navbar has a default height). This is the default style
+        used by Streamlit. When set to ``False``, it removes this padding and
+        positions the body right below the navbar.
 
     Examples
     --------
     >>> import streamlit as st
     >>> from streamlit_navigation_bar import st_navbar
     >>> page = st_navbar(
     ...     ["Home", "Documentation", "Examples", "Community", "About"]
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/errors.py` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,21 +203,22 @@
 
     for option, toggle in options.items():
         if not isinstance(option, str):
             raise StreamlitAPIException(
                 _dict_error(option, "options", "key", "bool")
             )
 
-        available = ["show_menu", "show_sidebar", "fix_shadow"]
+        available = ["show_menu", "show_sidebar", "fix_shadow", "use_padding"]
         if option not in available:
             raise StreamlitAPIException(
                 "The adjust parameter from st_navbar() received a "
                 "dictionary that has an invalid key. The key must be the name "
                 "of one of the available options.\n"
-                f"\nExpected: 'show_menu', 'show_sidebar', 'fix_shadow'  "
+                f"\nExpected: 'show_menu', 'show_sidebar', 'fix_shadow', "
+                "'use_padding'  "
                 f"\nGot: '{option}'"
             )
 
         if not isinstance(toggle, bool):
             raise StreamlitAPIException(
                 _dict_error(toggle, "options", "value", "bool")
             )
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/example.py` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css`

 * *Files 26% similar despite different names*

```diff
@@ -1 +1 @@
-*[data-v-f8fd9294]{margin:0;padding:0}nav[data-v-f8fd9294]{display:flex;justify-content:center;align-items:center;background-color:var(--secondary-background-color);font-family:var(--font);height:2.875rem;padding-left:2rem;padding-right:2rem}div[data-v-f8fd9294]{width:100%;max-width:700px}ul[data-v-f8fd9294]{display:flex;justify-content:space-between;width:100%}li[data-v-f8fd9294]{display:flex;align-items:center;list-style:none}a[data-v-f8fd9294]{text-decoration:none}img[data-v-f8fd9294]{display:flex;height:1.875rem}span[data-v-f8fd9294]{display:block;color:var(--text-color);text-align:center}.active[data-v-f8fd9294]{color:var(--text-color);font-weight:700}span[data-v-f8fd9294]:before{content:attr(data-text);display:flex;font-weight:700;height:0;overflow:hidden;visibility:hidden;-webkit-user-select:none;user-select:none;pointer-events:none}.hover-color[data-v-f8fd9294]:hover{color:var(--43711ce9)!important}.hover-bg-color[data-v-f8fd9294]:hover{background-color:var(--32628bb8)!important}.err__title[data-v-9ae37d8b],.err__msg[data-v-9ae37d8b],body{margin:0}#app{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}
+*[data-v-30156451]{margin:0;padding:0}nav[data-v-30156451]{display:flex;justify-content:center;align-items:center;background-color:var(--secondary-background-color);font-family:var(--font);height:2.875rem;padding-left:2rem;padding-right:2rem}div[data-v-30156451]{width:100%;max-width:43.75rem}ul[data-v-30156451]{display:flex;justify-content:space-between;width:100%}li[data-v-30156451]{display:flex;align-items:center;list-style:none}a[data-v-30156451]{text-decoration:none}img[data-v-30156451]{display:flex;height:1.875rem}span[data-v-30156451]{display:block;color:var(--text-color);text-align:center}.active[data-v-30156451]{color:var(--text-color);font-weight:700}span[data-v-30156451]:before{content:attr(data-text);display:flex;font-weight:700;height:0;overflow:hidden;visibility:hidden;-webkit-user-select:none;user-select:none;pointer-events:none}.hover-color[data-v-30156451]:hover{color:var(--0f327572)!important}.hover-bg-color[data-v-30156451]:hover{background-color:var(--70c7d726)!important}.err__title[data-v-9ae37d8b],.err__msg[data-v-9ae37d8b],body{margin:0}#app{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11800,16 +11800,16 @@
                 hoverColor: a,
                 hoverBgColor: c
             }
         }
     },
     il = () => {
         mp(e => ({
-            "43711ce9": e.color,
-            "32628bb8": e.bgColor
+            "0f327572": e.color,
+            "70c7d726": e.bgColor
         }))
     },
     rl = Ja.setup;
 Ja.setup = rl ? (e, t) => (il(), rl(e, t)) : il;
 const tb = ["src"],
     eb = ["src"],
     nb = ["href", "target", "onClick"],
@@ -11853,15 +11853,15 @@
             active: o === i.activePage
         }, i.hoverColor, i.hoverBgColor]),
         style: Rt(i.parseStyles(i.styles.span) + i.parseStyles(i.styles.active, o === i.activePage))
     }, ul(o), 15, ib)], 12, nb)], 4))), 128))], 4)], 4)], 4)
 }
 const sb = Ka(Ja, [
         ["render", rb],
-        ["__scopeId", "data-v-f8fd9294"]
+        ["__scopeId", "data-v-30156451"]
     ]),
     ob = Rl({
         name: "WithStreamlitConnection",
         setup() {
             const e = ei(void 0),
                 t = ei(""),
                 n = i => {
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/frontend/dist/index.html` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/frontend/dist/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Streamlit Navbar Component</title>
-    <script type="module" crossorigin src="./assets/index-K06dADTk.js"></script>
-    <link rel="stylesheet" crossorigin href="./assets/index-31IBmtiW.css">
+    <script type="module" crossorigin src="./assets/index-QGLefmoh.js"></script>
+    <link rel="stylesheet" crossorigin href="./assets/index-nKPQXLAl.css">
   </head>
   <body>
     <noscript>
       <strong>We're sorry but the website doesn't work properly without JavaScript enabled.
         Please enable it to continue.</strong>
     </noscript>
     <div id="app"></div>
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar/match_navbar.py` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar/match_navbar.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/PKG-INFO` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.0.3
+Version: 3.1.0
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,16 +76,16 @@
 by ``"hover"`` (if they are set to ``True`` in *options*). Currently,
 ``"hover"`` only accepts two CSS properties, they are: ``"color"`` and
 ``"background-color"``.
 
 **options** : `bool` or `dict of {str : bool}`, `default=True`</br>
 Customize the navbar with options that can be toggled on or off. It accepts a
 dictionary with the option name as the key and a boolean as the value. The
-available options are: ``"show_menu"``, ``"show_sidebar"`` and
-``"fix_shadow"``. Check the notes section for a description of each one.
+available options are: ``"show_menu"``, ``"show_sidebar"``, ``"fix_shadow"``
+and ``"use_padding"``. Check the notes section for a description of each one.
 
 It is also possible to toggle all options to the same state. Simply pass
 ``True`` to *options*, which is the parameter default value, or ``False``.
 
 **adjust** : `bool`, `default=True`</br>
 When set to ``True`` (default), it overrides some Streamlit behaviors and makes
 a series of CSS adjustments to display the navbar correctly.
@@ -187,18 +187,18 @@
 However, the ``"img"`` tag is unique to the logo, just as ``"span"`` is to the
 page names.
 
 ### Maximum width
 
 A fundamental CSS property to adjust is the ``"max-width"`` for the ``"div"``
 tag. Because it controls how much space the page names have between them. The
-default value is ``"700px"``, which works well in most cases. But if the navbar
-has a large number of pages, or longer names, it might be necessary to increase
-the maximum width. Conversely, whenever the navbar has few pages or short
-names, this value may need to be reduced.
+default value is ``"43.75rem"``, which works well in most cases. But if the
+navbar has a large number of pages, or longer names, it might be necessary to
+increase the maximum width. Conversely, whenever the navbar has few pages or
+short names, this value may need to be reduced.
 
 ### Options
 
 The available options and their descriptions are:
 
 `"show_menu"`</br>
 Show Streamlit's menu button in the navbar.
@@ -213,14 +213,20 @@
 It is useful when the navbar and the sidebar have the same background color,
 which they do by default, because the shadow makes it possible to differentiate
 between the two elements.
 
 When set to ``False``, it assumes Streamlit's default behavior, where it
 applies the shadow only when the window width is below a certain threshold.
 
+`"use_padding"`</br>
+Position the body of the app, in the y axis of the window, 6rem from the top
+(if the navbar has a default height). This is the default style used by
+Streamlit. When set to ``False``, it removes this padding and positions the
+body right below the navbar.
+
 ## Examples
 
 A basic example:
 ``` python
 import streamlit as st
 from streamlit_navigation_bar import st_navbar
```

### Comparing `streamlit-navigation-bar-3.0.3/streamlit_navigation_bar.egg-info/SOURCES.txt` & `streamlit-navigation-bar-3.1.0/streamlit_navigation_bar.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 streamlit_navigation_bar/match_navbar.py
 streamlit_navigation_bar.egg-info/PKG-INFO
 streamlit_navigation_bar.egg-info/SOURCES.txt
 streamlit_navigation_bar.egg-info/dependency_links.txt
 streamlit_navigation_bar.egg-info/requires.txt
 streamlit_navigation_bar.egg-info/top_level.txt
 streamlit_navigation_bar/frontend/dist/index.html
-streamlit_navigation_bar/frontend/dist/assets/index-31IBmtiW.css
-streamlit_navigation_bar/frontend/dist/assets/index-K06dADTk.js
+streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
+streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
```

