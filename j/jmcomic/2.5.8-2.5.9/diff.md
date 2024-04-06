# Comparing `tmp/jmcomic-2.5.8.tar.gz` & `tmp/jmcomic-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.5.8.tar", last modified: Sat Mar 16 08:31:17 2024, max compression
+gzip compressed data, was "jmcomic-2.5.9.tar", last modified: Sat Apr  6 02:57:16 2024, max compression
```

## Comparing `jmcomic-2.5.8.tar` & `jmcomic-2.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:31:17.703765 jmcomic-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-16 08:31:13.000000 jmcomic-2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-16 08:31:17.703765 jmcomic-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-16 08:31:13.000000 jmcomic-2.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 08:31:17.703765 jmcomic-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-16 08:31:13.000000 jmcomic-2.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:31:17.699764 jmcomic-2.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:31:17.703765 jmcomic-2.5.8/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    37811 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17234 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18851 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    21980 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    31209 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    28649 2024-03-16 08:31:13.000000 jmcomic-2.5.8/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:31:17.703765 jmcomic-2.5.8/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-16 08:31:17.000000 jmcomic-2.5.8/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-16 08:31:17.000000 jmcomic-2.5.8/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:31:17.000000 jmcomic-2.5.8/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-16 08:31:17.000000 jmcomic-2.5.8/src/jmcomic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-16 08:31:17.000000 jmcomic-2.5.8/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-16 08:31:17.000000 jmcomic-2.5.8/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:57:16.883236 jmcomic-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 02:57:13.000000 jmcomic-2.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-06 02:57:16.883236 jmcomic-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-06 02:57:13.000000 jmcomic-2.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:57:16.883236 jmcomic-2.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-06 02:57:13.000000 jmcomic-2.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:57:16.879236 jmcomic-2.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:57:16.879236 jmcomic-2.5.9/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37811 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17234 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15249 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18974 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22395 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32262 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28649 2024-04-06 02:57:13.000000 jmcomic-2.5.9/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:57:16.883236 jmcomic-2.5.9/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-06 02:57:16.000000 jmcomic-2.5.9/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-06 02:57:16.000000 jmcomic-2.5.9/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:57:16.000000 jmcomic-2.5.9/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 02:57:16.000000 jmcomic-2.5.9/src/jmcomic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 02:57:16.000000 jmcomic-2.5.9/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 02:57:16.000000 jmcomic-2.5.9/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.5.8/LICENSE` & `jmcomic-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.5.8/PKG-INFO` & `jmcomic-2.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.5.8
+Version: 2.5.9
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: commonX>=0.6.4
 Requires-Dist: curl_cffi
+Requires-Dist: commonX
 Requires-Dist: PyYAML
 Requires-Dist: Pillow
 Requires-Dist: pycryptodome
 
 # Python API For JMComic (禁漫天堂)
 
 本项目封装了一套可用于爬取JM的Python API.
```

### Comparing `jmcomic-2.5.8/README.md` & `jmcomic-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.5.8/setup.py` & `jmcomic-2.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     url='https://github.com/hect0x7/JMComic-Crawler-Python',
     author='hect0x7',
     author_email='93357912+hect0x7@users.noreply.github.com',
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.7",
     install_requires=[
-        'commonX>=0.6.4',
         'curl_cffi',
+        'commonX',
         'PyYAML',
         'Pillow',
         'pycryptodome',
     ],
     keywords=['python', 'jmcomic', '18comic', '禁漫天堂', 'NSFW'],
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `jmcomic-2.5.8/src/jmcomic/__init__.py` & `jmcomic-2.5.9/src/jmcomic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 模块依赖关系如下:
 # 被依赖方 <--- 使用方
 # config <--- entity <--- toolkit <--- client <--- option <--- downloader
 
-__version__ = '2.5.8'
+__version__ = '2.5.9'
 
 from .api import *
 from .jm_plugin import *
 
 # 下面进行注册组件（客户端、插件）
 gb = dict(filter(lambda pair: isinstance(pair[1], type), globals().items()))
```

### Comparing `jmcomic-2.5.8/src/jmcomic/api.py` & `jmcomic-2.5.9/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.5.8/src/jmcomic/cl.py` & `jmcomic-2.5.9/src/jmcomic/cl.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_client_impl.py` & `jmcomic-2.5.9/src/jmcomic/jm_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         # 将参数字典编码为查询字符串
         query_string = urlencode(params)
         url = f"{url}?{query_string}"
         return url
 
     # noinspection PyMethodMayBeStatic
     def decode(self, url: str):
