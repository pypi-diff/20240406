# Comparing `tmp/zen_dash-0.6.8.tar.gz` & `tmp/zen_dash-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_dash-0.6.8.tar", max compression
+gzip compressed data, was "zen_dash-0.6.9.tar", max compression
```

## Comparing `zen_dash-0.6.8.tar` & `zen_dash-0.6.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.6.8/LICENSE
--rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.6.8/README.md
--rw-r--r--   0        0        0     1288 2023-08-26 05:14:09.661305 zen_dash-0.6.8/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.6.8/zen_dash/__init__.py
--rw-r--r--   0        0        0     1521 2023-07-30 20:54:39.317930 zen_dash-0.6.8/zen_dash/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.6.8/zen_dash/cli/__init__.py
--rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.6.8/zen_dash/cli/main.py
--rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.6.8/zen_dash/cli/project_management.py
--rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/flex_data.py
--rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/instances.py
--rw-r--r--   0        0        0     1403 2023-07-22 15:37:24.864370 zen_dash-0.6.8/zen_dash/objects/__init__.py
--rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/objects/flex_data.py
--rw-r--r--   0        0        0    15249 2023-08-26 04:55:59.129550 zen_dash-0.6.8/zen_dash/objects/instances.py
--rw-r--r--   0        0        0      378 2023-08-15 01:00:21.701529 zen_dash-0.6.8/zen_dash/objects/page.py
--rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/objects/scripts.py
--rw-r--r--   0        0        0     2991 2023-08-17 05:11:11.724756 zen_dash-0.6.8/zen_dash/objects/sidebar.py
--rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/page.py
--rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/route.py
--rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/scripts.py
--rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.6.8/zen_dash/sidebar.py
--rw-r--r--   0        0        0  1017714 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/275.44cd52f9d992445f.js
--rw-r--r--   0        0        0    57081 2023-08-26 05:13:14.137009 zen_dash-0.6.8/zen_dash/static/3rdpartylicenses.txt
--rw-r--r--   0        0        0   128180 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
--rw-r--r--   0        0        0   143258 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
--rw-r--r--   0        0        0    44300 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
--rw-r--r--   0        0        0    57620 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
--rw-r--r--   0        0        0      948 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/favicon.ico
--rw-r--r--   0        0        0     2137 2023-08-26 05:13:14.893013 zen_dash-0.6.8/zen_dash/static/index.html
--rw-r--r--   0        0        0    98772 2023-08-26 05:13:14.137009 zen_dash-0.6.8/zen_dash/static/main.45cf7749f40f66b2.js
--rw-r--r--   0        0        0    33759 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/polyfills.0a8881ff36766b1e.js
--rw-r--r--   0        0        0     3285 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/runtime.6a9b461ae5a72237.js
--rw-r--r--   0        0        0   152653 2023-08-26 04:31:59.993176 zen_dash-0.6.8/zen_dash/static/styles.362a8260c32d36d9.css
--rw-r--r--   0        0        0  3062858 2023-08-26 05:05:30.945014 zen_dash-0.6.8/zen_dash/static/vendor.e2924b5928ad7742.js
--rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.6.8/zen_dash/support/__init__.py
--rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.6.8/zen_dash/support/encoder.py
--rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.6.8/zen_dash/tag/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.6.8/zen_dash/websocket/__init__.py
--rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 zen_dash-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.6.9/LICENSE
+-rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.6.9/README.md
+-rw-r--r--   0        0        0     1288 2023-08-26 14:09:42.288342 zen_dash-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.6.9/zen_dash/__init__.py
+-rw-r--r--   0        0        0     1521 2023-07-30 20:54:39.317930 zen_dash-0.6.9/zen_dash/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.6.9/zen_dash/cli/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.6.9/zen_dash/cli/main.py
+-rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.6.9/zen_dash/cli/project_management.py
+-rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/flex_data.py
+-rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/instances.py
+-rw-r--r--   0        0        0     1403 2023-07-22 15:37:24.864370 zen_dash-0.6.9/zen_dash/objects/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/objects/flex_data.py
+-rw-r--r--   0        0        0    15249 2023-08-26 04:55:59.129550 zen_dash-0.6.9/zen_dash/objects/instances.py
+-rw-r--r--   0        0        0      378 2023-08-15 01:00:21.701529 zen_dash-0.6.9/zen_dash/objects/page.py
+-rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/objects/scripts.py
+-rw-r--r--   0        0        0     2991 2023-08-17 05:11:11.724756 zen_dash-0.6.9/zen_dash/objects/sidebar.py
+-rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/page.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/route.py
+-rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/scripts.py
+-rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.6.9/zen_dash/sidebar.py
+-rw-r--r--   0        0        0  1017714 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/275.44cd52f9d992445f.js
+-rw-r--r--   0        0        0    57081 2023-08-26 14:07:19.730178 zen_dash-0.6.9/zen_dash/static/3rdpartylicenses.txt
+-rw-r--r--   0        0        0   128180 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
+-rw-r--r--   0        0        0   143258 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
+-rw-r--r--   0        0        0    44300 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
+-rw-r--r--   0        0        0    57620 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
+-rw-r--r--   0        0        0      948 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/favicon.ico
+-rw-r--r--   0        0        0     2137 2023-08-26 14:07:20.314187 zen_dash-0.6.9/zen_dash/static/index.html
+-rw-r--r--   0        0        0    98798 2023-08-26 14:07:19.730178 zen_dash-0.6.9/zen_dash/static/main.5464b3cdf07916b6.js
+-rw-r--r--   0        0        0    33759 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/polyfills.0a8881ff36766b1e.js
+-rw-r--r--   0        0        0     3285 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/runtime.6a9b461ae5a72237.js
+-rw-r--r--   0        0        0   152653 2023-08-26 14:02:40.021921 zen_dash-0.6.9/zen_dash/static/styles.362a8260c32d36d9.css
+-rw-r--r--   0        0        0  3063301 2023-08-26 14:06:16.837223 zen_dash-0.6.9/zen_dash/static/vendor.4feeecbf1ad09eca.js
+-rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.6.9/zen_dash/support/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.6.9/zen_dash/support/encoder.py
+-rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.6.9/zen_dash/tag/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.6.9/zen_dash/websocket/__init__.py
+-rw-r--r--   0        0        0     8861 1970-01-01 00:00:00.000000 zen_dash-0.6.9/PKG-INFO
```

### Comparing `zen_dash-0.6.8/LICENSE` & `zen_dash-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/README.md` & `zen_dash-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/pyproject.toml` & `zen_dash-0.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen_dash"
-version = "0.6.8"
+version = "0.6.9"
 license = "MIT"
 description = "Simple yet scable and production ready python dashboard that is better than shiny application for business."
 readme = "README.md"
 authors = ["Zen <zenreportz@pm.me>"]
 homepage = "https://zen-reportz.github.io/zen_dash/index.html"
 repository = "https://github.com/Zen-Reportz/zen_dash"
 include = [
```

### Comparing `zen_dash-0.6.8/zen_dash/auth/__init__.py` & `zen_dash-0.6.9/zen_dash/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/cli/project_management.py` & `zen_dash-0.6.9/zen_dash/cli/project_management.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/objects/__init__.py` & `zen_dash-0.6.9/zen_dash/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/objects/instances.py` & `zen_dash-0.6.9/zen_dash/objects/instances.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/objects/scripts.py` & `zen_dash-0.6.9/zen_dash/objects/scripts.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/objects/sidebar.py` & `zen_dash-0.6.9/zen_dash/objects/sidebar.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/page.py` & `zen_dash-0.6.9/zen_dash/page.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/275.44cd52f9d992445f.js` & `zen_dash-0.6.9/zen_dash/static/275.44cd52f9d992445f.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/3rdpartylicenses.txt` & `zen_dash-0.6.9/zen_dash/static/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf` & `zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot` & `zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2` & `zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff` & `zen_dash-0.6.9/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/favicon.ico` & `zen_dash-0.6.9/zen_dash/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/index.html` & `zen_dash-0.6.9/zen_dash/static/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -7,10 +7,10 @@
   <!-- <link rel="preconnect" href="https://fonts.gstatic.com">
   <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">
   <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"> -->
   <style type="text/css">@font-face{font-family:'Material Symbols Outlined';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialsymbolsoutlined/v134/kJF1BvYX7BgnkSrUwT8OhrdQw4oELdPIeeII9v6oDMzByHX9rA6RzaxHMPdY43zj-jCxv3fzvRNU22ZXGJpEpjC_1n-q_4MrImHCIJIZrDCvHOelbd5zrDAt.woff) format('woff');}.material-symbols-outlined{font-family:'Material Symbols Outlined';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
 <style>.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}body{font-family:Roboto,Helvetica Neue,sans-serif;margin:0;position:relative;overflow:auto;display:inline-block;overflow:hidden}html{margin:0;height:100%;width:100%}body{margin:0;min-height:100%;width:100%}</style><link rel="stylesheet" href="styles.362a8260c32d36d9.css" media="print" onload="this.media='all'"><noscript><link rel="stylesheet" href="styles.362a8260c32d36d9.css"></noscript></head>
 <body class="mat-typography">
   <app-root></app-root>
