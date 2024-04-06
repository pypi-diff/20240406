# Comparing `tmp/AnyPathLib-0.0.1-py3-none-any.whl.zip` & `tmp/AnyPathLib-0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17415 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      123 b- defN 24-Mar-28 18:51 anypathlib/__init__.py
--rw-rw-rw-  2.0 fat     7662 b- defN 24-Mar-27 15:20 anypathlib/anypath.py
+Zip file size: 17802 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      121 b- defN 24-Apr-06 11:17 anypathlib/__init__.py
+-rw-rw-rw-  2.0 fat     8123 b- defN 24-Apr-06 10:11 anypathlib/anypath.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-16 08:25 anypathlib/path_handlers/__init__.py
--rw-rw-rw-  2.0 fat    18389 b- defN 24-Mar-19 14:30 anypathlib/path_handlers/azure_handler.py
--rw-rw-rw-  2.0 fat     1663 b- defN 24-Mar-19 14:21 anypathlib/path_handlers/base_path_handler.py
--rw-rw-rw-  2.0 fat     2825 b- defN 24-Mar-28 14:09 anypathlib/path_handlers/local_handler.py
+-rw-rw-rw-  2.0 fat    18571 b- defN 24-Apr-06 10:59 anypathlib/path_handlers/azure_handler.py
+-rw-rw-rw-  2.0 fat     1721 b- defN 24-Apr-06 10:11 anypathlib/path_handlers/base_path_handler.py
+-rw-rw-rw-  2.0 fat     2855 b- defN 24-Apr-06 10:11 anypathlib/path_handlers/local_handler.py
 -rw-rw-rw-  2.0 fat      107 b- defN 24-Jan-25 09:14 anypathlib/path_handlers/path_types.py
--rw-rw-rw-  2.0 fat     8155 b- defN 24-Mar-19 15:20 anypathlib/path_handlers/s3_handler.py
--rw-rw-rw-  2.0 fat    11561 b- defN 24-Mar-28 18:56 AnyPathLib-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5875 b- defN 24-Mar-28 18:56 AnyPathLib-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-28 18:56 AnyPathLib-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Mar-28 18:56 AnyPathLib-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1136 b- defN 24-Mar-28 18:56 AnyPathLib-0.0.1.dist-info/RECORD
-13 files, 57599 bytes uncompressed, 15493 bytes compressed:  73.1%
+-rw-rw-rw-  2.0 fat     9013 b- defN 24-Apr-06 10:11 anypathlib/path_handlers/s3_handler.py
+-rw-rw-rw-  2.0 fat    11561 b- defN 24-Apr-06 11:19 AnyPathLib-0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6026 b- defN 24-Apr-06 11:19 AnyPathLib-0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-06 11:19 AnyPathLib-0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-06 11:19 AnyPathLib-0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1126 b- defN 24-Apr-06 11:19 AnyPathLib-0.1.dist-info/RECORD
+13 files, 59327 bytes uncompressed, 15900 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: anypathlib/path_handlers/path_types.py
 Comment: 
 
 Filename: anypathlib/path_handlers/s3_handler.py
 Comment: 
 
-Filename: AnyPathLib-0.0.1.dist-info/LICENSE
+Filename: AnyPathLib-0.1.dist-info/LICENSE
 Comment: 
 
-Filename: AnyPathLib-0.0.1.dist-info/METADATA
+Filename: AnyPathLib-0.1.dist-info/METADATA
 Comment: 
 
-Filename: AnyPathLib-0.0.1.dist-info/WHEEL
+Filename: AnyPathLib-0.1.dist-info/WHEEL
 Comment: 
 
-Filename: AnyPathLib-0.0.1.dist-info/top_level.txt
+Filename: AnyPathLib-0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: AnyPathLib-0.0.1.dist-info/RECORD
+Filename: AnyPathLib-0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anypathlib/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "0.0.1"
+__version__ = "0.1"
 
 from anypathlib.anypath import AnyPath
 from anypathlib.path_handlers.path_types import PathType
```

## anypathlib/anypath.py

```diff
@@ -104,15 +104,16 @@
     def stem(self) -> str:
         return self.path_handler.stem(self.base_path)
 
     @property
     def name(self) -> str:
         return self.path_handler.name(self.base_path)
 
-    def __get_local_path(self, target_path: Optional[Path] = None, force_overwrite: bool = False) -> Path:
+    def __get_local_path(self, target_path: Optional[Path] = None, force_overwrite: bool = False,
+                         verbose: bool = False) -> Optional[Path]:
         if target_path is None:
             if self.is_dir():
                 valid_target_path = Path(tempfile.mkdtemp())
             else:
                 valid_target_path = Path(tempfile.mktemp())
         else:
             if target_path.exists():
