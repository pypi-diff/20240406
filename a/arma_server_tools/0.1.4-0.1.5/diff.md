# Comparing `tmp/arma_server_tools-0.1.4.tar.gz` & `tmp/arma_server_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arma_server_tools-0.1.4.tar", max compression
+gzip compressed data, was "arma_server_tools-0.1.5.tar", max compression
```

## Comparing `arma_server_tools-0.1.4.tar` & `arma_server_tools-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2021-11-17 01:13:43.000000 arma_server_tools-0.1.4/arma_server_tools/__init__.py
--rw-r--r--   0        0        0     7184 2021-11-26 13:09:04.955356 arma_server_tools-0.1.4/arma_server_tools/arma_server.py
--rw-r--r--   0        0        0      910 2021-11-17 01:13:43.000000 arma_server_tools-0.1.4/arma_server_tools/preset_parser.py
--rw-r--r--   0        0        0      958 2021-11-17 01:13:43.000000 arma_server_tools-0.1.4/arma_server_tools/server_config.py
--rw-r--r--   0        0        0     5084 2021-11-24 03:22:30.453049 arma_server_tools-0.1.4/arma_server_tools/workshop.py
--rw-r--r--   0        0        0     1015 2021-11-17 01:13:43.000000 arma_server_tools-0.1.4/arma_server_tools/yaml_tools.py
--rw-r--r--   0        0        0      537 2021-11-26 13:13:37.297934 arma_server_tools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      896 2021-11-26 13:56:32.528227 arma_server_tools-0.1.4/setup.py
--rw-r--r--   0        0        0      495 2021-11-26 13:56:32.529227 arma_server_tools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-04-06 17:26:09.068543 arma_server_tools-0.1.5/arma_server_tools/__init__.py
+-rw-r--r--   0        0        0     7124 2024-04-06 17:33:50.153762 arma_server_tools-0.1.5/arma_server_tools/arma_server.py
+-rw-r--r--   0        0        0     1999 2024-04-06 17:29:11.548569 arma_server_tools-0.1.5/arma_server_tools/preset_parser.py
+-rw-r--r--   0        0        0     2207 2024-04-06 17:30:13.639865 arma_server_tools-0.1.5/arma_server_tools/server_config.py
+-rw-r--r--   0        0        0     5474 2024-04-06 15:57:23.294204 arma_server_tools-0.1.5/arma_server_tools/server_config_fields.yaml
+-rw-r--r--   0        0        0     4821 2024-04-06 17:29:40.974766 arma_server_tools-0.1.5/arma_server_tools/workshop.py
+-rw-r--r--   0        0        0     1257 2024-04-06 17:29:34.958157 arma_server_tools-0.1.5/arma_server_tools/yaml_tools.py
+-rw-r--r--   0        0        0     1374 2024-04-06 17:39:56.883404 arma_server_tools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 arma_server_tools-0.1.5/PKG-INFO
```

### Comparing `arma_server_tools-0.1.4/arma_server_tools/arma_server.py` & `arma_server_tools-0.1.5/arma_server_tools/arma_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import os
 import re
-import shutil
 import subprocess
 
 import click
 import click_log
 import yaml
 
 logger = logging.getLogger(__name__)
@@ -19,106 +18,104 @@
 # https://docs.python.org/dev/distutils/apiref.html#distutils.dir_util.copy_tree
 
 # local install variables
 # ARMA_HOME = '/home/steam/.steam/steamcmd/arma3/'
 # ARMA_SERVER = os.path.join(ARMA_HOME, "arma3server")
 
 
