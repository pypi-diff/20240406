# Comparing `tmp/apt-mirror-3.tar.gz` & `tmp/apt-mirror-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apt-mirror-3.tar", last modified: Sat Mar  9 10:33:54 2024, max compression
+gzip compressed data, was "apt-mirror-4.tar", last modified: Sat Apr  6 12:46:47 2024, max compression
```

## Comparing `apt-mirror-3.tar` & `apt-mirror-4.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 10:33:54.591815 apt-mirror-3/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-03-09 10:33:43.000000 apt-mirror-3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    44880 2024-03-09 10:33:54.591815 apt-mirror-3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2966 2024-03-09 10:33:43.000000 apt-mirror-3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 10:33:54.587815 apt-mirror-3/apt_mirror/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21131 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/apt_mirror.py
--rw-rw-rw-   0 root         (0) root         (0)    17782 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/config.py
--rw-rw-rw-   0 root         (0) root         (0)    31232 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/download.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/logs.py
--rw-rw-rw-   0 root         (0) root         (0)    24907 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/repository.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-03-09 10:33:43.000000 apt-mirror-3/apt_mirror/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 10:33:54.589815 apt-mirror-3/apt_mirror.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44880 2024-03-09 10:33:54.000000 apt-mirror-3/apt_mirror.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      481 2024-03-09 10:33:54.000000 apt-mirror-3/apt_mirror.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-09 10:33:54.000000 apt-mirror-3/apt_mirror.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-09 10:33:54.000000 apt-mirror-3/apt_mirror.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      211 2024-03-09 10:33:54.000000 apt-mirror-3/apt_mirror.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-09 10:33:54.000000 apt-mirror-3/apt_mirror.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2030 2024-03-09 10:33:43.000000 apt-mirror-3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-03-09 10:33:54.591815 apt-mirror-3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      104 2024-03-09 10:33:43.000000 apt-mirror-3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 10:33:54.589815 apt-mirror-3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1141 2024-03-09 10:33:43.000000 apt-mirror-3/tests/test_clean.py
--rw-rw-rw-   0 root         (0) root         (0)     8286 2024-03-09 10:33:43.000000 apt-mirror-3/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2024-03-09 10:33:43.000000 apt-mirror-3/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.563371 apt-mirror-4/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-04-06 12:46:36.000000 apt-mirror-4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45480 2024-04-06 12:46:47.563371 apt-mirror-4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2024-04-06 12:46:36.000000 apt-mirror-4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.558371 apt-mirror-4/apt_mirror/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25466 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/apt_mirror.py
+-rw-rw-rw-   0 root         (0) root         (0)    18418 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.560371 apt-mirror-4/apt_mirror/download/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    15148 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.561371 apt-mirror-4/apt_mirror/download/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/protocols/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/protocols/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/protocols/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2722 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)    28434 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.562371 apt-mirror-4/apt_mirror.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45480 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      845 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2024-04-06 12:46:36.000000 apt-mirror-4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-06 12:46:47.564371 apt-mirror-4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      104 2024-04-06 12:46:36.000000 apt-mirror-4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.562371 apt-mirror-4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     8286 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_repository.py
```

### Comparing `apt-mirror-3/LICENSE` & `apt-mirror-4/LICENSE`

 * *Files identical despite different names*

### Comparing `apt-mirror-3/PKG-INFO` & `apt-mirror-4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apt-mirror
-Version: 3
+Version: 4
 Summary: apt-mirror Python reimplementation
 Author-email: Yuri Konotopov <ykonotopov@gnome.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,20 +693,22 @@
 License-File: LICENSE
 Requires-Dist: aiofile==3.8.8
 Requires-Dist: aiolimiter==1.1.0
 Requires-Dist: aioftp==0.21.4
 Requires-Dist: httpx[http2]==0.26.0
 Requires-Dist: python-debian==0.1.49
 Provides-Extra: dev
-Requires-Dist: black==23.11.0; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: pip-tools==7.0.0; extra == "dev"
 Requires-Dist: pylint==3.0.3; extra == "dev"
 Requires-Dist: pytest==7.4.4; extra == "dev"
