# Comparing `tmp/zipline.py-0.8.1.tar.gz` & `tmp/zipline.py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline.py-0.8.1.tar", last modified: Fri Jul 28 08:54:07 2023, max compression
+gzip compressed data, was "zipline.py-0.9.0.tar", last modified: Tue Sep 12 23:39:43 2023, max compression
```

## Comparing `zipline.py-0.8.1.tar` & `zipline.py-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:54:07.367167 zipline.py-0.8.1/
--rw-r--r--   0 rdrescher   (501) staff       (20)     1046 2023-03-27 21:55:25.000000 zipline.py-0.8.1/LICENSE
--rw-r--r--   0 rdrescher   (501) staff       (20)     2007 2023-07-28 08:54:07.367038 zipline.py-0.8.1/PKG-INFO
--rw-r--r--   0 rdrescher   (501) staff       (20)      319 2023-03-29 21:28:07.000000 zipline.py-0.8.1/README.md
--rw-r--r--   0 rdrescher   (501) staff       (20)      879 2023-07-28 08:53:44.000000 zipline.py-0.8.1/pyproject.toml
--rw-r--r--   0 rdrescher   (501) staff       (20)       38 2023-07-28 08:54:07.367205 zipline.py-0.8.1/setup.cfg
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:54:07.366285 zipline.py-0.8.1/zipline/
--rw-r--r--   0 rdrescher   (501) staff       (20)     1274 2023-07-28 08:53:39.000000 zipline.py-0.8.1/zipline/__init__.py
--rw-r--r--   0 rdrescher   (501) staff       (20)    22979 2023-07-28 08:51:33.000000 zipline.py-0.8.1/zipline/client.py
--rw-r--r--   0 rdrescher   (501) staff       (20)     1261 2023-07-18 18:11:05.000000 zipline.py-0.8.1/zipline/enums.py
--rw-r--r--   0 rdrescher   (501) staff       (20)     1851 2023-07-18 18:48:18.000000 zipline.py-0.8.1/zipline/errors.py
--rw-r--r--   0 rdrescher   (501) staff       (20)    15314 2023-07-18 18:11:05.000000 zipline.py-0.8.1/zipline/models.py
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:54:07.366856 zipline.py-0.8.1/zipline.py.egg-info/
--rw-r--r--   0 rdrescher   (501) staff       (20)     2007 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/PKG-INFO
--rw-r--r--   0 rdrescher   (501) staff       (20)      292 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/SOURCES.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)        1 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/dependency_links.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)       55 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/requires.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)        8 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/top_level.txt
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-09-12 23:39:43.417152 zipline.py-0.9.0/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1046 2023-03-27 21:55:25.000000 zipline.py-0.9.0/LICENSE
+-rw-r--r--   0 rdrescher   (501) staff       (20)     2163 2023-09-12 23:39:43.416870 zipline.py-0.9.0/PKG-INFO
+-rw-r--r--   0 rdrescher   (501) staff       (20)      319 2023-03-29 21:28:07.000000 zipline.py-0.9.0/README.md
+-rw-r--r--   0 rdrescher   (501) staff       (20)      879 2023-09-12 23:10:16.000000 zipline.py-0.9.0/pyproject.toml
+-rw-r--r--   0 rdrescher   (501) staff       (20)       38 2023-09-12 23:39:43.417192 zipline.py-0.9.0/setup.cfg
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-09-12 23:39:43.415736 zipline.py-0.9.0/zipline/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1274 2023-09-12 23:10:26.000000 zipline.py-0.9.0/zipline/__init__.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)    23212 2023-09-12 23:32:56.000000 zipline.py-0.9.0/zipline/client.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1259 2023-09-12 23:34:47.000000 zipline.py-0.9.0/zipline/enums.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1861 2023-09-12 23:35:56.000000 zipline.py-0.9.0/zipline/errors.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)    15422 2023-09-12 23:34:36.000000 zipline.py-0.9.0/zipline/models.py
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-09-12 23:39:43.416413 zipline.py-0.9.0/zipline.py.egg-info/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     2163 2023-09-12 23:39:43.000000 zipline.py-0.9.0/zipline.py.egg-info/PKG-INFO
+-rw-r--r--   0 rdrescher   (501) staff       (20)      292 2023-09-12 23:39:43.000000 zipline.py-0.9.0/zipline.py.egg-info/SOURCES.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)        1 2023-09-12 23:39:43.000000 zipline.py-0.9.0/zipline.py.egg-info/dependency_links.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)       55 2023-09-12 23:39:43.000000 zipline.py-0.9.0/zipline.py.egg-info/requires.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)        8 2023-09-12 23:39:43.000000 zipline.py-0.9.0/zipline.py.egg-info/top_level.txt
```

### Comparing `zipline.py-0.8.1/LICENSE` & `zipline.py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zipline.py-0.8.1/PKG-INFO` & `zipline.py-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline.py
-Version: 0.8.1
+Version: 0.9.0
 Summary: An async wrapper for the Zipline api.
 Author-email: fretgfr <fretgfr@sudomail.com>
 License: Copyright 2023 fretgfr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -25,16 +25,20 @@
 Project-URL: Homepage, https://github.com/fretgfr/zipline.py/
 Keywords: zipline,api wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: aiohttp<4,>=3.7.4
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: typing_extensions; extra == "dev"
 
 
 # Quickstart
 
 ```py
 import asyncio
```

