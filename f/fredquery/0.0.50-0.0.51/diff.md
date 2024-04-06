# Comparing `tmp/fredquery-0.0.50.tar.gz` & `tmp/fredquery-0.0.51.tar.gz`

## Comparing `fredquery-0.0.50.tar` & `fredquery-0.0.51.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.50/Ploteg0.ipynb
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 fredquery-0.0.50/genusage.sh
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 fredquery-0.0.50/notes.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fredquery-0.0.50/requirements.txt
--rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.50/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/__about__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/__init__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/aa2csv.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/aa2html.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredcategories.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredplot.py
--rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredplotseries.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredreleases.py
--rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredseries.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredsources.py
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/fredtags.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/query.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fredquery-0.0.50/src/fredquery/xmlstr2aa.py
--rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 fredquery-0.0.50/tests/p.sh
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 fredquery-0.0.50/tests/plot.sh
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 fredquery-0.0.50/tests/s.sh
--rwxr-xr-x   0        0        0     2228 2020-02-02 00:00:00.000000 fredquery-0.0.50/tests/x.sh
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fredquery-0.0.50/LICENSE.txt
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 fredquery-0.0.50/README.md
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fredquery-0.0.50/pyproject.toml
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 fredquery-0.0.50/PKG-INFO
+-rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.51/Ploteg0.ipynb
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 fredquery-0.0.51/genusage.sh
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 fredquery-0.0.51/notes.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fredquery-0.0.51/requirements.txt
+-rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.51/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/__about__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/__init__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/aa2csv.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/aa2html.py
+-rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredcategories.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredplot.py
+-rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredplotseries.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredreleases.py
+-rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredseries.py
+-rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredsources.py
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/fredtags.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/query.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fredquery-0.0.51/src/fredquery/xmlstr2aa.py
+-rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 fredquery-0.0.51/tests/p.sh
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 fredquery-0.0.51/tests/plot.sh
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 fredquery-0.0.51/tests/s.sh
+-rwxr-xr-x   0        0        0     2228 2020-02-02 00:00:00.000000 fredquery-0.0.51/tests/x.sh
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fredquery-0.0.51/LICENSE.txt
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 fredquery-0.0.51/README.md
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fredquery-0.0.51/pyproject.toml
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 fredquery-0.0.51/PKG-INFO
```

### Comparing `fredquery-0.0.50/Ploteg0.ipynb` & `fredquery-0.0.51/Ploteg0.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/notes.txt` & `fredquery-0.0.51/notes.txt`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb` & `fredquery-0.0.51/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/aa2html.py` & `fredquery-0.0.51/src/fredquery/aa2html.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/fredcategories.py` & `fredquery-0.0.51/src/fredquery/fredcategories.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     collect and report stlouisfed.org FRED categories, their series, and
     their observations(timeseries data)
     """
     def __init__(self):
         self.cid = None
         self.curl = 'https://fred.stlouisfed.org/categories'
         self.acurl = 'https://api.stlouisfed.org/fred/category'
+        self.ccurl = 'https://api.stlouisfed.org/fred/category/children'
         self.csurl = 'https://api.stlouisfed.org/fred/category/series'
         self.ssurl = 'https://api.stlouisfed.org/fred/series'
         self.sourl = 'https://api.stlouisfed.org/fred/series/observations'
         self.kurl = 'https://fred.stlouisfed.org/docs/api/api_key.html'
         self.rapi_key = 'FRED_API_KEY'
         if 'FRED_API_KEY' in os.environ:
             self.api_key = os.environ['FRED_API_KEY']
@@ -45,14 +46,15 @@
             print('FRED api_key required: %s' % (self.kurl), file=sys.stderr)
             print('assign this key to FRED_API_KEY env variable',
                                   file=sys.stderr)
             sys.exit()
         self.npages  = 7
         self.verbose = False
         self.categorydict= {}
+        self.catchilddict= {}
         self.seriesdict = {}
         self.observationsdict = {}
 
         self.uq = query._URLQuery()
         self.ah = aa2html._AA2HTML()
         self.xa = xmlstr2aa._XMLStr2AA()
 
@@ -103,15 +105,16 @@
             return
         self.ah.aashow(self.seriesdict[id], 'Category %s series' % id)
 
     def reportseries(self, id, ofp):
         """ reportseries(ofp)
 
         report series data for categories
-        rstr - decoded response of a urllib request
+        id - category_id
+        ofp - output file pointer
         """
         aa = self.seriesdict[id]
         for a in aa:
             row = "','".join(a)
             print("'%s'" % (row), file=ofp)
 
     def returnseriesforcid(self, cid):
@@ -157,14 +160,68 @@
             aa = self.categorydict[k]
             assert aa[0][0] == 'cid'
             for i in range(1, len(aa) ):
                 a = aa[i]
                 cid = a[0]
                 self.getseriesforcid(cid)
 
+    def showchildrenforcid(self, cid):
+        """ showchildrenforcid(cid)
+
+        show the children categories for a category_id in your browser
+        cid - category_id
+        """
+        if cid not in self.catchilddict:
+            print('no data for category_id %s' % (cid), file=sys.stderr )
+            return
+        self.ah.aashow(self.catchilddict[cid], 'Category %s children' % cid)
+
+    def reportchildrenforcid(self, cid, ofp):
+        """ reportchildrenforcid(ofp)
+
+        report child data for categories
+        id - category_id
+        ofp - output file pointer
+        """
+        aa = self.catchilddict[cid]
+        for a in aa:
+            row = "','".join(a)
+            print("'%s'" % (row), file=ofp)
+
+    def returnchildrenforcid(self, cid):
+        if cid in self.catchilddict:
+            return self.catchilddict[cid]
+        return None
+
+    def getcategorychilddata(self, cid, rstr):
+        """ getcategorychilddata(cid, rstr)
+
+        get child data for a category_id
+        cid - category_id
+        rstr - url request query string
+        """
+        aa = self.xa.xmlstr2aa(rstr)
+        if len(aa) == 0:
+            print('getcategorychilddata(%s): no data' % (cid), file=sys.stderr)
+            return
+        self.catchilddict[cid] = aa
+
+    def getchildrenforcid(self, cid):
+        """ getchildrenforcid(cid)
+
+        get the child categories for a category_id
+        cid - category_id
+        """
+        url = '%s?category_id=%s&api_key=%s' % (self.ccurl, cid,
+              self.api_key)
+        resp = self.uq.query(url)
+        rstr = resp.read().decode('utf-8')
+        # print(rstr, file=sys.stderr)
+        self.getcategorychilddata(cid, rstr)
+
     def returncategories(self):
         cata = []
         for k in self.categorydict.keys():
             aa = self.categorydict[k]
             cata.extend(aa)
         return cata
 
@@ -265,14 +322,18 @@
 def main():
     argp = argparse.ArgumentParser(description='collect and report stlouisfed.org FRED categories and/or series')
 
     argp.add_argument('--categories', action='store_true', default=False,
                        help="report category data")
     argp.add_argument('--showcategories', action='store_true', default=False,
                        help="show categories in your browser")
+    argp.add_argument('--children', action='store_true', default=False,
+                       help="report category child data")
+    argp.add_argument('--showchildren', action='store_true', default=False,
+                       help="show children of a category  in your browser")
     argp.add_argument('--series', action='store_true', default=False,
                        help="report series urls for categories collected")
     argp.add_argument('--showseries', action='store_true', default=False,
                        help="show series for a category in your browser")
     argp.add_argument('--observations', action='store_true', default=False,
                        help="report timeseries data for categories")
 
@@ -284,15 +345,16 @@
             the file is created in the current directory")
     argp.add_argument('--directory',
                     help="directory to write the output use --directory for\n\
                          storing observations, filenames autogenerated")
 
     args = argp.parse_args()
 
-    if not args.categories and not args.series and not args.observations:
+    if not args.categories and not args.children and \
+       not args.series and not args.observations:
         argp.print_help()
         sys.exit()
 
     ofn = None
     fp = sys.stdout
 
     if not args.observations:
@@ -317,14 +379,22 @@
         if args.categoryid:
             fc.getseriesforcid(cid=args.categoryid)
             fc.getandreportobservations(odir=args.directory)
         else:
             fc.getcategories()
             fc.getseries()
             fc.getandreportobservations(odir=args.directory)
+    elif args.children and args.categoryid:
+        fc.getchildrenforcid(args.categoryid)
+        if args.showchildren:
+            fc.showchildrenforcid(args.categoryid)
+            if fp != sys.stdout:
+                fc.reportchildrenforcid(args.categoryid, ofp=fp)
+        else:
+            fc.reportchildrenforcid(args.categoryid, ofp=fp)
     elif args.series and args.categoryid:
         fc.getseriesforcid(cid=args.categoryid)
         if args.showseries:
             fc.showseries(args.categoryid)
             if fp != sys.stdout:
                 fc.reportseries(args.categoryid, ofp=fp)
         else:
```

