# Comparing `tmp/confluence.md-0.3.1.tar.gz` & `tmp/confluence.md-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluence.md-0.3.1.tar", last modified: Fri Mar 29 17:30:43 2024, max compression
+gzip compressed data, was "confluence.md-0.3.2.tar", last modified: Sat Apr  6 19:04:51 2024, max compression
```

## Comparing `confluence.md-0.3.1.tar` & `confluence.md-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:43.486110 confluence.md-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-29 17:30:43.486110 confluence.md-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-29 17:30:39.000000 confluence.md-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 17:30:39.000000 confluence.md-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-29 17:30:43.486110 confluence.md-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:43.486110 confluence.md-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:43.486110 confluence.md-0.3.1/src/confluence.md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-29 17:30:43.000000 confluence.md-0.3.1/src/confluence.md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-29 17:30:43.000000 confluence.md-0.3.1/src/confluence.md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:30:43.000000 confluence.md-0.3.1/src/confluence.md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 17:30:43.000000 confluence.md-0.3.1/src/confluence.md.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-29 17:30:43.000000 confluence.md-0.3.1/src/confluence.md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 17:30:43.000000 confluence.md-0.3.1/src/confluence.md.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:43.486110 confluence.md-0.3.1/src/md2cf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:39.000000 confluence.md-0.3.1/src/md2cf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5608 2024-03-29 17:30:39.000000 confluence.md-0.3.1/src/md2cf/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:43.486110 confluence.md-0.3.1/src/md2cf/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:30:39.000000 confluence.md-0.3.1/src/md2cf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-03-29 17:30:39.000000 confluence.md-0.3.1/src/md2cf/utils/confluencemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-29 17:30:39.000000 confluence.md-0.3.1/src/md2cf/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-06 19:04:51.125210 confluence.md-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-06 19:04:47.000000 confluence.md-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 19:04:47.000000 confluence.md-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-06 19:04:51.125210 confluence.md-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.121210 confluence.md-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/src/confluence.md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/src/md2cf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5608 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/src/md2cf/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/utils/confluencemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/utils/log.py
```

### Comparing `confluence.md-0.3.1/PKG-INFO` & `confluence.md-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluence.md
-Version: 0.3.1
+Version: 0.3.2
 Summary: Markdown to Confluence - upload any .md files to your Confluence cloud page
 Home-page: https://github.com/szn/confluence.md
 Download-URL: 
 Author: Szymon Nieradka
 License: MIT
 Project-URL: Bug Tracker, https://github.com/szn/confluence.md/issues
 Keywords: markdown,confluence,md,atlassian
```

### Comparing `confluence.md-0.3.1/README.md` & `confluence.md-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `confluence.md-0.3.1/setup.cfg` & `confluence.md-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confluence.md
-version = 0.3.1
+version = 0.3.2
 author = Szymon Nieradka
 description = Markdown to Confluence - upload any .md files to your Confluence cloud page
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/szn/confluence.md
 project_urls = 
 	Bug Tracker = https://github.com/szn/confluence.md/issues
```

### Comparing `confluence.md-0.3.1/src/confluence.md.egg-info/PKG-INFO` & `confluence.md-0.3.2/src/confluence.md.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluence.md
-Version: 0.3.1
+Version: 0.3.2
 Summary: Markdown to Confluence - upload any .md files to your Confluence cloud page
 Home-page: https://github.com/szn/confluence.md
 Download-URL: 
 Author: Szymon Nieradka
 License: MIT
 Project-URL: Bug Tracker, https://github.com/szn/confluence.md/issues
 Keywords: markdown,confluence,md,atlassian
```

### Comparing `confluence.md-0.3.1/src/md2cf/main.py` & `confluence.md-0.3.2/src/md2cf/main.py`

 * *Files identical despite different names*

### Comparing `confluence.md-0.3.1/src/md2cf/utils/confluencemd.py` & `confluence.md-0.3.2/src/md2cf/utils/confluencemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         self.md_file = md_file
         self.add_meta = add_meta
         self.add_info_panel = add_info_panel
         self.add_label = add_label
         self.md_file_dir = os.path.dirname(md_file)
         self.convert_jira = convert_jira
 
-    def rewrite_issues(self, html):
+    def rewrite_issues(self, html: str) -> str:
         if not self.convert_jira:
-            return
+            return html
         logger.debug("Replacing [ISSUE-KEY] with html links")
         issues = []
         for issue in ISSUE_PATTERN.finditer(html):
             issues.append((issue.group(), issue.group("key")))
         for issue in ISSUE_PATTERN_URL.finditer(html):
             if self.url.startswith(issue.group("domain")):
                 issues.append((issue.group(), issue.group("key")))
@@ -80,17 +80,16 @@
             status = issue['fields']['status']['name']
             issuetypeurl = issue['fields']['issuetype']['iconUrl']
             return (summary, status, issuetypeurl)
         except (RuntimeError, AssertionError, Exception) as error:
             logger.info("Unable to convert %s to Jira link: %s", key, error)
             return (None, None, None)
 
-
     def rewrite_images(
-        self, page_id: str, html: str, images: List[Tuple[str, str]]
+        self, html: str, images: List[Tuple[str, str]]
     ) -> str:
         """Replaces <img> html tags with Confluence specific <ac:image> and uploads
            images as attachements"""
         for (alt, path) in images:
             rel_path = os.path.join(self.md_file_dir, path)
             if not os.path.isfile(rel_path):
                 assert os.path.isfile(path), f"File `{path}` does not exist"
@@ -283,15 +282,15 @@
             ],
         )
         page_id_from_meta, url = ConfluenceMD.parse_confluence_url(html.metadata)
         if self.add_info_panel:
             html = self.get_info_panel() + html
 
         html = self.rewrite_issues(html)
-        html = self.rewrite_images(page_id if page_id else page_id_from_meta, html, images)
+        html = self.rewrite_images(html, images)
         return html, page_id_from_meta, url, len(images) > 0
 
     @staticmethod
     def parse_confluence_url(meta: Dict[str, str]) -> Tuple[Optional[str], Optional[str]]:
         """Parses Confluence page URL and returns page_id and host"""
         if "confluence-url" not in meta:
             return (None, None)
```

### Comparing `confluence.md-0.3.1/src/md2cf/utils/log.py` & `confluence.md-0.3.2/src/md2cf/utils/log.py`

 * *Files identical despite different names*

