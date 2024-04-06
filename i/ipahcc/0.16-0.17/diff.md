# Comparing `tmp/ipahcc-0.16.tar.gz` & `tmp/ipahcc-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipahcc-0.16.tar", last modified: Wed Apr  3 09:52:28 2024, max compression
+gzip compressed data, was "ipahcc-0.17.tar", last modified: Sat Apr  6 08:00:34 2024, max compression
```

## Comparing `ipahcc-0.16.tar` & `ipahcc-0.17.tar`

### file list

```diff
@@ -1,243 +1,246 @@
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.028221 ipahcc-0.16/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      342 2023-03-23 11:43:35.000000 ipahcc-0.16/.eslintrc.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      143 2023-06-29 14:35:25.000000 ipahcc-0.16/.yamllint.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4256 2024-03-26 15:14:27.000000 ipahcc-0.16/CONTRIBUTING.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)      212 2023-03-23 11:43:35.000000 ipahcc-0.16/CONTRIBUTORS.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)    35147 2023-03-23 11:43:35.000000 ipahcc-0.16/COPYING
--rw-r--r--   0 heimes    (1000) heimes    (1000)    12150 2024-03-26 15:14:27.000000 ipahcc-0.16/DEVELOPMENT.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)      412 2024-04-03 09:52:02.000000 ipahcc-0.16/MANIFEST.in
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10973 2024-04-03 09:52:02.000000 ipahcc-0.16/Makefile
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10575 2024-04-03 09:52:28.028221 ipahcc-0.16/PKG-INFO
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10079 2024-03-26 15:14:27.000000 ipahcc-0.16/README.md
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.973220 ipahcc-0.16/install/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.972220 ipahcc-0.16/install/client/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.987220 ipahcc-0.16/install/client/sysconfig/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      196 2024-03-27 14:17:19.000000 ipahcc-0.16/install/client/sysconfig/ipa-hcc-auto-enrollment
--rw-r--r--   0 heimes    (1000) heimes    (1000)       26 2023-12-01 09:54:54.000000 ipahcc-0.16/install/client/sysconfig/ipa-hcc-client-prepare
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.988220 ipahcc-0.16/install/client/systemd/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      594 2023-03-28 13:06:30.000000 ipahcc-0.16/install/client/systemd/ipa-hcc-auto-enrollment.service
--rw-r--r--   0 heimes    (1000) heimes    (1000)      643 2023-12-01 09:54:54.000000 ipahcc-0.16/install/client/systemd/ipa-hcc-client-prepare.service
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.973220 ipahcc-0.16/install/mockapi/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.988220 ipahcc-0.16/install/mockapi/httpd/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1074 2023-10-10 06:15:50.000000 ipahcc-0.16/install/mockapi/httpd/ipa-hcc-mockapi.conf
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.988220 ipahcc-0.16/install/mockapi/updates/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      198 2023-12-01 09:54:54.000000 ipahcc-0.16/install/mockapi/updates/87-hcc-mockapi.update
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.988220 ipahcc-0.16/install/mockapi/wsgi/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      161 2024-04-03 09:52:02.000000 ipahcc-0.16/install/mockapi/wsgi/hcc_mockapi.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.973220 ipahcc-0.16/install/registration/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.989220 ipahcc-0.16/install/registration/gssproxy/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      245 2023-10-10 06:15:50.000000 ipahcc-0.16/install/registration/gssproxy/85-ipa-hcc.conf
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.989220 ipahcc-0.16/install/registration/httpd/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      898 2023-04-20 14:11:03.000000 ipahcc-0.16/install/registration/httpd/ipa-hcc.conf
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.989220 ipahcc-0.16/install/registration/updates/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      252 2023-03-23 11:43:36.000000 ipahcc-0.16/install/registration/updates/86-hcc-registration-service.update
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.989220 ipahcc-0.16/install/registration/wsgi/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      166 2024-04-03 09:52:02.000000 ipahcc-0.16/install/registration/wsgi/hcc_registration_service.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.990220 ipahcc-0.16/install/server/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.991220 ipahcc-0.16/install/server/cacerts/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2472 2023-04-11 08:37:20.000000 ipahcc-0.16/install/server/cacerts/00-candlepin-redhat-ca-sha256.pem
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2679 2023-04-11 08:37:20.000000 ipahcc-0.16/install/server/cacerts/01-redhat-entitlement-authority-2022.pem
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2622 2023-04-11 08:37:20.000000 ipahcc-0.16/install/server/cacerts/02-redhat-entitlement-master-ca.pem
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2679 2023-04-11 08:37:20.000000 ipahcc-0.16/install/server/cacerts/3bba0b9d.0
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2472 2023-04-11 08:37:20.000000 ipahcc-0.16/install/server/cacerts/49f9274f.0
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2622 2023-04-11 08:37:20.000000 ipahcc-0.16/install/server/cacerts/fa9a18d6.0
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.991220 ipahcc-0.16/install/server/ipa/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      374 2024-04-03 09:52:02.000000 ipahcc-0.16/install/server/ipa/hcc.conf
--rw-r--r--   0 heimes    (1000) heimes    (1000)       66 2024-04-03 09:52:02.000000 ipahcc-0.16/install/server/ipa-hcc
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.991220 ipahcc-0.16/install/server/man/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1956 2023-10-10 06:15:50.000000 ipahcc-0.16/install/server/man/ipa-hcc.1
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.992220 ipahcc-0.16/install/server/schema.d/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2530 2023-10-10 06:15:50.000000 ipahcc-0.16/install/server/schema.d/85-hcc.ldif
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.992220 ipahcc-0.16/install/server/systemd/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      336 2023-03-23 14:16:28.000000 ipahcc-0.16/install/server/systemd/ipa-hcc-update.service
--rw-r--r--   0 heimes    (1000) heimes    (1000)      164 2023-03-23 11:43:36.000000 ipahcc-0.16/install/server/systemd/ipa-hcc-update.timer
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.974220 ipahcc-0.16/install/server/ui/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.974220 ipahcc-0.16/install/server/ui/js/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.975220 ipahcc-0.16/install/server/ui/js/plugins/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.992220 ipahcc-0.16/install/server/ui/js/plugins/hccconfig/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1830 2023-03-23 14:16:28.000000 ipahcc-0.16/install/server/ui/js/plugins/hccconfig/hccconfig.js
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.993220 ipahcc-0.16/install/server/ui/js/plugins/hcchost/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3168 2023-08-30 09:10:36.000000 ipahcc-0.16/install/server/ui/js/plugins/hcchost/hcchost.js
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.994220 ipahcc-0.16/install/server/ui/js/plugins/hccidp/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1286 2023-10-10 08:14:41.000000 ipahcc-0.16/install/server/ui/js/plugins/hccidp/hccidp.js
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.994220 ipahcc-0.16/install/server/uninstall/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      369 2023-08-30 09:10:36.000000 ipahcc-0.16/install/server/uninstall/85-hcc-uninstall-server.update
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.994220 ipahcc-0.16/install/server/updates/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5522 2023-10-10 06:15:50.000000 ipahcc-0.16/install/server/updates/85-hcc.update
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)      717 2023-12-01 09:54:54.000000 ipahcc-0.16/install_client.sh
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)     1578 2023-12-01 09:54:54.000000 ipahcc-0.16/install_server.sh
--rw-r--r--   0 heimes    (1000) heimes    (1000)      354 2024-04-03 09:52:02.000000 ipahcc-0.16/ipa-hcc.rpmlintrc
--rw-r--r--   0 heimes    (1000) heimes    (1000)    14182 2024-04-03 09:52:02.000000 ipahcc-0.16/ipa-hcc.spec.rpkg
--rw-r--r--   0 heimes    (1000) heimes    (1000)      919 2024-01-31 11:19:57.000000 ipahcc-0.16/pylintrc
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2997 2024-04-03 09:52:02.000000 ipahcc-0.16/pyproject.toml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      571 2024-03-26 15:14:27.000000 ipahcc-0.16/requirements.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)      905 2024-04-03 09:52:28.029221 ipahcc-0.16/setup.cfg
--rw-r--r--   0 heimes    (1000) heimes    (1000)       38 2023-06-29 14:35:26.000000 ipahcc-0.16/setup.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.995220 ipahcc-0.16/src/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.996220 ipahcc-0.16/src/ipahcc/
--rw-r--r--   0 heimes    (1000) heimes    (1000)       55 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4554 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/hccplatform.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.997220 ipahcc-0.16/src/ipahcc/mockapi/
--rw-r--r--   0 heimes    (1000) heimes    (1000)       52 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/mockapi/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2473 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/mockapi/domain_token.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    13353 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/mockapi/wsgi.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-08-30 09:10:36.000000 ipahcc-0.16/src/ipahcc/py.typed
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.997220 ipahcc-0.16/src/ipahcc/registration/
--rw-r--r--   0 heimes    (1000) heimes    (1000)       65 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/registration/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3584 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/registration/wsgi.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.999220 ipahcc-0.16/src/ipahcc/server/
--rw-r--r--   0 heimes    (1000) heimes    (1000)       67 2023-08-30 09:10:36.000000 ipahcc-0.16/src/ipahcc/server/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7680 2024-01-31 11:19:57.000000 ipahcc-0.16/src/ipahcc/server/cli.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    13407 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/server/framework.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    27300 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/server/hccapi.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.003220 ipahcc-0.16/src/ipahcc/server/schema/
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10473 2023-12-01 10:11:00.000000 ipahcc-0.16/src/ipahcc/server/schema/defs.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      356 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/domain_reg_token_request.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      706 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/domain_reg_token_response.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      567 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/errors.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      481 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/host_conf_request.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      943 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/host_conf_response.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      582 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/host_register_request.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      406 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/host_register_response.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      277 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/ipadomain_get_request.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      208 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/ipadomain_register_request.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      262 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/ipadomain_register_response.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      503 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/ipadomain_update_request.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      270 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/ipadomain_update_response.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      722 2023-11-29 06:37:30.000000 ipahcc-0.16/src/ipahcc/server/schema/signing_keys_response.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3344 2023-10-10 06:15:50.000000 ipahcc-0.16/src/ipahcc/server/schema.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4272 2024-01-31 11:19:57.000000 ipahcc-0.16/src/ipahcc/server/util.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.004220 ipahcc-0.16/src/ipahcc/sign/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      691 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/sign/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      271 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/sign/__main__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     6761 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/sign/_jwk.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     9601 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc/sign/_jwst.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.028221 ipahcc-0.16/src/ipahcc.egg-info/
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10575 2024-04-03 09:52:27.000000 ipahcc-0.16/src/ipahcc.egg-info/PKG-INFO
--rw-r--r--   0 heimes    (1000) heimes    (1000)     6042 2024-04-03 09:52:27.000000 ipahcc-0.16/src/ipahcc.egg-info/SOURCES.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)        1 2024-04-03 09:52:27.000000 ipahcc-0.16/src/ipahcc.egg-info/dependency_links.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)       94 2024-04-03 09:52:27.000000 ipahcc-0.16/src/ipahcc.egg-info/requires.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)       83 2024-04-03 09:52:27.000000 ipahcc-0.16/src/ipahcc.egg-info/top_level.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)    32823 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc_auto_enrollment.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5446 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc_client_prepare.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5999 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipahcc_stage_console.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.976220 ipahcc-0.16/src/ipaserver/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:27.976220 ipahcc-0.16/src/ipaserver/install/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.004220 ipahcc-0.16/src/ipaserver/install/plugins/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4398 2023-08-30 09:10:36.000000 ipahcc-0.16/src/ipaserver/install/plugins/update_hcc.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4955 2023-09-02 08:07:09.000000 ipahcc-0.16/src/ipaserver/install/plugins/update_hcc_enrollment_service.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1871 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipaserver/install/plugins/update_hcc_mockapi.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.005220 ipahcc-0.16/src/ipaserver/plugins/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5297 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipaserver/plugins/hccconfig.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4399 2023-08-30 09:10:36.000000 ipahcc-0.16/src/ipaserver/plugins/hcchost.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3215 2023-12-01 09:54:54.000000 ipahcc-0.16/src/ipaserver/plugins/hccidp.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    11491 2024-04-03 09:52:02.000000 ipahcc-0.16/src/ipaserver/plugins/hccjwk.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4926 2023-08-30 09:10:36.000000 ipahcc-0.16/src/ipaserver/plugins/hccserverroles.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.005220 ipahcc-0.16/stubs/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      238 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/README.md
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.006220 ipahcc-0.16/stubs/ipaclient/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-10-10 06:15:50.000000 ipahcc-0.16/stubs/ipaclient/__init__.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.006220 ipahcc-0.16/stubs/ipaclient/remote_plugins/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      506 2023-10-10 06:15:50.000000 ipahcc-0.16/stubs/ipaclient/remote_plugins/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      526 2023-10-10 06:15:50.000000 ipahcc-0.16/stubs/ipaclient/remote_plugins/schema.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.009220 ipahcc-0.16/stubs/ipalib/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1268 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1013 2023-06-06 08:01:03.000000 ipahcc-0.16/stubs/ipalib/backend.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      862 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/base.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      153 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipalib/capabilities.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      817 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/config.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1334 2023-04-21 07:58:26.000000 ipahcc-0.16/stubs/ipalib/constants.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1175 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/crud.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10321 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipalib/errors.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      102 2023-04-21 07:58:26.000000 ipahcc-0.16/stubs/ipalib/facts.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4917 2023-06-06 08:01:23.000000 ipahcc-0.16/stubs/ipalib/frontend.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.010220 ipahcc-0.16/stubs/ipalib/install/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipalib/install/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1599 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/install/certstore.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)       47 2024-03-26 15:14:27.000000 ipahcc-0.16/stubs/ipalib/install/dnsforwarders.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      758 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipalib/install/kinit.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4050 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/messages.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1219 2023-04-21 07:58:26.000000 ipahcc-0.16/stubs/ipalib/output.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5340 2023-10-10 06:15:50.000000 ipahcc-0.16/stubs/ipalib/parameters.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2846 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/plugable.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      463 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/request.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2017 2023-10-10 08:14:41.000000 ipahcc-0.16/stubs/ipalib/text.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4548 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipalib/util.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3114 2023-12-01 09:54:54.000000 ipahcc-0.16/stubs/ipalib/x509.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.011221 ipahcc-0.16/stubs/ipaplatform/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)       35 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/base.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1721 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/constants.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.012220 ipahcc-0.16/stubs/ipaplatform/fedora/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/fedora/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      510 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaplatform/fedora/services.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)       23 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/osinfo.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)    11300 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/paths.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.012220 ipahcc-0.16/stubs/ipaplatform/redhat/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaplatform/redhat/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1392 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaplatform/redhat/services.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4096 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaplatform/services.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3026 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaplatform/tasks.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.013220 ipahcc-0.16/stubs/ipapython/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipapython/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      217 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipapython/admintool.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1942 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipapython/dn.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2234 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipapython/dnsutil.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     9052 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipapython/ipaldap.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5664 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipapython/ipautil.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1064 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipapython/kerberos.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)       67 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipapython/version.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.014221 ipahcc-0.16/stubs/ipaserver/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaserver/__init__.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.014221 ipahcc-0.16/stubs/ipaserver/install/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaserver/install/__init__.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.015220 ipahcc-0.16/stubs/ipaserver/install/plugins/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaserver/install/plugins/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      311 2023-08-30 09:10:36.000000 ipahcc-0.16/stubs/ipaserver/install/plugins/update_hcc.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      336 2023-08-30 09:10:36.000000 ipahcc-0.16/stubs/ipaserver/install/plugins/update_hcc_enrollment_service.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      674 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/masters.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.017221 ipahcc-0.16/stubs/ipaserver/plugins/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/ipaserver/plugins/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)    11228 2023-10-10 06:15:50.000000 ipahcc-0.16/stubs/ipaserver/plugins/baseldap.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1727 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/plugins/config.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      470 2023-08-30 09:10:36.000000 ipahcc-0.16/stubs/ipaserver/plugins/hccconfig.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      397 2023-08-30 09:10:36.000000 ipahcc-0.16/stubs/ipaserver/plugins/hcchost.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      197 2023-10-10 08:14:41.000000 ipahcc-0.16/stubs/ipaserver/plugins/hccidp.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      532 2023-08-30 09:10:36.000000 ipahcc-0.16/stubs/ipaserver/plugins/hccserverroles.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7149 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/plugins/host.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1466 2023-10-10 08:14:41.000000 ipahcc-0.16/stubs/ipaserver/plugins/idp.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      548 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/plugins/internal.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      973 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/plugins/serverrole.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      859 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/plugins/serverroles.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2285 2023-04-21 06:04:57.000000 ipahcc-0.16/stubs/ipaserver/servroles.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.017221 ipahcc-0.16/stubs/rhsm/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2053 2024-03-27 14:17:19.000000 ipahcc-0.16/stubs/rhsm/config.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.017221 ipahcc-0.16/stubs/systemd/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/systemd/__init__.pyi
--rw-r--r--   0 heimes    (1000) heimes    (1000)      159 2023-04-20 14:31:48.000000 ipahcc-0.16/stubs/systemd/daemon.pyi
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.020221 ipahcc-0.16/tests/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.025221 ipahcc-0.16/tests/clients/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3268 2024-03-13 05:10:52.000000 ipahcc-0.16/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.key
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7874 2024-03-13 05:10:52.000000 ipahcc-0.16/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.pem
--rw-r--r--   0 heimes    (1000) heimes    (1000)      293 2024-03-13 05:10:52.000000 ipahcc-0.16/tests/clients/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     9699 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/conftest.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.026221 ipahcc-0.16/tests/data/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-03 09:52:28.027221 ipahcc-0.16/tests/data/autoenrollment/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2277 2023-03-23 11:43:36.000000 ipahcc-0.16/tests/data/autoenrollment/cert.pem
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1136 2024-02-22 10:13:55.000000 ipahcc-0.16/tests/data/autoenrollment/host-details.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1639 2023-03-27 07:08:50.000000 ipahcc-0.16/tests/data/autoenrollment/ipa_ca.crt
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3272 2023-03-23 11:43:36.000000 ipahcc-0.16/tests/data/autoenrollment/key.pem
--rw-r--r--   0 heimes    (1000) heimes    (1000)       36 2023-04-03 06:38:40.000000 ipahcc-0.16/tests/data/autoenrollment/machine-id
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1037 2023-04-11 08:37:20.000000 ipahcc-0.16/tests/data/kdc.conf
--rw-r--r--   0 heimes    (1000) heimes    (1000)    15766 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_autoenrollment.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2854 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_client_prepare.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5274 2023-10-10 06:15:50.000000 ipahcc-0.16/tests/test_framework.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    12648 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_hccapi.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3424 2023-10-19 07:59:23.000000 ipahcc-0.16/tests/test_ipaserver.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4162 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_ipaserver_integration.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     8697 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_mockapi.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3031 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_registration.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4520 2023-10-10 06:15:50.000000 ipahcc-0.16/tests/test_schema.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7455 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/test_sign.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1913 2024-04-03 09:52:02.000000 ipahcc-0.16/tests/tests.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2667 2024-04-03 09:52:02.000000 ipahcc-0.16/tox.ini
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.127162 ipahcc-0.17/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      342 2023-03-23 11:43:35.000000 ipahcc-0.17/.eslintrc.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      143 2023-06-29 14:35:25.000000 ipahcc-0.17/.yamllint.yaml
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4256 2024-03-26 15:14:27.000000 ipahcc-0.17/CONTRIBUTING.md
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      212 2023-03-23 11:43:35.000000 ipahcc-0.17/CONTRIBUTORS.txt
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    35147 2023-03-23 11:43:35.000000 ipahcc-0.17/COPYING
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    12165 2024-04-03 13:14:45.000000 ipahcc-0.17/DEVELOPMENT.md
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      443 2024-04-03 10:13:25.000000 ipahcc-0.17/MANIFEST.in
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     9740 2024-04-06 07:45:40.000000 ipahcc-0.17/Makefile
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    10696 2024-04-06 08:00:34.127162 ipahcc-0.17/PKG-INFO
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    10079 2024-03-26 15:14:27.000000 ipahcc-0.17/README.md
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.041160 ipahcc-0.17/install/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.040160 ipahcc-0.17/install/client/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.057160 ipahcc-0.17/install/client/sysconfig/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      196 2024-03-27 14:17:19.000000 ipahcc-0.17/install/client/sysconfig/ipa-hcc-auto-enrollment
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       26 2023-12-01 09:54:54.000000 ipahcc-0.17/install/client/sysconfig/ipa-hcc-client-prepare
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.058160 ipahcc-0.17/install/client/systemd/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      594 2023-03-28 13:06:30.000000 ipahcc-0.17/install/client/systemd/ipa-hcc-auto-enrollment.service
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      643 2023-12-01 09:54:54.000000 ipahcc-0.17/install/client/systemd/ipa-hcc-client-prepare.service
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.040160 ipahcc-0.17/install/mockapi/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.059161 ipahcc-0.17/install/mockapi/httpd/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1074 2023-10-10 06:15:50.000000 ipahcc-0.17/install/mockapi/httpd/ipa-hcc-mockapi.conf
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.060160 ipahcc-0.17/install/mockapi/updates/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      198 2023-12-01 09:54:54.000000 ipahcc-0.17/install/mockapi/updates/87-hcc-mockapi.update
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.060160 ipahcc-0.17/install/mockapi/wsgi/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      163 2024-04-03 10:13:25.000000 ipahcc-0.17/install/mockapi/wsgi/hcc_mockapi.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.041160 ipahcc-0.17/install/registration/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.061160 ipahcc-0.17/install/registration/gssproxy/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      245 2023-10-10 06:15:50.000000 ipahcc-0.17/install/registration/gssproxy/85-ipa-hcc.conf
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.061160 ipahcc-0.17/install/registration/httpd/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      898 2023-04-20 14:11:03.000000 ipahcc-0.17/install/registration/httpd/ipa-hcc.conf
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.062161 ipahcc-0.17/install/registration/updates/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      252 2023-03-23 11:43:36.000000 ipahcc-0.17/install/registration/updates/86-hcc-registration-service.update
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.063161 ipahcc-0.17/install/registration/wsgi/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      168 2024-04-03 10:13:25.000000 ipahcc-0.17/install/registration/wsgi/hcc_registration_service.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.042160 ipahcc-0.17/install/server/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.064161 ipahcc-0.17/install/server/cacerts/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2472 2023-04-11 08:37:20.000000 ipahcc-0.17/install/server/cacerts/00-candlepin-redhat-ca-sha256.pem
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2679 2023-04-11 08:37:20.000000 ipahcc-0.17/install/server/cacerts/01-redhat-entitlement-authority-2022.pem
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2622 2023-04-11 08:37:20.000000 ipahcc-0.17/install/server/cacerts/02-redhat-entitlement-master-ca.pem
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2679 2023-04-11 08:37:20.000000 ipahcc-0.17/install/server/cacerts/3bba0b9d.0
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2472 2023-04-11 08:37:20.000000 ipahcc-0.17/install/server/cacerts/49f9274f.0
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2622 2023-04-11 08:37:20.000000 ipahcc-0.17/install/server/cacerts/fa9a18d6.0
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.064161 ipahcc-0.17/install/server/ipa/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      517 2024-04-03 10:13:25.000000 ipahcc-0.17/install/server/ipa/hcc.conf
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.065161 ipahcc-0.17/install/server/man/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1956 2023-10-10 06:15:50.000000 ipahcc-0.17/install/server/man/ipa-hcc.1
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.065161 ipahcc-0.17/install/server/schema.d/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2530 2023-10-10 06:15:50.000000 ipahcc-0.17/install/server/schema.d/85-hcc.ldif
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.066161 ipahcc-0.17/install/server/systemd/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      336 2023-03-23 14:16:28.000000 ipahcc-0.17/install/server/systemd/ipa-hcc-update.service
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      164 2023-03-23 11:43:36.000000 ipahcc-0.17/install/server/systemd/ipa-hcc-update.timer
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.042160 ipahcc-0.17/install/server/ui/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.042160 ipahcc-0.17/install/server/ui/js/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.042160 ipahcc-0.17/install/server/ui/js/plugins/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.066161 ipahcc-0.17/install/server/ui/js/plugins/hccconfig/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1830 2023-03-23 14:16:28.000000 ipahcc-0.17/install/server/ui/js/plugins/hccconfig/hccconfig.js
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.067161 ipahcc-0.17/install/server/ui/js/plugins/hcchost/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3168 2023-08-30 09:10:36.000000 ipahcc-0.17/install/server/ui/js/plugins/hcchost/hcchost.js
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.067161 ipahcc-0.17/install/server/ui/js/plugins/hccidp/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1286 2023-10-10 08:14:41.000000 ipahcc-0.17/install/server/ui/js/plugins/hccidp/hccidp.js
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.067161 ipahcc-0.17/install/server/uninstall/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      369 2023-08-30 09:10:36.000000 ipahcc-0.17/install/server/uninstall/85-hcc-uninstall-server.update
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.068161 ipahcc-0.17/install/server/updates/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     5522 2023-10-10 06:15:50.000000 ipahcc-0.17/install/server/updates/85-hcc.update
+-rwxr-xr-x   0 heimes    (1000) heimes    (1000)      717 2023-12-01 09:54:54.000000 ipahcc-0.17/install_client.sh
+-rwxr-xr-x   0 heimes    (1000) heimes    (1000)     1578 2023-12-01 09:54:54.000000 ipahcc-0.17/install_server.sh
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      523 2024-04-03 11:57:34.000000 ipahcc-0.17/ipa-hcc.rpmlintrc
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    17403 2024-04-06 07:25:58.000000 ipahcc-0.17/ipa-hcc.spec.rpkg
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      919 2024-01-31 11:19:57.000000 ipahcc-0.17/pylintrc
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3271 2024-04-03 13:14:45.000000 ipahcc-0.17/pyproject.toml
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      571 2024-03-26 15:14:27.000000 ipahcc-0.17/requirements.txt
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.069161 ipahcc-0.17/selinux/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      201 2024-04-03 10:13:25.000000 ipahcc-0.17/selinux/ipa-hcc.fc
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      885 2024-04-03 10:13:25.000000 ipahcc-0.17/selinux/ipa-hcc.if
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      619 2024-04-03 10:13:25.000000 ipahcc-0.17/selinux/ipa-hcc.te
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1129 2024-04-06 08:00:34.128162 ipahcc-0.17/setup.cfg
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       38 2023-06-29 14:35:26.000000 ipahcc-0.17/setup.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.043160 ipahcc-0.17/src/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.071161 ipahcc-0.17/src/ipahcc/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      117 2024-04-03 13:14:45.000000 ipahcc-0.17/src/ipahcc/__init__.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       54 2024-04-06 07:45:42.000000 ipahcc-0.17/src/ipahcc/_version.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.073161 ipahcc-0.17/src/ipahcc/client/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       67 2024-04-03 13:14:45.000000 ipahcc-0.17/src/ipahcc/client/__init__.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    29561 2024-04-04 09:07:36.000000 ipahcc-0.17/src/ipahcc/client/auto_enrollment.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     5363 2024-04-03 13:14:45.000000 ipahcc-0.17/src/ipahcc/client/client_prepare.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     6058 2024-04-03 13:14:45.000000 ipahcc-0.17/src/ipahcc/client/stage_console.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     8707 2024-04-03 13:14:45.000000 ipahcc-0.17/src/ipahcc/hccplatform.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-08-30 09:10:36.000000 ipahcc-0.17/src/ipahcc/py.typed
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.076161 ipahcc-0.17/src/ipahcc/server/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       67 2023-08-30 09:10:36.000000 ipahcc-0.17/src/ipahcc/server/__init__.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     7680 2024-01-31 11:19:57.000000 ipahcc-0.17/src/ipahcc/server/cli.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2473 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/domain_token.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    13521 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/framework.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    27425 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/hccapi.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    13358 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/mockapi.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3572 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/registration.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.081161 ipahcc-0.17/src/ipahcc/server/schema/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    10473 2023-12-01 10:11:00.000000 ipahcc-0.17/src/ipahcc/server/schema/defs.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      356 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/domain_reg_token_request.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      706 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/domain_reg_token_response.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      567 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/errors.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      481 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/host_conf_request.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      943 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/host_conf_response.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      582 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/host_register_request.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      406 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/host_register_response.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      277 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/ipadomain_get_request.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      208 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/ipadomain_register_request.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      262 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/ipadomain_register_response.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      503 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/ipadomain_update_request.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      270 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/ipadomain_update_response.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      722 2023-11-29 06:37:30.000000 ipahcc-0.17/src/ipahcc/server/schema/signing_keys_response.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3344 2023-10-10 06:15:50.000000 ipahcc-0.17/src/ipahcc/server/schema.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.082161 ipahcc-0.17/src/ipahcc/server/sign/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      691 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/sign/__init__.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      271 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/sign/__main__.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     6761 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/sign/_jwk.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     9601 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipahcc/server/sign/_jwst.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4272 2024-01-31 11:19:57.000000 ipahcc-0.17/src/ipahcc/server/util.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.127162 ipahcc-0.17/src/ipahcc.egg-info/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    10696 2024-04-06 08:00:34.000000 ipahcc-0.17/src/ipahcc.egg-info/PKG-INFO
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     6151 2024-04-06 08:00:34.000000 ipahcc-0.17/src/ipahcc.egg-info/SOURCES.txt
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        1 2024-04-06 08:00:34.000000 ipahcc-0.17/src/ipahcc.egg-info/dependency_links.txt
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      228 2024-04-06 08:00:34.000000 ipahcc-0.17/src/ipahcc.egg-info/entry_points.txt
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      111 2024-04-06 08:00:34.000000 ipahcc-0.17/src/ipahcc.egg-info/requires.txt
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       17 2024-04-06 08:00:34.000000 ipahcc-0.17/src/ipahcc.egg-info/top_level.txt
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.044160 ipahcc-0.17/src/ipaserver/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.044160 ipahcc-0.17/src/ipaserver/install/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.083161 ipahcc-0.17/src/ipaserver/install/plugins/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4398 2023-08-30 09:10:36.000000 ipahcc-0.17/src/ipaserver/install/plugins/update_hcc.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4955 2023-09-02 08:07:09.000000 ipahcc-0.17/src/ipaserver/install/plugins/update_hcc_enrollment_service.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1896 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipaserver/install/plugins/update_hcc_mockapi.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.086161 ipahcc-0.17/src/ipaserver/plugins/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     5305 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipaserver/plugins/hccconfig.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4399 2023-08-30 09:10:36.000000 ipahcc-0.17/src/ipaserver/plugins/hcchost.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3215 2023-12-01 09:54:54.000000 ipahcc-0.17/src/ipaserver/plugins/hccidp.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    11516 2024-04-03 10:13:25.000000 ipahcc-0.17/src/ipaserver/plugins/hccjwk.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4926 2023-08-30 09:10:36.000000 ipahcc-0.17/src/ipaserver/plugins/hccserverroles.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.087161 ipahcc-0.17/stubs/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      238 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/README.md
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.087161 ipahcc-0.17/stubs/ipaclient/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-10-10 06:15:50.000000 ipahcc-0.17/stubs/ipaclient/__init__.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.087161 ipahcc-0.17/stubs/ipaclient/remote_plugins/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      506 2023-10-10 06:15:50.000000 ipahcc-0.17/stubs/ipaclient/remote_plugins/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      526 2023-10-10 06:15:50.000000 ipahcc-0.17/stubs/ipaclient/remote_plugins/schema.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.094161 ipahcc-0.17/stubs/ipalib/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1268 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1013 2023-06-06 08:01:03.000000 ipahcc-0.17/stubs/ipalib/backend.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      862 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/base.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      153 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipalib/capabilities.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      817 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/config.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1334 2023-04-21 07:58:26.000000 ipahcc-0.17/stubs/ipalib/constants.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1175 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/crud.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    10321 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipalib/errors.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      102 2023-04-21 07:58:26.000000 ipahcc-0.17/stubs/ipalib/facts.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4917 2023-06-06 08:01:23.000000 ipahcc-0.17/stubs/ipalib/frontend.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.095161 ipahcc-0.17/stubs/ipalib/install/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipalib/install/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1599 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/install/certstore.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       47 2024-03-26 15:14:27.000000 ipahcc-0.17/stubs/ipalib/install/dnsforwarders.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      758 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipalib/install/kinit.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4050 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/messages.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1219 2023-04-21 07:58:26.000000 ipahcc-0.17/stubs/ipalib/output.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     5340 2023-10-10 06:15:50.000000 ipahcc-0.17/stubs/ipalib/parameters.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2846 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/plugable.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      463 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/request.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2017 2023-10-10 08:14:41.000000 ipahcc-0.17/stubs/ipalib/text.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4548 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipalib/util.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3114 2023-12-01 09:54:54.000000 ipahcc-0.17/stubs/ipalib/x509.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.097161 ipahcc-0.17/stubs/ipaplatform/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       35 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/base.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1721 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/constants.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.097161 ipahcc-0.17/stubs/ipaplatform/fedora/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/fedora/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      510 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaplatform/fedora/services.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       23 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/osinfo.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    11300 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/paths.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.098161 ipahcc-0.17/stubs/ipaplatform/redhat/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaplatform/redhat/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1392 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaplatform/redhat/services.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4096 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaplatform/services.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3026 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaplatform/tasks.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.100161 ipahcc-0.17/stubs/ipapython/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipapython/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      217 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipapython/admintool.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1942 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipapython/dn.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2234 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipapython/dnsutil.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     9052 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipapython/ipaldap.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     5664 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipapython/ipautil.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1064 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipapython/kerberos.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       67 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipapython/version.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.103161 ipahcc-0.17/stubs/ipaserver/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaserver/__init__.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.103161 ipahcc-0.17/stubs/ipaserver/install/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaserver/install/__init__.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.104161 ipahcc-0.17/stubs/ipaserver/install/plugins/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaserver/install/plugins/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      311 2023-08-30 09:10:36.000000 ipahcc-0.17/stubs/ipaserver/install/plugins/update_hcc.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      336 2023-08-30 09:10:36.000000 ipahcc-0.17/stubs/ipaserver/install/plugins/update_hcc_enrollment_service.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      674 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/masters.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.108161 ipahcc-0.17/stubs/ipaserver/plugins/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/ipaserver/plugins/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    11228 2023-10-10 06:15:50.000000 ipahcc-0.17/stubs/ipaserver/plugins/baseldap.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1727 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/plugins/config.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      470 2023-08-30 09:10:36.000000 ipahcc-0.17/stubs/ipaserver/plugins/hccconfig.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      397 2023-08-30 09:10:36.000000 ipahcc-0.17/stubs/ipaserver/plugins/hcchost.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      197 2023-10-10 08:14:41.000000 ipahcc-0.17/stubs/ipaserver/plugins/hccidp.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      532 2023-08-30 09:10:36.000000 ipahcc-0.17/stubs/ipaserver/plugins/hccserverroles.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     7149 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/plugins/host.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1466 2023-10-10 08:14:41.000000 ipahcc-0.17/stubs/ipaserver/plugins/idp.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      548 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/plugins/internal.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      973 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/plugins/serverrole.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      859 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/plugins/serverroles.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2285 2023-04-21 06:04:57.000000 ipahcc-0.17/stubs/ipaserver/servroles.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.109161 ipahcc-0.17/stubs/rhsm/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2053 2024-03-27 14:17:19.000000 ipahcc-0.17/stubs/rhsm/config.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.109161 ipahcc-0.17/stubs/systemd/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/systemd/__init__.pyi
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      159 2023-04-20 14:31:48.000000 ipahcc-0.17/stubs/systemd/daemon.pyi
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.116161 ipahcc-0.17/tests/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.123161 ipahcc-0.17/tests/clients/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3268 2024-03-13 05:10:52.000000 ipahcc-0.17/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.key
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     7874 2024-03-13 05:10:52.000000 ipahcc-0.17/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.pem
+-rw-r--r--   0 heimes    (1000) heimes    (1000)      293 2024-03-13 05:10:52.000000 ipahcc-0.17/tests/clients/README.md
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    10165 2024-04-03 13:14:45.000000 ipahcc-0.17/tests/conftest.py
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.123161 ipahcc-0.17/tests/data/
+drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-04-06 08:00:34.126162 ipahcc-0.17/tests/data/autoenrollment/
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2277 2023-03-23 11:43:36.000000 ipahcc-0.17/tests/data/autoenrollment/cert.pem
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1136 2024-02-22 10:13:55.000000 ipahcc-0.17/tests/data/autoenrollment/host-details.json
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1639 2023-03-27 07:08:50.000000 ipahcc-0.17/tests/data/autoenrollment/ipa_ca.crt
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3272 2023-03-23 11:43:36.000000 ipahcc-0.17/tests/data/autoenrollment/key.pem
+-rw-r--r--   0 heimes    (1000) heimes    (1000)       36 2023-04-03 06:38:40.000000 ipahcc-0.17/tests/data/autoenrollment/machine-id
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     1037 2023-04-11 08:37:20.000000 ipahcc-0.17/tests/data/kdc.conf
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    14376 2024-04-03 13:14:45.000000 ipahcc-0.17/tests/test_autoenrollment.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2479 2024-04-03 13:14:45.000000 ipahcc-0.17/tests/test_client_prepare.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     5274 2023-10-10 06:15:50.000000 ipahcc-0.17/tests/test_framework.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)    12622 2024-04-03 10:13:25.000000 ipahcc-0.17/tests/test_hccapi.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3424 2023-10-19 07:59:23.000000 ipahcc-0.17/tests/test_ipaserver.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4187 2024-04-03 10:13:25.000000 ipahcc-0.17/tests/test_ipaserver_integration.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     8710 2024-04-03 10:13:25.000000 ipahcc-0.17/tests/test_mockapi.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     3041 2024-04-03 10:13:25.000000 ipahcc-0.17/tests/test_registration.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     4520 2023-10-10 06:15:50.000000 ipahcc-0.17/tests/test_schema.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     7462 2024-04-03 10:13:25.000000 ipahcc-0.17/tests/test_sign.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2115 2024-04-03 13:14:45.000000 ipahcc-0.17/tests/tests.py
+-rw-r--r--   0 heimes    (1000) heimes    (1000)     2634 2024-04-03 13:14:45.000000 ipahcc-0.17/tox.ini
```

### Comparing `ipahcc-0.16/CONTRIBUTING.md` & `ipahcc-0.17/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/COPYING` & `ipahcc-0.17/COPYING`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/DEVELOPMENT.md` & `ipahcc-0.17/DEVELOPMENT.md`

 * *Files 2% similar despite different names*

