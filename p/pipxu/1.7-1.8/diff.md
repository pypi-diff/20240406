# Comparing `tmp/pipxu-1.7.tar.gz` & `tmp/pipxu-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipxu-1.7.tar", last modified: Thu Apr  4 00:18:34 2024, max compression
+gzip compressed data, was "pipxu-1.8.tar", last modified: Sat Apr  6 04:32:47 2024, max compression
```

## Comparing `pipxu-1.7.tar` & `pipxu-1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2024-04-04 00:13:06.000000 pipxu-1.7/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-04-04 00:13:06.000000 pipxu-1.7/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      472 2024-04-04 00:13:57.000000 pipxu-1.7/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    16994 2024-04-04 00:18:34.375951 pipxu-1.7/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    16471 2024-04-04 00:14:10.000000 pipxu-1.7/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/doc/
--rw-r--r--   0 mark      (1000) mark      (1000)     2539 2024-04-04 00:13:06.000000 pipxu-1.7/doc/debug.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/pipxu/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/pipxu/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     1729 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/debug.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1186 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/inject.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4696 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/install.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1442 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/list.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1515 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/reinstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2953 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/reinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      958 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/runpip.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1176 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/uninject.py
--rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/uninstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)      938 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/uninstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/upgrade-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1407 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/upgrade.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1595 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/commands/version.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5786 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/pipxu.py
--rw-r--r--   0 mark      (1000) mark      (1000)      780 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/run.py
--rw-r--r--   0 mark      (1000) mark      (1000)    10070 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu/utils.py
--rwxr-xr-x   0 mark      (1000) mark      (1000)      316 2024-04-04 00:13:06.000000 pipxu-1.7/pipxu-bootstrap
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-04 00:18:34.375951 pipxu-1.7/pipxu.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    16994 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      688 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-04 00:18:34.000000 pipxu-1.7/pipxu.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1096 2024-04-04 00:13:06.000000 pipxu-1.7/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-04 00:18:34.375951 pipxu-1.7/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2024-04-04 00:13:06.000000 pipxu-1.8/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-04-04 00:13:06.000000 pipxu-1.8/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      472 2024-04-04 00:13:57.000000 pipxu-1.8/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    16992 2024-04-06 04:32:47.460507 pipxu-1.8/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    16469 2024-04-05 03:58:58.000000 pipxu-1.8/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/doc/
+-rw-r--r--   0 mark      (1000) mark      (1000)     2539 2024-04-04 00:13:06.000000 pipxu-1.8/doc/debug.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/pipxu/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/pipxu/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1729 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/debug.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1192 2024-04-06 00:46:58.000000 pipxu-1.8/pipxu/commands/inject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4772 2024-04-06 03:52:55.000000 pipxu-1.8/pipxu/commands/install.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1442 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/list.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1515 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/reinstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2960 2024-04-06 00:46:43.000000 pipxu-1.8/pipxu/commands/reinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      964 2024-04-06 00:46:12.000000 pipxu-1.8/pipxu/commands/runpip.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1182 2024-04-06 00:46:28.000000 pipxu-1.8/pipxu/commands/uninject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/uninstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      938 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/uninstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/upgrade-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1413 2024-04-06 00:47:39.000000 pipxu-1.8/pipxu/commands/upgrade.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1607 2024-04-06 00:44:27.000000 pipxu-1.8/pipxu/commands/version.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5800 2024-04-06 04:17:47.000000 pipxu-1.8/pipxu/pipxu.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      872 2024-04-06 03:24:54.000000 pipxu-1.8/pipxu/run.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    10394 2024-04-06 03:50:43.000000 pipxu-1.8/pipxu/utils.py
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      316 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu-bootstrap
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/pipxu.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    16992 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      688 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1096 2024-04-04 00:13:06.000000 pipxu-1.8/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-06 04:32:47.460507 pipxu-1.8/setup.cfg
```

### Comparing `pipxu-1.7/PKG-INFO` & `pipxu-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.7
+Version: 1.8
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: platformdirs
 Requires-Dist: importlib-metadata; python_version < "3.8"
 
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
-[`pipxu`][pipxu] installs Python applications, i.e. a Python packages
+[`pipxu`][pipxu] installs Python applications, i.e. Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
 are thus insulated from all other applications, and from the system
 Python. [`pipxu`][pipxu] creates links to application executables in a
 common directory, which you have in your [PATH][path]. Packages are
 typically sourced from [PyPI][pypi], the Python Package Index.