-        if not JmModuleConfig.flag_decode_url_when_logging or '/search/' not in url:
+        if not JmModuleConfig.FLAG_DECODE_URL_WHEN_LOGGING or '/search/' not in url:
             return url
 
         from urllib.parse import unquote
         return unquote(url.replace('+', ' '))
 
 
 # 基于网页实现的JmClient
@@ -763,15 +763,15 @@
         }
         """
         resp = self.req_api('/setting')
 
         # 检查禁漫最新的版本号
         setting_ver = str(resp.model_data.version)
         # 禁漫接口的版本 > jmcomic库内置版本
-        if setting_ver > JmMagicConstants.APP_VERSION and JmModuleConfig.flag_use_version_newer_if_behind:
+        if setting_ver > JmMagicConstants.APP_VERSION and JmModuleConfig.FLAG_USE_VERSION_NEWER_IF_BEHIND:
             jm_log('api.setting', f'change APP_VERSION from [{JmMagicConstants.APP_VERSION}] to [{setting_ver}]')
             JmMagicConstants.APP_VERSION = setting_ver
 
         return resp
 
     def login(self,
               username,
@@ -879,15 +879,15 @@
         if url == self.API_SCRAMBLE:
             # /chapter_view_template
             # 这个接口很特殊，用的密钥 18comicAPPContent 而不是 18comicAPP
             # 如果用后者，则会返回403信息
             ts = time_stamp()
             token, tokenparam = JmCryptoTool.token_and_tokenparam(ts, secret=JmMagicConstants.APP_TOKEN_SECRET_2)
 
-        elif JmModuleConfig.flag_use_fix_timestamp:
+        elif JmModuleConfig.FLAG_USE_FIX_TIMESTAMP:
             ts, token, tokenparam = JmModuleConfig.get_fix_ts_token_tokenparam()
 
         else:
             ts = time_stamp()
             token, tokenparam = JmCryptoTool.token_and_tokenparam(ts)
 
         # 设置headers
@@ -950,15 +950,15 @@
                 )
                 return resp
 
         ExceptionTool.raises_resp(f'响应无数据！request_url=[{url}]', resp)
 
     def after_init(self):
         # 保证拥有cookies，因为移动端要求必须携带cookies，否则会直接跳转同一本子【禁漫娘】
-        if JmModuleConfig.flag_api_client_require_cookies:
+        if JmModuleConfig.FLAG_API_CLIENT_REQUIRE_COOKIES:
             self.ensure_have_cookies()
 
     client_init_cookies_lock = Lock()
 
     def ensure_have_cookies(self):
         if self.get_meta_data('cookies'):
             return
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_client_interface.py` & `jmcomic-2.5.9/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_config.py` & `jmcomic-2.5.9/src/jmcomic/jm_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,33 +142,37 @@
     # 异常监听器
     # key: 异常类
     # value: 函数，参数只有异常对象，无需返回值
     # 这个异常类（或者这个异常的子类）的实例将要被raise前，你的listener方法会被调用
     REGISTRY_EXCEPTION_LISTENER = {}
 
     # 执行log的函数
-    executor_log = default_jm_logging
+    EXECUTOR_LOG = default_jm_logging
 
     # 使用固定时间戳
-    flag_use_fix_timestamp = True
+    FLAG_USE_FIX_TIMESTAMP = True
     # 移动端Client初始化cookies
-    flag_api_client_require_cookies = True
+    FLAG_API_CLIENT_REQUIRE_COOKIES = True
     # log开关标记
-    flag_enable_jm_log = True
+    FLAG_ENABLE_JM_LOG = True
     # log时解码url
-    flag_decode_url_when_logging = True
+    FLAG_DECODE_URL_WHEN_LOGGING = True
     # 当内置的版本号落后时，使用最新的禁漫app版本号
-    flag_use_version_newer_if_behind = True
+    FLAG_USE_VERSION_NEWER_IF_BEHIND = True
 
     # 关联dir_rule的自定义字段与对应的处理函数
     # 例如:
     # Amyname -> JmModuleConfig.AFIELD_ADVICE['myname'] = lambda album: "自定义名称"
     AFIELD_ADVICE = dict()
     PFIELD_ADVICE = dict()
 
+    # 当发生 oserror: [Errno 36] File name too long 时，
+    # 把文件名限制在指定个字符以内
+    VAR_FILE_NAME_LENGTH_LIMIT = 100
+
     @classmethod
     def downloader_class(cls):
         if cls.CLASS_DOWNLOADER is not None:
             return cls.CLASS_DOWNLOADER
 
         from .jm_downloader import JmDownloader
         return JmDownloader
@@ -315,20 +319,20 @@
         from .jm_toolkit import JmCryptoTool
         token, tokenparam = JmCryptoTool.token_and_tokenparam(ts)
         return ts, token, tokenparam
 
     # noinspection PyUnusedLocal
     @classmethod
     def jm_log(cls, topic: str, msg: str):
-        if cls.flag_enable_jm_log is True:
-            cls.executor_log(topic, msg)
+        if cls.FLAG_ENABLE_JM_LOG is True:
+            cls.EXECUTOR_LOG(topic, msg)
 
     @classmethod
     def disable_jm_log(cls):
-        cls.flag_enable_jm_log = False
+        cls.FLAG_ENABLE_JM_LOG = False
 
     @classmethod
     def new_postman(cls, session=False, **kwargs):
         kwargs.setdefault('impersonate', 'chrome110')
         kwargs.setdefault('headers', JmModuleConfig.new_html_headers())
         kwargs.setdefault('proxies', JmModuleConfig.DEFAULT_PROXIES)
 
@@ -343,15 +347,15 @@
     # 一般情况下，建议使用option配置文件来定制配置
     # 而如果只想修改几个简单常用的配置，也可以下方的DEFAULT_XXX属性
     JM_OPTION_VER = '2.1'
     DEFAULT_CLIENT_IMPL = 'api'  # 默认Client实现类型为网页端
     DEFAULT_CLIENT_CACHE = None  # 默认关闭Client缓存。缓存的配置详见 CacheRegistry
     DEFAULT_PROXIES = ProxyBuilder.system_proxy()  # 默认使用系统代理
 
-    default_option_dict: dict = {
+    DEFAULT_OPTION_DICT: dict = {
         'log': None,
         'dir_rule': {'rule': 'Bd_Pname', 'base_dir': None},
         'download': {
             'cache': True,
             'image': {'decode': True, 'suffix': None},
             'threading': {
                 'image': 30,
@@ -360,15 +364,15 @@
         },
         'client': {
             'cache': None,  # see CacheRegistry
             'domain': [],
             'postman': {
                 'type': 'cffi',
                 'meta_data': {
-                    'impersonate': 'chrome110',
+                    'impersonate': 'chrome',
                     'headers': None,
                     'proxies': None,
                 }
             },
             'impl': None,
             'retry_times': 5,
         },
@@ -383,19 +387,19 @@
     def option_default_dict(cls) -> dict:
         """
         返回JmOption.default()的默认配置字典。
         这样做是为了支持外界自行覆盖option默认配置字典
         """
         from copy import deepcopy
 
-        option_dict = deepcopy(cls.default_option_dict)
+        option_dict = deepcopy(cls.DEFAULT_OPTION_DICT)
 
         # log
         if option_dict['log'] is None:
-            option_dict['log'] = cls.flag_enable_jm_log
+            option_dict['log'] = cls.FLAG_ENABLE_JM_LOG
 
         # dir_rule.base_dir
         dir_rule = option_dict['dir_rule']
         if dir_rule['base_dir'] is None:
             import os
             dir_rule['base_dir'] = os.getcwd()
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_downloader.py` & `jmcomic-2.5.9/src/jmcomic/jm_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                )
 
     def after_photo(self, photo: JmPhotoDetail):
         jm_log('photo.after',
                f'章节下载完成: [{photo.id}] ({photo.album_id}[{photo.index}/{len(photo.from_album)}])')
 
     def before_image(self, image: JmImageDetail, img_save_path):
-        if image.is_exists:
+        if image.exists:
             jm_log('image.before',
                    f'图片已存在: {image.tag} ← [{img_save_path}]'
                    )
         else:
             jm_log('image.before',
                    f'图片准备下载: {image.tag}, [{image.img_url}] → [{img_save_path}]'
                    )
@@ -59,14 +59,16 @@
         client = self.client_for_album(album_id)
         album = client.get_album_detail(album_id)
         self.download_by_album_detail(album, client)
         return album
 
     def download_by_album_detail(self, album: JmAlbumDetail, client: JmcomicClient):
         self.before_album(album)
+        if album.skip:
+            return
         self.execute_by_condition(
             iter_objs=album,
             apply=lambda photo: self.download_by_photo_detail(photo, client),
             count_batch=self.option.decide_photo_batch_count(album)
         )
         self.after_album(album)
 
@@ -76,35 +78,40 @@
         self.download_by_photo_detail(photo, client)
         return photo
 
     def download_by_photo_detail(self, photo: JmPhotoDetail, client: JmcomicClient):
         client.check_photo(photo)
 
         self.before_photo(photo)
+        if photo.skip:
+            return
         self.execute_by_condition(
             iter_objs=photo,
             apply=lambda image: self.download_by_image_detail(image, client),
             count_batch=self.option.decide_image_batch_count(photo)
         )
         self.after_photo(photo)
 
     def download_by_image_detail(self, image: JmImageDetail, client: JmcomicClient):
         img_save_path = self.option.decide_image_filepath(image)
 
         image.save_path = img_save_path
-        image.is_exists = file_exists(img_save_path)
+        image.exists = file_exists(img_save_path)
 
         self.before_image(image, img_save_path)
 
+        if image.skip:
+            return
+
         # let option decide use_cache and decode_image
         use_cache = self.option.decide_download_cache(image)
         decode_image = self.option.decide_download_image_decode(image)
 
         # skip download
-        if use_cache is True and image.is_exists:
+        if use_cache is True and image.exists:
             return
 
         e = None
         try:
             client.download_by_image_detail(
                 image,
                 img_save_path,
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_entity.py` & `jmcomic-2.5.9/src/jmcomic/jm_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from common import *
 
 from .jm_config import *
 
 
+class Downloadable:
+
+    def __init__(self):
+        self.save_path: str = ''
+        self.exists: bool = False
+        self.skip = False
+
+
 class JmBaseEntity:
 
     def to_file(self, filepath):
         from common import PackerUtil
         PackerUtil.pack(self, filepath)
 
     @classmethod
@@ -113,15 +121,15 @@
         :return: '[id] oname'
         """
         return f'[{self.id}] {self.oname}'
 
     def __str__(self):
         return f'{self.__class__.__name__}' \
                '{' \
