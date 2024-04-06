# Comparing `tmp/dfelf-0.1.8-py3-none-any.whl.zip` & `tmp/dfelf-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7364123 bytes, number of entries: 15
+Zip file size: 7364226 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      146 b- defN 22-Jul-17 06:06 dfelf/__init__.py
--rw-r--r--  2.0 unx     3699 b- defN 22-Jul-17 06:07 dfelf/commons.py
--rw-r--r--  2.0 unx    25472 b- defN 22-Jul-27 01:23 dfelf/cvsfileelf.py
+-rw-r--r--  2.0 unx     3802 b- defN 22-Jul-28 06:37 dfelf/commons.py
+-rw-r--r--  2.0 unx    25802 b- defN 22-Jul-28 08:51 dfelf/cvsfileelf.py
 -rw-r--r--  2.0 unx     2698 b- defN 22-Feb-12 04:03 dfelf/datafileelf.py
 -rw-r--r--  2.0 unx    28106 b- defN 22-Jul-17 06:07 dfelf/imagefileelf.py
 -rw-r--r--  2.0 unx    20469 b- defN 22-Jul-27 07:50 dfelf/pdffileelf.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-10 00:52 dfelf/res/__init__.py
 -rw-rw-r--  2.0 unx  8482020 b- defN 18-Oct-22 07:42 dfelf/res/Noto_Sans_SC/NotoSansSC-Regular.otf
 -rw-r--r--  2.0 unx     4444 b- defN 18-Oct-22 07:42 dfelf/res/Noto_Sans_SC/OFL.txt
 -rw-r--r--  2.0 unx        0 b- defN 22-Mar-10 00:52 dfelf/res/Noto_Sans_SC/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 22-Jul-27 07:56 dfelf-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    14324 b- defN 22-Jul-27 07:56 dfelf-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-27 07:56 dfelf-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 22-Jul-27 07:56 dfelf-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1187 b- defN 22-Jul-27 07:56 dfelf-0.1.8.dist-info/RECORD
-15 files, 8583727 bytes uncompressed, 7362179 bytes compressed:  14.2%
+-rw-r--r--  2.0 unx     1064 b- defN 22-Jul-28 09:24 dfelf-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14324 b- defN 22-Jul-28 09:24 dfelf-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jul-28 09:24 dfelf-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 22-Jul-28 09:24 dfelf-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1187 b- defN 22-Jul-28 09:24 dfelf-0.1.9.dist-info/RECORD
+15 files, 8584160 bytes uncompressed, 7362282 bytes compressed:  14.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: dfelf/res/Noto_Sans_SC/OFL.txt
 Comment: 
 
 Filename: dfelf/res/Noto_Sans_SC/__init__.py
 Comment: 
 
-Filename: dfelf-0.1.8.dist-info/LICENSE
+Filename: dfelf-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: dfelf-0.1.8.dist-info/METADATA
+Filename: dfelf-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: dfelf-0.1.8.dist-info/WHEEL
+Filename: dfelf-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: dfelf-0.1.8.dist-info/top_level.txt
+Filename: dfelf-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dfelf-0.1.8.dist-info/RECORD
+Filename: dfelf-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dfelf/commons.py

```diff
@@ -15,14 +15,15 @@
 ERROR_DEF = {
     '0': '[{0}] 图像相似度不符合要求（{3}），MSE为{1}，SSIM为{2}。',
     '1': '[{0}] read_image中的参数"image_file"类型错误，应为Image.Image或者str。',
     '1000': '[{0}] "{1}"没有设置正确（不能直接使用默认设置值），请设置后重试。',
     '2000': '[{0}] 存在需要进行去重处理的值，详细请查阅文件：{1}\n{2}',
     '2001': '[{0}] 如下重复值将被去除，详细请查阅文件：{1}\n{2}',
     '2002': '[{0}] "split"中的"key"不存在，请检查数据文件"{1}"是否存在该字段"{2}"。',
+    '2003': '[{0}] "drop_duplicates"中的"subset"参数({1})类型({2})错误，应为str或list。',
     '3000': '[{0}] "splice"中没有正确设置"input"参数，请设置后重试。',
     '3001': '[{0}] 图片中未能解析到二维码。',
     '3002': '[{0}] 解码成功，内容为：\n{1}',
     '3003': '[{0}] 文件"{1}"转换为base64成功。',
     '3004': '[{0}] 坐标数据{1}异常，无法进行裁剪处理。',
     '3005': '[{0}] 坐标数据{1}异常，无法进行马赛克处理。',
     '3006': '[{0}] most_used_color方法中的参数"img"类型错误，应为Image.Image或者numpy.ndarray。',
```

## dfelf/cvsfileelf.py

