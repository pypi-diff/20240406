# Comparing `tmp/asktable-0.13.6-py3-none-any.whl.zip` & `tmp/asktable-0.13.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 29098 bytes, number of entries: 32
+Zip file size: 29493 bytes, number of entries: 32
 -rw-r--r--  2.0 unx       86 b- defN 24-Apr-02 15:29 asktable/__init__.py
 -rw-r--r--  2.0 unx     2180 b- defN 24-Apr-01 06:16 asktable/api.py
 -rw-r--r--  2.0 unx     1667 b- defN 24-Apr-01 06:16 asktable/cli.py
 -rw-r--r--  2.0 unx      887 b- defN 24-Apr-05 04:16 asktable/client.py
 -rw-r--r--  2.0 unx       41 b- defN 24-Apr-01 06:16 asktable/exceptions.py
 -rw-r--r--  2.0 unx      875 b- defN 24-Apr-01 06:44 asktable/log.py
 -rw-r--r--  2.0 unx     1492 b- defN 24-Apr-01 06:16 asktable/upload.py
 -rw-r--r--  2.0 unx      152 b- defN 24-Apr-01 06:16 asktable/models/__init__.py
 -rw-r--r--  2.0 unx     2588 b- defN 24-Apr-01 06:16 asktable/models/base.py
 -rw-r--r--  2.0 unx     2769 b- defN 24-Apr-01 06:16 asktable/models/chat.py
--rw-r--r--  2.0 unx    10178 b- defN 24-Apr-05 03:12 asktable/models/datasource.py
+-rw-r--r--  2.0 unx    10180 b- defN 24-Apr-06 02:14 asktable/models/datasource.py
 -rw-r--r--  2.0 unx     1264 b- defN 24-Apr-01 06:16 asktable/models/message.py
 -rw-r--r--  2.0 unx      878 b- defN 24-Apr-01 06:16 asktable/models/run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-08 14:27 atcommon/__init__.py
 -rw-r--r--  2.0 unx     3296 b- defN 24-Apr-04 03:57 atcommon/tools.py
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-05 04:31 atcommon/version.py
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-06 07:15 atcommon/version.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-31 13:33 atcommon/exceptions/__init__.py
 -rw-r--r--  2.0 unx     1282 b- defN 24-Apr-02 15:21 atcommon/exceptions/client.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-01 06:16 atcommon/exceptions/server.py
 -rw-r--r--  2.0 unx     2089 b- defN 24-Apr-02 14:43 atcommon/exceptions/server_base.py
 -rw-r--r--  2.0 unx      589 b- defN 24-Apr-01 06:16 atcommon/exceptions/server_plugins.py
 -rw-r--r--  2.0 unx      466 b- defN 24-Apr-01 06:16 atcommon/models/__init__.py
 -rw-r--r--  2.0 unx      731 b- defN 24-Jan-20 03:26 atcommon/models/base.py
 -rw-r--r--  2.0 unx     2344 b- defN 24-Apr-01 06:16 atcommon/models/bi.py
 -rw-r--r--  2.0 unx     1069 b- defN 24-Apr-01 06:16 atcommon/models/chat.py
 -rw-r--r--  2.0 unx     1424 b- defN 24-Apr-03 14:46 atcommon/models/datasource.py
--rw-r--r--  2.0 unx    25728 b- defN 24-Apr-04 14:45 atcommon/models/meta.py
--rw-r--r--  2.0 unx     9875 b- defN 24-Apr-05 04:31 asktable-0.13.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 04:31 asktable-0.13.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-Apr-05 04:31 asktable-0.13.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-05 04:31 asktable-0.13.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2558 b- defN 24-Apr-05 04:31 asktable-0.13.6.dist-info/RECORD
-32 files, 76776 bytes uncompressed, 25018 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx    27794 b- defN 24-Apr-06 01:31 atcommon/models/meta.py
+-rw-r--r--  2.0 unx     9875 b- defN 24-Apr-06 07:56 asktable-0.13.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 07:56 asktable-0.13.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-06 07:56 asktable-0.13.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-06 07:56 asktable-0.13.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2558 b- defN 24-Apr-06 07:56 asktable-0.13.7.dist-info/RECORD
+32 files, 78844 bytes uncompressed, 25413 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -75,23 +75,23 @@
 
 Filename: atcommon/models/datasource.py
 Comment: 
 
 Filename: atcommon/models/meta.py
 Comment: 
 
