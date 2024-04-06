# Comparing `tmp/pythondatautil-0.0.16.tar.gz` & `tmp/pythondatautil-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythondatautil-0.0.16.tar", last modified: Mon Mar  4 23:39:38 2024, max compression
+gzip compressed data, was "pythondatautil-0.0.17.tar", last modified: Sat Apr  6 15:53:04 2024, max compression
```

## Comparing `pythondatautil-0.0.16.tar` & `pythondatautil-0.0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-03-04 23:39:38.188675 pythondatautil-0.0.16/
--rw-r--r--   0 moritaippei   (501) staff       (20)     1072 2023-05-01 02:49:53.000000 pythondatautil-0.0.16/LICENSE
--rw-r--r--   0 moritaippei   (501) staff       (20)     4754 2024-03-04 23:39:38.187638 pythondatautil-0.0.16/PKG-INFO
--rw-r--r--   0 moritaippei   (501) staff       (20)     4223 2024-03-04 23:11:20.000000 pythondatautil-0.0.16/README.md
--rwxr-xr-x   0 moritaippei   (501) staff       (20)      621 2024-03-04 22:54:23.000000 pythondatautil-0.0.16/pyproject.toml
--rw-r--r--   0 moritaippei   (501) staff       (20)       38 2024-03-04 23:39:38.188781 pythondatautil-0.0.16/setup.cfg
-drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-03-04 23:39:38.183950 pythondatautil-0.0.16/src/
-drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-03-04 23:39:38.185863 pythondatautil-0.0.16/src/pythondatautil/
--rwxrwxrwx   0 moritaippei   (501) staff       (20)       57 2024-03-03 17:32:28.000000 pythondatautil-0.0.16/src/pythondatautil/__init__.py
--rwxr-xr-x   0 moritaippei   (501) staff       (20)    15531 2024-03-04 22:38:29.000000 pythondatautil-0.0.16/src/pythondatautil/datautil.py
--rw-r--r--   0 moritaippei   (501) staff       (20)     2727 2024-02-27 16:41:54.000000 pythondatautil-0.0.16/src/pythondatautil/tableutil.py
-drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-03-04 23:39:38.187057 pythondatautil-0.0.16/src/pythondatautil.egg-info/
--rw-r--r--   0 moritaippei   (501) staff       (20)     4754 2024-03-04 23:39:38.000000 pythondatautil-0.0.16/src/pythondatautil.egg-info/PKG-INFO
--rw-r--r--   0 moritaippei   (501) staff       (20)      294 2024-03-04 23:39:38.000000 pythondatautil-0.0.16/src/pythondatautil.egg-info/SOURCES.txt
--rw-r--r--   0 moritaippei   (501) staff       (20)        1 2024-03-04 23:39:38.000000 pythondatautil-0.0.16/src/pythondatautil.egg-info/dependency_links.txt
--rw-r--r--   0 moritaippei   (501) staff       (20)       15 2024-03-04 23:39:38.000000 pythondatautil-0.0.16/src/pythondatautil.egg-info/top_level.txt
+drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-04-06 15:53:04.844579 pythondatautil-0.0.17/
+-rw-r--r--   0 moritaippei   (501) staff       (20)     1072 2023-05-01 02:49:53.000000 pythondatautil-0.0.17/LICENSE
+-rw-r--r--   0 moritaippei   (501) staff       (20)     5137 2024-04-06 15:53:04.844367 pythondatautil-0.0.17/PKG-INFO
+-rw-r--r--   0 moritaippei   (501) staff       (20)     4606 2024-04-06 15:52:02.000000 pythondatautil-0.0.17/README.md
+-rwxr-xr-x   0 moritaippei   (501) staff       (20)      621 2024-04-06 15:32:24.000000 pythondatautil-0.0.17/pyproject.toml
+-rw-r--r--   0 moritaippei   (501) staff       (20)       38 2024-04-06 15:53:04.844623 pythondatautil-0.0.17/setup.cfg
+drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-04-06 15:53:04.842692 pythondatautil-0.0.17/src/
+drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-04-06 15:53:04.843424 pythondatautil-0.0.17/src/pythondatautil/
+-rwxrwxrwx   0 moritaippei   (501) staff       (20)       57 2024-03-03 17:32:28.000000 pythondatautil-0.0.17/src/pythondatautil/__init__.py
+-rwxr-xr-x   0 moritaippei   (501) staff       (20)    15553 2024-04-06 15:48:37.000000 pythondatautil-0.0.17/src/pythondatautil/datautil.py
+-rw-r--r--   0 moritaippei   (501) staff       (20)     2727 2024-02-27 16:41:54.000000 pythondatautil-0.0.17/src/pythondatautil/tableutil.py
+drwxr-xr-x   0 moritaippei   (501) staff       (20)        0 2024-04-06 15:53:04.844116 pythondatautil-0.0.17/src/pythondatautil.egg-info/
+-rw-r--r--   0 moritaippei   (501) staff       (20)     5137 2024-04-06 15:53:04.000000 pythondatautil-0.0.17/src/pythondatautil.egg-info/PKG-INFO
+-rw-r--r--   0 moritaippei   (501) staff       (20)      294 2024-04-06 15:53:04.000000 pythondatautil-0.0.17/src/pythondatautil.egg-info/SOURCES.txt
+-rw-r--r--   0 moritaippei   (501) staff       (20)        1 2024-04-06 15:53:04.000000 pythondatautil-0.0.17/src/pythondatautil.egg-info/dependency_links.txt
+-rw-r--r--   0 moritaippei   (501) staff       (20)       15 2024-04-06 15:53:04.000000 pythondatautil-0.0.17/src/pythondatautil.egg-info/top_level.txt
```

### Comparing `pythondatautil-0.0.16/LICENSE` & `pythondatautil-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `pythondatautil-0.0.16/PKG-INFO` & `pythondatautil-0.0.17/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: pythondatautil
-Version: 0.0.16
+Version: 0.0.17
 Summary: Libraries to simplify file processing in Python
 Author-email: Ippei Morita <ippei0923@gmail.com>
 Project-URL: Homepage, https://github.com/m-ippei/pythondatautil
 Project-URL: Documentation, https://m-ippei.github.io/pythondatautil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pythondatautil
 Pythonのファイル処理を簡単にするためのライブラリ
 
-
-## シェルコマンド一覧
 #### インストール
+
 ```console
