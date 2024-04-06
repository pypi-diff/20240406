# Comparing `tmp/pyfilebrowser-0.0.8-py3-none-any.whl.zip` & `tmp/pyfilebrowser-0.0.9b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 17046 bytes, number of entries: 14
--rw-r--r--  2.0 unx      105 b- defN 24-Apr-05 10:09 pyfilebrowser/__init__.py
--rw-r--r--  2.0 unx     8736 b- defN 24-Apr-05 10:09 pyfilebrowser/main.py
--rw-r--r--  2.0 unx       89 b- defN 24-Apr-05 10:09 pyfilebrowser/requirements.txt
--rw-r--r--  2.0 unx     5452 b- defN 24-Apr-05 10:09 pyfilebrowser/modals/config.py
--rw-r--r--  2.0 unx     1765 b- defN 24-Apr-05 10:09 pyfilebrowser/modals/models.py
--rw-r--r--  2.0 unx     1603 b- defN 24-Apr-05 10:09 pyfilebrowser/modals/users.py
--rw-r--r--  2.0 unx    10178 b- defN 24-Apr-05 10:09 pyfilebrowser/squire/download.py
--rw-r--r--  2.0 unx     4525 b- defN 24-Apr-05 10:09 pyfilebrowser/squire/steward.py
--rw-r--r--  2.0 unx     3056 b- defN 24-Apr-05 10:09 pyfilebrowser/squire/struct.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     8354 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1185 b- defN 24-Apr-05 10:09 pyfilebrowser-0.0.8.dist-info/RECORD
-14 files, 46222 bytes uncompressed, 15066 bytes compressed:  67.4%
+Zip file size: 17167 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-06 16:56 pyfilebrowser/__init__.py
+-rw-r--r--  2.0 unx     8656 b- defN 24-Apr-05 10:33 pyfilebrowser/main.py
+-rw-r--r--  2.0 unx       89 b- defN 24-Mar-31 04:11 pyfilebrowser/requirements.txt
+-rw-r--r--  2.0 unx     5452 b- defN 24-Mar-31 04:11 pyfilebrowser/modals/config.py
+-rw-r--r--  2.0 unx     1765 b- defN 24-Mar-27 22:22 pyfilebrowser/modals/models.py
+-rw-r--r--  2.0 unx     1603 b- defN 24-Mar-27 22:22 pyfilebrowser/modals/users.py
+-rw-r--r--  2.0 unx    10178 b- defN 24-Apr-05 10:58 pyfilebrowser/squire/download.py
+-rw-r--r--  2.0 unx     4525 b- defN 24-Apr-03 01:54 pyfilebrowser/squire/steward.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-Mar-31 04:11 pyfilebrowser/squire/struct.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8493 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1195 b- defN 24-Apr-06 16:57 pyfilebrowser-0.0.9b0.dist-info/RECORD
+14 files, 46296 bytes uncompressed, 15167 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pyfilebrowser/squire/steward.py
 Comment: 
 
 Filename: pyfilebrowser/squire/struct.py
 Comment: 
 
-Filename: pyfilebrowser-0.0.8.dist-info/LICENSE
+Filename: pyfilebrowser-0.0.9b0.dist-info/LICENSE
 Comment: 
 
-Filename: pyfilebrowser-0.0.8.dist-info/METADATA
+Filename: pyfilebrowser-0.0.9b0.dist-info/METADATA
 Comment: 
 
-Filename: pyfilebrowser-0.0.8.dist-info/WHEEL
+Filename: pyfilebrowser-0.0.9b0.dist-info/WHEEL
 Comment: 
 
-Filename: pyfilebrowser-0.0.8.dist-info/top_level.txt
+Filename: pyfilebrowser-0.0.9b0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyfilebrowser-0.0.8.dist-info/RECORD
+Filename: pyfilebrowser-0.0.9b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyfilebrowser/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Module for packaging."""
 
 from pyfilebrowser.main import FileBrowser  # noqa: F401
 
-version = "0.0.8"
+version = "0.0.9-beta"
```

## pyfilebrowser/main.py

```diff
@@ -20,24 +20,28 @@
     """
 
     def __init__(self, **kwargs):
         """Instantiates the object.
 
         Keyword Args:
             logger: Bring your own logger.
+            proxy: Boolean flag to enable proxy.
         """
         self.env = steward.EnvConfig(**kwargs)
         # Reset to stdout, so the log output stream can be controlled with custom logging
         self.env.config_settings.server.log = models.Log.stdout
         self.logger = kwargs.get('logger',
                                  steward.default_logger(self.env.config_settings.server.log == models.Log.file))
         github = download.GitHub(**kwargs)
         if not os.path.isfile(download.executable.filebrowser_bin):
             download.binary(logger=self.logger, github=github)
         self.proxy_engine: multiprocessing.Process | None = None
