# Comparing `tmp/masonite-orm-2.9.1.tar.gz` & `tmp/masonite-orm-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/masonite-orm-2.9.1.tar", last modified: Fri Apr 22 02:53:55 2022, max compression
+gzip compressed data, was "dist/masonite-orm-2.9.2.tar", last modified: Thu May  5 11:50:43 2022, max compression
```

## Comparing `masonite-orm-2.9.1.tar` & `masonite-orm-2.9.2.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masonite_orm.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/query/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/EagerRelation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/query/processors/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/processors/SQLitePostProcessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/processors/PostgresPostProcessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/processors/MySQLPostProcessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/processors/MSSQLPostProcessor.py
--rw-r--r--   0 runner    (1001) docker     (121)    51123 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/QueryBuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/SQLiteGrammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/MSSQLGrammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5733 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/PostgresGrammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/MySQLGrammar.py
--rw-r--r--   0 runner    (1001) docker     (121)    31885 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/query/grammars/BaseGrammar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/HasMany.py
--rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/MorphTo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/BelongsTo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5175 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/MorphOne.py
--rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/BaseRelationship.py
--rw-r--r--   0 runner    (1001) docker     (121)     5139 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/MorphMany.py
--rw-r--r--   0 runner    (1001) docker     (121)     7559 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/HasOneThrough.py
--rw-r--r--   0 runner    (1001) docker     (121)     7559 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/HasManyThrough.py
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/HasOne.py
--rw-r--r--   0 runner    (1001) docker     (121)    14383 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/BelongsToMany.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/relationships/MorphToMany.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/CanOverrideConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MakeModelCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/ShellCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MakeSeedCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/Command.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MigrateRollbackCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MigrateResetCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/Entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MigrateCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/SeedRunCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MigrateStatusCommand.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/commands/stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/stubs/create_migration.stub
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/stubs/observer.stub
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/stubs/model.stub
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/stubs/create_seed.stub
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/stubs/table_migration.stub
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/CanOverrideOptionsDefault.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MigrateRefreshCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MakeMigrationCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/commands/MakeObserverCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/models/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/models/Pivot.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/models/MigrationModel.py
--rw-r--r--   0 runner    (1001) docker     (121)    27860 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/models/Model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/collection/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14847 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/collection/Collection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/expressions/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7547 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/expressions/expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/connections/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/SQLiteConnection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/MSSQLConnection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/PostgresConnection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/ConnectionResolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     4803 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/MySQLConnection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/ConnectionFactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/connections/BaseConnection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/pagination/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/pagination/SimplePaginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/pagination/LengthAwarePaginator.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/pagination/BasePaginator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/testing/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16792 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/testing/BaseTestCaseSelectGrammar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/providers/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/providers/ORMProvider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/schema/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7766 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/Schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    29203 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/Blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/ForeignKeyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/ColumnDiff.py
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/TableDiff.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/Index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/Column.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/Table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)    15449 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/MySQLPlatform.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12550 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/MSSQLPlatform.py
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/Platform.py
--rw-r--r--   0 runner    (1001) docker     (121)    14700 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/SQLitePlatform.py
--rw-r--r--   0 runner    (1001) docker     (121)    17593 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/platforms/PostgresPlatform.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/schema/Constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/factories/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/factories/Factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/seeds/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/seeds/Seeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4070 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/observers/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/observers/ObservesEvents.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8716 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/migrations/Migration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/UUIDPrimaryKeyMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/UUIDPrimaryKeyScope.py
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/SoftDeleteScope.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/SoftDeletesMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/TimeStampsMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/TimeStampsScope.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/scopes/BaseScope.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/src/masoniteorm/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/src/masoniteorm/helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-04-22 02:53:30.000000 masonite-orm-2.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-22 02:53:55.000000 masonite-orm-2.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/query/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/query/processors/
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/processors/SQLitePostProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/processors/PostgresPostProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/processors/MySQLPostProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/processors/MSSQLPostProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51276 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/QueryBuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/
+-rw-r--r--   0 runner    (1001) docker     (121)    31885 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/BaseGrammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5733 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/PostgresGrammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/MSSQLGrammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/MySQLGrammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/grammars/SQLiteGrammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/query/EagerRelation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     8716 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/migrations/Migration.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/expressions/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7547 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/expressions/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/connections/
+-rw-r--r--   0 runner    (1001) docker     (121)     5087 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/SQLiteConnection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/PostgresConnection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4803 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/MySQLConnection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/ConnectionResolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/MSSQLConnection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/BaseConnection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/ConnectionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/observers/
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/observers/ObservesEvents.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/observers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/models/Pivot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/models/MigrationModel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28239 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/models/Model.py
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/ColumnDiff.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7766 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/Column.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29203 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/Blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/TableDiff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/Table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/ForeignKeyConstraint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/
+-rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/Platform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14700 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/SQLitePlatform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15449 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/MySQLPlatform.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12550 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/MSSQLPlatform.py
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17593 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/platforms/PostgresPlatform.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/schema/Index.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/pagination/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/pagination/BasePaginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/pagination/SimplePaginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/pagination/LengthAwarePaginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4070 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MigrateStatusCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MigrateCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MakeObserverCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MakeModelCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/CanOverrideConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/commands/stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/stubs/table_migration.stub
+-rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/stubs/observer.stub
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/stubs/create_seed.stub
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/stubs/create_migration.stub
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/stubs/model.stub
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MigrateRollbackCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MigrateResetCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MakeSeedCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/Entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/CanOverrideOptionsDefault.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/Command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MigrateRefreshCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/ShellCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/SeedRunCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/MakeMigrationCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/
+-rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/MorphToMany.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5175 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/MorphOne.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7559 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/HasOneThrough.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14469 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/BelongsToMany.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7559 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/HasManyThrough.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/BaseRelationship.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/MorphTo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/BelongsTo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/HasMany.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/HasOne.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5139 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/MorphMany.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/relationships/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/factories/
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/factories/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)    16792 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/testing/BaseTestCaseSelectGrammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/seeds/
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/seeds/Seeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/seeds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/TimeStampsScope.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/UUIDPrimaryKeyScope.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/SoftDeletesMixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/scope.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/UUIDPrimaryKeyMixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/SoftDeleteScope.py
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/BaseScope.py
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/scopes/TimeStampsMixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/collection/
+-rw-r--r--   0 runner    (1001) docker     (121)    15234 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/collection/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/collection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masoniteorm/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/providers/ORMProvider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/src/masoniteorm/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 11:50:43.000000 masonite-orm-2.9.2/src/masonite_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-05-05 11:50:07.000000 masonite-orm-2.9.2/README.md
```

### Comparing `masonite-orm-2.9.1/setup.py` & `masonite-orm-2.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="masonite-orm",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="2.9.1",
+    version="2.9.2",
     package_dir={"": "src"},
     description="The Official Masonite ORM",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/masoniteframework/orm",
     # Author details
