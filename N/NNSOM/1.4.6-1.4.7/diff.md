# Comparing `tmp/nnsom-1.4.6.tar.gz` & `tmp/nnsom-1.4.7.tar.gz`

## Comparing `nnsom-1.4.6.tar` & `nnsom-1.4.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 nnsom-1.4.6/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.6/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.6/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    16133 2020-02-02 00:00:00.000000 nnsom-1.4.7/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.7/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.7/README.md
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 nnsom-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.7/PKG-INFO
```

### Comparing `nnsom-1.4.6/.gitignore` & `nnsom-1.4.7/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 
 ### NetBeans template
 **/nbproject/private/
 **/nbproject/Makefile-*.mk
 **/nbproject/Package-*.bash
 build/
 nbbuild/
-dist/
 nbdist/
 .nb-gradle/
 
 ### GPG template
 secring.*
 
 
@@ -289,15 +288,14 @@
 *.rel
 
 # AUCTeX auto folder
 /auto/
 
 # cask packages
 .cask/
-dist/
 
 # Flycheck
 flycheck_*.el
 
 # server auth directory
 /server/
 
@@ -431,28 +429,26 @@
 ### Archives template
 # It's better to unpack these files and commit the raw source because
 # git has its own built in compression methods.
 *.7z
 *.jar
 *.rar
 *.zip
-*.gz
 *.gzip
 *.tgz
 *.bzip
 *.bzip2
 *.bz2
 *.xz
 *.lzma
 *.cab
 *.xar
 
 # Packing-only formats
 *.iso
-*.tar
 
 # Package management formats
 *.dmg
 *.xpi
 *.gem
 *.egg
 *.deb
@@ -1017,15 +1013,14 @@
 # https://packagecontrol.io/packages/sublime-github
 GitHub.sublime-settings
 
 ### SBT template
 # Simple Build Tool
 # http://www.scala-sbt.org/release/docs/Getting-Started/Directories.html#configuring-version-control
 
-dist/*
 target/
 lib_managed/
 src_managed/
 project/boot/
 project/plugins/project/
 .history
 .cache
```

### Comparing `nnsom-1.4.6/pyproject.toml` & `nnsom-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
-include = ["src/NNSOM/*.py"]
+include = ["src/NNSOM/**"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.6"
+version = "1.4.7"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.6/PKG-INFO` & `nnsom-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.6
+Version: 1.4.7
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

