# Comparing `tmp/django-db-connection-pool-1.2.4.tar.gz` & `tmp/django-db-connection-pool-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-db-connection-pool-1.2.4.tar", last modified: Sat Jun 10 01:58:53 2023, max compression
+gzip compressed data, was "django-db-connection-pool-1.2.5.tar", last modified: Sat Apr  6 09:49:11 2024, max compression
```

## Comparing `django-db-connection-pool-1.2.4.tar` & `django-db-connection-pool-1.2.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.956382 django-db-connection-pool-1.2.4/
--rw-rw-rw-   0        0        0     1067 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     7377 2023-06-10 01:58:53.955380 django-db-connection-pool-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4913 2023-04-20 13:46:44.000000 django-db-connection-pool-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.884674 django-db-connection-pool-1.2.4/dj_db_conn_pool/
--rw-rw-rw-   0        0        0      391 2023-06-10 01:54:31.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.886675 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.890677 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/
--rw-rw-rw-   0        0        0     2175 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.893675 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
--rw-rw-rw-   0        0        0      281 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.896675 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
--rw-rw-rw-   0        0        0      574 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.898671 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
--rw-rw-rw-   0        0        0      703 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.901684 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/base.py
--rw-rw-rw-   0        0        0      730 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.905039 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/__init__.py
--rw-rw-rw-   0        0        0      516 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/mysql/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.908037 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/__init__.py
--rw-rw-rw-   0        0        0      682 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/mixins.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.909057 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/
--rw-rw-rw-   0        0        0        1 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/oracle/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/oracle/__init__.py
--rw-rw-rw-   0        0        0      365 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/oceanbase/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/oracle/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/oracle/__init__.py
--rw-rw-rw-   0        0        0      454 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/oracle/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgis/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgis/__init__.py
--rw-rw-rw-   0        0        0      342 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgis/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/__init__.py
--rw-rw-rw-   0        0        0      446 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/base.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.913101 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/django_tenants/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/django_tenants/base.py
--rw-rw-rw-   0        0        0      302 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/postgresql/mixins.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.930864 django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/
--rw-rw-rw-   0        0        0      295 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/__init__.py
--rw-rw-rw-   0        0        0      914 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/jdbc.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.936922 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/
--rw-rw-rw-   0        0        0     1070 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/__init__.py
--rw-rw-rw-   0        0        0       70 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.936922 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/
--rw-rw-rw-   0        0        0       74 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/__init__.py
--rw-rw-rw-   0        0        0     5046 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/core.py
--rw-rw-rw-   0        0        0      385 2023-04-20 13:15:05.000000 django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/creation.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:58:53.953392 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/
--rw-rw-rw-   0        0        0     7377 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1854 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      314 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-10 01:58:53.000000 django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1520 2023-06-05 12:46:17.000000 django-db-connection-pool-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 01:58:53.956382 django-db-connection-pool-1.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.910993 django-db-connection-pool-1.2.5/
+-rw-rw-rw-   0        0        0     1088 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     8687 2024-04-06 09:49:11.909991 django-db-connection-pool-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5487 2024-04-06 09:01:20.000000 django-db-connection-pool-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.863988 django-db-connection-pool-1.2.5/dj_db_conn_pool/
+-rw-rw-rw-   0        0        0      403 2024-04-06 08:40:16.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.864987 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.866987 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/
+-rw-rw-rw-   0        0        0     2192 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.868986 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
+-rw-rw-rw-   0        0        0      265 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.870994 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
+-rw-rw-rw-   0        0        0      546 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.872986 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
+-rw-rw-rw-   0        0        0      678 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.875000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oracle/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oracle/__init__.py
+-rw-rw-rw-   0        0        0     1107 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oracle/base.py
+-rw-rw-rw-   0        0        0      741 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.877038 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/mysql/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/mysql/__init__.py
+-rw-rw-rw-   0        0        0      490 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/mysql/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.879023 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/__init__.py
+-rw-rw-rw-   0        0        0      676 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.880004 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/oceanbase/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/oceanbase/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.881989 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/oceanbase/oracle/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/oceanbase/oracle/__init__.py
+-rw-rw-rw-   0        0        0      353 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/oceanbase/oracle/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.884023 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/oracle/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/oracle/__init__.py
+-rw-rw-rw-   0        0        0      442 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/oracle/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.885986 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgis/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgis/__init__.py
+-rw-rw-rw-   0        0        0      326 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgis/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.887987 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/base.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.890987 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/django_tenants/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
+-rw-rw-rw-   0        0        0      298 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/django_tenants/base.py
+-rw-rw-rw-   0        0        0      710 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/postgresql/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.892988 django-db-connection-pool-1.2.5/dj_db_conn_pool/compat/
+-rw-rw-rw-   0        0        0      302 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/compat/__init__.py
+-rw-rw-rw-   0        0        0      949 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/compat/jdbc.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.894989 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/
+-rw-rw-rw-   0        0        0     1087 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/__init__.py
+-rw-rw-rw-   0        0        0       46 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.897994 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/mixins/
+-rw-rw-rw-   0        0        0       50 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/mixins/__init__.py
+-rw-rw-rw-   0        0        0     5047 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/mixins/core.py
+-rw-rw-rw-   0        0        0      335 2024-03-17 12:19:03.000000 django-db-connection-pool-1.2.5/dj_db_conn_pool/core/mixins/creation.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:49:11.905992 django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/
+-rw-rw-rw-   0        0        0     8687 2024-04-06 09:49:11.000000 django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1854 2024-04-06 09:49:11.000000 django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 09:49:11.000000 django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      365 2024-04-06 09:49:11.000000 django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-06 09:49:11.000000 django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1632 2024-04-06 08:12:45.000000 django-db-connection-pool-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 09:49:11.910993 django-db-connection-pool-1.2.5/setup.cfg
```

### Comparing `django-db-connection-pool-1.2.4/LICENSE` & `django-db-connection-pool-1.2.5/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Altair Bow
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 Altair Bow
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-db-connection-pool-1.2.4/PKG-INFO` & `django-db-connection-pool-1.2.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-db-connection-pool
-Version: 1.2.4
+Version: 1.2.5
 Summary: Database connection pool component library for Django
 Author-email: Altair Bow <altair.bow@foxmail.com>
 License: MIT License
         
         Copyright (c) 2019 Altair Bow
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,168 +34,227 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Django>=2.0
+Requires-Dist: SQLAlchemy>=1.4.24
+Requires-Dist: sqlparams>=4.0.0
 Provides-Extra: all
