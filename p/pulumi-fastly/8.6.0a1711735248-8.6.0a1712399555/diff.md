# Comparing `tmp/pulumi_fastly-8.6.0a1711735248.tar.gz` & `tmp/pulumi_fastly-8.6.0a1712399555.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.6.0a1711735248.tar", last modified: Fri Mar 29 18:22:15 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.6.0a1712399555.tar", last modified: Sat Apr  6 10:41:47 2024, max compression
```

## Comparing `pulumi_fastly-8.6.0a1711735248.tar` & `pulumi_fastly-8.6.0a1712399555.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:22:15.410050 pulumi_fastly-8.6.0a1711735248/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-03-29 18:22:15.410050 pulumi_fastly-8.6.0a1711735248/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:22:15.410050 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   524197 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:22:15.410050 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   472508 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    92270 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23295 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 18:22:15.410050 pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-03-29 18:22:15.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-29 18:22:15.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 18:22:15.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 18:22:15.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 18:22:15.000000 pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-29 18:22:05.000000 pulumi_fastly-8.6.0a1711735248/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 18:22:15.410050 pulumi_fastly-8.6.0a1711735248/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:41:47.326328 pulumi_fastly-8.6.0a1712399555/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-06 10:41:47.326328 pulumi_fastly-8.6.0a1712399555/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:41:47.326328 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   521997 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:41:47.326328 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470308 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92270 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23295 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:41:47.326328 pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-06 10:41:47.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 10:41:47.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:41:47.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 10:41:47.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 10:41:47.000000 pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-06 10:41:40.000000 pulumi_fastly-8.6.0a1712399555/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:41:47.326328 pulumi_fastly-8.6.0a1712399555/setup.cfg
```

### Comparing `pulumi_fastly-8.6.0a1711735248/PKG-INFO` & `pulumi_fastly-8.6.0a1712399555/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1711735248
+Version: 8.6.0a1712399555
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1711735248/README.md` & `pulumi_fastly-8.6.0a1712399555/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/__init__.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,15 +919,15 @@
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred in seconds. Default `3600`
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "account_name", account_name)
         pulumi.set(__self__, "container", container)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "sas_token", sas_token)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -1078,15 +1078,15 @@
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -1114,15 +1114,15 @@
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] region: The region to stream logs to. One of: DFW (Dallas), ORD (Chicago), IAD (Northern Virginia), LON (London), SYD (Sydney), HKG (Hong Kong)
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -1273,15 +1273,15 @@
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -1362,15 +1362,15 @@
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "secret_key", secret_key)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -1521,15 +1521,15 @@
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -1753,15 +1753,15 @@
         :param pulumi.Input[str] user: The username for the server (can be `anonymous`)
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param pulumi.Input[int] port: The port number. Default: `21`
         :param pulumi.Input[str] public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -1911,15 +1911,15 @@
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -1946,15 +1946,15 @@
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param pulumi.Input[str] user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
@@ -2096,15 +2096,15 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -3131,15 +3131,15 @@
         :param pulumi.Input[str] user: The username for your OpenStack account
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "url", url)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -3289,15 +3289,15 @@
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -3389,15 +3389,15 @@
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param pulumi.Input[str] s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param pulumi.Input[str] s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param pulumi.Input[str] s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param pulumi.Input[str] server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
         :param pulumi.Input[str] server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -3634,15 +3634,15 @@
     def server_side_encryption_kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_side_encryption_kms_key_id", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -3743,15 +3743,15 @@
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[int] port: The port the SFTP service listens on. (Default: `22`)
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] secret_key: The SSH private key for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "ssh_known_hosts", ssh_known_hosts)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -3929,15 +3929,15 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -6050,24 +6050,24 @@
         """
         :param pulumi.Input[str] account_name: The unique Azure Blob Storage namespace in which your data objects are stored
         :param pulumi.Input[str] container: The name of the Azure Blob Storage container in which to store logs
         :param pulumi.Input[str] name: A unique name to identify the Azure Blob Storage endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] sas_token: The Azure shared access signature providing write access to the blob service objects. Be sure to update your token before it expires or the logging functionality will not work
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
-        :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred in seconds. Default `3600`
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] response_condition: The name of the condition to apply
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "account_name", account_name)
         pulumi.set(__self__, "container", container)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "sas_token", sas_token)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -6166,15 +6166,15 @@
     def file_max_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "file_max_bytes", value)
 
     @property
     @pulumi.getter
     def format(self) -> Optional[pulumi.Input[str]]:
         """
