# Comparing `tmp/CnbcNews-2.0.tar.gz` & `tmp/CnbcNews-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CnbcNews-2.0.tar", last modified: Sat Apr  6 17:14:52 2024, max compression
+gzip compressed data, was "CnbcNews-2.1.tar", last modified: Sat Apr  6 17:40:55 2024, max compression
```

## Comparing `CnbcNews-2.0.tar` & `CnbcNews-2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 17:14:52.115474 CnbcNews-2.0/
-drwxrwxrwx   0        0        0        0 2024-04-06 17:14:52.015140 CnbcNews-2.0/CnbcNews/
--rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-2.0/CnbcNews/__init__.py
--rw-rw-rw-   0        0        0     4633 2024-04-06 17:11:19.000000 CnbcNews-2.0/CnbcNews/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 17:14:52.111473 CnbcNews-2.0/CnbcNews.egg-info/
--rw-rw-rw-   0        0        0     2729 2024-04-06 17:14:51.000000 CnbcNews-2.0/CnbcNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-06 17:14:51.000000 CnbcNews-2.0/CnbcNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 17:14:51.000000 CnbcNews-2.0/CnbcNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-06 17:14:51.000000 CnbcNews-2.0/CnbcNews.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-06 17:14:51.000000 CnbcNews-2.0/CnbcNews.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 17:14:51.000000 CnbcNews-2.0/CnbcNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2729 2024-04-06 17:14:52.114474 CnbcNews-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-06 16:52:16.000000 CnbcNews-2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 17:14:52.116479 CnbcNews-2.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-06 17:14:42.000000 CnbcNews-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:40:55.376283 CnbcNews-2.1/
+drwxrwxrwx   0        0        0        0 2024-04-06 17:40:55.294223 CnbcNews-2.1/CnbcNews/
+-rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-2.1/CnbcNews/__init__.py
+-rw-rw-rw-   0        0        0     4652 2024-04-06 17:39:46.000000 CnbcNews-2.1/CnbcNews/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:40:55.370288 CnbcNews-2.1/CnbcNews.egg-info/
+-rw-rw-rw-   0        0        0     2729 2024-04-06 17:40:54.000000 CnbcNews-2.1/CnbcNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-06 17:40:55.000000 CnbcNews-2.1/CnbcNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 17:40:54.000000 CnbcNews-2.1/CnbcNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-06 17:40:54.000000 CnbcNews-2.1/CnbcNews.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-06 17:40:54.000000 CnbcNews-2.1/CnbcNews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 17:40:54.000000 CnbcNews-2.1/CnbcNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2729 2024-04-06 17:40:55.373290 CnbcNews-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-06 16:52:16.000000 CnbcNews-2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 17:40:55.376283 CnbcNews-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-06 17:40:15.000000 CnbcNews-2.1/setup.py
```

### Comparing `CnbcNews-2.0/CnbcNews/main.py` & `CnbcNews-2.1/CnbcNews/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     :param dropna: Drop rows which contain missing values, True | False
     :return: None
     """
     if field not in ['technology', 'politics', 'tv', 'business', 'markets', 'investing']:
         print("Invalid field. Please provide one of the following sections: 'technology', 'politics', 'tv', 'business', 'markets', 'investing'.")
         return
     
+    print(f"crawling {field} articles ...")
     articles_url = getLinks(field, number,[])
     articles_df = pd.DataFrame({"url":articles_url})
     le = len(articles_df)
     for i in range(number):
         response = requests.get(articles_df.iloc[i].url)
         article_page = BeautifulSoup(response.content, "html.parser")
         article_headline = article_page.find("h1", class_="ArticleHeader-headline")
@@ -66,28 +67,29 @@
         articles_df.loc[i, 'article_body'] = article_body
         articles_df.loc[i, 'article_author'] = article_author
         articles_df.loc[i, 'article_publish_time'] = article_publish_time
         articles_df.loc[i, 'article_label'] = article_label
 
     if dropna: articles_df.dropna(how='any', inplace=True)
     if os.path.exists(f"articles_{field}.csv"):
-        old_articles_df = pd.read_csv(f"articles_{field}.csv").drop(columns=['id'])
+        old_articles_df = pd.read_csv(f"articles_{field}.csv")
         articles_df = pd.concat([old_articles_df, articles_df], ignore_index=True)
     articles_df.drop_duplicates(inplace=True, ignore_index=True)
-    articles_df.to_csv(f"articles_{field}.csv", index_label="id")
+    articles_df.to_csv(f"articles_{field}.csv", index=False)
     articles_url=[]
+    print("done")
+
 
 def from_fields(fields=[], number=10, timeout=6):
     r"""GET the Article from Cnbc
     :param fields: sections of the Articles, 'technology', 'politics', 'tv', 'business', 'markets', 'investing'
     :param number: number of collected articles for each field
     :return: None
     """
-    for field in fields:
-        print(field)
+    for field in fields: 
         getArticles(field=field, number=number)
         time.sleep(timeout)
 
 
 def main():
     import sys
     if len(sys.argv)==4:
```

### Comparing `CnbcNews-2.0/CnbcNews.egg-info/PKG-INFO` & `CnbcNews-2.1/CnbcNews.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 2.0
+Version: 2.1
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-2.0/PKG-INFO` & `CnbcNews-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 2.0
+Version: 2.1
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-2.0/README.md` & `CnbcNews-2.1/README.md`

 * *Files identical despite different names*

### Comparing `CnbcNews-2.0/setup.py` & `CnbcNews-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CnbcNews',
-    version='2.0',
+    version='2.1',
     packages=find_packages(),
     install_requires=[
         'beautifulsoup4',
         'pandas'
     ],
     entry_points={
         "console_scripts": [
```