+Requires-Dist: Django>=2.0; extra == "all"
+Requires-Dist: JPype1>=1.3.0; extra == "all"
+Requires-Dist: SQLAlchemy>=1.4.24; extra == "all"
+Requires-Dist: cx-Oracle>=6.4.1; extra == "all"
+Requires-Dist: mysqlclient>=1.3.0; extra == "all"
+Requires-Dist: psycopg2>=2.8.6; extra == "all"
+Requires-Dist: pyodbc>=4.0.34; extra == "all"
+Requires-Dist: sqlparams>=3.0.0; extra == "all"
 Provides-Extra: jdbc
+Requires-Dist: JPype1>=1.3.0; extra == "jdbc"
 Provides-Extra: mysql
+Requires-Dist: mysqlclient>=1.3.0; extra == "mysql"
 Provides-Extra: odbc
+Requires-Dist: pyodbc>=4.0.34; extra == "odbc"
 Provides-Extra: oracle
+Requires-Dist: cx-Oracle>=6.4.1; extra == "oracle"
 Provides-Extra: postgresql
-License-File: LICENSE
+Requires-Dist: psycopg2>=2.8.6; extra == "postgresql"
+Provides-Extra: psycopg2
+Requires-Dist: psycopg2>=2.8.6; extra == "psycopg2"
+Provides-Extra: psycopg3
+Requires-Dist: psycopg>=3; extra == "psycopg3"
 
 # django-db-connection-pool
 
-*:star: Leave a star if django-db-connection-pool is helpful to you, or you like it, Thank you:smile:*
+:star: If this project is helpful to you, please light up the star, Thank you:smile:
 
-MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool backends of Django, 
-Be based on [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy). 
-Work fine in multiprocessing and multithreading django project.
+MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool components for Django,
+Be based on [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy).
+Works fine in multiprocessing and multithreading django project.
 
 * [中文版](README_CN.md)
 
 ## Quickstart
 
 ### Installation
 
 Install with `pip` with all engines:
+
 ```bash
 $ pip install django-db-connection-pool[all]
 ```
+
 or select specific engines:
+
 ```bash
 $ pip install django-db-connection-pool[mysql,oracle,postgresql,jdbc]
 ```
+
 or one of mysql,oracle,postgresql,jdbc
+
 ```bash
 $ pip install django-db-connection-pool[oracle]
 ```
 
 ### Update settings.DATABASES
 
-#### MySQL  
+#### MySQL
+
 change `django.db.backends.mysql` to `dj_db_conn_pool.backends.mysql`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.mysql'
     }
 }
 ```
 
-#### Oracle  
+#### Oracle
+
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.oracle`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.oracle'
     }
 }
 ```
 
-#### PostgreSQL  
+#### PostgreSQL
+
 change `django.db.backends.postgresql` to `dj_db_conn_pool.backends.postgresql`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.postgresql'
     }
 }
 ```
 
 #### Pool options(optional)
+
 you can provide additional options to pass to SQLAlchemy's pool creation, key's name is `POOL_OPTIONS`:
 
 ```python
 DATABASES = {
     'default': {
-        'POOL_OPTIONS' : {
+        'POOL_OPTIONS': {
             'POOL_SIZE': 10,
             'MAX_OVERFLOW': 10,
             'RECYCLE': 24 * 60 * 60
         }
-     }
- }
+    }
+}
 ```
 
-`django-db-connection-pool` has more configuration options here: [PoolContainer.pool_default_params](https://github.com/altairbow/django-db-connection-pool/blob/master/dj_db_conn_pool/core/__init__.py#L13-L20)
-     
-Here's an explanation of these options(from SQLAlchemy's Doc):
+`django-db-connection-pool` has more configuration options
+here: [PoolContainer.pool_default_params](https://github.com/altairbow/django-db-connection-pool/blob/master/dj_db_conn_pool/core/__init__.py#L13-L20)
+
+Here's the explanation of these options(from SQLAlchemy's Doc):
 
 * **pool_size**: The size of the pool to be maintained,
-          defaults to 5. This is the largest number of connections that
-          will be kept persistently in the pool. Note that the pool
-          begins with no connections; once this number of connections
-          is requested, that number of connections will remain.
-          `pool_size` can be set to 0 to indicate no size limit; to
-          disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
-          instead.
+  defaults to 5. This is the largest number of connections that
+  will be kept persistently in the pool. Note that the pool
+  begins with no connections; once this number of connections
+  is requested, that number of connections will remain.
+  `pool_size` can be set to 0 to indicate no size limit; to
+  disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
+  instead.
 
 * **max_overflow**: The maximum overflow size of the
-          pool. When the number of checked-out connections reaches the
-          size set in pool_size, additional connections will be
-          returned up to this limit. When those additional connections
-          are returned to the pool, they are disconnected and
-          discarded. It follows then that the total number of
-          simultaneous connections the pool will allow is pool_size +
-          `max_overflow`, and the total number of "sleeping"
-          connections the pool will allow is pool_size. `max_overflow`
-          can be set to -1 to indicate no overflow limit; no limit
-          will be placed on the total number of concurrent
-          connections. Defaults to 10.
-          
-* **recycle**: If set to a value other than -1, number of seconds 
-          between connection recycling, which means upon checkout, 
-          if this timeout is surpassed the connection will be closed 
-          and replaced with a newly opened connection. 
-          Defaults to -1.          
+  pool. When the number of checked-out connections reaches the
+  size set in pool_size, additional connections will be
+  returned up to this limit. When those additional connections
+  are returned to the pool, they are disconnected and
+  discarded. It follows then that the total number of
+  simultaneous connections the pool will allow is pool_size +
+  `max_overflow`, and the total number of "sleeping"
+  connections the pool will allow is pool_size. `max_overflow`
+  can be set to -1 to indicate no overflow limit; no limit
+  will be placed on the total number of concurrent
+  connections. Defaults to 10.
+
+* **recycle**: If set to a value other than -1, number of seconds
+  between connection recycling, which means upon checkout,
+  if this timeout is surpassed the connection will be closed
+  and replaced with a newly opened connection.
+  Defaults to -1.
 
 Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
 
 ```python
 import dj_db_conn_pool
+
 dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
 ```
 
 #### multiprocessing environment
-In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container` object,
-It means that each process has an independent connection pool, for example: 
+
+In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container`
+object,
+It means that each process has an independent connection pool, for example:
 The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
 If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
 The maximum number of connections will not exceed `8 * 10 + 8 * 20`
 
+## JDBC
 