### Comparing `fredquery-0.0.50/src/fredquery/fredplot.py` & `fredquery-0.0.51/src/fredquery/fredplot.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/fredplotseries.py` & `fredquery-0.0.51/src/fredquery/fredplotseries.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/fredreleases.py` & `fredquery-0.0.51/src/fredquery/fredreleases.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/fredseries.py` & `fredquery-0.0.51/src/fredquery/fredseries.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/fredsources.py` & `fredquery-0.0.51/src/fredquery/fredsources.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/fredtags.py` & `fredquery-0.0.51/src/fredquery/fredtags.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/query.py` & `fredquery-0.0.51/src/fredquery/query.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/src/fredquery/xmlstr2aa.py` & `fredquery-0.0.51/src/fredquery/xmlstr2aa.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/tests/p.sh` & `fredquery-0.0.51/tests/p.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/tests/s.sh` & `fredquery-0.0.51/tests/s.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/tests/x.sh` & `fredquery-0.0.51/tests/x.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/LICENSE.txt` & `fredquery-0.0.51/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/README.md` & `fredquery-0.0.51/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,25 +33,27 @@
 
 ## [Usage]
 
 <br/>
 ##<br/>
 ## fredcategories<br/>
 ##<br/>
-usage: fredcategories [-h] [--categories] [--showcategories] [--series]<br/>
-[--showseries] [--observations]<br/>
-[--categoryid CATEGORYID] [--file FILE]<br/>
-[--directory DIRECTORY]<br/>
+usage: fredcategories [-h] [--categories] [--showcategories] [--children]<br/>
+[--showchildren] [--series] [--showseries]<br/>
+[--observations] [--categoryid CATEGORYID]<br/>
+[--file FILE] [--directory DIRECTORY]<br/>
 <br/>
 collect and report stlouisfed.org FRED categories and/or series<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --categories          report category data<br/>
 --showcategories      show categories in your browser<br/>