-Filename: asktable-0.13.6.dist-info/METADATA
+Filename: asktable-0.13.7.dist-info/METADATA
 Comment: 
 
-Filename: asktable-0.13.6.dist-info/WHEEL
+Filename: asktable-0.13.7.dist-info/WHEEL
 Comment: 
 
-Filename: asktable-0.13.6.dist-info/entry_points.txt
+Filename: asktable-0.13.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: asktable-0.13.6.dist-info/top_level.txt
+Filename: asktable-0.13.7.dist-info/top_level.txt
 Comment: 
 
-Filename: asktable-0.13.6.dist-info/RECORD
+Filename: asktable-0.13.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asktable/models/datasource.py

```diff
@@ -25,34 +25,34 @@
         self.update_from_dict(new_meta_dict)
         return self
 
     def delete(self):
         self.api.send(endpoint=f"/datasources/{self.datasource_id}/meta", method="DELETE")
         return True
 
-    def update_async(self):
+    def update(self):
         self.api.send(endpoint=f"/datasources/{self.datasource_id}/meta", method="POST")
         return True
 
-    def update(self, timeout=600):
+    def update_wait_success(self, timeout=600):
         """
         同步元数据并轮询其状态，直到超时、成功或失败。
 
         参数:
             timeout (int): 超时时间，单位为秒。默认值为 600 秒。
 
         返回:
             MetaDataClientModel: 更新后的元数据实例。
 
         异常:
             DataSourceMetaProcessError: 如果元数据更新失败。
             DataSourceMetaProcessTimeout: 如果元数据更新超时。
         """
         # 发起同步请求
-        self.update_async()
+        self.update()
 
         start_time = time.time()
 
         # 初始化斐波那契数列间隔
         fib_a, fib_b = 1, 1
 
         while True:
@@ -184,25 +184,25 @@
 
         if not id:
             raise ValueError("No ID or Name provided")
         # 通过资源ID来获取
         return self.api.send(endpoint=f"{self.endpoint}/{id}", method="GET")
 
     @convert_to_object(cls=DataSourceClientModel)
-    def register_async(self, type, access_config, name=None):
+    def register(self, type, access_config, name=None):
         data = {
             "type": type, "name": name,
             "access_config": access_config
         }
         return self.api.send(endpoint=self.endpoint, method="POST",
                              data=data)
 
-    def register(self, type, access_config, name=None, timeout=180):
+    def register_wait_success(self, type, access_config, name=None, timeout=180):
         # 注册数据源并获取其ID
-        ds = self.register_async(type, access_config, name)
+        ds = self.register(type, access_config, name)
         start_time = time.time()
 
         # 初始化斐波那契数列间隔
         fib_a, fib_b = 1, 1
 
         while True:
             # 获取数据源的最新状态
```

## atcommon/version.py

```diff
@@ -1 +1 @@
-VERSION="0.13.6"
+VERSION="0.13.7"
```

## atcommon/models/meta.py

