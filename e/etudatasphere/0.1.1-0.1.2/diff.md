# Comparing `tmp/etudatasphere-0.1.1.tar.gz` & `tmp/etudatasphere-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etudatasphere-0.1.1.tar", last modified: Tue Apr  2 17:11:03 2024, max compression
+gzip compressed data, was "etudatasphere-0.1.2.tar", last modified: Sat Apr  6 10:08:10 2024, max compression
```

## Comparing `etudatasphere-0.1.1.tar` & `etudatasphere-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/
--rw-rw-rw-   0        0        0     1110 2024-03-27 19:34:50.000000 etudatasphere-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      976 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-27 19:48:47.000000 etudatasphere-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 17:11:03.707794 etudatasphere-0.1.1/etudatasphere/
--rw-rw-rw-   0        0        0     8082 2024-04-02 17:05:48.000000 etudatasphere-0.1.1/etudatasphere/DataSphereManager.py
--rw-rw-rw-   0        0        0       50 2024-04-02 17:06:36.000000 etudatasphere-0.1.1/etudatasphere/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/etudatasphere.egg-info/
--rw-rw-rw-   0        0        0      976 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1332 2024-04-02 17:10:55.000000 etudatasphere-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/
+-rw-rw-rw-   0        0        0     1110 2024-03-27 19:34:50.000000 etudatasphere-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5803 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4765 2024-04-06 10:07:41.000000 etudatasphere-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.747349 etudatasphere-0.1.2/etudatasphere/
+-rw-rw-rw-   0        0        0     7745 2024-04-06 09:34:48.000000 etudatasphere-0.1.2/etudatasphere/DataSphereManager.py
+-rw-rw-rw-   0        0        0       50 2024-04-02 17:06:36.000000 etudatasphere-0.1.2/etudatasphere/__init__.py
+-rw-rw-rw-   0        0        0     1299 2024-04-05 20:14:18.000000 etudatasphere-0.1.2/etudatasphere/exceptions.py
+-rw-rw-rw-   0        0        0     2088 2024-04-06 09:17:14.000000 etudatasphere-0.1.2/etudatasphere/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/etudatasphere.egg-info/
+-rw-rw-rw-   0        0        0     5803 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 10:08:10.000000 etudatasphere-0.1.2/etudatasphere.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1432 2024-04-06 10:02:35.000000 etudatasphere-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:08:10.762958 etudatasphere-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1616 2024-04-06 10:01:22.000000 etudatasphere-0.1.2/tests/test_etudatasphere.py
```

### Comparing `etudatasphere-0.1.1/LICENSE` & `etudatasphere-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etudatasphere-0.1.1/etudatasphere/DataSphereManager.py` & `etudatasphere-0.1.2/etudatasphere/DataSphereManager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,197 +1,140 @@
 import requests
-import traceback
 import json