```diff
@@ -325,16 +325,16 @@
   `RHSM certificate subject` with same values as the RHSM cert. The
   subject string does not contain spaces.
 
 
 ## Release process
 
 1. Bump `VERSION` in `Makefile`, e.g. `VERSION = 0.99`
-2. Run `make version` to update `VERSION` in other files. It should modify
-   `pyproject.toml`, `setup.cfg`, and four `.py` files.
+2. Run `make version` to update `VERSION` in other files. It modifies
+   `src/ipahcc/_version.py`. The file is used by code and Python packaging.
 3. Commit the changes, e.g. `git commit --signoff -m "Release 0.99"`
 4. Push the changes and merge them into `main`
 5. Pull the release commit into your local checkout.
    > **IMPORTANT:** Your clone must be on `main` branch and the tip of your
        local `main` branch must be the release commit. Otherwise `rpkg` may
        not work as expected.
 6. Create a release tag with `rpkg tag --version 0.99`. Adjust the text
```

### Comparing `ipahcc-0.16/PKG-INFO` & `ipahcc-0.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ipahcc
-Version: 0.16
+Version: 0.17
 Summary: IPA enrollment agent for Red Hat Hybrid Cloud Console
 Author: Christian Heimes
 Author-email: Christian Heimes <cheimes@redhat.com>
 License: GPL-3.0-or-later
 Platform: any
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: requests
-Requires-Dist: cryptography
-Requires-Dist: ipaclient
-Requires-Dist: jsonschema
-Requires-Dist: jwcrypto
+Requires-Dist: ipalib
 Requires-Dist: netaddr<1.0.0; python_version == "3.6"
