# Comparing `tmp/metron_tagger-2.2.3.tar.gz` & `tmp/metron_tagger-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metron_tagger-2.2.3.tar", max compression
+gzip compressed data, was "metron_tagger-2.2.4.tar", max compression
```

## Comparing `metron_tagger-2.2.3.tar` & `metron_tagger-2.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      601 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/LICENSE
--rw-r--r--   0        0        0     2845 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/README.rst
--rw-r--r--   0        0        0       76 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/__init__.py
--rw-r--r--   0        0        0     1413 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/cli.py
--rw-r--r--   0        0        0     4501 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/duplicates.py
--rw-r--r--   0        0        0     7573 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/filerenamer.py
--rw-r--r--   0        0        0     3756 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/filesorter.py
--rw-r--r--   0        0        0      577 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/logging.py
--rw-r--r--   0        0        0     2787 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/options.py
--rw-r--r--   0        0        0    13377 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/run.py
--rw-r--r--   0        0        0     6443 2024-03-18 16:00:37.725829 metron_tagger-2.2.3/metrontagger/schema/v1/ComicInfo.xsd
--rw-r--r--   0        0        0     9518 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/metrontagger/schema/v2/ComicInfo.xsd
--rw-r--r--   0        0        0     4030 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/metrontagger/settings.py
--rw-r--r--   0        0        0      156 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/metrontagger/styles.py
--rw-r--r--   0        0        0    14910 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/metrontagger/talker.py
--rw-r--r--   0        0        0     1328 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/metrontagger/utils.py
--rw-r--r--   0        0        0     1763 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/metrontagger/validate_ci.py
--rw-r--r--   0        0        0     5176 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2534 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/conftest.py
--rw-r--r--   0        0        0     2567 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_filerenamer.py
--rw-r--r--   0        0        0     2693 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_filesorter.py
--rw-r--r--   0        0        0     6077 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_metron_tagger.py
--rw-r--r--   0        0        0     1431 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_options.py
--rw-r--r--   0        0        0     1336 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_settings.py
--rw-r--r--   0        0        0     9962 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_talker.py
--rw-r--r--   0        0        0     2314 2024-03-18 16:00:37.729829 metron_tagger-2.2.3/tests/test_utils.py
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 metron_tagger-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/LICENSE
+-rw-r--r--   0        0        0      897 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/NEWS.md
+-rw-r--r--   0        0        0     2845 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/README.rst
+-rw-r--r--   0        0        0       76 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/__init__.py
+-rw-r--r--   0        0        0     1413 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/cli.py
+-rw-r--r--   0        0        0     4936 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/duplicates.py
+-rw-r--r--   0        0        0     7573 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/filerenamer.py
+-rw-r--r--   0        0        0     3756 2024-04-06 13:17:19.527556 metron_tagger-2.2.4/metrontagger/filesorter.py
+-rw-r--r--   0        0        0      577 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/logging.py
+-rw-r--r--   0        0        0     2787 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/options.py
+-rw-r--r--   0        0        0    13377 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/run.py
+-rw-r--r--   0        0        0     6443 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/schema/v1/ComicInfo.xsd
+-rw-r--r--   0        0        0     9518 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/schema/v2/ComicInfo.xsd
+-rw-r--r--   0        0        0     4030 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/settings.py
+-rw-r--r--   0        0        0      156 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/styles.py
+-rw-r--r--   0        0        0    15026 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/talker.py
+-rw-r--r--   0        0        0     1328 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/utils.py
+-rw-r--r--   0        0        0     1763 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/metrontagger/validate_ci.py
+-rw-r--r--   0        0        0     5171 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     2534 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     2567 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_filerenamer.py
+-rw-r--r--   0        0        0     2693 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_filesorter.py
+-rw-r--r--   0        0        0     6077 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_metron_tagger.py
+-rw-r--r--   0        0        0     1431 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_options.py
+-rw-r--r--   0        0        0     1336 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_settings.py
+-rw-r--r--   0        0        0     9962 2024-04-06 13:17:19.531556 metron_tagger-2.2.4/tests/test_talker.py
+-rw-r--r--   0        0        0     2314 2024-04-06 13:17:19.535556 metron_tagger-2.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 metron_tagger-2.2.4/PKG-INFO
```

### Comparing `metron_tagger-2.2.3/LICENSE` & `metron_tagger-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/README.rst` & `metron_tagger-2.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/cli.py` & `metron_tagger-2.2.4/metrontagger/cli.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/duplicates.py` & `metron_tagger-2.2.4/metrontagger/duplicates.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,34 +31,45 @@
         self._file_lst = file_lst
         self._data_frame: pd.DataFrame | None = None
 
     def _image_hashes(self: "Duplicates") -> list[dict[str, any]]:
         """Method to get a list of dicts containing the file path, page index, and page hashes."""
         hashes_lst = []
         for item in self._file_lst:
-            comic = Comic(str(item))
+            comic = Comic(item)
             if not comic.is_writable():
                 questionary.print(f"'{comic}' is not writable. Skipping...")
                 continue
             questionary.print(
                 f"Attempting to get page hashes for '{comic}'.",
                 style=Styles.WARNING,
             )
             for i in range(comic.get_number_of_pages()):