```

### Comparing `pipxu-1.7/README.md` & `pipxu-1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
-[`pipxu`][pipxu] installs Python applications, i.e. a Python packages
+[`pipxu`][pipxu] installs Python applications, i.e. Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
 are thus insulated from all other applications, and from the system
 Python. [`pipxu`][pipxu] creates links to application executables in a
 common directory, which you have in your [PATH][path]. Packages are
 typically sourced from [PyPI][pypi], the Python Package Index.
```

### Comparing `pipxu-1.7/doc/debug.md` & `pipxu-1.8/doc/debug.md`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/debug.py` & `pipxu-1.8/pipxu/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/inject.py` & `pipxu-1.8/pipxu/commands/inject.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
 
     pip_args = utils.make_args((args.verbose, '-v'))
     extras = ' '.join(f'"{a}"' for a in args.extras)
-    if not utils.piprun(vdir, f'install{pip_args} --compile {extras}'):
+    if not utils.piprun(vdir, f'install{pip_args} --compile {extras}', args):
         return f'Error: failed to install "{extras}" to {pkgname}'
 
     return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args, add=True)
```

### Comparing `pipxu-1.7/pipxu/commands/install.py` & `pipxu-1.8/pipxu/commands/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,43 +46,44 @@
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
                                 (args.system_site_packages,
                                  '--system-site-packages'),
-                                (bool(pyexe), f'--python={pyexe}'))
+                                (True, f'--python={pyexe}'))
     pip_args = utils.make_args((args.verbose, '-v'), (args.editable, '-e'))
 
     lockfile = user_runtime_path() / f'{args._prog}.lock'
     vdirbase = args._venvs_dir
     for pkg in args.package:
         # Use a lock file in case we are running multiple installs in parallel
         with FileLock(lockfile):
             vdir = get_next_vdir(vdirbase)
             if not vdir:
                 return f'Error: Too many vdirs (>{MAX_VDIRS}) in {vdirbase}'
 
             # Create the vdir
-            if not run(f'uv venv{venv_args} {vdir}'):
+            if not run(f'{args._uv} venv{venv_args} {vdir}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to create {vdir} for {pkg}.'
 
         python_exe = (vdir / 'bin' / 'python').resolve()
-        python_ver = run(f'{python_exe} -V', capture=True)
+        python_ver = run(f'{python_exe} -V', capture=True, shell=False,
+                         ignore_error=True)
         python_ver = python_ver.strip().split()[1] if python_ver else '?ver?'
         print(f'Created {vdir} using {python_exe} ({python_ver})')
 
         # Install the package
         if not utils.piprun(vdir, f'install --compile --no-deps{pip_args} '
-                            f'"{pkg}"'):
+                            f'"{pkg}"', args):
             utils.rm_vdir(vdir, args)
             return f'Error: failed to preinstall "{pkg}".'
 
-        versions = utils.get_versions(vdir)
+        versions = utils.get_versions(vdir, args)
         if not versions:
             utils.rm_vdir(vdir, args)
             return f'Error: failed to get versions for {pkg}.'
 
         if len(versions) != 1:
             return f'Error: multiple packages qualified: {list(versions)}'
 
@@ -93,15 +94,15 @@
             if not args.force:
                 utils.rm_vdir(vdir, args)
                 return f'Error: venv for {pkgname} exists. Use -f to force.'
             print(f'Removing pre-existing {pkgname} venv dir.')
             utils.rm_vdir(pdir, args)
             pdir.unlink()
 