@@ -125,50 +126,60 @@
                     shutil.copytree(self.base_path, valid_target_path, dirs_exist_ok=True)
                 else:
                     Path(valid_target_path).parent.mkdir(exist_ok=True, parents=True)
                     shutil.copy(self.base_path, valid_target_path)
             return valid_target_path
         else:
             if self.is_dir():
-                local_path, _ = self.path_handler.download_directory(url=self.base_path,
-                                                                     force_overwrite=force_overwrite,
-                                                                     target_dir=valid_target_path)
+                result = self.path_handler.download_directory(url=self.base_path,
+                                                              force_overwrite=force_overwrite,
+                                                              target_dir=valid_target_path,
+                                                              verbose=verbose)
+                if result is not None:
+                    local_path, _ = result
+                else:
+                    return None
 
             else:
                 local_path = self.path_handler.download_file(url=self.base_path, force_overwrite=force_overwrite,
                                                              target_path=valid_target_path)
 
-        assert local_path == valid_target_path, f'local_path {local_path} is not equal to valid_target_path {valid_target_path}'
+        assert local_path == valid_target_path, \
+            f'local_path {local_path} is not equal to valid_target_path {valid_target_path}'
         return Path(local_path)
 
     def __get_local_cache_path(self) -> 'AnyPath':
         handler_prefix = 's3' if self.is_s3 else 'azure' if self.is_azure else 'local'
         local_cache_path = self.LOCAL_CACHE_PATH / handler_prefix / self.path_handler.relative_path(self.base_path)
         if self.is_dir():
             local_cache_path.mkdir(exist_ok=True, parents=True)
         elif self.is_file():
             local_cache_path.parent.mkdir(exist_ok=True, parents=True)
         return AnyPath(local_cache_path)
 
-    def copy(self, target: Optional['AnyPath'] = None, force_overwrite: bool = True) -> 'AnyPath':
+    def copy(self, target: Optional['AnyPath'] = None, force_overwrite: bool = True, verbose: bool = False) -> 'AnyPath':
         assert self.exists(), f'source path: {self.base_path} does not exist'
         if target is None:
             valid_target = self.__get_local_cache_path()
         else:
             valid_target = target
         if valid_target.is_local:
-            self.__get_local_path(target_path=Path(valid_target.base_path), force_overwrite=force_overwrite)
+            self.__get_local_path(target_path=Path(valid_target.base_path), force_overwrite=force_overwrite,
+                                  verbose=verbose)
         else:
             if valid_target.is_s3 and self.is_s3:
                 S3Handler.copy(source_url=self.base_path, target_url=valid_target.base_path)
             elif valid_target.is_azure and self.is_azure:
                 AzureHandler.copy(source_url=self.base_path, target_url=valid_target.base_path)
             else:
-                # valid_target and source are different, so we need to download the source and upload it to the valid_target
+                # valid_target and source are different,
+                # so we need to download the source and upload it to the valid_target
+
                 local_path = Path(self.base_path) if self.is_local else self.__get_local_path(
-                    force_overwrite=force_overwrite)
+                    force_overwrite=force_overwrite, verbose=verbose)
                 target_path_handler = valid_target.path_handler
                 if self.is_dir():
-                    target_path_handler.upload_directory(local_dir=local_path, target_url=valid_target.base_path)
+                    target_path_handler.upload_directory(local_dir=local_path, target_url=valid_target.base_path,
+                                                         verbose=verbose)
                 else:
                     target_path_handler.upload_file(local_path=str(local_path), target_url=valid_target.base_path)
         return valid_target
```

## anypathlib/path_handlers/azure_handler.py

```diff
@@ -2,14 +2,15 @@
 import shutil
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, List, Tuple
 from urllib.parse import urlparse
 
+from tqdm import tqdm
 from azure.core.exceptions import ResourceNotFoundError
 
 from azure.identity import DefaultAzureCredential
 from azure.mgmt.storage import StorageManagementClient
 from azure.storage.blob import BlobServiceClient
 
 from loguru import logger
@@ -236,48 +237,45 @@
             try:
                 container_client.delete_blob(azure_storage_path.blob_name)
             except ResourceNotFoundError as e:
                 if not allow_missing:
                     raise e
 
     @classmethod
-    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path) -> \
+    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path, verbose: bool) -> \
             Optional[Tuple[Path, List[Path]]]:
         """Download a directory (all blobs with the same prefix) from Azure Blob Storage."""
         assert target_dir.is_dir()
         azure_storage_path = cls.http_to_storage_params(url)
 
         blob_service_client = BlobServiceClient.from_connection_string(azure_storage_path.connection_string)
         container_client = blob_service_client.get_container_client(container=azure_storage_path.container_name)
         local_paths = []