-                with Image.open(io.BytesIO(comic.get_page(i))) as img:
-                    try:
-                        img_hash = average_hash(img)
-                    except OSError:
-                        questionary.print(
-                            f"Unable to get image hash for page {i} of '{comic}'",
-                            style=Styles.ERROR,
-                        )
-                        continue
-                    image_info = {"path": str(comic.path), "index": i, "hash": str(img_hash)}
-                    hashes_lst.append(image_info)
+                try:
+                    with Image.open(io.BytesIO(comic.get_page(i))) as img:
+                        try:
+                            img_hash = average_hash(img)
+                        except OSError:
+                            questionary.print(
+                                f"Unable to get image hash for page {i} of '{comic}'",
+                                style=Styles.ERROR,
+                            )
+                            continue
+                        image_info = {
+                            "path": str(comic.path),
+                            "index": i,
+                            "hash": str(img_hash),
+                        }
+                        hashes_lst.append(image_info)
+                except UnidentifiedImageError:
+                    questionary.print(
+                        f"UnidentifiedImageError: Skipping page {i} of '{comic}'",
+                        style=Styles.ERROR,
+                    )
+                    continue
         return hashes_lst
 
     def _get_page_hashes(self: "Duplicates") -> pd.DataFrame:
         """Method to get a dataframe of comics with duplicate pages."""
         comic_hashes = self._image_hashes()
         self._data_frame = pd.DataFrame(comic_hashes)
         hashes = self._data_frame["hash"]
```

### Comparing `metron_tagger-2.2.3/metrontagger/filerenamer.py` & `metron_tagger-2.2.4/metrontagger/filerenamer.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/filesorter.py` & `metron_tagger-2.2.4/metrontagger/filesorter.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/logging.py` & `metron_tagger-2.2.4/metrontagger/logging.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/options.py` & `metron_tagger-2.2.4/metrontagger/options.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/run.py` & `metron_tagger-2.2.4/metrontagger/run.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/schema/v1/ComicInfo.xsd` & `metron_tagger-2.2.4/metrontagger/schema/v1/ComicInfo.xsd`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/schema/v2/ComicInfo.xsd` & `metron_tagger-2.2.4/metrontagger/schema/v2/ComicInfo.xsd`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/settings.py` & `metron_tagger-2.2.4/metrontagger/settings.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/talker.py` & `metron_tagger-2.2.4/metrontagger/talker.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,18 @@
         return hamming_lst
 
     @staticmethod
     def _get_source_id(md: Metadata) -> tuple[InfoSource, int | None]:
         source: InfoSource = InfoSource.unknown
         id_: int | None = None
 
+        # If `Notes` element doesn't exist let's bail.
+        if md.notes is None:
+            return source, id_
+
         lower_notes = md.notes.lower()
         if "metrontagger" in lower_notes:
             source = InfoSource.metron
             try:
                 id_ = int(md.notes.split("issue_id:")[1].strip("]"))
             except ValueError:
                 LOGGER.exception("Comic has invalid id: %s #%s", md.series.name, md.issue)
```

### Comparing `metron_tagger-2.2.3/metrontagger/utils.py` & `metron_tagger-2.2.4/metrontagger/utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/metrontagger/validate_ci.py` & `metron_tagger-2.2.4/metrontagger/validate_ci.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/pyproject.toml` & `metron_tagger-2.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "metron-tagger"
-version = "2.2.3"
+version = "2.2.4"
 description = "A program to write metadata from metron.cloud to a comic archive"
 authors = ["Brian Pepple <bpepple@metron.cloud>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Brian Pepple <bpepple@metron.cloud>"]
 readme = "README.rst"
 packages = [{ include = "metrontagger" }]
 exclude = ["*/**/*~"]
 include = [
   { path = "tests", format = "sdist" },
-  { path = "CHANGELOG.md", format = "sdist" },
+  { path = "NEWS.md", format = "sdist" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Natural Language :: English",
```

### Comparing `metron_tagger-2.2.3/tests/conftest.py` & `metron_tagger-2.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_filerenamer.py` & `metron_tagger-2.2.4/tests/test_filerenamer.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_filesorter.py` & `metron_tagger-2.2.4/tests/test_filesorter.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_metron_tagger.py` & `metron_tagger-2.2.4/tests/test_metron_tagger.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_options.py` & `metron_tagger-2.2.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_settings.py` & `metron_tagger-2.2.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_talker.py` & `metron_tagger-2.2.4/tests/test_talker.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/tests/test_utils.py` & `metron_tagger-2.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `metron_tagger-2.2.3/PKG-INFO` & `metron_tagger-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metron-tagger
-Version: 2.2.3
+Version: 2.2.4
 Summary: A program to write metadata from metron.cloud to a comic archive
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata,tagging,tagger
 Author: Brian Pepple
 Author-email: bpepple@metron.cloud
 Maintainer: Brian Pepple
 Maintainer-email: bpepple@metron.cloud
```