```diff
@@ -242,19 +242,19 @@
     def add_schema(self, schema: DataSchema):
         self.schemas.append(schema)
         self.schemas_dict[schema.name] = schema
 
     def get_schema(self, schema_name):
         return self.schemas_dict.get(schema_name)
 
-    def filter_for_analysis(self) -> "MetaData":
+    def filter_for_process(self) -> "MetaData":
         """
         返回一个新的 MetaData 对象，其中只包含需要分析的字段。
         """
-        return self.load_from_analysed_simple_dict(self.to_simple_dict_for_analysis())
+        return self.load_from_processed_simple_dict(self.to_simple_dict_for_process())
 
     @classmethod
     def load_from_dict(cls, data: dict):
         """
         Load metadata from a dictionary structure.
         The expected format is:
         {
@@ -473,15 +473,15 @@
     #         'schemas': [schema.to_dict_for_analysis() for schema
     #                     in self.schemas if schema.to_dict_for_analysis()]
     #     }
     #
     # def to_markdown_for_analysis(self):
     #     return dict_to_markdown(self.to_dict_for_analysis(), table_format_keys=('fields',))
 
-    def to_simple_dict_for_analysis(self) -> dict:
+    def to_simple_dict_for_process(self) -> dict:
         schemas = []
         for s in self.schemas:
             tables = []
             for t in s.tables:
                 if t.curr_desc and all([f.curr_desc for f in t.fields]):
                     continue
                 fields = []
@@ -501,15 +501,15 @@
         return {
             'name': self.name,
             'datasource_id': self.datasource_id,
             'schemas': schemas,
         }
 
     @classmethod
-    def load_from_analysed_simple_dict(cls, data: dict) -> "MetaData":
+    def load_from_processed_simple_dict(cls, data: dict) -> "MetaData":
         """
         data =
         {
             "name": [name],
             "datasource_id": [datasource_id],
             "schemas": [
                 {
@@ -657,7 +657,49 @@
 
                 # 现在可以安全地添加 cloned_table 到新 schema 中
                 cloned_schema.add_table(cloned_table)
 
                 table_count += 1
 
         return chunks
+
+    def filter_tables_by_names(self, table_full_names: List[str]) -> "MetaData":
+        """
+        Filter tables by their full names and create a new MetaData instance containing only these tables.
+
+        :param table_full_names: A list of full names of tables to be included in the new MetaData instance.
+        :return: A new MetaData instance with the specified tables.
+        """
+        # 创建一个新的 MetaData 实例
+        filtered_metadata = MetaData(name=f"{self.name}_filtered", datasource_id=self.datasource_id)
+
+        for full_name in table_full_names:
+            schema_name, table_name = full_name.rsplit('.', 1)
+
+            # 查找匹配的 schema 和 table
+            schema = self.get_schema(schema_name)
+            if schema:
+                table = schema.get_table(table_name)
+                if table:
+                    # 如果找到匹配的 table，则复制到新的 MetaData 实例中
+                    # 首先确保 schema 存在于新的 MetaData 实例中
+                    filtered_schema = filtered_metadata.get_schema(schema_name)
+                    if not filtered_schema:
+                        # 如果不存在，则复制 schema 到新的 MetaData 实例中
+                        filtered_schema = DataSchema(
+                            name=schema.name,
+                            metadata=filtered_metadata,
+                            origin_desc=schema.origin_desc,
+                            curr_desc=schema.curr_desc,
+                            curr_desc_stat=schema.curr_desc_stat,
+                            custom_configs=schema.custom_configs
+                        )
+                        filtered_metadata.add_schema(filtered_schema)
+
+                    # 然后复制 table 到新的 schema 中
+                    cloned_table = deepcopy(table)
+                    # 更新 cloned_table 的 schema 属性为新的 schema
+                    cloned_table.schema = filtered_schema
+                    filtered_schema.add_table(cloned_table)
+
+        return filtered_metadata
+
```

## Comparing `asktable-0.13.6.dist-info/METADATA` & `asktable-0.13.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asktable
-Version: 0.13.6
+Version: 0.13.7
 Summary: AskTable SDK
 Home-page: https://asktable.com/
 Author: lele
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: pybase62
```

## Comparing `asktable-0.13.6.dist-info/RECORD` & `asktable-0.13.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 asktable/client.py,sha256=D50bWrMySDdJdsLs-AxD1oHCeEpRn_4R2_x_XHaMWS8,887
 asktable/exceptions.py,sha256=HUys_aPowtoLqjO4XhANXBQCUUpty1zLxV4fWPqBkLc,41
 asktable/log.py,sha256=CIRsQtXMB24sD5fFsUn2hxlEVJB33Ej8TIQKyET2pQ8,875
 asktable/upload.py,sha256=ZctBvZtKnBZWucRXzvdp25zBNGz3eQ6PAfdhzLzfMUU,1492
 asktable/models/__init__.py,sha256=LDrDHxIjYwQN-fLW4BKMkuogEUcDfLxMYtlEkq0Xzfk,152
 asktable/models/base.py,sha256=vDe19yuK6SJglgRlz8Gq9qKg_x1Cxs2tK82VKeJ3UCI,2588
 asktable/models/chat.py,sha256=Z-2p_crBI5HwljcIxtRNV46_FfsVmNc5oRrwq3dNigE,2769