-<script src="runtime.6a9b461ae5a72237.js" type="module"></script><script src="polyfills.0a8881ff36766b1e.js" type="module"></script><script src="vendor.e2924b5928ad7742.js" type="module"></script><script src="main.45cf7749f40f66b2.js" type="module"></script>
+<script src="runtime.6a9b461ae5a72237.js" type="module"></script><script src="polyfills.0a8881ff36766b1e.js" type="module"></script><script src="vendor.4feeecbf1ad09eca.js" type="module"></script><script src="main.5464b3cdf07916b6.js" type="module"></script>
 
 </body></html>
```

### Comparing `zen_dash-0.6.8/zen_dash/static/main.45cf7749f40f66b2.js` & `zen_dash-0.6.9/zen_dash/static/main.5464b3cdf07916b6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -298,15 +298,15 @@
                     dependencies: [g.O5],
                     styles: [".warn[_ngcontent-%COMP%]{color:#ffffe0}.error[_ngcontent-%COMP%]{color:#ff69b4}.success[_ngcontent-%COMP%]{color:#90ee90;margin:auto;width:50%;padding:10px}"]
                 }), n
             })();
             var At = p(21444),
                 N = p(35732),
                 f = p(52468),
-                J = p(21312),
+                O = p(21312),
                 dt = p(87241),
                 _t = p(84945),
                 at = p(33568),
                 mt = p(95990),
                 ht = p(44551),
                 $t = p(98826);
             let Jt = (() => {
@@ -358,22 +358,22 @@
                                     error: r => this.connect(i, r),
                                     complete: () => this.connect(i, "complete")
                                 }), this.subject.next(o)
                             })
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.LFG(J.gz), t.LFG(f.D))
+                        return new(e || n)(t.LFG(O.gz), t.LFG(f.D))
                     }, n.\u0275prov = t.Yz7({
                         token: n,
                         factory: n.\u0275fac,
                         providedIn: "root"
                     }), n
                 })(),
