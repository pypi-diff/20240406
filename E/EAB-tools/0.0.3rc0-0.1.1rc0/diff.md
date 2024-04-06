# Comparing `tmp/EAB_tools-0.0.3rc0.tar.gz` & `tmp/EAB_tools-0.1.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EAB_tools-0.0.3rc0.tar", last modified: Tue Jun 20 16:15:47 2023, max compression
+gzip compressed data, was "EAB_tools-0.1.1rc0.tar", last modified: Sat Apr  6 12:33:21 2024, max compression
```

## Comparing `EAB_tools-0.0.3rc0.tar` & `EAB_tools-0.1.1rc0.tar`

### file list

```diff
@@ -1,34 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/_testing/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/_testing/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/eab_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/io/
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/io/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/io/filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/util/test_hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/util/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/util/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 16:15:47.946732 EAB_tools-0.0.3rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.075733 EAB_tools-0.1.1rc0/EAB_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.075733 EAB_tools-0.1.1rc0/EAB_tools/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.075733 EAB_tools-0.1.1rc0/EAB_tools/_testing/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/test_scripts/generate_all_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24599 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/test_scripts/generate_fake_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/_testing/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18775 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/eab_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/io/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/io/enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/io/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/io/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools/tests/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/_testing/test_data_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/io/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/io/test_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/io/test_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/io/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/tests/util/test_hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/EAB_tools/util/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/EAB_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-06 12:33:21.000000 EAB_tools-0.1.1rc0/EAB_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-06 12:33:21.000000 EAB_tools-0.1.1rc0/EAB_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:33:21.000000 EAB_tools-0.1.1rc0/EAB_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-06 12:33:21.000000 EAB_tools-0.1.1rc0/EAB_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 12:33:21.000000 EAB_tools-0.1.1rc0/EAB_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:33:21.079733 EAB_tools-0.1.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 12:33:16.000000 EAB_tools-0.1.1rc0/setup.py
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/_testing/io.py` & `EAB_tools-0.1.1rc0/EAB_tools/_testing/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import tkinter
 from types import TracebackType
 
+from matplotlib.backends.backend_tkagg import FigureManagerTk
 import matplotlib.pyplot as plt
 
 from EAB_tools._testing.types import PathLike
 
 
 def _is_tkinter_error(
     err: tuple[type, Exception, TracebackType],
     *args: object,  # Flaky will pass more objects that I don't care about
 ) -> bool:
     return isinstance(err[1], tkinter.TclError)
 
 
 def _test_photos_are_equal(base: PathLike, other: PathLike) -> bool:
-    # https://stackoverflow.com/a/34669225
-    return open(base, "rb").read() == open(other, "rb").read()
+    # https://chat.openai.com/share/70244426-80d9-4668-b476-6bc36946cc6f
+    base, other = str(base), str(other)  # for mypy
+    return (plt.imread(base) == plt.imread(other)).all()
 
 
 def _minimize_tkagg() -> None:
     if plt.get_backend().casefold() == "tkagg":
         # Rapidly minimizes the window to prevent strobing effect.
         # Works on my Windows 10, at least...
-        plt.get_current_fig_manager().window.state("iconic")
+        fig_manager = plt.get_current_fig_manager()
+        assert isinstance(fig_manager, FigureManagerTk)
+        fig_manager.window.state("iconic")
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/io/display.py` & `EAB_tools-0.1.1rc0/EAB_tools/io/display.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 """Methods to display and save DataFrames, plots."""
+
+from __future__ import annotations
+
 from collections.abc import Sequence
-import os
 from pathlib import Path
-from typing import (
-    Any,
-    Optional,
-    Union,
-)
+from typing import Any
 import warnings
 
 from IPython.display import display
-import dataframe_image as dfi  # noqa
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", DeprecationWarning)
+    import dataframe_image as dfi  # noqa
+
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from pandas.io.formats.style import (
     Styler,
     Subset,
 )
 
 from EAB_tools.io.filenames import (
+    PathLike,
     sanitize_filename,
     sanitize_xl_sheetname,
 )
 from EAB_tools.util.hashing import (
     hash_df,
     hash_mpl_fig,
 )
 
-PathLike = Union[str, os.PathLike, Path]
-
 # Copied from Excel's conditional formatting Red-Yellow-Green built-in colormap.
 _xl_RYG_colors = ["#F8696B", "#FFEB84", "#63BE7B"]
