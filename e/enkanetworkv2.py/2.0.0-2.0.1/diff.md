# Comparing `tmp/enkanetworkV2.py-2.0.0.tar.gz` & `tmp/enkanetworkv2.py-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkanetworkv2.py-2.0.0.tar", last modified: Sat Feb 24 20:14:22 2024, max compression
+gzip compressed data, was "enkanetworkv2.py-2.0.1.tar", last modified: Sat Apr  6 17:23:26 2024, max compression
```

## Comparing `enkanetworkV2.py-2.0.0.tar` & `enkanetworkv2.py-2.0.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.757789 enkanetworkv2.py-2.0.0/
--rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.0/LICENSE
--rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    19341 2024-02-24 20:14:22.756284 enkanetworkv2.py-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.664851 enkanetworkv2.py-2.0.0/enkanetwork/
--rw-rw-rw-   0        0        0     1462 2024-02-24 18:52:06.000000 enkanetworkv2.py-2.0.0/enkanetwork/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.645823 enkanetworkv2.py-2.0.0/enkanetwork/assets/
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.709546 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/
--rw-rw-rw-   0        0        0    54227 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/artifact_props.json
--rw-rw-rw-   0        0        0  1078670 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/artifacts.json
--rw-rw-rw-   0        0        0    42696 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/characters.json
--rw-rw-rw-   0        0        0    51265 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/constellations.json
--rw-rw-rw-   0        0        0    12595 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/costumes.json
--rw-rw-rw-   0        0        0  1272766 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/fight_props.json
--rw-rw-rw-   0        0        0    55299 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/namecards.json
--rw-rw-rw-   0        0        0    84072 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/skills.json
--rw-rw-rw-   0        0        0    41143 2024-02-24 19:47:40.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.727581 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/
--rw-rw-rw-   0        0        0   542378 2024-02-24 19:50:20.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/artifact_sets.json
--rw-rw-rw-   0        0        0  2391495 2024-02-24 19:50:21.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/artifacts.json
--rw-rw-rw-   0        0        0    32493 2024-02-24 19:50:21.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/characters.json
--rw-rw-rw-   0        0        0   301057 2024-02-24 19:50:21.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/constellations.json
--rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/fight_props.json
--rw-rw-rw-   0        0        0   117871 2024-02-24 19:50:21.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/namecards.json
--rw-rw-rw-   0        0        0   297913 2024-02-24 19:50:21.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/skills.json
--rw-rw-rw-   0        0        0   111407 2024-02-24 19:50:21.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/weapons.json
--rw-rw-rw-   0        0        0     7582 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/assets.py
--rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/cache.py
--rw-rw-rw-   0        0        0    12435 2024-02-24 19:47:30.000000 enkanetworkv2.py-2.0.0/enkanetwork/client.py
--rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/config.py
--rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/enum.py
--rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/exception.py
--rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.0/enkanetwork/http.py
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.741765 enkanetworkv2.py-2.0.0/enkanetwork/model/
--rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/__init__.py
--rw-rw-rw-   0        0        0     4683 2024-02-24 18:46:33.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/assets.py
--rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/base.py
--rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/build.py
--rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/character.py
--rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/equipments.py
--rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/hoyos.py
--rw-rw-rw-   0        0        0     3855 2024-02-24 18:48:31.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/players.py
--rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/profile.py
--rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/stats.py
--rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/model/utils.py
--rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.743764 enkanetworkv2.py-2.0.0/enkanetwork/types/
--rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.0/enkanetwork/types/__init__.py
--rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.0/enkanetwork/types/enkanetwork.py
--rw-rw-rw-   0        0        0     2994 2024-02-24 18:56:15.000000 enkanetworkv2.py-2.0.0/enkanetwork/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-24 20:14:22.755284 enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/
--rw-rw-rw-   0        0        0    19341 2024-02-24 20:14:22.000000 enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1715 2024-02-24 20:14:22.000000 enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 20:14:22.000000 enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-02-24 20:14:22.000000 enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-24 20:14:22.000000 enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-24 20:14:22.758797 enkanetworkv2.py-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1105 2024-02-24 20:14:18.000000 enkanetworkv2.py-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.354288 enkanetworkv2.py-2.0.1/
+-rw-rw-rw-   0        0        0     1070 2024-02-24 18:53:52.000000 enkanetworkv2.py-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-02-24 18:58:13.000000 enkanetworkv2.py-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    19341 2024-04-06 17:23:26.351774 enkanetworkv2.py-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18242 2024-02-24 19:02:02.000000 enkanetworkv2.py-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.258345 enkanetworkv2.py-2.0.1/enkanetwork/
+-rw-rw-rw-   0        0        0     1462 2024-04-06 17:20:51.000000 enkanetworkv2.py-2.0.1/enkanetwork/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.234274 enkanetworkv2.py-2.0.1/enkanetwork/assets/
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.278434 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/
+-rw-rw-rw-   0        0        0    54227 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/artifact_props.json
+-rw-rw-rw-   0        0        0  1078669 2024-04-06 16:12:05.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/artifacts.json
+-rw-rw-rw-   0        0        0    43169 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/characters.json
+-rw-rw-rw-   0        0        0    51875 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/constellations.json
+-rw-rw-rw-   0        0        0    12713 2024-04-06 16:12:05.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/costumes.json
+-rw-rw-rw-   0        0        0  1313515 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/fight_props.json
+-rw-rw-rw-   0        0        0    55882 2024-04-06 16:12:04.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/namecards.json
+-rw-rw-rw-   0        0        0     6321 2024-04-06 16:43:28.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/pfps.json
+-rw-rw-rw-   0        0        0    85057 2024-04-06 16:12:07.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/skills.json
+-rw-rw-rw-   0        0        0    41531 2024-04-06 16:12:04.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.300180 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/
+-rw-rw-rw-   0        0        0   549230 2024-04-06 16:14:44.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/artifact_sets.json
+-rw-rw-rw-   0        0        0  2391484 2024-04-06 16:14:46.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/artifacts.json
+-rw-rw-rw-   0        0        0    32879 2024-04-06 16:14:46.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/characters.json
+-rw-rw-rw-   0        0        0   304646 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/constellations.json
+-rw-rw-rw-   0        0        0    30562 2024-02-24 19:12:22.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/fight_props.json
+-rw-rw-rw-   0        0        0   119245 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/namecards.json
+-rw-rw-rw-   0        0        0   301093 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/skills.json
+-rw-rw-rw-   0        0        0   112669 2024-04-06 16:14:47.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/weapons.json
+-rw-rw-rw-   0        0        0     8270 2024-04-06 17:04:36.000000 enkanetworkv2.py-2.0.1/enkanetwork/assets.py
+-rw-rw-rw-   0        0        0      645 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/cache.py
+-rw-rw-rw-   0        0        0    12476 2024-04-06 17:07:29.000000 enkanetworkv2.py-2.0.1/enkanetwork/client.py
+-rw-rw-rw-   0        0        0      798 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/config.py
+-rw-rw-rw-   0        0        0     1099 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/enum.py
+-rw-rw-rw-   0        0        0     1925 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/exception.py
+-rw-rw-rw-   0        0        0     7345 2024-02-24 18:56:30.000000 enkanetworkv2.py-2.0.1/enkanetwork/http.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.320675 enkanetworkv2.py-2.0.1/enkanetwork/model/
+-rw-rw-rw-   0        0        0      137 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/__init__.py
+-rw-rw-rw-   0        0        0     5029 2024-04-06 17:00:40.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/assets.py
+-rw-rw-rw-   0        0        0     1935 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/base.py
+-rw-rw-rw-   0        0        0     1403 2024-02-24 18:46:53.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/build.py
+-rw-rw-rw-   0        0        0     5183 2024-02-24 18:47:25.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/character.py
+-rw-rw-rw-   0        0        0     5634 2024-02-24 18:35:48.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/equipments.py
+-rw-rw-rw-   0        0        0      307 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/hoyos.py
+-rw-rw-rw-   0        0        0     4063 2024-04-06 17:07:07.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/players.py
+-rw-rw-rw-   0        0        0      346 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/profile.py
+-rw-rw-rw-   0        0        0     7763 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/stats.py
+-rw-rw-rw-   0        0        0      293 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/model/utils.py
+-rw-rw-rw-   0        0        0     1313 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.321673 enkanetworkv2.py-2.0.1/enkanetwork/types/
+-rw-rw-rw-   0        0        0      157 2024-02-24 18:56:57.000000 enkanetworkv2.py-2.0.1/enkanetwork/types/__init__.py
+-rw-rw-rw-   0        0        0     1157 2023-09-27 04:13:10.000000 enkanetworkv2.py-2.0.1/enkanetwork/types/enkanetwork.py
+-rw-rw-rw-   0        0        0     3404 2024-04-06 16:43:35.000000 enkanetworkv2.py-2.0.1/enkanetwork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:23:26.350774 enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/
+-rw-rw-rw-   0        0        0    19341 2024-04-06 17:23:26.000000 enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1550 2024-04-06 17:23:26.000000 enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 17:23:26.000000 enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-06 17:23:26.000000 enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 17:23:26.000000 enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 17:23:26.355288 enkanetworkv2.py-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2024-04-06 17:09:00.000000 enkanetworkv2.py-2.0.1/setup.py
```

### Comparing `enkanetworkv2.py-2.0.0/LICENSE` & `enkanetworkv2.py-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/PKG-INFO` & `enkanetworkv2.py-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.0
+Version: 2.0.1
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.0/README.md` & `enkanetworkv2.py-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/__init__.py` & `enkanetworkv2.py-2.0.1/enkanetwork/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE."""
 
 __title__ = 'enkanetworkV2.py'
 __author__ = 'DeviantUa'
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 
 from .client import *
 from .exception import *
 from .model import *
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/artifact_props.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/artifact_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/artifacts.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/artifacts.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999182531608778%*

 * *Differences: {"'23699'": "{'equipType': 'EQUIP_SHOES', 'icon': 'UI_RelicIcon_15032_5', 'rankLevel': 5, "*

 * *            "'mainPropDepotId': 1097, 'appendPropDepotId': 963}",*

 * * "'23708'": "{'rankLevel': 5, 'mainPropDepotId': 3099}",*

 * * "'23710'": "{'rankLevel': 5, 'mainPropDepotId': 1098}"}*

```diff
@@ -3866,21 +3866,21 @@
         "icon": "UI_RelicIcon_15032_3",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 3096,
         "nameTextMapHash": 282101028,
         "rankLevel": 4
     },
     "23699": {
-        "appendPropDepotId": 962,
-        "equipType": "EQUIP_BRACER",
-        "icon": "UI_RelicIcon_15032_4",
+        "appendPropDepotId": 963,
+        "equipType": "EQUIP_SHOES",
+        "icon": "UI_RelicIcon_15032_5",
         "itemType": "ITEM_RELIQUARY",
-        "mainPropDepotId": 4000,
+        "mainPropDepotId": 1097,
         "nameTextMapHash": 1942586956,
-        "rankLevel": 4
+        "rankLevel": 5
     },
     "23700": {
         "appendPropDepotId": 963,
         "equipType": "EQUIP_SHOES",
         "icon": "UI_RelicIcon_15032_5",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 1099,
@@ -3951,17 +3951,17 @@
         "rankLevel": 4
     },
     "23708": {
         "appendPropDepotId": 965,
         "equipType": "EQUIP_DRESS",
         "icon": "UI_RelicIcon_15033_3",
         "itemType": "ITEM_RELIQUARY",
-        "mainPropDepotId": 3094,
+        "mainPropDepotId": 3099,
         "nameTextMapHash": 1058555516,
-        "rankLevel": 4
+        "rankLevel": 5
     },
     "23709": {
         "appendPropDepotId": 962,
         "equipType": "EQUIP_BRACER",
         "icon": "UI_RelicIcon_15033_4",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 4000,
@@ -3969,17 +3969,17 @@
         "rankLevel": 4
     },
     "23710": {
         "appendPropDepotId": 963,
         "equipType": "EQUIP_SHOES",
         "icon": "UI_RelicIcon_15033_5",
         "itemType": "ITEM_RELIQUARY",
-        "mainPropDepotId": 1096,
+        "mainPropDepotId": 1098,
         "nameTextMapHash": 3809984692,
-        "rankLevel": 4
+        "rankLevel": 5
     },
     "23711": {
         "appendPropDepotId": 964,
         "equipType": "EQUIP_RING",
         "icon": "UI_RelicIcon_15034_1",
         "itemType": "ITEM_RELIQUARY",
         "mainPropDepotId": 5091,
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/characters.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/characters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989010989010989%*

 * *Differences: {"'10000094'": "OrderedDict([('nameTextMapHash', 1944606922), ('iconName', "*

 * *               "'UI_AvatarIcon_Chiori'), ('sideIconName', 'UI_AvatarIcon_Side_Chiori'), "*

 * *               "('qualityType', 'QUALITY_ORANGE'), ('costElemType', 'Rock'), ('skills', [10941, "*

 * *               "10942, 10945]), ('talents', [941, 942, 943, 944, 945, 946])])"}*

```diff
@@ -1794,9 +1794,29 @@
             931,
             932,
             933,
             934,
             935,
             936
         ]
+    },
+    "10000094": {
+        "costElemType": "Rock",
+        "iconName": "UI_AvatarIcon_Chiori",
+        "nameTextMapHash": 1944606922,
+        "qualityType": "QUALITY_ORANGE",
+        "sideIconName": "UI_AvatarIcon_Side_Chiori",
+        "skills": [
+            10941,
+            10942,
+            10945
+        ],
+        "talents": [
+            941,
+            942,
+            943,
+            944,
+            945,
+            946
+        ]
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/constellations.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/constellations.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'941'": "OrderedDict([('nameTextMapHash', 689897337), ('icon', 'UI_Talent_S_Chiori_01')])",*

 * * "'942'": "OrderedDict([('nameTextMapHash', 2112971153), ('icon', 'UI_Talent_S_Chiori_03')])",*

 * * "'943'": "OrderedDict([('nameTextMapHash', 645847961), ('icon', 'UI_Talent_U_Chiori_01')])",*

 * * "'944'": "OrderedDict([('nameTextMapHash', 6373505), ('icon', 'UI_Talent_S_Chiori_02')])",*

 * * "'945'": "OrderedDict([('nameTextMapHash', 167855529), ('icon', 'UI_Talent_U_Chiori_02')])",*

 * * "'946'": "OrderedDict([('nameTextMapHash', […]*

```diff
@@ -1979,14 +1979,38 @@
         "icon": "UI_Talent_S_Liuyun_04",
         "nameTextMapHash": 3383313401
     },
     "94": {
         "icon": "UI_Talent_S_PlayerRock_03",
         "nameTextMapHash": 161259209
     },
+    "941": {
+        "icon": "UI_Talent_S_Chiori_01",
+        "nameTextMapHash": 689897337
+    },
+    "942": {
+        "icon": "UI_Talent_S_Chiori_03",
+        "nameTextMapHash": 2112971153
+    },
+    "943": {
+        "icon": "UI_Talent_U_Chiori_01",
+        "nameTextMapHash": 645847961
+    },
+    "944": {
+        "icon": "UI_Talent_S_Chiori_02",
+        "nameTextMapHash": 6373505
+    },
+    "945": {
+        "icon": "UI_Talent_U_Chiori_02",
+        "nameTextMapHash": 167855529
+    },
+    "946": {
+        "icon": "UI_Talent_S_Chiori_04",
+        "nameTextMapHash": 94228129
+    },
     "95": {
         "icon": "UI_Talent_U_PlayerRock_01",
         "nameTextMapHash": 4177873769
     },
     "96": {
         "icon": "UI_Talent_S_PlayerRock_04",
         "nameTextMapHash": 4065853553
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/costumes.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/costumes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897959183673469%*

 * *Differences: {"'209400'": "OrderedDict([('iconName', ''), ('sideIconName', ''), ('nameTextMapHash', "*

 * *             '4268512138)])'}*

```diff
@@ -479,9 +479,14 @@
         "nameTextMapHash": 2007918858,
         "sideIconName": ""
     },
     "209300": {
         "iconName": "",
         "nameTextMapHash": 2283589170,
         "sideIconName": ""
+    },
+    "209400": {
+        "iconName": "",
+        "nameTextMapHash": 4268512138,
+        "sideIconName": ""
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/fight_props.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/fight_props.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411726637328501%*

 * *Differences: {"'LEVEL_BUTTON_CATCH_A_BUTTERFLY'": "OrderedDict([('nameTextMapHash', 3245009171)])",*

 * * "'NPC_EXPNAME_13932'": "OrderedDict([('nameTextMapHash', 907510180)])",*

 * * "'NPC_EXPNAME_13934'": "OrderedDict([('nameTextMapHash', 3455866188)])",*

 * * "'NPC_EXPNAME_13934_1'": "OrderedDict([('nameTextMapHash', 1732518161)])",*

 * * "'NPC_EXPNAME_13937'": "OrderedDict([('nameTextMapHash', 3377043356)])",*

 * * "'NPC_EXPNAME_13977'": "OrderedDict([('nameTextMapHash', 3000669924)])",*

 * * "'NPC_EXPNAME_13978'": "OrderedDict([('nameTextMapHas […]*

```diff
@@ -3910,14 +3910,17 @@
     },
     "LEVEL_Airship_refresh": {
         "nameTextMapHash": 2789321311
     },
     "LEVEL_BUTTON_CATCH": {
         "nameTextMapHash": 1925976587
     },
+    "LEVEL_BUTTON_CATCH_A_BUTTERFLY": {
+        "nameTextMapHash": 3245009171
+    },
     "LEVEL_BWBS_BoilLake": {
         "nameTextMapHash": 671115786
     },
     "LEVEL_BWBS_FontaineTopHill": {
         "nameTextMapHash": 184497330
     },
     "LEVEL_CYG_DAOBAODONG": {
@@ -4216,14 +4219,41 @@
     },
     "NPC_EXPNAME_13853": {
         "nameTextMapHash": 378388164
     },
     "NPC_EXPNAME_13854": {
         "nameTextMapHash": 2891725268
     },
+    "NPC_EXPNAME_13932": {
+        "nameTextMapHash": 907510180
+    },
+    "NPC_EXPNAME_13934": {
+        "nameTextMapHash": 3455866188
+    },
+    "NPC_EXPNAME_13934_1": {
+        "nameTextMapHash": 1732518161
+    },
+    "NPC_EXPNAME_13937": {
+        "nameTextMapHash": 3377043356
+    },
+    "NPC_EXPNAME_13977": {
+        "nameTextMapHash": 3000669924
+    },
+    "NPC_EXPNAME_13978": {
+        "nameTextMapHash": 3550423132
+    },
+    "NPC_EXPNAME_13979": {
+        "nameTextMapHash": 688835756
+    },
+    "NPC_EXPNAME_13980": {
+        "nameTextMapHash": 274769660
+    },
+    "NPC_EXPNAME_14016": {
+        "nameTextMapHash": 2151515700
+    },
     "NPC_EXPNAME_1702": {
         "nameTextMapHash": 989589180
     },
     "NPC_EXPNAME_1702_1": {
         "nameTextMapHash": 1903169727
     },
     "NPC_EXPNAME_20577": {
@@ -4582,14 +4612,20 @@
     },
     "NPC_EXPNAME_30416_1": {
         "nameTextMapHash": 3267872694
     },
     "NPC_EXPNAME_30419": {
         "nameTextMapHash": 2665002652
     },
+    "NPC_EXPNAME_30509": {
+        "nameTextMapHash": 138696796
+    },
+    "NPC_EXPNAME_30534": {
+        "nameTextMapHash": 1104502828
+    },
     "NPC_EXPNAME_4218": {
         "nameTextMapHash": 3574170172
     },
     "NPC_EXPNAME_4218_1": {
         "nameTextMapHash": 2828479470
     },
     "NPC_EXPNAME_4247": {
@@ -5404,14 +5440,44 @@
     },
     "NPC_TITLE_13857": {
         "nameTextMapHash": 4261199529
     },
     "NPC_TITLE_13890": {
         "nameTextMapHash": 3699973225
     },
+    "NPC_TITLE_13932": {
+        "nameTextMapHash": 1400631209
+    },
+    "NPC_TITLE_13933": {
+        "nameTextMapHash": 781766857
+    },
+    "NPC_TITLE_13935": {
+        "nameTextMapHash": 2290919105
+    },
+    "NPC_TITLE_13937": {
+        "nameTextMapHash": 4069868089
+    },
+    "NPC_TITLE_13976": {
+        "nameTextMapHash": 1894183049
+    },
+    "NPC_TITLE_13979": {
+        "nameTextMapHash": 3069275265
+    },
+    "NPC_TITLE_13980": {
+        "nameTextMapHash": 3452341617
+    },
+    "NPC_TITLE_13981": {
+        "nameTextMapHash": 4033678769
+    },
+    "NPC_TITLE_14016": {
+        "nameTextMapHash": 3615369441
+    },
+    "NPC_TITLE_14028": {
+        "nameTextMapHash": 569623201
+    },
     "NPC_TITLE_1405_TEST": {
         "nameTextMapHash": 1431829271
     },
     "NPC_TITLE_1409": {
         "nameTextMapHash": 1519934793
     },
     "NPC_TITLE_140901": {
@@ -6382,14 +6448,17 @@
     },
     "NPC_TITLE_2150": {
         "nameTextMapHash": 881677417
     },
     "NPC_TITLE_2151": {
         "nameTextMapHash": 452702409
     },
+    "NPC_TITLE_21517": {
+        "nameTextMapHash": 1981622281
+    },
     "NPC_TITLE_2152": {
         "nameTextMapHash": 2758728185
     },
     "NPC_TITLE_2153": {
         "nameTextMapHash": 2448635657
     },
     "NPC_TITLE_2154": {
@@ -7108,17 +7177,35 @@
     },
     "NPC_TITLE_30490": {
         "nameTextMapHash": 5338025
     },
     "NPC_TITLE_30491": {
         "nameTextMapHash": 2013150089
     },
+    "NPC_TITLE_30501": {
+        "nameTextMapHash": 2219846033
+    },
+    "NPC_TITLE_30509": {
+        "nameTextMapHash": 643950281
+    },
+    "NPC_TITLE_30518": {
+        "nameTextMapHash": 3207833201
+    },
+    "NPC_TITLE_30519": {
+        "nameTextMapHash": 1423239953
+    },
     "NPC_TITLE_3053": {
         "nameTextMapHash": 737661113
     },
+    "NPC_TITLE_30534": {
+        "nameTextMapHash": 2093933961
+    },
+    "NPC_TITLE_30539": {
+        "nameTextMapHash": 611722297
+    },
     "NPC_TITLE_3054": {
         "nameTextMapHash": 3390889657
     },
     "NPC_TITLE_3056": {
         "nameTextMapHash": 3790168681
     },
     "NPC_TITLE_3057": {
@@ -8875,14 +8962,20 @@
     },
     "PERSONAL_LINE_AYAKA": {
         "nameTextMapHash": 2778483999
     },
     "PERSONAL_LINE_AYAKA_LINE_START": {
         "nameTextMapHash": 1264643668
     },
+    "PERSONAL_LINE_CHIORI": {
+        "nameTextMapHash": 728395351
+    },
+    "PERSONAL_LINE_CHIORI_LINE_START": {
+        "nameTextMapHash": 52878078
+    },
     "PERSONAL_LINE_COMPLAINMENT": {
         "nameTextMapHash": 1029528935
     },
     "PERSONAL_LINE_COMPLAINMENT_TITLE": {
         "nameTextMapHash": 1904417612
     },
     "PERSONAL_LINE_EMPTY": {
@@ -8932,20 +9025,14 @@
     },
     "PERSONAL_LINE_KOKOMI_LINE_START": {
         "nameTextMapHash": 2885738697
     },
     "PERSONAL_LINE_LEVEL_LIMIT": {
         "nameTextMapHash": 4214780121
     },
-    "PERSONAL_LINE_LIUYUN": {
-        "nameTextMapHash": 1689507327
-    },
-    "PERSONAL_LINE_LIUYUN_LINE_START": {
-        "nameTextMapHash": 1500543096
-    },
     "PERSONAL_LINE_MISSION_BROWSE": {
         "nameTextMapHash": 584980306
     },
     "PERSONAL_LINE_MISSION_CHECK": {
         "nameTextMapHash": 770836202
     },
     "PERSONAL_LINE_MONA": {
@@ -12208,14 +12295,20 @@
     },
     "RetActivityContentClosed": {
         "nameTextMapHash": 3572402933
     },
     "RetActivityFriendHaveGiftLimit": {
         "nameTextMapHash": 168194605
     },
+    "RetAlchemySimCropExceedLimit": {
+        "nameTextMapHash": 589832955
+    },
+    "RetAlchemySimInvalidRoundState": {
+        "nameTextMapHash": 3547912525
+    },
     "RetAllBonfireExceedMaxCount": {
         "nameTextMapHash": 1107085557
     },
     "RetAllTargetSatiationFull": {
         "nameTextMapHash": 3142810869
     },
     "RetAlreadyHaveSignedIn": {
@@ -12763,14 +12856,17 @@
     },
     "RetGachaRandomNotMatch": {
         "nameTextMapHash": 2623679981
     },
     "RetGachaScheduleNotMatch": {
         "nameTextMapHash": 736453549
     },
+    "RetGachaWishNeedBeforeGacha": {
+        "nameTextMapHash": 3506602597
+    },
     "RetGadgetBuilderExceedMaxCount": {
         "nameTextMapHash": 268076317
     },
     "RetGadgetCreateFail": {
         "nameTextMapHash": 1632383053
     },
     "RetGadgetFoundationBildingPointNotEnought": {
@@ -14281,14 +14377,17 @@
     },
     "SHOP_SOLD_OUT": {
         "nameTextMapHash": 3493184645
     },
     "SHOP_SOLD_OUT2": {
         "nameTextMapHash": 2412825149
     },
+    "SHOP_TYPE_ACTIVITY": {
+        "nameTextMapHash": 2394375340
+    },
     "SHOP_TYPE_ACTIVITY_ASTER": {
         "nameTextMapHash": 1591933735
     },
     "SHOP_TYPE_ACTIVITY_BLITZ_RUSH": {
         "nameTextMapHash": 1756478775
     },
     "SHOP_TYPE_ACTIVITY_BRICK_BREAKER": {
@@ -14446,14 +14545,17 @@
     },
     "SHOP_TYPE_NPC_MasterLu": {
         "nameTextMapHash": 3370200772
     },
     "SHOP_TYPE_NPC_Mequignon": {
         "nameTextMapHash": 3527572012
     },
+    "SHOP_TYPE_NPC_SHOP": {
+        "nameTextMapHash": 646250532
+    },
     "SHOP_TYPE_NPC_Sanguinetti": {
         "nameTextMapHash": 3339140428
     },
     "SHOP_TYPE_NPC_Yueshu": {
         "nameTextMapHash": 3717248972
     },
     "SHOP_TYPE_NPC_Zhenyuan": {
@@ -15097,14 +15199,1163 @@
     },
     "UI_ACTIVITY_ADVERTISEMENT_GO_TO_MISSON_BUTTON": {
         "nameTextMapHash": 3231116544
     },
     "UI_ACTIVITY_ADVERTISEMENT_INVESTIGATE_BUTTON": {
         "nameTextMapHash": 3510170761
     },
+    "UI_ACTIVITY_ALCHEMYSIM_ALCHEMY": {
+        "nameTextMapHash": 3134607896
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ALCHEMY_NO_LIMIT": {
+        "nameTextMapHash": 3819496261
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG": {
+        "nameTextMapHash": 2439381488
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG_CROP_INFO": {
+        "nameTextMapHash": 349790828
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG_FILTER": {
+        "nameTextMapHash": 3791057152
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG_FILTER_ALL": {
+        "nameTextMapHash": 3377620651
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG_NO_ITEM": {
+        "nameTextMapHash": 1205441471
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG_POTION_INFO": {
+        "nameTextMapHash": 1943522205
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_BAG_UPGRADE_INFO": {
+        "nameTextMapHash": 1629456710
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CANCEL_UPGRADE": {
+        "nameTextMapHash": 4278013127
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CASH": {
+        "nameTextMapHash": 901035128
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CHAIR": {
+        "nameTextMapHash": 3220802392
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CHOOSE_GOODS": {
+        "nameTextMapHash": 872541786
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_COINS_NOT_ENOUGH": {
+        "nameTextMapHash": 2761980655
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CONFIRM_ADDED": {
+        "nameTextMapHash": 2652615786
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CONFIRM_UPGRADE": {
+        "nameTextMapHash": 1135465914
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_COST_NUMBER": {
+        "nameTextMapHash": 4206718581
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CRITICAL": {
+        "nameTextMapHash": 928722448
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP": {
+        "nameTextMapHash": 2267501104
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROPS_HARVEST_TIPS": {
+        "nameTextMapHash": 2167873314
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_ALL": {
+        "nameTextMapHash": 115337413
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_ALL_HINT": {
+        "nameTextMapHash": 3062264217
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_COIN_LACK": {
+        "nameTextMapHash": 1431897193
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_ACCELERATE_DENY": {
+        "nameTextMapHash": 1410785765
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_ADD_PS": {
+        "nameTextMapHash": 2016246831
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CANCEL_PS": {
+        "nameTextMapHash": 3199297745
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_BUTTON": {
+        "nameTextMapHash": 2417739209
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_CONFIRM_BUTTON": {
+        "nameTextMapHash": 2583420090
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_DENY_SAME": {
+        "nameTextMapHash": 3074326636
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_HINT": {
+        "nameTextMapHash": 1076426513
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CHANGE_TITLE": {
+        "nameTextMapHash": 1903088489
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_CLICK_HINT": {
+        "nameTextMapHash": 3941414025
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_ACCELERATE_ONCE": {
+        "nameTextMapHash": 61418156
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_GET_ONCE": {
+        "nameTextMapHash": 577590355
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_MATURE": {
+        "nameTextMapHash": 3215242155
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_NUM": {
+        "nameTextMapHash": 1144536627
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_PRODUCTION": {
+        "nameTextMapHash": 3200514923
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_INFO_TIME": {
+        "nameTextMapHash": 3092004531
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_PS": {
+        "nameTextMapHash": 2604867826
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_DETAIL_TITLE": {
+        "nameTextMapHash": 720302490
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_ALL": {
+        "nameTextMapHash": 1737218676
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_DENY": {
+        "nameTextMapHash": 2617960324
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_FULL": {
+        "nameTextMapHash": 3348335508
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_RESULT_EXTRA": {
+        "nameTextMapHash": 4020525449
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GET_RESULT_TITLE": {
+        "nameTextMapHash": 4203888713
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_ADD": {
+        "nameTextMapHash": 2220090266
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_CONFIRM_PS": {
+        "nameTextMapHash": 3221696647
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_GET": {
+        "nameTextMapHash": 305082602
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_PLANT": {
+        "nameTextMapHash": 4030535618
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_SELECT": {
+        "nameTextMapHash": 3711740906
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_GUIDE_SWITCH": {
+        "nameTextMapHash": 3509704994
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_HANDBOOK": {
+        "nameTextMapHash": 3826048254
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_LAND": {
+        "nameTextMapHash": 140959662
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_MAX": {
+        "nameTextMapHash": 2509421262
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_NEW_REMINDER": {
+        "nameTextMapHash": 1434514131
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_CONFIRM_BUTTON": {
+        "nameTextMapHash": 2431642612
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_NULL": {
+        "nameTextMapHash": 2263877997
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_NUM": {
+        "nameTextMapHash": 1959544773
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_PRODUCTION": {
+        "nameTextMapHash": 4068475453
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_INFO_TIME": {
+        "nameTextMapHash": 1409197253
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PLANT_LIST": {
+        "nameTextMapHash": 3499366211
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_PUZZLE_TITLE": {
+        "nameTextMapHash": 1164945941
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE": {
+        "nameTextMapHash": 3165600870
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_CONFIRM": {
+        "nameTextMapHash": 457646230
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_COST": {
+        "nameTextMapHash": 879243246
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_EMPTY_HINT": {
+        "nameTextMapHash": 892720849
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_FULL": {
+        "nameTextMapHash": 1915079070
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_LEVELUP_HINT": {
+        "nameTextMapHash": 2527655792
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_LIST": {
+        "nameTextMapHash": 1109419398
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_LV": {
+        "nameTextMapHash": 525862022
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NEXT_01": {
+        "nameTextMapHash": 3148634681
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NEXT_02": {
+        "nameTextMapHash": 2945057249
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NEXT_PREVIEW": {
+        "nameTextMapHash": 3128016425
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_NULL": {
+        "nameTextMapHash": 3577571342
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_PRESS_HINT": {
+        "nameTextMapHash": 3722527312
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_SELECT": {
+        "nameTextMapHash": 2049845350
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_REFINE_TECH_HINT": {
+        "nameTextMapHash": 2014867353
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_SELECT_PS": {
+        "nameTextMapHash": 3549833228
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_SWITCH_PS": {
+        "nameTextMapHash": 3073623065
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CROP_UPGRADE_TIPS": {
+        "nameTextMapHash": 2932826325
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_CURRENT_ROUND": {
+        "nameTextMapHash": 2335724395
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER": {
+        "nameTextMapHash": 3255049768
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_CHOOSE_STRATEGIES": {
+        "nameTextMapHash": 1552502322
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_COMING_TIPS": {
+        "nameTextMapHash": 3291950179
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_CONFIRM_TRADE": {
+        "nameTextMapHash": 147539766
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_DEMAND": {
+        "nameTextMapHash": 2865248228
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_PHASE": {
+        "nameTextMapHash": 3864318012
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_POTION_NOT_ENOUGH_TIPS": {
+        "nameTextMapHash": 3154371292
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_REPORT": {
+        "nameTextMapHash": 1450795460
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_RESELECT_GOODS": {
+        "nameTextMapHash": 2333750257
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_EXCEED_TIPS": {
+        "nameTextMapHash": 760392771
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_LAST_TIME": {
+        "nameTextMapHash": 1716876418
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_NOT_ENOUGH_TIPS": {
+        "nameTextMapHash": 3806717142
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGIES_PROCESS": {
+        "nameTextMapHash": 1265892505
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_FEEDBACK": {
+        "nameTextMapHash": 2864966597
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_GOOD": {
+        "nameTextMapHash": 3937080797
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_INCREASE": {
+        "nameTextMapHash": 96686469
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_NAME": {
+        "nameTextMapHash": 3923519965
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_NORMAL": {
+        "nameTextMapHash": 2826257381
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DEALER_STRATEGY_RESULT": {
+        "nameTextMapHash": 2076882197
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_DETAIL": {
+        "nameTextMapHash": 3359130232
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_END_ROUND": {
+        "nameTextMapHash": 2956363186
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_END_ROUND_TIPS": {
+        "nameTextMapHash": 4004383408
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM": {
+        "nameTextMapHash": 1489049872
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_AUTO_SUMBIT": {
+        "nameTextMapHash": 1860831001
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_BEST_RESULT": {
+        "nameTextMapHash": 1892615315
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_END": {
+        "nameTextMapHash": 2190725191
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_EXIT": {
+        "nameTextMapHash": 3368876455
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_FAIL": {
+        "nameTextMapHash": 42311719
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_FINISH_HINT": {
+        "nameTextMapHash": 3444308813
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_GET_TECH_REWARD": {
+        "nameTextMapHash": 3921170044
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_GOAL": {
+        "nameTextMapHash": 2459701479
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_NO_RESULT": {
+        "nameTextMapHash": 3958329889
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_PASS_TIPS": {
+        "nameTextMapHash": 1415089042
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_POTION_HINT": {
+        "nameTextMapHash": 2030579735
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_REMAINING": {
+        "nameTextMapHash": 2161529207
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_REMIND": {
+        "nameTextMapHash": 265180103
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT": {
+        "nameTextMapHash": 4072348335
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_A": {
+        "nameTextMapHash": 4228174836
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_B": {
+        "nameTextMapHash": 998804732
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_C": {
+        "nameTextMapHash": 1170346052
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_RULE": {
+        "nameTextMapHash": 3275548036
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RESULT_S": {
+        "nameTextMapHash": 2860802956
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_RETRY": {
+        "nameTextMapHash": 1813669831
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_START": {
+        "nameTextMapHash": 2776004447
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_START_TIPS": {
+        "nameTextMapHash": 411412398
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_SUBMIT": {
+        "nameTextMapHash": 372456407
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_SUCCESS": {
+        "nameTextMapHash": 467056263
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_SUMBIT_HINT": {
+        "nameTextMapHash": 241646308
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_TECH_BRANCH_LOCK_TIPS": {
+        "nameTextMapHash": 192054441
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXAM_TECH_REWARD_TIPS": {
+        "nameTextMapHash": 2353592830
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXIT": {
+        "nameTextMapHash": 206560576
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXIT_SELL_HINT": {
+        "nameTextMapHash": 268512874
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_EXTRA_TECH_BRANCH_LOCK_TIPS": {
+        "nameTextMapHash": 3642691247
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_FILTER_FAILED": {
+        "nameTextMapHash": 1564044491
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_FILTER_TIPS": {
+        "nameTextMapHash": 4083996483
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_FILTER_TITLE": {
+        "nameTextMapHash": 2950146595
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_FULLY_UPGRADE_TIPS": {
+        "nameTextMapHash": 3631102143
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOODS_CHANGED_TIPS": {
+        "nameTextMapHash": 1873612768
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOODS_COST": {
+        "nameTextMapHash": 2700845471
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOODS_LIMIT": {
+        "nameTextMapHash": 742519359
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOODS_OVERAGE": {
+        "nameTextMapHash": 3046547647
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOODS_RENEW": {
+        "nameTextMapHash": 2511938679
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOTO_FAIL": {
+        "nameTextMapHash": 3490945069
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GOTO_START": {
+        "nameTextMapHash": 1666156597
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_GUIDE_HANDBOOK": {
+        "nameTextMapHash": 3959957694
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK": {
+        "nameTextMapHash": 570630968
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_BLANK": {
+        "nameTextMapHash": 771501009
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_CASH_DESC": {
+        "nameTextMapHash": 2064421352
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_CASH_TITLE": {
+        "nameTextMapHash": 3504690048
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_COMPLETION": {
+        "nameTextMapHash": 1974352049
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_CONSUMPTION_TIPS": {
+        "nameTextMapHash": 3882944814
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_DEALER_COMING": {
+        "nameTextMapHash": 4086860917
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_DESC": {
+        "nameTextMapHash": 877106425
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_EVENT": {
+        "nameTextMapHash": 3987140081
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_FIXED_TASKS": {
+        "nameTextMapHash": 2886859136
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_GOAL_DESC": {
+        "nameTextMapHash": 1957695752
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_GOAL_TITLE": {
+        "nameTextMapHash": 720319984
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_LEVEL_DESC": {
+        "nameTextMapHash": 253681748
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_LEVEL_TITLE": {
+        "nameTextMapHash": 134930284
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_OVERVIEW": {
+        "nameTextMapHash": 838637073
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_REPORT": {
+        "nameTextMapHash": 3927094049
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_SHOP_TIPS": {
+        "nameTextMapHash": 2048656217
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_TECHTREE_TIPS": {
+        "nameTextMapHash": 2064685279
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_HANDBOOK_TITLE": {
+        "nameTextMapHash": 1804012113
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_INCOME": {
+        "nameTextMapHash": 1714191144
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_LAST_ROUND": {
+        "nameTextMapHash": 1770624946
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_LETTER": {
+        "nameTextMapHash": 2701171664
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_MARK_DESC": {
+        "nameTextMapHash": 69515334
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_MARK_TITLE": {
+        "nameTextMapHash": 1466883022
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_MONEY_LIMIT_TIPS": {
+        "nameTextMapHash": 3489785899
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NETWORK_DELAY": {
+        "nameTextMapHash": 1842511743
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NEWS": {
+        "nameTextMapHash": 2822277408
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NEWS_REFRESH_TIPS": {
+        "nameTextMapHash": 1293673642
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NEWS_TITLE_01": {
+        "nameTextMapHash": 1179269823
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NEWS_TITLE_02": {
+        "nameTextMapHash": 864701983
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NEWS_TITLE_03": {
+        "nameTextMapHash": 3915482759
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NO_GOODS_REPORT": {
+        "nameTextMapHash": 2070337323
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_NO_RECORD_TIPS": {
+        "nameTextMapHash": 3684601830
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_OPEN_HINT": {
+        "nameTextMapHash": 2663035169
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER": {
+        "nameTextMapHash": 3833116960
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER_BREAK_TIPS": {
+        "nameTextMapHash": 2620447979
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER_DELIVER": {
+        "nameTextMapHash": 4247664708
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER_NO_GOODS_TIPS": {
+        "nameTextMapHash": 3763775677
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER_POTION_NOT_ENOUGH_TIPS": {
+        "nameTextMapHash": 1518725925
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER_REMIND": {
+        "nameTextMapHash": 2075006004
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ORDER_START_TIPS": {
+        "nameTextMapHash": 517911730
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PHASE_REWARD_TITLE": {
+        "nameTextMapHash": 2100017299
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLANT": {
+        "nameTextMapHash": 2710041112
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLANT_HARVESTABLE": {
+        "nameTextMapHash": 3362799500
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL": {
+        "nameTextMapHash": 1007061820
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_LV": {
+        "nameTextMapHash": 2415299030
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_PREVIEW_REWARD": {
+        "nameTextMapHash": 872272043
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_PREVIEW_TITLE": {
+        "nameTextMapHash": 3148920187
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_TITLE": {
+        "nameTextMapHash": 1408865462
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_UNLOCK_TIPS": {
+        "nameTextMapHash": 1535061702
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PLAYER_LEVEL_UP": {
+        "nameTextMapHash": 3620871358
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION": {
+        "nameTextMapHash": 447909936
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_CANCEL_ALL_BUTTON": {
+        "nameTextMapHash": 4079748027
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_CANCEL_ALL_HINT": {
+        "nameTextMapHash": 525558803
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_CANCEL_BUTTON": {
+        "nameTextMapHash": 749318691
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_CONFIRM_BUTTON": {
+        "nameTextMapHash": 472499042
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DENY": {
+        "nameTextMapHash": 2055168299
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DETAIL_CLOSE_PS": {
+        "nameTextMapHash": 419438004
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DETAIL_OPEN_PS": {
+        "nameTextMapHash": 3835748974
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY": {
+        "nameTextMapHash": 3842102075
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_BOTTLE": {
+        "nameTextMapHash": 1640814649
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_CANCEL": {
+        "nameTextMapHash": 1846190417
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_DECORATION": {
+        "nameTextMapHash": 189398009
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_DECORATION_UNSELECT": {
+        "nameTextMapHash": 2263621212
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_FINISH_BUTTON": {
+        "nameTextMapHash": 633774831
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DIY_SELECT": {
+        "nameTextMapHash": 2958631497
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_BUTTON": {
+        "nameTextMapHash": 393120248
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_DESC": {
+        "nameTextMapHash": 3398214424
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_NEW_TITLE": {
+        "nameTextMapHash": 1789624271
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_OLD_TITLE": {
+        "nameTextMapHash": 3582173295
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_ONSALE": {
+        "nameTextMapHash": 2762213128
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_ONSALE_HINT": {
+        "nameTextMapHash": 1567713157
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_TITLE": {
+        "nameTextMapHash": 4208779544
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_DROP_UNSELECT": {
+        "nameTextMapHash": 1627540872
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_DETAIL": {
+        "nameTextMapHash": 224915786
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_HINT": {
+        "nameTextMapHash": 1008671994
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_MAIN": {
+        "nameTextMapHash": 1211384498
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXAM_SUB": {
+        "nameTextMapHash": 3582962242
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_EXIT_HINT": {
+        "nameTextMapHash": 924322210
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_BUTTON": {
+        "nameTextMapHash": 440184632
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_CANCEL_PS": {
+        "nameTextMapHash": 2950351602
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_CLOSE_PS": {
+        "nameTextMapHash": 1076593406
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_LACK": {
+        "nameTextMapHash": 336298272
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_RETURN_PS": {
+        "nameTextMapHash": 4048617206
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_SELECT_PS": {
+        "nameTextMapHash": 1640309246
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_TIPS": {
+        "nameTextMapHash": 3183767176
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FAST_UNSELECT": {
+        "nameTextMapHash": 1467721280
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FINISH_BUTTON": {
+        "nameTextMapHash": 2433712096
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FINISH_DENY": {
+        "nameTextMapHash": 634755296
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_FINISH_HINT": {
+        "nameTextMapHash": 3501538696
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_INFO": {
+        "nameTextMapHash": 1582478381
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_PUT": {
+        "nameTextMapHash": 1175889901
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_ROTATE": {
+        "nameTextMapHash": 910035949
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_SELECT": {
+        "nameTextMapHash": 285431381
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_GUIDE_SELECT_PS": {
+        "nameTextMapHash": 2152673139
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_MATERIAL": {
+        "nameTextMapHash": 1475721635
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_01": {
+        "nameTextMapHash": 2830500012
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_02": {
+        "nameTextMapHash": 3961146284
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_03": {
+        "nameTextMapHash": 27808028
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_04": {
+        "nameTextMapHash": 2690255596
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_05": {
+        "nameTextMapHash": 4024965420
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_06": {
+        "nameTextMapHash": 2511419844
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_DEFAULT": {
+        "nameTextMapHash": 1720178364
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_DUAL_PROP": {
+        "nameTextMapHash": 2344868076
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NAME_PLUS": {
+        "nameTextMapHash": 1338492332
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_NUM_FORMAT": {
+        "nameTextMapHash": 1316866658
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_OVERLAP_NUMBER": {
+        "nameTextMapHash": 2881035403
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_OVERLAP_TITLE": {
+        "nameTextMapHash": 2387902675
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_POT_FAST": {
+        "nameTextMapHash": 3075591664
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_POT_LIMIT": {
+        "nameTextMapHash": 2007284400
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_POT_NORMAL": {
+        "nameTextMapHash": 2493022544
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_PRICE": {
+        "nameTextMapHash": 767464803
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_PROP_CLOSE_PS": {
+        "nameTextMapHash": 1988142246
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_PROP_DETAIL": {
+        "nameTextMapHash": 3746493585
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_PROP_TITLE": {
+        "nameTextMapHash": 3513057881
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_PS_EDIT": {
+        "nameTextMapHash": 2964225862
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_PS_REGION_SWITCH": {
+        "nameTextMapHash": 322565970
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RATE_FORMAT": {
+        "nameTextMapHash": 596971908
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RATE_TITLE": {
+        "nameTextMapHash": 1560593844
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT": {
+        "nameTextMapHash": 3687991235
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_01": {
+        "nameTextMapHash": 2882278626
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_02": {
+        "nameTextMapHash": 1172118562
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_03": {
+        "nameTextMapHash": 1511707130
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_04": {
+        "nameTextMapHash": 3535212778
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_05": {
+        "nameTextMapHash": 476466738
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_BUFF_TITLE": {
+        "nameTextMapHash": 2415349850
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_LEVEL_MAX": {
+        "nameTextMapHash": 2296055327
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_LEVEL_TITLE": {
+        "nameTextMapHash": 3904180919
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_NEW_HINT": {
+        "nameTextMapHash": 1601802646
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_CROP_NEW_TITLE": {
+        "nameTextMapHash": 417296102
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_EFFICIENCY_NEW_HINT": {
+        "nameTextMapHash": 70358347
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_GET_BUTTON": {
+        "nameTextMapHash": 3695074862
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_LEVEL": {
+        "nameTextMapHash": 3737730609
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_OVERLAP_NEW_HINT": {
+        "nameTextMapHash": 4071250869
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_POTION_TWICE_HINT": {
+        "nameTextMapHash": 676684738
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_POT_NEW_HINT": {
+        "nameTextMapHash": 872995415
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_RESULT_SHOP_HINT": {
+        "nameTextMapHash": 1943562094
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_ROTATE_BUTTON": {
+        "nameTextMapHash": 907336942
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_TAG_CONNECT": {
+        "nameTextMapHash": 2217375106
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_UPGRADE": {
+        "nameTextMapHash": 561717907
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_UPGRADE_NONE": {
+        "nameTextMapHash": 710146989
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_POTION_UPGRADE_TIPS": {
+        "nameTextMapHash": 1395982909
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PROFIT": {
+        "nameTextMapHash": 1008304944
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_PROFIT_TREND": {
+        "nameTextMapHash": 2244650763
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_REVENUE": {
+        "nameTextMapHash": 3212714024
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_REVENUE_DETAIL": {
+        "nameTextMapHash": 2581133676
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_REVENUE_STRUCTURE": {
+        "nameTextMapHash": 3368000028
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_REWARD_TITLE": {
+        "nameTextMapHash": 2272915512
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ROUND": {
+        "nameTextMapHash": 1313001512
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ROUND_DETAIL": {
+        "nameTextMapHash": 2803436546
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ROUND_INTERVAL": {
+        "nameTextMapHash": 391144602
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_ROUND_REVENUE": {
+        "nameTextMapHash": 4210170850
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SALES_VOLUME": {
+        "nameTextMapHash": 3943910858
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SAVE_AND_EXIT": {
+        "nameTextMapHash": 1232609571
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SELECTED_GOODS": {
+        "nameTextMapHash": 3598429310
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SELL": {
+        "nameTextMapHash": 4735656
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SELLING_REPORT": {
+        "nameTextMapHash": 492526849
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SHELF": {
+        "nameTextMapHash": 3675317720
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SHOP_COST": {
+        "nameTextMapHash": 1880211474
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SHOP_GOODS_LOCK_01": {
+        "nameTextMapHash": 997220477
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SHOP_GOODS_LOCK_02": {
+        "nameTextMapHash": 2731785765
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SHOP_GOODS_UNLOCK": {
+        "nameTextMapHash": 1574109973
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_BREAK": {
+        "nameTextMapHash": 4158156572
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_BREAK_TIPS": {
+        "nameTextMapHash": 3966199568
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_GOAL": {
+        "nameTextMapHash": 398566652
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_GOAL_NO_TITLE": {
+        "nameTextMapHash": 3769819083
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_GOAL_PERCENTAGE": {
+        "nameTextMapHash": 1672542260
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_LAST_ROUND": {
+        "nameTextMapHash": 222021070
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_LOCK_TIPS": {
+        "nameTextMapHash": 3682890513
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_LOCK_TIPS_01": {
+        "nameTextMapHash": 2492805329
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_REWARD": {
+        "nameTextMapHash": 3362433252
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_TASK_TIPS": {
+        "nameTextMapHash": 4259781509
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_STAGE_TIPS": {
+        "nameTextMapHash": 3274191132
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY": {
+        "nameTextMapHash": 745584040
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC1": {
+        "nameTextMapHash": 2008955883
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC2": {
+        "nameTextMapHash": 1088689867
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC3": {
+        "nameTextMapHash": 2643554843
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC4": {
+        "nameTextMapHash": 1092531099
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_DESC5": {
+        "nameTextMapHash": 3397610147
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM1": {
+        "nameTextMapHash": 1684147851
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM2": {
+        "nameTextMapHash": 713505259
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM3": {
+        "nameTextMapHash": 2022157355
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM4": {
+        "nameTextMapHash": 648713187
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P1_PARM5": {
+        "nameTextMapHash": 3545579395
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC1": {
+        "nameTextMapHash": 1030065665
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC2": {
+        "nameTextMapHash": 1560583585
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC3": {
+        "nameTextMapHash": 2729727593
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC4": {
+        "nameTextMapHash": 111738681
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_DESC5": {
+        "nameTextMapHash": 126655801
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM1": {
+        "nameTextMapHash": 3252526905
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM2": {
+        "nameTextMapHash": 4127593785
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM3": {
+        "nameTextMapHash": 1225289801
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM4": {
+        "nameTextMapHash": 2091939337
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P2_PARM5": {
+        "nameTextMapHash": 1925051361
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC1": {
+        "nameTextMapHash": 547748127
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC2": {
+        "nameTextMapHash": 1762530087
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC3": {
+        "nameTextMapHash": 602357767
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC4": {
+        "nameTextMapHash": 1914013111
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_DESC5": {
+        "nameTextMapHash": 2526635311
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM1": {
+        "nameTextMapHash": 2824964847
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM2": {
+        "nameTextMapHash": 1660515759
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM3": {
+        "nameTextMapHash": 639497479
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM4": {
+        "nameTextMapHash": 431265415
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P3_PARM5": {
+        "nameTextMapHash": 1094503487
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC1": {
+        "nameTextMapHash": 2278648236
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC2": {
+        "nameTextMapHash": 1969932468
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC3": {
+        "nameTextMapHash": 2359385860
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC4": {
+        "nameTextMapHash": 2316047156
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_DESC5": {
+        "nameTextMapHash": 442403268
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM1": {
+        "nameTextMapHash": 3379185172
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM2": {
+        "nameTextMapHash": 4067807044
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM3": {
+        "nameTextMapHash": 1407939252
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM4": {
+        "nameTextMapHash": 196161084
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_P4_PARM5": {
+        "nameTextMapHash": 3005412876
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_SUMMARY_TITLE": {
+        "nameTextMapHash": 4184142263
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TAG_NAME": {
+        "nameTextMapHash": 3876860324
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TAG_TITLE": {
+        "nameTextMapHash": 4061151388
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TASK_NOT_FINISH": {
+        "nameTextMapHash": 2039395681
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_FINISH": {
+        "nameTextMapHash": 4289561557
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_LEVEL_DETAIL": {
+        "nameTextMapHash": 424028999
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UNLOCK": {
+        "nameTextMapHash": 3225681365
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UNLOCK_TIPS": {
+        "nameTextMapHash": 3124018265
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UPGRADE": {
+        "nameTextMapHash": 2242764437
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_BRANCH_UPGRADE_TIPS": {
+        "nameTextMapHash": 2136479449
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_ALCHEMY_TITLE": {
+        "nameTextMapHash": 3528541260
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_EXAM_TITLE": {
+        "nameTextMapHash": 3135623612
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_PLANT_TITLE": {
+        "nameTextMapHash": 3966241995
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_SELL_TITLE": {
+        "nameTextMapHash": 311730520
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TECH_TREE_TITLE": {
+        "nameTextMapHash": 1844405521
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TUTORIAL_NOT_RECORD": {
+        "nameTextMapHash": 3258793305
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TUTORIAL_TITLE": {
+        "nameTextMapHash": 3956948558
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TYPE_NAME": {
+        "nameTextMapHash": 3827195457
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_TYPE_TITLE": {
+        "nameTextMapHash": 778662985
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_UPGRADE_CONSUME": {
+        "nameTextMapHash": 1294297115
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_UPGRADE_SUCCESS": {
+        "nameTextMapHash": 245671115
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_WEAPON_REDEEM": {
+        "nameTextMapHash": 1449494223
+    },
+    "UI_ACTIVITY_ALCHEMYSIM_WEAPON_REDEEM_TIPS": {
+        "nameTextMapHash": 1470624583
+    },
     "UI_ACTIVITY_AREA_QUESTTIPS": {
         "nameTextMapHash": 896037515
     },
     "UI_ACTIVITY_ARENACHALLENGE3_REWARD_DESC": {
         "nameTextMapHash": 3591115396
     },
     "UI_ACTIVITY_ARENACHALLENGE4_CHALLENGE_FACTOR": {
@@ -15376,14 +16627,74 @@
     },
     "UI_ACTIVITY_ASTROLABLE_PROGRESS": {
         "nameTextMapHash": 3285814292
     },
     "UI_ACTIVITY_AUTO_QUIT": {
         "nameTextMapHash": 4213771873
     },
+    "UI_ACTIVITY_AUTO_TIME_STOP_ACTION_TIPS": {
+        "nameTextMapHash": 1577242564
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_CAMERA_TIPS": {
+        "nameTextMapHash": 2736393882
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_CHAR_CHANGE_TIPS": {
+        "nameTextMapHash": 2130506856
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_CHAR_NOT_FULL_TIPS": {
+        "nameTextMapHash": 1126526848
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_DUNGEON_ENTRY_INTERACTION": {
+        "nameTextMapHash": 567694789
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_DUNGEON_TITLE": {
+        "nameTextMapHash": 1720579352
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_END_QUEST_BUTTON": {
+        "nameTextMapHash": 3541305859
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_EXIT_DUNGEON_TIPS": {
+        "nameTextMapHash": 1646682641
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_EXIT_TIPS": {
+        "nameTextMapHash": 467104758
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_GUIDE_TIPS": {
+        "nameTextMapHash": 1921672378
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_GUIDE_TIPS_1": {
+        "nameTextMapHash": 2333823033
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_LEVEL_BUFF_TITLE": {
+        "nameTextMapHash": 1758507918
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_LEVEL_DESC": {
+        "nameTextMapHash": 1514102142
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_MAIN_PROGRESS": {
+        "nameTextMapHash": 1468022043
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_PRE_LEVEL_LOCKED": {
+        "nameTextMapHash": 1089988484
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_SUCCEED_DATA_TITLE": {
+        "nameTextMapHash": 4044858431
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_TARGET_1": {
+        "nameTextMapHash": 3025440236
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_TARGET_2": {
+        "nameTextMapHash": 776780460
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_TEAM_TITLE": {
+        "nameTextMapHash": 463757385
+    },
+    "UI_ACTIVITY_AUTO_TIME_STOP_TITLE": {
+        "nameTextMapHash": 3295518470
+    },
     "UI_ACTIVITY_AVARTARTRIAL_INDUNGEON_FINISHPANEL_CHANGE": {
         "nameTextMapHash": 575427936
     },
     "UI_ACTIVITY_AVARTARTRIAL_INDUNGEON_FINISHPANEL_CONTINUE": {
         "nameTextMapHash": 1536442424
     },
     "UI_ACTIVITY_AVARTARTRIAL_INDUNGEON_FINISHPANEL_LEAVE": {
@@ -15421,17 +16732,14 @@
     },
     "UI_ACTIVITY_AVATAR_PROGRESS_UNMET": {
         "nameTextMapHash": 3508067920
     },
     "UI_ACTIVITY_AWARDPAGE": {
         "nameTextMapHash": 2525653840
     },
-    "UI_ACTIVITY_BARTENDER_REDO_BUTTON": {
-        "nameTextMapHash": 1468543417
-    },
     "UI_ACTIVITY_BEGINTIME": {
         "nameTextMapHash": 3502714504
     },
     "UI_ACTIVITY_BESTSCORE_CRUCIBLE": {
         "nameTextMapHash": 3132123125
     },
     "UI_ACTIVITY_BEST_RECORD": {
@@ -15871,14 +17179,200 @@
     },
     "UI_ACTIVITY_BounceConjuring_DESC": {
         "nameTextMapHash": 3387641929
     },
     "UI_ACTIVITY_CANNOT_ONLINE_TIPS": {
         "nameTextMapHash": 1348315470
     },
+    "UI_ACTIVITY_CATCAFE_ABANDON": {
+        "nameTextMapHash": 1801579372
+    },
+    "UI_ACTIVITY_CATCAFE_ACTIVITYNAME": {
+        "nameTextMapHash": 815897364
+    },
+    "UI_ACTIVITY_CATCAFE_AFFECTION": {
+        "nameTextMapHash": 724136372
+    },
+    "UI_ACTIVITY_CATCAFE_AFFECTION_HINT": {
+        "nameTextMapHash": 4200307400
+    },
+    "UI_ACTIVITY_CATCAFE_AUTOSAVED_FINISHHINT": {
+        "nameTextMapHash": 1106471958
+    },
+    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT1COME": {
+        "nameTextMapHash": 3761692188
+    },
+    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT2COME": {
+        "nameTextMapHash": 1667709068
+    },
+    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT3COME": {
+        "nameTextMapHash": 2198233332
+    },
+    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT4COME": {
+        "nameTextMapHash": 3654060124
+    },
+    "UI_ACTIVITY_CATCAFE_BLACKSCREEN_CAT5COME": {
+        "nameTextMapHash": 974941804
+    },
+    "UI_ACTIVITY_CATCAFE_BOSSDES": {
+        "nameTextMapHash": 2058173052
+    },
+    "UI_ACTIVITY_CATCAFE_BOSSLEAVING": {
+        "nameTextMapHash": 1648213932
+    },
+    "UI_ACTIVITY_CATCAFE_BOSSLOCKED_HINT": {
+        "nameTextMapHash": 2928441111
+    },
+    "UI_ACTIVITY_CATCAFE_BOSSLOCKED_TITLE": {
+        "nameTextMapHash": 4193531119
+    },
+    "UI_ACTIVITY_CATCAFE_BOSSQUESTHINT": {
+        "nameTextMapHash": 315165860
+    },
+    "UI_ACTIVITY_CATCAFE_CATBALCONY": {
+        "nameTextMapHash": 1288757860
+    },
+    "UI_ACTIVITY_CATCAFE_CATBOSSQUEST_UNFINISHED": {
+        "nameTextMapHash": 3723515963
+    },
+    "UI_ACTIVITY_CATCAFE_CATNAME_TITLE": {
+        "nameTextMapHash": 1646487394
+    },
+    "UI_ACTIVITY_CATCAFE_CATREPUTATION": {
+        "nameTextMapHash": 32804988
+    },
+    "UI_ACTIVITY_CATCAFE_CATREPUTATION_FULL": {
+        "nameTextMapHash": 2399116886
+    },
+    "UI_ACTIVITY_CATCAFE_DECOFINISHED": {
+        "nameTextMapHash": 1467273508
+    },
+    "UI_ACTIVITY_CATCAFE_DECOFINISHED_CANTCHANGE": {
+        "nameTextMapHash": 1501870942
+    },
+    "UI_ACTIVITY_CATCAFE_DECOHINT": {
+        "nameTextMapHash": 607725564
+    },
+    "UI_ACTIVITY_CATCAFE_DECOQUIT_DESC": {
+        "nameTextMapHash": 455062617
+    },
+    "UI_ACTIVITY_CATCAFE_DECOQUIT_TITLE": {
+        "nameTextMapHash": 2014152769
+    },
+    "UI_ACTIVITY_CATCAFE_DECOSAVED": {
+        "nameTextMapHash": 178431740
+    },
+    "UI_ACTIVITY_CATCAFE_DECO_INTERACTNAME": {
+        "nameTextMapHash": 1195515751
+    },
+    "UI_ACTIVITY_CATCAFE_DECO_SCOREA": {
+        "nameTextMapHash": 2143870343
+    },
+    "UI_ACTIVITY_CATCAFE_DECO_SCOREB": {
+        "nameTextMapHash": 4006811063
+    },
+    "UI_ACTIVITY_CATCAFE_DECO_SCOREC": {
+        "nameTextMapHash": 475719719
+    },
+    "UI_ACTIVITY_CATCAFE_ENDINGQUEST": {
+        "nameTextMapHash": 201099028
+    },
+    "UI_ACTIVITY_CATCAFE_FAMILIAR": {
+        "nameTextMapHash": 2172787612
+    },
+    "UI_ACTIVITY_CATCAFE_FAMILIARHINT": {
+        "nameTextMapHash": 2372560476
+    },
+    "UI_ACTIVITY_CATCAFE_FAVORDROP": {
+        "nameTextMapHash": 3504299852
+    },
+    "UI_ACTIVITY_CATCAFE_FAVORSTOP": {
+        "nameTextMapHash": 88708364
+    },
+    "UI_ACTIVITY_CATCAFE_FAVOR_MINUS": {
+        "nameTextMapHash": 4095771853
+    },
+    "UI_ACTIVITY_CATCAFE_FAVOR_PLUS": {
+        "nameTextMapHash": 2847654109
+    },
+    "UI_ACTIVITY_CATCAFE_FEEDDESC": {
+        "nameTextMapHash": 481817724
+    },
+    "UI_ACTIVITY_CATCAFE_FEEDFINISHED": {
+        "nameTextMapHash": 295185188
+    },
+    "UI_ACTIVITY_CATCAFE_FEEDHINT": {
+        "nameTextMapHash": 1765445700
+    },
+    "UI_ACTIVITY_CATCAFE_FEEDTITLE": {
+        "nameTextMapHash": 800625676
+    },
+    "UI_ACTIVITY_CATCAFE_FEED_INTERACTNAME": {
+        "nameTextMapHash": 1554941298
+    },
+    "UI_ACTIVITY_CATCAFE_GOTO_DECO": {
+        "nameTextMapHash": 3537672899
+    },
+    "UI_ACTIVITY_CATCAFE_GOTO_FEED": {
+        "nameTextMapHash": 3531406491
+    },
+    "UI_ACTIVITY_CATCAFE_GOTO_PLAY": {
+        "nameTextMapHash": 2371412483
+    },
+    "UI_ACTIVITY_CATCAFE_HINT_COUNTDOWN": {
+        "nameTextMapHash": 2362168758
+    },
+    "UI_ACTIVITY_CATCAFE_HINT_LOCKED": {
+        "nameTextMapHash": 966928398
+    },
+    "UI_ACTIVITY_CATCAFE_MARK_DESC": {
+        "nameTextMapHash": 139343108
+    },
+    "UI_ACTIVITY_CATCAFE_MARK_TITLE": {
+        "nameTextMapHash": 2381868588
+    },
+    "UI_ACTIVITY_CATCAFE_PLAYQUIT_BLACK": {
+        "nameTextMapHash": 1455294909
+    },
+    "UI_ACTIVITY_CATCAFE_PLAYQUIT_DESC": {
+        "nameTextMapHash": 527884565
+    },
+    "UI_ACTIVITY_CATCAFE_PLAYQUIT_TITLE": {
+        "nameTextMapHash": 329069509
+    },
+    "UI_ACTIVITY_CATCAFE_PLAYUNLOCKHINT": {
+        "nameTextMapHash": 401580276
+    },
+    "UI_ACTIVITY_CATCAFE_PLAY_INTERACTNAME": {
+        "nameTextMapHash": 3205506787
+    },
+    "UI_ACTIVITY_CATCAFE_REPUTATION_NUM1": {
+        "nameTextMapHash": 2858381703
+    },
+    "UI_ACTIVITY_CATCAFE_REPUTATION_NUM2": {
+        "nameTextMapHash": 3107502759
+    },
+    "UI_ACTIVITY_CATCAFE_SAVEANDQUIT": {
+        "nameTextMapHash": 4129811156
+    },
+    "UI_ACTIVITY_CATCAFE_STATE": {
+        "nameTextMapHash": 2409443652
+    },
+    "UI_ACTIVITY_CATCAFE_UNDECOED": {
+        "nameTextMapHash": 283514756
+    },
+    "UI_ACTIVITY_CATCAFE_UNFARMILIAR": {
+        "nameTextMapHash": 3917719972
+    },
+    "UI_ACTIVITY_CATCAFE_UNLOCKHINT": {
+        "nameTextMapHash": 3389278892
+    },
+    "UI_ACTIVITY_CATCAFE_UNSUMMON": {
+        "nameTextMapHash": 3523262276
+    },
     "UI_ACTIVITY_CHALLENGE_BEGIN": {
         "nameTextMapHash": 678714236
     },
     "UI_ACTIVITY_CHALLENGE_DETAIL": {
         "nameTextMapHash": 3121683592
     },
     "UI_ACTIVITY_CHALLENGE_GOTO_BUTTON": {
@@ -16588,245 +18082,17 @@
     },
     "UI_ACTIVITY_CONTRACT_COST": {
         "nameTextMapHash": 670913866
     },
     "UI_ACTIVITY_CONTRACT_GET_BUTTON": {
         "nameTextMapHash": 3575927637
     },
-    "UI_ACTIVITY_COOKGAME_COND_LASTLEVEL": {
-        "nameTextMapHash": 1139594074
-    },
-    "UI_ACTIVITY_COOKGAME_FAIL_REDO": {
-        "nameTextMapHash": 4226004242
-    },
-    "UI_ACTIVITY_COOKGAME_INTERACT": {
-        "nameTextMapHash": 2793209322
-    },
-    "UI_ACTIVITY_COOKGAME_INTERACT2": {
-        "nameTextMapHash": 1095762682
-    },
-    "UI_ACTIVITY_COOKGAME_INTERACT3": {
-        "nameTextMapHash": 3660521562
-    },
-    "UI_ACTIVITY_COOKGAME_INTERACT4": {
-        "nameTextMapHash": 2906349986
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL1_PHASE1_PRODUCT1": {
-        "nameTextMapHash": 4215945465
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL1_PHASE1_PRODUCT2": {
-        "nameTextMapHash": 962108161
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL1_PHASE2_PRODUCT1": {
-        "nameTextMapHash": 2363372107
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL2_PHASE1_PRODUCT1": {
-        "nameTextMapHash": 1152584551
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL2_PHASE1_PRODUCT2": {
-        "nameTextMapHash": 1572626607
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL2_PHASE1_PRODUCT3": {
-        "nameTextMapHash": 3341991207
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL2_PHASE2_PRODUCT1": {
-        "nameTextMapHash": 78069206
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL3_PHASE1_PRODUCT1": {
-        "nameTextMapHash": 3785075237
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL3_PHASE1_PRODUCT2": {
-        "nameTextMapHash": 115061485
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL3_PHASE2_PRODUCT1": {
-        "nameTextMapHash": 633491784
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL4_PHASE1_PRODUCT1": {
-        "nameTextMapHash": 670113412
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL4_PHASE1_PRODUCT2": {
-        "nameTextMapHash": 3549857100
-    },
-    "UI_ACTIVITY_COOKGAME_LEVEL4_PHASE2_PRODUCT1": {
-        "nameTextMapHash": 4009720364
-    },
     "UI_ACTIVITY_COOKGAME_LEVELMENU_DESC_TITLE": {
         "nameTextMapHash": 1254517569
     },
-    "UI_ACTIVITY_COOKGAME_LEVELSELECT_DESC_TITLE": {
-        "nameTextMapHash": 2759700208
-    },
-    "UI_ACTIVITY_COOKGAME_LEVELSELECT_SWITCHCHARACTER_JS": {
-        "nameTextMapHash": 405853715
-    },
-    "UI_ACTIVITY_COOKGAME_LEVELSTART_MAIN_ITEM": {
-        "nameTextMapHash": 2256344695
-    },
-    "UI_ACTIVITY_COOKGAME_LEVELSTART_START": {
-        "nameTextMapHash": 2494983940
-    },
-    "UI_ACTIVITY_COOKGAME_NAME_TITLE": {
-        "nameTextMapHash": 2881111061
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_COMPLETE": {
-        "nameTextMapHash": 341443872
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_FAIL": {
-        "nameTextMapHash": 2671051432
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_INGAME_OP_JS": {
-        "nameTextMapHash": 41948532
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_INGAME_START_JS": {
-        "nameTextMapHash": 2990693523
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_JS": {
-        "nameTextMapHash": 3743722702
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_RULE": {
-        "nameTextMapHash": 3954436846
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_START": {
-        "nameTextMapHash": 452881566
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_TARGET": {
-        "nameTextMapHash": 3169055662
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_TARGET2": {
-        "nameTextMapHash": 1151017806
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_TARGET3": {
-        "nameTextMapHash": 3185534006
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_TARGET4": {
-        "nameTextMapHash": 854862062
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE1_START_TITLE": {
-        "nameTextMapHash": 2436648318
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_COMPLETE": {
-        "nameTextMapHash": 3325664256
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_FAIL": {
-        "nameTextMapHash": 3699524872
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_INGAME_OP_JS": {
-        "nameTextMapHash": 1855461306
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_START_RULE": {
-        "nameTextMapHash": 3949879822
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_START_TARGET": {
-        "nameTextMapHash": 1161405486
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_START_TARGET2": {
-        "nameTextMapHash": 3930828830
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_START_TARGET3": {
-        "nameTextMapHash": 2834787062
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_START_TARGET4": {
-        "nameTextMapHash": 3975925894
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE2_START_TITLE": {
-        "nameTextMapHash": 210361286
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_COMPLETE": {
-        "nameTextMapHash": 3286736797
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_FAIL": {
-        "nameTextMapHash": 2823907325
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_INGAME_OP_JS": {
-        "nameTextMapHash": 3033449423
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_START_RULE": {
-        "nameTextMapHash": 4208267945
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_START_TARGET": {
-        "nameTextMapHash": 1124539577
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_START_TARGET2": {
-        "nameTextMapHash": 949132297
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_START_TARGET3": {
-        "nameTextMapHash": 1946999001
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_START_TARGET4": {
-        "nameTextMapHash": 3258038633
-    },
-    "UI_ACTIVITY_COOKGAME_PHASE3_START_TITLE": {
-        "nameTextMapHash": 1766999505
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_CHANGE": {
-        "nameTextMapHash": 4098303214
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_DISH1": {
-        "nameTextMapHash": 102659638
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_DISH2": {
-        "nameTextMapHash": 40886182
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_DISH3": {
-        "nameTextMapHash": 1309374582
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_DISH4": {
-        "nameTextMapHash": 755509926
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_FINISH": {
-        "nameTextMapHash": 3235313950
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_LARGEDECRO1": {
-        "nameTextMapHash": 3228168526
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_LARGEDECRO2": {
-        "nameTextMapHash": 578197030
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_LARGEDECRO3": {
-        "nameTextMapHash": 2435014246
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_LARGEDECRO4": {
-        "nameTextMapHash": 1625550014
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SMALLDECRO1": {
-        "nameTextMapHash": 273195254
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SMALLDECRO2": {
-        "nameTextMapHash": 2290420422
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SMALLDECRO3": {
-        "nameTextMapHash": 3089609830
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SMALLDECRO4": {
-        "nameTextMapHash": 1124491446
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SORT1": {
-        "nameTextMapHash": 964017246
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SORT2": {
-        "nameTextMapHash": 753553046
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_SORT3": {
-        "nameTextMapHash": 173951486
-    },
-    "UI_ACTIVITY_COOKGAME_PLATING_TITLE": {
-        "nameTextMapHash": 2002199438
-    },
-    "UI_ACTIVITY_COOKGAME_RESTART_HINT1": {
-        "nameTextMapHash": 2456252062
-    },
-    "UI_ACTIVITY_COOKGAME_RESTART_HINT2": {
-        "nameTextMapHash": 1292268038
-    },
-    "UI_ACTIVITY_COOKGAME_RESTART_HINT3": {
-        "nameTextMapHash": 184333310
-    },
-    "UI_ACTIVITY_COOKGAME_WATCHER_REWARD": {
-        "nameTextMapHash": 3552791603
-    },
     "UI_ACTIVITY_COST": {
         "nameTextMapHash": 848838336
     },
     "UI_ACTIVITY_COUNT_DOWN_SECOND": {
         "nameTextMapHash": 4167222505
     },
     "UI_ACTIVITY_CO_TELEPORT_CANCEL": {
@@ -18187,20 +19453,14 @@
     },
     "UI_ACTIVITY_HACHI_TITLE": {
         "nameTextMapHash": 3577803108
     },
     "UI_ACTIVITY_HACHI_UNLOCK_TIPS": {
         "nameTextMapHash": 3700435254
     },
-    "UI_ACTIVITY_HERMIT_DESC": {
-        "nameTextMapHash": 256050870
-    },
-    "UI_ACTIVITY_HERMIT_TITLE": {
-        "nameTextMapHash": 2442246774
-    },
     "UI_ACTIVITY_HIDEANDSEEK_NPC_DESC": {
         "nameTextMapHash": 2892615686
     },
     "UI_ACTIVITY_HIDEANDSEEK_NPC_TITLE": {
         "nameTextMapHash": 4069858334
     },
     "UI_ACTIVITY_HIDE_AND_SEEK_BUTTOM_CHANGE_CONSOLE": {
@@ -19240,281 +20500,14 @@
     },
     "UI_ACTIVITY_LANTERNRITE_XIAO_QUEST_LEVEL": {
         "nameTextMapHash": 3485363580
     },
     "UI_ACTIVITY_LANTERNRITE_XIAO_QUEST_NAME": {
         "nameTextMapHash": 3572895900
     },
-    "UI_ACTIVITY_LANV4_CARPJUMP_END": {
-        "nameTextMapHash": 2282543615
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_GEAR": {
-        "nameTextMapHash": 4266022119
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_HINT": {
-        "nameTextMapHash": 3578588999
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_LEVELCOND": {
-        "nameTextMapHash": 2781814287
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_LEVELSELECT": {
-        "nameTextMapHash": 733571647
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_LEVEL_SCORE": {
-        "nameTextMapHash": 2605544344
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_MAPMARK_DESC": {
-        "nameTextMapHash": 2504718464
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_MAPMARK_NORECORD": {
-        "nameTextMapHash": 380196744
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_MAPMARK_SCORE": {
-        "nameTextMapHash": 140934488
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_MAPMARK_TITLE": {
-        "nameTextMapHash": 2680437696
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_NAME": {
-        "nameTextMapHash": 75286911
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_QUIT": {
-        "nameTextMapHash": 3111956495
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_REMINDER_DESC": {
-        "nameTextMapHash": 4199226899
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_REMINDER_TITLE": {
-        "nameTextMapHash": 3301055515
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_SCORE_COIN": {
-        "nameTextMapHash": 33617863
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_SCORE_TIME": {
-        "nameTextMapHash": 535563887
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_SCORE_TOTAL": {
-        "nameTextMapHash": 3814788607
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_TARGET_1": {
-        "nameTextMapHash": 1204703013
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_TARGET_2": {
-        "nameTextMapHash": 4146162765
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_TARGET_TITLE": {
-        "nameTextMapHash": 1335415181
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_TIPS_SCORE": {
-        "nameTextMapHash": 2540376027
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_TITLE_NAME": {
-        "nameTextMapHash": 1385957482
-    },
-    "UI_ACTIVITY_LANV4_CARPJUMP_TRYAGAIN": {
-        "nameTextMapHash": 3593364823
-    },
-    "UI_ACTIVITY_LANV4_GAMEPLAY_PAGE_TIITLE": {
-        "nameTextMapHash": 4085935122
-    },
-    "UI_ACTIVITY_LANV4_KV_COIN": {
-        "nameTextMapHash": 683500425
-    },
-    "UI_ACTIVITY_LANV4_KV_GAMEPLAY_ENTRANCE": {
-        "nameTextMapHash": 2921776319
-    },
-    "UI_ACTIVITY_LANV4_KV_QUEST_ENTRANCE": {
-        "nameTextMapHash": 1259655773
-    },
-    "UI_ACTIVITY_LANV4_OPEN_HINT": {
-        "nameTextMapHash": 131322010
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_CANCEL_MATCH_DESC": {
-        "nameTextMapHash": 35193014
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_DRAFT_TIPS_DESC": {
-        "nameTextMapHash": 1453345675
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_DUNGEON_BAN_EXIT": {
-        "nameTextMapHash": 393705649
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_DUNGEON_EXIT_TIPS_DESC": {
-        "nameTextMapHash": 2279045489
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_ENDED": {
-        "nameTextMapHash": 2256929572
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_INSIDE_DODGE_FAIL": {
-        "nameTextMapHash": 4009587332
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_INSIDE_DODGE_SUCCESS": {
-        "nameTextMapHash": 2867496356
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_INSIDE_DODGE_WARNING": {
-        "nameTextMapHash": 1721826700
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LACKPLAYER": {
-        "nameTextMapHash": 2885127444
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LEVEL_FIRST": {
-        "nameTextMapHash": 3918173988
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LEVEL_FIRST_TAG": {
-        "nameTextMapHash": 762121381
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LEVEL_INSTRUCTION": {
-        "nameTextMapHash": 192676628
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LEVEL_REWARD": {
-        "nameTextMapHash": 3792136756
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LEVEL_SINGLE": {
-        "nameTextMapHash": 821548444
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LEVEL_STAGE_SCORE": {
-        "nameTextMapHash": 323949659
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LIMIT_DESC": {
-        "nameTextMapHash": 3223952720
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LIMIT_OPTION": {
-        "nameTextMapHash": 2479109400
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_LIMIT_TITLE": {
-        "nameTextMapHash": 3227644464
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MAIN_ADVANCE": {
-        "nameTextMapHash": 2946979023
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MAIN_CURRENT_SCORE": {
-        "nameTextMapHash": 2307093975
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MAIN_GOTO": {
-        "nameTextMapHash": 2341143855
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MAIN_PUSHTIPS": {
-        "nameTextMapHash": 2310846831
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MARKDESC": {
-        "nameTextMapHash": 3992587180
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MARKSCORE": {
-        "nameTextMapHash": 1807204084
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_MARKTITLE": {
-        "nameTextMapHash": 3860577156
-    },
-    "UI_ACTIVITY_LANV4_PARTYLION_TITLE_NAME": {
-        "nameTextMapHash": 2823417999
-    },
-    "UI_ACTIVITY_LANV4_PERFECT": {
-        "nameTextMapHash": 2644874383
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_EASYDESC": {
-        "nameTextMapHash": 2686112365
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_EASYHINT": {
-        "nameTextMapHash": 3264051957
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_EASYMODE": {
-        "nameTextMapHash": 1662686005
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_EASYTIME": {
-        "nameTextMapHash": 2697384613
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_EXIT": {
-        "nameTextMapHash": 644596781
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_LOAD": {
-        "nameTextMapHash": 2318056861
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_LOAD_DESC": {
-        "nameTextMapHash": 1946271151
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_LOAD_NULL": {
-        "nameTextMapHash": 4189555167
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_MARKDESC": {
-        "nameTextMapHash": 2799313029
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_MARKTITLE": {
-        "nameTextMapHash": 1567772885
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_MOVE": {
-        "nameTextMapHash": 4193507197
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_MOVEHINT": {
-        "nameTextMapHash": 2114019981
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_NAME": {
-        "nameTextMapHash": 3237116781
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_NEXT": {
-        "nameTextMapHash": 2038139181
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_RESET": {
-        "nameTextMapHash": 216275733
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_RESET_DESC": {
-        "nameTextMapHash": 560568401
-    },
-    "UI_ACTIVITY_LANV4_PUSHBOX_TITLE_NAME": {
-        "nameTextMapHash": 3825287940
-    },
-    "UI_ACTIVITY_LANV4_QUEST_PAGE_TIITLE": {
-        "nameTextMapHash": 468235287
-    },
-    "UI_ACTIVITY_LANV4_QUEST_SKIP_DESC": {
-        "nameTextMapHash": 755124314
-    },
-    "UI_ACTIVITY_LANV4_QUEST_SKIP_HINT": {
-        "nameTextMapHash": 358986138
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_AVATAR_BUTTON": {
-        "nameTextMapHash": 1402312414
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_AVATAR_COIN_INSUFFICIENT": {
-        "nameTextMapHash": 2780565272
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_AVATAR_CONFIRM_DESC": {
-        "nameTextMapHash": 79398243
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_AVATAR_DESC": {
-        "nameTextMapHash": 3648833822
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_AVATAR_FINISH_TIPS": {
-        "nameTextMapHash": 1201284150
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_AVATAR_TITLE": {
-        "nameTextMapHash": 1765171774
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_COIN_DESC": {
-        "nameTextMapHash": 1052165627
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_COIN_SHOW": {
-        "nameTextMapHash": 1201710563
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_COIN_TITLE": {
-        "nameTextMapHash": 3759666115
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_FASHION_BUTTON": {
-        "nameTextMapHash": 1344400244
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_FASHION_DESC": {
-        "nameTextMapHash": 2472899948
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_FASHION_NAME": {
-        "nameTextMapHash": 2936635508
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_FASHION_TITLE": {
-        "nameTextMapHash": 937224356
-    },
-    "UI_ACTIVITY_LANV4_REWARD_PAGE_TITLE": {
-        "nameTextMapHash": 883769395
-    },
     "UI_ACTIVITY_LEFT_TIME": {
         "nameTextMapHash": 648142500
     },
     "UI_ACTIVITY_LUNARITE_ATMOSPHERE": {
         "nameTextMapHash": 2179748151
     },
     "UI_ACTIVITY_LUNARITE_ATMOSPHERE_NEED": {
@@ -20764,14 +21757,17 @@
     },
     "UI_ACTIVITY_PRE_UNFINISHED_CHAPTER": {
         "nameTextMapHash": 638325841
     },
     "UI_ACTIVITY_PROGRESS": {
         "nameTextMapHash": 1808037176
     },
+    "UI_ACTIVITY_QUESTFINISHED": {
+        "nameTextMapHash": 3336191368
+    },
     "UI_ACTIVITY_QUEST_GET": {
         "nameTextMapHash": 840703104
     },
     "UI_ACTIVITY_QUEST_GOTO_BUTTON": {
         "nameTextMapHash": 881070039
     },
     "UI_ACTIVITY_QUEST_LOCK_TIPS": {
@@ -20821,20 +21817,14 @@
     },
     "UI_ACTIVITY_RECOMMEND_QUEST_TITLE": {
         "nameTextMapHash": 1784175890
     },
     "UI_ACTIVITY_RECORD_WORLDLEVEL": {
         "nameTextMapHash": 1734478321
     },
-    "UI_ACTIVITY_REGION_CHENYUVALLEY_DESC": {
-        "nameTextMapHash": 3249790222
-    },
-    "UI_ACTIVITY_REGION_CHENYUVALLEY_TITLE": {
-        "nameTextMapHash": 2442631046
-    },
     "UI_ACTIVITY_RETURN_STARTPOS": {
         "nameTextMapHash": 3764332598
     },
     "UI_ACTIVITY_REWARDPREVIEW": {
         "nameTextMapHash": 3652606681
     },
     "UI_ACTIVITY_REWARD_PREVIEW": {
@@ -21145,145 +22135,127 @@
     },
     "UI_ACTIVITY_SIGNIN_TABNAME_1001": {
         "nameTextMapHash": 643898299
     },
     "UI_ACTIVITY_SIGNIN_TABNAME_1002": {
         "nameTextMapHash": 86487771
     },
-    "UI_ACTIVITY_STAGE_LOCK": {
-        "nameTextMapHash": 2117355951
-    },
-    "UI_ACTIVITY_STAGE_UNLOCK_TIPS": {
-        "nameTextMapHash": 4057832592
-    },
-    "UI_ACTIVITY_STAMINAFIGHT_AVAILABLE_CHARACTER": {
-        "nameTextMapHash": 1101254091
-    },
-    "UI_ACTIVITY_STAMINAFIGHT_BATTLE_PROFILE": {
-        "nameTextMapHash": 461533774
+    "UI_ACTIVITY_SLIMECANNON_COMBO": {
+        "nameTextMapHash": 1917326769
     },
-    "UI_ACTIVITY_STAMINAFIGHT_BESTSCORE": {
-        "nameTextMapHash": 3081365049
+    "UI_ACTIVITY_SLIMECANNON_CONTINUE": {
+        "nameTextMapHash": 1673071713
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CHALLENGE_DIFFICULTY_CHOOSE": {
-        "nameTextMapHash": 107579814
+    "UI_ACTIVITY_SLIMECANNON_COUNTDOWN": {
+        "nameTextMapHash": 3125845753
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CHALLENGE_PREVIEW_CHARACTER": {
-        "nameTextMapHash": 2408971719
+    "UI_ACTIVITY_SLIMECANNON_ENDEXIT": {
+        "nameTextMapHash": 216410281
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CHALLENGE_PREVIEW_TITLE": {
-        "nameTextMapHash": 3843565519
+    "UI_ACTIVITY_SLIMECANNON_ENDQUEST": {
+        "nameTextMapHash": 2506457577
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CHOOSE_CHARACTER_EMPTY": {
-        "nameTextMapHash": 909566648
+    "UI_ACTIVITY_SLIMECANNON_ENDRESTART": {
+        "nameTextMapHash": 44684953
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CHOOSE_CHARACTER_FULL": {
-        "nameTextMapHash": 82814200
+    "UI_ACTIVITY_SLIMECANNON_ENDSCORE": {
+        "nameTextMapHash": 484651073
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CONFIRM_CHARACTER": {
-        "nameTextMapHash": 2827009648
+    "UI_ACTIVITY_SLIMECANNON_ENDSELECT": {
+        "nameTextMapHash": 522717649
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CONNECT": {
-        "nameTextMapHash": 3300543697
+    "UI_ACTIVITY_SLIMECANNON_EXIT": {
+        "nameTextMapHash": 2164402529
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CONTENT": {
-        "nameTextMapHash": 2903546569
+    "UI_ACTIVITY_SLIMECANNON_EXITTIPS": {
+        "nameTextMapHash": 429458449
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CURRENT_DANGEROUS_ENEMY": {
-        "nameTextMapHash": 3843830007
+    "UI_ACTIVITY_SLIMECANNON_INGAMESCORE": {
+        "nameTextMapHash": 4196138145
     },
-    "UI_ACTIVITY_STAMINAFIGHT_CURRENT_ROUND_CHOOSE": {
-        "nameTextMapHash": 3054110029
+    "UI_ACTIVITY_SLIMECANNON_LOCK_TIPS": {
+        "nameTextMapHash": 918540446
     },
-    "UI_ACTIVITY_STAMINAFIGHT_DENY_MULTI": {
-        "nameTextMapHash": 283684332
+    "UI_ACTIVITY_SLIMECANNON_MELT": {
+        "nameTextMapHash": 4143020625
     },
-    "UI_ACTIVITY_STAMINAFIGHT_DESC": {
-        "nameTextMapHash": 1748376185
+    "UI_ACTIVITY_SLIMECANNON_NEXTBULLET": {
+        "nameTextMapHash": 2738566633
     },
-    "UI_ACTIVITY_STAMINAFIGHT_DIFFICULTY_CONFIRM": {
-        "nameTextMapHash": 3495409904
+    "UI_ACTIVITY_SLIMECANNON_NOTOPSCORE": {
+        "nameTextMapHash": 3837132673
     },
-    "UI_ACTIVITY_STAMINAFIGHT_DIFFICULTY_HINT": {
-        "nameTextMapHash": 890928384
+    "UI_ACTIVITY_SLIMECANNON_OBJTITLE": {
+        "nameTextMapHash": 1275247689
     },
-    "UI_ACTIVITY_STAMINAFIGHT_DIFFICULTY_TIME": {
-        "nameTextMapHash": 1671479032
+    "UI_ACTIVITY_SLIMECANNON_OVERLOAD": {
+        "nameTextMapHash": 1149045881
     },
-    "UI_ACTIVITY_STAMINAFIGHT_EASY": {
-        "nameTextMapHash": 3030679369
+    "UI_ACTIVITY_SLIMECANNON_QUESTDONETIPS": {
+        "nameTextMapHash": 3178182753
     },
-    "UI_ACTIVITY_STAMINAFIGHT_ENEMYLEVEL": {
-        "nameTextMapHash": 3153018713
+    "UI_ACTIVITY_SLIMECANNON_RECORD01": {
+        "nameTextMapHash": 1056482113
     },
-    "UI_ACTIVITY_STAMINAFIGHT_EXTREME": {
-        "nameTextMapHash": 4136090089
+    "UI_ACTIVITY_SLIMECANNON_RECORD02": {
+        "nameTextMapHash": 3483724633
     },
-    "UI_ACTIVITY_STAMINAFIGHT_FAIL_TIPS": {
-        "nameTextMapHash": 1188506790
+    "UI_ACTIVITY_SLIMECANNON_RECORD03": {
+        "nameTextMapHash": 1072425737
     },
-    "UI_ACTIVITY_STAMINAFIGHT_FIRSTROUND": {
-        "nameTextMapHash": 1009667465
+    "UI_ACTIVITY_SLIMECANNON_RESTART": {
+        "nameTextMapHash": 1382055993
     },
-    "UI_ACTIVITY_STAMINAFIGHT_FIRST_ROUND_CHOOSE": {
-        "nameTextMapHash": 4129692673
+    "UI_ACTIVITY_SLIMECANNON_REWARDTITLE": {
+        "nameTextMapHash": 3353278849
     },
-    "UI_ACTIVITY_STAMINAFIGHT_FIRST_ROUND_PICKING": {
-        "nameTextMapHash": 2428310785
+    "UI_ACTIVITY_SLIMECANNON_SCORELEVEL": {
+        "nameTextMapHash": 1098266305
     },
-    "UI_ACTIVITY_STAMINAFIGHT_FOURTHROUND": {
-        "nameTextMapHash": 3570251393
+    "UI_ACTIVITY_SLIMECANNON_STAGELEVEL": {
+        "nameTextMapHash": 1516664113
     },
-    "UI_ACTIVITY_STAMINAFIGHT_HARD": {
-        "nameTextMapHash": 1812061129
+    "UI_ACTIVITY_SLIMECANNON_STAGELOCK": {
+        "nameTextMapHash": 3109245937
     },
-    "UI_ACTIVITY_STAMINAFIGHT_INSUFFICIENT_HINT": {
-        "nameTextMapHash": 588144921
+    "UI_ACTIVITY_SLIMECANNON_START": {
+        "nameTextMapHash": 25343361
     },
-    "UI_ACTIVITY_STAMINAFIGHT_MONSTER_PREVIEW": {
-        "nameTextMapHash": 2220989686
+    "UI_ACTIVITY_SLIMECANNON_STARTTIPS": {
+        "nameTextMapHash": 2923980185
     },
-    "UI_ACTIVITY_STAMINAFIGHT_NEXT_BATTLE": {
-        "nameTextMapHash": 2647200274
+    "UI_ACTIVITY_SLIMECANNON_SUCCEED": {
+        "nameTextMapHash": 2686730433
     },
-    "UI_ACTIVITY_STAMINAFIGHT_PICKING": {
-        "nameTextMapHash": 2065374233
+    "UI_ACTIVITY_SLIMECANNON_SUPERCONDUCT": {
+        "nameTextMapHash": 1548535665
     },
-    "UI_ACTIVITY_STAMINAFIGHT_QUIT_CONFIRM_NO_START": {
-        "nameTextMapHash": 107690597
+    "UI_ACTIVITY_SLIMECANNON_TITLE": {
+        "nameTextMapHash": 1740925465
     },
-    "UI_ACTIVITY_STAMINAFIGHT_RESTART_BTN": {
-        "nameTextMapHash": 3804338904
+    "UI_ACTIVITY_SLIMECANNON_TOPSCORE": {
+        "nameTextMapHash": 1211108505
     },
-    "UI_ACTIVITY_STAMINAFIGHT_RESTART_CURRENT_ROUND_BTN": {
-        "nameTextMapHash": 650923705
+    "UI_ACTIVITY_SLIMECANNON_TUTORIAL1": {
+        "nameTextMapHash": 2822265537
     },
-    "UI_ACTIVITY_STAMINAFIGHT_ROUNDS": {
-        "nameTextMapHash": 513238153
+    "UI_ACTIVITY_SLIMECANNON_TUTORIAL2": {
+        "nameTextMapHash": 1152467785
     },
-    "UI_ACTIVITY_STAMINAFIGHT_SECONDROUND": {
-        "nameTextMapHash": 2852923377
+    "UI_ACTIVITY_SLIMECANNON_TUTORIAL3": {
+        "nameTextMapHash": 1331950273
     },
-    "UI_ACTIVITY_STAMINAFIGHT_STAMINA_BUFF": {
-        "nameTextMapHash": 3029027006
+    "UI_ACTIVITY_SLIMECANNON_TUTORIALTITLE": {
+        "nameTextMapHash": 1243599433
     },
-    "UI_ACTIVITY_STAMINAFIGHT_THIRDROUND": {
-        "nameTextMapHash": 2991727233
-    },
-    "UI_ACTIVITY_STAMINAFIGHT_TIMELIMIT": {
-        "nameTextMapHash": 945102617
-    },
-    "UI_ACTIVITY_STAMINAFIGHT_TIRED": {
-        "nameTextMapHash": 1339532017
-    },
-    "UI_ACTIVITY_STAMINAFIGHT_TITLE": {
-        "nameTextMapHash": 370069313
+    "UI_ACTIVITY_STAGE_LOCK": {
+        "nameTextMapHash": 2117355951
     },
-    "UI_ACTIVITY_STAMINAFIGHT_TRY_AGAIN_TIPS": {
-        "nameTextMapHash": 3566602685
+    "UI_ACTIVITY_STAGE_UNLOCK_TIPS": {
+        "nameTextMapHash": 4057832592
     },
     "UI_ACTIVITY_STARTFAILED_ENDED": {
         "nameTextMapHash": 944188230
     },
     "UI_ACTIVITY_STARTFAILED_LACKPLAYER": {
         "nameTextMapHash": 2715013766
     },
@@ -23968,74 +24940,14 @@
     },
     "UI_AVATAR_TITLE": {
         "nameTextMapHash": 2022941172
     },
     "UI_AVATAR_WINGS": {
         "nameTextMapHash": 257286060
     },
-    "UI_Activity_LostSamachurlBoss_BestRecord": {
-        "nameTextMapHash": 1858887033
-    },
-    "UI_Activity_LostSamachurlBoss_Desc": {
-        "nameTextMapHash": 3319571729
-    },
-    "UI_Activity_LostSamachurlBoss_DungeonEntry": {
-        "nameTextMapHash": 1473935993
-    },
-    "UI_Activity_LostSamachurlBoss_OnlineFailHint": {
-        "nameTextMapHash": 2106763569
-    },
-    "UI_Activity_LostSamachurlBoss_RecordTime": {
-        "nameTextMapHash": 34446977
-    },
-    "UI_Activity_LostSamachurlBoss_Title": {
-        "nameTextMapHash": 45331329
-    },
-    "UI_Activity_LostSamachurlSneak_FailHint1": {
-        "nameTextMapHash": 1140309625
-    },
-    "UI_Activity_LostSamachurlSneak_FailHint2": {
-        "nameTextMapHash": 278837193
-    },
-    "UI_Activity_LostSamachurlSneak_FailHint3": {
-        "nameTextMapHash": 4269708089
-    },
-    "UI_Activity_LostSamachurlSneak_Guide_Statue": {
-        "nameTextMapHash": 829984983
-    },
-    "UI_Activity_LostSamachurlSneak_Guide_Turn": {
-        "nameTextMapHash": 3524592879
-    },
-    "UI_Activity_LostSamachurlSneak_InviteFailed": {
-        "nameTextMapHash": 166342441
-    },
-    "UI_Activity_LostSamachurlSneak_OnlineTips": {
-        "nameTextMapHash": 2812565273
-    },
-    "UI_Activity_LostSamachurlSneak_ReturnHint": {
-        "nameTextMapHash": 2350210729
-    },
-    "UI_Activity_LostSamachurlSneak_TimeoutHint": {
-        "nameTextMapHash": 2509765985
-    },
-    "UI_Activity_LostSamachurlSneak_UnlockTips": {
-        "nameTextMapHash": 2155754369
-    },
-    "UI_Activity_LostSamachurl_Sneak_ChallengeTime": {
-        "nameTextMapHash": 3063621407
-    },
-    "UI_Activity_LostSamachurl_Sneak_NoChallenge": {
-        "nameTextMapHash": 1388006151
-    },
-    "UI_Activity_LostSamachurl_Title": {
-        "nameTextMapHash": 3350154888
-    },
-    "UI_Activity_LostSamachurl_UnlockTips2": {
-        "nameTextMapHash": 1323738336
-    },
     "UI_BAN_MAP_TIPS": {
         "nameTextMapHash": 3349593108
     },
     "UI_BATTLEPASS_PAY_TIME_COUNT_DOWN": {
         "nameTextMapHash": 1464495449
     },
     "UI_BATTLEPASS_PAY_TIME_END": {
@@ -26089,14 +27001,20 @@
     },
     "UI_COOP_DEFEAT_TITLE": {
         "nameTextMapHash": 1973254400
     },
     "UI_COOP_ENDING_GOTO_POINT": {
         "nameTextMapHash": 886135188
     },
+    "UI_COOP_LOCK_COND_TIPS": {
+        "nameTextMapHash": 434215022
+    },
+    "UI_COOP_POINT_UNLOCK_TIPS": {
+        "nameTextMapHash": 1410230953
+    },
     "UI_COOP_SYSTEM_REMINDER_BUBBLE": {
         "nameTextMapHash": 459665732
     },
     "UI_COOP_SYSTEM_TITLE": {
         "nameTextMapHash": 2350622662
     },
     "UI_COOP_TASK_ABANDON_BUTTON": {
@@ -26488,14 +27406,20 @@
     },
     "UI_DUNGEON_ENTRY_1109": {
         "nameTextMapHash": 1111225651
     },
     "UI_DUNGEON_ENTRY_1142": {
         "nameTextMapHash": 1525986819
     },
+    "UI_DUNGEON_ENTRY_1202": {
+        "nameTextMapHash": 3024443467
+    },
+    "UI_DUNGEON_ENTRY_1207": {
+        "nameTextMapHash": 4122575003
+    },
     "UI_DUNGEON_ENTRY_20": {
         "nameTextMapHash": 1177628219
     },
     "UI_DUNGEON_ENTRY_22": {
         "nameTextMapHash": 3585043443
     },
     "UI_DUNGEON_ENTRY_221": {
@@ -28087,14 +29011,32 @@
     },
     "UI_GACHA_LIMIT_REACHED": {
         "nameTextMapHash": 1065172664
     },
     "UI_GACHA_LIMIT_SHORTAGE": {
         "nameTextMapHash": 2265021184
     },
+    "UI_GACHA_NATIONAL_BUTTON_01": {
+        "nameTextMapHash": 3140133105
+    },
+    "UI_GACHA_NATIONAL_BUTTON_02": {
+        "nameTextMapHash": 3467683553
+    },
+    "UI_GACHA_NATIONAL_NOTICE_AVATAR_UP": {
+        "nameTextMapHash": 1177308313
+    },
+    "UI_GACHA_NATIONAL_NOTICE_WEAPON_UP": {
+        "nameTextMapHash": 2355534386
+    },
+    "UI_GACHA_NATIONAL_SHOW_PANEL_DETAIL_01": {
+        "nameTextMapHash": 3254850949
+    },
+    "UI_GACHA_NATIONAL_SHOW_PANEL_DETAIL_02": {
+        "nameTextMapHash": 3385460237
+    },
     "UI_GACHA_NEWBIE_DISCOUNT": {
         "nameTextMapHash": 986506778
     },
     "UI_GACHA_NEXT": {
         "nameTextMapHash": 2015840295
     },
     "UI_GACHA_PAGE_BUTTON_WISH": {
@@ -28276,14 +29218,17 @@
     },
     "UI_GACHA_SHOW_PANEL_A016_UP1_NAME": {
         "nameTextMapHash": 164926567
     },
     "UI_GACHA_SHOW_PANEL_A016_UP1_TITLE": {
         "nameTextMapHash": 2282930487
     },
+    "UI_GACHA_SHOW_PANEL_A0175_TITLE": {
+        "nameTextMapHash": 3719929892
+    },
     "UI_GACHA_SHOW_PANEL_A017_SUBTITLE": {
         "nameTextMapHash": 3455385674
     },
     "UI_GACHA_SHOW_PANEL_A017_TITLE": {
         "nameTextMapHash": 1175962018
     },
     "UI_GACHA_SHOW_PANEL_A017_UP1_NAME1": {
@@ -28603,14 +29548,17 @@
     },
     "UI_GACHA_SHOW_PANEL_A097_TITLE": {
         "nameTextMapHash": 686079202
     },
     "UI_GACHA_SHOW_PANEL_ALL_TYPE": {
         "nameTextMapHash": 619915093
     },
+    "UI_GACHA_SHOW_PANEL_B001_TITLE": {
+        "nameTextMapHash": 1278682412
+    },
     "UI_GACHA_SHOW_PANEL_DETAIL_00": {
         "nameTextMapHash": 759095825
     },
     "UI_GACHA_SHOW_PANEL_DETAIL_01": {
         "nameTextMapHash": 992785265
     },
     "UI_GACHA_SHOW_PANEL_DETAIL_02": {
@@ -28669,14 +29617,17 @@
     },
     "UI_GACHA_TYPE_04": {
         "nameTextMapHash": 2864268523
     },
     "UI_GACHA_TYPE_05": {
         "nameTextMapHash": 3352513147
     },
+    "UI_GACHA_TYPE_06": {
+        "nameTextMapHash": 2563094019
+    },
     "UI_GACHA_UNDERAGE_LIMIT": {
         "nameTextMapHash": 1037698853
     },
     "UI_GACHA_UNDERAGE_LIMIT_REACHED": {
         "nameTextMapHash": 3810705373
     },
     "UI_GACHA_UNDERAGE_LIMIT_SHORTAGE": {
@@ -28684,14 +29635,59 @@
     },
     "UI_GACHA_UNDERAGE_TODAY_TIMES": {
         "nameTextMapHash": 205565985
     },
     "UI_GACHA_WISH": {
         "nameTextMapHash": 2176913927
     },
+    "UI_GACHA_WISH_02": {
+        "nameTextMapHash": 203061159
+    },
+    "UI_GACHA_WISH_02_AVATAR": {
+        "nameTextMapHash": 2354162523
+    },
+    "UI_GACHA_WISH_02_AVATAR_UP": {
+        "nameTextMapHash": 450888899
+    },
+    "UI_GACHA_WISH_02_BUTTON_01": {
+        "nameTextMapHash": 2683000493
+    },
+    "UI_GACHA_WISH_02_CHECK_DETAILS": {
+        "nameTextMapHash": 3731203764
+    },
+    "UI_GACHA_WISH_02_CURRENT_CHOOSE": {
+        "nameTextMapHash": 4072542893
+    },
+    "UI_GACHA_WISH_02_DESC": {
+        "nameTextMapHash": 3807102715
+    },
+    "UI_GACHA_WISH_02_DETAIL": {
+        "nameTextMapHash": 1052429219
+    },
+    "UI_GACHA_WISH_02_NOTICE_01": {
+        "nameTextMapHash": 634346145
+    },
+    "UI_GACHA_WISH_02_NOTICE_02": {
+        "nameTextMapHash": 1079564521
+    },
+    "UI_GACHA_WISH_02_NOTICE_03": {
+        "nameTextMapHash": 4132271441
+    },
+    "UI_GACHA_WISH_02_POINT": {
+        "nameTextMapHash": 3025797203
+    },
+    "UI_GACHA_WISH_02_TITLE": {
+        "nameTextMapHash": 2731236947
+    },
+    "UI_GACHA_WISH_02_WEAPON": {
+        "nameTextMapHash": 2362736755
+    },
+    "UI_GACHA_WISH_02_WEAPON_UP": {
+        "nameTextMapHash": 3859474477
+    },
     "UI_GACHA_WISH_DESC": {
         "nameTextMapHash": 187682631
     },
     "UI_GACHA_WISH_POINT": {
         "nameTextMapHash": 2169238279
     },
     "UI_GADGETINTERACT_TEXT1": {
@@ -33466,14 +34462,32 @@
     },
     "UI_HOMEWORLD_CANCEL_CHOOSE_ONE": {
         "nameTextMapHash": 2945308152
     },
     "UI_HOMEWORLD_CANT_OPEN_EDITOR_AVATAR": {
         "nameTextMapHash": 2013224790
     },
+    "UI_HOMEWORLD_CAT_BUTTON": {
+        "nameTextMapHash": 3698952649
+    },
+    "UI_HOMEWORLD_CAT_CHANGECAT_TAB": {
+        "nameTextMapHash": 1477216511
+    },
+    "UI_HOMEWORLD_CAT_CHOOSECAT_TITLE": {
+        "nameTextMapHash": 1986095334
+    },
+    "UI_HOMEWORLD_CAT_NOCATS_TIPS": {
+        "nameTextMapHash": 3857409401
+    },
+    "UI_HOMEWORLD_CAT_PLAYQUIT_BLACK": {
+        "nameTextMapHash": 2370632744
+    },
+    "UI_HOMEWORLD_CAT_PLAY_TOUCH": {
+        "nameTextMapHash": 1959657171
+    },
     "UI_HOMEWORLD_CHANGEBGM_ALLOW_UNLOCK_REMIND": {
         "nameTextMapHash": 216514544
     },
     "UI_HOMEWORLD_CHANGEBGM_CONTROLLER_AUDITION_BUTTON": {
         "nameTextMapHash": 1413709416
     },
     "UI_HOMEWORLD_CHANGEBGM_CONTROLLER_LEAVE_BUTTON": {
@@ -36544,14 +37558,17 @@
     },
     "UI_MAP_AREA40_TITLE_4": {
         "nameTextMapHash": 278963228
     },
     "UI_MAP_AREA40_TITLE_5": {
         "nameTextMapHash": 1727468580
     },
+    "UI_MAP_AREA40_TITLE_6": {
+        "nameTextMapHash": 354861716
+    },
     "UI_MAP_AREA41_TITLE_1": {
         "nameTextMapHash": 2134194813
     },
     "UI_MAP_AREA41_TITLE_2": {
         "nameTextMapHash": 1915423749
     },
     "UI_MAP_AREA41_TITLE_3": {
@@ -36631,14 +37648,17 @@
     },
     "UI_MAP_AREA6_TITLE_6": {
         "nameTextMapHash": 1590757389
     },
     "UI_MAP_AREA6_TITLE_7": {
         "nameTextMapHash": 3034482533
     },
+    "UI_MAP_AREA6_TITLE_8": {
+        "nameTextMapHash": 1590696557
+    },
     "UI_MAP_AREA7_TITLE_1": {
         "nameTextMapHash": 1348018420
     },
     "UI_MAP_AREA7_TITLE_2": {
         "nameTextMapHash": 4038355020
     },
     "UI_MAP_AREA7_TITLE_3": {
@@ -39064,14 +40084,20 @@
     },
     "UI_QUEST_FINISHWQ": {
         "nameTextMapHash": 1900071618
     },
     "UI_QUEST_GODDESSLOCKED": {
         "nameTextMapHash": 1161309330
     },
+    "UI_QUEST_Guide_To_Layer": {
+        "nameTextMapHash": 4262858181
+    },
+    "UI_QUEST_Guide_To_Layer_Hint": {
+        "nameTextMapHash": 3759187128
+    },
     "UI_QUEST_IN_AREA": {
         "nameTextMapHash": 92877145
     },
     "UI_QUEST_IN_MIRROREDBIGWORLD_TIPS": {
         "nameTextMapHash": 1243994784
     },
     "UI_QUEST_LEVELCOND": {
@@ -39145,14 +40171,38 @@
     },
     "UI_QUEST_UNAVAILABLE": {
         "nameTextMapHash": 3969335770
     },
     "UI_QUEST_UNCLAIMED": {
         "nameTextMapHash": 21877282
     },
+    "UI_QuestCheck_AdditionTittle": {
+        "nameTextMapHash": 867444798
+    },
+    "UI_QuestCheck_CardDrawButton_PS": {
+        "nameTextMapHash": 3180830625
+    },
+    "UI_QuestCheck_CardDrawTips": {
+        "nameTextMapHash": 1009668726
+    },
+    "UI_QuestCheck_CloseTips": {
+        "nameTextMapHash": 2262921278
+    },
+    "UI_QuestCheck_FailTips": {
+        "nameTextMapHash": 3890824366
+    },
+    "UI_QuestCheck_MainTittleName": {
+        "nameTextMapHash": 774483030
+    },
+    "UI_QuestCheck_RuleExplain": {
+        "nameTextMapHash": 1838487678
+    },
+    "UI_QuestCheck_SuccessTips": {
+        "nameTextMapHash": 797606734
+    },
     "UI_RACING_NEWRECORD": {
         "nameTextMapHash": 1727146555
     },
     "UI_RACING_TIMESPENT": {
         "nameTextMapHash": 4063423715
     },
     "UI_RANDOM_FACTOR": {
@@ -39697,14 +40747,17 @@
     },
     "UI_ROUTINE_REWARD": {
         "nameTextMapHash": 247640290
     },
     "UI_RTT_MS": {
         "nameTextMapHash": 3304234625
     },
+    "UI_RandNumIndicator_Interact_Draw": {
+        "nameTextMapHash": 3304064944
+    },
     "UI_Rechallenge_Desc": {
         "nameTextMapHash": 628037445
     },
     "UI_Rechallenge_Remark": {
         "nameTextMapHash": 1583881837
     },
     "UI_Rechallenge_Title": {
@@ -40837,20 +41890,26 @@
     },
     "UI_SCENE_ENTRY_ENTER_CHATEAU": {
         "nameTextMapHash": 2815777616
     },
     "UI_SCENE_ENTRY_ENTER_CHURCH": {
         "nameTextMapHash": 2488849224
     },
+    "UI_SCENE_ENTRY_ENTER_CatCafe": {
+        "nameTextMapHash": 2449332256
+    },
     "UI_SCENE_ENTRY_ENTER_CattailTavern": {
         "nameTextMapHash": 1973039687
     },
     "UI_SCENE_ENTRY_ENTER_Chagongfang": {
         "nameTextMapHash": 4253315296
     },
+    "UI_SCENE_ENTRY_ENTER_ChioriRoom": {
+        "nameTextMapHash": 243574256
+    },
     "UI_SCENE_ENTRY_ENTER_Chunzhangjia": {
         "nameTextMapHash": 55084384
     },
     "UI_SCENE_ENTRY_ENTER_Coffeehouse": {
         "nameTextMapHash": 2272663336
     },
     "UI_SCENE_ENTRY_ENTER_Csd": {
@@ -40927,20 +41986,26 @@
     },
     "UI_SCENE_ENTRY_EXIT_CHATEAU": {
         "nameTextMapHash": 2700645941
     },
     "UI_SCENE_ENTRY_EXIT_CHURCH": {
         "nameTextMapHash": 3182591029
     },
+    "UI_SCENE_ENTRY_EXIT_CatCafe": {
+        "nameTextMapHash": 1745663109
+    },
     "UI_SCENE_ENTRY_EXIT_CattailTavern": {
         "nameTextMapHash": 3941042764
     },
     "UI_SCENE_ENTRY_EXIT_Chagongfang": {
         "nameTextMapHash": 2264749869
     },
+    "UI_SCENE_ENTRY_EXIT_ChioriRoom": {
+        "nameTextMapHash": 2218668957
+    },
     "UI_SCENE_ENTRY_EXIT_Chunzhangjia": {
         "nameTextMapHash": 1431632885
     },
     "UI_SCENE_ENTRY_EXIT_Coffeehouse": {
         "nameTextMapHash": 268983437
     },
     "UI_SCENE_ENTRY_EXIT_Csd": {
@@ -41908,14 +42973,17 @@
     },
     "UI_SKILL_PREVIEW": {
         "nameTextMapHash": 605718139
     },
     "UI_SKILL_UPGRADE_NEED": {
         "nameTextMapHash": 265448998
     },
+    "UI_SKILL_UPGRADE_NEXT_LEVEL_NEED": {
+        "nameTextMapHash": 2762030786
+    },
     "UI_SKILL_UPGRADE_PROP_CHANGE": {
         "nameTextMapHash": 171268013
     },
     "UI_SKILL_UPGRADE_PROP_UNLOCK": {
         "nameTextMapHash": 1224574709
     },
     "UI_SKILL_UPGRADE_REMINDER": {
@@ -43195,14 +44263,269 @@
     },
     "UI_TOWER_WIN_NEXT_INFO": {
         "nameTextMapHash": 703502488
     },
     "UI_TOYS_MIRACLERING": {
         "nameTextMapHash": 886625471
     },
+    "UI_TRAININGGUIDE_AVATARLEVEL": {
+        "nameTextMapHash": 1433650698
+    },
+    "UI_TRAININGGUIDE_AVATARLEVEL_FINISH": {
+        "nameTextMapHash": 1692052302
+    },
+    "UI_TRAININGGUIDE_AVATARLEVEL_LEVELBREAK_TITLE": {
+        "nameTextMapHash": 4093117499
+    },
+    "UI_TRAININGGUIDE_AVATARLEVEL_LEVELBREAK_TITLE_2": {
+        "nameTextMapHash": 2918732704
+    },
+    "UI_TRAININGGUIDE_AVATARLEVEL_LEVELUP_TITLE": {
+        "nameTextMapHash": 2138370568
+    },
+    "UI_TRAININGGUIDE_AVATARLEVEL_LEVELUP_TITLE_2": {
+        "nameTextMapHash": 459875339
+    },
+    "UI_TRAININGGUIDE_BLUETIP_ENTRY": {
+        "nameTextMapHash": 2193574529
+    },
+    "UI_TRAININGGUIDE_BLUETIP_ENTRY_FIRSTTIME": {
+        "nameTextMapHash": 2594472736
+    },
+    "UI_TRAININGGUIDE_BLUETIP_LEVELUP": {
+        "nameTextMapHash": 1365034105
+    },
+    "UI_TRAININGGUIDE_BLUETIP_MENU": {
+        "nameTextMapHash": 1419918417
+    },
+    "UI_TRAININGGUIDE_BLUETIP_MENU_FIRSTTIME": {
+        "nameTextMapHash": 748511507
+    },
+    "UI_TRAININGGUIDE_EMPTY": {
+        "nameTextMapHash": 3269668098
+    },
+    "UI_TRAININGGUIDE_ENTRY_TIP": {
+        "nameTextMapHash": 1809660311
+    },
+    "UI_TRAININGGUIDE_FAIL_TIP": {
+        "nameTextMapHash": 1505664154
+    },
+    "UI_TRAININGGUIDE_MATERIAL_LACK_TIP": {
+        "nameTextMapHash": 2871914952
+    },
+    "UI_TRAININGGUIDE_NODATA": {
+        "nameTextMapHash": 2641855762
+    },
+    "UI_TRAININGGUIDE_OTHER": {
+        "nameTextMapHash": 724785018
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_MEMBER_IMPROVE": {
+        "nameTextMapHash": 3997968643
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_MEMBER_STATISTIC_HIGH": {
+        "nameTextMapHash": 881518202
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_MEMBER_STATISTIC_LOW": {
+        "nameTextMapHash": 77925834
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_MEMBER_STATISTIC_MEDIUM": {
+        "nameTextMapHash": 973052138
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_MEMBER_STATISTIC_TITLE": {
+        "nameTextMapHash": 4135270810
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_OTHER": {
+        "nameTextMapHash": 2998895879
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_PARTY_MEMBER_STATISTIC_TITLE": {
+        "nameTextMapHash": 4084926260
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_PARTY_STATISTIC_HIGH": {
+        "nameTextMapHash": 326382843
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_PARTY_STATISTIC_LOW": {
+        "nameTextMapHash": 547967747
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_PARTY_STATISTIC_MEDIUM": {
+        "nameTextMapHash": 38754939
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_PARTY_STATISTIC_TITLE": {
+        "nameTextMapHash": 3434506451
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_RULE_DESC": {
+        "nameTextMapHash": 3164178491
+    },
+    "UI_TRAININGGUIDE_OVERVIEW_WORLDLEVEL": {
+        "nameTextMapHash": 2479125431
+    },
+    "UI_TRAININGGUIDE_RECOMMEND_UNKNOWN": {
+        "nameTextMapHash": 3963058643
+    },
+    "UI_TRAININGGUIDE_RELIQUARY": {
+        "nameTextMapHash": 156274666
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_EQUIP_TIP": {
+        "nameTextMapHash": 3202532341
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_EQUIP_TITLE": {
+        "nameTextMapHash": 47414317
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_FINISH": {
+        "nameTextMapHash": 3804347976
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_GOAL": {
+        "nameTextMapHash": 1044048648
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_NEW": {
+        "nameTextMapHash": 3405924640
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_NODATA": {
+        "nameTextMapHash": 2154204232
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_PLAN1": {
+        "nameTextMapHash": 1970187560
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_PLAN2": {
+        "nameTextMapHash": 2290075224
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_PLAN3": {
+        "nameTextMapHash": 1993738264
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_QUALITY_1": {
+        "nameTextMapHash": 1489927012
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_QUALITY_2": {
+        "nameTextMapHash": 3741294844
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_QUALITY_3": {
+        "nameTextMapHash": 15232684
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_QUALITY_4": {
+        "nameTextMapHash": 1704470988
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_QUALITY_5": {
+        "nameTextMapHash": 4241690388
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_RECOMMEND": {
+        "nameTextMapHash": 772901288
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_TIP": {
+        "nameTextMapHash": 1495140856
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_TITLE": {
+        "nameTextMapHash": 1994897136
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_TITLE1": {
+        "nameTextMapHash": 2737526920
+    },
+    "UI_TRAININGGUIDE_RELIQUARY_TITLE2": {
+        "nameTextMapHash": 2476434664
+    },
+    "UI_TRAININGGUIDE_REWARD_RESOURCE": {
+        "nameTextMapHash": 3011157390
+    },
+    "UI_TRAININGGUIDE_SOURCE_ALCHEMY_TIP": {
+        "nameTextMapHash": 3377815014
+    },
+    "UI_TRAININGGUIDE_SOURCE_BLOSSON_TIP": {
+        "nameTextMapHash": 4148704350
+    },
+    "UI_TRAININGGUIDE_SOURCE_BOSS_ANY_TIP": {
+        "nameTextMapHash": 1493990555
+    },
+    "UI_TRAININGGUIDE_SOURCE_BOSS_TIP": {
+        "nameTextMapHash": 4281009596
+    },
+    "UI_TRAININGGUIDE_SOURCE_DUNGEON_TIP": {
+        "nameTextMapHash": 1909730384
+    },
+    "UI_TRAININGGUIDE_SOURCE_WEAPON_ORE_TIP": {
+        "nameTextMapHash": 1191493553
+    },
+    "UI_TRAININGGUIDE_STAMINA_TIP": {
+        "nameTextMapHash": 1544233825
+    },
+    "UI_TRAININGGUIDE_TALENT": {
+        "nameTextMapHash": 2200092034
+    },
+    "UI_TRAININGGUIDE_TALENT_FINISH": {
+        "nameTextMapHash": 2624000958
+    },
+    "UI_TRAININGGUIDE_TALENT_LEVELUP_TITLE": {
+        "nameTextMapHash": 3204556918
+    },
+    "UI_TRAININGGUIDE_TALENT_LEVELUP_TITLE_2": {
+        "nameTextMapHash": 3133322338
+    },
+    "UI_TRAININGGUIDE_TALENT_PRIORITY_HIGH": {
+        "nameTextMapHash": 570302140
+    },
+    "UI_TRAININGGUIDE_TALENT_PRIORITY_LOW": {
+        "nameTextMapHash": 2562017868
+    },
+    "UI_TRAININGGUIDE_TALENT_PRIORITY_MID": {
+        "nameTextMapHash": 558319492
+    },
+    "UI_TRAININGGUIDE_TALENT_TITLE": {
+        "nameTextMapHash": 1152735174
+    },
+    "UI_TRAININGGUIDE_TITLE": {
+        "nameTextMapHash": 3569108122
+    },
+    "UI_TRAININGGUIDE_WEAPON": {
+        "nameTextMapHash": 4156109530
+    },
+    "UI_TRAININGGUIDE_WEAPON_FINISH": {
+        "nameTextMapHash": 1306544230
+    },
+    "UI_TRAININGGUIDE_WEAPON_LEVELBREAK_TIP": {
+        "nameTextMapHash": 3252587379
+    },
+    "UI_TRAININGGUIDE_WEAPON_LEVELBREAK_TITLE": {
+        "nameTextMapHash": 1563756339
+    },
+    "UI_TRAININGGUIDE_WEAPON_LEVELBREAK_TITLE_2": {
+        "nameTextMapHash": 2101229144
+    },
+    "UI_TRAININGGUIDE_WEAPON_LEVELUP_TITLE": {
+        "nameTextMapHash": 2054448684
+    },
+    "UI_TRAININGGUIDE_WEAPON_LEVELUP_TITLE_2": {
+        "nameTextMapHash": 683160426
+    },
+    "UI_TRAININGGUIDE_WEAPON_LEVEL_TITLE": {
+        "nameTextMapHash": 1643220111
+    },
+    "UI_TRAININGGUIDE_WEAPON_RECOMMEND_FORGE": {
+        "nameTextMapHash": 3273097682
+    },
+    "UI_TRAININGGUIDE_WEAPON_RECOMMEND_NAME": {
+        "nameTextMapHash": 159873314
+    },
+    "UI_TRAININGGUIDE_WEAPON_RECOMMEND_NODATA": {
+        "nameTextMapHash": 2360413042
+    },
+    "UI_TRAININGGUIDE_WEAPON_RECOMMEND_OCCUPY": {
+        "nameTextMapHash": 1410377490
+    },
+    "UI_TRAININGGUIDE_WEAPON_RECOMMEND_TIP": {
+        "nameTextMapHash": 3107010674
+    },
+    "UI_TRAININGGUIDE_WEAPON_RECOMMEND_TITLE": {
+        "nameTextMapHash": 3289230026
+    },
+    "UI_TRAININGGUIDE_WEAPON_USE_RATE_HIGH": {
+        "nameTextMapHash": 3647343381
+    },
+    "UI_TRAININGGUIDE_WEAPON_USE_RATE_LOW": {
+        "nameTextMapHash": 78588725
+    },
+    "UI_TRAININGGUIDE_WEAPON_USE_RATE_MEDIUN": {
+        "nameTextMapHash": 2345765733
+    },
     "UI_TRANSPORT_ENTRY_UNLOCK_CONDITION": {
         "nameTextMapHash": 2327958170
     },
     "UI_UGC_ADJUST_VISIBILITY": {
         "nameTextMapHash": 913062161
     },
     "UI_UGC_AUTHOR_NAME": {
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/namecards.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/namecards.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894736842105263%*

 * *Differences: {"'210193'": "OrderedDict([('nameTextMapHash', 3292114052), ('icon', 'UI_NameCardIcon_Chiori'), "*

 * *             "('picPath', ['UI_NameCardPic_Chiori_Alpha', 'UI_NameCardPic_Chiori_P']), "*

 * *             "('rankLevel', 4), ('materialType', 'MATERIAL_NAMECARD')])",*

 * * "'210194'": "OrderedDict([('nameTextMapHash', 882758588), ('icon', 'UI_NameCardIcon_Bp31'), "*

 * *             "('picPath', ['UI_NameCardPic_Bp31_Alpha', 'UI_NameCardPic_Bp31_P']), ('rankLevel', "*

 * *             "4), ('materialType', 'MATERIAL_NAMECARD')]) […]*

```diff
@@ -1874,9 +1874,29 @@
         "materialType": "MATERIAL_NAMECARD",
         "nameTextMapHash": 1212836964,
         "picPath": [
             "UI_NameCardPic_OST4_Alpha",
             "UI_NameCardPic_OST4_P"
         ],
         "rankLevel": 4
+    },
+    "210193": {
+        "icon": "UI_NameCardIcon_Chiori",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 3292114052,
+        "picPath": [
+            "UI_NameCardPic_Chiori_Alpha",
+            "UI_NameCardPic_Chiori_P"
+        ],
+        "rankLevel": 4
+    },
+    "210194": {
+        "icon": "UI_NameCardIcon_Bp31",
+        "materialType": "MATERIAL_NAMECARD",
+        "nameTextMapHash": 882758588,
+        "picPath": [
+            "UI_NameCardPic_Bp31_Alpha",
+            "UI_NameCardPic_Bp31_P"
+        ],
+        "rankLevel": 4
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/skills.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/skills.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.987274220032841%*

 * *Differences: {"'10941'": "OrderedDict([('nameTextMapHash', 914798901), ('skillIcon', 'Skill_A_01'), "*

 * *            "('proudSkillGroupId', 9431)])",*

 * * "'10942'": "OrderedDict([('nameTextMapHash', 2315821309), ('skillIcon', 'Skill_S_Chiori_01'), "*

 * *            "('proudSkillGroupId', 9432)])",*

 * * "'10944'": "OrderedDict([('nameTextMapHash', 2873692477), ('skillIcon', 'Skill_S_Chiori_03'), "*

 * *            "('proudSkillGroupId', '')])",*

 * * "'10945'": "OrderedDict([('nameTextMapHash', 373425821), ('skillIcon', 'Skill_E_Chiori_01'), "*

 * * […]*

```diff
@@ -1935,14 +1935,34 @@
         "skillIcon": "Skill_S_Liuyun_03"
     },
     "10937": {
         "nameTextMapHash": 2928796237,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_S_Liuyun_05"
     },
+    "10941": {
+        "nameTextMapHash": 914798901,
+        "proudSkillGroupId": 9431,
+        "skillIcon": "Skill_A_01"
+    },
+    "10942": {
+        "nameTextMapHash": 2315821309,
+        "proudSkillGroupId": 9432,
+        "skillIcon": "Skill_S_Chiori_01"
+    },
+    "10944": {
+        "nameTextMapHash": 2873692477,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_S_Chiori_03"
+    },
+    "10945": {
+        "nameTextMapHash": 373425821,
+        "proudSkillGroupId": 9439,
+        "skillIcon": "Skill_E_Chiori_01"
+    },
     "11301": {
         "nameTextMapHash": 3802462781,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_02"
     },
     "11302": {
         "nameTextMapHash": 2467360621,
@@ -2195,14 +2215,24 @@
         "skillIcon": "Skill_LanV4PartyLion_01"
     },
     "20084": {
         "nameTextMapHash": 682415765,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_LanV4PartyLion_01"
     },
+    "20093": {
+        "nameTextMapHash": 3906587141,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_SlimeCannon_Fire_01"
+    },
+    "20094": {
+        "nameTextMapHash": 2428119293,
+        "proudSkillGroupId": "",
+        "skillIcon": "Btn_SlimeCannon_Fire_04"
+    },
     "20100": {
         "nameTextMapHash": 4176490093,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Seeker_A_01"
     },
     "20101": {
         "nameTextMapHash": 2129541325,
@@ -2413,60 +2443,60 @@
         "nameTextMapHash": 2209588093,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_Recon_Bait"
     },
     "20400": {
         "nameTextMapHash": 2657714069,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Seeker_A_01"
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_S"
     },
     "20401": {
         "nameTextMapHash": 66214933,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Seeker_A_01"
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_S"
     },
     "20410": {
         "nameTextMapHash": 169502221,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Seeker_S_01"
     },
     "20411": {
         "nameTextMapHash": 1752388581,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Seeker_S_02"
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_A_02"
     },
     "20420": {
         "nameTextMapHash": 816489501,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Seeker_E_01"
     },
     "20421": {
         "nameTextMapHash": 1050865533,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Seeker_E_02"
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_E_02"
     },
     "20422": {
         "nameTextMapHash": 2689008917,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Seeker_E_03"
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_E_01"
     },
     "20500": {
         "nameTextMapHash": 902040061,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Hider_A_01"
     },
     "20501": {
         "nameTextMapHash": 1233705669,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Hider_A_03"
     },
     "20510": {
         "nameTextMapHash": 2713313077,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Hider_S_01"
+        "skillIcon": "Btn_HideAndSeekV4_Hider_A_01"
     },
     "20511": {
         "nameTextMapHash": 1882966981,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Hider_S_02"
     },
     "20512": {
@@ -2478,35 +2508,35 @@
         "nameTextMapHash": 1833806357,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Hider_S_02_Borbid"
     },
     "20520": {
         "nameTextMapHash": 2680677653,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Hider_E_01"
+        "skillIcon": "Btn_HideAndSeekV4_Hider_E"
     },
     "20521": {
         "nameTextMapHash": 2973812453,
         "proudSkillGroupId": "",
         "skillIcon": "UI_Icon_Skill_Hunter_Net"
     },
     "20522": {
         "nameTextMapHash": 3495989125,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Hider_S_02"
     },
     "20523": {
         "nameTextMapHash": 2450340517,
         "proudSkillGroupId": "",
-        "skillIcon": "UI_Icon_Skill_Prey_Invisible_Bait"
+        "skillIcon": "Btn_HideAndSeekV4_Hider_A_02"
     },
     "20524": {
         "nameTextMapHash": 1356540013,
         "proudSkillGroupId": "",
-        "skillIcon": "Btn_HideAndSeek_Seeker_S_01"
+        "skillIcon": "Btn_HideAndSeekV4_Seeker_A_01"
     },
     "20525": {
         "nameTextMapHash": 3710444509,
         "proudSkillGroupId": "",
         "skillIcon": "Btn_HideAndSeek_Hider_A_01"
     },
     "20526": {
@@ -3004,9 +3034,14 @@
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_04"
     },
     "5093010": {
         "nameTextMapHash": 345620165,
         "proudSkillGroupId": "",
         "skillIcon": "Skill_A_Catalyst_MD"
+    },
+    "5094010": {
+        "nameTextMapHash": 331992085,
+        "proudSkillGroupId": "",
+        "skillIcon": "Skill_A_01"
     }
 }
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/data/weapons.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/data/weapons.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9905660377358491%*

 * *Differences: {"'11514'": "OrderedDict([('nameTextMapHash', 1818340435), ('icon', 'UI_EquipIcon_Sword_Needle'), "*

 * *            "('awakenIcon', 'UI_EquipIcon_Sword_Needle_Awaken'), ('rankLevel', 5)])",*

 * * "'13426'": "OrderedDict([('nameTextMapHash', 2847771107), ('icon', 'UI_EquipIcon_Pole_Caduceus'), "*

 * *            "('awakenIcon', 'UI_EquipIcon_Pole_Caduceus_Awaken'), ('rankLevel', 4)])"}*

```diff
@@ -325,14 +325,20 @@
     },
     "11513": {
         "awakenIcon": "UI_EquipIcon_Sword_Regalis_Awaken",
         "icon": "UI_EquipIcon_Sword_Regalis",
         "nameTextMapHash": 1473399443,
         "rankLevel": 5
     },
+    "11514": {
+        "awakenIcon": "UI_EquipIcon_Sword_Needle_Awaken",
+        "icon": "UI_EquipIcon_Sword_Needle",
+        "nameTextMapHash": 1818340435,
+        "rankLevel": 5
+    },
     "12101": {
         "awakenIcon": "UI_EquipIcon_Claymore_Aniki_Awaken",
         "icon": "UI_EquipIcon_Claymore_Aniki",
         "nameTextMapHash": 2666951267,
         "rankLevel": 1
     },
     "12201": {
@@ -697,14 +703,20 @@
     },
     "13425": {
         "awakenIcon": "UI_EquipIcon_Pole_Vorpal_Awaken",
         "icon": "UI_EquipIcon_Pole_Vorpal",
         "nameTextMapHash": 4158971171,
         "rankLevel": 4
     },
+    "13426": {
+        "awakenIcon": "UI_EquipIcon_Pole_Caduceus_Awaken",
+        "icon": "UI_EquipIcon_Pole_Caduceus",
+        "nameTextMapHash": 2847771107,
+        "rankLevel": 4
+    },
     "13427": {
         "awakenIcon": "UI_EquipIcon_Pole_Mechanic_Awaken",
         "icon": "UI_EquipIcon_Pole_Mechanic",
         "nameTextMapHash": 882305891,
         "rankLevel": 4
     },
     "13501": {
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/artifact_sets.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/artifact_sets.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9900891972249752%*

 * *Differences: {"'1092884699'": "OrderedDict([('CHS', '均衡的原理'), ('DE', 'Prinzip des Gleichgewichts'), ('EN', "*

 * *                 "'Principle of Equilibrium'), ('ES', 'Ley del equilibrio'), ('FR', "*

 * *                 '"Principe de l\'équilibre"), (\'ID\', \'Principle of Equilibrium\'), (\'IT\', '*

 * *                 '"Principio dell\'Equilibrio"), (\'JP\', \'均衡の原理\'), (\'KR\', \'균형 원리\'), '*

 * *                 "('PT', 'Princípio do Equilíbrio'), ('RU', 'Принцип равновесия'), ('TH', "*

 * *                 "'Principle of Equilibrium'),  […]*

```diff
@@ -347,14 +347,30 @@
         "KR": "\u300c\uc815\uc758\u300d",
         "PT": "Justi\u00e7a",
         "RU": "\u0421\u043f\u0440\u0430\u0432\u0435\u0434\u043b\u0438\u0432\u043e\u0441\u0442\u044c",
         "TH": "Justice",
         "TR": "Adalet",
         "VI": "Ch\u00ednh Ngh\u0129a"
     },
+    "1092884699": {
+        "CHS": "\u5747\u8861\u7684\u539f\u7406",
+        "DE": "Prinzip des Gleichgewichts",
+        "EN": "Principle of Equilibrium",
+        "ES": "Ley del equilibrio",
+        "FR": "Principe de l'\u00e9quilibre",
+        "ID": "Principle of Equilibrium",
+        "IT": "Principio dell'Equilibrio",
+        "JP": "\u5747\u8861\u306e\u539f\u7406",
+        "KR": "\uade0\ud615 \uc6d0\ub9ac",
+        "PT": "Princ\u00edpio do Equil\u00edbrio",
+        "RU": "\u041f\u0440\u0438\u043d\u0446\u0438\u043f \u0440\u0430\u0432\u043d\u043e\u0432\u0435\u0441\u0438\u044f",
+        "TH": "Principle of Equilibrium",
+        "TR": "Denge \u0130lkesi",
+        "VI": "Nguy\u00ean L\u00fd C\u00e2n B\u1eb1ng"
+    },
     "1097898243": {
         "CHS": "\u6c89\u91cd",
         "DE": "Schwergewicht",
         "EN": "Heavy",
         "ES": "Pesado",
         "FR": "\u00c9crasement",
         "ID": "Heavy",
@@ -539,14 +555,30 @@
         "KR": "\uc6a9\uc790\uc758 \uac80",
         "PT": "Espada do Her\u00f3i",
         "RU": "\u041c\u0435\u0447 \u0433\u0435\u0440\u043e\u044f",
         "TH": "Hero's Blade",
         "TR": "Kahraman\u0131n K\u0131l\u0131c\u0131",
         "VI": "L\u01b0\u1ee1i Ki\u1ebfm Anh H\u00f9ng"
     },
+    "1132036667": {
+        "CHS": "\u5747\u8861\u7684\u539f\u7406",
+        "DE": "Prinzip des Gleichgewichts",
+        "EN": "Principle of Equilibrium",
+        "ES": "Ley del equilibrio",
+        "FR": "Principe de l'\u00e9quilibre",
+        "ID": "Principle of Equilibrium",
+        "IT": "Principio dell'Equilibrio",
+        "JP": "\u5747\u8861\u306e\u539f\u7406",
+        "KR": "\uade0\ud615 \uc6d0\ub9ac",
+        "PT": "Princ\u00edpio do Equil\u00edbrio",
+        "RU": "\u041f\u0440\u0438\u043d\u0446\u0438\u043f \u0440\u0430\u0432\u043d\u043e\u0432\u0435\u0441\u0438\u044f",
+        "TH": "Principle of Equilibrium",
+        "TR": "Denge \u0130lkesi",
+        "VI": "Nguy\u00ean L\u00fd C\u00e2n B\u1eb1ng"
+    },
     "1133599347": {
         "CHS": "\u77e2\u5fd7\u4e0d\u5fd8",
         "DE": "Willensstarker Pfeil",
         "EN": "Strong-Willed",
         "ES": "Flecha imparable",
         "FR": "Fl\u00e8che de la volont\u00e9",
         "ID": "Strong-willed Arrow",
@@ -1595,14 +1627,30 @@
         "KR": "\ubaa8\ub798 \uc704 \ub204\uac01",
         "PT": "Pavilh\u00e3o do Deserto",
         "RU": "\u0427\u0435\u0440\u0442\u043e\u0433\u0438 \u0432 \u043f\u0443\u0441\u0442\u044b\u043d\u0435",
         "TH": "Desert Pavilion",
         "TR": "\u00c7\u00f6l Kona\u011f\u0131",
         "VI": "\u0110\u00ecnh \u0110\u00e0i Tr\u00ean C\u00e1t"
     },
+    "1391705475": {
+        "CHS": "\u9526\u4e4b\u82b1\u4e0e\u9f9b\u4e2d\u5251",
+        "DE": "Die Blume im Brokat und das Schwert im Schrein",
+        "EN": "Brocade Bloom, Shrine Sword",
+        "ES": "Flor bordada y espada consagrada",
+        "FR": "Fleur brod\u00e9e et \u00e9p\u00e9e consacr\u00e9e",
+        "ID": "Brocade Bloom, Shrine Sword",
+        "IT": "Broccato in fiore, Spada del santuario",
+        "JP": "\u9326\u306e\u82b1\u3068\u5c0f\u7960\u306e\u5200",
+        "KR": "\ube44\ub2e8 \uaf43\uacfc \uac10\uc2e4 \uac80",
+        "PT": "Brocado Florescente, Espada do Santu\u00e1rio",
+        "RU": "\u041f\u0430\u0440\u0447\u043e\u0432\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0438 \u043c\u0435\u0447 \u0441\u0432\u044f\u0442\u0438\u043b\u0438\u0449\u0430",
+        "TH": "Brocade Bloom, Shrine Sword",
+        "TR": "S\u0131rmal\u0131 \u00c7i\u00e7ek ve Tap\u0131nak K\u0131l\u0131c\u0131",
+        "VI": "Hoa Th\u1ed5 C\u1ea9m V\u00e0 Ki\u1ebfm \u0110\u1ec1n Th\u1edd"
+    },
     "1394994395": {
         "CHS": "\u971c\u846c",
         "DE": "Frostgrab",
         "EN": "Frost Burial",
         "ES": "Entierro helado",
         "FR": "Deuil givr\u00e9",
         "ID": "Frost Burial",
@@ -2187,14 +2235,30 @@
         "KR": "\uc720\ubc30\uc790",
         "PT": "O Exilado",
         "RU": "\u0418\u0437\u0433\u043d\u0430\u043d\u043d\u0438\u043a",
         "TH": "The Exile",
         "TR": "S\u00fcrg\u00fcn",
         "VI": "K\u1ebb L\u01b0u \u0110\u00e0y"
     },
+    "1520322691": {
+        "CHS": "\u9526\u4e4b\u82b1\u4e0e\u9f9b\u4e2d\u5251",
+        "DE": "Die Blume im Brokat und das Schwert im Schrein",
+        "EN": "Brocade Bloom, Shrine Sword",
+        "ES": "Flor bordada y espada consagrada",
+        "FR": "Fleur brod\u00e9e et \u00e9p\u00e9e consacr\u00e9e",
+        "ID": "Brocade Bloom, Shrine Sword",
+        "IT": "Broccato in fiore, Spada del santuario",
+        "JP": "\u9326\u306e\u82b1\u3068\u5c0f\u7960\u306e\u5200",
+        "KR": "\ube44\ub2e8 \uaf43\uacfc \uac10\uc2e4 \uac80",
+        "PT": "Brocado Florescente, Espada do Santu\u00e1rio",
+        "RU": "\u041f\u0430\u0440\u0447\u043e\u0432\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0438 \u043c\u0435\u0447 \u0441\u0432\u044f\u0442\u0438\u043b\u0438\u0449\u0430",
+        "TH": "Brocade Bloom, Shrine Sword",
+        "TR": "S\u0131rmal\u0131 \u00c7i\u00e7ek ve Tap\u0131nak K\u0131l\u0131c\u0131",
+        "VI": "Hoa Th\u1ed5 C\u1ea9m V\u00e0 Ki\u1ebfm \u0110\u1ec1n Th\u1edd"
+    },
     "1522029867": {
         "CHS": "\u8e0f\u706b\u606f\u96f7",
         "DE": "Bew\u00e4hrtheit von Feuer und Blitz",
         "EN": "Bane of Fire and Thunder",
         "ES": "Perdici\u00f3n del fuego y el trueno",
         "FR": "Fl\u00e9au de feu et de foudre",
         "ID": "Bane of Fire and Thunder",
@@ -4539,14 +4603,30 @@
         "KR": "\uc9d1\uc911",
         "PT": "Foco",
         "RU": "\u0421\u043e\u0441\u0440\u0435\u0434\u043e\u0442\u043e\u0447\u0435\u043d\u043d\u044b\u0439",
         "TH": "Focus",
         "TR": "Odaklanma",
         "VI": "Chuy\u00ean Ch\u00fa"
     },
+    "2109946579": {
+        "CHS": "\u9526\u4e4b\u82b1\u4e0e\u9f9b\u4e2d\u5251",
+        "DE": "Die Blume im Brokat und das Schwert im Schrein",
+        "EN": "Brocade Bloom, Shrine Sword",
+        "ES": "Flor bordada y espada consagrada",
+        "FR": "Fleur brod\u00e9e et \u00e9p\u00e9e consacr\u00e9e",
+        "ID": "Brocade Bloom, Shrine Sword",
+        "IT": "Broccato in fiore, Spada del santuario",
+        "JP": "\u9326\u306e\u82b1\u3068\u5c0f\u7960\u306e\u5200",
+        "KR": "\ube44\ub2e8 \uaf43\uacfc \uac10\uc2e4 \uac80",
+        "PT": "Brocado Florescente, Espada do Santu\u00e1rio",
+        "RU": "\u041f\u0430\u0440\u0447\u043e\u0432\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0438 \u043c\u0435\u0447 \u0441\u0432\u044f\u0442\u0438\u043b\u0438\u0449\u0430",
+        "TH": "Brocade Bloom, Shrine Sword",
+        "TR": "S\u0131rmal\u0131 \u00c7i\u00e7ek ve Tap\u0131nak K\u0131l\u0131c\u0131",
+        "VI": "Hoa Th\u1ed5 C\u1ea9m V\u00e0 Ki\u1ebfm \u0110\u1ec1n Th\u1edd"
+    },
     "2111115387": {
         "CHS": "\u51b3\u5fc3",
         "DE": "Zielstrebigkeit",
         "EN": "Determination",
         "ES": "Resoluci\u00f3n",
         "FR": "D\u00e9termination",
         "ID": "Determination",
@@ -7051,14 +7131,30 @@
         "KR": "\ubb34\uc808(\u9727\u5207) \uc5b4\uac80",
         "PT": "Bainha Quebra-nuvens",
         "RU": "\u041b\u0435\u0437\u0432\u0438\u0435 \u0440\u0430\u0441\u0441\u0435\u043a\u0430\u0442\u0435\u043b\u044f \u0442\u0443\u043c\u0430\u043d\u0430",
         "TH": "Mistsplitter's Edge",
         "TR": "Siskesen K\u0131l\u0131\u00e7 K\u0131n\u0131",
         "VI": "Linh V\u1eadt C\u1eaft S\u01b0\u01a1ng"
     },
+    "2682729115": {
+        "CHS": "\u5747\u8861\u7684\u539f\u7406",
+        "DE": "Prinzip des Gleichgewichts",
+        "EN": "Principle of Equilibrium",
+        "ES": "Ley del equilibrio",
+        "FR": "Principe de l'\u00e9quilibre",
+        "ID": "Principle of Equilibrium",
+        "IT": "Principio dell'Equilibrio",
+        "JP": "\u5747\u8861\u306e\u539f\u7406",
+        "KR": "\uade0\ud615 \uc6d0\ub9ac",
+        "PT": "Princ\u00edpio do Equil\u00edbrio",
+        "RU": "\u041f\u0440\u0438\u043d\u0446\u0438\u043f \u0440\u0430\u0432\u043d\u043e\u0432\u0435\u0441\u0438\u044f",
+        "TH": "Principle of Equilibrium",
+        "TR": "Denge \u0130lkesi",
+        "VI": "Nguy\u00ean L\u00fd C\u00e2n B\u1eb1ng"
+    },
     "2684365579": {
         "CHS": "\u767b\u573a\u4e50",
         "DE": "Ouvert\u00fcre",
         "EN": "Debut",
         "ES": "Debut",
         "FR": "Musique d'ouverture",
         "ID": "Debut",
@@ -12379,14 +12475,30 @@
         "KR": "\uc9d1\uc911",
         "PT": "Foco",
         "RU": "\u0421\u043e\u0441\u0440\u0435\u0434\u043e\u0442\u043e\u0447\u0435\u043d\u043d\u044b\u0439",
         "TH": "Focus",
         "TR": "Odaklanma",
         "VI": "Chuy\u00ean Ch\u00fa"
     },
+    "4019696531": {
+        "CHS": "\u5747\u8861\u7684\u539f\u7406",
+        "DE": "Prinzip des Gleichgewichts",
+        "EN": "Principle of Equilibrium",
+        "ES": "Ley del equilibrio",
+        "FR": "Principe de l'\u00e9quilibre",
+        "ID": "Principle of Equilibrium",
+        "IT": "Principio dell'Equilibrio",
+        "JP": "\u5747\u8861\u306e\u539f\u7406",
+        "KR": "\uade0\ud615 \uc6d0\ub9ac",
+        "PT": "Princ\u00edpio do Equil\u00edbrio",
+        "RU": "\u041f\u0440\u0438\u043d\u0446\u0438\u043f \u0440\u0430\u0432\u043d\u043e\u0432\u0435\u0441\u0438\u044f",
+        "TH": "Principle of Equilibrium",
+        "TR": "Denge \u0130lkesi",
+        "VI": "Nguy\u00ean L\u00fd C\u00e2n B\u1eb1ng"
+    },
     "4022012131": {
         "CHS": "\u4e58\u80dc\u8ffd\u51fb",
         "DE": "Triumphaler \u00dcbermut",
         "EN": "Press the Advantage",
         "ES": "Victoria tras victoria",
         "FR": "De victoire en victoire",
         "ID": "Press the Advantage",
@@ -12891,14 +13003,30 @@
         "KR": "\uc9c1\uc124",
         "PT": "Convencer",
         "RU": "\u0413\u043e\u0432\u043e\u0440\u0438 \u043a\u0430\u043a \u0435\u0441\u0442\u044c",
         "TH": "Blunt Conclusion",
         "TR": "Kesin Sonu\u00e7",
         "VI": "L\u1eddi N\u00f3i Th\u1eb3ng Th\u1eafn"
     },
+    "413367035": {
+        "CHS": "\u9526\u4e4b\u82b1\u4e0e\u9f9b\u4e2d\u5251",
+        "DE": "Die Blume im Brokat und das Schwert im Schrein",
+        "EN": "Brocade Bloom, Shrine Sword",
+        "ES": "Flor bordada y espada consagrada",
+        "FR": "Fleur brod\u00e9e et \u00e9p\u00e9e consacr\u00e9e",
+        "ID": "Brocade Bloom, Shrine Sword",
+        "IT": "Broccato in fiore, Spada del santuario",
+        "JP": "\u9326\u306e\u82b1\u3068\u5c0f\u7960\u306e\u5200",
+        "KR": "\ube44\ub2e8 \uaf43\uacfc \uac10\uc2e4 \uac80",
+        "PT": "Brocado Florescente, Espada do Santu\u00e1rio",
+        "RU": "\u041f\u0430\u0440\u0447\u043e\u0432\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0438 \u043c\u0435\u0447 \u0441\u0432\u044f\u0442\u0438\u043b\u0438\u0449\u0430",
+        "TH": "Brocade Bloom, Shrine Sword",
+        "TR": "S\u0131rmal\u0131 \u00c7i\u00e7ek ve Tap\u0131nak K\u0131l\u0131c\u0131",
+        "VI": "Hoa Th\u1ed5 C\u1ea9m V\u00e0 Ki\u1ebfm \u0110\u1ec1n Th\u1edd"
+    },
     "4134324539": {
         "CHS": "\u5143\u7d20\u719f\u7ec3",
         "DE": "Meister der Elemente",
         "EN": "Elemental Mastery",
         "ES": "Maestr\u00eda Elemental",
         "FR": "Maestria \u00e9l\u00e9mentaire",
         "ID": "Elemental Mastery",
@@ -14603,14 +14731,30 @@
         "KR": "\uc2e0\ube44\ud55c \uc9c0\ud61c\uc758 \uc740\ucd1d",
         "PT": "Favor da Sabedoria Secreta",
         "RU": "\u0411\u043b\u0430\u0433\u043e\u0432\u043e\u043b\u0435\u043d\u0438\u0435 \u0442\u0430\u0439\u043d\u043e\u0439 \u043c\u0443\u0434\u0440\u043e\u0441\u0442\u0438",
         "TH": "Secret Wisdom's Favor",
         "TR": "Sakl\u0131 Bilgeli\u011fin L\u00fctfu",
         "VI": "\u00c2n Hu\u1ec7 C\u1ee7a Con Ng\u01b0\u01a1i Tr\u00ed Tu\u1ec7"
     },
+    "651127963": {
+        "CHS": "\u5747\u8861\u7684\u539f\u7406",
+        "DE": "Prinzip des Gleichgewichts",
+        "EN": "Principle of Equilibrium",
+        "ES": "Ley del equilibrio",
+        "FR": "Principe de l'\u00e9quilibre",
+        "ID": "Principle of Equilibrium",
+        "IT": "Principio dell'Equilibrio",
+        "JP": "\u5747\u8861\u306e\u539f\u7406",
+        "KR": "\uade0\ud615 \uc6d0\ub9ac",
+        "PT": "Princ\u00edpio do Equil\u00edbrio",
+        "RU": "\u041f\u0440\u0438\u043d\u0446\u0438\u043f \u0440\u0430\u0432\u043d\u043e\u0432\u0435\u0441\u0438\u044f",
+        "TH": "Principle of Equilibrium",
+        "TR": "Denge \u0130lkesi",
+        "VI": "Nguy\u00ean L\u00fd C\u00e2n B\u1eb1ng"
+    },
     "651784635": {
         "CHS": "\u514b\u67d4",
         "DE": "Weicher Schlag",
         "EN": "Bane of the Soft",
         "ES": "Antipegajoso",
         "FR": "Anti-Blob",
         "ID": "Hard Hitter",
@@ -15147,14 +15291,30 @@
         "KR": "\ud48d\uc694\ub85c\uc6b4 \uafc8\uc758 \uaecd\ub370\uae30",
         "PT": "Casca de Sonhos Opulentos",
         "RU": "\u041a\u043e\u043a\u043e\u043d \u0441\u043b\u0430\u0434\u043a\u0438\u0445 \u0433\u0440\u0451\u0437",
         "TH": "Husk of Opulent Dreams",
         "TR": "Bereketli R\u00fcyalar\u0131n Hat\u0131ralar\u0131",
         "VI": "Gi\u1ea5c M\u1ed9ng Ph\u00f9 Hoa"
     },
+    "801463315": {
+        "CHS": "\u9526\u4e4b\u82b1\u4e0e\u9f9b\u4e2d\u5251",
+        "DE": "Die Blume im Brokat und das Schwert im Schrein",
+        "EN": "Brocade Bloom, Shrine Sword",
+        "ES": "Flor bordada y espada consagrada",
+        "FR": "Fleur brod\u00e9e et \u00e9p\u00e9e consacr\u00e9e",
+        "ID": "Brocade Bloom, Shrine Sword",
+        "IT": "Broccato in fiore, Spada del santuario",
+        "JP": "\u9326\u306e\u82b1\u3068\u5c0f\u7960\u306e\u5200",
+        "KR": "\ube44\ub2e8 \uaf43\uacfc \uac10\uc2e4 \uac80",
+        "PT": "Brocado Florescente, Espada do Santu\u00e1rio",
+        "RU": "\u041f\u0430\u0440\u0447\u043e\u0432\u044b\u0439 \u0446\u0432\u0435\u0442\u043e\u043a \u0438 \u043c\u0435\u0447 \u0441\u0432\u044f\u0442\u0438\u043b\u0438\u0449\u0430",
+        "TH": "Brocade Bloom, Shrine Sword",
+        "TR": "S\u0131rmal\u0131 \u00c7i\u00e7ek ve Tap\u0131nak K\u0131l\u0131c\u0131",
+        "VI": "Hoa Th\u1ed5 C\u1ea9m V\u00e0 Ki\u1ebfm \u0110\u1ec1n Th\u1edd"
+    },
     "802457699": {
         "CHS": "",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/artifacts.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/artifacts.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999364191251272%*

 * *Differences: {"'1942586956'": "{'CHS': '黄金时代的先声', 'DE': 'Ouvertüre zum Goldenen Zeitalter', 'EN': "*

 * *                 '"Golden Era\'s Prelude", \'ES\': \'Preludio de la Era Dorada\', \'FR\': "Prélude '*

 * *                 'de l\'ère dorée", \'ID\': "Golden Era\'s Prelude", \'IT\': "Preludio dell\'Era '*

 * *                 'dorata", \'JP\': \'黄金の時代の前兆\', \'KR\': \'황금 시대의 서곡\', \'PT\': \'Abertura da Era '*

 * *                 'Dourada\', \'RU\': \'Предзнаменование золотой эпохи\', \'TH\': "Golden Era\'s '*

 * *                 'Prelude", […]*

```diff
@@ -15692,28 +15692,28 @@
         "PT": "Esperan\u00e7a do Gladiador",
         "RU": "\u0421\u0442\u0440\u0435\u043c\u043b\u0435\u043d\u0438\u0435 \u0433\u043b\u0430\u0434\u0438\u0430\u0442\u043e\u0440\u0430",
         "TH": "Gladiator's Longing",
         "TR": "Gladyat\u00f6r\u00fcn \u00d6zlemi",
         "VI": "Hy V\u1ecdng C\u1ee7a Gi\u00e1c \u0110\u1ea5u S\u0129"
     },
     "1942586956": {
-        "CHS": "\u9ec4\u91d1\u4e50\u66f2\u7684\u53d8\u594f",
-        "DE": "Variation der Goldpartitur",
-        "EN": "Golden Song's Variation",
-        "ES": "Variaci\u00f3n de la Serenata Dorada",
-        "FR": "Variation de la m\u00e9lodie dor\u00e9e",
-        "ID": "Golden Song's Variation",
-        "IT": "Variazione della Canzone dorata",
-        "JP": "\u9ec4\u91d1\u306e\u65cb\u5f8b\u306e\u5909\u594f",
-        "KR": "\ud669\uae08 \uc74c\uc545\uc758 \ubcc0\uc8fc",
-        "PT": "Varia\u00e7\u00e3o da Composi\u00e7\u00e3o Dourada",
-        "RU": "\u0412\u0430\u0440\u0438\u0430\u0446\u0438\u044f \u0437\u043e\u043b\u043e\u0442\u043e\u0439 \u043f\u0435\u0441\u043d\u0438",
-        "TH": "Golden Song's Variation",
-        "TR": "Alt\u0131n \u015eark\u0131 \u00c7e\u015fitlemesi",
-        "VI": "Bi\u1ebfn T\u1ea5u Kh\u00fac Nh\u1ea1c Ho\u00e0ng Kim"
+        "CHS": "\u9ec4\u91d1\u65f6\u4ee3\u7684\u5148\u58f0",
+        "DE": "Ouvert\u00fcre zum Goldenen Zeitalter",
+        "EN": "Golden Era's Prelude",
+        "ES": "Preludio de la Era Dorada",
+        "FR": "Pr\u00e9lude de l'\u00e8re dor\u00e9e",
+        "ID": "Golden Era's Prelude",
+        "IT": "Preludio dell'Era dorata",
+        "JP": "\u9ec4\u91d1\u306e\u6642\u4ee3\u306e\u524d\u5146",
+        "KR": "\ud669\uae08 \uc2dc\ub300\uc758 \uc11c\uace1",
+        "PT": "Abertura da Era Dourada",
+        "RU": "\u041f\u0440\u0435\u0434\u0437\u043d\u0430\u043c\u0435\u043d\u043e\u0432\u0430\u043d\u0438\u0435 \u0437\u043e\u043b\u043e\u0442\u043e\u0439 \u044d\u043f\u043e\u0445\u0438",
+        "TH": "Golden Era's Prelude",
+        "TR": "Alt\u0131n \u00c7a\u011f\u0131n Ba\u015flang\u0131c\u0131",
+        "VI": "Kh\u00fac D\u1ea1o \u0110\u1ea7u Th\u1eddi K\u1ef3 Ho\u00e0ng Kim"
     },
     "1943148676": {
         "CHS": "\u661f\u7f57\u572d\u74a7\u4e4b\u6677",
         "DE": "Sonnenuhr der d\u00fcsteren Jade",
         "EN": "Sundial of Enduring Jade",
         "ES": "Reloj de Sol de Jade Sempiterno",
         "FR": "Cadran du jade immuable",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/characters.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/characters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9876543209876543%*

 * *Differences: {"'1944606922'": "OrderedDict([('CHS', '千织'), ('DE', 'Chiori'), ('EN', 'Chiori'), ('ES', "*

 * *                 "'Chiori'), ('FR', 'Chiori'), ('ID', 'Chiori'), ('IT', 'Chiori'), ('JP', '千織'), "*

 * *                 "('KR', '치오리'), ('PT', 'Chiori'), ('RU', 'Тиори'), ('TH', 'Chiori'), ('TR', "*

 * *                 "'Chiori'), ('VI', 'Chiori')])"}*

```diff
@@ -299,14 +299,30 @@
         "KR": "\ud638\ub450",
         "PT": "Hutao",
         "RU": "\u0425\u0443 \u0422\u0430\u043e",
         "TH": "Hu Tao",
         "TR": "Hu Tao",
         "VI": "Hu Tao"
     },
+    "1944606922": {
+        "CHS": "\u5343\u7ec7",
+        "DE": "Chiori",
+        "EN": "Chiori",
+        "ES": "Chiori",
+        "FR": "Chiori",
+        "ID": "Chiori",
+        "IT": "Chiori",
+        "JP": "\u5343\u7e54",
+        "KR": "\uce58\uc624\ub9ac",
+        "PT": "Chiori",
+        "RU": "\u0422\u0438\u043e\u0440\u0438",
+        "TH": "Chiori",
+        "TR": "Chiori",
+        "VI": "Chiori"
+    },
     "1966438658": {
         "CHS": "\u5b89\u67cf",
         "DE": "Amber",
         "EN": "Amber",
         "ES": "Amber",
         "FR": "Amber",
         "ID": "Amber",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/constellations.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/constellations.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880243764172336%*

 * *Differences: {"'167855529'": "OrderedDict([('CHS', '绫羽二重'), ('DE', 'Zwei seidene Federn'), ('EN', 'Two Silken "*

 * *                "Plumules'), ('ES', 'Seda habutai'), ('FR', 'Deux plumules de satin'), ('ID', 'Two "*

 * *                "Silken Plumules'), ('IT', 'Due piume seriche'), ('JP', '綾羽二重'), ('KR', '이중 능직'), "*

 * *                "('PT', 'Duas Plumas de Seda'), ('RU', 'Два шёлковых пера'), ('TH', 'Two Silken "*

 * *                "Plumules'), ('TR', 'İki İpek Filizi'), ('VI', 'Hai Tầng Trang Phục')])",*

 * * "'2112971153'": "Ordere […]*

```diff
@@ -1355,14 +1355,30 @@
         "KR": "\uc544\uacc4(\u6211\u754c)",
         "PT": "Meu Mundo",
         "RU": "\u0413\u0440\u0435\u0445 \u0433\u043e\u0440\u0434\u044b\u043d\u0438",
         "TH": "Sin of Pride",
         "TR": "Kibir",
         "VI": "B\u1ea3n Ng\u00e3"
     },
+    "167855529": {
+        "CHS": "\u7eeb\u7fbd\u4e8c\u91cd",
+        "DE": "Zwei seidene Federn",
+        "EN": "Two Silken Plumules",
+        "ES": "Seda habutai",
+        "FR": "Deux plumules de satin",
+        "ID": "Two Silken Plumules",
+        "IT": "Due piume seriche",
+        "JP": "\u7dbe\u7fbd\u4e8c\u91cd",
+        "KR": "\uc774\uc911 \ub2a5\uc9c1",
+        "PT": "Duas Plumas de Seda",
+        "RU": "\u0414\u0432\u0430 \u0448\u0451\u043b\u043a\u043e\u0432\u044b\u0445 \u043f\u0435\u0440\u0430",
+        "TH": "Two Silken Plumules",
+        "TR": "\u0130ki \u0130pek Filizi",
+        "VI": "Hai T\u1ea7ng Trang Ph\u1ee5c"
+    },
     "168010785": {
         "CHS": "\u771f\u706b\u70bc\u5b9d\u5370",
         "DE": "Siegel in lodernder Flamme",
         "EN": "Samadhi Fire-Forged",
         "ES": "Sello p\u00edrico del samadhi",
         "FR": "Mise sous scell\u00e9s",
         "ID": "Samadhi Fire-Forged",
@@ -2235,14 +2251,30 @@
         "KR": "\ub178\ub825\uc774 \uace7 \ub9c8\ubc95",
         "PT": "A Aten\u00e7\u00e3o \u00e9 o Meu Poder",
         "RU": "\u041c\u0430\u0433\u0438\u044f \u0443\u0441\u0435\u0440\u0434\u0438\u044f",
         "TH": "Attentiveness be My Power",
         "TR": "\u00c7al\u0131\u015fkanl\u0131\u011f\u0131n B\u00fcy\u00fcs\u00fc",
         "VI": "N\u1ed7 L\u1ef1c L\u00e0 Ma Thu\u1eadt"
     },
+    "2112971153": {
+        "CHS": "\u843d\u67d3\u4e94\u8272",
+        "DE": "F\u00fcnffarbige F\u00e4rbung",
+        "EN": "In Five Colors Dyed",
+        "ES": "Tintura pol\u00edcroma",
+        "FR": "Cinq couleurs de la teinture",
+        "ID": "In Five Colors Dyed",
+        "IT": "In cinque colori",
+        "JP": "\u843d\u67d3\u4e94\u8272",
+        "KR": "\uc624\uc0c9 \uc5fc\uc0c9",
+        "PT": "Em Cinco Cores Tingidas",
+        "RU": "\u041f\u044f\u0442\u044c \u0446\u0432\u0435\u0442\u043e\u0432 \u0442\u043a\u0430\u043d\u0438",
+        "TH": "In Five Colors Dyed",
+        "TR": "Be\u015f Renk Boya",
+        "VI": "N\u0103m M\u00e0u Thu\u1ed1c Nhu\u1ed9m"
+    },
     "2128995113": {
         "CHS": "\u7089\u706b\u4e0e\u6b22\u7b11\u4e4b\u591c",
         "DE": "N\u00e4chte voll behaglichem Herdfeuer und Fr\u00f6hlichkeit",
         "EN": "Nights of Hearth and Happiness",
         "ES": "Noche de hogueras y j\u00fabilo",
         "FR": "Nuit de feu et de joie",
         "ID": "Nights of Hearth and Happiness",
@@ -3457,15 +3489,15 @@
     },
     "2696040833": {
         "CHS": "\u5e84\u8c10\u5e76\u4e3e",
         "DE": "Gemeinsame Unternehmung",
         "EN": "Decorous Harmony",
         "ES": "Armon\u00eda y decoro",
         "FR": "Harmonie esth\u00e9tique",
-        "ID": "Hiasan yang Harmonis",
+        "ID": "Decorous Harmony",
         "IT": "Armonia e decoro",
         "JP": "\u8358\u8ae7\u4f75\u6301",
         "KR": "\uc7a5\uc5c4\ud558\uace0 \uc775\uc0b4\uc2a4\ub7ec\uc6b4 \ub178\ub7ab\uc18c\ub9ac",
         "PT": "Harmonia e Decoro",
         "RU": "\u0413\u0430\u0440\u043c\u043e\u043d\u0438\u0447\u043d\u043e\u0435 \u0440\u0430\u0437\u0432\u0438\u0442\u0438\u0435",
         "TH": "Decorous Harmony",
         "TR": "Zarif Bir Ahenk",
@@ -4867,15 +4899,15 @@
         "CHS": "\u6df7\u5143\u71b5\u589e\u8bba",
         "DE": "Chaotische Entropie",
         "EN": "Chaotic Entropy",
         "ES": "Entrop\u00eda ca\u00f3tica",
         "FR": "Th\u00e9orie de l'entropie",
         "ID": "Chaotic Entropy",
         "IT": "Entropia caotica",
-        "JP": "\u6df7\u5143\u71b5\u589e\u8ad6",
+        "JP": "\u6df7\u5143\u71b5\u5897\u8ad6",
         "KR": "\ud63c\ub3c8\uc758 \uc5d4\ud2b8\ub85c\ud53c",
         "PT": "Entropia Ca\u00f3tica",
         "RU": "\u042d\u043d\u0442\u0440\u043e\u043f\u0438\u044f \u0445\u0430\u043e\u0441\u0430",
         "TH": "Chaotic Entropy",
         "TR": "Entropi Yasas\u0131",
         "VI": "Thuy\u1ebft H\u1ed7n Lo\u1ea1n"
     },
@@ -7147,14 +7179,30 @@
         "KR": "\uce60\uc131\uc758 \uc544\ub984\ub2f5\uace0 \ucc2c\ub780\ud55c \ube5b",
         "PT": "Grandiosas sejam as Sete Estrelas",
         "RU": "\u0413\u0440\u0430\u043d\u0434\u0438\u043e\u0437\u043d\u043e\u0441\u0442\u044c \u0426\u0438\u0441\u0438\u043d",
         "TH": "Grandeur be the Seven Stars",
         "TR": "Yedi Y\u0131ld\u0131z\u0131n \u0130hti\u015fam\u0131",
         "VI": "Th\u1ea5t Tinh L\u01b0u Quang"
     },
+    "6373505": {
+        "CHS": "\u8863\u88c1\u4e09\u793c",
+        "DE": "Drei Rituale der Schneiderei",
+        "EN": "A Tailor's Three Courtesies",
+        "ES": "Protocolo de sastre",
+        "FR": "Trois us de broderie",
+        "ID": "A Tailor's Three Courtesies",
+        "IT": "Tre cortesie sartoriali",
+        "JP": "\u8863\u88c1\u4e09\u793c",
+        "KR": "\uc0bc\ub840 \uc7ac\ub2e8",
+        "PT": "Tr\u00eas Cortesias da Costura",
+        "RU": "\u0422\u0440\u0438 \u043b\u044e\u0431\u0435\u0437\u043d\u043e\u0441\u0442\u0438 \u043f\u043e\u0440\u0442\u043d\u043e\u0433\u043e",
+        "TH": "A Tailor's Three Courtesies",
+        "TR": "Terzinin \u00dc\u00e7 G\u00f6rg\u00fc Kural\u0131",
+        "VI": "Ba Ph\u1ea7n Cung K\u00ednh"
+    },
     "63855777": {
         "CHS": "\u76c8\u865a\u85cf\u8c61",
         "DE": "Verborgene Ebbe und Flut",
         "EN": "The Hidden Ebb and Flow",
         "ES": "S\u00edntomas variables",
         "FR": "Fluctuations d\u00e9routantes",
         "ID": "The Hidden Ebb and Flow",
@@ -7163,14 +7211,30 @@
         "KR": "\uc228\uc740 \ubcd1",
         "PT": "Sinais Ocultos da Mudan\u00e7a",
         "RU": "\u0421\u043e\u043a\u0440\u044b\u0442\u044b\u0435 \u0442\u043e\u043a\u0438",
         "TH": "The Hidden Ebb and Flow",
         "TR": "Gizli Metcezir",
         "VI": "Doanh H\u01b0 T\u00e0ng T\u01b0\u1ee3ng"
     },
+    "645847961": {
+        "CHS": "\u7f00\u9526\u56db\u5206",
+        "DE": "Vier Brokatverzierungen",
+        "EN": "Four Brocade Embellishments",
+        "ES": "Bordado y rematado",
+        "FR": "Quatre retouches de brocart",
+        "ID": "Four Brocade Embellishments",
+        "IT": "Quattro decorazioni in broccato",
+        "JP": "\u7db4\u9326\u56db\u5206",
+        "KR": "\uc0ac\ubd84 \uc790\uc218",
+        "PT": "Quatro Embelezamentos de Brocado",
+        "RU": "\u0427\u0435\u0442\u044b\u0440\u0435 \u0443\u043a\u0440\u0430\u0448\u0435\u043d\u0438\u044f \u043f\u0430\u0440\u0447\u0438",
+        "TH": "Four Brocade Embellishments",
+        "TR": "D\u00f6rt S\u0131rmal\u0131 S\u00fcsleme",
+        "VI": "B\u1ed1n B\u1ed9 Trang S\u1ee9c"
+    },
     "652576049": {
         "CHS": "\u73ca\u745a\u4e00\u5fc3",
         "DE": "Sango Isshin",
         "EN": "Sango Isshin",
         "ES": "Coraz\u00f3n del coral",
         "FR": "Sango Isshin",
         "ID": "Sango Isshin",
@@ -7275,14 +7339,30 @@
         "KR": "\ubd81\ub450\uc758 \uadc0\uc2e0 \ud1f4\uce58",
         "PT": "Destrui\u00e7\u00e3o do Mal",
         "RU": "\u041f\u043e\u0433\u0438\u0431\u0435\u043b\u044c \u043f\u043e\u0440\u043e\u043a\u0430",
         "TH": "Bane of Evil",
         "TR": "\u015eer Lanet",
         "VI": "Beidou Di\u1ec7t \u00c1c"
     },
+    "689897337": {
+        "CHS": "\u6b63\u7ee2\u516d\u901a",
+        "DE": "Sechs Pfade der Seidigkeit",
+        "EN": "Six Paths of Sage Silkcraft",
+        "ES": "Maestr\u00eda de la seda",
+        "FR": "Six voies de la soierie",
+        "ID": "Six Paths of Sage Silkcraft",
+        "IT": "Sei vie della seteria sapiente",
+        "JP": "\u6b63\u7d79\u516d\u901a",
+        "KR": "\uc721\ud560 \ubb34\ub2ac",
+        "PT": "Seis Caminhos da Seda da Sabedoria",
+        "RU": "\u0428\u0435\u0441\u0442\u044c \u0437\u043d\u0430\u043d\u0438\u0439 \u0448\u0451\u043b\u043a\u0430",
+        "TH": "Six Paths of Sage Silkcraft",
+        "TR": "\u0130pek Ustal\u0131\u011f\u0131 \u0130lminin Alt\u0131 Yolu",
+        "VI": "S\u00e1u Kh\u1ed5 L\u1ee5a L\u00e0"
+    },
     "690499809": {
         "CHS": "\u5360\u7406\u4e0d\u9976\u4eba",
         "DE": "Rechthaberei",
         "EN": "The Law Knows No Kindness",
         "ES": "Insisto, Se\u00f1or\u00eda",
         "FR": "Plaidoyer convaincant",
         "ID": "The Law Knows No Kindness",
@@ -7787,14 +7867,30 @@
         "KR": "\ub0b4\uc77c\uc758 \uc2a4\ud0c0",
         "PT": "Estrela de Amanh\u00e3",
         "RU": "\u0423\u0442\u0440\u0435\u043d\u043d\u044f\u044f \u0437\u0432\u0435\u0437\u0434\u0430",
         "TH": "Star of Tomorrow",
         "TR": "Yar\u0131n\u0131n Y\u0131ld\u0131z\u0131",
         "VI": "Ng\u00f4i Sao Ng\u00e0y Mai"
     },
+    "94228129": {
+        "CHS": "\u4e07\u7406\u4e00\u7a7a",
+        "DE": "Verfolgung des einen Prinzips",
+        "EN": "Sole Principle Pursuit",
+        "ES": "Convicci\u00f3n y ambici\u00f3n",
+        "FR": "Un pr\u00e9cepte",
+        "ID": "Sole Principle Pursuit",
+        "IT": "Un unico principio",
+        "JP": "\u4e07\u7406\u4e00\u7a7a",
+        "KR": "\ub9cc\ub9ac\uc77c\uacf5",
+        "PT": "Buscando o Princ\u00edpio Universal",
+        "RU": "\u0421\u043b\u0435\u0434\u0443\u044f \u0435\u0434\u0438\u043d\u043e\u043c\u0443 \u043f\u0440\u0438\u043d\u0446\u0438\u043f\u0443",
+        "TH": "Sole Principle Pursuit",
+        "TR": "Tek ve Esas Hedef",
+        "VI": "M\u1ed9t L\u00f2ng Tu\u00e2n Th\u1ee7"
+    },
     "94680617": {
         "CHS": "\u9e64\u5533\u8fdc\u4eba\u95f4",
         "DE": "Ausgestiegen aus der Welt",
         "EN": "Aloof From the World",
         "ES": "Graznido ermita\u00f1o",
         "FR": "R\u00e9clusion du monde",
         "ID": "Aloof From the World",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/fight_props.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/fight_props.json`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/namecards.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/namecards.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894736842105263%*

 * *Differences: {"'3292114052'": "OrderedDict([('CHS', '千织·展袖'), ('DE', 'Chiori – Spektakuläre Ärmel'), ('EN', "*

 * *                 "'Chiori: Spectacular Sleeves'), ('ES', 'Chiori - Tamoto'), ('FR', 'Chiori - "*

 * *                 "Manches spectaculaires'), ('ID', 'Chiori: Spectacular Sleeves'), ('IT', 'Chiori: "*

 * *                 "Maniche mozzafiato'), ('JP', '千織·展袂'), ('KR', '치오리·펼친 소매'), ('PT', 'Chiori - "*

 * *                 "Mangas Abertas'), ('RU', 'Развевающиеся рукава'), ('TH', 'Chiori - สยายกิโมโน'), "*

 * *                 "(' […]*

```diff
@@ -1755,14 +1755,30 @@
         "KR": "\ubaac\ub4dc\u00b7\ucd95\ubcf5",
         "PT": "Mondstadt - B\u00ean\u00e7\u00e3o",
         "RU": "\u041c\u043e\u043b\u0438\u0442\u0432\u0430",
         "TH": "Mondstadt - Blessing",
         "TR": "Mondstadt: L\u00fctuf",
         "VI": "Mondstadt - Ch\u00fac Ph\u00fac"
     },
+    "3292114052": {
+        "CHS": "\u5343\u7ec7\u00b7\u5c55\u8896",
+        "DE": "Chiori \u2013 Spektakul\u00e4re \u00c4rmel",
+        "EN": "Chiori: Spectacular Sleeves",
+        "ES": "Chiori - Tamoto",
+        "FR": "Chiori - Manches spectaculaires",
+        "ID": "Chiori: Spectacular Sleeves",
+        "IT": "Chiori: Maniche mozzafiato",
+        "JP": "\u5343\u7e54\u00b7\u5c55\u8882",
+        "KR": "\uce58\uc624\ub9ac\u00b7\ud3bc\uce5c \uc18c\ub9e4",
+        "PT": "Chiori - Mangas Abertas",
+        "RU": "\u0420\u0430\u0437\u0432\u0435\u0432\u0430\u044e\u0449\u0438\u0435\u0441\u044f \u0440\u0443\u043a\u0430\u0432\u0430",
+        "TH": "Chiori - \u0e2a\u0e22\u0e32\u0e22\u0e01\u0e34\u0e42\u0e21\u0e42\u0e19",
+        "TR": "Chiori: G\u00f6steri\u015fli Kollar",
+        "VI": "Chiori - Tay \u00c1o Tr\u00ecnh Di\u1ec5n"
+    },
     "3295622364": {
         "CHS": "\u7a3b\u59bb\u00b7\u5e38\u4e16",
         "DE": "Inazuma \u2013 Tokoyo",
         "EN": "Inazuma: Tokoyo",
         "ES": "Inazuma - Tokoyo",
         "FR": "Inazuma - Tokoyo",
         "ID": "Inazuma: Tokoyo",
@@ -2859,14 +2875,30 @@
         "KR": "\uae30\ud589\u00b7\uc7a0\uae34 \ubcc4",
         "PT": "Passe de Batalha: Estrela-cadente",
         "RU": "\u041f\u0430\u0434\u0430\u044e\u0449\u0430\u044f \u0437\u0432\u0435\u0437\u0434\u0430",
         "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e14\u0e32\u0e23\u0e32\u0e17\u0e35\u0e48\u0e23\u0e48\u0e27\u0e07\u0e2b\u0e25\u0e48\u0e19",
         "TR": "Gezi Notlar\u0131: Kayan Y\u0131ld\u0131z",
         "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - Sao R\u01a1i"
     },
+    "882758588": {
+        "CHS": "\u7eaa\u884c\u00b7\u9b54\u8403",
+        "DE": "Erlebnispass \u2013 Scheidekunst",
+        "EN": "Travel Notes: Arcane Amassing",
+        "ES": "PB - Arcanidad",
+        "FR": "PB - Arcanicit\u00e9",
+        "ID": "Catatan Perjalanan: Pengumpulan Misterius",
+        "IT": "Appunti di viaggio: Convergenza arcana",
+        "JP": "\u7d00\u884c\u00b7\u9b54\u8403",
+        "KR": "\uae30\ud589\u00b7\uc751\ucd95\ub41c \uc2e0\ube44",
+        "PT": "Passe de Batalha: Cole\u00e7\u00e3o Arcana",
+        "RU": "\u041c\u0438\u0441\u0442\u0438\u0447\u0435\u0441\u043a\u043e\u0435 \u0441\u043a\u043e\u043f\u043b\u0435\u043d\u0438\u0435",
+        "TH": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01 - \u0e28\u0e32\u0e2a\u0e15\u0e23\u0e4c\u0e2b\u0e25\u0e2d\u0e21\u0e23\u0e27\u0e21",
+        "TR": "Gezi Notlar\u0131: Sakl\u0131 Birikim",
+        "VI": "Nh\u1eadt K\u00fd H\u00e0nh Tr\u00ecnh - H\u00f3a K\u1ef9"
+    },
     "884046340": {
         "CHS": "\u5bb5\u5bab\u00b7\u7409\u91d1\u706b\u82b1",
         "DE": "Yoimiya \u2013 Auratus-Funken",
         "EN": "Yoimiya: Auratus Spark",
         "ES": "Yoimiya - Pirotecnia dorada",
         "FR": "Yoimiya - \u00c9tincelle dor\u00e9e",
         "ID": "Yoimiya: Auratus Spark",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/skills.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/skills.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9885057471264368%*

 * *Differences: {"'2315821309'": "OrderedDict([('CHS', '羽袖一触'), ('DE', 'Streichelnde Hasode'), ('EN', 'Fluttering "*

 * *                 "Hasode'), ('ES', 'Caricia de mangas'), ('FR', 'Caresse de plume'), ('ID', "*

 * *                 "'Fluttering Hasode'), ('IT', 'Hasode svolazzante'), ('JP', '羽袖一触'), ('KR', '하소데의 "*

 * *                 "손길'), ('PT', 'Carícia da Pluma Penada'), ('RU', 'Порхание хасодэ'), ('TH', "*

 * *                 "'Fluttering Hasode'), ('TR', 'Hasode Darbesi'), ('VI', 'Hasode Lả Lướt')])",*

 * * "'2428119293'": "OrderedDi […]*

```diff
@@ -3099,14 +3099,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "2315821309": {
+        "CHS": "\u7fbd\u8896\u4e00\u89e6",
+        "DE": "Streichelnde Hasode",
+        "EN": "Fluttering Hasode",
+        "ES": "Caricia de mangas",
+        "FR": "Caresse de plume",
+        "ID": "Fluttering Hasode",
+        "IT": "Hasode svolazzante",
+        "JP": "\u7fbd\u8896\u4e00\u89e6",
+        "KR": "\ud558\uc18c\ub370\uc758 \uc190\uae38",
+        "PT": "Car\u00edcia da Pluma Penada",
+        "RU": "\u041f\u043e\u0440\u0445\u0430\u043d\u0438\u0435 \u0445\u0430\u0441\u043e\u0434\u044d",
+        "TH": "Fluttering Hasode",
+        "TR": "Hasode Darbesi",
+        "VI": "Hasode L\u1ea3 L\u01b0\u1edbt"
+    },
     "232048445": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5377\u79ef\u5fae\u5c18",
         "DE": "Standardangriff: Aufgewirbelter Staub",
         "EN": "Normal Attack: Whirlwind Thrust",
         "ES": "Ataque Normal: Impulso de torbellino",
         "FR": "Attaque normale : Coup de tourbillon",
         "ID": "Normal Attack: Whirlwind Thrust",
@@ -3387,14 +3403,30 @@
         "KR": "\uacbd\uce58 \ucf58\ud150\uce20",
         "PT": "Jogabilidade Paisag\u00edstica",
         "RU": "\u0418\u0433\u0440\u0430 \u043f\u0435\u0439\u0437\u0430\u0436\u0435\u0439",
         "TH": "Sceneplay",
         "TR": "Sahne Oyunu",
         "VI": "C\u00e1ch Ch\u01a1i C\u1ea3nh Quan"
     },
+    "2428119293": {
+        "CHS": "4.5\u53f2\u83b1\u59c6\u7403-\u7269\u7406\u8fde\u5c04",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "2430743149": {
         "CHS": "\u6d6e\u51b0\u589e\u538b",
         "DE": "Treibeis-Druck",
         "EN": "Pressurized Floe",
         "ES": "Criopresurizaci\u00f3n",
         "FR": "Pressurisation des floes",
         "ID": "Pressurized Floe",
@@ -4715,14 +4747,30 @@
         "KR": "\ud48d\ub9c8\ub958-\uc9c0\uba74",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "2873692477": {
+        "CHS": "\u5343\u7ec7\u4e8c\u6bb5E\u540e-\u6280\u80fd\u66ff\u6362",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "2874294485": {
         "CHS": "\u65ab\u96f7",
         "DE": "Blitzbrecher",
         "EN": "Stormbreaker",
         "ES": "Quebrantatormentas",
         "FR": "Brisure d'orage",
         "ID": "Stormbreaker",
@@ -5819,14 +5867,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "331992085": {
+        "CHS": "\u5343\u7ec7\u7a7a\u4e2d\u653b\u51fb",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "33306749": {
         "CHS": "\u6d41\u6d6a\u8005\u5143\u7d20\u6218\u6280",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -6795,14 +6859,30 @@
         "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc8c4\uba78\uc758 \ud654\uc0b4",
         "PT": "Ataque Normal: Flechas da Culpa",
         "RU": "\u0421\u0442\u0440\u0435\u043b\u0430 \u0432\u043e\u0437\u043c\u0435\u0437\u0434\u0438\u044f",
         "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Bolts of Downfall",
         "TR": "Normal Sald\u0131r\u0131: D\u00fc\u015fen Y\u0131ld\u0131r\u0131mlar",
         "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - M\u0169i T\u00ean Di\u1ec7t \u00c1c"
     },
+    "373425821": {
+        "CHS": "\u4e8c\u5200\u4e4b\u5f62\u00b7\u6bd4\u7ffc",
+        "DE": "Doppelklinge \u2013 Hiyoku",
+        "EN": "Hiyoku: Twin Blades",
+        "ES": "Filos gemelos: Desenvaine al\u00edgero",
+        "FR": "Hiyoku : Lames jumelles",
+        "ID": "Hiyoku: Twin Blades",
+        "IT": "Hiyoku: Lame gemelle",
+        "JP": "\u4e8c\u5200\u306e\u578b\u00b7\u6bd4\u7ffc",
+        "KR": "\uc30d\uac80\u00b7\ube44\uc775",
+        "PT": "L\u00e2minas G\u00eameas: Em Voo",
+        "RU": "\u0425\u0438\u0451\u043a\u0443: \u041f\u0430\u0440\u043d\u044b\u0435 \u043a\u043b\u0438\u043d\u043a\u0438",
+        "TH": "Hiyoku: Twin Blades",
+        "TR": "Hiyoku: \u00c7ift K\u0131l\u0131\u00e7",
+        "VI": "Hiyoku - Song \u0110ao Th\u1ee9c"
+    },
     "3734682949": {
         "CHS": "\u767d\u672f\u7a7a\u4e2d\u653b\u51fb",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
@@ -7291,14 +7371,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "3906587141": {
+        "CHS": "4.5\u53f2\u83b1\u59c6\u7403-\u5143\u7d20\u5f39",
+        "DE": "",
+        "EN": "",
+        "ES": "",
+        "FR": "",
+        "ID": "",
+        "IT": "",
+        "JP": "",
+        "KR": "",
+        "PT": "",
+        "RU": "",
+        "TH": "",
+        "TR": "",
+        "VI": ""
+    },
     "3909984477": {
         "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u53e4\u534e\u5251\u6cd5",
         "DE": "Standardangriff: Guhua-Stil",
         "EN": "Normal Attack: Guhua Style",
         "ES": "Ataque Normal: T\u00e9cnica de espada Guhua",
         "FR": "Attaque normale : Style Guhua",
         "ID": "Normal Attack: Guhua Style",
@@ -9563,14 +9659,30 @@
         "KR": "",
         "PT": "",
         "RU": "",
         "TH": "",
         "TR": "",
         "VI": ""
     },
+    "914798901": {
+        "CHS": "\u666e\u901a\u653b\u51fb\u00b7\u5fc3\u7ec7\u5200\u6d41",
+        "DE": "Standardangriff: Webende Klinge",
+        "EN": "Normal Attack: Weaving Blade",
+        "ES": "Ataque Normal: T\u00e9cnica tejecorazones",
+        "FR": "Attaque normale : Lame de tissage",
+        "ID": "Normal Attack: Weaving Blade",
+        "IT": "Attacco normale: Lama intrecciata",
+        "JP": "\u901a\u5e38\u653b\u6483\u00b7\u5fc3\u7e54\u5200\u6d41",
+        "KR": "\uc77c\ubc18 \uacf5\uaca9\u00b7\uc9c1\uc870 \uac80\uc220",
+        "PT": "Ataque Normal: L\u00e2mina Tecel\u00e3",
+        "RU": "\u0422\u043a\u0443\u0449\u0438\u0439 \u043a\u043b\u0438\u043d\u043e\u043a",
+        "TH": "\u0e42\u0e08\u0e21\u0e15\u0e35\u0e1b\u0e01\u0e15\u0e34: Weaving Blade",
+        "TR": "Normal Sald\u0131r\u0131: \u00d6rg\u00fc K\u0131l\u0131c\u0131",
+        "VI": "T\u1ea5n C\u00f4ng Th\u01b0\u1eddng - L\u01b0\u1ee1i \u0110ao D\u1ec7t G\u1ea5m"
+    },
     "92557693": {
         "CHS": "\u6d41\u6d6a\u8005\u5143\u7d20\u6218\u6280",
         "DE": "",
         "EN": "",
         "ES": "",
         "FR": "",
         "ID": "",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets/langs/weapons.json` & `enkanetworkv2.py-2.0.1/enkanetwork/assets/langs/weapons.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9905660377358491%*

 * *Differences: {"'1818340435'": "OrderedDict([('CHS', '有乐御簾切'), ('DE', 'Uraku Misugiri'), ('EN', 'Uraku "*

 * *                 "Misugiri'), ('ES', 'Cortatelones de Urakusai'), ('FR', 'Uraku Misugiri'), ('ID', "*

 * *                 "'Uraku Misugiri'), ('IT', 'Uraku Misugiri'), ('JP', '有楽御簾切'), ('KR', '우라쿠의 "*

 * *                 "미스기리'), ('PT', 'Urakugo Rensai'), ('RU', 'Ураку мисугири'), ('TH', 'Uraku "*

 * *                 "Misugiri'), ('TR', 'Uraku Misugiri'), ('VI', 'Uraku Misugiri')])",*

 * * "'2847771107'": "OrderedDict([('CHS', '沙中伟贤的对 […]*

```diff
@@ -587,14 +587,30 @@
         "KR": "\ubc43\ub3c4\ub791 \uc7a5\uac80",
         "PT": "A Doca",
         "RU": "\u0412\u0435\u0440\u0444\u044c",
         "TH": "The Dockhand's Assistant",
         "TR": "R\u0131ht\u0131m K\u0131l\u0131c\u0131",
         "VI": "Ki\u1ebfm B\u1ebfn T\u00e0u"
     },
+    "1818340435": {
+        "CHS": "\u6709\u4e50\u5fa1\u7c3e\u5207",
+        "DE": "Uraku Misugiri",
+        "EN": "Uraku Misugiri",
+        "ES": "Cortatelones de Urakusai",
+        "FR": "Uraku Misugiri",
+        "ID": "Uraku Misugiri",
+        "IT": "Uraku Misugiri",
+        "JP": "\u6709\u697d\u5fa1\u7c3e\u5207",
+        "KR": "\uc6b0\ub77c\ucfe0\uc758 \ubbf8\uc2a4\uae30\ub9ac",
+        "PT": "Urakugo Rensai",
+        "RU": "\u0423\u0440\u0430\u043a\u0443 \u043c\u0438\u0441\u0443\u0433\u0438\u0440\u0438",
+        "TH": "Uraku Misugiri",
+        "TR": "Uraku Misugiri",
+        "VI": "Uraku Misugiri"
+    },
     "1860795787": {
         "CHS": "\u66da\u4e91\u4e4b\u6708",
         "DE": "Mouun-Mond",
         "EN": "Mouun's Moon",
         "ES": "Luna de Mouun",
         "FR": "Lune de Mouun",
         "ID": "Mouun's Moon",
@@ -1467,14 +1483,30 @@
         "KR": "\uac08\ub300 \ubc14\ub2e4\uc758 \ub4f1\ub300",
         "PT": "Sinal dos Mares",
         "RU": "\u041c\u0430\u044f\u043a \u0442\u0440\u043e\u0441\u0442\u043d\u0438\u043a\u043e\u0432\u043e\u0433\u043e \u043c\u043e\u0440\u044f",
         "TH": "Beacon of the Reed Sea",
         "TR": "K\u0131z\u0131l \u00c7\u00f6l\u00fcn \u0130radesi",
         "VI": "H\u1ea3i \u0110\u0103ng B\u1edd Bi\u1ec3n Lau"
     },
+    "2847771107": {
+        "CHS": "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54",
+        "DE": "Dialoge der Weisen der W\u00fcste",
+        "EN": "Dialogues of the Desert Sages",
+        "ES": "Discusi\u00f3n de los Sabios del Desierto",
+        "FR": "Dialogues des sages du d\u00e9sert",
+        "ID": "Dialogues of the Desert Sages",
+        "IT": "Dialoghi dei saggi del deserto",
+        "JP": "\u7802\u4e2d\u306e\u8ce2\u8005\u9054\u306e\u554f\u7b54",
+        "KR": "\uc704\ub300\ud55c \uc0ac\ub9c9 \ud604\uc790\uc758 \ub300\ub2f5",
+        "PT": "Conversas dos S\u00e1bios do Deserto",
+        "RU": "\u0414\u0438\u0430\u043b\u043e\u0433 \u043f\u0443\u0441\u0442\u044b\u043d\u043d\u044b\u0445 \u043c\u0443\u0434\u0440\u0435\u0446\u043e\u0432",
+        "TH": "Dialogues of the Desert Sages",
+        "TR": "\u00c7\u00f6l Alimleriyle Sohbet",
+        "VI": "\u0110\u1ed1i Tho\u1ea1i C\u1ee7a Hi\u1ec1n Gi\u1ea3 Sa M\u1ea1c"
+    },
     "2918525947": {
         "CHS": "\u98de\u96f7\u4e4b\u5f26\u632f",
         "DE": "Donnerpuls",
         "EN": "Thundering Pulse",
         "ES": "Agitador del Rel\u00e1mpago",
         "FR": "Pulsation du tonnerre",
         "ID": "Thundering Pulse",
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/assets.py` & `enkanetworkv2.py-2.0.1/enkanetwork/assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,26 @@
             "id": id if str(id).isdigit() else id.split("-")[0],
             "skill_id": str(id).split("-")[1] if not str(id).isdigit() else 0,
             "images": cls.create_character_icon(data["sideIconName"]),
             **data
         })
 
     @classmethod
+    def character_avatar(cls, id: int) -> Optional[assets.CharacterCostume]:
+        LOGGER.debug(f"Getting costume assets with id: {id}")
+        data = cls.DATA["pfps"].get(str(id))
+        if not data:
+            LOGGER.error(f"Costume not found with id: {id}")
+            return        
+        return assets.CharacterAvatar.parse_obj({
+            "id": id,
+            "images": cls.create_character_icon(data["iconPath"])
+        })
+    
+    @classmethod
     def character_costume(cls, id: int) -> Optional[assets.CharacterCostume]:
         LOGGER.debug(f"Getting costume assets with id: {id}")
         data = cls.DATA["costumes"].get(str(id))
         if not data:
             LOGGER.error(f"Costume not found with id: {id}")
             return
 
@@ -161,23 +173,33 @@
     @classmethod
     def character_icon(cls, id: int) -> Optional[assets.CharacterIconAsset]:
         data = cls.character(id)
         if not data:
             return
 
         return data.images
+    
+    @classmethod
+    def character_icon_pfps(cls, id: int) -> Optional[assets.CharacterIconAsset]:
+        data = cls.character(id)
+        if not data:
+            return
+
+        return data.images
 
     @staticmethod
     def create_character_icon(path: str) -> assets.CharacterIconAsset:
         return assets.CharacterIconAsset(
             icon=utils.IconAsset(filename=path.replace("_Side", "")),
             side=utils.IconAsset(filename=path),
             banner=utils.IconAsset(filename=path.replace("AvatarIcon_Side", "Gacha_AvatarImg")),  # noqa: E501
             card=utils.IconAsset(filename=path.replace("_Side", "") + "_Card")
         )
+        
+         
 
     @classmethod
     def create_chractar_costume_icon(cls, path: str) -> assets.CharacterIconAsset:  # noqa: E501
         _data = cls.create_character_icon(path)
         _data.banner = utils.IconAsset(filename=_data.banner.filename.replace("Gacha_AvatarImg", "Costume"))  # noqa: E501
         return _data
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/cache.py` & `enkanetworkv2.py-2.0.1/enkanetwork/cache.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/client.py` & `enkanetworkv2.py-2.0.1/enkanetwork/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
-import os
 import json
 import logging
 
 from typing import Union, Optional, Type, TYPE_CHECKING, List, Any, Dict
 from enkacard import enkatools
 
 from .http import HTTPClient
 from .model.base import (
     EnkaNetworkResponse,
     EnkaNetworkProfileResponse
 )
 from .model.hoyos import PlayerHoyos
 from .model.build import Builds
 
+from .utils import update_pfps
 from .assets import Assets
 from .enum import Language
 from .cache import Cache, StaticCache
 from .config import Config
 from .tools import (
     merge_raw_data
 )
@@ -198,15 +198,14 @@
             data["owner"] = {
                 **data["owner"],
                 "builds": await self.fetch_builds(
                     profile_id=data["owner"]["username"],
                     metaname=data["owner"]["hash"]
                 )
             }
-
         return EnkaNetworkResponse.parse_obj(data)
 
     async def fetch_user_by_username(
         self,
         profile_id: Optional[str]
     ) -> EnkaNetworkProfileResponse:
         """ Fetch user profile by Username / patreon ID