-        Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         """
         return pulumi.get(self, "format")
 
     @format.setter
     def format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "format", value)
 
@@ -6274,15 +6274,15 @@
     def response_condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "response_condition", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -6318,15 +6318,15 @@
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
         :param pulumi.Input[str] public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] region: The region to stream logs to. One of: DFW (Dallas), ORD (Chicago), IAD (Northern Virginia), LON (London), SYD (Sydney), HKG (Hong Kong)
         :param pulumi.Input[str] response_condition: The name of an existing condition in the configured endpoint, or leave blank to always execute.
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -6533,15 +6533,15 @@
     def response_condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "response_condition", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -6694,15 +6694,15 @@
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: The path to upload logs to
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] response_condition: The name of an existing condition in the configured endpoint, or leave blank to always execute.
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "secret_key", secret_key)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -6909,15 +6909,15 @@
     def response_condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "response_condition", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -7213,15 +7213,15 @@
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
         :param pulumi.Input[int] port: The port number. Default: `21`
         :param pulumi.Input[str] public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] response_condition: The name of the condition to apply.
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -7427,15 +7427,15 @@
     def response_condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "response_condition", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -7470,15 +7470,15 @@
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
         :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] response_condition: Name of a condition to apply this logging.
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param pulumi.Input[str] user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
@@ -7676,15 +7676,15 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -9492,15 +9492,15 @@
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] response_condition: The name of an existing condition in the configured endpoint, or leave blank to always execute.
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "url", url)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -9706,15 +9706,15 @@
     def response_condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "response_condition", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -9878,15 +9878,15 @@
         :param pulumi.Input[str] redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param pulumi.Input[str] response_condition: Name of blockAttributes condition to apply this logging.
         :param pulumi.Input[str] s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param pulumi.Input[str] s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param pulumi.Input[str] s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param pulumi.Input[str] server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
         :param pulumi.Input[str] server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -10179,15 +10179,15 @@
     def server_side_encryption_kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_side_encryption_kms_key_id", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -10360,15 +10360,15 @@
         :param pulumi.Input[str] password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param pulumi.Input[int] period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
         :param pulumi.Input[int] port: The port the SFTP service listens on. (Default: `22`)
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] response_condition: The name of the condition to apply.
         :param pulumi.Input[str] secret_key: The SSH private key for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
-        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "ssh_known_hosts", ssh_known_hosts)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -10602,15 +10602,15 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[pulumi.Input[str]]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @timestamp_format.setter
     def timestamp_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timestamp_format", value)
 
@@ -10630,15 +10630,15 @@
                  tls_client_key: Optional[pulumi.Input[str]] = None,
                  tls_hostname: Optional[pulumi.Input[str]] = None,
                  use_tls: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] name: A unique name to identify the Splunk endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] token: The Splunk token to be used for authentication
         :param pulumi.Input[str] url: The Splunk URL to stream logs to
-        :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed
         :param pulumi.Input[str] response_condition: The name of the condition to apply
         :param pulumi.Input[str] tls_ca_cert: A secure certificate to authenticate the server with. Must be in PEM format. You can provide this certificate via an environment variable, `FASTLY_SPLUNK_CA_CERT`
         :param pulumi.Input[str] tls_client_cert: The client certificate used to make authenticated requests. Must be in PEM format.
         :param pulumi.Input[str] tls_client_key: The client private key used to make authenticated requests. Must be in PEM format.
         :param pulumi.Input[str] tls_hostname: The hostname used to verify the server's certificate. It can either be the Common Name or a Subject Alternative Name (SAN)
@@ -10702,15 +10702,15 @@
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter
     def format(self) -> Optional[pulumi.Input[str]]:
         """
-        Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         """
         return pulumi.get(self, "format")
 
     @format.setter
     def format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "format", value)
```

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/alert.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/configstore.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_services.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/outputs.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -860,15 +860,15 @@
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param int period: How frequently the logs should be transferred in seconds. Default `3600`
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "account_name", account_name)
         pulumi.set(__self__, "container", container)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "sas_token", sas_token)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -975,15 +975,15 @@
         """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingCloudfile(dict):
     @staticmethod