-        blob_urls = []
-        for blob in container_client.list_blobs(name_starts_with=azure_storage_path.blob_name):
+
+        if verbose:
+            container_iterator = container_client.list_blobs(name_starts_with=azure_storage_path.blob_name)
+            progress_bar = tqdm(container_iterator, desc='Downloading directory',
+                                total=len(list(container_iterator)))
+        else:
+            progress_bar = container_client.list_blobs(name_starts_with=azure_storage_path.blob_name)
+
+        for blob in progress_bar:
             blob_url = AzureStoragePath(storage_account=azure_storage_path.storage_account,
                                         container_name=azure_storage_path.container_name, blob_name=blob.name,
                                         connection_string=azure_storage_path.connection_string).http_url
-            local_target = target_dir / blob.name
+            local_target = target_dir / Path(blob_url).relative_to(Path(url))
             local_path = cls.download_file(url=blob_url, force_overwrite=force_overwrite, target_path=local_target)
             assert local_path is not None, f'could not download from {url}'
             local_paths.append(Path(local_path))
-            blob_urls.append(blob_url)
         if len(local_paths) == 0:
             return None
-        if target_dir is not None:
-            local_files = []
-            for blob_url, local_file in zip(blob_urls, local_paths):
-                relative_path = Path(blob_url).relative_to(Path(url))
-                target_path = target_dir / relative_path
-                target_path.parent.mkdir(parents=True, exist_ok=True)
-                shutil.move(local_file, target_path)
-                local_files.append(target_path)
-            return target_dir, local_files
         return local_paths[0].parent, local_paths
 
     @classmethod
-    def upload_directory(cls, local_dir: Path, target_url: str):
+    def upload_directory(cls, local_dir: Path, target_url: str, verbose: bool):
         """Upload a directory to Azure Blob Storage."""
         azure_storage_path = cls.http_to_storage_params(target_url)
         blob_service_client = BlobServiceClient.from_connection_string(azure_storage_path.connection_string)
         # Check if the container exists and create if it does not
         container_client = blob_service_client.get_container_client(azure_storage_path.container_name)
         try:
             container_client.get_container_properties()
@@ -298,16 +296,22 @@
             blob_name = os.path.join(azure_storage_path.blob_name, file_path.relative_to(local_dir))
             files_to_upload.append((file_path, blob_name))
 
         # Upload files in parallel
         with ThreadPoolExecutor() as executor:
             futures = [executor.submit(upload_file_wrapper, str(local_path), blob_name) for local_path, blob_name in
                        files_to_upload]
-            for future in futures:
-                future.result()  # Wait for each upload to complete
+            if verbose:
+                with tqdm(total=len(files_to_upload), desc='Uploading directory') as pbar:
+                    for future in futures:
+                        future.result()  # Wait for each upload to complete
+                        pbar.update(1)
+            else:
+                for future in futures:
+                    future.result()  # Wait for each upload to complete
 
     @classmethod
     def copy(cls, source_url: str, target_url: str):
         source_storage_path = cls.http_to_storage_params(source_url)
         target_storage_path = cls.http_to_storage_params(target_url)
 
         source_blob_service_client = BlobServiceClient.from_connection_string(
```

## anypathlib/path_handlers/base_path_handler.py

```diff
@@ -17,25 +17,26 @@
     @classmethod
     @abstractmethod
     def remove(cls, url: str):
         pass
 
     @classmethod
     @abstractmethod
-    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path) -> Optional[Tuple[Path, List[Path]]]:
+    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path,
+                           verbose: bool) -> Optional[Tuple[Path, List[Path]]]:
         pass
 
     @classmethod
     @abstractmethod
     def upload_file(cls, local_path: str, target_url: str):
         pass
 
     @classmethod
     @abstractmethod
-    def upload_directory(cls, local_dir: Path, target_url: str):
+    def upload_directory(cls, local_dir: Path, target_url: str, verbose: bool):
         pass
 
     @classmethod
     @abstractmethod
     def copy(cls, source_url: str, target_url: str):
         pass
```

## anypathlib/path_handlers/local_handler.py

```diff
@@ -28,15 +28,15 @@
             shutil.rmtree(local_path)
 
     @classmethod
     def upload_file(cls, local_path: str, target_url: str):
         cls.copy_path(url=Path(local_path).absolute().as_posix(), target_path=Path(target_url), force_overwrite=True)
 
     @classmethod