-## JDBC (experimental, NOT PRODUCTION READY)
 Thanks to [JPype](https://github.com/jpype-project/jpype),
-django-db-connection-pool can connect to database in jdbc way
+django-db-connection-pool can connect to database by jdbc
 
 ### Usage
+
 #### Set Java runtime environment
+
 ```bash
 export JAVA_HOME=$PATH_TO_JRE;
 export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
 ```
 
 #### Update settings.DATABASES
+
 ##### Oracle
 
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.jdbc.oracle'
     }
 }
 ```
 
 ##### OceanBase
+
 use `dj_db_conn_pool.backends.jdbc.oceanbase`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase'
     }
 }
 ```
+
+### Performing raw SQL queries
+
+Just like django's built-in backends, all JDBC backends support named parameters in raw SQL queries,
+you can execute raw sql queries like this:
+
+```python
+from django.db import connections
+
+with connections["default"].cursor() as cursor:
+    cursor.execute('select name, phone from users where name = %(name)s', params={"name": "Altair"})
+    result = cursor.fetchall()
+```
+
+### Acknowledgments
+- Thanks to all friends who provided PR and suggestions !
+- Thanks to [JetBrains](https://www.jetbrains.com/?from=django-db-connection-pool) for providing development tools for django-db-connection-pool !
```

### Comparing `django-db-connection-pool-1.2.4/README.md` & `django-db-connection-pool-1.2.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,153 +1,192 @@
-# django-db-connection-pool
-
-*:star: Leave a star if django-db-connection-pool is helpful to you, or you like it, Thank you:smile:*
-
-MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool backends of Django, 
-Be based on [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy). 
-Work fine in multiprocessing and multithreading django project.
-
-* [中文版](README_CN.md)
-
-## Quickstart
-
-### Installation
-
-Install with `pip` with all engines:
-```bash
-$ pip install django-db-connection-pool[all]
-```
-or select specific engines:
-```bash
-$ pip install django-db-connection-pool[mysql,oracle,postgresql,jdbc]
-```
-or one of mysql,oracle,postgresql,jdbc
-```bash
-$ pip install django-db-connection-pool[oracle]
-```
-
-### Update settings.DATABASES
-
-#### MySQL  
-change `django.db.backends.mysql` to `dj_db_conn_pool.backends.mysql`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.mysql'
-    }
-}
-```
-
-#### Oracle  
-change `django.db.backends.oracle` to `dj_db_conn_pool.backends.oracle`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.oracle'
-    }
-}
-```
-
-#### PostgreSQL  
-change `django.db.backends.postgresql` to `dj_db_conn_pool.backends.postgresql`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.postgresql'
-    }
-}
-```
-
-#### Pool options(optional)
-you can provide additional options to pass to SQLAlchemy's pool creation, key's name is `POOL_OPTIONS`:
-
-```python
-DATABASES = {
-    'default': {
-        'POOL_OPTIONS' : {
-            'POOL_SIZE': 10,
-            'MAX_OVERFLOW': 10,
-            'RECYCLE': 24 * 60 * 60
-        }
-     }
- }
-```
-
-`django-db-connection-pool` has more configuration options here: [PoolContainer.pool_default_params](https://github.com/altairbow/django-db-connection-pool/blob/master/dj_db_conn_pool/core/__init__.py#L13-L20)
-     
-Here's an explanation of these options(from SQLAlchemy's Doc):
-
-* **pool_size**: The size of the pool to be maintained,
-          defaults to 5. This is the largest number of connections that
-          will be kept persistently in the pool. Note that the pool
-          begins with no connections; once this number of connections
-          is requested, that number of connections will remain.
-          `pool_size` can be set to 0 to indicate no size limit; to
-          disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
-          instead.
-
-* **max_overflow**: The maximum overflow size of the
-          pool. When the number of checked-out connections reaches the
-          size set in pool_size, additional connections will be
-          returned up to this limit. When those additional connections
-          are returned to the pool, they are disconnected and
-          discarded. It follows then that the total number of
-          simultaneous connections the pool will allow is pool_size +
-          `max_overflow`, and the total number of "sleeping"
-          connections the pool will allow is pool_size. `max_overflow`
-          can be set to -1 to indicate no overflow limit; no limit
-          will be placed on the total number of concurrent
-          connections. Defaults to 10.
-          
-* **recycle**: If set to a value other than -1, number of seconds 
-          between connection recycling, which means upon checkout, 
-          if this timeout is surpassed the connection will be closed 
-          and replaced with a newly opened connection. 
-          Defaults to -1.          
-
-Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
-
-```python
-import dj_db_conn_pool
-dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
-```
-
-#### multiprocessing environment
-In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container` object,
-It means that each process has an independent connection pool, for example: 
-The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
-If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
-The maximum number of connections will not exceed `8 * 10 + 8 * 20`
-
-
-## JDBC (experimental, NOT PRODUCTION READY)
-Thanks to [JPype](https://github.com/jpype-project/jpype),
-django-db-connection-pool can connect to database in jdbc way
-
-### Usage
-#### Set Java runtime environment
-```bash
-export JAVA_HOME=$PATH_TO_JRE;
-export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
-```
-
-#### Update settings.DATABASES
-##### Oracle
-
-change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oracle'
-    }
-}
-```
-
-##### OceanBase
-use `dj_db_conn_pool.backends.jdbc.oceanbase`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase'
-    }
-}
-```
+# django-db-connection-pool
+
+:star: If this project is helpful to you, please light up the star, Thank you:smile:
+
+MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool components for Django,
+Be based on [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy).
+Works fine in multiprocessing and multithreading django project.
+
+* [中文版](README_CN.md)
+
+## Quickstart
+
+### Installation
+
+Install with `pip` with all engines:
+
+```bash
+$ pip install django-db-connection-pool[all]
+```
+
+or select specific engines:
+
+```bash
+$ pip install django-db-connection-pool[mysql,oracle,postgresql,jdbc]
+```
+
+or one of mysql,oracle,postgresql,jdbc
+
+```bash
+$ pip install django-db-connection-pool[oracle]
+```
+
+### Update settings.DATABASES
+
+#### MySQL
+
+change `django.db.backends.mysql` to `dj_db_conn_pool.backends.mysql`:
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.mysql'
+    }
+}
+```
+
+#### Oracle
+
+change `django.db.backends.oracle` to `dj_db_conn_pool.backends.oracle`:
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.oracle'
+    }
+}
+```
+
+#### PostgreSQL
+
+change `django.db.backends.postgresql` to `dj_db_conn_pool.backends.postgresql`:
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.postgresql'
+    }
+}
+```
+
+#### Pool options(optional)
+
+you can provide additional options to pass to SQLAlchemy's pool creation, key's name is `POOL_OPTIONS`:
+
+```python
+DATABASES = {
+    'default': {
+        'POOL_OPTIONS': {
+            'POOL_SIZE': 10,
+            'MAX_OVERFLOW': 10,
+            'RECYCLE': 24 * 60 * 60
+        }
+    }
+}
+```
+
+`django-db-connection-pool` has more configuration options
+here: [PoolContainer.pool_default_params](https://github.com/altairbow/django-db-connection-pool/blob/master/dj_db_conn_pool/core/__init__.py#L13-L20)
+
+Here's the explanation of these options(from SQLAlchemy's Doc):
+
+* **pool_size**: The size of the pool to be maintained,
+  defaults to 5. This is the largest number of connections that
+  will be kept persistently in the pool. Note that the pool
+  begins with no connections; once this number of connections
+  is requested, that number of connections will remain.
+  `pool_size` can be set to 0 to indicate no size limit; to
+  disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
+  instead.
+
+* **max_overflow**: The maximum overflow size of the
+  pool. When the number of checked-out connections reaches the
+  size set in pool_size, additional connections will be
+  returned up to this limit. When those additional connections
+  are returned to the pool, they are disconnected and
+  discarded. It follows then that the total number of
+  simultaneous connections the pool will allow is pool_size +
+  `max_overflow`, and the total number of "sleeping"
+  connections the pool will allow is pool_size. `max_overflow`
+  can be set to -1 to indicate no overflow limit; no limit
+  will be placed on the total number of concurrent
+  connections. Defaults to 10.
+
+* **recycle**: If set to a value other than -1, number of seconds
+  between connection recycling, which means upon checkout,
+  if this timeout is surpassed the connection will be closed
+  and replaced with a newly opened connection.
+  Defaults to -1.
+
+Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
+
+```python
+import dj_db_conn_pool
+
+dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
+```
+
+#### multiprocessing environment
+
+In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container`
+object,
+It means that each process has an independent connection pool, for example:
+The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
+If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
+The maximum number of connections will not exceed `8 * 10 + 8 * 20`
+
+## JDBC
+
+Thanks to [JPype](https://github.com/jpype-project/jpype),
+django-db-connection-pool can connect to database by jdbc
+
+### Usage
+
+#### Set Java runtime environment
+
+```bash
+export JAVA_HOME=$PATH_TO_JRE;
+export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
+```
+
+#### Update settings.DATABASES
+
+##### Oracle
+
+change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oracle'
+    }
+}
+```
+
+##### OceanBase
+
+use `dj_db_conn_pool.backends.jdbc.oceanbase`:
+
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase'
+    }
+}
+```
+
+### Performing raw SQL queries
+
+Just like django's built-in backends, all JDBC backends support named parameters in raw SQL queries,
+you can execute raw sql queries like this:
+
+```python
+from django.db import connections
+
+with connections["default"].cursor() as cursor:
+    cursor.execute('select name, phone from users where name = %(name)s', params={"name": "Altair"})
+    result = cursor.fetchall()
+```
+
+### Acknowledgments
+- Thanks to all friends who provided PR and suggestions !
+- Thanks to [JetBrains](https://www.jetbrains.com/?from=django-db-connection-pool) for providing development tools for django-db-connection-pool !
```

### Comparing `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/__init__.py` & `django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# -*- coding: utf-8 -*-
-
-import threading
-import jpype
-import jpype.dbapi2
-from dj_db_conn_pool.core.mixins import PersistentDatabaseWrapperMixin
-from dj_db_conn_pool.backends.jdbc.utils import CursorWrapper
-
-import logging
-logger = logging.getLogger(__name__)
-
-jdbc_type_converters = {}
-
-lock_check_jvm_status = threading.Lock()
-
-
-class JDBCDatabaseWrapperMixin(PersistentDatabaseWrapperMixin):
-    @property
-    def jdbc_driver(self):
-        raise NotImplementedError()
-
-    @property
-    def jdbc_url_prefix(self):
-        raise NotImplementedError()
-
-    @property
-    def jdbc_url(self):
-        return '{prefix}//{HOST}:{PORT}/{NAME}'.format(
-            prefix=self.jdbc_url_prefix,
-            **self.settings_dict
-        )
-
-    def create_cursor(self, name=None):
-        cursor = self.connection.cursor()
-        return CursorWrapper(cursor)
-
-    def get_connection_params(self):
-        return self.settings_dict.get('OPTIONS', {})
-
-    def _get_new_connection(self, conn_params):
-        with lock_check_jvm_status:
-            if not jpype.isJVMStarted():
-                jpype.startJVM(ignoreUnrecognized=True)
-
-        conn = jpype.dbapi2.connect(
-            self.jdbc_url,
-            driver=self.jdbc_driver,
-            driver_args=dict(
-                user=self.settings_dict['USER'],
-                password=self.settings_dict['PASSWORD'],
-                **conn_params
-            ),
-            converters=jdbc_type_converters,
-        )
-
-        return conn
-
-    def _close(self):
-        if self.connection is not None and self.connection.driver_connection.autocommit:
-            # if jdbc connection's autoCommit is on
-            # jpype will throw NotSupportedError after rollback called
-            # we make a little dynamic patch here, make sure
-            # SQLAlchemy will not do rollback before recycling connection
-            self.connection._pool._reset_on_return = None
-
-            logger.debug(
-                "autoCommit of current JDBC connection to %s %s is on, won't do rollback before returning",
-                self.alias, self.connection.driver_connection)
-
-        return super(JDBCDatabaseWrapperMixin, self)._close()
+import logging
+import threading
+
+import jpype
+import jpype.dbapi2
+
+from dj_db_conn_pool.backends.jdbc.utils import CursorWrapper
+from dj_db_conn_pool.core.mixins import PersistentDatabaseWrapperMixin
+
+logger = logging.getLogger(__name__)
+
+jdbc_type_converters = {}
+
+lock_check_jvm_status = threading.Lock()
+
+
+class JDBCDatabaseWrapperMixin(PersistentDatabaseWrapperMixin):
+    @property
+    def jdbc_driver(self):
+        raise NotImplementedError()
+
+    @property
+    def jdbc_url_prefix(self):
+        raise NotImplementedError()
+
+    @property
+    def jdbc_url(self):
+        return '{prefix}//{HOST}:{PORT}/{NAME}'.format(
+            prefix=self.jdbc_url_prefix,
+            **self.settings_dict
+        )
+
+    def create_cursor(self, name=None):
+        cursor = self.connection.cursor()
+        return CursorWrapper(cursor)
+
+    def get_connection_params(self):
+        return self.settings_dict.get('OPTIONS', {})
+
+    def _get_new_connection(self, conn_params):
+        with lock_check_jvm_status:
+            if not jpype.isJVMStarted():
+                jpype.startJVM(ignoreUnrecognized=True)
+
+        conn = jpype.dbapi2.connect(
+            self.jdbc_url,
+            driver=self.jdbc_driver,
+            driver_args=dict(
+                user=self.settings_dict['USER'],
+                password=self.settings_dict['PASSWORD'],
+                **conn_params
+            ),
+            converters=jdbc_type_converters,
+        )
+
+        return conn
+
+    def _close(self):
+        if self.connection is not None and self.connection.driver_connection.autocommit:
+            # if jdbc connection's autoCommit is on
+            # jpype will throw NotSupportedError after rollback called
+            # we make a little dynamic patch here, make sure
+            # SQLAlchemy will not do rollback before recycling connection
+            self.connection._pool._reset_on_return = None
+
+            logger.debug(
+                "autoCommit of current JDBC connection to %s %s is on, won't do rollback before returning",
+                self.alias, self.connection.driver_connection)
+
+        return super()._close()
```

### Comparing `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py` & `django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-# -*- coding: utf-8 -*-
-
-import jpype.dbapi2
-from django.db.backends.mysql import base
-from sqlalchemy.dialects.mysql.base import MySQLDialect
-from dj_db_conn_pool.backends.jdbc.oceanbase.mixins import JDBCOceanBaseDatabaseWrapperMixin
-
-
-class DatabaseWrapper(JDBCOceanBaseDatabaseWrapperMixin, base.DatabaseWrapper):
-    class SQLAlchemyDialect(MySQLDialect):
-        def do_ping(self, dbapi_connection):
-            try:
-                return super(MySQLDialect, self).do_ping(dbapi_connection)
-            except jpype.dbapi2.DatabaseError:
-                return False
+import jpype.dbapi2
+from django.db.backends.oracle import base
+from sqlalchemy.dialects.oracle.base import OracleDialect
+
+from dj_db_conn_pool.backends.jdbc.oceanbase.mixins import JDBCOceanBaseDatabaseWrapperMixin
+
+
+class DatabaseWrapper(JDBCOceanBaseDatabaseWrapperMixin, base.DatabaseWrapper):
+    class SQLAlchemyDialect(OracleDialect):
+        def do_ping(self, dbapi_connection):
+            try:
+                return super().do_ping(dbapi_connection)
+            except jpype.dbapi2.DatabaseError:
+                return False
+
+    def init_connection_state(self):
+        # TODO: custom OceanBase (Oracle mode) connection initialization
+        pass
```

### Comparing `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/jdbc/oracle/base.py` & `django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/jdbc/oracle/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# -*- coding: utf-8 -*-
-
-import getpass
-import socket
-from multiprocessing import current_process
-import jpype.dbapi2
-from django.db.backends.oracle import base
-from sqlalchemy.dialects.oracle.base import OracleDialect
-from dj_db_conn_pool.backends.jdbc import JDBCDatabaseWrapperMixin
-
-
-import logging
-logger = logging.getLogger(__name__)
-
-oracle_session_info = {
-    'v$session.process': str(current_process().pid),
-    'v$session.osuser': getpass.getuser(),
-    'v$session.machine': socket.gethostname(),
-    'v$session.program': 'python',
-}
-
-
-class DatabaseWrapper(JDBCDatabaseWrapperMixin, base.DatabaseWrapper):
-    class SQLAlchemyDialect(OracleDialect):
-        def do_ping(self, dbapi_connection):
-            try:
-                return super(OracleDialect, self).do_ping(dbapi_connection)
-            except jpype.dbapi2.DatabaseError:
-                return False
-
-    jdbc_driver = 'oracle.jdbc.OracleDriver'
-
-    jdbc_url_prefix = 'jdbc:oracle:thin:@'
-
-    def get_connection_params(self):
-        return {
-            **oracle_session_info,
-            **super(DatabaseWrapper, self).get_connection_params()
-        }
+import getpass
+import logging
+import socket
+from multiprocessing import current_process
+
+import jpype.dbapi2
+from django.db.backends.oracle import base
+from sqlalchemy.dialects.oracle.base import OracleDialect
+
+from dj_db_conn_pool.backends.jdbc import JDBCDatabaseWrapperMixin
+
+logger = logging.getLogger(__name__)
+
+oracle_session_info = {
+    'v$session.process': str(current_process().pid),
+    'v$session.osuser': getpass.getuser(),
+    'v$session.machine': socket.gethostname(),
+    'v$session.program': 'python',
+}
+
+
+class DatabaseWrapper(JDBCDatabaseWrapperMixin, base.DatabaseWrapper):
+    class SQLAlchemyDialect(OracleDialect):
+        def do_ping(self, dbapi_connection):
+            try:
+                return super().do_ping(dbapi_connection)
+            except jpype.dbapi2.DatabaseError:
+                return False
+
+    jdbc_driver = 'oracle.jdbc.OracleDriver'
+
+    jdbc_url_prefix = 'jdbc:oracle:thin:@'
+
+    def get_connection_params(self):
+        return {
+            **oracle_session_info,
+            **super().get_connection_params()
+        }
```

### Comparing `django-db-connection-pool-1.2.4/dj_db_conn_pool/backends/odbc/mixins.py` & `django-db-connection-pool-1.2.5/dj_db_conn_pool/backends/odbc/mixins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
-
-import pyodbc
-from django.conf import ImproperlyConfigured
-from dj_db_conn_pool.core.mixins import PersistentDatabaseWrapperMixin
-
-
-class ODBCWrapperMixin(PersistentDatabaseWrapperMixin):
-    def _get_new_connection(self, conn_params):
-        try:
-            driver = self.settings_dict['ODBC_OPTIONS']['DRIVER']
-        except KeyError:
-            raise ImproperlyConfigured('No odbc driver provided')
-
-        conn_str_template = 'DRIVER={DRIVER};SERVER={HOST}:{PORT};DATABASE={NAME};UID={USER};PWD={PASSWORD}'
-
-        connection_string = conn_str_template.format(DRIVER=driver, **self.settings_dict)
-
-        return pyodbc.connect(connection_string)
+import pyodbc
+from django.conf import ImproperlyConfigured
+
+from dj_db_conn_pool.core.mixins import PersistentDatabaseWrapperMixin
+
+
+class ODBCWrapperMixin(PersistentDatabaseWrapperMixin):
+    def _get_new_connection(self, conn_params):
+        try:
+            driver = self.settings_dict['ODBC_OPTIONS']['DRIVER']
+        except KeyError:
+            raise ImproperlyConfigured('No odbc driver provided')
+
+        conn_str_template = 'DRIVER={DRIVER};SERVER={HOST}:{PORT};DATABASE={NAME};UID={USER};PWD={PASSWORD}'
+
+        connection_string = conn_str_template.format(DRIVER=driver, **self.settings_dict)
+
+        return pyodbc.connect(connection_string)
```

### Comparing `django-db-connection-pool-1.2.4/dj_db_conn_pool/compat/jdbc.py` & `django-db-connection-pool-1.2.5/dj_db_conn_pool/compat/jdbc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import jpype
-
-
-def patch_all():
-    patch_converters()
-
-
-def patch_converters():
-    """
-    patch jpype's jdbc converters
-    """
-    def to_python(value):
-        return value._py()
-
-    def to_number(value):
-        string = str(value.toString())
-
-        if value.scale() > 0:
-            return float(string)
-
-        return int(string)
-
-    @jpype.onJVMStart
-    def register_converters():
-        from dj_db_conn_pool.backends.jdbc import jdbc_type_converters
-
-        jdbc_type_converters[jpype.java.lang.String] = str
-        jdbc_type_converters[jpype.java.sql.Date] = to_python
-        jdbc_type_converters[jpype.java.sql.Time] = to_python
-        jdbc_type_converters[jpype.java.sql.Timestamp] = to_python
-        jdbc_type_converters[jpype.java.math.BigDecimal] = to_number
-        jdbc_type_converters[jpype.JArray(jpype.types.JByte)] = bytes
-        # jdbc_type_converters[type(None)] = lambda v: v
+import jpype
+
+
+def patch_all():
+    patch_converters()
+
+
+def patch_converters():
+    """
+    patch jpype's jdbc converters
+    """
+
+    def to_python(value):
+        return value._py()
+
+    def to_number(value):
+        string = str(value.toString())
+
+        if value.scale() > 0:
+            return float(string)
+
+        return int(string)
+
+    @jpype.onJVMStart
+    def register_converters():
+        from dj_db_conn_pool.backends.jdbc import jdbc_type_converters
+
+        jdbc_type_converters[jpype.java.lang.String] = str
+        jdbc_type_converters[jpype.java.sql.Date] = to_python
+        jdbc_type_converters[jpype.java.sql.Time] = to_python
+        jdbc_type_converters[jpype.java.sql.Timestamp] = to_python
+        jdbc_type_converters[jpype.java.math.BigDecimal] = to_number
+        jdbc_type_converters[jpype.JArray(jpype.types.JByte)] = bytes
+        # jdbc_type_converters[type(None)] = lambda v: v
```

### Comparing `django-db-connection-pool-1.2.4/dj_db_conn_pool/core/mixins/core.py` & `django-db-connection-pool-1.2.5/dj_db_conn_pool/core/mixins/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,119 @@
-# -*- coding: utf-8 -*-
-
-from sqlalchemy import pool
-from dj_db_conn_pool.compat import gettext_lazy as _
-from dj_db_conn_pool.core import pool_container
-from dj_db_conn_pool.core.mixins.creation import DatabaseCreationMixin
-
-
-import logging
-logger = logging.getLogger(__name__)
-
-
-class PersistentDatabaseWrapperMixin(object):
-    def __init__(self, *args, **kwargs):
-        # override creation_class
-        self.creation_class = type('', (DatabaseCreationMixin, self.creation_class), {})
-
-        super(PersistentDatabaseWrapperMixin, self).__init__(*args, **kwargs)
-
-    def __str__(self):
-        try:
-            conn = repr(self.connection.driver_connection)
-        except AttributeError:
-            conn = '<Not connected>'
-
-        return f'{self.vendor} connection to {self.alias}: {conn}'
-
-    __repr__ = __str__
-
-    def _set_dbapi_autocommit(self, autocommit):
-        self.connection.driver_connection.autocommit = autocommit
-
-    def _set_autocommit(self, autocommit):
-        with self.wrap_database_errors:
-            try:
-                self._set_dbapi_autocommit(autocommit)
-            except (Exception, ) as exc:
-                logger.exception('unable to set autocommit mode of %s(%s) to %s, caused by: %s',
-                                 self.vendor, self.alias, autocommit, exc)
-                raise exc from None
-
-    def _get_dialect(self):
-        return self.SQLAlchemyDialect(dbapi=self.Database)
-
-    def _get_new_connection(self, conn_params):
-        return super(PersistentDatabaseWrapperMixin, self).get_new_connection(conn_params)
-
-    def get_new_connection(self, conn_params):
-        """
-        override django.db.backends.<database>.base.DatabaseWrapper.get_new_connection to
-        change the default behavior of getting new connection to database, we maintain
-        pool_container who contains the connection pool of each database here
-        when django call this method to get new connection, we check whether there exists
-        the pool of this database(self.alias)
-        if the target pool doesn't exist, we will create one
-        then grab one connection from the pool and return it to django
-        :return:
-        """
-        with pool_container.lock:
-            # acquire the lock, check whether there exists the pool of current database
-            # note: the value of self.alias is the name of current database, one of setting.DATABASES
-            if not pool_container.has(self.alias):
-                # self.alias's pool doesn't exist, time to create it
-
-                # parse parameters of current database from self.settings_dict
-                pool_setting = {
-                    # transform the keys in POOL_OPTIONS to lower case
-                    # to fit sqlalchemy.pool.QueuePool's arguments requirement
-                    key.lower(): value
-                    # traverse POOL_OPTIONS to get arguments
-                    for key, value in
-                    # self.settings_dict was created by Django
-                    # is the connection parameters of self.alias
-                    self.settings_dict.get('POOL_OPTIONS', {}).items()
-                    # There are some limits of self.alias's pool's option(POOL_OPTIONS):
-                    # the keys in POOL_OPTIONS must be capitalised
-                    # and the key's lowercase must be in pool_container.pool_default_params
-                    if key == key.upper() and key.lower() in pool_container.pool_default_params
-                }
-
-                # replace pool_params's items with pool_setting's items
-                # to import custom settings
-                pool_params = {
-                    **pool_container.pool_default_params,
-                    **pool_setting
-                }
-
-                # now we have all parameters of self.alias
-                # create self.alias's pool
-                alias_pool = pool.QueuePool(
-                    lambda: self._get_new_connection(conn_params),
-                    # SQLAlchemy use the dialect to maintain the pool
-                    dialect=self._get_dialect(),
-                    # parameters of self.alias
-                    **pool_params
-                )
-
-                logger.debug(_("%s's pool has been created, parameter: %s"), self.alias, pool_params)
-
-                # pool has been created
-                # put into pool_container for reusing
-                pool_container.put(self.alias, alias_pool)
-
-        # get self.alias's pool from pool_container
-        db_pool = pool_container.get(self.alias)
-        # get one connection from the pool
-        conn = db_pool.connect()
-
-        logger.debug(
-            _("got %s's connection %s from its pool"),
-            self.alias, conn.driver_connection)
-
-        return conn
-
-    def close(self, *args, **kwargs):
-        logger.debug(
-            _("release %s's connection %s to its pool"),
-            self.alias, getattr(self.connection, 'driver_connection', None))
-
-        return super(PersistentDatabaseWrapperMixin, self).close(*args, **kwargs)
+import logging
+
+from sqlalchemy import pool
+
+from dj_db_conn_pool.compat import gettext_lazy as _
+from dj_db_conn_pool.core import pool_container
+from dj_db_conn_pool.core.mixins.creation import DatabaseCreationMixin
+
+logger = logging.getLogger(__name__)
+
+
+class PersistentDatabaseWrapperMixin:
+    def __init__(self, *args, **kwargs):
+        # override creation_class
+        self.creation_class = type('DatabaseCreationWrapper', (DatabaseCreationMixin, self.creation_class), {})
+
+        super().__init__(*args, **kwargs)
+
+    def __str__(self):
+        try:
+            conn = repr(self.connection.driver_connection)
+        except AttributeError:
+            conn = '<Not connected>'
+
+        return f'{self.vendor} connection to {self.alias}: {conn}'
+
+    __repr__ = __str__
+
+    def _set_dbapi_autocommit(self, autocommit):
+        self.connection.driver_connection.autocommit = autocommit
+
+    def _set_autocommit(self, autocommit):
+        with self.wrap_database_errors:
+            try:
+                self._set_dbapi_autocommit(autocommit)
+            except (Exception,) as exc:
+                logger.exception('unable to set autocommit mode of %s(%s) to %s, caused by: %s',
+                                 self.vendor, self.alias, autocommit, exc)
+                raise exc from None
+
+    def _get_dialect(self):
+        return self.SQLAlchemyDialect(dbapi=self.Database)
+
+    def _get_new_connection(self, conn_params):
+        return super().get_new_connection(conn_params)
+
+    def get_new_connection(self, conn_params):
+        """
+        override django.db.backends.<database>.base.DatabaseWrapper.get_new_connection to
+        change the default behavior of getting new connection to database, we maintain
+        pool_container who contains the connection pool of each database here
+        when django call this method to get new connection, we check whether there exists
+        the pool of this database(self.alias)
+        if the target pool doesn't exist, we will create one
+        then grab one connection from the pool and return it to django
+        :return:
+        """
+        with pool_container.lock:
+            # acquire the lock, check whether there exists the pool of current database
+            # note: the value of self.alias is the name of current database, one of setting.DATABASES
+            if not pool_container.has(self.alias):
+                # self.alias's pool doesn't exist, time to create it
+
+                # parse parameters of current database from self.settings_dict
+                pool_setting = {
+                    # transform the keys in POOL_OPTIONS to lower case
+                    # to fit sqlalchemy.pool.QueuePool's arguments requirement
+                    key.lower(): value
+                    # traverse POOL_OPTIONS to get arguments
+                    for key, value in
+                    # self.settings_dict was created by Django
+                    # is the connection parameters of self.alias
+                    self.settings_dict.get('POOL_OPTIONS', {}).items()
+                    # There are some limits of self.alias's pool's option(POOL_OPTIONS):
+                    # the keys in POOL_OPTIONS must be capitalised
+                    # and the key's lowercase must be in pool_container.pool_default_params
+                    if key == key.upper() and key.lower() in pool_container.pool_default_params
+                }
+
+                # replace pool_params's items with pool_setting's items
+                # to import custom settings
+                pool_params = {
+                    **pool_container.pool_default_params,
+                    **pool_setting
+                }
+
+                # now we have all parameters of self.alias
+                # create self.alias's pool
+                alias_pool = pool.QueuePool(
+                    lambda: self._get_new_connection(conn_params),
+                    # SQLAlchemy use the dialect to maintain the pool
+                    dialect=self._get_dialect(),
+                    # parameters of self.alias
+                    **pool_params
+                )
+
+                logger.debug(_("%s's pool has been created, parameter: %s"), self.alias, pool_params)
+
+                # pool has been created
+                # put into pool_container for reusing
+                pool_container.put(self.alias, alias_pool)
+
+        # get self.alias's pool from pool_container
+        db_pool = pool_container.get(self.alias)
+        # get one connection from the pool
+        conn = db_pool.connect()
+
+        logger.debug(
+            _("got %s's connection %s from its pool"),
+            self.alias, conn.driver_connection)
+
+        return conn
+
+    def close(self, *args, **kwargs):
+        logger.debug(
+            _("release %s's connection %s to its pool"),
+            self.alias, getattr(self.connection, 'driver_connection', None))
+
+        return super().close(*args, **kwargs)
```

### Comparing `django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/PKG-INFO` & `django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-db-connection-pool
-Version: 1.2.4
+Version: 1.2.5
 Summary: Database connection pool component library for Django
 Author-email: Altair Bow <altair.bow@foxmail.com>
 License: MIT License
         
         Copyright (c) 2019 Altair Bow
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,168 +34,227 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Django>=2.0
+Requires-Dist: SQLAlchemy>=1.4.24
+Requires-Dist: sqlparams>=4.0.0
 Provides-Extra: all
+Requires-Dist: Django>=2.0; extra == "all"
+Requires-Dist: JPype1>=1.3.0; extra == "all"
+Requires-Dist: SQLAlchemy>=1.4.24; extra == "all"
+Requires-Dist: cx-Oracle>=6.4.1; extra == "all"
+Requires-Dist: mysqlclient>=1.3.0; extra == "all"
+Requires-Dist: psycopg2>=2.8.6; extra == "all"
+Requires-Dist: pyodbc>=4.0.34; extra == "all"
+Requires-Dist: sqlparams>=3.0.0; extra == "all"
 Provides-Extra: jdbc
+Requires-Dist: JPype1>=1.3.0; extra == "jdbc"
 Provides-Extra: mysql
+Requires-Dist: mysqlclient>=1.3.0; extra == "mysql"
 Provides-Extra: odbc
+Requires-Dist: pyodbc>=4.0.34; extra == "odbc"
 Provides-Extra: oracle
+Requires-Dist: cx-Oracle>=6.4.1; extra == "oracle"
 Provides-Extra: postgresql
-License-File: LICENSE
+Requires-Dist: psycopg2>=2.8.6; extra == "postgresql"
+Provides-Extra: psycopg2
+Requires-Dist: psycopg2>=2.8.6; extra == "psycopg2"
+Provides-Extra: psycopg3
+Requires-Dist: psycopg>=3; extra == "psycopg3"
 
 # django-db-connection-pool
 
-*:star: Leave a star if django-db-connection-pool is helpful to you, or you like it, Thank you:smile:*
+:star: If this project is helpful to you, please light up the star, Thank you:smile:
 
-MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool backends of Django, 
-Be based on [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy). 
-Work fine in multiprocessing and multithreading django project.
+MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool components for Django,
+Be based on [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy).
+Works fine in multiprocessing and multithreading django project.
 
 * [中文版](README_CN.md)
 
 ## Quickstart
 
 ### Installation
 
 Install with `pip` with all engines:
+
 ```bash
 $ pip install django-db-connection-pool[all]
 ```
+
 or select specific engines:
+
 ```bash
 $ pip install django-db-connection-pool[mysql,oracle,postgresql,jdbc]
 ```
+
 or one of mysql,oracle,postgresql,jdbc
+
 ```bash
 $ pip install django-db-connection-pool[oracle]
 ```
 
 ### Update settings.DATABASES
 
-#### MySQL  
+#### MySQL
+
 change `django.db.backends.mysql` to `dj_db_conn_pool.backends.mysql`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.mysql'
     }
 }
 ```
 
-#### Oracle  
+#### Oracle
+
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.oracle`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.oracle'
     }
 }
 ```
 
-#### PostgreSQL  
+#### PostgreSQL
+
 change `django.db.backends.postgresql` to `dj_db_conn_pool.backends.postgresql`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.postgresql'
     }
 }
 ```
 
 #### Pool options(optional)