+Provides-Extra: server
+Requires-Dist: cryptography; extra == "server"
+Requires-Dist: ipaclient; extra == "server"
+Requires-Dist: jsonschema; extra == "server"
+Requires-Dist: jwcrypto; extra == "server"
 
 # IPA plugin for Hybrid Cloud Console
 
 The *ipa-hcc* plugin provides schema extension of IPA for
 Hybrid Cloud Console integration. The plugin must be installed on all FreeIPA
 servers, preferable before the server/replica is installed.
```

### Comparing `ipahcc-0.16/README.md` & `ipahcc-0.17/README.md`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/client/systemd/ipa-hcc-auto-enrollment.service` & `ipahcc-0.17/install/client/systemd/ipa-hcc-auto-enrollment.service`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/client/systemd/ipa-hcc-client-prepare.service` & `ipahcc-0.17/install/client/systemd/ipa-hcc-client-prepare.service`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/mockapi/httpd/ipa-hcc-mockapi.conf` & `ipahcc-0.17/install/mockapi/httpd/ipa-hcc-mockapi.conf`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/registration/httpd/ipa-hcc.conf` & `ipahcc-0.17/install/registration/httpd/ipa-hcc.conf`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/cacerts/00-candlepin-redhat-ca-sha256.pem` & `ipahcc-0.17/install/server/cacerts/00-candlepin-redhat-ca-sha256.pem`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/cacerts/01-redhat-entitlement-authority-2022.pem` & `ipahcc-0.17/install/server/cacerts/01-redhat-entitlement-authority-2022.pem`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/cacerts/02-redhat-entitlement-master-ca.pem` & `ipahcc-0.17/install/server/cacerts/02-redhat-entitlement-master-ca.pem`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/cacerts/3bba0b9d.0` & `ipahcc-0.17/install/server/cacerts/3bba0b9d.0`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/cacerts/49f9274f.0` & `ipahcc-0.17/install/server/cacerts/49f9274f.0`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/cacerts/fa9a18d6.0` & `ipahcc-0.17/install/server/cacerts/fa9a18d6.0`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/man/ipa-hcc.1` & `ipahcc-0.17/install/server/man/ipa-hcc.1`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/schema.d/85-hcc.ldif` & `ipahcc-0.17/install/server/schema.d/85-hcc.ldif`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/ui/js/plugins/hccconfig/hccconfig.js` & `ipahcc-0.17/install/server/ui/js/plugins/hccconfig/hccconfig.js`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/ui/js/plugins/hcchost/hcchost.js` & `ipahcc-0.17/install/server/ui/js/plugins/hcchost/hcchost.js`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/ui/js/plugins/hccidp/hccidp.js` & `ipahcc-0.17/install/server/ui/js/plugins/hccidp/hccidp.js`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install/server/updates/85-hcc.update` & `ipahcc-0.17/install/server/updates/85-hcc.update`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install_client.sh` & `ipahcc-0.17/install_client.sh`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/install_server.sh` & `ipahcc-0.17/install_server.sh`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/ipa-hcc.spec.rpkg` & `ipahcc-0.17/ipa-hcc.spec.rpkg`

 * *Files 13% similar despite different names*

