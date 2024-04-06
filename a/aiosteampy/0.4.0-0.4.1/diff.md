# Comparing `tmp/aiosteampy-0.4.0.tar.gz` & `tmp/aiosteampy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosteampy-0.4.0.tar", max compression
+gzip compressed data, was "aiosteampy-0.4.1.tar", max compression
```

## Comparing `aiosteampy-0.4.0.tar` & `aiosteampy-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1088 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/LICENSE
--rw-r--r--   0        0        0     4985 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/README.md
--rw-r--r--   0        0        0      309 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/__init__.py
--rw-r--r--   0        0        0    10637 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/client.py
--rw-r--r--   0        0        0    10180 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/confirmation.py
--rw-r--r--   0        0        0     6695 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/constants.py
--rw-r--r--   0        0        0     4428 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/converter.py
--rw-r--r--   0        0        0      701 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/exceptions.py
--rw-r--r--   0        0        0      933 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/guard.py
--rw-r--r--   0        0        0      942 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/http.py
--rw-r--r--   0        0        0    10384 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/login.py
--rw-r--r--   0        0        0    21582 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/market.py
--rw-r--r--   0        0        0    11350 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/models.py
--rw-r--r--   0        0        0    16132 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/public.py
--rw-r--r--   0        0        0    22283 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/trade.py
--rw-r--r--   0        0        0     2287 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/typed.py
--rw-r--r--   0        0        0    11934 2024-01-22 14:40:01.827645 aiosteampy-0.4.0/aiosteampy/utils.py
--rw-r--r--   0        0        0     1791 2024-01-22 14:40:01.831645 aiosteampy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6268 1970-01-01 00:00:00.000000 aiosteampy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4985 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/README.md
+-rw-r--r--   0        0        0      309 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/__init__.py
+-rw-r--r--   0        0        0    10637 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/client.py
+-rw-r--r--   0        0        0    10180 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/confirmation.py
+-rw-r--r--   0        0        0     6695 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/constants.py
+-rw-r--r--   0        0        0     4428 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/converter.py
+-rw-r--r--   0        0        0      701 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/exceptions.py
+-rw-r--r--   0        0        0      933 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/guard.py
+-rw-r--r--   0        0        0      942 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/http.py
+-rw-r--r--   0        0        0    10384 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/login.py
+-rw-r--r--   0        0        0    21582 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/market.py
+-rw-r--r--   0        0        0    11350 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/models.py
+-rw-r--r--   0        0        0    16132 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/public.py
+-rw-r--r--   0        0        0    22283 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/trade.py
+-rw-r--r--   0        0        0     2287 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/typed.py
+-rw-r--r--   0        0        0    12464 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/utils.py
+-rw-r--r--   0        0        0     1791 2024-04-06 19:51:46.490327 aiosteampy-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6268 1970-01-01 00:00:00.000000 aiosteampy-0.4.1/PKG-INFO
```

### Comparing `aiosteampy-0.4.0/LICENSE` & `aiosteampy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/README.md` & `aiosteampy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/client.py` & `aiosteampy-0.4.1/aiosteampy/client.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/confirmation.py` & `aiosteampy-0.4.1/aiosteampy/confirmation.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/constants.py` & `aiosteampy-0.4.1/aiosteampy/constants.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/converter.py` & `aiosteampy-0.4.1/aiosteampy/converter.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/exceptions.py` & `aiosteampy-0.4.1/aiosteampy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/guard.py` & `aiosteampy-0.4.1/aiosteampy/guard.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/http.py` & `aiosteampy-0.4.1/aiosteampy/http.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/login.py` & `aiosteampy-0.4.1/aiosteampy/login.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/market.py` & `aiosteampy-0.4.1/aiosteampy/market.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/models.py` & `aiosteampy-0.4.1/aiosteampy/models.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/public.py` & `aiosteampy-0.4.1/aiosteampy/public.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/trade.py` & `aiosteampy-0.4.1/aiosteampy/trade.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/typed.py` & `aiosteampy-0.4.1/aiosteampy/typed.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.0/aiosteampy/utils.py` & `aiosteampy-0.4.1/aiosteampy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 if TYPE_CHECKING:
     from .client import SteamCommunityMixin
 
 __all__ = (
     "gen_two_factor_code",
     "generate_confirmation_key",
     "generate_device_id",
+    "extract_openid_payload",
     "do_session_steam_auth",
     "get_cookie_value_from_session",
     "async_throttle",
     "create_ident_code",
     "account_id_to_steam_id",
     "steam_id_to_account_id",
+    "id64_to_id32",
+    "id32_to_id64",
     "to_int_boolean",
     "restore_from_cookies",
     "get_jsonable_cookies",
     "buyer_pays_to_receive",
     "receive_to_buyer_pays",
     "generate_session_id",
     "decode_jwt",
@@ -72,38 +75,49 @@
 
     hexed_steam_id = sha1(str(steam_id).encode("ascii")).hexdigest()
     return "android:" + "-".join(
         [hexed_steam_id[:8], hexed_steam_id[8:12], hexed_steam_id[12:16], hexed_steam_id[16:20], hexed_steam_id[20:32]]
     )
 
 
-# TODO make enum with service urls (loot.farm, ...)
+def extract_openid_payload(page_text: str) -> dict[str, str]:
+    """
+    Extract steam openid payload (specs) from page html raw text.
+    Use it if 3rd party websites have extra or non-cookie auth (JWT via service API call, for ex.).
+
+    :param page_text:
+    :return: dict with payload data
+    """
+
+    # not so beautiful as with bs4 but dependency free
+    return {
+        "action": re_search(r"id=\"actionInput\"[\w=\"\s]+value=\"(?P<action>\w+)\"", page_text)["action"],
+        "openid.mode": re_search(r"name=\"openid\.mode\"[\w=\"\s]+value=\"(?P<mode>\w+)\"", page_text)["mode"],
+        "openidparams": re_search(r"name=\"openidparams\"[\w=\"\s]+value=\"(?P<params>[\w=/]+)\"", page_text)["params"],
+        "nonce": re_search(r"name=\"nonce\"[\w=\"\s]+value=\"(?P<nonce>\w+)\"", page_text)["nonce"],
+    }
+
+
 async def do_session_steam_auth(session: ClientSession, auth_url: str | URL):
     """
     Request auth page, find specs of steam openid and log in through steam with passed session.
-    Use it when you need to log in 3rd party site trough Steam.
+    Use it when you need to log in 3rd party site trough Steam using only cookies.
 
     .. seealso:: https://aiosteampy.somespecial.one/examples/auth_3rd_party_site/
 
     :param session: just session.
     :param auth_url: url to site, which redirect you to steam login page.
     """
 
     r = await session.get(auth_url)
     rt = await r.text()
 
-    # not so beautiful as with bs4 but dependency free
-    login_data = {
-        "action": re_search(r"id=\"actionInput\".+value=\"(?P<action>\w+)\"", rt)["action"],
-        "openid.mode": re_search(r"name=\"openid\.mode\".+value=\"(?P<mode>\w+)\"", rt)["mode"],
-        "openidparams": re_search(r"name=\"openidparams\".+value=\"(?P<params>[\w=]+)\"", rt)["params"],
-        "nonce": re_search(r"name=\"nonce\".+value=\"(?P<nonce>\w+)\"", rt)["nonce"],
-    }
+    data = extract_openid_payload(rt)
 
-    await session.post("https://steamcommunity.com/openid/login", data=login_data)
+    await session.post("https://steamcommunity.com/openid/login", data=data, allow_redirects=True)
 
 
 def get_cookie_value_from_session(session: ClientSession, url: URL, field: str) -> str | None:
     """Just get value from session cookies."""
 
     c = session.cookie_jar.filter_cookies(url)
     return c[field].value if field in c else None
@@ -206,14 +220,18 @@
 
 def account_id_to_steam_id(account_id: int) -> int:
     """Convert steam id32 to steam id64."""
 
     return 1 << 56 | 1 << 52 | 1 << 32 | account_id
 
 
+id64_to_id32 = steam_id_to_account_id
+id32_to_id64 = account_id_to_steam_id
+
+
 def to_int_boolean(s):
     """Convert something to 1, 0."""
 
     return 1 if s else 0
 
 
 JSONABLE_COOKIE_JAR: TypeAlias = list[dict[str, dict[str, str, None, bool]]]
```

### Comparing `aiosteampy-0.4.0/pyproject.toml` & `aiosteampy-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiosteampy"
-version = "0.4.0"
+version = "0.4.1"
 description = "Simple library to trade and interact with steam market, webapi, guard"
 license = "MIT"
 authors = ["Dmytro Tkachenko <itsme@somespecial.one>"]
 readme = "README.md"
 homepage = "https://aiosteampy.somespecial.one"
 repository = "https://github.com/somespecialone/aiosteampy"
 documentation = "https://aiosteampy.somespecial.one"
```

### Comparing `aiosteampy-0.4.0/PKG-INFO` & `aiosteampy-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosteampy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple library to trade and interact with steam market, webapi, guard
 Home-page: https://aiosteampy.somespecial.one
 License: MIT
 Keywords: steam,trade,steamguard,asyncio,steam-market
 Author: Dmytro Tkachenko
 Author-email: itsme@somespecial.one
 Requires-Python: >=3.10,<4.0
```