-class LineConsumer():
+class LineConsumer:
 
     # https://regex101.com/
 
     # regex patterns collections
     omit_re = [
-        re.compile('^\d+:\d+:\d+ Updating base class.*'),
-        re.compile('^\d+:\d+:\d+ ==== Loaded addons ===='),
-        re.compile('^\d+:\d+:\d+\s[\/\w+\.]+\s-\s.*'),
-        re.compile('^\d+:\d+:\d+ =+'),
-        re.compile('^\d+:\d+:\d+ =+ List of mods =+'),
-        re.compile('^\d+:\d+:\d+ -+'),
-        re.compile('^\d+:\d+:\d+ +name.*fullPath'),
-        re.compile('^.*:Some of magazines weren\'t stored in soldier Vest or Uniform\?'),
-        re.compile('^.*: ?No geometry and no visual shape'),
-        re.compile('^\d+:\d+:\d+ Strange convex.*'),
-        re.compile('^\d+:\d+:\d+ ?Unsupported language.*'),
+        re.compile(r"^\d+:\d+:\d+ Updating base class.*"),
+        re.compile(r"^\d+:\d+:\d+ ==== Loaded addons ===="),
+        re.compile(r"^\d+:\d+:\d+\s[\/\w+\.]+\s-\s.*"),
+        re.compile(r"^\d+:\d+:\d+ =+"),
+        re.compile(r"^\d+:\d+:\d+ =+ List of mods =+"),
+        re.compile(r"^\d+:\d+:\d+ -+"),
+        re.compile(r"^\d+:\d+:\d+ +name.*fullPath"),
+        re.compile(r"^.*:Some of magazines weren\'t stored in soldier Vest or Uniform\?"),
+        re.compile(r"^.*: ?No geometry and no visual shape"),
+        re.compile(r"^\d+:\d+:\d+ Strange convex.*"),
+        re.compile(r"^\d+:\d+:\d+ ?Unsupported language.*"),
     ]
 
     warning_re = [
-        re.compile('^.* Warning:.*'),
-        re.compile('^.* Warning Message:.*'),
+        re.compile(r"^.* Warning:.*"),
+        re.compile(r"^.* Warning Message:.*"),
     ]
 
     green_re = [
-        re.compile('^\d+:\d+:\d+\sBattlEye Server:.*'),
-        re.compile('.* Connected to Steam servers'),
-        re.compile('^\d+:\d+:\d+ ? Roles assigned'),
-        re.compile('^\d+:\d+:\d+ ? Reading mission.*'),
-        re.compile('^\d+:\d+:\d+ ?Starting mission:'),
-        re.compile('^\d+:\d+:\d+ ? ? Mission file:.*'),
-        re.compile('^\d+:\d+:\d+ ? ? Mission world:.*'),
-        re.compile('^\d+:\d+:\d+ ? ? Mission directory:.*'),
+        re.compile(r"^\d+:\d+:\d+\sBattlEye Server:.*"),
+        re.compile(r".* Connected to Steam servers"),
+        re.compile(r"^\d+:\d+:\d+ ? Roles assigned"),
+        re.compile(r"^\d+:\d+:\d+ ? Reading mission.*"),
+        re.compile(r"^\d+:\d+:\d+ ?Starting mission:"),
+        re.compile(r"^\d+:\d+:\d+ ? ? Mission file:.*"),
+        re.compile(r"^\d+:\d+:\d+ ? ? Mission world:.*"),
+        re.compile(r"^\d+:\d+:\d+ ? ? Mission directory:.*"),
     ]
 
     extract_re = [
         re.compile(
-            "^\d+:\d+:\d+\s+"+
-            "(?P<name>[\w+\s\(\)-]+)\s+\|\s+"+
-            "(?P<modDir>[\w+\s]+)\s+\|\s+"+
-            "(?P<default>[\w+\s]+)\s+\|\s+"+
-            "(?P<official>[\w+\s]+)\s+\|\s+"+
-            "(?P<origin>[\w+\s]+)\s+\|\s+"+
-            "(?P<hash>[\w+\s]+)\s+\|\s+"+
-            "(?P<hashShort>[\w+\s]+)\s+\|\s+"+
-            "(?P<fullPath>[\w+\s\.\/]+)"
-
+            r"^\d+:\d+:\d+\s+"
+            + r"(?P<name>[\w+\s\(\)-]+)\s+\|\s+"
+            + r"(?P<modDir>[\w+\s]+)\s+\|\s+"
+            + r"(?P<default>[\w+\s]+)\s+\|\s+"
+            + r"(?P<official>[\w+\s]+)\s+\|\s+"
+            + r"(?P<origin>[\w+\s]+)\s+\|\s+"
+            + r"(?P<hash>[\w+\s]+)\s+\|\s+"
+            + r"(?P<hashShort>[\w+\s]+)\s+\|\s+"
+            + r"(?P<fullPath>[\w+\s\.\/]+)"
             # 14:21:06 Player dent connected (id=76561198017256167).
             # 14:09:27 Player dent disconnected.
-
         ),
     ]
 
     # 9:22:26 Initializing Steam server - Game Port: 2302, Steam Query Port: 2303
     # Arma 3 Console version 2.00.146766 x86 : port 2302
 