```diff
@@ -7,29 +7,32 @@
   # ipa-client-install supports PKINIT options since 4.9.11 (RHEL 8.8)
   # and 4.10.1 (RHEL 9.2).
   %if 0%{?rhel} >= 9
     # RHEL 9.2+ with PKINIT support in ipa-client-install
     %global ipa_version 4.10.1
     %global include_client 1
     %global with_pyproject_macros 1
+    %global selinux_policy_version 38.1.1-1
   %else
     # RHEL 8.8+ with PKINIT support in ipa-client-install
     # NOTE: python3 macro points to platform-python
     %global ipa_version 4.9.11
     %global include_client 1
     # RHEL 8's build root does not provide pyproject-rpm-macros
     %global without_pyproject_macros 1
+    %global selinux_policy_version 3.14.3-107
   %endif
 %else
   # Fedora 37+ with PKINIT support in ipa-client-install
   %global ipa_name freeipa
   %global ipa_version 4.10.1
   # Fedora is missing rhc and insights-client
   %global include_client 0
   %global with_pyproject_macros 1
+  %global selinux_policy_version 36.16-1
 %endif
 
 # always include ipa-hcc-server package
 %global with_server 1
 
 # --with client (enabled on RHEL, disabled on Fedora)
 # include ipa-hcc-client package
@@ -48,18 +51,26 @@
   %{error:--with mockapi requires --with server}
 %endif
 
 # --with stageconsole (disabled by default)
 # setup system for internal stage console
 %bcond_with stageconsole
 
+# --without selinux (enabled by default)
+# SELinux rules for ipa-hcc-server
+%bcond_without selinux
+
 # --with devel (disabled by default)
 # local development depedencies
 %bcond_with devel
 
+%if %{with selinux}
+    %global selinuxtype targeted
+    %global modulename ipa-hcc
+%endif
 
 Name:           %{package_name}
 Version:        {{{ git_dir_version }}}
 Release:        1%{?dist}
 Summary:        Hybrid Cloud Console extension for IPA
 
 BuildArch:      noarch
@@ -70,28 +81,31 @@
 # tag names are generated by rpkg
 Source:         {{{ git_dir_pack }}}
 
 BuildRequires: python3-devel
 %if %{with pyproject_macros}
 BuildRequires: pyproject-rpm-macros
 %endif
-%if %{with server}
+# RHEL 8 buildroot does not have idm:DL1 module
+%if %{with server} && 0%{?rhel} != 8
 BuildRequires: python3-ipaserver >= %{ipa_version}
 %else
 BuildRequires: python3-ipaclient >= %{ipa_version}
 %endif
 BuildRequires: python3-requests
 BuildRequires: python3-systemd
 BuildRequires: python3-sssdconfig
 BuildRequires: python3-jsonschema
 BuildRequires: python3-jwcrypto
 BuildRequires: make
 BuildRequires: openssl
 BuildRequires: systemd-devel
-BuildRequires: selinux-policy-devel
+%if %{with selinux}
+BuildRequires: selinux-policy-devel >= %{selinux_policy_version}
+%endif
 BuildRequires: subscription-manager-rhsm-certificates
 %if %{with devel}
 BuildRequires: ipa-client
 BuildRequires: tox
 BuildRequires: python3.6
 BuildRequires: python3.9
 BuildRequires: rpmlint
@@ -106,32 +120,56 @@
 BuildRequires: rpmdeplint
 BuildRequires: rpmlint
 %endif
 
 %description
 An extension for IPA integration with Red Hat Hybrid Cloud Console.
 
+
+%package -n python3-ipahcc
+Summary: Python libraries for ipa-hcc, IPA Hybrid Cloud Console integration
+BuildArch: noarch
+%{?python_provide:%python_provide python3-ipahcc}
+Requires: python3-ipalib >= %{ipa_version}
+Requires: python3-requests
+Recommends: python3-subscription-manager-rhsm
+Conflicts: %{package_name}-server <= 0.16-1
+
+
+%description  -n python3-ipahcc
+python3-ipahcc provides Python libraries that are used by ipa-hcc-client and
+ipa-hcc-server packages.
+
+%if %{with pyproject_macros}
+%pyproject_extras_subpkg -n python3-ipahcc server
+%endif
+
 %if %{with server}
 %package server
 Summary: IPA server plugin for Hybrid Cloud Console integration
 BuildArch: noarch
 
-%py_provides python3-ipahcc
+%if %{with pyproject_macros}
+Requires: python3-ipahcc+server = %{version}-%{release}
+%else
+Requires: python3-ipahcc = %{version}-%{release}
+Requires: python3-cryptography
+Requires: python3-jsonschema
+Requires: python3-jwcrypto
+# pyproject_macros extra dependencies
+%endif
 Requires: %{ipa_name}-server >= %{ipa_version}
 Requires(post): %{ipa_name}-server >= %{ipa_version}
 Requires: httpd
 Requires: mod_ssl
-%if %{without pyproject_macros}
-Requires: python3-cryptography
-Requires: python3-jsonschema
-Requires: python3-jwcrypto
-Requires: python3-requests
+%if %{with selinux}
+Requires: selinux-policy >= %{selinux_policy_version}
+Requires(post): selinux-policy-base >= %{selinux_policy_version}
+Requires(post): (%{name}-selinux = %{version}-%{release} if selinux-policy-%{selinuxtype})
 %endif
-Requires: selinux-policy
-Requires(post): selinux-policy
 %{?systemd_requires}
 
 %description server
 This package contains IPA server plugins, LDAP schema extension, WebUI
 extension, and registration agent for Hybrid Cloud Console integration. The
 extensions require an account on https://console.redhat.com/ and registration
 with subscription manager.
@@ -150,29 +188,25 @@
 fi
 
 %pre server
 # create user account for service
 getent passwd ipahcc >/dev/null || useradd -r -g ipaapi -s /sbin/nologin -d / -c "IPA Hybrid Cloud Console enrollment service" ipahcc
 
 %post server
-# SELinux context for cache dir
-/usr/sbin/semanage fcontext -a -f a -s system_u -t httpd_cache_t -r 's0' '/var/cache/ipa-hcc(/.*)?' 2>/dev/null || :
-/usr/sbin/restorecon -R /var/cache/ipa-hcc || :
 # ipa-hcc-update.timer is started by ipactl
 %systemd_post ipa-hcc-update.service
 %systemd_post ipa-hcc-update.timer
 /bin/systemctl daemon-reload
 
 %preun server
 %systemd_preun ipa-hcc-update.service
 %systemd_preun ipa-hcc-update.timer
 
 
 %postun server
-/usr/sbin/semanage fcontext -d '/var/cache/ipa-hcc(/.*)?' 2>/dev/null || :
 # remove pkinit_anchors line from KRB5 KDC config
 sed --in-place=.bak '/\/usr\/share\/ipa-hcc\/cacerts/d' /var/kerberos/krb5kdc/kdc.conf || :
 systemctl try-restart krb5kdc.service || :
 %systemd_postun ipa-hcc-update.service
 %systemd_postun ipa-hcc-update.timer
 
 # with server
@@ -257,15 +291,15 @@
 
 
 %if %{with client}
 %package client
 Summary: Automatic IPA client enrollment for Hybrid Cloud Console
 BuildArch: noarch
 
-Requires: %{ipa_name}-client >= %{ipa_version}
+Requires: python3-ipahcc = %{version}-%{release}
 # ipa-client RHEL 8.7, 9.1, and ealier, do not come with pkinit
 Requires: krb5-pkinit-openssl
 Recommends: subscription-manager
 %if 0%{?rhel}
 # Recommend remote host configuration and Insights client on RHEL
 # The packages are not available on Fedora. We don't support Yggdrasil.
 Recommends: rhc
@@ -287,51 +321,80 @@
 %postun client
 %systemd_postun_with_restart ipa-hcc-auto-enrollment.service
 
 # with client
 %endif
 
 
+%if %{with selinux}
+%package selinux
+Summary: SELinux policy for ipa-hcc-server
+BuildArch: noarch
+Requires: selinux-policy-%{selinuxtype} >= %{selinux_policy_version}
+Requires(post): selinux-policy-%{selinuxtype} >= %{selinux_policy_version}
+
+%description selinux
+Custom SELinux policy module for ipa-hcc-server
+
+%pre selinux
+%selinux_relabel_pre -s %{selinuxtype}
+
+%post selinux
+%selinux_modules_install -s %{selinuxtype} %{_datadir}/selinux/packages/%{selinuxtype}/%{modulename}.pp.bz2
+
+%postun selinux
+if [ $1 -eq 0 ]; then
+    %selinux_modules_uninstall -s %{selinuxtype} %{modulename}
+fi
+
+%posttrans selinux
+%selinux_relabel_post -s %{selinuxtype}
+/usr/sbin/restorecon -R /var/cache/ipa-hcc || :
+
+# with selinux
+%endif
+
+
 %prep
 # tag names are generated by rpkg
 # Release 0.14 has tag name "ipa-hcc-0.14-1", which results in top level
 # directory "ipa-hcc-ipa-hcc-0.14-1".
 {{{ git_dir_setup_macro }}}
 
 
 %if %{with pyproject_macros}
 %generate_buildrequires
 %pyproject_buildrequires
 %endif
 
 
 %build
-make module_version VERSION=%{version}
 %if %{with pyproject_macros}
 %pyproject_wheel
 %endif
 touch debugfiles.list
 
 
 %check
 %if %{without mockapi}
 # tests depend on ipahcc.mockapi
-ln -s $(pwd)/src/ipahcc/mockapi %{buildroot}%{python3_sitelib}/ipahcc/mockapi
+ln -s $(pwd)/src/ipahcc/server/mockapi.py %{buildroot}%{python3_sitelib}/ipahcc/server/mockapi.py
 %endif
 
 # tests depend on ipahcc_ modules
 ln -s -t %{buildroot}%{python3_sitelib}/ $(pwd)/src/ipahcc_*.py
 
 export PYTHONPATH=%{buildroot}%{python3_sitelib}
 %{python3} -B -Wignore -m unittest discover -s tests/
 
 # cleanup after tests
 rm -rf %{buildroot}%{python3_sitelib}/ipahcc_*.py
 %if %{without mockapi}
-rm %{buildroot}%{python3_sitelib}/ipahcc/mockapi
+rm %{buildroot}%{python3_sitelib}/ipahcc/server/mockapi.py
+rm -f %{buildroot}%{python3_sitelib}/ipahcc/server/__pycache__/mockapi*.pyc
 %endif
 
 %if %{with client}
 %{buildroot}%{_libexecdir}/ipa-hcc/ipa-hcc-auto-enrollment --help >/dev/null
 %{buildroot}%{_libexecdir}/ipa-hcc/ipa-hcc-auto-enrollment --version
 %endif
 
@@ -349,81 +412,110 @@
 %{buildroot}%{_libexecdir}/ipa-hcc/ipa-hcc-stage-console --version
 %endif
 
 
 %install
 %global make %__make -j1 DEST=%{buildroot} PREFIX=%{_prefix} PYTHON=%{python3} PYTHON_SITELIB=%{python3_sitelib} VERSION=%{version}
 
+%{__mkdir_p} %{buildroot}%{_libexecdir}/ipa-hcc
+
 %if %{with server}
+# ghost config
+%{__mkdir_p} %{buildroot}%{_sysconfdir}/ipa
+touch %{buildroot}%{_sysconfdir}/ipa/hcc.conf
 
 %if %{with pyproject_macros}
 %pyproject_install
 %else
 %make install_python
 %endif
 
 %make install_server_plugin install_registration_service
+%{__mkdir_p} %{buildroot}%{_sbindir}
+mv %{buildroot}%{_bindir}/ipa-hcc %{buildroot}%{_sbindir}/ipa-hcc
 %py3_shebang_fix %{buildroot}%{_sbindir}/ipa-hcc
-mkdir -p %{buildroot}%{_sharedstatedir}/gssproxy
+%{__mkdir_p} %{buildroot}%{_sharedstatedir}/gssproxy
 touch %{buildroot}%{_sharedstatedir}/gssproxy/hcc-enrollment.keytab
 %else
-rm -rf %{buildroot}%{python3_sitelib}/ipahcc
 rm -rf %{buildroot}%{python3_sitelib}/ipaserver
 rm -rf %{buildroot}%{python3_sitelib}/ipahcc*.dist-info
 rm -rf %{buildroot}%{python3_sitelib}/ipahcc*.egg-info
 # with server
 %endif
 
 %if %{with client}
 %make install_client
+mv %{buildroot}%{_bindir}/ipa-hcc-auto-enrollment %{buildroot}%{_libexecdir}/ipa-hcc/
+%py3_shebang_fix %{buildroot}%{_libexecdir}/ipa-hcc/ipa-hcc-auto-enrollment
+%else
+rm %{buildroot}%{_bindir}/ipa-hcc-auto-enrollment
 %endif
 
 %if %{with mockapi}
 %make install_mockapi install_client_prepare
+mv %{buildroot}%{_bindir}/ipa-hcc-client-prepare %{buildroot}%{_libexecdir}/ipa-hcc/
 %py3_shebang_fix %{buildroot}%{_libexecdir}/ipa-hcc/ipa-hcc-client-prepare
+%{__mkdir_p} %{buildroot}%{_sysconfdir}/ipa/hcc
 %else
-rm -rf %{buildroot}%{python3_sitelib}/ipahcc/mockapi
+rm %{buildroot}%{_bindir}/ipa-hcc-client-prepare
+rm %{buildroot}%{python3_sitelib}/ipahcc/server/mockapi.py
+rm -f %{buildroot}%{python3_sitelib}/ipahcc/server/__pycache__/mockapi*.pyc
 rm %{buildroot}%{python3_sitelib}/ipaserver/install/plugins/update_hcc_mockapi.py
-rm %{buildroot}%{python3_sitelib}/ipaserver/install/plugins/__pycache__/update_hcc_mockapi.*.pyc
+rm -f %{buildroot}%{python3_sitelib}/ipaserver/install/plugins/__pycache__/update_hcc_mockapi.*.pyc
 %endif
 
 %if %{with stageconsole}
-%make install_stage_console
+mv %{buildroot}%{_bindir}/ipa-hcc-stage-console %{buildroot}%{_libexecdir}/ipa-hcc/
 %py3_shebang_fix %{buildroot}%{_libexecdir}/ipa-hcc/ipa-hcc-stage-console
+%else
+rm %{buildroot}%{_bindir}/ipa-hcc-stage-console
+%endif
+
+%if %{with selinux}
+%make install_selinux SELINUXTYPE=%{selinuxtype} SELINUX_MODULENAME=%{modulename}
 %endif
 
 # We use the scripts in /usr/libexec/ipa-hcc
 rm -f  %{buildroot}%{python3_sitelib}/ipahcc_auto_enrollment.py
 rm -f  %{buildroot}%{python3_sitelib}/ipahcc_client_prepare.py
 rm -f  %{buildroot}%{python3_sitelib}/ipahcc_stage_console.py
 rm -rf %{buildroot}%{python3_sitelib}/__pycache__
 
+%files -n python3-ipahcc
+%doc README.md CONTRIBUTORS.txt
+%license COPYING
+%{python3_sitelib}/ipahcc
+%if %{with pyproject_macros}
+%{python3_sitelib}/ipahcc*.dist-info
+%else
+%{python3_sitelib}/ipahcc*.egg-info
+%endif
+# exclude files that are in mockapi package
+%if %{with mockapi}
+%exclude %{python3_sitelib}/ipahcc/server/mockapi.py
+%exclude %{python3_sitelib}/ipahcc/server/__pycache__/mockapi*.pyc
+%endif
+
 
 %if %{with server}
 %files server
 %doc README.md CONTRIBUTORS.txt
 %license COPYING
-%attr(0644,root,root) %config(noreplace) %{_sysconfdir}/ipa/hcc.conf
+%ghost %attr(0644,root,root) %config(noreplace) %{_sysconfdir}/ipa/hcc.conf
 %{_sbindir}/ipa-hcc
 %{_mandir}/man1/ipa-hcc.1*
 %dir %{_datadir}/ipa-hcc
 %{_datadir}/ipa-hcc/cacerts
+%{_datadir}/ipa-hcc/hcc.conf.example
 %{_unitdir}/ipa-hcc-update.*
-%if %{with pyproject_macros}
-%{python3_sitelib}/ipahcc*.dist-info
-%else
-%{python3_sitelib}/ipahcc*.egg-info
-%endif
 # exclude files that are in mockapi package
 %if %{with mockapi}
-%exclude %{python3_sitelib}/ipahcc/mockapi
 %exclude %{python3_sitelib}/ipaserver/install/plugins/update_hcc_mockapi.py
 %exclude %{python3_sitelib}/ipaserver/install/plugins/__pycache__/update_hcc_mockapi.*.pyc
 %endif
-%{python3_sitelib}/ipahcc
 %{python3_sitelib}/ipaserver/plugins/*.py
 %{python3_sitelib}/ipaserver/plugins/__pycache__/*.pyc
 %{python3_sitelib}/ipaserver/install/plugins/*.py
 %{python3_sitelib}/ipaserver/install/plugins/__pycache__/*.pyc
 
 %{_datadir}/ipa/schema.d/85-hcc.ldif
 %{_datadir}/ipa/updates/85-hcc.update
@@ -440,15 +532,16 @@
 %endif
 
 
 %if %{with mockapi}
 %files mockapi
 %doc README.md CONTRIBUTORS.txt
 %license COPYING
-%{python3_sitelib}/ipahcc/mockapi
+%{python3_sitelib}/ipahcc/server/mockapi.py
+%{python3_sitelib}/ipahcc/server/__pycache__/mockapi*.pyc
 %{_datadir}/ipa-hcc/hcc_mockapi.py
 %attr(0644,root,root) %config(noreplace) %{_sysconfdir}/httpd/conf.d/ipa-hcc-mockapi.conf
 %{python3_sitelib}/ipaserver/install/plugins/update_hcc_mockapi.py
 %{python3_sitelib}/ipaserver/install/plugins/__pycache__/update_hcc_mockapi.*.pyc
 %{_datadir}/ipa/updates/87-hcc-mockapi.update
 # non-standard ownership and permission to restrict the directory to ipahcc:root
 %attr(0750,ipahcc,root) %dir %{_sysconfdir}/ipa/hcc
@@ -476,9 +569,17 @@
 %doc README.md CONTRIBUTORS.txt
 %license COPYING
 %attr(0755,root,root) %{_libexecdir}/ipa-hcc/ipa-hcc-auto-enrollment
 %attr(0644,root,root) %{_unitdir}/ipa-hcc-auto-enrollment.service
 %attr(0644,root,root) %config(noreplace) %{_sysconfdir}/sysconfig/ipa-hcc-auto-enrollment
 %endif
 
+%if %{with selinux}
+%files selinux
+%doc README.md CONTRIBUTORS.txt
+%license COPYING
+%{_datadir}/selinux/packages/%{selinuxtype}/%{modulename}.pp.*
+# with selinux
+%endif
+
 %changelog
 {{{ git_dir_changelog }}}
```

### Comparing `ipahcc-0.16/pylintrc` & `ipahcc-0.17/pylintrc`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/pyproject.toml` & `ipahcc-0.17/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ipahcc"
-version = "0.16"
+dynamic = ["version"]
 description = "IPA enrollment agent for Red Hat Hybrid Cloud Console"
 readme = "README.md"
 authors = [
     {name = "Christian Heimes", email = "cheimes@redhat.com"},
 ]
 license = {text = "GPL-3.0-or-later"}
 requires-python = ">=3.6"
 dependencies = [
     "requests",
+    "ipalib",
+    # RHEL 8 with Python 3.6
+    "netaddr < 1.0.0; python_version == '3.6'",
+]
+
+[project.optional-dependencies]
+server = [
     "cryptography",
     "ipaclient",
     "jsonschema",
     "jwcrypto",
-    # RHEL 8 with Python 3.6
-    "netaddr < 1.0.0; python_version == '3.6'",
 ]
 
+[project.scripts]
+ipa-hcc = "ipahcc.server.cli:main"
+ipa-hcc-auto-enrollment = "ipahcc.client.auto_enrollment:main"
+ipa-hcc-client-prepare = "ipahcc.client.client_prepare:main"
+ipa-hcc-stage-console = "ipahcc.client.stage_console:main"
+
 [tool.setuptools]
 package-dir = {"" = "src"}
 packages = [
     "ipahcc",
-    "ipahcc.mockapi",
-    "ipahcc.registration",
+    "ipahcc.client",
     "ipahcc.server",
     "ipahcc.server.schema",
-    "ipahcc.sign",
+    "ipahcc.server.sign",
     "ipaserver.install.plugins",
     "ipaserver.plugins",
 ]
-py-modules = [
-    "ipahcc_auto_enrollment",
-    "ipahcc_client_prepare",
-    "ipahcc_stage_console",
-]
+
+[tool.setuptools.dynamic]
+version = {attr = "ipahcc._version.__version__"}
 
 [tool.setuptools.package-data]
 "ipahcc" = ["py.typed"]
 "ipahcc.server" = ["schema/*.json"]
 
 [tool.black]
 line-length = 78
@@ -57,15 +65,15 @@
     "ipahcc_auto_enrollment",
     "ipahcc",
     "ipaserver",
     "tests/",
 ]
 omit = [
     "/usr/*",
-    "*/ipahcc/sign/__main__.py",
+    "*/ipahcc/server/sign/__main__.py",
 ]
 
 [tool.coverage.paths]
 source = [
    "src/",
    ".tox/*/lib*/python*/site-packages/",
 ]
@@ -121,17 +129,17 @@
 target-version = "py37"
 extend-exclude = ["api/*.py"]
 
 [tool.ruff.per-file-ignores]
 # don't resort auto-generated stub files
 "stubs/*" = ["I"]
 # allow print in CLI scripts
+"src/ipahcc/client/auto_enrollment.py" = ["T20"]
 "src/ipahcc/server/cli.py" = ["T20"]