-                D = (() => {
+                F = (() => {
                     class n {
                         constructor(e, a, i) {
                             this.http = e, this.dataService = a, this.ws = i, this.refresh_listener = new t.vpe, this.config = {
                                 retry_count: 2,
                                 show_right_sidebar: !1,
                                 refresh: {
                                     refresh: !0,
@@ -416,37 +416,37 @@
                         }
                         call_response(e, a, i) {
                             let o = this.get_url(e),
                                 l = {};
                             if (void 0 !== i) {
                                 l = i;
                                 let y = this.dataService.get_all();
-                                Object.entries(y).forEach((F, E) => {
-                                    l.append(E, F)
+                                Object.entries(y).forEach((Z, E) => {
+                                    l.append(E, Z)
                                 })
                             } else l = this.dataService.get_all();
                             let r, c = {
                                     error: "Error or Unathorized"
                                 },
                                 _ = this.get_retry();
-                            return r = void 0 === a ? this.http.post(o, l).pipe((0, at.K)((y, F) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(2e3), (0, ht.b)(() => F)) : new dt.y(E => {
+                            return r = void 0 === a ? this.http.post(o, l).pipe((0, at.K)((y, Z) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(2e3), (0, ht.b)(() => Z)) : new dt.y(E => {
                                 E.next(c)
-                            }))) : this.http.post(o, l, a).pipe((0, at.K)((y, F) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => F)) : new dt.y(E => {
+                            }))) : this.http.post(o, l, a).pipe((0, at.K)((y, Z) => _-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => Z)) : new dt.y(E => {
                                 E.next(c)
                             }))), r
                         }
                         second_call_response(e, a, i) {
                             let o = this.get_url(e),
                                 l = this.dataService.get_all();
                             void 0 !== a && (l[a] = i);
                             let r, c = this.get_retry(),
                                 _ = {
                                     error: "Error or Unathorized"
                                 };
-                            return r = this.http.post(o, l).pipe((0, at.K)((y, F) => c-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => F)) : new dt.y(E => {
+                            return r = this.http.post(o, l).pipe((0, at.K)((y, Z) => c-- > 0 && 401 !== y.status ? (0, _t.of)(y).pipe((0, mt.g)(1e3), (0, ht.b)(() => Z)) : new dt.y(E => {
                                 E.next(_)
                             }))), r
                         }
                         my_url() {
                             return window.location.href.split("?")[0]
                         }
                     }
@@ -476,15 +476,15 @@
                     return new(e || n)(t.LFG(Ot.N))
                 }, n.\u0275prov = t.Yz7({
                     token: n,
                     factory: n.\u0275fac,
                     providedIn: "root"
                 }), n
             })();
-            var A = p(46842),
+            var D = p(46842),
                 I = p(9638),
                 G = p(83331),
                 B = p(50814),
                 tt = p(83319),
                 it = p(42094),
                 ft = p(64639),
                 It = p(25295),
@@ -699,15 +699,15 @@
                         this.flexData.set(e, a)
                     }
                     setReactivity(e, a) {
                         this.reactivityData.set(e, a)
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(N.eN), t.Y36(J.gz), t.Y36(D), t.Y36(Mt), t.Y36(f.D))
+                    return new(e || n)(t.Y36(N.eN), t.Y36(O.gz), t.Y36(F), t.Y36(Mt), t.Y36(f.D))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-sidebar"]
                     ],
                     inputs: {
                         url: "url"
@@ -728,20 +728,20 @@
                         ["mat-list-item", "", "type", "button", 3, "routerLink", "queryParams"],
                         [3, "selected", 4, "ngFor", "ngForOf"],
                         [3, "hidden", "url", "isSidebar", "fx", "rd"]
                     ],
                     template: function(e, a) {
                         1 & e && t.YNc(0, ce, 2, 1, "span", 0), 2 & e && t.Q6J("ngIf", !((a.call.config.auth.SSO || a.call.config.auth.UP_Login) && a.auth.not_logged()))
                     },
-                    dependencies: [Yt.d, q.ib, q.yz, G.Hw, B.Hk, B.Tg, B.Ub, B.vS, g.sg, g.O5, J.yS, et],
+                    dependencies: [Yt.d, q.ib, q.yz, G.Hw, B.Hk, B.Tg, B.Ub, B.vS, g.sg, g.O5, O.yS, et],
                     styles: [".mat-icon[_ngcontent-%COMP%]{vertical-align:middle}.toolbar-item-spacer[_ngcontent-%COMP%]{flex:1 1 auto}.app-container[_ngcontent-%COMP%]{height:90%;margin:0}.app-sidenav[_ngcontent-%COMP%]{width:230px}.app-sidenav-content[_ngcontent-%COMP%]{display:flex;height:100%;align-items:center;justify-content:center}"]
                 }), n
             })();
             var m = p(20092),
-                Z = p(11997),
+                A = p(11997),
                 x = p(88659),
                 j = p(39665);
 
             function de(n, s) {
                 if (1 & n) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-card")(1, "mat-card-content")(2, "h2"), t._uU(3, "Login with Username and Password"), t.qZA(), t.TgZ(4, "form")(5, "mat-form-field", 2)(6, "mat-label"), t._uU(7, "Username"), t.qZA(), t._UZ(8, "input", 3), t.qZA(), t.TgZ(9, "mat-form-field", 2)(10, "mat-label"), t._uU(11, "Password"), t.qZA(), t._UZ(12, "input", 4), t.qZA(), t.TgZ(13, "div", 5)(14, "button", 6), t.NdJ("click", function() {
@@ -782,15 +782,15 @@
                     }
                     sso_logic() {
                         let e = this.call.get_url("/auth/login");
                         window.location.replace(e)
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(J.F0), t.Y36(N.eN), t.Y36(D), t.Y36(U.ux))
+                    return new(e || n)(t.Y36(O.F0), t.Y36(N.eN), t.Y36(F), t.Y36(U.ux))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-login"]
                     ],
                     decls: 3,
                     vars: 2,
@@ -802,15 +802,15 @@
                         ["matInput", "", "type", "password"],
                         [2, "display", "flex", "justify-content", "center", "align-items", "center"],
                         ["mat-raised-button", "", "color", "primary", 3, "click"]
                     ],
                     template: function(e, a) {
                         1 & e && (t.TgZ(0, "div", 0), t.YNc(1, de, 16, 0, "mat-card", 1), t.YNc(2, _e, 8, 0, "mat-card", 1), t.qZA()), 2 & e && (t.xp6(1), t.Q6J("ngIf", !a.is_sso), t.xp6(1), t.Q6J("ngIf", a.is_sso))
                     },
