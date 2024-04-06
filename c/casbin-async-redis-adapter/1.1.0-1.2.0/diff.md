# Comparing `tmp/casbin_async_redis_adapter-1.1.0.tar.gz` & `tmp/casbin_async_redis_adapter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_async_redis_adapter-1.1.0.tar", last modified: Fri Mar 29 10:09:55 2024, max compression
+gzip compressed data, was "casbin_async_redis_adapter-1.2.0.tar", last modified: Sat Apr  6 02:45:16 2024, max compression
```

## Comparing `casbin_async_redis_adapter-1.1.0.tar` & `casbin_async_redis_adapter-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:09:55.017662 casbin_async_redis_adapter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-03-29 10:09:55.017662 casbin_async_redis_adapter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:09:55.017662 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:09:55.017662 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-03-29 10:09:55.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-29 10:09:55.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 10:09:55.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-29 10:09:55.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-29 10:09:55.000000 casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-29 10:09:55.021662 casbin_async_redis_adapter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:09:55.017662 casbin_async_redis_adapter-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-03-29 10:09:27.000000 casbin_async_redis_adapter-1.1.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:45:16.926664 casbin_async_redis_adapter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-06 02:45:16.926664 casbin_async_redis_adapter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:45:16.922664 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:45:16.926664 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-06 02:45:16.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 02:45:16.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:45:16.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 02:45:16.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 02:45:16.000000 casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 02:45:16.926664 casbin_async_redis_adapter-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:45:16.926664 casbin_async_redis_adapter-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-04-06 02:44:42.000000 casbin_async_redis_adapter-1.2.0/tests/test_adapter.py
```

### Comparing `casbin_async_redis_adapter-1.1.0/LICENSE` & `casbin_async_redis_adapter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_async_redis_adapter-1.1.0/PKG-INFO` & `casbin_async_redis_adapter-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_async_redis_adapter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Async Redis Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-redis-adapter
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Redis,casbin-adapter,async,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `casbin_async_redis_adapter-1.1.0/README.md` & `casbin_async_redis_adapter-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter/adapter.py` & `casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter/adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         # else find all given rules and delete them
         if len(line.dict()) == 0:
             return 0
         else:
             await self.client.lrem(self.key, 0, json.dumps(line.dict()))
 
     async def save_policy(self, model) -> bool:
-        """Implement add Interface for casbin. Save the policy in mongodb
+        """Implement add Interface for casbin. Save the policy in redis
 
         Args:
             model (Class Model): Casbin Model which loads from .conf file usually.
 
         Returns:
             bool: True if succeed
         """
@@ -127,28 +127,58 @@
 
         Returns:
             bool: True if succeed else False
         """
         await self._save_policy_line(ptype, rule)
         return True
 
+    async def add_policies(self, sec, ptype, rules):
+        """AddPolicies adds policy rules to the storage.
+
+        Args:
+            sec (str): Section name, 'g' or 'p'
+            ptype (str): Policy type, 'g', 'g2', 'p', etc.
+            rules: Casbin rules will be added
+
+        Returns:
+            bool: True if succeed else False
+        """
+        for rule in rules:
+            await self.add_policy(sec, ptype, rule)
+        return True
+
     async def remove_policy(self, sec, ptype, rule):
         """Remove policy rules in redis(rules duplicate will all be removed)
 
         Args:
             sec (str): Section name, 'g' or 'p'
             ptype (str): Policy type, 'g', 'g2', 'p', etc.
             rule (CasbinRule): Casbin rule if it is exactly same as will be removed.
 
         Returns:
             bool: True if succeed else False
         """
         await self._delete_policy_lines(ptype, rule)
         return True
 
+    async def remove_policies(self, sec, ptype, rules):
+        """RemovePolicies removes policy rules from the storage.
+
+        Args:
+            sec (str): Section name, 'g' or 'p'
+            ptype (str): Policy type, 'g', 'g2', 'p', etc.
+            rules: Casbin rules will be removed
+
+        Returns:
+            bool: True if succeed else False
+        """
+        for rule in rules:
+            await self.remove_policy(sec, ptype, rule)
+        return True
+
     async def remove_filtered_policy(self, sec, ptype, field_index, *field_values):
         """Remove policy rules that match the filter from the storage.
            This is part of the Auto-Save feature.
 
         Args:
             sec (str): Section name, 'g' or 'p'
             ptype (str): Policy type, 'g', 'g2', 'p', etc.
@@ -179,7 +209,94 @@
                 else:
                     break
             if is_match:
                 await self.client.lset(self.key, i, "__CASBIN_DELETED__")
 
         await self.client.lrem(self.key, 0, "__CASBIN_DELETED__")
         return True
+
+    async def update_policy(self, sec, ptype, old_rule, new_rule):
+        """
+        update_policy updates a policy rule from storage.
+        This is part of the Auto-Save feature.
+
+        Args:
+            sec (str): Section name, 'g' or 'p'
+            ptype (str): Policy type, 'g', 'g2', 'p', etc.
+            old_rule: Casbin rule if it is exactly same as will be removed.
+            new_rule: Casbin rule if it is exactly same as will be added.
+
+        Returns:
+            bool: True if succeed else False
+        """
+        old_rule_obj = CasbinRule(ptype=ptype)
+        new_rule_obj = CasbinRule(ptype=ptype)
+        for index, value in enumerate(old_rule):
+            setattr(old_rule_obj, f"v{index}", value)
+        for index, value in enumerate(new_rule):
+            setattr(new_rule_obj, f"v{index}", value)
+
+        # Convert old_rule_obj and new_rule_obj to json
+        old_rule_json = json.dumps(old_rule_obj.dict())
+        new_rule_json = json.dumps(new_rule_obj.dict())
+
+        lua_script = """
+            local old_rule_json = ARGV[1]
+            local new_rule_json = ARGV[2]
+            local rules = redis.call('lrange', KEYS[1], 0, -1)
+            for i, rule_json in ipairs(rules) do
+                local rule = cjson.decode(rule_json)
+                if rule.ptype == ARGV[3] and rule_json == old_rule_json then
+                    redis.call('lset', KEYS[1], i-1, new_rule_json)
+                    return 1
+                end
+            end
+            return 0
+            """
+
+        result = await self.client.eval(
+            lua_script, 1, self.key, old_rule_json, new_rule_json, ptype
+        )
+
+        return result == 1
+
+    async def update_policies(self, sec, ptype, old_rules, new_rules):
+        """
+        UpdatePolicies updates some policy rules to storage, like db, redis.
+
+        Args:
+            sec (str): Section name, 'g' or 'p'
+            ptype (str): Policy type, 'g', 'g2', 'p', etc.
+            old_rules: Casbin rule if it is exactly same as will be removed.
+            new_rules: Casbin rule if it is exactly same as will be added.
+
+        Returns:
+            bool: True if succeed else False
+        """
+        for i in range(len(old_rules)):
+            await self.update_policy(sec, ptype, old_rules[i], new_rules[i])
+        return True
+
+    async def update_filtered_policies(
+        self, sec, ptype, new_rules, field_index, *field_values
+    ):
+        """
+        update_filtered_policies deletes old rules and adds new rules.
+
+        Args:
+            sec (str): Section name, 'g' or 'p'
+            ptype (str): Policy type, 'g', 'g2', 'p', etc.
+            new_rules: Casbin rule if it is exactly same as will be added.
+            field_index (int): The policy index at which the filed_values begins filtering. Its range is [0, 5]
+            field_values(List[str]): A list of rules to filter policy which starts from
+
+        Returns:
+            bool: True if succeed else False
+        """
+        if not (0 <= field_index <= 5):
+            return False
+        if not (1 <= field_index + len(field_values) <= 6):
+            return False
+
+        await self.remove_filtered_policy(sec, ptype, field_index, *field_values)
+        await self.add_policies(sec, ptype, new_rules)
+        return True
```

### Comparing `casbin_async_redis_adapter-1.1.0/casbin_async_redis_adapter.egg-info/PKG-INFO` & `casbin_async_redis_adapter-1.2.0/casbin_async_redis_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_async_redis_adapter
-Version: 1.1.0
+Version: 1.2.0
 Summary: Async Redis Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-redis-adapter
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Redis,casbin-adapter,async,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `casbin_async_redis_adapter-1.1.0/setup.py` & `casbin_async_redis_adapter-1.2.0/setup.py`

 * *Files identical despite different names*

