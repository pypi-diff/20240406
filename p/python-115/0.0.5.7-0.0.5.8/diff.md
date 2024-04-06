# Comparing `tmp/python_115-0.0.5.7.tar.gz` & `tmp/python_115-0.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.7.tar", max compression
+gzip compressed data, was "python_115-0.0.5.8.tar", max compression
```

## Comparing `python_115-0.0.5.7.tar` & `python_115-0.0.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.7/LICENSE
--rw-r--r--   0        0        0   261107 2024-04-05 06:47:37.395609 python_115-0.0.5.7/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.7/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.7/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.7/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.7/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.7/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.7/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.7/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.7/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.7/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.7/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.7/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.7/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.7/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.7/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.7/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.7/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.7/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.7/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.7/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.7/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-05 06:48:24.210543 python_115-0.0.5.7/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.7/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.8/LICENSE
+-rw-r--r--   0        0        0   263926 2024-04-06 09:35:16.733796 python_115-0.0.5.8/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.8/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.8/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.8/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.8/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.8/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.8/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.8/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.8/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.8/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.8/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.8/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.8/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.8/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.8/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.8/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.8/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.8/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.8/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.8/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.8/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-06 09:40:34.864409 python_115-0.0.5.8/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.8/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.8/PKG-INFO
```

### Comparing `python_115-0.0.5.7/LICENSE` & `python_115-0.0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/__init__.py` & `python_115-0.0.5.8/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,20 +105,22 @@
         return fn
     elif iscoroutinefunction(fn):
         async def wrapper(*args, **kwds):
             resp = await fn(*args, **kwds)
             if not resp.get("state", True):
                 raise OSError(errno.EIO, resp)
             return resp
-    else:
+    elif callable(fn):
         def wrapper(*args, **kwds):
             resp = fn(*args, **kwds)
             if not resp.get("state", True):
                 raise OSError(errno.EIO, resp)
             return resp
+    else:
+        raise TypeError
     return update_wrapper(wrapper, fn)
 
 
 def console_qrcode(text: str) -> None:
     qr = qrcode.QRCode(border=1)
     qr.add_data(text)
     qr.print_ascii(tty=True)
@@ -171,14 +173,38 @@
     if keep_raw:
         info2["raw"] = info
     if extra_data:
         info2.update(extra_data)
     return info2
 
 
+class UrlStr(str):
+
+    def __new__(cls, url="", /, *args, **kwds):
+        return super().__new__(cls, url)
+
+    def __init__(self, url="", /, *args, **kwds):
+        self.__dict__.update(*args, **kwds)
+
+    def __delattr__(self, attr, /) -> Never:
+        raise TypeError("can't delete attributes")
+
+    def __getitem__(self, key, /):
+        return self.__dict__[key]
+
+    def __setattr__(self, attr, val, /) -> Never:
+        raise TypeError("can't set attributes")
+
+    def __repr__(self, /) -> str:
+        return f"{type(self).__qualname__}({str(self)!r}, {self.__dict__})"
+
+    def geturl(self) -> str:
+        return str(self)
+
+
 class P115Client:
     cookie: str
     session: Session
     user_id: int
     user_key: str
 
     def __init__(self, /, cookie=None, login_app: str = "web"):
@@ -199,15 +225,15 @@
     def __eq__(self, other, /) -> bool:
         return type(self) is type(other) and self.user_id == other.user_id
 
     def __hash__(self, /) -> int:
         return hash((self.user_id, self.cookie))
 
     def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attribute")
+        raise TypeError("can't set attributes")
 
     @cached_property
     def async_session(self, /) -> ClientSession:
         session = ClientSession(raise_for_status=True)
         session.headers.update(self.session.headers) # type: ignore
         cookiejar = session.cookie_jar
         cookiejar.clear()