-                    dependencies: [m._Y, m.JL, m.F, I.lW, Z.a8, Z.dn, x.KE, x.hX, j.Nt, g.O5]
+                    dependencies: [m._Y, m.JL, m.F, I.lW, A.a8, A.dn, x.KE, x.hX, j.Nt, g.O5]
                 }), n
             })();
 
             function he(n, s) {
                 if (1 & n) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "button", 1), t.NdJ("click", function() {
@@ -826,16 +826,16 @@
             }
 
             function fe(n, s) {
                 1 & n && t._UZ(0, "router-outlet")
             }
             let xe = (() => {
                     class n {
-                        constructor(e, a, i, o, l, r, c, _, y, F, E) {
-                            this.http = i, this.ds = o, this._snackBar = l, this.aRoute = r, this.call = c, this.titleService = _, this.clipboard = y, this.ws = F, this.auth = E, this.durationInSeconds = 5, this.mySize = "500px", this.mySize2 = "500px", this.color = "primary", this.checked = !1, this.mobileQuery = a.matchMedia("(max-width: 600px)"), this._mobileQueryListener = () => e.detectChanges(), this.mobileQuery.addListener(this._mobileQueryListener)
+                        constructor(e, a, i, o, l, r, c, _, y, Z, E) {
+                            this.http = i, this.ds = o, this._snackBar = l, this.aRoute = r, this.call = c, this.titleService = _, this.clipboard = y, this.ws = Z, this.auth = E, this.durationInSeconds = 5, this.mySize = "500px", this.mySize2 = "500px", this.color = "primary", this.checked = !1, this.mobileQuery = a.matchMedia("(max-width: 600px)"), this._mobileQueryListener = () => e.detectChanges(), this.mobileQuery.addListener(this._mobileQueryListener)
                         }
                         ngOnDestroy() {
                             this.mobileQuery.removeListener(this._mobileQueryListener)
                         }
                         setTitle() {
                             this.http.get(this.call.my_url() + "backend/title").subscribe(e => {
                                 this.titleService.setTitle(e), this.title = e
@@ -925,15 +925,15 @@
                             console.log("call refresh"), e.config.websocket.active ? i.request_change() : a.refresh.emit("AutoRefresh")
                         }
                         set_auto(e) {
                             e.checked ? this.runRefresh = setInterval(this.call_refresh, 1e3 * this.call.config.refresh.rate_in_seconds, this.call, this.ds, this.ws) : clearInterval(this.runRefresh)
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(t.sBO), t.Y36(At.vx), t.Y36(N.eN), t.Y36(f.D), t.Y36(U.ux), t.Y36(J.gz), t.Y36(D), t.Y36(T.Dx), t.Y36(gt.TU), t.Y36(Jt), t.Y36(Mt))
+                        return new(e || n)(t.Y36(t.sBO), t.Y36(At.vx), t.Y36(N.eN), t.Y36(f.D), t.Y36(U.ux), t.Y36(O.gz), t.Y36(F), t.Y36(T.Dx), t.Y36(gt.TU), t.Y36(Jt), t.Y36(Mt))
                     }, n.\u0275cmp = t.Xpm({
                         type: n,
                         selectors: [
                             ["app-root"]
                         ],
                         decls: 41,
                         vars: 16,
@@ -982,15 +982,15 @@
                             }
                             if (2 & e) {
                                 const i = t.MAs(12),
                                     o = t.MAs(40);
                                 t.xp6(5), t.Oqu(a.title), t.xp6(2), t.Q6J("ngIf", a.call.show_right_sidebar()), t.xp6(1), t.Q6J("matMenuTriggerFor", i), t.xp6(11), t.Q6J("checked", a.checked), t.xp6(3), t.Udp("width", a.mySize), t.Q6J("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar"), t.xp6(1), t.Udp("width", a.mySize2), t.Q6J("position", "end")("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar2"), t.xp6(6), t.Q6J("color", a.color), t.xp6(3), t.Q6J("ngIf", (a.call.config.auth.SSO || a.call.config.auth.UP_Login) && a.auth.not_logged())("ngIfElse", o)
                             }
                         },
-                        dependencies: [A.Wh, A.yH, I.lW, G.Hw, B.Hk, tt.VK, tt.OP, tt.p6, it.JX, it.TM, it.Rh, ft.Rr, It.Ye, g.O5, J.lC, ue, me],
+                        dependencies: [D.Wh, D.yH, I.lW, G.Hw, B.Hk, tt.VK, tt.OP, tt.p6, it.JX, it.TM, it.Rh, ft.Rr, It.Ye, g.O5, O.lC, ue, me],
                         styles: ["[_nghost-%COMP%]{position:absolute;left:0;right:0;bottom:0;top:0}mat-sidenav-container[_ngcontent-%COMP%]{margin:0;min-height:100%;height:100%;width:100%;display:inline-block}.increase-size[_ngcontent-%COMP%]{width:200px}mat-sidenav[_ngcontent-%COMP%]{min-width:200px}.float[_ngcontent-%COMP%]{position:fixed;bottom:1rem;right:1rem;z-index:5}.app-container[_ngcontent-%COMP%]{height:90%;margin:0}.app-sidenav[_ngcontent-%COMP%]{width:230px}.app-sidenav-content[_ngcontent-%COMP%]{display:flex;height:100%;align-items:center;justify-content:center}.toolbar-item-spacer[_ngcontent-%COMP%]{flex:1 1 auto}"]
                     }), n
                 })(),
                 be = (() => {
                     class n {
                         constructor() {}
                         set_title(e, a, i) {
@@ -1005,44 +1005,45 @@
                         return new(e || n)
                     }, n.\u0275prov = t.Yz7({
                         token: n,
                         factory: n.\u0275fac,
                         providedIn: "root"
                     }), n
                 })();
-            var O = p(88696);
+            var J = p(88696);
             let xt = (() => {
                 class n {
                     constructor(e, a) {
                         this.dialogRef = e, this.data = a
                     }
                     ngOnInit() {}
                     onCancel() {
                         this.dialogRef.close()
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(O.so), t.Y36(O.WI))
+                    return new(e || n)(t.Y36(J.so), t.Y36(J.WI))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-support-dialog"]
                     ],
                     decls: 7,
                     vars: 1,
                     consts: [
-                        [2, "width", "95%", "height", "95%"],
+                        [1, "continer"],
+                        ["mat-dialog-actions", "", 2, "margin-top", "auto", "height", "90%", "overflow-y", "auto"],
                         [2, "margin", "5px", 3, "innerHTML"],
                         ["css", ""],
                         ["mat-button", "", "mat-dialog-close", ""]
                     ],
                     template: function(e, a) {
-                        1 & e && (t.TgZ(0, "mat-card", 0)(1, "mat-card-content"), t._UZ(2, "div", 1, 2), t.qZA(), t.TgZ(4, "mat-card-actions")(5, "button", 3), t._uU(6, "Close"), t.qZA()()()), 2 & e && (t.xp6(2), t.Q6J("innerHTML", a.data.custom_html, t.oJD))
+                        1 & e && (t.TgZ(0, "div", 0)(1, "div", 1), t._UZ(2, "div", 2, 3), t.qZA(), t.TgZ(4, "div")(5, "button", 4), t._uU(6, "Close"), t.qZA()()()), 2 & e && (t.xp6(2), t.Q6J("innerHTML", a.data.custom_html, t.oJD))
                     },
-                    dependencies: [I.lW, Z.a8, Z.dn, Z.hq, O.ZT],
+                    dependencies: [I.lW, J.ZT, J.H8],
                     styles: [".container[_ngcontent-%COMP%]{display:flex;flex-direction:column;border:1px solid #000;min-height:200px;width:100px}"]
                 }), n
             })();
             var Ce = p(8239);
             let bt = (() => {
                 class n {
                     constructor(e, a, i) {
@@ -1141,28 +1142,28 @@
                             let y = c.callService.call_response(a, void 0, void 0);
                             return c.ds.input_emitter.emit({
                                 calling: !0,
                                 lookup: i,
                                 t: void 0,
                                 message: void 0
                             }), c.ds.all_input.delete(i), c.subscription_lookup[i] = yield y.subscribe({
-                                next: F => {
-                                    void 0 === F?.error ? c.updateData(l, a, o, F, i) : c.ds.input_emitter.emit({
+                                next: Z => {
+                                    void 0 === Z?.error ? c.updateData(l, a, o, Z, i) : c.ds.input_emitter.emit({
                                         calling: !1,
                                         lookup: i,
                                         t: void 0,
-                                        message: F.error
+                                        message: Z.error
                                     })
                                 },
-                                error: F => {
+                                error: Z => {
                                     c.ds.input_emitter.emit({
                                         calling: !1,
                                         lookup: i,
                                         t: void 0,
-                                        message: F.message
+                                        message: Z.message
                                     })
                                 }
                             }), {
                                 error: "not called"
                             }
                         })()
                     }
@@ -1220,15 +1221,15 @@
                             delete l.page[o], 0 === Object.keys(l.page).length && delete l.page
                         } catch {}
                         let r = JSON.stringify(l);
                         this.data_[o] = r
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.LFG(f.D), t.LFG(D), t.LFG(O.uw))
+                    return new(e || n)(t.LFG(f.D), t.LFG(F), t.LFG(J.uw))
                 }, n.\u0275prov = t.Yz7({
                     token: n,
                     factory: n.\u0275fac,
                     providedIn: "root"
                 }), n
             })();
 
@@ -1350,15 +1351,15 @@
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(U.ux), t.Y36(bt), t.Y36(O.uw))
+                    return new(e || n)(t.Y36(f.D), t.Y36(F), t.Y36(U.ux), t.Y36(bt), t.Y36(J.uw))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-fab-button"]
                     ],
                     inputs: {
                         url: "url"
@@ -1442,15 +1443,15 @@
                             this.flexData.set(e, a)
                         }
                         setReactivity(e, a) {
                             this.reactivityData.set(e, a)
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(N.eN), t.Y36(T.Dx), t.Y36(J.gz), t.Y36(D), t.Y36(f.D))
+                        return new(e || n)(t.Y36(N.eN), t.Y36(T.Dx), t.Y36(O.gz), t.Y36(F), t.Y36(f.D))
                     }, n.\u0275cmp = t.Xpm({
                         type: n,
                         selectors: [
                             ["app-page"]
                         ],
                         decls: 1,
                         vars: 1,
@@ -1463,29 +1464,29 @@
                             ["class", "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd", 4, "ngFor", "ngForOf"],
                             [1, "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd"],
                             [3, "url"]
                         ],
                         template: function(e, a) {
                             1 & e && t.YNc(0, De, 3, 2, "div", 0), 2 & e && t.Q6J("ngIf", a.page)
                         },
-                        dependencies: [A.xw, A.SQ, A.Wh, A.s9, A.yH, Z.a8, Z.dn, g.sg, g.O5, et, Se],
+                        dependencies: [D.xw, D.SQ, D.Wh, D.s9, D.yH, A.a8, A.dn, g.sg, g.O5, et, Se],
                         styles: [".padding[_ngcontent-%COMP%]{padding:5px;margin-bottom:1em;min-width:100px}.max[_ngcontent-%COMP%]{max-height:200px}"]
                     }), n
                 })()
             }];
             let Ae = (() => {
                 class n {}
                 return n.\u0275fac = function(e) {
                     return new(e || n)
                 }, n.\u0275mod = t.oAB({
                     type: n
                 }), n.\u0275inj = t.cJS({
-                    imports: [J.Bz.forRoot(ke, {
+                    imports: [O.Bz.forRoot(ke, {
                         relativeLinkResolution: "legacy"
-                    }), J.Bz]
+                    }), O.Bz]
                 }), n
             })();
             var Je = p(25544),
                 Oe = p(38954),
                 Me = p(58698),
                 Ie = p(27165),
                 Ye = p(18632),
