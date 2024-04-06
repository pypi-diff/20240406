# Comparing `tmp/llama_index_readers_wikipedia-0.1.3.tar.gz` & `tmp/llama_index_readers_wikipedia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_wikipedia-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_wikipedia-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_wikipedia-0.1.3.tar` & `llama_index_readers_wikipedia-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-02-13 13:53:01.896434 llama_index_readers_wikipedia-0.1.3/README.md
--rw-r--r--   0        0        0       94 2024-02-13 13:53:01.896642 llama_index_readers_wikipedia-0.1.3/llama_index/readers/wikipedia/__init__.py
--rw-r--r--   0        0        0     1190 2024-02-13 13:53:01.896712 llama_index_readers_wikipedia-0.1.3/llama_index/readers/wikipedia/base.py
--rw-r--r--   0        0        0     1474 2024-02-21 21:06:40.245960 llama_index_readers_wikipedia-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 llama_index_readers_wikipedia-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-06 11:16:20.165896 llama_index_readers_wikipedia-0.1.4/README.md
+-rw-r--r--   0        0        0       94 2024-04-06 11:16:20.169896 llama_index_readers_wikipedia-0.1.4/llama_index/readers/wikipedia/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-06 11:16:20.169896 llama_index_readers_wikipedia-0.1.4/llama_index/readers/wikipedia/base.py
+-rw-r--r--   0        0        0     1474 2024-04-06 11:16:20.169896 llama_index_readers_wikipedia-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 llama_index_readers_wikipedia-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_wikipedia-0.1.3/llama_index/readers/wikipedia/base.py` & `llama_index_readers_wikipedia-0.1.4/llama_index/readers/wikipedia/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Simple reader that reads wikipedia."""
+
 from typing import Any, List
 
 from llama_index.core.readers.base import BasePydanticReader
 from llama_index.core.schema import Document
 
 
 class WikipediaReader(BasePydanticReader):
@@ -23,23 +24,34 @@
                 "`wikipedia` package not found, please run `pip install wikipedia`"
             )
 
     @classmethod
     def class_name(cls) -> str:
         return "WikipediaReader"
 
-    def load_data(self, pages: List[str], **load_kwargs: Any) -> List[Document]:
+    def load_data(
+        self, pages: List[str], lang_prefix: str = "en", **load_kwargs: Any
+    ) -> List[Document]:
         """Load data from the input directory.
 
         Args:
             pages (List[str]): List of pages to read.
-
+            lang_prefix (str): Language prefix for Wikipedia. Defaults to English. Valid Wikipedia language codes
+            can be found at https://en.wikipedia.org/wiki/List_of_Wikipedias.
         """
         import wikipedia
 
+        if lang_prefix.lower() != "en":
+            if lang_prefix.lower() in wikipedia.languages():
+                wikipedia.set_lang(lang_prefix.lower())
+            else:
+                raise ValueError(
+                    f"Language prefix '{lang_prefix}' for Wikipedia is not supported. Check supported languages at https://en.wikipedia.org/wiki/List_of_Wikipedias."
+                )
+
         results = []
         for page in pages:
             wiki_page = wikipedia.page(page, **load_kwargs)
             page_content = wiki_page.content
             page_id = wiki_page.pageid
             results.append(Document(id_=page_id, text=page_content))
         return results
```

### Comparing `llama_index_readers_wikipedia-0.1.3/pyproject.toml` & `llama_index_readers_wikipedia-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers wikipedia integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["jerryjliu"]
 name = "llama-index-readers-wikipedia"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_readers_wikipedia-0.1.3/PKG-INFO` & `llama_index_readers_wikipedia-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-wikipedia
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers wikipedia integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: jerryjliu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Readers Integration: Wikipedia
```

