# Comparing `tmp/PandaPosMetrik-2.0.9.tar.gz` & `tmp/PandaPosMetrik-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandaPosMetrik-2.0.9.tar", last modified: Tue Apr  2 14:24:19 2024, max compression
+gzip compressed data, was "PandaPosMetrik-2.1.0.tar", last modified: Sat Apr  6 07:23:47 2024, max compression
```

## Comparing `PandaPosMetrik-2.0.9.tar` & `PandaPosMetrik-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:24:19.879103 PandaPosMetrik-2.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-02 14:24:19.822953 PandaPosMetrik-2.0.9/Metrik/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:31:39.000000 PandaPosMetrik-2.0.9/Metrik/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:24:19.837669 PandaPosMetrik-2.0.9/Metrik/exceptions/
--rw-rw-rw-   0        0        0      358 2024-03-19 12:28:53.000000 PandaPosMetrik-2.0.9/Metrik/exceptions/ObjectDoesNotExists.py
--rw-rw-rw-   0        0        0       69 2024-03-19 12:29:03.000000 PandaPosMetrik-2.0.9/Metrik/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:24:19.857304 PandaPosMetrik-2.0.9/Metrik/models/
--rw-rw-rw-   0        0        0     1546 2024-04-02 13:53:40.000000 PandaPosMetrik-2.0.9/Metrik/models/ORMModel.py
--rw-rw-rw-   0        0        0     3265 2024-04-02 14:00:03.000000 PandaPosMetrik-2.0.9/Metrik/models/OrmManager.py
--rw-rw-rw-   0        0        0     2073 2024-04-02 13:26:51.000000 PandaPosMetrik-2.0.9/Metrik/models/Ticket.py
--rw-rw-rw-   0        0        0        0 2024-02-23 15:16:01.000000 PandaPosMetrik-2.0.9/Metrik/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:24:19.858564 PandaPosMetrik-2.0.9/Metrik/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:17:49.000000 PandaPosMetrik-2.0.9/Metrik/utils/__init__.py
--rw-rw-rw-   0        0        0       61 2024-04-02 14:24:19.878087 PandaPosMetrik-2.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 14:24:19.877183 PandaPosMetrik-2.0.9/PandaPosMetrik.egg-info/
--rw-rw-rw-   0        0        0       61 2024-04-02 14:24:19.000000 PandaPosMetrik-2.0.9/PandaPosMetrik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-04-02 14:24:19.000000 PandaPosMetrik-2.0.9/PandaPosMetrik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:24:19.000000 PandaPosMetrik-2.0.9/PandaPosMetrik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 14:24:19.000000 PandaPosMetrik-2.0.9/PandaPosMetrik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 14:24:19.000000 PandaPosMetrik-2.0.9/PandaPosMetrik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 14:24:19.880087 PandaPosMetrik-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0      221 2024-04-02 14:24:09.000000 PandaPosMetrik-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 07:23:47.637443 PandaPosMetrik-2.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-06 07:23:47.570463 PandaPosMetrik-2.1.0/Metrik/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:31:39.000000 PandaPosMetrik-2.1.0/Metrik/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 07:23:47.576906 PandaPosMetrik-2.1.0/Metrik/exceptions/
+-rw-rw-rw-   0        0        0      358 2024-03-19 12:28:53.000000 PandaPosMetrik-2.1.0/Metrik/exceptions/ObjectDoesNotExists.py
+-rw-rw-rw-   0        0        0       69 2024-03-19 12:29:03.000000 PandaPosMetrik-2.1.0/Metrik/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 07:23:47.599391 PandaPosMetrik-2.1.0/Metrik/models/
+-rw-rw-rw-   0        0        0     1546 2024-04-02 13:53:40.000000 PandaPosMetrik-2.1.0/Metrik/models/ORMModel.py
+-rw-rw-rw-   0        0        0     4101 2024-04-06 07:19:26.000000 PandaPosMetrik-2.1.0/Metrik/models/OrmManager.py
+-rw-rw-rw-   0        0        0     2073 2024-04-02 13:26:51.000000 PandaPosMetrik-2.1.0/Metrik/models/Ticket.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:16:01.000000 PandaPosMetrik-2.1.0/Metrik/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 07:23:47.605054 PandaPosMetrik-2.1.0/Metrik/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:17:49.000000 PandaPosMetrik-2.1.0/Metrik/utils/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-04-06 07:23:47.625930 PandaPosMetrik-2.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 07:23:47.625930 PandaPosMetrik-2.1.0/PandaPosMetrik.egg-info/
+-rw-rw-rw-   0        0        0       61 2024-04-06 07:23:46.000000 PandaPosMetrik-2.1.0/PandaPosMetrik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-06 07:23:47.000000 PandaPosMetrik-2.1.0/PandaPosMetrik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 07:23:46.000000 PandaPosMetrik-2.1.0/PandaPosMetrik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 07:23:47.000000 PandaPosMetrik-2.1.0/PandaPosMetrik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 07:23:47.000000 PandaPosMetrik-2.1.0/PandaPosMetrik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 07:23:47.638608 PandaPosMetrik-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      221 2024-04-06 07:19:48.000000 PandaPosMetrik-2.1.0/setup.py
```

### Comparing `PandaPosMetrik-2.0.9/Metrik/models/ORMModel.py` & `PandaPosMetrik-2.1.0/Metrik/models/ORMModel.py`

 * *Files identical despite different names*

### Comparing `PandaPosMetrik-2.0.9/Metrik/models/OrmManager.py` & `PandaPosMetrik-2.1.0/Metrik/models/OrmManager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 from typing import Generic, TypeVar
+from attr import dataclass
 import pyodbc
 
 from Metrik.exceptions import ObjectDoesNotExists
 settings = __import__("settings")
 
 T = TypeVar('T', bound='OrmManager')
