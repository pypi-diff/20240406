# Comparing `tmp/nbmetaclean-0.0.7.tar.gz` & `tmp/nbmetaclean-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbmetaclean-0.0.7.tar", last modified: Fri Nov 17 16:22:32 2023, max compression
+gzip compressed data, was "nbmetaclean-0.0.8.tar", last modified: Sat Apr  6 12:35:02 2024, max compression
```

## Comparing `nbmetaclean-0.0.7.tar` & `nbmetaclean-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-11-17 16:22:32.194475 nbmetaclean-0.0.7/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-10-23 08:22:02.000000 nbmetaclean-0.0.7/LICENSE
--rw-r--r--   0 aya       (1000) aya       (1000)      830 2023-11-17 16:22:32.194475 nbmetaclean-0.0.7/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)       25 2023-10-23 08:20:49.000000 nbmetaclean-0.0.7/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      162 2023-10-23 08:20:01.000000 nbmetaclean-0.0.7/pyproject.toml
--rw-rw-r--   0 aya       (1000) aya       (1000)      923 2023-11-17 16:22:32.194475 nbmetaclean-0.0.7/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-10-23 08:20:45.000000 nbmetaclean-0.0.7/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-11-17 16:22:32.182475 nbmetaclean-0.0.7/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-11-17 16:22:32.190475 nbmetaclean-0.0.7/src/nbmetaclean/
--rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-11-08 09:52:33.000000 nbmetaclean-0.0.7/src/nbmetaclean/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1561 2023-11-17 16:21:12.000000 nbmetaclean-0.0.7/src/nbmetaclean/app.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     7069 2023-11-17 16:21:12.000000 nbmetaclean-0.0.7/src/nbmetaclean/clean.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2406 2023-11-17 16:21:12.000000 nbmetaclean-0.0.7/src/nbmetaclean/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      266 2023-10-30 10:20:58.000000 nbmetaclean-0.0.7/src/nbmetaclean/typing.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       42 2023-11-17 16:21:12.000000 nbmetaclean-0.0.7/src/nbmetaclean/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-11-17 16:22:32.194475 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/
--rw-r--r--   0 aya       (1000) aya       (1000)      830 2023-11-17 16:22:32.000000 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      485 2023-11-17 16:22:32.000000 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-11-17 16:22:32.000000 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       90 2023-11-17 16:22:32.000000 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/entry_points.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       26 2023-11-17 16:22:32.000000 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       12 2023-11-17 16:22:32.000000 nbmetaclean-0.0.7/src/nbmetaclean.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-11-17 16:22:32.194475 nbmetaclean-0.0.7/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)    10942 2023-11-17 16:21:12.000000 nbmetaclean-0.0.7/tests/test_clean.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3727 2023-11-17 16:21:12.000000 nbmetaclean-0.0.7/tests/test_read_write.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-10-26 06:15:52.000000 nbmetaclean-0.0.8/LICENSE
+-rw-r--r--   0 aya       (1000) aya       (1000)     1342 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      538 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      162 2023-10-26 06:15:52.000000 nbmetaclean-0.0.8/pyproject.toml
+-rw-rw-r--   0 aya       (1000) aya       (1000)      923 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      596 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/src/nbmetaclean/
+-rw-rw-r--   0 aya       (1000) aya       (1000)        0 2023-10-26 06:15:52.000000 nbmetaclean-0.0.8/src/nbmetaclean/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3019 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/src/nbmetaclean/app.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7308 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/src/nbmetaclean/clean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2886 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/src/nbmetaclean/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1662 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/src/nbmetaclean/typing.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       42 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/src/nbmetaclean/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/
+-rw-r--r--   0 aya       (1000) aya       (1000)     1342 2024-04-06 12:35:02.000000 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      514 2024-04-06 12:35:02.000000 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2024-04-06 12:35:02.000000 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       90 2024-04-06 12:35:02.000000 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/entry_points.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       26 2024-04-06 12:35:02.000000 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       12 2024-04-06 12:35:02.000000 nbmetaclean-0.0.8/src/nbmetaclean.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:35:02.056442 nbmetaclean-0.0.8/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11188 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/tests/test_clean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3389 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/tests/test_get_nbnames.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1386 2024-04-06 12:34:32.000000 nbmetaclean-0.0.8/tests/test_read_write.py
```

### Comparing `nbmetaclean-0.0.7/LICENSE` & `nbmetaclean-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nbmetaclean-0.0.7/setup.cfg` & `nbmetaclean-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `nbmetaclean-0.0.7/src/nbmetaclean/app.py` & `nbmetaclean-0.0.8/src/nbmetaclean/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from pathlib import Path
+from typing import Union
 
-from .clean import CleanConfig, clean_nb_file
-from .core import get_nb_names
+from .clean import CleanConfig, TupleStr, clean_nb_file
+from .helpers import get_nb_names
 
 parser = argparse.ArgumentParser(
     prog="nbclean",
     description="Clean metadata and execution_count from Jupyter notebooks.",
 )
 parser.add_argument(
     "path",
@@ -21,36 +22,85 @@
     help="Silent mode.",
 )
 parser.add_argument(
     "--not-pt",
     action="store_true",
     help="Do not preserve timestamp.",
 )
+parser.add_argument(
+    "--dont_clear_nb_metadata",
+    action="store_true",
+    help="Do not clear notebook metadata.",
+)
+parser.add_argument(
+    "--clear_cell_metadata",
+    action="store_true",
+    help="Clear cell metadata.",
+)
+parser.add_argument(
+    "--clear_outputs",
+    action="store_true",
+    help="Clear outputs.",
+)
+parser.add_argument(
+    "--nb_metadata_preserve_mask",
+    nargs="+",
+    help="Preserve mask for notebook metadata.",
+)
+parser.add_argument(
+    "--cell_metadata_preserve_mask",
+    nargs="+",
+    help="Preserve mask for cell metadata.",
+)
+parser.add_argument(
+    "--dont_merge_masks",
+    action="store_true",
+    help="Do not merge masks.",
+)
+parser.add_argument(
+    "--clean_hidden_nbs",
+    action="store_true",
+    help="Clean hidden notebooks.",
+)
+
+
+def process_mask(mask: Union[list[str], None]) -> Union[tuple[TupleStr, ...], None]:
+    if mask is None:
+        return None
+    return tuple(tuple(item.split(".")) for item in mask)
 
 
 def app() -> None:
     """Clean metadata and execution_count from Jupyter notebook."""
     cfg = parser.parse_args()
     path_list = cfg.path if isinstance(cfg.path, list) else [cfg.path]
     nb_files: list[Path] = []
     if not cfg.silent:
         print(f"Path: {', '.join(cfg.path)}, preserve timestamp: {not cfg.not_pt}")
     for path in path_list:
         try:
-            nb_files.extend(get_nb_names(path))
+            nb_files.extend(get_nb_names(path, hidden=cfg.clean_hidden_nbs))
         except FileNotFoundError:
             print(f"{path} not exists!")
     if not cfg.silent:
         print(f"notebooks to check: {len(nb_files)} ")
+    clean_config = CleanConfig(
+        clear_nb_metadata=not cfg.dont_clear_nb_metadata,
+        clear_cell_metadata=cfg.clear_cell_metadata,
+        clear_execution_count=True,
+        clear_outputs=cfg.clear_outputs,
+        preserve_timestamp=not cfg.not_pt,
+        silent=cfg.silent,
+        nb_metadata_preserve_mask=process_mask(cfg.nb_metadata_preserve_mask),
+        cell_metadata_preserve_mask=process_mask(cfg.cell_metadata_preserve_mask),
+        mask_merge=not cfg.dont_merge_masks,
+    )
     cleaned, errors = clean_nb_file(
         nb_files,
-        CleanConfig(
-            silent=cfg.silent,
-            preserve_timestamp=not cfg.not_pt,
-        ),
+        clean_config,
     )
     if not cfg.silent:
         print(f"cleaned nbs: {len(cleaned)}")
         if errors:
             print(f"with errors: {len(errors)}")
             for nb, exc in errors:
                 print(f"{nb}: {exc}")
```