### Comparing `zipline.py-0.8.1/pyproject.toml` & `zipline.py-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zipline.py"
-version = "0.8.1"
+version = "0.9.0"
 description = "An async wrapper for the Zipline api."
 readme = "README.md"
 authors = [{ name = "fretgfr", email = "fretgfr@sudomail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zipline.py-0.8.1/zipline/__init__.py` & `zipline.py-0.9.0/zipline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from .errors import *
 from .models import *
 
 __title__ = "zipline.py"
 __author__ = "fretgfr"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 fretgfr"
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

### Comparing `zipline.py-0.8.1/zipline/client.py` & `zipline.py-0.9.0/zipline/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         token : str
             Your Zipline token.
         """
         self.server_url = server_url
         self._session = aiohttp.ClientSession(base_url=server_url, headers={"Authorization": token})
 
     async def create_user(self, *, username: str, password: str, administrator: bool = False) -> User:
-        """Creates a User.
+        """|coro|
+
+        Creates a User.
 
         Parameters
         ----------
         username : str
             The username of the user to create.
         password : str
             The password of the user to create.
@@ -94,15 +96,17 @@
                 raise BadRequest(f"400: {msg}")
             elif status == 403:
                 raise Forbidden("You cannot access this resource.")
 
         raise UnhandledError(f"{status} not handled in create_user!")
 
     async def get_password_protected_image(self, *, id: int, password: str) -> bytes:
-        """Retrieves the content of a password protected File.
+        """|coro|
+
+        Retrieves the content of a password protected File.
 
         Parameters
         ----------
         id : int
             The id of the File to get.
         password : str
             The password of the File to get.
@@ -131,15 +135,17 @@
                 raise BadRequest(f"400: {msg}")
             elif status == 404:
                 raise NotFound("404: Requested file not found.")
 
         raise UnhandledError(f"Code {status} raised in get_password_protected_image not handled!")
 
     async def get_all_invites(self) -> List[Invite]:
-        """Retrieves all Invites.
+        """|coro|
+
+        Retrieves all Invites.
 
         Returns
         -------
         List[Invite]
             The invites on the server.
 
         Raises
@@ -158,15 +164,17 @@
                 raise BadRequest("Invites are disabled on this server")
             elif status == 403:
                 raise Forbidden("You cannot access this resource.")
 
         raise UnhandledError(f"Code {status} unhandled in get_all_invites!")
 
     async def create_invites(self, *, count: int = 1, expires_at: Optional[datetime] = None) -> List[PartialInvite]:
-        """Creates user invites.
+        """|coro|
+
+        Creates user invites.
 
         Parameters
         ----------
         count : int, optional
             The number of invites to create, by default 1
         expires_at : Optional[datetime], optional
             When the created invite(s) should expire, by default None
@@ -207,15 +215,17 @@
                 raise BadRequest(f"400: {msg}")
             elif status == 403:
                 raise Forbidden("You cannot access this resource.")
 
         raise UnhandledError(f"Code {status} unhandled in create_invites!")
 
     async def delete_invite(self, code: str, /) -> Invite:
-        """Deletes an Invite with given code.
+        """|coro|
+
+        Deletes an Invite with given code.
 
         Parameters
         ----------
         code : str
             The code of the Invite to delete.
 
         Returns
@@ -240,15 +250,17 @@
                 raise Forbidden("You cannot access this resource.")
             elif status == 404:
                 raise NotFound(f"Could not find invite with code '{code}'")
 
         raise UnhandledError(f"Code {status} unhandled in delete_invite!")
 
     async def get_all_folders(self, *, with_files: bool = False) -> List[Folder]:
-        """Returns all Folders
+        """|coro|
+
+        Returns all Folders
 
         Parameters
         ----------
         with_files : bool, optional
             Whether the retrieved Folder should contain File information, by default False
 
         Returns
@@ -264,15 +276,17 @@
             if status == 200:
                 js = await resp.json()
                 return [Folder._from_data(data, session=self._session) for data in js]
 
         raise UnhandledError(f"Code {status} unhandled in get_all_folders!")
 
     async def create_folder(self, name: str, /, *, files: Optional[List[File]] = None) -> Folder:
-        """Creates a Folder.
+        """|coro|
+
+        Creates a Folder.
 
         Parameters
         ----------
         name : str
             The name of the folder to create.
         files : Optional[List[File]], optional
             Files that should be added to the created folder, by default None
@@ -297,15 +311,17 @@
                 msgjson = await resp.json()
                 msg = msgjson["error"]
                 raise BadRequest(f"400: {msg}")
 
         raise UnhandledError(f"Code {status} unhandled in create_folder!")
 
     async def get_folder(self, id: int, /, *, with_files: bool = False) -> Folder:
-        """Gets a folder with a given id.
+        """|coro|
+
+        Gets a folder with a given id.
 
         Parameters
         ----------
         id : int
             The id of the folder to get.
         with_files : bool, optional
             Whether File information should be retrieved, by default False
@@ -334,15 +350,17 @@
                 raise Forbidden("You do not have access to that folder.")
             elif status == 404:
                 raise NotFound(f"Folder with id {id} not found.")
 
         raise UnhandledError(f"Code {status} unhandled in create_folder!")
 
     async def get_user(self, id: int, /) -> User:
-        """Returns a User with the given id.
+        """|coro|
+
+        Returns a User with the given id.
 
         Parameters
         ----------
         id : int
             The id of the User to get.
 
         Returns
@@ -368,15 +386,17 @@
                 raise NotFound(f"Could not find a user with id {id}")
 
         raise UnhandledError(f"Code {status} unhandled in get_user!")
 
     # TODO methods for /api/user/export
 
     async def get_all_files(self) -> List[File]:
-        """Gets all Files belonging to your user.
+        """|coro|
+
+        Gets all Files belonging to your user.
 
         Returns
         -------
         List[File]
             The returned Files
         """
         async with self._session.get("/api/user/files") as resp:
@@ -385,15 +405,17 @@
                 js = await resp.json()
                 return [File._from_data(data, session=self._session) for data in js]
 
         raise UnhandledError(f"Code {status} unhandled in get_all_files !")
 
     # TODO BROKEN FOR SOME REASON
     async def delete_all_files(self) -> int:
-        """Deletes all of your Files
+        """|coro|
+
+        Deletes all of your Files
 
         Returns
         -------
         int
             The number of removed Files
         """
         data = {"id": None, "all": True}
@@ -404,15 +426,17 @@
                 return js["count"]
             elif status >= 500:
                 raise ServerError("Unhandled exception on the server.")
 
         raise UnhandledError(f"Code {status} unhandled in delete_all_files!")
 
     async def get_recent_files(self, *, amount: int = 4, filter: Literal["all", "media"] = "all") -> List[File]:
-        """Gets recent files uploaded by you.
+        """|coro|
+
+        Gets recent files uploaded by you.
 
         Parameters
         ----------
         amount : int, optional
             The number of results to return. Must be in 1 <= amount <= 50, by default 4
         filter : Literal["all", "media"], optional
             What files to get. "all" to get all Files, "media" to get images/videos/etc., by default "all"
@@ -436,15 +460,17 @@
             if status == 200:
                 js = await resp.json()
                 return [File._from_data(data, session=self._session) for data in js]
 
         raise UnhandledError(f"Code {status} unhandled in get_recent_files!")
 
     async def get_all_shortened_urls(self) -> List[ShortenedURL]:
-        """Retrieves all shortened urls for your user.
+        """|coro|
+
+        Retrieves all shortened urls for your user.
 
         Returns
         -------
         List[ShortenedURL]
             The requested shortened urls.
         """
         async with self._session.get("/api/user/urls") as resp:
@@ -459,15 +485,17 @@
         self,
         original_url: str,
         *,
         vanity: Optional[str] = None,
         max_views: Optional[int] = None,
         zero_width_space: bool = False,
     ) -> str:
-        """Shortens a url
+        """|coro|
+
+        Shortens a url
 
         Parameters
         ----------
         original_url : str
             The url to shorten
         vanity : Optional[str], optional
             A vanity name to use. None to shorten normally, by default None
@@ -508,15 +536,17 @@
                 raise BadRequest(f"400: {msg}")
             elif status == 401:
                 raise NotAuthenticated("Auth header incorrect.")
 
         raise UnhandledError(f"Code {status} unhandled in shorten_url!")
 
     async def get_all_users(self) -> List[User]:
-        """Gets all users.
+        """|coro|
+
+        Gets all users.
 
         Returns
         -------
         List[User]
             The retrieved users
 
         Raises
@@ -536,32 +566,34 @@
 
     # TODO /api/stats methods
 
     # TODO /api/exif methods
 
     async def upload_file(
         self,
-        payload: FileUploadPayload,
+        payload: FileData,
         *,
         format: NameFormat = NameFormat.uuid,
         compression_percent: int = 0,
         expiry: Optional[datetime] = None,
         password: Optional[str] = None,
         zero_width_space: bool = False,
         embed: bool = False,
         max_views: Optional[int] = None,
         text: bool = False,
         override_name: Optional[str] = None,
         original_name: Optional[str] = None,
-    ) -> FileUploadResponse:
-        """Uploads a File to zipline
+    ) -> UploadResponse:
+        """|coro|
+
+        Uploads a File to Zipline
 
         Parameters
         ----------
-        payload : UploadFile
+        payload : FileData
             The file to upload.
         format : NameFormat, optional
             The format of the name to assign to the uploaded File, by default NameFormat.uuid
         compression_percent : int, optional
             How compressed should the uploaded File be, by default 0
         expiry : Optional[datetime], optional
             When the uploaded File should expire, by default None
@@ -578,15 +610,15 @@
         override_name : Optional[str], optional
             A name to give the uploaded file. If provided this will override the server generated name, by default None
         original_name : Optional[str], optional
             The original_name of the file. None to not preserve this data, by default None
 
         Returns
         -------
-        FileUploadResponse
+        UploadResponse
             The uploaded File
 
         Raises
         ------
         ValueError
             compression_percent was not in 0 <= compression_percent <= 100
         ValueError
@@ -618,15 +650,15 @@
         formdata = aiohttp.FormData()
         formdata.add_field("file", payload.data, filename=payload.filename, content_type=payload.mimetype)
 
         async with self._session.post("/api/upload", headers=headers, data=formdata) as resp:
             status = resp.status
             if status == 200:
                 js = await resp.json()
-                return FileUploadResponse._from_data(js)
+                return UploadResponse._from_data(js)
 
             elif status == 400:
                 js = await resp.json()
                 err_message = js["error"]
                 raise BadRequest(f"400: {err_message}")
 
             elif status >= 500:
```

### Comparing `zipline.py-0.8.1/zipline/enums.py` & `zipline.py-0.9.0/zipline/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 class NameFormat(Enum):
     """Format for the name of uploaded Files"""
 
     original_name = "name"
     uuid = "uuid"
     date = "date"
     random = "random"
-    # gfycat = "gfycat"
+    gfycat = "gfycat"
```

### Comparing `zipline.py-0.8.1/zipline/errors.py` & `zipline.py-0.9.0/zipline/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
     pass
 
 
 class NotFound(ZiplineError):
     """Server returned a 404 response."""
 
+    pass
+
 
 class ServerError(ZiplineError):
     """Server returned a 500 response code."""
 
     pass
```

### Comparing `zipline.py-0.8.1/zipline/models.py` & `zipline.py-0.9.0/zipline/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, NamedTuple, Optional, Union
 
 import aiohttp
 
 from .errors import NotFound, UnhandledError
 
-__all__ = ("File", "User", "PartialInvite", "Invite", "Folder", "ShortenedURL", "FileUploadResponse", "FileUploadPayload")
+__all__ = ("File", "User", "PartialInvite", "Invite", "Folder", "ShortenedURL", "UploadResponse", "FileData")
 
 
 @dataclass(slots=True)
 class File:
     """Represents a file stored on Zipline.
 
     Fields
@@ -97,26 +97,30 @@
             "size": data["size"],
             "url": data["url"],
             "original_name": data.get("originalName"),
         }
         return cls(_session=session, **fields)
 
     async def read(self) -> bytes:
-        """Read the File into memory.
+        """|coro|
+
+        Read the File into memory.
 
         Returns
         -------
         bytes
             The data of the File
         """
         async with self._session.get(self.full_url) as resp:
             return await resp.read()
 
     async def delete(self) -> None:
-        """Delete this File.
+        """|coro|
+
+        Delete this File.
 
         Returns
         -------
         File
             The deleted File
 
         Raises
@@ -131,15 +135,17 @@
                 return
             elif status == 404:
                 raise NotFound("404: The file could not be found.")
 
         raise UnhandledError(f"Code {status} unhandled in File.delete!")
 
     async def edit(self, *, favorite: Optional[bool] = None) -> File:
-        """Edit this File.
+        """|coro|
+
+        Edit this File.
 
         Parameters
         ----------
         favorite : Optional[bool], optional
             Whether this File is favorited., by default None
 
         Returns
@@ -164,14 +170,15 @@
         raise UnhandledError(f"Code {status} unhandled in File.delete!")
 
     @property
     def full_url(self) -> str:
         """Returns the full URL of this File."""
         return f"{self._session._base_url}{self.url}"
 
+
 @dataclass(slots=True)
 class User:
     """Represents a Zipline User.
 
     Fields
     --------
     id: int
@@ -301,15 +308,17 @@
 
     @property
     def url(self):
         """The full url of this invite."""
         return f"{self._session._base_url}/auth/register?code={self.code}"
 
     async def delete(self) -> Invite:
-        """Delete this Invite.
+        """|coro|
+
+        Delete this Invite.
 
         Returns
         -------
         Invite
             The deleted Invite.
 
         Raises
@@ -420,15 +429,17 @@
         return cls(_session=session, **fields)
 
     @property
     def full_url(self) -> str:
         return f"{self._session._base_url}{self.url}"
 
     async def delete(self) -> None:
-        """Deletes this ShortenedURL
+        """|coro|
+
+        Deletes this ShortenedURL
 
         Returns
         -------
         ShortenedURL
             The deleted url.
         """
         data = {"id": self.id}
@@ -436,15 +447,15 @@
             status = resp.status
             if status == 200:
                 return
 
         raise UnhandledError(f"Code {status} unhandled in ShortenedURL.delete!")
 
 
-class FileUploadResponse(NamedTuple):
+class UploadResponse(NamedTuple):
     """Represents a response to a File upload.
 
     Fields
     --------
     file_urls: List[str]
         The urls of the Files that were uploaded.
     expires_at: Optional[datetime]
@@ -454,26 +465,27 @@
     """
 
     file_urls: List[str]
     expires_at: Optional[datetime]
     removed_gps: Optional[bool]
 
     @classmethod
-    def _from_data(cls, data: Dict[str, Any]) -> FileUploadResponse:
+    def _from_data(cls, data: Dict[str, Any]) -> UploadResponse:
         expires_at = data.get("expiresAt")
         fields = {
             "file_urls": data["files"],
             "expires_at": datetime.fromisoformat(expires_at) if expires_at is not None else None,
             "removed_gps": data.get("removed_gps"),
         }
 
         return cls(**fields)
 
 
-class FileUploadPayload:
+# TODO support files on disk
+class FileData:
     """Represents a File to upload to Zipline."""
 
     __slots__ = ("filename", "data", "mimetype")
 
     def __init__(self, filename: str, data: Union[bytes, io.BytesIO], *, mimetype: Optional[str] = None) -> None:
         """Create a File to upload to Zipline
 
@@ -491,14 +503,15 @@
         ValueError
             An invalid value was passed to the data parameter
         TypeError
             The MIME type of the file could not be determined.
         """
         self.filename = filename
 
+        # FIXME: Suboptimal
         if isinstance(data, io.BytesIO):
             self.data = data.read()
         elif isinstance(data, bytes):
             self.data = data
         else:
             raise ValueError("data must be bytes or a BytesIO")
```

### Comparing `zipline.py-0.8.1/zipline.py.egg-info/PKG-INFO` & `zipline.py-0.9.0/zipline.py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline.py
-Version: 0.8.1
+Version: 0.9.0
 Summary: An async wrapper for the Zipline api.
 Author-email: fretgfr <fretgfr@sudomail.com>
 License: Copyright 2023 fretgfr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -25,16 +25,20 @@
 Project-URL: Homepage, https://github.com/fretgfr/zipline.py/
 Keywords: zipline,api wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: aiohttp<4,>=3.7.4
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: typing_extensions; extra == "dev"
 
 
 # Quickstart
 
 ```py
 import asyncio
```

