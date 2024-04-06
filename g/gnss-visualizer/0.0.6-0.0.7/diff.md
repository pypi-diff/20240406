# Comparing `tmp/gnss_visualizer-0.0.6.tar.gz` & `tmp/gnss_visualizer-0.0.7.tar.gz`

## Comparing `gnss_visualizer-0.0.6.tar` & `gnss_visualizer-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,37 @@
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/babel.cfg
--rw-r--r--   0        0        0   115228 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/coldstart.ubx
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/requirements-dev.in
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/requirements-dev.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/requirements.in
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/requirements.txt
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/.github/workflows/check.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   494548 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/images/logo.webp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/__init__.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/app.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/constants.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/conversions.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/main.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/plot.py
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/run_server.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/ubx_stream.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/models/__init__,py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/models/plot.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/src/gnss_visualizer/translations/fi/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/tests/test_file_reading.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/LICENSE
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/README.md
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    48277 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/babel.cfg
+-rw-r--r--   0        0        0   115228 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/coldstart.ubx
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/renovate.json
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/requirements-dev.in
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/requirements-dev.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/requirements.in
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/.github/workflows/check.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   494548 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/images/logo.webp
+-rwxr-xr-x   0        0        0     2509 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/scripts/extract-ubx-messages.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/app.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/constants.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/conversions.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/main.py
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/run_server.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/ubx_stream.py
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/ui_handler.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/plots/__init__.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/plots/cno.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/plots/generic_plot.py
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/plots/map.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/protocols/ubx.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/src/gnss_visualizer/translations/fi/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/tests/test_ubx_stream.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/tests/test_ui_handler.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/README.md
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    49559 2020-02-02 00:00:00.000000 gnss_visualizer-0.0.7/PKG-INFO
```

### Comparing `gnss_visualizer-0.0.6/coldstart.ubx` & `gnss_visualizer-0.0.7/coldstart.ubx`

 * *Files identical despite different names*

### Comparing `gnss_visualizer-0.0.6/requirements-dev.txt` & `gnss_visualizer-0.0.7/requirements-dev.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile /home/jop/dev/gnss-visualizer/requirements-dev.in
 asttokens==2.4.1
     # via stack-data
-build==1.1.1
+build==1.2.1
 cachetools==5.3.3
     # via tox
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 chardet==5.2.0
     # via tox
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tox
+coverage==7.4.4
 cryptography==42.0.5
     # via secretstorage
 decorator==5.1.1
     # via
     #   ipdb
     #   ipython
 distlib==0.3.8
     # via virtualenv
 docutils==0.20.1
     # via readme-renderer
 executing==2.0.1
     # via stack-data
-filelock==3.13.1
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
 idna==3.6
     # via requests
-importlib-metadata==7.0.2
+importlib-metadata==7.1.0
     # via twine
 iniconfig==2.0.0
     # via pytest
 ipdb==0.13.13
-ipython==8.22.2
+ipython==8.23.0
     # via ipdb
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==5.2.0
+    # via keyring
+jaraco-functools==4.0.0
     # via keyring
 jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==24.3.1
+keyring==25.1.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 matplotlib-inline==0.1.6
     # via ipython
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
-    # via jaraco-classes
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
 mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
-nh3==0.2.15
+nh3==0.2.17
     # via readme-renderer
+numpy==1.26.4
+    # via pandas-stubs
 packaging==24.0
     # via
     #   build
     #   pyproject-api
     #   pytest
     #   tox
-parso==0.8.3
+pandas-stubs==2.2.1.240316
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pip==24.0
 pkginfo==1.10.0
     # via twine
 platformdirs==4.2.0
@@ -86,15 +96,15 @@
     #   tox
 prompt-toolkit==3.0.43
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pygments==2.17.2
     # via
     #   ipython
     #   readme-renderer
     #   rich
 pyproject-api==1.6.1
@@ -116,21 +126,35 @@
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via asttokens
 stack-data==0.6.3
     # via ipython
-tox==4.14.1
+tox==4.14.2
 traitlets==5.14.2
     # via
     #   ipython
     #   matplotlib-inline
 twine==5.0.0
-typing-extensions==4.10.0
+types-colorama==0.4.15.20240311
+types-decorator==5.1.8.20240310
+types-docutils==0.20.0.20240406
+    # via types-pygments
+types-openpyxl==3.1.0.20240402
+types-pillow==10.2.0.20240406
+types-pycurl==7.45.2.20240311
+types-pygments==2.17.0.20240310
+types-pytz==2024.1.0.20240203
+    # via pandas-stubs
+types-pyyaml==6.0.12.20240311
+types-setuptools==69.2.0.20240317
+    # via types-pygments
+types-six==1.16.21.20240311
+typing-extensions==4.11.0
     # via mypy
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 virtualenv==20.25.1
     # via tox
```

### Comparing `gnss_visualizer-0.0.6/requirements.txt` & `gnss_visualizer-0.0.7/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile /home/jop/dev/gnss-visualizer/requirements.in
 bokeh==3.4.0
 certifi==2024.2.2
     # via pyproj
-contourpy==1.2.0
+contourpy==1.2.1
     # via bokeh
 jinja2==3.1.3
     # via bokeh
 markupsafe==2.1.5
     # via jinja2
 numpy==1.26.4
     # via
     #   bokeh
     #   contourpy
     #   pandas
 packaging==24.0
     # via bokeh
 pandas==2.2.1
     # via bokeh
-pillow==10.2.0
+pillow==10.3.0
     # via bokeh
-pynmeagps==1.0.33
+pynmeagps==1.0.35
     # via pyubx2
 pyproj==3.6.1