+from etudatasphere.exceptions import BadProjectRequest, BadStatusCode
+from etudatasphere.utils import parse_projects, ProjectSettings
 
 
-def handle_exceptions(func):
-    def wrapper(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except Exception as e:
-            print(f"Exception occurred: {e}")
-            print(f"Exception {traceback.format_exc()}")
+def request_iam_token(oauth_token):
+    url = "https://iam.api.cloud.yandex.net/iam/v1/tokens"
+    headers = {"Authorization": f"OAuth {oauth_token}"}
+    payload = {"yandexPassportOauthToken": oauth_token}
 
-    return wrapper
+    res = requests.post(url, headers=headers, json=payload)
 
+    if res.status_code != 200:
+        raise BadStatusCode(res.status_code, res.text)
+    else:
+        response_json = res.json()
+        return response_json.get("iamToken")
 
-class BadStatusCode(Exception):
-    def __init__(self, status_code, message="Bad request"):
-        self.status_code = status_code
-        if status_code == 401:
-            self.message = f"Check or update your IAM Token. Status code = {status_code}"
-        if status_code == 404:
-            self.message = f"{message}. Status code = {status_code}"
-        super().__init__(self.message)
-
-
-class BadProjectRequest(Exception):
-    def __init__(self, project_id, community_id):
-        self.project_id = project_id
-        self.community_id = community_id
-        if self.project_id and self.community_id:
-            self.message = 'Use only one of the available options'
-        if (not self.project_id) and (not self.community_id):
-            self.message = 'One of the parameters must be present'
-        super().__init__(self.message)
-
-
-class ProjectSettings():
-    settings = ('vmInactivityTimeout')
-    limits = ('maxUnitsPerHour', 'maxUnitsPerExecution')
-
-    def __init__(self, community_id: str,
-                 name: str,
-                 maxUnitsPerHour: int = None,
-                 maxUnitsPerExecution: int = None,
-                 description: str = None,
-                 vmInactivityTimeout: str = "300s") -> dict:
-        self.community_id = community_id
-        self.name = name
-        if description:
-            self.description = description
-        if maxUnitsPerHour:
-            self.maxUnitsPerHour = maxUnitsPerHour
-        if maxUnitsPerExecution:
-            self.maxUnitsPerExecution = maxUnitsPerExecution
-        if vmInactivityTimeout:
-            self.vmInactivityTimeout = vmInactivityTimeout
-
-    def to_dict(self):
-        base_dict = {}
-        settings_dict = {}
-        limits_dict = {}
-        for key, value in self.__dict__.items():
-            if not (key.startswith('_') or key.endswith('__') or callable(
-                    key)):
-                if key in self.settings:
-                    settings_dict[key] = value
-                elif key in self.limits:
-                    limits_dict[key] = value
-                else:
-                    base_dict[key] = value
-        if settings_dict:
-            base_dict['settings'] = settings_dict
-        if limits_dict:
-            base_dict['limits'] = limits_dict
-        return base_dict
 
+class DataSphereManager:
 
-class DataSphereManager():
-
-    def __init__(self, iam_token: str) -> None:
+    def __init__(self, oauth_token: str) -> None:
+        iam_token = request_iam_token(oauth_token)
         self.HEADERS = {"Authorization": "Bearer {}".format(iam_token)}
 
-    @handle_exceptions
     def __make_get_request(self, url, params=None):
         res = requests.get(url, headers=self.HEADERS, params=params)
         if res.status_code != 200:
-            raise BadStatusCode(res.status_code)
+            raise BadStatusCode(res.status_code, res.text)
         else:
             return res
 
-    @handle_exceptions
     def __make_post_request(self, url, data):
         res = requests.post(url, headers=self.HEADERS, data=json.dumps(data))
         if res.status_code != 200:
-            raise BadStatusCode(res.status_code)
+            raise BadStatusCode(res.status_code, res.text)
+        else:
+            return res
+
+    def __make_patch_request(self, url, data):
+        res = requests.patch(url, headers=self.HEADERS, data=json.dumps(data))
+        if res.status_code != 200:
+            raise BadStatusCode(res.status_code, res.text)
         else:
             return res
 
-    @handle_exceptions
     def get_organizations(self):
 
         url = "https://resource-manager.api.cloud.yandex.net/resource-manager/v1/clouds"
         res = self.__make_get_request(url)
         orgs = res.json()['clouds']
 
         for org in orgs:
             print('NAME', org['name'])
             print('ID', org['organizationId'])
             print('*' * 25)
 
-    @handle_exceptions
+    def get_unit_balance(self, project_id):
+        url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/projects/{}:unitBalance".format(project_id)
+        res = self.__make_get_request(url)
+        return res.json()
+
     def get_billing_accounts(self):
         url = "https://billing.api.cloud.yandex.net/billing/v1/billingAccounts"
         res = self.__make_get_request(url)
         return res.json()
 
-    @handle_exceptions
     def get_possible_ds_roles(self):
         url = "https://iam.api.cloud.yandex.net/iam/v1/roles"
         res = self.__make_get_request(url)
         roles = res.json()['roles']
         return [role for role in roles if 'datasphere' in role['id']]
 
-    @handle_exceptions
     def get_organization_members(self, org_id: str):
 
         url = "https://organization-manager.api.cloud.yandex.net/organization-manager/v1/organizations/{}/users".format(
             org_id)
         res = self.__make_get_request(url)
         users = res.json()['users']
         for user in users:
             print('NAME', user['subjectClaims']['name'])
             print('ID', user['subjectClaims']['sub'])
             print('*' * 25)
 
-    @handle_exceptions
     def get_organization_communities(self, organization_id: str):
         url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/communities"
         params = {
             "organizationId": organization_id
         }
         res = self.__make_get_request(url, params)
         return res.json()
 
-    @handle_exceptions
     def create_project(self,
                        community_id: str,
                        name: str,
                        description: str = None,
-                       maxUnitsPerHour: int = None,
-                       maxUnitsPerExecution: int = None,
-                       vmInactivityTimeout: str = "300s"):
+                       vmInactivityTimeout: str = "1800s"):
         data = ProjectSettings(
             community_id=community_id,
             name=name,
             description=description,
-            maxUnitsPerHour=maxUnitsPerHour,
-            maxUnitsPerExecution=maxUnitsPerExecution,
             vmInactivityTimeout=vmInactivityTimeout
         ).to_dict()
         url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/projects"
         res = self.__make_post_request(url, data)
         return res.json()
 