+
 you can provide additional options to pass to SQLAlchemy's pool creation, key's name is `POOL_OPTIONS`:
 
 ```python
 DATABASES = {
     'default': {
-        'POOL_OPTIONS' : {
+        'POOL_OPTIONS': {
             'POOL_SIZE': 10,
             'MAX_OVERFLOW': 10,
             'RECYCLE': 24 * 60 * 60
         }
-     }
- }
+    }
+}
 ```
 
-`django-db-connection-pool` has more configuration options here: [PoolContainer.pool_default_params](https://github.com/altairbow/django-db-connection-pool/blob/master/dj_db_conn_pool/core/__init__.py#L13-L20)
-     
-Here's an explanation of these options(from SQLAlchemy's Doc):
+`django-db-connection-pool` has more configuration options
+here: [PoolContainer.pool_default_params](https://github.com/altairbow/django-db-connection-pool/blob/master/dj_db_conn_pool/core/__init__.py#L13-L20)
+
+Here's the explanation of these options(from SQLAlchemy's Doc):
 
 * **pool_size**: The size of the pool to be maintained,
-          defaults to 5. This is the largest number of connections that
-          will be kept persistently in the pool. Note that the pool
-          begins with no connections; once this number of connections
-          is requested, that number of connections will remain.
-          `pool_size` can be set to 0 to indicate no size limit; to
-          disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
-          instead.
+  defaults to 5. This is the largest number of connections that
+  will be kept persistently in the pool. Note that the pool
+  begins with no connections; once this number of connections
+  is requested, that number of connections will remain.
+  `pool_size` can be set to 0 to indicate no size limit; to
+  disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
+  instead.
 
 * **max_overflow**: The maximum overflow size of the