### Comparing `nbmetaclean-0.0.7/src/nbmetaclean/clean.py` & `nbmetaclean-0.0.8/src/nbmetaclean/clean.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
+
 import copy
-from dataclasses import dataclass
 import os
-
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterable, Optional, Union
+from typing import Optional, Tuple, Union
 
-from nbmetaclean.core import read_nb, write_nb
+from nbmetaclean.helpers import read_nb, write_nb
 
-from .typing import NbNode, Metadata
+from .typing import Cell, CodeCell, Metadata, Nb, Output
+
+TupleStr = Tuple[str, ...]
 
 NB_METADATA_PRESERVE_MASKS = (
     ("language_info", "name"),
     ("authors",),
 )
 
 
@@ -37,22 +39,22 @@
 
     clear_nb_metadata: bool = True
     clear_cell_metadata: bool = False
     clear_execution_count: bool = True
     clear_outputs: bool = False
     preserve_timestamp: bool = True
     silent: bool = False
-    nb_metadata_preserve_mask: Optional[Iterable[tuple[str, ...]]] = None
-    cell_metadata_preserve_mask: Optional[Iterable[tuple[str, ...]]] = None
+    nb_metadata_preserve_mask: Optional[tuple[TupleStr, ...]] = None
+    cell_metadata_preserve_mask: Optional[tuple[TupleStr, ...]] = None
     mask_merge: bool = True
 
 
 def filter_meta_mask(
     nb_meta: Union[str, int, Metadata],
-    mask: Optional[Iterable[tuple[str, ...]]] = None,
+    mask: Optional[tuple[str, ...]] = None,
 ) -> Union[str, int, Metadata]:
     """Filter metadata by mask. If no mask return empty dict."""
     if isinstance(nb_meta, (str, int)) or mask == ():
         return nb_meta
     if mask is None:
         return {}
     new_meta = {}
