# Comparing `tmp/cfnresponse-1.1.2.tar.gz` & `tmp/cfnresponse-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfnresponse-1.1.2.tar", last modified: Mon Sep 27 15:15:59 2021, max compression
+gzip compressed data, was "cfnresponse-1.1.3.tar", last modified: Sat Apr  6 19:33:48 2024, max compression
```

## Comparing `cfnresponse-1.1.2.tar` & `cfnresponse-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 15:15:59.858666 cfnresponse-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-09-27 15:15:59.858666 cfnresponse-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 15:15:59.858666 cfnresponse-1.1.2/cfnresponse/
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/cfnresponse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 15:15:59.858666 cfnresponse-1.1.2/cfnresponse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/cfnresponse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/cfnresponse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/cfnresponse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/cfnresponse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/cfnresponse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-27 15:15:59.858666 cfnresponse-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      825 2021-09-27 15:15:59.000000 cfnresponse-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:33:48.629397 cfnresponse-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-06 19:33:48.629397 cfnresponse-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:33:48.625397 cfnresponse-1.1.3/cfnresponse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/cfnresponse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:33:48.629397 cfnresponse-1.1.3/cfnresponse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/cfnresponse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/cfnresponse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/cfnresponse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/cfnresponse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/cfnresponse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:33:48.629397 cfnresponse-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 19:33:48.000000 cfnresponse-1.1.3/setup.py
```

### Comparing `cfnresponse-1.1.2/LICENSE` & `cfnresponse-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfnresponse-1.1.2/PKG-INFO` & `cfnresponse-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: cfnresponse
-Version: 1.1.2
+Version: 1.1.3
 Summary: Send a response object to a custom resource by way of an Amazon S3 presigned URL
 Home-page: https://github.com/gene1wood/cfnresponse
 Author: Amazon Web Services
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3
 
 # cfnresponse
 
 This package contains the Amazon Web Services (AWS) cfnresponse module which is
 available in Python AWS Lambda environments.
 