-    def upload_directory(cls, local_dir: Path, target_url: str):
+    def upload_directory(cls, local_dir: Path, target_url: str, verbose: bool):
         cls.copy_path(url=local_dir.absolute().as_posix(), target_path=Path(target_url), force_overwrite=True)
 
     @classmethod
     def copy(cls, source_url: str, target_url: str):
         cls.copy_path(url=source_url, target_path=Path(target_url), force_overwrite=True)
 
     @classmethod
@@ -48,15 +48,15 @@
         local_path = Path(url)
         if local_path.is_dir():
             shutil.copytree(local_path, target_path)
         else:
             shutil.copy(local_path, target_path)
 
     @classmethod
-    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path) -> \
+    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path, verbose: bool) -> \
             Optional[Tuple[Path, List[Path]]]:
         cls.copy_path(url=url, target_path=target_dir, force_overwrite=force_overwrite)
         return target_dir, [p for p in target_dir.rglob('*')]
 
     @classmethod
     def download_file(cls, url: str, target_path: Path, force_overwrite: bool = True) -> Path:
         return cls.copy_path(url=url, target_path=target_path, force_overwrite=force_overwrite)
```

## anypathlib/path_handlers/s3_handler.py

```diff
@@ -2,14 +2,15 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from typing import List, Tuple, Optional, ClassVar
 from urllib.parse import urlparse
 
 import boto3 as boto3
 import botocore
+from tqdm import tqdm
 
 from anypathlib.path_handlers.base_path_handler import BasePathHandler
 
 
 class S3Handler(BasePathHandler):
     AWS_ACCESS_KEY_ID = os.environ.get('AWS_ACCESS_KEY_ID', None)
     MAX_POOL_CONNECTIONS = 50
@@ -107,15 +108,15 @@
     def remove(cls, url: str):
         bucket, key = cls.get_bucket_and_key_from_uri(url)
         s3_resource = boto3.resource('s3')
         bucket = s3_resource.Bucket(bucket)
         bucket.objects.filter(Prefix=key).delete()
 
     @classmethod
-    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path) -> \
+    def download_directory(cls, url: str, force_overwrite: bool, target_dir: Path, verbose: bool) -> \
             Optional[Tuple[Path, List[Path]]]:
 
         s3_resource = boto3.resource('s3')
 
         bucket, source_key = cls.get_bucket_and_key_from_uri(url)
         bucket = s3_resource.Bucket(bucket)
         all_files = []
@@ -133,38 +134,65 @@
         # Download in parallel
         with ThreadPoolExecutor() as executor:
             future_to_s3_path = {executor.submit(cls.download_file,
                                                  url=s3_path,
                                                  target_path=s3_path_to_local_file_path(s3_path=s3_path,
                                                                                         local_base_path=target_dir),
                                                  force_overwrite=force_overwrite): s3_path for s3_path in s3_paths}
-            for future in as_completed(future_to_s3_path):
-                s3_path = future_to_s3_path[future]
-                try:
-                    local_path = future.result()
-                    if local_path:
-                        all_files.append(local_path)
-                except Exception as exc:
-                    print(f'{s3_path} generated an exception: {exc}')
+
+            def process_futures():
+                for future in as_completed(future_to_s3_path):
+                    s3_path = future_to_s3_path[future]
+                    try:
+                        local_path = future.result()
+                        if local_path:
+                            all_files.append(local_path)
+                    except Exception as exc:
+                        print(f'{s3_path} generated an exception: {exc}')
+
+                    yield None
+
+            if verbose:
+                with tqdm(total=len(s3_paths), desc='Downloading directory') as pbar:
+                    for _ in process_futures():
+                        pbar.update(1)
+            else:
+                for _ in process_futures():
+                    pass
+
         return target_dir, all_files
 
     @classmethod
     def upload_file(cls, local_path: str, target_url: str):
         bucket, key = cls.get_bucket_and_key_from_uri(target_url)
         cls.s3_client.upload_file(local_path, bucket, key)
 
     @classmethod
-    def upload_directory(cls, local_dir: Path, target_url: str):
+    def upload_directory(cls, local_dir: Path, target_url: str, verbose: bool = False):
         bucket, key = cls.get_bucket_and_key_from_uri(target_url)
-        for root, dirs, files in os.walk(local_dir):
+
+        total_files = 0
+        if verbose:
+            for root, dirs, files in os.walk(local_dir):
+                total_files += len(files)
+
+        if verbose:
+            progress_bar = tqdm(os.walk(local_dir), desc='Uploading directory', total=total_files)
+        else:
+            progress_bar = os.walk(local_dir)
+
+        for root, dirs, files in progress_bar:
             for file in files:
                 local_path = os.path.join(root, file)