-               f'{self.id}: {self.title}'\
+               f'{self.id}: {self.title}' \
                '}'
 
     @classmethod
     def __alias__(cls):
         # "JmAlbumDetail" -> "album" (本子)
         # "JmPhotoDetail" -> "photo" (章节)
         cls_name = cls.__name__
@@ -152,44 +160,41 @@
 
         if advice_func is not None:
             return advice_func(detail)
 
         return getattr(detail, ref)
 
 
-class JmImageDetail(JmBaseEntity):
+class JmImageDetail(JmBaseEntity, Downloadable):
 
     def __init__(self,
                  aid,
                  scramble_id,
                  img_url,
                  img_file_name,
                  img_file_suffix,
                  from_photo=None,
                  query_params=None,
                  index=-1,
-                 ) -> None:
+                 ):
+        super().__init__()
         if scramble_id is None or (isinstance(scramble_id, str) and scramble_id == ''):
             from .jm_toolkit import ExceptionTool
             ExceptionTool.raises(f'图片的scramble_id不能为空')
 
         self.aid: str = str(aid)
         self.scramble_id: str = str(scramble_id)
         self.img_url: str = img_url
         self.img_file_name: str = img_file_name  # without suffix
         self.img_file_suffix: str = img_file_suffix
 
         self.from_photo: Optional[JmPhotoDetail] = from_photo
         self.query_params: Optional[str] = query_params
         self.index = index  # 从1开始
 