-        if not utils.piprun(vdir, f'install --compile{pip_args} "{pkg}"'):
+        if not utils.piprun(vdir, f'install --compile{pip_args} "{pkg}"', args):
             utils.rm_vdir(vdir, args)
             return f'Error: failed to install "{pkg}".'
 
         pdir.symlink_to(vdir)
 
         data: dict = {'name': pkgname}
         if editpath:
```

### Comparing `pipxu-1.7/pipxu/commands/list.py` & `pipxu-1.8/pipxu/commands/list.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/reinstall-all.py` & `pipxu-1.8/pipxu/commands/reinstall-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/reinstall.py` & `pipxu-1.8/pipxu/commands/reinstall.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parser.add_argument('package', nargs='+',
                         help='application[s] to reinstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
-                                (bool(pyexe), f'--python={pyexe}'))
+                                (True, f'--python={pyexe}'))
     pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
             return f'Application {pkgname} is not installed.'
 
         print(f'Reinstalling {pkgname} ..')
@@ -52,20 +52,20 @@
 
         sysp = ' --system-site-packages' if data.get('sys') else ''
         with tempfile.TemporaryDirectory() as tdir:
             tfile = Path(tdir, args._freeze_file)
             shutil.copyfile(vdir / args._freeze_file, tfile)
 
             # Recreate the vdir
-            if not run(f'uv venv{venv_args}{sysp} {vdir}'):
+            if not run(f'{args._uv} venv{venv_args}{sysp} {vdir}'):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to recreate {vdir} for {pkgname}.'
 
             if not utils.piprun(vdir, f'sync{pip_args} --compile --reinstall '
-                                f'{tfile}'):
+                                f'{tfile}', args):
                 utils.rm_vdir(vdir, args)
                 return f'Error: failed to resync {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
```

### Comparing `pipxu-1.7/pipxu/commands/runpip.py` & `pipxu-1.8/pipxu/commands/runpip.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
 
-    if not utils.piprun(vdir, ' '.join(args.args), quiet=True):
+    if not utils.piprun(vdir, ' '.join(args.args), args, quiet=True):
         return f'Error: failed to run pip for {pkgname}'
     return None
```

### Comparing `pipxu-1.7/pipxu/commands/uninject.py` & `pipxu-1.8/pipxu/commands/uninject.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
 
     pip_args = utils.make_args((args.verbose, '-v'))
     extras = ' '.join(f'"{a}"' for a in args.extras)
-    if not utils.piprun(vdir, f'uninstall{pip_args} {extras}'):
+    if not utils.piprun(vdir, f'uninstall{pip_args} {extras}', args):
         return f'Error: failed to uninstall {extras} to {pkgname}'
 
     return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args, add=False)
```

### Comparing `pipxu-1.7/pipxu/commands/uninstall-all.py` & `pipxu-1.8/pipxu/commands/uninstall-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/uninstall.py` & `pipxu-1.8/pipxu/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/upgrade-all.py` & `pipxu-1.8/pipxu/commands/upgrade-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pipxu/commands/upgrade.py` & `pipxu-1.8/pipxu/commands/upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         print(f'Upgrading {pkgname} ..')
         data = utils.get_json(vdir, args) or {}
         editpath = data.get('editpath')
         pkg = f'-e {editpath}' if editpath else pkgname
         extras = ' '.join(data.get('injected', []))
         if not utils.piprun(vdir, 'install --compile --reinstall -U'
-                            f'{pip_args} {pkg} {extras}'):
+                            f'{pip_args} {pkg} {extras}', args):
             return f'Error: failed to {args.name} {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             return err
 
         print(f'{pkgname} upgraded.')
```

### Comparing `pipxu-1.7/pipxu/commands/version.py` & `pipxu-1.8/pipxu/commands/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         print(f'{pkgname}=={ver}')
 
     if args.package:
         pkgname, vdir = utils.get_package_from_arg(args.package, args)
         if not vdir:
             return f'Application {pkgname} not found.'
 