-          pool. When the number of checked-out connections reaches the
-          size set in pool_size, additional connections will be
-          returned up to this limit. When those additional connections
-          are returned to the pool, they are disconnected and
-          discarded. It follows then that the total number of
-          simultaneous connections the pool will allow is pool_size +
-          `max_overflow`, and the total number of "sleeping"
-          connections the pool will allow is pool_size. `max_overflow`
-          can be set to -1 to indicate no overflow limit; no limit
-          will be placed on the total number of concurrent
-          connections. Defaults to 10.
-          
-* **recycle**: If set to a value other than -1, number of seconds 
-          between connection recycling, which means upon checkout, 
-          if this timeout is surpassed the connection will be closed 
-          and replaced with a newly opened connection. 
-          Defaults to -1.          
+  pool. When the number of checked-out connections reaches the
+  size set in pool_size, additional connections will be
+  returned up to this limit. When those additional connections
+  are returned to the pool, they are disconnected and
+  discarded. It follows then that the total number of
+  simultaneous connections the pool will allow is pool_size +
+  `max_overflow`, and the total number of "sleeping"
+  connections the pool will allow is pool_size. `max_overflow`
+  can be set to -1 to indicate no overflow limit; no limit
+  will be placed on the total number of concurrent
+  connections. Defaults to 10.
+
+* **recycle**: If set to a value other than -1, number of seconds
+  between connection recycling, which means upon checkout,
+  if this timeout is surpassed the connection will be closed
+  and replaced with a newly opened connection.
+  Defaults to -1.
 
 Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
 
 ```python
 import dj_db_conn_pool
+
 dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
 ```
 
 #### multiprocessing environment
