# Comparing `tmp/hashed-1.0.0.tar.gz` & `tmp/hashed-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashed-1.0.0.tar", last modified: Sat Apr  6 05:45:20 2024, max compression
+gzip compressed data, was "hashed-2.0.0.tar", last modified: Sat Apr  6 07:20:52 2024, max compression
```

## Comparing `hashed-1.0.0.tar` & `hashed-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 05:45:20.007999 hashed-1.0.0/
--rw-rw-rw-   0        0        0     1092 2024-04-06 05:12:18.000000 hashed-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2276 2024-04-06 05:45:20.007249 hashed-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1656 2024-04-06 05:31:35.000000 hashed-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 05:45:19.994019 hashed-1.0.0/hashed.egg-info/
--rw-rw-rw-   0        0        0     2276 2024-04-06 05:45:19.000000 hashed-1.0.0/hashed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-06 05:45:19.000000 hashed-1.0.0/hashed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 05:45:19.000000 hashed-1.0.0/hashed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 05:45:19.000000 hashed-1.0.0/hashed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 05:45:20.007999 hashed-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-04-06 05:44:43.000000 hashed-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 05:45:20.006250 hashed-1.0.0/src/
--rw-rw-rw-   0        0        0       28 2024-04-06 05:12:18.000000 hashed-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0      718 2024-04-06 05:12:18.000000 hashed-1.0.0/src/buffer_reader.py
--rw-rw-rw-   0        0        0     2652 2024-04-06 05:12:18.000000 hashed-1.0.0/src/cli.py
--rw-rw-rw-   0        0        0      700 2024-04-06 05:12:18.000000 hashed-1.0.0/src/common.py
--rw-rw-rw-   0        0        0      804 2024-04-06 05:12:18.000000 hashed-1.0.0/src/hash.py
--rw-rw-rw-   0        0        0      335 2024-04-06 05:12:18.000000 hashed-1.0.0/src/hash_lib.py
--rw-rw-rw-   0        0        0     6183 2024-04-06 05:12:18.000000 hashed-1.0.0/src/sha256.py
--rw-rw-rw-   0        0        0     7247 2024-04-06 05:12:18.000000 hashed-1.0.0/src/sha512.py
-drwxrwxrwx   0        0        0        0 2024-04-06 05:45:20.007249 hashed-1.0.0/test/
--rw-rw-rw-   0        0        0        0 2024-04-06 05:23:42.000000 hashed-1.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:20:52.532006 hashed-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 07:20:44.000000 hashed-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-06 07:20:52.532006 hashed-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 07:20:44.000000 hashed-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:20:52.532006 hashed-2.0.0/hashed/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/buffer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/hash_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-06 07:20:44.000000 hashed-2.0.0/hashed/sha512.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:20:52.532006 hashed-2.0.0/hashed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-06 07:20:52.000000 hashed-2.0.0/hashed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-06 07:20:52.000000 hashed-2.0.0/hashed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:20:52.000000 hashed-2.0.0/hashed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 07:20:52.000000 hashed-2.0.0/hashed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:20:52.536006 hashed-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-06 07:20:44.000000 hashed-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:20:52.532006 hashed-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 07:20:44.000000 hashed-2.0.0/test/__init__.py
```

### Comparing `hashed-1.0.0/LICENSE` & `hashed-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Mukund Agarwal
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
+Copyright (c) 2024 Mukund Agarwal
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

