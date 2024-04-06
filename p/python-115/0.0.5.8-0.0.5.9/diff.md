# Comparing `tmp/python_115-0.0.5.8.tar.gz` & `tmp/python_115-0.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.8.tar", max compression
+gzip compressed data, was "python_115-0.0.5.9.tar", max compression
```

## Comparing `python_115-0.0.5.8.tar` & `python_115-0.0.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.8/LICENSE
--rw-r--r--   0        0        0   263926 2024-04-06 09:35:16.733796 python_115-0.0.5.8/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.8/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.8/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.8/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.8/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.8/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.8/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.8/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.8/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.8/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.8/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.8/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.8/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.8/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.8/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.8/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.8/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.8/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.8/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.8/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.8/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-06 09:40:34.864409 python_115-0.0.5.8/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.8/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.9/LICENSE
+-rw-r--r--   0        0        0   263878 2024-04-06 09:57:04.283346 python_115-0.0.5.9/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.9/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.9/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.9/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.9/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.9/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.9/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.9/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.9/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.9/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.9/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.9/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.9/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.9/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.9/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.9/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.9/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.9/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.9/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.9/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.9/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-06 09:59:36.533085 python_115-0.0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.9/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.9/PKG-INFO
```

### Comparing `python_115-0.0.5.8/LICENSE` & `python_115-0.0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/__init__.py` & `python_115-0.0.5.9/p115/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                 t = int(info[k1])
                 info2[k2] = datetime.fromtimestamp(t)
                 if k3:
                     info2[k3] = t
             except ValueError:
                 pass
     if "pc" in info:
-        info2["pick_code"] = info["pc"]
+        info2["pickcode"] = info["pc"]
     if "m" in info:
         info2["star"] = bool(info["m"])
     if "u" in info:
         info2["thumb"] = info["u"]
     if "play_long" in info:
         info2["play_long"] = info["play_long"]
     if keep_raw:
@@ -1771,45 +1771,45 @@
             data={"data": RSA_ENCODER.encode(dumps(payload))}, 
             async_=async_, 
             **request_kwargs, 
         )
 
     def download_url(
         self, 
-        pick_code: str, 
+        pickcode: str, 
         /, 
         detail: bool = False, 
         strict: bool = True, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> str:
         """获取文件的下载链接，此接口是对 `download_url_app` 的封装
         """
         resp = self.download_url_app(
-            {"pickcode": pick_code}, 
+            {"pickcode": pickcode}, 
             async_=async_, 
             **request_kwargs, 
         )
         def get_url(resp: dict) -> str:
             data = check_response(resp)["data"]
             for fid, info in data.items():
                 url = info["url"]
                 if strict and not url:
                     raise IsADirectoryError(errno.EISDIR, f"{fid} is a directory")
                 if not detail:
                     return url["url"] if url else ""
                 return UrlStr(
                     url["url"] if url else "", 
                     id=int(fid), 
-                    pick_code=info["pick_code"], 
+                    pickcode=info["pickcode"], 
                     file_name=info["file_name"], 
                     file_size=int(info["file_size"]), 
                     is_directory=not url,
                 )
-            raise FileNotFoundError(errno.ENOENT, f"no such pick_code: {pick_code!r}")
+            raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}")
         if async_:
             async def wrapper() -> str:
                 return get_url(await resp)  # type: ignore
             return wrapper() # type: ignore
         return get_url(resp)
 
     ########## Upload API ##########
