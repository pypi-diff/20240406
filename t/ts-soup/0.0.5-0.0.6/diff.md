# Comparing `tmp/ts-soup-0.0.5.tar.gz` & `tmp/ts-soup-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-uk6qaado\ts-soup-0.0.5.tar", last modified: Fri Apr  5 21:23:57 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-ti3kbx8q\ts-soup-0.0.6.tar", last modified: Fri Apr  5 21:50:44 2024, max compression
```

## Comparing `ts-soup-0.0.5.tar` & `ts-soup-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.287247 ts-soup-0.0.5/
--rw-rw-rw-   0        0        0     1028 2024-04-05 21:23:57.286234 ts-soup-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 21:23:57.287247 ts-soup-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-05 21:23:54.000000 ts-soup-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.277591 ts-soup-0.0.5/ts_soup/
--rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.5/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1322 2024-04-05 21:23:28.000000 ts-soup-0.0.5/ts_soup/app.py
--rw-rw-rw-   0        0        0    18041 2024-04-05 21:23:28.000000 ts-soup-0.0.5/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.284590 ts-soup-0.0.5/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.5/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.5/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.5/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:23:57.285594 ts-soup-0.0.5/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 21:23:57.000000 ts-soup-0.0.5/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.069219 ts-soup-0.0.6/
+-rw-rw-rw-   0        0        0     1028 2024-04-05 21:50:44.068221 ts-soup-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 21:50:44.069219 ts-soup-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-05 21:50:07.000000 ts-soup-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.060219 ts-soup-0.0.6/ts_soup/
+-rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.6/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts-soup-0.0.6/ts_soup/app.py
+-rw-rw-rw-   0        0        0    18128 2024-04-05 21:49:15.000000 ts-soup-0.0.6/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.066219 ts-soup-0.0.6/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.6/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.6/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.6/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.067219 ts-soup-0.0.6/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.0.5/PKG-INFO` & `ts-soup-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.5
+Version: 0.0.6
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.0.5/README.md` & `ts-soup-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.5/setup.py` & `ts-soup-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.0.5",
+  version="0.0.6",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.0.5/ts_soup/app.py` & `ts-soup-0.0.6/ts_soup/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 import importlib
 import os
 import sys
 
 from dateutil.relativedelta import relativedelta
 
 parser = argparse.ArgumentParser()
-parser.add_argument('--table',default=[],nargs='+')
-parser.add_argument('--time',default=[],nargs='+')
+parser.add_argument('--table', default=[], nargs='+')
+parser.add_argument('--time', default=[], nargs='+')
 args = parser.parse_args()
 
 from ts_soup.common import __init
 
 
-
-def run_sync(db_infos:dict, sync_start_from=None, sync_delay:int=1):
+def run_sync(db_infos: dict, sync_start_from=None, sync_delay: int = 1, funcs_file: str = 'funcs'):
     if sync_start_from is None:
         sync_start_from = {'months': 3}
+
     sync_end = datetime.datetime.now() + relativedelta(days=sync_delay)
     sync_start = (sync_end - relativedelta(**sync_start_from)).strftime('%Y-%m-%d')
     sync_end = sync_end.strftime('%Y-%m-%d')
     to_update_tables = __init(args.table, args.time, sync_start, sync_end, db_infos)
-    cwd = os.getcwd()
-    sys.path.append(os.path.join(cwd,'funcs'))
+
+    cwd = os.getcwd()  # 手动导包
+    sys.path.append(os.path.join(cwd, funcs_file))
     modules = []
-    for file in os.listdir(os.path.join(cwd,'funcs')):
+    for file in os.listdir(os.path.join(cwd, funcs_file)):
         modules.append(importlib.import_module(file.split('.')[0]))
-    for table in to_update_tables:
+
+    for table in to_update_tables:  # 执行funcs_name下模块的方法
         for module in modules:
             if table in dir(module):
-                getattr(module,table)()
+                getattr(module, table)()
 
-    # 检测是否异常
-    from ts_soup.common import EXECUTE_STATE
+    from ts_soup.common import EXECUTE_STATE  # 检测是否异常
     if not EXECUTE_STATE:
         raise Exception("同步异常")
 
 
-
 if __name__ == '__main__':
     pass