@@ -1036,15 +1036,15 @@
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str region: The region to stream logs to. One of: DFW (Dallas), ORD (Chicago), IAD (Northern Virginia), LON (London), SYD (Sydney), HKG (Hong Kong)
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -1151,15 +1151,15 @@
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingDatadog(dict):
     def __init__(__self__, *,
@@ -1255,15 +1255,15 @@
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param str domain: The domain of the DigitalOcean Spaces endpoint (default `nyc3.digitaloceanspaces.com`)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "secret_key", secret_key)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -1370,15 +1370,15 @@
         """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingElasticsearch(dict):
     @staticmethod
@@ -1602,15 +1602,15 @@
         :param str user: The username for the server (can be `anonymous`)
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param int period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param int port: The port number. Default: `21`
         :param str public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -1716,15 +1716,15 @@
         """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingGc(dict):
     @staticmethod
@@ -1778,15 +1778,15 @@
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param str project_id: The ID of your Google Cloud Platform project
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param str user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
@@ -1888,15 +1888,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
@@ -2839,15 +2839,15 @@
         :param str user: The username for your OpenStack account
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "url", url)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -2953,15 +2953,15 @@
         """
         return pulumi.get(self, "public_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingPapertrail(dict):
     def __init__(__self__, *,
@@ -3076,15 +3076,15 @@
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param str s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param str s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param str s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param str server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
         :param str server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -3253,15 +3253,15 @@
         """
         return pulumi.get(self, "server_side_encryption_kms_key_id")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingScalyr(dict):
     @staticmethod
@@ -3388,15 +3388,15 @@
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param int port: The port the SFTP service listens on. (Default: `22`)
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str secret_key: The SSH private key for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "ssh_known_hosts", ssh_known_hosts)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -3522,15 +3522,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceComputeLoggingSplunk(dict):
     @staticmethod
@@ -5496,24 +5496,24 @@
         """
         :param str account_name: The unique Azure Blob Storage namespace in which your data objects are stored
         :param str container: The name of the Azure Blob Storage container in which to store logs
         :param str name: A unique name to identify the Azure Blob Storage endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str sas_token: The Azure shared access signature providing write access to the blob service objects. Be sure to update your token before it expires or the logging functionality will not work
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
-        :param str format: Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        :param str format: Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to. Must end with a trailing slash. If this field is left empty, the files will be saved in the container's root path
         :param int period: How frequently the logs should be transferred in seconds. Default `3600`
         :param str placement: Where in the generated VCL the logging call should be placed
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str response_condition: The name of the condition to apply
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "account_name", account_name)
         pulumi.set(__self__, "container", container)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "sas_token", sas_token)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -5588,15 +5588,15 @@
         """
         return pulumi.get(self, "file_max_bytes")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
-        Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         """
         return pulumi.get(self, "format")
 
     @property
     @pulumi.getter(name="formatVersion")
     def format_version(self) -> Optional[int]:
         """
@@ -5660,15 +5660,15 @@
         """
         return pulumi.get(self, "response_condition")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingCloudfile(dict):
     @staticmethod
@@ -5733,15 +5733,15 @@
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
         :param str public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str region: The region to stream logs to. One of: DFW (Dallas), ORD (Chicago), IAD (Northern Virginia), LON (London), SYD (Sydney), HKG (Hong Kong)
         :param str response_condition: The name of an existing condition in the configured endpoint, or leave blank to always execute.
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -5888,15 +5888,15 @@
         """
         return pulumi.get(self, "response_condition")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingDatadog(dict):
     @staticmethod
@@ -6071,15 +6071,15 @@
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: The path to upload logs to
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str response_condition: The name of an existing condition in the configured endpoint, or leave blank to always execute.
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "secret_key", secret_key)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -6226,15 +6226,15 @@
         """
         return pulumi.get(self, "response_condition")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingElasticsearch(dict):
     @staticmethod
@@ -6522,15 +6522,15 @@
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param int period: How frequently the logs should be transferred, in seconds (Default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed.
         :param int port: The port number. Default: `21`
         :param str public_key: The PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str response_condition: The name of the condition to apply.
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -6676,15 +6676,15 @@
         """
         return pulumi.get(self, "response_condition")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingGc(dict):
     @staticmethod