-    @handle_exceptions
     def check_operation_status(self, id_operation: str):
         url = "https://operation.api.cloud.yandex.net/operations/{}".format(id_operation)
         res = self.__make_get_request(url)
         return res.json()
 
-    @handle_exceptions
-    def get_projects(self, project_id: str = None, community_id: str = None):
+    def get_projects(self, project_id: str = None, community_id: str = None, parse_projects_flag=False):
         if (community_id and project_id) or (
                 (not project_id) and (not community_id)
         ):
             raise BadProjectRequest(community_id, project_id)
 
         if community_id:
             params = {
                 "communityId": community_id
             }
         else:
             params = None
         url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/projects/{}".format(
             project_id if project_id else "")
         res = self.__make_get_request(url, params)
-        return res.json()
+        if parse_projects_flag:
+            return parse_projects(res.json())
+        else:
+            return res.json()
 
-    @handle_exceptions
     def add_contributors(self, project_id, contributors: list[dict]):
         """
         project_id: str - ID of project
         contributors: list[dict] - The list of contributors to add
             format:
                 [
                     {
@@ -204,23 +147,58 @@
                     }
                 ]
         """
 
         if not contributors:
             return 'No participants selected'
         else:
-            data = {}
-            data['accessBindings'] = []
+            data = {'accessBindings': []}
 
             for user in contributors:
                 data['accessBindings'].append({
                     "roleId": user['role'],
                     "subject": {
                         "id": user['id'],
                         "type": "userAccount"
                     }
                 })
         url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/projects/{}:setAccessBindings". \
             format(project_id)
 
         res = self.__make_post_request(url, data)
         return res.json()
+
+    def update_unit_balance(self, project_id, new_unit_balance):
+        url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/projects/{}:unitBalance".format(project_id)
+        data = {"unitBalance": new_unit_balance}
+        res = self.__make_post_request(url, data)
+        return res.json()
+
+    def update_all_community_projects(self,
+                                      community_id: str,
+                                      vmInactivityTimeout: str = "1000s",
+                                      unit_balance: int = None):
+        data = ProjectSettings(
+            vmInactivityTimeout=vmInactivityTimeout
+        ).to_dict()
+
+        projects = self.get_projects(community_id=community_id)
+
+        updateMask_list = []
+        for k, v in data.items():
+            for n in v.keys():
+                updateMask_list.append(f"{k}.{n}")
+        data['updateMask'] = ', '.join(updateMask_list)
+
+        try:
+            for idx, project in enumerate(projects['projects']):
+                print(f"{idx + 1}/{len(projects['projects'])}")
+                url = "https://datasphere.api.cloud.yandex.net/datasphere/v2/projects/{}".format(project.get('id'))
+                res = self.__make_patch_request(url, data)
+                print('Operation id:', res.json()['id'])
+
+                if unit_balance is not None:
+                    self.update_unit_balance(project.get('id'), unit_balance)
+
+            return 'ok'
+        except Exception as e:
+            raise e
```

### Comparing `etudatasphere-0.1.1/setup.py` & `etudatasphere-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import open
 from setuptools import setup
 
-version = '0.1.1'
+version = '0.1.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='etudatasphere',
     version=version,
@@ -26,14 +26,20 @@
     ),
 
     license='MIT License, see LICENSE file',
 
     packages=['etudatasphere'],
     install_requires=['requests'],
 
+    extras_require={
+            'dev': [
+                'pytest',
+            ]
+        },
+
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