@@ -1572,15 +1573,15 @@
                             this.flexData.set(e, a)
                         }
                         setReactivity(e, a) {
                             this.reactivityData.set(e, a)
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(O.so), t.Y36(O.WI), t.Y36(N.eN), t.Y36(J.gz), t.Y36(D), t.Y36(f.D))
+                        return new(e || n)(t.Y36(J.so), t.Y36(J.WI), t.Y36(N.eN), t.Y36(O.gz), t.Y36(F), t.Y36(f.D))
                     }, n.\u0275cmp = t.Xpm({
                         type: n,
                         selectors: [
                             ["app-dialog"]
                         ],
                         decls: 1,
                         vars: 1,
@@ -1591,15 +1592,15 @@
                             ["fxLayout", "row wrap", "fxLayout.lt-sm", "column", "fxLayoutGap", "row_data.layoutGap", "fxLayoutAlign", "space-around center", "fxLayoutAlign.lt-sm", "space-around stretch", "fxFlexFill", ""],
                             ["class", "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd", 4, "ngFor", "ngForOf"],
                             [1, "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd"]
                         ],
                         template: function(e, a) {
                             1 & e && t.YNc(0, Ke, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", a.page)
                         },
-                        dependencies: [A.xw, A.SQ, A.Wh, A.s9, A.yH, Z.a8, Z.dn, g.sg, g.O5, et]
+                        dependencies: [D.xw, D.SQ, D.Wh, D.s9, D.yH, A.a8, A.dn, g.sg, g.O5, et]
                     }), n
                 })(),
                 Xe = (() => {
                     class n {
                         constructor(e) {
                             this.ds = e
                         }
@@ -2636,15 +2637,15 @@
                     fileLabel() {
                         return this.data?.label
                     }
                     onSuc(e) {}
                     onErr(e) {}
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(qt.m9), t.Y36(D), t.Y36(U.ux))
+                    return new(e || n)(t.Y36(f.D), t.Y36(qt.m9), t.Y36(F), t.Y36(U.ux))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-app-download"]
                     ],
                     inputs: {
                         url: "url"
@@ -2708,15 +2709,15 @@
                                         status: "error"
                                     }
                                 })
                             })
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(U.ux))
+                        return new(e || n)(t.Y36(f.D), t.Y36(F), t.Y36(U.ux))
                     }, n.\u0275cmp = t.Xpm({
                         type: n,
                         selectors: [
                             ["app-app-upload"]
                         ],
                         inputs: {
                             url: "url"
@@ -2755,15 +2756,15 @@
                             })
                         }
                         ngOnInit() {
                             this.get_data(), this.get_image()
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(T.H7), t.Y36(D))
+                        return new(e || n)(t.Y36(f.D), t.Y36(T.H7), t.Y36(F))
                     }, n.\u0275cmp = t.Xpm({
                         type: n,
                         selectors: [
                             ["app-app-image"]
                         ],
                         inputs: {
                             url: "url"
@@ -2772,15 +2773,15 @@
                         vars: 5,
                         consts: [
                             ["mat-card-sm-image", "", 3, "src"]
                         ],
                         template: function(e, a) {
                             1 & e && (t.TgZ(0, "span"), t._UZ(1, "img", 0), t.qZA()), 2 & e && (t.xp6(1), t.Udp("height", a.height)("width", a.width), t.Q6J("src", a.imageURL, t.LSH))
                         },
-                        dependencies: [Z.vP]
+                        dependencies: [A.vP]
                     }), n
                 })();
             var Ln = p(63156),
                 Rn = p(74970),
                 qn = p(98168),
                 Hn = p(83151),
                 Gn = p(27969);