-                s3_key = os.path.join(key, os.path.relpath(local_path, local_dir))
+                s3_key = f'{key}/{os.path.relpath(local_path, local_dir)}'
                 cls.s3_client.upload_file(local_path, bucket, s3_key)
 
+            if verbose:
+                progress_bar.update(len(files))
+
     @classmethod
     def copy(cls, source_url: str, target_url: str):
         s3_resource = boto3.resource('s3')
         source_bucket_name, source_key = cls.get_bucket_and_key_from_uri(source_url)
         target_bucket_name, target_key = cls.get_bucket_and_key_from_uri(target_url)
 
         source_bucket = s3_resource.Bucket(source_bucket_name)
```

## Comparing `AnyPathLib-0.0.1.dist-info/LICENSE` & `AnyPathLib-0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `AnyPathLib-0.0.1.dist-info/METADATA` & `AnyPathLib-0.1.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-Metadata-Version: 2.1
-Name: AnyPathLib
-Version: 0.0.1
-Summary: A unified API for every storage resource
-Home-page: 
-Author: Kfir Goldberg @ WSC-Sports
-License: Apache License 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: azure-storage-blob (>=12.14.0)
-Requires-Dist: azure-identity (>=1.15.0)
-Requires-Dist: azure-mgmt-storage (>=21.1.0)
-Requires-Dist: boto3 (>=1.34.23)
-Requires-Dist: loguru (>=0.7.2)
-
-<p align="center"><img src="https://raw.githubusercontent.com/kfirgoldberg/AnyPathLib/master/docs/anypathlib_logo.png" alt="logo" width="70%" /></p>
-
-
-<div align="center">
-
-[![wsc_logo](https://raw.githubusercontent.com/kfirgoldberg/AnyPathLib/master/docs/wsc_logo.png)](https://wsc-sports.com/)
-
-</div>
-
-# AnyPathLib - Crossing Cloud Borders With a Simple API
-
-<p align="center">
-    <a href="https://badge.fury.io/py/anypathlib"><img src="https://badge.fury.io/py/anypathlib.svg" alt="PyPI version" height="18"></a>
-    <a href="https://pepy.tech/project/anypathlib"><img src="https://pepy.tech/badge/anypathlib" alt="Downloads" height="18"></a>
-    <a href="#contributors-"><img src="https://img.shields.io/badge/all_contributors-2-orange.svg" alt="All Contributors" height="18"></a>
-    <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0" height="18"></a>
-</p>
-
-
-Welcome to AnyPathLib, a Python library designed to allow hassle-free file operations across different cloud and local
-storage
-
-## Why `AnyPathLib`?
-
-With `AnyPathLib` you can write the same code to handle files across different storage systems, without worrying about
-the
-underlying details.
-Operations can be optimized per-backend and the library is easily extendable to support additional cloud storage
-providers.
-
-## Getting Started With `AnyPathLib` with 3 easy examples ️🛣️
-
-### ️🛣️ 1/3 Copying a file or directory from anywhere to anywhere ️🛣️
-
-```python
-from anypathlib import AnyPath
-
-# Create an AnyPath instance for a local file
-local_file = AnyPath("/path/to/local/file.txt")
-
-# Create an AnyPath instance for an S3 object
-s3_file = AnyPath("s3://bucket/path/to/object.txt")
-
-# Copy a file from local to S3
-local_file.copy(s3_file)
-
-# Copy a directory from S3 to Azure
-s3_dir = AnyPath("s3://bucket/path/to/dir")
-azure_dir = AnyPath("https://account_name.blob.core.windows.net/container_name/path")
-s3_dir.copy(azure_dir)
-```
-
-### ️🛣️ 2/3 Local caching for quicker access ️🛣️
-
-Use "copy" without a target to get a local copy of the file which is stored in a local cache.
-Use `force_overwrite=False` to prevent repeated downloads of the same file
-
-```python
-my_dir = AnyPath("https://account_name.blob.core.windows.net/container_name/path/to/dir")
-local_dir_path = my_dir.copy()
-
-my_file = AnyPath("s3://bucket/path/to/file.txt")
-local_file_path = my_file.copy()
-local_file_path = my_file.copy(force_overwrite=False)  # Returns the path of the previously downloaded file
-```
-
-### 🛣️ 3/3 A simplified pathlib-like Interface 🛣️
-
-```python
-my_dir = AnyPath("https://account_name.blob.core.windows.net/container_name/path/to/dir")
-my_dir.exists()  # True if my_path exists, otherwise False
-parent, name, stem = my_dir.parent, my_dir.name, my_dir.stem
-files_in_dir: List[AnyPath] = my_dir.listdir()  # List of AnyPath instances for files in the directory
-
-my_file = AnyPath("s3://bucket/path/to/file.txt")
-my_file.is_file()  # True if my_path exists, otherwise False
-my_file.is_dir()  # False
-my_file.remove()
-```
-
-### Key Features
-
-* **Unified, Cloud Agnostic, API**: Perform file operations across different storage backends using the same set of
-  methods.
-* **Path-like Operations**: Supports common path operations like joining paths, listing directories, checking file
-  existence, etc.
-* **Performance**: Local caching for repeated downloads across different sessions, multithreading, and more.
-* **Extensibility**: Easily extendable to support additional cloud storage providers.
-
-### Security and Credentials
-
-`AnyPath` does not store any credentials in it. In order to access cloud storage, you need to have the necessary
-environment variables defined.
-
-#### Azure
-
-```bash
-export AZURE_SUBSCRIPTION_ID="your-subscription-id"
-export AZURE_RESOURCE_GROUP_NAME="your-resource-group-name"
-```
-
-#### AWS S3
-
-Same as Boto3:
-
-```bash
-export AWS_DEFAULT_REGION="your-region"
-export AWS_SECRET_ACCESS_KEY="your-secret"
-export AWS_ACCESS_KEY_ID="your-key"
-```
-
-# TODOs:
-
-- [ ] Add support for additional cloud storage providers.
-
-> GCP
-
-- [ ] Improve API
-
-> Add support for file-to-dir in copy
-
-- [ ] Implement cloud-to-cloud ops more efficiently.
-
-> For example, s3->azure can use AZCopy
-
-- [ ] Improve logging and add verbose mode.
-
-> progress bar, etc.
-
-## Contributors ✨
-
-Thanks goes to these wonderful people:
-
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tr>
-    <td align="center"><a href="https://github.com/shomerYu"><img src="https://avatars.githubusercontent.com/u/49059794?v=4" width="100px;" alt=""/><br /><sub><b>Yuval Shomer</b></sub></a><br /><a href="#design-shomerYu" title="Design">🎨</a> <a href="#ideas-shomerYu" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/jeremy-levy"><img src="https://avatars.githubusercontent.com/u/61752548?v=4" width="100px;" alt=""/><br /><sub><b>Jeremy Levy</b></sub></a><br /><a href="#design-jeremy-levy" title="Design">🎨</a> <a href="#ideas-jeremy-levy" title="Ideas, Planning, & Feedback">🤔</a></td>
-
-
-  </tr>
-</table>
+Metadata-Version: 2.1
+Name: AnyPathLib
+Version: 0.1
+Summary: A unified API for every storage resource
+Home-page: 
+Author: Kfir Goldberg @ WSC-Sports
+License: Apache License 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: azure-storage-blob >=12.14.0
+Requires-Dist: azure-identity >=1.15.0
+Requires-Dist: azure-mgmt-storage >=21.1.0
+Requires-Dist: boto3 >=1.34.23
+Requires-Dist: loguru >=0.7.2
+
+<p align="center"><img src="https://raw.githubusercontent.com/kfirgoldberg/AnyPathLib/master/docs/anypathlib_logo.png" alt="logo" width="70%" /></p>
+
+
+<div align="center">
+
+[![wsc_logo](https://raw.githubusercontent.com/kfirgoldberg/AnyPathLib/master/docs/wsc_logo.png)](https://wsc-sports.com/)
+
+</div>
+
+# AnyPathLib - Crossing Cloud Borders With a Simple API
+
+<p align="center">
+    <a href="https://badge.fury.io/py/AnyPathLib"><img src="https://badge.fury.io/py/AnyPathLib.svg" alt="PyPI version" height="18"></a>
+    <a href="https://pepy.tech/project/anypathlib"><img src="https://pepy.tech/badge/anypathlib" alt="Downloads" height="18"></a>
+    <a href="#contributors-"><img src="https://img.shields.io/badge/all_contributors-2-orange.svg" alt="All Contributors" height="18"></a>
+    <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License: Apache 2.0" height="18"></a>
+</p>
+
+
+Welcome to AnyPathLib, a Python library designed to allow hassle-free file operations across different cloud and local
+storage
+
+## Why `AnyPathLib`?
+
+With `AnyPathLib` you can write the same code to handle files across different storage systems, without worrying about
+the
+underlying details.
+Operations can be optimized per-backend and the library is easily extendable to support additional cloud storage
+providers.
+
+## Getting Started With `AnyPathLib` with 3 easy examples ️🛣️
+
+### ️🛣️ 1/3 Copying a file or directory from anywhere to anywhere ️🛣️
+
+```python
+from anypathlib import AnyPath
+
+# Create an AnyPath instance for a local file
+local_file = AnyPath("/path/to/local/file.txt")
+
+# Create an AnyPath instance for an S3 object
+s3_file = AnyPath("s3://bucket/path/to/object.txt")
+
+# Copy a file from local to S3
+local_file.copy(s3_file)
+
+# Copy a directory from S3 to Azure
+s3_dir = AnyPath("s3://bucket/path/to/dir")
+azure_dir = AnyPath("https://account_name.blob.core.windows.net/container_name/path")
+s3_dir.copy(azure_dir)
+```
+
+### ️🛣️ 2/3 Local caching for quicker access ️🛣️
+
+Use "copy" without a target to get a local copy of the file which is stored in a local cache.
+Use `force_overwrite=False` to prevent repeated downloads of the same file
+
+```python
+my_dir = AnyPath("https://account_name.blob.core.windows.net/container_name/path/to/dir")
+local_dir_path = my_dir.copy()
+
+my_file = AnyPath("s3://bucket/path/to/file.txt")
+local_file_path = my_file.copy()
+local_file_path = my_file.copy(force_overwrite=False)  # Returns the path of the previously downloaded file
+```
+
+### 🛣️ 3/3 A simplified pathlib-like Interface 🛣️
+
+```python
+my_dir = AnyPath("https://account_name.blob.core.windows.net/container_name/path/to/dir")
+my_dir.exists()  # True if my_path exists, otherwise False
+parent, name, stem = my_dir.parent, my_dir.name, my_dir.stem
+files_in_dir: List[AnyPath] = my_dir.listdir()  # List of AnyPath instances for files in the directory
+
+my_file = AnyPath("s3://bucket/path/to/file.txt")
+my_file.is_file()  # True if my_path exists, otherwise False
+my_file.is_dir()  # False
+my_file.remove()
+```
+
+### Key Features
+
+* **Unified, Cloud Agnostic, API**: Perform file operations across different storage backends using the same set of
+  methods.
+* **Path-like Operations**: Supports common path operations like joining paths, listing directories, checking file
+  existence, etc.
+* **Performance**: Local caching for repeated downloads across different sessions, multithreading, and more.
+* **Extensibility**: Easily extendable to support additional cloud storage providers.
+
+### Security and Credentials
+
+`AnyPath` does not store any credentials in it. In order to access cloud storage, you need to have the necessary
+environment variables defined.
+
+#### Azure
+
+```bash
+export AZURE_SUBSCRIPTION_ID="your-subscription-id"
+export AZURE_RESOURCE_GROUP_NAME="your-resource-group-name"
+```
+
+#### AWS S3
+
+Same as Boto3:
+
+```bash
+export AWS_DEFAULT_REGION="your-region"
+export AWS_SECRET_ACCESS_KEY="your-secret"
+export AWS_ACCESS_KEY_ID="your-key"
+```
+
+# TODOs:
+
+- [ ] Add support for additional cloud storage providers.
+
+> GCP
+
+- [ ] Improve API
+
+> Add support for file-to-dir in copy
+
+- [ ] Implement cloud-to-cloud ops more efficiently.
+
+> For example, s3->azure can use AZCopy
+
+- [ ] Improve logging and add verbose mode.
+
+> progress bar, etc.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people:
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="https://github.com/shomerYu"><img src="https://avatars.githubusercontent.com/u/49059794?v=4" width="100px;" alt=""/><br /><sub><b>Yuval Shomer</b></sub></a><br /><a href="#design-shomerYu" title="Design">🎨</a> <a href="#ideas-shomerYu" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/jeremy-levy"><img src="https://avatars.githubusercontent.com/u/61752548?v=4" width="100px;" alt=""/><br /><sub><b>Jeremy Levy</b></sub></a><br /><a href="#design-jeremy-levy" title="Design">🎨</a> <a href="#ideas-jeremy-levy" title="Ideas, Planning, & Feedback">🤔</a></td>
+
+
+  </tr>
+</table>
```

### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: AnyPathLib Version: 0.0.1 Summary: A unified API
-for every storage resource Home-page: Author: Kfir Goldberg @ WSC-Sports
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: azure-storage-blob
-(>=12.14.0) Requires-Dist: azure-identity (>=1.15.0) Requires-Dist: azure-mgmt-
-storage (>=21.1.0) Requires-Dist: boto3 (>=1.34.23) Requires-Dist: loguru
-(>=0.7.2)
+Metadata-Version: 2.1 Name: AnyPathLib Version: 0.1 Summary: A unified API for
+every storage resource Home-page: Author: Kfir Goldberg @ WSC-Sports License:
+Apache License 2.0 Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: azure-storage-blob >=12.14.0
+Requires-Dist: azure-identity >=1.15.0 Requires-Dist: azure-mgmt-storage
+>=21.1.0 Requires-Dist: boto3 >=1.34.23 Requires-Dist: loguru >=0.7.2
                                     [logo]
 [![wsc_logo](https://raw.githubusercontent.com/kfirgoldberg/AnyPathLib/master/
                  docs/wsc_logo.png)](https://wsc-sports.com/)
 # AnyPathLib - Crossing Cloud Borders With a Simple API
        _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_A_l_l_ _C_o_n_t_r_i_b_u_t_o_r_s_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_]
 Welcome to AnyPathLib, a Python library designed to allow hassle-free file
 operations across different cloud and local storage ## Why `AnyPathLib`? With