@@ -61,58 +63,60 @@
         new_mask = tuple(mask[1:])
         new_meta[mask[0]] = filter_meta_mask(value, new_mask) or value
     return new_meta
 
 
 def filter_metadata(
     nb_meta: Metadata,
-    masks: Optional[list[tuple[str, ...]]] = None,
+    masks: Optional[tuple[TupleStr, ...]] = None,
 ) -> Metadata:
     """Clean notebooknode metadata."""
     if masks is None:
         return {}
     filtered_meta: Metadata = {}
     for mask in masks:
         filtered_meta.update(filter_meta_mask(nb_meta, mask))  # type: ignore
     return filtered_meta
 
 
 def clean_cell(
-    cell: NbNode,
+    cell: Cell | CodeCell,
     cfg: CleanConfig,
 ) -> bool:
     """Clean cell: optionally metadata, execution_count and outputs."""
     changed = False
 
     if cfg.clear_cell_metadata:
-        if metadata := cell.get("metadata", None):
+        if cell.get("metadata", None):
+            metadata = cell["metadata"]
             old_metadata = copy.deepcopy(metadata)
             cell["metadata"] = filter_metadata(
                 metadata, cfg.cell_metadata_preserve_mask
             )
             if cell["metadata"] != old_metadata:
                 changed = True
 
-    if cfg.clear_execution_count and cell.get("execution_count"):
-        cell["execution_count"] = None
-        changed = True
-
-    if cell.get("outputs"):
-        if cfg.clear_outputs:
-            cell["outputs"] = []
+    if cell["cell_type"] == "code":
+        if cfg.clear_execution_count and cell.get("execution_count"):
+            cell["execution_count"] = None  # type: ignore # it's code cell
             changed = True
-        elif cfg.clear_cell_metadata or cfg.clear_execution_count:
-            result = clean_outputs(cell["outputs"], cfg)
-            if result:
+
+        if cell.get("outputs"):
+            if cfg.clear_outputs:
+                cell["outputs"] = []  # type: ignore  # it's code cell
                 changed = True
+            elif cfg.clear_cell_metadata or cfg.clear_execution_count:
+                result = clean_outputs(cell["outputs"], cfg)  # type: ignore # it's code cell
+                if result:
+                    changed = True
 
     return changed
 
 
-def clean_outputs(outputs: list[NbNode], cfg: CleanConfig) -> bool:
+def clean_outputs(outputs: list[Output], cfg: CleanConfig) -> bool:
     """Clean outputs."""
     changed = False
     for output in outputs:
         if cfg.clear_execution_count and output.get("execution_count", None):
             output["execution_count"] = None
             changed = True
         if cfg.clear_cell_metadata and (metadata := output.get("metadata", None)):
