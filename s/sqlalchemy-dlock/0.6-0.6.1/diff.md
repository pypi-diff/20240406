# Comparing `tmp/sqlalchemy-dlock-0.6.tar.gz` & `tmp/sqlalchemy-dlock-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-dlock-0.6.tar", last modified: Thu Mar 28 09:51:07 2024, max compression
+gzip compressed data, was "sqlalchemy-dlock-0.6.1.tar", last modified: Sat Apr  6 15:24:39 2024, max compression
```

## Comparing `sqlalchemy-dlock-0.6.tar` & `sqlalchemy-dlock-0.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.350520 sqlalchemy-dlock-0.6/
--rw-rw-rw-   0        0        0      183 2023-02-24 15:23:29.000000 sqlalchemy-dlock-0.6/AUTHORS.md
--rw-rw-rw-   0        0        0     3302 2024-03-28 09:07:02.000000 sqlalchemy-dlock-0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1519 2023-06-19 06:24:19.000000 sqlalchemy-dlock-0.6/LICENSE
--rw-rw-rw-   0        0        0      167 2023-12-06 14:32:38.000000 sqlalchemy-dlock-0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     9597 2024-03-28 09:51:07.342814 sqlalchemy-dlock-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6980 2024-03-28 09:07:02.000000 sqlalchemy-dlock-0.6/README.md
--rw-rw-rw-   0        0        0     2428 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/pyproject.toml
--rw-rw-rw-   0        0        0      207 2024-03-15 14:40:03.000000 sqlalchemy-dlock-0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 09:51:07.351480 sqlalchemy-dlock-0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.105374 sqlalchemy-dlock-0.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.202622 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/
--rw-rw-rw-   0        0        0       12 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/.gitignore
--rw-rw-rw-   0        0        0      189 2024-03-17 08:44:18.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/__init__.py
--rw-rw-rw-   0        0        0      159 2024-03-15 14:40:03.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/_sa_types.py
--rw-rw-rw-   0        0        0      540 2024-03-15 14:40:03.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/_sa_types_backward.py
--rw-rw-rw-   0        0        0      422 2024-03-28 09:51:06.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.284628 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/
--rw-rw-rw-   0        0        0       37 2024-03-15 14:40:03.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/__init__.py
--rw-rw-rw-   0        0        0      175 2024-03-15 14:40:03.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/_sa_types.py
--rw-rw-rw-   0        0        0      555 2024-03-15 14:40:03.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py
--rw-rw-rw-   0        0        0     1167 2024-03-17 10:19:18.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/factory.py
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.304311 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:37:07.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/__init__.py
--rw-rw-rw-   0        0        0     1881 2024-03-17 15:54:11.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/base.py
--rw-rw-rw-   0        0        0     3209 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/mysql.py
--rw-rw-rw-   0        0        0     3214 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/postgresql.py
--rw-rw-rw-   0        0        0      210 2023-06-16 06:26:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/exceptions.py
--rw-rw-rw-   0        0        0     2248 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/factory.py
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.321193 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:37:07.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/base.py
--rw-rw-rw-   0        0        0     5397 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/mysql.py
--rw-rw-rw-   0        0        0     7621 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/postgresql.py
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.335785 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/statement/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:37:07.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/statement/__init__.py
--rw-rw-rw-   0        0        0      119 2023-06-25 13:52:18.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/statement/mysql.py
--rw-rw-rw-   0        0        0      686 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/statement/postgresql.py
--rw-rw-rw-   0        0        0     2452 2024-03-27 13:36:40.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-28 09:51:07.339786 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/
--rw-rw-rw-   0        0        0     9597 2024-03-28 09:51:06.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2024-03-28 09:51:07.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 09:51:06.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      463 2024-03-28 09:51:06.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-28 09:51:06.000000 sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.416332 sqlalchemy-dlock-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:24:39.416332 sqlalchemy-dlock-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.404332 sqlalchemy-dlock-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.408332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_sa_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_sa_types_backward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.408332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/_sa_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-06 15:24:32.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:24:39.412332 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 15:24:39.000000 sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/top_level.txt
```

### Comparing `sqlalchemy-dlock-0.6/CHANGELOG.md` & `sqlalchemy-dlock-0.6.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGELOG
 
+## v0.6.1
+
+> 📅 **Date** 2024-4-6
+
+- ✅ Changes:
+  - `typing-extensions` required for Python earlier than 3.10
+
 ## v0.6
 
 > 📅 **Date** 2024-3-28
 
 - ❎ Breaking Changes:
   - Remove `level` arguments of PostgreSQL lock class' constructor.
     `xact` and `shared` arguments were added.
