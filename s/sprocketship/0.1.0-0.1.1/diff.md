# Comparing `tmp/sprocketship-0.1.0.tar.gz` & `tmp/sprocketship-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.1.0.tar", last modified: Sat Apr  6 15:37:50 2024, max compression
+gzip compressed data, was "sprocketship-0.1.1.tar", last modified: Sat Apr  6 15:53:27 2024, max compression
```

## Comparing `sprocketship-0.1.0.tar` & `sprocketship-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.293699 sprocketship-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 15:37:46.000000 sprocketship-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:37:46.000000 sprocketship-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 15:37:50.293699 sprocketship-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-06 15:37:46.000000 sprocketship-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 15:37:46.000000 sprocketship-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:37:50.293699 sprocketship-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.289699 sprocketship-0.1.0/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-06 15:37:46.000000 sprocketship-0.1.0/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.293699 sprocketship-0.1.0/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 15:37:46.000000 sprocketship-0.1.0/sprocketship/templates/javascript.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.293699 sprocketship-0.1.0/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:53:27.413284 sprocketship-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 15:53:20.000000 sprocketship-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:53:20.000000 sprocketship-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 15:53:27.413284 sprocketship-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-06 15:53:20.000000 sprocketship-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 15:53:20.000000 sprocketship-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:53:27.413284 sprocketship-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:53:27.409284 sprocketship-0.1.1/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-06 15:53:20.000000 sprocketship-0.1.1/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:53:27.413284 sprocketship-0.1.1/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 15:53:20.000000 sprocketship-0.1.1/sprocketship/templates/javascript.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:53:27.413284 sprocketship-0.1.1/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 15:53:27.000000 sprocketship-0.1.1/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 15:53:27.000000 sprocketship-0.1.1/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:53:27.000000 sprocketship-0.1.1/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 15:53:27.000000 sprocketship-0.1.1/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 15:53:27.000000 sprocketship-0.1.1/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 15:53:27.000000 sprocketship-0.1.1/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.1.0/LICENSE` & `sprocketship-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.0/PKG-INFO` & `sprocketship-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.0
+Version: 0.1.1
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.1 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

### Comparing `sprocketship-0.1.0/README.md` & `sprocketship-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.0/pyproject.toml` & `sprocketship-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.1.0/sprocketship/cli.py` & `sprocketship-0.1.1/sprocketship/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     procedure_def_dict = {'procedure_definition': get_file_contents(path)}
     return render_file(os.path.join(Path(__file__).parent, "templates/javascript.sql"), **kwargs, **procedure_def_dict)
 
 
 @click.command()
 @click.argument("subcommand", type=click.Choice(["liftoff"]))
 @click.argument("dir", default=".")
-def main(subcommand, dir):
+@click.option('--show', is_flag=True)
+def main(subcommand, dir, show):
     if subcommand == "liftoff":
         click.echo(click.style(f"🚀 Sprocketship lifting off!", fg='white', bold=True))
         # Open config in current directory
 
         data = render_file(os.path.join(dir, '.sprocketship.yml'), return_dict=True)
 
         con = connector.connect(**data["snowflake"])
@@ -53,19 +54,20 @@
         # Get the configurations for each procedure and attach relative path to file directory
         configs_with_paths = extract_configs(data["procedures"])
         procs = list(itertools.chain(*configs_with_paths.values()))
 
         for proc in procs:
             try:
                 rendered_proc = create_javascript_stored_procedure(**proc, **{'project_dir': dir})
-                print(rendered_proc)
                 con.cursor().execute(rendered_proc)
                 msg = click.style(f"{proc['name']} ", fg='green', bold=True)
                 msg += click.style(f"launched into schema ", fg='white', bold=True)
                 msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
                 click.echo(msg)
+                if show:
+                    click.echo(rendered_proc)
             except Exception as e:
                 msg = click.style(f"{proc['name']} ", fg='red', bold=True)
                 msg += click.style(f"could not be launched into schema ", fg='white', bold=True)
                 msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
                 click.echo(msg)
                 click.echo(e, err=True)
```

### Comparing `sprocketship-0.1.0/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.1.1/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.0
+Version: 0.1.1
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.1 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