+--children            report category child data<br/>
+--showchildren        show children of a category in your browser<br/>
 --series              report series urls for categories collected<br/>
 --showseries          show series for a category in your browser<br/>
 --observations        report timeseries data for categories<br/>
 --categoryid CATEGORYID<br/>
 categories are identified by category_id<br/>
 --file FILE           path to an output filename if just a filename and--<br/>
 directory is not provided the file is created in the<br/>
```

### Comparing `fredquery-0.0.50/pyproject.toml` & `fredquery-0.0.51/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.50/PKG-INFO` & `fredquery-0.0.51/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fredquery
-Version: 0.0.50
+Version: 0.0.51
 Summary: Downloads various stlouisfed.org FRED files to CSV files and creates plots based on category, release, series, source, or tag
 Project-URL: Documentation, https://github.com/dfwcnj/fredquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/fredquery/issues
 Project-URL: Source, https://github.com/dfwcnj/fredquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -55,25 +55,27 @@
 
 ## [Usage]
 
 <br/>
 ##<br/>
 ## fredcategories<br/>
 ##<br/>
-usage: fredcategories [-h] [--categories] [--showcategories] [--series]<br/>
-[--showseries] [--observations]<br/>
-[--categoryid CATEGORYID] [--file FILE]<br/>
-[--directory DIRECTORY]<br/>
+usage: fredcategories [-h] [--categories] [--showcategories] [--children]<br/>
+[--showchildren] [--series] [--showseries]<br/>
+[--observations] [--categoryid CATEGORYID]<br/>
+[--file FILE] [--directory DIRECTORY]<br/>
 <br/>
 collect and report stlouisfed.org FRED categories and/or series<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --categories          report category data<br/>
 --showcategories      show categories in your browser<br/>
+--children            report category child data<br/>
+--showchildren        show children of a category in your browser<br/>
 --series              report series urls for categories collected<br/>
 --showseries          show series for a category in your browser<br/>
 --observations        report timeseries data for categories<br/>
 --categoryid CATEGORYID<br/>
 categories are identified by category_id<br/>
 --file FILE           path to an output filename if just a filename and--<br/>
 directory is not provided the file is created in the<br/>
```