-        versions = utils.get_versions(args._packages_dir / pkgname)
+        versions = utils.get_versions(args._packages_dir / pkgname, args)
         if not versions:
             return f'Application {pkgname} versions not found.'
 
         # Reorder version dict to put pkgname first
         if pkgname in versions:
             sversions = {pkgname: versions[pkgname]}
             del versions[pkgname]
@@ -40,12 +40,12 @@
         for pkg, ver in versions.items():
             display(pkg, ver)
 
         return None
 
     for pdir, data in utils.get_all_pkg_venvs(args):
         package = pdir.name
-        versions = utils.get_versions(pdir)
+        versions = utils.get_versions(pdir, args)
         if versions:
             display(package, versions.get(package, ("unknown", None)))
 
     return None
```

### Comparing `pipxu-1.7/pipxu/pipxu.py` & `pipxu-1.8/pipxu/pipxu.py`

 * *Files 16% similar despite different names*

```diff
@@ -94,48 +94,51 @@
 
     args = mainparser.parse_args(shlex.split(cnflines) + sys.argv[1:])
 
     if args.version:
         print(f'{PROG}=={utils.version()}')
         return None
 
-    homedir = args.home or os.getenv(f'{PROGU}_HOME')
-    bindir = args.bin_dir or os.getenv(f'{PROGU}_BIN_DIR')
-    mandir = args.man_dir or os.getenv(f'{PROGU}_MAN_DIR')
+    is_root = os.geteuid() == 0
+    home_dir = args.home or os.getenv(f'{PROGU}_HOME')
+    bin_dir = args.bin_dir or os.getenv(f'{PROGU}_BIN_DIR')
+    man_dir = args.man_dir or os.getenv(f'{PROGU}_MAN_DIR')
     pyexe = args.default_python or os.getenv(f'{PROGU}_DEFAULT_PYTHON') or DEFPY
 
-    if os.geteuid() == 0:
-        home_dir = Path(homedir if homedir else f'/opt/{PROG}')
-        bin_dir = Path(bindir if bindir else '/usr/local/bin')
-        man_dir = Path(mandir if mandir else '/usr/local/share/man')
-    else:
-        home_dir = Path(homedir) if homedir else \
-                        (platformdirs.user_data_path() / PROG)
-        bin_dir = Path(bindir) if bindir else \
-                Path('~/.local/bin').expanduser()
-        man_dir = Path(mandir) if mandir else \
-                Path('~/.local/share/man').expanduser()
+    if not home_dir:
+        home_dir = f'/opt/{PROG}' if is_root else \
+                f'{platformdirs.user_data_dir()}/{PROG}'
+    if not bin_dir:
+        bin_dir = '/usr/local/bin' if is_root else '~/.local/bin'
+    if not man_dir:
+        man_dir = '/usr/local/share/man' if is_root else '~/.local/share/man'
+
+    home_dir = utils.subenvars(home_dir)
+    bin_dir = utils.subenvars(bin_dir)
+    man_dir = utils.subenvars(man_dir)
+    pyexe = utils.subenvars(pyexe)
 
     if not args.func:
         mainparser.print_help()
         print('\nEnvironment:')
         print(f'{PROGU}_HOME = {home_dir}')
         print(f'{PROGU}_BIN_DIR = {bin_dir}')
         print(f'{PROGU}_MAN_DIR = {man_dir}')
         print(f'{PROGU}_DEFAULT_PYTHON = {pyexe}')
         print()
         print(path_check(f'{PROGU}_BIN_DIR', bin_dir))
         return None
 
     # Ensure uv is installed/available
     uv = args.uv or DEFUV
-    version = run(f'{uv} --version', capture=True)
+    version = run(f'{uv} --version', capture=True, shell=False,
+                  ignore_error=True)
     if not version:
         if args.uv:
-            return f'Error: uv program not found at "{uv}"'
+            return f'Error: specified uv "{uv}" program not found.'
 
         return f'Error: {uv} program must be installed, and in your PATH '\
                 'or specified with --uv option.'
 
     # Keep some useful info in the namespace passed to the command
     args._uv = uv
     args._packages_dir = home_dir / 'packages'
