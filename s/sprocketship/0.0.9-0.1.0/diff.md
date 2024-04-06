# Comparing `tmp/sprocketship-0.0.9.tar.gz` & `tmp/sprocketship-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.9.tar", last modified: Fri Apr  5 17:44:43 2024, max compression
+gzip compressed data, was "sprocketship-0.1.0.tar", last modified: Sat Apr  6 15:37:50 2024, max compression
```

## Comparing `sprocketship-0.0.9.tar` & `sprocketship-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:44:43.652487 sprocketship-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 17:44:36.000000 sprocketship-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-05 17:44:43.652487 sprocketship-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-05 17:44:36.000000 sprocketship-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:44:36.000000 sprocketship-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:44:43.652487 sprocketship-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:44:43.648487 sprocketship-0.0.9/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 17:44:36.000000 sprocketship-0.0.9/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:44:43.652487 sprocketship-0.0.9/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 17:44:43.000000 sprocketship-0.0.9/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.293699 sprocketship-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 15:37:46.000000 sprocketship-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:37:46.000000 sprocketship-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 15:37:50.293699 sprocketship-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-06 15:37:46.000000 sprocketship-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 15:37:46.000000 sprocketship-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:37:50.293699 sprocketship-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.289699 sprocketship-0.1.0/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-06 15:37:46.000000 sprocketship-0.1.0/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.293699 sprocketship-0.1.0/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 15:37:46.000000 sprocketship-0.1.0/sprocketship/templates/javascript.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:37:50.293699 sprocketship-0.1.0/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 15:37:50.000000 sprocketship-0.1.0/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.9/LICENSE` & `sprocketship-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.9/PKG-INFO` & `sprocketship-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: sprocketship
-Version: 0.0.9
-Summary: Better stored procedure management
-Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
-Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: snowflake
-Requires-Dist: ABSQL
-Requires-Dist: ruamel.yaml
-Requires-Dist: jinja2
-
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -130,38 +112,63 @@
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
 procedures:
   development:
     - name: create_temp_database
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
     - name: create_database_reader
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
     - name: create_database_writer
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
+### Exhaustive Options for Stored Procedure Configuration
+
+```
+name: The name of the procedure
+database: The name of the database where the procedure will be stored
+schema: The name of the schema where the procedure will be stored
+language: The language of the procedure definition
+execute_as: caller or owner
+args:
+    - name: Name of argument
+      type: Type of argument
+      default: (Optional) default value for the argument
+returns: The return type
+comment: Explanation of the procedure
+```
+
+## Support
+
+sprocketship currently only supports Javascript-based stored procedures (Python support coming soon!). Additionally, there are a few options from the `CREATE STORED PROCEDURE` function that are not yet supported:
+
+* `RETURNS <result-data-type> NOT NULL`
+* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }`
+* `VOLATILE | IMMUTABLE` (deprecated)
+
+
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,19 +1,10 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.9 Summary: Better stored
-procedure management Author-email: Nicklaus Roacb
-gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
-Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
-url]
+[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -33,24 +24,34 @@
 dbt_models â âââ customers.sql â âââ products.sql âââ
 procedures â âââ admin â â âââ create_database_writer_role.js
 â â âââ create_database_reader_role.js â âââ development â
 â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
 path to each procedure in the `sprocketship.yml` should follow that of the
 paths to their corresponding files in the `procedures/` directory. ```
 procedures: development: - name: create_temp_database replace_if_exists: true