-        # temp fields, in order to simplify passing parameter
-        self.save_path: str = ''
-        self.is_exists: bool = False
-
     @property
     def filename_without_suffix(self):
         return self.img_file_name
 
     @property
     def filename(self):
         return self.img_file_name + self.img_file_suffix
@@ -248,29 +253,30 @@
         return f'{self.aid}/{self.img_file_name}{self.img_file_suffix} [{self.index}/{len(self.from_photo)}]'
 
     @classmethod
     def is_image(cls):
         return True
 
 
-class JmPhotoDetail(DetailEntity):
+class JmPhotoDetail(DetailEntity, Downloadable):
 
     def __init__(self,
                  photo_id,
                  name,
                  series_id,
                  sort,
                  tags='',
                  scramble_id='',
                  page_arr=None,
                  data_original_domain=None,
                  data_original_0=None,
                  author=None,
                  from_album=None,
                  ):
+        super().__init__()
         self.photo_id: str = str(photo_id)
         self.scramble_id: str = str(scramble_id)
         self.name: str = str(name).strip()
         self.sort: int = int(sort)
         self._tags: str = tags
         self._series_id: int = int(series_id)
 
@@ -407,15 +413,15 @@
         return super().__iter__()
 
     @classmethod
     def is_photo(cls):
         return True
 
 
