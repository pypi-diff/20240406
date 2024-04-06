# Comparing `tmp/stomp.py-8.1.0.tar.gz` & `tmp/stomp_py-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stomp.py-8.1.0.tar", last modified: Sat Oct 29 18:19:08 2022, max compression
+gzip compressed data, was "stomp_py-8.1.1.tar", max compression
```

## Comparing `stomp.py-8.1.0.tar` & `stomp_py-8.1.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0    11358 2022-01-04 14:32:34.815789 stomp.py-8.1.0/LICENSE
--rw-r--r--   0        0        0     4854 2022-10-27 21:08:42.218840 stomp.py-8.1.0/README.rst
--rw-r--r--   0        0        0      976 2022-10-29 18:18:43.711199 stomp.py-8.1.0/pyproject.toml
--rw-r--r--   0        0        0     1338 2022-10-29 18:19:08.467303 stomp.py-8.1.0/stomp/__init__.py
--rw-r--r--   0        0        0    20853 2022-10-27 21:08:42.242840 stomp.py-8.1.0/stomp/__main__.py
--rw-r--r--   0        0        0       86 2022-10-27 21:08:42.242840 stomp.py-8.1.0/stomp/adapter/__init__.py
--rw-r--r--   0        0        0     6143 2022-10-27 21:08:42.242840 stomp.py-8.1.0/stomp/adapter/multicast.py
--rw-r--r--   0        0        0    19459 2022-10-27 21:08:42.242840 stomp.py-8.1.0/stomp/adapter/ws.py
--rw-r--r--   0        0        0      277 2022-01-04 14:36:21.951494 stomp.py-8.1.0/stomp/colours.py
--rw-r--r--   0        0        0     8575 2022-01-04 14:36:21.951494 stomp.py-8.1.0/stomp/connect.py
--rw-r--r--   0        0        0      685 2022-01-04 14:36:21.951494 stomp.py-8.1.0/stomp/constants.py
--rw-r--r--   0        0        0      859 2022-01-04 14:36:21.955494 stomp.py-8.1.0/stomp/exception.py
--rw-r--r--   0        0        0    20213 2022-10-27 21:08:42.242840 stomp.py-8.1.0/stomp/listener.py
--rw-r--r--   0        0        0      663 2022-01-04 14:36:21.955494 stomp.py-8.1.0/stomp/logging.py
--rw-r--r--   0        0        0    22759 2022-10-27 21:08:42.242840 stomp.py-8.1.0/stomp/protocol.py
--rw-r--r--   0        0        0    35167 2022-10-27 21:08:42.246840 stomp.py-8.1.0/stomp/transport.py
--rw-r--r--   0        0        0     8521 2022-10-27 21:08:42.246840 stomp.py-8.1.0/stomp/utils.py
--rw-r--r--   0        0        0     5836 2022-10-29 18:19:08.974002 stomp.py-8.1.0/setup.py
--rw-r--r--   0        0        0     5811 2022-10-29 18:19:08.974744 stomp.py-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-01-08 20:24:28.435496 stomp_py-8.1.1/LICENSE
+-rw-r--r--   0        0        0     4854 2022-08-01 07:39:51.672854 stomp_py-8.1.1/README.rst
+-rw-r--r--   0        0        0     1031 2023-03-11 17:16:41.468918 stomp_py-8.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-03-11 17:16:41.480919 stomp_py-8.1.1/stomp/__init__.py
+-rw-r--r--   0        0        0    20806 2023-03-22 21:16:43.493015 stomp_py-8.1.1/stomp/__main__.py
+-rw-r--r--   0        0        0       86 2022-11-13 16:44:23.491555 stomp_py-8.1.1/stomp/adapter/__init__.py
+-rw-r--r--   0        0        0     6143 2022-11-13 16:44:23.491555 stomp_py-8.1.1/stomp/adapter/multicast.py
+-rw-r--r--   0        0        0    18804 2023-03-11 11:48:42.973118 stomp_py-8.1.1/stomp/adapter/ws.py
+-rw-r--r--   0        0        0      277 2022-01-04 23:22:01.024428 stomp_py-8.1.1/stomp/colours.py
+-rw-r--r--   0        0        0     8575 2022-11-13 16:44:23.503555 stomp_py-8.1.1/stomp/connect.py
+-rw-r--r--   0        0        0      685 2022-11-13 16:44:23.503555 stomp_py-8.1.1/stomp/constants.py
+-rw-r--r--   0        0        0      859 2022-01-04 23:22:01.024428 stomp_py-8.1.1/stomp/exception.py
+-rw-r--r--   0        0        0    20213 2022-11-13 16:44:23.507556 stomp_py-8.1.1/stomp/listener.py
+-rw-r--r--   0        0        0      663 2022-10-22 18:46:40.395770 stomp_py-8.1.1/stomp/logging.py
+-rw-r--r--   0        0        0    22859 2023-06-06 20:38:54.908052 stomp_py-8.1.1/stomp/protocol.py
+-rw-r--r--   0        0        0    35167 2022-11-13 16:44:23.507556 stomp_py-8.1.1/stomp/transport.py
+-rw-r--r--   0        0        0     8521 2022-11-13 16:44:23.511556 stomp_py-8.1.1/stomp/utils.py
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 stomp_py-8.1.1/PKG-INFO
```

### Comparing `stomp.py-8.1.0/LICENSE` & `stomp_py-8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/README.rst` & `stomp_py-8.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/pyproject.toml` & `stomp_py-8.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stomp.py"
-version = "8.1.0"
+version = "8.1.1"
 description = "Python STOMP client, supporting versions 1.0, 1.1 and 1.2 of the protocol"
 authors = ["Jason R Briggs <jasonrbriggs@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/jasonrbriggs/stomp.py"
 documentation = "http://jasonrbriggs.github.io/stomp.py/"
 keywords = ["stomp", "messaging", "events", "client"]
@@ -15,24 +15,26 @@
 ]
 
 packages = [
     { include = "stomp" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 docopt = "^0.6.2"
 websocket-client = "^1.2.3"
 
 [tool.poetry.dev-dependencies]
-pytest = ">=5.2"
-pytest-cov = ">=2.8.1"
-pytest-mock = ">=2.0.0"
-pytest-html = ">=2.0.1"
+pytest = ">=7.2.0"
+pytest-cov = ">=4.0.0"
+pytest-mock = ">=3.10.0"
+pytest-html = ">=3.2.0"
 pytest-ordering = ">=0.6"
 
 [tool.poetry.scripts]
 stomp = "stomp.__main__:main"
 
+[tool.poetry_bumpversion.file."stomp/__init__.py"]
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `stomp.py-8.1.0/stomp/__init__.py` & `stomp_py-8.1.1/stomp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 
 import stomp.adapter as adapter
 import stomp.connect as connect
 import stomp.listener as listener
 import stomp.logging as logging
 
-__version__ = (8, 1, 0)
+__version__ = "8.1.1"
 
 ##
 # Alias for STOMP 1.0 connections.
 #
 Connection10 = connect.StompConnection10
 StompConnection10 = Connection10
```

### Comparing `stomp.py-8.1.0/stomp/__main__.py` & `stomp_py-8.1.1/stomp/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,14 @@
 from stomp.adapter.multicast import MulticastConnection
 from stomp.connect import StompConnection10, StompConnection11, StompConnection12
 from stomp.listener import ConnectionListener, StatsListener
 
 sys.path.append(".")
 import stomp
 
-version_string = "%s.%s.%s" % stomp.__version__
-
 heartbeat_pattern = re.compile(r"[0-9]+,[0-9]+")
 
 
 class SubscriptionInfo(object):
     """
     Used to store info about a subscription.
     """
@@ -366,15 +364,15 @@
         self.help("sendfile <destination> <filename> [headers.json]",
                   "Sends a file to a destination in the messaging system.",
                   ["destination - where to send the message", "filename - the file to send",
                    "headers.json - json map with headers to send"])
 
     def do_version(self, args):
         self.__sysout("%s%s [Protocol version %s]%s" %
-                      (stomp.colours.BOLD, version_string, self.conn.version, stomp.colours.NO_COLOUR))
+                      (stomp.colours.BOLD, stomp.version, self.conn.version, stomp.colours.NO_COLOUR))
     do_ver = do_version
 
     def help_version(self):
         self.help("version", "Display the version of the client")
     help_ver = help_version
 
     def check_ack_nack(self, acknackfunc, args):
@@ -500,15 +498,15 @@
 
 def do_nothing_loop():
     while 1:
         time.sleep(1)
 
 
 def main():
-    arguments = docopt(__doc__, version=version_string)
+    arguments = docopt(__doc__, version=stomp.__version__)
 
     if arguments["--listen"] is not None:
         prompt = ""
     else:
         prompt = "> "
 
     if not heartbeat_pattern.match(arguments["--heartbeats"]):
```

### Comparing `stomp.py-8.1.0/stomp/adapter/multicast.py` & `stomp_py-8.1.1/stomp/adapter/multicast.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/adapter/ws.py` & `stomp_py-8.1.1/stomp/adapter/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,35 +166,21 @@
 
     def disconnect_socket(self):
         """
         Disconnect the underlying socket connection
         """
         self.running = False
         if self.socket is not None:
-            if self.__need_ssl():
-                #
-                # Even though we don't want to use the socket, unwrap is the only API method which does a proper SSL
-                # shutdown
-                #
-                try:
-                    self.socket = self.socket.unwrap()
-                except Exception:
-                    #
-                    # unwrap seems flaky on Win with the back-ported ssl mod, so catch any exception and log it
-                    #
-                    _, e, _ = sys.exc_info()
-                    logging.warning(e)
-            elif hasattr(socket, "SHUT_RDWR"):
-                try:
-                    self.socket.shutdown(socket.SHUT_RDWR)
-                except socket.error:
-                    _, e, _ = sys.exc_info()
-                    # ignore when socket already closed
-                    if get_errno(e) != errno.ENOTCONN:
-                        logging.warning("Unable to issue SHUT_RDWR on socket because of error '%s'", e)
+            try:
+                self.socket.shutdown()
+            except socket.error:
+                _, e, _ = sys.exc_info()
+                # ignore when socket already closed
+                if get_errno(e) != errno.ENOTCONN:
+                    logging.warning("Unable to issue SHUT_RDWR on socket because of error '%s'", e)
 
         #
         # split this into a separate check, because sometimes the socket is nulled between shutdown and this call
         #
         if self.socket is not None:
             try:
                 self.socket.close()
```

### Comparing `stomp.py-8.1.0/stomp/connect.py` & `stomp_py-8.1.1/stomp/connect.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/constants.py` & `stomp_py-8.1.1/stomp/constants.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/exception.py` & `stomp_py-8.1.1/stomp/exception.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/listener.py` & `stomp_py-8.1.1/stomp/listener.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/logging.py` & `stomp_py-8.1.1/stomp/logging.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/protocol.py` & `stomp_py-8.1.1/stomp/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,16 @@
         """
         cmd = CMD_CONNECT if with_connect_command else CMD_STOMP
         headers = utils.merge_headers([headers, keyword_headers])
         headers[HDR_ACCEPT_VERSION] = self.version
 
         if self.transport.vhost:
             headers[HDR_HOST] = self.transport.vhost
+        else:
+            headers[HDR_HOST] = "/"
 
         if username is not None:
             headers[HDR_LOGIN] = username
 
         if passcode is not None:
             headers[HDR_PASSCODE] = passcode
 
@@ -512,14 +514,16 @@
         cmd = CMD_CONNECT if with_connect_command else CMD_STOMP
         headers = utils.merge_headers([headers, keyword_headers])
         headers[HDR_ACCEPT_VERSION] = self.version
         headers[HDR_HOST] = self.transport.current_host_and_port[0]
 
         if self.transport.vhost:
             headers[HDR_HOST] = self.transport.vhost
+        else:
+            headers[HDR_HOST] = "/"
 
         if username is not None:
             headers[HDR_LOGIN] = username
 
         if passcode is not None:
             headers[HDR_PASSCODE] = passcode
```

### Comparing `stomp.py-8.1.0/stomp/transport.py` & `stomp_py-8.1.1/stomp/transport.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/stomp/utils.py` & `stomp_py-8.1.1/stomp/utils.py`

 * *Files identical despite different names*

### Comparing `stomp.py-8.1.0/setup.py` & `stomp_py-8.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,142 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: stomp-py
+Version: 8.1.1
+Summary: Python STOMP client, supporting versions 1.0, 1.1 and 1.2 of the protocol
+Home-page: https://github.com/jasonrbriggs/stomp.py
+License: Apache-2.0
+Keywords: stomp,messaging,events,client
+Author: Jason R Briggs
+Author-email: jasonrbriggs@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: websocket-client (>=1.2.3,<2.0.0)
+Project-URL: Documentation, http://jasonrbriggs.github.io/stomp.py/
+Project-URL: Repository, https://github.com/jasonrbriggs/stomp.py
+Description-Content-Type: text/x-rst
 
-packages = \
-['stomp', 'stomp.adapter']
+========
+stomp.py
+========
 
-package_data = \
-{'': ['*']}
+.. image:: https://badge.fury.io/py/stomp.py.svg
+    :target: https://badge.fury.io/py/stomp.py
+    :alt: PyPI version
 
-install_requires = \
-['docopt>=0.6.2,<0.7.0', 'websocket-client>=1.2.3,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['stomp = stomp.__main__:main']}
-
-setup_kwargs = {
-    'name': 'stomp.py',
-    'version': '8.1.0',
-    'description': 'Python STOMP client, supporting versions 1.0, 1.1 and 1.2 of the protocol',
-    'long_description': '========\nstomp.py\n========\n\n.. image:: https://badge.fury.io/py/stomp.py.svg\n    :target: https://badge.fury.io/py/stomp.py\n    :alt: PyPI version\n\n"stomp.py" is a Python client library for accessing messaging servers (such as ActiveMQ_, Artemis_ or RabbitMQ_) using the STOMP_ protocol (`STOMP v1.0`_, `STOMP v1.1`_ and `STOMP v1.2`_). It can also be run as a standalone, command-line client for testing.  NOTE: Stomp.py has officially ended support for Python2.x. See `python3statement.org`_ for more information. \n\n.. contents:: \\ \n    :depth: 1\n\n\nQuick Start\n===========\n\nYou can connect to a message broker running on the local machine, and send a message using the following example.\n\n.. code-block:: python\n\n  import stomp\n\n  conn = stomp.Connection()\n  conn.connect(\'admin\', \'password\', wait=True)\n  conn.send(body=\' \'.join(sys.argv[1:]), destination=\'/queue/test\')\n  conn.disconnect()\n\n\nDocumentation and Resources\n===========================\n\n- `Main documentation`_\n- `API documentation`_ (see `stomp.github.io`_ for details on the STOMP protocol itself)\n- A basic example of using stomp.py with a message listener can be found in the `quick start`_ section of the main documentation\n- Description of the `command-line interface`_\n- `Travis`_ for continuous integration builds\n- Current `test coverage report`_\n- `PyPi stomp.py page`_\n\nThe current version of stomp.py supports:\n\n- Python 3.x (Python2 support ended as of Jan 2020)\n- STOMP version 1.0, 1.1 and 1.2\n\nThere is also legacy 3.1.7 version using the old 3-series code (see `3.1.7 on PyPi`_ and `3.1.7 on GitHub`_). This is no longer supported, but (at least as of 2018) there were still a couple of reports of this version still being used in the wild.\n\nNote: stomp.py now follows `semantic versioning`_:\n\n- MAJOR version for incompatible API changes,\n- MINOR version for functionality added in a backwards compatible manner, and\n- PATCH version for backwards compatible bug fixes.\n\n\n\nTesting\n=======\n\nstomp.py has been perfunctorily tested on:\n\n- Pivotal `RabbitMQ`_   (`test_rabbitmq.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_rabbitmq.py>`_)\n- Apache `ActiveMQ`_   (`test_activemq.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_activemq.py>`_)\n- Apache ActiveMQ `Artemis`_  (`test_artemis.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_artemis.py>`_)\n- `stompserver`_  (`test_stompserver.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_stompserver.py>`_)\n\nFor testing locally, you\'ll need to install docker (or `podman`_). Once installed:\n\n#. Install dependencies:\n        ``poetry install``\n#. Create the docker (or podman) image:\n        ``make docker-image`` (or ``make podman-image``)\n#. Run the container:\n        ``make run-docker`` (or ``make run-podman``)\n#. Run stomp.py unit tests:\n        ``make test``\n#. Cleanup the container afterwards if you don\'t need it any more:\n        ``make remove-docker`` (or ``make remove-podman``)\n\nIf you want to connect to the test services locally (other than from the included tests), you\'ll want to add test domain names to your hosts file like so:\n      |  172.17.0.2  my.example.com\n      |  172.17.0.2  my.example.org\n      |  172.17.0.2  my.example.net\n\nIf you\'re using `podman`_ and you want to access services via their private IP addresses, you\'ll want to run your commands with::\n\n  podman unshare --rootless-netns <command>\n\nso that <command> has access to the private container network. Service ports are also exposed to the host and can be accessed directly.\n\n\n.. _`STOMP`: http://stomp.github.io\n.. _`STOMP v1.0`: http://stomp.github.io/stomp-specification-1.0.html\n.. _`STOMP v1.1`: http://stomp.github.io/stomp-specification-1.1.html\n.. _`STOMP v1.2`: http://stomp.github.io/stomp-specification-1.2.html\n.. _`python3statement.org`: http://python3statement.org/\n\n.. _`Main documentation`: http://jasonrbriggs.github.io/stomp.py/index.html\n.. _`stomp.github.io`: http://stomp.github.io/\n.. _`quick start`: http://jasonrbriggs.github.io/stomp.py/quickstart.html\n.. _`command-line interface`: http://jasonrbriggs.github.io/stomp.py/commandline.html\n.. _`PyPi stomp.py page`: https://pypi.org/project/stomp.py/\n.. _`API documentation`: http://jasonrbriggs.github.io/stomp.py/api.html\n.. _`test coverage report`: http://jasonrbriggs.github.io/stomp.py/htmlcov/\n.. _`Travis`: https://travis-ci.org/jasonrbriggs/stomp.py\n\n.. _`3.1.7 on PyPi`: https://pypi.org/project/stomp.py/3.1.7/\n.. _`3.1.7 on GitHub`: https://github.com/jasonrbriggs/stomp.py/tree/stomppy-3series\n\n.. _`ActiveMQ`:  http://activemq.apache.org/\n.. _`Artemis`: https://activemq.apache.org/components/artemis/\n.. _`RabbitMQ`: http://www.rabbitmq.com\n.. _`stompserver`: http://stompserver.rubyforge.org\n\n.. _`semantic versioning`: https://semver.org/\n\n.. _`podman`: https://podman.io/\n',
-    'author': 'Jason R Briggs',
-    'author_email': 'jasonrbriggs@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/jasonrbriggs/stomp.py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+"stomp.py" is a Python client library for accessing messaging servers (such as ActiveMQ_, Artemis_ or RabbitMQ_) using the STOMP_ protocol (`STOMP v1.0`_, `STOMP v1.1`_ and `STOMP v1.2`_). It can also be run as a standalone, command-line client for testing.  NOTE: Stomp.py has officially ended support for Python2.x. See `python3statement.org`_ for more information. 
 
+.. contents:: \ 
+    :depth: 1
+
+
+Quick Start
+===========
+
+You can connect to a message broker running on the local machine, and send a message using the following example.
+
+.. code-block:: python
+
+  import stomp
+
+  conn = stomp.Connection()
+  conn.connect('admin', 'password', wait=True)
+  conn.send(body=' '.join(sys.argv[1:]), destination='/queue/test')
+  conn.disconnect()
+
+
+Documentation and Resources
+===========================
+
+- `Main documentation`_
+- `API documentation`_ (see `stomp.github.io`_ for details on the STOMP protocol itself)
+- A basic example of using stomp.py with a message listener can be found in the `quick start`_ section of the main documentation
+- Description of the `command-line interface`_
+- `Travis`_ for continuous integration builds
+- Current `test coverage report`_
+- `PyPi stomp.py page`_
+
+The current version of stomp.py supports:
+
+- Python 3.x (Python2 support ended as of Jan 2020)
+- STOMP version 1.0, 1.1 and 1.2
+
+There is also legacy 3.1.7 version using the old 3-series code (see `3.1.7 on PyPi`_ and `3.1.7 on GitHub`_). This is no longer supported, but (at least as of 2018) there were still a couple of reports of this version still being used in the wild.
+
+Note: stomp.py now follows `semantic versioning`_:
+
+- MAJOR version for incompatible API changes,
+- MINOR version for functionality added in a backwards compatible manner, and
+- PATCH version for backwards compatible bug fixes.
+
+
+
+Testing
+=======
+
+stomp.py has been perfunctorily tested on:
+
+- Pivotal `RabbitMQ`_   (`test_rabbitmq.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_rabbitmq.py>`_)
+- Apache `ActiveMQ`_   (`test_activemq.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_activemq.py>`_)
+- Apache ActiveMQ `Artemis`_  (`test_artemis.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_artemis.py>`_)
+- `stompserver`_  (`test_stompserver.py <https://github.com/jasonrbriggs/stomp.py/blob/dev/tests/test_stompserver.py>`_)
+
+For testing locally, you'll need to install docker (or `podman`_). Once installed:
+
+#. Install dependencies:
+        ``poetry install``
+#. Create the docker (or podman) image:
+        ``make docker-image`` (or ``make podman-image``)
+#. Run the container:
+        ``make run-docker`` (or ``make run-podman``)
+#. Run stomp.py unit tests:
+        ``make test``
+#. Cleanup the container afterwards if you don't need it any more:
+        ``make remove-docker`` (or ``make remove-podman``)
+
+If you want to connect to the test services locally (other than from the included tests), you'll want to add test domain names to your hosts file like so:
+      |  172.17.0.2  my.example.com
+      |  172.17.0.2  my.example.org
+      |  172.17.0.2  my.example.net
+
+If you're using `podman`_ and you want to access services via their private IP addresses, you'll want to run your commands with::
+
+  podman unshare --rootless-netns <command>
+
+so that <command> has access to the private container network. Service ports are also exposed to the host and can be accessed directly.
+
+
+.. _`STOMP`: http://stomp.github.io
+.. _`STOMP v1.0`: http://stomp.github.io/stomp-specification-1.0.html
+.. _`STOMP v1.1`: http://stomp.github.io/stomp-specification-1.1.html
+.. _`STOMP v1.2`: http://stomp.github.io/stomp-specification-1.2.html
+.. _`python3statement.org`: http://python3statement.org/
+
+.. _`Main documentation`: http://jasonrbriggs.github.io/stomp.py/index.html
+.. _`stomp.github.io`: http://stomp.github.io/
+.. _`quick start`: http://jasonrbriggs.github.io/stomp.py/quickstart.html
+.. _`command-line interface`: http://jasonrbriggs.github.io/stomp.py/commandline.html
+.. _`PyPi stomp.py page`: https://pypi.org/project/stomp.py/
+.. _`API documentation`: http://jasonrbriggs.github.io/stomp.py/api.html
+.. _`test coverage report`: http://jasonrbriggs.github.io/stomp.py/htmlcov/
+.. _`Travis`: https://travis-ci.org/jasonrbriggs/stomp.py
+
+.. _`3.1.7 on PyPi`: https://pypi.org/project/stomp.py/3.1.7/
+.. _`3.1.7 on GitHub`: https://github.com/jasonrbriggs/stomp.py/tree/stomppy-3series
+
+.. _`ActiveMQ`:  http://activemq.apache.org/
+.. _`Artemis`: https://activemq.apache.org/components/artemis/
+.. _`RabbitMQ`: http://www.rabbitmq.com
+.. _`stompserver`: http://stompserver.rubyforge.org
+
+.. _`semantic versioning`: https://semver.org/
+
+.. _`podman`: https://podman.io/
 
-setup(**setup_kwargs)
```

