# Comparing `tmp/brother-4.0.2.tar.gz` & `tmp/brother-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brother-4.0.2.tar", last modified: Wed Mar 13 16:04:43 2024, max compression
+gzip compressed data, was "brother-4.1.0.tar", last modified: Sat Apr  6 11:47:50 2024, max compression
```

## Comparing `brother-4.0.2.tar` & `brother-4.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:04:43.901388 brother-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-13 16:04:35.000000 brother-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-13 16:04:35.000000 brother-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-13 16:04:43.901388 brother-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-13 16:04:35.000000 brother-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:04:43.901388 brother-4.0.2/brother/
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-03-13 16:04:35.000000 brother-4.0.2/brother/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-03-13 16:04:35.000000 brother-4.0.2/brother/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-13 16:04:35.000000 brother-4.0.2/brother/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-13 16:04:35.000000 brother-4.0.2/brother/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:04:35.000000 brother-4.0.2/brother/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:04:43.901388 brother-4.0.2/brother.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-13 16:04:43.000000 brother-4.0.2/brother.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-13 16:04:43.000000 brother-4.0.2/brother.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:04:43.000000 brother-4.0.2/brother.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 16:04:43.000000 brother-4.0.2/brother.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-13 16:04:43.000000 brother-4.0.2/brother.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:04:43.000000 brother-4.0.2/brother.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-13 16:04:35.000000 brother-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-13 16:04:35.000000 brother-4.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 16:04:35.000000 brother-4.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 16:04:43.901388 brother-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-13 16:04:35.000000 brother-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:04:43.901388 brother-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-03-13 16:04:35.000000 brother-4.0.2/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:50.001337 brother-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-06 11:47:41.000000 brother-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 11:47:41.000000 brother-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-06 11:47:50.001337 brother-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-06 11:47:41.000000 brother-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:50.001337 brother-4.1.0/brother/
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-06 11:47:41.000000 brother-4.1.0/brother/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-06 11:47:41.000000 brother-4.1.0/brother/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 11:47:41.000000 brother-4.1.0/brother/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-06 11:47:41.000000 brother-4.1.0/brother/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:41.000000 brother-4.1.0/brother/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:50.001337 brother-4.1.0/brother.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-06 11:47:49.000000 brother-4.1.0/brother.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 11:47:49.000000 brother-4.1.0/brother.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:47:49.000000 brother-4.1.0/brother.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:47:49.000000 brother-4.1.0/brother.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 11:47:49.000000 brother-4.1.0/brother.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:47:49.000000 brother-4.1.0/brother.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-06 11:47:41.000000 brother-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-06 11:47:41.000000 brother-4.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:47:41.000000 brother-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:47:50.001337 brother-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-06 11:47:41.000000 brother-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:47:50.001337 brother-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-06 11:47:41.000000 brother-4.1.0/tests/test_init.py
```

### Comparing `brother-4.0.2/LICENSE` & `brother-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brother-4.0.2/PKG-INFO` & `brother-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brother
-Version: 4.0.2
+Version: 4.1.0
 Summary: Python wrapper for getting data from Brother laser and inkjet printers via SNMP.
 Home-page: https://github.com/bieniu/brother
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `brother-4.0.2/README.md` & `brother-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `brother-4.0.2/brother/__init__.py` & `brother-4.1.0/brother/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,20 +178,16 @@
             raise UnsupportedModelError(
                 "It seems that this printer model is not supported"
             ) from err
 
         self.mac = raw_data[OIDS[ATTR_MAC]]
         self._firmware = raw_data.get(OIDS[ATTR_FIRMWARE])
 
-        charset = CHARSET_MAP.get(raw_data.get(OIDS[ATTR_CHARSET], "unknown"), "roman8")
-
         if status := raw_data[OIDS[ATTR_STATUS]]:
-            data[ATTR_STATUS] = (
-                self._cleanse_status(status).encode("latin1").decode(charset).lower()
-            )
+            data[ATTR_STATUS] = self._cleanse_status(status.lower())
 
         try:
             uptime = int(cast(str, raw_data.get(OIDS[ATTR_UPTIME]))) / 100
         except TypeError:
             pass
         else:
             if self._last_uptime:
@@ -285,14 +281,15 @@
         """Unconfigure SNMP engine."""
         if self._snmp_engine:
             lcd.unconfigure(self._snmp_engine, None)
 
     async def _get_data(self) -> dict[str, Any]:
         """Retrieve data from printer."""
         raw_data: dict[str, str | list[str]] = {}