-pyrtcm==1.0.16
+pyrtcm==1.0.17
     # via pyubx2
 pyserial==3.5
 python-dateutil==2.9.0.post0
     # via pandas
 pytz==2024.1
     # via pandas
 pyubx2==1.2.39
@@ -35,9 +35,9 @@
     # via bokeh
 six==1.16.0
     # via python-dateutil
 tornado==6.4
     # via bokeh
 tzdata==2024.1
     # via pandas
-xyzservices==2023.10.1
+xyzservices==2024.4.0
     # via bokeh
```

### Comparing `gnss_visualizer-0.0.6/.github/workflows/check.yml` & `gnss_visualizer-0.0.7/.github/workflows/check.yml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
           - "3.12"
           - "3.11"
         os:
           - ubuntu-latest
           - macos-latest
           - windows-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.py }}
       - name: Install tox
```

### Comparing `gnss_visualizer-0.0.6/.github/workflows/python-publish.yml` & `gnss_visualizer-0.0.7/.github/workflows/python-publish.yml`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   deploy:
 
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `gnss_visualizer-0.0.6/images/logo.webp` & `gnss_visualizer-0.0.7/images/logo.webp`

 * *Files identical despite different names*

### Comparing `gnss_visualizer-0.0.6/src/gnss_visualizer/app.py` & `gnss_visualizer-0.0.7/src/gnss_visualizer/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 Visualization tool for GNSS data. Reads UBX messages from a file or device and
 generates plots from the data.
 """
 
 import argparse
 import logging
 from pathlib import Path
-from threading import Thread
 
-from bokeh.plotting import curdoc
-
-from gnss_visualizer.plot import LOGGER as plot_logger
-from gnss_visualizer.plot import PlotHandler
 from gnss_visualizer.ubx_stream import LOGGER as ubx_logger
-from gnss_visualizer.ubx_stream import UbxStreamReader
+from gnss_visualizer.ui_handler import LOGGER as plot_logger
+from gnss_visualizer.ui_handler import UIHandler
 
 LOGGER = logging.getLogger(__name__)
 
 
 def handle_args() -> argparse.Namespace:
     """Handle command-line arguments."""
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("input", type=Path, help="Input file or device.")
     parser.add_argument(
         "-w",
-        "--simulate-wait-s",
+        "--default-simulate-wait-s",
         type=float,
-        default=None,
-        help="Simulate wait time between NAV-PVT messages, only applies for reading files.",
+        default=0.1,
+        help="Default value for simulated wait time between NAV-PVT messages, only applies for reading files.",
+    )
+    parser.add_argument(
+        "--dev",
+        action="store_true",
+        help="Enable live reloading during app development.",
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="count",
         default=0,
         help="Produce verbose output. Use multiple times to increase verbosity.",
@@ -56,19 +57,15 @@
     )
     for logger in (LOGGER, plot_logger, ubx_logger):
         logger.setLevel(level)
 
     return args
 
 
-def run_app(args: argparse.Namespace):
+def run_app(args: argparse.Namespace) -> None:
     """Start the application.
 
     This is meant to be called from bokeh server.
     """
     LOGGER.info("Starting GNSS Visualizer application.")
 
-    plot_handler = PlotHandler(curdoc())
-    stream_reader = UbxStreamReader(args.input, plot_handler, args.simulate_wait_s)
-
-    thread = Thread(target=stream_reader.read)
-    thread.start()
+    UIHandler(args.input, args.default_simulate_wait_s)
```

### Comparing `gnss_visualizer-0.0.6/src/gnss_visualizer/plot.py` & `gnss_visualizer-0.0.7/src/gnss_visualizer/plots/map.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,368 +1,265 @@
-"""Generate plots."""
+"""C/N0 plots for GNSS Visualizer."""
 
 import gettext
 import locale
 import logging
-from math import isnan
 from pathlib import Path
-from typing import Any, Callable, Iterable
+from typing import Any
 
 import pyubx2
 import xyzservices.providers as xyz
-from bokeh.document import Document
 from bokeh.layouts import Spacer, column, row
-from bokeh.models import ColumnDataSource, Div, Toggle
+from bokeh.models import (  # type: ignore[attr-defined]
+    Button,
+    ColumnDataSource,
+    Toggle,
+    UIElement,
+)
 from bokeh.plotting import figure
 
-from gnss_visualizer.constants import RINEX_CONSTELLATION_COLORS, UBX_GNSSID_TO_RINEX
+from gnss_visualizer.constants import TOP_SPACER_HEIGHT
 from gnss_visualizer.conversions import lat_lon_to_web_mercator
-from gnss_visualizer.models.plot import Plot
-
-LOGGER = logging.getLogger(__name__)
+from gnss_visualizer.plots.generic_plot import GenericContinuousPlot
+from gnss_visualizer.protocols.ubx import get_full_ubx_msg_id
 
 locale.setlocale(locale.LC_ALL, "")
 lang = gettext.translation(
-    "messages", localedir=Path(__file__).parent / "translations", fallback=True
+    "messages", localedir=Path(__file__).parent.parent / "translations", fallback=True
 )
 lang.install()
 _ = lang.gettext
 
+LOGGER = logging.getLogger(__name__)
 
-class PlotHandler:
-    """Generate plots from GNSS receiver messages."""
 
-    DEFAULT_PLOT_HEIGHT = 400
-    MAP_PLOT_HEIGHT = 380
-    SPACER_HEIGHT = 25
-
-    DEFAULT_MAP_TOOLS = "pan,wheel_zoom,zoom_out,box_zoom,hover,undo,redo,reset"
-    DEFAULT_TOOLS = "pan,wheel_zoom,zoom_out,box_zoom,hover,undo,redo,reset"
-
-    TITLE = _("GNSS Visualizer")
-
-    def __init__(self, doc: Document):
-        """Initialize an instance."""
-        self.doc = doc
-
-        self._main_column = column(sizing_mode="stretch_width")
-        self._side_column = column()
-
-        title_div = Div(
-            text=f"<h1>{self.TITLE}</h1>",
-            styles={
-                "text-align": "center",
-            },
-            height=20,
-            sizing_mode="stretch_width",
+class LivePositionMapPlot(GenericContinuousPlot):
+    """Live plot for positions on map."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        """Init the instance."""
+        super().__init__(*args, **kwargs)
+        self._side_layout = column(
+            height=self.MAP_PLOT_HEIGHT,
         )
 
-        root_row = row(
-            self._main_column,
-            self._side_column,
-            Spacer(width=100),
+        self._center_map_button = self._generate_center_map_button()
+        self._autocenter_toggle = self._generate_autocenter_toggle()
+        self._autozoom_toggle = self._generate_autozoom_toggle()
+
+    @property
+    def visible_on_start(self) -> bool:
+        """Get whether the plot is visible on start."""
+        return True
+
+    @property
+    def name(self) -> str:
+        """Get the name of the plot."""
+        return _("Position map (live)")
+
+    @property
+    def required_messages(self) -> list[str]:
+        """Get required messages for this plot."""
+        return ["UBX-NAV-PVT"]
+
+    def _generate_center_map_button(self) -> Button:
+        """Add center map button."""
+        button = Button(
+            label=_("Center map"),
+            button_type="success",
             sizing_mode="stretch_width",
         )
-        root_column = column(title_div, root_row, sizing_mode="stretch_width")
 
-        self.doc.add_root(root_column)
+        def click(_: Any) -> None:
+            """Change apperance of the button upon a click."""
+            self._update_canvas_extent(force_center=True)
 
-        self.plots = []
-        self.plots.append(
-            Plot(
-                id="pos_map",
-                init=self._generate_pos_map,
-                messages={"NAV-PVT": self._update_pos_map},
-                priority=1,
-            )
-        )
-        self.plots.append(
-            Plot(
-                id="sv_cno",
-                init=self._generate_sv_cno,
-                messages={"NAV-SIG": self._update_sv_cno},
-            )
+        button.on_click(click)
+        return button
+
+    def _generate_autocenter_toggle(self) -> Toggle:
+        """Add center map toggle button.
+
+        The button toggles map centering and changes color based on the state of
+        the centering.
+        """
+        toggle = Toggle(
+            label=_("Keep centered"),
+            button_type="success",
+            active=True,
+            sizing_mode="stretch_width",
         )
 
-    @property
-    def required_msgs(self) -> set[str]:
-        """Get required messages for all plots."""
-        return {msg for plot in self.plots for msg in plot.messages.keys()}
-
-    def get_handlers_for_msg(self, msg_str: str) -> list[Callable]:
-        """Get handlers for a message."""
-        handlers = []
-        for plot in self.plots:
-            if msg_str in plot.messages:
-                handler = plot.messages[msg_str]
-                if handler:
-                    handlers.append(handler)
-
-        return handlers
-
-    def get_plot(self, id: str) -> Plot:
-        """Get plot by id."""
-        for plot in self.plots:
-            if plot.id == id:
-                return plot
-
-        raise ValueError(f"Plot {id} not found.")
-
-    def _sort_rinex_sv_ids(self, rinex_sv_ids: Iterable[str]) -> list[str]:
-        def constellation_sort(item: str) -> tuple[int, int]:
-            if item.startswith("G"):
-                return (0, int(item[1:]))
-            elif item.startswith("E"):
-                return (1, int(item[1:]))
-            elif item.startswith("C"):
-                return (2, int(item[1:]))
-            elif item.startswith("R"):
-                return (3, int(item[1:]))
-            elif item.startswith("S"):
-                return (4, int(item[1:]))
-            elif item.startswith("J"):
-                return (5, int(item[1:]))
+        def click(_: Any) -> None:
+            """Change apperance of the button upon a click."""
+            if toggle.active:
+                toggle.button_type = "success"
             else:
-                return (6, int(item[1:]))
+                toggle.button_type = "default"
+                # never autozoom when centering is disabled
+                self._autozoom_toggle.active = False
+            if self._side_layout is not None:
+                self._side_layout.children = self._get_side_layout_children()  # type: ignore[assignment]
 
-        return sorted(rinex_sv_ids, key=constellation_sort)
+        toggle.on_click(click)
+        return toggle
+
+    def _generate_autozoom_toggle(self) -> Toggle:
+        """Add autozoom toggle button.
+
+        The button toggles map autozoom and changes color based on the state of
+        the autozoom.
+        """
+        toggle = Toggle(
+            label=_("Autozoom"),
+            button_type="success",
+            active=True,
+            sizing_mode="stretch_width",
+        )
 
-    def _set_plot_styles(self, plot: figure) -> None:
-        """Set plot styles."""
-        # font sizes
-        plot.xaxis.axis_label_text_font_size = "14pt"
-        plot.yaxis.axis_label_text_font_size = "14pt"
-        plot.xaxis.major_label_text_font_size = "12pt"
-        plot.yaxis.major_label_text_font_size = "12pt"
-        plot.title.text_font_size = "16pt"
+        def click(_: Any) -> None:
+            """Change apperance of the button upon a click."""
+            if toggle.active:
+                toggle.button_type = "success"
+                # always autocenter when autozoom is active
+                self._autocenter_toggle.active = True
+            else:
+                toggle.button_type = "default"
+            self._side_layout.children = self._get_side_layout_children()  # type: ignore[assignment]
 
-        plot.xgrid.grid_line_color = None
-        plot.ygrid.grid_line_color = None
+        toggle.on_click(click)
+        return toggle
 
-        plot.toolbar.autohide = True
+    def _update_canvas_extent(self, force_center: bool = False) -> None:
+        """Update map canvas extents."""
+        if self.datasource is None or self.figure is None:
+            return
 
-    def _center_map(self, plot: Plot) -> None:
-        """Center map on the current position."""
         if (
-            not self._center_map_toggle.active
-            or plot.datasource is None
-            or plot.figure is None
+            not force_center
+            and not self._autocenter_toggle.active
+            and not self._autozoom_toggle.active
         ):
             return
-        hacc = plot.datasource.data["h_acc"][0]
+
+        hacc = self.datasource.data["h_acc"][0]
 
         if hacc is None:
             return
 
         # current plot range
-        dx_orig = (plot.figure.x_range.end - plot.figure.x_range.start) / 2
-
-        aspect_ratio = plot.figure.inner_height / plot.figure.inner_width
+        dx_orig = (self.figure.x_range.end - self.figure.x_range.start) / 2  # type: ignore[attr-defined]
 
-        # set x scale based on the horizontal accuracy
-        if hacc > 10000:
-            dx = 10000.0 * 1e3
-        elif hacc > 1000:
-            dx = 100.0 * 1e3
-        elif hacc > 100:
-            dx = 10 * 1e3
-        elif hacc > 50 or isnan(dx_orig):
-            dx = 1e3
-        else:
-            # keep the old range
-            dx = dx_orig
+        try:
+            aspect_ratio = self.figure.inner_height / self.figure.inner_width  # type: ignore[operator]
+        except ValueError:
+            aspect_ratio = 1
+
+        dx = dx_orig
+        if self._autozoom_toggle.active:
+            # autozoom aka set x scale based on the horizontal accuracy
+            # limit to 100 meters at most to avoid too much zooming
+            dx = max(100, hacc * 5)
 
         dy = dx * aspect_ratio
-        plot.figure.x_range.update(
-            start=plot.datasource.data["x"][0] - dx,
-            end=plot.datasource.data["x"][0] + dx,
-        )
-        plot.figure.y_range.update(
-            start=plot.datasource.data["y"][0] - dy,
-            end=plot.datasource.data["y"][0] + dy,
+        self.figure.x_range.update(  # type: ignore[attr-defined]
+            start=self.datasource.data["x"][0] - dx,
+            end=self.datasource.data["x"][0] + dx,
+        )
+        self.figure.y_range.update(  # type: ignore[attr-defined]
+            start=self.datasource.data["y"][0] - dy,
+            end=self.datasource.data["y"][0] + dy,
         )
 
         LOGGER.debug("Centered map with dx: %s, dy: %s", dx, dy)
 
-    async def _update_pos_map(self, msg: pyubx2.UBXMessage) -> None:
-        """Update position on a map."""
+    def update_plot(self, msg: pyubx2.UBXMessage) -> None:
+        """Update the plot."""
         LOGGER.info("Process position map plot")
 
-        plot = self.get_plot("pos_map")
+        if get_full_ubx_msg_id(msg) != "UBX-NAV-PVT":
+            return
 
         lat = msg.lat
         lon = msg.lon
         h_acc = msg.hAcc * 1e-3  # convert from mm to meters
 
         if lat is None or lon is None:
             return
 
         LOGGER.debug(f"Lat: {lat}, Lon: {lon}, hAcc: {h_acc}")
 
         x, y = lat_lon_to_web_mercator(lat, lon)
-        data = dict(x=[x], y=[y], h_acc=[h_acc], lat=[lat], lon=[lon])
-        if plot.figure is None or plot.datasource is None:
-            plot.init(ColumnDataSource(data=data))
-        else:
-            plot.datasource.data = data
-            self._center_map(plot)
-
-    async def _update_sv_cno(self, msg: pyubx2.UBXMessage) -> None:
-        """Handle SV C/N0 plot."""
-        LOGGER.info("Process SV C/N0 plot")
-
-        plot = self.get_plot("sv_cno")
-
-        # make dict of the SV C/N0 values
-        cnos: dict[str, int] = {}
-        for ix in range(1, msg.numSigs + 1):
-            gnss_id = getattr(msg, f"gnssId_{ix:02}")
-            sv_id = getattr(msg, f"svId_{ix:02}")
-            cno = getattr(msg, f"cno_{ix:02}")
-
-            if cno:
-                rinex_sv_id = f"{UBX_GNSSID_TO_RINEX[gnss_id]}{sv_id}"
-                if rinex_sv_id not in cnos or cno > cnos[rinex_sv_id]:
-                    cnos[rinex_sv_id] = cno
-
-        # convert to dict suitable for column data source
-        data: dict[str, list[Any]] = {
-            "x": list(cnos.keys()),
-            "y": list(cnos.values()),
-        }
-
-        # add colors
-        data["color"] = [RINEX_CONSTELLATION_COLORS[sv_id[0]] for sv_id in data["x"]]
-
-        if plot.figure is None or plot.datasource is None:
-            plot.init(ColumnDataSource(data=data))
+        data: dict[str, Any] = dict(x=[x], y=[y], h_acc=[h_acc], lat=[lat], lon=[lon])
+        if self.figure is None or self.datasource is None:
+            self.init_plot(ColumnDataSource(data=data))
         else:
-            plot.datasource.data = data
-            plot.figure.x_range.factors = self._sort_rinex_sv_ids(
-                set(list(plot.figure.x_range.factors) + data["x"])
-            )
-
-    def _add_plot_to_column(self, plot: Plot) -> None:
-        """Add plot to column.
-
-        Regenerate entire column by adding all plots to the column.
-
-        Also set the new plot as visible.
-
-        Set the column order based on priority. Higher priority values go
-        before lower values.
-        """
-        if plot.figure is None or plot.visible:
-            return
-
-        plot.visible = True
-
-        plots_to_add = [
-            plot for plot in self.plots if plot.visible and plot.figure is not None
-        ]
-        plots_prioritized = sorted(plots_to_add, key=lambda x: x.priority, reverse=True)
+            self.datasource.data = data
+            self._update_canvas_extent()
 
-        for plot in plots_prioritized:
-            self._main_column.children.append(plot.main_layout)
-            self._main_column.children.append(Spacer(height=self.SPACER_HEIGHT))
-            self._side_column.children.append(plot.side_layout)
-            self._side_column.children.append(Spacer(height=self.SPACER_HEIGHT))
-
-    def _generate_pos_map(self, datasource: ColumnDataSource) -> None:
-        """Plot position on a map."""
-        LOGGER.info("Generate position map plot")
-        plot = self.get_plot("pos_map")
+    def init_plot(self, datasource: ColumnDataSource) -> None:
+        """Initialize the plot."""
+        LOGGER.info("Initialize continuous position map plot")
 
         tooltip = [
-            ("Leveysaste", "@{lat}°"),
-            ("Pituusaste", "@{lon}°"),
-            ("Tarkkuus", "@h_acc m"),
+            (_("Latitude"), "@{lat}°"),
+            (_("Longitude"), "@{lon}°"),
+            (_("Horizontal Accuracy"), "@h_acc m"),
         ]
 
-        p = figure(
+        self.datasource = datasource
+        self.figure = figure(
             height=self.MAP_PLOT_HEIGHT,
             title=_("Position map"),
-            x_range=(datasource.data["x"][0] - 1e3, datasource.data["x"][0] + 1e3),
-            y_range=(datasource.data["y"][0] - 1e3, datasource.data["y"][0] + 1e3),
+            x_range=(
+                self.datasource.data["x"][0] - 1e3,
+                self.datasource.data["x"][0] + 1e3,
+            ),
+            y_range=(
+                self.datasource.data["y"][0] - 1e3,
+                self.datasource.data["y"][0] + 1e3,
+            ),
             x_axis_type="mercator",
             y_axis_type="mercator",
-            tools=self.DEFAULT_MAP_TOOLS,
+            tools=self.DEFAULT_TOOLS,
             tooltips=tooltip,
             sizing_mode="inherit",
         )
-        p.add_tile(xyz.OpenStreetMap.Mapnik)
-        p.circle(
+        self.figure.add_tile(xyz.OpenStreetMap.Mapnik)
+        self.figure.circle(
             x="x",
             y="y",
             radius="h_acc",
             fill_color="blue",
             fill_alpha=0.4,
-            source=datasource,
-        )
-        p.circle(
-            x="x", y="y", size=15, fill_color="#d62728", fill_alpha=1, source=datasource
-        )
-
-        # create button that toggles map_centering and changes color based on the state of the centering
-        self._center_map_toggle = Toggle(
-            label=_("Center map"),
-            button_type="success",
-            active=True,
+            source=self.datasource,
         )
-
-        def center_map_click(_) -> None:
-            """Change apperance of center map button upon a click."""
-            if self._center_map_toggle.active:
-                self._center_map_toggle.button_type = "success"
-            else:
-                self._center_map_toggle.button_type = "default"
-
-        self._center_map_toggle.on_click(center_map_click)
-
-        self._set_plot_styles(p)
-        plot.datasource = datasource
-        plot.figure = p
-        plot.side_layout = column(
-            Spacer(height=40, sizing_mode="fixed"),
-            self._center_map_toggle,
-            height=self.MAP_PLOT_HEIGHT,
+        self.figure.scatter(
+            x="x",
+            y="y",
+            size=15,
+            marker="circle",
+            fill_color="#d62728",
+            fill_alpha=1,
+            source=self.datasource,
         )
-        self._add_plot_to_column(plot)
 
-    def _generate_sv_cno(self, datasource: ColumnDataSource) -> None:
-        """Generate plot for C/N0 values.
+        self._finalize_figure()
 