-The code for this module can be found [in the Lambda Function Code documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-lambda-function-code.html#cfn-lambda-function-code-cfnresponsemodule)
+The code for this module can be found [in the AWS documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-lambda-function-code-cfnresponsemodule.html#w2ab1c23c23c16b9c15)
 and in the [awslabs GitHub repo](https://github.com/awslabs/aws-cloudformation-templates/blob/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py)
 
 You can compare the code in `awslabs` with this pypi package with this command
 
 ```
 if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(curl -s https://raw.githubusercontent.com/gene1wood/cfnresponse/master/cfnresponse/__init__.py | sha256sum)" ]; then echo "GitHub matches AWS"; fi
-if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(wget --quiet https://files.pythonhosted.org/packages/91/1c/99d3119ee59205ef321e48ecaf3a3bb92fe6de6d3d5ec296e9025975061c/cfnresponse-1.1.1-py2.py3-none-any.whl && unzip -p cfnresponse-1.1.1-py2.py3-none-any.whl cfnresponse/__init__.py | sha256sum && rm cfnresponse-1.1.1-py2.py3-none-any.whl)" ]; then echo "Pypi matches AWS"; fi
+if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(wget --quiet https://files.pythonhosted.org/packages/03/69/2d3fafdf434a0d8ef62a5c1fa09feda25b31fad4db20c54ed067054f9b95/cfnresponse-1.1.2-py2.py3-none-any.whl && unzip -p cfnresponse-1.1.2-py2.py3-none-any.whl cfnresponse/__init__.py | sha256sum && rm cfnresponse-1.1.2-py2.py3-none-any.whl)" ]; then echo "Pypi matches AWS"; fi
 ```
 
 This module [used to use the vendored version of `requests`](https://github.com/awslabs/aws-cloudformation-templates/blob/dd484dd32680fcbfc52b34de45923f78b5626e39/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py)
 provided by `botocore` but this changed in 
 [April 2020](https://github.com/awslabs/aws-cloudformation-templates/commit/44b76a1f694f82eeee14fe804bf9dc973fdc2230#diff-f6c57142d56d8704aaf1d429ff1a06a6dd3f2ee6d80f0572ada8af010ff17124)
 to instead use `urllib3` as
 [`botocore.vendored.requests` was removed](https://github.com/boto/botocore/pull/1829).
-
```

### Comparing `cfnresponse-1.1.2/README.md` & `cfnresponse-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # cfnresponse
 
 This package contains the Amazon Web Services (AWS) cfnresponse module which is
 available in Python AWS Lambda environments.
 
-The code for this module can be found [in the Lambda Function Code documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-lambda-function-code.html#cfn-lambda-function-code-cfnresponsemodule)
+The code for this module can be found [in the AWS documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-lambda-function-code-cfnresponsemodule.html#w2ab1c23c23c16b9c15)
 and in the [awslabs GitHub repo](https://github.com/awslabs/aws-cloudformation-templates/blob/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py)
 
 You can compare the code in `awslabs` with this pypi package with this command
 
 ```
 if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(curl -s https://raw.githubusercontent.com/gene1wood/cfnresponse/master/cfnresponse/__init__.py | sha256sum)" ]; then echo "GitHub matches AWS"; fi
-if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(wget --quiet https://files.pythonhosted.org/packages/91/1c/99d3119ee59205ef321e48ecaf3a3bb92fe6de6d3d5ec296e9025975061c/cfnresponse-1.1.1-py2.py3-none-any.whl && unzip -p cfnresponse-1.1.1-py2.py3-none-any.whl cfnresponse/__init__.py | sha256sum && rm cfnresponse-1.1.1-py2.py3-none-any.whl)" ]; then echo "Pypi matches AWS"; fi
+if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(wget --quiet https://files.pythonhosted.org/packages/03/69/2d3fafdf434a0d8ef62a5c1fa09feda25b31fad4db20c54ed067054f9b95/cfnresponse-1.1.2-py2.py3-none-any.whl && unzip -p cfnresponse-1.1.2-py2.py3-none-any.whl cfnresponse/__init__.py | sha256sum && rm cfnresponse-1.1.2-py2.py3-none-any.whl)" ]; then echo "Pypi matches AWS"; fi
 ```
 
 This module [used to use the vendored version of `requests`](https://github.com/awslabs/aws-cloudformation-templates/blob/dd484dd32680fcbfc52b34de45923f78b5626e39/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py)
 provided by `botocore` but this changed in 
 [April 2020](https://github.com/awslabs/aws-cloudformation-templates/commit/44b76a1f694f82eeee14fe804bf9dc973fdc2230#diff-f6c57142d56d8704aaf1d429ff1a06a6dd3f2ee6d80f0572ada8af010ff17124)
 to instead use `urllib3` as
-[`botocore.vendored.requests` was removed](https://github.com/boto/botocore/pull/1829).
+[`botocore.vendored.requests` was removed](https://github.com/boto/botocore/pull/1829).
```

### Comparing `cfnresponse-1.1.2/cfnresponse/__init__.py` & `cfnresponse-1.1.3/cfnresponse/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import urllib3
 import json
 http = urllib3.PoolManager()
 SUCCESS = "SUCCESS"
 FAILED = "FAILED"
 
-def send(event, context, responseStatus, responseData, physicalResourceId=None, noEcho=False):
+def send(event, context, responseStatus, responseData, physicalResourceId=None, noEcho=False, reason=None):
     responseUrl = event['ResponseURL']
 
     print(responseUrl)
 
     responseBody = {}
     responseBody['Status'] = responseStatus
-    responseBody['Reason'] = 'See the details in CloudWatch Log Stream: ' + context.log_stream_name
+    responseBody['Reason'] = reason or 'See the details in CloudWatch Log Stream: ' + context.log_stream_name
     responseBody['PhysicalResourceId'] = physicalResourceId or context.log_stream_name
     responseBody['StackId'] = event['StackId']
     responseBody['RequestId'] = event['RequestId']
     responseBody['LogicalResourceId'] = event['LogicalResourceId']
     responseBody['NoEcho'] = noEcho
     responseBody['Data'] = responseData
 
@@ -28,12 +28,12 @@
 
     headers = {
         'content-type' : '',
         'content-length' : str(len(json_responseBody))
     }
 
     try:
-        
+
         response = http.request('PUT',responseUrl,body=json_responseBody.encode('utf-8'),headers=headers)
         print("Status code: " + response.reason)
     except Exception as e:
         print("send(..) failed executing requests.put(..): " + str(e))
```

### Comparing `cfnresponse-1.1.2/cfnresponse.egg-info/PKG-INFO` & `cfnresponse-1.1.3/cfnresponse.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: cfnresponse
-Version: 1.1.2
+Version: 1.1.3
 Summary: Send a response object to a custom resource by way of an Amazon S3 presigned URL
 Home-page: https://github.com/gene1wood/cfnresponse
 Author: Amazon Web Services
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3
 
 # cfnresponse
 
 This package contains the Amazon Web Services (AWS) cfnresponse module which is
 available in Python AWS Lambda environments.
 
-The code for this module can be found [in the Lambda Function Code documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-lambda-function-code.html#cfn-lambda-function-code-cfnresponsemodule)
+The code for this module can be found [in the AWS documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-lambda-function-code-cfnresponsemodule.html#w2ab1c23c23c16b9c15)
 and in the [awslabs GitHub repo](https://github.com/awslabs/aws-cloudformation-templates/blob/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py)
 
 You can compare the code in `awslabs` with this pypi package with this command
 
 ```
 if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(curl -s https://raw.githubusercontent.com/gene1wood/cfnresponse/master/cfnresponse/__init__.py | sha256sum)" ]; then echo "GitHub matches AWS"; fi
-if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(wget --quiet https://files.pythonhosted.org/packages/91/1c/99d3119ee59205ef321e48ecaf3a3bb92fe6de6d3d5ec296e9025975061c/cfnresponse-1.1.1-py2.py3-none-any.whl && unzip -p cfnresponse-1.1.1-py2.py3-none-any.whl cfnresponse/__init__.py | sha256sum && rm cfnresponse-1.1.1-py2.py3-none-any.whl)" ]; then echo "Pypi matches AWS"; fi
+if [ "$(curl -s https://raw.githubusercontent.com/awslabs/aws-cloudformation-templates/master/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py | sha256sum)" = "$(wget --quiet https://files.pythonhosted.org/packages/03/69/2d3fafdf434a0d8ef62a5c1fa09feda25b31fad4db20c54ed067054f9b95/cfnresponse-1.1.2-py2.py3-none-any.whl && unzip -p cfnresponse-1.1.2-py2.py3-none-any.whl cfnresponse/__init__.py | sha256sum && rm cfnresponse-1.1.2-py2.py3-none-any.whl)" ]; then echo "Pypi matches AWS"; fi
 ```
 
 This module [used to use the vendored version of `requests`](https://github.com/awslabs/aws-cloudformation-templates/blob/dd484dd32680fcbfc52b34de45923f78b5626e39/aws/services/CloudFormation/MacrosExamples/StackMetrics/lambda/cfnresponse.py)
 provided by `botocore` but this changed in 
 [April 2020](https://github.com/awslabs/aws-cloudformation-templates/commit/44b76a1f694f82eeee14fe804bf9dc973fdc2230#diff-f6c57142d56d8704aaf1d429ff1a06a6dd3f2ee6d80f0572ada8af010ff17124)
 to instead use `urllib3` as
 [`botocore.vendored.requests` was removed](https://github.com/boto/botocore/pull/1829).
-
```

### Comparing `cfnresponse-1.1.2/setup.py` & `cfnresponse-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cfnresponse",
-    version="1.1.2",
+    version="1.1.3",
     author="Amazon Web Services",
     description="Send a response object to a custom resource by way of an Amazon S3 presigned URL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gene1wood/cfnresponse",
     packages=setuptools.find_packages(),
     classifiers=[
```

