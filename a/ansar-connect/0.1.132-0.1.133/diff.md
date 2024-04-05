# Comparing `tmp/ansar-connect-0.1.132.tar.gz` & `tmp/ansar-connect-0.1.133.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.132.tar", last modified: Fri Apr  5 21:36:53 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.133.tar", last modified: Fri Apr  5 21:58:21 2024, max compression
```

## Comparing `ansar-connect-0.1.132.tar` & `ansar-connect-0.1.133.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:36:53.074394 ansar-connect-0.1.132/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.132/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-05 21:36:53.074394 ansar-connect-0.1.132/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.132/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.132/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-05 21:36:53.074394 ansar-connect-0.1.132/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.132/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:36:53.070394 ansar-connect-0.1.132/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:36:53.070394 ansar-connect-0.1.132/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:36:53.070394 ansar-connect-0.1.132/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.132/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.132/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.132/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.132/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:36:53.074394 ansar-connect-0.1.132/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-05 21:36:49.000000 ansar-connect-0.1.132/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13387 2024-03-23 02:08:11.000000 ansar-connect-0.1.132/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    79138 2024-04-05 21:35:44.000000 ansar-connect-0.1.132/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.132/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.132/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.132/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.132/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.132/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21086 2024-03-08 13:33:32.000000 ansar-connect-0.1.132/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.132/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.132/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.132/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.132/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.132/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.132/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.132/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.132/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6187 2024-03-28 02:15:57.000000 ansar-connect-0.1.132/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:36:53.074394 ansar-connect-0.1.132/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-05 21:36:53.000000 ansar-connect-0.1.132/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-05 21:36:53.000000 ansar-connect-0.1.132/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-05 21:36:53.000000 ansar-connect-0.1.132/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-05 21:36:53.000000 ansar-connect-0.1.132/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-05 21:36:53.000000 ansar-connect-0.1.132/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-05 21:36:53.000000 ansar-connect-0.1.132/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:58:21.129532 ansar-connect-0.1.133/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.133/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-05 21:58:21.129532 ansar-connect-0.1.133/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.133/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.133/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-05 21:58:21.129532 ansar-connect-0.1.133/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.133/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:58:21.125532 ansar-connect-0.1.133/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:58:21.125532 ansar-connect-0.1.133/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:58:21.125532 ansar-connect-0.1.133/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.133/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.133/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.133/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.133/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:58:21.129532 ansar-connect-0.1.133/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-05 21:58:18.000000 ansar-connect-0.1.133/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13387 2024-03-23 02:08:11.000000 ansar-connect-0.1.133/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    79138 2024-04-05 21:57:14.000000 ansar-connect-0.1.133/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.133/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.133/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.133/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.133/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.133/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21086 2024-03-08 13:33:32.000000 ansar-connect-0.1.133/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.133/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.133/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.133/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.133/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.133/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.133/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.133/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.133/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6187 2024-03-28 02:15:57.000000 ansar-connect-0.1.133/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-05 21:58:21.129532 ansar-connect-0.1.133/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-05 21:58:21.000000 ansar-connect-0.1.133/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-05 21:58:21.000000 ansar-connect-0.1.133/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-05 21:58:21.000000 ansar-connect-0.1.133/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-05 21:58:21.000000 ansar-connect-0.1.133/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-05 21:58:21.000000 ansar-connect-0.1.133/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-05 21:58:21.000000 ansar-connect-0.1.133/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.132/LICENSE` & `ansar-connect-0.1.133/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/PKG-INFO` & `ansar-connect-0.1.133/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.132
+Version: 0.1.133
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.132/README.md` & `ansar-connect-0.1.133/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/pyproject.toml` & `ansar-connect-0.1.133/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/setup.py` & `ansar-connect-0.1.133/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.133/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.133/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.133/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.133/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/__init__.py` & `ansar-connect-0.1.133/src/ansar/connect/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 7e6617dfdb3b6894adc025607294ba90421c5224
-Version: 0.1.131 (2024-04-06@10:36:49+NZDT)
+Commit: 9c1703580e6d96203e8a1c54e8adc97c25994014
+Version: 0.1.132 (2024-04-06@10:58:18+NZDT)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.132/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.133/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/directory.py` & `ansar-connect-0.1.133/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -2446,15 +2446,15 @@
 	self.forward(opened, self.return_address, self.connected.remote_address)
 	return CONNECTED
 
 def ConnectToPeer_CONNECTED_ClosePeer(self, message):
 	self.client_address.discard(self.return_address)
 	if len(self.client_address) < 1:
 		self.not_connected = 'Cleared last peer'
-		self.send(Close(ar.Aborted()), self.connected.return_address)
+		self.send(Close(ar.Aborted()), self.connected.remote_address)
 		self.start(ar.T1, 4.0)
 		return GLARING
 	return CONNECTED
 
 def ConnectToPeer_CONNECTED_Stop(self, message):
 	self.not_connected = 'Process termination'
 	return_address = self.connected.remote_address
```

### Comparing `ansar-connect-0.1.132/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.133/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.133/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/group_if.py` & `ansar-connect-0.1.133/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/grouping.py` & `ansar-connect-0.1.133/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/moving.py` & `ansar-connect-0.1.133/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/networking.py` & `ansar-connect-0.1.133/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.133/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/node.py` & `ansar-connect-0.1.133/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.133/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/procedure.py` & `ansar-connect-0.1.133/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/product.py` & `ansar-connect-0.1.133/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/socketry.py` & `ansar-connect-0.1.133/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/standard.py` & `ansar-connect-0.1.133/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/transporting.py` & `ansar-connect-0.1.133/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar/connect/wan.py` & `ansar-connect-0.1.133/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.132/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.133/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.132
+Version: 0.1.133
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.132/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.133/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

