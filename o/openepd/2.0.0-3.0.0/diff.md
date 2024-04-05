# Comparing `tmp/openepd-2.0.0.tar.gz` & `tmp/openepd-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-2.0.0.tar", max compression
+gzip compressed data, was "openepd-3.0.0.tar", max compression
```

## Comparing `openepd-2.0.0.tar` & `openepd-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,59 @@
--rw-r--r--   0        0        0    11357 2023-07-22 15:23:14.993885 openepd-2.0.0/LICENSE
--rw-r--r--   0        0        0     5799 2023-07-22 15:23:14.993885 openepd-2.0.0/README.md
--rw-r--r--   0        0        0     3030 2023-07-22 15:23:14.993885 openepd-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-07-22 15:23:14.993885 openepd-2.0.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-07-22 15:23:14.993885 openepd-2.0.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-07-22 15:23:14.993885 openepd-2.0.0/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2023-07-22 15:23:14.993885 openepd-2.0.0/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2668 2023-07-22 15:23:14.993885 openepd-2.0.0/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6935 2023-07-22 15:23:14.993885 openepd-2.0.0/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8366 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     5361 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     5617 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    13737 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0    16731 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3816 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     3372 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-07-22 15:23:14.997885 openepd-2.0.0/src/openepd/py.typed
--rw-r--r--   0        0        0     6691 1970-01-01 00:00:00.000000 openepd-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-18 14:32:16.267817 openepd-3.0.0/LICENSE
+-rw-r--r--   0        0        0     6786 2024-04-05 22:32:16.863523 openepd-3.0.0/README.md
+-rw-r--r--   0        0        0     3132 2024-04-05 22:34:29.805796 openepd-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-05 22:35:07.736448 openepd-3.0.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5659 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     2315 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/aluminium.py
+-rw-r--r--   0        0        0     3549 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0    23219 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0    14840 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/glass.py
+-rw-r--r--   0        0        0     6480 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/steel.py
+-rw-r--r--   0        0        0     5144 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/specs/wood.py
+-rw-r--r--   0        0        0     1535 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     5194 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:11:54.308584 openepd-3.0.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 openepd-3.0.0/PKG-INFO
```

### Comparing `openepd-2.0.0/LICENSE` & `openepd-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-2.0.0/README.md` & `openepd-3.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -30,26 +30,55 @@
 The openEPD format is **extensible**. Standard extensions exist for concrete products, and for
 documenting supply-chain specific data.
 
 [Read More about OpenEPD format here](https://www.buildingtransparency.org/programs/openepd/).
 
 ## Usage
 
+## Usage
+
 **❗ ATTENTION**: Pick the right version. The cornerstone of this library models package representing openEPD models. 
 Models are defined with Pydantic library which is a dependency for openepd package. If you use Pydantic in your project
 carefully pick the version:
 
-* Use version below `1.0.0` if your project uses Pydantic version below `2.0.0`
-* Use version `1.0.0` or higher if your project uses Pydantic version `2.0.0` or above
+* Use version **below** `2.0.0` if your project uses Pydantic version below `2.0.0`
+* Use version `2.x.x` or higher if your project uses Pydantic version `2.0.0` or above
 
 ### Models
 
 The library provides the Pydantic models for all the OpenEPD entities. The models are available in the `openepd.models`
 module. For mode details on the usage please refer to Pydantic documentation.
 
+### API Client
+
+The library provides the API client to work with the OpenEPD API. The client is available in the `openepd.client` module.
+Currently, the only available implementation is based on synchronous [requests]() library. Client provides the following
+features:
+* Error handling - depending on HTTP status code the client raises different exceptions allowing to handle errors
+  in a more granular way.
+* Throttling - the client is able to throttle the requests to the API to avoid hitting the rate limits.
+* Retry - the client is able to retry the requests in case of the network errors.
+
+#### API Client Usage
+
+The following example illustrates the usage of the API client:
+
+```python
+from openepd.api.sync_client import OpenEpdApiClientSync
+
+# Setup the client
+api_client = OpenEpdApiClientSync(
+    "https://openepd.buildingtransparency.org/api",
+    "<Your API Token>",
+)
+
+# Use API, e.g. get EPD by ID
+epd = api_client.epds.get_by_openxpd_uuid("ec3b9j5t")
+```
+
 ### Bundle
 
 Bundle is a format which allows to bundle multiple openEPD objects together (it might be EPDs, PCRs, Orgs + any
 other files which might be related to mentioned objects like pdf version of EPD, logo of the PCR company, etc).
 
 Bundle consists of root-level and dependent objects. Dependents are objects which are referenced by root-level objects
 or related to the root-level objects. For example, EPD is a root-level object, PDF version of this EPD is a dependent,
```

#### html2text {}

```diff
@@ -18,49 +18,62 @@
 ways that modern databases can use. openEPD can be used alongside a printable
 document, or can generate printable EPDs. Unlike existing formats such as
 ILCD+EPD, it enforces a key set of guarantees for interoperable data
 processing, including uniqueness of organizations/plants, precise PCR
 references, and dated version control. The openEPD format is **extensible**.
 Standard extensions exist for concrete products, and for documenting supply-
 chain specific data. [Read More about OpenEPD format here](https://
-www.buildingtransparency.org/programs/openepd/). ## Usage **â ATTENTION**:
-Pick the right version. The cornerstone of this library models package
-representing openEPD models. Models are defined with Pydantic library which is
-a dependency for openepd package. If you use Pydantic in your project carefully
-pick the version: * Use version below `1.0.0` if your project uses Pydantic
-version below `2.0.0` * Use version `1.0.0` or higher if your project uses
-Pydantic version `2.0.0` or above ### Models The library provides the Pydantic
-models for all the OpenEPD entities. The models are available in the
-`openepd.models` module. For mode details on the usage please refer to Pydantic
-documentation. ### Bundle Bundle is a format which allows to bundle multiple
-openEPD objects together (it might be EPDs, PCRs, Orgs + any other files which
-might be related to mentioned objects like pdf version of EPD, logo of the PCR
-company, etc). Bundle consists of root-level and dependent objects. Dependents
-are objects which are referenced by root-level objects or related to the root-
-level objects. For example, EPD is a root-level object, PDF version of this EPD
-is a dependent, translated version of the same EPD is dependent as well. The
-following example illustrates reading of the bundle file containing PCR and
-some of the related objects: ```python from openepd.bundle.reader import
-DefaultBundleReader from openepd.bundle.model import AssetType, RelType with
-DefaultBundleReader("test-bundle.epb") as reader: # You could either file path
-or file-like object pcr = reader.get_first_root_asset(AssetType.Pcr) # Get
-FIRST available root level PCR object. We consider that # there is only one PCR
-in the bundle # Read relative PDF file of the found PCR. `related_pdf` is a
-reference to the PDF file containing metadata only related_pdf =
-reader.get_first_relative_asset(pcr, RelType.Pdf) # We have to read the file
-content separately with reader.read_blob_asset(related_pdf) as f: pass # Do
-something with the file content here ``` The next example illustrates the
-writing of the bundle file: ```python from openepd.bundle.writer import
-DefaultBundleWriter from openepd.bundle.model import RelType from
-openepd.model.pcr import Pcr pcr_obj = Pcr(...) # Let's assume we already have
-PCR object with DefaultBundleWriter("my-bundle.epb") as writer, open("test-
-pcr.pdf", "rb") as pcr_pdf_file: # Add our PCR to the bundle. We do not specify
-any extra information, however you might what to add language # and a file name
-to make it look nicer in the bundle. If omitted the name will be generated
-automatically. pcr_asset = writer.write_object_asset(pcr_obj) # Now add related
-PDF document. We have to specify the content type, related (parent) object and
-the # type of relation. Again, optionally you might want to specify the
-language and file name. writer.write_blob_asset(pcr_pdf_file, "application/
-pdf", pcr_asset, RelType.Pdf) ``` # Credits This library has been written and
-maintained by [C-Change Labs](https://c-change-labs.com/). # License This
-library is licensed under [Apache 2](/LICENSE). This means you are free to use
-it in commercial projects.
+www.buildingtransparency.org/programs/openepd/). ## Usage ## Usage **â
+ATTENTION**: Pick the right version. The cornerstone of this library models
+package representing openEPD models. Models are defined with Pydantic library
+which is a dependency for openepd package. If you use Pydantic in your project
+carefully pick the version: * Use version **below** `2.0.0` if your project
+uses Pydantic version below `2.0.0` * Use version `2.x.x` or higher if your
+project uses Pydantic version `2.0.0` or above ### Models The library provides
+the Pydantic models for all the OpenEPD entities. The models are available in
+the `openepd.models` module. For mode details on the usage please refer to
+Pydantic documentation. ### API Client The library provides the API client to
+work with the OpenEPD API. The client is available in the `openepd.client`
+module. Currently, the only available implementation is based on synchronous
+[requests]() library. Client provides the following features: * Error handling
+- depending on HTTP status code the client raises different exceptions allowing
+to handle errors in a more granular way. * Throttling - the client is able to
+throttle the requests to the API to avoid hitting the rate limits. * Retry -
+the client is able to retry the requests in case of the network errors. ####
+API Client Usage The following example illustrates the usage of the API client:
+```python from openepd.api.sync_client import OpenEpdApiClientSync # Setup the
+client api_client = OpenEpdApiClientSync( "https://
+openepd.buildingtransparency.org/api", "", ) # Use API, e.g. get EPD by ID epd
+= api_client.epds.get_by_openxpd_uuid("ec3b9j5t") ``` ### Bundle Bundle is a
+format which allows to bundle multiple openEPD objects together (it might be
+EPDs, PCRs, Orgs + any other files which might be related to mentioned objects
+like pdf version of EPD, logo of the PCR company, etc). Bundle consists of
+root-level and dependent objects. Dependents are objects which are referenced
+by root-level objects or related to the root-level objects. For example, EPD is
+a root-level object, PDF version of this EPD is a dependent, translated version
+of the same EPD is dependent as well. The following example illustrates reading
+of the bundle file containing PCR and some of the related objects: ```python
+from openepd.bundle.reader import DefaultBundleReader from openepd.bundle.model
+import AssetType, RelType with DefaultBundleReader("test-bundle.epb") as
+reader: # You could either file path or file-like object pcr =
+reader.get_first_root_asset(AssetType.Pcr) # Get FIRST available root level PCR
+object. We consider that # there is only one PCR in the bundle # Read relative
+PDF file of the found PCR. `related_pdf` is a reference to the PDF file
+containing metadata only related_pdf = reader.get_first_relative_asset(pcr,
+RelType.Pdf) # We have to read the file content separately with
+reader.read_blob_asset(related_pdf) as f: pass # Do something with the file
+content here ``` The next example illustrates the writing of the bundle file:
+```python from openepd.bundle.writer import DefaultBundleWriter from
+openepd.bundle.model import RelType from openepd.model.pcr import Pcr pcr_obj =
+Pcr(...) # Let's assume we already have PCR object with DefaultBundleWriter
+("my-bundle.epb") as writer, open("test-pcr.pdf", "rb") as pcr_pdf_file: # Add
+our PCR to the bundle. We do not specify any extra information, however you
+might what to add language # and a file name to make it look nicer in the
+bundle. If omitted the name will be generated automatically. pcr_asset =
+writer.write_object_asset(pcr_obj) # Now add related PDF document. We have to
+specify the content type, related (parent) object and the # type of relation.
+Again, optionally you might want to specify the language and file name.
+writer.write_blob_asset(pcr_pdf_file, "application/pdf", pcr_asset,
+RelType.Pdf) ``` # Credits This library has been written and maintained by [C-
+Change Labs](https://c-change-labs.com/). # License This library is licensed
+under [Apache 2](/LICENSE). This means you are free to use it in commercial
+projects.
```

### Comparing `openepd-2.0.0/pyproject.toml` & `openepd-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "2.0.0"
+version = "3.0.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -17,16 +17,17 @@
 ]
 readme = "README.md"
 packages = [{include = "openepd", from = "src"}]
 exclude = ["**/test_*.py", "**/tests/**"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pydantic = ">=2.0,<3.0"
-email-validator = ">=1.3.0"
+pydantic = ">=1.10,<3.0"
+email-validator = ">=1.3.1"
+requests = { version = ">=2.0", optional = true }
 
 # Optional dependencies
 # lxml = { version = "~=4.9.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
 coverage = { version = "=6.5", extras = ["toml"] }
@@ -41,31 +42,31 @@
 licenseheaders = "~=0.8"
 flake8 = "~=4.0"
 flake8-import-graph = "~=0.1.3"
 flake8-docstrings = "~=1.7.0"
 isort = "~=5.11"
 mypy = ">=1.0.1"
 pre-commit = "~=2.19"
-commitizen = "~=2.42.1"
+commitizen = "~=3.16.0"
 
 # Type checking
 types-dateparser = ">=1.1.3"
 types-deprecated = ">=1.2.9"
+types-requests = ">=2.0"
 
 [tool.poetry.extras]
-#xml = ["lxml"]
+api_client = ["requests"]
 
 
 [tool.commitizen]
-version = "2.0.0"
+version_provider = "poetry"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
-    "pyproject.toml",
     "src/openepd/__version__.py",
 ]
 
 [tool.black]
 line-length = 120
 target-version = ['py311']
 exclude = '''
@@ -118,14 +119,15 @@
 python_version = "3.11"
 show_error_codes = true
 ignore_errors = false
 warn_return_any = false
 disallow_any_generics = false
 pretty = true
 mypy_path = "$MYPY_CONFIG_FILE_DIR/stubs"
+plugins = ["pydantic.mypy"]
 exclude = ["test_.*\\.py$", ]
 
 [[tool.mypy.overrides]]
 # External libs which doesn't have type hints (py.typed marker)
 module = []
 ignore_missing_imports = true
 follow_imports = "skip"
```

### Comparing `openepd-2.0.0/src/openepd/__init__.py` & `openepd-3.0.0/src/openepd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `openepd-2.0.0/src/openepd/__version__.py` & `openepd-3.0.0/src/openepd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "2.0.0"
+VERSION = "3.0.0"
```

### Comparing `openepd-2.0.0/src/openepd/bundle/__init__.py` & `openepd-3.0.0/src/openepd/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `openepd-2.0.0/src/openepd/bundle/base.py` & `openepd-3.0.0/src/openepd/bundle/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `openepd-2.0.0/src/openepd/bundle/model.py` & `openepd-3.0.0/src/openepd/bundle/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,16 +15,15 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
-import pydantic as pyd
-
+from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
 
 
 class BundleManifestAssetsStats(BaseOpenEpdSchema):
     """The statistics of assets in a bundle."""
 
     total_count: int = 0
@@ -73,16 +72,16 @@
 
     ref: str
     """The ID of the asset."""
     name: str | None = None
     """The name of the asset."""
     type: AssetType
     """The type of the asset."""
-    lang: str | None = None
+    lang: str | None
     """The language of the asset."""
-    rel_type: str | None = None
-    rel_asset: str | None = None
+    rel_type: str | None
+    rel_asset: str | None
     comment: str | None = pyd.Field(default=None)
     content_type: str | None = pyd.Field(default=None)
     size: int | None = pyd.Field(default=None)
     custom_type: str | None = pyd.Field(default=None)
     custom_data: str | None = pyd.Field(default=None)
```

### Comparing `openepd-2.0.0/src/openepd/bundle/reader.py` & `openepd-3.0.0/src/openepd/bundle/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,29 +31,29 @@
 class DefaultBundleReader(BaseBundleReader):
     """Default bundle reader implementation. Reads the bundle from a ZIP file."""
 
     def __init__(self, bundle_file: PathLike | IO[bytes] | str):
         self._bundle_archive = zipfile.ZipFile(bundle_file, mode="r")
         try:
             with self._bundle_archive.open("manifest", "r") as manifest_stream:
-                self.__manifest = BundleManifest.model_validate_json(manifest_stream.read())
+                self.__manifest = BundleManifest.parse_raw(manifest_stream.read())
         except Exception as e:
             raise ValueError("The bundle file is not valid. Manifest reading error: " + str(e)) from e
         try:
             self.__check_toc()
         except Exception as e:
             raise ValueError("The bundle file is not valid. TOC reading error: " + str(e)) from e
 
     def close(self):
         """Close the reader."""
         self._bundle_archive.close()
 
     def get_manifest(self) -> BundleManifest:
         """Get the manifest of the bundle. Manifest object is immutable."""
-        return self.__manifest.model_copy(deep=True)
+        return self.__manifest.copy(deep=True)
 
     def __create_asset_filter(
         self,
         asset_type: AssetType | str | None = None,
         name: str | None = None,
         parent_ref: AssetRef | None = None,
         ref_type: str | None = None,
@@ -82,15 +82,15 @@
         return input_dict
 
     def assets_iter(self) -> Iterator[AssetInfo]:
         """Iterate over all assets in the bundle."""
         with self._bundle_archive.open("toc", "r") as toc_stream:
             toc_reader = csv.DictReader(io.TextIOWrapper(toc_stream, encoding="utf-8"), dialect="toc")
             for x in toc_reader:
-                yield AssetInfo.model_validate(self.__preprocess_csv_dict(x))
+                yield AssetInfo.parse_obj(self.__preprocess_csv_dict(x))
 
     def __check_toc(self):
         with self._bundle_archive.open("toc", "r") as toc_stream:
             toc_reader = csv.DictReader(io.TextIOWrapper(toc_stream, encoding="utf-8"), dialect="toc")
             if not toc_reader.fieldnames or len(toc_reader.fieldnames) < len(self._TOC_FIELDS):
                 raise ValueError("The bundle file is not valid. TOC reading error: wrong number of fields")
 
@@ -154,8 +154,8 @@
         if asset is None:
             raise ValueError("Asset not found")
         if obj_class.get_asset_type() is None:
             raise ValueError(f"Target object {obj_class.__name__} is not supported asset")
         if asset.type != obj_class.get_asset_type():
             raise ValueError(f"Asset type mismatch. Expected {obj_class.get_asset_type()}, got {asset.type}")
         with self._bundle_archive.open(asset.ref, "r") as asset_stream:
-            return obj_class.model_validate_json(asset_stream.read())
+            return obj_class.parse_raw(asset_stream.read())
```

### Comparing `openepd-2.0.0/src/openepd/bundle/writer.py` & `openepd-3.0.0/src/openepd/bundle/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -113,35 +113,36 @@
             rel_type=rel_type,
             content_type="application/json",
             comment=comment,
             custom_type=custom_type,
             custom_data=custom_data,
         )
         self.__write_data_stream(
-            asset_info, BytesIO(obj.model_dump_json(indent=2, exclude_unset=True, exclude_none=True).encode("utf-8"))
+            asset_info,
+            BytesIO(obj.json(indent=2, exclude_unset=True, exclude_none=True, by_alias=True).encode("utf-8")),
         )
         self.__register_entry(asset_info)
         return asset_info
 
     def commit(self):
         """Write the manifest and TOC to the bundle. This will be called automatically when the bundle is closed."""
         with self._bundle_archive.open("manifest", "w") as manifest_stream:
-            manifest_stream.write(self.__manifest.model_dump_json(indent=2, exclude_none=True).encode("utf-8"))
+            manifest_stream.write(self.__manifest.json(indent=2, exclude_none=True).encode("utf-8"))
         with self._bundle_archive.open("toc", "w") as toc_stream:
             toc_stream.write(self.__toc_buffer.getvalue().encode("utf-8"))
 
     def close(self):
         """Write the manifest and TOC and close the bundle stream."""
         self.commit()
         self._bundle_archive.close()
 
     def __register_entry(self, asset_info: AssetInfo):
         if asset_info.ref in self.__added_entries:
             raise ValueError(f"Asset {asset_info.ref} already exists in the bundle.")
-        self._toc_writer.writerow(asset_info.model_dump(mode="json", exclude_unset=True, exclude_none=True))
+        self._toc_writer.writerow(asset_info.dict(exclude_unset=True, exclude_none=True))
         self.__added_entries.add(asset_info.ref)
         type_counter = self.__manifest.assets.count_by_type.get(asset_info.type, 0) + 1
         self.__manifest.assets.count_by_type[asset_info.type] = type_counter
         self.__manifest.assets.total_count += 1
         if asset_info.size is None:
             raise ValueError("Size of asset is not set.")
         self.__manifest.assets.total_size += asset_info.size
```

### Comparing `openepd-2.0.0/src/openepd/model/__init__.py` & `openepd-3.0.0/src/openepd/api/category/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `openepd-2.0.0/src/openepd/model/base.py` & `openepd-3.0.0/src/openepd/model/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,126 +13,143 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-import abc
-from typing import Any, Optional, Type, TypeVar
+from enum import StrEnum
+from typing import Annotated, Any
 
-import pydantic
+from openepd.compat.pydantic import pyd
+from openepd.model.base import BaseOpenEpdSchema
 
-AnySerializable = int | str | bool | float | list | dict | pydantic.BaseModel | None
-TAnySerializable = TypeVar("TAnySerializable", bound=AnySerializable)
 
+class Amount(BaseOpenEpdSchema):
+    """A value-and-unit pairing for amounts that do not have an uncertainty."""
+
+    qty: float | None = pyd.Field(description="How much of this in the amount.", default=None)
+    unit: str | None = pyd.Field(description="Which unit.  SI units are preferred.", example="kg", default=None)
+
+    @pyd.root_validator
+    def check_qty_or_unit(cls, values: dict[str, Any]):
+        """Ensure that qty or unit is provided."""
+        if values["qty"] is None and values["unit"] is None:
+            raise ValueError("Either qty or unit must be provided.")
+        return values
+
+    def to_quantity_str(self):
+        """Return a string representation of the amount."""
+        return f"{self.qty or ''} {self.unit or 'str'}".strip()
+
+
+class Measurement(BaseOpenEpdSchema):
+    """A scientific value with units and uncertainty."""
+
+    mean: float = pyd.Field(description="Mean (expected) value of the measurement")
+    unit: str = pyd.Field(description="Measurement unit")
+    rsd: pyd.PositiveFloat | None = pyd.Field(
+        description="Relative standard deviation, i.e. standard_deviation/mean", default=None
+    )
+    dist: str | None = pyd.Field(description="Statistical distribution of the measurement error.", default=None)
+
+
+class Ingredient(BaseOpenEpdSchema):
+    """
+    An ingredient of a product.
+
+    The Ingredients list gives the core data references and quantities. This list is used to document supply-chain
+    transparency, such as the EPDs of major components (e.g. cement in concrete, or recycled steel
+    in hot-rolled sections).
+    """
+
+    qty: float | None = pyd.Field(
+        description="Number of declared units of this consumed. Negative values indicate an outflow."
+    )
+    link: pyd.AnyUrl | None = pyd.Field(
+        description="Link to this object's OpenEPD declaration. "
+        "An OpenIndustryEPD or OpenLCI link is also acceptable.",
+        default=None,
+    )
+
+
+class LatLng(BaseOpenEpdSchema):
+    """A latitude and longitude."""
+
+    lat: float = pyd.Field(description="Latitude", example=47.6062)
+    lng: float = pyd.Field(description="Longitude", example=-122.3321)
+
+
+class Location(BaseOpenEpdSchema):
+    """A location on the Earth's surface."""
+
+    pluscode: str | None = pyd.Field(default=None, description="Open Location code of this location")
+    latlng: LatLng | None = pyd.Field(default=None, description="Latitude and longitude of this location")
+    address: str | None = pyd.Field(default=None, description="Text address, preferably geocoded")
+    country: str | None = pyd.Field(default=None, description="2-alpha country code")
+    jurisdiction: str | None = pyd.Field(
+        default=None, description="Province, State, or similar subdivision below the level of a country"
+    )
+
+
+class WithAttachmentsMixin(pyd.BaseModel):
+    """Mixin for objects that can have attachments."""
+
+    attachments: dict[Annotated[str, pyd.Field(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
+        description="Dict of URLs relevant to this entry",
+        example={
+            "Contact Us": "https://www.c-change-labs.com/en/contact-us/",
+            "LinkedIn": "https://www.linkedin.com/company/c-change-labs/",
+        },
+        default=None,
+    )
+
+    def set_attachment(self, name: str, url: str):
+        """Set an attachment."""
+        if self.attachments is None:
+            self.attachments = {}  # type: ignore
+        self.attachments[name] = url  # type: ignore
+
+    def set_attachment_if_any(self, name: str, url: str | None):
+        """Set an attachment if url is not None."""
+        if url is not None:
+            self.set_attachment(name, url)
+
+
+class WithAltIdsMixin(pyd.BaseModel):
+    """Mixin for objects that can have alt_ids."""
+
+    alt_ids: dict[Annotated[str, pyd.Field(max_length=200)], str] | None = pyd.Field(
+        description="Dict identifiers for this entry.",
+        example={
+            "oekobau.dat": "bdda4364-451f-4df2-a68b-5912469ee4c9",
+        },
+        default=None,
+    )
+
+    def set_alt_id(self, domain_name: str, value: str):
+        """Set an alt_id."""
+        if self.alt_ids is None:
+            self.alt_ids = {}
+        self.alt_ids[domain_name] = value
 
-class BaseOpenEpdSchema(pydantic.BaseModel):
-    """Base class for all OpenEPD models."""
-
-    model_config = pydantic.ConfigDict(validate_assignment=False, populate_by_name=True, use_enum_values=True)
-
-    ext: dict[str, AnySerializable] | None = pydantic.Field(alias="ext", default=None)
-
-    def to_serializable(self, *args, **kwargs) -> dict[str, Any]:
-        """
-        Return a serializable dict representation of the DTO.
-
-        It expects the same arguments as the pydantic.BaseModel.json() method.
-        """
-        return self.model_dump(mode="json", *args, **kwargs)
-
-    def has_values(self) -> bool:
-        """Return True if the model has any values."""
-        return len(self.model_dump(mode="python", exclude_unset=True, exclude_none=True)) > 0
-
-    def set_ext(self, ext: "OpenEpdExtension") -> None:
-        """Set the extension field."""
-        self.set_ext_field(ext.get_extension_name(), ext)
+    def set_alt_id_if_any(self, domain_name: str, value: str | None):
+        """Set an alt_id if value is not None."""
+        if value is not None:
+            self.set_alt_id(domain_name, value)
 
-    def set_ext_field(self, key: str, value: AnySerializable) -> None:
-        """Add an extension field to the model."""
-        if self.ext is None:
-            self.ext = {}
-        self.ext[key] = value
 
-    def set_ext_field_if_any(self, key: str, value: AnySerializable) -> None:
-        """Add an extension field to the model if the value is not None."""
-        if value is not None:
-            self.set_ext_field(key, value)
+class OpenEPDUnit(StrEnum):
+    """OpenEPD allowed units."""
 
-    def get_ext_field(self, key: str, default: AnySerializable = None) -> AnySerializable | None:
-        """Get an extension field from the model."""
-        if self.ext is None:
-            return default
-        return self.ext.get(key, default)
-
-    def get_typed_ext_field(
-        self, key: str, target_type: Type[TAnySerializable], default: Optional[TAnySerializable] = None
-    ) -> TAnySerializable:
-        """
-        Get an extension field from the model and convert it to the target type.
-
-        :raise ValueError: if the value cannot be converted to the target type.
-        """
-        value = self.get_ext_field(key, default)
-        if value is None:
-            return None  # type: ignore
-        if issubclass(target_type, pydantic.BaseModel) and isinstance(value, dict):
-            return target_type.construct(**value)  # type: ignore
-        elif isinstance(value, target_type):
-            return value
-        raise ValueError(f"Cannot convert {value} to {target_type}")
-
-    def get_ext(self, ext_type: Type["TOpenEpdExtension"]) -> Optional["TOpenEpdExtension"]:
-        """Get an extension field from the model or None if it doesn't exist."""
-        return self.get_typed_ext_field(ext_type.get_extension_name(), ext_type, None)
-
-    def get_ext_or_empty(self, ext_type: Type["TOpenEpdExtension"]) -> "TOpenEpdExtension":
-        """Get an extension field from the model or an empty instance if it doesn't exist."""
-        return self.get_typed_ext_field(ext_type.get_extension_name(), ext_type, ext_type.construct(**{}))
-
-    @classmethod
-    def is_allowed_field_name(cls, field_name: str) -> bool:
-        """
-        Return True if the field name is defined in the module.
-
-        Both property name and aliases are checked.
-        """
-        if field_name in cls.model_fields:
-            return True
-        else:
-            for x in cls.model_fields.values():
-                if x.alias == field_name:
-                    return True
-        return False
-
-    @classmethod
-    def get_asset_type(cls) -> str | None:
-        """
-        Return the asset type as it should be written into bundle.
-
-        Only independent (e.g. Pcr, Org, Epd, etc) objects have asset type.
-        Supplementary objects (e.g. ResourceUseSet, Location, LatLng) must always return None.
-        """
-        return None
-
-
-class BaseOpenEpdSpec(BaseOpenEpdSchema):
-    """Base class for all OpenEPD specs."""
-
-    pass
-
-
-class OpenEpdExtension(BaseOpenEpdSchema, metaclass=abc.ABCMeta):
-    """Base class for OpenEPD extension models."""
-
-    @classmethod
-    @abc.abstractmethod
-    def get_extension_name(cls) -> str:
-        """Return the name of the extension."""
-        pass
-
-
-TOpenEpdExtension = TypeVar("TOpenEpdExtension", bound=OpenEpdExtension)
-TOpenEpdObject = TypeVar("TOpenEpdObject", bound=BaseOpenEpdSchema)
-TOpenEpdObjectClass = TypeVar("TOpenEpdObjectClass", bound=Type[BaseOpenEpdSchema])
+    kg = "kg"
+    m2 = "m2"
+    m = "m"
+    M2_RSI = "m2 * RSI"
+    MJ = "MJ"
+    t_km = "t * km"
+    MPa = "MPa"
+    item = "item"
+    W = "W"
+    use = "use"
+    degree_c = "°C"
+    kg_co2 = "kgCO2e"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openepd-2.0.0/src/openepd/model/common.py` & `openepd-3.0.0/src/openepd/model/pcr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,135 +13,100 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Annotated, Any
-
-import pydantic as pyd
-from pydantic import BaseModel, model_validator
+import datetime
+from enum import StrEnum
+from typing import Annotated, Optional
 
+from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
+from openepd.model.common import WithAltIdsMixin, WithAttachmentsMixin
+from openepd.model.org import Org
 
 
-class Amount(BaseOpenEpdSchema):
-    """A value-and-unit pairing for amounts that do not have an uncertainty."""
-
-    qty: float | None = pyd.Field(description="How much of this in the amount.", default=None)
-    unit: str | None = pyd.Field(
-        description="Which unit.  SI units are preferred.",
-        default=None,
-        json_schema_extra=dict(example="kg"),
-    )
-
-    @model_validator(mode="before")
-    def check_qty_or_unit(cls, values: dict[str, Any]):
-        """Ensure that qty or unit is provided."""
-        if values["qty"] is None and values["unit"] is None:
-            raise ValueError("Either qty or unit must be provided.")
-        return values
+class PcrStatus(StrEnum):
+    """Status of a PCR."""
 
-    def to_quantity_str(self):
-        """Return a string representation of the amount."""
-        return f"{self.qty or ''} {self.unit or 'str'}".strip()
+    InDevelopment = "InDevelopment"
+    Published = "Published"
+    NonPublic = "NonPublic"
+    Expired = "Expired"
+    Sunset = "Sunset"
 
 
-class Measurement(BaseOpenEpdSchema):
-    """A scientific value with units and uncertainty."""
+class Pcr(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
+    """Represent a PCR (Product Category Rules)."""
 
-    mean: float = pyd.Field(description="Mean (expected) value of the measurement")
-    unit: str = pyd.Field(description="Measurement unit")
-    rsd: pyd.PositiveFloat | None = pyd.Field(
-        description="Relative standard deviation, i.e. standard_deviation/mean", default=None
+    id: str | None = pyd.Field(
+        description="The unique ID for this PCR.  To ensure global uniqueness, should be registered "
+        "at open-xpd-uuid.cqd.io/register or a coordinating registry.",
+        example="ec3xpgq2",
+        default=None,
     )
-    dist: str | None = pyd.Field(description="Statistical distribution of the measurement error.", default=None)
-
-
-class Ingredient(BaseOpenEpdSchema):
-    """
-    An ingredient of a product.
-
-    The Ingredients list gives the core data references and quantities. This list is used to document supply-chain
-    transparency, such as the EPDs of major components (e.g. cement in concrete, or recycled steel
-    in hot-rolled sections).
-    """
-
-    qty: float | None = pyd.Field(
-        description="Number of declared units of this consumed. Negative values indicate an outflow."
+    issuer: Org | None = pyd.Field(description="Organization issuing this PCR", default=None)
+    issuer_doc_id: str | None = pyd.Field(
+        max_length=40,
+        default=None,
+        description="Document ID or code created by issuer",
+        example="c-PCR-003",
     )
-    link: pyd.AnyUrl | None = pyd.Field(
-        description="Link to this object's OpenEPD declaration. "
-        "An OpenIndustryEPD or OpenLCI link is also acceptable.",
+    name: str | None = pyd.Field(
+        max_length=200,
         default=None,
+        description="Full document name as listed in source document",
+        example="c-PCR-003 Concrete and concrete elements (EN 16757)",
     )
-
-
-class LatLng(BaseOpenEpdSchema):
-    """A latitude and longitude."""
-
-    lat: float = pyd.Field(description="Latitude", json_schema_extra=dict(example=47.6062))
-    lng: float = pyd.Field(description="Longitude", json_schema_extra=dict(example=-122.3321))
-
-
-class Location(BaseOpenEpdSchema):
-    """A location on the Earth's surface."""
-
-    pluscode: str | None = pyd.Field(default=None, description="Open Location code of this location")
-    latlng: LatLng | None = pyd.Field(default=None, description="Latitude and longitude of this location")
-    address: str | None = pyd.Field(default=None, description="Text address, preferably geocoded")
-    country: str | None = pyd.Field(default=None, description="2-alpha country code")
-    jurisdiction: str | None = pyd.Field(
-        default=None, description="Province, State, or similar subdivision below the level of a country"
+    short_name: str | None = pyd.Field(
+        default=None,
+        description="A shortened name without boilerplate text.",
+        example="Concrete and Concrete Elements",
     )
-
-
-class WithAttachmentsMixin(BaseModel):
-    """Mixin for objects that can have attachments."""
-
-    attachments: dict[Annotated[str, pyd.Field(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
-        description="Dict of URLs relevant to this entry",
+    version: str | None = pyd.Field(
+        description="Document version, as expressed in document.",
+        example="1.0.2",
         default=None,
-        json_schema_extra={
-            "example": {
-                "Contact Us": "https://www.c-change-labs.com/en/contact-us/",
-                "LinkedIn": "https://www.linkedin.com/company/c-change-labs/",
-            }
-        },
     )
-
-    def set_attachment(self, name: str, url: str):
-        """Set an attachment."""
-        if self.attachments is None:
-            self.attachments = {}  # type: ignore
-        self.attachments[name] = url  # type: ignore
-
-    def set_attachment_if_any(self, name: str, url: str | None):
-        """Set an attachment if url is not None."""
-        if url is not None:
-            self.set_attachment(name, url)
-
-
-class WithAltIdsMixin(BaseModel):
-    """Mixin for objects that can have alt_ids."""
-
-    alt_ids: dict[Annotated[str, pyd.Field(max_length=200)], str] | None = pyd.Field(
-        description="Dict identifiers for this entry.",
+    date_of_issue: datetime.datetime | None = pyd.Field(
+        example=datetime.date(day=11, month=2, year=2022),
         default=None,
-        json_schema_extra=dict(
-            example={
-                "oekobau.dat": "bdda4364-451f-4df2-a68b-5912469ee4c9",
-            }
-        ),
+        description="First day on which the document is valid",
+    )
+    valid_until: datetime.datetime | None = pyd.Field(
+        example=datetime.date(day=11, month=2, year=2024),
+        default=None,
+        description="Last day on which the document is valid",
+    )
+    doc: str | None = pyd.Field(default=None, description="URL to original document, preferably directly to a PDF.")
+    parent: Optional["Pcr"] = pyd.Field(
+        description="The parent PCR, base PCR, `Part A` PCR",
+        default=None,
+    )
+    status: PcrStatus | None = pyd.Field(
+        default=None,
+        description="The current release status of this PCR. "
+        "A PCR with valid_until in the past must have status Expired or Sunset; a PCR with valid_until "
+        "more than 5 years in the past must have status Sunset. Compliant systems should automatically "
+        "update these fields within 24 hours.",
+    )
+    product_classes: dict[str, str | list[str]] = pyd.Field(
+        description="List of classifications, including Masterformat and UNSPC", default_factory=dict
+    )
+    applicable_in: list[Annotated[str, pyd.Field(min_length=2, max_length=2)]] | None = pyd.Field(
+        max_items=100,
+        default=None,
+        description="Jurisdiction(s) in which EPD is applicable. An empty array, or absent properties, "
+        "implies global applicability. Accepts "
+        "[2-letter country codes](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2), "
+        "[M49 region codes](https://unstats.un.org/unsd/methodology/m49/), "
+        'or the alias "EU27" for the 27 members of the Euro bloc, or the alias "NAFTA" '
+        "for the members of North American Free Trade Agreement",
+        example=["US", "CA", "MX", "EU27", "NAFTA"],
     )
 
-    def set_alt_id(self, domain_name: str, value: str):
-        """Set an alt_id."""
-        if self.alt_ids is None:
-            self.alt_ids = {}
-        self.alt_ids[domain_name] = value
-
-    def set_alt_id_if_any(self, domain_name: str, value: str | None):
-        """Set an alt_id if value is not None."""
-        if value is not None:
-            self.set_alt_id(domain_name, value)
+    @classmethod
+    def get_asset_type(cls) -> str | None:
+        """Return the asset type of this class (see BaseOpenEpdSchema.get_asset_type for details)."""
+        return "pcr"
```

### Comparing `openepd-2.0.0/src/openepd/model/epd.py` & `openepd-3.0.0/src/openepd/model/epd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,143 +16,136 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
 from typing import Annotated
 
-import pydantic as pyd
-
-from openepd.model.base import BaseOpenEpdSchema
+from openepd.compat.pydantic import pyd
+from openepd.model.base import BaseDocumentFactory, RootDocument
 from openepd.model.common import Amount, Ingredient, WithAltIdsMixin, WithAttachmentsMixin
 from openepd.model.lcia import Impacts, OutputFlowSet, ResourceUseSet
 from openepd.model.org import Org, Plant
 from openepd.model.pcr import Pcr
 from openepd.model.specs import Specs
 from openepd.model.standard import Standard
+from openepd.model.versioning import OpenEpdVersions, Version
+
 
+class BaseEpd(RootDocument):
+    """
+    Base class for EPD documents.
+
+    This class should not be used directly.  Use Epd or EpdVx instead.
+    """
 
-class Epd(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
+    pass
+
+
+class EpdV0(WithAttachmentsMixin, WithAltIdsMixin, BaseEpd):
     """Represent an EPD."""
 
+    _FORMAT_VERSION = OpenEpdVersions.Version0.as_str()
+
     # TODO: Add validator for open-xpd-uuid on this field
     id: str | None = pyd.Field(
         description="The unique ID for this EPD.  To ensure global uniqueness, should be registered at "
         "open-xpd-uuid.cqd.io/register or a coordinating registry.",
+        example="1u7zsed8",
         default=None,
-        json_schema_extra=dict(example="1u7zsed8"),
-    )
-    doctype: str = pyd.Field(
-        description='Describes the type and schema of the document. Must always always read "openEPD".',
-        default="OpenEPD",
     )
     product_name: str | None = pyd.Field(
-        max_length=200,
-        description="The name of the product described by this EPD",
-        json_schema_extra=dict(example="Mix 12345AC"),
+        max_length=200, description="The name of the product described by this EPD", example="Mix 12345AC", default=None
     )
     product_sku: str | None = pyd.Field(
-        default=None, max_length=200, description="Unique stock keeping identifier assigned by manufacturer"
+        max_length=200, description="Unique stock keeping identifier assigned by manufacturer"
     )
     product_description: str | None = pyd.Field(
         max_length=2000,
-        description="1-paragraph description of product. " "Supports plain text or github flavored markdown.",
+        description="1-paragraph description of product. Supports plain text or github flavored markdown.",
     )
     # TODO: add product_alt_names? E.g. ILCD has a list of synonymous names
     product_classes: dict[str, str | list[str]] = pyd.Field(
         description="List of classifications, including Masterformat and UNSPC", default_factory=dict
     )
     product_image_small: pyd.AnyUrl | None = pyd.Field(
         description="Pointer to image illustrating the product, which is no more than 200x200 pixels", default=None
     )
-    product_image: pyd.AnyUrl | None = pyd.Field(
+    product_image: pyd.AnyUrl | pyd.FileUrl | None = pyd.Field(
         description="pointer to image illustrating the product no more than 10MB", default=None
     )
     version: pyd.PositiveInt | None = pyd.Field(
         description="Version of this document. The document's issuer should increment it anytime even a single "
         "character changes, as this value is used to determine the most recent version.",
+        example=1,
         default=None,
-        json_schema_extra=dict(example=1),
     )
     language: str | None = pyd.Field(
-        default=None,
         min_length=2,
         max_length=2,
+        strip_whitespace=True,
         description="Language this EPD is captured in, as an ISO 639-1 code",
-        json_schema_extra=dict(example="en"),
+        example="en",
     )
     private: bool = pyd.Field(
         default=False,
         description="This document's author does not wish the contents published. "
         "Useful for draft, partial, or confidential declarations.  "
         "How (or whether) privacy is implemented is up to the receiving system.  "
         "Null is treated as false (public).  Private (draft) entries have a reduced "
         "number of required fields, to allow for multiple systems to coordinate "
         "incomplete EPDs.",
     )
-    declaration_url: pyd.AnyUrl | None = pyd.Field(
-        default=None,
+    declaration_url: str | None = pyd.Field(
         description="Link to data object on original registrar's site",
-        json_schema_extra=dict(example="https://epd-online.com/EmbeddedEpdList/Download/6029"),
+        example="https://epd-online.com/EmbeddedEpdList/Download/6029",
     )
     manufacturer: Org | None = pyd.Field(
-        default=None,
         description="JSON object for declaring Org. Sometimes called the "
-        '"Declaration Holder" or "Declaration Owner".',
+        '"Declaration Holder" or "Declaration Owner".'
     )
     epd_developer: Org | None = pyd.Field(
-        default=None,
         description="The organization responsible for the underlying LCA (and subsequent summarization as EPD).",
+        default=None,
     )
     epd_developer_email: pyd.EmailStr | None = pyd.Field(
         default=None,
+        example="john.doe@we-do-lca.com",
         description="Email contact for inquiries about development of this EPD. "
         "This must be an email which can be publicly shared.",
-        json_schema_extra=dict(example="john.doe@we-do-lca.com"),
     )
     plants: list[Plant] = pyd.Field(
-        max_length=32,
+        max_items=32,
         description="List of object(s) for one or more plant(s) that this declaration applies to.",
         default_factory=list,
     )
     program_operator: Org | None = pyd.Field(description="JSON object for program operator Org")
     program_operator_doc_id: str | None = pyd.Field(
-        default=None,
-        max_length=200,
-        description="Document identifier from Program Operator.",
-        json_schema_extra=dict(example="123-456.789/b"),
+        max_length=200, description="Document identifier from Program Operator.", example="123-456.789/b"
     )
     program_operator_version: str | None = pyd.Field(
-        default=None,
-        max_length=200,
-        description="Document version number from Program Operator.",
-        json_schema_extra=dict(example="4.3.0"),
+        max_length=200, description="Document version number from Program Operator.", example="4.3.0"
     )
     third_party_verifier: Org | None = pyd.Field(
-        default=None, description="JSON object for Org that performed a critical review of the EPD data"
+        description="JSON object for Org that performed a critical review of the EPD data"
     )
     third_party_verification_url: pyd.AnyUrl | None = pyd.Field(
-        default=None,
         description="Optional link to a verification statement.",
-        json_schema_extra=dict(example="https://we-verify-epds.com/en/letters/123-456.789b.pdf"),
+        example="https://we-verify-epds.com/en/letters/123-456.789b.pdf",
     )
     third_party_verifier_email: pyd.EmailStr | None = pyd.Field(
-        description="Email address of the third party verifier",
-        default=None,
-        json_schema_extra=dict(example="john.doe@example.com"),
+        description="Email address of the third party verifier", example="john.doe@example.com", default=None
     )
-    date_of_issue: datetime.date | None = pyd.Field(
-        default=None,
+    date_of_issue: datetime.datetime | None = pyd.Field(
+        example=datetime.datetime(day=11, month=9, year=2019, tzinfo=datetime.timezone.utc),
         description="Date the EPD was issued. This should be the first day on which the EPD is valid.",
-        json_schema_extra=dict(example=datetime.date(day=11, month=9, year=2019)),
     )
-    valid_until: datetime.date | None = pyd.Field(
-        default=None,
+    valid_until: datetime.datetime | None = pyd.Field(
+        example=datetime.datetime(day=11, month=9, year=2028, tzinfo=datetime.timezone.utc),
         description="Last date the EPD is valid on, including any extensions.",
-        json_schema_extra=dict(example=datetime.date(day=11, month=9, year=2028)),
     )
     pcr: Pcr | None = pyd.Field(
         description="JSON object for product category rules. Should point to the "
         "most-specific PCR that applies; the PCR entry should point to any "
         "parent PCR.",
         default=None,
     )
@@ -160,55 +153,58 @@
         description="SI declared unit for this EPD.  If a functional unit is "
         "utilized, the declared unit shall refer to the amount of "
         "product associated with the A1-A3 life cycle stage."
     )
     kg_per_declared_unit: Amount | None = pyd.Field(
         default=None,
         description="Mass of the product, in kilograms, per declared unit",
-        json_schema_extra=dict(example=Amount(qty=12.5, unit="kg")),
+        example=Amount(qty=12.5, unit="kg"),
     )
     kg_C_per_declared_unit: Amount | None = pyd.Field(
         default=None,
         description="Mass of elemental carbon, per declared unit, contained in the product itself at the manufacturing "
         "facility gate.  Used (among other things) to check a carbon balance or calculate incineration "
         "emissions.  The source of carbon (e.g. biogenic) is not relevant in this field.",
-        json_schema_extra=dict(example=Amount(qty=8.76, unit="kg")),
+        example=Amount(qty=8.76, unit="kg"),
     )
     kg_C_biogenic_per_declared_unit: Amount | None = pyd.Field(
         default=None,
         description="Mass of elemental carbon from biogenic sources, per declared unit, contained in the product "
         "itself at the manufacturing facility gate.  It may be presumed that any biogenic carbon content "
         "has been accounted for as -44/12 kgCO2e per kg C in stages A1-A3, per EN15804 and ISO 21930.",
-        json_schema_extra=dict(example=Amount(qty=8.76, unit="kg")),
+        example=Amount(qty=8.76, unit="kg"),
     )
     product_service_life_years: float | None = pyd.Field(
-        default=None,
         gt=0.0009,
         lt=101,
         description="Reference service life of the product, in years.  Serves as a maximum for replacement interval, "
         "which may also be constrained by usage or the service life of what the product goes into "
         "(e.g. a building).",
-        json_schema_extra=dict(example=50.0),
+        example=50.0,
     )
     annual_production: float | None = pyd.Field(
         gt=0,
         default=None,
         description="Approximate annual production volume, in declared units, of product covered by this EPD. "
         "This value is intended to be used for weighting of averages. "
         "Providing this data is optional, and it is acceptable to round or obfuscate it downwards "
         "(but not upwards) by any amount desired to protect confidentiality. For example, if the "
         "product volume is 123,456 m3, a value of 120,000, 100,000 or even 87,654 would be acceptable.",
-        json_schema_extra=dict(example=10000),
+        example=10000,
     )
     applicable_in: list[Annotated[str, pyd.Field(min_length=2, max_length=2)]] | None = pyd.Field(
-        max_length=100,
+        max_items=100,
         default=None,
         description="Jurisdiction(s) in which EPD is applicable. An empty array, or absent properties, "
-        "implies global applicability.",
-        json_schema_extra=dict(example=["US", "CA", "MX"]),
+        "implies global applicability. Accepts "
+        "[2-letter country codes](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2), "
+        "[M49 region codes](https://unstats.un.org/unsd/methodology/m49/), "
+        'or the alias "EU27" for the 27 members of the Euro bloc, or the alias "NAFTA" '
+        "for the members of North American Free Trade Agreement",
+        example=["US", "CA", "MX", "EU27", "NAFTA"],
     )
     product_usage_description: str | None = pyd.Field(
         default=None,
         description="Text description of how product is typically used. Can be used to describe accessories "
         "like fasteners, adhesives, etc.  Supports plain text or github flavored markdown.",
     )
     product_usage_image: pyd.AnyUrl | None = pyd.Field(
@@ -235,45 +231,68 @@
         description="Standard(s) to which this declaration is compliant.", default_factory=list
     )
     specs: Specs = pyd.Field(
         default_factory=Specs,
         description="Data structure(s) describing performance specs of product. Unique for each material type.",
     )
     includes: list[Ingredient] = pyd.Field(
-        max_length=255,
+        max_items=255,
         description="List of JSON objects pointing to product components. "
         "Each one should be an EPD or digitized LCI process.",
         default_factory=list,
     )
     lca_discussion: str | None = pyd.Field(
         max_length=20000,
-        description="""A rich text description containing information for experts reviewing the EPD contents. 
-Text descriptions required by ISO 14025, ISO 21930, EN 15804,, relevant PCRs, or program instructions and which do not 
-have specific openEPD fields should be entered here.  This field may be large, and may contain multiple sections 
-separated by github flavored markdown formatting.""",
-        json_schema_extra=dict(
-            example="""# Packaging
-Information on product-specific packaging: type, composition and possible reuse of packaging materials (paper, 
-strapping, pallets, foils, drums, etc.) shall be included in this Section. The EPD shall describe specific packaging 
-scenario assumptions, including disposition pathways for each packaging material by reuse, recycling, or landfill 
-disposal based on packaging type.*
-
-# Product Installation
-
-A description of the type of processing, machinery, tools, dust extraction equipment, auxiliary materials, etc. 
-to be used during installation shall be included. Information on industrial and environmental protection may be 
-included in this section. Any waste treatment included within the system boundary of installation waste should be 
-specified.
-
-# Use Conditions
-
-Use-stage environmental impacts of flooring products during building operations depend on product cleaning assumptions. 
-Information on cleaning frequency and cleaning products shall be provided based on the manufacturer’s recommendations. 
-In the absence of primary data, cleaning assumptions shall be documented.
-    """
-        ),
+        description="""A rich text description containing information for experts reviewing the EPD contents.
+    Text descriptions required by ISO 14025, ISO 21930, EN 15804,, relevant PCRs, or program instructions and which do not
+    have specific openEPD fields should be entered here.  This field may be large, and may contain multiple sections
+    separated by github flavored markdown formatting.""",
+        example="""# Packaging
+
+    Information on product-specific packaging: type, composition and possible reuse of packaging materials (paper,
+    strapping, pallets, foils, drums, etc.) shall be included in this Section. The EPD shall describe specific packaging
+    scenario assumptions, including disposition pathways for each packaging material by reuse, recycling, or landfill
+    disposal based on packaging type.*
+
+    # Product Installation
+
+    A description of the type of processing, machinery, tools, dust extraction equipment, auxiliary materials, etc.
+    to be used during installation shall be included. Information on industrial and environmental protection may be
+    included in this section. Any waste treatment included within the system boundary of installation waste should be
+    specified.
+
+    # Use Conditions
+
+    Use-stage environmental impacts of flooring products during building operations depend on product cleaning assumptions.
+    Information on cleaning frequency and cleaning products shall be provided based on the manufacturer’s recommendations.
+    In the absence of primary data, cleaning assumptions shall be documented.
+    """,
     )
 
     @classmethod
     def get_asset_type(cls) -> str | None:
         """Return the asset type of this class (see BaseOpenEpdSchema.get_asset_type for details)."""
         return "epd"
+
+    @pyd.validator("compliance", always=True, pre=True)
+    def validate_compliance(cls, v: list | None):
+        """Handle correctly None values for compliance field."""
+        if v is None:
+            return []
+        return v
+
+    @pyd.validator("includes", always=True, pre=True)
+    def validate_includes(cls, v: list | None):
+        """Handle correctly None values for includes field."""
+        if v is None:
+            return []
+        return v
+
+
+Epd = EpdV0
+
+
+class EpdFactory(BaseDocumentFactory[BaseEpd]):
+    """Factory for EPD objects."""
+
+    DOCTYPE_CONSTRAINT = "openEPD"
+    VERSION_MAP: dict[Version, type[BaseEpd]] = {OpenEpdVersions.Version0: EpdV0}
```

### Comparing `openepd-2.0.0/src/openepd/model/lcia.py` & `openepd-3.0.0/src/openepd/model/lcia.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,38 +15,37 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
-import pydantic as pyd
-
+from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Measurement
 
 
 class EolScenario(BaseOpenEpdSchema):
     """
     A scenario for end-of-life.
 
     If a particular implementation commits to a specific scenario, then that value can be used;
     otherwise the outcomes can be statistically combined.
     """
 
     name: str = pyd.Field(
         max_length=40,
+        example="Landfill",
         description="A brief text description of the scenario, preferably from list eol_scenario_names",
-        json_schema_extra=dict(example="Landfill"),
     )
     likelihood: float | None = pyd.Field(
         description="The weigting of this scenario used in the C1 .. C4 dataset. For example, the overall C1 shoudl be "
         "equal to weighted sum of C1 from all the scenarios, weighted by likelihood.",
+        example=0.33,
         default=None,
-        json_schema_extra=dict(example=0.33),
     )
     C1: Measurement | None = pyd.Field(
         description="Deconstruction and Demolition under this scenario",
         default=None,
     )
     C2: Measurement | None = pyd.Field(
         description="Transport to waste processing or disposal under this scenario.",
@@ -292,53 +291,65 @@
             return cls.UNKNOWN
         try:
             return cls(d_name)
         except ValueError:
             return cls.UNKNOWN
 
 
-class Impacts(pyd.RootModel):
+class Impacts(pyd.BaseModel):
     """List of environmental impacts, compiled per one of the standard Impact Assessment methods."""
 
-    root: dict[LCIAMethod, ImpactSet]
+    __root__: dict[LCIAMethod, ImpactSet]
 
     def set_unknown_lcia(self, impact_set: ImpactSet):
         """Set the impact set as an unknown LCIA method."""
-        self.root[LCIAMethod.UNKNOWN] = impact_set
+        self.__root__[LCIAMethod.UNKNOWN] = impact_set
 
     def set_impact_set(self, lcia_method: LCIAMethod | str | None, impact_set: ImpactSet):
         """
         Set the impact set for the given LCIA method.
 
         If the LCIA method is None, set it as an unknown LCIA method.
         """
         if lcia_method is None:
             self.set_unknown_lcia(impact_set)
         else:
             if isinstance(lcia_method, str):
                 lcia_method = LCIAMethod.get_by_name(lcia_method)
-            self.root[lcia_method] = impact_set
+            self.__root__[lcia_method] = impact_set
+
+    def replace_lcia_method(self, lcia_method: LCIAMethod, new_lcia_method: LCIAMethod) -> None:
+        """
+        Replace the LCIA method.
+
+        If the there is no impact set for the given LCIA method, do nothing.
+        """
+        impact_set = self.get_impact_set(lcia_method)
+        if impact_set is None:
+            return None
+        self.set_impact_set(new_lcia_method, impact_set)
+        del self.__root__[lcia_method]
 
     def get_impact_set(
         self, lcia_method: LCIAMethod | str | None, default_val: ImpactSet | None = None
     ) -> ImpactSet | None:
         """Return the impact set for the given LCIA method."""
         if lcia_method is None:
-            return self.root.get(LCIAMethod.UNKNOWN, default_val)
+            return self.__root__.get(LCIAMethod.UNKNOWN, default_val)
         if isinstance(lcia_method, str):
             lcia_method = LCIAMethod.get_by_name(lcia_method)
-        return self.root.get(lcia_method, default_val)
+        return self.__root__.get(lcia_method, default_val)
 
     def available_methods(self) -> set[LCIAMethod]:
         """Return a list of available LCIA methods."""
-        return set(self.root.keys())
+        return set(self.__root__.keys())
 
     def as_dict(self) -> dict[LCIAMethod, ImpactSet]:
         """Return the impacts as a dictionary."""
-        return self.root
+        return self.__root__
 
 
 class ResourceUseSet(BaseOpenEpdSchema):
     """A set of resource use indicators, such as RPRec, RPRm, etc."""
 
     RPRec: ScopeSet | None = pyd.Field(
         description="Renewable primary resources used as energy carrier (fuel). "
```

### Comparing `openepd-2.0.0/src/openepd/model/org.py` & `openepd-3.0.0/src/openepd/model/org.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,79 +15,89 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Annotated, Optional
 
-import pydantic as pyd
-
+from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Location, WithAltIdsMixin, WithAttachmentsMixin
+from openepd.model.validation.common import ReferenceStr
 
 
-class Org(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
-    """Represent an organization."""
+class OrgRef(BaseOpenEpdSchema):
+    """Represents Organisation with minimal data."""
 
     web_domain: str | None = pyd.Field(
         description="A web domain owned by organization. Typically is the org's home website address", default=None
     )
     name: str | None = pyd.Field(
         max_length=200,
         description="Common name for organization",
+        example="C Change Labs",
+        default=None,
+    )
+    ref: ReferenceStr | None = pyd.Field(
         default=None,
-        json_schema_extra=dict(example="C Change Labs"),
+        example="https://buildingtransparency.org/ec3/epds/1u7zsed8",
+        description="Reference to this Org's JSON object",
     )
-    alt_names: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_length=255)] | None = pyd.Field(
+
+
+class Org(WithAttachmentsMixin, WithAltIdsMixin, OrgRef):
+    """Represent an organization."""
+
+    alt_names: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
         description="List of other names for organization",
+        example=["C-Change Labs", "C-Change Labs inc."],
         default=None,
-        json_schema_extra=dict(example=["C-Change Labs", "C-Change Labs inc."]),
     )
     # TODO: NEW field, not in the spec
+
     owner: Optional["Org"] = pyd.Field(description="Organization that controls this organization", default=None)
-    subsidiaries: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_length=255)] | None = pyd.Field(
+    subsidiaries: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
         description="Organizations controlled by this organization",
+        example=["cqd.io", "supplychaincarbonpricing.org"],
         default=None,
-        json_schema_extra=dict(example=["cqd.io", "supplychaincarbonpricing.org"]),
     )
     hq_location: Location | None = pyd.Field(
         default=None,
         description="Location of a place of business, prefereably the corporate headquarters.",
     )
 
 
 class Plant(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent a manufacturing plant."""
 
-    model_config = pyd.ConfigDict(populate_by_name=True)
-
     # TODO: Add proper validator
     id: str | None = pyd.Field(
         description="Plus code (aka Open Location Code) of plant's location and "
         "owner's web domain joined with `.`(dot).",
+        example="865P2W3V+3W.interface.com",
         alias="pluscode",
         default=None,
-        json_schema_extra=dict(example="865P2W3V+3W.interface.com"),
     )
     owner: Org | None = pyd.Field(description="Organization that owns the plant", default=None)
     name: str | None = pyd.Field(
         max_length=200,
         description="Manufacturer's name for plant. Recommended < 40 chars",
+        example="Dalton, GA",
         default=None,
-        json_schema_extra=dict(example="Dalton, GA"),
     )
     address: str | None = pyd.Field(
         max_length=200,
         default=None,
         description="Text address, preferably geocoded",
-        json_schema_extra=dict(example="1503 Orchard Hill Rd, LaGrange, GA 30240, United States"),
+        example="1503 Orchard Hill Rd, LaGrange, GA 30240, United States",
     )
     contact_email: pyd.EmailStr | None = pyd.Field(
-        description="Email contact",
-        default=None,
-        json_schema_extra=dict(example="info@interface.com"),
+        description="Email contact", example="info@interface.com", default=None
     )
 
     @classmethod
     def get_asset_type(cls) -> str | None:
         """Return the asset type of this class (see BaseOpenEpdSchema.get_asset_type for details)."""
         return "org"
+
+    class Config(BaseOpenEpdSchema.Config):
+        allow_population_by_field_name = True
```

### Comparing `openepd-2.0.0/src/openepd/model/specs/__init__.py` & `openepd-3.0.0/src/openepd/api/dto/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,17 +13,29 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-import pydantic as pyd
+import abc
 
-from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.specs.concrete import CmuSpec
+from openepd.compat.pydantic import pyd
 
 
-class Specs(BaseOpenEpdSchema):
-    """Material specific specs."""
+class BaseOpenEpdApiModel(pyd.BaseModel):
+    """Base class for OpenEPD API DTOs."""
 
-    cmu: CmuSpec | None = pyd.Field(default=None, description="Concrete Masonry Unit-specific (CMU) specs")
+    class Config:
+        extra = pyd.Extra.ignore
+
+
+class BaseMetaDto(BaseOpenEpdApiModel, metaclass=abc.ABCMeta):
+    """Base class for all meta DTOs."""
+
+    pass
+
+
+class MetaExtensionBase(BaseOpenEpdApiModel):
+    """Base class for custom meta extensions."""
+
+    pass
```

### Comparing `openepd-2.0.0/src/openepd/model/standard.py` & `openepd-3.0.0/src/openepd/model/standard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright 2023 by C Change Labs Inc. www.c-change-labs.com
+#  Copyright 2024 by C Change Labs Inc. www.c-change-labs.com
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,16 +13,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-import pydantic as pyd
-
+from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.org import Org
 
 
 class Standard(BaseOpenEpdSchema):
     """A standard, such as EN 15804, ISO 14044, ISO 14024:2018, etc."""
```

### Comparing `openepd-2.0.0/PKG-INFO` & `openepd-3.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
@@ -12,16 +12,18 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: email-validator (>=1.3.0)
-Requires-Dist: pydantic (>=2.0,<3.0)
+Provides-Extra: api-client
+Requires-Dist: email-validator (>=1.3.1)
+Requires-Dist: pydantic (>=1.10,<3.0)
+Requires-Dist: requests (>=2.0) ; extra == "api-client"
 Project-URL: Repository, https://github.com/cchangelabs/openepd
 Description-Content-Type: text/markdown
 
 # Python Library to work with OpenEPD format
 
 <p align="center">
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/l/openepd?style=for-the-badge" title="License: Apache-2"/></a> 
@@ -53,26 +55,55 @@
 The openEPD format is **extensible**. Standard extensions exist for concrete products, and for
 documenting supply-chain specific data.
 
 [Read More about OpenEPD format here](https://www.buildingtransparency.org/programs/openepd/).
 
 ## Usage
 
+## Usage
+
 **❗ ATTENTION**: Pick the right version. The cornerstone of this library models package representing openEPD models. 
 Models are defined with Pydantic library which is a dependency for openepd package. If you use Pydantic in your project
 carefully pick the version:
 
-* Use version below `1.0.0` if your project uses Pydantic version below `2.0.0`
-* Use version `1.0.0` or higher if your project uses Pydantic version `2.0.0` or above
+* Use version **below** `2.0.0` if your project uses Pydantic version below `2.0.0`
+* Use version `2.x.x` or higher if your project uses Pydantic version `2.0.0` or above
 
 ### Models
 
 The library provides the Pydantic models for all the OpenEPD entities. The models are available in the `openepd.models`
 module. For mode details on the usage please refer to Pydantic documentation.
 
+### API Client
+
+The library provides the API client to work with the OpenEPD API. The client is available in the `openepd.client` module.
+Currently, the only available implementation is based on synchronous [requests]() library. Client provides the following
+features:
+* Error handling - depending on HTTP status code the client raises different exceptions allowing to handle errors
+  in a more granular way.
+* Throttling - the client is able to throttle the requests to the API to avoid hitting the rate limits.
+* Retry - the client is able to retry the requests in case of the network errors.
+
+#### API Client Usage
+
+The following example illustrates the usage of the API client:
+
+```python
+from openepd.api.sync_client import OpenEpdApiClientSync
+
+# Setup the client
+api_client = OpenEpdApiClientSync(
+    "https://openepd.buildingtransparency.org/api",
+    "<Your API Token>",
+)
+
+# Use API, e.g. get EPD by ID
+epd = api_client.epds.get_by_openxpd_uuid("ec3b9j5t")
+```
+
 ### Bundle
 
 Bundle is a format which allows to bundle multiple openEPD objects together (it might be EPDs, PCRs, Orgs + any
 other files which might be related to mentioned objects like pdf version of EPD, logo of the PCR company, etc).
 
 Bundle consists of root-level and dependent objects. Dependents are objects which are referenced by root-level objects
 or related to the root-level objects. For example, EPD is a root-level object, PDF version of this EPD is a dependent,
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: openepd Version: 2.0.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.0.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Dist: email-validator
-(>=1.3.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL: Repository, https:/
+Development :: Libraries :: Python Modules Provides-Extra: api-client Requires-
+Dist: email-validator (>=1.3.1) Requires-Dist: pydantic (>=1.10,<3.0) Requires-
+Dist: requests (>=2.0) ; extra == "api-client" Project-URL: Repository, https:/
 /github.com/cchangelabs/openepd Description-Content-Type: text/markdown #
 Python Library to work with OpenEPD format
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
      _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_S_t_y_l_e_-_b_l_a_c_k_-_b_l_a_c_k_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/
                         _d_m_/_o_p_e_n_e_p_d_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
@@ -30,49 +31,62 @@
 ways that modern databases can use. openEPD can be used alongside a printable
 document, or can generate printable EPDs. Unlike existing formats such as
 ILCD+EPD, it enforces a key set of guarantees for interoperable data
 processing, including uniqueness of organizations/plants, precise PCR
 references, and dated version control. The openEPD format is **extensible**.
 Standard extensions exist for concrete products, and for documenting supply-
 chain specific data. [Read More about OpenEPD format here](https://
-www.buildingtransparency.org/programs/openepd/). ## Usage **â ATTENTION**:
-Pick the right version. The cornerstone of this library models package
-representing openEPD models. Models are defined with Pydantic library which is
-a dependency for openepd package. If you use Pydantic in your project carefully
-pick the version: * Use version below `1.0.0` if your project uses Pydantic
-version below `2.0.0` * Use version `1.0.0` or higher if your project uses
-Pydantic version `2.0.0` or above ### Models The library provides the Pydantic
-models for all the OpenEPD entities. The models are available in the
-`openepd.models` module. For mode details on the usage please refer to Pydantic
-documentation. ### Bundle Bundle is a format which allows to bundle multiple
-openEPD objects together (it might be EPDs, PCRs, Orgs + any other files which
-might be related to mentioned objects like pdf version of EPD, logo of the PCR
-company, etc). Bundle consists of root-level and dependent objects. Dependents
-are objects which are referenced by root-level objects or related to the root-
-level objects. For example, EPD is a root-level object, PDF version of this EPD
-is a dependent, translated version of the same EPD is dependent as well. The
-following example illustrates reading of the bundle file containing PCR and
-some of the related objects: ```python from openepd.bundle.reader import
-DefaultBundleReader from openepd.bundle.model import AssetType, RelType with
-DefaultBundleReader("test-bundle.epb") as reader: # You could either file path
-or file-like object pcr = reader.get_first_root_asset(AssetType.Pcr) # Get
-FIRST available root level PCR object. We consider that # there is only one PCR
-in the bundle # Read relative PDF file of the found PCR. `related_pdf` is a
-reference to the PDF file containing metadata only related_pdf =
-reader.get_first_relative_asset(pcr, RelType.Pdf) # We have to read the file
-content separately with reader.read_blob_asset(related_pdf) as f: pass # Do
-something with the file content here ``` The next example illustrates the
-writing of the bundle file: ```python from openepd.bundle.writer import
-DefaultBundleWriter from openepd.bundle.model import RelType from
-openepd.model.pcr import Pcr pcr_obj = Pcr(...) # Let's assume we already have
-PCR object with DefaultBundleWriter("my-bundle.epb") as writer, open("test-
-pcr.pdf", "rb") as pcr_pdf_file: # Add our PCR to the bundle. We do not specify
-any extra information, however you might what to add language # and a file name
-to make it look nicer in the bundle. If omitted the name will be generated
-automatically. pcr_asset = writer.write_object_asset(pcr_obj) # Now add related
-PDF document. We have to specify the content type, related (parent) object and
-the # type of relation. Again, optionally you might want to specify the
-language and file name. writer.write_blob_asset(pcr_pdf_file, "application/
-pdf", pcr_asset, RelType.Pdf) ``` # Credits This library has been written and
-maintained by [C-Change Labs](https://c-change-labs.com/). # License This
-library is licensed under [Apache 2](/LICENSE). This means you are free to use
-it in commercial projects.
+www.buildingtransparency.org/programs/openepd/). ## Usage ## Usage **â
+ATTENTION**: Pick the right version. The cornerstone of this library models
+package representing openEPD models. Models are defined with Pydantic library
+which is a dependency for openepd package. If you use Pydantic in your project
+carefully pick the version: * Use version **below** `2.0.0` if your project
+uses Pydantic version below `2.0.0` * Use version `2.x.x` or higher if your
+project uses Pydantic version `2.0.0` or above ### Models The library provides
+the Pydantic models for all the OpenEPD entities. The models are available in
+the `openepd.models` module. For mode details on the usage please refer to
+Pydantic documentation. ### API Client The library provides the API client to
+work with the OpenEPD API. The client is available in the `openepd.client`
+module. Currently, the only available implementation is based on synchronous
+[requests]() library. Client provides the following features: * Error handling
+- depending on HTTP status code the client raises different exceptions allowing
+to handle errors in a more granular way. * Throttling - the client is able to
+throttle the requests to the API to avoid hitting the rate limits. * Retry -
+the client is able to retry the requests in case of the network errors. ####
+API Client Usage The following example illustrates the usage of the API client:
+```python from openepd.api.sync_client import OpenEpdApiClientSync # Setup the
+client api_client = OpenEpdApiClientSync( "https://
+openepd.buildingtransparency.org/api", "", ) # Use API, e.g. get EPD by ID epd
+= api_client.epds.get_by_openxpd_uuid("ec3b9j5t") ``` ### Bundle Bundle is a
+format which allows to bundle multiple openEPD objects together (it might be
+EPDs, PCRs, Orgs + any other files which might be related to mentioned objects
+like pdf version of EPD, logo of the PCR company, etc). Bundle consists of
+root-level and dependent objects. Dependents are objects which are referenced
+by root-level objects or related to the root-level objects. For example, EPD is
+a root-level object, PDF version of this EPD is a dependent, translated version
+of the same EPD is dependent as well. The following example illustrates reading
+of the bundle file containing PCR and some of the related objects: ```python
+from openepd.bundle.reader import DefaultBundleReader from openepd.bundle.model
+import AssetType, RelType with DefaultBundleReader("test-bundle.epb") as
+reader: # You could either file path or file-like object pcr =
+reader.get_first_root_asset(AssetType.Pcr) # Get FIRST available root level PCR
+object. We consider that # there is only one PCR in the bundle # Read relative
+PDF file of the found PCR. `related_pdf` is a reference to the PDF file
+containing metadata only related_pdf = reader.get_first_relative_asset(pcr,
+RelType.Pdf) # We have to read the file content separately with
+reader.read_blob_asset(related_pdf) as f: pass # Do something with the file
+content here ``` The next example illustrates the writing of the bundle file:
+```python from openepd.bundle.writer import DefaultBundleWriter from
+openepd.bundle.model import RelType from openepd.model.pcr import Pcr pcr_obj =
+Pcr(...) # Let's assume we already have PCR object with DefaultBundleWriter
+("my-bundle.epb") as writer, open("test-pcr.pdf", "rb") as pcr_pdf_file: # Add
+our PCR to the bundle. We do not specify any extra information, however you
+might what to add language # and a file name to make it look nicer in the
+bundle. If omitted the name will be generated automatically. pcr_asset =
+writer.write_object_asset(pcr_obj) # Now add related PDF document. We have to
+specify the content type, related (parent) object and the # type of relation.
+Again, optionally you might want to specify the language and file name.
+writer.write_blob_asset(pcr_pdf_file, "application/pdf", pcr_asset,
+RelType.Pdf) ``` # Credits This library has been written and maintained by [C-
+Change Labs](https://c-change-labs.com/). # License This library is licensed
+under [Apache 2](/LICENSE). This means you are free to use it in commercial
+projects.
```

