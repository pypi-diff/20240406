# Comparing `tmp/httplint-2024.1.1.tar.gz` & `tmp/httplint-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httplint-2024.1.1.tar", last modified: Tue Jan 30 04:27:54 2024, max compression
+gzip compressed data, was "httplint-2024.4.1.tar", last modified: Sat Apr  6 07:59:30 2024, max compression
```

## Comparing `httplint-2024.1.1.tar` & `httplint-2024.4.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.736261 httplint-2024.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-30 04:27:19.000000 httplint-2024.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-01-30 04:27:54.736261 httplint-2024.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-30 04:27:19.000000 httplint-2024.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.720261 httplint-2024.1.1/httplint/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.724261 httplint-2024.1.1/httplint/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/cli/http_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/content_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.724261 httplint-2024.1.1/httplint/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/notes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.732261 httplint-2024.1.1/httplint/field/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/accept_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/age.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/allow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/connectiox.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_disposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_range.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_transfer_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/cteonnt_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/expires.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/last_modified.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/mime_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/p3p.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/pragma.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/proxy_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/retry_after.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/set_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/set_cookie2.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/soapaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/tcn.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/te.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/trailer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/transfer_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/vary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/via.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/www_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/x_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/x_cache_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/x_content_type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/x_frame_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/x_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/parsers/x_xss_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/section.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/field/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/note.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.736261 httplint-2024.1.1/httplint/syntax/
--rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7384 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc3986.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc5234.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc5322.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc5646.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc5987.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc5988.py
--rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc7230.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc7231.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc7232.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc7233.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc7234.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc7235.py
--rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc9110.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/syntax/rfc9111.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-01-30 04:27:19.000000 httplint-2024.1.1/httplint/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.736261 httplint-2024.1.1/httplint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-01-30 04:27:54.000000 httplint-2024.1.1/httplint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-30 04:27:54.000000 httplint-2024.1.1/httplint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 04:27:54.000000 httplint-2024.1.1/httplint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-30 04:27:54.000000 httplint-2024.1.1/httplint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-30 04:27:54.000000 httplint-2024.1.1/httplint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-30 04:27:54.000000 httplint-2024.1.1/httplint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-01-30 04:27:19.000000 httplint-2024.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 04:27:54.736261 httplint-2024.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 04:27:54.736261 httplint-2024.1.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-01-30 04:27:19.000000 httplint-2024.1.1/test/smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-01-30 04:27:19.000000 httplint-2024.1.1/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-30 04:27:19.000000 httplint-2024.1.1/test/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-30 04:27:19.000000 httplint-2024.1.1/test/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-30 04:27:19.000000 httplint-2024.1.1/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.811627 httplint-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-06 07:59:06.000000 httplint-2024.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-06 07:59:30.811627 httplint-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-06 07:59:06.000000 httplint-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.795627 httplint-2024.4.1/httplint/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.795627 httplint-2024.4.1/httplint/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/cli/http_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/content_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.799627 httplint-2024.4.1/httplint/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/notes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.807627 httplint-2024.4.1/httplint/field/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/accept_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/age.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/allow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/connectiox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_disposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_transfer_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/cteonnt_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/etag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/expires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/last_modified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/mime_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/p3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/pragma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/proxy_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/retry_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/set_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/set_cookie2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/soapaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/te.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/trailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/transfer_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/vary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/via.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/www_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/x_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/x_cache_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/x_content_type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/x_frame_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/x_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/parsers/x_xss_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/field/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.807627 httplint-2024.4.1/httplint/syntax/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7384 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc3986.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc5234.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc5322.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc5646.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc5987.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc5988.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc7230.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc7231.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc7232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc7233.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc7234.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc7235.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc9110.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/syntax/rfc9111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-06 07:59:06.000000 httplint-2024.4.1/httplint/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.811627 httplint-2024.4.1/httplint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-06 07:59:30.000000 httplint-2024.4.1/httplint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-06 07:59:30.000000 httplint-2024.4.1/httplint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:59:30.000000 httplint-2024.4.1/httplint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-06 07:59:30.000000 httplint-2024.4.1/httplint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 07:59:30.000000 httplint-2024.4.1/httplint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 07:59:30.000000 httplint-2024.4.1/httplint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-06 07:59:06.000000 httplint-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:59:30.811627 httplint-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:59:30.807627 httplint-2024.4.1/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-04-06 07:59:06.000000 httplint-2024.4.1/test/smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-06 07:59:06.000000 httplint-2024.4.1/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 07:59:06.000000 httplint-2024.4.1/test/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-06 07:59:06.000000 httplint-2024.4.1/test/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-06 07:59:06.000000 httplint-2024.4.1/test/utils.py
```

### Comparing `httplint-2024.1.1/LICENSE.md` & `httplint-2024.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/PKG-INFO` & `httplint-2024.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httplint
-Version: 2024.1.1
+Version: 2024.4.1
 Summary: Lint for HTTP messages.
 Author-email: Mark Nottingham <mnot@mnot.net>
 License: Copyright (c) Mark Nottingham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -50,15 +50,15 @@
 Requires-Dist: types-Markdown; extra == "dev"
 
 
 # httplint
 
 This Python library _lints_ HTTP messages; it checks them for correctness and reports any issues it finds.
 
