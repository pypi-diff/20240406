# Comparing `tmp/dkist-processing-ops-1.0.0rc3.tar.gz` & `tmp/dkist-processing-ops-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-ops-1.0.0rc3.tar", last modified: Wed Mar  6 22:32:20 2024, max compression
+gzip compressed data, was "dkist-processing-ops-1.0.0rc4.tar", last modified: Fri Apr  5 22:56:45 2024, max compression
```

## Comparing `dkist-processing-ops-1.0.0rc3.tar` & `dkist-processing-ops-1.0.0rc4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1497 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      740 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2632 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1667 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/tasks/wait.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/tests/test_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3103 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops/workflows/scale.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1497 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-06 22:32:20.000000 dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1977 2024-03-06 22:32:05.000000 dkist-processing-ops-1.0.0rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-06 22:32:20.942135 dkist-processing-ops-1.0.0rc3/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2759 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.919491 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/dags/
+-rw-rw-rw-   0 root         (0) root         (0)     2341 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/dags/scale.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/tasks/wait.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/tests/test_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops/workflows/smoke.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-05 22:56:45.000000 dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2024-04-05 22:56:33.000000 dkist-processing-ops-1.0.0rc4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-05 22:56:45.923491 dkist-processing-ops-1.0.0rc4/setup.cfg
```

### Comparing `dkist-processing-ops-1.0.0rc3/.gitignore` & `dkist-processing-ops-1.0.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-ops-1.0.0rc3/.pre-commit-config.yaml` & `dkist-processing-ops-1.0.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-ops-1.0.0rc3/PKG-INFO` & `dkist-processing-ops-1.0.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dkist-processing-ops
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Automated Processing smoke test and operations workflows
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-processing-ops
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: dkist-processing-core==3.0.2rc1
+Requires-Dist: dkist-processing-common==6.1.0
 Requires-Dist: dkist-service-configuration==1.1.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 
 dkist-processing-ops
```

### Comparing `dkist-processing-ops-1.0.0rc3/README.rst` & `dkist-processing-ops-1.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-ops-1.0.0rc3/bitbucket-pipelines.yml` & `dkist-processing-ops-1.0.0rc4/bitbucket-pipelines.yml`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         name: Push Workflow
         script:
           - pip install -U pip
           - pip install .
           - export BUILD_VERSION="${BITBUCKET_TAG:1}"
           - export ARTIFACT_FOLDER="${BITBUCKET_REPO_SLUG}_${BUILD_VERSION}/"
           - python -c "from dkist_processing_core.build_utils import export_dags; import dkist_processing_ops.workflows as workflow_package; export_dags(workflow_package, '${ARTIFACT_FOLDER}')"
+          - python -c "from dkist_processing_ops.dags.scale import export_scale_dags; export_scale_dags('${ARTIFACT_FOLDER}')"
           - export SOURCE_PATH="workflow_${BUILD_VERSION}.gz"
           - tar --exclude="bitbucket-pipelines.yml" -cvzf ${SOURCE_PATH} ${ARTIFACT_FOLDER}
           - export TARGET_PATH="generic-packages/dkist-processing-ops/${BUILD_VERSION}/"
           - curl -fL https://getcli.jfrog.io | sh
           - ./jfrog rt u --url $ARTIFACTORY_URL --user $ARTIFACTORY_USER --password $ARTIFACTORY_PASSWORD ${SOURCE_PATH} ${TARGET_PATH}
     - step: &push_code
         caches:
```

### Comparing `dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/PKG-INFO` & `dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dkist-processing-ops
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Automated Processing smoke test and operations workflows
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-processing-ops
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: dkist-processing-core==3.0.2rc1
+Requires-Dist: dkist-processing-common==6.1.0
 Requires-Dist: dkist-service-configuration==1.1.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 
 dkist-processing-ops
```

### Comparing `dkist-processing-ops-1.0.0rc3/dkist_processing_ops.egg-info/SOURCES.txt` & `dkist-processing-ops-1.0.0rc4/dkist_processing_ops.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 dkist_processing_ops/_version.py
 dkist_processing_ops.egg-info/PKG-INFO
 dkist_processing_ops.egg-info/SOURCES.txt
 dkist_processing_ops.egg-info/dependency_links.txt
 dkist_processing_ops.egg-info/not-zip-safe
 dkist_processing_ops.egg-info/requires.txt
 dkist_processing_ops.egg-info/top_level.txt
+dkist_processing_ops/dags/scale.py
 dkist_processing_ops/tasks/__init__.py
 dkist_processing_ops/tasks/wait.py
 dkist_processing_ops/tests/__init__.py
 dkist_processing_ops/tests/test_workflows.py
 dkist_processing_ops/workflows/__init__.py
-dkist_processing_ops/workflows/scale.py
+dkist_processing_ops/workflows/smoke.py
```

### Comparing `dkist-processing-ops-1.0.0rc3/pyproject.toml` & `dkist-processing-ops-1.0.0rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 license = { text = "BSD 3-Clause" }
 authors = [
   { name = "NSO / AURA", email = "dkistdc@nso.edu" },
 ]
 
 dependencies = [
-    "dkist-processing-core==3.0.2rc1",
+    "dkist-processing-common==6.1.0",
     "dkist-service-configuration==1.1.0",
 ]
 dynamic = ["version"]
 
 # tox is not required to run the tests, but simplifies IDE integration
 # Pygments is solely to support README.rst rendering
 [project.optional-dependencies]
```