-    def is_omit(self, line):
+    def is_omit(self, line: str) -> bool:
 
         for item in self.omit_re:
             if item.match(line):
                 return True
         return False
 
-    def is_warning(self, line):
+    def is_warning(self, line: str) -> bool:
         for item in self.warning_re:
             if item.match(line):
                 return True
         return False
 
-    def is_green(self, line):
+    def is_green(self, line: str) -> bool:
         for item in self.green_re:
             if item.match(line):
                 return True
         return False
 
-    def extract(self, line):
+    def extract(self, line: str):
         for item in self.extract_re:
             results = item.match(line)
             if results:
                 return results
         return False
 
-    def parse(self, line):
+    def parse(self, line: str):
         if self.is_omit(line):
             return
 
         if self.is_warning(line):
-            click.secho(line, fg='red')
+            click.secho(line, fg="red")
             return
 
         if self.is_green(line):
-            click.secho(line, fg='green')
+            click.secho(line, fg="green")
             return
 
         # result = self.extract(line)
         # if result:
         #     # print(result.groupdict())
         #     return
 
@@ -139,108 +136,100 @@
 #         for line in iter(lambda: process.stdout.readline(), b''):
 #             cleaned = line.decode('utf-8').strip()
 #             consumer.parse(cleaned)
 #     except KeyboardInterrupt:
 #         print("~~~EXIT~~~")
 #     return success
 
-class ArmaServer():
+
+class ArmaServer:
 
     name = None
     config = None
     mods = None
     port = 2302
-    arma_home = '/home/steam/.steam/steamcmd/arma3/'
-    arma_config = '/home/steam/arma_configs'
+    arma_home = "/home/steam/.steam/steamcmd/arma3/"
+    arma_config = "/home/steam/arma_configs"
     arma_command = None
     # mods_folder = "mods"
 
     def parse_yaml(self, yaml_file):
-        with open(yaml_file, 'r') as stream:
+        with open(yaml_file, "r") as stream:
             try:
                 meta = yaml.safe_load(stream)
 
-                if 'name' in meta:
-                    self.name = meta['name']
+                if "name" in meta:
+                    self.name = meta["name"]
 
-                if 'config' in meta:
-                    self.config = os.path.join(
-                        self.arma_config, meta['config']
-                    )
+                if "config" in meta:
+                    self.config = os.path.join(self.arma_config, meta["config"])
 
-                if 'port' in meta:
-                    self.port = meta['port']
+                if "port" in meta:
+                    self.port = meta["port"]
 
-                if 'mods' in meta:
-                    self.mods = meta['mods']
+                if "mods" in meta:
+                    self.mods = meta["mods"]
 
             except yaml.YAMLError as exc:
                 print(exc)
 
     def generate_command(self):
         server_path = os.path.join(self.arma_home, "arma3server")
-        command = [server_path, ]
+        command = [
+            server_path,
+        ]
         if self.name:
             command.append(f'-name="{self.name}"')
 
-        command.append(f'-port={self.port}')
+        command.append(f"-port={self.port}")
 
         if self.config:
             command.append(f'-config="{self.config}"')
 
         if self.mods:
 
             # MOD="mods/@cba_a3;mods/@ace;"  # cannot handle cdlc content
 
             mods_list = []
             for m in self.mods:
                 # cannot handle cdlc content
                 # mods_list.append(f'{self.mods_folder}/@{m};')
-                mods_list.append(f'{m};')
+                mods_list.append(f"{m};")
 
             mods_string = "".join(mods_list)
-            command.append(f'-mods={mods_string}')
+            command.append(f"-mods={mods_string}")
         return command
 
     def serve(self):
         success = True
         arma_cmd = self.generate_command()
         try:
             consumer = LineConsumer()