-It has been extracted from [REDbot](https://redbot.org/), which will eventually depend upon it. Unlike REDbot, it does not perform any 'active' checks by making requests to the network, and it does not have a Web user interface.
+It performs all message-level checks for [REDbot](https://redbot.org/), but does not perform any 'active' checks by making requests to the network, and it does not have a Web user interface.
 
 
 ## Using httplint as a Library
 
 httplint exposes two classes for linting: `HttpRequestLinter` and `HttpResponseLinter`. They expose the following methods for telling the linter about the HTTP message:
 
 * As appropriate:
```

### Comparing `httplint-2024.1.1/README.md` & `httplint-2024.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # httplint
 
 This Python library _lints_ HTTP messages; it checks them for correctness and reports any issues it finds.
 
-It has been extracted from [REDbot](https://redbot.org/), which will eventually depend upon it. Unlike REDbot, it does not perform any 'active' checks by making requests to the network, and it does not have a Web user interface.
+It performs all message-level checks for [REDbot](https://redbot.org/), but does not perform any 'active' checks by making requests to the network, and it does not have a Web user interface.
 
 
 ## Using httplint as a Library
 
 httplint exposes two classes for linting: `HttpRequestLinter` and `HttpResponseLinter`. They expose the following methods for telling the linter about the HTTP message:
 
 * As appropriate:
```

### Comparing `httplint-2024.1.1/httplint/cache.py` & `httplint-2024.4.1/httplint/cache.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/cli/__init__.py` & `httplint-2024.4.1/httplint/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/cli/http_parser.py` & `httplint-2024.4.1/httplint/cli/http_parser.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/content_encoding.py` & `httplint-2024.4.1/httplint/content_encoding.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/__init__.py` & `httplint-2024.4.1/httplint/field/__init__.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/deprecated.py` & `httplint-2024.4.1/httplint/field/deprecated.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/finder.py` & `httplint-2024.4.1/httplint/field/finder.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/notes.py` & `httplint-2024.4.1/httplint/field/notes.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/accept_ranges.py` & `httplint-2024.4.1/httplint/field/parsers/accept_ranges.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/age.py` & `httplint-2024.4.1/httplint/field/parsers/age.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/allow.py` & `httplint-2024.4.1/httplint/field/parsers/allow.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/cache_control.py` & `httplint-2024.4.1/httplint/field/parsers/cache_control.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/connection.py` & `httplint-2024.4.1/httplint/field/parsers/connection.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/connectiox.py` & `httplint-2024.4.1/httplint/field/parsers/connectiox.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_disposition.py` & `httplint-2024.4.1/httplint/field/parsers/content_disposition.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_encoding.py` & `httplint-2024.4.1/httplint/field/parsers/content_encoding.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_language.py` & `httplint-2024.4.1/httplint/field/parsers/content_language.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_length.py` & `httplint-2024.4.1/httplint/field/parsers/content_length.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_location.py` & `httplint-2024.4.1/httplint/field/parsers/content_location.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_md5.py` & `httplint-2024.4.1/httplint/field/parsers/content_md5.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_range.py` & `httplint-2024.4.1/httplint/field/parsers/content_range.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/content_type.py` & `httplint-2024.4.1/httplint/field/parsers/content_type.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/cteonnt_length.py` & `httplint-2024.4.1/httplint/field/parsers/cteonnt_length.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/date.py` & `httplint-2024.4.1/httplint/field/parsers/date.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/etag.py` & `httplint-2024.4.1/httplint/field/parsers/etag.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/expires.py` & `httplint-2024.4.1/httplint/field/parsers/expires.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/keep_alive.py` & `httplint-2024.4.1/httplint/field/parsers/keep_alive.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/last_modified.py` & `httplint-2024.4.1/httplint/field/parsers/last_modified.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/link.py` & `httplint-2024.4.1/httplint/field/parsers/link.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/location.py` & `httplint-2024.4.1/httplint/field/parsers/location.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/mime_version.py` & `httplint-2024.4.1/httplint/field/parsers/mime_version.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/pragma.py` & `httplint-2024.4.1/httplint/field/parsers/pragma.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/proxy_authenticate.py` & `httplint-2024.4.1/httplint/field/parsers/proxy_authenticate.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/retry_after.py` & `httplint-2024.4.1/httplint/field/parsers/retry_after.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/set_cookie.py` & `httplint-2024.4.1/httplint/field/parsers/set_cookie.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
             cookie_attribute_list.append(("Expires", expiry_time))
         elif case_norm_attribute_name == "max-age":
             if attribute_value == "":
                 add_note(SET_COOKIE_EMPTY_MAX_AGE, cookie_name=cookie_name)
                 continue
             if attribute_value[0] == "0":
                 add_note(SET_COOKIE_LEADING_ZERO_MAX_AGE, cookie_name=cookie_name)
-                continue
             if not attribute_value.isdigit():
                 add_note(SET_COOKIE_NON_DIGIT_MAX_AGE, cookie_name=cookie_name)
                 continue
             delta_seconds = int(attribute_value)
             cookie_attribute_list.append(("Max-Age", delta_seconds))
         elif case_norm_attribute_name == "domain":
             if attribute_value == "":
@@ -124,26 +123,27 @@
                 cookie_samesite = attribute_value
                 add_note(
                     SET_COOKIE_UNKNOWN_ATTRIBUTE_VALUE,
                     cookie_name=cookie_name,
                     attribute_name=attribute_name,
                     attribute_value=attribute_value,
                 )
+                continue
             cookie_attribute_list.append(("SameSite", cookie_samesite))
         else:
             add_note(
                 SET_COOKIE_UNKNOWN_ATTRIBUTE,
                 cookie_name=cookie_name,
                 attribute=attribute_name,
             )
-        if ("SameSite", "None") in cookie_attribute_list and (
-            "Secure",
-            "",
-        ) not in cookie_attribute_list:
-            add_note(SET_COOKIE_NOT_SECURE, cookie_name=cookie_name)
+    if ("SameSite", "None") in cookie_attribute_list and (
+        "Secure",
+        "",
+    ) not in cookie_attribute_list:
+        add_note(SET_COOKIE_NOT_SECURE, cookie_name=cookie_name)
     return (cookie_name, cookie_value, cookie_attribute_list)
 
 
 DELIMITER = r"(?:[\x09\x20-\x2F\x3B-\x40\x5B-\x60\x7B-\x7E])"
 NON_DELIMITER = r"(?:[\x00-\x08\x0A-\x1F0-0\:a-zA-Z\x7F-\xFF])"
 MONTHS = {
     "jan": 1,
@@ -385,15 +385,15 @@
     inputs = [b"lang=en-US; Max-Age=123"]
     expected_out = [("lang", "en-US", [("Max-Age", 123)])]
 
 
 class MaxAgeLeadingZeroScTest(FieldTest):
     name = "Set-Cookie"
     inputs = [b"lang=en-US; Max-Age=0123"]
-    expected_out = [("lang", "en-US", [])]
+    expected_out = [("lang", "en-US", [("Max-Age", 123)])]
     expected_notes = [SET_COOKIE_LEADING_ZERO_MAX_AGE]
 
 
 class RemoveSCTest(FieldTest):
     name = "Set-Cookie"
     inputs = [b"lang=; Expires=Sun, 06 Nov 1994 08:49:37 GMT"]
     expected_out = [("lang", "", [("Expires", 784111777)])]
```

### Comparing `httplint-2024.1.1/httplint/field/parsers/te.py` & `httplint-2024.4.1/httplint/field/parsers/te.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/transfer_encoding.py` & `httplint-2024.4.1/httplint/field/parsers/transfer_encoding.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/upgrade.py` & `httplint-2024.4.1/httplint/field/parsers/upgrade.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/vary.py` & `httplint-2024.4.1/httplint/field/parsers/vary.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/via.py` & `httplint-2024.4.1/httplint/field/parsers/via.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/warning.py` & `httplint-2024.4.1/httplint/field/parsers/warning.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/www_authenticate.py` & `httplint-2024.4.1/httplint/field/parsers/www_authenticate.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/x_cache_lookup.py` & `httplint-2024.4.1/httplint/field/parsers/x_cache_lookup.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/x_content_type_options.py` & `httplint-2024.4.1/httplint/field/parsers/x_content_type_options.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/x_frame_options.py` & `httplint-2024.4.1/httplint/field/parsers/x_frame_options.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/x_pad.py` & `httplint-2024.4.1/httplint/field/parsers/x_pad.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/parsers/x_xss_protection.py` & `httplint-2024.4.1/httplint/field/parsers/x_xss_protection.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/section.py` & `httplint-2024.4.1/httplint/field/section.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/tests.py` & `httplint-2024.4.1/httplint/field/tests.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/field/utils.py` & `httplint-2024.4.1/httplint/field/utils.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/message.py` & `httplint-2024.4.1/httplint/message.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/note.py` & `httplint-2024.4.1/httplint/note.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/status.py` & `httplint-2024.4.1/httplint/status.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc3986.py` & `httplint-2024.4.1/httplint/syntax/rfc3986.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc5234.py` & `httplint-2024.4.1/httplint/syntax/rfc5234.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc5322.py` & `httplint-2024.4.1/httplint/syntax/rfc5322.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc5646.py` & `httplint-2024.4.1/httplint/syntax/rfc5646.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc5987.py` & `httplint-2024.4.1/httplint/syntax/rfc5987.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc5988.py` & `httplint-2024.4.1/httplint/syntax/rfc5988.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc7230.py` & `httplint-2024.4.1/httplint/syntax/rfc7230.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc7231.py` & `httplint-2024.4.1/httplint/syntax/rfc7231.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc7232.py` & `httplint-2024.4.1/httplint/syntax/rfc7232.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc7233.py` & `httplint-2024.4.1/httplint/syntax/rfc7233.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc7234.py` & `httplint-2024.4.1/httplint/syntax/rfc7234.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc7235.py` & `httplint-2024.4.1/httplint/syntax/rfc7235.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/syntax/rfc9110.py` & `httplint-2024.4.1/httplint/syntax/rfc9110.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/httplint/util.py` & `httplint-2024.4.1/httplint/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from binascii import b2a_hex
 import locale
 import time
-from typing import Optional, List
+from typing import List
 import unittest
 from urllib.parse import urlsplit, urlunsplit, quote as urlquote
 
 
 def iri_to_uri(iri: str) -> str:
     "Takes a string that can contain an IRI and return a URI."
     scheme, authority, path, query, frag = urlsplit(iri)
@@ -66,31 +66,29 @@
     if length == 2:
         return f"{mu}{inlist[0]}{mu} and {mu}{inlist[1]}{mu}"
     return (
         f"{', '.join([f'{mu}{i}{mu}' for i in inlist[:-1]])}, and {mu}{inlist[-1]}{mu}"
     )
 
 
-def relative_time(utime: float, now: Optional[float] = None, show_sign: int = 1) -> str:
+def relative_time(utime: float, now: float, show_sign: int = 1) -> str:
     """
     Given two times, return a string that explains how far apart they are.
     show_sign can be:
         0 - don't show
         1 - ago / from now  [DEFAULT]
         2 - early / late
     """
 
     signs = {
         0: ("0", "", ""),
         1: ("now", "ago", "from now"),
         2: ("none", "behind", "ahead"),
     }
 
-    if now is None:
-        now = time.time()
     age = round(now - utime)
     if age == 0:
         return signs[show_sign][0]
 
     aa = abs(age)
     yrs = int(aa / 60 / 60 / 24 / 365)
     day = int(aa / 60 / 60 / 24) % 365
```

### Comparing `httplint-2024.1.1/httplint.egg-info/PKG-INFO` & `httplint-2024.4.1/httplint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httplint
-Version: 2024.1.1
+Version: 2024.4.1
 Summary: Lint for HTTP messages.
 Author-email: Mark Nottingham <mnot@mnot.net>
 License: Copyright (c) Mark Nottingham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -50,15 +50,15 @@
 Requires-Dist: types-Markdown; extra == "dev"
 
 
 # httplint
 
 This Python library _lints_ HTTP messages; it checks them for correctness and reports any issues it finds.
 
-It has been extracted from [REDbot](https://redbot.org/), which will eventually depend upon it. Unlike REDbot, it does not perform any 'active' checks by making requests to the network, and it does not have a Web user interface.
+It performs all message-level checks for [REDbot](https://redbot.org/), but does not perform any 'active' checks by making requests to the network, and it does not have a Web user interface.
 
 
 ## Using httplint as a Library
 
 httplint exposes two classes for linting: `HttpRequestLinter` and `HttpResponseLinter`. They expose the following methods for telling the linter about the HTTP message:
 
 * As appropriate:
```

### Comparing `httplint-2024.1.1/httplint.egg-info/SOURCES.txt` & `httplint-2024.4.1/httplint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/pyproject.toml` & `httplint-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/test/test_fields.py` & `httplint-2024.4.1/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/test/test_notes.py` & `httplint-2024.4.1/test/test_notes.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/test/test_syntax.py` & `httplint-2024.4.1/test/test_syntax.py`

 * *Files identical despite different names*

### Comparing `httplint-2024.1.1/test/utils.py` & `httplint-2024.4.1/test/utils.py`

 * *Files identical despite different names*

