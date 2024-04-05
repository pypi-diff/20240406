# Comparing `tmp/njsscan-0.3.6.tar.gz` & `tmp/njsscan-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njsscan-0.3.6.tar", last modified: Wed Aug 30 04:54:25 2023, max compression
+gzip compressed data, was "njsscan-0.3.7.tar", last modified: Fri Apr  5 22:02:21 2024, max compression
```

## Comparing `njsscan-0.3.6.tar` & `njsscan-0.3.7.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.868480 njsscan-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (999)     7651 2023-08-30 04:54:10.000000 njsscan-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      147 2023-08-30 04:54:10.000000 njsscan-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)    13903 2023-08-30 04:54:25.868480 njsscan-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    13356 2023-08-30 04:54:10.000000 njsscan-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.856479 njsscan-0.3.6/njsscan/
--rw-r--r--   0 runner    (1001) docker     (999)      408 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3647 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      178 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/formatters/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2901 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/formatters/cli.py
--rw-r--r--   0 runner    (1001) docker     (999)      429 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (999)     5484 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/formatters/sarif.py
--rw-r--r--   0 runner    (1001) docker     (999)     1840 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/formatters/sonarqube.py
--rw-r--r--   0 runner    (1001) docker     (999)     1538 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/logger.py
--rw-r--r--   0 runner    (1001) docker     (999)     5903 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/njsscan.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/rules/
--rw-r--r--   0 runner    (1001) docker     (999)     2724 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/missing_controls.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/rules/pattern_matcher/
--rw-r--r--   0 runner    (1001) docker     (999)     2864 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/pattern_matcher/template_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.856479 njsscan-0.3.6/njsscan/rules/semantic_grep/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/
--rw-r--r--   0 runner    (1001) docker     (999)     2416 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/crypto_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    13303 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/timing_attack_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      788 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/tls_node.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/rules/semantic_grep/database/
--rw-r--r--   0 runner    (1001) docker     (999)     1962 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/nosql_find_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1502 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/nosql_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1140 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/sequelize_tls.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1120 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/sequelize_tls_validation.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1089 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/sequelize_weak_tls.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1510 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/sql_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2105 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/database/sql_injection_knex.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/rules/semantic_grep/dos/
--rw-r--r--   0 runner    (1001) docker     (999)      443 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/dos/express_bodyparser_dos.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/dos/layer7_object_dos.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2213 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/dos/regex_dos.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2333 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/dos/regex_injection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan/rules/semantic_grep/electronjs/
--rw-r--r--   0 runner    (1001) docker     (999)     3147 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/electronjs/security_electron.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/
--rw-r--r--   0 runner    (1001) docker     (999)      864 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_deserialize.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_grpc_deserialize.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2449 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1040 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_require.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1587 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_sandbox.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     9113 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_vm2_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    11622 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_vm_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      375 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_yaml_deserialize.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2738 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/eval/server_side_template_injection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/exec/
--rw-r--r--   0 runner    (1001) docker     (999)     1653 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/exec/exec_os_command.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1162 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/exec/exec_shelljs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/generic/
--rw-r--r--   0 runner    (1001) docker     (999)     1515 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/generic/error_disclosure.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    16017 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/generic/hardcoded_passport.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2261 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/generic/hardcoded_secrets.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2008 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/generic/logic_bypass.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/good/
--rw-r--r--   0 runner    (1001) docker     (999)      521 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/good/good_anti_csrf.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     7340 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/good/good_helmet_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      377 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/good/good_ratelimiting.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/
--rw-r--r--   0 runner    (1001) docker     (999)    10458 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1580 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_cors_star.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1251 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_helmet_disabled.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1945 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_injection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1558 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_xss_protection.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2053 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/headers/host_header_injection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/
--rw-r--r--   0 runner    (1001) docker     (999)     6449 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_exposed_credentials.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      870 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_exposed_data.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      873 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_express_hardcoded.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2366 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_hardcoded.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1201 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_none_algorithm.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      631 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_not_revoked.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/memory/
--rw-r--r--   0 runner    (1001) docker     (999)     1699 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/memory/buffer_noassert.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/redirect/
--rw-r--r--   0 runner    (1001) docker     (999)     2991 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/redirect/open_redirect.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.864479 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/
--rw-r--r--   0 runner    (1001) docker     (999)     6576 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2856 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_phantomjs.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     4101 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_playwright.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     4252 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_puppeteer.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1200 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltoimage.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1186 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltopdf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.868480 njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/
--rw-r--r--   0 runner    (1001) docker     (999)     4859 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/archive_path_overwrite.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1711 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/express_hbs_lfr.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     4330 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/path_traversal.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1628 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/resolve_path_traversal.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.868480 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/
--rw-r--r--   0 runner    (1001) docker     (999)     1143 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xml_entity_expansion_dos.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2184 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xpathi_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1786 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_expat.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     4352 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_sax.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1169 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_xml2json.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.868480 njsscan-0.3.6/njsscan/rules/semantic_grep/xss/
--rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_mustache_escape.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     4919 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_node.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_serialize_js.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1076 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_templates.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1712 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/settings.py
--rw-r--r--   0 runner    (1001) docker     (999)     3190 2023-08-30 04:54:10.000000 njsscan-0.3.6/njsscan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 04:54:25.860479 njsscan-0.3.6/njsscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    13903 2023-08-30 04:54:25.000000 njsscan-0.3.6/njsscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4343 2023-08-30 04:54:25.000000 njsscan-0.3.6/njsscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 04:54:25.000000 njsscan-0.3.6/njsscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       85 2023-08-30 04:54:25.000000 njsscan-0.3.6/njsscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       89 2023-08-30 04:54:25.000000 njsscan-0.3.6/njsscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-30 04:54:25.000000 njsscan-0.3.6/njsscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-30 04:54:25.868480 njsscan-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1593 2023-08-30 04:54:10.000000 njsscan-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.148392 njsscan-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-05 22:02:12.000000 njsscan-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 22:02:12.000000 njsscan-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-04-05 22:02:21.148392 njsscan-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-04-05 22:02:12.000000 njsscan-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.132392 njsscan-0.3.7/njsscan/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.136392 njsscan-0.3.7/njsscan/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/formatters/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/formatters/json_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/formatters/sarif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/formatters/sonarqube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/njsscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.136392 njsscan-0.3.7/njsscan/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/missing_controls.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.136392 njsscan-0.3.7/njsscan/rules/pattern_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/pattern_matcher/template_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.132392 njsscan-0.3.7/njsscan/rules/semantic_grep/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.136392 njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/crypto_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/timing_attack_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/tls_node.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.136392 njsscan-0.3.7/njsscan/rules/semantic_grep/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/nosql_find_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/nosql_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/sequelize_tls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/sequelize_tls_validation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/sequelize_weak_tls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/sql_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/database/sql_injection_knex.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.136392 njsscan-0.3.7/njsscan/rules/semantic_grep/dos/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/dos/express_bodyparser_dos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/dos/layer7_object_dos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/dos/regex_dos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/dos/regex_injection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.140392 njsscan-0.3.7/njsscan/rules/semantic_grep/electronjs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/electronjs/security_electron.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.140392 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_deserialize.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_grpc_deserialize.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_require.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_sandbox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_vm2_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_vm_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_yaml_deserialize.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/eval/server_side_template_injection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.140392 njsscan-0.3.7/njsscan/rules/semantic_grep/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/exec/exec_os_command.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/exec/exec_shelljs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.140392 njsscan-0.3.7/njsscan/rules/semantic_grep/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/generic/error_disclosure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/generic/hardcoded_passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/generic/hardcoded_secrets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/generic/logic_bypass.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.140392 njsscan-0.3.7/njsscan/rules/semantic_grep/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/good/good_anti_csrf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/good/good_helmet_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/good/good_ratelimiting.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.140392 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_cors_star.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_helmet_disabled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_injection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_xss_protection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/headers/host_header_injection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.144392 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_exposed_credentials.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_exposed_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_express_hardcoded.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_hardcoded.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_none_algorithm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_not_revoked.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.144392 njsscan-0.3.7/njsscan/rules/semantic_grep/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/memory/buffer_noassert.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.144392 njsscan-0.3.7/njsscan/rules/semantic_grep/redirect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/redirect/open_redirect.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.144392 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_phantomjs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_playwright.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_puppeteer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltoimage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltopdf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.144392 njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/archive_path_overwrite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/express_hbs_lfr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/path_traversal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/resolve_path_traversal.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.144392 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xml_entity_expansion_dos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xpathi_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_expat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_sax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_xml2json.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.148392 njsscan-0.3.7/njsscan/rules/semantic_grep/xss/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_mustache_escape.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_serialize_js.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_templates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-05 22:02:12.000000 njsscan-0.3.7/njsscan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:02:21.148392 njsscan-0.3.7/njsscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-04-05 22:02:21.000000 njsscan-0.3.7/njsscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-05 22:02:21.000000 njsscan-0.3.7/njsscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:02:21.000000 njsscan-0.3.7/njsscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 22:02:21.000000 njsscan-0.3.7/njsscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 22:02:21.000000 njsscan-0.3.7/njsscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 22:02:21.000000 njsscan-0.3.7/njsscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:02:21.148392 njsscan-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 22:02:12.000000 njsscan-0.3.7/setup.py
```

### Comparing `njsscan-0.3.6/LICENSE` & `njsscan-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/PKG-INFO` & `njsscan-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: njsscan
-Version: 0.3.6
-Summary: njsscan is a SAST tool that can find insecure code patterns in your Node.js applications.
-Home-page: https://github.com/ajinabraham/njsscan
-Author: Ajin Abraham
-Author-email: ajin25@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # njsscan
 **njsscan** is a static application testing (SAST) tool that can find insecure code patterns in your node.js applications using simple pattern matcher from [libsast](https://github.com/ajinabraham/libsast) and syntax-aware semantic code pattern search tool [semgrep](https://github.com/returntocorp/semgrep).
 
 Made with ![Love](https://cloud.githubusercontent.com/assets/4301109/16754758/82e3a63c-4813-11e6-9430-6015d98aeaab.png) in India  [![Tweet](https://img.shields.io/twitter/url?url=https://github.com/ajinabraham/njsscan)](https://twitter.com/intent/tweet/?text=njsscan%20is%20a%20semantic%20aware%20SAST%20tool%20that%20can%20find%20insecure%20code%20patterns%20in%20your%20Node.js%20applications%20by%20%40ajinabraham%20%40OpenSecurity_IN&url=https://github.com/ajinabraham/njsscan)
 
 [![PyPI version](https://badge.fury.io/py/njsscan.svg)](https://badge.fury.io/py/njsscan)
 [![platform](https://img.shields.io/badge/platform-osx%2Flinux-green.svg)](https://github.com/ajinabraham/njsscan)
```

### Comparing `njsscan-0.3.6/README.md` & `njsscan-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: njsscan
+Version: 0.3.7
+Summary: njsscan is a SAST tool that can find insecure code patterns in your Node.js applications.
+Home-page: https://github.com/ajinabraham/njsscan
+Author: Ajin Abraham
+Author-email: ajin25@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: colorama>=0.4.5
+Requires-Dist: libsast>=2.0.0
+Requires-Dist: sarif-om>=1.0.4
+Requires-Dist: jschema-to-python>=1.2.3
+Requires-Dist: tabulate>=0.8.10
+
 # njsscan
 **njsscan** is a static application testing (SAST) tool that can find insecure code patterns in your node.js applications using simple pattern matcher from [libsast](https://github.com/ajinabraham/libsast) and syntax-aware semantic code pattern search tool [semgrep](https://github.com/returntocorp/semgrep).
 
 Made with ![Love](https://cloud.githubusercontent.com/assets/4301109/16754758/82e3a63c-4813-11e6-9430-6015d98aeaab.png) in India  [![Tweet](https://img.shields.io/twitter/url?url=https://github.com/ajinabraham/njsscan)](https://twitter.com/intent/tweet/?text=njsscan%20is%20a%20semantic%20aware%20SAST%20tool%20that%20can%20find%20insecure%20code%20patterns%20in%20your%20Node.js%20applications%20by%20%40ajinabraham%20%40OpenSecurity_IN&url=https://github.com/ajinabraham/njsscan)
 
 [![PyPI version](https://badge.fury.io/py/njsscan.svg)](https://badge.fury.io/py/njsscan)
 [![platform](https://img.shields.io/badge/platform-osx%2Flinux-green.svg)](https://github.com/ajinabraham/njsscan)
```

### Comparing `njsscan-0.3.6/njsscan/__main__.py` & `njsscan-0.3.7/njsscan/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 import sys
 
 from njsscan import __version__
 from njsscan.njsscan import NJSScan
 from njsscan.formatters import (
     cli,
-    json,
+    json_out,
     sarif,
     sonarqube,
 )
 
 
 def handle_exit(results, exit_warn):
     """Handle Exit."""
@@ -77,15 +77,15 @@
         ).scan()
         if args.sonarqube:
             sonarqube.sonarqube_output(
                 args.output,
                 scan_results,
                 __version__)
         elif args.json:
-            json.json_output(
+            json_out.json_output(
                 args.output,
                 scan_results,
                 __version__)
         elif args.sarif:
             sarif.sarif_output(
                 args.output,
                 scan_results,
```

### Comparing `njsscan-0.3.6/njsscan/formatters/cli.py` & `njsscan-0.3.7/njsscan/formatters/cli.py`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/formatters/sarif.py` & `njsscan-0.3.7/njsscan/formatters/sarif.py`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/formatters/sonarqube.py` & `njsscan-0.3.7/njsscan/formatters/sonarqube.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf_8 -*-
 """Sonarqube output format."""
 
-from njsscan.formatters.json import json_output
+from njsscan.formatters.json_out import json_output
 
 
 def get_sonarqube_issue(njsscan_issue):
     sonarqube_severity_mapping = {
         'ERROR': 'CRITICAL',
         'WARNING': 'MAJOR',
         'INFO': 'MINOR',
```

### Comparing `njsscan-0.3.6/njsscan/logger.py` & `njsscan-0.3.7/njsscan/logger.py`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/njsscan.py` & `njsscan-0.3.7/njsscan/njsscan.py`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/missing_controls.yaml` & `njsscan-0.3.7/njsscan/rules/missing_controls.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/pattern_matcher/template_rules.yaml` & `njsscan-0.3.7/njsscan/rules/pattern_matcher/template_rules.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/crypto_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/crypto_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/timing_attack_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/timing_attack_node.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -481,14 +481,15 @@
               return secret != $X;
           - pattern: |
               return $X != api;
           - pattern: |
               return api != $X;
     message: >-
       String comparisons using '===', '!==', '!=' and '==' is vulnerable to timing attacks.
-      More info: https://snyk.io/blog/node-js-timing-attack-ccc-ctf/
+      A timing attack allows the attacker to learn potentially sensitive information by, for example, measuring how long it takes for the application to respond to a request. 
+      More info: https://nodejs.org/en/learn/getting-started/security-best-practices#information-exposure-through-timing-attacks-cwe-208
     languages:
       - javascript
     severity: WARNING
     metadata:
       owasp-web: a9
       cwe: cwe-208
```

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/crypto/tls_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/crypto/tls_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/nosql_find_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/nosql_find_injection.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 rules:
 - id: node_nosqli_injection
   patterns:
   - pattern-not-inside: |
+      $SEQUELIZE = require('sequelize')
+      ...
+      $SEQUELIZE(...)
+      ...
+  - pattern-not-inside: |
+      import $SEQUELIZE from 'sequelize'
+      ...
+      $SEQUELIZE(...)
+      ...
+  - pattern-not-inside: |
       $SANITIZE = require('mongo-sanitize')
       ...
       $SANITIZE(...)
       ...
   - pattern-not-inside: |
       import $SANITIZE from 'mongo-sanitize'
       ...
```

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/nosql_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/nosql_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/sequelize_tls.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/sequelize_tls.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/sequelize_tls_validation.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/sequelize_tls_validation.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/sequelize_weak_tls.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/sequelize_weak_tls.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/sql_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/sql_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/database/sql_injection_knex.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/database/sql_injection_knex.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/dos/layer7_object_dos.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/dos/layer7_object_dos.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/dos/regex_dos.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/dos/regex_dos.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/dos/regex_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/dos/regex_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/electronjs/security_electron.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/electronjs/security_electron.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_deserialize.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_deserialize.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_require.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_require.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_sandbox.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_sandbox.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_vm2_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_vm2_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/eval_vm_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/eval_vm_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/eval/server_side_template_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/eval/server_side_template_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/exec/exec_os_command.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/exec/exec_os_command.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/exec/exec_shelljs.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/exec/exec_shelljs.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/generic/error_disclosure.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/generic/error_disclosure.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/generic/hardcoded_passport.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/generic/hardcoded_passport.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/generic/hardcoded_secrets.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/generic/hardcoded_secrets.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/generic/logic_bypass.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/generic/logic_bypass.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/good/good_anti_csrf.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/good/good_anti_csrf.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/good/good_helmet_checks.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/good/good_helmet_checks.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_cookie.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_cookie.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_cors_star.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_cors_star.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_helmet_disabled.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_helmet_disabled.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/headers/header_xss_protection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/headers/header_xss_protection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/headers/host_header_injection.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/headers/host_header_injection.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_exposed_credentials.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_exposed_credentials.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_exposed_data.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_exposed_data.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_express_hardcoded.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_express_hardcoded.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_hardcoded.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_hardcoded.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_none_algorithm.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_none_algorithm.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/jwt/jwt_not_revoked.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/jwt/jwt_not_revoked.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/memory/buffer_noassert.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/memory/buffer_noassert.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/redirect/open_redirect.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/redirect/open_redirect.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_phantomjs.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_phantomjs.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_playwright.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_playwright.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_puppeteer.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_puppeteer.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltoimage.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltoimage.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltopdf.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/ssrf/ssrf_wkhtmltopdf.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/archive_path_overwrite.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/archive_path_overwrite.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/express_hbs_lfr.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/express_hbs_lfr.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/path_traversal.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/path_traversal.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/traversal/resolve_path_traversal.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/traversal/resolve_path_traversal.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xml_entity_expansion_dos.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xml_entity_expansion_dos.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xpathi_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xpathi_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_expat.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_expat.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_sax.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_sax.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xml/xxe_xml2json.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xml/xxe_xml2json.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_node.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_node.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_serialize_js.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_serialize_js.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/rules/semantic_grep/xss/xss_templates.yaml` & `njsscan-0.3.7/njsscan/rules/semantic_grep/xss/xss_templates.yaml`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/settings.py` & `njsscan-0.3.7/njsscan/settings.py`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan/utils.py` & `njsscan-0.3.7/njsscan/utils.py`

 * *Files identical despite different names*

### Comparing `njsscan-0.3.6/njsscan.egg-info/PKG-INFO` & `njsscan-0.3.7/njsscan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: njsscan
-Version: 0.3.6
+Version: 0.3.7
 Summary: njsscan is a SAST tool that can find insecure code patterns in your Node.js applications.
 Home-page: https://github.com/ajinabraham/njsscan
 Author: Ajin Abraham
 Author-email: ajin25@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorama>=0.4.5
+Requires-Dist: libsast>=2.0.0
+Requires-Dist: sarif-om>=1.0.4
+Requires-Dist: jschema-to-python>=1.2.3
+Requires-Dist: tabulate>=0.8.10
 
 # njsscan
 **njsscan** is a static application testing (SAST) tool that can find insecure code patterns in your node.js applications using simple pattern matcher from [libsast](https://github.com/ajinabraham/libsast) and syntax-aware semantic code pattern search tool [semgrep](https://github.com/returntocorp/semgrep).
 
 Made with ![Love](https://cloud.githubusercontent.com/assets/4301109/16754758/82e3a63c-4813-11e6-9430-6015d98aeaab.png) in India  [![Tweet](https://img.shields.io/twitter/url?url=https://github.com/ajinabraham/njsscan)](https://twitter.com/intent/tweet/?text=njsscan%20is%20a%20semantic%20aware%20SAST%20tool%20that%20can%20find%20insecure%20code%20patterns%20in%20your%20Node.js%20applications%20by%20%40ajinabraham%20%40OpenSecurity_IN&url=https://github.com/ajinabraham/njsscan)
 
 [![PyPI version](https://badge.fury.io/py/njsscan.svg)](https://badge.fury.io/py/njsscan)
```

### Comparing `njsscan-0.3.6/njsscan.egg-info/SOURCES.txt` & `njsscan-0.3.7/njsscan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 njsscan.egg-info/SOURCES.txt
 njsscan.egg-info/dependency_links.txt
 njsscan.egg-info/entry_points.txt
 njsscan.egg-info/requires.txt
 njsscan.egg-info/top_level.txt
 njsscan/formatters/__init__.py
 njsscan/formatters/cli.py
-njsscan/formatters/json.py
+njsscan/formatters/json_out.py
 njsscan/formatters/sarif.py
 njsscan/formatters/sonarqube.py
 njsscan/rules/missing_controls.yaml
 njsscan/rules/pattern_matcher/template_rules.yaml
 njsscan/rules/semantic_grep/crypto/crypto_node.yaml
 njsscan/rules/semantic_grep/crypto/timing_attack_node.yaml
 njsscan/rules/semantic_grep/crypto/tls_node.yaml
```

### Comparing `njsscan-0.3.6/setup.py` & `njsscan-0.3.7/setup.py`

 * *Files identical despite different names*