-class JmAlbumDetail(DetailEntity):
+class JmAlbumDetail(DetailEntity, Downloadable):
 
     def __init__(self,
                  album_id,
                  scramble_id,
                  name,
                  episode_list,
                  page_count,
@@ -426,14 +432,15 @@
                  comment_count,
                  works,
                  actors,
                  authors,
                  tags,
                  related_list=None,
                  ):
+        super().__init__()
         self.album_id: str = str(album_id)
         self.scramble_id: str = str(scramble_id)
         self.name: str = name
         self.page_count: int = int(page_count)  # 总页数
         self.pub_date: str = pub_date  # 发布日期
         self.update_date: str = update_date  # 更新日期
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_exception.py` & `jmcomic-2.5.9/src/jmcomic/jm_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,14 @@
     """
 
     CONTEXT_KEY_RESP = 'resp'
     CONTEXT_KEY_HTML = 'html'
     CONTEXT_KEY_RE_PATTERN = 'pattern'
     CONTEXT_KEY_MISSING_JM_ID = 'missing_jm_id'
 
-    # 兼容旧版本
-
-    EXTRA_KEY_RESP = 'resp'
-    EXTRA_KEY_HTML = 'html'
-    EXTRA_KEY_RE_PATTERN = 'pattern'
-    EXTRA_KEY_MISSING_JM_ID = 'missing_jm_id'
-
     @classmethod
     def raises(cls,
                msg: str,
                context: dict = None,
                etype: Optional[Type[Exception]] = None,
                ):
         """
@@ -140,15 +133,16 @@
                       jmid: str,
                       ):
         """
         抛出本子/章节的异常
         :param resp: 响应对象
         :param jmid: 禁漫本子/章节id
         """
