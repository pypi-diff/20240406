# Comparing `tmp/ProcruSQL-0.0.8.tar.gz` & `tmp/ProcruSQL-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcruSQL-0.0.8.tar", last modified: Thu Sep  8 10:15:16 2022, max compression
+gzip compressed data, was "ProcruSQL-0.0.9.tar", last modified: Mon Sep 19 12:40:28 2022, max compression
```

## Comparing `ProcruSQL-0.0.8.tar` & `ProcruSQL-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-08 10:15:16.718673 ProcruSQL-0.0.8/
--rw-------   0 hjp       (1000) hjp       (1000)     1073 2022-02-26 10:52:22.000000 ProcruSQL-0.0.8/LICENSE
--rw-r--r--   0 hjp       (1000) hjp       (1000)      621 2022-09-08 10:15:16.718673 ProcruSQL-0.0.8/PKG-INFO
--rw-------   0 hjp       (1000) hjp       (1000)      122 2022-02-26 10:52:22.000000 ProcruSQL-0.0.8/README.md
--rw-------   0 hjp       (1000) hjp       (1000)      104 2022-02-26 10:52:22.000000 ProcruSQL-0.0.8/pyproject.toml
--rw-r--r--   0 hjp       (1000) hjp       (1000)      699 2022-09-08 10:15:16.722673 ProcruSQL-0.0.8/setup.cfg
-drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-08 10:15:16.718673 ProcruSQL-0.0.8/src/
-drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-08 10:15:16.718673 ProcruSQL-0.0.8/src/ProcruSQL.egg-info/
--rw-r--r--   0 hjp       (1000) hjp       (1000)      621 2022-09-08 10:15:16.000000 ProcruSQL-0.0.8/src/ProcruSQL.egg-info/PKG-INFO
--rw-r--r--   0 hjp       (1000) hjp       (1000)      280 2022-09-08 10:15:16.000000 ProcruSQL-0.0.8/src/ProcruSQL.egg-info/SOURCES.txt
--rw-r--r--   0 hjp       (1000) hjp       (1000)        1 2022-09-08 10:15:16.000000 ProcruSQL-0.0.8/src/ProcruSQL.egg-info/dependency_links.txt
--rw-r--r--   0 hjp       (1000) hjp       (1000)       49 2022-09-08 10:15:16.000000 ProcruSQL-0.0.8/src/ProcruSQL.egg-info/entry_points.txt
--rw-r--r--   0 hjp       (1000) hjp       (1000)       10 2022-09-08 10:15:16.000000 ProcruSQL-0.0.8/src/ProcruSQL.egg-info/top_level.txt
-drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-08 10:15:16.718673 ProcruSQL-0.0.8/src/procrusql/
--rw-r--r--   0 hjp       (1000) hjp       (1000)    12870 2022-08-02 12:51:15.000000 ProcruSQL-0.0.8/src/procrusql/__init__.py
--rwxr-xr-x   0 hjp       (1000) hjp       (1000)    11304 2022-09-08 10:07:24.000000 ProcruSQL-0.0.8/src/procrusql/parser.py
+drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-19 12:40:28.628857 ProcruSQL-0.0.9/
+-rw-------   0 hjp       (1000) hjp       (1000)     1073 2022-02-26 10:52:22.000000 ProcruSQL-0.0.9/LICENSE
+-rw-r--r--   0 hjp       (1000) hjp       (1000)      621 2022-09-19 12:40:28.628857 ProcruSQL-0.0.9/PKG-INFO
+-rw-------   0 hjp       (1000) hjp       (1000)      122 2022-02-26 10:52:22.000000 ProcruSQL-0.0.9/README.md
+-rw-------   0 hjp       (1000) hjp       (1000)      104 2022-02-26 10:52:22.000000 ProcruSQL-0.0.9/pyproject.toml
+-rw-r--r--   0 hjp       (1000) hjp       (1000)      699 2022-09-19 12:40:28.628857 ProcruSQL-0.0.9/setup.cfg
+drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-19 12:40:28.628857 ProcruSQL-0.0.9/src/
+drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-19 12:40:28.628857 ProcruSQL-0.0.9/src/ProcruSQL.egg-info/
+-rw-r--r--   0 hjp       (1000) hjp       (1000)      621 2022-09-19 12:40:28.000000 ProcruSQL-0.0.9/src/ProcruSQL.egg-info/PKG-INFO
+-rw-r--r--   0 hjp       (1000) hjp       (1000)      280 2022-09-19 12:40:28.000000 ProcruSQL-0.0.9/src/ProcruSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 hjp       (1000) hjp       (1000)        1 2022-09-19 12:40:28.000000 ProcruSQL-0.0.9/src/ProcruSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 hjp       (1000) hjp       (1000)       49 2022-09-19 12:40:28.000000 ProcruSQL-0.0.9/src/ProcruSQL.egg-info/entry_points.txt
+-rw-r--r--   0 hjp       (1000) hjp       (1000)       10 2022-09-19 12:40:28.000000 ProcruSQL-0.0.9/src/ProcruSQL.egg-info/top_level.txt
+drwxr-xr-x   0 hjp       (1000) hjp       (1000)        0 2022-09-19 12:40:28.628857 ProcruSQL-0.0.9/src/procrusql/
+-rw-r--r--   0 hjp       (1000) hjp       (1000)    13613 2022-09-19 12:36:07.000000 ProcruSQL-0.0.9/src/procrusql/__init__.py
+-rwxr-xr-x   0 hjp       (1000) hjp       (1000)    11418 2022-09-19 11:43:24.000000 ProcruSQL-0.0.9/src/procrusql/parser.py
```

### Comparing `ProcruSQL-0.0.8/LICENSE` & `ProcruSQL-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ProcruSQL-0.0.8/PKG-INFO` & `ProcruSQL-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcruSQL
-Version: 0.0.8
+Version: 0.0.9
 Summary: Make a database fit its description
 Home-page: https://git.hjp.at:3000/hjp/procrusql
 Author: Peter J. Holzer
 Author-email: hjp@hjp.at
 Project-URL: Bug Tracker, https://git.hjp.at:3000/hjp/procrusql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProcruSQL-0.0.8/setup.cfg` & `ProcruSQL-0.0.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ProcruSQL