@@ -2826,15 +2827,15 @@
                         }
                         detectChange(e) {
                             let a = new b;
                             a.key = this.ds.all_input.get(this.url)?.simple_server_filter_data?.name, a.value = e.value, a.page = this.ds.dataLookup(this.isSidebar), a.url = this.url, this.ds.data_setter.emit(a)
                         }
                     }
                     return n.\u0275fac = function(e) {
-                        return new(e || n)(t.Y36(f.D), t.Y36(D))
+                        return new(e || n)(t.Y36(f.D), t.Y36(F))
                     }, n.\u0275cmp = t.Xpm({
                         type: n,
                         selectors: [
                             ["app-simple-server-filter"]
                         ],
                         inputs: {
                             url: "url",
@@ -3015,15 +3016,15 @@
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(U.ux), t.Y36(O.uw))
+                    return new(e || n)(t.Y36(f.D), t.Y36(F), t.Y36(U.ux), t.Y36(J.uw))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-button"]
                     ],
                     inputs: {
                         url: "url"
@@ -3074,15 +3075,15 @@
                             e !== this.current_value && (this.current_value = e, this.fetchSuggestions(e).subscribe(a => {
                                 this.options = a.simple_fitler_data
                             }))
                         })
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(D), t.Y36(kt.KT))
+                    return new(e || n)(t.Y36(F), t.Y36(kt.KT))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-json-forms-server-side"]
                     ],
                     features: [t.qOj],
                     decls: 10,
@@ -3105,15 +3106,15 @@
                             }), t.qZA(), t.TgZ(4, "mat-autocomplete", 2, 3), t.NdJ("optionSelected", function(o) {
                                 return a.onSelect(o)
                             }), t.YNc(6, Wn, 2, 0, "mat-option", 4), t.YNc(7, ta, 2, 1, "ng-container", 5), t.qZA(), t.TgZ(8, "mat-error"), t._uU(9), t.qZA()()), 2 & e) {
                             const i = t.MAs(5);
                             t.xp6(2), t.Oqu(a.label), t.xp6(1), t.s9C("placeholder", a.description), t.Q6J("id", a.id)("formControl", a.form)("matAutocomplete", i), t.xp6(3), t.Q6J("ngIf", a.isLoading), t.xp6(1), t.Q6J("ngIf", !a.isLoading), t.xp6(2), t.Oqu(a.error)
                         }
                     },
-                    dependencies: [A.yH, m.Fj, m.JJ, m.oH, vt.XC, vt.ZL, w.ey, x.TO, x.KE, x.hX, j.Nt, Ut.Ou, g.sg, g.O5]
+                    dependencies: [D.yH, m.Fj, m.JJ, m.oH, vt.XC, vt.ZL, w.ey, x.TO, x.KE, x.hX, j.Nt, Ut.Ou, g.sg, g.O5]
                 }), n
             })();
 
             function na(n, s) {
                 1 & n && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 3), t.qZA())
             }
             const aa = (0, rt.xDy)((0, rt.TDq)("string"), (0, rt.wcO)(n => n.hasOwnProperty("url")));