-        url = resp.url
+        from .jm_toolkit import JmcomicText
+        url = JmcomicText.format_album_url(jmid)
 
         req_type = "本子" if "album" in url else "章节"
         cls.raises(
             (
                 f'请求的{req_type}不存在！({url})\n'
                 '原因可能为:\n'
                 f'1. id有误，检查你的{req_type}id\n'
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_option.py` & `jmcomic-2.5.9/src/jmcomic/jm_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,23 @@
         # 使用 self.dir_rule 决定 save_dir
         save_dir = self.dir_rule.decide_image_save_dir(
             photo.from_album,
             photo
         )
 
         if ensure_exists:
-            mkdir_if_not_exists(save_dir)
+            try:
+                mkdir_if_not_exists(save_dir)
+            except OSError as e:
+                if e.errno == 36:
+                    # 目录名过长
+                    limit = JmModuleConfig.VAR_FILE_NAME_LENGTH_LIMIT
+                    jm_log('error', f'目录名过长，无法创建目录，强制缩短到{limit}个字符并重试')
+                    save_dir = save_dir[0:limit]
+                    mkdir_if_not_exists(save_dir)
 
         return save_dir
 
     def decide_image_filepath(self, image: JmImageDetail, consider_custom_suffix=True) -> str:
         # 以此决定保存文件夹、后缀、不包含后缀的文件名
         save_dir = self.decide_image_save_dir(image.from_photo)
         suffix = self.decide_image_suffix(image) if consider_custom_suffix else image.img_file_suffix
@@ -355,15 +363,15 @@
         # 2: 插件配置项 plugin -> plugins
         if 'plugin' in dic:
             dic['plugins'] = dic.pop('plugin')
 
     def deconstruct(self) -> Dict:
         return {
             'version': JmModuleConfig.JM_OPTION_VER,
-            'log': JmModuleConfig.flag_enable_jm_log,
+            'log': JmModuleConfig.FLAG_ENABLE_JM_LOG,
             'dir_rule': {
                 'rule': self.dir_rule.rule_dsl,
                 'base_dir': self.dir_rule.base_dir,
             },
             'download': self.download.src_dict,
             'client': self.client.src_dict,
             'plugins': self.plugins.src_dict
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_plugin.py` & `jmcomic-2.5.9/src/jmcomic/jm_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,17 +441,15 @@
 
         option_decide_cache = self.option.decide_download_cache
 
         def apply_filter_then_decide_cache(image: JmImageDetail):
             if image.img_file_suffix not in allowed_suffix_set:
                 self.log(f'跳过下载图片: {image.tag}，'
                          f'因为其后缀\'{image.img_file_suffix}\'不在允许的后缀集合{allowed_suffix_set}内')
-                # hook is_exists True to skip download
-                image.is_exists = True
-                return True
+                image.skip = True
 
             # let option decide
             return option_decide_cache(image)
 
         self.option.decide_download_cache = apply_filter_then_decide_cache
 
 
@@ -480,23 +478,23 @@
 class LogTopicFilterPlugin(JmOptionPlugin):
     plugin_key = 'log_topic_filter'
 
     def invoke(self, whitelist) -> None:
         if whitelist is not None:
             whitelist = set(whitelist)
 
-        old_jm_log = JmModuleConfig.executor_log
+        old_jm_log = JmModuleConfig.EXECUTOR_LOG
 
         def new_jm_log(topic, msg):
             if whitelist is not None and topic not in whitelist:
                 return
 
             old_jm_log(topic, msg)
 
-        JmModuleConfig.executor_log = new_jm_log
+        JmModuleConfig.EXECUTOR_LOG = new_jm_log
 
 
 class AutoSetBrowserCookiesPlugin(JmOptionPlugin):
     plugin_key = 'auto_set_browser_cookies'
 
     accepted_cookies_keys = str_to_set('''
     yuo1
@@ -959,7 +957,38 @@
             if is_new_photo:
                 photo_new_list.append(photo.photo_id)
 
             if int(photo.photo_id) == sentinel:
                 is_new_photo = True
 
         return len(photo_new_list) != 0, photo_new_list
+
+
+class SkipPhotoWithFewImagesPlugin(JmOptionPlugin):
+    plugin_key = 'skip_photo_with_few_images'
+
+    def invoke(self,
+               at_least_image_count: int,
+               photo: Optional[JmPhotoDetail] = None,
+               image: Optional[JmImageDetail] = None,
+               album: Optional[JmAlbumDetail] = None,
+               **kwargs
+               ):
+        self.try_mark_photo_skip_and_log(photo, at_least_image_count)
+        if image is not None:
+            self.try_mark_photo_skip_and_log(image.from_photo, at_least_image_count)
+
+    def try_mark_photo_skip_and_log(self, photo: JmPhotoDetail, at_least_image_count: int):
+        if photo is None:
+            return
+
+        if len(photo) >= at_least_image_count:
+            return
+
+        self.log(f'跳过下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}])，'
+                 f'因为其图片数: {len(photo)} < {at_least_image_count} (at_least_image_count)')
+        photo.skip = True
+
+    @classmethod
+    @field_cache()  # 单例
+    def build(cls, option: JmOption) -> 'JmOptionPlugin':
+        return super().build(option)
```

### Comparing `jmcomic-2.5.8/src/jmcomic/jm_toolkit.py` & `jmcomic-2.5.9/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.5.8/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.5.9/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.5.8
+Version: 2.5.9
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: commonX>=0.6.4
 Requires-Dist: curl_cffi
+Requires-Dist: commonX
 Requires-Dist: PyYAML
 Requires-Dist: Pillow
 Requires-Dist: pycryptodome
 
 # Python API For JMComic (禁漫天堂)
 
 本项目封装了一套可用于爬取JM的Python API.
```

### Comparing `jmcomic-2.5.8/src/jmcomic.egg-info/SOURCES.txt` & `jmcomic-2.5.9/src/jmcomic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