-In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container` object,
-It means that each process has an independent connection pool, for example: 
+
+In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container`
+object,
+It means that each process has an independent connection pool, for example:
 The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
 If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
 The maximum number of connections will not exceed `8 * 10 + 8 * 20`
 
+## JDBC
 
-## JDBC (experimental, NOT PRODUCTION READY)
 Thanks to [JPype](https://github.com/jpype-project/jpype),
-django-db-connection-pool can connect to database in jdbc way
+django-db-connection-pool can connect to database by jdbc
 
 ### Usage
+
 #### Set Java runtime environment
+
 ```bash
 export JAVA_HOME=$PATH_TO_JRE;
 export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
 ```
 
 #### Update settings.DATABASES
+
 ##### Oracle
 
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.jdbc.oracle'
     }
 }
 ```
 
 ##### OceanBase
+
 use `dj_db_conn_pool.backends.jdbc.oceanbase`:
+
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase'
     }
 }
 ```
+
+### Performing raw SQL queries
+
+Just like django's built-in backends, all JDBC backends support named parameters in raw SQL queries,
+you can execute raw sql queries like this:
+
+```python
+from django.db import connections
+
+with connections["default"].cursor() as cursor:
+    cursor.execute('select name, phone from users where name = %(name)s', params={"name": "Altair"})
+    result = cursor.fetchall()
+```
+
+### Acknowledgments
+- Thanks to all friends who provided PR and suggestions !
+- Thanks to [JetBrains](https://www.jetbrains.com/?from=django-db-connection-pool) for providing development tools for django-db-connection-pool !
```

### Comparing `django-db-connection-pool-1.2.4/django_db_connection_pool.egg-info/SOURCES.txt` & `django-db-connection-pool-1.2.5/django_db_connection_pool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