```

### Comparing `ts-soup-0.0.5/ts_soup/common.py` & `ts-soup-0.0.6/ts_soup/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import warnings
-from abc import abstractmethod,ABC
+from abc import abstractmethod, ABC
 from urllib import parse
 
 import pandas as pd
 from functools import wraps
 import traceback
 
 import pymysql
 from sqlalchemy import create_engine
+
 """
 """
 
 warnings.filterwarnings('ignore')
 
 USABLE_DBS = {}
 
@@ -23,33 +24,34 @@
 """
 DATA_UPDATED_STATE = None
 
 
 def query_in_sql(list_):
     return ','.join(list(map(lambda x: '"' + x + '"', list_)))
 
-def get_sqlalchemy_engine(db_info,db_type):
+
+def get_sqlalchemy_engine(db_info, db_type):
     global USABLE_DBS
     engine = create_engine(
         f'mysql+pymysql://{db_info["user"]}:{parse.quote_plus(db_info["pwd"])}@{db_info["ip"]}:3306/{db_info["db"]}')
     USABLE_DBS[db_info['alias']] = engine
     if db_info['default']:
         USABLE_DBS[f'{db_type}_default'] = engine
 
 
-def get_pymsql_engine(db_info,db_type):
+def get_pymsql_engine(db_info, db_type):
     global USABLE_DBS
     engine = pymysql.connect(
-                host=db_info['ip'],
-                user=db_info['user'],
-                password=db_info['pwd'],
-                port=int(db_info['port']),
-                database=db_info['db']
-                )
-    USABLE_DBS[db_info['alias']+'_pym'] = engine
+        host=db_info['ip'],
+        user=db_info['user'],
+        password=db_info['pwd'],
+        port=int(db_info['port']),
+        database=db_info['db']
+    )
+    USABLE_DBS[db_info['alias'] + '_pym'] = engine
     if db_info['default']:
         USABLE_DBS[f'{db_type}_default_pym'] = engine
 
 
 def __init(customized_table, customized_time, sync_start, sync_end, db_infos):
     """
      1、指定时间，未指定表格:
@@ -66,102 +68,103 @@
         to_update_tables: 返回查询结果
     :param sync_end: 同步结束日期
     :param sync_start: 同步开始日期
     :param customized_table: 手动指定的表
     :param customized_time: 手动指定的时间
     :return:
     """
-    global DATA_UPDATED_STATE,SYNC_FROM_DATE,CURRENT_DATE,USABLE_DBS
-    # 加载数据源配置 设置数据库连接
-    for db_type in ['sources', 'targets']:
+    global DATA_UPDATED_STATE, SYNC_FROM_DATE, CURRENT_DATE, USABLE_DBS
+
+    for db_type in ['sources', 'targets']:  # 加载数据源配置 设置数据库连接
         for db_info in db_infos[db_type]:
             engine_types = db_info.get('engine_type')
 
             if engine_types:
                 for engine_type in engine_types:
                     if engine_type == 'sqlalchemy':
-                        get_sqlalchemy_engine(db_info,db_type)
+                        get_sqlalchemy_engine(db_info, db_type)
                     else:
-                        get_pymsql_engine(db_info,db_type)
+                        get_pymsql_engine(db_info, db_type)
 
             else:
                 raise ValueError('未配置engine类型')
 
-
     SYNC_FROM_DATE = sync_start
     CURRENT_DATE = sync_end
     to_update_tables = pd.read_sql('select * from to_update_tables', con=USABLE_DBS['targets_default'])['table_name']
     with USABLE_DBS['targets_default'].begin() as conn:
         conn.execute("""
         CREATE TABLE if not exists `updated_state`  (
                       `update_date` date DEFAULT NULL,
                       `table_name` varchar(50) COLLATE utf8mb4_general_ci NOT NULL,
                       UNIQUE KEY `index` (`update_date`,`table_name`) USING BTREE COMMENT '唯一索引'
                     ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci
         """)
 
-    data_updated_state = pd.read_sql('select * from updated_state where update_date >= "{}"'.format(SYNC_FROM_DATE),con=USABLE_DBS['targets_default'])
-    # 统一时间类型
-    data_updated_state['update_date'] = pd.to_datetime(data_updated_state['update_date'])
+    data_updated_state = pd.read_sql('select * from updated_state where update_date >= "{}"'.format(SYNC_FROM_DATE),
+                                     con=USABLE_DBS['targets_default'])
+
+    data_updated_state['update_date'] = pd.to_datetime(data_updated_state['update_date'])  # 统一时间类型
     sync_date_range = pd.date_range(SYNC_FROM_DATE, CURRENT_DATE)
     fill_date_range = pd.DataFrame(sync_date_range, columns=['update_date'])
     fill_date_range['table_name'] = 'fill_date_range'
     # 利用fill_date_range把后面的Pivot table时间索引补全到 sync_from_date 开始到明天的日期
     data_updated_state = pd.concat([data_updated_state, fill_date_range])
     data_updated_state['state'] = 1
     pivot_table = data_updated_state.pivot_table(index='update_date', columns='table_name', values='state')
-    # 原来记录里有且现在仍需要的表
-    both_columns = [i for i in to_update_tables if i in pivot_table.columns.values.tolist()]
-    # 原来记录没有现在新增的表
-    non_columns = [i for i in to_update_tables if i not in pivot_table.columns.values.tolist()]
+
+    both_columns = [i for i in to_update_tables if i in pivot_table.columns.values.tolist()]  # 原来记录里有且现在仍需要的表
+
+    non_columns = [i for i in to_update_tables if i not in pivot_table.columns.values.tolist()]  # 原来记录没有现在新增的表
     state_table = pivot_table[both_columns].fillna(0)
     state_table[non_columns] = 0
     state_table = state_table.reset_index()
     state_table['update_date'] = state_table['update_date'].apply(lambda x: x.strftime('%Y-%m-%d'))
-    # 1、指定时间，未指定表格:
-    if len(customized_time) > 0 and len(customized_table) == 0:
+
+    if len(customized_time) > 0 and len(customized_table) == 0:  # 1、指定时间，未指定表格:
         DATA_UPDATED_STATE = state_table.loc[state_table['update_date'].isin(customized_time)]
-        DATA_UPDATED_STATE.iloc[:,1:] = 0
+        DATA_UPDATED_STATE.iloc[:, 1:] = 0
         return to_update_tables
-    # 2、指定表格，未指定时间：
-    elif len(customized_time) ==0 and len(customized_table) > 0:
+
+    elif len(customized_time) == 0 and len(customized_table) > 0:  # 2、指定表格，未指定时间：
         DATA_UPDATED_STATE = state_table
         return customized_table
-    # 3、指定时间，指定表格:
-    elif len(customized_time) > 0 and len(customized_table) > 0:
+
+    elif len(customized_time) > 0 and len(customized_table) > 0:  # 3、指定时间，指定表格:
         DATA_UPDATED_STATE = state_table.loc[state_table['update_date'].isin(customized_time)]
         DATA_UPDATED_STATE.loc[:, customized_table] = 0
         return customized_table
-    # 4、未指定时间，未指定表格:
+
     else:
-        DATA_UPDATED_STATE = state_table
+        DATA_UPDATED_STATE = state_table  # 4、未指定时间，未指定表格:
         return to_update_tables
 
 
 class BaseSource(ABC):
-    def __init__(self, db,index_field,empty_check):
+    def __init__(self, db, index_field, empty_check):
         """
         :param db: 数据库名
         :param index_field: 数据源筛选日期的字段，如果不提供则默认"date",如果需要查询全表，则index_field需要设置为 None。
         :param empty_check: 是否为当前方法主要数据源（除了配置信息的数据源），判空时使用，若不想使当前数据源参与判空，可设为 False
         """
         self.empty_check = empty_check
         if db:
             self.db = USABLE_DBS[db]
         else:
             self.db = USABLE_DBS['sources_default']
         self.index_field = index_field
 
-
     @abstractmethod
     def build_source(self, to_update_date):
         pass
 
+
 class BaseTarget(ABC):
-    def __init__(self,tb,index_field, db, user_def_pro,drop_axis,drop_na_subset,drop_na_thresh,has_unique_idx,is_seperated):
+    def __init__(self, tb, index_field, db, user_def_pro, drop_axis, drop_na_subset, drop_na_thresh, has_unique_idx,
+                 is_seperated):
         self.tb = tb
         self.user_def_pro = user_def_pro
         if user_def_pro is None:
             self.user_def_pro = []
 
         if db:
             self.db = USABLE_DBS[db]
@@ -188,33 +191,32 @@
     """
     数据处理原则：
         n2one: 数据源配置为is_data=True的对应日期查询结果只要存在一个全为空，则视当天的所有数据都为空，不更新数据表，也不更新操作记录表(updated_state)
         one2n:
                如果数据结果存在一个 None或者 emptyDataframe ，则当次调用 updated_state 表不更新
                如果数据结果全都有值，但是存在个别天数的行中存在空数据，则会删除空数据对应的行，updated_state更新取每个数据结果的交集作为日期
     """
+
     def __init__(self, sources, targets, executed_table):
         """
         数据库的操作器，负责从源表读取数据 _make_source_data，以及写入目标表 _handle_result
         """
         self.any_source_empty = False
         self.value = []
         self.sources = sources
         self.targets = targets
         self.source_data = []
         self.executed_table = executed_table
         self.to_update_date = self.__get_update_date()
         self.index_map = None
         self.customized_updated_state = None
 
-
     def __get_update_date(self):
         return DATA_UPDATED_STATE.loc[~(DATA_UPDATED_STATE[self.executed_table] == 1), 'update_date']
 
-
     def make_source_data(self):
         """
         产生数据源source_data的方法，按照TargetInfo顺序写入 source_data中
         判断传入的主要数据源（除了配置信息）是存在空，如果存在空则视所有数据源都为空，当天数据未更新
         :return:
         """
         for source in self.sources:
@@ -229,16 +231,14 @@
                 self.any_source_empty = True
                 for _ in self.targets:
                     self.value.append(None)
                 return
 
             self.source_data.append(data)
 
-
-
     def handle_result(self):
         """
         处理结果的方法
         1.有分表的处理：
             将value和target_info顺序展开 ，得到对应处理完的df，根据df的日期取出分表的suffix，
             再根据suffix选择需要插入的数据进行数据插入，同时删除对应日期的数据
         2.无分表的处理：
@@ -249,16 +249,15 @@
         :return:
         """
         update_state_date = None
         func_update_flag = True
         for index, target in enumerate(self.targets):
             cur_result = self.value[index]
 
-            #获取在funcs里传入的额外属性（target未定义的）
-            if len(target.user_def_pro)>0:
+            if len(target.user_def_pro) > 0:  # 获取在funcs里传入的额外属性（target未定义的）
                 for pro in target.user_def_pro:
                     exec(f"target.{pro} = self.{pro}")
             # target.index_map = self.index_map
 
             """
              处理返回值整个为none，如有一个返回结果为none，则整个方法的 这段to_update_date时间都应视为无数据，防止下文
              转str和合并索引时产生keyError
@@ -277,73 +276,79 @@
             # 处理经过dropna以后如果全为空的情况，视为全为空，原理同上
             if cur_result.empty:
                 func_update_flag = False
                 print(f'{target.tb} 无数据同步')
                 continue
 
             """统一把index_field字段转为str类型，防止后面在insert_update_state 和各表插入数据时 使用datetime64 或 int等类型"""
-                                                                           # datetime.date 在dataframe中有可能是Object类型
-            if str(cur_result[target.index_field].dtypes)=='datetime64' or str(cur_result[target.index_field].dtypes).lower() == 'object':
-                cur_result[target.index_field] = pd.to_datetime(cur_result[target.index_field]).apply(lambda x: x.strftime('%Y-%m-%d'))
+            # datetime.date 在dataframe中有可能是Object类型
+            if str(cur_result[target.index_field].dtypes) == 'datetime64' or str(
+                    cur_result[target.index_field].dtypes).lower() == 'object':
+                cur_result[target.index_field] = pd.to_datetime(cur_result[target.index_field]).apply(
+                    lambda x: x.strftime('%Y-%m-%d'))
             else:
                 # 碰到其他情况再继续完善，例如此处是inheritId，则把int或float转str
-                cur_result[target.index_field] = cur_result[target.index_field].astype(str).apply(lambda x:x.split('.')[0])
+                cur_result[target.index_field] = cur_result[target.index_field].astype(str).apply(
+                    lambda x: x.split('.')[0])
 
             # 调用统一接口完成成果产出
             target.build_output(cur_result)
 
             # 如果未传入自定义更新日期，则取数据日期作为 处理操作表的更新日期，取各数据结果交集
             if (update_state_date is not None) and (self.customized_updated_state is None):
                 update_state_date = update_state_date.merge(
-                    cur_result[[target.index_field]].drop_duplicates().apply(lambda x:self.index_map[x] if self.index_map is not None else x),
+                    cur_result[[target.index_field]].drop_duplicates().apply(
+                        lambda x: self.index_map[x] if self.index_map is not None else x),
                     left_on='update_date',
                     right_on=target.index_field,
                     how='inner'
                 )[['update_date']]
-            elif(update_state_date is None) and (self.customized_updated_state is None):
+            elif (update_state_date is None) and (self.customized_updated_state is None):
                 update_state_date = pd.DataFrame(
-                    cur_result[target.index_field].drop_duplicates().apply(lambda x:self.index_map[x] if self.index_map is not None else x).values,
+                    cur_result[target.index_field].drop_duplicates().apply(
+                        lambda x: self.index_map[x] if self.index_map is not None else x).values,
                     columns=['update_date']
                 )
 
         # 将方法的操作记录写入数据库
         if func_update_flag:
             if update_state_date is not None and not update_state_date.empty:
                 self.__handle_insert_update_state(update_state_date)
             # 如果update_state_date无值，则说明传了customized值，更新日期在二者中选其一有值的
             else:
                 if self.customized_updated_state is not None and not self.customized_updated_state.empty:
                     self.__handle_insert_update_state(self.customized_updated_state)
 
-
-
-
     def __handle_insert_update_state(self, update_state):
         """
         为update_state可能分表做准备
         :param update_state:
         :return:
         """
         update_state['table_name'] = self.executed_table
         with USABLE_DBS['targets_default'].begin() as conn:
-            conn.execute(f'delete from updated_state where table_name = "{self.executed_table}" and update_date in ({query_in_sql(update_state["update_date"].values.tolist())})')
+            conn.execute(
+                f'delete from updated_state where table_name = "{self.executed_table}" and update_date in ({query_in_sql(update_state["update_date"].values.tolist())})')
             update_state.to_sql('updated_state', con=conn, index=False, if_exists='append')
 
+
 """
 数据库装饰器 按数据流向类型区分，向数据库写入数据
 one2one:
 表示数据仅从一张表导入另一张表
 n2one:
 表示数据从多张表取汇聚成一张表
 one2n:
 数据从一张表导出分多张表导入
 n2n:
 _seperate: 采用了分表策略的表
 ...
 """
+
+
 def db_operator(sources: list, targets: list):
     """
     数据库操作器，包括源表与目标表，在funcs中需按照target_info顺序将结果添加到 executor.value中
     使用三个类来完成工作  1. Executor   方法层面，对应funcs模块中每个方法
                        2. Source 数据源层面，对应装饰器中定义的数据源
                        3. Target 目标表层面，对应装饰器中配置的目标表
     :param sources: 源表信息，list类型:
@@ -354,40 +359,43 @@
     :param targets:目标表信息，list类型:
     [
         Target(db=目标数据库，tb=目标表名,date_field=目标表日期字段名),
         Target(db=目标数据库，tb=目标表名,date_field=目标表日期字段名) ...
     ]
     :return:
     """
+
     def wrapper(func):
         @wraps(func)
         def inner_wrapper():
             executor = None
             try:
                 executor = Executor(targets=targets,
                                     sources=sources,
                                     executed_table=func.__name__)
 
                 # 表示该方法已同步完所有数据，则不再执行后续操作
                 if len(executor.to_update_date) == 0:
                     print(f'{func.__name__} 方法已同步至最新')
                     return
 
-                if len(sources)!=0:
+                if len(sources) != 0:
                     executor.make_source_data()
 
-                #empty_check为True且有一天数据源为空则不执行数据处理函数
+                # empty_check为True且有一天数据源为空则不执行数据处理函数
                 if not executor.any_source_empty:
                     func(executor)
 
                 executor.handle_result()
             except Exception:
                 global EXECUTE_STATE
                 EXECUTE_STATE = False
-                print(executor.executed_table+'同步失败')
+                print(executor.executed_table + '同步失败')
                 print(traceback.format_exc())
+
         return inner_wrapper
+
     return wrapper
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `ts-soup-0.0.5/ts_soup/workers/sources.py` & `ts-soup-0.0.6/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.5/ts_soup/workers/targets.py` & `ts-soup-0.0.6/ts_soup/workers/targets.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.5/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.0.6/ts_soup.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.5
+Version: 0.0.6
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