-asktable/models/datasource.py,sha256=jIs4S3hcIESsbthwLqkvb3vPABnb0VgdyxQ4p7SMhPY,10178
+asktable/models/datasource.py,sha256=S4Js9u9iV3PlfWTaYyTIxPrFJYgrpY5c3cOPFimhN5A,10180
 asktable/models/message.py,sha256=4bIt5VTBXvH5iQYb5_LoOIIbbNEkjmUsLfkjx4Il7-M,1264
 asktable/models/run.py,sha256=xf4oNReawEmQk0rmYn-uWPu_zkZD7ws1-77bOfUWYTw,878
 atcommon/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atcommon/tools.py,sha256=TWlukRR8iaDY0FW4zM1hXO-2xM9NPcDB9PA4eYHipDI,3296
-atcommon/version.py,sha256=csXdmQRoJaLLMv4De_BYgUYYOu15o-wdPUt_seOcfOI,16
+atcommon/version.py,sha256=GceneUTRRAdKaqJxWYOIA20h2wpMEccJSg897QOFntA,16
 atcommon/exceptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atcommon/exceptions/client.py,sha256=qHJfByYYiVOwdAs_L-R655tBmep6Kpg1ixvktBNQNA0,1282
 atcommon/exceptions/server.py,sha256=BSlYmdfDasoAq6oK9fyGhws3EBPII_hkHpx_JQmMdAY,95
 atcommon/exceptions/server_base.py,sha256=-X7xH1cmypIwl007CvuN2MIGqCv89sYb5jVi7s-Uzkc,2089
 atcommon/exceptions/server_plugins.py,sha256=MqQgXsGHUn0JB3EAos1vlf8SLjUMNGXAY7lcBKSA_8c,589
 atcommon/models/__init__.py,sha256=QDsebmmUAHCKrMs789lDMt9HU9DR0kH-TGnE1CtW9kU,466
 atcommon/models/base.py,sha256=UVM9dKL22-k4k44H6DYQeNIe35vJ1Vg0ppGDZiVDiIU,731
 atcommon/models/bi.py,sha256=77HEtXOEj2tJwXe34s5Shsu4LWDihxAols8Rcz5cOFU,2344
 atcommon/models/chat.py,sha256=Si_eo8H8h_NtIOc76qhXoYcHp_tPMavud2sEnUXEejo,1069
 atcommon/models/datasource.py,sha256=Qv-IIC9hDGXrWe5s__4U_f51QNDi9BCMJrf42cUJ5Tg,1424
-atcommon/models/meta.py,sha256=U5ZQxjlHbo62343nE_RCDz23OrN5vSL-YTOW_HdzuzQ,25728
-asktable-0.13.6.dist-info/METADATA,sha256=ZnIf8Mub7ZhNqyS0HfstYnDaToRJEJHgbas7xQB_D9g,9875
-asktable-0.13.6.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-asktable-0.13.6.dist-info/entry_points.txt,sha256=OS7zXFo5f2wYttNLFf6EScGBaN_2XtYbV_Fl_C3RhY8,47
-asktable-0.13.6.dist-info/top_level.txt,sha256=j_dz8lioIJZMGAy7UUdXv0ytGGhh8HFsGhSXaULxT4M,18
-asktable-0.13.6.dist-info/RECORD,,
+atcommon/models/meta.py,sha256=OZesut61aJuotvzhj6k92tvcvaOut6E5v5rNNpFzVGo,27794
+asktable-0.13.7.dist-info/METADATA,sha256=duqv4vYPwNkJ9NOVKVJAbNez9_91riSmdIfGAdyIatA,9875
+asktable-0.13.7.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+asktable-0.13.7.dist-info/entry_points.txt,sha256=OS7zXFo5f2wYttNLFf6EScGBaN_2XtYbV_Fl_C3RhY8,47
+asktable-0.13.7.dist-info/top_level.txt,sha256=j_dz8lioIJZMGAy7UUdXv0ytGGhh8HFsGhSXaULxT4M,18
+asktable-0.13.7.dist-info/RECORD,,
```