```

### Comparing `sqlalchemy-dlock-0.6/LICENSE` & `sqlalchemy-dlock-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6/PKG-INFO` & `sqlalchemy-dlock-0.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-dlock
-Version: 0.6
-Summary: A distributed lock implementation based on SQLAlchemy
-Author-email: liu xue yan <liu_xue_yan@foxmail.com>
-License: BSD-3-Clause
-Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
-Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
-Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
-Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Database :: Front-Ends
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-Requires-Dist: SQLAlchemy<3.0,>=1.4
-Requires-Dist: typing-extensions; python_version < "3.11"
-Provides-Extra: asyncio
-Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncio"
-Provides-Extra: mysqlclient
-Requires-Dist: mysqlclient; extra == "mysqlclient"
-Provides-Extra: pymysql
-Requires-Dist: pymysql; extra == "pymysql"
-Provides-Extra: aiomysql
-Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "aiomysql"
-Requires-Dist: aiomysql; extra == "aiomysql"
-Provides-Extra: psycopg2
-Requires-Dist: psycopg2>=2.8; extra == "psycopg2"
-Provides-Extra: psycopg2-binary
-Requires-Dist: psycopg2-binary>=2.8; extra == "psycopg2-binary"
-Provides-Extra: psycopg3
-Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3"
-Requires-Dist: psycopg; extra == "psycopg3"
-Provides-Extra: psycopg3-binary
-Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-binary"
-Requires-Dist: psycopg[binary]; extra == "psycopg3-binary"
-Provides-Extra: psycopg3-c
-Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-c"
-Requires-Dist: psycopg[c]; extra == "psycopg3-c"
-Provides-Extra: asyncpg
-Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncpg"
-Requires-Dist: asyncpg; extra == "asyncpg"
-
-# sqlalchemy-dlock
-
-[![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
-[![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![Documentation Status](https://readthedocs.org/projects/sqlalchemy-dlock/badge/?version=latest)](https://sqlalchemy-dlock.readthedocs.io/en/latest/)
-[![codecov](https://codecov.io/gh/tanbro/sqlalchemy-dlock/branch/main/graph/badge.svg)](https://codecov.io/gh/tanbro/sqlalchemy-dlock)
-
-`sqlalchemy-dlock` is a distributed-lock library based on Database and [SQLAlchemy][].
-
-It currently supports below locks:
-
- Database  |                                             Lock
----------- | ---------------------------------------------------------------------------------------------
-MySQL      | [named lock](https://dev.mysql.com/doc/refman/en/locking-functions.html)
-PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
-
-## Install
-
-```bash
-pip install sqlalchemy-dlock
-```
-
-## Usage
-
-- Work with [SQLAlchemy][] [`Connection`](https://docs.sqlalchemy.org/20/core/connections.html):
-
-  ```python
-  from sqlalchemy import create_engine
-  from sqlalchemy_dlock import create_sadlock
-
-  key = 'user/001'
-
-  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
-  conn = engine.connect()
-
-  # Create the D-Lock on the connection
-  lock = create_sadlock(conn, key)
-
-  # it's not lock when constructed
-  assert not lock.locked
-
-  # lock
-  lock.acquire()
-  assert lock.locked
-
-  # un-lock
-  lock.release()
-  assert not lock.locked
-  ```
-
-- `with` statement
-
-  ```python
-  from contextlib import closing
-
-  from sqlalchemy import create_engine
-  from sqlalchemy_dlock import create_sadlock
-
-  key = 'user/001'
-
-  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
-  with engine.connect() as conn:
-
-      # Create the D-Lock on the connection
-      with create_sadlock(conn, key) as lock:
-          # It's locked
-          assert lock.locked
-
-      # Auto un-locked
-      assert not lock.locked
-
-      # If do not want to be locked in `with`, a `closing` wrapper may help
-      with closing(create_sadlock(conn, key)) as lock2:
-          # It's NOT locked here !!!
-          assert not lock2.locked
-          # lock it now:
-          lock2.acquire()
-          assert lock2.locked
-
-      # Auto un-locked
-      assert not lock2.locked
-  ```
-
-- Work with [SQLAlchemy][] [`ORM` `Session`](https://docs.sqlalchemy.org/en/20/orm/session.html):
-
-  ```python
-  from sqlalchemy import create_engine
-  from sqlalchemy.orm import sessionmaker
-  from sqlalchemy_dlock import create_sadlock
-
-  key = 'user/001'
-
-  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
-  Session = sessionmaker(bind=engine)
-
-  with Session() as session:
-    with create_sadlock(session, key) as lock:
-        assert lock.locked
-    assert not lock.locked
-  ```
-
-- Asynchronous I/O Support
-
-  > 💡 **TIP**
-  >
-  > - [SQLAlchemy][] `1.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
-  > - [SQLAlchemy][] `2.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
-
-  ```python
-  from sqlalchemy.ext.asyncio import create_async_engine
-  from sqlalchemy_dlock.asyncio import create_async_sadlock
-
-  key = 'user/001'
-
-  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
-
-  async with engine.connect() as conn:
-      async with create_async_sadlock(conn, key) as lock:
-          assert lock.locked
-          await lock.release()
-          assert not lock.locked
-          await lock.acquire()
-      assert not lock.locked
-  ```
-
-  > ℹ️ **NOTE** \
-  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers.
-  >
-  > We can install it with asynchronous DB libraries:
-  >
-  > ```bash
-  > pip install SQLAlchemy[asyncio] aiomysql sqlalchemy-dlock
-  > ```
-  >
-  > or
-  >
-  > ```bash
-  > pip install SQLAlchemy[asyncio] asyncpg sqlalchemy-dlock
-  > ```
-
-## Test
-
-Following drivers are tested:
-
-- MySQL:
-  - [mysqlclient][] (synchronous)
-  - [pymysql][] (synchronous)
-  - [aiomysql][] (asynchronous)
-- Postgres:
-  - [psycopg2][] (synchronous)
-  - [asyncpg][] (asynchronous)
-  - [psycopg][] (synchronous and asynchronous)
-
-You can run unit-tests
-
-- on local environment:
-
-  1. Install the project in editable mode with `asyncio` optional dependencies, and libraries/drivers needed in test. A virtual environment ([venv][]) is strongly advised:
-
-     ```bash
-     pip install -e .[asyncio] -r tests/requirements.txt
-     ```
-
-  1. start up mysql and postgresql service
-
-     There is a docker [compose][] file `db.docker-compose.yml` in project's top directory,
-     which can be used to run mysql and postgresql develop environment conveniently:
-
-     ```bash
-     docker compose -f db.docker-compose.yml up
-     ```
-
-  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
-     Multiple connections separated by space.
-
-     eg: (following values are also the defaults, and can be omitted)
-
-     ```ini
-     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
-     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
-     ```
-
-     > ℹ️ **NOTE** \
-     > The test cases would load environment variables from dot-env file `tests/.env`.
-
-  1. run unit-test
-
-     ```bash
-     python -m unittest
-     ```
-
-- or on docker [compose][]:
-
-  `tests/docker-compose.yml` defines a Python and [SQLAlchemy][] version matrix -- it combines Python `3.8` to `3.12` and [SQLAlchemy][] `v1`/`v2` for test cases. We can run it by:
-
-  ```bash
-  cd tests
-  docker-compose up --abort-on-container-exit
-  ```
-
-[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-[venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
-[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
-[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
-[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
-[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
-[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
-[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
-[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
+Metadata-Version: 2.1
+Name: sqlalchemy-dlock
+Version: 0.6.1
+Summary: A distributed lock implementation based on SQLAlchemy
+Author-email: liu xue yan <liu_xue_yan@foxmail.com>
+License: BSD-3-Clause
+Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
+Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
+Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
+Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: SQLAlchemy<3.0,>=1.4
+Requires-Dist: typing-extensions; python_version < "3.10"
+Provides-Extra: asyncio
+Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncio"
+Provides-Extra: mysqlclient
+Requires-Dist: mysqlclient; extra == "mysqlclient"
+Provides-Extra: pymysql
+Requires-Dist: pymysql; extra == "pymysql"
+Provides-Extra: aiomysql
+Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "aiomysql"
+Requires-Dist: aiomysql; extra == "aiomysql"
+Provides-Extra: psycopg2
+Requires-Dist: psycopg2>=2.8; extra == "psycopg2"
+Provides-Extra: psycopg2-binary
+Requires-Dist: psycopg2-binary>=2.8; extra == "psycopg2-binary"
+Provides-Extra: psycopg3
+Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3"
+Requires-Dist: psycopg; extra == "psycopg3"
+Provides-Extra: psycopg3-binary
+Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-binary"
+Requires-Dist: psycopg[binary]; extra == "psycopg3-binary"
+Provides-Extra: psycopg3-c
+Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-c"
+Requires-Dist: psycopg[c]; extra == "psycopg3-c"
+Provides-Extra: asyncpg
+Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncpg"
+Requires-Dist: asyncpg; extra == "asyncpg"
+
+# sqlalchemy-dlock
+
+[![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
+[![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
+[![Documentation Status](https://readthedocs.org/projects/sqlalchemy-dlock/badge/?version=latest)](https://sqlalchemy-dlock.readthedocs.io/en/latest/)
+[![codecov](https://codecov.io/gh/tanbro/sqlalchemy-dlock/branch/main/graph/badge.svg)](https://codecov.io/gh/tanbro/sqlalchemy-dlock)
+
+`sqlalchemy-dlock` is a distributed-lock library based on Database and [SQLAlchemy][].
+
+It currently supports below locks:
+
+ Database  |                                             Lock
+---------- | ---------------------------------------------------------------------------------------------
+MySQL      | [named lock](https://dev.mysql.com/doc/refman/en/locking-functions.html)
+PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
+
+## Install
+
+```bash
+pip install sqlalchemy-dlock
+```
+
+## Usage
+
+- Work with [SQLAlchemy][] [`Connection`](https://docs.sqlalchemy.org/20/core/connections.html):
+
+  ```python
+  from sqlalchemy import create_engine
+  from sqlalchemy_dlock import create_sadlock
+
+  key = 'user/001'
+
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
+  conn = engine.connect()
+
+  # Create the D-Lock on the connection
+  lock = create_sadlock(conn, key)
+
+  # it's not lock when constructed
+  assert not lock.locked
+
+  # lock
+  lock.acquire()
+  assert lock.locked
+
+  # un-lock
+  lock.release()
+  assert not lock.locked
+  ```
+
+- `with` statement
+
+  ```python
+  from contextlib import closing
+
+  from sqlalchemy import create_engine
+  from sqlalchemy_dlock import create_sadlock
+
+  key = 'user/001'
+
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
+  with engine.connect() as conn:
+
+      # Create the D-Lock on the connection
+      with create_sadlock(conn, key) as lock:
+          # It's locked
+          assert lock.locked
+
+      # Auto un-locked
+      assert not lock.locked
+
+      # If do not want to be locked in `with`, a `closing` wrapper may help
+      with closing(create_sadlock(conn, key)) as lock2:
+          # It's NOT locked here !!!
+          assert not lock2.locked
+          # lock it now:
+          lock2.acquire()
+          assert lock2.locked
+
+      # Auto un-locked
+      assert not lock2.locked
+  ```
+
+- Work with [SQLAlchemy][] [`ORM` `Session`](https://docs.sqlalchemy.org/en/20/orm/session.html):
+
+  ```python
+  from sqlalchemy import create_engine
+  from sqlalchemy.orm import sessionmaker
+  from sqlalchemy_dlock import create_sadlock
+
+  key = 'user/001'
+
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
+  Session = sessionmaker(bind=engine)
+
+  with Session() as session:
+    with create_sadlock(session, key) as lock:
+        assert lock.locked
+    assert not lock.locked
+  ```
+
+- Asynchronous I/O Support
+
+  > 💡 **TIP**
+  >
+  > - [SQLAlchemy][] `1.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
+  > - [SQLAlchemy][] `2.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
+
+  ```python
+  from sqlalchemy.ext.asyncio import create_async_engine
+  from sqlalchemy_dlock.asyncio import create_async_sadlock
+
+  key = 'user/001'
+
+  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
+
+  async with engine.connect() as conn:
+      async with create_async_sadlock(conn, key) as lock:
+          assert lock.locked
+          await lock.release()
+          assert not lock.locked
+          await lock.acquire()
+      assert not lock.locked
+  ```
+
+  > ℹ️ **NOTE** \
+  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers.
+  >
+  > We can install it with asynchronous DB libraries:
+  >
+  > ```bash
+  > pip install SQLAlchemy[asyncio] aiomysql sqlalchemy-dlock
+  > ```
+  >
+  > or
+  >
+  > ```bash
+  > pip install SQLAlchemy[asyncio] asyncpg sqlalchemy-dlock
+  > ```
+
+## Test
+
+Following drivers are tested:
+
+- MySQL:
+  - [mysqlclient][] (synchronous)
+  - [pymysql][] (synchronous)
+  - [aiomysql][] (asynchronous)
+- Postgres:
+  - [psycopg2][] (synchronous)
+  - [asyncpg][] (asynchronous)
+  - [psycopg][] (synchronous and asynchronous)
+
+You can run unit-tests
+
+- on local environment:
+
+  1. Install the project in editable mode with `asyncio` optional dependencies, and libraries/drivers needed in test. A virtual environment ([venv][]) is strongly advised:
+
+     ```bash
+     pip install -e .[asyncio] -r tests/requirements.txt
+     ```
+
+  1. start up mysql and postgresql service
+
+     There is a docker [compose][] file `db.docker-compose.yml` in project's top directory,
+     which can be used to run mysql and postgresql develop environment conveniently:
+
+     ```bash
+     docker compose -f db.docker-compose.yml up
+     ```
+
+  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+     Multiple connections separated by space.
+
+     eg: (following values are also the defaults, and can be omitted)
+
+     ```ini
+     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
+     ```
+
+     > ℹ️ **NOTE** \
+     > The test cases would load environment variables from dot-env file `tests/.env`.
+
+  1. run unit-test
+
+     ```bash
+     python -m unittest
+     ```
+
+- or on docker [compose][]:
+
+  `tests/docker-compose.yml` defines a Python and [SQLAlchemy][] version matrix -- it combines Python `3.8` to `3.12` and [SQLAlchemy][] `v1`/`v2` for test cases. We can run it by:
+
+  ```bash
+  cd tests
+  docker compose up --abort-on-container-exit
+  ```
+
+[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
+[venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
+[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
+[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
+[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
+[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
+[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
+[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
+[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
```

### Comparing `sqlalchemy-dlock-0.6/README.md` & `sqlalchemy-dlock-0.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
 - or on docker [compose][]:
 
   `tests/docker-compose.yml` defines a Python and [SQLAlchemy][] version matrix -- it combines Python `3.8` to `3.12` and [SQLAlchemy][] `v1`/`v2` for test cases. We can run it by:
 
   ```bash
   cd tests
-  docker-compose up --abort-on-container-exit
+  docker compose up --abort-on-container-exit
   ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
 [mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
 [psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
 [psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
```

### Comparing `sqlalchemy-dlock-0.6/pyproject.toml` & `sqlalchemy-dlock-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 dynamic = ["version"]
 
 # requires python version
 requires-python = ">=3.7"
 # requires
 dependencies = [
   "SQLAlchemy>=1.4,<3.0",
-  "typing-extensions; python_version<'3.11'",
+  "typing-extensions; python_version<'3.10'",
 ]
 # extra requires
 [project.optional-dependencies]
 # SQLAlchemy with asyncio, no engines
 asyncio = ["SQLAlchemy[asyncio]>=1.4,<3.0"]
 # MySQL
 mysqlclient = ["mysqlclient"]
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/_sa_types_backward.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/_sa_types_backward.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/_sa_types_backward.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/factory.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/factory.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/base.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from typing import Any, Union
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .._sa_types_backward import TAsyncConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from .._sa_types import TAsyncConnectionOrSession
+else:  # pragma: no cover
+    from .._sa_types_backward import TAsyncConnectionOrSession
 
 
 class BaseAsyncSadLock:
     def __init__(
         self,
         connection_or_session: TAsyncConnectionOrSession,
         key: Any,
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/mysql.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import sys
-from typing import Any, Callable, Union
+from typing import Union
 
 from ...exceptions import SqlAlchemyDLockDatabaseError
 from ...lock.mysql import MysqlSadLockMixin
 from ...statement.mysql import LOCK, UNLOCK
 from .base import BaseAsyncSadLock
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .._sa_types_backward import TAsyncConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from .._sa_types import TAsyncConnectionOrSession
+else:  # pragma: no cover
+    from .._sa_types_backward import TAsyncConnectionOrSession
 
 MYSQL_LOCK_NAME_MAX_LENGTH = 64
 
-TConvertFunction = Callable[[Any], str]
-
 
 def default_convert(key: Union[bytearray, bytes, int, float]) -> str:
     if isinstance(key, (bytearray, bytes)):
         result = key.decode()
     elif isinstance(key, (int, float)):
         result = str(key)
     else:
         raise TypeError(f"{type(key)}")
     return result
 
 
-class MysqlAsyncSadLock(BaseAsyncSadLock, MysqlSadLockMixin):
+class MysqlAsyncSadLock(MysqlSadLockMixin, BaseAsyncSadLock):
     def __init__(self, connection_or_session: TAsyncConnectionOrSession, key, **kwargs):
         MysqlSadLockMixin.__init__(self, key=key, **kwargs)
         BaseAsyncSadLock.__init__(self, connection_or_session, self._actual_key, **kwargs)
 
     async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/asyncio/lock/postgresql.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/asyncio/lock/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from warnings import warn
 
 from ...exceptions import SqlAlchemyDLockDatabaseError
 from ...lock.postgresql import PostgresqlSadLockMixin
 from ...statement.postgresql import SLEEP_INTERVAL_DEFAULT, SLEEP_INTERVAL_MIN
 from .base import BaseAsyncSadLock
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .._sa_types_backward import TAsyncConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from .._sa_types import TAsyncConnectionOrSession
+else:  # pragma: no cover
+    from .._sa_types_backward import TAsyncConnectionOrSession
 
 
-class PostgresqlAsyncSadLock(BaseAsyncSadLock, PostgresqlSadLockMixin):
+class PostgresqlAsyncSadLock(PostgresqlSadLockMixin, BaseAsyncSadLock):
     def __init__(self, connection_or_session: TAsyncConnectionOrSession, key, **kwargs):
         PostgresqlSadLockMixin.__init__(self, key=key, **kwargs)
         BaseAsyncSadLock.__init__(self, connection_or_session, self._actual_key, **kwargs)
 
     async def acquire(
         self,
         block: bool = True,
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/factory.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import Type, Union
 
 from sqlalchemy.engine import Connection
 
 from .lock.base import BaseSadLock
 from .utils import pascal_case, safe_name
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from ._sa_types_backward import TConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from ._sa_types import TConnectionOrSession
+else:  # pragma: no cover
+    from ._sa_types_backward import TConnectionOrSession
 
 __all__ = ["create_sadlock"]
 
 
 def create_sadlock(
     connection_or_session: TConnectionOrSession, key, /, contextual_timeout: Union[float, int, None] = None, **kwargs
 ) -> BaseSadLock:
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/base.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from threading import local
 from typing import Union
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .._sa_types_backward import TConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from .._sa_types import TConnectionOrSession
+else:  # pragma: no cover
+    from .._sa_types_backward import TConnectionOrSession
 
 
 class BaseSadLock(local):
     """Base class of database lock implementation
 
     Note:
         * It's Thread-Local (:class:`threading.local`)
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/mysql.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/mysql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import sys
-from typing import Any, Callable, Optional, Union
+from typing import Any, Optional, Union
+
+if sys.version_info >= (3, 9):
+    from collections.abc import Callable
+else:
+    from typing import Callable
 
 from ..exceptions import SqlAlchemyDLockDatabaseError
 from ..statement.mysql import LOCK, UNLOCK
 from .base import BaseSadLock
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .._sa_types_backward import TConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from .._sa_types import TConnectionOrSession
+else:  # pragma: no cover
+    from .._sa_types_backward import TConnectionOrSession
 
 MYSQL_LOCK_NAME_MAX_LENGTH = 64
 
 
 def default_convert(key: Union[bytearray, bytes, int, float]) -> str:
     if isinstance(key, (bytearray, bytes)):
         result = key.decode()
@@ -59,31 +64,31 @@
         if not isinstance(key, str):
             raise TypeError("MySQL named lock requires the key given by string")
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
             raise ValueError(f"MySQL enforces a maximum length on lock names of {MYSQL_LOCK_NAME_MAX_LENGTH} characters.")
         self._actual_key = key
 
 
-class MysqlSadLock(BaseSadLock, MysqlSadLockMixin):
+class MysqlSadLock(MysqlSadLockMixin, BaseSadLock):
     """A distributed lock implemented by MySQL named-lock
 
     See Also:
         https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html
 
     Caution:
         To MySQL locking function, it is even possible for a given session to acquire multiple locks for the same name.
         Other sessions cannot acquire a lock with that name until the acquiring session releases all its locks for the name.
         When perform multiple :meth:`.acquire` for a key on the **same** SQLAlchemy connection, latter :meth:`.acquire` will success immediately no wait and never block, it causes cascade lock instead!
     """  # noqa: E501
 
     def __init__(self, connection_or_session: TConnectionOrSession, key, **kwargs):
         """
         Args:
-            connection_or_session: see :attr:`.BaseSadLock.connection_or_session`
-            key: see :attr:`.BaseSadLock.key`
+            connection_or_session: :attr:`.BaseSadLock.connection_or_session`
+            key: :attr:`.BaseSadLock.key`
             **kwargs: other named parameters pass to :class:`.BaseSadLock` and :class:`.MysqlSadLockMixin`
         """
         MysqlSadLockMixin.__init__(self, key=key, **kwargs)
         BaseSadLock.__init__(self, connection_or_session, self._actual_key, **kwargs)
 
     def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
         if self._acquired:
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/lock/postgresql.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/lock/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import sys
 from time import sleep, time
-from typing import Any, Callable, Optional, Union
+from typing import Any, Optional, Union
 from warnings import warn
 
+if sys.version_info >= (3, 9):
+    from collections.abc import Callable
+else:
+    from typing import Callable
+
 from ..exceptions import SqlAlchemyDLockDatabaseError
 from ..statement.postgresql import (
     LOCK,
     LOCK_SHARED,
     LOCK_XACT,
     LOCK_XACT_SHARED,
     SLEEP_INTERVAL_DEFAULT,
@@ -17,18 +22,18 @@
     TRY_LOCK_XACT_SHARED,
     UNLOCK,
     UNLOCK_SHARED,
 )
 from ..utils import ensure_int64, to_int64_key
 from .base import BaseSadLock
 
-if sys.version_info < (3, 12):  # pragma: no cover
-    from .._sa_types_backward import TConnectionOrSession
-else:  # pragma: no cover
+if sys.version_info >= (3, 12):  # pragma: no cover
     from .._sa_types import TConnectionOrSession
+else:  # pragma: no cover
+    from .._sa_types_backward import TConnectionOrSession
 
 
 class PostgresqlSadLockMixin:
     """A Mix-in class for PostgreSQL advisory lock"""
 
     def __init__(
         self, *, key, shared: bool = False, xact: bool = False, convert: Optional[Callable[[Any], int]] = None, **kwargs
@@ -44,16 +49,16 @@
 
                 * Or you can specify a ``convert`` function to that argument::
 
                     def convert(val: Any) -> int:
                         int64_key: int = do_sth(val)
                         return int64_key
 
-            shared: for :attr:`.shared`
-            xact: for :attr:`.xact`
+            shared: :attr:`.shared`
+            xact: :attr:`.xact`
             convert: Custom function to covert ``key`` to required data type.
         """  # noqa: E501
         if convert:
             key = ensure_int64(convert(key))
         elif isinstance(key, int):
             key = ensure_int64(key)
         else:
@@ -87,15 +92,15 @@
 
     @property
     def xact(self):
         """Is the advisory lock transaction level or session level"""
         return self._xact
 
 
-class PostgresqlSadLock(BaseSadLock, PostgresqlSadLockMixin):
+class PostgresqlSadLock(PostgresqlSadLockMixin, BaseSadLock):
     """A distributed lock implemented by PostgreSQL advisory lock
 
     See also:
         https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS
 
     Tip:
         Locks can be either shared or exclusive: a shared lock does not conflict with other shared locks on the same resource, only with exclusive locks.
@@ -103,18 +108,18 @@
         Multiple session-level lock requests stack, so that if the same resource identifier is locked three times there must then be three unlock requests to release the resource in advance of session end.
     """
 
     def __init__(self, connection_or_session: TConnectionOrSession, key, **kwargs):
         """
         Args:
             connection_or_session: see :attr:`.BaseSadLock.connection_or_session`
-            key: see :attr:`.BaseSadLock.key`
-            shared: see :attr:`.PostgresqlSadLockMixin.shared`
-            xact: see :attr:`.PostgresqlSadLockMixin.xact`
-            convert: see :class:`.PostgresqlSadLockMixin`
+            key: :attr:`.BaseSadLock.key`
+            shared: :attr:`.PostgresqlSadLockMixin.shared`
+            xact: :attr:`.PostgresqlSadLockMixin.xact`
+            convert: :class:`.PostgresqlSadLockMixin`
             **kwargs: other named parameters pass to :class:`.BaseSadLock` and :class:`.PostgresqlSadLockMixin`
         """  # noqa: E501
         PostgresqlSadLockMixin.__init__(self, key=key, **kwargs)
         BaseSadLock.__init__(self, connection_or_session, self._actual_key, **kwargs)
 
     def acquire(
         self,
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/statement/postgresql.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/statement/postgresql.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock/utils.py` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/PKG-INFO` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-dlock
-Version: 0.6
-Summary: A distributed lock implementation based on SQLAlchemy
-Author-email: liu xue yan <liu_xue_yan@foxmail.com>
-License: BSD-3-Clause
-Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
-Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
-Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
-Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Database :: Front-Ends
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-Requires-Dist: SQLAlchemy<3.0,>=1.4
-Requires-Dist: typing-extensions; python_version < "3.11"
-Provides-Extra: asyncio
-Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncio"
-Provides-Extra: mysqlclient
-Requires-Dist: mysqlclient; extra == "mysqlclient"
-Provides-Extra: pymysql
-Requires-Dist: pymysql; extra == "pymysql"
-Provides-Extra: aiomysql
-Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "aiomysql"
-Requires-Dist: aiomysql; extra == "aiomysql"
-Provides-Extra: psycopg2
-Requires-Dist: psycopg2>=2.8; extra == "psycopg2"
-Provides-Extra: psycopg2-binary
-Requires-Dist: psycopg2-binary>=2.8; extra == "psycopg2-binary"
-Provides-Extra: psycopg3
-Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3"
-Requires-Dist: psycopg; extra == "psycopg3"
-Provides-Extra: psycopg3-binary
-Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-binary"
-Requires-Dist: psycopg[binary]; extra == "psycopg3-binary"
-Provides-Extra: psycopg3-c
-Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-c"
-Requires-Dist: psycopg[c]; extra == "psycopg3-c"
-Provides-Extra: asyncpg
-Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncpg"
-Requires-Dist: asyncpg; extra == "asyncpg"
-
-# sqlalchemy-dlock
-
-[![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
-[![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
-[![Documentation Status](https://readthedocs.org/projects/sqlalchemy-dlock/badge/?version=latest)](https://sqlalchemy-dlock.readthedocs.io/en/latest/)
-[![codecov](https://codecov.io/gh/tanbro/sqlalchemy-dlock/branch/main/graph/badge.svg)](https://codecov.io/gh/tanbro/sqlalchemy-dlock)
-
-`sqlalchemy-dlock` is a distributed-lock library based on Database and [SQLAlchemy][].
-
-It currently supports below locks:
-
- Database  |                                             Lock
----------- | ---------------------------------------------------------------------------------------------
-MySQL      | [named lock](https://dev.mysql.com/doc/refman/en/locking-functions.html)
-PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
-
-## Install
-
-```bash
-pip install sqlalchemy-dlock
-```
-
-## Usage
-
-- Work with [SQLAlchemy][] [`Connection`](https://docs.sqlalchemy.org/20/core/connections.html):
-
-  ```python
-  from sqlalchemy import create_engine
-  from sqlalchemy_dlock import create_sadlock
-
-  key = 'user/001'
-
-  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
-  conn = engine.connect()
-
-  # Create the D-Lock on the connection
-  lock = create_sadlock(conn, key)
-
-  # it's not lock when constructed
-  assert not lock.locked
-
-  # lock
-  lock.acquire()
-  assert lock.locked
-
-  # un-lock
-  lock.release()
-  assert not lock.locked
-  ```
-
-- `with` statement
-
-  ```python
-  from contextlib import closing
-
-  from sqlalchemy import create_engine
-  from sqlalchemy_dlock import create_sadlock
-
-  key = 'user/001'
-
-  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
-  with engine.connect() as conn:
-
-      # Create the D-Lock on the connection
-      with create_sadlock(conn, key) as lock:
-          # It's locked
-          assert lock.locked
-
-      # Auto un-locked
-      assert not lock.locked
-
-      # If do not want to be locked in `with`, a `closing` wrapper may help
-      with closing(create_sadlock(conn, key)) as lock2:
-          # It's NOT locked here !!!
-          assert not lock2.locked
-          # lock it now:
-          lock2.acquire()
-          assert lock2.locked
-
-      # Auto un-locked
-      assert not lock2.locked
-  ```
-
-- Work with [SQLAlchemy][] [`ORM` `Session`](https://docs.sqlalchemy.org/en/20/orm/session.html):
-
-  ```python
-  from sqlalchemy import create_engine
-  from sqlalchemy.orm import sessionmaker
-  from sqlalchemy_dlock import create_sadlock
-
-  key = 'user/001'
-
-  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
-  Session = sessionmaker(bind=engine)
-
-  with Session() as session:
-    with create_sadlock(session, key) as lock:
-        assert lock.locked
-    assert not lock.locked
-  ```
-
-- Asynchronous I/O Support
-
-  > 💡 **TIP**
-  >
-  > - [SQLAlchemy][] `1.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
-  > - [SQLAlchemy][] `2.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
-
-  ```python
-  from sqlalchemy.ext.asyncio import create_async_engine
-  from sqlalchemy_dlock.asyncio import create_async_sadlock
-
-  key = 'user/001'
-
-  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
-
-  async with engine.connect() as conn:
-      async with create_async_sadlock(conn, key) as lock:
-          assert lock.locked
-          await lock.release()
-          assert not lock.locked
-          await lock.acquire()
-      assert not lock.locked
-  ```
-
-  > ℹ️ **NOTE** \
-  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers.
-  >
-  > We can install it with asynchronous DB libraries:
-  >
-  > ```bash
-  > pip install SQLAlchemy[asyncio] aiomysql sqlalchemy-dlock
-  > ```
-  >
-  > or
-  >
-  > ```bash
-  > pip install SQLAlchemy[asyncio] asyncpg sqlalchemy-dlock
-  > ```
-
-## Test
-
-Following drivers are tested:
-
-- MySQL:
-  - [mysqlclient][] (synchronous)
-  - [pymysql][] (synchronous)
-  - [aiomysql][] (asynchronous)
-- Postgres:
-  - [psycopg2][] (synchronous)
-  - [asyncpg][] (asynchronous)
-  - [psycopg][] (synchronous and asynchronous)
-
-You can run unit-tests
-
-- on local environment:
-
-  1. Install the project in editable mode with `asyncio` optional dependencies, and libraries/drivers needed in test. A virtual environment ([venv][]) is strongly advised:
-
-     ```bash
-     pip install -e .[asyncio] -r tests/requirements.txt
-     ```
-
-  1. start up mysql and postgresql service
-
-     There is a docker [compose][] file `db.docker-compose.yml` in project's top directory,
-     which can be used to run mysql and postgresql develop environment conveniently:
-
-     ```bash
-     docker compose -f db.docker-compose.yml up
-     ```
-
-  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
-     Multiple connections separated by space.
-
-     eg: (following values are also the defaults, and can be omitted)
-
-     ```ini
-     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
-     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
-     ```
-
-     > ℹ️ **NOTE** \
-     > The test cases would load environment variables from dot-env file `tests/.env`.
-
-  1. run unit-test
-
-     ```bash
-     python -m unittest
-     ```
-
-- or on docker [compose][]:
-
-  `tests/docker-compose.yml` defines a Python and [SQLAlchemy][] version matrix -- it combines Python `3.8` to `3.12` and [SQLAlchemy][] `v1`/`v2` for test cases. We can run it by:
-
-  ```bash
-  cd tests
-  docker-compose up --abort-on-container-exit
-  ```
-
-[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-[venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
-[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
-[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
-[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
-[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
-[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
-[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
-[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
+Metadata-Version: 2.1
+Name: sqlalchemy-dlock
+Version: 0.6.1
+Summary: A distributed lock implementation based on SQLAlchemy
+Author-email: liu xue yan <liu_xue_yan@foxmail.com>
+License: BSD-3-Clause
+Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
+Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
+Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
+Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: SQLAlchemy<3.0,>=1.4
+Requires-Dist: typing-extensions; python_version < "3.10"
+Provides-Extra: asyncio
+Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncio"
+Provides-Extra: mysqlclient
+Requires-Dist: mysqlclient; extra == "mysqlclient"
+Provides-Extra: pymysql
+Requires-Dist: pymysql; extra == "pymysql"
+Provides-Extra: aiomysql
+Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "aiomysql"
+Requires-Dist: aiomysql; extra == "aiomysql"
+Provides-Extra: psycopg2
+Requires-Dist: psycopg2>=2.8; extra == "psycopg2"
+Provides-Extra: psycopg2-binary
+Requires-Dist: psycopg2-binary>=2.8; extra == "psycopg2-binary"
+Provides-Extra: psycopg3
+Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3"
+Requires-Dist: psycopg; extra == "psycopg3"
+Provides-Extra: psycopg3-binary
+Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-binary"
+Requires-Dist: psycopg[binary]; extra == "psycopg3-binary"
+Provides-Extra: psycopg3-c
+Requires-Dist: SQLAlchemy<3.0,>=2.0; extra == "psycopg3-c"
+Requires-Dist: psycopg[c]; extra == "psycopg3-c"
+Provides-Extra: asyncpg
+Requires-Dist: SQLAlchemy[asyncio]<3.0,>=1.4; extra == "asyncpg"
+Requires-Dist: asyncpg; extra == "asyncpg"
+
+# sqlalchemy-dlock
+
+[![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
+[![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
+[![Documentation Status](https://readthedocs.org/projects/sqlalchemy-dlock/badge/?version=latest)](https://sqlalchemy-dlock.readthedocs.io/en/latest/)
+[![codecov](https://codecov.io/gh/tanbro/sqlalchemy-dlock/branch/main/graph/badge.svg)](https://codecov.io/gh/tanbro/sqlalchemy-dlock)
+
+`sqlalchemy-dlock` is a distributed-lock library based on Database and [SQLAlchemy][].
+
+It currently supports below locks:
+
+ Database  |                                             Lock
+---------- | ---------------------------------------------------------------------------------------------
+MySQL      | [named lock](https://dev.mysql.com/doc/refman/en/locking-functions.html)
+PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
+
+## Install
+
+```bash
+pip install sqlalchemy-dlock
+```
+
+## Usage
+
+- Work with [SQLAlchemy][] [`Connection`](https://docs.sqlalchemy.org/20/core/connections.html):
+
+  ```python
+  from sqlalchemy import create_engine
+  from sqlalchemy_dlock import create_sadlock
+
+  key = 'user/001'
+
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
+  conn = engine.connect()
+
+  # Create the D-Lock on the connection
+  lock = create_sadlock(conn, key)
+
+  # it's not lock when constructed
+  assert not lock.locked
+
+  # lock
+  lock.acquire()
+  assert lock.locked
+
+  # un-lock
+  lock.release()
+  assert not lock.locked
+  ```
+
+- `with` statement
+
+  ```python
+  from contextlib import closing
+
+  from sqlalchemy import create_engine
+  from sqlalchemy_dlock import create_sadlock
+
+  key = 'user/001'
+
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
+  with engine.connect() as conn:
+
+      # Create the D-Lock on the connection
+      with create_sadlock(conn, key) as lock:
+          # It's locked
+          assert lock.locked
+
+      # Auto un-locked
+      assert not lock.locked
+
+      # If do not want to be locked in `with`, a `closing` wrapper may help
+      with closing(create_sadlock(conn, key)) as lock2:
+          # It's NOT locked here !!!
+          assert not lock2.locked
+          # lock it now:
+          lock2.acquire()
+          assert lock2.locked
+
+      # Auto un-locked
+      assert not lock2.locked
+  ```
+
+- Work with [SQLAlchemy][] [`ORM` `Session`](https://docs.sqlalchemy.org/en/20/orm/session.html):
+
+  ```python
+  from sqlalchemy import create_engine
+  from sqlalchemy.orm import sessionmaker
+  from sqlalchemy_dlock import create_sadlock
+
+  key = 'user/001'
+
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
+  Session = sessionmaker(bind=engine)
+
+  with Session() as session:
+    with create_sadlock(session, key) as lock:
+        assert lock.locked
+    assert not lock.locked
+  ```
+
+- Asynchronous I/O Support
+
+  > 💡 **TIP**
+  >
+  > - [SQLAlchemy][] `1.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
+  > - [SQLAlchemy][] `2.x`'s asynchronous I/O: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
+
+  ```python
+  from sqlalchemy.ext.asyncio import create_async_engine
+  from sqlalchemy_dlock.asyncio import create_async_sadlock
+
+  key = 'user/001'
+
+  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
+
+  async with engine.connect() as conn:
+      async with create_async_sadlock(conn, key) as lock:
+          assert lock.locked
+          await lock.release()
+          assert not lock.locked
+          await lock.acquire()
+      assert not lock.locked
+  ```
+
+  > ℹ️ **NOTE** \
+  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers.
+  >
+  > We can install it with asynchronous DB libraries:
+  >
+  > ```bash
+  > pip install SQLAlchemy[asyncio] aiomysql sqlalchemy-dlock
+  > ```
+  >
+  > or
+  >
+  > ```bash
+  > pip install SQLAlchemy[asyncio] asyncpg sqlalchemy-dlock
+  > ```
+
+## Test
+
+Following drivers are tested:
+
+- MySQL:
+  - [mysqlclient][] (synchronous)
+  - [pymysql][] (synchronous)
+  - [aiomysql][] (asynchronous)
+- Postgres:
+  - [psycopg2][] (synchronous)
+  - [asyncpg][] (asynchronous)
+  - [psycopg][] (synchronous and asynchronous)
+
+You can run unit-tests
+
+- on local environment:
+
+  1. Install the project in editable mode with `asyncio` optional dependencies, and libraries/drivers needed in test. A virtual environment ([venv][]) is strongly advised:
+
+     ```bash
+     pip install -e .[asyncio] -r tests/requirements.txt
+     ```
+
+  1. start up mysql and postgresql service
+
+     There is a docker [compose][] file `db.docker-compose.yml` in project's top directory,
+     which can be used to run mysql and postgresql develop environment conveniently:
+
+     ```bash
+     docker compose -f db.docker-compose.yml up
+     ```
+
+  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+     Multiple connections separated by space.
+
+     eg: (following values are also the defaults, and can be omitted)
+
+     ```ini
+     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
+     ```
+
+     > ℹ️ **NOTE** \
+     > The test cases would load environment variables from dot-env file `tests/.env`.
+
+  1. run unit-test
+
+     ```bash
+     python -m unittest
+     ```
+
+- or on docker [compose][]:
+
+  `tests/docker-compose.yml` defines a Python and [SQLAlchemy][] version matrix -- it combines Python `3.8` to `3.12` and [SQLAlchemy][] `v1`/`v2` for test cases. We can run it by:
+
+  ```bash
+  cd tests
+  docker compose up --abort-on-container-exit
+  ```
+
+[SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
+[venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
+[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
+[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
+[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
+[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
+[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
+[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
+[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
```

### Comparing `sqlalchemy-dlock-0.6/src/sqlalchemy_dlock.egg-info/SOURCES.txt` & `sqlalchemy-dlock-0.6.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