@@ -385,17 +384,18 @@
 
         new_data = await self.fetch_raw_data(uid)
         return await merge_raw_data(new_data, old_data)
 
     async def update_assets(self) -> None:
         path = Assets._get_path_assets()
         tools = enkatools.Tools()
-        path =  path["data"].replace("\data",'').replace("\\data",'')
-        await tools.update_assets(path = path)
+        path = path["data"].replace("\\data", '')
         
+        await update_pfps(papath = path)
+        await tools.update_assets(path = path)
         
         self.assets.reload_assets()
         
     async def __format_hoyos(self, username: str, data: List[Any]) -> List[PlayerHoyos]:  # noqa
         return [PlayerHoyos.parse_obj({
             "builds": await self.fetch_builds(profile_id=username,
                                               metaname=data[key]["hash"]),
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/config.py` & `enkanetworkv2.py-2.0.1/enkanetwork/config.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/enum.py` & `enkanetworkv2.py-2.0.1/enkanetwork/enum.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/exception.py` & `enkanetworkv2.py-2.0.1/enkanetwork/exception.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/http.py` & `enkanetworkv2.py-2.0.1/enkanetwork/http.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/assets.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,29 @@
     hash_id: :class:`str`
         Costume hash id
     icon: :class:`IconAsset`
         A icon assets. Please refers in `IconAsset` class
     """
     id: int = 0
     images: CharacterIconAsset = None
+    
+class CharacterAvatar(BaseModel):
+    """ Character Costume (Assets)
+
+    Attributes
+    ------------
+    id: :class:`int`
+        Costume ID
+    hash_id: :class:`str`
+        Costume hash id
+    icon: :class:`IconAsset`
+        A icon assets. Please refers in `IconAsset` class
+    """
+    id: int = 0
+    images: CharacterIconAsset = None
 
 class AritfactProps(BaseModel):
     id: int = 0
     type: str = Field('', alias='propType')
     digit: str = Field('DIGIT', alias='propDigit')
     value: Union[int, float] = Field(0, alias='propValue')
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/base.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/base.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/build.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/build.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/character.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/character.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/equipments.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/equipments.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/players.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/players.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,24 @@
         LOGGER.debug("=== Avatar ===")
         if "avatarId" in data:
             if "costumeId" in data:
                 _data = Assets.character_costume(str(data["costumeId"]))
                 icon = _data.images if _data is not None else _data
             else:
                 icon = Assets.character_icon(str(data["avatarId"]))
-
-            if not icon:
-                return
-
-            self.icon = icon.icon
+        elif "id" in data:
+            self.id = int(data["id"])
+            _data = Assets.character_avatar(self.id)
+            icon = _data.images if _data is not None else _data
+            
+            
+        if not icon:
+            return    
+         
+        self.icon = icon.icon
 
 
 class showAvatar(BaseModel):
     """
         API Response data
     """
     id: Union[int, str] = Field(0, alias="avatarId")
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/model/stats.py` & `enkanetworkv2.py-2.0.1/enkanetwork/model/stats.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/tools.py` & `enkanetworkv2.py-2.0.1/enkanetwork/tools.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/types/enkanetwork.py` & `enkanetworkv2.py-2.0.1/enkanetwork/types/enkanetwork.py`

 * *Files identical despite different names*

### Comparing `enkanetworkv2.py-2.0.0/enkanetwork/utils.py` & `enkanetworkv2.py-2.0.1/enkanetwork/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 """
 
 from __future__ import annotations
 
 import re
 import logging
 import sys
+import os
+import aiohttp
+import json
 
 from typing import Any, Dict, TYPE_CHECKING
 
 from . import __version__
 
 if TYPE_CHECKING:
     from aiohttp import ClientResponse
@@ -117,7 +120,16 @@
             red += len(chunk)
 
     content = {
         "status": response.status,
         "content": data
     }
     return content
+
+
+async def update_pfps(path):
+    async with aiohttp.ClientSession() as session:
+        async with session.get("https://raw.githubusercontent.com/EnkaNetwork/API-docs/master/store/pfps.json") as response:
+            data = await response.json()
+    
+    with open(os.path.join(path, "pfps.json"), 'w',  encoding='utf-8') as file:
+        json.dump(data, file, indent=4)
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/PKG-INFO` & `enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkanetworkv2.py
-Version: 2.0.0
+Version: 2.0.1
 Summary: Library for fetching JSON data from site https://enka.network/
 Home-page: https://github.com/DEViantUA/EnkaNetworkV2.py
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: enkanetwork.py,enkanetwork,enka.network,genshinapi,enkanetworkV2,enkanetworkV2.py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enkanetworkv2.py-2.0.0/enkanetworkV2.py.egg-info/SOURCES.txt` & `enkanetworkv2.py-2.0.1/enkanetworkv2.py.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,26 +8,22 @@
 enkanetwork/client.py
 enkanetwork/config.py
 enkanetwork/enum.py
 enkanetwork/exception.py
 enkanetwork/http.py
 enkanetwork/tools.py
 enkanetwork/utils.py
-enkanetworkV2.py.egg-info/PKG-INFO
-enkanetworkV2.py.egg-info/SOURCES.txt
-enkanetworkV2.py.egg-info/dependency_links.txt
-enkanetworkV2.py.egg-info/requires.txt
-enkanetworkV2.py.egg-info/top_level.txt
 enkanetwork/assets/data/artifact_props.json
 enkanetwork/assets/data/artifacts.json
 enkanetwork/assets/data/characters.json
 enkanetwork/assets/data/constellations.json
 enkanetwork/assets/data/costumes.json
 enkanetwork/assets/data/fight_props.json
 enkanetwork/assets/data/namecards.json
+enkanetwork/assets/data/pfps.json
 enkanetwork/assets/data/skills.json
 enkanetwork/assets/data/weapons.json
 enkanetwork/assets/langs/artifact_sets.json
 enkanetwork/assets/langs/artifacts.json
 enkanetwork/assets/langs/characters.json
 enkanetwork/assets/langs/constellations.json
 enkanetwork/assets/langs/fight_props.json
```

### Comparing `enkanetworkv2.py-2.0.0/setup.py` & `enkanetworkv2.py-2.0.1/setup.py`

 * *Files identical despite different names*