+        self.proxy = kwargs.get('proxy')
+        assert self.proxy is None or isinstance(self.proxy, bool), \
+            f"\n\tproxy flag should be a boolean value, received {type(self.proxy).__name__!r}"
 
     def exit_process(self) -> None:
         """Deletes the database file, and all the subtitles that were created by this application."""
         if os.path.isfile(download.executable.filebrowser_db):
             self.logger.info("Removing database %s", download.executable.filebrowser_db)
             os.remove(download.executable.filebrowser_db)
         if self.proxy_engine:
@@ -112,40 +116,32 @@
             user_settings.update(model_settings)  # insert cleaned 'model_settings' into new dict 'user_settings'
             final_settings.append(user_settings)
         with open(steward.fileio.users, 'w') as file:
             json.dump(final_settings, file, indent=4)
             file.flush()
         return auth_map
 
-    def create_config(self, proxy: bool) -> None:
-        """Creates the JSON file for configuration.
-
-        Args:
-            proxy: Boolean flag to enable proxy.
-        """
-        if proxy:
+    def create_config(self) -> None:
+        """Creates the JSON file for configuration."""
+        if self.proxy:
             self.env.config_settings.settings.authMethod = "json"
             self.env.config_settings.settings.authHeader = ""
         if str(self.env.config_settings.settings.branding.files) == ".":
             self.env.config_settings.settings.branding.files = ""
         self.env.config_settings.server.port = str(self.env.config_settings.server.port)
         with warnings.catch_warnings(action="ignore"):
             final_settings = steward.remove_trailing_underscore(json.loads(self.env.config_settings.model_dump_json()))
         with open(steward.fileio.config, 'w') as file:
             json.dump(final_settings, file, indent=4)
             file.flush()
 
-    def import_config(self, proxy: bool) -> None:
-        """Imports the configuration file into filebrowser.
-
-        Args:
-            proxy: Boolean flag to enable proxy.
-        """
+    def import_config(self) -> None:
+        """Imports the configuration file into filebrowser."""
         self.logger.info("Importing configuration from %s", steward.fileio.config)
-        self.create_config(proxy)
+        self.create_config()
         assert os.path.isfile(steward.fileio.config), f"{steward.fileio.config!r} doesn't exist"
         self.run_subprocess(["config", "import", steward.fileio.config],
                             "Failed to import configuration")
 
     def import_users(self) -> Dict[str, str]:
         """Imports the user profiles into filebrowser.
 
@@ -156,39 +152,34 @@
         self.logger.info("Importing user profiles from %s", steward.fileio.users)
         auth_map = self.create_users()
         assert os.path.isfile(steward.fileio.users), f"{steward.fileio.users!r} doesn't exist"
         self.run_subprocess(["users", "import", steward.fileio.users],
                             "Failed to import user profiles")
         return auth_map
 
-    def background_tasks(self, auth_map: Dict[str, str], proxy: bool) -> None:
+    def background_tasks(self, auth_map: Dict[str, str]) -> None:
         """Initiates the proxy engine and subtitles' format conversion as background tasks.
 
         Args:
             auth_map: Authentication map provided as environment variables.