-python -m pip install git+https://github.com/m-ippei/pythondatautil.git
+python -m pip install pythondatautil
 ```
+
 #### アップデート
+
 ```console
-python -m pip install git+https://github.com/m-ippei/pythondatautil.git -U
+python -m pip install pythondatautil -U
 ```
+
 #### アンインストール
+
 ```console
 python -m pip uninstall pythondatautil
 ```
 
-## 簡易リファレンス DataUtil
+## 簡易リファレンス DataUtil(du)
 
 ### 概要
 
 ファイルとPythonのデータ型を双方に使いやすく変換
 
 ### 使い方
 ```Python
 from pythondatautil import du
 
 # テキストファイルの自動読み込み
 """tmp1.txt
 Hi!
 """
 
+# tmp1.txtというファイルを読み込む(パスを指定する)
 data = du.r_auto("tmp1.txt")
 print(data) # Hi!
 
 # データの自動書き込み
 du.w_auto([1,2,3]) 
 
 """tmp2.txt
@@ -140,11 +144,25 @@
 ```
 
 Wheelインストール
 ```console
 python -m pip install <wheel>
 ```
 
+## シェルコマンド一覧(GitHubからパッケージインストール等をする場合)
+#### インストール
+```console
+python -m pip install git+https://github.com/m-ippei/pythondatautil.git
+```
+#### アップデート
+```console
+python -m pip install git+https://github.com/m-ippei/pythondatautil.git -U
+```
+#### アンインストール
+```console
+python -m pip uninstall pythondatautil
+```
+
 ## 備考
 デフォルトで取り扱う文字コードはUTF-8
```

### Comparing `pythondatautil-0.0.16/README.md` & `pythondatautil-0.0.17/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # pythondatautil
 Pythonのファイル処理を簡単にするためのライブラリ
 
-
-## シェルコマンド一覧
 #### インストール
+
 ```console
-python -m pip install git+https://github.com/m-ippei/pythondatautil.git
+python -m pip install pythondatautil
 ```
+
 #### アップデート
+
 ```console
-python -m pip install git+https://github.com/m-ippei/pythondatautil.git -U
+python -m pip install pythondatautil -U
 ```
+
 #### アンインストール
+
 ```console
 python -m pip uninstall pythondatautil
 ```
 
-## 簡易リファレンス DataUtil
+## 簡易リファレンス DataUtil(du)
 
 ### 概要
 
 ファイルとPythonのデータ型を双方に使いやすく変換
 
 ### 使い方
 ```Python
 from pythondatautil import du
 
 # テキストファイルの自動読み込み
 """tmp1.txt
 Hi!
 """
 
+# tmp1.txtというファイルを読み込む(パスを指定する)
 data = du.r_auto("tmp1.txt")
 print(data) # Hi!
 
 # データの自動書き込み
 du.w_auto([1,2,3]) 
 
 """tmp2.txt