-version = 0.0.8
+version = 0.0.9
 author = Peter J. Holzer
 author_email = hjp@hjp.at
 description = Make a database fit its description
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://git.hjp.at:3000/hjp/procrusql
 project_urls =
```

### Comparing `ProcruSQL-0.0.8/src/ProcruSQL.egg-info/PKG-INFO` & `ProcruSQL-0.0.9/src/ProcruSQL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcruSQL
-Version: 0.0.8
+Version: 0.0.9
 Summary: Make a database fit its description
 Home-page: https://git.hjp.at:3000/hjp/procrusql
 Author: Peter J. Holzer
 Author-email: hjp@hjp.at
 Project-URL: Bug Tracker, https://git.hjp.at:3000/hjp/procrusql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProcruSQL-0.0.8/src/procrusql/__init__.py` & `ProcruSQL-0.0.9/src/procrusql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,29 +208,40 @@
                 """
                 select * from information_schema.columns
                 where table_schema = %s and table_name = %s and column_name = %s
                 """,
                 (self.schema, self.table, self.column, ))
         r = csr.fetchall()
         if len(r) == 1:
-            # Column exists, all ok
+            # Column exists, check attributes
+            if (r[0]["is_nullable"] == "YES") != self.definition["nullable"]:
+                log_action.info("Changing column %s of %s.%s to %s",
+                                self.column, self.schema, self.table,
+                                "null" if self.definition["nullable"] else "not null")
+                q = sql.SQL("alter table {schema}.{table} alter {column} {action} not null").format(
+                        schema=sql.Identifier(self.schema),
+                        table=sql.Identifier(self.table),
+                        column=sql.Identifier(self.column),
+                        action=sql.SQL("drop" if self.definition["nullable"] else "set")
+                    )
+                csr.execute(q)
             self.set_order()
             self.ok = True
             log_state.info("%s is now ok", self.name)
             return
         if len(r) > 1:
             raise RuntimeError(f"Found {len(r)} columns with nam {self.columnr} in {self.schema}.{self.table}")
 
         # Create column
         log_action.info("Adding column %s to table %s.%s", self.column, self.schema, self.table)
         q = sql.SQL("alter table {schema}.{table} add {column} {definition}").format(
                 schema=sql.Identifier(self.schema),
                 table=sql.Identifier(self.table),
                 column=sql.Identifier(self.column),
-                definition=sql.SQL(self.definition),
+                definition=sql.SQL(self.definition["text"]),
             )
         csr.execute(q)
         self.set_order()
         self.ok = True
         log_state.info("%s is now ok", self.name)
 
 class HaveUniqueConstraint(Node):
```

### Comparing `ProcruSQL-0.0.8/src/procrusql/parser.py` & `ProcruSQL-0.0.9/src/procrusql/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,17 @@
         "date", "timestamp with time zone", "timestamptz"
     )
     pattern = "(" + "|".join(sqltypes) + ")" + r"([ \t]+(default .*|not null\b|primary key\b|unique\b|references \w+\b))*"
     m = ps2.match(pattern)
     if not m:
         ps.record_child_failure(ps2, "expected column definition")
         return
-    ps2.ast.append(m.group(0))
+    text = m.group(0)
+    nullable = not("not null" in text or "primary key" in text)
+    ps2.ast.append({ "text": text, "nullable": nullable })
     return ps2
 
 def parse_dict(ps):
     ps2 = ps.clone()
     d = {}
     ps2.skip_whitespace_and_comments()
     if not ps2.match(r"{"):
```