@@ -3173,15 +3174,15 @@
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(D), t.Y36(U.ux), t.Y36(O.uw))
+                    return new(e || n)(t.Y36(f.D), t.Y36(F), t.Y36(U.ux), t.Y36(J.uw))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-form"]
                     ],
                     inputs: {
                         url: "url"
@@ -3502,15 +3503,15 @@
                             height: this.dialog_data.height,
                             width: this.dialog_data.width,
                             data: this.dialog_data.url
                         })
                     }
                 }
                 return n.\u0275fac = function(e) {
-                    return new(e || n)(t.Y36(f.D), t.Y36(gt.TU), t.Y36(O.uw), t.Y36(bt))
+                    return new(e || n)(t.Y36(f.D), t.Y36(gt.TU), t.Y36(J.uw), t.Y36(bt))
                 }, n.\u0275cmp = t.Xpm({
                     type: n,
                     selectors: [
                         ["app-sub-entry-point"]
                     ],
                     inputs: {
                         url: "url",
@@ -3542,15 +3543,15 @@
                         if (1 & e && (t.TgZ(0, "span", 0), t.NdJ("click", function() {
                                 return a.openDialog()
                             }), t.YNc(1, sa, 2, 1, "span", 1), t.YNc(2, oa, 2, 2, "span", 1), t.YNc(3, la, 2, 1, "span", 1), t.YNc(4, ra, 2, 1, "span", 1), t.YNc(5, pa, 2, 1, "span", 2), t.YNc(6, ca, 2, 2, "span", 2), t.YNc(7, ua, 2, 2, "span", 2), t.YNc(8, da, 2, 2, "span", 2), t.YNc(9, _a, 2, 2, "span", 2), t.YNc(10, ha, 2, 1, "span", 1), t.YNc(11, fa, 3, 1, "span", 1), t.YNc(12, ba, 5, 1, "span", 1), t.YNc(13, Ca, 2, 2, "span", 2), t.YNc(14, va, 2, 2, "span", 2), t.YNc(15, ya, 2, 2, "span", 2), t.YNc(16, Ta, 2, 2, "span", 2), t.YNc(17, Sa, 2, 1, "span", 2), t.YNc(18, wa, 2, 1, "span", 2), t.YNc(19, Za, 2, 1, "span", 1), t.YNc(20, Fa, 2, 1, "span", 1), t.YNc(21, Da, 2, 1, "span", 1), t.YNc(22, ka, 2, 1, "span", 1), t.YNc(23, Aa, 2, 1, "span", 2), t.YNc(24, Ja, 2, 1, "span", 1), t.YNc(25, Oa, 2, 0, "span", 1), t._UZ(26, "br"), t.YNc(27, Ma, 11, 0, "span", 1), t.qZA()), 2 & e) {
                             let i;
                             t.Q6J("matTooltip", null !== (i = null == a.tooltip_data ? null : a.tooltip_data.label) && void 0 !== i ? i : "")("matTooltipDisabled", void 0 === a.tooltip_data), t.xp6(1), t.Q6J("ngIf", "box" === a.type), t.xp6(1), t.Q6J("ngIf", "date" === a.type), t.xp6(1), t.Q6J("ngIf", "table" === a.type), t.xp6(1), t.Q6J("ngIf", "chart" === a.type), t.xp6(1), t.Q6J("ngIf", "checkbox" === a.type), t.xp6(1), t.Q6J("ngIf", "radio" === a.type), t.xp6(1), t.Q6J("ngIf", "slider" === a.type), t.xp6(1), t.Q6J("ngIf", "button_toggle" === a.type), t.xp6(1), t.Q6J("ngIf", "toggle" === a.type), t.xp6(1), t.Q6J("ngIf", "multi_list" === a.type), t.xp6(1), t.Q6J("ngIf", "multi_tabs" === a.type), t.xp6(1), t.Q6J("ngIf", "multi_expand" === a.type), t.xp6(1), t.Q6J("ngIf", "simple_filter" == a.type), t.xp6(1), t.Q6J("ngIf", "simple_server_filter" == a.type), t.xp6(1), t.Q6J("ngIf", "group_filter" == a.type), t.xp6(1), t.Q6J("ngIf", "input" == a.type), t.xp6(1), t.Q6J("ngIf", "download" == a.type), t.xp6(1), t.Q6J("ngIf", "upload" == a.type), t.xp6(1), t.Q6J("ngIf", "image" == a.type), t.xp6(1), t.Q6J("ngIf", "highchart" == a.type), t.xp6(1), t.Q6J("ngIf", "iframe" == a.type), t.xp6(1), t.Q6J("ngIf", "custom_html" == a.type), t.xp6(1), t.Q6J("ngIf", "button" == a.type), t.xp6(1), t.Q6J("ngIf", "form" == a.type), t.xp6(1), t.Q6J("ngIf", a.loading), t.xp6(2), t.Q6J("ngIf", a.failed)
                         }
                     },
-                    dependencies: [A.yH, q.pp, q.ib, q.yz, q.yK, q.u4, G.Hw, tt.OP, K.pW, wt.SP, wt.uX, Et.gM, g.sg, g.O5, Xe, Ve, cn, un, gn, vn, et, yn, Sn, wn, Dn, On, n, Yn, Qn, Nn, En, Ln.q, jn, zn, Ht, $n, ia],
+                    dependencies: [D.yH, q.pp, q.ib, q.yz, q.yK, q.u4, G.Hw, tt.OP, K.pW, wt.SP, wt.uX, Et.gM, g.sg, g.O5, Xe, Ve, cn, un, gn, vn, et, yn, Sn, wn, Dn, On, n, Yn, Qn, Nn, En, Ln.q, jn, zn, Ht, $n, ia],
                     styles: [".center[_ngcontent-%COMP%]{display:flex;justify-content:center;align-items:center}.full[_ngcontent-%COMP%]{width:100%;display:flex;justify-content:center;align-items:center}"]
                 }), n
             })();
             var Ya = p(44740),
                 Pa = p(83787);
             let Qa = (() => {
                     class n {
@@ -3593,21 +3594,21 @@
                         bootstrap: [xe]
                     }), n.\u0275inj = t.cJS({
                         providers: [Ot.N, {
                             provide: N.TP,
                             useClass: Qa,
                             multi: !0
                         }, Gt],
-                        imports: [Ge.o9, m.u5, m.UX, Oe.rt, Me.XD, gt.Iq, Qe.U5, Ct.HT, Ue.nZ, Ie._t, vt.Bb, Ne.g, Ee._r, I.ot, yt.vV, Z.QW, Qt.p9, Le.Hi, Re.T5, H.FA, O.Is, Yt.t, q.To, nt.N6, G.Ps, j.c, B.ie, tt.Tx, w.XK, Tt.TU, K.Cv, Ut.Cq, St.Fk, w.si, st.LD, it.SJ, Nt.KP, ft.rP, U.ZX, ot.JX, Y.p0, wt.Nh, It.g0, Et.AV, qe.dp, He.U8, Ye.eL, Pe.Cl, T.b2, N.JF, Ae, J.Bz, Je.PW, At.xu, Lt.Ns.forRoot({
+                        imports: [Ge.o9, m.u5, m.UX, Oe.rt, Me.XD, gt.Iq, Qe.U5, Ct.HT, Ue.nZ, Ie._t, vt.Bb, Ne.g, Ee._r, I.ot, yt.vV, A.QW, Qt.p9, Le.Hi, Re.T5, H.FA, J.Is, Yt.t, q.To, nt.N6, G.Ps, j.c, B.ie, tt.Tx, w.XK, Tt.TU, K.Cv, Ut.Cq, St.Fk, w.si, st.LD, it.SJ, Nt.KP, ft.rP, U.ZX, ot.JX, Y.p0, wt.Nh, It.g0, Et.AV, qe.dp, He.U8, Ye.eL, Pe.Cl, T.b2, N.JF, Ae, O.Bz, Je.PW, At.xu, Lt.Ns.forRoot({
                             echarts: () => p.e(275).then(p.bind(p, 36275))
                         }), lt.Co, qt.pL, Ya.SD, kt.R2, Dt.D]
                     }), n
                 })();
             t.B6R(et, function() {
-                return [Z.a8, Z.dk, Z.dn, Z.rt, g.O5, Ia, Ht]
+                return [A.a8, A.dk, A.dn, A.rt, g.O5, Ia, Ht]
             }, []), (0, t.G48)(), T.q6().bootstrapModule(Ua).catch(n => console.error(n)), console.info("Angular CDK version", pt.q.full), console.info("Angular Material version", w.q4.full)
         }
     },
     M => {
         M.O(0, [736], () => M(M.s = 34996)), M.O()
     }
 ]);
