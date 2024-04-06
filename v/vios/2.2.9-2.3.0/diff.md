# Comparing `tmp/vios-2.2.9-py3-none-any.whl.zip` & `tmp/vios-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 46668 bytes, number of entries: 25
+Zip file size: 46683 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat     2858 b- defN 24-Mar-19 11:19 quark/__main__.py
--rw-rw-rw-  2.0 fat    18911 b- defN 24-Apr-05 13:39 quark/proxy.py
+-rw-rw-rw-  2.0 fat    18952 b- defN 24-Apr-06 02:13 quark/proxy.py
 -rw-rw-rw-  2.0 fat    18861 b- defN 24-Mar-21 10:46 quark/app/__init__.py
 -rw-rw-rw-  2.0 fat     2575 b- defN 24-Mar-19 11:19 quark/app/_data.py
 -rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 11:19 quark/app/demo.py
 -rw-rw-rw-  2.0 fat     9043 b- defN 24-Mar-19 11:19 quark/app/task.py
 -rw-rw-rw-  2.0 fat     5876 b- defN 24-Mar-19 11:19 quark/app/uapi.py
 -rw-rw-rw-  2.0 fat     7914 b- defN 24-Mar-19 11:19 quark/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat      386 b- defN 24-Mar-19 11:19 quark/driver/__init__.py
@@ -13,15 +13,15 @@
 -rw-rw-rw-  2.0 fat     4663 b- defN 24-Mar-19 11:19 quark/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5432 b- defN 24-Mar-19 11:19 quark/driver/common/visadriver.py
 -rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-19 11:19 quark/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    15111 b- defN 24-Mar-19 11:19 quark/envelope/assembler.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 24-Mar-19 11:19 quark/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-19 11:19 quark/envelope/device.py
 -rw-rw-rw-  2.0 fat     3758 b- defN 24-Mar-23 03:45 quark/envelope/processor.py
--rw-rw-rw-  2.0 fat     4224 b- defN 24-Apr-04 12:39 quark/envelope/router.py
+-rw-rw-rw-  2.0 fat     4258 b- defN 24-Apr-06 02:13 quark/envelope/router.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 24-Mar-21 12:16 quark/envelope/systemq.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-05 13:42 vios-2.2.9.dist-info/RECORD
-25 files, 128358 bytes uncompressed, 43492 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-06 02:27 vios-2.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-06 02:27 vios-2.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-06 02:27 vios-2.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-06 02:27 vios-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-06 02:27 vios-2.3.0.dist-info/RECORD
+25 files, 128433 bytes uncompressed, 43507 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: quark/envelope/router.py
 Comment: 
 
 Filename: quark/envelope/systemq.py
 Comment: 
 
-Filename: vios-2.2.9.dist-info/LICENSE
+Filename: vios-2.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: vios-2.2.9.dist-info/METADATA
+Filename: vios-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: vios-2.2.9.dist-info/WHEEL
+Filename: vios-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: vios-2.2.9.dist-info/top_level.txt
+Filename: vios-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-2.2.9.dist-info/RECORD
+Filename: vios-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quark/proxy.py

```diff
@@ -482,15 +482,15 @@
         try:
             result = get_data_by_tid(tid, 'count')
             return result if raw else self.process(result)
         except Exception as e:
             return f'No data found for {tid}!'
 
     @classmethod
-    def process(cls, result: dict, circuit: bool = False):
+    def process(cls, result: dict, dropout: bool = False):
         def _delete_dict(ret: dict, num: int = 0):
             while num > 0:
                 tmp = np.cumsum(list(ret.values()))
                 ran_num = np.random.randint(tmp[-1]+1)
                 ran_pos = np.searchsorted(tmp, ran_num)
                 ret[list(ret.keys())[ran_pos]] -= 1
                 if ret[list(ret.keys())[ran_pos]] == 0:
@@ -515,17 +515,18 @@
                 for kv in dat:
                     if kv[-1] < 0:
                         continue
                     base = tuple(kv[:-1]-1)  # from 1&2 to 0&1
                     dres[base] = dres.get(base, 0)+kv[-1]
 
             try:
-                shots = meta['other']['shots'] * \
-                    len(meta['axis']['repeat']['repeat'])
-                _delete_dict(dres, shots - (shots//1000)*1000)
+                if dropout:
+                    shots = meta['other']['shots'] * \
+                        len(meta['axis']['repeat']['repeat'])
+                    _delete_dict(dres, shots - (shots//1000)*1000)
             except Exception as e:
                 logger.error(f'Failed to dropout: {e}')
 
             try:
                 # if meta['coqis']['correct']:
                 from home.ylfeng.cloud import correct_readout
                 cdres = correct_readout(dres, meta['other']['measure'])
```