```diff
@@ -303,25 +303,31 @@
             else:
                 output_filename = self.get_log_path(self._config[task_key]['output']['name'])
             bom = self._config[task_key]['output']['BOM']
             nn = self._config[task_key]['output']['non-numeric']
             CSVFileElf.to_csv(kwargs['df'], output_filename, bom, nn)
 
     def drop_duplicates(self, df, subset):
-        mask = pd.Series(df.duplicated(subset=subset))
+        if isinstance(subset, str):
+            subset_value = [subset]
+        elif isinstance(subset, list):
+            subset_value = subset.copy()
+        else:
+            raise TypeError(logger.error([2003, subset, type(subset)]))
+        mask = pd.Series(df.duplicated(subset=subset_value))
         log_filename = 'drop_duplicates' + moment().format('.YYYYMMDD.HHmmss') + '.log'
         filename = self.get_log_path(log_filename)
         log_filename_pre = 'pre_' + log_filename
         pre_filename = self.get_log_path(log_filename_pre)
         duplicates = df[mask]
         else_mask = ~ mask
         if not duplicates.empty:
             CSVFileElf.to_csv_with_bom(duplicates, filename)
-            tmp_df = df[df[subset].isin(duplicates[subset])]
-            logger.warning([2000, log_filename_pre, tmp_df.sort_values(by=[subset])])
+            tmp_df = df[df[subset_value].isin(duplicates[subset_value])]
+            logger.warning([2000, log_filename_pre, tmp_df.sort_values(by=subset_value)])
             CSVFileElf.to_csv_with_bom(tmp_df, pre_filename)
             logger.warning([2001, log_filename, duplicates])
         return df[else_mask], log_filename
 
     @staticmethod
     def tidy(df, nn):
         df_export = df.copy()
@@ -596,15 +602,16 @@
             all_cols.remove(col)
         all_cols = on_cols + all_cols
         df_res = pd.DataFrame([], columns=all_cols)
         df_on, log_file = self.drop_duplicates(df_on, on_cols)
         df_on.reset_index(drop=True, inplace=True)
         df_res[on_cols] = df_on[on_cols]
         for df in df_ori:
-            index = df_on[df_on.set_index(on_cols).index.isin(df.set_index(on_cols).index)].index
-            df.set_index(index, inplace=True)
-            df_res[df_res.isnull()] = df
+            df_adj = self.drop_duplicates(df, on_cols)[0]
+            index = df_on[df_on.set_index(on_cols).index.isin(df_adj.set_index(on_cols).index)].index
+            df_adj.set_index(index, inplace=True)
+            df_res[df_res.isnull()] = df_adj
         if silent:
             pass
         else:
             self.to_output(task_key, df=df_res)
         return df_res
```

## Comparing `dfelf-0.1.8.dist-info/LICENSE` & `dfelf-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dfelf-0.1.8.dist-info/METADATA` & `dfelf-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfelf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data File Elf
 Home-page: https://github.com/KrixTam/dfelf
 Author: Krix Tam
 Author-email: krix.tam@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/KrixTam/dfelf/issues
 Platform: UNKNOWN
```

## Comparing `dfelf-0.1.8.dist-info/RECORD` & `dfelf-0.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 dfelf/__init__.py,sha256=O7r5peO9ujBZZVfa3exQX3-mU6f8V2ME6KEtsfexAN4,146
-dfelf/commons.py,sha256=ArP3YYbiWKDx3Cq5V7Onrgdk3U42pjK0Y_LzaHt1A9I,3699
-dfelf/cvsfileelf.py,sha256=ZoFQVaJY-HI98fCb2920aupzShzk4VO9gn-tHVFTOAU,25472
+dfelf/commons.py,sha256=4wHE6ED77l9gydDBPq1gol7sbz7-bLJ2YCXyf6nuyiM,3802
+dfelf/cvsfileelf.py,sha256=AJ-aCtalZcgoLllccEYaoM3j4-9JGICOivvv_fUU8BU,25802
 dfelf/datafileelf.py,sha256=VrxbCGATgKvZxiddkRUYkhy99e9zJJ9A35Tpb5MSRtg,2698
 dfelf/imagefileelf.py,sha256=T_V4xeK27_V5TuH_yxbDWpMqUeX5HONwFtb6Ndy1pHs,28106
 dfelf/pdffileelf.py,sha256=cMuIdYflW0nVPBp8mGNuCUasDByrl0jeQ3MenrQop-U,20469
 dfelf/res/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dfelf/res/Noto_Sans_SC/NotoSansSC-Regular.otf,sha256=ork-bC2wXWu79vJ9QT7HMmlzW3tnkBnIpaqWcP8P-_I,8482020
 dfelf/res/Noto_Sans_SC/OFL.txt,sha256=hXyc_pnamxyzEyNIhdCQn002VFQQu25ta5RDQNEzHZE,4444
 dfelf/res/Noto_Sans_SC/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dfelf-0.1.8.dist-info/LICENSE,sha256=h1e8DPh-OUUfenwpKq4Bh-0XzzCQPuI-4iVaenYLRiU,1064
-dfelf-0.1.8.dist-info/METADATA,sha256=HLhtMW7KoCuS14PtiNyiX43Dj3L1UNG9R9mg3G4m26I,14324
-dfelf-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dfelf-0.1.8.dist-info/top_level.txt,sha256=pkth8GNfn__jecrSEkrFYbzPFwyEOSw-ZPHKDlt4iJ4,6
-dfelf-0.1.8.dist-info/RECORD,,
+dfelf-0.1.9.dist-info/LICENSE,sha256=h1e8DPh-OUUfenwpKq4Bh-0XzzCQPuI-4iVaenYLRiU,1064
+dfelf-0.1.9.dist-info/METADATA,sha256=jtVfWqkRbz-QG9AmjCSGel29x3SoqvB-zQAVMVtSLE4,14324
+dfelf-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dfelf-0.1.9.dist-info/top_level.txt,sha256=pkth8GNfn__jecrSEkrFYbzPFwyEOSw-ZPHKDlt4iJ4,6
+dfelf-0.1.9.dist-info/RECORD,,
```