-"src/ipahcc_auto_enrollment.py" = ["T20"]
-"src/ipahcc/sign/__main__.py" = ["T20"]
+"src/ipahcc/server/sign/__main__.py" = ["T20"]
 
 [tool.ruff.isort]
 known-first-party = [
     "conftest",
     "ipahcc",
     "ipahcc_auto_enrollment",
     "ipaserver.plugins.hccserverroles",
```

### Comparing `ipahcc-0.16/requirements.txt` & `ipahcc-0.17/requirements.txt`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/mockapi/domain_token.py` & `ipahcc-0.17/src/ipahcc/server/domain_token.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/mockapi/wsgi.py` & `ipahcc-0.17/src/ipahcc/server/mockapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import typing
 from time import monotonic as monotonic_time
 
 import requests
 from ipalib import errors
 from ipaplatform.paths import paths
 
-from ipahcc import hccplatform, sign
-from ipahcc.server.framework import UUID_RE, HTTPException, JSONWSGIApp, route
+from ipahcc import hccplatform
 
-from . import domain_token
+from . import domain_token, sign
+from .framework import UUID_RE, HTTPException, JSONWSGIApp, route
 
 logging.basicConfig(format="%(message)s", level=logging.INFO)
 logger = logging.getLogger("ipa-mockapi")
 logger.setLevel(logging.DEBUG)
 
 
 class Application(JSONWSGIApp):
@@ -43,18 +43,22 @@
     #     self._connect_ipa()
 
     def _load_priv_jwk(self) -> typing.Optional[sign.JWKDict]:
         logger.info(
             "Loading mockapi JWK from %s", hccplatform.MOCKAPI_PRIV_JWK
         )
         try:
-            with open(hccplatform.MOCKAPI_PRIV_JWK, "r", encoding="utf-8") as f:
+            with open(
+                hccplatform.MOCKAPI_PRIV_JWK, "r", encoding="utf-8"
+            ) as f:
                 return sign.load_key(f.read())
         except OSError:
-            logger.exception("Unable to load %s", hccplatform.MOCKAPI_PRIV_JWK)
+            logger.exception(
+                "Unable to load %s", hccplatform.MOCKAPI_PRIV_JWK
+            )
             return None
 
     def get_access_token(self) -> str:  # pragma: no cover
         """Get a bearer access token from an offline token
 
         TODO: Poor man's OAuth2 workflow. Replace with
         requests-oauthlib.
@@ -78,15 +82,15 @@
             raise
 
         data = {
             "grant_type": "refresh_token",
             "client_id": hccplatform.TOKEN_CLIENT_ID,
             "refresh_token": refresh_token,
         }
-        url = hccplatform.CONFIG.token_url
+        url = self.config.token_url
         start = monotonic_time()
         resp = self.session.post(url, data)
         dur = monotonic_time() - start
         if resp.status_code >= 400:
             raise HTTPException(
                 resp.status_code,
                 f"get_access_token() failed: {resp} {resp.content!r} ({url})",
@@ -108,15 +112,15 @@
     ) -> typing.Tuple[str, str, str]:
         """Lookup host by its inventory_id
 
         Returns fqdn, inventory_id, rhsm_id
         """
         # cannot lookup from .../hosts/{inventory_id}, RHEL 7 does not include
         # subscription_manager_id in return value.
-        url = "/".join((hccplatform.CONFIG.inventory_api_url.rstrip("/"), "hosts"))
+        url = "/".join((self.config.inventory_api_url.rstrip("/"), "hosts"))
         logger.debug(
             "Looking up inventory id %s / rhsm %s in console inventory %s",
             inventory_id,
             rhsm_id,
             url,
         )
         headers = {"Authorization": f"Bearer {access_token}"}
@@ -368,13 +372,13 @@
         ipa dnszone-add podengo-project.internal.
         ipa dnsrecord-add podengo-project.internal. _hccconf \
             --uri-priority=0 --uri-weight=100 \
             --uri-target=https://$(hostname)/api/idmsvc/v1/internal/hccconf
         """
         result = {
             "domain": self.api.env.domain,
-            "idmsvc_api_url": hccplatform.CONFIG.idmsvc_api_url,
+            "idmsvc_api_url": self.config.idmsvc_api_url,
         }
-        if hccplatform.CONFIG.dev_username:
-            result["dev_username"] = hccplatform.CONFIG.dev_username
-            result["dev_password"] = hccplatform.CONFIG.dev_password
+        if self.config.dev_username:
+            result["dev_username"] = self.config.dev_username
+            result["dev_password"] = self.config.dev_password
         return result
```

### Comparing `ipahcc-0.16/src/ipahcc/registration/wsgi.py` & `ipahcc-0.17/src/ipahcc/server/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 # See COPYING for license
 #
 
 import logging
 
 from ipalib import errors
 
-from ipahcc import hccplatform, sign
-from ipahcc.server.framework import (
+from ipahcc import hccplatform
+
+from . import sign
+from .framework import (
     HTTPException,
     JSONWSGIApp,
     route,
 )
-from ipahcc.server.util import read_cert_dir
+from .util import read_cert_dir
 
 logging.basicConfig(format="%(message)s", level=logging.INFO)
 logger = logging.getLogger("ipa-hcc")
 logger.setLevel(logging.DEBUG)
 
 
 class Application(JSONWSGIApp):
```

### Comparing `ipahcc-0.16/src/ipahcc/server/cli.py` & `ipahcc-0.17/src/ipahcc/server/cli.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/framework.py` & `ipahcc-0.17/src/ipahcc/server/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import typing
 from http.client import responses as http_responses
 from urllib.parse import parse_qs
 
 import gssapi
 import ipalib
 
-from ipahcc import hccplatform, sign
+from ipahcc import hccplatform
+from ipahcc.server import sign
 from ipahcc.server.hccapi import HCCAPI, APIResult
 from ipahcc.server.schema import ValidationError, validate_schema
 from ipahcc.server.util import parse_rhsm_cert
 
 logger = logging.getLogger(__name__)
 
 
@@ -113,14 +114,18 @@
                 cachepath=hccplatform.HCC_ENROLLMENT_AGENT_CACHE_DIR,
             )
 
         self.hccapi = HCCAPI(self.api)
         self.routes = self._get_routes()
         self._cache: typing.Dict[str, typing.Any] = {}
 
+    @property
+    def config(self) -> hccplatform.HCCConfig:
+        return self.hccapi.config
+
     def _get_routes(self) -> typing.List[typing.Tuple["re.Pattern", dict]]:
         """Inspect class and get a list of routes"""
         routes: typing.Dict[str, dict] = {}
         for name, meth in inspect.getmembers(self, inspect.ismethod):
             if name.startswith("_"):
                 continue
             wr = getattr(meth, "wsgi_route", None)
@@ -218,15 +223,15 @@
     def _clear_cache(self) -> None:
         self._cache.clear()
 
     def before_call(self) -> None:
         """Before handle method call hook"""
         # check for modified hcc.conf in development mode
         if hccplatform.DEVELOPMENT_MODE:
-            hccplatform.CONFIG.refresh_config()
+            self.config.refresh_config()
 
     def after_call(self) -> None:
         """After handle method call hook"""
         self._disconnect_ipa()
         # invalidate cache and force refresh in development mode
         if hccplatform.DEVELOPMENT_MODE:
             self._clear_cache()
```

### Comparing `ipahcc-0.16/src/ipahcc/server/hccapi.py` & `ipahcc-0.17/src/ipahcc/server/hccapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
         compat_realm,
         compat_ipa_ca,
         filter_subject: typing.Optional[typing.Any] = None,
     ):  # pylint: disable=unused-argument
         raise NotImplementedError
 
 
-from ipahcc import hccplatform, sign
+from ipahcc import hccplatform
 
-from . import schema
+from . import schema, sign
 from .util import create_certinfo, parse_rhsm_cert
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_TIMEOUT = 10
 _missing = object()
 
@@ -235,18 +235,22 @@
     """Register or update domain information in HCC"""
 
     def __init__(self, api, timeout: int = DEFAULT_TIMEOUT):
         # if not api.isdone("finalize") or not api.env.in_server:
         #     raise ValueError(
         #         "api must be an in_server and finalized API object"
         #     )
-
         self.api = api
         self.timeout = timeout
+        self.config = hccplatform.HCCConfig()
         self.session = requests.Session()
+        proxy_map = self.config.proxy_map
+        if proxy_map:
+            logger.debug("Using console proxy for %s", ", ".join(proxy_map))
+            self.session.proxies = proxy_map
 
     def __enter__(self) -> "HCCAPI":
         self.api.Backend.ldap2.connect(time_limit=self.timeout)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.api.Backend.ldap2.disconnect()
@@ -688,19 +692,19 @@
         NOTE: If you use Ephemeral with RHSM cert, then you have to update
         the ``org_id`` attribute of the development user (``jdoe``) in
         Keycloak, too. The default value for ``jdoe``'s org id is ``12345``.
 
         ``openssl x509 -subject -noout -in /etc/pki/consumer/cert.pem``
         """
         if (
-            hccplatform.CONFIG.dev_org_id is not None
-            and hccplatform.CONFIG.dev_cert_cn is not None
+            self.config.dev_org_id is not None
+            and self.config.dev_cert_cn is not None
         ):
-            org_id = hccplatform.CONFIG.dev_org_id
-            cn = hccplatform.CONFIG.dev_cert_cn
+            org_id = self.config.dev_org_id
+            cn = self.config.dev_cert_cn
             source = hccplatform.HCC_CONFIG
 
         else:
             # dev_cert_cn is not set, use values from RHSM cert
             source = hccplatform.RHSM_CERT
             with open(hccplatform.RHSM_CERT, "rb") as f:
                 org_id, cn = parse_rhsm_cert(f.read())
@@ -738,32 +742,29 @@
     def _submit_idmsvc_api(
         self,
         method: str,
         subpath: tuple,
         payload: typing.Optional[typing.Dict[str, typing.Any]] = None,
         extra_headers=None,
     ) -> requests.Response:
-        api_url = hccplatform.CONFIG.idmsvc_api_url.rstrip("/")
+        api_url = self.config.idmsvc_api_url.rstrip("/")
         url = "/".join((api_url,) + subpath)
         headers = {}
         headers.update(hccplatform.HTTP_HEADERS)
         if extra_headers:
             headers.update(extra_headers)
 
-        if (
-            hccplatform.CONFIG.dev_username
-            and hccplatform.CONFIG.dev_password
-        ):
+        if self.config.dev_username and self.config.dev_password:
             logger.info(
                 "Using dev basic auth with account '%s'",
-                hccplatform.CONFIG.dev_username,
+                self.config.dev_username,
             )
             auth = requests.auth.HTTPBasicAuth(
-                hccplatform.CONFIG.dev_username,
-                hccplatform.CONFIG.dev_password,
+                self.config.dev_username,
+                self.config.dev_password,
             )
             cert = None
             headers.update(self._get_dev_headers())
         else:
             auth = None
             cert = (hccplatform.RHSM_CERT, hccplatform.RHSM_KEY)
             # open cert in reading mode to check that the file exists and is
```

### Comparing `ipahcc-0.16/src/ipahcc/server/schema/defs.json` & `ipahcc-0.17/src/ipahcc/server/schema/defs.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/schema/domain_reg_token_response.json` & `ipahcc-0.17/src/ipahcc/server/schema/domain_reg_token_response.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/schema/errors.json` & `ipahcc-0.17/src/ipahcc/server/schema/errors.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/schema/host_conf_response.json` & `ipahcc-0.17/src/ipahcc/server/schema/host_conf_response.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/schema/host_register_request.json` & `ipahcc-0.17/src/ipahcc/server/schema/host_register_request.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/schema/signing_keys_response.json` & `ipahcc-0.17/src/ipahcc/server/schema/signing_keys_response.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/schema.py` & `ipahcc-0.17/src/ipahcc/server/schema.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/server/util.py` & `ipahcc-0.17/src/ipahcc/server/util.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/sign/__init__.py` & `ipahcc-0.17/src/ipahcc/server/sign/__init__.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/sign/_jwk.py` & `ipahcc-0.17/src/ipahcc/server/sign/_jwk.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc/sign/_jwst.py` & `ipahcc-0.17/src/ipahcc/server/sign/_jwst.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipahcc.egg-info/PKG-INFO` & `ipahcc-0.17/src/ipahcc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ipahcc
-Version: 0.16
+Version: 0.17
 Summary: IPA enrollment agent for Red Hat Hybrid Cloud Console
 Author: Christian Heimes
 Author-email: Christian Heimes <cheimes@redhat.com>
 License: GPL-3.0-or-later
 Platform: any
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: requests
-Requires-Dist: cryptography
-Requires-Dist: ipaclient
-Requires-Dist: jsonschema
-Requires-Dist: jwcrypto
+Requires-Dist: ipalib
 Requires-Dist: netaddr<1.0.0; python_version == "3.6"
+Provides-Extra: server
+Requires-Dist: cryptography; extra == "server"
+Requires-Dist: ipaclient; extra == "server"
+Requires-Dist: jsonschema; extra == "server"
+Requires-Dist: jwcrypto; extra == "server"
 
 # IPA plugin for Hybrid Cloud Console
 
 The *ipa-hcc* plugin provides schema extension of IPA for
 Hybrid Cloud Console integration. The plugin must be installed on all FreeIPA
 servers, preferable before the server/replica is installed.
```

### Comparing `ipahcc-0.16/src/ipahcc.egg-info/SOURCES.txt` & `ipahcc-0.17/src/ipahcc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 install/mockapi/httpd/ipa-hcc-mockapi.conf
 install/mockapi/updates/87-hcc-mockapi.update
 install/mockapi/wsgi/hcc_mockapi.py
 install/registration/gssproxy/85-ipa-hcc.conf
 install/registration/httpd/ipa-hcc.conf
 install/registration/updates/86-hcc-registration-service.update
 install/registration/wsgi/hcc_registration_service.py
-install/server/ipa-hcc
 install/server/cacerts/00-candlepin-redhat-ca-sha256.pem
 install/server/cacerts/01-redhat-entitlement-authority-2022.pem
 install/server/cacerts/02-redhat-entitlement-master-ca.pem
 install/server/cacerts/3bba0b9d.0
 install/server/cacerts/49f9274f.0
 install/server/cacerts/fa9a18d6.0
 install/server/ipa/hcc.conf
@@ -41,34 +40,38 @@
 install/server/systemd/ipa-hcc-update.service
 install/server/systemd/ipa-hcc-update.timer
 install/server/ui/js/plugins/hccconfig/hccconfig.js
 install/server/ui/js/plugins/hcchost/hcchost.js
 install/server/ui/js/plugins/hccidp/hccidp.js
 install/server/uninstall/85-hcc-uninstall-server.update
 install/server/updates/85-hcc.update
-src/ipahcc_auto_enrollment.py
-src/ipahcc_client_prepare.py
-src/ipahcc_stage_console.py
+selinux/ipa-hcc.fc
+selinux/ipa-hcc.if
+selinux/ipa-hcc.te
 src/ipahcc/__init__.py
+src/ipahcc/_version.py
 src/ipahcc/hccplatform.py
 src/ipahcc/py.typed
 src/ipahcc.egg-info/PKG-INFO
 src/ipahcc.egg-info/SOURCES.txt
 src/ipahcc.egg-info/dependency_links.txt
+src/ipahcc.egg-info/entry_points.txt
 src/ipahcc.egg-info/requires.txt
 src/ipahcc.egg-info/top_level.txt
-src/ipahcc/mockapi/__init__.py
-src/ipahcc/mockapi/domain_token.py
-src/ipahcc/mockapi/wsgi.py
-src/ipahcc/registration/__init__.py
-src/ipahcc/registration/wsgi.py
+src/ipahcc/client/__init__.py
+src/ipahcc/client/auto_enrollment.py
+src/ipahcc/client/client_prepare.py
+src/ipahcc/client/stage_console.py
 src/ipahcc/server/__init__.py
 src/ipahcc/server/cli.py
+src/ipahcc/server/domain_token.py
 src/ipahcc/server/framework.py
 src/ipahcc/server/hccapi.py
+src/ipahcc/server/mockapi.py
+src/ipahcc/server/registration.py
 src/ipahcc/server/schema.py
 src/ipahcc/server/util.py
 src/ipahcc/server/schema/defs.json
 src/ipahcc/server/schema/domain_reg_token_request.json
 src/ipahcc/server/schema/domain_reg_token_response.json
 src/ipahcc/server/schema/errors.json
 src/ipahcc/server/schema/host_conf_request.json
@@ -77,18 +80,18 @@
 src/ipahcc/server/schema/host_register_response.json
 src/ipahcc/server/schema/ipadomain_get_request.json
 src/ipahcc/server/schema/ipadomain_register_request.json
 src/ipahcc/server/schema/ipadomain_register_response.json
 src/ipahcc/server/schema/ipadomain_update_request.json
 src/ipahcc/server/schema/ipadomain_update_response.json
 src/ipahcc/server/schema/signing_keys_response.json
-src/ipahcc/sign/__init__.py
-src/ipahcc/sign/__main__.py
-src/ipahcc/sign/_jwk.py
-src/ipahcc/sign/_jwst.py
+src/ipahcc/server/sign/__init__.py
+src/ipahcc/server/sign/__main__.py
+src/ipahcc/server/sign/_jwk.py
+src/ipahcc/server/sign/_jwst.py
 src/ipaserver/install/plugins/update_hcc.py
 src/ipaserver/install/plugins/update_hcc_enrollment_service.py
 src/ipaserver/install/plugins/update_hcc_mockapi.py
 src/ipaserver/plugins/hccconfig.py
 src/ipaserver/plugins/hcchost.py
 src/ipaserver/plugins/hccidp.py
 src/ipaserver/plugins/hccjwk.py
```

### Comparing `ipahcc-0.16/src/ipahcc_auto_enrollment.py` & `ipahcc-0.17/src/ipahcc/client/auto_enrollment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 """IPA client auto-enrollment for Hybrid Cloud Console
 
 Installation with older clients that lack PKINIT:
 
 - get configuration from remote api /host-conf
 - write a temporary krb5.conf for kinit and ipa-getkeytab commands
 - with kinit using PKINIT identity and host principal 'host/$FQDN'
