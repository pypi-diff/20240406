# Comparing `tmp/facebook_page_scraper-5.0.3.tar.gz` & `tmp/facebook_page_scraper-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_page_scraper-5.0.3.tar", last modified: Sat Mar 30 08:59:05 2024, max compression
+gzip compressed data, was "facebook_page_scraper-5.0.4.tar", last modified: Sat Apr  6 05:28:51 2024, max compression
```

## Comparing `facebook_page_scraper-5.0.3.tar` & `facebook_page_scraper-5.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 08:59:05.920895 facebook_page_scraper-5.0.3/
--rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.3/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    13544 2024-03-30 08:59:05.918900 facebook_page_scraper-5.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12100 2024-03-30 08:55:07.000000 facebook_page_scraper-5.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 08:59:05.886894 facebook_page_scraper-5.0.3/facebook_page_scraper/
--rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.3/facebook_page_scraper/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.3/facebook_page_scraper/driver_initialization.py
--rw-rw-rw-   0        0        0     8090 2024-03-30 08:49:54.000000 facebook_page_scraper-5.0.3/facebook_page_scraper/driver_utilities.py
--rw-rw-rw-   0        0        0    22655 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.3/facebook_page_scraper/element_finder.py
--rw-rw-rw-   0        0        0    18018 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.3/facebook_page_scraper/scraper.py
--rw-rw-rw-   0        0        0     5435 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.3/facebook_page_scraper/scraping_utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-30 08:59:05.917897 facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/
--rw-rw-rw-   0        0        0    13544 2024-03-30 08:59:05.000000 facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-03-30 08:59:05.000000 facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 08:59:05.000000 facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-03-30 08:59:05.000000 facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-30 08:59:05.000000 facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 08:59:05.920895 facebook_page_scraper-5.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1744 2024-03-30 08:58:29.000000 facebook_page_scraper-5.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:28:51.938172 facebook_page_scraper-5.0.4/
+-rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.4/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    13544 2024-04-06 05:28:51.936184 facebook_page_scraper-5.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12100 2024-03-30 08:55:07.000000 facebook_page_scraper-5.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 05:28:51.898170 facebook_page_scraper-5.0.4/facebook_page_scraper/
+-rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/driver_initialization.py
+-rw-rw-rw-   0        0        0     8090 2024-03-30 08:49:54.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/driver_utilities.py
+-rw-rw-rw-   0        0        0    22657 2024-04-06 05:28:13.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/element_finder.py
+-rw-rw-rw-   0        0        0    18018 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/scraper.py
+-rw-rw-rw-   0        0        0     5435 2024-03-30 08:49:55.000000 facebook_page_scraper-5.0.4/facebook_page_scraper/scraping_utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-06 05:28:51.935174 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/
+-rw-rw-rw-   0        0        0    13544 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-06 05:28:51.000000 facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 05:28:51.939168 facebook_page_scraper-5.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2024-04-06 05:28:13.000000 facebook_page_scraper-5.0.4/setup.py
```

### Comparing `facebook_page_scraper-5.0.3/LICENSE` & `facebook_page_scraper-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.3/PKG-INFO` & `facebook_page_scraper-5.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_page_scraper
-Version: 5.0.3
+Version: 5.0.4
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.3 Summary:
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.4 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `facebook_page_scraper-5.0.3/README.md` & `facebook_page_scraper-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.3/facebook_page_scraper/driver_initialization.py` & `facebook_page_scraper-5.0.4/facebook_page_scraper/driver_initialization.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.3/facebook_page_scraper/driver_utilities.py` & `facebook_page_scraper-5.0.4/facebook_page_scraper/driver_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.3/facebook_page_scraper/element_finder.py` & `facebook_page_scraper-5.0.4/facebook_page_scraper/element_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,23 +75,25 @@
                 )
                 print("old link layouut\n")
                 # extract out post id from post's url
                 status = Scraping_utilities._Scraping_utilities__extract_id_from_link(
                     status_link
                 )
             elif layout == "new":
-                
+
                 link = post.find_element(
                     By.CSS_SELECTOR, 'span > a[role="link"]' if isGroup else 'span > a[aria-label][role="link"]'
                 )
                 if link is not None:
                     status_link = link.get_attribute("href")
                     status = Scraping_utilities._Scraping_utilities__extract_id_from_link(
                         status_link
                     )
+                    if not isGroup and status_link and status: #early exit for non group
+                        return (status, status_link, link)
 
                 links = post.find_elements(By.TAG_NAME, 'a')
                 if links:
                     # Initialize variables to store the matching link element and URL
                     matching_link_element = None
                     post_url = None
 
@@ -303,31 +305,31 @@
                     # NOTE There is no aria_label on these link elements anymore
                     # Facebook uses a shadowDOM element to hide timestamp, which is tricky to extract
                     # An unsuccesful attempt to extract time from nested shadowDOMs is below
 
                     js_script = """
                         // Starting from the provided element, find the SVG using querySelector
                         var svgElement = arguments[0].querySelector('svg');
-                        
+
                         // Assuming we're looking for a shadow DOM inside or related to the <use> tag, which is unconventional
                         // var useElement = svgElement.querySelector('use');
-                        
+
                         // Placeholder for accessing the shadow DOM, which is not directly applicable to <use> tags.
                         // This step assumes there's some unconventional method to access related shadow content
                         var shadowContent;
-                        
+
                         // Hypothetically accessing shadow DOM or related content. This part needs adjustment based on actual structure or intent
                         // As <use> tags don't host shadow DOMs, this is speculative and might represent a different approach in practice
                         if (svgElement.shadowRoot) {
                             shadowContent = svgElement.shadowRoot.querySelector('some-element').textContent;
                         } else {
                             // Fallback or alternative method to access intended content, as direct shadow DOM access on <use> is not standard
                             shadowContent = 'Fallback or alternative content access method needed';
                         }
-                        
+
                         return shadowContent;
                     """
                     # Execute the script with the link_element as the argument
                     timestamp = driver.execute_script(js_script, link_element)
                     print("TIMESTAMP: " + str(timestamp))
                 elif not isGroup:
                     aria_label_value = link_element.get_attribute("aria-label")
@@ -417,25 +419,25 @@
             Utilities.__close_driver(driver)
             sys.exit(1)
 
     @staticmethod
     def __find_name(driverOrPost, layout):
         """finds name of the facebook page or post using selenium's webdriver's method"""
         # Attempt to print the outer HTML of the driverOrPost for debugging
-        
+
         try:
             if layout == "old":
                 name = driverOrPost.find_element(By.CSS_SELECTOR, "a._64-f").get_attribute(
                     "textContent"
             )
             elif layout == "new":
                 name = driverOrPost.find_element(By.TAG_NAME, "strong").get_attribute(
                     "textContent"
                 )
-                
+
             return name
         except Exception as ex:
             logger.exception("Error at __find_name method : {}".format(ex))
 
     @staticmethod
     def __detect_ui(driver):
         try:
@@ -481,15 +483,15 @@
 
             # NOTE this closes the login modal pop-up if you choose to not login above
             try:
                 element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[aria-label="Close"]')))
                 element.click()  # Click the element
             except Exception as ex:
                 print(f"no pop-up")
-            
+
             time.sleep(1)
             #target username
             username_element = WebDriverWait(driver, 10).until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input[name='email']")))
             password_element = WebDriverWait(driver, 10).until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input[name='pass']")))
 
             #enter username and password
             username_element.clear()
```

### Comparing `facebook_page_scraper-5.0.3/facebook_page_scraper/scraper.py` & `facebook_page_scraper-5.0.4/facebook_page_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.3/facebook_page_scraper/scraping_utilities.py` & `facebook_page_scraper-5.0.4/facebook_page_scraper/scraping_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.3/facebook_page_scraper.egg-info/PKG-INFO` & `facebook_page_scraper-5.0.4/facebook_page_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_page_scraper
-Version: 5.0.3
+Version: 5.0.4
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.3 Summary:
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.4 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `facebook_page_scraper-5.0.3/setup.py` & `facebook_page_scraper-5.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                 'webdriver-manager==3.2.2',
                 'selenium-wire==5.1.0',
                 'python-dateutil==2.8.2']
 
 
 setuptools.setup(
     name="facebook_page_scraper",
-    version="5.0.3",
+    version="5.0.4",
     author="Sajid Shaikh",
     author_email="shaikhsajid3732@gmail.com",
     description="Python package to scrap facebook's pages front end with no limitations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/shaikhsajid1111/facebook_page_scraper",
```