```

### Comparing `masonite-orm-2.9.1/PKG-INFO` & `masonite-orm-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-orm
-Version: 2.9.1
+Version: 2.9.2
 Summary: The Official Masonite ORM
 Home-page: https://github.com/masoniteframework/orm
 Author: Joe Mancuso
 Author-email: joe@masoniteproject.com
 License: MIT
 Description: <p align="center">
           <img src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4trhpkkdbbzutc5ufxi9.png" width="160px">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masonite-orm Version: 2.9.1 Summary: The Official
+Metadata-Version: 2.1 Name: masonite-orm Version: 2.9.2 Summary: The Official
 Masonite ORM Home-page: https://github.com/masoniteframework/orm Author: Joe
 Mancuso Author-email: joe@masoniteproject.com License: MIT Description:
           [https://dev-to-uploads.s3.amazonaws.com/uploads/articles/
                            4trhpkkdbbzutc5ufxi9.png]
                           ************ MMaassoonniittee OORRMM ************
  _[_M_a_s_o_n_i_t_e_ _P_a_c_k_a_g_e_][Python Version][GitHub release (latest by date)][License]
                               _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
```

### Comparing `masonite-orm-2.9.1/src/masonite_orm.egg-info/PKG-INFO` & `masonite-orm-2.9.2/src/masonite_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-orm
-Version: 2.9.1
+Version: 2.9.2
 Summary: The Official Masonite ORM
 Home-page: https://github.com/masoniteframework/orm
 Author: Joe Mancuso
 Author-email: joe@masoniteproject.com
 License: MIT
 Description: <p align="center">
           <img src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4trhpkkdbbzutc5ufxi9.png" width="160px">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masonite-orm Version: 2.9.1 Summary: The Official