## quark/envelope/router.py

```diff
@@ -83,18 +83,18 @@
         ``` 
     """
 
     # print(result.keys(),result['meta'].keys())
 
     quafu = result['meta'].get('coqis', {})
     # savefig(result)
-    if not quafu.get('token', ''):
+    if not quafu.get('token', '') or not quafu.get('eid', ''):
         return
 
-    res = QuarkProxy.process(result)
+    res = QuarkProxy.process(result, True)
 
     rshot = 0
     post_data = {"task_id": quafu['eid'],
                  "status": res['status'],
                  "raw": "",
                  "res": "",
                  'transpiled_circuit': res['transpiled'],
```

## Comparing `vios-2.2.9.dist-info/LICENSE` & `vios-2.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-2.2.9.dist-info/METADATA` & `vios-2.3.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 2.2.9
+Version: 2.3.0
 Summary: runtime requirements for systemq
 Author-email: YL Feng <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-2.2.9.dist-info/RECORD` & `vios-2.3.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 quark/__main__.py,sha256=ky318p_RHmGRdMyzIL2meu-JOgqzRrH-hWfFvhceZGE,2858
-quark/proxy.py,sha256=dQfdU1SoQ5sJR1zVpTmTeoPDSOGeJNbCSUvTJPIT_Ko,18911
+quark/proxy.py,sha256=bHvoQZ1BRFAgZbxbA5Oy1R-oH4vT3Nn359S7j3DAzKg,18952
 quark/app/__init__.py,sha256=MjOh4mkjvwFzEEfPNv-dMOcoktAtYCBtl-P5_UA7MzQ,18861
 quark/app/_data.py,sha256=EGGTD2FrZ8vlbMh4jlmWhYk4fEG3FolGoWaQ26qxoss,2575
 quark/app/demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
 quark/app/task.py,sha256=QEZuNia59sLEWa8pl2XIjItx2NismSTPZFnFt8-90HM,9043
 quark/app/uapi.py,sha256=itjEa89SUXozZqBGLH-3o4mKtRssNQODDj60knC-cGE,5876
 quark/driver/VirtualDevice.py,sha256=Cswl_ykFhIsocGV6Okh_YS1b48FeLm2fh1ruXqmNoyw,7914
 quark/driver/__init__.py,sha256=p1pVx1xTulBT8-qdp_zJ859tdIsA92XdvwrkqcVHL4s,386
@@ -12,14 +12,14 @@
 quark/driver/common/quantity.py,sha256=fV9DMmjys44efe7TTvzXmFdozqGdS2QUm23wtfLxeBE,4663
 quark/driver/common/visadriver.py,sha256=LRyYDBF0u9EYf6p47LeGGKhx9pHiq4pux_pzDakaICY,5432
 quark/envelope/__init__.py,sha256=5_cs0tZ7mV4GjOsY2isx8sUQu4u6Y3WN-9DUGG27SQM,1188
 quark/envelope/assembler.py,sha256=ENwX7FutJvpg6_Wcm42_Zx-ddq40JozuYqHPwJp09ZA,15111
 quark/envelope/calculator.py,sha256=0rZAA46sWh_X8wOBmpBvmljqCV53ID4VHPX1cE_abEc,4322
 quark/envelope/device.py,sha256=5E3oWZ84IYnQdzlmzltgPyayYz_au7p7UIbFVpJUa0Q,1106
 quark/envelope/processor.py,sha256=uMIwu83a4SDZVM3OE5_WrBya_4jxtdcXPd6pYa0osrk,3758
-quark/envelope/router.py,sha256=wVx-rWnCZg_BrPV8fja4kjI5jiQ5vEoAyXsCtDpdBdA,4224
+quark/envelope/router.py,sha256=-Qxhd4qmMsJU_Ik7YDdERmmesegB4-19y9S-JoyE1HM,4258
 quark/envelope/systemq.py,sha256=QAaHLv68C9UjMp9qHt9t-HJkOTpCkbHZTlNVOsAzIBc,2841
-vios-2.2.9.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
-vios-2.2.9.dist-info/METADATA,sha256=zQS7ExtZ485hD9MsYFdRMMcqHhwm_R0zzY2pIh8_bYk,1211
-vios-2.2.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-vios-2.2.9.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
-vios-2.2.9.dist-info/RECORD,,
+vios-2.3.0.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
+vios-2.3.0.dist-info/METADATA,sha256=RjgcCKQftPzzTWbdjaqg-cVFuTruBdHqqAeo8LqvOBI,1211
+vios-2.3.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+vios-2.3.0.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
+vios-2.3.0.dist-info/RECORD,,
```