@@ -1658,35 +1684,45 @@
         data = RSA_ENCODER.encode(dumps(payload))
         return self.request(api, "POST", data={"data": data}, async_=async_, **request_kwargs)
 
     def share_download_url(
         self, 
         payload: dict, 
         /, 
+        detail: bool = False, 
+        strict: bool = True, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> str:
         """获取分享链接中某个文件的下载链接，此接口是对 `share_download_url_app` 的封装
         POST https://proapi.115.com/app/share/downurl
         payload:
             - file_id: int | str
             - receive_code: str
             - share_code: str
             - user_id: int | str = <default>
         """
         resp = self.share_download_url_app(payload, async_=async_, **request_kwargs)
         def get_url(resp: dict) -> str:
-            data = check_response(resp)["data"]
+            info = check_response(resp)["data"]
             file_id = payload.get("file_id")
-            if not data:
+            if not info:
                 raise FileNotFoundError(errno.ENOENT, f"no such id: {file_id!r}")
-            url = data["url"]
-            if not url:
-                raise IsADirectoryError(errno.EISDIR, f"this id refers to a directory: {file_id!r}")
-            return url["url"]
+            url = info["url"]
+            if strict and not url:
+                raise IsADirectoryError(errno.EISDIR, f"{file_id} is a directory")
+            if not detail:
+                return url["url"] if url else ""
+            return UrlStr(
+                url["url"] if url else "", 
+                id=int(info["fid"]), 
+                file_name=info["fn"], 
+                file_size=int(info["fs"]), 
+                is_directory=not url, 
+            )
         if async_:
             async def wrapper() -> str:
                 return get_url(await resp) # type: ignore
             return wrapper() # type: ignore
         return get_url(resp)
 
     ########## Download API ##########
@@ -1737,23 +1773,43 @@
             **request_kwargs, 
         )
 
     def download_url(
         self, 
         pick_code: str, 
         /, 
+        detail: bool = False, 
+        strict: bool = True, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> str:
         """获取文件的下载链接，此接口是对 `download_url_app` 的封装
         """
-        resp = self.download_url_app({"pickcode": pick_code}, async_=async_, **request_kwargs)
+        resp = self.download_url_app(
+            {"pickcode": pick_code}, 
+            async_=async_, 
+            **request_kwargs, 
+        )
         def get_url(resp: dict) -> str:
             data = check_response(resp)["data"]
-            return next(iter(data.values()))["url"]["url"]
+            for fid, info in data.items():
+                url = info["url"]
+                if strict and not url:
+                    raise IsADirectoryError(errno.EISDIR, f"{fid} is a directory")
+                if not detail:
+                    return url["url"] if url else ""
+                return UrlStr(
+                    url["url"] if url else "", 
+                    id=int(fid), 
+                    pick_code=info["pick_code"], 
+                    file_name=info["file_name"], 
+                    file_size=int(info["file_size"]), 
+                    is_directory=not url,
+                )
+            raise FileNotFoundError(errno.ENOENT, f"no such pick_code: {pick_code!r}")
         if async_:
             async def wrapper() -> str:
                 return get_url(await resp)  # type: ignore
             return wrapper() # type: ignore
         return get_url(resp)
 
     ########## Upload API ##########
@@ -3351,15 +3407,18 @@
         path: str, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> str:
         """获取压缩包中文件的下载链接，此接口是对 `extract_download_url_web` 的封装
         """
         resp = self.extract_download_url_web(
-            {"pick_code": pick_code, "full_name": path.strip("/")}, 
+            {
+                "pick_code": pick_code, 
+                "full_name": path.strip("/"), 
+            }, 
             async_=async_, 
             **request_kwargs, 
         )
         def get_url(resp: dict) -> str:
             data = check_response(resp)["data"]
             return quote(data["url"], safe=":/?&=%#")
         if async_:
@@ -3998,15 +4057,15 @@
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
             name = module + "." + name
         return f"{name}({self.__dict__})"
 
     def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attribute")
+        raise TypeError("can't set attributes")
 
     def __str__(self, /) -> str:
         return self.path
 
     def __truediv__(self, path: str | PathLike[str], /) -> Self:
         return self.joinpath(path)
 
@@ -5337,15 +5396,15 @@
     def __delitem__(self, id_or_path: IDOrPathType, /):
         self.rmtree(id_or_path)
 
     def __len__(self, /) -> int:
         return self.get_directory_capacity(self.cid)
 
     def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attribute")
+        raise TypeError("can't set attributes")
 
     def __setitem__(
         self, 
         id_or_path: IDOrPathType, 
         file: None | str | bytes | bytearray | memoryview | PathLike = None, 
         /, 
     ):
@@ -5978,25 +6037,58 @@
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
     ) -> int:
         return self._files(self.get_id(id_or_path, pid), limit=1)["count"]
 