@@ -25,138 +24,37 @@
 import time
 import typing
 import urllib.request
 import uuid
 
 from dns.exception import DNSException
 from ipalib import constants, util, x509
-from ipaplatform.osinfo import osinfo
 from ipaplatform.paths import paths
 from ipaplatform.tasks import tasks
 from ipapython import ipautil
 from ipapython.dnsutil import query_srv
 from ipapython.version import VENDOR_VERSION as IPA_VERSION
 
+from ipahcc import hccplatform
+
 try:
     # pylint: disable=ungrouped-imports
     from ipalib.install.dnsforwarders import detect_resolve1_resolv_conf
 except ModuleNotFoundError:
 
     def detect_resolve1_resolv_conf() -> bool:
         return False
 
 
-get_rhsm_config: typing.Optional[typing.Callable]
-try:
-    # pylint: disable=ungrouped-imports
-    from rhsm.config import get_config_parser as get_rhsm_config
-except ImportError:
-    get_rhsm_config = None
-
 FQDN = socket.gethostname()
 
-# version is updated by Makefile
-VERSION = "0.16"
-
-# copied from ipahcc.hccplatform
-DEVELOPMENT_MODE = True
-RHSM_CERT = "/etc/pki/consumer/cert.pem"
-RHSM_KEY = "/etc/pki/consumer/key.pem"
-RHSM_CONF = "/etc/rhsm/rhsm.conf"
-INSIGHTS_MACHINE_ID = "/etc/insights-client/machine-id"
-INSIGHTS_HOST_DETAILS = "/var/lib/insights/host-details.json"
-# Prod cert-api uses internal CA while stage uses a public CA
-IPA_DEFAULT_CONF = paths.IPA_DEFAULT_CONF
-HCC_DOMAIN_TYPE = "rhel-idm"
-HTTP_HEADERS = {
-    "User-Agent": f"IPA HCC auto-enrollment {VERSION} (IPA: {IPA_VERSION})",
-    "X-RH-IDM-Version": json.dumps(
-        {
-            "ipa-hcc": VERSION,
-            "ipa": IPA_VERSION,
-            "os-release-id": osinfo["ID"],
-            "os-release-version-id": osinfo["VERSION_ID"],
-        }
-    ),
-}
 
 logger = logging.getLogger(__name__)
 
 
-class ConsoleConfig(typing.NamedTuple):
-    env: str
-    rhsm_server: str
-    # base url for inventory v1
-    inventory_cert_url: str
-    # base url for idmsvc v1
-    idmsvc_cert_url: str
-    # Prod cert-api uses internal CA while stage uses a public CA
-    cert_api_cafile: typing.Optional[str]
-
-
-PROD_CONSOLE = ConsoleConfig(
-    env="prod",
-    rhsm_server="subscription.rhsm.redhat.com",
-    inventory_cert_url="https://cert.console.redhat.com/api/inventory/v1",
-    idmsvc_cert_url="https://cert.console.redhat.com/api/idmsvc/v1",
-    cert_api_cafile="/etc/rhsm/ca/redhat-uep.pem",
-)
-
-STAGE_CONSOLE = ConsoleConfig(
-    env="stage",
-    rhsm_server="subscription.rhsm.stage.redhat.com",
-    inventory_cert_url="https://cert.console.stage.redhat.com/api/inventory/v1",
-    idmsvc_cert_url="https://cert.console.stage.redhat.com/api/idmsvc/v1",
-    cert_api_cafile=None,
-)
-
-ProxyUrl = typing.Optional[str]
-
-
-def detect_rhsm_config() -> typing.Tuple[ConsoleConfig, ProxyUrl]:
-    """Detect configuration from RHSM config"""
-    rhsm_server: str
-    proxy_url: ProxyUrl = None
-    if get_rhsm_config is not None:
-        logger.debug("Using RHSM config")
-        rhsm_config = get_rhsm_config()
-        rhsm_server = rhsm_config.get("server", "hostname").strip()
-        proxy_hostname = rhsm_config.get("server", "proxy_hostname").strip()
-        if proxy_hostname:
-            proxy_scheme = (
-                rhsm_config.get("server", "proxy_scheme").strip() or "http"
-            )
-            proxy_port = (
-                rhsm_config.get("server", "proxy_port").strip() or "3128"
-            )
-            proxy_user = rhsm_config.get("server", "proxy_user").strip()
-            proxy_password = rhsm_config.get(
-                "server", "proxy_password"
-            ).strip()
-            proxy_auth = (
-                f"{proxy_user}:{proxy_password}@" if proxy_user else ""
-            )
-            proxy_url = (
-                f"{proxy_scheme}://{proxy_auth}{proxy_hostname}:{proxy_port}"
-            )
-        logger.debug(
-            "Detected RHSM server: %s, proxy: %s", rhsm_server, proxy_url
-        )
-    else:
-        logger.debug("RHSM is not available, default to prod")
-        rhsm_server = "subscription.rhsm.redhat.com"
-
-    if rhsm_server == STAGE_CONSOLE.rhsm_server:
-        cfg = STAGE_CONSOLE
-    else:
-        cfg = PROD_CONSOLE
-    logger.info("Detected configuration %s, RHSM proxy '%s'", cfg, proxy_url)
-    return cfg, proxy_url
-
-
 def check_arg_hostname(arg: str) -> str:
     hostname = arg.lower()
     if hostname in {"localhost", "localhost.localdomain"}:
         raise argparse.ArgumentError(
             None,
             f"Invalid hostname {arg}, host's FQDN is not configured.",
         )
@@ -221,15 +119,15 @@
     action="count",
 )
 parser.add_argument(
     "--version",
     "-V",
     help="Show version number and exit",
     action="version",
-    version=f"ipa-hcc {VERSION} (IPA {IPA_VERSION})",
+    version=f"ipa-hcc {hccplatform.VERSION} (IPA {IPA_VERSION})",
 )
 parser.add_argument(
     "--insecure",
     action="store_true",
     help="Use insecure connection to Console API",
 )
 parser.add_argument(
@@ -287,15 +185,15 @@
     dev_org_id=None,
     dev_cert_cn=None,
     upto=None,
     override_ipa_server=None,
     console_proxy=None,
     nameservers=None,
 )
-if DEVELOPMENT_MODE:
+if hccplatform.DEVELOPMENT_MODE:
     g_ephemeral = parser.add_argument_group("Ephemeral environment")
     # presence of --dev-username enables Ephemeral login and fake identity
     g_ephemeral.add_argument(
         "--dev-username",
         metavar="USERNAME",
         help="Ephemeral basic auth user",
         type=str,
@@ -377,15 +275,17 @@
         self.realm: typing.Optional[str] = None
         self.domain_id: typing.Optional[str] = None
         self.insights_machine_id: typing.Optional[str] = None
         self.inventory_id: typing.Optional[str] = None
         self.token: typing.Optional[str] = None
         self.install_args: typing.Iterable[str] = ()
         self.automount_location: typing.Optional[str] = None
-        self.console_config: ConsoleConfig = PROD_CONSOLE
+        self.console_config: hccplatform.ConsoleConfig = (
+            hccplatform.PROD_CONSOLE
+        )
         # internals
         self.tmpdir: typing.Optional[str] = None
 
     def __enter__(self) -> "AutoEnrollment":
         self.tmpdir = tempfile.mkdtemp()
         return self
 
@@ -403,21 +303,21 @@
         creds = f"{self.args.dev_username}:{self.args.dev_password}"
         basic_auth = base64.b64encode(creds.encode("utf-8")).decode("ascii")
         req.add_unredirected_header("Authorization", f"Basic {basic_auth}")
 
         org_id = self.args.dev_org_id
         cn = self.args.dev_cert_cn
         if cn is None or org_id is None:
-            cert = x509.load_certificate_from_file(RHSM_CERT)
+            cert = x509.load_certificate_from_file(hccplatform.RHSM_CERT)
             nas = list(cert.subject)
             org_id = nas[0].value
             cn = nas[1].value
             logger.debug(
                 "Using cert info from %s: org_id: %s, cn: %s",
-                RHSM_CERT,
+                hccplatform.RHSM_CERT,
                 org_id,
                 cn,
             )
         else:
             logger.debug(
                 "Using cert info from CLI: org_id: %s, cn: %s", org_id, cn
             )
@@ -455,38 +355,38 @@
         cafile: typing.Optional[str] = None,
         proxy: typing.Optional[str] = None,
     ) -> dict:
         headers = {
             "Accept": "application/json",
             "Content-Type": "application/json",
         }
-        headers.update(HTTP_HEADERS)
+        headers.update(hccplatform.HTTP_HEADERS)
         if body is None:
             logger.debug("GET request %s: %s", url, body)
             req = urllib.request.Request(url, headers=headers)
             assert req.get_method() == "GET"
         else:
             logger.debug("POST request %s: %s", url, body)
             data = json.dumps(body).encode("utf-8")
             # Requests with data are always POST requests.
             req = urllib.request.Request(url, data=data, headers=headers)
             assert req.get_method() == "POST"
 
         context = ssl.create_default_context(cafile=cafile)
-        context.load_cert_chain(RHSM_CERT, RHSM_KEY)
+        context.load_cert_chain(hccplatform.RHSM_CERT, hccplatform.RHSM_KEY)
         if getattr(context, "post_handshake_auth", None) is not None:
             context.post_handshake_auth = True
         if verify:
             context.verify_mode = ssl.CERT_REQUIRED
             context.check_hostname = True
         else:
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
 
-        if DEVELOPMENT_MODE and self.args.dev_username:
+        if hccplatform.DEVELOPMENT_MODE and self.args.dev_username:
             self._ephemeral_config(req)
 
         # build URL opener with custom handlers
         handlers: typing.List[urllib.request.BaseHandler]
         handlers = [urllib.request.HTTPSHandler(context=context)]
         if proxy:
             logger.info("Using proxy %s for request to %s", proxy, url)
@@ -568,44 +468,44 @@
             f"FILE:{self.kdc_cacert}",
             # IPA CA signs KDC cert
             f"FILE:{self.ipa_cacert}",
         ]
 
     @property
     def pkinit_identity(self) -> str:
-        return f"FILE:{RHSM_CERT},{RHSM_KEY}"
+        return f"FILE:{hccplatform.RHSM_CERT},{hccplatform.RHSM_KEY}"
 
     @property
     def krb_name(self) -> str:
         if typing.TYPE_CHECKING:
             assert self.tmpdir
         return os.path.join(self.tmpdir, "krb5.conf")
 
     def check_system_state(self) -> None:
-        for fname in (RHSM_CERT, RHSM_KEY):
+        for fname in (hccplatform.RHSM_CERT, hccplatform.RHSM_KEY):
             if not os.path.isfile(fname):
                 raise SystemStateError(
                     "Host is not registered with subscription-manager.",
                     "subscription-manager register",
                     fname,
                 )
-        if not os.path.isfile(INSIGHTS_MACHINE_ID):
+        if not os.path.isfile(hccplatform.INSIGHTS_MACHINE_ID):
             raise SystemStateError(
                 "Host is not registered with Insights.",
                 "insights-client --register",
-                INSIGHTS_MACHINE_ID,
+                hccplatform.INSIGHTS_MACHINE_ID,
             )
         # if INSIGHTS_HOST_DETAILS is missing, fall back to HTTP API call
-        if os.path.isfile(IPA_DEFAULT_CONF) and not self.args.upto:
+        if os.path.isfile(paths.IPA_DEFAULT_CONF) and not self.args.upto:
             raise SystemStateError(
-                "Host is already an IPA client.", None, IPA_DEFAULT_CONF
+                "Host is already an IPA client.", None, paths.IPA_DEFAULT_CONF
             )
 
     def enroll_host(self) -> None:
-        self.console_config, proxy_url = detect_rhsm_config()
+        self.console_config, proxy_url = hccplatform.detect_rhsm_config()
         if self.args.console_proxy is None and proxy_url is not None:
             logger.debug("Using console proxy from RHSM: %s", proxy_url)
             self.args.console_proxy = proxy_url
         if self.args.idmsvc_api_url is None:
             logger.debug("Using default idmsvc url")
             self.args.idmsvc_api_url = self.console_config.idmsvc_cert_url
 
@@ -652,15 +552,15 @@
 
     def get_host_details(self) -> dict:
         """Get inventory id from Insights' host details file or API call.
 
         insights-client stores the result of Insights API query in a local file
         once the host is registered.
         """