-            proxy: Boolean flag to enable proxy.
         """
-        if proxy:
+        if self.proxy:
             assert proxy_settings.port != int(self.env.config_settings.server.port), \
                 f"\n\tProxy server can't run on the same port [{proxy_settings.port}] as the server!!"
             log_config = struct.LoggerConfig(self.logger).get()
             if proxy_settings.debug:
                 log_config = struct.update_log_level(log_config, logging.DEBUG)
             # noinspection HttpUrlsUsage
             self.proxy_engine = multiprocessing.Process(
                 target=proxy_server, daemon=True,
                 args=(f"http://{self.env.config_settings.server.address}:{self.env.config_settings.server.port}",
                       log_config, auth_map)
             )
             self.proxy_engine.start()
 
-    def start(self, proxy: bool = False) -> None:
-        """Handler for all the functions above.
-
-        Args:
-            proxy: Boolean flag to enable proxy.
-        """
+    def start(self) -> None:
+        """Handler for all the functions above."""
         if os.path.isfile(download.executable.filebrowser_db):
             os.remove(download.executable.filebrowser_db)
-        self.import_config(proxy)
-        self.background_tasks(self.import_users(), proxy)
+        self.import_config()
+        self.background_tasks(self.import_users())
         self.run_subprocess([], "Failed to run the server", True)
```

## Comparing `pyfilebrowser-0.0.8.dist-info/LICENSE` & `pyfilebrowser-0.0.9b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyfilebrowser-0.0.8.dist-info/METADATA` & `pyfilebrowser-0.0.9b0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilebrowser
-Version: 0.0.8
+Version: 0.0.9b0
 Summary: Python module designed to streamline interactions with filebrowser
 Author-email: Vignesh Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Vignesh Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -95,25 +95,26 @@
 python -m pip install pyfilebrowser
 ```
 
 **Initiate**
 ```python
 import pyfilebrowser
 
-
 if __name__ == '__main__':
     browser = pyfilebrowser.FileBrowser()
+    # browser.proxy = True  # [Optional] Enables proxy server to run in parallel
     browser.start()
 ```
 
 ## Environment Variables
 Env vars can either be loaded from `.env` files or directly passed during object init.
 
 #### `.env` files
 
+- `.proxy.env` - Loads the proxy server's configuration.
 - `.config.env` - Loads the server's default configuration. Reference: [config]
 - `.user*.env` - Loads each user's profile specific configuration. Reference: [users]
 
 Multiple user profiles can be loaded using `.user1.env`, `.user2.env` and so on.<br>
 User profile's permissions are automatically set based on the `admin` flag.
 
 Refer [samples] directory for sample `.env` files. For nested configuration settings, refer the [runbook]
```

## Comparing `pyfilebrowser-0.0.8.dist-info/RECORD` & `pyfilebrowser-0.0.9b0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pyfilebrowser/__init__.py,sha256=J6Tuo-HN2MdoRA3ykq-f7jKbtoB8f41wFmp5FLKTFkU,105
-pyfilebrowser/main.py,sha256=Xmguv0jTcDLfDnYFctk82LXNwIozscezSU0z-xLxCUs,8736
+pyfilebrowser/__init__.py,sha256=Uu3IuPmX3NJtM2scQAqxqousy7cbzW1Q71vtLgsg044,110
+pyfilebrowser/main.py,sha256=QDkl11k7BY__8DAf8jjlIqkfzBC3fTWByrV1E_6P2gU,8656
 pyfilebrowser/requirements.txt,sha256=iqRgXyC9MTSdgB8LD5yJDMfc7c5Zmuf82M2AqTakh1w,89
 pyfilebrowser/modals/config.py,sha256=nMRWu1esluHosN3wUw3w5EooubJuBTzpxIoHWcDZB6M,5452
 pyfilebrowser/modals/models.py,sha256=1RVSZaNgWChLv8c0-zMXgSpLDonitMgrc9fYvlzEs3U,1765
 pyfilebrowser/modals/users.py,sha256=xKdpMrcbWTza2llFTRPkKJG3ySEVlvC03rSMA4KgK5s,1603
 pyfilebrowser/squire/download.py,sha256=FI_1GZrjcTtYBE3bXOSa4f-FSgjU9ejANW-NdEZq2KQ,10178
 pyfilebrowser/squire/steward.py,sha256=hVoWBrJWa2HSvR56JKnk_vXh0Qm0jPbEGwQ4dWtpXM8,4525
 pyfilebrowser/squire/struct.py,sha256=rg19tpW1iX17792uFWLQAhVZ2PLiHYETYc21GFulldE,3056
-pyfilebrowser-0.0.8.dist-info/LICENSE,sha256=xnHdLNCLt4RW3vtnE_TfN_cjViUHyIv0m8024fS4bws,1068
-pyfilebrowser-0.0.8.dist-info/METADATA,sha256=HhFlxavpr9gHo_b9rPiLDHXvEbokg3TrxRZJx9u0l1Q,8354
-pyfilebrowser-0.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyfilebrowser-0.0.8.dist-info/top_level.txt,sha256=RrwbvxqHTriDpUwaZC3F5o53eZtUKODCQQ0iRryM_Zo,14
-pyfilebrowser-0.0.8.dist-info/RECORD,,
+pyfilebrowser-0.0.9b0.dist-info/LICENSE,sha256=xnHdLNCLt4RW3vtnE_TfN_cjViUHyIv0m8024fS4bws,1068
+pyfilebrowser-0.0.9b0.dist-info/METADATA,sha256=hJ1d5qbuSczYUCkgFbOPKJ1gkTyZZYQXaNkaWOmvcCM,8493
+pyfilebrowser-0.0.9b0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyfilebrowser-0.0.9b0.dist-info/top_level.txt,sha256=RrwbvxqHTriDpUwaZC3F5o53eZtUKODCQQ0iRryM_Zo,14
+pyfilebrowser-0.0.9b0.dist-info/RECORD,,
```