-        Plots the C/N0 for the strongest signal for each SV.
-        """
-        LOGGER.info("Generate SV C/N0 plot")
-        plot = self.get_plot("sv_cno")
+        self._side_layout.children = self._get_side_layout_children()  # type: ignore[assignment]
 
-        y_label = "C/N0 [dBHz]"
-        x_label = _("Satellite")
+        self.main_layout = row(self.figure, self._side_layout, sizing_mode="inherit")
 
-        tooltip = [
-            (x_label, "@x"),
-            (y_label, "@y"),
+    def _get_side_layout_children(self) -> list[UIElement]:
+        """Generate side layout for the plot."""
+        items = [
+            Spacer(height=TOP_SPACER_HEIGHT, sizing_mode="fixed"),
         ]
-
-        p = figure(
-            height=self.DEFAULT_PLOT_HEIGHT,
-            title=_("Signal strength"),
-            tools=self.DEFAULT_TOOLS,
-            tooltips=tooltip,
-            x_range=self._sort_rinex_sv_ids(datasource.data["x"]),
-            sizing_mode="inherit",
+        if self._autocenter_toggle is not None and not self._autocenter_toggle.active:
+            items.append(self._center_map_button)
+        items.extend(
+            [
+                self._autocenter_toggle,
+                self._autozoom_toggle,
+            ]
         )
-
-        p.vbar(x="x", top="y", source=datasource, width=0.9, color="color")
-
-        p.y_range.start = 0
-        p.y_range.end = 64
-        p.xaxis.major_label_orientation = 3.14 / 4
-
-        p.yaxis.axis_label = y_label
-        p.xaxis.axis_label = x_label
-
-        self._set_plot_styles(p)
-        plot.datasource = datasource
-        plot.figure = p
-        self._add_plot_to_column(plot)
+        return items
```

### Comparing `gnss_visualizer-0.0.6/.gitignore` & `gnss_visualizer-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `gnss_visualizer-0.0.6/LICENSE` & `gnss_visualizer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gnss_visualizer-0.0.6/README.md` & `gnss_visualizer-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -60,55 +60,65 @@
 
 GNSS visualizer is a tool for visualizing GNSS data in an interactive environment.
 
 ![GNSS visualizer screenshot](https://github.com/jopppis/gnss-visualizer/assets/25751262/4b94577d-ca44-40c9-b3b9-71b695eca2f6)
 
 It is designed to offer a simple interface in a web browser with ever extending plotting capabilities.
 
+The tool is still in very early development so don't expect much just yet!
+
+
+GNSS receivers collect lots of information about the satellites and the signals they observe which can help to understand the quality of the positioning solution and the behavior of the receiver. Vast amounts of this data make it sometimes difficult to take proper advantage of it. GNSS visualizer aims to make this easier by providing easy to use tool that can be used to explore the data.
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built with
 
-The interface and all the plots are built using awesome [Bokeh](https://bokeh.org/) library.
+The interface and all the plots are built using awesome [Bokeh](https://bokeh.org/) library. Bokeh gives lots of power for creating pretty plots with nice interactive features including callbacks to python code.
 
 Parsing of ubx messages leverages [pyubx2](https://github.com/semuconsulting/pyubx2) library.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ## Getting started
 
+### Prequisites
+- Python 3.11 or later. Earlier versions might work but are not tested.
+
 ### Installation via pip
 
 ```sh
 python -m pip install gnss-visualizer
 ```
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 ## Usage
 After installing, the tool provides a command `gnss-visualizer` that can be used to launch the tool and open the UI in a web browser.
 
 
-### Reading ubx files
-Analyzing an ubx file can be done in the following way:
+### Reading ubx files in playback mode
+Analyzing an ubx file in playback mode can be done in the following way:
 ```sh
 gnss-visualizer ~/path/to/file.ubx -w 1
 ```
-where -w (shorthand for --simulate-wait-s) is used to add delay of 1 second after each UBX-NAV-PVT message. This will make files with 1 Hz navigation rate playback as if they were done in (almost) realtime.
+where -w (shorthand for --default-simulate-wait-s) is used to add delay of 1 second after each UBX-NAV-PVT message. This will make files with 1 Hz navigation rate playback as if they were done in (almost) realtime.
 
-The input file should contain UBX-NAV-PVT message and in order to generate signal and satellite based plots also UBX-NAV-SIG message.
+The input file should contain UBX-NAV-PVT messages and in order to generate signal and satellite based plots also UBX-NAV-SIG messages.
 
 
+For testing purposes the repository contains a file `coldstart.ubx` that can be used to test the tool. It contains data from a coldstart of a stationary receiver.
+
 ### Reading serial devices
 Data can be read also from a serial device using:
 ```sh
 gnss-visualizer /dev/ttyUSB0
 ```
 
 ### Details
@@ -119,22 +129,23 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ## Roadmap
 
+- [x] Test setup
+- [x] Github CICD
 - [ ] Tests
-- [ ] Github CICD
-- [ ] Plot selection mechanism
-- [ ] Make plotting module with classess for different plots
+- [x] Plot selection mechanism
+- [x] Make plotting module with classess for different plots
 - [ ] Set up whole file reading for timeseries plots
 - [ ] More plots
-- [ ] Allow playback after reading the whole file
-- [ ] Configurable wait delay
+- [x] Allow playback after reading the whole file
+- [x] Configurable wait delay
 - [ ] Non-ubx file support (some basic plots?)
 - [ ] Even more plots
 - [ ] Truth location handling (coordinates / files)
 - [ ] Lots more plots
 - [ ] UI for file input
 
 See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).
@@ -146,19 +157,31 @@
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue.
 Don't forget to give the project a star! Thanks again!
 
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
+### Setting up a local repository
+
+1. Fork the project
+2. Clone the forked project
+3. Install dependencies (`pip install -r requirements.txt && pip install -r requirements-dev.txt`)
+4. Install the project in editable mode (`pip install -e .`)
+5. Install pre-commit (`pipx install pre-commit`)
+5. Install pre-commit hooks (`pre-commit install`)
+
+### Steps to contribute
+
+1. Set up a local repository
+2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the branch (`git push origin feature/AmazingFeature`)
+5. Open a pull request
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 ## License
 
 Distributed under the AGPL-3.0 license. See `LICENSE` for more information.
```

#### html2text {}

```diff
@@ -19,55 +19,71 @@
    6. _L_i_c_e_n_s_e
    7. _C_o_n_t_a_c_t
    8. _A_c_k_n_o_w_l_e_d_g_m_e_n_t_s
 ## About the project GNSS visualizer is a tool for visualizing GNSS data in an
 interactive environment. ![GNSS visualizer screenshot](https://github.com/
 jopppis/gnss-visualizer/assets/25751262/4b94577d-ca44-40c9-b3b9-71b695eca2f6)
 It is designed to offer a simple interface in a web browser with ever extending
-plotting capabilities.
+plotting capabilities. The tool is still in very early development so don't
+expect much just yet! GNSS receivers collect lots of information about the
+satellites and the signals they observe which can help to understand the
+quality of the positioning solution and the behavior of the receiver. Vast
+amounts of this data make it sometimes difficult to take proper advantage of
+it. GNSS visualizer aims to make this easier by providing easy to use tool that
+can be used to explore the data.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built with The interface and all the plots are built using awesome [Bokeh]
-(https://bokeh.org/) library. Parsing of ubx messages leverages [pyubx2](https:
-//github.com/semuconsulting/pyubx2) library.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting started ### Installation via pip ```sh python -m pip install gnss-
-visualizer ```
+(https://bokeh.org/) library. Bokeh gives lots of power for creating pretty
+plots with nice interactive features including callbacks to python code.
+Parsing of ubx messages leverages [pyubx2](https://github.com/semuconsulting/
+pyubx2) library.
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Getting started ### Prequisites - Python 3.11 or later. Earlier versions
+might work but are not tested. ### Installation via pip ```sh python -m pip
+install gnss-visualizer ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage After installing, the tool provides a command `gnss-visualizer` that
 can be used to launch the tool and open the UI in a web browser. ### Reading
-ubx files Analyzing an ubx file can be done in the following way: ```sh gnss-
-visualizer ~/path/to/file.ubx -w 1 ``` where -w (shorthand for --simulate-wait-
-s) is used to add delay of 1 second after each UBX-NAV-PVT message. This will
-make files with 1 Hz navigation rate playback as if they were done in (almost)
-realtime. The input file should contain UBX-NAV-PVT message and in order to
-generate signal and satellite based plots also UBX-NAV-SIG message. ### Reading
-serial devices Data can be read also from a serial device using: ```sh gnss-
-visualizer /dev/ttyUSB0 ``` ### Details `gnss-visualizer` command can be
-substituted to `bokeh serve src/gnss_visualizer --show --args INPUT` and in
-case the bokeh serve command needs to be modified, it can simply be used
-manually instead of calling `gnss-visualizer`.
-                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
-## Roadmap - [ ] Tests - [ ] Github CICD - [ ] Plot selection mechanism - [ ]
-Make plotting module with classess for different plots - [ ] Set up whole file
-reading for timeseries plots - [ ] More plots - [ ] Allow playback after
-reading the whole file - [ ] Configurable wait delay - [ ] Non-ubx file support
-(some basic plots?) - [ ] Even more plots - [ ] Truth location handling
-(coordinates / files) - [ ] Lots more plots - [ ] UI for file input See the
-[open issues](https://github.com/othneildrew/Best-README-Template/issues) for a
-full list of proposed features (and known issues).
+ubx files in playback mode Analyzing an ubx file in playback mode can be done
+in the following way: ```sh gnss-visualizer ~/path/to/file.ubx -w 1 ``` where -
+w (shorthand for --default-simulate-wait-s) is used to add delay of 1 second
+after each UBX-NAV-PVT message. This will make files with 1 Hz navigation rate
+playback as if they were done in (almost) realtime. The input file should
+contain UBX-NAV-PVT messages and in order to generate signal and satellite
+based plots also UBX-NAV-SIG messages. For testing purposes the repository
+contains a file `coldstart.ubx` that can be used to test the tool. It contains
+data from a coldstart of a stationary receiver. ### Reading serial devices Data
+can be read also from a serial device using: ```sh gnss-visualizer /dev/ttyUSB0
+``` ### Details `gnss-visualizer` command can be substituted to `bokeh serve
+src/gnss_visualizer --show --args INPUT` and in case the bokeh serve command
+needs to be modified, it can simply be used manually instead of calling `gnss-
+visualizer`.
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
+## Roadmap - [x] Test setup - [x] Github CICD - [ ] Tests - [x] Plot selection
+mechanism - [x] Make plotting module with classess for different plots - [ ]
+Set up whole file reading for timeseries plots - [ ] More plots - [x] Allow
+playback after reading the whole file - [x] Configurable wait delay - [ ] Non-
+ubx file support (some basic plots?) - [ ] Even more plots - [ ] Truth location
+handling (coordinates / files) - [ ] Lots more plots - [ ] UI for file input
+See the [open issues](https://github.com/othneildrew/Best-README-Template/
+issues) for a full list of proposed features (and known issues).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
-issue. Don't forget to give the project a star! Thanks again! 1. Fork the
-Project 2. Create your Feature Branch (`git checkout -b feature/
-AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
-AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request
+issue. Don't forget to give the project a star! Thanks again! ### Setting up a
+local repository 1. Fork the project 2. Clone the forked project 3. Install
+dependencies (`pip install -r requirements.txt && pip install -r requirements-
+dev.txt`) 4. Install the project in editable mode (`pip install -e .`) 5.
+Install pre-commit (`pipx install pre-commit`) 5. Install pre-commit hooks
+(`pre-commit install`) ### Steps to contribute 1. Set up a local repository 2.
+Create your feature branch (`git checkout -b feature/AmazingFeature`) 3. Commit
+your changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the branch
+(`git push origin feature/AmazingFeature`) 5. Open a pull request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the AGPL-3.0 license. See `LICENSE` for more
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact Ville Joensuu - [Linkedin](https://www.linkedin.com/in/ville-
 joensuu-dev/) - jopppis@iki.fi Project Link: [https://github.com/jopppis/gnss-
 visualizer](https://github.com/jopppis/gnss-visualizer)
```

### Comparing `gnss_visualizer-0.0.6/pyproject.toml` & `gnss_visualizer-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gnss-visualizer"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
   "pyubx2",
   "bokeh",
   "pyserial",
   "xyzservices",
   "pyproj",
 ]
@@ -39,14 +39,27 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/gnss_visualizer"]
 
 [project.scripts]
 gnss-visualizer = "gnss_visualizer.run_server:main"
 
+[tool.mypy]
+strict = true
+exclude = ["tests/"]
+
+[[tool.mypy.overrides]]
+module = [
+    "pyubx2",
+    "xyzservices",
+    "xyzservices.providers",
+    "serial"
+]
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `gnss_visualizer-0.0.6/PKG-INFO` & `gnss_visualizer-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gnss-visualizer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Visualize GNSS data in a web browser
 Project-URL: Homepage, https://github.com/jopppis/gnss-visualizer
 Project-URL: Documentation, https://github.com/jopppis/gnss-visualizer
 Project-URL: Repository, https://github.com/jopppis/gnss-visualizer.git
 Project-URL: Bug Tracker, https://github.com/jopppis/gnss-visualizer/issues
 Project-URL: Changelog, https://github.com/jopppis/gnss-visualizer/blob/main/CHANGELOG.md
 Author-email: Ville Joensuu <ville.joensuu@iki.fi>
@@ -743,55 +743,65 @@
 
 GNSS visualizer is a tool for visualizing GNSS data in an interactive environment.
 
 ![GNSS visualizer screenshot](https://github.com/jopppis/gnss-visualizer/assets/25751262/4b94577d-ca44-40c9-b3b9-71b695eca2f6)
 
 It is designed to offer a simple interface in a web browser with ever extending plotting capabilities.
 
+The tool is still in very early development so don't expect much just yet!
+
+
+GNSS receivers collect lots of information about the satellites and the signals they observe which can help to understand the quality of the positioning solution and the behavior of the receiver. Vast amounts of this data make it sometimes difficult to take proper advantage of it. GNSS visualizer aims to make this easier by providing easy to use tool that can be used to explore the data.
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built with
 
-The interface and all the plots are built using awesome [Bokeh](https://bokeh.org/) library.
+The interface and all the plots are built using awesome [Bokeh](https://bokeh.org/) library. Bokeh gives lots of power for creating pretty plots with nice interactive features including callbacks to python code.
 
 Parsing of ubx messages leverages [pyubx2](https://github.com/semuconsulting/pyubx2) library.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ## Getting started
 
+### Prequisites
+- Python 3.11 or later. Earlier versions might work but are not tested.
+
 ### Installation via pip
 
 ```sh
 python -m pip install gnss-visualizer
 ```
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 ## Usage
 After installing, the tool provides a command `gnss-visualizer` that can be used to launch the tool and open the UI in a web browser.
 
 
-### Reading ubx files
-Analyzing an ubx file can be done in the following way:
+### Reading ubx files in playback mode
+Analyzing an ubx file in playback mode can be done in the following way:
 ```sh
 gnss-visualizer ~/path/to/file.ubx -w 1
 ```
-where -w (shorthand for --simulate-wait-s) is used to add delay of 1 second after each UBX-NAV-PVT message. This will make files with 1 Hz navigation rate playback as if they were done in (almost) realtime.
+where -w (shorthand for --default-simulate-wait-s) is used to add delay of 1 second after each UBX-NAV-PVT message. This will make files with 1 Hz navigation rate playback as if they were done in (almost) realtime.
 
-The input file should contain UBX-NAV-PVT message and in order to generate signal and satellite based plots also UBX-NAV-SIG message.
+The input file should contain UBX-NAV-PVT messages and in order to generate signal and satellite based plots also UBX-NAV-SIG messages.
 
 
+For testing purposes the repository contains a file `coldstart.ubx` that can be used to test the tool. It contains data from a coldstart of a stationary receiver.
+
 ### Reading serial devices
 Data can be read also from a serial device using:
 ```sh
 gnss-visualizer /dev/ttyUSB0
 ```
 
 ### Details
@@ -802,22 +812,23 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ## Roadmap
 
+- [x] Test setup
+- [x] Github CICD
 - [ ] Tests
-- [ ] Github CICD
-- [ ] Plot selection mechanism
-- [ ] Make plotting module with classess for different plots
+- [x] Plot selection mechanism
+- [x] Make plotting module with classess for different plots
 - [ ] Set up whole file reading for timeseries plots
 - [ ] More plots
-- [ ] Allow playback after reading the whole file
-- [ ] Configurable wait delay
+- [x] Allow playback after reading the whole file
+- [x] Configurable wait delay
 - [ ] Non-ubx file support (some basic plots?)
 - [ ] Even more plots
 - [ ] Truth location handling (coordinates / files)
 - [ ] Lots more plots
 - [ ] UI for file input
 
 See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).
@@ -829,19 +840,31 @@
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue.
 Don't forget to give the project a star! Thanks again!
 
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
+### Setting up a local repository
+
+1. Fork the project
+2. Clone the forked project
+3. Install dependencies (`pip install -r requirements.txt && pip install -r requirements-dev.txt`)
+4. Install the project in editable mode (`pip install -e .`)
+5. Install pre-commit (`pipx install pre-commit`)
+5. Install pre-commit hooks (`pre-commit install`)
+
+### Steps to contribute
+
+1. Set up a local repository
+2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the branch (`git push origin feature/AmazingFeature`)
+5. Open a pull request
+
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 ## License
 
 Distributed under the AGPL-3.0 license. See `LICENSE` for more information.
```

