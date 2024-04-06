# Comparing `tmp/aws-cdk.aws-pipes-targets-alpha-2.135.0a0.tar.gz` & `tmp/aws-cdk.aws-pipes-targets-alpha-2.136.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk.aws-pipes-targets-alpha-2.135.0a0.tar", last modified: Mon Apr  1 23:12:32 2024, max compression
+gzip compressed data, was "aws-cdk.aws-pipes-targets-alpha-2.136.0a0.tar", last modified: Sat Apr  6 02:37:07 2024, max compression
```

## Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0.tar` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2698 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1720 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1935 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/
--rw-r--r--   0 root         (0) root         (0)    11967 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      568 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22609 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.135.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 23:12:22.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 23:12:32.120314 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2698 2024-04-01 23:12:32.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-04-01 23:12:32.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 23:12:32.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-01 23:12:32.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-01 23:12:32.000000 aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 02:37:07.794838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-06 02:37:07.794838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 02:37:07.794838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 02:37:07.790838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 02:37:07.790838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 02:37:07.794838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/
+-rw-r--r--   0 root         (0) root         (0)    11967 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 02:37:07.794838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      568 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22609 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.136.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 02:36:56.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 02:37:07.794838 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-06 02:37:07.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-04-06 02:37:07.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 02:37:07.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-06 02:37:07.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-06 02:37:07.000000 aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/LICENSE` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/PKG-INFO` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-pipes-targets-alpha
-Version: 2.135.0a0
+Version: 2.136.0a0
 Summary: The CDK Construct Library for Amazon EventBridge Pipes Targets
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/README.md` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/setup.py` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-pipes-targets-alpha",
-    "version": "2.135.0.a0",
+    "version": "2.136.0.a0",
     "description": "The CDK Construct Library for Amazon EventBridge Pipes Targets",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.aws_pipes_targets_alpha",
         "aws_cdk.aws_pipes_targets_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_pipes_targets_alpha._jsii": [
-            "aws-pipes-targets-alpha@2.135.0-alpha.0.jsii.tgz"
+            "aws-pipes-targets-alpha@2.136.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_pipes_targets_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.135.0, <3.0.0",
-        "aws-cdk.aws-pipes-alpha==2.135.0.a0",
+        "aws-cdk-lib>=2.136.0, <3.0.0",
+        "aws-cdk.aws-pipes-alpha==2.136.0.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/__init__.py` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.aws_pipes_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-pipes-targets-alpha",
-    "2.135.0-alpha.0",
+    "2.136.0-alpha.0",
     __name__[0:-6],
-    "aws-pipes-targets-alpha@2.135.0-alpha.0.jsii.tgz",
+    "aws-pipes-targets-alpha@2.136.0-alpha.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.135.0-alpha.0.jsii.tgz` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.136.0-alpha.0.jsii.tgz`

 * *Files 1% similar despite different names*

#### Comparing `aws-pipes-targets-alpha@2.135.0-alpha.0.jsii.tgz-content` & `aws-pipes-targets-alpha@2.136.0-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'dependencies'": "{'@aws-cdk/aws-pipes-alpha': '2.136.0-alpha.0', 'aws-cdk-lib': '^2.136.0'}",*

 * * "'version'": "'2.136.0-alpha.0'"}*

```diff
@@ -4,16 +4,16 @@
         "organization": true,
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "dependencies": {
-        "@aws-cdk/aws-pipes-alpha": "2.135.0-alpha.0",
-        "aws-cdk-lib": "^2.135.0",
+        "@aws-cdk/aws-pipes-alpha": "2.136.0-alpha.0",
+        "aws-cdk-lib": "^2.136.0",
         "constructs": "^10.0.0"
     },
     "dependencyClosure": {
         "@aws-cdk/asset-awscli-v1": {
             "targets": {
                 "dotnet": {
                     "namespace": "Amazon.CDK.Asset.AwsCliV1",
@@ -3943,9 +3943,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "lib/sqs:SqsTargetParameters"
         }
     },
-    "version": "2.135.0-alpha.0"
+    "version": "2.136.0-alpha.0"
 }
```

##### package/lib/sqs.js

###### js-beautify {}

