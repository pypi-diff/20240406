# Comparing `tmp/poetry_aws_plugin-0.1.3.tar.gz` & `tmp/poetry_aws_plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.3.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.4.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.3.tar` & `poetry_aws_plugin-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.3/LICENSE
--rw-r--r--   0        0        0     2634 2024-04-05 17:44:43.428417 poetry_aws_plugin-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.3/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     6487 2024-04-05 17:45:40.640420 poetry_aws_plugin-0.1.3/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-05 17:45:13.176419 poetry_aws_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2634 2024-04-05 23:55:14.069809 poetry_aws_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.4/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     6634 2024-04-05 23:53:51.981806 poetry_aws_plugin-0.1.4/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-05 23:56:08.545811 poetry_aws_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.4/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.3/LICENSE` & `poetry_aws_plugin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.3/README.md` & `poetry_aws_plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.3/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.4/poetry_aws_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         try:
             boto3.client("sts").get_caller_identity()
             return True
         except ClientError as err:
             io.write_line(f"\nError using current credentials: {err}\n")
             return False
         except Exception as err:
-            io.write_line("Unexpected error while validating AWS credentials")
+            io.write_line("Unexpected error while validating AWS credentials\n")
+            io.write_line(RETRY_ERROR_MESSAGE)
             raise err
 
     def get_auth_token_with_current_credentials(domain: str, domain_owner: str) -> str:
         try:
             token_response = boto3.client("codeartifact").get_authorization_token(
                 domain=domain,
                 domainOwner=domain_owner,
@@ -62,15 +63,16 @@
         except ClientError as err:
             io.write_line(
                 f"\nError getting CodeArtifact token using current credentials: {err}\n",
                 verbosity=Verbosity.VERBOSE,
             )
             return ""
         except Exception as err:
-            io.write_line("Unexpected error while getting CodeArtifact authorization token")
+            io.write_line("Unexpected error while getting CodeArtifact authorization token\n")
+            io.write_line(RETRY_ERROR_MESSAGE)
             raise err
 
     def get_auth_token_with_iam_role(domain: str, domain_owner: str) -> str:
         role_arn = os.environ.get(POETRY_AWS_PLUGIN_ROLE_ARN_VAR)
         if not role_arn:
             io.write_line(
                 f"\nError getting CodeArtifact token using IAM role: "
@@ -100,16 +102,17 @@
             io.write_line(
                 f"\nError getting CodeArtifact token using IAM role '{role_arn}': {err}\n",
                 verbosity=Verbosity.VERBOSE,
             )
             return ""
         except Exception as err:
             io.write_line(
-                "Unexpected error while assuming CodeArtifact role and getting CodeArtifact authorization token"
+                "Unexpected error while assuming CodeArtifact role and getting CodeArtifact authorization token\n"
             )
+            io.write_line(RETRY_ERROR_MESSAGE)
             raise err
 
     def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
         return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
     def get_auth_token(domain: str, domain_owner: str) -> str:
         io.write_line(
```

### Comparing `poetry_aws_plugin-0.1.3/pyproject.toml` & `poetry_aws_plugin-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.3"
+version = "0.1.4"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.3/PKG-INFO` & `poetry_aws_plugin-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
```

