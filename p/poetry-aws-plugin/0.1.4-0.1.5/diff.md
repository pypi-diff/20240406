# Comparing `tmp/poetry_aws_plugin-0.1.4.tar.gz` & `tmp/poetry_aws_plugin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.4.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.5.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.4.tar` & `poetry_aws_plugin-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.4/LICENSE
--rw-r--r--   0        0        0     2634 2024-04-05 23:55:14.069809 poetry_aws_plugin-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.4/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     6634 2024-04-05 23:53:51.981806 poetry_aws_plugin-0.1.4/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-05 23:56:08.545811 poetry_aws_plugin-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2634 2024-04-05 23:55:14.069809 poetry_aws_plugin-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.5/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     6606 2024-04-06 00:14:58.477846 poetry_aws_plugin-0.1.5/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-06 00:08:26.653834 poetry_aws_plugin-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.5/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.4/LICENSE` & `poetry_aws_plugin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.4/README.md` & `poetry_aws_plugin-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.4/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.5/poetry_aws_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 POETRY_AWS_PLUGIN_ROLE_ARN_VAR = "POETRY_AWS_PLUGIN_ROLE_ARN"
 POETRY_AWS_PLUGIN_SESSION_NAME = "poetry-aws-plugin"
 POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR = "POETRY_AWS_PLUGIN_AUTH_TOKEN"
 
 UNAUTHORIZED_STATUS_CODES = (401, 403)
 CODEARTIFACT_URL_REGEX = r"^https://([a-z][a-z-]*)-(\d+)\.d\.codeartifact\.[^.]+\.amazonaws\.com/.*$"
 
-RETRY_ERROR_MESSAGE = f"""\
+RETRY_ERROR_MESSAGE = f"""
 Make sure you have AWS credentials configured and up-to-date
 
 Then make sure you have atleast one of the following:
     1. Authorization for CodeArtifact with your current credentials
     2. Authorization for an IAM role that has access to CodeArtifact and
        environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' set to that role's ARN
-
 """
 
 
 def patch(io: IO):
     request = Authenticator.request
 
     def is_retryable(response: requests.Response) -> bool:
@@ -42,45 +41,46 @@
         return True
 
     def validate_credentials() -> bool:
         try:
             boto3.client("sts").get_caller_identity()
             return True
         except ClientError as err:
-            io.write_line(f"\nError using current credentials: {err}\n")
+            io.write_line(f"Error using current credentials: {err}")
             return False
         except Exception as err:
-            io.write_line("Unexpected error while validating AWS credentials\n")
+            io.write_line("Unexpected error while validating AWS credentials")
             io.write_line(RETRY_ERROR_MESSAGE)
             raise err
 
     def get_auth_token_with_current_credentials(domain: str, domain_owner: str) -> str:
         try:
             token_response = boto3.client("codeartifact").get_authorization_token(
                 domain=domain,
                 domainOwner=domain_owner,
             )
             return token_response["authorizationToken"]
         except ClientError as err:
             io.write_line(
-                f"\nError getting CodeArtifact token using current credentials: {err}\n",
+                f"Error getting CodeArtifact token using current credentials: {err}",
                 verbosity=Verbosity.VERBOSE,
             )
-            return ""
         except Exception as err:
-            io.write_line("Unexpected error while getting CodeArtifact authorization token\n")
-            io.write_line(RETRY_ERROR_MESSAGE)
-            raise err
+            io.write_line(
+                f"Unexpected error while getting CodeArtifact authorization token: {err}",
+                verbosity=Verbosity.VERBOSE,
+            )
+        return ""
 
     def get_auth_token_with_iam_role(domain: str, domain_owner: str) -> str:
         role_arn = os.environ.get(POETRY_AWS_PLUGIN_ROLE_ARN_VAR)
         if not role_arn:
             io.write_line(
-                f"\nError getting CodeArtifact token using IAM role: "
-                f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found\n",
+                f"Error getting CodeArtifact token using IAM role: "
+                f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found",
                 verbosity=Verbosity.VERBOSE,
             )
             return ""
 
         try:
             assume_role_response = boto3.client("sts").assume_role(
                 RoleArn=role_arn,
@@ -96,32 +96,32 @@
             token_response = session.client("codeartifact").get_authorization_token(
                 domain=domain,
                 domainOwner=domain_owner,
             )
             return token_response["authorizationToken"]
         except ClientError as err:
             io.write_line(
-                f"\nError getting CodeArtifact token using IAM role '{role_arn}': {err}\n",
+                f"Error getting CodeArtifact token using IAM role '{role_arn}': {err}",
                 verbosity=Verbosity.VERBOSE,
             )
-            return ""
         except Exception as err:
             io.write_line(
-                "Unexpected error while assuming CodeArtifact role and getting CodeArtifact authorization token\n"
+                "Unexpected error while assuming CodeArtifact role "
+                f"and getting CodeArtifact authorization token: {err}",
+                verbosity=Verbosity.VERBOSE,
             )
-            io.write_line(RETRY_ERROR_MESSAGE)
-            raise err
+        return ""
 
     def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
         return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
     def get_auth_token(domain: str, domain_owner: str) -> str:
         io.write_line(
-            "\nGetting new CodeArtifact authorization token for "
-            f"domain '{domain}' and domain owner '{domain_owner}'\n",
+            "Getting new CodeArtifact authorization token for "
+            f"domain '{domain}' and domain owner '{domain_owner}'",
             verbosity=Verbosity.VERBOSE,
         )
 
         is_valid = validate_credentials()
         if not is_valid:
             return ""
 
@@ -145,27 +145,27 @@
         raise_for_status: bool = True,
         **kwargs: Any,
     ) -> requests.Response:
         response = request(self, method=method, url=url, raise_for_status=False, **kwargs)
 
         if is_retryable(response):
             io.write_line(
-                "\nFailed to get authorization for CodeArtifact\n",
+                "Failed to get authorization for CodeArtifact",
                 verbosity=Verbosity.VERBOSE,
             )
 
             match = re.match(CODEARTIFACT_URL_REGEX, response.url)
             domain, domain_owner = match.groups()
 
             auth_token = get_auth_token(domain, domain_owner)
             if not auth_token:
                 raise PoetryException(RETRY_ERROR_MESSAGE)
 
             io.write_line(
-                "\nSuccessfully got CodeArtifact authorization token!\n\nRetrying request...\n",
+                "Successfully got CodeArtifact authorization token! Retrying request...",
                 verbosity=Verbosity.VERBOSE,
             )
 
             # Overwrite the credentials for this URL
             self._credentials[url] = HTTPAuthCredential(username="aws", password=auth_token)
 
             # Now retry the original request with new credentials
```

### Comparing `poetry_aws_plugin-0.1.4/pyproject.toml` & `poetry_aws_plugin-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.4"
+version = "0.1.5"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.4/PKG-INFO` & `poetry_aws_plugin-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
```

