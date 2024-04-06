# Comparing `tmp/chromadb_data_pipes-0.0.7.tar.gz` & `tmp/chromadb_data_pipes-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb_data_pipes-0.0.7.tar", max compression
+gzip compressed data, was "chromadb_data_pipes-0.0.8.tar", max compression
```

## Comparing `chromadb_data_pipes-0.0.7.tar` & `chromadb_data_pipes-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1077 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/LICENSE.md
--rw-r--r--   0        0        0     4852 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/README.md
--rw-r--r--   0        0        0     1989 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/chroma/__init__.py
--rw-r--r--   0        0        0     5356 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_export.py
--rw-r--r--   0        0        0     5306 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_import.py
--rw-r--r--   0        0        0    15486 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/huggingface/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/huggingface/utils.py
--rw-r--r--   0        0        0     2866 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/main.py
--rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/__init__.py
--rw-r--r--   0        0        0     3071 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/chunk.py
--rw-r--r--   0        0        0     3066 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/embed.py
--rw-r--r--   0        0        0     4921 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/id.py
--rw-r--r--   0        0        0     1343 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/langchain_utils.py
--rw-r--r--   0        0        0     4473 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/metadata.py
--rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/misc/__init__.py
--rw-r--r--   0        0        0     2028 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/processor/misc/emoji_clean.py
--rw-r--r--   0        0        0        0 2024-04-04 17:19:13.948305 chromadb_data_pipes-0.0.7/chroma_dp/producer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/__init__.py
--rw-r--r--   0        0        0     4188 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/csv.py
--rw-r--r--   0        0        0     2302 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/pdf.py
--rw-r--r--   0        0        0     2363 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/file/text.py
--rw-r--r--   0        0        0       97 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/langchain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/url/__init__.py
--rw-r--r--   0        0        0     2900 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/producer/url/url_loader.py
--rw-r--r--   0        0        0      482 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/chroma.py
--rw-r--r--   0        0        0     2918 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/embedding.py
--rw-r--r--   0        0        0      608 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/chroma_dp/utils/templating.py
--rw-r--r--   0        0        0     1604 2024-04-04 17:19:13.952304 chromadb_data_pipes-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 chromadb_data_pipes-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0     4852 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/README.md
+-rw-r--r--   0        0        0     1989 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/chroma/__init__.py
+-rw-r--r--   0        0        0     5792 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_export.py
+-rw-r--r--   0        0        0     5478 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_import.py
+-rw-r--r--   0        0        0    15486 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/huggingface/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/huggingface/utils.py
+-rw-r--r--   0        0        0     2866 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/main.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/__init__.py
+-rw-r--r--   0        0        0     3071 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/chunk.py
+-rw-r--r--   0        0        0     3066 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/embed.py
+-rw-r--r--   0        0        0     4921 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/id.py
+-rw-r--r--   0        0        0     1343 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/langchain_utils.py
+-rw-r--r--   0        0        0     4473 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/misc/__init__.py
+-rw-r--r--   0        0        0     2028 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/misc/emoji_clean.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/__init__.py
+-rw-r--r--   0        0        0     4188 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/csv.py
+-rw-r--r--   0        0        0     2302 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/pdf.py
+-rw-r--r--   0        0        0     2363 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/text.py
+-rw-r--r--   0        0        0       97 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/url/__init__.py
+-rw-r--r--   0        0        0     2900 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/url/url_loader.py
+-rw-r--r--   0        0        0      482 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/__init__.py
+-rw-r--r--   0        0        0     6598 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/chroma.py
+-rw-r--r--   0        0        0     2918 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/embedding.py
+-rw-r--r--   0        0        0      608 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/templating.py
+-rw-r--r--   0        0        0     1604 2024-04-06 16:10:19.459087 chromadb_data_pipes-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 chromadb_data_pipes-0.0.8/PKG-INFO
```

### Comparing `chromadb_data_pipes-0.0.7/LICENSE.md` & `chromadb_data_pipes-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/README.md` & `chromadb_data_pipes-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/__init__.py` & `chromadb_data_pipes-0.0.8/chroma_dp/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_export.py` & `chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_export.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,14 +96,18 @@
     ),
     where_document: Optional[str] = typer.Option(
         None,
         "--where-document",
         "-d",
         help='Document filter string - JSON with Chroma syntax is expected - \'{"$contains": "search for this"}\'',
     ),
+    format_output: Optional[str] = typer.Option(
+        "record", "--format",
+        help="Export format. Default is `record`. Supported formats: `record` and `jsonl`. "
+    ),
 ) -> None:
     if uri is None:
         raise ValueError("Please provide a ChromaDP URI.")
     parsed_uri = CDPUri.from_uri(uri)
     client = get_client_for_uri(parsed_uri)
     _collection = parsed_uri.collection or collection
     _batch_size = parsed_uri.batch_size or batch_size
@@ -128,24 +132,29 @@
                 chroma_collection,
                 offset=offset,
                 limit=min(total_results_to_fetch - offset, _batch_size),
                 where=_where,
                 where_document=_where_document,
             )
         )
-        _final_results = [
-            remap_features(
-                doc,
-                doc_feature=doc_feature,
-                embed_feature=embed_feature,
-                id_feature=id_feature,
-                meta_features=meta_features,
-            )
-            for doc in _results
-        ]
+        if format_output == "record":
+            _final_results = [r.model_dump() for r in _results]
+        elif format_output == "jsonl":
+            _final_results = [
+                remap_features(
+                    doc,
+                    doc_feature=doc_feature,
+                    embed_feature=embed_feature,
+                    id_feature=id_feature,
+                    meta_features=meta_features,
+                )
+                for doc in _results
+            ]
+        else:
+            raise ValueError(f"Unsupported format: {format}")
         if export_file:
             with open(export_file, "a") as f:
                 for _doc in _final_results:
                     f.write(str(json.dumps(_doc)) + "\n")
         else:
             for _doc in _final_results:
                 typer.echo(json.dumps(_doc))