+    def get_id_from_pickcode(self, /, pick_code: str = "") -> int:
+        if not pick_code:
+            return 0
+        data = self.get_info_from_pickcode(pick_code)
+        for fid in data:
+            return int(fid)
+        raise FileNotFoundError(errno.ENOENT, f"no such pick_code: {pick_code!r}") 
+
+    def get_info_from_pickcode(
+        self, 
+        /, 
+        pick_code: str, 
+    ) -> dict:
+        return check_response(self.client.download_url_app(pick_code))["data"]
+
+    def get_pickcode(
+        self, 
+        id_or_path: IDOrPathType, 
+        /, 
+        pid: Optional[int] = None, 
+    ) -> str:
+        return self.attr(id_or_path, pid).get("pick_code", "")
+
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
+        detail: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
-        return self.client.download_url(attr["pick_code"], headers=headers)
+        return self.client.download_url(attr["pick_code"], detail=detail, headers=headers)
+
+    def get_url_from_pickcode(
+        self, 
+        /, 
+        pick_code: str, 
+        headers: Optional[Mapping] = None, 
+        detail: bool = False, 
+    ) -> str:
+        return self.client.download_url(pick_code, detail=detail, headers=headers)
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
@@ -6563,15 +6655,15 @@
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
             name = module + "." + name
         return f"<{name}(client={self.client!r}, share_link={self.share_link!r}, cid={self.cid!r}, path={self.path!r}) at {hex(id(self))}>"
 
     def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attribute")
+        raise TypeError("can't set attributes")
 
     @classmethod
     def login(
         cls, 
         /, 
         share_link: str, 
         cookie = None, 
@@ -6991,15 +7083,15 @@
             full_loaded=False, 
             _nextid=count(1).__next__, 
         )
         if file_id is None:
             self.__dict__["create_time"] = datetime.fromtimestamp(0)
 
     def __setattr__(self, attr, val, /) -> Never:
-        raise TypeError("can't set attribute")
+        raise TypeError("can't set attributes")
 
     @classmethod
     def login(
         cls, 
         /, 
         id_or_pickcode: int | str, 
         cookie = None,
```

### Comparing `python_115-0.0.5.7/p115/util/_init_mimetypes.py` & `python_115-0.0.5.8/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/cipher.py` & `python_115-0.0.5.8/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/concurrent.py` & `python_115-0.0.5.8/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/download.py` & `python_115-0.0.5.8/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/file.py` & `python_115-0.0.5.8/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/hash.py` & `python_115-0.0.5.8/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/ignore.py` & `python_115-0.0.5.8/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/iter.py` & `python_115-0.0.5.8/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/path.py` & `python_115-0.0.5.8/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/property.py` & `python_115-0.0.5.8/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/response.py` & `python_115-0.0.5.8/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/retry.py` & `python_115-0.0.5.8/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/text.py` & `python_115-0.0.5.8/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/p115/util/urlopen.py` & `python_115-0.0.5.8/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/pyproject.toml` & `python_115-0.0.5.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.7"
+version = "0.0.5.8"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.7/readme.md` & `python_115-0.0.5.8/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.7/PKG-INFO` & `python_115-0.0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.7
+Version: 0.0.5.8
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