+Provides-Extra: prometheus
+Requires-Dist: prometheus-client==0.20.0; extra == "prometheus"
 Provides-Extra: uvloop
 Requires-Dist: uvloop==0.19.0; extra == "uvloop"
 
 # apt-mirror2
 
 [`apt-mirror2`](https://gitlab.com/apt-mirror2/apt-mirror2) is the Python/asyncio reimplementation of the
 [apt-mirror](https://github.com/apt-mirror/apt-mirror) developed as drop-in replacement for the latest.  
@@ -777,24 +779,31 @@
 ```
 
 # apt-mirror configuration compatibility
 
 Most of `apt-mirror` configuration directives are supported.  
 As of now proxy for FTP repositories is not supported.  
 
+File lists (ALL, NEW, MD5, SHA256, SHA512) are not written by default, but you can enable them with the `write_file_lists` option.
+
 In addition there are some enhancements available:
 
 - Repositories without MD5 hashsums are correctly mirrored
 - Old index files are properly cleaned and don't produces errors in mirror processing
 - Standard source.list `[ arch=arch1,arch2 ]` can be used to specify multiple repository architectures for mirroring.
+- multiple codenames (or flat folders) can be specified using comma as delimiter.
 - `mirror_path URL PATH` option may be used to specify `PATH` to use for saving mirror files instead of path that is generated from `URL`.
 - Additional configuration is loaded from the `*.list` files in the directory named same as `configfile` with the `.d` suffix. Eg `/etc/apt/mirror.list.d/*.list`.
 - Rate limit is enforced for overall download rate.
 - Non-zero exit code is returned if some of required files were not downloaded due to network or server errors or
   no repositories were configured.
 - HTTP user agent can be configured via `user_agent` configuration.
 - Configuration variables are exposed to postmirror_script.
 - `by-hash` list option can be used to control whether `Acquire-By-Hash` Release option should be respected or enforced.
+- mirror wipe protection is available and configurable via `wipe_size_ratio` and `wipe_count_ratio` settings.
+- per-repository log files are available in the `var_path` folder
+- `dists` folder is almost atomicaly replaced using move instead of copy/link
+- native Prometheus metrics are supported
 
 # License
 
 GNU General Public License v3.0 or later
```

### Comparing `apt-mirror-3/README.md` & `apt-mirror-4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -69,24 +69,31 @@
 ```
 
 # apt-mirror configuration compatibility
 
 Most of `apt-mirror` configuration directives are supported.  
 As of now proxy for FTP repositories is not supported.  
 
+File lists (ALL, NEW, MD5, SHA256, SHA512) are not written by default, but you can enable them with the `write_file_lists` option.
+
 In addition there are some enhancements available:
 
 - Repositories without MD5 hashsums are correctly mirrored
 - Old index files are properly cleaned and don't produces errors in mirror processing
 - Standard source.list `[ arch=arch1,arch2 ]` can be used to specify multiple repository architectures for mirroring.
+- multiple codenames (or flat folders) can be specified using comma as delimiter.
 - `mirror_path URL PATH` option may be used to specify `PATH` to use for saving mirror files instead of path that is generated from `URL`.
 - Additional configuration is loaded from the `*.list` files in the directory named same as `configfile` with the `.d` suffix. Eg `/etc/apt/mirror.list.d/*.list`.
 - Rate limit is enforced for overall download rate.
 - Non-zero exit code is returned if some of required files were not downloaded due to network or server errors or
   no repositories were configured.
 - HTTP user agent can be configured via `user_agent` configuration.
 - Configuration variables are exposed to postmirror_script.
 - `by-hash` list option can be used to control whether `Acquire-By-Hash` Release option should be respected or enforced.
+- mirror wipe protection is available and configurable via `wipe_size_ratio` and `wipe_count_ratio` settings.
+- per-repository log files are available in the `var_path` folder
+- `dists` folder is almost atomicaly replaced using move instead of copy/link
+- native Prometheus metrics are supported
 
 # License
 
 GNU General Public License v3.0 or later
```

### Comparing `apt-mirror-3/apt_mirror/apt_mirror.py` & `apt-mirror-4/apt_mirror/apt_mirror.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,33 @@
 
 import argparse
 import asyncio
 import itertools
 import os
 import shutil
 import signal
+from contextlib import ExitStack
 from errno import EWOULDBLOCK
 from fcntl import LOCK_EX, LOCK_NB, flock
 from pathlib import Path
 from typing import IO, Any, Awaitable, Iterable, Sequence
 
 from aiolimiter import AsyncLimiter
 
 from .config import Config
-from .download import Downloader, DownloadFile, DownloadFileCompressionVariant
+from .download import (
+    Downloader,
+    DownloaderFactory,
+    DownloadFile,
+    DownloadFileCompressionVariant,
+    HashType,
+)
 from .logs import LoggerFactory
-from .repository import BaseRepository
+from .prometheus import DownloaderCollector
+from .repository import BaseRepository, InvalidReleaseFilesException
 from .version import __version__
 
 LOG = LoggerFactory.get_logger(__package__)
 
 
 class PathCleaner:
     def __init__(
@@ -118,19 +126,21 @@
 
     @property
     def folders_count(self):
         return len(self._folders_queue)
 
     def write_clean_script(self, fp: IO[str], repository: BaseRepository):
         fp.write(
-            "\n".join([
-                "#!/bin/bash",
-                "set -e",
-                "",
-            ])
+            "\n".join(
+                [
+                    "#!/bin/bash",
+                    "set -e",
+                    "",
+                ]
+            )
         )
 
         if not self._clean_allowed():
             self._log_wipe_threashold_warning()
             fp.write("echo ")
             fp.write(self._wipe_threashold_warning())
             fp.write(os.linesep)
@@ -194,60 +204,68 @@
     def __init__(
         self,
         repository: BaseRepository,
         config: Config,
         semaphore: asyncio.Semaphore,
         download_semaphore: asyncio.Semaphore,
         rate_limiter: AsyncLimiter | None,
+        metrics_collector: DownloaderCollector,
     ) -> None:
         self._log = LoggerFactory.get_logger(self, logger_id=repository.url)
 
         self._error = False
 
         self._repository = repository
         self._pool_folders: set[Path] = set()
 
         self._config = config
         self._download_semaphore = download_semaphore
         self._semaphore = semaphore
         self._rate_limiter = rate_limiter
 
-        self._downloader = Downloader.for_url(
+        self._downloader = DownloaderFactory.for_url(
             url=self._repository.url,
             target_root_path=self._config.skel_path
             / self._repository.get_mirror_path(self._config.encode_tilde),
             proxy=self._config.proxy,
             user_agent=self._config.user_agent,
             semaphore=self._download_semaphore,
             rate_limiter=self._rate_limiter,
             verify_ca_certificate=self._config.verify_ca_certificate,
             client_certificate=self._config.client_certificate,
             client_private_key=self._config.client_private_key,
         )
 
+        metrics_collector.add_downloader(self._repository, self._downloader)
+
     async def mirror(self) -> bool:
         """Start repository mirror process
 
         Returns:
             bool: True if mirror was successful, False otherwise
         """
         async with self._semaphore:
             self._log.info(f"Mirroring repository {self._repository}")
 
-            await self.download_release_files()
+            release_files = await self.download_release_files()
+            if not release_files:
+                self._log.error(
+                    f"Unable to obtain release files for repository {self._repository}"
+                )
+                return False
 
             # Download other metadata files
             metadata_files = await self.download_metadata_files()
             if not metadata_files:
                 self._log.error(
                     f"Unable to obtain metadata files for repository {self._repository}"
                 )
                 return False
 
-            downloaded_metadata_files = self._downloader.get_downloaded_files()
+            downloaded_metadata_files = self._downloader.get_all_files()
 
             await self.clean_repository_skel(
                 set(
                     itertools.chain.from_iterable(
                         v.get_all_paths() for v in downloaded_metadata_files
                     )
                 )
@@ -258,35 +276,64 @@
             await self.download_pool_files()
 
             # Move skel to mirror
             await self.move_metadata(downloaded_metadata_files)
 
             if self._repository.clean:
                 await self.clean_repository(
-                    needed_files=set(
-                        itertools.chain.from_iterable(
-                            v.get_all_paths()
-                            for v in self._downloader.get_downloaded_files()
-                        )
-                    )
-                    - self._downloader.get_missing_sources(),
+                    needed_files=self._downloader.get_downloaded_files_paths(),
                     unlink=self._config.autoclean,
                 )
 
+            self._log.info(f"Repository {self._repository} mirroring complete")
+
         return not self._error
 
     async def download_release_files(self) -> Sequence[DownloadFile]:
         # Download release files
         self._log.info(f"Downloading release files for repository {self._repository}")
         release_files = [
             DownloadFile.from_path(path, ignore_missing=True)
             for path in self._repository.release_files
         ]
-        self._downloader.add(*release_files)
-        await self._downloader.download()
+
+        tries = 15
+        while True:
+            self._downloader.reset_paths()
+            self._downloader.add(*release_files)
+            await self._downloader.download()
+
+            # Drop release files in skel which we were unable to download
+            downloaded_paths = self._downloader.get_downloaded_files_paths()
+            for relative_path in self._repository.release_files:
+                path = (
+                    self._config.skel_path
+                    / self._repository.get_mirror_path(self._config.encode_tilde)
+                    / relative_path
+                )
+
+                if path.exists() and relative_path not in downloaded_paths:
+                    path.unlink()
+
+            # Check release files
+            try:
+                self._repository.validate_release_files(
+                    self._config.skel_path, self._config.encode_tilde
+                )
+                break
+            except InvalidReleaseFilesException as ex:
+                self._log.warning(
+                    f"Release files are invalid: {ex.message}. Retrying..."
+                )
+                tries -= 1
+
+                if tries < 1:
+                    return []
+
+                await asyncio.sleep(5)
 
         return release_files
 
     async def download_metadata_files(self) -> Iterable[DownloadFile]:
         metadata_files = self._repository.get_metadata_files(
             self._config.skel_path,
             self._config.encode_tilde,
@@ -298,15 +345,15 @@
             return metadata_files
 
         self._downloader.add(*metadata_files)
 
         self._log.info(
             f"Downloading {self._downloader.queue_files_count} metadata files for"
             f" repository {self._repository}. Total size is"
-            f" {self._downloader.queue_files_size}"
+            f" {self._downloader.queue_files_formatted_size}"
         )
 
         await self._downloader.download()
 
         if self._downloader.has_errors() or self._downloader.has_missing():
             self._error = True
 
@@ -326,15 +373,15 @@
         )
 
         self._downloader.add(*pool_files)
 
         self._log.info(
             f"Downloading {self._downloader.queue_files_count} pool files for"
             f" repository {self._repository}. Total size is"
-            f" {self._downloader.queue_files_size}"
+            f" {self._downloader.queue_files_formatted_size}"
         )
 
         await self._downloader.download()
 
         if self._downloader.has_errors() or self._downloader.has_missing():
             self._error = True
 
@@ -430,14 +477,16 @@
                 mirror_parent_path,
             )
 
             # Drop dists.apt_mirror_old
             if mirror_parent_old_path.exists():
                 shutil.rmtree(mirror_parent_old_path)
 
+        self._log.info("Metadata moved")
+
     async def clean_repository(self, needed_files: set[Path], unlink: bool):
         cleaner = PathCleaner(
             self._config.mirror_path
             / self._repository.get_mirror_path(self._config.encode_tilde),
             needed_files | self._repository.skip_clean,
             wipe_size_ratio=self._config.wipe_size_ratio,
             wipe_count_ratio=self._config.wipe_count_ratio,
@@ -465,18 +514,28 @@
     async def clean_repository_skel(self, needed_files: set[Path]):
         self._log.info(f"Cleaning skel folder for repository {self._repository}")
 
         cleaner = PathCleaner(
             self._config.skel_path
             / self._repository.get_mirror_path(self._config.encode_tilde),
             needed_files,
+            logger_id=self._repository.url,
         )
 
         cleaner.clean()
 
+    def get_repository(self) -> BaseRepository:
+        return self._repository
+
+    def get_downloaded_files(self) -> list[DownloadFileCompressionVariant]:
+        return self._downloader.get_downloaded_files()
+
+    def get_unmodified_files(self) -> list[DownloadFileCompressionVariant]:
+        return self._downloader.get_unmodified_files()
+
 
 class APTMirror:
     LOCK_FILE = "apt-mirror.lock"
 
     def __init__(self, config: Config) -> None:
         self.stopped = False
 
@@ -489,66 +548,113 @@
 
         self._error: bool = False
 
         self._rate_limiter = None
         if self._config.limit_rate:
             self._rate_limiter = AsyncLimiter(self._config.limit_rate * 60, 60)
 
+        self._metrics_collector = DownloaderCollector(
+            self._config.prometheus_host, self._config.prometheus_port
+        )
+        if (
+            self._config.prometheus_enable
+            and not self._metrics_collector.prometheus_available()
+        ):
+            self._log.warning("Prometheus python client is not available")
+
     def on_stop(self):
         self.stopped = True
+        self._metrics_collector.shutdown()
         asyncio.get_running_loop().stop()
 
     async def run(self) -> int:
         self._log.info(f"apt-mirror2 version {__version__}")
         signal.signal(signal.SIGTERM, lambda _, __: self.on_stop())
 
         if not self._config.repositories:
             self._log.error("No repositories are found in the configuration")
             return 2
 
         self.lock()
 
         tasks: list[Awaitable[bool]] = []
+        mirrors: list[RepositoryMirror] = []
         for repository in self._config.repositories.values():
             mirror = RepositoryMirror(
                 repository,
                 self._config,
                 self._semaphore,
                 self._download_semaphore,
                 self._rate_limiter,
+                self._metrics_collector,
             )
             tasks.append(asyncio.create_task(mirror.mirror()))
+            mirrors.append(mirror)
 
         self._error = not all(await asyncio.gather(*tasks))
 
         if not self._config.autoclean and any(
             r.clean for r in self._config.repositories.values()
         ):
             self._log.info(f"Writing clean script {self._config.cleanscript}")
             with open(self._config.cleanscript, "wt", encoding="utf-8") as fp:
                 fp.write(
-                    "\n".join([
-                        "#!/bin/sh",
-                        "set -e",
-                        "",
-                    ])
+                    "\n".join(
+                        [
+                            "#!/bin/sh",
+                            "set -e",
+                            "",
+                        ]
+                    )
                 )
 
                 for repository in self._config.repositories.values():
                     if not repository.clean:
                         continue
 
                     clean_script = (
                         self._config.cleanscript.parent
                         / repository.get_clean_script_name(self._config.encode_tilde)
                     )
                     fp.write(f"sh '{clean_script}'\n")
 
             self._config.cleanscript.chmod(0o750)
 
+        if self._config.write_file_lists:
+            with ExitStack() as stack:
+                fp_all = stack.enter_context(
+                    open(self._config.var_path / "ALL", "wt", encoding="utf-8")
+                )
+                fp_new = stack.enter_context(
+                    open(self._config.var_path / "NEW", "wt", encoding="utf-8")
+                )
+
+                fp_hash_types: dict[HashType, IO[str]] = {}
+                for hash_type in HashType:
+                    fp_hash_types[hash_type] = stack.enter_context(
+                        open(
+                            self._config.var_path / hash_type.name,
+                            "wt",
+                            encoding="utf-8",
+                        )
+                    )
+
+                for mirror in mirrors:
+                    for download_variant in mirror.get_downloaded_files():
+                        fp_all.write(f"{download_variant.path}{os.linesep}")
+                        fp_new.write(
+                            mirror.get_repository().url.for_path(download_variant.path)
+                            + os.linesep
+                        )
+
+                        self._write_hashsums(fp_hash_types, download_variant)
+
+                    for download_variant in mirror.get_unmodified_files():
+                        self._write_hashsums(fp_hash_types, download_variant)
+
         if self._config.run_postmirror:
             if not self._config.postmirror_script.is_file():
                 self._log.error(
                     f"Post Mirror script is missing: {self._config.postmirror_script}"
                 )
             else:
                 self._log.info(
@@ -568,14 +674,16 @@
                 await process.wait()
 
                 self._log.info(
                     "Post Mirror script has completed. See above output for any"
                     " possible errors."
                 )
 
+        self._metrics_collector.shutdown()
+
         self.unlock()
 
         if self._error:
             self._log.error(
                 "Some files were not downloaded. Please check logs above for details."
             )
             return 1
@@ -606,14 +714,24 @@
     def unlock(self):
         if self._lock_fd:
             self._lock_fd.close()
             self._lock_fd = None
 
             self.get_lock_file().unlink(missing_ok=True)
 
+    def _write_hashsums(
+        self,
+        fp_hash_types: dict[HashType, IO[str]],
+        download_variant: DownloadFileCompressionVariant,
+    ):
+        for hashsum in download_variant.hashes.values():
+            fp_hash_types[hashsum.type].write(
+                f"{hashsum.hash}  {download_variant.path}{os.linesep}"
+            )
+
 
 def get_config_file() -> Path:
     parser = argparse.ArgumentParser()
     parser.add_argument("--version", action="store_true", help="Show version")
     parser.add_argument(
         "configfile",
         help=f"Path to config file. Default {Config.DEFAULT_CONFIGFILE}",
```

### Comparing `apt-mirror-3/apt_mirror/config.py` & `apt-mirror-4/apt_mirror/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,14 +236,15 @@
             "nthreads": "20",
             "uvloop": "1",
             "base_path": "/var/spool/apt-mirror",
             "mirror_path": "$base_path/mirror",
             "skel_path": "$base_path/skel",
             "var_path": "$base_path/var",
             "cleanscript": "$var_path/clean.sh",
+            "write_file_lists": "off",
             "run_postmirror": "0",
             "postmirror_script": "$var_path/postmirror.sh",
             "_contents": "1",
             "_autoclean": "0",
             "wipe_size_ratio": "0.4",
             "wipe_count_ratio": "0.4",
             "_tilde": "0",
@@ -255,14 +256,17 @@
             "proxy_user": "",
             "proxy_password": "",
             "http_user_agent": f"apt-mirror2/{__version__}",
             "no_check_certificate": "0",
             "certificate": "",
             "private_key": "",
             "ca_certificate": "",
+            "prometheus_enable": "off",
+            "prometheus_host": "localhost",
+            "prometheus_port": "8000",
         }
 
         self._parse_config_file()
         self._substitute_variables()
 
     def _parse_config_file(self):
         clean: list[str] = []
@@ -392,19 +396,20 @@
     def create_working_directories(self):
         for variable in ("mirror_path", "base_path", "var_path"):
             path = Path(self[variable])
             path.mkdir(parents=True, exist_ok=True)
 
     def init_log_files(self):
         LoggerFactory.add_log_file(None, self.var_path / "apt-mirror2.log")
-        for repository_url, repository in self.repositories.items():
+        for repository in self.repositories.values():
             log_name = repository.as_filename(self.encode_tilde)
-            LoggerFactory.add_log_file(
-                repository_url, self.var_path / f"{log_name}.log"
-            )
+            self._add_url_log_file(repository.url, self.var_path / f"{log_name}.log")
+
+    def _add_url_log_file(self, repository_url: URL, log_file: Path):
+        LoggerFactory.add_log_file(repository_url, log_file)
 
     def get_bool(self, key: str) -> bool:
         return bool(self[key]) and self[key].lower() not in ("0", "off", "no")
 
     def get_path(self, key: str) -> Path:
         return Path(self[key])
 
@@ -491,14 +496,18 @@
         return self.get_path("postmirror_script")
 
     @property
     def repositories(self):
         return self._repositories.copy()
 
     @property
+    def write_file_lists(self):
+        return self.get_bool("write_file_lists")
+
+    @property
     def run_postmirror(self):
         return self.get_bool("run_postmirror")
 
     @property
     def skel_path(self) -> Path:
         return self.get_path("skel_path")
 
@@ -519,7 +528,19 @@
             username=self._variables.get("proxy_user"),
             password=self._variables.get("proxy_password"),
         )
 
     @property
     def user_agent(self) -> str:
         return self["http_user_agent"]
+
+    @property
+    def prometheus_enable(self) -> bool:
+        return self.get_bool("prometheus_enable")
+
+    @property
+    def prometheus_host(self) -> str:
+        return self["prometheus_host"]
+
+    @property
+    def prometheus_port(self) -> int:
+        return int(self["prometheus_port"])
```

### Comparing `apt-mirror-3/apt_mirror/logs.py` & `apt-mirror-4/apt_mirror/logs.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-3/apt_mirror/repository.py` & `apt-mirror-4/apt_mirror/repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 import os
 import shutil
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from mmap import MADV_SEQUENTIAL, MAP_POPULATE, MAP_PRIVATE, mmap
 from pathlib import Path
-from typing import IO, Iterable, Sequence
+from typing import IO, Any, Iterable, Sequence
 
 from debian.deb822 import Release
 
 from .download import URL, DownloadFile, FileCompression, HashSum, HashType
 from .logs import LoggerFactory
 
 
 def should_ignore_errors(ignored_paths: set[str], path: Path):
     return any(path.is_relative_to(ignored_path) for ignored_path in ignored_paths)
 
 
+class InvalidReleaseFilesException(RuntimeError):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+        self.message = message
+
+
 @dataclass
 class PackageFile:
     path: Path
     size: int
     hashes: dict[HashType, HashSum]
 
     def to_download_file(self, directory: str):
@@ -43,19 +49,23 @@
             )
 
         return download_file
 
 
 class IndexFileParser(ABC):
     def __init__(
-        self, repository_path: Path, index_files: set[Path], ignore_errors: set[str]
+        self,
+        repository_path: Path,
+        index_files: set[Path],
+        ignore_errors: set[str],
+        logger_id: Any | None = None,
     ) -> None:
         super().__init__()
 
-        self._log = LoggerFactory.get_logger(self)
+        self._log = LoggerFactory.get_logger(self, logger_id=logger_id)
         self._repository_path = repository_path
         self._index_files = index_files
         self._ignore_errors = ignore_errors
         self._pool_files: dict[Path, DownloadFile] = {}
 
     def parse(self) -> set[DownloadFile]:
         for index_file_relative_path in self._index_files:
@@ -76,19 +86,17 @@
                 mfp = fp
                 if index_file_size > 1 * 1024 * 1024:
                     mfp = mmap(
                         fp.fileno(),
                         length=0,
                         flags=MAP_PRIVATE | MAP_POPULATE,
                     )
+                    mfp.madvise(MADV_SEQUENTIAL)
 
                 try:
-                    if isinstance(mfp, mmap):
-                        mfp.madvise(MADV_SEQUENTIAL)
-
                     self._do_parse_index(mfp)
                 finally:
                     if isinstance(mfp, mmap):
                         mfp.close()
 
         return set(self._pool_files.values())
 
@@ -115,17 +123,23 @@
 
     @abstractmethod
     def _do_parse_index(self, fp: IO[bytes] | mmap): ...
 
 
 class SourcesParser(IndexFileParser):
     def __init__(
-        self, repository_path: Path, index_files: set[Path], ignore_errors: set[str]
+        self,
+        repository_path: Path,
+        index_files: set[Path],
+        ignore_errors: set[str],
+        logger_id: Any | None = None,
     ) -> None:
-        super().__init__(repository_path, index_files, ignore_errors)
+        super().__init__(
+            repository_path, index_files, ignore_errors, logger_id=logger_id
+        )
         self._reset_block_parser()
 
     # https://github.com/pylint-dev/pylint/issues/5214
     def _reset_block_parser(self):
         self._directory: str | None = None
         self._hash_type = None
         self._package_files: dict[Path, PackageFile] = {}
@@ -194,17 +208,23 @@
                     self._pool_files[download_file.path] = download_file
 
                 self._reset_block_parser()
 
 
 class PackagesParser(IndexFileParser):
     def __init__(
-        self, repository_path: Path, index_files: set[Path], ignore_errors: set[str]
+        self,
+        repository_path: Path,
+        index_files: set[Path],
+        ignore_errors: set[str],
+        logger_id: Any | None = None,
     ) -> None:
-        super().__init__(repository_path, index_files, ignore_errors)
+        super().__init__(
+            repository_path, index_files, ignore_errors, logger_id=logger_id
+        )
         self._reset_block_parser()
 
     def _reset_block_parser(self):
         self._file_path = None
         self._size = 0
         self._hashes: dict[HashType, HashSum] = {}
 
@@ -275,15 +295,15 @@
 
     @staticmethod
     def default():
         return ByHash.YES
 
 
 @dataclass
-class BaseRepositoryMetadata:
+class BaseRepositoryMetadata(ABC):
     by_hash: ByHash
 
     @abstractmethod
     def as_path(self) -> Path: ...
 
     def as_string(self) -> str:
         return str(self)
@@ -471,28 +491,99 @@
 
         if self.is_source_enabled:
             pool_files.update(
                 SourcesParser(
                     repository_root / self.get_mirror_path(encode_tilde),
                     set(self.sources_files) - missing_sources,
                     ignore_errors=self.ignore_errors,
+                    logger_id=self.url,
                 ).parse()
             )
 
         if self.is_binaries_enabled:
             pool_files.update(
                 PackagesParser(
                     repository_root / self.get_mirror_path(encode_tilde),
                     set(self.packages_files) - missing_sources,
                     ignore_errors=self.ignore_errors,
+                    logger_id=self.url,
                 ).parse()
             )
 
         return pool_files
 
+    def validate_release_files(self, repository_root: Path, encode_tilde: bool):
+        release_files_exists = False
+
+        for _, metadata_release_files in self.release_files_per_metadata.items():
+            metadata_sizes: dict[str, list[tuple[int, Path]]] = {}
+            metadata_hashes: dict[str, dict[HashType, list[tuple[str, Path]]]] = {}
+
+            for release_file_relative_path in metadata_release_files:
+                if release_file_relative_path.suffix == ".gpg":
+                    continue
+
+                release_file = (
+                    repository_root
+                    / self.get_mirror_path(encode_tilde)
+                    / release_file_relative_path
+                )
+
+                if not release_file.exists():
+                    continue
+
+                with open(release_file, "rt", encoding="utf-8") as fp:
+                    release = Release(fp)
+
+                release_files_exists = True
+                for hash_type in HashType:
+                    for file in release.get(hash_type.value, []):
+                        try:
+                            size = int(file["size"])
+                        except ValueError:
+                            size = 0
+
+                        if size <= 0:
+                            continue
+
+                        # Ignore release files in release files
+                        if file["name"] in self.RELEASE_FILES:
+                            continue
+
+                        path = file["name"]
+                        hash_sum = file[hash_type.value]
+
+                        if any(size != s[0] for s in metadata_sizes.get(path, [])):
+                            raise InvalidReleaseFilesException(
+                                f"Size of file {path} in release file"
+                                f" {release_file_relative_path} differs from size in"
+                                f" release file {metadata_sizes[path][0][1]}"
+                            )
+
+                        if any(
+                            hash_sum != s[0]
+                            for s in metadata_hashes.get(path, {}).get(hash_type, [])
+                        ):
+                            raise InvalidReleaseFilesException(
+                                f"Hashsum of type {hash_type} of file {path} in release"
+                                f" file {release_file_relative_path} differs from"
+                                " hashsum in release file"
+                                f" {metadata_hashes[path][hash_type][0][1]}"
+                            )
+
+                        metadata_sizes.setdefault(path, []).append(
+                            (size, release_file_relative_path)
+                        )
+                        metadata_hashes.setdefault(path, {}).setdefault(
+                            hash_type, []
+                        ).append((hash_sum, release_file_relative_path))
+
+        if not release_files_exists:
+            raise InvalidReleaseFilesException("No release files were found")
+
     @property
     def release_files(self) -> Sequence[Path]:
         return [
             path
             for _, paths in self.release_files_per_metadata.items()
             for path in paths
         ]
```

### Comparing `apt-mirror-3/apt_mirror.egg-info/PKG-INFO` & `apt-mirror-4/apt_mirror.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apt-mirror
-Version: 3
+Version: 4
 Summary: apt-mirror Python reimplementation
 Author-email: Yuri Konotopov <ykonotopov@gnome.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,20 +693,22 @@
 License-File: LICENSE
 Requires-Dist: aiofile==3.8.8
 Requires-Dist: aiolimiter==1.1.0
 Requires-Dist: aioftp==0.21.4
 Requires-Dist: httpx[http2]==0.26.0
 Requires-Dist: python-debian==0.1.49
 Provides-Extra: dev
-Requires-Dist: black==23.11.0; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: pip-tools==7.0.0; extra == "dev"
 Requires-Dist: pylint==3.0.3; extra == "dev"
 Requires-Dist: pytest==7.4.4; extra == "dev"
+Provides-Extra: prometheus
+Requires-Dist: prometheus-client==0.20.0; extra == "prometheus"
 Provides-Extra: uvloop
 Requires-Dist: uvloop==0.19.0; extra == "uvloop"
 
 # apt-mirror2
 
 [`apt-mirror2`](https://gitlab.com/apt-mirror2/apt-mirror2) is the Python/asyncio reimplementation of the
 [apt-mirror](https://github.com/apt-mirror/apt-mirror) developed as drop-in replacement for the latest.  
@@ -777,24 +779,31 @@
 ```
 
 # apt-mirror configuration compatibility
 
 Most of `apt-mirror` configuration directives are supported.  
 As of now proxy for FTP repositories is not supported.  
 
+File lists (ALL, NEW, MD5, SHA256, SHA512) are not written by default, but you can enable them with the `write_file_lists` option.
+
 In addition there are some enhancements available:
 
 - Repositories without MD5 hashsums are correctly mirrored
 - Old index files are properly cleaned and don't produces errors in mirror processing
 - Standard source.list `[ arch=arch1,arch2 ]` can be used to specify multiple repository architectures for mirroring.
+- multiple codenames (or flat folders) can be specified using comma as delimiter.
 - `mirror_path URL PATH` option may be used to specify `PATH` to use for saving mirror files instead of path that is generated from `URL`.
 - Additional configuration is loaded from the `*.list` files in the directory named same as `configfile` with the `.d` suffix. Eg `/etc/apt/mirror.list.d/*.list`.
 - Rate limit is enforced for overall download rate.
 - Non-zero exit code is returned if some of required files were not downloaded due to network or server errors or
   no repositories were configured.
 - HTTP user agent can be configured via `user_agent` configuration.
 - Configuration variables are exposed to postmirror_script.
 - `by-hash` list option can be used to control whether `Acquire-By-Hash` Release option should be respected or enforced.
+- mirror wipe protection is available and configurable via `wipe_size_ratio` and `wipe_count_ratio` settings.
+- per-repository log files are available in the `var_path` folder
+- `dists` folder is almost atomicaly replaced using move instead of copy/link
+- native Prometheus metrics are supported
 
 # License
 
 GNU General Public License v3.0 or later
```

### Comparing `apt-mirror-3/pyproject.toml` & `apt-mirror-4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apt-mirror"
-version = "3"
+version = "4"
 authors = [
     {name = "Yuri Konotopov", email = "ykonotopov@gnome.org"},
 ]
 description = "apt-mirror Python reimplementation"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["apt", "debian"]
@@ -25,21 +25,24 @@
     "aioftp==0.21.4",
     "httpx[http2]==0.26.0",
     "python-debian==0.1.49",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "black==23.11.0",
+    "black==24.3.0",
     "flake8==6.0.0",
     "isort==5.12.0",
     "pip-tools==7.0.0",
     "pylint==3.0.3",
     "pytest==7.4.4",
 ]
+prometheus = [
+    "prometheus-client==0.20.0"
+]
 uvloop = [
     "uvloop==0.19.0",
 ]
 
 [project.scripts]
 apt-mirror = "apt_mirror.apt_mirror:main"
 
@@ -47,18 +50,19 @@
 Homepage = "https://gitlab.com/apt-mirror2/apt-mirror2/"
 Repository = "https://gitlab.com/apt-mirror2/apt-mirror2.git"
 Github = "https://github.com/nE0sIghT/apt-mirror2.git"
 Issues = "https://gitlab.com/apt-mirror2/apt-mirror2/-/issues"
 Changelog = "https://gitlab.com/apt-mirror2/apt-mirror2/-/commits/master/"
 
 [tool.setuptools.packages.find]
-include = ["apt_mirror"]
+include = ["apt_mirror*"]
 
 [tool.black]
 preview = true
+enable-unstable-feature = ["string_processing"]
 
 [tool.isort]
 profile = "black"
 default_section = "THIRDPARTY"
 known_first_party = "apt_mirror"
 
 [tool.pylint.main]
```

### Comparing `apt-mirror-3/tests/test_clean.py` & `apt-mirror-4/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-3/tests/test_config.py` & `apt-mirror-4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-3/tests/test_repository.py` & `apt-mirror-4/tests/test_repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,56 @@
 from pathlib import Path
 from typing import Iterable
 
 from apt_mirror.download import DownloadFile
+from apt_mirror.download.url import URL
+from apt_mirror.repository import (
+    ByHash,
+    Codename,
+    InvalidReleaseFilesException,
+    Repository,
+)
 from tests.base import BaseTest
 
 
 class TestRepository(BaseTest):
     @staticmethod
     def get_from_set(collection: Iterable[DownloadFile], element: Path) -> DownloadFile:
         for e in collection:
             if hash(e) == hash(element):
                 return e
 
         raise RuntimeError(f"No element {element} found in set {collection}")
 
+    def get_repository(self):
+        components = ["main", "contrib", "non-free"]
+
+        return Repository(
+            url=URL.from_string("http://localhost.local/repo"),
+            clean=False,
+            skip_clean=set(),
+            mirror_path=Path("repo"),
+            ignore_errors=set(),
+            codenames=Repository.Codenames(
+                [
+                    (
+                        "test",
+                        Codename(
+                            ByHash.default(),
+                            "test",
+                            {
+                                component: Codename.Component("main", True, ["amd64"])
+                                for component in components
+                            },
+                        ),
+                    )
+                ]
+            ),
+        )
+
     def test_ignore_errors(self):
         config = self.get_config("IgnoreErrorsConfig")
 
         repository = self.ensure_repository(
             config.repositories[
                 "https://packages.gitlab.com/runner/gitlab-runner/debian"
             ]
@@ -41,7 +74,22 @@
         )
         self.assertFalse(file.ignore_errors)
 
         repository = self.ensure_repository(
             config.repositories["http://ftp.debian.org/debian-security"]
         )
         self.assertFalse(repository.ignore_errors)
+
+    def test_release_files(self):
+        repository = self.get_repository()
+
+        with self.assertRaises(InvalidReleaseFilesException):
+            repository.validate_release_files(
+                self.TEST_DATA / "UnsyncedReleaseFiles", False
+            )
+
+        repository.validate_release_files(self.TEST_DATA / "SyncedReleaseFiles", False)
+
+        with self.assertRaises(InvalidReleaseFilesException):
+            repository.validate_release_files(
+                self.TEST_DATA / "NonExistingFolder", False
+            )
```