```diff
@@ -40,10 +40,10 @@
         };
     }
 }
 exports.SqsTarget = SqsTarget;
 _a = JSII_RTTI_SYMBOL_1;
 SqsTarget[_a] = {
     fqn: "@aws-cdk/aws-pipes-targets-alpha.SqsTarget",
-    version: "2.135.0-alpha.0"
+    version: "2.136.0-alpha.0"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic3FzLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsic3FzLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7OztBQW1DQTs7R0FFRztBQUNILE1BQWEsU0FBUztJQUlwQixZQUFZLEtBQWEsRUFBRSxVQUFnQzs7Ozs7OytDQUpoRCxTQUFTOzs7O1FBS2xCLElBQUksQ0FBQyxLQUFLLEdBQUcsS0FBSyxDQUFDO1FBQ25CLElBQUksQ0FBQyxTQUFTLEdBQUcsS0FBSyxDQUFDLFFBQVEsQ0FBQztRQUNoQyxJQUFJLENBQUMsZUFBZSxHQUFHLFVBQVUsQ0FBQztLQUNuQztJQUNELFNBQVMsQ0FBQyxPQUFjO1FBQ3RCLElBQUksQ0FBQyxLQUFLLENBQUMsaUJBQWlCLENBQUMsT0FBTyxDQUFDLENBQUM7S0FDdkM7SUFDRCxJQUFJLENBQUMsSUFBVztRQUNkLElBQUksQ0FBQyxJQUFJLENBQUMsZUFBZSxFQUFFLENBQUM7WUFDMUIsT0FBTztnQkFDTCxnQkFBZ0IsRUFBRSxFQUFFO2FBQ3JCLENBQUM7UUFDSixDQUFDO1FBRUQsT0FBTztZQUNMLGdCQUFnQixFQUFFO2dCQUNoQixhQUFhLEVBQUUsSUFBSSxDQUFDLGVBQWUsQ0FBQyxtQkFBbUIsRUFBRSxJQUFJLENBQUMsSUFBSSxDQUFDLENBQUMsYUFBYTtnQkFDakYsa0JBQWtCLEVBQUUsSUFBSSxDQUFDLGVBQWU7YUFDekM7U0FDRixDQUFDO0tBQ0g7O0FBekJILDhCQTBCQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IElJbnB1dFRyYW5zZm9ybWF0aW9uLCBJUGlwZSwgSVRhcmdldCwgVGFyZ2V0Q29uZmlnIH0gZnJvbSAnQGF3cy1jZGsvYXdzLXBpcGVzLWFscGhhJztcbmltcG9ydCB7IElSb2xlIH0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWlhbSc7XG5pbXBvcnQgeyBJUXVldWUgfSBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtc3FzJztcblxuLyoqXG4gKiBTUVMgdGFyZ2V0IHByb3BlcnRpZXMuXG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgU3FzVGFyZ2V0UGFyYW1ldGVycyB7XG4gIC8qKlxuICAgKiBUaGUgaW5wdXQgdHJhbnNmb3JtYXRpb24gdG8gYXBwbHkgdG8gdGhlIG1lc3NhZ2UgYmVmb3JlIHNlbmRpbmcgaXQgdG8gdGhlIHRhcmdldC5cbiAgICpcbiAgICogQHNlZSBodHRwczovL2RvY3MuYXdzLmFtYXpvbi5jb20vQVdTQ2xvdWRGb3JtYXRpb24vbGF0ZXN0L1VzZXJHdWlkZS9hd3MtcHJvcGVydGllcy1waXBlcy1waXBlLXBpcGV0YXJnZXRwYXJhbWV0ZXJzLmh0bWwjY2ZuLXBpcGVzLXBpcGUtcGlwZXRhcmdldHBhcmFtZXRlcnMtaW5wdXR0ZW1wbGF0ZVxuICAgKiBAZGVmYXVsdCBub25lXG4gICAqL1xuICByZWFkb25seSBpbnB1dFRyYW5zZm9ybWF0aW9uPzogSUlucHV0VHJhbnNmb3JtYXRpb247XG5cbiAgLyoqXG4gICAqIFRoaXMgcGFyYW1ldGVyIGFwcGxpZXMgb25seSB0byBGSUZPIChmaXJzdC1pbi1maXJzdC1vdXQpIHF1ZXVlcy5cbiAgICpcbiAgICogVGhlIHRva2VuIHVzZWQgZm9yIGRlZHVwbGljYXRpb24gb2Ygc2VudCBtZXNzYWdlcy5cbiAgICpcbiAgICogQHNlZSBodHRwOi8vZG9jcy5hd3MuYW1hem9uLmNvbS9BV1NDbG91ZEZvcm1hdGlvbi9sYXRlc3QvVXNlckd1aWRlL2F3cy1wcm9wZXJ0aWVzLXBpcGVzLXBpcGUtcGlwZXRhcmdldHNxc3F1ZXVlcGFyYW1ldGVycy5odG1sI2Nmbi1waXBlcy1waXBlLXBpcGV0YXJnZXRzcXNxdWV1ZXBhcmFtZXRlcnMtbWVzc2FnZWRlZHVwbGljYXRpb25pZFxuICAgKiBAZGVmYXVsdCBub25lXG4gICAqL1xuICByZWFkb25seSBtZXNzYWdlRGVkdXBsaWNhdGlvbklkPzogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBUaGUgRklGTyBtZXNzYWdlIGdyb3VwIElEIHRvIHVzZSBhcyB0aGUgdGFyZ2V0LlxuICAgKlxuICAgKiBAc2VlIGh0dHA6Ly9kb2NzLmF3cy5hbWF6b24uY29tL0FXU0Nsb3VkRm9ybWF0aW9uL2xhdGVzdC9Vc2VyR3VpZGUvYXdzLXByb3BlcnRpZXMtcGlwZXMtcGlwZS1waXBldGFyZ2V0c3FzcXVldWVwYXJhbWV0ZXJzLmh0bWwjY2ZuLXBpcGVzLXBpcGUtcGlwZXRhcmdldHNxc3F1ZXVlcGFyYW1ldGVycy1tZXNzYWdlZ3JvdXBpZFxuICAgKiBAZGVmYXVsdCBub25lXG4gICAqL1xuICByZWFkb25seSBtZXNzYWdlR3JvdXBJZD86IHN0cmluZztcbn1cblxuLyoqXG4gKiBBIEV2ZW50QnJpZGdlIFBpcGVzIHRhcmdldCB0aGF0IHNlbmRzIG1lc3NhZ2VzIHRvIGFuIFNRUyBxdWV1ZS5cbiAqL1xuZXhwb3J0IGNsYXNzIFNxc1RhcmdldCBpbXBsZW1lbnRzIElUYXJnZXQge1xuICBwcml2YXRlIHF1ZXVlOiBJUXVldWU7XG4gIHByaXZhdGUgcXVldWVQYXJhbWV0ZXJzPzogU3FzVGFyZ2V0UGFyYW1ldGVycztcbiAgcHVibGljIHJlYWRvbmx5IHRhcmdldEFybjogc3RyaW5nO1xuICBjb25zdHJ1Y3RvcihxdWV1ZTogSVF1ZXVlLCBwYXJhbWV0ZXJzPzogU3FzVGFyZ2V0UGFyYW1ldGVycykge1xuICAgIHRoaXMucXVldWUgPSBxdWV1ZTtcbiAgICB0aGlzLnRhcmdldEFybiA9IHF1ZXVlLnF1ZXVlQXJuO1xuICAgIHRoaXMucXVldWVQYXJhbWV0ZXJzID0gcGFyYW1ldGVycztcbiAgfVxuICBncmFudFB1c2goZ3JhbnRlZTogSVJvbGUpOiB2b2lkIHtcbiAgICB0aGlzLnF1ZXVlLmdyYW50U2VuZE1lc3NhZ2VzKGdyYW50ZWUpO1xuICB9XG4gIGJpbmQocGlwZTogSVBpcGUpOiBUYXJnZXRDb25maWcge1xuICAgIGlmICghdGhpcy5xdWV1ZVBhcmFtZXRlcnMpIHtcbiAgICAgIHJldHVybiB7XG4gICAgICAgIHRhcmdldFBhcmFtZXRlcnM6IHt9LFxuICAgICAgfTtcbiAgICB9XG5cbiAgICByZXR1cm4ge1xuICAgICAgdGFyZ2V0UGFyYW1ldGVyczoge1xuICAgICAgICBpbnB1dFRlbXBsYXRlOiB0aGlzLnF1ZXVlUGFyYW1ldGVycy5pbnB1dFRyYW5zZm9ybWF0aW9uPy5iaW5kKHBpcGUpLmlucHV0VGVtcGxhdGUsXG4gICAgICAgIHNxc1F1ZXVlUGFyYW1ldGVyczogdGhpcy5xdWV1ZVBhcmFtZXRlcnMsXG4gICAgICB9LFxuICAgIH07XG4gIH1cbn1cbiJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.963768115942029%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.136.0-alpha.0', '@aws-cdk/integ-runner': "*

 * *                      "'2.136.0-alpha.0', '@aws-cdk/pkglint': '2.136.0-alpha.0', 'aws-cdk-lib': "*

 * *                      "'2.136.0', '@aws-cdk/aws-pipes-alpha': '2.136.0-alpha.0', "*

 * *                      "'@aws-cdk/integ-tests-alpha': '2.136.0-alpha.0'}",*

 * * "'peerDependencies'": "{'@aws-cdk/aws-pipes-alpha': '2.136.0-alpha.0', 'aws-cdk-lib': '^2.136.0'}",*

 * * "'version'": "'2.136.0-alpha.0'"}*

```diff
@@ -11,21 +11,21 @@
         "env": {
             "AWSLINT_BASE_CONSTRUCT": true
         }
     },
     "dependencies": {},
     "description": "The CDK Construct Library for Amazon EventBridge Pipes Targets",
     "devDependencies": {
-        "@aws-cdk/aws-pipes-alpha": "2.135.0-alpha.0",
-        "@aws-cdk/cdk-build-tools": "2.135.0-alpha.0",
-        "@aws-cdk/integ-runner": "2.135.0-alpha.0",
-        "@aws-cdk/integ-tests-alpha": "2.135.0-alpha.0",
-        "@aws-cdk/pkglint": "2.135.0-alpha.0",
+        "@aws-cdk/aws-pipes-alpha": "2.136.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.136.0-alpha.0",
+        "@aws-cdk/integ-runner": "2.136.0-alpha.0",
+        "@aws-cdk/integ-tests-alpha": "2.136.0-alpha.0",
+        "@aws-cdk/pkglint": "2.136.0-alpha.0",
         "@types/jest": "^29.5.12",
-        "aws-cdk-lib": "2.135.0",
+        "aws-cdk-lib": "2.136.0",
         "constructs": "^10.0.0",
         "jest": "^29"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
     "homepage": "https://github.com/aws/aws-cdk",
@@ -76,16 +76,16 @@
         "aws-pipes"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "maturity": "experimental",
     "name": "@aws-cdk/aws-pipes-targets-alpha",
     "peerDependencies": {
-        "@aws-cdk/aws-pipes-alpha": "2.135.0-alpha.0",
-        "aws-cdk-lib": "^2.135.0",
+        "@aws-cdk/aws-pipes-alpha": "2.136.0-alpha.0",
+        "aws-cdk-lib": "^2.136.0",
         "constructs": "^10.0.0"
     },
     "pkglint": {
         "exclude": [
             "naming/package-matches-directory",
             "assert/assert-dependency"
         ]
@@ -112,9 +112,9 @@
         "pkglint": "pkglint -f",
         "rosetta:extract": "yarn --silent jsii-rosetta extract",
         "test": "cdk-test",
         "watch": "cdk-watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "2.135.0-alpha.0"
+    "version": "2.136.0-alpha.0"
 }
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-pipes-targets-alpha
-Version: 2.135.0a0
+Version: 2.136.0a0
 Summary: The CDK Construct Library for Amazon EventBridge Pipes Targets
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-pipes-targets-alpha-2.135.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-pipes-targets-alpha-2.136.0a0/src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/requires.txt
 src/aws_cdk.aws_pipes_targets_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_pipes_targets_alpha/__init__.py
 src/aws_cdk/aws_pipes_targets_alpha/py.typed
 src/aws_cdk/aws_pipes_targets_alpha/_jsii/__init__.py
-src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.135.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_pipes_targets_alpha/_jsii/aws-pipes-targets-alpha@2.136.0-alpha.0.jsii.tgz
```