@@ -2812,15 +2812,15 @@
             )
         resp["state"] = True
         resp["data"] = {
             "file_name": filename, 
             "file_size": filesize, 
             "sha1": file_sha1, 
             "cid": pid, 
-            "pick_code": resp["pickcode"], 
+            "pickcode": resp["pickcode"], 
         }
         return resp
 
     async def _upload_file_init_async(
         self, 
         /, 
         filename: str, 
@@ -2870,15 +2870,15 @@
             )
         resp["state"] = True
         resp["data"] = {
             "file_name": filename, 
             "file_size": filesize, 
             "sha1": file_sha1, 
             "cid": pid, 
-            "pick_code": resp["pickcode"], 
+            "pickcode": resp["pickcode"], 
         }
         return resp
 
     def upload_file_init(
         self, 
         /, 
         filename: str, 
@@ -3280,27 +3280,27 @@
         """
         api = "https://webapi.115.com/files/extract_info"
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def extract_list(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
         path: str = "", 
         next_marker: str = "", 
         page_count: int = 999, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """获取压缩文件的文件列表，此方法是对 `extract_info` 的封装，推荐使用
         """
         if not 1 <= page_count <= 999:
             page_count = 999
         payload = {
-            "pick_code": pick_code, 
+            "pick_code": pickcode, 
             "file_name": path.strip("/"), 
             "paths": "文件", 
             "next_marker": next_marker, 
             "page_count": page_count, 
         }
         return self.extract_info(payload, async_=async_, **request_kwargs)
 
@@ -3351,36 +3351,36 @@
         if isinstance(payload, (int, str)):
             payload = {"extract_id": payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def extract_file(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
         paths: str | Sequence[str] = "", 
         dirname: str = "", 
         to_pid: int | str = 0, 
         **request_kwargs, 
     ) -> dict:
         """解压缩到某个文件夹，是对 `extract_add_file` 的封装，推荐使用
         """
         dirname = dirname.strip("/")
         dir2 = f"文件/{dirname}" if dirname else "文件"
         data = [
-            ("pick_code", pick_code), 
+            ("pick_code", pickcode), 
             ("paths", dir2), 
             ("to_pid", to_pid), 
         ]
         if not paths:
-            resp = self.extract_list(pick_code, dirname)
+            resp = self.extract_list(pickcode, dirname)
             if not resp["state"]:
                 return resp
             paths = [p["file_name"] if p["file_category"] else p["file_name"]+"/" for p in resp["data"]["list"]]
             while (next_marker := resp["data"].get("next_marker")):
-                resp = self.extract_list(pick_code, dirname, next_marker)
+                resp = self.extract_list(pickcode, dirname, next_marker)
                 paths.extend(p["file_name"] if p["file_category"] else p["file_name"]+"/" for p in resp["data"]["list"])
         if isinstance(paths, str):
             data.append(("extract_dir[]" if paths.endswith("/") else "extract_file[]", paths.strip("/")))
         else:
             data.extend(("extract_dir[]" if path.endswith("/") else "extract_file[]", path.strip("/")) for path in paths)
         return self.extract_add_file(data, **request_kwargs)
 
@@ -3399,24 +3399,24 @@
         """
         api = "https://webapi.115.com/files/extract_down_file"
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def extract_download_url(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
         path: str, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> str:
         """获取压缩包中文件的下载链接，此接口是对 `extract_download_url_web` 的封装
         """
         resp = self.extract_download_url_web(
             {
-                "pick_code": pick_code, 
+                "pick_code": pickcode, 
                 "full_name": path.strip("/"), 
             }, 
             async_=async_, 
             **request_kwargs, 
         )
         def get_url(resp: dict) -> str:
             data = check_response(resp)["data"]
@@ -3426,40 +3426,40 @@
                 return get_url(await resp) # type: ignore
             return wrapper() # type: ignore
         return get_url(resp)
 
     def extract_push_future(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
         secret: str = "", 
         **request_kwargs, 
     ) -> Optional[PushExtractProgress]:
         """执行在线解压，如果早就已经完成，返回 None，否则新开启一个线程，用于检查进度
         """
         resp = check_response(self.extract_push(
-            {"pick_code": pick_code, "secret": secret}, **request_kwargs
+            {"pick_code": pickcode, "secret": secret}, **request_kwargs
         ))
         if resp["data"]["unzip_status"] == 4:
             return None
-        return PushExtractProgress(self, pick_code)
+        return PushExtractProgress(self, pickcode)
 
     def extract_file_future(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
         paths: str | Sequence[str] = "", 
         dirname: str = "", 
         to_pid: int | str = 0, 
         **request_kwargs, 
     ) -> ExtractProgress:
         """执行在线解压到目录，新开启一个线程，用于检查进度
         """
         resp = check_response(self.extract_file(
-            pick_code, paths, dirname, to_pid, **request_kwargs
+            pickcode, paths, dirname, to_pid, **request_kwargs
         ))
         return ExtractProgress(self, resp["data"]["extract_id"])
 
     ########## Offline Download API ##########
 
     def offline_info(
         self, 
@@ -6037,58 +6037,58 @@
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
     ) -> int:
         return self._files(self.get_id(id_or_path, pid), limit=1)["count"]
 
-    def get_id_from_pickcode(self, /, pick_code: str = "") -> int:
-        if not pick_code:
+    def get_id_from_pickcode(self, /, pickcode: str = "") -> int:
+        if not pickcode:
             return 0
-        data = self.get_info_from_pickcode(pick_code)
+        data = self.get_info_from_pickcode(pickcode)
         for fid in data:
             return int(fid)
-        raise FileNotFoundError(errno.ENOENT, f"no such pick_code: {pick_code!r}") 
+        raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}") 
 
     def get_info_from_pickcode(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
     ) -> dict:
-        return check_response(self.client.download_url_app(pick_code))["data"]
+        return check_response(self.client.download_url_app(pickcode))["data"]
 
     def get_pickcode(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
     ) -> str:
-        return self.attr(id_or_path, pid).get("pick_code", "")
+        return self.attr(id_or_path, pid).get("pickcode", "")
 
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
-        return self.client.download_url(attr["pick_code"], detail=detail, headers=headers)
+        return self.client.download_url(attr["pickcode"], detail=detail, headers=headers)
 
     def get_url_from_pickcode(
         self, 
         /, 
-        pick_code: str, 
+        pickcode: str, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
     ) -> str:
-        return self.client.download_url(pick_code, detail=detail, headers=headers)
+        return self.client.download_url(pickcode, detail=detail, headers=headers)
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
@@ -6951,35 +6951,35 @@
         Thread(target=update_progress).start()
 
 
 class PushExtractProgress(Future):
     _condition: Condition
     _state: str
 
-    def __init__(self, /, client: P115Client, pick_code: str):
+    def __init__(self, /, client: P115Client, pickcode: str):
         super().__init__()
         self.progress = 0
         self.set_running_or_notify_cancel()
-        self._run_check(client, pick_code)
+        self._run_check(client, pickcode)
 
     def __del__(self, /):
         self.stop()
 
     def __bool__(self, /) -> bool:
         return self.progress == 100
 
     def stop(self, /):
         with self._condition:
             if self._state in ["RUNNING", "PENDING"]:
                 self._state = "CANCELLED"
                 self.set_exception(OSError(errno.ECANCELED, "canceled"))
 
-    def _run_check(self, client, pick_code: str, /):
+    def _run_check(self, client, pickcode: str, /):
         check = check_response(client.extract_push_progress)
-        payload = {"pick_code": pick_code}
+        payload = {"pick_code": pickcode}
         def update_progress():
             while self.running():
                 try:
                     data = check(payload)["data"]
                     extract_status = data["extract_status"]
                     progress = extract_status["progress"]
                     if progress == 100:
@@ -7044,15 +7044,15 @@
         Thread(target=update_progress).start()
 
 
 # TODO: 参考 zipfile 模块的接口设计 namelist、filelist 等属性，以及其它的和 zipfile 兼容的接口
 # TODO: 当文件特别多时，可以用 zipfile 等模块来读取文件列表
 class P115ZipFileSystem(P115FileSystemBase[P115ZipPath]):
     file_id: Optional[int]
-    pick_code: str
+    pickcode: str
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, AttrDict]
     attr_cache: MutableMapping[int, tuple[AttrDict]]
     full_loaded: bool
     path_class = P115ZipPath
 
     def __init__(
@@ -7060,26 +7060,26 @@
         /, 
         client: P115Client, 
         id_or_pickcode: int | str, 
     ):
         file_id: Optional[int]
         if isinstance(id_or_pickcode, int):
             file_id = id_or_pickcode