```

### Comparing `pipxu-1.7/pipxu/run.py` & `pipxu-1.8/pipxu/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 'Common module containing shared functions'
 from __future__ import annotations
 
 import subprocess
 import sys
 from typing import Optional
 
-def run(cmd: str, *, capture: bool = False,
-        quiet: bool = False) -> Optional[str]:
+def run(cmd: str, *, capture: bool = False, quiet: bool = False,
+        shell=True, ignore_error=False) -> Optional[str]:
     'Run given command string'
     if capture:
         stdout = subprocess.PIPE
     else:
         stdout = None
         if not quiet:
             print(f'>>> Running {cmd}')
     try:
-        res = subprocess.run(cmd, shell=True, stdout=stdout,
-                             universal_newlines=True)
+        res = subprocess.run(cmd if shell else cmd.split(), shell=shell,
+                             stdout=stdout, universal_newlines=True)
     except Exception as e:
-        print(f'{cmd} failed: {e}', file=sys.stderr)
+        if not ignore_error:
+            print(f'{cmd} failed: {e}', file=sys.stderr)
         return None
 
     if res.returncode != 0:
         return None
 
     return (res.stdout and res.stdout.strip()) if capture else 'ok'
```

### Comparing `pipxu-1.7/pipxu/utils.py` & `pipxu-1.8/pipxu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 import sys
 from argparse import Namespace
 from pathlib import Path
 from typing import Iterable, Optional
 
 from .run import run
 
+def subenvars(path: str) -> Path:
+    'Substitute environment variables in a path string'
+    return Path(os.path.expandvars(path)).expanduser()
+
 def get_json(vdir: Path, args: Namespace) -> Optional[dict]:
     'Get JSON data for this virtual environment'
     tgt = vdir.resolve() / args._meta_file
     try:
         with tgt.open() as fp:
             return json.load(fp)
     except Exception:
@@ -28,22 +32,23 @@
         with tgt.open('w') as fp:
             json.dump(data, fp)
     except Exception as e:
         return str(e)
 
     return None
 
-def piprun(vdir: Path, cmd: str, **args) -> Optional[str]:
+def piprun(vdir: Path, cmd: str, args: Namespace, **kargs) -> Optional[str]:
     'Run given pip command in the virtual environment'
     os.environ['VIRTUAL_ENV'] = str(vdir.resolve())
-    return run(f'uv pip {cmd}', **args)
+    return run(f'{args._uv} pip {cmd}', **kargs)
 
-def get_versions(vdir: Path) -> Optional[dict[str, tuple[str, Optional[str]]]]:
+def get_versions(vdir: Path, args: Namespace) -> \
+        Optional[dict[str, tuple[str, Optional[str]]]]:
     'Return the versions of the packages in the virtual environment'
-    out = piprun(vdir, 'list', capture=True)
+    out = piprun(vdir, 'list', args, capture=True, shell=False)
     if not out:
         return None
 
     found = False
     data: dict[str, tuple[str, Optional[str]]] = {}
     for line in out.splitlines():
         if line.startswith('-'):
@@ -154,32 +159,33 @@
         _link_all_files(vdir / 'share' / 'man', args._man_dir, '*/*',
                         args.verbose)
 
     # Save the apps in the JSON data
     if not apps:
         return f'Error: {pkgname} has no executables to install.'
 
-    freeze = piprun(vdir, 'freeze', capture=True)
+    freeze = piprun(vdir, 'freeze', args, capture=True, shell=False)
     if not freeze:
         return 'Error: Failed to fetch freeze list.'
 
     (vdir / args._freeze_file).write_text(freeze)
     data['apps'] = sorted(apps)
     return _set_json(vdir, args, data)
 
 def rm_vdir(vdir: Path, args: Namespace) -> None:
     'Remove all links that point into the virtual environment'
     vdir = vdir.resolve()
     _unlink_all_files(vdir, args)
 
     # Remove the venv
-    if args.verbose:
-        print(f'Removing {vdir}')
+    if vdir.exists():
+        if args.verbose:
+            print(f'Removing {vdir}')
 