### Comparing `hashed-1.0.0/PKG-INFO` & `hashed-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,74 @@
-Metadata-Version: 2.1
-Name: hashed
-Version: 1.0.0
-Summary: Provides secured hashes for given data
-Home-page: https://github.com/mukund26/hashed
-Author: Mukund Agarwal
-Author-email: m.agarwalhp@gmail.com
-License: MIT
-Keywords: python,hashing,sha256,sha512
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-> A simple SHA-2 implementation in python which gives hash for string or a file.
-> It calculates SHA-256 and SHA-512 right now
-
-## Usage - as CLI Tool
-
-* Example
-
-```python
-python src/cli.py -s "Hello World!!" --sha256
-```
-
-* For help
-```python
-usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
-
-Provides secured hashes for given data
-
-options:
-  -h, --help            show this help message and exit
-  --sha256              Generates SHA-256 for given input (default: False)
-  --sha512              Generates SHA-512 for given input (default: False)
-  -s STRING, --string STRING
-                        String to be hashed (default: None)
-  -f FILE, --file FILE  File to be hashed (default: None)
-  -fb BINARY_FILE, --binary_file BINARY_FILE
-                        Binary file to be hashed (default: None)
-  -t, --test            Test accuracy of algorithm (default: False)
-  -p, --perf            Log performance of the algorithm (default: False)
-  -b, --bits            Returns size of hashed message in bytes (default: False)
-
-Currently supported hashes [SHA256, SHA512]
-```
-
-
-## Usage - as Library
-
-```python
-from hashed import HashLib
-h = HashLib('sha256').hasher_class()
-h.hex_digest("Hello World")
-```
-
-## Functions Supported
-
-- hex_digest
-- file_digest
-- digest
-- hashed_bits
-- digest_size
-
-## For Algo refer: [SHA-256 Wiki](https://en.wikipedia.org/wiki/SHA-2)
-
-## For more refer:
-
-- https://blog.boot.dev/cryptography/how-sha-2-works-step-by-step-sha-256/
-- https://github.com/mukund26/softwareEnggGuide/blob/main/sha256-384-512.pdf
-
-
+Metadata-Version: 2.1
+Name: hashed
+Version: 2.0.0
+Summary: Provides secured hashes for given data
+Home-page: https://github.com/mukund26/hashed
+Author: Mukund Agarwal
+Author-email: m.agarwalhp@gmail.com
+License: MIT
+Keywords: python,hashing,sha256,sha512
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+> A simple SHA-2 implementation in python which gives hash for string or a file.
+> It calculates SHA-256 and SHA-512 right now
+
+## Usage - as CLI Tool
+
+* Example
+
+```python
+python src/cli.py -s "Hello World!!" --sha256
+```
+
+* For help
+```python
+usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
+
+Provides secured hashes for given data
+
+options:
+  -h, --help            show this help message and exit
+  --sha256              Generates SHA-256 for given input (default: False)
+  --sha512              Generates SHA-512 for given input (default: False)
+  -s STRING, --string STRING
+                        String to be hashed (default: None)
+  -f FILE, --file FILE  File to be hashed (default: None)
+  -fb BINARY_FILE, --binary_file BINARY_FILE
+                        Binary file to be hashed (default: None)
+  -t, --test            Test accuracy of algorithm (default: False)
+  -p, --perf            Log performance of the algorithm (default: False)
+  -b, --bits            Returns size of hashed message in bytes (default: False)
+
+Currently supported hashes [SHA256, SHA512]
+```
+
+
+## Usage - as Library
+
+```python
+from hashed import HashLib
+h = HashLib('sha256').hasher_class()
+h.hex_digest("Hello World")
+```
+
+## Functions Supported
+
+- hex_digest
+- file_digest
+- digest
+- hashed_bits
+- digest_size
+
+## For Algo refer: [SHA-256 Wiki](https://en.wikipedia.org/wiki/SHA-2)
+
+## For more refer:
+
+- https://blog.boot.dev/cryptography/how-sha-2-works-step-by-step-sha-256/
+- https://github.com/mukund26/softwareEnggGuide/blob/main/sha256-384-512.pdf
```

### Comparing `hashed-1.0.0/README.md` & `hashed-2.0.0/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-> A simple SHA-2 implementation in python which gives hash for string or a file.
-> It calculates SHA-256 and SHA-512 right now
-
-## Usage - as CLI Tool
-
-* Example
-
-```python
-python src/cli.py -s "Hello World!!" --sha256
-```
-
-* For help
-```python
-usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
-
-Provides secured hashes for given data
-
-options:
-  -h, --help            show this help message and exit
-  --sha256              Generates SHA-256 for given input (default: False)
-  --sha512              Generates SHA-512 for given input (default: False)
-  -s STRING, --string STRING
-                        String to be hashed (default: None)
-  -f FILE, --file FILE  File to be hashed (default: None)
-  -fb BINARY_FILE, --binary_file BINARY_FILE
-                        Binary file to be hashed (default: None)
-  -t, --test            Test accuracy of algorithm (default: False)
-  -p, --perf            Log performance of the algorithm (default: False)
-  -b, --bits            Returns size of hashed message in bytes (default: False)
-
-Currently supported hashes [SHA256, SHA512]
-```
-
-
-## Usage - as Library
-
-```python
-from hashed import HashLib
-h = HashLib('sha256').hasher_class()
-h.hex_digest("Hello World")
-```
-
-## Functions Supported
-
-- hex_digest
-- file_digest
-- digest
-- hashed_bits
-- digest_size
-
-## For Algo refer: [SHA-256 Wiki](https://en.wikipedia.org/wiki/SHA-2)
-
-## For more refer:
-
-- https://blog.boot.dev/cryptography/how-sha-2-works-step-by-step-sha-256/
-- https://github.com/mukund26/softwareEnggGuide/blob/main/sha256-384-512.pdf
+> A simple SHA-2 implementation in python which gives hash for string or a file.
+> It calculates SHA-256 and SHA-512 right now
+
+## Usage - as CLI Tool
+
+* Example
+
+```python
+python src/cli.py -s "Hello World!!" --sha256
+```
+
+* For help
+```python
+usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
+
+Provides secured hashes for given data
+
+options:
+  -h, --help            show this help message and exit
+  --sha256              Generates SHA-256 for given input (default: False)
+  --sha512              Generates SHA-512 for given input (default: False)
+  -s STRING, --string STRING
+                        String to be hashed (default: None)
+  -f FILE, --file FILE  File to be hashed (default: None)
+  -fb BINARY_FILE, --binary_file BINARY_FILE
+                        Binary file to be hashed (default: None)
+  -t, --test            Test accuracy of algorithm (default: False)
+  -p, --perf            Log performance of the algorithm (default: False)
+  -b, --bits            Returns size of hashed message in bytes (default: False)
+
+Currently supported hashes [SHA256, SHA512]
+```
+
+
+## Usage - as Library
+
+```python
+from hashed import HashLib
+h = HashLib('sha256').hasher_class()
+h.hex_digest("Hello World")
+```
+
+## Functions Supported
+
+- hex_digest
+- file_digest
+- digest
+- hashed_bits
+- digest_size
+
+## For Algo refer: [SHA-256 Wiki](https://en.wikipedia.org/wiki/SHA-2)
+
+## For more refer:
+
+- https://blog.boot.dev/cryptography/how-sha-2-works-step-by-step-sha-256/
+- https://github.com/mukund26/softwareEnggGuide/blob/main/sha256-384-512.pdf
```

### Comparing `hashed-1.0.0/hashed.egg-info/PKG-INFO` & `hashed-2.0.0/hashed.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,74 @@
-Metadata-Version: 2.1
-Name: hashed
-Version: 1.0.0
-Summary: Provides secured hashes for given data
-Home-page: https://github.com/mukund26/hashed
-Author: Mukund Agarwal
-Author-email: m.agarwalhp@gmail.com
-License: MIT
-Keywords: python,hashing,sha256,sha512
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-> A simple SHA-2 implementation in python which gives hash for string or a file.
-> It calculates SHA-256 and SHA-512 right now
-
-## Usage - as CLI Tool
-
-* Example
-
-```python
-python src/cli.py -s "Hello World!!" --sha256
-```
-
-* For help
-```python
-usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
-
-Provides secured hashes for given data
-
-options:
-  -h, --help            show this help message and exit
-  --sha256              Generates SHA-256 for given input (default: False)
-  --sha512              Generates SHA-512 for given input (default: False)
-  -s STRING, --string STRING
-                        String to be hashed (default: None)
-  -f FILE, --file FILE  File to be hashed (default: None)
-  -fb BINARY_FILE, --binary_file BINARY_FILE
-                        Binary file to be hashed (default: None)
-  -t, --test            Test accuracy of algorithm (default: False)
-  -p, --perf            Log performance of the algorithm (default: False)
-  -b, --bits            Returns size of hashed message in bytes (default: False)
-
-Currently supported hashes [SHA256, SHA512]
-```
-
-
-## Usage - as Library
-
-```python
-from hashed import HashLib
-h = HashLib('sha256').hasher_class()
-h.hex_digest("Hello World")
-```
-
-## Functions Supported
-
-- hex_digest
-- file_digest
-- digest
-- hashed_bits
-- digest_size
-
-## For Algo refer: [SHA-256 Wiki](https://en.wikipedia.org/wiki/SHA-2)
-
-## For more refer:
-
-- https://blog.boot.dev/cryptography/how-sha-2-works-step-by-step-sha-256/
-- https://github.com/mukund26/softwareEnggGuide/blob/main/sha256-384-512.pdf
-
-
+Metadata-Version: 2.1
+Name: hashed
+Version: 2.0.0
+Summary: Provides secured hashes for given data
+Home-page: https://github.com/mukund26/hashed
+Author: Mukund Agarwal
+Author-email: m.agarwalhp@gmail.com
+License: MIT
+Keywords: python,hashing,sha256,sha512
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+> A simple SHA-2 implementation in python which gives hash for string or a file.
+> It calculates SHA-256 and SHA-512 right now
+
+## Usage - as CLI Tool
+
+* Example
+
+```python
+python src/cli.py -s "Hello World!!" --sha256
+```
+
+* For help
+```python
+usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
+
+Provides secured hashes for given data
+
+options:
+  -h, --help            show this help message and exit
+  --sha256              Generates SHA-256 for given input (default: False)
+  --sha512              Generates SHA-512 for given input (default: False)
+  -s STRING, --string STRING
+                        String to be hashed (default: None)
+  -f FILE, --file FILE  File to be hashed (default: None)
+  -fb BINARY_FILE, --binary_file BINARY_FILE
+                        Binary file to be hashed (default: None)
+  -t, --test            Test accuracy of algorithm (default: False)
+  -p, --perf            Log performance of the algorithm (default: False)
+  -b, --bits            Returns size of hashed message in bytes (default: False)
+
+Currently supported hashes [SHA256, SHA512]
+```
+
+
+## Usage - as Library
+
+```python
+from hashed import HashLib
+h = HashLib('sha256').hasher_class()
+h.hex_digest("Hello World")
+```
+
+## Functions Supported
+
+- hex_digest
+- file_digest
+- digest
+- hashed_bits
+- digest_size
+
+## For Algo refer: [SHA-256 Wiki](https://en.wikipedia.org/wiki/SHA-2)
+
+## For more refer:
+
+- https://blog.boot.dev/cryptography/how-sha-2-works-step-by-step-sha-256/
+- https://github.com/mukund26/softwareEnggGuide/blob/main/sha256-384-512.pdf
```

### Comparing `hashed-1.0.0/src/buffer_reader.py` & `hashed-2.0.0/hashed/buffer_reader.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import io
-
-class BufferedReader:
-    def __init__(self, reader):
-        self.reader = reader
-        self.buffer = []
-
-    def read(self, size=-1):
-        if not self.buffer:
-            self.buffer = self.reader.read(io.DEFAULT_BUFFER_SIZE)
-        if size == -1:
-            size = len(self.buffer)
-        data = self.buffer[:size]
-        self.buffer = self.buffer[size:]
-        return data
-
-    def readline(self):
-        while True:
-            line = self.reader.readline()
-            if not line:
-                return line
-            if line.endswith('\n'):
-                return line
-            self.buffer.append(line)
-
-    def close(self):
-        self.reader.close()
-
+import io
+
+class BufferedReader:
+    def __init__(self, reader):
+        self.reader = reader
+        self.buffer = []
+
+    def read(self, size=-1):
+        if not self.buffer:
+            self.buffer = self.reader.read(io.DEFAULT_BUFFER_SIZE)
+        if size == -1:
+            size = len(self.buffer)
+        data = self.buffer[:size]
+        self.buffer = self.buffer[size:]
+        return data
+
+    def readline(self):
+        while True:
+            line = self.reader.readline()
+            if not line:
+                return line
+            if line.endswith('\n'):
+                return line
+            self.buffer.append(line)
+
+    def close(self):
+        self.reader.close()
+
```

### Comparing `hashed-1.0.0/src/cli.py` & `hashed-2.0.0/hashed/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import argparse
-from hash_lib import HashLib
-import time
-
-def setup_args():
-    parser = argparse.ArgumentParser(
-                    prog='Hashing Library',
-                    description='Provides secured hashes for given data',
-                    epilog='Currently supported hashes [SHA256, SHA512]',
-                    formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    
-    parser.add_argument("--sha256", action='store_true', help="Generates SHA-256 for given input")
-    parser.add_argument("--sha512", action='store_true', help="Generates SHA-512 for given input")
-    parser.add_argument("-s", "--string", help="String to be hashed")
-    parser.add_argument("-f", "--file", help="File to be hashed")
-    parser.add_argument("-fb", "--binary_file", help='Binary file to be hashed')
-    parser.add_argument("-t", "--test", action='store_true', help='Test accuracy of algorithm')
-    parser.add_argument("-p", "--perf", action='store_true', help='Log performance of the algorithm')
-    parser.add_argument("-b", "--bits", action='store_true', help='Returns size of hashed message in bytes')
-    return parser
-
-
-if __name__ == '__main__':
-    parser = setup_args()
-    args = vars(parser.parse_args())
-    
-    if args['sha256']:
-        start_time = time.time()
-        h = HashLib('sha256').hasher_class()
-        if args['string']:
-            print('Hash: ', h.hex_digest(args["string"]))
-            end_time = time.time()
-        if args['file']:
-            print('Hash: ', h.file_digest(args["file"], False))
-            end_time = time.time()
-        if args['binary_file']:
-            print('Hash: ', h.file_digest(args['binary_file'], True))
-            end_time = time.time()
-        if args['bits']:
-            print("Bytes Hashed: ", h.hashed_bits/8)
-        if args['perf']:
-            print(f'Time Taken: {end_time - start_time} seconds')
-            
-    elif args['sha512']:
-        start_time = time.time()
-        h = HashLib('sha512').hasher_class()
-        if args['string']:
-            print('Hash: ', h.hex_digest(args["string"]))
-            end_time = time.time()
-        if args['file']:
-            print('Hash: ', h.file_digest(args["file"], False))
-            end_time = time.time()
-        if args['binary_file']:
-            print('Hash: ', h.file_digest(args['binary_file'], True))
-            end_time = time.time()
-        if args['bits']:
-            print("Bytes Hashed: ", h.hashed_bits/8)
-        if args['perf']:
-            print(f'Time Taken: {end_time - start_time} seconds')
-            
-    else:
+import argparse
+from hashed.hash_lib import HashLib
+import time
+
+def setup_args():
+    parser = argparse.ArgumentParser(
+                    prog='Hashing Library',
+                    description='Provides secured hashes for given data',
+                    epilog='Currently supported hashes [SHA256, SHA512]',
+                    formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    
+    parser.add_argument("--sha256", action='store_true', help="Generates SHA-256 for given input")
+    parser.add_argument("--sha512", action='store_true', help="Generates SHA-512 for given input")
+    parser.add_argument("-s", "--string", help="String to be hashed")
+    parser.add_argument("-f", "--file", help="File to be hashed")
+    parser.add_argument("-fb", "--binary_file", help='Binary file to be hashed')
+    parser.add_argument("-t", "--test", action='store_true', help='Test accuracy of algorithm')
+    parser.add_argument("-p", "--perf", action='store_true', help='Log performance of the algorithm')
+    parser.add_argument("-b", "--bits", action='store_true', help='Returns size of hashed message in bytes')
+    return parser
+
+
+if __name__ == '__main__':
+    parser = setup_args()
+    args = vars(parser.parse_args())
+    
+    if args['sha256']:
+        start_time = time.time()
+        h = HashLib('sha256').hasher_class()
+        if args['string']:
+            print('Hash: ', h.hex_digest(args["string"]))
+            end_time = time.time()
+        if args['file']:
+            print('Hash: ', h.file_digest(args["file"], False))
+            end_time = time.time()
+        if args['binary_file']:
+            print('Hash: ', h.file_digest(args['binary_file'], True))
+            end_time = time.time()
+        if args['bits']:
+            print("Bytes Hashed: ", h.hashed_bits)
+        if args['perf']:
+            print(f'Time Taken: {end_time - start_time} seconds')
+            
+    elif args['sha512']:
+        start_time = time.time()
+        h = HashLib('sha512').hasher_class()
+        if args['string']:
+            print('Hash: ', h.hex_digest(args["string"]))
+            end_time = time.time()
+        if args['file']:
+            print('Hash: ', h.file_digest(args["file"], False))
+            end_time = time.time()
+        if args['binary_file']:
+            print('Hash: ', h.file_digest(args['binary_file'], True))
+            end_time = time.time()
+        if args['bits']:
+            print("Bytes Hashed: ", h.hashed_bits)
+        if args['perf']:
+            print(f'Time Taken: {end_time - start_time} seconds')
+            
+    else:
         parser.print_help()
```

### Comparing `hashed-1.0.0/src/common.py` & `hashed-2.0.0/hashed/common.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-def right_rotate(num, val, size = 32):
-    return num >> val | num << (size - val)
-
-def right_shift(num, val):
-    return num >> val
-
-def string_to_binary(msg):
-    binary = []
-    for ch in msg:
-        binary.append(bin(ord(ch))[2:].zfill(8))
-    return ''.join(binary)
-
-def binaries_to_binary_string(binary_data):
-    binary_string = ''.join(format(byte, '08b') for byte in binary_data)
-    return binary_string
-
-def create_blocks(binary_string, block_size = 512):
-    blocks = []
-    for i in range(0, len(binary_string), block_size):
-        blocks.append(binary_string[i : i + block_size])
-    return blocks
-
-def string_to_int(binary_str):
-    return int(binary_str, 2)
+def right_rotate(num, val, size = 32):
+    return num >> val | num << (size - val)
+
+def right_shift(num, val):
+    return num >> val
+
+def string_to_binary(msg):
+    binary = []
+    for ch in msg:
+        binary.append(bin(ord(ch))[2:].zfill(8))
+    return ''.join(binary)
+
+def binaries_to_binary_string(binary_data):
+    binary_string = ''.join(format(byte, '08b') for byte in binary_data)
+    return binary_string
+
+def create_blocks(binary_string, block_size = 512):
+    blocks = []
+    for i in range(0, len(binary_string), block_size):
+        blocks.append(binary_string[i : i + block_size])
+    return blocks
+
+def string_to_int(binary_str):
+    return int(binary_str, 2)
```

### Comparing `hashed-1.0.0/src/sha256.py` & `hashed-2.0.0/hashed/sha256.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,153 +1,152 @@
-from hash import Hash
-from common import string_to_binary, create_blocks, string_to_int, right_rotate, right_shift, binaries_to_binary_string
-from buffer_reader import BufferedReader
-
-class SHA256(Hash):
-    
-    def __init__(self):
-        super().__init__()
-        self.H = [
-            0x6a09e667, 0xbb67ae85, 0x3c6ef372, 0xa54ff53a, 
-            0x510e527f, 0x9b05688c, 0x1f83d9ab, 0x5be0cd19
-        ]
-        self.K =  [
-            0x428a2f98, 0x71374491, 0xb5c0fbcf, 0xe9b5dba5, 0x3956c25b, 0x59f111f1, 0x923f82a4, 0xab1c5ed5,
-            0xd807aa98, 0x12835b01, 0x243185be, 0x550c7dc3, 0x72be5d74, 0x80deb1fe, 0x9bdc06a7, 0xc19bf174,
-            0xe49b69c1, 0xefbe4786, 0x0fc19dc6, 0x240ca1cc, 0x2de92c6f, 0x4a7484aa, 0x5cb0a9dc, 0x76f988da,
-            0x983e5152, 0xa831c66d, 0xb00327c8, 0xbf597fc7, 0xc6e00bf3, 0xd5a79147, 0x06ca6351, 0x14292967,
-            0x27b70a85, 0x2e1b2138, 0x4d2c6dfc, 0x53380d13, 0x650a7354, 0x766a0abb, 0x81c2c92e, 0x92722c85,
-            0xa2bfe8a1, 0xa81a664b, 0xc24b8b70, 0xc76c51a3, 0xd192e819, 0xd6990624, 0xf40e3585, 0x106aa070,
-            0x19a4c116, 0x1e376c08, 0x2748774c, 0x34b0bcb5, 0x391c0cb3, 0x4ed8aa4a, 0x5b9cca4f, 0x682e6ff3,
-            0x748f82ee, 0x78a5636f, 0x84c87814, 0x8cc70208, 0x90befffa, 0xa4506ceb, 0xbef9a3f7, 0xc67178f2
-        ]
-        self.MOD = 2**32
-        self.BLOCK_SIZE = 512
-        self.HASHED_BITS = 0
-        self.DIGEST_SIZE= 32
-        
-        
-    def create_message_schedule(self, block):
-        w = []
-        
-        for i in range(0, 512, 32):
-            w.append(string_to_int(block[i : i + 32]))
-                    
-        for i in range(16, 64):
-            s0 = right_rotate(w[i - 15], 7) ^ right_rotate(w[i - 15], 18) ^ right_shift(w[i - 15], 3)
-            s1 = right_rotate(w[i - 2], 17) ^ right_rotate(w[i - 2], 19) ^ right_shift(w[i - 2], 10)
-            ans = (w[i - 16] + s0 + w[i - 7] + s1) % self.MOD
-            w.append(ans)
-            
-        return w
-
-
-    def compression(self, w):
-        a = self.H[0]
-        b = self.H[1]
-        c = self.H[2]
-        d = self.H[3]
-        e = self.H[4]
-        f = self.H[5]
-        g = self.H[6]
-        h = self.H[7]    
-            
-        for i in range(0, 64):
-            s1 = right_rotate(e, 6) ^ right_rotate(e, 11) ^ right_rotate(e, 25)
-            ch = (e & f) ^ ((~e) & g)
-            temp1 = (h + s1 + ch + self.K[i] + w[i]) % self.MOD
-            s0 = right_rotate(a, 2) ^ right_rotate(a, 13) ^ right_rotate(a, 22)
-            maj = (a & b) ^ (a & c) ^ (b & c)
-            temp2 = (s0 + maj) % self.MOD
-            
-            h = g
-            g = f
-            f = e
-            e = (d + temp1) % self.MOD
-            d = c
-            c = b
-            b = a
-            a = (temp1 + temp2) % self.MOD
-            
-        self.H[0] = (self.H[0] + a) % self.MOD
-        self.H[1] = (self.H[1] + b) % self.MOD
-        self.H[2] = (self.H[2] + c) % self.MOD
-        self.H[3] = (self.H[3] + d) % self.MOD
-        self.H[4] = (self.H[4] + e) % self.MOD
-        self.H[5] = (self.H[5] + f) % self.MOD
-        self.H[6] = (self.H[6] + g) % self.MOD
-        self.H[7] = (self.H[7] + h) % self.MOD
-    
-    
-    def update(self, binary_string):
-        orig_len = len(binary_string)
-        
-        binary_string += '1'
-    
-        L = len(binary_string)
-        
-        x = (self.BLOCK_SIZE - (L + 64) % self.BLOCK_SIZE) % self.BLOCK_SIZE
-    
-        binary_string += '0' * x
-            
-        #append 64 bit value of no of bits in original msg
-        binary_string += ''.join(bin(orig_len)[2:].zfill(64))
-                    
-        # create 512 bit blocks
-        blocks = create_blocks(binary_string, self.BLOCK_SIZE)
-                    
-        #sha computation
-        for block in blocks:
-            w = self.create_message_schedule(block)
-            self.compression(w)
-        
-        self.HASHED_BITS += len(binary_string)
-        
-        
-    def digest(self, msg):
-        if isinstance(msg, str):
-            binary_string = string_to_binary(msg)
-        elif not isinstance(msg, bytearray):
-            raise TypeError  
-        
-        self.update(binary_string)
-        
-        return ((self.H[0]).to_bytes(4, 'big') + (self.H[1]).to_bytes(4, 'big') +
-                (self.H[2]).to_bytes(4, 'big') + (self.H[3]).to_bytes(4, 'big') +
-                (self.H[4]).to_bytes(4, 'big') + (self.H[5]).to_bytes(4, 'big') +
-                (self.H[6]).to_bytes(4, 'big') + (self.H[7]).to_bytes(4, 'big'))  
-        
-    
-    def hex_digest(self, msg):
-        if isinstance(msg, str):
-            binary_string = string_to_binary(msg)
-        elif not isinstance(msg, bytearray):
-            raise TypeError  
-        
-        self.update(binary_string)
-        
-        return ((self.H[0]).to_bytes(4, 'big') + (self.H[1]).to_bytes(4, 'big') +
-                (self.H[2]).to_bytes(4, 'big') + (self.H[3]).to_bytes(4, 'big') +
-                (self.H[4]).to_bytes(4, 'big') + (self.H[5]).to_bytes(4, 'big') +
-                (self.H[6]).to_bytes(4, 'big') + (self.H[7]).to_bytes(4, 'big')).hex()
-        
-        
-    def file_digest(self, filename, isBinary):
-        flag = 'r' if not isBinary else 'rb'
-        total = 0
-        with open(filename, flag) as f:
-            reader = BufferedReader(f)
-            while True:
-                data = reader.read(16384)
-                if not data:
-                    break
-                total += len(data)
-                print(f'Calculating hash, read {total} bytes')
-                binary_string = string_to_binary(data) if not isBinary else binaries_to_binary_string(data)
-                self.update(binary_string)
-        
-        return ((self.H[0]).to_bytes(4, 'big') + (self.H[1]).to_bytes(4, 'big') +
-                (self.H[2]).to_bytes(4, 'big') + (self.H[3]).to_bytes(4, 'big') +
-                (self.H[4]).to_bytes(4, 'big') + (self.H[5]).to_bytes(4, 'big') +
-                (self.H[6]).to_bytes(4, 'big') + (self.H[7]).to_bytes(4, 'big')).hex()       
-            
+from hashed.hash import Hash
+from hashed.common import string_to_binary, create_blocks, string_to_int, right_rotate, right_shift, binaries_to_binary_string
+from hashed.buffer_reader import BufferedReader
+
+class SHA256(Hash):
+    
+    def __init__(self):
+        super().__init__()
+        self.H = [
+            0x6a09e667, 0xbb67ae85, 0x3c6ef372, 0xa54ff53a, 
+            0x510e527f, 0x9b05688c, 0x1f83d9ab, 0x5be0cd19
+        ]
+        self.K =  [
+            0x428a2f98, 0x71374491, 0xb5c0fbcf, 0xe9b5dba5, 0x3956c25b, 0x59f111f1, 0x923f82a4, 0xab1c5ed5,
+            0xd807aa98, 0x12835b01, 0x243185be, 0x550c7dc3, 0x72be5d74, 0x80deb1fe, 0x9bdc06a7, 0xc19bf174,
+            0xe49b69c1, 0xefbe4786, 0x0fc19dc6, 0x240ca1cc, 0x2de92c6f, 0x4a7484aa, 0x5cb0a9dc, 0x76f988da,
+            0x983e5152, 0xa831c66d, 0xb00327c8, 0xbf597fc7, 0xc6e00bf3, 0xd5a79147, 0x06ca6351, 0x14292967,
+            0x27b70a85, 0x2e1b2138, 0x4d2c6dfc, 0x53380d13, 0x650a7354, 0x766a0abb, 0x81c2c92e, 0x92722c85,
+            0xa2bfe8a1, 0xa81a664b, 0xc24b8b70, 0xc76c51a3, 0xd192e819, 0xd6990624, 0xf40e3585, 0x106aa070,
+            0x19a4c116, 0x1e376c08, 0x2748774c, 0x34b0bcb5, 0x391c0cb3, 0x4ed8aa4a, 0x5b9cca4f, 0x682e6ff3,
+            0x748f82ee, 0x78a5636f, 0x84c87814, 0x8cc70208, 0x90befffa, 0xa4506ceb, 0xbef9a3f7, 0xc67178f2
+        ]
+        self.MOD = 2**32
+        self.BLOCK_SIZE = 512
+        self.HASHED_BITS = 0
+        self.DIGEST_SIZE= 32
+        
+        
+    def create_message_schedule(self, block):
+        w = []
+        
+        for i in range(0, 512, 32):
+            w.append(string_to_int(block[i : i + 32]))
+                    
+        for i in range(16, 64):
+            s0 = right_rotate(w[i - 15], 7) ^ right_rotate(w[i - 15], 18) ^ right_shift(w[i - 15], 3)
+            s1 = right_rotate(w[i - 2], 17) ^ right_rotate(w[i - 2], 19) ^ right_shift(w[i - 2], 10)
+            ans = (w[i - 16] + s0 + w[i - 7] + s1) % self.MOD
+            w.append(ans)
+            
+        return w
+
+
+    def compression(self, w):
+        a = self.H[0]
+        b = self.H[1]
+        c = self.H[2]
+        d = self.H[3]
+        e = self.H[4]
+        f = self.H[5]
+        g = self.H[6]
+        h = self.H[7]    
+            
+        for i in range(0, 64):
+            s1 = right_rotate(e, 6) ^ right_rotate(e, 11) ^ right_rotate(e, 25)
+            ch = (e & f) ^ ((~e) & g)
+            temp1 = (h + s1 + ch + self.K[i] + w[i]) % self.MOD
+            s0 = right_rotate(a, 2) ^ right_rotate(a, 13) ^ right_rotate(a, 22)
+            maj = (a & b) ^ (a & c) ^ (b & c)
+            temp2 = (s0 + maj) % self.MOD
+            
+            h = g
+            g = f
+            f = e
+            e = (d + temp1) % self.MOD
+            d = c
+            c = b
+            b = a
+            a = (temp1 + temp2) % self.MOD
+            
+        self.H[0] = (self.H[0] + a) % self.MOD
+        self.H[1] = (self.H[1] + b) % self.MOD
+        self.H[2] = (self.H[2] + c) % self.MOD
+        self.H[3] = (self.H[3] + d) % self.MOD
+        self.H[4] = (self.H[4] + e) % self.MOD
+        self.H[5] = (self.H[5] + f) % self.MOD
+        self.H[6] = (self.H[6] + g) % self.MOD
+        self.H[7] = (self.H[7] + h) % self.MOD
+    
+    
+    def update(self, binary_string):
+        orig_len = len(binary_string)
+        
+        binary_string += '1'
+    
+        L = len(binary_string)
+        
+        x = (self.BLOCK_SIZE - (L + 64) % self.BLOCK_SIZE) % self.BLOCK_SIZE
+    
+        binary_string += '0' * x
+            
+        #append 64 bit value of no of bits in original msg
+        binary_string += ''.join(bin(orig_len)[2:].zfill(64))
+                    
+        # create 512 bit blocks
+        blocks = create_blocks(binary_string, self.BLOCK_SIZE)
+                    
+        #sha computation
+        for block in blocks:
+            w = self.create_message_schedule(block)
+            self.compression(w)
+        
+        self.HASHED_BITS += len(binary_string)
+        
+        
+    def digest(self, msg):
+        if isinstance(msg, str):
+            binary_string = string_to_binary(msg)
+        elif not isinstance(msg, bytearray):
+            raise TypeError  
+        
+        self.update(binary_string)
+        
+        return ((self.H[0]).to_bytes(4, 'big') + (self.H[1]).to_bytes(4, 'big') +
+                (self.H[2]).to_bytes(4, 'big') + (self.H[3]).to_bytes(4, 'big') +
+                (self.H[4]).to_bytes(4, 'big') + (self.H[5]).to_bytes(4, 'big') +
+                (self.H[6]).to_bytes(4, 'big') + (self.H[7]).to_bytes(4, 'big'))  
+        
+    
+    def hex_digest(self, msg):
+        if isinstance(msg, str):
+            binary_string = string_to_binary(msg)
+        elif not isinstance(msg, bytearray):
+            raise TypeError  
+        
+        self.update(binary_string)
+        
+        return ((self.H[0]).to_bytes(4, 'big') + (self.H[1]).to_bytes(4, 'big') +
+                (self.H[2]).to_bytes(4, 'big') + (self.H[3]).to_bytes(4, 'big') +
+                (self.H[4]).to_bytes(4, 'big') + (self.H[5]).to_bytes(4, 'big') +
+                (self.H[6]).to_bytes(4, 'big') + (self.H[7]).to_bytes(4, 'big')).hex()
+        
+        
+    def file_digest(self, filename, isBinary):
+        flag = 'r' if not isBinary else 'rb'
+        total = 0
+        with open(filename, flag) as f:
+            reader = BufferedReader(f)
+            while True:
+                data = reader.read(16384)
+                if not data:
+                    break
+                total += len(data)
+                binary_string = string_to_binary(data) if not isBinary else binaries_to_binary_string(data)
+                self.update(binary_string)
+        
+        return ((self.H[0]).to_bytes(4, 'big') + (self.H[1]).to_bytes(4, 'big') +
+                (self.H[2]).to_bytes(4, 'big') + (self.H[3]).to_bytes(4, 'big') +
+                (self.H[4]).to_bytes(4, 'big') + (self.H[5]).to_bytes(4, 'big') +
+                (self.H[6]).to_bytes(4, 'big') + (self.H[7]).to_bytes(4, 'big')).hex()       
+
```

### Comparing `hashed-1.0.0/src/sha512.py` & `hashed-2.0.0/hashed/sha512.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,161 +1,160 @@
-from hash import Hash
-from common import string_to_binary, create_blocks, string_to_int, right_rotate, right_shift, binaries_to_binary_string
-from buffer_reader import BufferedReader
-
-class SHA512(Hash):
-    
-    def __init__(self):
-        super().__init__()
-        self.H = [
-            0x6a09e667f3bcc908, 0xbb67ae8584caa73b, 0x3c6ef372fe94f82b, 0xa54ff53a5f1d36f1,
-            0x510e527fade682d1, 0x9b05688c2b3e6c1f, 0x1f83d9abfb41bd6b, 0x5be0cd19137e2179
-        ]
-        self.K = [
-            0x428a2f98d728ae22, 0x7137449123ef65cd, 0xb5c0fbcfec4d3b2f, 0xe9b5dba58189dbbc, 0x3956c25bf348b538, 
-            0x59f111f1b605d019, 0x923f82a4af194f9b, 0xab1c5ed5da6d8118, 0xd807aa98a3030242, 0x12835b0145706fbe, 
-            0x243185be4ee4b28c, 0x550c7dc3d5ffb4e2, 0x72be5d74f27b896f, 0x80deb1fe3b1696b1, 0x9bdc06a725c71235, 
-            0xc19bf174cf692694, 0xe49b69c19ef14ad2, 0xefbe4786384f25e3, 0x0fc19dc68b8cd5b5, 0x240ca1cc77ac9c65, 
-            0x2de92c6f592b0275, 0x4a7484aa6ea6e483, 0x5cb0a9dcbd41fbd4, 0x76f988da831153b5, 0x983e5152ee66dfab, 
-            0xa831c66d2db43210, 0xb00327c898fb213f, 0xbf597fc7beef0ee4, 0xc6e00bf33da88fc2, 0xd5a79147930aa725, 
-            0x06ca6351e003826f, 0x142929670a0e6e70, 0x27b70a8546d22ffc, 0x2e1b21385c26c926, 0x4d2c6dfc5ac42aed, 
-            0x53380d139d95b3df, 0x650a73548baf63de, 0x766a0abb3c77b2a8, 0x81c2c92e47edaee6, 0x92722c851482353b, 
-            0xa2bfe8a14cf10364, 0xa81a664bbc423001, 0xc24b8b70d0f89791, 0xc76c51a30654be30, 0xd192e819d6ef5218, 
-            0xd69906245565a910, 0xf40e35855771202a, 0x106aa07032bbd1b8, 0x19a4c116b8d2d0c8, 0x1e376c085141ab53, 
-            0x2748774cdf8eeb99, 0x34b0bcb5e19b48a8, 0x391c0cb3c5c95a63, 0x4ed8aa4ae3418acb, 0x5b9cca4f7763e373, 
-            0x682e6ff3d6b2b8a3, 0x748f82ee5defb2fc, 0x78a5636f43172f60, 0x84c87814a1f0ab72, 0x8cc702081a6439ec, 
-            0x90befffa23631e28, 0xa4506cebde82bde9, 0xbef9a3f7b2c67915, 0xc67178f2e372532b, 0xca273eceea26619c, 
-            0xd186b8c721c0c207, 0xeada7dd6cde0eb1e, 0xf57d4f7fee6ed178, 0x06f067aa72176fba, 0x0a637dc5a2c898a6, 
-            0x113f9804bef90dae, 0x1b710b35131c471b, 0x28db77f523047d84, 0x32caab7b40c72493, 0x3c9ebe0a15c9bebc, 
-            0x431d67c49c100d4c, 0x4cc5d4becb3e42b6, 0x597f299cfc657e2a, 0x5fcb6fab3ad6faec, 0x6c44198c4a475817
-        ]
-        self.MOD = 2**64
-        self.BLOCK_SIZE = 1024
-        self.HASHED_BITS = 0
-        self.DIGEST_SIZE = 64
-        
-        
-    def create_message_schedule(self, block):
-        w = []
-        
-        for i in range(0, 1024, 64):
-            w.append(string_to_int(block[i : i + 64]))
-                    
-        for i in range(16, 80):
-            s0 = right_rotate(w[i - 15], 1, 64) ^ right_rotate(w[i - 15], 8, 64) ^ right_shift(w[i - 15], 7)
-            s1 = right_rotate(w[i - 2], 19, 64) ^ right_rotate(w[i - 2], 61, 64) ^ right_shift(w[i - 2], 6)
-            ans = (w[i - 16] + s0 + w[i - 7] + s1) % self.MOD
-            w.append(ans)
-                
-        return w
-
-
-    def compression(self, w):
-        a = self.H[0]
-        b = self.H[1]
-        c = self.H[2]
-        d = self.H[3]
-        e = self.H[4]
-        f = self.H[5]
-        g = self.H[6]
-        h = self.H[7]    
-            
-        for i in range(0, 80):
-            s1 = right_rotate(e, 14, 64) ^ right_rotate(e, 18, 64) ^ right_rotate(e, 41, 64)
-            ch = (e & f) ^ ((~e) & g)
-            temp1 = (h + s1 + ch + self.K[i] + w[i]) % self.MOD
-            s0 = right_rotate(a, 28, 64) ^ right_rotate(a, 34, 64) ^ right_rotate(a, 39, 64)
-            maj = (a & b) ^ (a & c) ^ (b & c)
-            temp2 = (s0 + maj) % self.MOD
-            
-            h = g
-            g = f
-            f = e
-            e = (d + temp1) % self.MOD
-            d = c
-            c = b
-            b = a
-            a = (temp1 + temp2) % self.MOD
-            
-        self.H[0] = (self.H[0] + a) % self.MOD
-        self.H[1] = (self.H[1] + b) % self.MOD
-        self.H[2] = (self.H[2] + c) % self.MOD
-        self.H[3] = (self.H[3] + d) % self.MOD
-        self.H[4] = (self.H[4] + e) % self.MOD
-        self.H[5] = (self.H[5] + f) % self.MOD
-        self.H[6] = (self.H[6] + g) % self.MOD
-        self.H[7] = (self.H[7] + h) % self.MOD
-    
-    
-    def update(self, binary_string):
-        orig_len = len(binary_string)
-        
-        binary_string += '1'
-    
-        L = len(binary_string)
-        
-        x = (self.BLOCK_SIZE - (L + 128) % self.BLOCK_SIZE) % self.BLOCK_SIZE
-    
-        binary_string += '0' * x
-            
-        #append 64 bit value of no of bits in original msg
-        binary_string += ''.join(bin(orig_len)[2:].zfill(128))
-                    
-        # create 512 bit blocks
-        blocks = create_blocks(binary_string, self.BLOCK_SIZE)
-                    
-        #sha computation
-        for block in blocks:
-            w = self.create_message_schedule(block)
-            self.compression(w)
-        
-        self.HASHED_BITS += len(binary_string)
-        
-        
-    def digest(self, msg):
-        if isinstance(msg, str):
-            binary_string = string_to_binary(msg)
-        elif not isinstance(msg, bytearray):
-            raise TypeError  
-        
-        self.update(binary_string)
-        
-        return ((self.H[0]).to_bytes(8, 'big') + (self.H[1]).to_bytes(8, 'big') +
-                (self.H[2]).to_bytes(8, 'big') + (self.H[3]).to_bytes(8, 'big') +
-                (self.H[4]).to_bytes(8, 'big') + (self.H[5]).to_bytes(8, 'big') +
-                (self.H[6]).to_bytes(8, 'big') + (self.H[7]).to_bytes(8, 'big'))  
-        
-    
-    def hex_digest(self, msg):
-        if isinstance(msg, str):
-            binary_string = string_to_binary(msg)
-        elif not isinstance(msg, bytearray):
-            raise TypeError  
-        
-        self.update(binary_string)
-        
-        return ((self.H[0]).to_bytes(8, 'big') + (self.H[1]).to_bytes(8, 'big') +
-                (self.H[2]).to_bytes(8, 'big') + (self.H[3]).to_bytes(8, 'big') +
-                (self.H[4]).to_bytes(8, 'big') + (self.H[5]).to_bytes(8, 'big') +
-                (self.H[6]).to_bytes(8, 'big') + (self.H[7]).to_bytes(8, 'big')).hex()
-        
-        
-    def file_digest(self, filename, isBinary):
-        flag = 'r' if not isBinary else 'rb'
-        total = 0
-        with open(filename, flag) as f:
-            reader = BufferedReader(f)
-            while True:
-                data = reader.read(16384)
-                if not data:
-                    break
-                total += len(data)
-                # print(f'Calculating hash, read {total} bytes')
-                binary_string = string_to_binary(data) if not isBinary else binaries_to_binary_string(data)
-                self.update(binary_string)
-        
-        return ((self.H[0]).to_bytes(8, 'big') + (self.H[1]).to_bytes(8, 'big') +
-                (self.H[2]).to_bytes(8, 'big') + (self.H[3]).to_bytes(8, 'big') +
-                (self.H[4]).to_bytes(8, 'big') + (self.H[5]).to_bytes(8, 'big') +
-                (self.H[6]).to_bytes(8, 'big') + (self.H[7]).to_bytes(8, 'big')).hex()       
-            
+from hashed.hash import Hash
+from hashed.common import string_to_binary, create_blocks, string_to_int, right_rotate, right_shift, binaries_to_binary_string
+from hashed.buffer_reader import BufferedReader
+
+class SHA512(Hash):
+    
+    def __init__(self):
+        super().__init__()
+        self.H = [
+            0x6a09e667f3bcc908, 0xbb67ae8584caa73b, 0x3c6ef372fe94f82b, 0xa54ff53a5f1d36f1,
+            0x510e527fade682d1, 0x9b05688c2b3e6c1f, 0x1f83d9abfb41bd6b, 0x5be0cd19137e2179
+        ]
+        self.K = [
+            0x428a2f98d728ae22, 0x7137449123ef65cd, 0xb5c0fbcfec4d3b2f, 0xe9b5dba58189dbbc, 0x3956c25bf348b538, 
+            0x59f111f1b605d019, 0x923f82a4af194f9b, 0xab1c5ed5da6d8118, 0xd807aa98a3030242, 0x12835b0145706fbe, 
+            0x243185be4ee4b28c, 0x550c7dc3d5ffb4e2, 0x72be5d74f27b896f, 0x80deb1fe3b1696b1, 0x9bdc06a725c71235, 
+            0xc19bf174cf692694, 0xe49b69c19ef14ad2, 0xefbe4786384f25e3, 0x0fc19dc68b8cd5b5, 0x240ca1cc77ac9c65, 
+            0x2de92c6f592b0275, 0x4a7484aa6ea6e483, 0x5cb0a9dcbd41fbd4, 0x76f988da831153b5, 0x983e5152ee66dfab, 
+            0xa831c66d2db43210, 0xb00327c898fb213f, 0xbf597fc7beef0ee4, 0xc6e00bf33da88fc2, 0xd5a79147930aa725, 
+            0x06ca6351e003826f, 0x142929670a0e6e70, 0x27b70a8546d22ffc, 0x2e1b21385c26c926, 0x4d2c6dfc5ac42aed, 
+            0x53380d139d95b3df, 0x650a73548baf63de, 0x766a0abb3c77b2a8, 0x81c2c92e47edaee6, 0x92722c851482353b, 
+            0xa2bfe8a14cf10364, 0xa81a664bbc423001, 0xc24b8b70d0f89791, 0xc76c51a30654be30, 0xd192e819d6ef5218, 
+            0xd69906245565a910, 0xf40e35855771202a, 0x106aa07032bbd1b8, 0x19a4c116b8d2d0c8, 0x1e376c085141ab53, 
+            0x2748774cdf8eeb99, 0x34b0bcb5e19b48a8, 0x391c0cb3c5c95a63, 0x4ed8aa4ae3418acb, 0x5b9cca4f7763e373, 
+            0x682e6ff3d6b2b8a3, 0x748f82ee5defb2fc, 0x78a5636f43172f60, 0x84c87814a1f0ab72, 0x8cc702081a6439ec, 
+            0x90befffa23631e28, 0xa4506cebde82bde9, 0xbef9a3f7b2c67915, 0xc67178f2e372532b, 0xca273eceea26619c, 
+            0xd186b8c721c0c207, 0xeada7dd6cde0eb1e, 0xf57d4f7fee6ed178, 0x06f067aa72176fba, 0x0a637dc5a2c898a6, 
+            0x113f9804bef90dae, 0x1b710b35131c471b, 0x28db77f523047d84, 0x32caab7b40c72493, 0x3c9ebe0a15c9bebc, 
+            0x431d67c49c100d4c, 0x4cc5d4becb3e42b6, 0x597f299cfc657e2a, 0x5fcb6fab3ad6faec, 0x6c44198c4a475817
+        ]
+        self.MOD = 2**64
+        self.BLOCK_SIZE = 1024
+        self.HASHED_BITS = 0
+        self.DIGEST_SIZE = 64
+        
+        
+    def create_message_schedule(self, block):
+        w = []
+        
+        for i in range(0, 1024, 64):
+            w.append(string_to_int(block[i : i + 64]))
+                    
+        for i in range(16, 80):
+            s0 = right_rotate(w[i - 15], 1, 64) ^ right_rotate(w[i - 15], 8, 64) ^ right_shift(w[i - 15], 7)
+            s1 = right_rotate(w[i - 2], 19, 64) ^ right_rotate(w[i - 2], 61, 64) ^ right_shift(w[i - 2], 6)
+            ans = (w[i - 16] + s0 + w[i - 7] + s1) % self.MOD
+            w.append(ans)
+                
+        return w
+
+
+    def compression(self, w):
+        a = self.H[0]
+        b = self.H[1]
+        c = self.H[2]
+        d = self.H[3]
+        e = self.H[4]
+        f = self.H[5]
+        g = self.H[6]
+        h = self.H[7]    
+            
+        for i in range(0, 80):
+            s1 = right_rotate(e, 14, 64) ^ right_rotate(e, 18, 64) ^ right_rotate(e, 41, 64)
+            ch = (e & f) ^ ((~e) & g)
+            temp1 = (h + s1 + ch + self.K[i] + w[i]) % self.MOD
+            s0 = right_rotate(a, 28, 64) ^ right_rotate(a, 34, 64) ^ right_rotate(a, 39, 64)
+            maj = (a & b) ^ (a & c) ^ (b & c)
+            temp2 = (s0 + maj) % self.MOD
+            
+            h = g
+            g = f
+            f = e
+            e = (d + temp1) % self.MOD
+            d = c
+            c = b
+            b = a
+            a = (temp1 + temp2) % self.MOD
+            
+        self.H[0] = (self.H[0] + a) % self.MOD
+        self.H[1] = (self.H[1] + b) % self.MOD
+        self.H[2] = (self.H[2] + c) % self.MOD
+        self.H[3] = (self.H[3] + d) % self.MOD
+        self.H[4] = (self.H[4] + e) % self.MOD
+        self.H[5] = (self.H[5] + f) % self.MOD
+        self.H[6] = (self.H[6] + g) % self.MOD
+        self.H[7] = (self.H[7] + h) % self.MOD
+    
+    
+    def update(self, binary_string):
+        orig_len = len(binary_string)
+        
+        binary_string += '1'
+    
+        L = len(binary_string)
+        
+        x = (self.BLOCK_SIZE - (L + 128) % self.BLOCK_SIZE) % self.BLOCK_SIZE
+    
+        binary_string += '0' * x
+            
+        #append 64 bit value of no of bits in original msg
+        binary_string += ''.join(bin(orig_len)[2:].zfill(128))
+                    
+        # create 512 bit blocks
+        blocks = create_blocks(binary_string, self.BLOCK_SIZE)
+                    
+        #sha computation
+        for block in blocks:
+            w = self.create_message_schedule(block)
+            self.compression(w)
+        
+        self.HASHED_BITS += len(binary_string)
+        
+        
+    def digest(self, msg):
+        if isinstance(msg, str):
+            binary_string = string_to_binary(msg)
+        elif not isinstance(msg, bytearray):
+            raise TypeError  
+        
+        self.update(binary_string)
+        
+        return ((self.H[0]).to_bytes(8, 'big') + (self.H[1]).to_bytes(8, 'big') +
+                (self.H[2]).to_bytes(8, 'big') + (self.H[3]).to_bytes(8, 'big') +
+                (self.H[4]).to_bytes(8, 'big') + (self.H[5]).to_bytes(8, 'big') +
+                (self.H[6]).to_bytes(8, 'big') + (self.H[7]).to_bytes(8, 'big'))  
+        
+    
+    def hex_digest(self, msg):
+        if isinstance(msg, str):
+            binary_string = string_to_binary(msg)
+        elif not isinstance(msg, bytearray):
+            raise TypeError  
+        
+        self.update(binary_string)
+        
+        return ((self.H[0]).to_bytes(8, 'big') + (self.H[1]).to_bytes(8, 'big') +
+                (self.H[2]).to_bytes(8, 'big') + (self.H[3]).to_bytes(8, 'big') +
+                (self.H[4]).to_bytes(8, 'big') + (self.H[5]).to_bytes(8, 'big') +
+                (self.H[6]).to_bytes(8, 'big') + (self.H[7]).to_bytes(8, 'big')).hex()
+        
+        
+    def file_digest(self, filename, isBinary):
+        flag = 'r' if not isBinary else 'rb'
+        total = 0
+        with open(filename, flag) as f:
+            reader = BufferedReader(f)
+            while True:
+                data = reader.read(16384)
+                if not data:
+                    break
+                total += len(data)
+                binary_string = string_to_binary(data) if not isBinary else binaries_to_binary_string(data)
+                self.update(binary_string)
+        
+        return ((self.H[0]).to_bytes(8, 'big') + (self.H[1]).to_bytes(8, 'big') +
+                (self.H[2]).to_bytes(8, 'big') + (self.H[3]).to_bytes(8, 'big') +
+                (self.H[4]).to_bytes(8, 'big') + (self.H[5]).to_bytes(8, 'big') +
+                (self.H[6]).to_bytes(8, 'big') + (self.H[7]).to_bytes(8, 'big')).hex()       
+
```