-xl_RYG_cmap = plt.cm.colors.LinearSegmentedColormap.from_list(
+xl_RYG_cmap = mpl.colors.LinearSegmentedColormap.from_list(
     "xl_RYG_cmap", _xl_RYG_colors
 )
 xl_GYR_cmap = xl_RYG_cmap.reversed()
 
 
 def _to_excel(
     df: pd.DataFrame,
     styler: Styler,
-    filepath: Path,
-    percentage_format_subset: Optional[Union[Subset, str]],
-    thousands_format_subset: Optional[Union[Subset, str]],
-    bar_subset: Optional[Union[Subset, str]],
+    excel_output: Path,
+    sheet_name: PathLike | None,
+    percentage_format_subset: Subset | str | None,
+    thousands_format_subset: Subset | str | None,
+    bar_subset: Subset | str | None,
     date_format: str,
     percentage_format_precision: int,
-    bar_vmin: Optional[float],
-    bar_vmax: Optional[float],
+    bar_vmin: float | None,
+    bar_vmax: float | None,
 ) -> None:
     """Export DataFrame to Excel. Used as a helper function to display_and_save_df."""
     try:
         import openpyxl
     except ImportError as e:
         raise ImportError("openpyxl is required for Excel functionality") from e
 
-    excel_output = filepath.parent / "output.xlsx"
     # Determine ExcelWriter params based on if the file exists or not
     mode, if_sheet_exists = ("a", "replace") if excel_output.exists() else ("w", None)
 
     # Determine an Excel sheet name:
-    sn = filepath.name.replace(".png", "")
-    sn = sanitize_xl_sheetname(sn)
+    if sheet_name is None:
+        sheet_name = excel_output.name.replace(".png", "").replace(".xlsx", "")
+    sheet_name = Path(sheet_name)
+    sheet_name = sheet_name.name.replace(".df.png", "").replace(".png", "")
+    sheet_name = sanitize_xl_sheetname(sheet_name)
 
     # Excel does NOT support datetimes with timezones
     for col in df.select_dtypes(["datetime", "datetimetz"]).columns:
         df[col] = df[col].dt.tz_localize(None)
         styler.data[col] = df[col]
         styler = styler.format(f"{{:{date_format}}}", subset=col)
 
     # Export to Excel:
     with pd.ExcelWriter(
         excel_output, engine="openpyxl", mode=mode, if_sheet_exists=if_sheet_exists
     ) as wb:
         print(
             f"Exporting to Excel as '{excel_output.resolve().parent}\\"
-            f"[{excel_output.name}]{sn}'",
+            f"[{excel_output.name}]{sheet_name}'",
             end=" ... ",
         )
-        styler.to_excel(wb, sheet_name=sn, engine="openpyxl")
+        styler.to_excel(wb, sheet_name=sheet_name, engine="openpyxl")
 
         if (
             percentage_format_subset is not None
             or thousands_format_subset is not None
             or bar_subset is not None
         ):
             # Number formatting doesn't seem to carry over to
@@ -98,32 +103,54 @@
             if isinstance(thousands_format_subset, str):
                 thousands_format_subset = [thousands_format_subset]
             if isinstance(bar_subset, str):
                 bar_subset = [bar_subset]
             len_index = df.index.nlevels
 
             # Get the worksheet
-            ws: openpyxl.workbook.workbook.Worksheet = wb.book[sn]
+            sheet_name = next(
+                sheet
+                for sheet in wb.book.sheetnames
+                if sheet.casefold() == sheet_name.casefold()
+            )
+            ws: openpyxl.workbook.workbook.Worksheet = wb.book[sheet_name]
 
             # Determine the 0-based pd indices for number formatting
             pcnt_cols = (
                 [df.columns.get_loc(col) for col in percentage_format_subset]
                 if percentage_format_subset is not None
                 else []
             )
+            try:
+                # Check if we have a list containing a list
+                iter(pcnt_cols[0])
+                pcnt_cols = pcnt_cols[0]
+            except (TypeError, IndexError):
+                # We just have a normal list
+                pass
             tsnd_cols = (
                 [df.columns.get_loc(col) for col in thousands_format_subset]
                 if thousands_format_subset is not None
                 else []
             )
-            bar_cols = (
-                [df.columns.get_loc(col) for col in bar_subset]
-                if bar_subset is not None
-                else []
-            )
+            try:
+                if isinstance(bar_subset, (list, tuple)) and len(bar_subset) > 1:
+                    # If `bar_subset` is a tuple, then it's
+                    # (rows, cols)
+                    bar_subset = bar_subset[1]
+                bar_cols = (
+                    [df.columns.get_loc(col) for col in bar_subset]
+                    if bar_subset is not None
+                    else []
+                )
+            except TypeError:
+                # `bar_subset`` contains more than just columns.
+                # For now, we must abort trying to export data bar conditional
+                # formatting.
+                bar_cols = []
 
             # Iterate through the columns, applying styles to all
             # cells in a column
             for col_num, col in enumerate(ws.iter_cols()):
                 # Apply percentage, thousands number formats
                 if np.any(col_num - len_index in pcnt_cols):
                     for cell in col:
@@ -158,44 +185,45 @@
                     # I could not even find the function
                     # ws.conditional_formatting.add() in the openpyxl docs. Thank
                     # god for https://stackoverflow.com/a/32454012.
                     ws.conditional_formatting.add(xl_range, rule)
 
 
 def display_and_save_df(
-    df: Union[pd.DataFrame, pd.Series, Styler],
-    caption: Optional[str] = None,
-    filename: Optional[PathLike] = None,
+    df: pd.DataFrame | pd.Series | Styler,
+    caption: str | None = None,
+    filename: PathLike | None = None,
     large_title: bool = True,
     large_col_names: bool = True,
     cell_borders: bool = True,
     highlight_total_row: bool = False,
     border_width: str = "1px",
-    thousands_format_subset: Optional[Union[Subset, str]] = "auto",
-    date_format_subset: Optional[Union[Subset, str]] = "auto",
+    thousands_format_subset: Subset | str | None = "auto",
+    date_format_subset: Subset | str | None = "auto",
     date_format: str = "%#m/%#d/%Y",
-    percentage_format_subset: Optional[Union[Subset, str]] = "auto",
+    percentage_format_subset: Subset | str | None = "auto",
     percentage_format_precision: int = 1,
-    float_format_subset: Optional[Union[Subset, str]] = "auto",
+    float_format_subset: Subset | str | None = "auto",
     float_format_precision: int = 1,
     hide_index: bool = False,
     convert_dtypes: bool = True,
-    ryg_bg_subset: Optional[Union[Subset, str]] = None,
-    ryg_bg_vmin: Optional[float] = None,
-    ryg_bg_vmax: Optional[float] = None,
-    gyr_bg_subset: Optional[Union[Subset, str]] = None,
-    gyr_bg_vmin: Optional[float] = None,
-    gyr_bg_vmax: Optional[float] = None,
-    bar_subset: Optional[Union[Subset, str]] = None,
-    bar_vmin: Optional[float] = None,
-    bar_vmax: Optional[float] = None,
-    format_kwargs: Optional[Sequence[dict[str, Any]]] = None,
-    background_gradient_kwargs: Optional[Sequence[dict[str, Any]]] = None,
-    bar_kwargs: Optional[Sequence[dict[str, Any]]] = None,
+    ryg_bg_subset: Subset | str | None = None,
+    ryg_bg_vmin: float | None = None,
+    ryg_bg_vmax: float | None = None,
+    gyr_bg_subset: Subset | str | None = None,
+    gyr_bg_vmin: float | None = None,
+    gyr_bg_vmax: float | None = None,
+    bar_subset: Subset | str | None = None,
+    bar_vmin: float | None = None,
+    bar_vmax: float | None = None,
+    format_kwargs: Sequence[dict[str, Any]] | None = None,
+    background_gradient_kwargs: Sequence[dict[str, Any]] | None = None,
+    bar_kwargs: Sequence[dict[str, Any]] | None = None,
     save_excel: bool = False,
+    excel_path: PathLike = "output.xlsx",
     save_image: bool = False,
     min_width: str = "10em",
     max_width: str = "25em",
 ) -> Styler:
     """
     Display and save a pandas DataFrame or Styler object.
 
@@ -433,15 +461,15 @@
             # But don't accept cols that are a string dtype
             percentage_format_subset_mask &= [
                 not pd.api.types.is_string_dtype(df[col]) for col in df
             ]
             percentage_format_subset = df.columns[percentage_format_subset_mask]
         except AttributeError as e:
             # Can only use .str accessor with Index, not MultiIndex
-            warnings.warn(str(e))
+            warnings.warn(str(e), stacklevel=2)
             percentage_format_subset = []
     # Apply the percentage format
     if percentage_format_subset is not None:
         formatter = f"{{:.{percentage_format_precision}%}}"
         styler = styler.format(formatter=formatter, subset=percentage_format_subset)
 
     # Apply thousands seperator
@@ -533,15 +561,16 @@
         styler.export_png(str(filename), fontsize=16, max_rows=200, max_cols=200)
 
     # Save the Styler to Excel sheet
     if save_excel:
         _to_excel(
             df=df,
             styler=styler,
-            filepath=filename,
+            excel_output=Path(excel_path),
+            sheet_name=filename,
             percentage_format_subset=percentage_format_subset,
             thousands_format_subset=thousands_format_subset,
             bar_subset=bar_subset,
             date_format=date_format,
             percentage_format_precision=percentage_format_precision,
             bar_vmin=bar_vmin,
             bar_vmax=bar_vmax,
@@ -550,16 +579,16 @@
     # Finally, display with styler with IPython
     display(styler)
 
     return styler
 
 
 def display_and_save_fig(
-    fig: Union[plt.Figure, plt.Axes],
-    filename: Optional[str] = None,
+    fig: plt.Figure | plt.Axes,
+    filename: str | None = None,
     save_image: bool = False,
 ) -> None:
     """
     Display and save a `matplotlib` figure.
 
     Displays and saves and `matplotlib` `Figure` or `Axes` with the default `matplotlib`
     backend and optionally saves the image to disk as a png.
@@ -592,30 +621,29 @@
     plt.show(block=False)
 
     if not save_image:
         # If we're not saving the image, then this is the end of the function.
         return
 
     # If they passed an `Axes` object, get the `Figure`
-    if isinstance(fig, plt.Axes):
-        fig = fig.get_figure()
-    fig.canvas.draw()
+    figure = fig.get_figure() if isinstance(fig, plt.Axes) else fig
+    assert figure is not None  # for `mypy`
 
     # Attempt to infer the filename if it is None
     if filename is None:
-        if fig._suptitle is not None:
-            filename = fig._suptitle.get_text()
-        elif fig.axes[0].title.get_text() != "":
-            filename = fig.axes[0].title.get_text()
+        if figure._suptitle is not None:  # type: ignore[attr-defined]
+            filename = figure._suptitle.get_text()  # type: ignore[attr-defined]
+        elif figure.axes[0].title.get_text() != "":
+            filename = figure.axes[0].title.get_text()
         else:
-            filename = hash_mpl_fig(fig)
+            filename = hash_mpl_fig(figure)
     filename = sanitize_filename(filename)
 
     # Needed to make `mypy` happy
     filename = str(filename)
     if filename[-4:] != ".png":
         filename = filename + ".png"
 
     filepath = Path(filename)
 
     print(f"Saving as {filepath} ... ", end="")
-    fig.savefig(filepath)
+    figure.savefig(filepath)
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/io/filenames.py` & `EAB_tools-0.1.1rc0/EAB_tools/io/filenames.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Utilities for dealing with filenames and Excel sheet names."""
 
+import os
+from pathlib import Path
 import re
+from typing import Union
 
+PathLike = Union[str, os.PathLike[str], Path]
 
-def sanitize_filename(filename: str) -> str:
+
+def sanitize_filename(filename: PathLike) -> str:
     """
     Ensure valid filenames.
 
     Given a filename, remove all characters that are
     potentially hazardous in a filename.
     The only chars allowed are
 
@@ -32,18 +37,19 @@
     sanitize_xl_sheetname : Ensure valid Excel sheetnames.
 
     Examples
     --------
     >>> sanitize_filename('python is fun 🐍.py')
     'python is fun _.py'
     """
+    filename = str(filename)
     return re.sub(r"[^\w\-_. ()]", "_", filename)
 
 
-def sanitize_xl_sheetname(sheetname: str) -> str:
+def sanitize_xl_sheetname(sheetname: PathLike) -> str:
     """
     Ensure valid Excel sheetnames.
 
     This function replaces most invalid characters with underscores and
     truncates the sheetname to an appropriate size.
 
     Parameters
@@ -63,14 +69,15 @@
     Examples
     --------
     >>> sanitize_xl_sheetname("9:00 AM")
     '9_00 AM'
     >>> sanitize_xl_sheetname("'single quoted'")
     '_single quoted_'
     """
+    sheetname = str(sheetname)
     # A worksheet cannot be named history, regardless of case
     # A worksheet name cannot be left blank
     if sheetname == "" or sheetname.lower() == "history":
         raise ValueError(f'Invalid sheet name "{sheetname}"')
 
     # A sheetname cannot start or end with an apostrophe
     sheetname = re.sub(r"^'|'$", "_", sheetname)
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_display.py` & `EAB_tools-0.1.1rc0/EAB_tools/tests/io/test_display.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # pylint: disable=C0114, C0116
+from __future__ import annotations
+
 from collections.abc import Sequence
-from contextlib import nullcontext as does_not_raise
 import itertools
-import os
 from pathlib import Path
 import re
 from typing import (
     Any,
     ContextManager,
-    Optional,
-    Union,
 )
 
 from matplotlib import pyplot as plt
 import pandas as pd
 import pytest
 
 import EAB_tools as eab
@@ -28,19 +26,14 @@
     import openpyxl as _openpyxl  # noqa: F401 # 'openpyxl ... imported but unused
 
     _HAS_OPENPYXL = True
 except ImportError:
     _HAS_OPENPYXL = False
 
 
-@pytest.fixture(autouse=True)
-def _init(tmp_path: Path) -> None:
-    os.chdir(tmp_path)
-
-
 SaveImageTrueParam = pytest.param(True, marks=pytest.mark.slow)
 SaveExcelTrueParam = pytest.param(
     True, marks=pytest.mark.skipif(not _HAS_OPENPYXL, reason="openpyxl required")
 )
 
 
 @pytest.mark.parametrize(
@@ -68,15 +61,15 @@
         self, iris: pd.DataFrame, save_image: bool, save_excel: bool
     ) -> None:
         iris_mi = iris.set_index("Name", append=True)
         display_and_save_df(iris_mi, save_image=save_image, save_excel=save_excel)
         display_and_save_df(iris_mi.T, save_image=save_image, save_excel=save_excel)
 
     @staticmethod
-    def col_name_from_iris_single_col_subset(col_name: Union[str, pd.Index]) -> str:
+    def col_name_from_iris_single_col_subset(col_name: str | pd.Index) -> str:
         return col_name if isinstance(col_name, str) else col_name[0]
 
     @pytest.mark.parametrize(
         "kwargs",
         [
             pytest.param(
                 {
@@ -119,15 +112,15 @@
                 id="float.2f",
             ),
         ],
     )
     def test_styler_expected_text(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         kwargs: dict[str, Any],
         save_image: bool,
         save_excel: bool,
     ) -> None:
         """Test for expected text in Stylers"""
         iris, kwargs = iris.copy(), kwargs.copy()
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
@@ -145,17 +138,17 @@
             an_expected_value = kwargs.pop("format").format(an_expected_value)
         except ValueError:
             # Number formatting can't be applied to str
             # Just make sure everything goes ok
             an_expected_value = ""
 
         if pd.api.types.is_string_dtype(col):
-            context: ContextManager[Optional[object]] = pytest.raises(ValueError)
+            context: ContextManager[object | None] = pytest.raises(ValueError)
         else:
-            context = does_not_raise()
+            context = tm.does_not_raise()
         with context:
             # str columns with incorrect format code should
             # throw a ValueError
 
             # d is really dict[str, Union[str, pd.Index]], but mypy complains
             d: dict[str, Any] = {
                 kwargs.pop("display_and_save_kw"): iris_single_col_subset
@@ -321,27 +314,27 @@
         html_with_index = styler_with_index.to_html()
 
         assert all(name in html_with_index for name in iris.index.unique())
 
     def test_ryg_background_gradient(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         # Should get ValueError on string dtypes
         if pd.api.types.is_string_dtype(iris[col_name]):
-            context: ContextManager[Optional[object]] = pytest.raises(
+            context: ContextManager[object | None] = pytest.raises(
                 ValueError, match="could not convert string to float"
             )
         else:
-            context = does_not_raise()
+            context = tm.does_not_raise()
 
         with context:
             styler = display_and_save_df(
                 iris,
                 ryg_bg_subset=iris_single_col_subset,
                 save_image=save_image,
                 save_excel=save_excel,
@@ -351,15 +344,15 @@
             expected_max_color = "background-color: #63be7b"
             assert expected_min_color.casefold() in html.casefold()
             assert expected_max_color.casefold() in html.casefold()
 
     def test_ryg_background_vmin(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
 
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
@@ -383,15 +376,15 @@
 
         assert expected_min_color.casefold() not in html
         assert expected_max_color.casefold() in html
 
     def test_ryg_background_vmax(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
 
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
@@ -413,15 +406,15 @@
 
         assert expected_min_color.casefold() in html
         assert expected_max_color.casefold() not in html
 
     def test_gyr_background_vmin(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
             return
@@ -444,15 +437,15 @@
 
         assert expected_min_color.casefold() not in html
         assert expected_max_color.casefold() in html
 
     def test_gyr_background_vmax(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
             return
@@ -473,15 +466,15 @@
 
         assert expected_min_color.casefold() in html
         assert expected_max_color.casefold() not in html
 
     def test_bar_style(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
             # Can't apply bar format to string dtype columns
@@ -508,15 +501,15 @@
         pcnts = re.findall(regexp, html)
         series = pd.Series(pcnts, dtype=float)
         return series
 
     def test_bar_vmin(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
             return
@@ -540,15 +533,15 @@
         regular_pcnts = self.bar_pcnt_from_html(regular_styler.to_html())
         vmin_pcnts = self.bar_pcnt_from_html(vmin_styler.to_html())
         assert (vmin_pcnts >= regular_pcnts).all()
 
     def test_bar_vmax(
         self,
         iris: pd.DataFrame,
-        iris_single_col_subset: Union[str, pd.Index],
+        iris_single_col_subset: str | pd.Index,
         save_image: bool,
         save_excel: bool,
     ) -> None:
         col_name = self.col_name_from_iris_single_col_subset(iris_single_col_subset)
 
         if pd.api.types.is_string_dtype(iris[col_name]):
             return
@@ -582,15 +575,15 @@
     def display_and_save_fig(self, *args: Any, **kwargs: Any) -> None:
         from EAB_tools.io.display import display_and_save_fig as display_and_save_fig_og
 
         display_and_save_fig_og(*args, **kwargs)
         tm._minimize_tkagg()
 
     def test_doesnt_fail(
-        self, mpl_figs_and_axes: Union[plt.Figure, plt.Axes], save_image: bool
+        self, mpl_figs_and_axes: plt.Figure | plt.Axes, save_image: bool
     ) -> None:
         display_and_save_fig(mpl_figs_and_axes, save_image=save_image)
 
     def test_expected_output(
         self,
         save_image: bool,
         iris: pd.DataFrame,
@@ -616,30 +609,32 @@
             Path(__file__).parent / "data" / "test_expected_output.png",
         )
         plt.close(fig)
 
     def test_infer_filename_from_fig_suptitle(
         self,
         save_image: bool,
-        mpl_figs_and_axes: Union[plt.Figure, plt.Axes],
+        mpl_figs_and_axes: plt.Figure | plt.Axes,
     ) -> None:
         fig: plt.Figure
         if isinstance(mpl_figs_and_axes, plt.Axes):
-            fig = mpl_figs_and_axes.get_figure()
+            get_figure = mpl_figs_and_axes.get_figure()
+            assert get_figure is not None  # for `mypy`
+            fig = get_figure
         else:
             fig = mpl_figs_and_axes
 
         name = sanitize_filename(str(fig))
         fig.suptitle(name)
 
         display_and_save_fig(mpl_figs_and_axes, save_image=True)
         assert Path(f"{name}.png").exists()
 
     def test_infer_filename_from_axis(
-        self, save_image: bool, mpl_figs_and_axes: Union[plt.Figure, plt.Axes]
+        self, save_image: bool, mpl_figs_and_axes: plt.Figure | plt.Axes
     ) -> None:
         if isinstance(mpl_figs_and_axes, plt.Figure):
             axes: plt.Axes = mpl_figs_and_axes.axes[0]
         else:
             axes = mpl_figs_and_axes
 
         # Pretty random name
@@ -648,13 +643,13 @@
 
         display_and_save_fig(mpl_figs_and_axes, save_image=True)
         assert Path(f"{name}.png").exists()
 
     def test_filename_from_hash(
         self,
         save_image: bool,
-        mpl_figs_and_axes: Union[plt.Figure, plt.Axes],
+        mpl_figs_and_axes: plt.Figure | plt.Axes,
     ) -> None:
         expected_hash = eab.util.hash_mpl_fig(mpl_figs_and_axes)
         display_and_save_fig(mpl_figs_and_axes, save_image=True)
 
         assert Path(f"{expected_hash}.png").exists()
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_filenames.py` & `EAB_tools-0.1.1rc0/EAB_tools/tests/io/test_filenames.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/tests/util/test_hashing.py` & `EAB_tools-0.1.1rc0/EAB_tools/tests/util/test_hashing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for hashing"""
+
 from typing import Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 
@@ -90,10 +91,10 @@
 
     def test_sensitivity(self, mpl_axes: plt.Axes, seed: int = 0) -> None:
         a = hash_mpl_fig(mpl_axes)
 
         rng = np.random.default_rng(seed=seed)
         xy = rng.random(2)
         color = rng.random(3)
-        mpl_axes.scatter(*xy, c=color)
+        mpl_axes.scatter(xy[0], xy[1], color=color)
         b = hash_mpl_fig(mpl_axes)
         assert a != b
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools/util/hashing.py` & `EAB_tools-0.1.1rc0/EAB_tools/util/hashing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Utilities for hashing objects."""
+
+from __future__ import annotations
+
 import hashlib
-from typing import (
-    Optional,
-    Union,
-)
+from typing import cast
 
+from matplotlib.backends.backend_agg import FigureCanvasAgg
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pandas.io.formats.style
 
 from EAB_tools.eab_rc import eab_rc
 
 
 def hash_df(
-    df: Union[pd.DataFrame, pd.Series, pd.Index, pd.MultiIndex],
-    styler: Optional[pd.io.formats.style.Styler] = None,
-    max_len: Optional[int] = eab_rc["hash_len"],
+    df: pd.DataFrame | pd.Series | pd.Index | pd.MultiIndex,
+    styler: pd.io.formats.style.Styler | None = None,
+    max_len: int | None = eab_rc["hash_len"],
     usedforsecurity: bool = False,
 ) -> str:
     """
     Create a unique hash for a pandas object.
 
     Parameters
     ----------
@@ -59,21 +60,23 @@
     if styler is not None:
         h.update(styler.to_html().encode("UTF8"))
 
     return h.hexdigest()[:max_len]
 
 
 def hash_mpl_fig(
-    fig: Union[plt.Figure, plt.Axes],
-    max_len: Optional[int] = eab_rc["hash_len"],
+    fig: plt.Figure | plt.Axes,
+    max_len: int | None = eab_rc["hash_len"],
     usedforsecurity: bool = False,
 ) -> str:
     """Hash a matplotlib figure."""
-    if isinstance(fig, plt.Axes):
-        fig = fig.get_figure()
-    fig.canvas.draw()
-    buf = fig.canvas.buffer_rgba()
+    figure = fig.get_figure() if isinstance(fig, plt.Axes) else fig
+    assert figure is not None
+
+    canvas: FigureCanvasAgg = cast(FigureCanvasAgg, figure.canvas)
+    canvas.draw()
+    buf = canvas.buffer_rgba()
     X = np.asarray(buf).tobytes()
 
     h = hashlib.sha1(usedforsecurity=usedforsecurity)
     h.update(X)
     return h.hexdigest()[:max_len]
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools.egg-info/PKG-INFO` & `EAB_tools-0.1.1rc0/EAB_tools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: EAB-tools
-Version: 0.0.3rc0
+Name: EAB_tools
+Version: 0.1.1rc0
 Summary: Tools for analyzing data exported from the EAB Navigate Student Success Management Software.
 Author: Moshe Rubin
 Author-email: Moshe Rubin <mosherubin137@gmail.com>
 License: MIT License
         
         Copyright 2022 Moshe Rubin https://github.com/moshemoshe137
         
@@ -35,14 +35,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dataframe_image
+Requires-Dist: ipython
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Provides-Extra: progress-bar
+Requires-Dist: tqdm; extra == "progress-bar"
 
 # EAB Tools
 [![License: MIT](https://img.shields.io/github/license/moshemoshe137/EAB_tools)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/EAB_tools)](https://pypi.org/project/EAB-tools/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -99,10 +105,40 @@
 
 Installing EAB tools will install these packages and their dependencies:
 
 - [pandas](https://github.com/pandas-dev/pandas)
 - [IPython](https://github.com/ipython/ipython)
 - [dataframe_image](https://github.com/dexplo/dataframe_image)
 
+## Acknowledgements and Disclaimer
+###  Acknowledgements
+This project is not affiliated with, endorsed by, or sponsored by EAB Global, Inc.
+"EAB Navigate" is a trademark of EAB Global, Inc. The use of the name "EAB Navigate"
+in this project is for identification purposes only and does not imply any
+association with EAB Global, Inc.
+
+### Disclaimer
+
+This independent project is developed for educational and informational purposes,
+to assist users in analyzing data they have legally exported from the EAB Navigate
+software. Users are responsible for ensuring their use of this tool complies with
+EAB's Terms of Use and any other applicable EAB policies. This project does not
+reproduce, distribute, or commercially exploit any EAB properties or services.
+
+### Additional Notes
+
+- This project's compatibility with EAB Navigate data relies on publicly available
+data formats or legally exported data. It does not reverse engineer or derive
+methods from EAB Navigate's proprietary technologies.
+
+- For concerns about the use of the "EAB Navigate" trademark, [please contact
+me](https://github.com/moshemoshe137).
+
+- Efforts have been made to avoid confusion or misrepresentation of this project's
+affiliation with EAB Global, Inc., or its products, including EAB Navigate.
+
+- Mention of EAB Navigate within this project does not imply endorsement by
+EAB Global, Inc.
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `EAB_tools-0.0.3rc0/EAB_tools.egg-info/SOURCES.txt` & `EAB_tools-0.1.1rc0/EAB_tools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 EAB_tools/__init__.py
 EAB_tools/conftest.py
 EAB_tools/eab_rc.py
 EAB_tools.egg-info/PKG-INFO
 EAB_tools.egg-info/SOURCES.txt
 EAB_tools.egg-info/dependency_links.txt
 EAB_tools.egg-info/requires.txt
 EAB_tools.egg-info/top_level.txt
 EAB_tools/_testing/__init__.py
+EAB_tools/_testing/context_managers.py
+EAB_tools/_testing/data_generation.py
 EAB_tools/_testing/io.py
 EAB_tools/_testing/types.py
+EAB_tools/_testing/test_scripts/generate_all_test_data.py
+EAB_tools/_testing/test_scripts/generate_fake_enrollments.py
+EAB_tools/io/__init__.py
 EAB_tools/io/display.py
+EAB_tools/io/enrollment.py
 EAB_tools/io/filenames.py
+EAB_tools/io/io.py
 EAB_tools/tests/__init__.py
+EAB_tools/tests/_testing/test_data_generation.py
 EAB_tools/tests/io/test_display.py
+EAB_tools/tests/io/test_enrollment.py
 EAB_tools/tests/io/test_filenames.py
+EAB_tools/tests/io/test_io.py
 EAB_tools/tests/util/test_hashing.py
 EAB_tools/util/__init__.py
 EAB_tools/util/hashing.py
```

### Comparing `EAB_tools-0.0.3rc0/LICENSE` & `EAB_tools-0.1.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.3rc0/PKG-INFO` & `EAB_tools-0.1.1rc0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAB_tools
-Version: 0.0.3rc0
+Version: 0.1.1rc0
 Summary: Tools for analyzing data exported from the EAB Navigate Student Success Management Software.
 Author: Moshe Rubin
 Author-email: Moshe Rubin <mosherubin137@gmail.com>
 License: MIT License
         
         Copyright 2022 Moshe Rubin https://github.com/moshemoshe137
         
@@ -35,14 +35,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dataframe_image
+Requires-Dist: ipython
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Provides-Extra: progress-bar
+Requires-Dist: tqdm; extra == "progress-bar"
 
 # EAB Tools
 [![License: MIT](https://img.shields.io/github/license/moshemoshe137/EAB_tools)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/EAB_tools)](https://pypi.org/project/EAB-tools/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -99,10 +105,40 @@
 
 Installing EAB tools will install these packages and their dependencies:
 
 - [pandas](https://github.com/pandas-dev/pandas)
 - [IPython](https://github.com/ipython/ipython)
 - [dataframe_image](https://github.com/dexplo/dataframe_image)
 
+## Acknowledgements and Disclaimer
+###  Acknowledgements
+This project is not affiliated with, endorsed by, or sponsored by EAB Global, Inc.
+"EAB Navigate" is a trademark of EAB Global, Inc. The use of the name "EAB Navigate"
+in this project is for identification purposes only and does not imply any
+association with EAB Global, Inc.
+
+### Disclaimer
+
+This independent project is developed for educational and informational purposes,
+to assist users in analyzing data they have legally exported from the EAB Navigate
+software. Users are responsible for ensuring their use of this tool complies with
+EAB's Terms of Use and any other applicable EAB policies. This project does not
+reproduce, distribute, or commercially exploit any EAB properties or services.
+
+### Additional Notes
+
+- This project's compatibility with EAB Navigate data relies on publicly available
+data formats or legally exported data. It does not reverse engineer or derive
+methods from EAB Navigate's proprietary technologies.
+
+- For concerns about the use of the "EAB Navigate" trademark, [please contact
+me](https://github.com/moshemoshe137).
+
+- Efforts have been made to avoid confusion or misrepresentation of this project's
+affiliation with EAB Global, Inc., or its products, including EAB Navigate.
+
+- Mention of EAB Navigate within this project does not imply endorsement by
+EAB Global, Inc.
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `EAB_tools-0.0.3rc0/pyproject.toml` & `EAB_tools-0.1.1rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,27 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Topic :: Database",
 ]
 dynamic = ["version", "dependencies"]  # Defined in setup.py
 
+[project.optional-dependencies]
+progress_bar = ['tqdm']
+
 [project.urls]
 "Homepage" = "https://github.com/moshemoshe137/EAB_tools"
 "Bug Tracker" = "https://github.com/moshemoshe137/EAB_tools/issues"
 
 [tool.black]
-target-version = ["py39", "py310"]
+target-version = ["py39", "py310", "py311", "py312"]
+
+[tool.flake8]
+count = true
+max-line-length = 88
 
 [tool.isort]
 # Most settings are barrowed from pandas
 # https://github.com/pandas-dev/pandas/blob/f4ca4d3d0ea6a907262f8c84/pyproject.toml#L143
 atomic = true
 combine_as_imports = true
 force_grid_wrap = 2
```