-            process = subprocess.Popen(
-                arma_cmd,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.STDOUT,
-                cwd=self.arma_home
-            )
-            for line in iter(lambda: process.stdout.readline(), b''):
-                cleaned = line.decode('utf-8').strip()
+            process = subprocess.Popen(arma_cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=self.arma_home)
+            for line in iter(lambda: process.stdout.readline(), b""):
+                cleaned = line.decode("utf-8").strip()
                 consumer.parse(cleaned)
         except KeyboardInterrupt:
             print("~~~EXIT~~~")
         return success
 
 
-@click.option(
-    "--yaml",
-    "yaml_file",
-    help="path to yaml config file"
-)
+@click.option("--yaml", "yaml_file", help="path to yaml config file")
 @click.command()
 @click_log.simple_verbosity_option(logger)
 def main(yaml_file):
 
     if yaml_file:
         arma = ArmaServer()
         arma.parse_yaml(yaml_file)
         print(arma.name)
         print(arma.config)
         print(arma.port)
 
         logger.debug(arma.generate_command())
         arma.serve()
     else:
-        logger.error('yaml file is required')
+        logger.error("yaml file is required")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `arma_server_tools-0.1.4/arma_server_tools/workshop.py` & `arma_server_tools-0.1.5/arma_server_tools/workshop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,75 @@
 import logging
 import os
 import re
-import shutil
 import subprocess
 
 import click
 import click_log
-import yaml
 
 from .yaml_tools import home_config
 
 logger = logging.getLogger(__name__)
 click_log.basic_config(logger)
 
 
 class Workshop(object):
 
     # regex patterns collections
     omit_re = [
         re.compile("^.*type 'quit' to exit"),
-        re.compile('^Loading Steam API.*'),
-        re.compile('^.*Assertion Failed: Is64BitOS.*'),
+        re.compile("^Loading Steam API.*"),
+        re.compile("^.*Assertion Failed: Is64BitOS.*"),
         # re.compile(''),
     ]
 
     def __init__(self, item_id, item_name, is_examine, beta, betapassword):
         self.item_id = item_id
         self.item_name = item_name
         self.is_examine = is_examine
-        self.arma_config = home_config('arma_server.yaml')
-        self.beta = beta 
+        self.arma_config = home_config("arma_server.yaml")
+        self.beta = beta
         self.betapassword = betapassword
 
     def download(self):
-        click.secho(
-            f'Downloading item {self.item_id} : {self.item_name}',
-            fg='green'
-        )
+        click.secho(f"Downloading item {self.item_id} : {self.item_name}", fg="green")
         success = True
         steam_cmd = [
-            'steamcmd',
-            '+login',
-            self.arma_config['username'],
-            self.arma_config['password'],
-            '+workshop_download_item',
-            '107410',
+            "steamcmd",
+            "+login",
+            self.arma_config["username"],
+            self.arma_config["password"],
+            "+workshop_download_item",
+            "107410",
             self.item_id,
         ]
 
         if self.beta:
-            steam_cmd.append('-beta')
+            steam_cmd.append("-beta")
             steam_cmd.append(self.beta)
 
         if self.betapassword:
-            steam_cmd.append('-betapassword')
+            steam_cmd.append("-betapassword")
             steam_cmd.append(self.betapassword)
 
-        steam_cmd.append('validate')
-        steam_cmd.append('+quit')
-        
+        steam_cmd.append("validate")
+        steam_cmd.append("+quit")
 
         process = subprocess.Popen(
             steam_cmd,
             stdout=subprocess.PIPE,
         )
-        for line in iter(lambda: process.stdout.readline(), b''):
+        for line in iter(lambda: process.stdout.readline(), b""):
 
-            cleaned = line.decode('utf-8').strip()
-            if '...' in cleaned:
-                pieces = cleaned.split('...')
+            cleaned = line.decode("utf-8").strip()
+            if "..." in cleaned:
+                pieces = cleaned.split("...")
                 click.echo(pieces[0])
             elif "ERROR" in cleaned:
-                click.secho(cleaned, fg='red')
+                click.secho(cleaned, fg="red")
                 success = False
             elif not self.is_omit(cleaned):
                 click.echo(cleaned)
 
         return success
 
     def is_omit(self, line):
@@ -83,75 +77,57 @@
         for item in self.omit_re:
             if item.match(line):
                 return True
         return False
 
     def examine(self):
         src = os.path.join(
-            self.arma_config['workshop'],
+            self.arma_config["workshop"],
             self.item_id,
         )
         dst = os.path.join(
-            self.arma_config['arma_home'],
-            'mods',
+            self.arma_config["arma_home"],
+            "mods",
             self.item_name,
         )
         if self.is_examine:
-            print(f'src: {src}')
-            print(f'dst: {dst}')
+            print(f"src: {src}")
+            print(f"dst: {dst}")
             files = os.listdir(src)
             for f in files:
-                print(f'  {f}')
+                print(f"  {f}")
 
     def symlink_to_mods(self):
         src = os.path.join(
-            self.arma_config['workshop'],
+            self.arma_config["workshop"],
             self.item_id,
         )
         dst = os.path.join(
-            self.arma_config['arma_home'],
-            'mods',
+            self.arma_config["arma_home"],
+            "mods",
             self.item_name,
         )
         if not os.path.exists(dst):
             os.symlink(src, dst, target_is_directory=True)
 
     def symlink_to_mpmissions(self):
-        item_folder = os.path.join(
-            self.arma_config['workshop'],
-            self.item_id
-        )
+        item_folder = os.path.join(self.arma_config["workshop"], self.item_id)
         files = os.listdir(item_folder)
-        if(len(files)) == 1:
-            src = os.path.join(
-                item_folder,
-                files[0]
-            )
-            dst = os.path.join(
-                self.arma_config['arma_home'],
-                'mpmissions',
-                self.item_name
-            )
+        if (len(files)) == 1:
+            src = os.path.join(item_folder, files[0])
+            dst = os.path.join(self.arma_config["arma_home"], "mpmissions", self.item_name)
             if not os.path.exists(dst):
                 os.symlink(src, dst, target_is_directory=False)
         else:
             print("!! not a packaged pbo file !!")
 
 
 @click.command()
-@click.option(
-    "--id",
-    "item_id",
-    help="workshop id of mod"
-)
-@click.option(
-    "--name",
-    "item_name",
-    help="name of mod"
-)
+@click.option("--id", "item_id", help="workshop id of mod")
+@click.option("--name", "item_name", help="name of mod")
 @click.option(
     "--mission",
     "is_mission",
     is_flag=True,
     help="indicate this links to MPMissions and not mods",
 )
 @click.option(
@@ -187,9 +163,9 @@
                 workshop.examine()
             if is_mission:
                 workshop.symlink_to_mpmissions()
             elif is_mod:
                 workshop.symlink_to_mods()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `arma_server_tools-0.1.4/arma_server_tools/yaml_tools.py` & `arma_server_tools-0.1.5/arma_server_tools/yaml_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,15 +20,26 @@
         except yaml.YAMLError as exc:
             print(exc)
     return result
 
 
 def build_empty_config(config_file):
     data = {
-        'username': 'STEAM_USERNAME',
-        'password': 'STEAM_PASSWORD',
-        'workshop': "/home/steam/.steam/steamapps/workshop/content/107410",
-        'arma_home': "/home/steam/.steam/steamcmd/arma3",
-        'arma_configs': "/home/steam/arma_configs",
+        "username": "STEAM_USERNAME",
+        "password": "STEAM_PASSWORD",
+        "workshop": "/home/steam/.steam/steamapps/workshop/content/107410",
+        "arma_home": "/home/steam/.steam/steamcmd/arma3",
+        "arma_configs": "/home/steam/arma_configs",
     }
-    with open(config_file, 'w', encoding='utf8') as outfile:
+    with open(config_file, "w", encoding="utf8") as outfile:
         yaml.dump(data, outfile, default_flow_style=False, allow_unicode=True)
+
+
+def load_local_yaml(filename):
+
+    product = None
+    with open(filename, "r") as stream:
+        try:
+            product = yaml.safe_load(stream)
+        except yaml.YAMLError as exc:
+            print(exc)
+    return product
```