```

### Comparing `zen_dash-0.6.8/zen_dash/static/polyfills.0a8881ff36766b1e.js` & `zen_dash-0.6.9/zen_dash/static/polyfills.0a8881ff36766b1e.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/runtime.6a9b461ae5a72237.js` & `zen_dash-0.6.9/zen_dash/static/runtime.6a9b461ae5a72237.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/styles.362a8260c32d36d9.css` & `zen_dash-0.6.9/zen_dash/static/styles.362a8260c32d36d9.css`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/static/vendor.e2924b5928ad7742.js` & `zen_dash-0.6.9/zen_dash/static/vendor.4feeecbf1ad09eca.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -87959,14 +87959,15 @@
                         imports: [b.ez, F.ot, z.U8, A.rt, K.eL, Z.BQ, U.ZD]
                     }), se
                 })()
         },
         88696: (At, mt, V) => {
             "use strict";
             V.d(mt, {
+                H8: () => T,
                 Is: () => k,
                 WI: () => y,
                 ZT: () => w,
                 so: () => v,
                 uw: () => i
             });
             var A = V(95122),
@@ -88313,14 +88314,39 @@
                             dialogResult: ["mat-dialog-close", "dialogResult"],
                             _matDialogClose: ["matDialogClose", "_matDialogClose"]
                         },
                         exportAs: ["matDialogClose"],
                         features: [b.TTD]
                     }), e
                 })(),
+                T = (() => {
+                    class e {
+                        constructor() {
+                            this.align = "start"
+                        }
+                    }
+                    return e.\u0275fac = function(O) {
+                        return new(O || e)
+                    }, e.\u0275dir = b.lG2({
+                        type: e,
+                        selectors: [
+                            ["", "mat-dialog-actions", ""],
+                            ["mat-dialog-actions"],
+                            ["", "matDialogActions", ""]
+                        ],
+                        hostAttrs: [1, "mat-dialog-actions"],
+                        hostVars: 4,
+                        hostBindings: function(O, B) {
+                            2 & O && b.ekj("mat-dialog-actions-align-center", "center" === B.align)("mat-dialog-actions-align-end", "end" === B.align)
+                        },
+                        inputs: {
+                            align: "align"
+                        }
+                    }), e
+                })(),
                 k = (() => {
                     class e {}
                     return e.\u0275fac = function(O) {
                         return new(O || e)
                     }, e.\u0275mod = b.oAB({
                         type: e
                     }), e.\u0275inj = b.cJS({
```

### Comparing `zen_dash-0.6.8/zen_dash/support/__init__.py` & `zen_dash-0.6.9/zen_dash/support/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/tag/__init__.py` & `zen_dash-0.6.9/zen_dash/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/zen_dash/websocket/__init__.py` & `zen_dash-0.6.9/zen_dash/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.6.8/PKG-INFO` & `zen_dash-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-dash
-Version: 0.6.8
+Version: 0.6.9
 Summary: Simple yet scable and production ready python dashboard that is better than shiny application for business.
 Home-page: https://zen-reportz.github.io/zen_dash/index.html
 License: MIT
 Author: Zen
 Author-email: zenreportz@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