```

## Comparing `AnyPathLib-0.0.1.dist-info/RECORD` & `AnyPathLib-0.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-anypathlib/__init__.py,sha256=AApnJLITyhZP036gV5RVSF4lWu96xWm1alFY1j-FKao,123
-anypathlib/anypath.py,sha256=G_pN4he8TGWsgGn3aUAaLtmQ2k2Yighoqf2KV3MiIbY,7662
+anypathlib/__init__.py,sha256=wllwHErnP4RKPu1AeHPCbWr-H2cnPDUod8BKwdU7gTo,121
+anypathlib/anypath.py,sha256=rR6c7MegfwsOftHuxR9pqCleXcFYDpt-iYe4bb0vxLo,8123
 anypathlib/path_handlers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-anypathlib/path_handlers/azure_handler.py,sha256=WLv0ox1yr0_q6RnxG8zZRyzJ1Lh91Ns23uEZY9ZxTbo,18389
-anypathlib/path_handlers/base_path_handler.py,sha256=8vuRoQf6EcK21eaiJFKZeYOrKfBF9SFzaV5bJ7fHoWI,1663
-anypathlib/path_handlers/local_handler.py,sha256=MoPgoEIiB7G4Kla0s4h-qKR_mRwHSg92Ch2yg0Vb0FM,2825
+anypathlib/path_handlers/azure_handler.py,sha256=HH08Nj9tbYSCvyuMFRN8bVFqiADNtxu9qCcTxhlPw-w,18571
+anypathlib/path_handlers/base_path_handler.py,sha256=9oaiIch-us1gXYMxXW3N4TYUyVmF8LEobtU6hwfskFQ,1721
+anypathlib/path_handlers/local_handler.py,sha256=HU8MWJG0dwQjKtBd5aYYXYqAPl28FAZQgwCDhGYss5s,2855
 anypathlib/path_handlers/path_types.py,sha256=gv5o_e8JSZ16qOXpxZcnu5LV8tbnHS_I9hdaP82sjT8,107