```

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/chroma/chroma_import.py` & `chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,18 @@
     embedding_function: Optional[SupportedEmbeddingFunctions] = typer.Option(
         None, "--ef", help="The embedding function."
     ),
     upsert: Annotated[bool, typer.Option(help="Upsert documents.")] = False,
     embed_feature: Annotated[
         str, typer.Option(help="The embedding feature.")
     ] = "embedding",
-    meta_features: Annotated[
-        Optional[List[str]], typer.Option(help="The metadata features.")
-    ] = None,
+    meta_features: Optional[List[str]] = typer.Option(None,
+                                                      '-m',
+                                                      '--meta-features',
+                                                      help="The metadata features to import."),
     id_feature: Annotated[str, typer.Option(help="The id feature.")] = "id",
     doc_feature: Annotated[
         str, typer.Option(help="The document feature.")
     ] = "text_chunk",
     distance_function: Optional[DistanceFunction] = typer.Option(
         None,
         "--df",
```

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/huggingface/__init__.py` & `chromadb_data_pipes-0.0.8/chroma_dp/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/huggingface/utils.py` & `chromadb_data_pipes-0.0.8/chroma_dp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/main.py` & `chromadb_data_pipes-0.0.8/chroma_dp/main.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/processor/chunk.py` & `chromadb_data_pipes-0.0.8/chroma_dp/processor/chunk.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/processor/embed.py` & `chromadb_data_pipes-0.0.8/chroma_dp/processor/embed.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/processor/id.py` & `chromadb_data_pipes-0.0.8/chroma_dp/processor/id.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/processor/langchain_utils.py` & `chromadb_data_pipes-0.0.8/chroma_dp/processor/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/processor/metadata.py` & `chromadb_data_pipes-0.0.8/chroma_dp/processor/metadata.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/processor/misc/emoji_clean.py` & `chromadb_data_pipes-0.0.8/chroma_dp/processor/misc/emoji_clean.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/producer/file/csv.py` & `chromadb_data_pipes-0.0.8/chroma_dp/producer/file/csv.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/producer/file/pdf.py` & `chromadb_data_pipes-0.0.8/chroma_dp/producer/file/pdf.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/producer/file/text.py` & `chromadb_data_pipes-0.0.8/chroma_dp/producer/file/text.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/producer/url/url_loader.py` & `chromadb_data_pipes-0.0.8/chroma_dp/producer/url/url_loader.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/utils/chroma.py` & `chromadb_data_pipes-0.0.8/chroma_dp/utils/chroma.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     # if standard metadata is present and no specific metadata is provided use the standard metadata
     if "metadata" in in_dict and not meta_features:
         # print("in_dict", in_dict)
         _meta = get_default_metadata(in_dict)
     elif "metadata" in in_dict and meta_features:
         _meta = {k: in_dict["metadata"][k] for k in meta_features}
     elif "metadata" not in in_dict and meta_features:
-        _meta = {k: None for k in meta_features}
+        _meta = {k: in_dict[k] for k in meta_features}
     else:
         _meta = None
     _doc = in_dict[doc_feature]
     _embed = in_dict[embed_feature] if embed_feature else None
     _id = in_dict[id_feature] if id_feature else None
     return EmbeddableTextResource(
         text_chunk=_doc, embedding=_embed, metadata=_meta, id=_id
```

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/utils/embedding.py` & `chromadb_data_pipes-0.0.8/chroma_dp/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/chroma_dp/utils/templating.py` & `chromadb_data_pipes-0.0.8/chroma_dp/utils/templating.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.7/pyproject.toml` & `chromadb_data_pipes-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromadb-data-pipes"
-version = "0.0.7"
+version = "0.0.8"
 description = "ChromaDB Data Pipes 🖇️ - The easiest way to get data into and out of ChromaDB"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "chroma_dp" }]
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/amikos-tech/chromadb-data-pipes/issues"
@@ -12,15 +12,15 @@
 "Source" = "https://github.com/amikos-tech/chromadb-data-pipes/"
 
 [tool.poetry.scripts]
 "cdp" = "chroma_dp.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-chromadb = "0.4.22"
+chromadb = "0.4.24"
 datasets = "^2.15.0"
 tqdm = "^4.66.1"
 rich = "^13.7.0"
 typer = { extras = ["all"], version = "^0.9.0" }
 pydantic = "^2.5.3"
 tenacity = "^8.2.3"
 fastapi = "^0.108.0"
```

### Comparing `chromadb_data_pipes-0.0.7/PKG-INFO` & `chromadb_data_pipes-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: chromadb-data-pipes
-Version: 0.0.7
+Version: 0.0.8
 Summary: ChromaDB Data Pipes 🖇️ - The easiest way to get data into and out of ChromaDB
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: chromadb (==0.4.22)
+Requires-Dist: chromadb (==0.4.24)
 Requires-Dist: datasets (>=2.15.0,<3.0.0)
 Requires-Dist: fastapi (>=0.108.0,<0.109.0)
 Requires-Dist: langchain (>=0.1.0,<0.2.0)
 Requires-Dist: orjson (>=3.9.12,<4.0.0)
 Requires-Dist: py-ulid (>=1.0.3,<2.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pypdf (>=3.17.4,<4.0.0)
```