-        with open(INSIGHTS_MACHINE_ID, encoding="utf-8") as f:
+        with open(hccplatform.INSIGHTS_MACHINE_ID, encoding="utf-8") as f:
             self.insights_machine_id = f.read().strip()
         result = self._read_host_details_file()
         if result is None:
             result = self._get_host_details_api()
         self.inventory_id = result["results"][0]["id"]
         logger.info(
             "Host '%s' has inventory id '%s', insights id '%s'.",
@@ -674,19 +574,23 @@
         """Attempt to read host-details.json file
 
         The file is created and updated by insights-clients. On some older
         versions, the file is not created during the initial
         'insights-client --register' execution.
         """
         try:
-            with open(INSIGHTS_HOST_DETAILS, encoding="utf-8") as f:
+            with open(
+                hccplatform.INSIGHTS_HOST_DETAILS, encoding="utf-8"
+            ) as f:
                 j = json.load(f)
         except (OSError, ValueError) as e:
             logger.debug(
-                "Failed to read JSON file %s: %s", INSIGHTS_HOST_DETAILS, e
+                "Failed to read JSON file %s: %s",
+                hccplatform.INSIGHTS_HOST_DETAILS,
+                e,
             )
             return None
         else:
             if j["total"] != 1:
                 return None
             return j
 
@@ -700,15 +604,14 @@
         time.sleep(3)  # short initial sleep
         sleep_dur = 10  # sleep for 10, 20, 40, ...
         for _i in range(5):
             try:
                 j = self._do_json_request(
                     url,
                     verify=True,
-                    cafile=self.console_config.cert_api_cafile,
                     proxy=self.args.console_proxy,
                 )
             except Exception:  # pylint: disable=broad-exception-caught
                 logger.exception(
                     "Failed to request host details from %s", url
                 )
                 break
@@ -781,15 +684,15 @@
                 idx += 1000
             dsu[fqdn] = idx
 
         return sorted(dsu, key=dsu.get, reverse=True)  # type: ignore
 
     def hcc_host_conf(self) -> dict:
         body = {
-            "domain_type": HCC_DOMAIN_TYPE,
+            "domain_type": hccplatform.HCC_DOMAIN_TYPE,
         }
         for key in ["domain_name", "domain_id", "location"]:
             value = getattr(self.args, key)
             if value is not None:
                 body[key] = value
 
         url = "{api_url}/host-conf/{inventory_id}/{hostname}".format(
@@ -808,32 +711,29 @@
                 verify=verify,
                 proxy=self.args.console_proxy,
             )
         except Exception:
             logger.error("Failed to get host configuration from %s", url)
             raise SystemExit(2) from None
 
+        if j["domain_type"] != hccplatform.HCC_DOMAIN_TYPE:
+            raise ValueError(j["domain_type"])
+        dt = hccplatform.HCC_DOMAIN_TYPE
         with open(self.ipa_cacert, "w", encoding="utf-8") as f:
-            f.write(j[HCC_DOMAIN_TYPE]["cabundle"])
+            f.write(j[dt]["cabundle"])
 
-        if j["domain_type"] != HCC_DOMAIN_TYPE:
-            raise ValueError(j["domain_type"])
         self.domain = j["domain_name"]
         self.domain_id = j["domain_id"]
         # TODO: make token required
         self.token = j.get("token")
-        self.realm = j[HCC_DOMAIN_TYPE]["realm_name"]
+        self.realm = j[dt]["realm_name"]
         # install args and automount location are optional
-        self.install_args = j[HCC_DOMAIN_TYPE].get(
-            "ipa_client_install_args", []
-        )
-        self.automount_location = j[HCC_DOMAIN_TYPE].get(
-            "automount_location", None
-        )
-        self.enrollment_servers = j[HCC_DOMAIN_TYPE]["enrollment_servers"]
+        self.install_args = j[dt].get("ipa_client_install_args", [])
+        self.automount_location = j[dt].get("automount_location", None)
+        self.enrollment_servers = j[dt]["enrollment_servers"]
         if typing.TYPE_CHECKING:
             assert self.enrollment_servers
         logger.info("Domain: %s", self.domain)
         logger.info("Realm: %s", self.realm)
         logger.info(
             "Enrollment servers: %s", json.dumps(self.enrollment_servers)
         )
@@ -897,15 +797,15 @@
         """
         url = "https://{server}/hcc/{inventory_id}/{hostname}".format(
             server=self.server,
             inventory_id=self.inventory_id,
             hostname=self.args.hostname,
         )
         body = {
-            "domain_type": HCC_DOMAIN_TYPE,
+            "domain_type": hccplatform.HCC_DOMAIN_TYPE,
             "domain_name": self.domain,
             "domain_id": self.domain_id,
         }
         if self.token is not None:
             body["token"] = self.token
         logger.info("Registering host at %s", url)
         try:
```

### Comparing `ipahcc-0.16/src/ipahcc_client_prepare.py` & `ipahcc-0.17/src/ipahcc/client/client_prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#!/usr/bin/env python3
 """IPA HCC client preparation service
 
 Prepares a host in stage and ephemeral testing environment
 
 - Look up magic ``_hccconf.podengo-project.internal.`` URI record in DNS
 - Retrieve configuration from the HCC configuration endpoint, which is
   provided by mockapi.
 - Fix up hostname if the hostname is not a FQDN
 - Write ``/etc/sysconfig/ipa-hcc-auto-enrollment`` with ephemeral
   configuration.
 - Run post fixers (e.g. SELinux bool for NFS home directory)
 """
+
 import argparse
 import json
 import logging
 import shlex
 import socket
 import ssl
 import typing
@@ -22,27 +22,24 @@
 
 import dns.exception
 import dns.rdatatype
 from ipaplatform.tasks import tasks
 from ipapython.dnsutil import get_ipa_resolver
 from ipapython.version import VENDOR_VERSION as IPA_VERSION
 
-# version is updated by Makefile
-VERSION = "0.16"
+from ipahcc import hccplatform
 
 HCCCONF_URI = "_hccconf.podengo-project.internal."
-RHSM_CERT = "/etc/pki/consumer/cert.pem"
-RHSM_KEY = "/etc/pki/consumer/key.pem"
 SYSCONFIG = "/etc/sysconfig/ipa-hcc-auto-enrollment"
 
 logger = logging.getLogger(__name__)
 
 parser = argparse.ArgumentParser(
-    prog="ipa-hcc-client-prepare",
-    description="IPA client prepare for testing of auto-enrollment",
+    prog="ipa-hcc-ephemeral-prepare",
+    description="IPA client pepare for testing of auto-enrollment",
 )
 
 parser.add_argument(
     "--verbose",
     "-v",
     help="Enable verbose logging",
     dest="verbose",
@@ -56,15 +53,15 @@
     default=10,
 )
 parser.add_argument(
     "--version",
     "-V",
     help="Show version number and exit",
     action="version",
-    version=f"ipa-hcc {VERSION} (IPA {IPA_VERSION})",
+    version=f"ipa-hcc {hccplatform.VERSION} (IPA {IPA_VERSION})",
 )
 
 
 class ClientPrepare:
     def __init__(self, args: argparse.Namespace):
         self.args = args
 
@@ -96,15 +93,15 @@
     def fetch_config(self, url: str, verify: bool = False) -> dict:
         headers = {
             "Accept": "application/json",
             "Content-Type": "application/json",
         }
         req = Request(url, headers=headers)
         context = ssl.create_default_context()
-        context.load_cert_chain(RHSM_CERT, RHSM_KEY)
+        context.load_cert_chain(hccplatform.RHSM_CERT, hccplatform.RHSM_KEY)
         if getattr(context, "post_handshake_auth", None) is not None:
             context.post_handshake_auth = True
         if verify:
             context.verify_mode = ssl.CERT_REQUIRED
             context.check_hostname = True
         else:
             context.check_hostname = False
```

### Comparing `ipahcc-0.16/src/ipahcc_stage_console.py` & `ipahcc-0.17/src/ipahcc/client/stage_console.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-#!/usr/bin/env python3
 """IPA HCC stage console setup
 
 Configure system to use stage console services:
 - subscription manager
 - rhc
 - insights-client
 
 WARNING: This script is for testing only. It makes no effort to retain
 existing configuration.
 """
+
 import argparse
 import configparser
 import logging
 import pathlib
 import shutil
 import subprocess
 from urllib.parse import urlparse
 
-# version is updated by Makefile
-VERSION = "0.16"
+from ipahcc import hccplatform
 
 RHSM_CONF_FILE = pathlib.Path("/etc/rhsm/rhsm.conf")
 RHSM_SERVER_HOSTNAME = "subscription.rhsm.{suffix}"
 RHSM_RHSM_BASEURL = "https://cdn.{suffix}"
 
 INSIGHTS_CLIENT_CONF_FILE = pathlib.Path(
     "/etc/insights-client/insights-client.conf"
@@ -80,15 +79,15 @@
     help="Override ipa-hcc's and insight-client's auto-detection",
 )
 parser.add_argument(
     "--version",
     "-V",
     help="Show version number and exit",
     action="version",
-    version=f"ipa-hcc {VERSION}",
+    version=f"ipa-hcc {hccplatform.VERSION}",
 )
 parser.add_argument(
     "suffix",
     choices=["stage.redhat.com"],
 )
 parser.add_argument(
     "--proxy",
@@ -132,54 +131,54 @@
         ]
     )
 
 
 def configure_rhc(suffix: str, proxy: str):
     logger.info("Configuring RHC for %s", suffix)
     _backup_file(RHC_CONFIG_TOML_FILE)
-    with RHC_CONFIG_TOML_FILE.open("w") as f:
+    with RHC_CONFIG_TOML_FILE.open("w", encoding="utf-8") as f:
         f.write(RHC_CONF.format(suffix=suffix))
 
     logger.info("Configuring rhcd.service for proxy: %s", proxy)
     RHCD_SYSTEMD_PROXY_CONF_FILE.parent.mkdir(exist_ok=True)
-    with RHCD_SYSTEMD_PROXY_CONF_FILE.open("w") as f:
+    with RHCD_SYSTEMD_PROXY_CONF_FILE.open("w", encoding="utf-8") as f:
         f.write(RHCD_SYSTEMD_PROXY_CONF.format(proxy=proxy))
     logger.info("Reloading systemd daemon and try-restarting rhcd.service")
     subprocess.check_call(["/bin/systemctl", "daemon-reload"])
     subprocess.check_call(["/bin/systemctl", "try-restart", "rhcd.service"])
 
 
 def configure_insights_client(suffix: str, proxy: str):
     logger.info(
         "Configuring insights-client for %s, proxy: %s", suffix, proxy
     )
     _backup_file(INSIGHTS_CLIENT_CONF_FILE)
     cfg = configparser.ConfigParser()
     cfg.add_section("insights-client")
-    with INSIGHTS_CLIENT_CONF_FILE.open() as f:
+    with INSIGHTS_CLIENT_CONF_FILE.open(encoding="utf-8") as f:
         cfg.read_file(f)
     # https://github.com/RedHatInsights/insights-client?tab=readme-ov-file#recommended-developer-config
     cfg.set(
         "insights-client", "base_url", INSIGHTS_BASE_URL.format(suffix=suffix)
     )
     # insight-cores auto-config should detect rhsm_proxy_hostname, too.
     # Set proxy again in case auto-config is disabled.
     cfg.set("insights-client", "proxy", proxy)
-    with INSIGHTS_CLIENT_CONF_FILE.open("w") as f:
+    with INSIGHTS_CLIENT_CONF_FILE.open("w", encoding="utf-8") as f:
         cfg.write(f, space_around_delimiters=False)
 
 
 def configure_ipahcc_auto_enrollment(suffix: str, proxy: str):
     logger.info(
         "Configuring ipa-hcc-auto-enrollment.service for %s, proxy: %s",
         suffix,
         proxy,
     )
     _backup_file(IPAHCC_AUTO_ENROLLMENT_ENVFILE)
-    with IPAHCC_AUTO_ENROLLMENT_ENVFILE.open("w") as f:
+    with IPAHCC_AUTO_ENROLLMENT_ENVFILE.open("w", encoding="utf-8") as f:
         f.write(
             IPAHCC_AUTO_ENROLLMENT_CONF.format(
                 suffix=suffix,
                 proxy=proxy,
             )
         )
```

### Comparing `ipahcc-0.16/src/ipaserver/install/plugins/update_hcc.py` & `ipahcc-0.17/src/ipaserver/install/plugins/update_hcc.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipaserver/install/plugins/update_hcc_enrollment_service.py` & `ipahcc-0.17/src/ipaserver/install/plugins/update_hcc_enrollment_service.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipaserver/install/plugins/update_hcc_mockapi.py` & `ipahcc-0.17/src/ipaserver/install/plugins/update_hcc_mockapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 """Configure Hybrid Cloud Console MockAPI settings
 """
 import logging
 import os
 
 from ipalib import Registry, Updater, errors
 
-from ipahcc import hccplatform, sign
+from ipahcc import hccplatform
+from ipahcc.server import sign
 
 logger = logging.getLogger(__name__)
 
 register = Registry()
 
 
 @register()
```

### Comparing `ipahcc-0.16/src/ipaserver/plugins/hccconfig.py` & `ipahcc-0.17/src/ipaserver/plugins/hccconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
 config_mod.register_exc_callback(config_mod_hcc_exccb)
 
 i18n_messages.messages["hccconfig"] = {
     "name": _("Hybrid Cloud Console configuration")
 }
 
 # hcc_inventory_url is used by browser UI to generate a link to HBI.
-# This value is not refreshed when hccplatform.CONFIG is reloaded.
-inventory_url = urlparse(hccplatform.CONFIG.inventory_api_url)
+# This value is not refreshed when hccplatform.HCCConfig is reloaded.
+inventory_url = urlparse(hccplatform.HCCConfig().inventory_api_url)
 
 # pylint: disable=protected-access
 api.env._Env__d.update(
     hcc_inventory_url=(
         f"{inventory_url.scheme}://{inventory_url.netloc}/insights/inventory"
     ),
 )
```

### Comparing `ipahcc-0.16/src/ipaserver/plugins/hcchost.py` & `ipahcc-0.17/src/ipaserver/plugins/hcchost.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipaserver/plugins/hccidp.py` & `ipahcc-0.17/src/ipaserver/plugins/hccidp.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/src/ipaserver/plugins/hccjwk.py` & `ipahcc-0.17/src/ipaserver/plugins/hccjwk.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     LDAPDelete,
     LDAPObject,
     LDAPRetrieve,
     LDAPSearch,
     LDAPUpdate,
 )
 
-from ipahcc import hccplatform, sign
+from ipahcc import hccplatform
+from ipahcc.server import sign
 
 logger = logging.getLogger(__name__)
 
 
 REVOKED_MARKER = sign.KeyState.REVOKED.value
```

### Comparing `ipahcc-0.16/src/ipaserver/plugins/hccserverroles.py` & `ipahcc-0.17/src/ipaserver/plugins/hccserverroles.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaclient/remote_plugins/schema.pyi` & `ipahcc-0.17/stubs/ipaclient/remote_plugins/schema.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/__init__.pyi` & `ipahcc-0.17/stubs/ipalib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/backend.pyi` & `ipahcc-0.17/stubs/ipalib/backend.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/base.pyi` & `ipahcc-0.17/stubs/ipalib/base.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/config.pyi` & `ipahcc-0.17/stubs/ipalib/config.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/constants.pyi` & `ipahcc-0.17/stubs/ipalib/constants.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/crud.pyi` & `ipahcc-0.17/stubs/ipalib/crud.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/errors.pyi` & `ipahcc-0.17/stubs/ipalib/errors.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/frontend.pyi` & `ipahcc-0.17/stubs/ipalib/frontend.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/install/certstore.pyi` & `ipahcc-0.17/stubs/ipalib/install/certstore.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/install/kinit.pyi` & `ipahcc-0.17/stubs/ipalib/install/kinit.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/messages.pyi` & `ipahcc-0.17/stubs/ipalib/messages.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/output.pyi` & `ipahcc-0.17/stubs/ipalib/output.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/parameters.pyi` & `ipahcc-0.17/stubs/ipalib/parameters.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/plugable.pyi` & `ipahcc-0.17/stubs/ipalib/plugable.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/text.pyi` & `ipahcc-0.17/stubs/ipalib/text.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/util.pyi` & `ipahcc-0.17/stubs/ipalib/util.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipalib/x509.pyi` & `ipahcc-0.17/stubs/ipalib/x509.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaplatform/constants.pyi` & `ipahcc-0.17/stubs/ipaplatform/constants.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaplatform/paths.pyi` & `ipahcc-0.17/stubs/ipaplatform/paths.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaplatform/redhat/services.pyi` & `ipahcc-0.17/stubs/ipaplatform/redhat/services.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaplatform/services.pyi` & `ipahcc-0.17/stubs/ipaplatform/services.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaplatform/tasks.pyi` & `ipahcc-0.17/stubs/ipaplatform/tasks.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipapython/dn.pyi` & `ipahcc-0.17/stubs/ipapython/dn.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipapython/dnsutil.pyi` & `ipahcc-0.17/stubs/ipapython/dnsutil.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipapython/ipaldap.pyi` & `ipahcc-0.17/stubs/ipapython/ipaldap.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipapython/ipautil.pyi` & `ipahcc-0.17/stubs/ipapython/ipautil.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipapython/kerberos.pyi` & `ipahcc-0.17/stubs/ipapython/kerberos.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/masters.pyi` & `ipahcc-0.17/stubs/ipaserver/masters.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/baseldap.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/baseldap.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/config.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/config.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/hccserverroles.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/hccserverroles.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/host.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/host.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/idp.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/idp.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/internal.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/internal.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/serverrole.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/serverrole.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/plugins/serverroles.pyi` & `ipahcc-0.17/stubs/ipaserver/plugins/serverroles.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/ipaserver/servroles.pyi` & `ipahcc-0.17/stubs/ipaserver/servroles.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/stubs/rhsm/config.pyi` & `ipahcc-0.17/stubs/rhsm/config.pyi`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.key` & `ipahcc-0.17/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.key`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.pem` & `ipahcc-0.17/tests/clients/3cc18ba1-1bdf-4873-b95d-7375789eefbd.pem`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/conftest.py` & `ipahcc-0.17/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # pylint: disable=too-many-locals,ungrouped-imports
 
+import configparser
 import contextlib
 import importlib
 import io
 import json
 import logging
 import os
 import sys
+import textwrap
 import typing
 import unittest
 from http.client import responses as http_responses
 from unittest import mock
 
 import gssapi
 from ipalib import api
@@ -57,14 +59,29 @@
 IPA_CA_NICKNAME = "IPA-HCC.TEST IPA CA"
 IPA_CA_CERTINFO = create_certinfo(
     load_pem_x509_certificate(IPA_CA_DATA.encode("ascii")),
     nickname=IPA_CA_NICKNAME,
 )
 KDC_CA_DATA = read_cert_dir(KDC_CA_DIR)
 
+RHSM_CONFIG = configparser.ConfigParser()
+RHSM_CONFIG.read_string(
+    textwrap.dedent(
+        """
+        [server]
+        hostname=subscription.rhsm.redhat.com
+        proxy_hostname=
+        proxy_scheme=http
+        proxy_port=
+        proxy_user=
+        proxy_password=
+        """
+    )
+)
+
 try:
     # pylint: disable=unused-import,ungrouped-imports
     import ipalib.install  # noqa: F401
 except ImportError:
     HAS_IPA_INSTALL = False
 else:
     HAS_IPA_INSTALL = True
@@ -157,33 +174,35 @@
             domain=DOMAIN,
             realm=REALM,
             host=SERVER_FQDN,
             basedn="dc=ipa-hcc,dc=test",
         )
 
     def mock_hccplatform(self):
-        cfg = mock.Mock(spec=hccplatform.CONFIG)
-        cfg.configure_mock(
+        cfgcls = mock.create_autospec(hccplatform.HCCConfig)
+        cfgcls().configure_mock(
             idmsvc_api_url="http://invalid.test",
             token_url="http://invalid.test",  # noqa: S106
             inventory_api_url="http://invalid.test",
             dev_org_id=None,
             dev_cert_cn=None,
             dev_username=None,
             dev_password=None,
         )
 
         p = mock.patch.multiple(
             "ipahcc.hccplatform",
             RHSM_CERT=RHSM_CERT,
             RHSM_KEY=RHSM_KEY,
             INSIGHTS_HOST_DETAILS=HOST_DETAILS,
+            INSIGHTS_MACHINE_ID=MACHINE_ID,
             HCC_CACERTS_DIR=KDC_CA_DIR,
             HCC_ENROLLMENT_AGENT_KEYTAB=NO_FILE,
-            CONFIG=cfg,
+            HCCConfig=cfgcls,
+            get_rhsm_config=mock.Mock(return_value=RHSM_CONFIG),
         )
         p.start()
         self.addCleanup(p.stop)
 
     def mkresponse(self, status_code, body):
         j = json.dumps(body).encode("utf-8")
         resp = Response()
```

### Comparing `ipahcc-0.16/tests/data/autoenrollment/cert.pem` & `ipahcc-0.17/tests/data/autoenrollment/cert.pem`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/data/autoenrollment/host-details.json` & `ipahcc-0.17/tests/data/autoenrollment/host-details.json`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/data/autoenrollment/ipa_ca.crt` & `ipahcc-0.17/tests/data/autoenrollment/ipa_ca.crt`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/data/autoenrollment/key.pem` & `ipahcc-0.17/tests/data/autoenrollment/key.pem`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/data/kdc.conf` & `ipahcc-0.17/tests/data/kdc.conf`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/test_autoenrollment.py` & `ipahcc-0.17/tests/test_autoenrollment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import configparser
 import json
 import os
-import textwrap
 import unittest
 from email.message import Message
 from unittest import mock
 from urllib.error import HTTPError
 from urllib.request import OpenerDirector
 
 from dns.rdtypes.IN.SRV import SRV
 from ipaplatform.paths import paths
 from ipapython import ipautil
 
 import conftest
-import ipahcc_auto_enrollment as auto_enrollment
 from ipahcc import hccplatform
+from ipahcc.client import auto_enrollment
 from ipahcc.server import schema
 
 HOST_CONF_REQUEST = {
     "domain_type": hccplatform.HCC_DOMAIN_TYPE,
 }
 
 HOST_CONF_RESPONSE = {
@@ -47,68 +45,27 @@
     "token": conftest.DUMMY_TOKEN,
 }
 
 REGISTER_RESPONSE = {"status": "ok", "kdc_cabundle": conftest.KDC_CA_DATA}
 
 IDMSVC_API_URL = f"https://{conftest.SERVER_FQDN}/api/idmsvc/v1"
 
-RHSM_CONFIG = configparser.ConfigParser()
-RHSM_CONFIG.read_string(
-    textwrap.dedent(
-        """
-        [server]
-        hostname=subscription.rhsm.redhat.com
-        proxy_hostname=
-        proxy_scheme=http
-        proxy_port=
-        proxy_user=
-        proxy_password=
-        """
-    )
-)
-
 
 class TestAutoEnrollmentNoMock(unittest.TestCase):
-    def test_module_attributes(self):
-        self.assertEqual(hccplatform.RHSM_CERT, auto_enrollment.RHSM_CERT)
-        self.assertEqual(hccplatform.RHSM_KEY, auto_enrollment.RHSM_KEY)
-        self.assertEqual(
-            hccplatform.HCC_DOMAIN_TYPE, auto_enrollment.HCC_DOMAIN_TYPE
-        )
-        self.assertEqual(
-            hccplatform.INSIGHTS_HOST_DETAILS,
-            auto_enrollment.INSIGHTS_HOST_DETAILS,
-        )
-        self.assertEqual(
-            hccplatform.HTTP_HEADERS, auto_enrollment.HTTP_HEADERS
-        )
-
     def test_schema(self):
         schema.validate_schema(HOST_CONF_REQUEST, "HostConfRequest")
         schema.validate_schema(HOST_CONF_RESPONSE, "HostConfResponse")
         schema.validate_schema(REGISTER_REQUEST, "HostRegisterRequest")
         schema.validate_schema(REGISTER_RESPONSE, "HostRegisterResponse")
 
 
 class TestAutoEnrollment(conftest.IPABaseTests):
     def setUp(self):
         super().setUp()
-        modname = "ipahcc_auto_enrollment"
-        p = mock.patch.multiple(
-            modname,
-            RHSM_CERT=conftest.RHSM_CERT,
-            RHSM_KEY=conftest.RHSM_KEY,
-            RHSM_CONF=conftest.NO_FILE,
-            INSIGHTS_HOST_DETAILS=conftest.HOST_DETAILS,
-            INSIGHTS_MACHINE_ID=conftest.MACHINE_ID,
-            IPA_DEFAULT_CONF=conftest.NO_FILE,
-            get_rhsm_config=mock.Mock(return_value=RHSM_CONFIG),
-        )
-        p.start()
-        self.addCleanup(p.stop)
+        self.mock_hccplatform()
 
         p = mock.patch.object(ipautil, "run")
         self.m_run = p.start()
         self.addCleanup(p.stop)
 
         p = mock.patch.object(OpenerDirector, "open")
         self.m_urlopen = p.start()
@@ -161,15 +118,15 @@
             # fmt: on
         )
         self.assertEqual(args.timeout, 20)
         self.assertEqual(args.idmsvc_api_url, IDMSVC_API_URL)
         self.assertEqual(args.dev_username, None)
         self.assertEqual(args.dev_cert_cn, None)
 
-        if auto_enrollment.DEVELOPMENT_MODE:
+        if hccplatform.DEVELOPMENT_MODE:
             args = self.parse_args(
                 # fmt: off
                 "--dev-username", "jdoe",
                 "--dev-password", "example",
                 "--dev-org-id", conftest.ORG_ID,
                 "--dev-cert-cn", conftest.CLIENT_RHSM_ID,
                 # fmt: on
@@ -193,25 +150,26 @@
         args = (
             "--idmsvc-api-url",
             IDMSVC_API_URL,
             "--hostname",
             conftest.CLIENT_FQDN,
         )
 
+        # any file
+        with mock.patch("ipaplatform.paths.paths.IPA_DEFAULT_CONF", __file__):
+            self.assert_args_error(
+                args, expected="Host is already an IPA client."
+            )
+
         # module vars are already mocked
-        auto_enrollment.IPA_DEFAULT_CONF = conftest.RHSM_CERT  # any file
-        self.assert_args_error(
-            args, expected="Host is already an IPA client."
-        )
-        auto_enrollment.IPA_DEFAULT_CONF = conftest.NO_FILE
-        auto_enrollment.INSIGHTS_MACHINE_ID = conftest.NO_FILE
+        hccplatform.INSIGHTS_MACHINE_ID = conftest.NO_FILE
         self.assert_args_error(
             args, expected="Host is not registered with Insights."
         )
-        auto_enrollment.RHSM_CERT = conftest.NO_FILE
+        hccplatform.RHSM_CERT = conftest.NO_FILE
         self.assert_args_error(
             args,
             expected="Host is not registered with subscription-manager.",
         )
 
     def test_sort_servers(self):
         p = mock.patch("random.random", return_value=0.5)
@@ -262,15 +220,15 @@
         with ae:
             self.assertEqual(ae.inventory_id, None)
             ae.get_host_details()
             self.assertEqual(ae.inventory_id, conftest.CLIENT_INVENTORY_ID)
 
     def test_inventory_from_api(self):
         args = self.parse_args()
-        auto_enrollment.INSIGHTS_HOST_DETAILS = conftest.NO_FILE
+        hccplatform.INSIGHTS_HOST_DETAILS = conftest.NO_FILE
         # first call to urlopen gets host details from API
         with open(conftest.HOST_DETAILS, encoding="utf-8") as f:
             host_details = json.load(f)
         self.m_urlopen.side_effect = [
             conftest.jsonio(host_details),
             Exception,
         ]
@@ -379,15 +337,15 @@
                 "--hostname",
                 conftest.CLIENT_FQDN,
                 "--domain",
                 conftest.DOMAIN,
                 "--realm",
                 conftest.REALM,
                 "--pkinit-identity",
-                f"FILE:{auto_enrollment.RHSM_CERT},{auto_enrollment.RHSM_KEY}",
+                f"FILE:{hccplatform.RHSM_CERT},{hccplatform.RHSM_KEY}",
                 "--pkinit-anchor",
                 f"FILE:{tmpdir}/kdc_ca.crt",
                 "--pkinit-anchor",
                 f"FILE:{tmpdir}/ipa_ca.crt",
                 "--unattended",
                 "--enable-dns-updates",
             ],
```

### Comparing `ipahcc-0.16/tests/test_client_prepare.py` & `ipahcc-0.17/tests/test_client_prepare.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 import os
 import shutil
 import tempfile
-import unittest
 from unittest import mock
 
-import ipahcc_client_prepare as client_prepare
 from dns.rdtypes.ANY.URI import URI
 from ipaplatform.tasks import tasks
 
 import conftest
-from ipahcc import hccplatform
+from ipahcc.client import client_prepare
 
 CONFIG = {
     "domain": conftest.DOMAIN,
     "idmsvc_api_url": "https://api.test/api/idmsvc/v1",
     "dev_username": "user",
     "dev_password": "test",
 }
 
 
-class TestAutoEnrollmentNoMock(unittest.TestCase):
-    def test_module_attributes(self):
-        self.assertEqual(hccplatform.RHSM_CERT, client_prepare.RHSM_CERT)
-        self.assertEqual(hccplatform.RHSM_KEY, client_prepare.RHSM_KEY)
-
-
 class TestAutoEnrollment(conftest.IPABaseTests):
     def setUp(self):
         super().setUp()
         self.tmpdir = tempfile.mkdtemp()
         self.addCleanup(shutil.rmtree, self.tmpdir)
 
-        modname = "ipahcc_client_prepare"
+        self.mock_hccplatform()
         p = mock.patch.multiple(
-            modname,
-            RHSM_CERT=conftest.RHSM_CERT,
-            RHSM_KEY=conftest.RHSM_KEY,
+            client_prepare,
             SYSCONFIG=os.path.join(self.tmpdir, "ipa-hcc-auto-enrollment"),
         )
         p.start()
         self.addCleanup(p.stop)
 
         p = mock.patch.object(client_prepare, "get_ipa_resolver")
         resolver = p.start()
```

### Comparing `ipahcc-0.16/tests/test_framework.py` & `ipahcc-0.17/tests/test_framework.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/test_hccapi.py` & `ipahcc-0.17/tests/test_hccapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from unittest import mock
 
 from ipalib import x509
 from ipapython import admintool
 from ipapython.dnsutil import DNSName
 
 import conftest
-from ipahcc import hccplatform, sign
-from ipahcc.mockapi import domain_token
-from ipahcc.server import hccapi
+from ipahcc import hccplatform
+from ipahcc.server import domain_token, hccapi, sign
 
 CACERT = x509.load_pem_x509_certificate(conftest.IPA_CA_DATA.encode("ascii"))
 
 COMMON_RESULT: typing.Dict[str, typing.Any] = {
     "domain_name": conftest.DOMAIN,
     "domain_type": hccplatform.HCC_DOMAIN_TYPE,
     hccplatform.HCC_DOMAIN_TYPE: {
```

### Comparing `ipahcc-0.16/tests/test_ipaserver.py` & `ipahcc-0.17/tests/test_ipaserver.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/test_ipaserver_integration.py` & `ipahcc-0.17/tests/test_ipaserver_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import datetime
 import os
 import unittest
 
 from ipalib import api, errors
 from ipalib.facts import is_ipa_configured
 
-from ipahcc import hccplatform, sign
+from ipahcc import hccplatform
+from ipahcc.server import sign
 
 
 @unittest.skipUnless(is_ipa_configured(), "host is not an IPA server")
 class TestIPAServerIntegration(unittest.TestCase):  # pragma: no cover
     maxDiff = None
 
     @classmethod
```

### Comparing `ipahcc-0.16/tests/test_mockapi.py` & `ipahcc-0.17/tests/test_mockapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import time
 import typing
 import unittest
 import uuid
 from unittest import mock
 
 import conftest
-from ipahcc import hccplatform, sign
-from ipahcc.mockapi import domain_token, wsgi
+from ipahcc import hccplatform
+from ipahcc.server import domain_token, mockapi, sign
 
 DOMAIN_REQUEST = {
     "domain_name": conftest.DOMAIN,
     "domain_type": hccplatform.HCC_DOMAIN_TYPE,
     hccplatform.HCC_DOMAIN_TYPE: {
         "realm_name": conftest.REALM,
         "servers": [
@@ -49,18 +49,18 @@
 }
 
 PRIV_KEY = sign.generate_private_key()
 PUB_KEY = sign.get_public_key(PRIV_KEY)
 
 
 class TestMockAPIWSGI(conftest.IPAWSGIBaseTests):
-    wsgi_class = wsgi.Application
+    wsgi_class = mockapi.Application
 
     def setUp(self):
-        p = mock.patch.object(wsgi.Application, "_load_priv_jwk")
+        p = mock.patch.object(mockapi.Application, "_load_priv_jwk")
         self.m_load_priv_jwk = p.start()
         self.m_load_priv_jwk.return_value = PRIV_KEY
         self.addCleanup(p.stop)
 
         super().setUp()
 
         p = mock.patch.object(self.app, "session")
@@ -202,15 +202,15 @@
             path, DOMAIN_REQUEST, method="GET"
         )
         self.assert_response(200, status_code, status_msg, headers, response)
         self.assertEqual(
             response,
             {
                 "domain": conftest.DOMAIN,
-                "idmsvc_api_url": "https://console.redhat.com/api/idmsvc/v1",
+                "idmsvc_api_url": "https://cert.console.redhat.com/api/idmsvc/v1",
             },
         )
 
 
 class TestDomRegToken(unittest.TestCase):
     token = "F3n-iOZn1VI.wbzIH7v-kRrdvfIvia4nBKAvEpIKGdv6MSIFXeUtqVY"  # noqa: S105
     domain_id = uuid.UUID("7b160558-8273-5a24-b559-6de3ff053c63")
```

### Comparing `ipahcc-0.16/tests/test_registration.py` & `ipahcc-0.17/tests/test_registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 from unittest import mock
 
 import conftest
-from ipahcc import hccplatform, sign
-from ipahcc.registration import wsgi
+from ipahcc import hccplatform
+from ipahcc.server import registration, sign
 
 PRIV_KEY = sign.generate_private_key()
 PUB_KEY = sign.get_public_key(PRIV_KEY)
 
 
 class TestRegistrationWSGI(conftest.IPAWSGIBaseTests):
-    wsgi_class = wsgi.Application
+    wsgi_class = registration.Application
 
     def setUp(self):
         super().setUp()
 
         p = mock.patch.object(self.app, "_get_ipa_jwkset")
         self.m_get_jwkset = p.start()
         self.m_get_jwkset.return_value = PUB_KEY
```

### Comparing `ipahcc-0.16/tests/test_schema.py` & `ipahcc-0.17/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipahcc-0.16/tests/test_sign.py` & `ipahcc-0.17/tests/test_sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from unittest import mock
 
 import jwcrypto.jwk
 import jwcrypto.jws
 import jwcrypto.jwt
 
 import conftest
-from ipahcc import sign
+from ipahcc.server import sign
 
 
 class TestJWK(unittest.TestCase):
     def test_jwk(self):
         priv = sign.generate_private_key()
         self.assertTrue(priv.has_private)
         self.assertIsInstance(priv, sign.JWKDict)
```

### Comparing `ipahcc-0.16/tests/tests.py` & `ipahcc-0.17/tests/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 from ipahcc.server.util import parse_rhsm_cert
 
 # pylint: disable=import-outside-toplevel
 
 
 class IPAClientTests(conftest.IPABaseTests):
     def test_auto_enrollment_help(self):
-        import ipahcc_auto_enrollment
-
-        self.assert_cli_run(ipahcc_auto_enrollment.main, "--help")
+        from ipahcc.client import (
+            auto_enrollment,
+            client_prepare,
+            stage_console,
+        )
+
+        self.assert_cli_run(auto_enrollment.main, "--help")
+        self.assert_cli_run(client_prepare.main, "--help")
+        self.assert_cli_run(stage_console.main, "--help")
 
 
 @conftest.requires_ipaserver
 class IPAServerTests(conftest.IPABaseTests):
     def test_server_plugin_imports(self):
         # pylint: disable=unused-import,unused-variable,import-error
         from ipaserver.install.plugins import update_hcc  # noqa: F401
```

### Comparing `ipahcc-0.16/tox.ini` & `ipahcc-0.17/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 [testenv:pylint]
 sitepackages = true
 deps =
     pylint
 commands =
     {envpython} -m pylint \
         ipahcc \
-        ipahcc_auto_enrollment \
         src/ipaserver/install/plugins/update_hcc_enrollment_service.py \
         src/ipaserver/install/plugins/update_hcc.py \
         src/ipaserver/plugins/hccconfig.py \
         src/ipaserver/plugins/hcchost.py \
         src/ipaserver/plugins/hccidp.py \
         src/ipaserver/plugins/hccserverroles.py \
         tests/conftest.py \
```