-anypathlib/path_handlers/s3_handler.py,sha256=aN_KdZy_okSANdYfofAFO4MNbsiD3V_wWuzwfqcXuf0,8155
-AnyPathLib-0.0.1.dist-info/LICENSE,sha256=Ls_5-emELRHMIJYSfoJ7X-jye7mWU6Y6cjcwlaYJUOs,11561
-AnyPathLib-0.0.1.dist-info/METADATA,sha256=fO9PhQSlbRWXEcIOftN4z-yMDZObLWLqFZN7RNR6ssI,5875
-AnyPathLib-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-AnyPathLib-0.0.1.dist-info/top_level.txt,sha256=aHyf6q1CvDie1Gm6yQYrS6pbFySD4ZNRI-maqhKbxJk,11
-AnyPathLib-0.0.1.dist-info/RECORD,,
+anypathlib/path_handlers/s3_handler.py,sha256=P1mS_fkYJpnGzzlDIXRO3oY5AO49SzGaSYU7EomtlKg,9013
+AnyPathLib-0.1.dist-info/LICENSE,sha256=Ls_5-emELRHMIJYSfoJ7X-jye7mWU6Y6cjcwlaYJUOs,11561
+AnyPathLib-0.1.dist-info/METADATA,sha256=X7equ-_qYZiSZLMdw-EEnh_X1VEdRtbgU-ismxoQPiw,6026
+AnyPathLib-0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+AnyPathLib-0.1.dist-info/top_level.txt,sha256=aHyf6q1CvDie1Gm6yQYrS6pbFySD4ZNRI-maqhKbxJk,11
+AnyPathLib-0.1.dist-info/RECORD,,
```