-            pick_code = client.fs.attr(file_id)["pick_code"]
+            pickcode = client.fs.attr(file_id)["pickcode"]
         else:
             file_id = None
-            pick_code = id_or_pickcode
-        resp = check_response(client.extract_push_progress(pick_code))
+            pickcode = id_or_pickcode
+        resp = check_response(client.extract_push_progress(pickcode))
         if resp["data"]["extract_status"]["unzip_status"] != 4:
             raise OSError(errno.EIO, "file was not decompressed")
         self.__dict__.update(
             client=client, 
             cid=0, 
             path="/", 
-            pick_code=pick_code, 
+            pickcode=pickcode, 
             file_id=file_id, 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
             attr_cache={}, 
             full_loaded=False, 
             _nextid=count(1).__next__, 
         )
@@ -7104,15 +7104,15 @@
         self, 
         /, 
         path: str = "", 
         next_marker: str = "", 
     ) -> dict:
         return self.client.extract_list(
             path=path, 
-            pick_code=self.pick_code, 
+            pickcode=self.pickcode, 
         )
 
     @cached_property
     def create_time(self, /) -> datetime:
         if self.file_id is None:
             return datetime.fromtimestamp(0)
         return self.client.fs.attr(self.file_id)["ptime"]
@@ -7205,27 +7205,27 @@
     def extract(
         self, 
         /, 
         paths: str | Sequence[str] = "", 
         dirname: str = "", 
         to_pid: int | str = 0, 
     ) -> ExtractProgress:
-        return self.client.extract_file_future(self.pick_code, paths, dirname, to_pid)
+        return self.client.extract_file_future(self.pickcode, paths, dirname, to_pid)
 
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
-        return self.client.extract_download_url(self.pick_code, attr["path"], headers=headers)
+        return self.client.extract_download_url(self.pickcode, attr["path"], headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> Iterator[AttrDict]:
```

### Comparing `python_115-0.0.5.8/p115/util/_init_mimetypes.py` & `python_115-0.0.5.9/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/cipher.py` & `python_115-0.0.5.9/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/concurrent.py` & `python_115-0.0.5.9/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/download.py` & `python_115-0.0.5.9/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/file.py` & `python_115-0.0.5.9/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/hash.py` & `python_115-0.0.5.9/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/ignore.py` & `python_115-0.0.5.9/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/iter.py` & `python_115-0.0.5.9/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/path.py` & `python_115-0.0.5.9/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/property.py` & `python_115-0.0.5.9/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/response.py` & `python_115-0.0.5.9/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/retry.py` & `python_115-0.0.5.9/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/text.py` & `python_115-0.0.5.9/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/p115/util/urlopen.py` & `python_115-0.0.5.9/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/pyproject.toml` & `python_115-0.0.5.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.8"
+version = "0.0.5.9"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.8/readme.md` & `python_115-0.0.5.9/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.8/PKG-INFO` & `python_115-0.0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.8
+Version: 0.0.5.9
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