+
+
+
+class WhereFilters:
+    __gt: str = "{field} > {value}"
+    __lt: str = "{field} < {value}"
+    __eq: str = "{field} = {value}"
+    __ne: str = "!="
+    __date: str = "CONVERT(DATE, {field}) = '{value}'"
+
+
+
+
+
+
 class OrmManager(Generic[T]):
     
     _connection = None
     def _get_or_create_connection(self) -> pyodbc.Connection:
         if self._connection is None:
             self._connection = pyodbc.connect(
                 driver=settings.DB_DRIVER,
@@ -47,15 +63,26 @@
         cursor.execute(sql)
         columns = [column[0] for column in cursor.description]
         rows = [self.owner(**dict(zip(columns, row))) for row in cursor.fetchall()] #cursor.fetchall()
         return rows
     
     
     def where_clause_generate(self, **kwargs):
-        where_clause = 'WHERE ' + ' AND '.join([k +' = ' + str(v) for k, v in kwargs.items()])
+        queries = []
+        for key, value in kwargs.items():
+            field, *lookups = key.split('__')
+            if not lookups: lookups = ['eq']
+            
+            for lookup in lookups:
+                where_clause = WhereFilters[f"__{lookup}"]
+                where_clause = where_clause.format(field=field, value=value)
+                queries.append(where_clause)
+            
+        #where_clause = 'WHERE ' + ' AND '.join([k +' = ' + str(v) for k, v in kwargs.items()])
+        return 'WHERE ' + ' AND '.join(queries)
         return where_clause
     
     
     def filter(self, **kwargs) -> list[T]:
         cursor = self.connection.cursor()
         sql = f"""
         SELECT * FROM {self.owner.__tablename_plural__} {self.where_clause_generate(**kwargs)}"""
@@ -74,14 +101,21 @@
             UPDATE {self.owner.__tablename_plural__} SET {', '.join([k +' = ?' for k in kwargs.keys()])}"""
         cursor.execute(sql, list(kwargs.values()))
         cursor.commit()
         return self.owner(**kwargs)
     
     def get(self, **kwargs) -> T:
         
+        where_filter = {}
+        
+        for key, value in kwargs.items():
+            
+        
+        
+        
         results = self.filter(**kwargs)
         if len(results) == 0:
             raise ObjectDoesNotExists(self.owner, **kwargs)
 
         return results[0]
     
     def delete(self, **kwargs):
```

### Comparing `PandaPosMetrik-2.0.9/Metrik/models/Ticket.py` & `PandaPosMetrik-2.1.0/Metrik/models/Ticket.py`

 * *Files identical despite different names*