@@ -6750,15 +6750,15 @@
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param str placement: Where in the generated VCL the logging call should be placed.
         :param str project_id: The ID of your Google Cloud Platform project
         :param str response_condition: Name of a condition to apply this logging.
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param str user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
@@ -6900,15 +6900,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
@@ -8578,15 +8578,15 @@
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str placement: Where in the generated VCL the logging call should be placed. Can be `none` or `waf_debug`.
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str response_condition: The name of an existing condition in the configured endpoint, or leave blank to always execute.
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "access_key", access_key)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "url", url)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -8732,15 +8732,15 @@
         """
         return pulumi.get(self, "response_condition")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingPapertrail(dict):
     @staticmethod
@@ -8934,15 +8934,15 @@
         :param str redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param str response_condition: Name of blockAttributes condition to apply this logging.
         :param str s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
         :param str s3_iam_role: The Amazon Resource Name (ARN) for the IAM role granting Fastly access to S3. Not required if `access_key` and `secret_key` are provided. You can provide this value via an environment variable, `FASTLY_S3_IAM_ROLE`
         :param str s3_secret_key: AWS Secret Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This secret will be not be encrypted. Not required if `iam_role` is provided. You can provide this secret via an environment variable, `FASTLY_S3_SECRET_KEY`
         :param str server_side_encryption: Specify what type of server side encryption should be used. Can be either `AES256` or `aws:kms`
         :param str server_side_encryption_kms_key_id: Optional server-side KMS Key Id. Must be set if server*side*encryption is set to `aws:kms`
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
@@ -9151,15 +9151,15 @@
         """
         return pulumi.get(self, "server_side_encryption_kms_key_id")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingScalyr(dict):
     @staticmethod
@@ -9350,15 +9350,15 @@
         :param str password: The password for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
         :param int period: How frequently log files are finalized so they can be available for reading (in seconds, default `3600`)
         :param str placement: Where in the generated VCL the logging call should be placed.
         :param int port: The port the SFTP service listens on. (Default: `22`)
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str response_condition: The name of the condition to apply.
         :param str secret_key: The SSH private key for the server. If both `password` and `secret_key` are passed, `secret_key` will be preferred
-        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "ssh_known_hosts", ssh_known_hosts)
         pulumi.set(__self__, "user", user)
         if compression_codec is not None:
@@ -9524,15 +9524,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter(name="timestampFormat")
     def timestamp_format(self) -> Optional[str]:
         """
-        The `strftime` specified timestamp formatting (default `%!Y(MISSING)-%!m(MISSING)-%!d(MISSING)T%!H(MISSING):%!M(MISSING):%!S(MISSING).000`)
+        The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         """
         return pulumi.get(self, "timestamp_format")
 
 
 @pulumi.output_type
 class ServiceVclLoggingSplunk(dict):
     @staticmethod
@@ -9577,15 +9577,15 @@
                  tls_client_key: Optional[str] = None,
                  tls_hostname: Optional[str] = None,
                  use_tls: Optional[bool] = None):
         """
         :param str name: A unique name to identify the Splunk endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str token: The Splunk token to be used for authentication
         :param str url: The Splunk URL to stream logs to
-        :param str format: Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        :param str format: Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (default: 2)
         :param str placement: Where in the generated VCL the logging call should be placed
         :param str response_condition: The name of the condition to apply
         :param str tls_ca_cert: A secure certificate to authenticate the server with. Must be in PEM format. You can provide this certificate via an environment variable, `FASTLY_SPLUNK_CA_CERT`
         :param str tls_client_cert: The client certificate used to make authenticated requests. Must be in PEM format.
         :param str tls_client_key: The client private key used to make authenticated requests. Must be in PEM format.
         :param str tls_hostname: The hostname used to verify the server's certificate. It can either be the Common Name or a Subject Alternative Name (SAN)
@@ -9637,15 +9637,15 @@
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
-        Apache-style string or VCL variables to use for log formatting (default: `%!h(MISSING) %!l(MISSING) %!u(MISSING) %!t(MISSING) "%!r(MISSING)" %!>(MISSING)s %!b(MISSING)`)
+        Apache-style string or VCL variables to use for log formatting (default: `%h %l %u %t "%r" %>s %b`)
         """
         return pulumi.get(self, "format")
 
     @property
     @pulumi.getter(name="formatVersion")
     def format_version(self) -> Optional[int]:
         """
```

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/provider.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/secretstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly/user.py` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1711735248
+Version: 8.6.0a1712399555
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1711735248/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.6.0a1712399555/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1711735248/pyproject.toml` & `pulumi_fastly-8.6.0a1712399555/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.6.0a1711735248"
+  version = "8.6.0a1712399555"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