-    shutil.rmtree(vdir)
+        shutil.rmtree(vdir)
 
 def add_or_remove_pkg(vdir: Path, pkgname: str, pkgs: list[str],
                       args: Namespace, *, add: bool) -> Optional[str]:
     'Record the addition/removal of a package into the virtual environment'
     data = get_json(vdir, args)
     if not data:
         return 'No JSON data found'
@@ -233,15 +239,15 @@
     return name, (path if path.exists() else None)
 
 def _rm_path(path: Path) -> None:
     'Remove the given path'
     print(f'Purging stray {path}', file=sys.stderr)
     if path.is_dir():
         shutil.rmtree(path)
-    else:
+    elif path.exists():
         path.unlink()
 
 def purge_old_files(args: Namespace) -> None:
     'Clean out any old virtual environments, packages, and executables'
     # Remove any packages that do not point to a dir in the venvs directory
     valids_venvs = set()
     for pkg in args._packages_dir.iterdir():
@@ -264,36 +270,36 @@
             _rm_path(exe)
 
 def get_all_package_names(args: Namespace) -> list[str]:
     'Return a sorted list of all package names'
     return sorted(set(f.name for f in args._packages_dir.iterdir())
                   - set(args.skip or []))
 
-def get_python(args: Namespace) -> str:
+def get_python(args: Namespace) -> Path:
     'Return the python executable based on command line args'
     if args.pyenv:
-        pyenv_root = run('pyenv root', capture=True)
+        pyenv_root = run('pyenv root', capture=True, shell=False,
+                         ignore_error=True)
         if not pyenv_root:
             sys.exit('Error: Can not find pyenv. Is it installed?')
 
-        pyenv_version = run(f'pyenv latest {args.pyenv}', capture=True)
+        pyenv_version = run(f'pyenv latest {args.pyenv}', capture=True,
+                            shell=False, ignore_error=True)
         if not pyenv_version:
             sys.exit(f'Error: no pyenv version {args.pyenv} installed.')
 
         pyexe = Path(pyenv_root, 'versions', pyenv_version, 'bin', 'python')
         if not pyexe.exists():
             sys.exit(f'Can not determine pyenv version for {args.pyenv}')
     elif args.python:
-        pyexe = Path(args.python)
-        if not pyexe.exists():
-            sys.exit(f'{pyexe} does not exist.')
+        pyexe = subenvars(args.python)
     else:
         pyexe = args._pyexe
 
-    return str(pyexe)
+    return pyexe
 
 def version() -> str:
     'Return the version of this package'
     if sys.version_info >= (3, 8):
         from importlib.metadata import version
     else:
         from importlib_metadata import version
```

### Comparing `pipxu-1.7/pipxu.egg-info/PKG-INFO` & `pipxu-1.8/pipxu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.7
+Version: 1.8
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: platformdirs
 Requires-Dist: importlib-metadata; python_version < "3.8"
 
 ## PIPXU - Install and Run Python Applications in Isolated Environments using UV
 [![PyPi](https://img.shields.io/pypi/v/pipxu)](https://pypi.org/project/pipxu/)
 [![AUR](https://img.shields.io/aur/version/pipxu)](https://aur.archlinux.org/packages/pipxu/)
 
-[`pipxu`][pipxu] installs Python applications, i.e. a Python packages
+[`pipxu`][pipxu] installs Python applications, i.e. Python packages
 which have one or more executable programs, into independent isolated
 virtual environments on your system. Each package and it's dependencies
 are thus insulated from all other applications, and from the system
 Python. [`pipxu`][pipxu] creates links to application executables in a
 common directory, which you have in your [PATH][path]. Packages are
 typically sourced from [PyPI][pypi], the Python Package Index.
```

### Comparing `pipxu-1.7/pipxu.egg-info/SOURCES.txt` & `pipxu-1.8/pipxu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipxu-1.7/pyproject.toml` & `pipxu-1.8/pyproject.toml`

 * *Files identical despite different names*