-database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
-('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
-replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
-replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `$ sprocketship
-liftoff` from the project directory (or provide the directory, e.g.
-`sprocketship liftoff my/directory/path`) and sprocketship will launch your
-stored procedures into the given directory. ## License Distributed under the
-MIT License. See `LICENSE` for more information.
+database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
+admin: - name: create_database_reader replace_if_exists: true database:
+!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... - name:
+create_database_writer replace_if_exists: true database: !env_var
+SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
+run `$ sprocketship liftoff` from the project directory (or provide the
+directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
+launch your stored procedures into the given directory. ### Exhaustive Options
+for Stored Procedure Configuration ``` name: The name of the procedure
+database: The name of the database where the procedure will be stored schema:
+The name of the schema where the procedure will be stored language: The
+language of the procedure definition execute_as: caller or owner args: - name:
+Name of argument type: Type of argument default: (Optional) default value for
+the argument returns: The return type comment: Explanation of the procedure ```
+## Support sprocketship currently only supports Javascript-based stored
+procedures (Python support coming soon!). Additionally, there are a few options
+from the `CREATE STORED PROCEDURE` function that are not yet supported: *
+`RETURNS NOT NULL` * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT |
+STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License Distributed under
+the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-0.0.9/README.md` & `sprocketship-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sprocketship
+Version: 0.1.0
+Summary: Better stored procedure management
+Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
+Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: snowflake
+Requires-Dist: ABSQL
+Requires-Dist: ruamel.yaml
+Requires-Dist: jinja2
+
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -112,38 +130,63 @@
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
 procedures:
   development:
     - name: create_temp_database
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
     - name: create_database_reader
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
     - name: create_database_writer
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
+### Exhaustive Options for Stored Procedure Configuration
+
+```
+name: The name of the procedure
+database: The name of the database where the procedure will be stored
+schema: The name of the schema where the procedure will be stored
+language: The language of the procedure definition
+execute_as: caller or owner
+args:
+    - name: Name of argument
+      type: Type of argument
+      default: (Optional) default value for the argument
+returns: The return type
+comment: Explanation of the procedure
+```
+
+## Support
+
+sprocketship currently only supports Javascript-based stored procedures (Python support coming soon!). Additionally, there are a few options from the `CREATE STORED PROCEDURE` function that are not yet supported:
+
+* `RETURNS <result-data-type> NOT NULL`
+* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }`
+* `VOLATILE | IMMUTABLE` (deprecated)
+
+
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,10 +1,19 @@
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.0 Summary: Better stored
+procedure management Author-email: Nicklaus Roacb
+gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
+Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
+[Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
+url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -24,24 +33,34 @@
 dbt_models â âââ customers.sql â âââ products.sql âââ
 procedures â âââ admin â â âââ create_database_writer_role.js
 â â âââ create_database_reader_role.js â âââ development â
 â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
 path to each procedure in the `sprocketship.yml` should follow that of the
 paths to their corresponding files in the `procedures/` directory. ```
 procedures: development: - name: create_temp_database replace_if_exists: true
-database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
-('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
-replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
-replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `$ sprocketship
-liftoff` from the project directory (or provide the directory, e.g.
-`sprocketship liftoff my/directory/path`) and sprocketship will launch your
-stored procedures into the given directory. ## License Distributed under the
-MIT License. See `LICENSE` for more information.
+database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
+admin: - name: create_database_reader replace_if_exists: true database:
+!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... - name:
+create_database_writer replace_if_exists: true database: !env_var
+SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
+run `$ sprocketship liftoff` from the project directory (or provide the
+directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
+launch your stored procedures into the given directory. ### Exhaustive Options
+for Stored Procedure Configuration ``` name: The name of the procedure
+database: The name of the database where the procedure will be stored schema:
+The name of the schema where the procedure will be stored language: The
+language of the procedure definition execute_as: caller or owner args: - name:
+Name of argument type: Type of argument default: (Optional) default value for
+the argument returns: The return type comment: Explanation of the procedure ```
+## Support sprocketship currently only supports Javascript-based stored
+procedures (Python support coming soon!). Additionally, there are a few options
+from the `CREATE STORED PROCEDURE` function that are not yet supported: *
+`RETURNS NOT NULL` * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT |
+STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License Distributed under
+the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-0.0.9/pyproject.toml` & `sprocketship-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
@@ -24,8 +24,8 @@
 ]
 
 [project.scripts]
 sprocketship = "sprocketship.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/nicklausroach/sprocketship"
-Issues = "https://github.com/pypa/nicklausroach/sprocketship"
+Issues = "https://github.com/pypa/nicklausroach/sprocketship"
```

### Comparing `sprocketship-0.0.9/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.1.0/sprocketship.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.9
+Version: 0.1.0
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -130,38 +130,63 @@
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
 procedures:
   development:
     - name: create_temp_database
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
     - name: create_database_reader
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
     - name: create_database_writer
       replace_if_exists: true
-      database: {{ env.get('SNOWFLAKE_DATABASE') }}
-      schema: {{ env.get('SNOWFLAKE_SCHEMA') }}
+      database: !env_var SNOWFLAKE_DATABASE
+      schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
+### Exhaustive Options for Stored Procedure Configuration
+
+```
+name: The name of the procedure
+database: The name of the database where the procedure will be stored
+schema: The name of the schema where the procedure will be stored
+language: The language of the procedure definition
+execute_as: caller or owner
+args:
+    - name: Name of argument
+      type: Type of argument
+      default: (Optional) default value for the argument
+returns: The return type
+comment: Explanation of the procedure
+```
+
+## Support
+
+sprocketship currently only supports Javascript-based stored procedures (Python support coming soon!). Additionally, there are a few options from the `CREATE STORED PROCEDURE` function that are not yet supported:
+
+* `RETURNS <result-data-type> NOT NULL`
+* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }`
+* `VOLATILE | IMMUTABLE` (deprecated)
+
+
 <!-- LICENSE -->
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.9 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.0 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
@@ -33,24 +33,34 @@
 dbt_models â âââ customers.sql â âââ products.sql âââ
 procedures â âââ admin â â âââ create_database_writer_role.js
 â â âââ create_database_reader_role.js â âââ development â
 â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
 path to each procedure in the `sprocketship.yml` should follow that of the
 paths to their corresponding files in the `procedures/` directory. ```
 procedures: development: - name: create_temp_database replace_if_exists: true
-database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {{ env.get
-('SNOWFLAKE_SCHEMA') }} ... admin: - name: create_database_reader
-replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... - name: create_database_writer
-replace_if_exists: true database: {{ env.get('SNOWFLAKE_DATABASE') }} schema: {
-{ env.get('SNOWFLAKE_SCHEMA') }} ... ``` From here, simply run `$ sprocketship
-liftoff` from the project directory (or provide the directory, e.g.
-`sprocketship liftoff my/directory/path`) and sprocketship will launch your
-stored procedures into the given directory. ## License Distributed under the
-MIT License. See `LICENSE` for more information.
+database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
+admin: - name: create_database_reader replace_if_exists: true database:
+!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... - name:
+create_database_writer replace_if_exists: true database: !env_var
+SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
+run `$ sprocketship liftoff` from the project directory (or provide the
+directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
+launch your stored procedures into the given directory. ### Exhaustive Options
+for Stored Procedure Configuration ``` name: The name of the procedure
+database: The name of the database where the procedure will be stored schema:
+The name of the schema where the procedure will be stored language: The
+language of the procedure definition execute_as: caller or owner args: - name:
+Name of argument type: Type of argument default: (Optional) default value for
+the argument returns: The return type comment: Explanation of the procedure ```
+## Support sprocketship currently only supports Javascript-based stored
+procedures (Python support coming soon!). Additionally, there are a few options
+from the `CREATE STORED PROCEDURE` function that are not yet supported: *
+`RETURNS NOT NULL` * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT |
+STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License Distributed under
+the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