@@ -126,11 +130,25 @@
 ```
 
 Wheelインストール
 ```console
 python -m pip install <wheel>
 ```
 
+## シェルコマンド一覧(GitHubからパッケージインストール等をする場合)
+#### インストール
+```console
+python -m pip install git+https://github.com/m-ippei/pythondatautil.git
+```
+#### アップデート
+```console
+python -m pip install git+https://github.com/m-ippei/pythondatautil.git -U
+```
+#### アンインストール
+```console
+python -m pip uninstall pythondatautil
+```
+
 ## 備考
 デフォルトで取り扱う文字コードはUTF-8
```

### Comparing `pythondatautil-0.0.16/pyproject.toml` & `pythondatautil-0.0.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pythondatautil"
-version = "0.0.16"
+version = "0.0.17"
 authors = [
   { name="Ippei Morita", email="ippei0923@gmail.com" },
 ]
 description = "Libraries to simplify file processing in Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pythondatautil-0.0.16/src/pythondatautil/datautil.py` & `pythondatautil-0.0.17/src/pythondatautil/datautil.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,27 +156,27 @@
 
         Args:
             path (str): パス名 
 
         Returns:
             list (list): リスト
         """
-        with open(path,mode='r',encoding=read_encoding) as f:
+        with open(path,mode='r',encoding=read_encoding,newline='') as f:
             return [v for v in csv.reader(f)]
 
     def r_tsv(self,path) -> list:
         """TSVのパスを読み込んでリストにして返す
 
         Args:
             path (str): パス名 
 
         Returns:
             list (list): リスト
         """
-        with open(path,mode='r',encoding='utf-8') as f:
+        with open(path,mode='r',encoding='utf-8',newline='') as f:
             return [v for v in csv.reader(f,delimiter="\t")]
 
     def r_json(self,json_path):
         """JSONのパスを読み込んで辞書型にして返す
 
         Args:
             path (str): パス名
```

### Comparing `pythondatautil-0.0.16/src/pythondatautil/tableutil.py` & `pythondatautil-0.0.17/src/pythondatautil/tableutil.py`

 * *Files identical despite different names*

### Comparing `pythondatautil-0.0.16/src/pythondatautil.egg-info/PKG-INFO` & `pythondatautil-0.0.17/src/pythondatautil.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: pythondatautil
-Version: 0.0.16
+Version: 0.0.17
 Summary: Libraries to simplify file processing in Python
 Author-email: Ippei Morita <ippei0923@gmail.com>
 Project-URL: Homepage, https://github.com/m-ippei/pythondatautil
 Project-URL: Documentation, https://m-ippei.github.io/pythondatautil
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pythondatautil
 Pythonのファイル処理を簡単にするためのライブラリ
 
-
-## シェルコマンド一覧
 #### インストール
+
 ```console
-python -m pip install git+https://github.com/m-ippei/pythondatautil.git
+python -m pip install pythondatautil
 ```
+
 #### アップデート
+
 ```console
-python -m pip install git+https://github.com/m-ippei/pythondatautil.git -U
+python -m pip install pythondatautil -U
 ```
+
 #### アンインストール
+
 ```console
 python -m pip uninstall pythondatautil
 ```
 
-## 簡易リファレンス DataUtil
+## 簡易リファレンス DataUtil(du)
 
 ### 概要
 
 ファイルとPythonのデータ型を双方に使いやすく変換
 
 ### 使い方
 ```Python
 from pythondatautil import du
 
 # テキストファイルの自動読み込み
 """tmp1.txt
 Hi!
 """
 
+# tmp1.txtというファイルを読み込む(パスを指定する)
 data = du.r_auto("tmp1.txt")
 print(data) # Hi!
 
 # データの自動書き込み
 du.w_auto([1,2,3]) 
 
 """tmp2.txt
@@ -140,11 +144,25 @@
 ```
 
 Wheelインストール
 ```console
 python -m pip install <wheel>
 ```
 
+## シェルコマンド一覧(GitHubからパッケージインストール等をする場合)
+#### インストール
+```console
+python -m pip install git+https://github.com/m-ippei/pythondatautil.git
+```
+#### アップデート
+```console
+python -m pip install git+https://github.com/m-ippei/pythondatautil.git -U
+```
+#### アンインストール
+```console
+python -m pip uninstall pythondatautil
+```
+
 ## 備考
 デフォルトで取り扱う文字コードはUTF-8
```