+        raw_status: bytes | None = None
 
         try:
             request_args = [
                 self._snmp_engine,
                 hlapi.CommunityData("public", mpModel=0),
                 hlapi.UdpTransportTarget(
                     (self._host, self._port), timeout=2, retries=10
@@ -327,16 +324,29 @@
                     for ind in range(0, len(data_str), CHUNK_SIZE)
                 ]
                 # map sensors names to OIDs
                 raw_data[str(resrow[0])] = result
             elif str(resrow[0]) == OIDS[ATTR_MAC]:
                 data = resrow[-1].asOctets()
                 raw_data[str(resrow[0])] = ":".join([f"{x:02x}" for x in data])
+            elif str(resrow[0]) == OIDS[ATTR_STATUS]:
+                raw_status = resrow[-1]._value  # noqa: SLF001
             else:
                 raw_data[str(resrow[0])] = str(resrow[-1])
+
+        if raw_status is not None:
+            charset = raw_data.get(OIDS[ATTR_CHARSET], "unknown")
+
+            if TYPE_CHECKING:
+                assert isinstance(charset, str)
+
+            encoding = CHARSET_MAP.get(charset, "roman8")
+            if status := self._decode_status(raw_status, encoding):
+                raw_data[OIDS[ATTR_STATUS]] = status
+
         # for legacy printers
         for resrow in restable:
             if str(resrow[0]) == OIDS[ATTR_MAINTENANCE]:
                 # asOctets() gives bytes data
                 data = resrow[-1].asOctets()
                 # convert to string without checksum FF at the end, gives
                 # 'a101020414a201020c14a301020614a401020b14'
@@ -393,7 +403,18 @@
                     round(int(item[6:8], 16) / int(item[8:10], 16) * 100),
                 )
 
     @staticmethod
     def _cleanse_status(status: str) -> str:
         """Cleanse and format status."""
         return " ".join(status.split()).strip()
+
+    @staticmethod
+    def _decode_status(status: bytes, encoding: str) -> str | None:
+        """Decode status."""
+        _LOGGER.debug("Status: %s, encoding: %s", status, encoding)
+        try:
+            result = status.decode(encoding)
+        except UnicodeDecodeError:
+            return None
+        else:
+            return result
```

### Comparing `brother-4.0.2/brother/const.py` & `brother-4.1.0/brother/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 VAL_YELLOW_TONER_STATUS: Final = "yellow_toner_status"
 
 CHARSET_MAP: Final = {
     "5": "latin2",
     "2004": "roman8",
     "8": "cyrillic",
     "12": "latin5",
+    "106": "utf-8",
 }
 
 PRINTER_TYPES: Final = ("ink", "laser")
 
 OIDS: Final = {
     ATTR_CHARSET: "1.3.6.1.2.1.43.7.1.1.4.1.1",
     ATTR_COUNTERS: "1.3.6.1.4.1.2435.2.3.9.4.2.1.5.5.10.0",
```

### Comparing `brother-4.0.2/brother/model.py` & `brother-4.1.0/brother/model.py`

 * *Files identical despite different names*

### Comparing `brother-4.0.2/brother.egg-info/PKG-INFO` & `brother-4.1.0/brother.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brother
-Version: 4.0.2
+Version: 4.1.0
 Summary: Python wrapper for getting data from Brother laser and inkjet printers via SNMP.
 Home-page: https://github.com/bieniu/brother
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `brother-4.0.2/pyproject.toml` & `brother-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brother-4.0.2/setup.py` & `brother-4.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "4.0.2"
+VERSION = "4.1.0"
 
 with open("requirements.txt", encoding="utf-8") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="brother",
     version=VERSION,
```

### Comparing `brother-4.0.2/tests/test_init.py` & `brother-4.1.0/tests/test_init.py`

 * *Files 8% similar despite different names*

```diff
@@ -355,7 +355,51 @@
     brother = Brother(HOST)
     oids = OIDS.values()
     result = list(brother._iterate_oids(oids))
 
     assert len(result) == 11
     for item in result:
         assert isinstance(item, ObjectType)
+
+
+@pytest.mark.asyncio()
+async def test_dcp_1618w_model() -> None:
+    """Test with valid data from DCP-1618W printer."""
+    with open("tests/fixtures/dcp-1618w.json", encoding="utf-8") as file:
+        data = json.load(file)
+    brother = Brother(HOST, printer_type="laser")
+
+    with patch("brother.Brother._get_data", return_value=data):
+        sensors = await brother.async_update()
+
+    brother.shutdown()
+
+    assert brother.model == "DCP-1618W"
+    assert brother.firmware == "D1605021248"
+    assert brother.serial == "serial_number"
+    assert sensors.status == "请等待"
+    assert sensors.page_counter == 3914
+    assert sensors.black_toner_remaining == 77
+    assert sensors.drum_counter == 312
+    assert sensors.black_toner == 80
+    assert sensors.drum_remaining_life == 97
+    assert sensors.drum_remaining_pages == 9688
+
+
+@pytest.mark.parametrize(
+    ("status", "encoding", "expected"),
+    [
+        (b"TRYB U\xa6PIENIA", "latin2", "TRYB UŚPIENIA"),
+        (b"PROSZ\xca CZEKA\xc6", "latin2", "PROSZĘ CZEKAĆ"),
+        (b"MA\xa3O TONERU (Y)", "latin2", "MAŁO TONERU (Y)"),
+        (b"\xe8\xaf\xb7\xe7\xad\x89\xe5\xbe\x85", "utf-8", "请等待"),
+        (b"Stap. Kopie\xcdn:01", "roman8", "Stap. Kopieën:01"),
+        (b"\xc1\xdf\xef\xe9\xd8\xd9 \xe0\xd5\xd6\xd8\xdc", "cyrillic", "Спящий режим"),
+    ],
+)
+def test_decode_status(status: bytes, encoding: str, expected: str) -> None:
+    """Test decoding status."""
+    brother = Brother(HOST, printer_type="laser")
+
+    result = brother._decode_status(status, encoding)
+
+    assert result == expected
```

