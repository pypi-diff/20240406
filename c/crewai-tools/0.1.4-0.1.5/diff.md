# Comparing `tmp/crewai_tools-0.1.4.tar.gz` & `tmp/crewai_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.1.4.tar", max compression
+gzip compressed data, was "crewai_tools-0.1.5.tar", max compression
```

## Comparing `crewai_tools-0.1.4.tar` & `crewai_tools-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.4/LICENSE
--rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.4/README.md
--rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.4/crewai_tools/__init__.py
--rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.4/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.4/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.4/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.4/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.4/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1682 2024-04-04 16:45:56.494162 crewai_tools-0.1.4/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.4/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.494340 crewai_tools-0.1.4/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.4/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.4/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.4/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1739 2024-04-04 16:45:56.494732 crewai_tools-0.1.4/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.4/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1601 2024-04-04 16:45:56.494892 crewai_tools-0.1.4/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.4/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.4/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     2733 2024-03-27 18:04:45.823902 crewai_tools-0.1.4/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     1995 2024-04-04 16:45:56.495032 crewai_tools-0.1.4/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.4/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1636 2024-04-04 16:45:56.495258 crewai_tools-0.1.4/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.4/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.495395 crewai_tools-0.1.4/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.4/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1421 2024-03-27 18:04:45.826870 crewai_tools-0.1.4/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.4/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.1.4/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.4/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.4/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.4/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.4/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.4/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2107 2024-03-02 15:41:34.656120 crewai_tools-0.1.4/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.4/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.4/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.4/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.4/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.4/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1586 2024-04-04 16:45:56.495704 crewai_tools-0.1.4/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.4/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1672 2024-04-04 16:45:56.495856 crewai_tools-0.1.4/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.4/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.496107 crewai_tools-0.1.4/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.4/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     2030 2024-04-04 16:45:56.496381 crewai_tools-0.1.4/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.4/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1804 2024-04-04 16:45:56.496557 crewai_tools-0.1.4/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      730 2024-04-04 16:46:02.436174 crewai_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3550 2024-02-26 00:09:39.177886 crewai_tools-0.1.5/README.md
+-rw-r--r--   0        0        0      470 2024-03-03 02:54:55.157064 crewai_tools-0.1.5/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.1.5/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.1.5/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1410 2024-03-03 02:54:59.436707 crewai_tools-0.1.5/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.1.5/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.1.5/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1682 2024-04-04 16:45:56.494162 crewai_tools-0.1.5/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.1.5/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.494340 crewai_tools-0.1.5/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.1.5/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.1.5/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.1.5/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1739 2024-04-04 16:45:56.494732 crewai_tools-0.1.5/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.1.5/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1601 2024-04-04 16:45:56.494892 crewai_tools-0.1.5/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.1.5/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1056 2024-02-29 06:10:11.674186 crewai_tools-0.1.5/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2733 2024-03-27 18:04:45.823902 crewai_tools-0.1.5/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     2226 2024-04-06 01:44:50.972453 crewai_tools-0.1.5/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.1.5/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1636 2024-04-04 18:15:36.456434 crewai_tools-0.1.5/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.1.5/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.495395 crewai_tools-0.1.5/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.1.5/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1421 2024-03-27 18:04:45.826870 crewai_tools-0.1.5/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.1.5/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.1.5/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.1.5/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.1.5/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.1.5/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.1.5/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.1.5/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2107 2024-03-02 15:41:34.656120 crewai_tools-0.1.5/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.1.5/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2558 2024-02-29 06:10:11.665178 crewai_tools-0.1.5/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.1.5/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1365 2024-03-03 02:55:52.486790 crewai_tools-0.1.5/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.1.5/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1586 2024-04-04 16:45:56.495704 crewai_tools-0.1.5/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.1.5/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1672 2024-04-04 16:45:56.495856 crewai_tools-0.1.5/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.1.5/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1580 2024-04-04 16:45:56.496107 crewai_tools-0.1.5/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.1.5/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     2030 2024-04-04 16:45:56.496381 crewai_tools-0.1.5/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.1.5/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1804 2024-04-04 16:45:56.496557 crewai_tools-0.1.5/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      730 2024-04-06 01:45:07.095076 crewai_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 crewai_tools-0.1.5/PKG-INFO
```

### Comparing `crewai_tools-0.1.4/LICENSE` & `crewai_tools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/README.md` & `crewai_tools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/adapters/embedchain_adapter.py` & `crewai_tools-0.1.5/crewai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.1.5/crewai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/__init__.py` & `crewai_tools-0.1.5/crewai_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/base_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/code_docs_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/code_docs_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/csv_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/csv_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/csv_search_tool/csv_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/csv_search_tool/csv_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/directory_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/directory_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/directory_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/docx_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/docx_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/docx_search_tool/docx_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/docx_search_tool/docx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/github_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,34 +32,39 @@
     gh_token: str
     args_schema: Type[BaseModel] = GithubSearchToolSchema
     content_types: List[str]
 
     def __init__(self, github_repo: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         if github_repo is not None:
-            self.add(github_repo)
+            self.add(repo=github_repo)
             self.description = f"A tool that can be used to semantic search a query the {github_repo} github repo's content."
             self.args_schema = FixedGithubSearchToolSchema
 
     def add(
         self,
-        *args: Any,
+        repo: str,
+        content_types: List[str] | None = None,
         **kwargs: Any,
     ) -> None:
+        content_types = content_types or self.content_types
+
         kwargs["data_type"] = "github"
         kwargs["loader"] = GithubLoader(config={"token": self.gh_token})
-        super().add(*args, **kwargs)
+        super().add(f"repo:{repo} type:{','.join(content_types)}", **kwargs)
 
     def _before_run(
         self,
         query: str,
         **kwargs: Any,
     ) -> Any:
         if "github_repo" in kwargs:
-            self.add(kwargs["github_repo"])
+            self.add(
+                repo=kwargs["github_repo"], content_types=kwargs.get("content_types")
+            )
 
     def _run(
         self,
         search_query: str,
         **kwargs: Any,
     ) -> Any:
         return super()._run(query=search_query)
```

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/json_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/json_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/json_search_tool/json_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/json_search_tool/json_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/mdx_seach_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/mdx_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/pdf_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/pdf_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/pg_seach_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/pg_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/pg_seach_tool/pg_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/pg_seach_tool/pg_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/rag/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/rag/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/rag/rag_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/rag/rag_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.1.5/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/txt_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/txt_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/website_search/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/website_search/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/xml_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/xml_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/xml_search_tool/xml_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/xml_search_tool/xml_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/youtube_channel_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/youtube_channel_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/youtube_video_search_tool/README.md` & `crewai_tools-0.1.5/crewai_tools/tools/youtube_video_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py` & `crewai_tools-0.1.5/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.1.4/pyproject.toml` & `crewai_tools-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.1.4"
+version = "0.1.5"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
```

### Comparing `crewai_tools-0.1.4/PKG-INFO` & `crewai_tools-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