@@ -122,15 +126,15 @@
             )
             if output["metadata"] != old_metadata:
                 changed = True
     return changed
 
 
 def clean_nb(
-    nb: NbNode,
+    nb: Nb,
     cfg: CleanConfig,
 ) -> bool:
     """Clean notebook - metadata, execution_count, outputs.
 
     Args:
         nb (Notebook): Notebook to clean.
         clear_execution_count (bool, optional): Clear execution_count. Defaults to True.
@@ -144,15 +148,14 @@
         old_metadata = copy.deepcopy(metadata)
         masks = NB_METADATA_PRESERVE_MASKS
         if cfg.nb_metadata_preserve_mask:
             if not cfg.mask_merge:
                 masks = cfg.nb_metadata_preserve_mask
             else:
                 masks = cfg.nb_metadata_preserve_mask + masks
-
         nb["metadata"] = filter_metadata(metadata, masks=masks)
         if nb["metadata"] != old_metadata:
             changed = True
     if cfg.clear_cell_metadata or cfg.clear_execution_count or cfg.clear_outputs:
         for cell in nb["cells"]:
             result = clean_cell(
                 cell,
```

### Comparing `nbmetaclean-0.0.7/src/nbmetaclean/core.py` & `nbmetaclean-0.0.8/src/nbmetaclean/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
 
 import json
 from pathlib import Path
 from typing import Optional
 
-from .typing import NbNode, PathOrStr
+from .typing import Nb, PathOrStr
 
 
-def read_nb(path: PathOrStr) -> NbNode:
+def read_nb(path: PathOrStr) -> Nb:
     """Read notebook from filename.
 
     Args:
         path (Union[str, PosixPath): Notebook filename.
 
     Returns:
         Notebook: Jupyter Notebook as dict.
     """
     return json.load(open(path, "r", encoding="utf-8"))
 
 
 def write_nb(
-    nb: NbNode,
+    nb: Nb,
     path: PathOrStr,
 ) -> Path:
     """Write notebook to file
 
     Args:
         nb (Notebook): Notebook to write
         path (Union[str, PosixPath]): filename to write
     Returns:
-        Path: Filename of writed Nb.
+        Path: Filename of written notebook.
     """
     filename = Path(path)
     if filename.suffix != ".ipynb":
         filename = filename.with_suffix(".ipynb")
     with filename.open("w", encoding="utf-8") as fh:
         fh.write(
             json.dumps(
@@ -44,14 +44,31 @@
                 sort_keys=True,
             )
             + "\n",
         )
     return filename
 
 
+def is_notebook(path: Path, hidden: bool = False) -> bool:
+    """Check if `path` is a notebook and not hidden. If `hidden` is True check also hidden files.
+
+    Args:
+        path (Union[Path, str]): Path to check.
+        hidden bool: If True also check hidden files, defaults to False.
+
+    Returns:
+        bool: True if `path` is a notebook and not hidden.
+    """
+    if path.suffix == ".ipynb":
+        if path.name.startswith(".") and not hidden:
+            return False
+        return True
+    return False
+
+
 def get_nb_names(
     path: Optional[PathOrStr] = None,
     recursive: bool = True,
     hidden: bool = False,
 ) -> list[Path]:
     """Return list of notebooks from `path`. If no `path` return notebooks from current folder.
 
@@ -67,25 +84,26 @@
         List[Path]: List of notebooks names.
     """
     nb_path = Path(path or ".")
 
     if not nb_path.exists():
         raise FileNotFoundError(f"{nb_path} not exists!")
 
+    if nb_path.is_file():
+        if is_notebook(nb_path, hidden):
+            return [nb_path]
+
     if nb_path.is_dir():
         result = []
         for item in nb_path.iterdir():
-            if item.is_file() and item.suffix == ".ipynb":
-                if not hidden and item.name.startswith("."):
-                    continue
+            if item.is_file() and is_notebook(item, hidden):
                 result.append(item)
-            if item.is_dir():
-                if recursive:
-                    if not hidden and item.name.startswith("."):
-                        continue
-                    if "checkpoint" in item.name:
-                        continue
-                    result.extend(get_nb_names(item, recursive, hidden))
+            if item.is_dir() and recursive:
+                if item.name.startswith(".") and not hidden:
+                    continue
+                if "checkpoint" in item.name:
+                    continue
+                result.extend(get_nb_names(item, recursive, hidden))
 
         return result
 
-    return [nb_path]
+    return []
```

### Comparing `nbmetaclean-0.0.7/tests/test_clean.py` & `nbmetaclean-0.0.8/tests/test_clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     CleanConfig,
     clean_cell,
     clean_nb,
     clean_nb_file,
     filter_meta_mask,
     filter_metadata,
 )
-from nbmetaclean.core import read_nb, write_nb
+from nbmetaclean.helpers import read_nb, write_nb
 
 
 def test_get_meta_by_mask():
     """test get_meta_by_mask"""
     nb = read_nb(Path("tests/test_nbs/.test_nb_2_meta.ipynb"))
     nb_meta = nb.get("metadata")
 
@@ -79,14 +79,15 @@
 
 def test_clean_cell_metadata():
     """test clean_cell_metadata"""
     test_nb = read_nb("tests/test_nbs/.test_nb_2_meta.ipynb")
 
     # clear outputs
     cell = copy.deepcopy(test_nb.get("cells")[1])
+    assert cell["cell_type"] == "code"
     assert cell.get("outputs")
     assert not cell.get("metadata")
     assert cell.get("execution_count") == 1
     cell["metadata"] = {"some key": "some value"}
     changed = clean_cell(
         cell,
         cfg=CleanConfig(
@@ -94,14 +95,23 @@
             clear_cell_metadata=True,
         ),
     )
     assert changed
     assert not cell.get("outputs")
     assert not cell.get("metadata")
     assert not cell.get("execution_count")
+    # run again - no changes
+    changed = clean_cell(
+        cell,
+        cfg=CleanConfig(
+            clear_outputs=True,
+            clear_cell_metadata=True,
+        ),
+    )
+    assert not changed
 
     # dont clear outputs, execution_count, mask
     cell = copy.deepcopy(test_nb.get("cells")[1])
     cell["metadata"] = {"some key": "some value"}
     cell["outputs"][0]["metadata"] = {
         "some key": "some value",
         "some other key": "some value",
```