+Metadata-Version: 2.1 Name: masonite-orm Version: 2.9.2 Summary: The Official
 Masonite ORM Home-page: https://github.com/masoniteframework/orm Author: Joe
 Mancuso Author-email: joe@masoniteproject.com License: MIT Description:
           [https://dev-to-uploads.s3.amazonaws.com/uploads/articles/
                            4trhpkkdbbzutc5ufxi9.png]
                           ************ MMaassoonniittee OORRMM ************
  _[_M_a_s_o_n_i_t_e_ _P_a_c_k_a_g_e_][Python Version][GitHub release (latest by date)][License]
                               _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
```

### Comparing `masonite-orm-2.9.1/src/masonite_orm.egg-info/SOURCES.txt` & `masonite-orm-2.9.2/src/masonite_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/EagerRelation.py` & `masonite-orm-2.9.2/src/masoniteorm/query/EagerRelation.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/processors/SQLitePostProcessor.py` & `masonite-orm-2.9.2/src/masoniteorm/query/processors/SQLitePostProcessor.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/processors/PostgresPostProcessor.py` & `masonite-orm-2.9.2/src/masoniteorm/query/processors/PostgresPostProcessor.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/processors/MySQLPostProcessor.py` & `masonite-orm-2.9.2/src/masoniteorm/query/processors/MySQLPostProcessor.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/processors/MSSQLPostProcessor.py` & `masonite-orm-2.9.2/src/masoniteorm/query/processors/MSSQLPostProcessor.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/QueryBuilder.py` & `masonite-orm-2.9.2/src/masoniteorm/query/QueryBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,16 +808,15 @@
                 (
                     QueryExpression(
                         column, "IN", SubSelectExpression(wheres(self.new()))
                     )
                 ),
             )
         else:
-            wheres = [str(x) for x in wheres]
-            self._wheres += ((QueryExpression(column, "IN", wheres)),)
+            self._wheres += ((QueryExpression(column, "IN", list(wheres))),)
         return self
 
     def get_relation(self, relationship, builder=None):
         if not builder:
             builder = self
 
         if not builder._model:
@@ -869,16 +868,15 @@
         wheres = wheres or []
 
         if isinstance(wheres, QueryBuilder):
             self._wheres += (
                 (QueryExpression(column, "NOT IN", SubSelectExpression(wheres))),
             )
         else:
-            wheres = [str(x) for x in wheres]
-            self._wheres += ((QueryExpression(column, "NOT IN", wheres)),)
+            self._wheres += ((QueryExpression(column, "NOT IN", list(wheres))),)
         return self
 
     def join(
         self, table: str, column1=None, equality=None, column2=None, clause="inner"
     ):
         """Specifies a join expression.
 
@@ -1596,14 +1594,24 @@
         for name, scope in self._global_scopes.get(self._action, {}).items():
             scope(self)
 
         grammar = self.get_grammar()
         sql = grammar.compile(self._action, qmark=False).to_sql()
         return sql
 
+    def explain(self):
+        """Explains the Query execution plan.
+
+        Returns:
+            Collection
+        """
+        sql = self.to_sql()
+        explanation = self.statement(f'EXPLAIN {sql}')
+        return explanation
+
     def run_scopes(self):
         for name, scope in self._global_scopes.get(self._action, {}).items():
             scope(self)
 
         return self
 
     def to_qmark(self):
```

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/grammars/SQLiteGrammar.py` & `masonite-orm-2.9.2/src/masoniteorm/query/grammars/SQLiteGrammar.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/grammars/MSSQLGrammar.py` & `masonite-orm-2.9.2/src/masoniteorm/query/grammars/MSSQLGrammar.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/grammars/PostgresGrammar.py` & `masonite-orm-2.9.2/src/masoniteorm/query/grammars/PostgresGrammar.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/grammars/MySQLGrammar.py` & `masonite-orm-2.9.2/src/masoniteorm/query/grammars/MySQLGrammar.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/query/grammars/BaseGrammar.py` & `masonite-orm-2.9.2/src/masoniteorm/query/grammars/BaseGrammar.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/HasMany.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/HasMany.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/MorphTo.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/MorphTo.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/BelongsTo.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/BelongsTo.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/MorphOne.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/MorphOne.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/BaseRelationship.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/BaseRelationship.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/MorphMany.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/MorphMany.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/HasOneThrough.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/HasOneThrough.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/HasManyThrough.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/HasManyThrough.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/HasOne.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/HasOne.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/BelongsToMany.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/BelongsToMany.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,22 +135,22 @@
                 model.delete_attribute("m_reserved3")
 
             if self.with_fields:
                 for field in self.with_fields:
                     pivot_data.update({field: getattr(model, field)})
                     model.delete_attribute(field)
 
-            setattr(
-                model,
-                self._as,
-                Pivot.on(query.connection)
-                .table(self._table)
-                .hydrate(pivot_data)
-                .activate_timestamps(self.with_timestamps),
-            )
+            model.__original_attributes__.update({
+                self._as: (
+                    Pivot.on(query.connection)
+                    .table(self._table)
+                    .hydrate(pivot_data)
+                    .activate_timestamps(self.with_timestamps)
+                )
+            })
 
         return result
 
     def table(self, table):
         self._table = table
         return self
 
@@ -266,22 +266,22 @@
                 model.delete_attribute("m_reserved3")
 
             if self.with_fields:
                 for field in self.with_fields:
                     pivot_data.update({field: getattr(model, field)})
                     model.delete_attribute(field)
 
-            setattr(
-                model,
-                self._as,
-                Pivot.on(builder.connection)
-                .table(self._table)
-                .hydrate(pivot_data)
-                .activate_timestamps(self.with_timestamps),
-            )
+            model.__original_attributes__.update({
+                self._as: (
+                    Pivot.on(builder.connection)
+                    .table(self._table)
+                    .hydrate(pivot_data)
+                    .activate_timestamps(self.with_timestamps)
+                )
+            })
 
         return final_result
 
     def register_related(self, key, model, collection):
         model.add_relation(
             {
                 key: collection.where(
```

### Comparing `masonite-orm-2.9.1/src/masoniteorm/relationships/MorphToMany.py` & `masonite-orm-2.9.2/src/masoniteorm/relationships/MorphToMany.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/__init__.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MakeModelCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MakeModelCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/ShellCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/ShellCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MakeSeedCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MakeSeedCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MigrateRollbackCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MigrateRollbackCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MigrateResetCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MigrateResetCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/Entry.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/Entry.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MigrateCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MigrateCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/SeedRunCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/SeedRunCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MigrateStatusCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MigrateStatusCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/stubs/observer.stub` & `masonite-orm-2.9.2/src/masoniteorm/commands/stubs/observer.stub`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/CanOverrideOptionsDefault.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/CanOverrideOptionsDefault.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MigrateRefreshCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MigrateRefreshCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MakeMigrationCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MakeMigrationCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/commands/MakeObserverCommand.py` & `masonite-orm-2.9.2/src/masoniteorm/commands/MakeObserverCommand.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/models/Model.py` & `masonite-orm-2.9.2/src/masoniteorm/models/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         "decrement",
         "delete",
         "find_or_404",
         "find_or_fail",
         "first_or_fail",
         "first",
         "first_where",
+        "first_or_create",
         "force_update",
         "from_",
         "from_raw",
         "get",
         "group_by_raw",
         "group_by",
         "has",
@@ -345,20 +346,14 @@
         result = cls.find(record_id, query)
 
         if not result:
             raise ModelNotFound()
 
         return result
 
-    def first_or_new(self):
-        pass
-
-    def first_or_create(self):
-        pass
-
     def is_loaded(self):
         return bool(self.__attributes__)
 
     def is_created(self):
         return self.get_primary_key() in self.__attributes__
 
     def add_relation(self, relations):
@@ -565,14 +560,30 @@
 
         Returns:
             string
         """
         return json.dumps(self.serialize())
 
     @classmethod
+    def first_or_create(cls, wheres, creates):
+        """Get the first record matching the attributes or create it.
+
+        Returns:
+            Model
+        """
+        self = cls()
+        record = self.where(wheres).first()
+        total = {}
+        total.update(creates)
+        total.update(wheres)
+        if not record:
+            return self.create(total, id_key=cls.get_primary_key())
+        return record
+
+    @classmethod
     def update_or_create(cls, wheres, updates):
         self = cls()
         record = self.where(wheres).first()
         total = {}
         total.update(updates)
         total.update(wheres)
         if not record:
```

### Comparing `masonite-orm-2.9.1/src/masoniteorm/collection/Collection.py` & `masonite-orm-2.9.2/src/masoniteorm/collection/Collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,28 +405,36 @@
                 comparison = item.get(key)
             else:
                 comparison = getattr(item, key) if hasattr(item, key) else False
             if self._make_comparison(comparison, value, op):
                 attributes.append(item)
         return self.__class__(attributes)
 
-    def where_in(self, key, args: list):
+    def where_in(self, key, args: list) -> 'Collection':
 
         attributes = []
-        args = [str(x) for x in args]
 
         for item in self._items:
             if isinstance(item, dict):
+                if key not in item:
+                    continue
                 comparison = item.get(key)
             else:
-                comparison = getattr(item, key) if hasattr(item, key) else False
+                if not hasattr(item, key):
+                    continue
+                comparison = getattr(item, key)
 
-            if str(comparison) in args:
+            if comparison in args:
                 attributes.append(item)
 
+        # Compatibility patch - allow numeric strings to match integers
+        # (if all args are numeric strings and no matches were found)
+        if len(attributes) == 0 and all([isinstance(arg, str) and arg.isnumeric() for arg in args]):
+            return self.where_in(key, [int(arg) for arg in args])
+
         return self.__class__(attributes)
 
     def zip(self, items):
         items = self.__get_items(items)
         if not isinstance(items, list):
             raise ValueError("The 'items' parameter must be a list or a Collection")
```

### Comparing `masonite-orm-2.9.1/src/masoniteorm/expressions/expressions.py` & `masonite-orm-2.9.2/src/masoniteorm/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/SQLiteConnection.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/SQLiteConnection.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/MSSQLConnection.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/MSSQLConnection.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/PostgresConnection.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/PostgresConnection.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/ConnectionResolver.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/ConnectionResolver.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/MySQLConnection.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/MySQLConnection.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/ConnectionFactory.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/ConnectionFactory.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/connections/BaseConnection.py` & `masonite-orm-2.9.2/src/masoniteorm/connections/BaseConnection.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/pagination/SimplePaginator.py` & `masonite-orm-2.9.2/src/masoniteorm/pagination/SimplePaginator.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/pagination/LengthAwarePaginator.py` & `masonite-orm-2.9.2/src/masoniteorm/pagination/LengthAwarePaginator.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/testing/BaseTestCaseSelectGrammar.py` & `masonite-orm-2.9.2/src/masoniteorm/testing/BaseTestCaseSelectGrammar.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/providers/ORMProvider.py` & `masonite-orm-2.9.2/src/masoniteorm/providers/ORMProvider.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/Schema.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/Schema.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/Blueprint.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/Blueprint.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/ForeignKeyConstraint.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/ForeignKeyConstraint.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/TableDiff.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/TableDiff.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/Column.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/Column.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/Table.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/Table.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/platforms/MySQLPlatform.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/platforms/MySQLPlatform.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/platforms/MSSQLPlatform.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/platforms/MSSQLPlatform.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/platforms/Platform.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/platforms/Platform.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/platforms/SQLitePlatform.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/platforms/SQLitePlatform.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/schema/platforms/PostgresPlatform.py` & `masonite-orm-2.9.2/src/masoniteorm/schema/platforms/PostgresPlatform.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/factories/Factory.py` & `masonite-orm-2.9.2/src/masoniteorm/factories/Factory.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/seeds/Seeder.py` & `masonite-orm-2.9.2/src/masoniteorm/seeds/Seeder.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/config.py` & `masonite-orm-2.9.2/src/masoniteorm/config.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/migrations/Migration.py` & `masonite-orm-2.9.2/src/masoniteorm/migrations/Migration.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/scopes/UUIDPrimaryKeyScope.py` & `masonite-orm-2.9.2/src/masoniteorm/scopes/UUIDPrimaryKeyScope.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/scopes/SoftDeleteScope.py` & `masonite-orm-2.9.2/src/masoniteorm/scopes/SoftDeleteScope.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/scopes/TimeStampsScope.py` & `masonite-orm-2.9.2/src/masoniteorm/scopes/TimeStampsScope.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/src/masoniteorm/helpers/misc.py` & `masonite-orm-2.9.2/src/masoniteorm/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `masonite-orm-2.9.1/README.md` & `masonite-orm-2.9.2/README.md`

 * *Files identical despite different names*

