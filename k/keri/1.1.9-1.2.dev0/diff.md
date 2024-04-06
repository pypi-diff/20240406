# Comparing `tmp/keri-1.1.9.tar.gz` & `tmp/keri-1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keri-1.1.9.tar", last modified: Wed Mar 27 01:43:02 2024, max compression
+gzip compressed data, was "keri-1.2.dev0.tar", last modified: Sat Apr  6 17:12:51 2024, max compression
```

## Comparing `keri-1.1.9.tar` & `keri-1.2.dev0.tar`

### file list

```diff
@@ -1,199 +1,207 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.248848 keri-1.1.9/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.1.9/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1527 2024-03-27 01:43:02.248636 keri-1.1.9/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2456 2024-03-27 00:38:35.000000 keri-1.1.9/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-03-27 01:43:02.248888 keri-1.1.9/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3783 2024-03-27 00:38:35.000000 keri-1.1.9/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.218186 keri-1.1.9/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.220522 keri-1.1.9/src/keri/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-03-27 00:38:35.000000 keri-1.1.9/src/keri/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.226283 keri-1.1.9/src/keri/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    36847 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/apping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/challenging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.226744 keri-1.1.9/src/keri/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.230853 keri-1.1.9/src/keri/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.231577 keri-1.1.9/src/keri/app/cli/commands/challenge/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/respond.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/verify.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.231976 keri-1.1.9/src/keri/app/cli/commands/contacts/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/contacts/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2281 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/contacts/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.232392 keri-1.1.9/src/keri/app/cli/commands/delegate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/delegate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9345 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/delegate/confirm.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4082 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/delegate/request.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.232601 keri-1.1.9/src/keri/app/cli/commands/did/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/did/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/did/generate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.233286 keri-1.1.9/src/keri/app/cli/commands/ends/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/ends/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ends/add.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ends/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ends/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/escrow.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3774 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7160 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5419 2024-03-26 19:38:12.000000 keri-1.1.9/src/keri/app/cli/commands/init.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3855 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/interact.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.234799 keri-1.1.9/src/keri/app/cli/commands/ipex/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/admit.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/agree.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/apply.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/grant.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/offer.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/spurn.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/kevers.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2023-11-27 19:46:40.000000 keri-1.1.9/src/keri/app/cli/commands/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.235058 keri-1.1.9/src/keri/app/cli/commands/local/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/local/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/local/watch.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.235705 keri-1.1.9/src/keri/app/cli/commands/mailbox/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/mailbox/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/mailbox/debug.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/mailbox/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5900 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/migrate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.237139 keri-1.1.9/src/keri/app/cli/commands/multisig/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3048 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/continue.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6701 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/interact.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30794 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/notice.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10193 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/shell.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4898 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/nonce.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.237681 keri-1.1.9/src/keri/app/cli/commands/oobi/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2023-11-27 19:46:40.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/clean.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2023-11-15 20:54:14.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/resolve.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.238233 keri-1.1.9/src/keri/app/cli/commands/passcode/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/remove.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2475 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/set.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/query.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1860 2024-03-26 19:38:12.000000 keri-1.1.9/src/keri/app/cli/commands/rename.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/rollback.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8454 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/saidify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      528 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/salt.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/sign.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.238424 keri-1.1.9/src/keri/app/cli/commands/ssh/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ssh/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ssh/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/time.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.239298 keri-1.1.9/src/keri/app/cli/commands/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10784 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/create.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.239861 keri-1.1.9/src/keri/app/cli/commands/vc/registry/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/vc/revoke.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2928 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      429 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/version.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.240410 keri-1.1.9/src/keri/app/cli/commands/watcher/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1002 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2471 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/update.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.240827 keri-1.1.9/src/keri/app/cli/commands/witness/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/witness/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3059 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/witness/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4618 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/witness/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3624 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/witness/submit.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.241854 keri-1.1.9/src/keri/app/cli/common/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/config.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3893 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/common/displaying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3264 2024-03-26 19:38:12.000000 keri-1.1.9/src/keri/app/cli/common/existing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/common/incepting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/rotating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/terming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/kli.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7485 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/configing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/connecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10218 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24656 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/directing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18772 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/forwarding.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26582 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   124547 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/habbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8565 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    41620 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    73666 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/kiwiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/oobiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/querying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/signaling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/storing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.243529 keri-1.1.9/src/keri/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      114 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   240644 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/coring.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   276895 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    58260 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/parsing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26300 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/routing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/core/scheming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    63844 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/serdering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.245101 keri-1.1.9/src/keri/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   120727 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/db/basing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    75451 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/db/dbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9322 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/db/escrowing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/db/koming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    59260 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/db/subing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.245942 keri-1.1.9/src/keri/demo/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2794 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_bob.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2811 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_eve.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_kev.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2836 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_sam.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demoing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.246353 keri-1.1.9/src/keri/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24878 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/end/ending.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/end/priming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.246729 keri-1.1.9/src/keri/help/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      557 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/help/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8211 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/help/helping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18567 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/kering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.246963 keri-1.1.9/src/keri/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    19487 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.247459 keri-1.1.9/src/keri/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vc/protocoling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2505 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vc/proving.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/vc/walleting.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.248191 keri-1.1.9/src/keri/vdr/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/vdr/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34269 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    84543 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14342 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/verifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35871 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/viring.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.248381 keri-1.1.9/src/keri.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1527 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5641 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.1.9/src/keri.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      282 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.876299 keri-1.2.dev0/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.dev0/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1563 2024-04-06 17:12:51.876030 keri-1.2.dev0/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-04-05 21:44:00.000000 keri-1.2.dev0/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-04-06 17:12:51.876356 keri-1.2.dev0/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4018 2024-04-06 17:05:56.000000 keri-1.2.dev0/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.839004 keri-1.2.dev0/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.841874 keri-1.2.dev0/src/keri/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       81 2024-04-06 17:06:28.000000 keri-1.2.dev0/src/keri/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.847806 keri-1.2.dev0/src/keri/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37074 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/apping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/challenging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.848349 keri-1.2.dev0/src/keri/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.852701 keri-1.2.dev0/src/keri/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.853277 keri-1.2.dev0/src/keri/app/cli/commands/challenge/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/challenge/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/challenge/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/challenge/respond.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/challenge/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/clean.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.853666 keri-1.2.dev0/src/keri/app/cli/commands/contacts/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/contacts/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-04-05 21:54:29.000000 keri-1.2.dev0/src/keri/app/cli/commands/contacts/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.854045 keri-1.2.dev0/src/keri/app/cli/commands/delegate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/delegate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9342 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/delegate/confirm.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/delegate/request.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.854238 keri-1.2.dev0/src/keri/app/cli/commands/did/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/did/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/did/generate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.854941 keri-1.2.dev0/src/keri/app/cli/commands/ends/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/ends/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ends/add.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ends/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ends/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/escrow.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3774 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7156 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/init.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3855 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/interact.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.856464 keri-1.2.dev0/src/keri/app/cli/commands/ipex/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/admit.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/agree.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/apply.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/grant.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/offer.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ipex/spurn.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/kevers.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2023-11-27 19:46:40.000000 keri-1.2.dev0/src/keri/app/cli/commands/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.856694 keri-1.2.dev0/src/keri/app/cli/commands/local/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/local/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/local/watch.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.857175 keri-1.2.dev0/src/keri/app/cli/commands/mailbox/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/mailbox/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/mailbox/debug.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/mailbox/update.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.857646 keri-1.2.dev0/src/keri/app/cli/commands/migrate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/migrate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/migrate/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/migrate/run.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/migrate/show.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/migrate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.859038 keri-1.2.dev0/src/keri/app/cli/commands/multisig/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/continue.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/interact.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30790 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/notice.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10190 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/shell.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-04-05 21:54:29.000000 keri-1.2.dev0/src/keri/app/cli/commands/multisig/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/nonce.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.859609 keri-1.2.dev0/src/keri/app/cli/commands/oobi/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/oobi/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2023-11-27 19:46:40.000000 keri-1.2.dev0/src/keri/app/cli/commands/oobi/clean.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/oobi/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2023-11-15 20:54:14.000000 keri-1.2.dev0/src/keri/app/cli/commands/oobi/resolve.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.860471 keri-1.2.dev0/src/keri/app/cli/commands/passcode/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/passcode/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/passcode/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/passcode/remove.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2475 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/passcode/set.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/query.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/rename.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/rollback.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8450 2024-04-05 21:21:34.000000 keri-1.2.dev0/src/keri/app/cli/commands/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/saidify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      528 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/salt.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/sign.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.860753 keri-1.2.dev0/src/keri/app/cli/commands/ssh/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ssh/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/ssh/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/time.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.861767 keri-1.2.dev0/src/keri/app/cli/commands/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10784 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/create.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-03-29 15:29:32.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.862281 keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/cli/commands/vc/revoke.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/commands/version.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.862911 keri-1.2.dev0/src/keri/app/cli/commands/witness/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/witness/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3059 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/commands/witness/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4833 2024-04-05 21:21:50.000000 keri-1.2.dev0/src/keri/app/cli/commands/witness/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3624 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/commands/witness/submit.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.864583 keri-1.2.dev0/src/keri/app/cli/common/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/common/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/common/config.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/common/displaying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/cli/common/existing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/common/incepting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/common/rotating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/cli/common/terming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/cli/kli.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/configing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/connecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10240 2024-04-05 21:20:43.000000 keri-1.2.dev0/src/keri/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/directing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/forwarding.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26589 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   124508 2024-04-05 21:21:01.000000 keri-1.2.dev0/src/keri/app/habbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8557 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    41662 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    73666 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/kiwiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/oobiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/querying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/signaling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/app/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/app/storing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.866466 keri-1.2.dev0/src/keri/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      465 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   233518 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/coring.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37102 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/counting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   305955 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34157 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/indexing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    58447 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/parsing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26305 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/routing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/core/scheming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    80505 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/core/serdering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.870775 keri-1.2.dev0/src/keri/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   127626 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/db/basing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/db/dbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9316 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/db/escrowing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/db/koming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.871020 keri-1.2.dev0/src/keri/db/migrations/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/db/migrations/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/db/migrations/rekey_habs.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    59483 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/db/subing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.872632 keri-1.2.dev0/src/keri/demo/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/demo/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2794 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/demo/demo_bob.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2811 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/demo/demo_eve.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/demo/demo_kev.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2836 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/demo/demo_sam.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/demo/demoing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.873230 keri-1.2.dev0/src/keri/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24903 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/end/ending.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/end/priming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.873574 keri-1.2.dev0/src/keri/help/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      557 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/help/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12490 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/help/helping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    27047 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.873805 keri-1.2.dev0/src/keri/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    19472 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.874407 keri-1.2.dev0/src/keri/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.dev0/src/keri/vc/protocoling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2511 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/vc/proving.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.dev0/src/keri/vc/walleting.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.875238 keri-1.2.dev0/src/keri/vdr/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.dev0/src/keri/vdr/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34269 2024-04-04 13:35:27.000000 keri-1.2.dev0/src/keri/vdr/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    84597 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/vdr/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14381 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/vdr/verifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-04-05 21:19:51.000000 keri-1.2.dev0/src/keri/vdr/viring.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.875744 keri-1.2.dev0/src/keri.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1563 2024-04-06 17:12:51.000000 keri-1.2.dev0/src/keri.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5817 2024-04-06 17:12:51.000000 keri-1.2.dev0/src/keri.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-04-06 17:12:51.000000 keri-1.2.dev0/src/keri.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-04-06 17:12:51.000000 keri-1.2.dev0/src/keri.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.dev0/src/keri.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      300 2024-04-06 17:12:51.000000 keri-1.2.dev0/src/keri.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-04-06 17:12:51.000000 keri-1.2.dev0/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-06 17:12:51.875370 keri-1.2.dev0/tests/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-04-05 21:19:51.000000 keri-1.2.dev0/tests/test_kering.py
```

### Comparing `keri-1.1.9/LICENSE` & `keri-1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/PKG-INFO` & `keri-1.2.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.1.9
+Version: 1.2.dev0
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/WebOfTrust/keripy/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10.4
+Requires-Python: >=3.12.2
 License-File: LICENSE
-Requires-Dist: lmdb>=1.3.0
-Requires-Dist: pysodium>=0.7.12
-Requires-Dist: blake3>=0.3.1
-Requires-Dist: msgpack>=1.0.4
-Requires-Dist: cbor2>=5.4.3
-Requires-Dist: multidict>=6.0.2
+Requires-Dist: lmdb>=1.4.1
+Requires-Dist: pysodium>=0.7.17
+Requires-Dist: blake3>=0.4.1
+Requires-Dist: msgpack>=1.0.8
+Requires-Dist: cbor2>=5.6.2
+Requires-Dist: multidict>=6.0.5
 Requires-Dist: ordered-set>=4.1.0
-Requires-Dist: hio>=0.6.9
+Requires-Dist: hio>=0.6.12
 Requires-Dist: multicommand>=1.0.0
-Requires-Dist: jsonschema>=4.17.0
-Requires-Dist: falcon>=3.1.0
-Requires-Dist: hjson>=3.0.2
-Requires-Dist: PyYaml>=6.0
-Requires-Dist: apispec>=6.0.0
-Requires-Dist: mnemonic>=0.20
-Requires-Dist: PrettyTable>=3.5.0
-Requires-Dist: http_sfv>=0.9.8
-Requires-Dist: cryptography>=39.0.2
+Requires-Dist: jsonschema>=4.21.1
+Requires-Dist: falcon>=3.1.3
+Requires-Dist: hjson>=3.1.0
+Requires-Dist: PyYaml>=6.0.1
+Requires-Dist: apispec>=6.6.0
+Requires-Dist: mnemonic>=0.21
+Requires-Dist: PrettyTable>=3.10.0
+Requires-Dist: http_sfv>=0.9.9
+Requires-Dist: cryptography>=42.0.5
+Requires-Dist: semver>=3.0.2
 
 KERI Decentralized Key Management Infrastructure
```

### Comparing `keri-1.1.9/README.md` & `keri-1.2.dev0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 to get a version string similar to the following: 
 
 `1.0.0`
 
 ### Local installation - Docker build
 Run `make build-keri` to build your docker image.
 
-Then run `docker run --pull=never -it --entrypoint /bin/bash weboftrust/keri:1.1.9` and you can run `kli version` from within the running container to play with KERIpy.
+Then run `docker run --pull=never -it --entrypoint /bin/bash weboftrust/keri:1.1.10` and you can run `kli version` from within the running container to play with KERIpy.
 
 Make sure the image tag matches the version used in the `Makefile`.
 We use `--pull=never` to ensure that docker does not implicitly pull a remote image and relies on the local image tagged during `make build-keri`.
 
 ### Dependencies
 #### Binaries
 
-python 3.10.4+
+python 3.12.1+
 libsodium 1.0.18+
 
 
 #### python packages
 lmdb 0.98+
 pysodium 0.7.5+
 blake3 0.1.5+
@@ -62,15 +62,15 @@
 $ pip3 install -U cbor2
 ```
 
 
 ## Development
 
 ### Setup
-* Ensure Python 3.10.4 is present along with venv and dev header files;
+* Ensure Python 3.12.1 is present along with venv and dev header files;
 * Setup virtual environment: `python3 -m venv keripy`
 * Activate virtual environment: `source keripy/bin/activate`
 * Setup dependencies: `pip install -r requirements.txt`
 
 ### Testing
 * Install pytest: `pip install pytest`
```

### Comparing `keri-1.1.9/setup.py` & `keri-1.2.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 Pypi Release
 $ pip3 install twine
 
 $ python3 setup.py sdist
 $ twine upload dist/keri-0.0.1.tar.gz
 
 Create release git:
+$ git tag # lists all tags
+$ git tag -a v0.6.11 -m "new feature"
+$ git show v0.6.11
+$ git push --tags # pushes tags to default remote
+$ git push wot --tags   # pushes tags to wot remote
+
 $ git tag -a v0.4.2 -m "bump version"
 $ git push --tags
 $ git checkout -b release_0.4.2
 $ git push --set-upstream origin release_0.4.2
 $ git checkout master
 
 Best practices for setup.py and requirements.txt
@@ -27,15 +33,15 @@
 from glob import glob
 from os.path import basename
 from os.path import splitext
 
 from setuptools import find_packages, setup
 setup(
     name='keri',
-    version='1.1.9',  # also change in src/keri/__init__.py
+    version='1.2.dev0',  # also change in src/keri/__init__.py
     license='Apache Software License 2.0',
     description='Key Event Receipt Infrastructure',
     long_description="KERI Decentralized Key Management Infrastructure",
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
     url='https://github.com/WebOfTrust/keripy',
     packages=find_packages('src'),
@@ -47,15 +53,15 @@
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: Unix',
         'Operating System :: POSIX',
         'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         # uncomment if you test on these interpreters:
         # 'Programming Language :: Python :: Implementation :: PyPy',
         # 'Programming Language :: Python :: Implementation :: IronPython',
         # 'Programming Language :: Python :: Implementation :: Jython',
         # 'Programming Language :: Python :: Implementation :: Stackless',
         'Topic :: Utilities',
@@ -64,40 +70,41 @@
         'Documentation': 'https://keri.readthedocs.io/',
         'Changelog': 'https://keri.readthedocs.io/en/latest/changelog.html',
         'Issue Tracker': 'https://github.com/WebOfTrust/keripy/issues',
     },
     keywords=[
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
-    python_requires='>=3.10.4',
+    python_requires='>=3.12.2',
     install_requires=[
-                        'lmdb>=1.3.0',
-                        'pysodium>=0.7.12',
-                        'blake3>=0.3.1',
-                        'msgpack>=1.0.4',
-                        'cbor2>=5.4.3',
-                        'multidict>=6.0.2',
+                        'lmdb>=1.4.1',
+                        'pysodium>=0.7.17',
+                        'blake3>=0.4.1',
+                        'msgpack>=1.0.8',
+                        'cbor2>=5.6.2',
+                        'multidict>=6.0.5',
                         'ordered-set>=4.1.0',
-                        'hio>=0.6.9',
+                        'hio>=0.6.12',
                         'multicommand>=1.0.0',
-                        'jsonschema>=4.17.0',
-                        'falcon>=3.1.0',
-                        'hjson>=3.0.2',
-                        'PyYaml>=6.0',
-                        'apispec>=6.0.0',
-                        'mnemonic>=0.20',
-                        'PrettyTable>=3.5.0',
-                        'http_sfv>=0.9.8',
-                        'cryptography>=39.0.2'
+                        'jsonschema>=4.21.1',
+                        'falcon>=3.1.3',
+                        'hjson>=3.1.0',
+                        'PyYaml>=6.0.1',
+                        'apispec>=6.6.0',
+                        'mnemonic>=0.21',
+                        'PrettyTable>=3.10.0',
+                        'http_sfv>=0.9.9',
+                        'cryptography>=42.0.5',
+                        'semver>=3.0.2'
     ],
     extras_require={
     },
     tests_require=[
-                    'coverage>=6.5.0',
-                    'pytest>=7.2.0',
+                    'coverage>=7.4.4',
+                    'pytest>=8.1.1',
                     'pytest-shell>=0.3.2'
                   ],
     setup_requires=[
     ],
     entry_points={
         'console_scripts': [
             'keri_bob = keri.demo.demo_bob:main',
```

### Comparing `keri-1.1.9/src/keri/app/agenting.py` & `keri-1.2.dev0/src/keri/app/agenting.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 from urllib.parse import urlparse, urljoin
 
 from hio.base import doing
 from hio.core import http
 from hio.core.tcp import clienting
 from hio.help import decking, Hict
 
+from socket import gaierror
+
 from . import httping, forwarding
 from .. import help
 from .. import kering
-from ..core import eventing, parsing, coring, serdering
+from ..core import eventing, parsing, coring, serdering, indexing
 from ..core.coring import CtrDex
 from ..db import dbing
 from ..kering import Roles
 
 logger = help.ogler.getLogger()
 
 
@@ -70,18 +72,21 @@
             adds = ser.ked["ba"]
             for wit in adds:
                 yield from self.catchup(ser.pre, wit)
 
         clients = dict()
         doers = []
         for wit in wits:
-            client, clientDoer = httpClient(hab, wit)
-            clients[wit] = client
-            doers.append(clientDoer)
-            self.extend([clientDoer])
+            try:
+                client, clientDoer = httpClient(hab, wit)
+                clients[wit] = client
+                doers.append(clientDoer)
+                self.extend([clientDoer])
+            except (kering.MissingEntryError, gaierror) as e:
+                logger.error(f"unable to create http client for witness {wit}: {e}")
 
         rcts = dict()
         for wit, client in clients.items():
             httping.streamCESRRequests(client=client, dest=wit, ims=bytearray(msg), path="/receipts")
             while not client.responses:
                 yield self.tock
 
@@ -94,16 +99,16 @@
 
                 # pull off the count code
                 coring.Counter(qb64b=rct, strip=True)
                 rcts[wit] = rct
             else:
                 logger.error(f"invalid response {rep.status} from witnesses {wit}")
 
-        for wit in rcts.keys():
-            ewits = [w for w in rcts.keys() if w != wit]
+        for wit in rcts:
+            ewits = [w for w in rcts if w != wit]
             wigs = [sig for w, sig in rcts.items() if w != wit]
 
             msg = bytearray()
             if ser.ked['t'] in (coring.Ilks.icp, coring.Ilks.dip):  # introduce new witnesses
                 msg.extend(schemes(self.hby.db, eids=ewits))
             elif ser.ked['t'] in (coring.Ilks.rot, coring.Ilks.drt) and \
                     ("ba" in ser.ked and wit in ser.ked["ba"]):  # Newly added witness, introduce to all
@@ -351,15 +356,15 @@
 
                 # If we started with all our recipts, exit unless told to force resubmit of all receipts
                 if completed and not self.force:
                     self.cues.push(evt)
                     continue
 
                 # generate all rct msgs to send to all witnesses
-                awigers = [coring.Siger(qb64b=bytes(wig)) for wig in wigs]
+                awigers = [indexing.Siger(qb64b=bytes(wig)) for wig in wigs]
 
                 # make sure all witnesses have fully receipted KERL and know about each other
                 for witer in witers:
                     ewits = []
                     wigers = []
                     for i, wit in enumerate(wits):
                         if wit == witer.wit:
@@ -714,15 +719,15 @@
             tock is injected initial tock value
             opts is dict of injected optional additional parameters
 
 
         Usage:
             add result of doify on this method to doers list
         """
-        yield from self.parser.parsator()  # process messages continuously
+        yield from self.parser.parsator(local=True)  # process messages continuously
 
     @property
     def idle(self):
         return len(self.sent) == self.posted
 
 
 class TCPStreamMessenger(doing.DoDoer):
@@ -808,15 +813,15 @@
             tock is injected initial tock value
             opts is dict of injected optional additional parameters
 
 
         Usage:
             add result of doify on this method to doers list
         """
-        yield from self.parser.parsator()  # process messages continuously
+        yield from self.parser.parsator(local=True)  # process messages continuously
 
     @property
     def idle(self):
         return len(self.sent) == self.posted
 
 
 class HTTPMessenger(doing.DoDoer):
```

### Comparing `keri-1.1.9/src/keri/app/apping.py` & `keri-1.2.dev0/src/keri/app/apping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/challenging.py` & `keri-1.2.dev0/src/keri/app/challenging.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/challenge/generate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/challenge/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/challenge/respond.py` & `keri-1.2.dev0/src/keri/app/cli/commands/challenge/respond.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/challenge/verify.py` & `keri-1.2.dev0/src/keri/app/cli/commands/challenge/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/contacts/list.py` & `keri-1.2.dev0/src/keri/app/cli/commands/contacts/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 """
 import argparse
 import json
 
 from hio import help
 from hio.base import doing
+from keri import kering
 
 from keri.app import connecting
 from keri.app.cli.common import existing
 from keri.kering import ConfigurationError
 
 logger = help.ogler.getLogger()
 
@@ -49,16 +50,22 @@
                 aid = c['id']
                 accepted = [saider.qb64 for saider in hby.db.chas.get(keys=(aid,))]
                 received = [saider.qb64 for saider in hby.db.reps.get(keys=(aid,))]
                 valid = set(accepted) & set(received)
 
                 challenges = []
                 for said in valid:
-                    exn = hby.db.exns.get(keys=(said,))
-                    challenges.append(dict(dt=exn.ked['dt'], words=exn.ked['a']['words']))
+                    try:
+                        exn = hby.db.exns.get(keys=(said,))
+                    except kering.ValidationError:
+                        val = hby.db.getVal(db=hby.db.exns.sdb, key=hby.db.exns._tokey((said,)))
+                        d = json.loads(bytes(val).decode("utf-8"))
+                        challenges.append(dict(dt=d['dt'], words=d['a']['words']))
+                    else:
+                        challenges.append(dict(dt=exn.ked['dt'], words=exn.ked['a']['words']))
 
                 c["challenges"] = challenges
 
                 wellKnowns = []
                 wkans = hby.db.wkas.get(keys=(aid,))
                 for wkan in wkans:
                     wellKnowns.append(dict(url=wkan.url, dt=wkan.dt))
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/delegate/confirm.py` & `keri-1.2.dev0/src/keri/app/cli/commands/delegate/confirm.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 if ilk in (coring.Ilks.dip,):
                     typ = "inception"
                     delpre = eserder.sad["di"]
 
                 elif ilk in (coring.Ilks.drt,):
                     typ = "rotation"
                     dkever = self.hby.kevers[eserder.pre]
-                    delpre = dkever.delegator
+                    delpre = dkever.delpre
 
                 else:
                     continue
 
                 if delpre in self.hby.prefixes:
                     hab = self.hby.habs[delpre]
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/delegate/request.py` & `keri-1.2.dev0/src/keri/app/cli/commands/delegate/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,28 +82,28 @@
 
         esc = self.hby.db.gdee.get(keys=(hab.pre,))
         if not esc:
             raise ValueError(f"no escrowed events for {self.alias} ({hab.pre})")
 
         (seqner, saider) = esc[0]
         evt = hab.makeOwnEvent(sn=seqner.sn)
-        delpre = hab.kever.delegator  # get the delegator identifier
+        delpre = hab.kever.delpre  # get the delegator identifier
 
         if isinstance(hab, GroupHab):
             phab = hab.mhab
         else:
             phab = self.hby.habByName(f"{self.alias}-proxy")
 
         exn, atc = delegating.delegateRequestExn(hab.mhab, delpre=delpre, evt=bytes(evt), aids=hab.smids)
 
         # delegate AID ICP and exn of delegation request EXN
         srdr = serdering.SerderKERI(raw=evt) # coring.Serder(raw=evt)
         del evt[:srdr.size]
         self.postman.send(src=phab.pre, dest=delpre, topic="delegate", serder=srdr, attachment=evt)
-        self.postman.send(src=phab.pre, dest=hab.kever.delegator, topic="delegate", serder=exn, attachment=atc)
+        self.postman.send(src=phab.pre, dest=hab.kever.delpre, topic="delegate", serder=exn, attachment=atc)
 
         while True:
             while self.postman.cues:
                 cue = self.postman.cues.popleft()
                 if "said" in cue and cue["said"] == exn.said:
                     print("Delegation request resent")
                     self.remove(self.toRemove)
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/did/generate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/did/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ends/add.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ends/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ends/export.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ends/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ends/list.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ends/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/escrow.py` & `keri-1.2.dev0/src/keri/app/cli/commands/escrow.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/export.py` & `keri-1.2.dev0/src/keri/app/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/incept.py` & `keri-1.2.dev0/src/keri/app/cli/commands/incept.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                                     temp=False,
                                     reopen=True,
                                     clear=False)
         self.endpoint = endpoint
         self.proxy = proxy
         hby = existing.setupHby(name=name, base=base, bran=bran, cf=cf)
         self.hbyDoer = habbing.HaberyDoer(habery=hby)  # setup doer
-        self.swain = delegating.Sealer(hby=hby)
+        self.swain = delegating.Anchorer(hby=hby)
         self.postman = forwarding.Poster(hby=hby)
         self.mbx = indirecting.MailboxDirector(hby=hby, topics=['/receipt', "/replay", "/reply"])
         doers = [self.hbyDoer, self.postman, self.mbx, self.swain, doing.doify(self.inceptDo)]
 
         self.inits = kwa
         self.alias = alias
         self.hby = hby
@@ -164,30 +164,30 @@
         _ = (yield self.tock)
 
         hab = self.hby.makeHab(name=self.alias, **self.inits)
         witDoer = agenting.WitnessReceiptor(hby=self.hby)
         receiptor = agenting.Receiptor(hby=self.hby)
         self.extend([witDoer, receiptor])
 
-        if hab.kever.delegator:
+        if hab.kever.delpre:
             self.swain.delegation(pre=hab.pre, sn=0, proxy=self.hby.habByName(self.proxy))
             print("Waiting for delegation approval...")
             while not self.swain.complete(hab.kever.prefixer, coring.Seqner(sn=hab.kever.sn)):
                 yield self.tock
 
         elif hab.kever.wits:
             print("Waiting for witness receipts...")
             if self.endpoint:
                 yield from receiptor.receipt(hab.pre, sn=0)
             else:
                 witDoer.msgs.append(dict(pre=hab.pre))
                 while not witDoer.cues:
                     _ = yield self.tock
 
-        if hab.kever.delegator:
+        if hab.kever.delpre:
             yield from self.postman.sendEvent(hab=hab, fn=hab.kever.sn)
 
         print(f'Prefix  {hab.pre}')
         for idx, verfer in enumerate(hab.kever.verfers):
             print(f'\tPublic key {idx + 1}:  {verfer.qb64}')
         print()
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/init.py` & `keri-1.2.dev0/src/keri/app/cli/commands/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- encoding: utf-8 -*-
 """
 keri.kli.commands module
 
 """
 import argparse
 import getpass
+import os
+import sys
 
 from hio import help
 from hio.base import doing
 
 import keri.app.oobiing
-from keri.app import habbing, configing, oobiing, connecting
+from keri import kering
+from keri.app import habbing, configing, oobiing
 from keri.app.keeping import Algos
+from keri.db import basing
 from keri.kering import ConfigurationError
 from keri.vdr import credentialing
 
 logger = help.ogler.getLogger()
 
 
 def handler(args):
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/interact.py` & `keri-1.2.dev0/src/keri/app/cli/commands/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/admit.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/admit.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/agree.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/agree.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/grant.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/grant.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/join.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/list.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/offer.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/offer.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ipex/spurn.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ipex/spurn.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/kevers.py` & `keri-1.2.dev0/src/keri/app/cli/commands/kevers.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/list.py` & `keri-1.2.dev0/src/keri/app/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/local/watch.py` & `keri-1.2.dev0/src/keri/app/cli/commands/local/watch.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/mailbox/debug.py` & `keri-1.2.dev0/src/keri/app/cli/commands/mailbox/debug.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/mailbox/update.py` & `keri-1.2.dev0/src/keri/app/cli/commands/mailbox/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/migrate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/migrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,14 +121,23 @@
                 prefixer = coring.Prefixer(qb64=said)
                 seqner = coring.Seqner(sn=0)
                 saider = coring.Saider(qb64b=bytes(dig))
                 rgy.cancs.pin(keys=said, val=[prefixer, seqner, saider])
 
             migrateKeys(hby.db)
 
+            # clear escrows
+            print("clearing escrows")
+            hby.db.gpwe.trim()
+            hby.db.gdee.trim()
+            hby.db.dpwe.trim()
+            hby.db.gpse.trim()
+            hby.db.epse.trim()
+            hby.db.dune.trim()
+
     except ConfigurationError:
         print(f"identifier prefix for {name} does not exist, incept must be run first", )
         return -1
 
 
 def migrateKeys(db):
     # public keys mapped to the AID and event seq no they appeared in
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/continue.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/continue.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         esc = self.hby.db.gdee.get(keys=(hab.pre,))
         if not esc:
             raise ValueError(f"no escrowed events for {self.alias} ({hab.pre})")
 
         (seqner, saider) = esc[0]
         src = hab.mhab.pre if isinstance(hab, GroupHab) else hab.pre
         anchor = dict(i=hab.pre, s=seqner.snh, d=saider.qb64)
-        self.witq.query(src=src, pre=hab.kever.delegator, anchor=anchor)
+        self.witq.query(src=src, pre=hab.kever.delpre, anchor=anchor)
 
         print(f"Checking mailboxes for any events to process")
         while self.hby.db.cgms.get(keys=(hab.pre, seqner.qb64)) is None:
             yield 1.0
 
         print()
         displaying.printIdentifier(self.hby, hab.pre)
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/demo.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/incept.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/incept.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,14 @@
         while True:
             saider = self.hby.db.cgms.get(keys=(prefixer.qb64, seqner.qb64))
             if saider is not None:
                 break
 
             yield self.tock
 
-        if ghab.kever.delegator:
+        if ghab.kever.delpre:
             yield from self.postman.sendEvent(hab=ghab, fn=ghab.kever.sn)
 
         print()
         displaying.printIdentifier(self.hby, ghab.pre)
         self.remove(self.toRemove)
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/interact.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/join.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/join.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,16 +339,16 @@
             m = self.org.get(ked["di"])
             alias = m['alias'] if m else "Unknown Delegator"
             tab.add_row(["Delegator", f"{alias} ({ked['di']}))"])
 
         if not thold.weighted:
             tab.add_row(["Signature Threshold", thold.num])
 
-        tab.add_row(["Establishment Only", eventing.TraitCodex.EstOnly in ked["c"]])
-        tab.add_row(["Do Not Delegate", eventing.TraitCodex.DoNotDelegate in ked["c"]])
+        tab.add_row(["Establishment Only", eventing.TraitDex.EstOnly in ked["c"]])
+        tab.add_row(["Do Not Delegate", eventing.TraitDex.DoNotDelegate in ked["c"]])
         tab.add_row(["Witness Threshold", ked["bt"]])
         tab.add_row(["Witnesses", "\n".join(ked["b"])])
 
         print(tab)
 
     def rotate(self, attrs):
         """ Rotate group multisig
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/notice.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/notice.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/rotate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/rotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,13 +229,13 @@
         while True:
             saider = self.hby.db.cgms.get(keys=(ghab.pre, seqner.qb64))
             if saider is not None:
                 break
 
             yield self.tock
 
-        if ghab.kever.delegator:
+        if ghab.kever.delpre:
             yield from self.postman.sendEvent(hab=ghab, fn=ghab.kever.sn)
 
         print()
         displaying.printIdentifier(self.hby, ghab.pre)
         self.remove(self.toRemove)
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/shell.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/shell.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/multisig/update.py` & `keri-1.2.dev0/src/keri/app/cli/commands/multisig/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,16 @@
                 return
 
             yield self.tock
 
         print("")
 
         witstate = self.hab.db.ksns.get((saider.qb64,))
-        if witstate.sn != self.sn and witstate.ked['d'] != self.said:
-            print(f"Witness state ({witstate.sn}, {witstate.ked['d']}) does not match requested state.")
+        if int(witstate.s, 16) != self.sn and witstate.d != self.said:
+            print(f"Witness state ({witstate.s}, {witstate.d}) does not match requested state.")
             self.remove(self.toRemove)
 
             return
 
         print("Witness at requested state, updating now...")
         self.witq.query(src=self.hab.pre, pre=self.hab.pre, r="logs")
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/oobi/clean.py` & `keri-1.2.dev0/src/keri/app/cli/commands/oobi/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/oobi/generate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/oobi/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/oobi/resolve.py` & `keri-1.2.dev0/src/keri/app/cli/commands/oobi/resolve.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/passcode/generate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/passcode/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/passcode/remove.py` & `keri-1.2.dev0/src/keri/app/cli/commands/passcode/remove.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/passcode/set.py` & `keri-1.2.dev0/src/keri/app/cli/commands/passcode/set.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/query.py` & `keri-1.2.dev0/src/keri/app/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/rename.py` & `keri-1.2.dev0/src/keri/app/cli/commands/rename.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,24 @@
     alias = args.alias
     base = args.base
     bran = args.bran
     newAlias = args.new
 
     try:
         with existing.existingHab(name=name, alias=alias, base=base, bran=bran) as (hby, hab):
-            habord = hab.db.habs.get(keys=alias)
-            hab.db.habs.put(keys=newAlias,
-                            val=habord)
-            hab.db.habs.rem(keys=alias)
+            if hby.habByName(newAlias) is not None:
+                print(f"{newAlias} is already in use")
 
-            print(f"Hab {alias} renamed to {newAlias}")
+            if (pre := hab.db.names.get(keys=("", name))) is not None:
+
+                habord = hab.db.habs.get(keys=pre)
+                habord.name = name
+                hab.db.habs.pin(keys=habord.hid,
+                                val=habord)
+                hab.db.names.pin(keys=("", name), val=pre)
+                hab.db.names.rem(keys=("", alias))
+
+                print(f"Hab {alias} renamed to {newAlias}")
 
     except ConfigurationError as e:
         print(f"identifier prefix for {name} does not exist, incept must be run first", )
         return -1
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/rollback.py` & `keri-1.2.dev0/src/keri/app/cli/commands/rollback.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/rotate.py` & `keri-1.2.dev0/src/keri/app/cli/commands/rotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         self.wits = wits if wits is not None else []
         self.cuts = cuts if cuts is not None else []
         self.adds = adds if adds is not None else []
 
         self.hby = existing.setupHby(name=name, base=base, bran=bran)
         self.hbyDoer = habbing.HaberyDoer(habery=self.hby)  # setup doer
-        self.swain = delegating.Sealer(hby=self.hby)
+        self.swain = delegating.Anchorer(hby=self.hby)
         self.postman = forwarding.Poster(hby=self.hby)
         self.mbx = indirecting.MailboxDirector(hby=self.hby, topics=['/receipt', "/replay", "/reply"])
         doers = [self.hbyDoer, self.mbx, self.swain, self.postman, doing.doify(self.rotateDo)]
 
         super(RotateDoer, self).__init__(doers=doers)
 
     def rotateDo(self, tymth, tock=0.0):
@@ -183,15 +183,15 @@
                 for wit in self.adds:
                     yield from receiptor.catchup(hab.pre, wit)
 
         hab.rotate(isith=self.isith, nsith=self.nsith, ncount=self.count, toad=self.toad,
                    cuts=list(self.cuts), adds=list(self.adds),
                    data=self.data)
 
-        if hab.kever.delegator:
+        if hab.kever.delpre:
             self.swain.delegation(pre=hab.pre, sn=hab.kever.sn, proxy=self.hby.habByName(self.proxy))
             print("Waiting for delegation approval...")
             while not self.swain.complete(hab.kever.prefixer, coring.Seqner(sn=hab.kever.sn)):
                 yield self.tock
 
         elif hab.kever.wits:
             if self.endpoint:
@@ -207,15 +207,15 @@
 
                 witDoer.msgs.append(dict(pre=hab.pre))
                 while not witDoer.cues:
                     _ = yield self.tock
 
                 self.remove([witDoer])
 
-        if hab.kever.delegator:
+        if hab.kever.delpre:
             yield from self.postman.sendEvent(hab=hab, fn=hab.kever.sn)
 
         print(f'Prefix  {hab.pre}')
         print(f'New Sequence No.  {hab.kever.sn}')
         for idx, verfer in enumerate(hab.kever.verfers):
             print(f'\tPublic key {idx + 1}:  {verfer.qb64}')
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/saidify.py` & `keri-1.2.dev0/src/keri/app/cli/commands/saidify.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/salt.py` & `keri-1.2.dev0/src/keri/app/cli/commands/salt.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/sign.py` & `keri-1.2.dev0/src/keri/app/cli/commands/sign.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/ssh/export.py` & `keri-1.2.dev0/src/keri/app/cli/commands/ssh/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/status.py` & `keri-1.2.dev0/src/keri/app/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/create.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/create.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/export.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/list.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/registry/incept.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/incept.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 parser.set_defaults(handler=lambda args: registryIncept(args),
                     transferable=True)
 parser.add_argument('--name', '-n', help='Human readable reference', required=True)
 parser.add_argument('--registry-name', '-r', help='Human readable name for registry, defaults to name of Habitat',
                     default=None)
 parser.add_argument('--nonce', help='Unique random value to seed the credential registry',
                     default=None, required=False)
-parser.add_argument("--no-backers", "-nb", help="do not allow setting up backers different from the ahcnoring KEL "
+parser.add_argument("--no-backers", "-nb", help="do not allow setting up backers different from the anchoring KEL "
                                                 "witnesses", default=True, action="store")
 parser.add_argument('--backers', help='New set of backers different from the anchoring KEL witnesses.  Can '
                                       'appear multiple times', metavar="<prefix>", default=[], action="append",
                     required=False)
 parser.add_argument("--establishment-only", "-eo", help="Only allow establishment events for the anchoring events of "
                                                         "this registry", default=False, action="store")
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/registry/list.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/registry/status.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/registry/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/vc/revoke.py` & `keri-1.2.dev0/src/keri/app/cli/commands/vc/revoke.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/verify.py` & `keri-1.2.dev0/src/keri/app/cli/commands/verify.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import argparse
 
 from hio.base import doing
 
 from keri import kering
 from keri.app.cli.common import existing
-from keri.core import coring
+from keri.core import coring, indexing
 
 parser = argparse.ArgumentParser(description='Verify signature(s) on arbitrary data')
 parser.set_defaults(handler=lambda args: handler(args))
 parser.add_argument('--name', '-n', help='keystore name and file location of KERI keystore', required=True)
 parser.add_argument('--base', '-b', help='additional optional prefix to file location of KERI keystore',
                     required=False, default="")
 parser.add_argument('--alias', '-a', help='human readable alias for the new identifier prefix', required=True)
@@ -45,15 +45,15 @@
     args = opts["args"]
 
     name = args.name
     alias = args.alias
     base = args.base
     bran = args.bran
 
-    sigers = [coring.Siger(qb64=sig) for sig in args.signature]
+    sigers = [indexing.Siger(qb64=sig) for sig in args.signature]
 
     try:
         with existing.existingHab(name=name, alias=alias, base=base, bran=bran) as (_, hab):
 
             kever = hab.kevers[args.prefix]
 
             txt = args.text
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/witness/demo.py` & `keri-1.2.dev0/src/keri/app/cli/commands/witness/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/commands/witness/start.py` & `keri-1.2.dev0/src/keri/app/cli/commands/witness/start.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,19 +45,23 @@
                     default=None,
                     help="configuration filename override")
 parser.add_argument("--keypath", action="store", required=False, default=None)
 parser.add_argument("--certpath", action="store", required=False, default=None)
 parser.add_argument("--cafilepath", action="store", required=False, default=None)
 parser.add_argument("--loglevel", action="store", required=False, default="CRITICAL",
                     help="Set log level to DEBUG | INFO | WARNING | ERROR | CRITICAL. Default is CRITICAL")
+parser.add_argument("--logfile", action="store", required=False, default=None,
+                    help="path of the log file. If not defined, logs will not be written to the file.")
 
 
 def launch(args):
     help.ogler.level = logging.getLevelName(args.loglevel)
-    help.ogler.reopen(name=args.name, temp=True, clear=True)  # need to configure for logging persistent file
+    if(args.logfile != None):
+        help.ogler.headDirPath = args.logfile
+        help.ogler.reopen(name=args.name, temp=False, clear=True)
     logger = help.ogler.getLogger()
 
     logger.info("\n******* Starting Witness for %s listening: http/%s, tcp/%s "
                 ".******\n\n", args.name, args.http, args.tcp)
 
     runWitness(name=args.name,
                base=args.base,
```

### Comparing `keri-1.1.9/src/keri/app/cli/commands/witness/submit.py` & `keri-1.2.dev0/src/keri/app/cli/commands/witness/submit.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/common/config.py` & `keri-1.2.dev0/src/keri/app/cli/common/config.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/common/displaying.py` & `keri-1.2.dev0/src/keri/app/cli/common/displaying.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         seal = hab.db.getAes(dgkey)
 
         print(f"Alias: \t{hab.name}")
         print("{}: {}".format(label, pre))
         print("Seq No:\t{}".format(kever.sner.num))
         if kever.delegated:
             print("Delegated Identifier")
-            sys.stdout.write(f"    Delegator:  {kever.delegator} ")
+            sys.stdout.write(f"    Delegator:  {kever.delpre} ")
             if seal:
                 print(f"{terming.Colors.OKGREEN}{terming.Symbols.CHECKMARK} Anchored{terming.Colors.ENDC}")
             else:
                 print(f"{terming.Colors.FAIL}{terming.Symbols.FAILED} Not Anchored{terming.Colors.ENDC}")
             print()
 
         if isinstance(hab, GroupHab):
@@ -89,15 +89,15 @@
     dgkey = dbing.dgKey(ser.preb, kever.lastEst.d)
     anchor = hby.db.getAes(dgkey)
 
     print("{}: {}".format(label, pre))
     print("Seq No:\t{}".format(kever.sner.num))
     if kever.delegated:
         print("Delegated Identifier")
-        sys.stdout.write(f"    Delegator:  {kever.delegator} ")
+        sys.stdout.write(f"    Delegator:  {kever.delpre} ")
         if anchor:
             print(f"{terming.Colors.OKGREEN}{terming.Symbols.CHECKMARK} Anchored{terming.Colors.ENDC}")
         else:
             print(f"{terming.Colors.FAIL}{terming.Symbols.FAILED} Not Anchored{terming.Colors.ENDC}")
         print()
```

### Comparing `keri-1.1.9/src/keri/app/cli/common/existing.py` & `keri-1.2.dev0/src/keri/app/cli/common/existing.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 import sys
 from contextlib import contextmanager
 
 from keri import kering
 from keri.app import habbing, keeping
 
 
-def setupHby(name, base="", bran=None, cf=None):
+def setupHby(name, base="", bran=None, cf=None, temp=False):
     """ Create Habery off of existing directory
 
     Parameters:
         name(str): name of habitat to create
         base(str): optional base directory prefix
         bran(str): optional passcode if the Habery was created encrypted
         cf (Configer): optional configuration for loading reference data
+        temp (bool): True means create database in /tmp
 
     Returns:
           Habery:  the configured habery
 
     """
     ks = keeping.Keeper(name=name,
                         base=base,
-                        temp=False,
+                        temp=temp,
                         cf=cf,
                         reopen=True)
     aeid = ks.gbls.get('aeid')
     if aeid is None:
         print("Keystore must already exist, exiting")
         sys.exit(-1)
 
@@ -42,15 +43,16 @@
         try:
             if bran:
                 bran = bran.replace("-", "")
 
             retries += 1
             hby = habbing.Habery(name=name, base=base, bran=bran, cf=cf, free=True)
             break
-        except (kering.AuthError, ValueError):
+        except (kering.AuthError, ValueError) as e:
+            print(e)
             if retries >= 3:
                 raise kering.AuthError("too many attempts")
             print("Valid passcode required, try again...")
             bran = getpass.getpass("Passcode: ")
     return hby
```

### Comparing `keri-1.1.9/src/keri/app/cli/common/incepting.py` & `keri-1.2.dev0/src/keri/app/cli/common/incepting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/common/rotating.py` & `keri-1.2.dev0/src/keri/app/cli/common/rotating.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/cli/kli.py` & `keri-1.2.dev0/src/keri/app/cli/kli.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/configing.py` & `keri-1.2.dev0/src/keri/app/configing.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,43 @@
     uses HJSON because HJSON can get (load) a strict json file.
     To use strict json on put (dump) then set .human to false.
 
     See https://github.com/hjson/hjson-py
 
     Attributes:  (see Filer for inherited attributes)
         human (bool): True (default) means use human friendly HJSON when fext is JSON
+
+
+
+    config file  json or hjon
+
+    {
+      "dt": "2021-01-01T00:00:00.000000+00:00",
+      "nel":
+      {
+        "dt": "2021-01-01T00:00:00.000000+00:00",
+        "curls":
+        [
+          "tcp://localhost:5621/"
+        ]
+      },
+      "iurls":
+      [
+        "tcp://localhost:5620/?role=peer&name=tam"
+      ],
+      "durls":
+      [
+        "http://127.0.0.1:7723/oobi/EBNaNu-M9P5cgrnfl2Fvymy4E_jvxxyjb70PRtiANlJy",
+        "http://127.0.0.1:7723/oobi/EMhvwOlyEJ9kN4PrwCpr9Jsv7TxPhiYveZ0oP3lJzdEi",
+      ],
+      "wurls":
+      [
+        "http://127.0.0.1:5644/.well-known/keri/oobi/EBNaNu-M9P5cgrnfl2Fvymy4E_jvxxyjb70PRtiANlJy?name=Root"
+      ]
+    }
     """
     TailDirPath = "keri/cf"
     CleanTailDirPath = "keri/clean/cf"
     AltTailDirPath = ".keri/cf"
     AltCleanTailDirPath = ".keri/clean/cf"
     TempPrefix = "keri_cf_"
```

### Comparing `keri-1.1.9/src/keri/app/connecting.py` & `keri-1.2.dev0/src/keri/app/connecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/delegating.py` & `keri-1.2.dev0/src/keri/app/delegating.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ..core import coring, eventing, serdering
 from ..db import dbing
 from ..peer import exchanging
 
 logger = help.ogler.getLogger()
 
 
-class Sealer(doing.DoDoer):
-    """
+class Anchorer(doing.DoDoer):
+    """Anchorer subclass of DoDoer
     Sends messages to Delegator of an identifier and wait for the anchoring event to
     be processed to ensure the inception or rotation event has been approved by the delegator.
 
     Removes all Doers and exits as Done once the event has been anchored.
 
     """
 
@@ -42,24 +42,24 @@
         """
         self.hby = hby
         self.postman = forwarding.Poster(hby=hby)
         self.witq = agenting.WitnessInquisitor(hby=hby)
         self.witDoer = agenting.Receiptor(hby=self.hby)
         self.proxy = proxy
 
-        super(Sealer, self).__init__(doers=[self.witq, self.witDoer, self.postman, doing.doify(self.escrowDo)],
+        super(Anchorer, self).__init__(doers=[self.witq, self.witDoer, self.postman, doing.doify(self.escrowDo)],
                                      **kwa)
 
     def delegation(self, pre, sn=None, proxy=None):
         if pre not in self.hby.habs:
             raise kering.ValidationError(f"{pre} is not a valid local AID for delegation")
 
         # load the hab of the delegated identifier to anchor
         hab = self.hby.habs[pre]
-        delpre = hab.kever.delegator  # get the delegator identifier
+        delpre = hab.kever.delpre  # get the delegator identifier
         if delpre not in hab.kevers:
             raise kering.ValidationError(f"delegator {delpre} not found, unable to process delegation")
 
         dkever = hab.kevers[delpre]  # and the delegator's kever
         sn = sn if sn is not None else hab.kever.sner.num
 
         # load the event and signatures
@@ -77,15 +77,15 @@
             phab = self.proxy
         else:
             raise kering.ValidationError("no proxy to send messages for delegation")
 
         # Send exn message for notification purposes
         exn, atc = delegateRequestExn(phab, delpre=delpre, evt=bytes(evt), aids=smids)
 
-        self.postman.send(hab=phab, dest=hab.kever.delegator, topic="delegate", serder=exn, attachment=atc)
+        self.postman.send(hab=phab, dest=hab.kever.delpre, topic="delegate", serder=exn, attachment=atc)
 
         srdr = serdering.SerderKERI(raw=evt)
         del evt[:srdr.size]
         self.postman.send(hab=phab, dest=delpre, topic="delegate", serder=srdr, attachment=evt)
 
         seal = dict(i=srdr.pre, s=srdr.snh, d=srdr.said)
         self.witq.query(hab=phab, pre=dkever.prefixer.qb64, anchor=seal)
@@ -147,15 +147,15 @@
         Process escrow of partially signed multisig group KEL events.  Message
         processing will send this local controllers signature to all other participants
         then this escrow waits for signatures from all other participants
 
         """
         for (pre, said), serder in self.hby.db.dune.getItemIter():  # group partial witness escrow
             kever = self.hby.kevers[pre]
-            dkever = self.hby.kevers[kever.delegator]
+            dkever = self.hby.kevers[kever.delpre]
 
             seal = dict(i=serder.pre, s=serder.snh, d=serder.said)
             if dserder := self.hby.db.findAnchoringSealEvent(dkever.prefixer.qb64, seal=seal):
                 seqner = coring.Seqner(sn=dserder.sn)
                 couple = seqner.qb64b + dserder.saidb
                 dgkey = dbing.dgKey(kever.prefixer.qb64b, kever.serder.saidb)
                 self.hby.db.setAes(dgkey, couple)  # authorizer event seal (delegator/issuer)
```

### Comparing `keri-1.1.9/src/keri/app/directing.py` & `keri-1.2.dev0/src/keri/app/directing.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
         Usage:
             add result of doify on this method to doers list
         """
         yield  # enter context
         if self.parser.ims:
             logger.info("Client %s received:\n%s\n...\n", self.hab.name, self.parser.ims[:1024])
-        done = yield from self.parser.parsator()  # process messages continuously
+        done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
 
     def cueDo(self, tymth=None, tock=0.0, **opts):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery.cues deque
@@ -581,15 +581,15 @@
         Usage:
             add result of doify on this method to doers list
         """
         yield  # enter context
         if self.parser.ims:
             logger.info("Server %s: received:\n%s\n...\n", self.hab.name,
                         self.parser.ims[:1024])
-        done = yield from self.parser.parsator()  # process messages continuously
+        done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
 
     def cueDo(self, tymth=None, tock=0.0, **opts):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery.cues deque
```

### Comparing `keri-1.1.9/src/keri/app/forwarding.py` & `keri-1.2.dev0/src/keri/app/forwarding.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         """ Returns generator for sending event and waiting until send is complete """
         # Send KEL event for processing
         icp = self.hby.db.cloneEvtMsg(pre=hab.pre, fn=fn, dig=hab.kever.serder.saidb)
         ser = serdering.SerderKERI(raw=icp)
         del icp[:ser.size]
 
         sender = hab.mhab.pre if isinstance(hab, GroupHab) else hab.pre
-        self.send(src=sender, dest=hab.kever.delegator, topic="delegate", serder=ser, attachment=icp)
+        self.send(src=sender, dest=hab.kever.delpre, topic="delegate", serder=ser, attachment=icp)
         while True:
             if self.cues:
                 cue = self.cues.popleft()
                 if cue["said"] == ser.said:
                     break
                 else:
                     self.cues.append(cue)
```

### Comparing `keri-1.1.9/src/keri/app/grouping.py` & `keri-1.2.dev0/src/keri/app/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
 from hio.base import doing
 from hio.help import decking
 
 from .. import kering
 from .. import help
 from ..app import delegating, agenting
-from ..core import coring, routing, eventing, parsing, serdering
+from ..core import coring, routing, eventing, parsing, serdering, indexing
 from ..db import dbing
 from ..db.dbing import snKey
 from ..peer import exchanging
 
 logger = help.ogler.getLogger()
 
 
 class Counselor(doing.DoDoer):
 
     def __init__(self, hby, swain=None, proxy=None, **kwa):
 
         self.hby = hby
-        self.swain = swain if swain is not None else delegating.Sealer(hby=self.hby)
+        self.swain = swain if swain is not None else delegating.Anchorer(hby=self.hby)
         self.proxy = proxy
         self.witDoer = agenting.Receiptor(hby=self.hby)
         self.witq = agenting.WitnessInquisitor(hby=hby)
 
         doers = [self.swain, self.witq, self.witDoer, doing.doify(self.escrowDo)]
 
         super(Counselor, self).__init__(doers=doers, **kwa)
@@ -120,31 +120,31 @@
                 ghab = self.hby.habs[pre]
                 kever = ghab.kever
                 keys = [verfer.qb64 for verfer in kever.verfers]
                 sigs = self.hby.db.getSigs(dbing.dgKey(pre, bytes(sdig)))
                 if not sigs:  # otherwise its a list of sigs
                     continue
 
-                sigers = [coring.Siger(qb64b=bytes(sig)) for sig in sigs]
+                sigers = [indexing.Siger(qb64b=bytes(sig)) for sig in sigs]
                 windex = min([siger.index for siger in sigers])
 
                 # True if Elected to perform delegation and witnessing
                 witered = ghab.mhab.kever.verfers[0].qb64 == keys[windex]
 
                 if kever.delegated and kever.ilk in (coring.Ilks.dip, coring.Ilks.drt):
                     # We are a delegated identifier, must wait for delegator approval for dip and drt
                     if witered:  # We are elected to perform delegation and witnessing messaging
                         print(f"We are the witnesser, sending {pre} to delegator")
                         self.swain.delegation(pre=pre, sn=seqner.sn)
                     else:
                         anchor = dict(i=pre, s=seqner.snh, d=saider.qb64)
                         if self.proxy:
-                            self.witq.query(hab=self.proxy, pre=kever.delegator, anchor=anchor)
+                            self.witq.query(hab=self.proxy, pre=kever.delpre, anchor=anchor)
                         else:
-                            self.witq.query(src=ghab.mhab.pre, pre=kever.delegator, anchor=anchor)
+                            self.witq.query(src=ghab.mhab.pre, pre=kever.delpre, anchor=anchor)
 
                     print("Waiting for delegation approval...")
                     self.hby.db.gdee.add(keys=(pre,), val=(seqner, saider))
                 else:  # Non-delegation, move on to witnessing
                     if witered:  # We are elected witnesser, send off event to witnesses
                         print(f"We are the fully signed witnesser {seqner.sn}, sending to witnesses")
                         self.witDoer.msgs.append(dict(pre=pre, sn=seqner.sn))
@@ -171,15 +171,15 @@
                 if self.swain.complete(prefixer=kever.prefixer, seqner=coring.Seqner(sn=kever.sn)):
                     self.hby.db.gdee.rem(keys=(pre,))
                     print(f"Delegation approval for {pre} received.")
 
                     self.hby.db.cgms.put(keys=(pre, seqner.qb64), val=saider)
 
             else:  # Not witnesser, we need to look for the anchor and then wait for receipts
-                if serder := self.hby.db.findAnchoringSealEvent(kever.delegator, seal=anchor):
+                if serder := self.hby.db.findAnchoringSealEvent(kever.delpre, seal=anchor):
                     aseq = coring.Seqner(sn=serder.sn)
                     couple = aseq.qb64b + serder.saidb
                     dgkey = dbing.dgKey(pre, saider.qb64b)
                     self.hby.db.setAes(dgkey, couple)  # authorizer event seal (delegator/issuer)
                     self.hby.db.gdee.rem(keys=(pre,))
                     print(f"Delegation approval for {pre} received.")
 
@@ -512,15 +512,15 @@
     dig = bytes(dig)
     key = dbing.dgKey(pre, dig)  # digest key
     msg = db.getEvt(key)
     serder = serdering.SerderKERI(raw=bytes(msg))
 
     sigs = []
     for sig in db.getSigsIter(key):
-        sigs.append(coring.Siger(qb64b=bytes(sig)))
+        sigs.append(indexing.Siger(qb64b=bytes(sig)))
 
     couple = db.getAes(key)
 
     msg = bytearray()
     msg.extend(serder.raw)
     msg.extend(coring.Counter(code=coring.CtrDex.ControllerIdxSigs,
                               count=len(sigs)).qb64b)  # attach cnt
```

### Comparing `keri-1.1.9/src/keri/app/habbing.py` & `keri-1.2.dev0/src/keri/app/habbing.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from hio.base import doing
 from hio.help import hicting
 
 from keri.peer import exchanging
 from . import keeping, configing
 from .. import help
 from .. import kering
-from ..core import coring, eventing, parsing, routing, serdering
+from ..core import coring, eventing, parsing, routing, serdering, indexing
 from ..db import dbing, basing
 from ..kering import MissingSignatureError, Roles
 
 logger = help.ogler.getLogger()
 
 @contextmanager
 def openHby(*, name="test", base="", temp=True, salt=None, **kwa):
@@ -64,26 +64,26 @@
         algo (str): algorithm (randy or salty) for creating key pairs
             default is root algo which defaults to salty
         tier (str): security tier for generating keys from salt (Tierage)
         free (boo): free resources by closing on Doer exit if any
 
     """
     habery = None
-    salt = salt if not None else coring.Salter(raw=b'0123456789abcdef').qb64
+    salt = salt if salt is not None else coring.Salter().qb64
     try:
         habery = Habery(name=name, base=base, temp=temp, salt=salt, **kwa)
         yield habery
 
     finally:
         if habery:
             habery.close(clear=habery.temp)
 
 
 @contextmanager
-def openHab(name="test", base="", salt=b'0123456789abcdef', temp=True, cf=None, **kwa):
+def openHab(name="test", base="", salt=None, temp=True, cf=None, **kwa):
     """
     Context manager wrapper for Hab instance.
     Defaults to temporary resources
     Context 'with' statements call .close on exit of 'with' block
 
     Parameters:
         name(str): name of habitat to create
@@ -125,16 +125,18 @@
         mgr (keeping.Manager): creates and rotates keys in key store
         rtr (routing.Router): routes reply 'rpy' messages
         rvy (routing.Revery): factory that processes reply 'rpy' messages
         kvy (eventing.Kevery): factory for local processing of local event msgs
         psr (parsing.Parser):  parses local messages for .kvy .rvy
 
         habs (dict): Hab instances keyed by prefix.
-            To look up Hab by name get prefix from db.habs .prefix field using
-            .habByName
+            To look up Hab by name use use .habByName
+            To look up Hab by prefix us .habByPrefix
+            to get hab from db need name for key
+            hab prefix in db.habs record .hid field
 
         inited (bool): True means fully initialized wrt databases.
                           False means not yet fully initialized
 
     Properties:
         kevers (dict): of eventing.Kever(s) keyed by qb64 prefix
         prefixes (OrderedSet): local prefixes for .db
@@ -217,28 +219,29 @@
 
         self.mgr = None  # wait to setup until after ks is known to be opened
         self.rtr = routing.Router()
         self.rvy = routing.Revery(db=self.db, rtr=self.rtr)
         self.exc = exchanging.Exchanger(hby=self, handlers=[])
         self.kvy = eventing.Kevery(db=self.db, lax=False, local=True, rvy=self.rvy)
         self.kvy.registerReplyRoutes(router=self.rtr)
-        self.psr = parsing.Parser(framed=True, kvy=self.kvy, rvy=self.rvy, exc=self.exc)
+        self.psr = parsing.Parser(framed=True, kvy=self.kvy, rvy=self.rvy,
+                                  exc=self.exc, local=True)
         self.habs = {}  # empty .habs
-        self.namespaces = {}  # empty .namespaces
         self._signator = None
         self.inited = False
 
         # save init kwy word arg parameters as ._inits in order to later finish
         # init setup elseqhere after databases are opened if not below
         self._inits = kwa
         self._inits['temp'] = temp  # add temp for seed from bran tier override
 
         if self.db.opened and self.ks.opened:
             self.setup(**self._inits)  # finish setup later
 
+
     def setup(self, *, seed=None, aeid=None, bran=None, pidx=None, algo=None,
               salt=None, tier=None, free=False, temp=None, ):
         """
         Setup Habery. Assumes that both .db and .ks have been opened.
         This allows dependency injection of .db and .ks into Habery instance
         prior to .db and .kx being opened to accomodate asynchronous process
         setup of these resources. Putting the .db and .ks associated
@@ -289,15 +292,15 @@
                                                      tier=tier,
                                                      temp=temp)
             seed = signer.qb64
             if not aeid:  # aeid must not be empty event on initial creation
                 aeid = signer.verfer.qb64  # lest it remove encryption
 
         if salt is None:  # salt for signing keys not aeid seed
-            salt = coring.Salter(raw=b'0123456789abcdef').qb64
+            salt = coring.Salter().qb64
         else:
             salt = coring.Salter(qb64=salt).qb64
 
         try:
             self.mgr = keeping.Manager(ks=self.ks, seed=seed, aeid=aeid, pidx=pidx,
                                        algo=algo, salt=salt, tier=tier)
         except kering.AuthError as ex:
@@ -318,87 +321,48 @@
         It also removes any bare .habs without key state
         Thus by now know that .habs are valid so can create Hab instances
 
         """
         self.reconfigure()  # pre hab load reconfiguration
 
         groups = []
-        for name, habord in self.db.habs.getItemIter():
-            name = ".".join(name)  # detupleize the database key name
+        for prefix, habord in self.db.habs.getItemIter():
             pre = habord.hid
 
             # create Hab instance and inject dependencies
             if habord.mid and not habord.sid:
                 hab = GroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                                rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                               name=name, pre=pre, temp=self.temp, smids=habord.smids)
+                               name=habord.name, pre=pre, temp=self.temp, smids=habord.smids)
                 groups.append(habord)
             elif habord.sid and not habord.mid:
                 hab = SignifyHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                                  rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                                 name=name, pre=habord.sid)
+                                 name=habord.name, pre=habord.sid)
             elif habord.sid and habord.mid:
                 hab = SignifyGroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                                       rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                                      name=name, pre=pre)
+                                      name=habord.name, pre=pre)
                 groups.append(habord)
             else:
                 hab = Hab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                           rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                          name=name, pre=pre, temp=self.temp)
+                          name=habord.name, pre=pre, temp=self.temp)
 
-            # Rules for acceptance
-            #  if its delegated its accepted into its own local KEL even if the
-            #    delegator has not sealed it
+            # Rules for acceptance:
+            # It is accepted into its own local KEL even if it has not been fully
+            # witnessed and if delegated, its delegator has not yet sealed it
             if not hab.accepted and not habord.mid:
                 raise kering.ConfigurationError(f"Problem loading Hab pre="
-                                                f"{pre} name={name} from db.")
+                                                f"{pre} name={habord.name} from db.")
 
             # read in config file and process any oobis or endpoints for hab
             hab.inited = True
             self.habs[hab.pre] = hab
 
-        for keys, habord in self.db.nmsp.getItemIter():
-            ns = keys[0]
-            name = ".".join(keys[1:])  # detupleize the database key name
-            pre = habord.hid
-
-            # create Hab instance and inject dependencies
-            if habord.mid and not habord.sid:
-                hab = GroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
-                               rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                               name=name, ns=ns, pre=pre, temp=self.temp, smids=habord.smids)
-                groups.append(habord)
-            elif habord.sid and not habord.mid:
-                hab = SignifyHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
-                                 rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                                 name=name, ns=ns, pre=habord.sid)
-            elif habord.sid and habord.mid:
-                hab = SignifyGroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
-                                      rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                                      name=name, pre=habord.sid)
-                groups.append(habord)
-            else:
-                hab = Hab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
-                          rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                          name=name, ns=ns, pre=pre, temp=self.temp)
-
-            # Rules for acceptance
-            #  if its delegated its accepted into its own local KEL even if the
-            #    delegator has not sealed it
-            if not hab.accepted and not habord.mid:
-                raise kering.ConfigurationError(f"Problem loading Hab pre="
-                                                f"{pre} name={name} from db.")
-
-            # read in config file and process any oobis or endpoints for hab
-            hab.inited = True
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
-
         # Populate the participant hab after loading all habs
         for habord in groups:
             self.habs[habord.hid].mhab = self.habs[habord.mid]
 
         self.reconfigure()  # post hab load reconfiguration
 
     def makeHab(self, name, ns=None, cf=None, **kwa):
@@ -413,35 +377,29 @@
             isith (Union[int, str, list]): incepting signing threshold as int, str hex, or list
             icount (int): incepting key count for number of keys
             nsith (Union[int, str, list]): next signing threshold as int, str hex or list
             ncount (int): next key count for number of next keys
             toad (Union[int,str]): int or str hex of witness threshold
             wits (list): of qb64 prefixes of witnesses
             delpre (str): qb64 of delegator identifier prefix
-            estOnly (str): eventing.TraitCodex.EstOnly means only establishment
+            estOnly (str): eventing.TraitDex.EstOnly means only establishment
                 events allowed in KEL for this Hab
             data (list | None): seal dicts
         """
         if ns is not None and "." in ns:
             raise kering.ConfigurationError("Hab namespace names are not allowed to contain the '.' character")
 
         cf = cf if cf is not None else self.cf
         hab = Hab(ks=self.ks, db=self.db, cf=cf, mgr=self.mgr,
                   rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
                   name=name, ns=ns, temp=self.temp)
 
         hab.make(**kwa)
 
-        if ns is None:
-            self.habs[hab.pre] = hab
-        else:
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
-
+        self.habs[hab.pre] = hab
         return hab
 
     def makeGroupHab(self, group, mhab, smids, rmids=None, ns=None, **kwa):
         """Make new Group Hab using group has group hab name, with lhab as local
         participant.
 
         Parameters: (non-pass-through):
@@ -465,17 +423,17 @@
             isith (Union[int, str, list]): incepting signing threshold as int, str hex, or list
             icount (int): incepting key count for number of keys
             nsith (Union[int, str, list]): next signing threshold as int, str hex or list
             ncount (int): next key count for number of next keys
             toad (Union[int,str]): int or str hex of witness threshold
             wits (list): of qb64 prefixes of witnesses
             delpre (str): qb64 of delegator identifier prefix
-            estOnly (str): eventing.TraitCodex.EstOnly means only establishment
+            estOnly (str): eventing.TraitDex.EstOnly means only establishment
                 events allowed in KEL for this Hab
-            DnD (bool): eventing.TraitCodex.DnD means do allow delegated identifiers from this identifier
+            DnD (bool): eventing.TraitDex.DnD means do allow delegated identifiers from this identifier
 
         ToDo: NRR
         add midxs tuples for each group member or all in group multisig.
 
         """
 
         if mhab.pre not in smids and mhab.pre not in rmids:
@@ -504,21 +462,15 @@
 
         # create group Hab in this Habery
         hab = GroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                        rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
                        name=group, ns=ns, mhab=mhab, smids=smids, rmids=rmids, temp=self.temp)
 
         hab.make(**kwa)  # finish making group hab with injected pass throughs
-        if ns is None:
-            self.habs[hab.pre] = hab
-        else:
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
-
+        self.habs[hab.pre] = hab
         return hab
 
     def joinGroupHab(self, pre, group, mhab, smids, rmids=None, ns=None):
         """Make new Group Hab using group has group hab name, with lhab as local
         participant.
 
         Parameters: (non-pass-through):
@@ -558,61 +510,46 @@
         # create group Hab in this Habery
         hab = GroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                        rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
                        name=group, ns=ns, mhab=mhab, smids=smids, rmids=rmids, temp=self.temp)
 
         hab.pre = pre
         habord = basing.HabitatRecord(hid=hab.pre,
+                                      name=self.name,
+                                      domain=ns,
                                       mid=mhab.pre,
                                       smids=smids,
                                       rmids=rmids)
 
         hab.save(habord)
         hab.prefixes.add(pre)
         hab.inited = True
 
-        if ns is None:
-            self.habs[hab.pre] = hab
-        else:
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
-
+        self.habs[hab.pre] = hab
         return hab
 
     def makeSignifyHab(self, name, ns=None, **kwa):
         # create group Hab in this Habery
         hab = SignifyHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                          rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
                          name=name, ns=ns, temp=self.temp)
 
         hab.make(**kwa)  # finish making group hab with injected pass throughs
-        if ns is None:
-            self.habs[hab.pre] = hab
-        else:
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
-
+        self.habs[hab.pre] = hab
         return hab
 
-    def makeSignifyGroupHab(self, name, mhab, ns=None, **kwa):
+    def makeSignifyGroupHab(self, name, mhab, smids, rmids=None,  ns=None, **kwa):
         # create group Hab in this Habery
         hab = SignifyGroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                               rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                              name=name, mhab=mhab, ns=ns, temp=self.temp)
+                              name=name, mhab=mhab, smids=smids, rmids=rmids, ns=ns, temp=self.temp)
 
         hab.make(**kwa)  # finish making group hab with injected pass throughs
-        if ns is None:
-            self.habs[hab.pre] = hab
-        else:
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
 
+        self.habs[hab.pre] = hab
         return hab
 
     def joinSignifyGroupHab(self, pre, name, mhab, smids, rmids=None, ns=None):
         """Make new Group Hab using group has group hab name, with lhab as local
         participant.
 
         Parameters: (non-pass-through):
@@ -648,45 +585,47 @@
                     raise kering.ConfigurationError(f"KEL missing for next member "
                                                     f"identifier {rmid} in group's"
                                                     f" next members ={rmids}")
 
         # create group Hab in this Habery
         hab = SignifyGroupHab(ks=self.ks, db=self.db, cf=self.cf, mgr=self.mgr,
                               rtr=self.rtr, rvy=self.rvy, kvy=self.kvy, psr=self.psr,
-                              name=name, mhab=mhab, ns=ns, temp=self.temp)
+                              name=name, mhab=mhab, smids=smids, rmids=rmids, ns=ns, temp=self.temp)
 
         hab.pre = pre
         habord = basing.HabitatRecord(hid=hab.pre,
                                       sid=mhab.pre,
+                                      name=name,
+                                      domain=ns,
                                       smids=smids,
                                       rmids=rmids)
 
         hab.save(habord)
         hab.prefixes.add(pre)
         hab.inited = True
 
-        if ns is None:
-            self.habs[hab.pre] = hab
-        else:
-            if ns not in self.namespaces:
-                self.namespaces[ns] = dict()
-            self.namespaces[ns][hab.pre] = hab
-
+        self.habs[hab.pre] = hab
         return hab
 
-    def deleteHab(self, name):
-        hab = self.habByName(name)
+    def deleteHab(self, name, ns=None):
+        hab = self.habByName(name, ns=ns)
         if not hab:
             return False
 
-        if not self.db.habs.rem(keys=(name,)):
+        if not self.db.habs.rem(keys=(hab.pre,)):
+            return False
+
+        ns = "" if ns is None else ns
+        if not self.db.names.rem(keys=(ns, name)):
             return False
 
         del self.habs[hab.pre]
         self.db.prefixes.remove(hab.pre)
+        if hab.pre in self.db.groups:
+            self.db.groups.remove(hab.pre)
 
         return True
 
     def extractMerfersMigers(self, smids, rmids=None):
         """
         Extract the public key verfer and next digest diger from the current
         est event of all the members of the multisig group. Assumes that the KEL
@@ -748,63 +687,78 @@
         """
         Returns .db.prefixes of local prefixes
         """
         return self.db.prefixes
 
     def habByPre(self, pre):
         """
-        Returns the Hab from and namespace including the default namespace.
+        Returns the Hab instance from .habs or None
+        including the default namespace.
 
         Args:
             pre (str): qb64 aid of hab to find
 
         Returns:
             Hab: Hab instance for the aid pre or None
         """
-        hab = None
         if pre in self.habs:
-            hab = self.habs[pre]
-        else:
-            for nsp in self.namespaces.values():
-                if pre in nsp:
-                    hab = nsp[pre]
+            return self.habs[pre]
 
-        return hab
+        return None
 
     def habByName(self, name, ns=None):
         """
         Returns:
-            hab (Hab): instance from .habs by name if any otherwise None
+            hab (Hab): instance by name from .habs or .namspaces
+            if any otherwise None
 
         Parameters:
            name (str): alias of Hab
            ns (str): optional namespace of hab
 
         """
-        if ns is not None:
-            if (habord := self.db.nmsp.get(keys=(ns, name))) is not None:
-                habs = self.namespaces[ns]
-                return habs[habord.hid] if habord.hid in habs else None
-
-        elif (habord := self.db.habs.get(name)) is not None:
-            return self.habs[habord.hid] if habord.hid in self.habs else None
+        ns = "" if ns is None else ns
+        if (pre := self.db.names.get(keys=(ns, name))) is not None:
+            if pre in self.habs:
+                return self.habs[pre]
 
         return None
 
     def reconfigure(self):
         """Apply configuration from config file managed by .cf. to this Habery
         Process any oobis or endpoints
 
-        conf
+        config file  json or hjon
+
         {
-          dt: "isodatetime",
-          curls: ["tcp://localhost:5620/"],
-          iurls: ["tcp://localhost:5621/?name=eve"],
+          "dt": "2021-01-01T00:00:00.000000+00:00",
+          "nel":
+          {
+            "dt": "2021-01-01T00:00:00.000000+00:00",
+            "curls":
+            [
+              "tcp://localhost:5621/"
+            ]
+          },
+          "iurls":
+          [
+            "tcp://localhost:5620/?role=peer&name=tam"
+          ],
+          "durls":
+          [
+            "http://127.0.0.1:7723/oobi/EBNaNu-M9P5cgrnfl2Fvymy4E_jvxxyjb70PRtiANlJy",
+            "http://127.0.0.1:7723/oobi/EMhvwOlyEJ9kN4PrwCpr9Jsv7TxPhiYveZ0oP3lJzdEi",
+          ],
+          "wurls":
+          [
+            "http://127.0.0.1:5644/.well-known/keri/oobi/EBNaNu-M9P5cgrnfl2Fvymy4E_jvxxyjb70PRtiANlJy?name=Root"
+          ]
         }
 
+
         Config file is meant to be read only at init not changed by app at
         run time. Any dynamic app changes must go in database not config file
         that way we don't have to worry about multiple writers of cf.
         Use config file to preload database not as a database. Config file may
         have named sections for Habery or individual Habs as needed.
 
         """
@@ -1022,15 +976,15 @@
         self.mgr = mgr  # injected
         self.rtr = rtr  # injected
         self.rvy = rvy  # injected
         self.kvy = kvy  # injected
         self.psr = psr  # injected
 
         self.name = name
-        self.ns = ns
+        self.ns = ns  # what is this?
         self.pre = pre  # wait to setup until after db is known to be opened
         self.temp = True if temp else False
 
         self.inited = False
         self.delpre = None  # assigned laster if delegated
 
     def make(self, DnD, code, data, delpre, estOnly, isith, verfers, nsith, digers, toad, wits):
@@ -1048,18 +1002,18 @@
                 digers
             verfers (list[Verfer]): Verfer instances for initial signing keys
             digers  (list[Diger] | None) Diger instances for next key digests
             toad (int |str| None): int or str hex of witness threshold if
                 specified else compute default based on number of wits (backers)
             wits (list | None): qb64 prefixes of witnesses if any
             delpre (str | None): qb64 of delegator identifier prefix if any
-            estOnly (bool | None): True means add trait eventing.TraitCodex.EstOnly
+            estOnly (bool | None): True means add trait eventing.TraitDex.EstOnly
                 which means only establishment events allowed in KEL for this Hab
                 False (default) means allows non-est events and no trait is added.
-            DnD (bool): True means add trait of eventing.TraitCodex.DnD which
+            DnD (bool): True means add trait of eventing.TraitDex.DnD which
                     means do not allow delegated identifiers from this identifier
                     False (default) means do allow and no trait is added.
 
             data (list | None): seal dicts
 
         """
         icount = len(verfers)
@@ -1068,17 +1022,17 @@
             isith = f"{max(1, ceil(icount / 2)):x}"
         if nsith is None:  # compute default
             nsith = f"{max(0, ceil(ncount / 2)):x}"
         cst = coring.Tholder(sith=isith).sith  # current signing threshold
         nst = coring.Tholder(sith=nsith).sith  # next signing threshold
         cnfg = []
         if estOnly:
-            cnfg.append(eventing.TraitCodex.EstOnly)
+            cnfg.append(eventing.TraitDex.EstOnly)
         if DnD:
-            cnfg.append(eventing.TraitCodex.DoNotDelegate)
+            cnfg.append(eventing.TraitDex.DoNotDelegate)
         self.delpre = delpre
         keys = [verfer.qb64 for verfer in verfers]
         if self.delpre:
             serder = eventing.delcept(keys=keys,
                                       delpre=self.delpre,
                                       isith=cst,
                                       nsith=nst,
@@ -1096,33 +1050,57 @@
                                      wits=wits,
                                      cnfg=cnfg,
                                      code=code,
                                      data=data)
         return serder
 
     def save(self, habord):
-        if self.ns is None:
-            self.db.habs.pin(keys=self.name,
-                             val=habord)
-        else:
-            self.db.nmsp.put(keys=(self.ns, self.name),
-                             val=habord)
+        self.db.habs.pin(keys=self.pre,
+                         val=habord)
+        ns = "" if self.ns is None else self.ns
+        if self.db.names.get(keys=(ns, self.name)) is not None:
+            raise ValueError("AID already exists with that name")
+
+        self.db.names.pin(keys=(ns, self.name),
+                          val=self.pre)
 
     def reconfigure(self):
         """Apply configuration from config file managed by .cf. to this Hab.
         Assumes that .pre and signing keys have been setup in order to create
         own endpoint auth when provided in .cf.
 
-        conf
+        config file  json or hjon
+
         {
-          dt: "isodatetime",
-          curls: ["tcp://localhost:5620/"],
-          iurls: ["tcp://localhost:5621/?name=eve"]
+          "dt": "2021-01-01T00:00:00.000000+00:00",
+          "nel":
+          {
+            "dt": "2021-01-01T00:00:00.000000+00:00",
+            "curls":
+            [
+              "tcp://localhost:5621/"
+            ]
+          },
+          "iurls":
+          [
+            "tcp://localhost:5620/?role=peer&name=tam"
+          ],
+          "durls":
+          [
+            "http://127.0.0.1:7723/oobi/EBNaNu-M9P5cgrnfl2Fvymy4E_jvxxyjb70PRtiANlJy",
+            "http://127.0.0.1:7723/oobi/EMhvwOlyEJ9kN4PrwCpr9Jsv7TxPhiYveZ0oP3lJzdEi",
+          ],
+          "wurls":
+          [
+            "http://127.0.0.1:5644/.well-known/keri/oobi/EBNaNu-M9P5cgrnfl2Fvymy4E_jvxxyjb70PRtiANlJy?name=Root"
+          ]
         }
 
+
+
         Config file is meant to be read only at init not changed by app at
         run time. Any dynamic app changes must go in database not config file
         that way we don't have to worry about multiple writers of cf.
         Use config file to preload database not as a database. Config file may
         have named sections for Habery or individual Habs as needed.
         """
 
@@ -1235,15 +1213,15 @@
             pdigs = [coring.Diger(ser=verfer.qb64b, code=diger.code).qb64 for verfer in verfers]
             if diger.qb64 in pdigs:
                 indices.append(idx)
 
         if not kever.ntholder.satisfy(indices):
             raise kering.ValidationError("invalid rotation, new key set unable to satisfy prior next signing threshold")
 
-        if kever.delegator is not None:  # delegator only shows up in delcept
+        if kever.delpre is not None:  # delegator only shows up in delcept
             serder = eventing.deltate(pre=kever.prefixer.qb64,
                                       keys=keys,
                                       dig=kever.serder.said,
                                       sn=kever.sner.num + 1,
                                       isith=cst,
                                       nsith=nst,
                                       ndigs=[diger.qb64 for diger in digers],
@@ -1489,16 +1467,18 @@
 
     def witness(self, serder):
         """
         Returns own receipt, rct, message of serder with count code and witness
         indexed receipt signatures if key state of serder.pre shows that own pre
         is a current witness of event in serder
 
-        Before calling this must check that serder being witnessed has been
-        accepted as valid event into controller's KEL
+        ToDo XXXX add parameter to force check that serder as been accepted
+        as valid. Otherwise must assume that before calling this that serder
+        being witnessed has been accepted as valid event into this hab
+        controller's KEL
 
         """
         if self.kever.prefixer.transferable:  # not non-transferable prefix
             raise ValueError("Attempt to create witness receipt with"
                              " transferable pre={}.".format(self.pre))
         ked = serder.ked
 
@@ -2027,15 +2007,15 @@
         dig = bytes(dig)
         key = dbing.dgKey(self.pre, dig)  # digest key
         msg = self.db.getEvt(key)
         serder = serdering.SerderKERI(raw=bytes(msg))
 
         sigs = []
         for sig in self.db.getSigsIter(key):
-            sigs.append(coring.Siger(qb64b=bytes(sig)))
+            sigs.append(indexing.Siger(qb64b=bytes(sig)))
 
         couple = self.db.getAes(key)
 
         return serder, sigs, couple
 
     def makeOwnEvent(self, sn, allowPartiallySigned=False):
         """
@@ -2140,14 +2120,15 @@
             # ToDo XXXX cue for kin = "noticeBadCloneFN"
             # ToDo XXXX cue for kin = "approveDelegation" own is delegator
 
             # ToDo XXXX cue for kin = "keyStateSaved"
             # ToDo XXXX cue for kin = "psUnescrow"
             # ToDo XXXX cue for kin = "stream"
             # ToDo XXXX cue for kin = "invalid"
+            # ToDo XXXX cue for kin=""remoteMemberedSig""
 
 
     def witnesser(self):
         return True
 
 
 class Hab(BaseHab):
@@ -2222,18 +2203,18 @@
                 str hex or list weighted if any, otherwise compute default from
                 digers
             ncount (int | None): next key count for number of next keys
             toad (int |str| None): int or str hex of witness threshold if
                 specified else compute default based on number of wits (backers)
             wits (list | None): qb64 prefixes of witnesses if any
             delpre (str | None): qb64 of delegator identifier prefix if any
-            estOnly (bool | None): True means add trait eventing.TraitCodex.EstOnly
+            estOnly (bool | None): True means add trait eventing.TraitDex.EstOnly
                 which means only establishment events allowed in KEL for this Hab
                 False (default) means allows non-est events and no trait is added.
-            DnD (bool): True means add trait of eventing.TraitCodex.DnD which
+            DnD (bool): True means add trait of eventing.TraitDex.DnD which
                     means do not allow delegated identifiers from this identifier
                     False (default) means do allow and no trait is added.
 
             hidden (bool): A hidden Hab is not included in the list of Habs.
             data (list | None): seal dicts
                         algo is str key creation algorithm code
             salt(str): qb64 salt for randomization when salty algorithm used
@@ -2289,15 +2270,15 @@
 
         self.pre = serder.ked["i"]  # new pre
 
         opre = verfers[0].qb64  # default zeroth original pre from key store
         self.mgr.move(old=opre, new=self.pre)  # move to incept event pre
 
         # may want db method that updates .habs. and .prefixes together
-        habord = basing.HabitatRecord(hid=self.pre)
+        habord = basing.HabitatRecord(hid=self.pre, name=self.name, domain=self.ns)
 
         if not hidden:
             self.save(habord)
             self.prefixes.add(self.pre)
 
         # sign handles group hab with .mhab case
         sigers = self.sign(ser=serder.raw, verfers=verfers)
@@ -2377,15 +2358,15 @@
 
     def make(self, *, serder, sigers, **kwargs):
         self.pre = serder.ked["i"]  # new pre
         self.prefixes.add(self.pre)
 
         self.processEvent(serder, sigers)
 
-        habord = basing.HabitatRecord(hid=self.pre, sid=self.pre)
+        habord = basing.HabitatRecord(hid=self.pre, sid=self.pre, name=self.name, domain=self.ns)
         self.save(habord)
 
         self.inited = True
 
     def sign(self, ser, verfers=None, indexed=True, indices=None, ondices=None, **kwa):
         """Sign given serialization ser using appropriate keys.
         Use provided verfers or .kever.verfers to lookup keys to sign.
@@ -2526,25 +2507,29 @@
                 msgs.extend(self.loadLocScheme(eid=eid, scheme=scheme))
                 msgs.extend(self.loadEndRole(cid=cid, eid=eid, role=erole))
 
         return msgs
 
 
 class SignifyGroupHab(SignifyHab):
-    def __init__(self, mhab=None, **kwa):
+    def __init__(self, smids, mhab=None, rmids=None, **kwa):
         self.mhab = mhab
+        self.smids = smids  # group signing member aids in this group hab
+        self.rmids = rmids or smids # group rotating member aids in this group hab
+
         super(SignifyGroupHab, self).__init__(**kwa)
 
     def make(self, *, serder, sigers, **kwargs):
         self.pre = serder.ked["i"]  # new pre
         self.prefixes.add(self.pre)
 
         self.processEvent(serder, sigers)
 
-        habord = basing.HabitatRecord(hid=self.pre, mid=self.mhab.pre, sid=self.pre)
+        habord = basing.HabitatRecord(hid=self.pre, mid=self.mhab.pre, smids=self.smids, rmids=self.rmids,
+                                      sid=self.pre, name=self.name, domain=self.ns)
         self.save(habord)
 
         self.inited = True
 
     def processEvent(self, serder, sigers):
         """ Process event with signatures ignoring missing signature exceptions
 
@@ -2562,14 +2547,28 @@
             self.kvy.processEvent(serder=serder, sigers=sigers)
         except MissingSignatureError:
             pass
         except Exception:
             raise kering.ValidationError(f"Improper Habitat event type={serder.ked['t']} for "
                                          f"pre={self.pre}.")
 
+    def rotate(self, *, smids=None, rmids=None, serder=None, sigers=None, **kwargs):
+
+        if (habord := self.db.habs.get(keys=(self.pre,))) is None:
+            raise kering.ValidationError(f"Missing HabitatRecord for pre={self.pre}")
+
+        super(SignifyGroupHab, self).rotate(serder=serder, sigers=sigers, **kwargs)
+
+        self.smids = smids
+        self.rmids = rmids
+        habord.smids = smids
+        habord.rmids = rmids
+
+        self.db.habs.pin(keys=(self.pre,), val=habord)
+
 
 class GroupHab(BaseHab):
     """
     Hab class provides a given idetnifier controller's local resource environment
     i.e. hab or habitat. Includes dependency injection of database, keystore,
     configuration file as well as Kevery and key store Manager.
 
@@ -2643,15 +2642,15 @@
             temp (bool): True means testing:
                 use weak level when salty algo for stretching in key creation
                 for incept and rotate of keys for this hab.pre
 
         """
         self.mhab = mhab  # local participant Hab of this group hab
         self.smids = smids  # group signing member aids in this group hab
-        self.rmids = rmids  # group rotating member aids in this group hab
+        self.rmids = rmids or smids  # group rotating member aids in this group hab
 
         super(GroupHab, self).__init__(**kwa)
 
     def make(self, *, code=coring.MtrDex.Blake3_256, transferable=True, isith=None, nsith=None,
              toad=None, wits=None, delpre=None, estOnly=False, DnD=False,
              merfers, migers=None, data=None):
         """
@@ -2668,18 +2667,18 @@
             nsith (int, str, list | None ): next signing threshold as int,
                 str hex or list weighted if any, otherwise compute default from
                 digers
             toad (int |str| None): int or str hex of witness threshold if
                 specified else compute default based on number of wits (backers)
             wits (list | None): qb64 prefixes of witnesses if any
             delpre (str | None): qb64 of delegator identifier prefix if any
-            estOnly (bool | None): True means add trait eventing.TraitCodex.EstOnly
+            estOnly (bool | None): True means add trait eventing.TraitDex.EstOnly
                 which means only establishment events allowed in KEL for this Hab
                 False (default) means allows non-est events and no trait is added.
-            DnD (bool): True means add trait of eventing.TraitCodex.DnD which
+            DnD (bool): True means add trait of eventing.TraitDex.DnD which
                     means do not allow delegated identifiers from this identifier
                     False (default) means do allow and no trait is added.
             merfers (list[Verfer] | None): group member Verfer instances of
                     public keys qb64
                     one collected from each multisig group member
             migers (list[Diger] | None): group member Diger instances of public
                     next key digests qb64
@@ -2724,41 +2723,52 @@
             pass
         except Exception as ex:
             raise kering.ConfigurationError("Improper Habitat inception for "
                                             "pre={} {}".format(self.pre, ex))
 
         habord = basing.HabitatRecord(hid=self.pre,
                                       mid=self.mhab.pre,
+                                      name=self.name,
+                                      domain=self.ns,
                                       smids=self.smids,
                                       rmids=self.rmids)
 
         self.save(habord)
         self.prefixes.add(self.pre)
 
         self.inited = True
 
-    def rotate(self, serder=None, **kwargs):
+    def rotate(self, smids=None, rmids=None, serder=None, **kwargs):
 
         if serder is None:
             return super(GroupHab, self).rotate(**kwargs)
 
+        if (habord := self.db.habs.get(keys=(self.pre,))) is None:
+            raise kering.ValidationError(f"Missing HabitatRecord for pre={self.pre}")
+
         # sign handles group hab with .mhab case
         sigers = self.sign(ser=serder.raw, verfers=serder.verfers, rotated=True)
 
         # update own key event verifier state
         msg = eventing.messagize(serder, sigers=sigers)
 
         try:
             self.kvy.processEvent(serder=serder, sigers=sigers)
         except MissingSignatureError:
             pass
         except Exception as ex:
             raise kering.ValidationError("Improper Habitat rotation for "
                                          "pre={self.pre}.") from ex
 
+        self.smids = smids
+        self.rmids = rmids
+        habord.smids = smids
+        habord.rmids = rmids
+        self.db.habs.pin(keys=(self.pre,), val=habord)
+
         return msg
 
     def sign(self, ser, verfers=None, indexed=True, rotated=False, indices=None, ondices=None):
         """ Sign given serialization ser using appropriate keys.
 
         Walk .mhab's kel to find latest contribution of signing key material to group
         in order to sign properly. Contributions to group key material always use the
@@ -2876,12 +2886,12 @@
         """
         kever = self.kever
         keys = [verfer.qb64 for verfer in kever.verfers]
         sigs = self.db.getSigs(dbing.dgKey(self.pre, kever.serder.saidb))
         if not sigs:  # otherwise its a list of sigs
             return False
 
-        sigers = [coring.Siger(qb64b=bytes(sig)) for sig in sigs]
+        sigers = [indexing.Siger(qb64b=bytes(sig)) for sig in sigs]
         windex = min([siger.index for siger in sigers])
 
         # True if Elected to perform delegation and witnessing
         return self.mhab.kever.verfers[0].qb64 == keys[windex]
```

### Comparing `keri-1.1.9/src/keri/app/httping.py` & `keri-1.2.dev0/src/keri/app/httping.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     Returns
        int: Number of individual requests posted
 
     """
     path = path if path is not None else "/"
 
-    cold = parsing.Parser.sniff(ims)  # check for spurious counters at front of stream
+    cold = kering.sniff(ims)  # check for spurious counters at front of stream
     if cold in (parsing.Colds.txt, parsing.Colds.bny):  # not message error out to flush stream
         # replace with pipelining here once CESR message format supported.
         raise kering.ColdStartError("Expecting message counter tritet={}"
                                     "".format(cold))
 
     # Otherwise its a message cold start
     cnt = 0
```

### Comparing `keri-1.1.9/src/keri/app/indirecting.py` & `keri-1.2.dev0/src/keri/app/indirecting.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         """
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         if self.parser.ims:
             logger.info("Client %s received:\n%s\n...\n", self.kvy, self.parser.ims[:1024])
-        done = yield from self.parser.parsator()  # process messages continuously
+        done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
     def escrowDo(self, tymth=None, tock=0.0):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery and .tevery escrows.
 
@@ -378,15 +378,15 @@
         """
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
         if self.parser.ims:
             logger.info("Client %s received:\n%s\n...\n", self.hab.pre, self.parser.ims[:1024])
-        done = yield from self.parser.parsator()  # process messages continuously
+        done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
     def cueDo(self, tymth=None, tock=0.0):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery.cues deque
 
@@ -669,15 +669,15 @@
         Usage:
             add result of doify on this method to doers list
         """
         self.wind(tymth)
         self.tock = tock
         _ = (yield self.tock)
 
-        done = yield from self.parser.parsator()  # process messages continuously
+        done = yield from self.parser.parsator(local=True)  # process messages continuously
         return done  # should nover get here except forced close
 
     def escrowDo(self, tymth=None, tock=0.0):
         """
          Returns doifiable Doist compatibile generator method (doer dog) to process
             .kevery escrows.
 
@@ -1068,15 +1068,15 @@
         ilk = serder.ked["t"]
         if ilk not in (Ilks.icp, Ilks.rot, Ilks.ixn, Ilks.dip, Ilks.drt):
             raise falcon.HTTPBadRequest(description=f"invalid event type ({ilk})for receipting")
 
         msg = bytearray(serder.raw)
         msg.extend(cr.attachments.encode("utf-8"))
 
-        self.psr.parseOne(ims=msg)
+        self.psr.parseOne(ims=msg, local=True)
 
         if pre in self.hab.kevers:
             kever = self.hab.kevers[pre]
             wits = kever.wits
 
             if self.hab.pre not in wits:
                 raise falcon.HTTPBadRequest(description=f"{self.hab.pre} is not a valid witness for {pre} event at "
```

### Comparing `keri-1.1.9/src/keri/app/keeping.py` & `keri-1.2.dev0/src/keri/app/keeping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/notifying.py` & `keri-1.2.dev0/src/keri/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/oobiing.py` & `keri-1.2.dev0/src/keri/app/oobiing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/querying.py` & `keri-1.2.dev0/src/keri/app/querying.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/signaling.py` & `keri-1.2.dev0/src/keri/app/signaling.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/signing.py` & `keri-1.2.dev0/src/keri/app/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/specing.py` & `keri-1.2.dev0/src/keri/app/specing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/app/storing.py` & `keri-1.2.dev0/src/keri/app/storing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/core/coring.py` & `keri-1.2.dev0/src/keri/core/coring.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 """
 keri.core.coring module
 
 """
 import re
 import json
 from typing import Union
-from collections.abc import Iterable
-
-from dataclasses import dataclass, astuple
 from collections import namedtuple, deque
+from collections.abc import Sequence, Mapping
+from dataclasses import dataclass, astuple
 from base64 import urlsafe_b64encode as encodeB64
 from base64 import urlsafe_b64decode as decodeB64
 from fractions import Fraction
 
 import cbor2 as cbor
 import msgpack
 import pysodium
@@ -21,50 +20,45 @@
 import hashlib
 
 from cryptography import exceptions
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 from cryptography.hazmat.primitives.asymmetric import ec, utils
 
-from ..kering import (EmptyMaterialError, RawMaterialError, InvalidCodeError,
+from ..kering import MaxON
+
+from ..kering import (EmptyMaterialError, RawMaterialError, SoftMaterialError,
+                      InvalidCodeError, InvalidSoftError,
+                      InvalidSizeError,
                       InvalidCodeSizeError, InvalidVarIndexError,
                       InvalidVarSizeError, InvalidVarRawSizeError,
                       ConversionError, InvalidValueError, InvalidTypeError,
                       ValidationError, VersionError, DerivationError,
                       EmptyListError,
                       ShortageError, UnexpectedCodeError, DeserializeError,
                       UnexpectedCountCodeError, UnexpectedOpCodeError)
-from ..kering import (Versionage, Version, VERRAWSIZE, VERFMT, VERFULLSIZE,
-                      versify, deversify, Rever)
-from ..kering import Serials, Serialage, Protos, Protocolage, Ilkage, Ilks
-from ..kering import (ICP_LABELS, DIP_LABELS, ROT_LABELS, DRT_LABELS, IXN_LABELS,
-                      RPY_LABELS)
-from ..kering import (VCP_LABELS, VRT_LABELS, ISS_LABELS, BIS_LABELS, REV_LABELS,
-                      BRV_LABELS, TSN_LABELS, CRED_TSN_LABELS)
+from ..kering import (Versionage, Version, Vrsn_1_0, Vrsn_2_0,
+                      VERRAWSIZE, VERFMT, MAXVERFULLSPAN,
+                      versify, deversify, Rever, smell)
+from ..kering import (Serials, Serialage, Protocols, Protocolage, Ilkage, Ilks,
+                      TraitDex, )
 
 from ..help import helping
-from ..help.helping import sceil, nonStringIterable
+from ..help.helping import sceil, nonStringIterable, nonStringSequence
+from ..help.helping import (intToB64, intToB64b, b64ToInt, B64_CHARS,
+                            codeB64ToB2, codeB2ToB64, Reb64, nabSextets)
 
-
-Labels = Ilkage(icp=ICP_LABELS, rot=ROT_LABELS, ixn=IXN_LABELS, dip=DIP_LABELS,
-                drt=DRT_LABELS, rct=[], qry=[], rpy=RPY_LABELS,
-                exn=[], pro=[], bar=[],
-                vcp=VCP_LABELS, vrt=VRT_LABELS, iss=ISS_LABELS, rev=REV_LABELS,
-                bis=BIS_LABELS, brv=BRV_LABELS)
+from . import indexing
 
 
 DSS_SIG_MODE = "fips-186-3"
 ECDSA_256r1_SEEDBYTES = 32
 ECDSA_256k1_SEEDBYTES = 32
 
 
-Vstrings = Serialage(json=versify(kind=Serials.json, size=0),
-                     mgpk=versify(kind=Serials.mgpk, size=0),
-                     cbor=versify(kind=Serials.cbor, size=0))
-
 # SAID field labels
 Saidage = namedtuple("Saidage", "dollar at id_ i d")
 
 Saids = Saidage(dollar="$id", at="@id", id_="id", i="i", d="d")
 
 def sizeify(ked, kind=None, version=Version):
     """
@@ -87,15 +81,15 @@
 
     Assumes only supports Version
     """
     if "v" not in ked:
         raise ValueError("Missing or empty version string in key event "
                          "dict = {}".format(ked))
 
-    proto, vrsn, knd, size = deversify(ked["v"])  # extract kind and version
+    proto, vrsn, knd, size, _ = deversify(ked["v"])  # extract kind and version
     if vrsn != version:
         raise ValueError("Unsupported version = {}.{}".format(vrsn.major,
                                                               vrsn.minor))
 
     if not kind:
         kind = knd
 
@@ -107,166 +101,24 @@
 
     match = Rever.search(raw)  # Rever's regex takes bytes
     if not match or match.start() > 12:
         raise ValueError("Invalid version string in raw = {}".format(raw))
 
     fore, back = match.span()  # full version string
     # update vs with latest kind version size
-    vs = versify(proto=proto, version=vrsn, kind=kind, size=size)
+    vs = versify(protocol=proto, version=vrsn, kind=kind, size=size)
     # replace old version string in raw with new one
     raw = b'%b%b%b' % (raw[:fore], vs.encode("utf-8"), raw[back:])
     if size != len(raw):  # substitution messed up
         raise ValueError("Malformed version string size = {}".format(vs))
     ked["v"] = vs  # update ked
 
     return raw, proto, kind, ked, vrsn
 
 
-# Base64 utilities
-BASE64_PAD = b'='
-
-# Mappings between Base64 Encode Index and Decode Characters
-#  B64ChrByIdx is dict where each key is a B64 index and each value is the B64 char
-#  B64IdxByChr is dict where each key is a B64 char and each value is the B64 index
-# Map Base64 index to char
-B64ChrByIdx = dict((index, char) for index, char in enumerate([chr(x) for x in range(65, 91)]))
-B64ChrByIdx.update([(index + 26, char) for index, char in enumerate([chr(x) for x in range(97, 123)])])
-B64ChrByIdx.update([(index + 52, char) for index, char in enumerate([chr(x) for x in range(48, 58)])])
-B64ChrByIdx[62] = '-'
-B64ChrByIdx[63] = '_'
-# Map char to Base64 index
-B64IdxByChr = {char: index for index, char in B64ChrByIdx.items()}
-B64_CHARS = tuple(B64ChrByIdx.values())  # tuple of characters in Base64
-
-B64REX = b'^[A-Za-z0-9\-\_]*\Z'
-Reb64 = re.compile(B64REX)  # compile is faster
-
-
-def intToB64(i, l=1):
-    """
-    Returns conversion of int i to Base64 str
-    l is min number of b64 digits left padded with Base64 0 == "A" char
-    """
-    d = deque()  # deque of characters base64
-
-    while l:
-        d.appendleft(B64ChrByIdx[i % 64])
-        i = i // 64
-        if not i:
-            break
-        # d.appendleft(B64ChrByIdx[i % 64])
-        # i = i // 64
-    for j in range(l - len(d)):  # range(x)  x <= 0 means do not iterate
-        d.appendleft("A")
-    return ("".join(d))
-
-
-def intToB64b(i, l=1):
-    """
-    Returns conversion of int i to Base64 bytes
-    l is min number of b64 digits left padded with Base64 0 == "A" char
-    """
-    return (intToB64(i=i, l=l).encode("utf-8"))
-
-
-def b64ToInt(s):
-    """
-    Returns conversion of Base64 str s or bytes to int
-    """
-    if not s:
-        raise ValueError("Empty string, conversion undefined.")
-    if hasattr(s, 'decode'):
-        s = s.decode("utf-8")
-    i = 0
-    for e, c in enumerate(reversed(s)):
-        i |= B64IdxByChr[c] << (e * 6)  # same as i += B64IdxByChr[c] * (64 ** e)
-    return i
-
-
-def codeB64ToB2(s):
-    """
-    Returns conversion (decode) of Base64 chars to Base2 bytes.
-    Where the number of total bytes returned is equal to the minimun number of
-    octets sufficient to hold the total converted concatenated sextets from s,
-    with one sextet per each Base64 decoded char of s. Assumes no pad chars in s.
-    Sextets are left aligned with pad bits in last (rightmost) byte.
-    This is useful for decoding as bytes, code characters from the front of
-    a Base64 encoded string of characters.
-    """
-    i = b64ToInt(s)
-    i <<= 2 * (len(s) % 4)  # add 2 bits right zero padding for each sextet
-    n = sceil(len(s) * 3 / 4)  # compute min number of ocetets to hold all sextets
-    return (i.to_bytes(n, 'big'))
-
-
-def codeB2ToB64(b, l):
-    """
-    Returns conversion (encode) of l Base2 sextets from front of b to Base64 chars.
-    One char for each of l sextets from front (left) of b.
-    This is useful for encoding as code characters, sextets from the front of
-    a Base2 bytes (byte string). Must provide l because of ambiguity between l=3
-    and l=4. Both require 3 bytes in b.
-    """
-    if hasattr(b, 'encode'):
-        b = b.encode("utf-8")  # convert to bytes
-    n = sceil(l * 3 / 4)  # number of bytes needed for l sextets
-    if n > len(b):
-        raise ValueError("Not enough bytes in {} to nab {} sextets.".format(b, l))
-    i = int.from_bytes(b[:n], 'big')  # convert only first n bytes to int
-    # check if prepad bits are zero
-    tbs = 2 * (l % 4)  # trailing bit size in bits
-    i >>= tbs  # right shift out trailing bits to make right aligned
-    return (intToB64(i, l))  # return as B64
-
-
-def nabSextets(b, l):
-    """
-    Return first l sextets from front (left) of b as bytes (byte string).
-    Length of bytes returned is minimum sufficient to hold all l sextets.
-    Last byte returned is right bit padded with zeros
-    b is bytes or str
-    """
-    if hasattr(b, 'encode'):
-        b = b.encode("utf-8")  # convert to bytes
-    n = sceil(l * 3 / 4)  # number of bytes needed for l sextets
-    if n > len(b):
-        raise ValueError("Not enough bytes in {} to nab {} sextets.".format(b, l))
-    i = int.from_bytes(b[:n], 'big')
-    p = 2 * (l % 4)
-    i >>= p  # strip of last bits
-    i <<= p  # pad with empty bits
-    return (i.to_bytes(n, 'big'))
-
-MINSNIFFSIZE = 12 + VERFULLSIZE  # min bytes in buffer to sniff else need more
-
-def sniff(raw):
-    """
-    Returns serialization kind, version and size from serialized event raw
-    by investigating leading bytes that contain version string
-
-    Parameters:
-      raw is bytes of serialized event
-
-    """
-    if len(raw) < MINSNIFFSIZE:
-        raise ShortageError("Need more bytes.")
-
-    match = Rever.search(raw)  # Rever's regex takes bytes
-    if not match or match.start() > 12:
-        raise VersionError("Invalid version string in raw = {}".format(raw))
-
-    proto, major, minor, kind, size = match.group("proto", "major", "minor", "kind", "size")
-    version = Versionage(major=int(major, 16), minor=int(minor, 16))
-    kind = kind.decode("utf-8")
-    proto = proto.decode("utf-8")
-    if kind not in Serials:
-        raise DeserializeError("Invalid serialization kind = {}".format(kind))
-    size = int(size, 16)
-
-    return proto, kind, version, size
 
 
 def dumps(ked, kind=Serials.json):
     """
     utility function to handle serialization by kind
 
     Returns:
@@ -327,73 +179,65 @@
     else:
         raise DeserializeError("Invalid deserialization kind: {}"
                                    "".format(kind))
 
     return ked
 
 
-def generateSigners(salt=None, count=8, transferable=True):
-    """
-    Returns list of Signers for Ed25519
+def generateSigners(raw=None, count=8, transferable=True):
+    """Returns list of Signers for Ed25519
+
+    Deprecated, use Salter.signers instead.
+
+    Use this when simply need valid AIDs but not when need valid controller
+    contexts. In the latter case use openHby or openHab which create databases.
 
     Parameters:
-        salt is bytes 16 byte long root cryptomatter from which seeds for Signers
-            in list are derived
+        raw (bytes):  16 byte long salt cryptomatter from which seeds
+            for Signers in list are derived
             random salt created if not provided
         count is number of signers in list
         transferable is boolean true means signer.verfer code is transferable
                                 non-transferable otherwise
     """
-    if not salt:
-        salt = pysodium.randombytes(pysodium.crypto_pwhash_SALTBYTES)
+    if not raw:
+        raw = pysodium.randombytes(pysodium.crypto_pwhash_SALTBYTES)
 
     signers = []
     for i in range(count):
         path = f"{i:x}"
         # algorithm default is argon2id
         seed = pysodium.crypto_pwhash(outlen=32,
                                       passwd=path,
-                                      salt=salt,
+                                      salt=raw,
                                       opslimit=2,  # pysodium.crypto_pwhash_OPSLIMIT_INTERACTIVE,
                                       memlimit=67108864,  # pysodium.crypto_pwhash_MEMLIMIT_INTERACTIVE,
                                       alg=pysodium.crypto_pwhash_ALG_ARGON2ID13)
 
         signers.append(Signer(raw=seed, transferable=transferable))
 
     return signers
 
 
-def generatePrivates(salt=None, count=8):
-    """
-    Returns list of fully qualified Base64 secret Ed25519 seeds  i.e private keys
-
-    Parameters:
-        salt is bytes 16 byte long root cryptomatter from which seeds for Signers
-            in list are derived
-            random salt created if not provided
-        count is number of signers in list
-    """
-    signers = generateSigners(salt=salt, count=count)
-
-    return [signer.qb64 for signer in signers]  # fetch sigkey as private key
+# ToDo: nonces only need 128 bits of entropy. a Salt is enough
+# Just use Salter().qb64.
+# Deprecated
 
+def randomNonce():
+    """ Generate a random ed25519 seed and encode as qb64
 
-def generatePublics(salt=None, count=8, transferable=True):
+    Returns:
+        str: qb64 encoded ed25519 random seed
     """
-    Returns list of fully qualified Base64 secret seeds for Ed25519 private keys
+    preseed = pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)
+    seedqb64 = Matter(raw=preseed, code=MtrDex.Ed25519_Seed).qb64
+    return seedqb64
+
 
-    Parameters:
-        salt is bytes 16 byte long root cryptomatter from which seeds for Signers
-            in list are derived
-            random salt created if not provided
-        count is number of signers in list
-    """
-    signers = generateSigners(salt=salt, count=count, transferable=transferable)
 
-    return [signer.verfer.qb64 for signer in signers]  # fetch verkey as public key
 
 
 # secret derivation security tier
 Tierage = namedtuple("Tierage", 'low med high')
 
 Tiers = Tierage(low='low', med='med', high='high')
 
@@ -404,65 +248,73 @@
     MatterCodex is codex code (stable) part of all matter derivation codes.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
     """
 
     Ed25519_Seed:         str = 'A'  # Ed25519 256 bit random seed for private key
     Ed25519N:             str = 'B'  # Ed25519 verification key non-transferable, basic derivation.
-    X25519:               str = 'C'  # X25519 public encryption key, converted from Ed25519 or Ed25519N.
+    X25519:               str = 'C'  # X25519 public encryption key, may be converted from Ed25519 or Ed25519N.
     Ed25519:              str = 'D'  # Ed25519 verification key basic derivation
     Blake3_256:           str = 'E'  # Blake3 256 bit digest self-addressing derivation.
     Blake2b_256:          str = 'F'  # Blake2b 256 bit digest self-addressing derivation.
     Blake2s_256:          str = 'G'  # Blake2s 256 bit digest self-addressing derivation.
     SHA3_256:             str = 'H'  # SHA3 256 bit digest self-addressing derivation.
     SHA2_256:             str = 'I'  # SHA2 256 bit digest self-addressing derivation.
     ECDSA_256k1_Seed:     str = 'J'  # ECDSA secp256k1 256 bit random Seed for private key
     Ed448_Seed:           str = 'K'  # Ed448 448 bit random Seed for private key
     X448:                 str = 'L'  # X448 public encryption key, converted from Ed448
     Short:                str = 'M'  # Short 2 byte b2 number
     Big:                  str = 'N'  # Big 8 byte b2 number
-    X25519_Private:       str = 'O'  # X25519 private decryption key converted from Ed25519
+    X25519_Private:       str = 'O'  # X25519 private decryption key/seed, may be converted from Ed25519
     X25519_Cipher_Seed:   str = 'P'  # X25519 sealed box 124 char qb64 Cipher of 44 char qb64 Seed
     ECDSA_256r1_Seed:     str = "Q"  # ECDSA secp256r1 256 bit random Seed for private key
     Tall:                 str = 'R'  # Tall 5 byte b2 number
     Large:                str = 'S'  # Large 11 byte b2 number
     Great:                str = 'T'  # Great 14 byte b2 number
     Vast:                 str = 'U'  # Vast 17 byte b2 number
-    Label1:               str = 'V'  # Label1 as one char (bytes) field map label lead size 1
-    Label2:               str = 'W'  # Label2 as two char (bytes) field map label lead size 0
-    Tag3:                 str = 'X'  # Tag3 3 B64 encoded chars for field tag or packet type, semver, trait like 'DND'
-    Tag7:                 str = 'Y'  # Tag7 7 B64 encoded chars for field tag or packet kind and version KERIVVV
-    Salt_128:             str = '0A'  # 128 bit random salt or 128 bit number (see Huge)
+    Label1:               str = 'V'  # Label1 1 bytes for label lead size 1
+    Label2:               str = 'W'  # Label2 2 bytes for label lead size 0
+    Tag3:                 str = 'X'  # Tag3  3 B64 encoded chars for special values
+    Tag7:                 str = 'Y'  # Tag7  7 B64 encoded chars for special values
+    Blind:                str = 'Z'  # Blinding factor 256 bits, Cryptographic strength deterministically generated from random salt
+    Salt_128:             str = '0A'  # random salt/seed/nonce/private key or number of length 128 bits (Huge)
     Ed25519_Sig:          str = '0B'  # Ed25519 signature.
     ECDSA_256k1_Sig:      str = '0C'  # ECDSA secp256k1 signature.
     Blake3_512:           str = '0D'  # Blake3 512 bit digest self-addressing derivation.
     Blake2b_512:          str = '0E'  # Blake2b 512 bit digest self-addressing derivation.
     SHA3_512:             str = '0F'  # SHA3 512 bit digest self-addressing derivation.
     SHA2_512:             str = '0G'  # SHA2 512 bit digest self-addressing derivation.
     Long:                 str = '0H'  # Long 4 byte b2 number
     ECDSA_256r1_Sig:      str = '0I'  # ECDSA secp256r1 signature.
-    Tag1:                 str = '0J'  # Tag1 1 B64 encoded char with pre pad for field tag
-    Tag2:                 str = '0K'  # Tag2 2 B64 encoded chars for field tag or version VV or trait like 'EO'
-    Tag5:                 str = '0L'  # Tag5 5 B64 encoded chars with pre pad for field tag
-    Tag6:                 str = '0M'  # Tag6 6 B64 encoded chars for field tag or protocol kind version like KERIVV (KERI 1.1) or KKKVVV
+    Tag1:                 str = '0J'  # Tag1 1 B64 encoded char + 1 prepad for special values
+    Tag2:                 str = '0K'  # Tag2 2 B64 encoded chars for for special values
+    Tag5:                 str = '0L'  # Tag5 5 B64 encoded chars + 1 prepad for special values
+    Tag6:                 str = '0M'  # Tag6 6 B64 encoded chars for special values
+    Tag9:                 str = '0N'  # Tag9 9 B64 encoded chars + 1 prepad for special values
+    Tag10:                str = '0O'  # Tag10 10 B64 encoded chars for special values
     ECDSA_256k1N:         str = '1AAA'  # ECDSA secp256k1 verification key non-transferable, basic derivation.
     ECDSA_256k1:          str = '1AAB'  # ECDSA public verification or encryption key, basic derivation
     Ed448N:               str = '1AAC'  # Ed448 non-transferable prefix public signing verification key. Basic derivation.
     Ed448:                str = '1AAD'  # Ed448 public signing verification key. Basic derivation.
     Ed448_Sig:            str = '1AAE'  # Ed448 signature. Self-signing derivation.
-    Tag4:                 str = '1AAF'  # Tag4 4 B64 encoded chars for field tag or message kind
+    Tag4:                 str = '1AAF'  # Tag4 4 B64 encoded chars for special values
     DateTime:             str = '1AAG'  # Base64 custom encoded 32 char ISO-8601 DateTime
     X25519_Cipher_Salt:   str = '1AAH'  # X25519 sealed box 100 char qb64 Cipher of 24 char qb64 Salt
     ECDSA_256r1N:         str = '1AAI'  # ECDSA secp256r1 verification key non-transferable, basic derivation.
     ECDSA_256r1:          str = '1AAJ'  # ECDSA secp256r1 verification or encryption key, basic derivation
     Null:                 str = '1AAK'  # Null None or empty value
-    Yes:                  str = '1AAL'  # Yes Truthy Boolean value
-    No:                   str = '1AAM'  # No Falsey Boolean value
-    TBD1:                 str = '2AAA'  # Testing purposes only fixed with lead size 1
-    TBD2:                 str = '3AAA'  # Testing purposes only of fixed with lead size 2
+    No:                   str = '1AAL'  # No Falsey Boolean value
+    Yes:                  str = '1AAM'  # Yes Truthy Boolean value
+    Tag8:                 str = '1AAN'  # Tag8 8 B64 encoded chars for special values
+    TBD0S:                str = '1__-'  # Testing purposes only, fixed special values with non-empty raw lead size 0
+    TBD0:                 str = '1___'  # Testing purposes only, fixed with lead size 0
+    TBD1S:                str = '2__-'  # Testing purposes only, fixed special values with non-empty raw lead size 1
+    TBD1:                 str = '2___'  # Testing purposes only, fixed with lead size 1
+    TBD2S:                str = '3__-'  # Testing purposes only, fixed special values with non-empty raw lead size 2
+    TBD2:                 str = '3___'  # Testing purposes only, fixed with lead size 2
     StrB64_L0:            str = '4A'  # String Base64 only lead size 0
     StrB64_L1:            str = '5A'  # String Base64 only lead size 1
     StrB64_L2:            str = '6A'  # String Base64 only lead size 2
     StrB64_Big_L0:        str = '7AAA'  # String Base64 only big lead size 0
     StrB64_Big_L1:        str = '8AAA'  # String Base64 only big lead size 1
     StrB64_Big_L2:        str = '9AAA'  # String Base64 only big lead size 2
     Bytes_L0:             str = '4B'  # Byte String lead size 0
@@ -494,14 +346,16 @@
     def __iter__(self):
         return iter(astuple(self))  # enables inclusion test with "in"
 
 
 MtrDex = MatterCodex()  # Make instance
 
 
+
+
 @dataclass(frozen=True)
 class SmallVarRawSizeCodex:
     """
     SmallVarRawSizeCodex is codex all selector characters for the three small
     variable raw size tables that act as one table but with different leader
     byte sizes.
 
@@ -536,81 +390,14 @@
     def __iter__(self):
         return iter(astuple(self))
 
 
 LargeVrzDex = LargeVarRawSizeCodex()  # Make instance
 
 
-@dataclass(frozen=True)
-class NonTransCodex:
-    """
-    NonTransCodex is codex all non-transferable derivation codes
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Ed25519N: str = 'B'  # Ed25519 verification key non-transferable, basic derivation.
-    ECDSA_256k1N: str = '1AAA'  # ECDSA secp256k1 verification key non-transferable, basic derivation.
-    Ed448N: str = '1AAC'  # Ed448 non-transferable prefix public signing verification key. Basic derivation.
-    ECDSA_256r1N: str = "1AAI"  # ECDSA secp256r1 verification key non-transferable, basic derivation.
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-
-NonTransDex = NonTransCodex()  # Make instance
-
-# When add new to DigCodes update Saider.Digests and Serder.Digests class attr
-@dataclass(frozen=True)
-class DigCodex:
-    """
-    DigCodex is codex all digest derivation codes. This is needed to ensure
-    delegated inception using a self-addressing derivation i.e. digest derivation
-    code.
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Blake3_256: str = 'E'  # Blake3 256 bit digest self-addressing derivation.
-    Blake2b_256: str = 'F'  # Blake2b 256 bit digest self-addressing derivation.
-    Blake2s_256: str = 'G'  # Blake2s 256 bit digest self-addressing derivation.
-    SHA3_256: str = 'H'  # SHA3 256 bit digest self-addressing derivation.
-    SHA2_256: str = 'I'  # SHA2 256 bit digest self-addressing derivation.
-    Blake3_512: str = '0D'  # Blake3 512 bit digest self-addressing derivation.
-    Blake2b_512: str = '0E'  # Blake2b 512 bit digest self-addressing derivation.
-    SHA3_512: str = '0F'  # SHA3 512 bit digest self-addressing derivation.
-    SHA2_512: str = '0G'  # SHA2 512 bit digest self-addressing derivation.
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-
-DigDex = DigCodex()  # Make instance
-
-
-@dataclass(frozen=True)
-class NumCodex:
-    """
-    NumCodex is codex of Base64 derivation codes for compactly representing
-    numbers across a wide rage of sizes.
-
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Short:   str = 'M'  # Short 2 byte b2 number
-    Long:    str = '0H'  # Long 4 byte b2 number
-    Big:     str = 'N'  # Big 8 byte b2 number
-    Huge:    str = '0A'  # Huge 16 byte b2 number (same as Salt_128)
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-
-NumDex = NumCodex()  # Make instance
-
-
-
 
 @dataclass(frozen=True)
 class BextCodex:
     """
     BextCodex is codex of all variable sized Base64 Text (Bext) derivation codes.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
@@ -646,14 +433,15 @@
 
     def __iter__(self):
         return iter(astuple(self))
 
 
 TexDex = TextCodex()  # Make instance
 
+
 @dataclass(frozen=True)
 class CipherX25519VarCodex:
     """
     CipherX25519VarCodex is codex all variable sized cipher bytes derivation codes
     for sealed box encryped ciphertext. Plaintext is B2.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
@@ -756,14 +544,163 @@
 
 
 CiXVarQB2Dex = CipherX25519QB2VarCodex()  # Make instance
 
 
 
 
+@dataclass(frozen=True)
+class NonTransCodex:
+    """
+    NonTransCodex is codex all non-transferable derivation codes
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+    """
+    Ed25519N: str = 'B'  # Ed25519 verification key non-transferable, basic derivation.
+    ECDSA_256k1N: str = '1AAA'  # ECDSA secp256k1 verification key non-transferable, basic derivation.
+    Ed448N: str = '1AAC'  # Ed448 non-transferable prefix public signing verification key. Basic derivation.
+    ECDSA_256r1N: str = "1AAI"  # ECDSA secp256r1 verification key non-transferable, basic derivation.
+
+    def __iter__(self):
+        return iter(astuple(self))
+
+
+NonTransDex = NonTransCodex()  # Make instance
+
+# When add new to DigCodes update Saider.Digests and Serder.Digests class attr
+@dataclass(frozen=True)
+class DigCodex:
+    """
+    DigCodex is codex all digest derivation codes. This is needed to ensure
+    delegated inception using a self-addressing derivation i.e. digest derivation
+    code.
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+    """
+    Blake3_256: str = 'E'  # Blake3 256 bit digest self-addressing derivation.
+    Blake2b_256: str = 'F'  # Blake2b 256 bit digest self-addressing derivation.
+    Blake2s_256: str = 'G'  # Blake2s 256 bit digest self-addressing derivation.
+    SHA3_256: str = 'H'  # SHA3 256 bit digest self-addressing derivation.
+    SHA2_256: str = 'I'  # SHA2 256 bit digest self-addressing derivation.
+    Blake3_512: str = '0D'  # Blake3 512 bit digest self-addressing derivation.
+    Blake2b_512: str = '0E'  # Blake2b 512 bit digest self-addressing derivation.
+    SHA3_512: str = '0F'  # SHA3 512 bit digest self-addressing derivation.
+    SHA2_512: str = '0G'  # SHA2 512 bit digest self-addressing derivation.
+
+    def __iter__(self):
+        return iter(astuple(self))
+
+
+DigDex = DigCodex()  # Make instance
+
+
+@dataclass(frozen=True)
+class NumCodex:
+    """
+    NumCodex is codex of Base64 derivation codes for compactly representing
+    numbers across a wide rage of sizes.
+
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+    """
+    Short:   str = 'M'  # Short 2 byte b2 number
+    Long:    str = '0H'  # Long 4 byte b2 number
+    Tall:    str = 'R'  # Tall 5 byte b2 number
+    Big:     str = 'N'  # Big 8 byte b2 number
+    Large:   str = 'S'  # Large 11 byte b2 number
+    Great:   str = 'T'  # Great 14 byte b2 number
+    Huge:    str = '0A'  # Huge 16 byte b2 number (same as Salt_128)
+    Vast:    str = 'U'  # Vast 17 byte b2 number
+
+    def __iter__(self):
+        return iter(astuple(self))
+
+
+NumDex = NumCodex()  # Make instance
+
+
+@dataclass(frozen=True)
+class TagCodex:
+    """
+    TagCodex is codex of Base64 derivation codes for compactly representing
+    various small Base64 tag values as special code soft part values.
+
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+    """
+    Tag1:  str = '0J'  # 1 B64 char tag with 1 pre pad
+    Tag2:  str = '0K'  # 1 B64 char tag
+    Tag3:  str = 'X'  # 1 B64 char tag
+    Tag4:  str = '1AAF'  # 1 B64 char tag
+    Tag5:  str = '0L'  # 1 B64 char tag with 1 pre pad
+    Tag6:  str = '0M'  # 1 B64 char tag
+    Tag7:  str = 'Y'  # 1 B64 char tag
+    Tag8:  str = '1AAN'  # 1 B64 char tag
+    Tag9:  str = '0N'  # 1 B64 char tag with 1 pre pad
+    Tag10: str = '0O'  # 1 B64 char tag
+
+    def __iter__(self):
+        return iter(astuple(self))
+
+
+TagDex = TagCodex()  # Make instance
+
+
+@dataclass(frozen=True)
+class PadTagCodex:
+    """
+    TagCodex is codex of Base64 derivation codes for compactly representing
+    various small Base64 tag values as prepadded special code soft part values.
+    Prepad is 1 B64 char.
+
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+    """
+    Tag1:  str = '0J'  # 1 B64 char tag with 1 pre pad
+    Tag5:  str = '0L'  # 1 B64 char tag with 1 pre pad
+    Tag9:  str = '0N'  # 1 B64 char tag with 1 pre pad
+
+    def __iter__(self):
+        return iter(astuple(self))
+
+
+PadTagDex = PadTagCodex()  # Make instance
+
+
+@dataclass(frozen=True)
+class PreCodex:
+    """
+    PreCodex is codex all identifier prefix derivation codes.
+    This is needed to verify valid inception events.
+    Only provide defined codes.
+    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+    """
+    Ed25519N:      str = 'B'  # Ed25519 verification key non-transferable, basic derivation.
+    Ed25519:       str = 'D'  # Ed25519 verification key basic derivation
+    Blake3_256:    str = 'E'  # Blake3 256 bit digest self-addressing derivation.
+    Blake2b_256:   str = 'F'  # Blake2b 256 bit digest self-addressing derivation.
+    Blake2s_256:   str = 'G'  # Blake2s 256 bit digest self-addressing derivation.
+    SHA3_256:      str = 'H'  # SHA3 256 bit digest self-addressing derivation.
+    SHA2_256:      str = 'I'  # SHA2 256 bit digest self-addressing derivation.
+    Blake3_512:    str = '0D'  # Blake3 512 bit digest self-addressing derivation.
+    Blake2b_512:   str = '0E'  # Blake2b 512 bit digest self-addressing derivation.
+    SHA3_512:      str = '0F'  # SHA3 512 bit digest self-addressing derivation.
+    SHA2_512:      str = '0G'  # SHA2 512 bit digest self-addressing derivation.
+    ECDSA_256k1N:  str = '1AAA'  # ECDSA secp256k1 verification key non-transferable, basic derivation.
+    ECDSA_256k1:   str = '1AAB'  # ECDSA public verification or encryption key, basic derivation
+    ECDSA_256r1N:  str = "1AAI"  # ECDSA secp256r1 verification key non-transferable, basic derivation.
+    ECDSA_256r1:   str = "1AAJ"  # ECDSA secp256r1 verification or encryption key, basic derivation
+
+    def __iter__(self):
+        return iter(astuple(self))
+
+
+PreDex = PreCodex()  # Make instance
+
+
 # namedtuple for size entries in Matter  and Counter derivation code tables
 # hs is the hard size int number of chars in hard (stable) part of code
 # ss is the soft size int number of chars in soft (unstable) part of code
 # fs is the full size int number of chars in code plus appended material if any
 # ls is the lead size int number of bytes to pre-pad pre-converted raw binary
 Sizage = namedtuple("Sizage", "hs ss fs ls")
 
@@ -773,56 +710,77 @@
     Matter is fully qualified cryptographic material primitive base class for
     non-indexed primitives.
 
     Sub classes are derivation code and key event element context specific.
 
     Includes the following attributes and properties:
 
+    Class Attributes:
+        Codex (MatterCodex):  MtrDex
+        Hards (dict): hard sizes keyed by qb64 selector
+        Bards (dict): hard size keyed by qb2 selector
+        Sizes (dict): sizes tables for codes
+
+    Calss Methods:
+
+
     Attributes:
 
     Properties:
         code (str): hard part of derivation code to indicate cypher suite
-        both (int): hard and soft parts of full text code
-        size (int): Number of triplets of bytes including lead bytes
-            (quadlets of chars) of variable sized material. Value of soft size,
-            ss, part of full text code.
-            Otherwise None.
-        rize (int): number of bytes of raw material not including
-                    lead bytes
-        raw (bytes): crypto material only without code
+        hard (str): hard part of derivation code. alias for code
+        soft (str | bytes): soft part of derivation code fs any.
+                    Empty when ss = 0.
+        both (str): hard + soft parts of full text code
+        size (int | None): Number of quadlets/triplets of chars/bytes including
+                            lead bytes of variable sized material (fs = None).
+                            Converted value of the soft part (of len ss) of full
+                            derivation code.
+                          Otherwise None when not variably sized (fs != None)
+        fullSize (int): full size of primitive
+        raw (bytes): crypto material only. Not derivation code or lead bytes.
         qb64 (str): Base64 fully qualified with derivation code + crypto mat
         qb64b (bytes): Base64 fully qualified with derivation code + crypto mat
         qb2  (bytes): binary with derivation code + crypto material
         transferable (bool): True means transferable derivation code False otherwise
         digestive (bool): True means digest derivation code False otherwise
         prefixive (bool): True means identifier prefix derivation code False otherwise
+        special (bool): True when soft is special raw is empty and fixed size
+        composable (bool): True when .qb64b and .qb2 are 24 bit aligned and round trip
 
     Hidden:
         _code (str): value for .code property
+        _soft (str): soft value of full code
         _raw (bytes): value for .raw property
-        _rsize (bytes): value for .rsize property. Raw size in bytes when
-            variable sized material else None.
-        _size (int): value for .size property. Number of triplets of bytes
-            including lead bytes (quadlets of chars) of variable sized material
-            else None.
-        _infil (types.MethodType): creates qb64b from .raw and .code
-                                   (fully qualified Base64)
-        _exfil (types.MethodType): extracts .code and .raw from qb64b
-                                   (fully qualified Base64)
+        _rawSize():
+        _leadSize():
+        _special():
+        _infil(): creates qb64b from .raw and .code (fully qualified Base64)
+        _binfil(): creates qb2 from .raw and .code (fully qualified Base2)
+        _exfil(): extracts .code and .raw from qb64b (fully qualified Base64)
+        _bexfil(): extracts .code and .raw from qb2 (fully qualified Base2)
+
+
+    Special soft values are indicated when fn in table is None and ss > 0.
 
     """
-    Codex = MtrDex
     # Hards table maps from bytes Base64 first code char to int of hard size, hs,
     # (stable) of code. The soft size, ss, (unstable) is always 0 for Matter
     # unless fs is None which allows for variable size multiple of 4, i.e.
     # not (hs + ss) % 4.
     Hards = ({chr(c): 1 for c in range(65, 65 + 26)})  # size of hard part of code
     Hards.update({chr(c): 1 for c in range(97, 97 + 26)})
     Hards.update([('0', 2), ('1', 4), ('2', 4), ('3', 4), ('4', 2), ('5', 2),
                   ('6', 2), ('7', 4), ('8', 4), ('9', 4)])
+
+
+    # Bards table maps first code char. converted to binary sextext of hard size,
+    # hs. Used for ._bexfil.
+    Bards = ({codeB64ToB2(c): hs for c, hs in Hards.items()})
+
     # Sizes table maps from value of hs chars of code to Sizage namedtuple of
     # (hs, ss, fs, ls) where hs is hard size, ss is soft size, and fs is full size
     # and ls is lead size
     # soft size, ss, should always be 0 for Matter unless fs is None which allows
     # for variable size multiple of 4, i.e. not (hs + ss) % 4.
     Sizes = {
         'A': Sizage(hs=1, ss=0, fs=44, ls=0),
@@ -844,44 +802,52 @@
         'Q': Sizage(hs=1, ss=0, fs=44, ls=0),
         'R': Sizage(hs=1, ss=0, fs=8, ls=0),
         'S': Sizage(hs=1, ss=0, fs=16, ls=0),
         'T': Sizage(hs=1, ss=0, fs=20, ls=0),
         'U': Sizage(hs=1, ss=0, fs=24, ls=0),
         'V': Sizage(hs=1, ss=0, fs=4, ls=1),
         'W': Sizage(hs=1, ss=0, fs=4, ls=0),
-        'X': Sizage(hs=1, ss=0, fs=4, ls=0),
-        'Y': Sizage(hs=1, ss=0, fs=8, ls=0),
+        'X': Sizage(hs=1, ss=3, fs=4, ls=0),
+        'Y': Sizage(hs=1, ss=7, fs=8, ls=0),
+        'Z': Sizage(hs=1, ss=0, fs=44, ls=0),
         '0A': Sizage(hs=2, ss=0, fs=24, ls=0),
         '0B': Sizage(hs=2, ss=0, fs=88, ls=0),
         '0C': Sizage(hs=2, ss=0, fs=88, ls=0),
         '0D': Sizage(hs=2, ss=0, fs=88, ls=0),
         '0E': Sizage(hs=2, ss=0, fs=88, ls=0),
         '0F': Sizage(hs=2, ss=0, fs=88, ls=0),
         '0G': Sizage(hs=2, ss=0, fs=88, ls=0),
         '0H': Sizage(hs=2, ss=0, fs=8, ls=0),
         '0I': Sizage(hs=2, ss=0, fs=88, ls=0),
-        '0J': Sizage(hs=2, ss=0, fs=4, ls=0),
-        '0K': Sizage(hs=2, ss=0, fs=4, ls=0),
-        '0L': Sizage(hs=2, ss=0, fs=8, ls=0),
-        '0M': Sizage(hs=2, ss=0, fs=8, ls=0),
+        '0J': Sizage(hs=2, ss=2, fs=4, ls=0),
+        '0K': Sizage(hs=2, ss=2, fs=4, ls=0),
+        '0L': Sizage(hs=2, ss=6, fs=8, ls=0),
+        '0M': Sizage(hs=2, ss=6, fs=8, ls=0),
+        '0N': Sizage(hs=2, ss=10, fs=12, ls=0),
+        '0O': Sizage(hs=2, ss=10, fs=12, ls=0),
         '1AAA': Sizage(hs=4, ss=0, fs=48, ls=0),
         '1AAB': Sizage(hs=4, ss=0, fs=48, ls=0),
         '1AAC': Sizage(hs=4, ss=0, fs=80, ls=0),
         '1AAD': Sizage(hs=4, ss=0, fs=80, ls=0),
         '1AAE': Sizage(hs=4, ss=0, fs=56, ls=0),
-        '1AAF': Sizage(hs=4, ss=0, fs=8, ls=0),
+        '1AAF': Sizage(hs=4, ss=4, fs=8, ls=0),
         '1AAG': Sizage(hs=4, ss=0, fs=36, ls=0),
         '1AAH': Sizage(hs=4, ss=0, fs=100, ls=0),
         '1AAI': Sizage(hs=4, ss=0, fs=48, ls=0),
         '1AAJ': Sizage(hs=4, ss=0, fs=48, ls=0),
         '1AAK': Sizage(hs=4, ss=0, fs=4, ls=0),
         '1AAL': Sizage(hs=4, ss=0, fs=4, ls=0),
         '1AAM': Sizage(hs=4, ss=0, fs=4, ls=0),
-        '2AAA': Sizage(hs=4, ss=0, fs=8, ls=1),
-        '3AAA': Sizage(hs=4, ss=0, fs=8, ls=2),
+        '1AAN': Sizage(hs=4, ss=8, fs=12, ls=0),
+        '1__-': Sizage(hs=4, ss=2, fs=12, ls=0),
+        '1___': Sizage(hs=4, ss=0, fs=8, ls=0),
+        '2__-': Sizage(hs=4, ss=2, fs=12, ls=1),
+        '2___': Sizage(hs=4, ss=0, fs=8, ls=1),
+        '3__-': Sizage(hs=4, ss=2, fs=12, ls=2),
+        '3___': Sizage(hs=4, ss=0, fs=8, ls=2),
         '4A': Sizage(hs=2, ss=2, fs=None, ls=0),
         '5A': Sizage(hs=2, ss=2, fs=None, ls=1),
         '6A': Sizage(hs=2, ss=2, fs=None, ls=2),
         '7AAA': Sizage(hs=4, ss=4, fs=None, ls=0),
         '8AAA': Sizage(hs=4, ss=4, fs=None, ls=1),
         '9AAA': Sizage(hs=4, ss=4, fs=None, ls=2),
         '4B': Sizage(hs=2, ss=2, fs=None, ls=0),
@@ -907,106 +873,149 @@
         '6E': Sizage(hs=2, ss=2, fs=None, ls=2),
         '7AAE': Sizage(hs=4, ss=4, fs=None, ls=0),
         '8AAE': Sizage(hs=4, ss=4, fs=None, ls=1),
         '9AAE': Sizage(hs=4, ss=4, fs=None, ls=2),
     }
 
 
-    # Bards table maps first code char. converted to binary sextext of hard size,
-    # hs. Used for ._bexfil.
-    Bards = ({codeB64ToB2(c): hs for c, hs in Hards.items()})
 
-    def __init__(self, raw=None, code=MtrDex.Ed25519N, rize=None,
+    def __init__(self, raw=None, code=MtrDex.Ed25519N, soft='', rize=None,
                  qb64b=None, qb64=None, qb2=None, strip=False):
         """
         Validate as fully qualified
         Parameters:
-            raw (bytes): unqualified crypto material usable for crypto operations
+            raw (bytes | bytearray | None): unqualified crypto material usable
+                    for crypto operations.
             code (str): stable (hard) part of derivation code
-            rize (int): raw size in bytes when variable sized material else None
-            qb64b (bytes): fully qualified crypto material Base64
-            qb64 (str, bytes):  fully qualified crypto material Base64
-            qb2 (bytes): fully qualified crypto material Base2
+            soft (str | bytes): soft part for special codes
+            rize (int | None): raw size in bytes when variable sized material not
+                        including lead bytes if any
+                        Otherwise None
+            qb64b (bytes | None): fully qualified crypto material Base64
+            qb64 (str | bytes | None):  fully qualified crypto material Base64
+            qb2 (bytes | None): fully qualified crypto material Base2
             strip (bool): True means strip (delete) matter from input stream
                 bytearray after parsing qb64b or qb2. False means do not strip
 
 
-        Needs either (raw and code and optionally size and rsize)
+        Needs either (raw and code and optionally rsize)
                or qb64b or qb64 or qb2
         Otherwise raises EmptyMaterialError
-        When raw and code and optional size and rsize provided
-            then validate that code is correct for length of raw, size, rsize
-            and assign .raw
+        When raw and code and optional rsize provided
+            then validate that code is correct for length of raw, rsize,
+            computed size from Sizes and assign .raw
         Else when qb64b or qb64 or qb2 provided extract and assign
             .raw and .code and .size and .rsize
 
         """
-        size = None  # variable raw binary size including leader in quadlets
-        if raw is not None:  # raw provided
+        if hasattr(soft, "decode"):  # make soft str
+            soft = soft.decode("utf-8")
+
+        if raw is not None:  # raw provided but may be empty
             if not code:
                 raise EmptyMaterialError(f"Improper initialization need either "
-                                         f"(raw and code) or qb64b or qb64 or qb2.")
+                                         f"(raw not None and code) or "
+                                         f"(code and soft) or "
+                                         f"qb64b or qb64 or qb2.")
 
             if not isinstance(raw, (bytes, bytearray)):
-                raise TypeError(f"Not a bytes or bytearray, raw={raw}.")
+                raise TypeError(f"Not a bytes or bytearray {raw=}.")
 
             if code not in self.Sizes:
-                raise InvalidCodeError("Unsupported code={}.".format(code))
+                raise InvalidCodeError(f"Unsupported {code=}.")
 
-            if code[0] in SmallVrzDex or code[0] in LargeVrzDex:  # dynamic size
-                if rize:  # use rsize to determin length of raw to extract
+            hs, ss, fs, ls = self.Sizes[code]  # assumes unit tests force valid sizes
+
+            if fs is None:  # variable sized assumes code[0] in SmallVrzDex or LargeVrzDex
+                if rize:  # use rsize to determine length of raw to extract
                     if rize < 0:
                         raise InvalidVarRawSizeError(f"Missing var raw size for "
                                                      f"code={code}.")
                 else:  # use length of provided raw as rize
                     rize = len(raw)
 
                 ls = (3 - (rize % 3)) % 3  # calc actual lead (pad) size
                 # raw binary size including leader in bytes
                 size = (rize + ls) // 3  # calculate value of size in triplets
+
                 if code[0] in SmallVrzDex:  # compute code with sizes
-                    if size <= (64 ** 2 - 1):
+                    if size <= (64 ** 2 - 1):  # ss = 2
                         hs = 2
                         s = astuple(SmallVrzDex)[ls]
                         code = f"{s}{code[1:hs]}"
-                    elif size <= (64 ** 4 - 1):  # make big version of code
+                        ss = 2
+                    elif size <= (64 ** 4 - 1):  # ss = 4 make big version of code
                         hs = 4
                         s = astuple(LargeVrzDex)[ls]
                         code = f"{s}{'A' * (hs - 2)}{code[1]}"
+                        soft = intToB64(size, 4)
+                        ss = 4
                     else:
-                        raise InvalidVarRawSizeError(r"Unsupported raw size for "
-                                                     f"code={code}.")
+                        raise InvalidVarRawSizeError(f"Unsupported raw size for "
+                                                     f"{code=}.")
                 elif code[0] in LargeVrzDex:  # compute code with sizes
-                    if size <= (64 ** 4 - 1):
+                    if size <= (64 ** 4 - 1):  # ss = 4
                         hs = 4
                         s = astuple(LargeVrzDex)[ls]
                         code = f"{s}{code[1:hs]}"
+                        ss = 4
                     else:
-                        raise InvalidVarRawSizeError(r"Unsupported raw size for "
-                                                     f"code={code}.")
+                        raise InvalidVarRawSizeError(f"Unsupported raw size for "
+                                                     f"{code=}.")
                 else:
-                    raise InvalidVarRawSizeError(r"Unsupported variable raw size "
-                                                 f"code={code}.")
+                    raise InvalidVarRawSizeError(f"Unsupported variable raw size "
+                                                 f"{code=}.")
+                soft = intToB64(size, ss)
+
+            else:  # fixed size but raw may be empty and/or special soft
+                rize = Matter._rawSize(code)  # get raw size from Sizes for code
+
+                if ss > 0: # special soft size, so soft must be provided
+                    soft = soft[:ss]
+                    if len(soft) != ss:
+                        raise SoftMaterialError(f"Not enough chars in {soft=} "
+                                                 f"with {ss=} for {code=}.")
+
+                    if not Reb64.match(soft.encode("utf-8")):
+                        raise InvalidSoftError(f"Non Base64 chars in {soft=}.")
+                else:
+                    soft = ''  # must be empty when ss == 0
 
-            else:
-                hs, ss, fs, ls = self.Sizes[code]  # get sizes assumes ls consistent
-                if not fs:  # invalid
-                    raise InvalidVarSizeError(r"Unsupported variable size "
-                                              f"code={code}.")
-                rize = Matter._rawSize(code)
 
             raw = raw[:rize]  # copy only exact size from raw stream
             if len(raw) != rize:  # forbids shorter
                 raise RawMaterialError(f"Not enougth raw bytes for code={code}"
-                                       f"expected {rize} got {len(raw)}.")
+                                       f"expected {rize=} got {len(raw)}.")
 
-            self._code = code  # hard value part of code
-            self._size = size  # soft value part of code in int
+            self._code = code  # str hard part of code
+            self._soft = soft  # str soft part of code, empty when ss=0
             self._raw = bytes(raw)  # crypto ops require bytes not bytearray
 
+        elif soft and code:  # fixed size and special when raw None
+            hs, ss, fs, ls = self.Sizes[code]  # assumes unit tests force valid sizes
+            if not fs:  # variable sized code so can't be soft
+                raise InvalidSoftError(f"Unsupported variable sized {code=} "
+                                       f" with {fs=} for special {soft=}.")
+
+            if not ss > 0 or (fs == hs + ss and not ls == 0):  # not special soft
+                raise InvalidSoftError("Invalid soft size={ss} or lead={ls} "
+                                       f" or {code=} {fs=} when special soft.")
+
+            soft = soft[:ss]
+            if len(soft) != ss:
+                raise SoftMaterialError(f"Not enough chars in {soft=} "
+                                         f"with {ss=} for {code=}.")
+
+            if not Reb64.match(soft.encode("utf-8")):
+                raise InvalidSoftError(f"Non Base64 chars in {soft=}.")
+
+            self._code = code  # str hard part of code
+            self._soft = soft  # str soft part of code, empty when ss=0
+            self._raw = b''  # make raw empty when None and when special soft
+
         elif qb64b is not None:
             self._exfil(qb64b)
             if strip:  # assumes bytearray
                 del qb64b[:self.fullSize]
 
         elif qb64 is not None:
             self._exfil(qb64)
@@ -1014,67 +1023,125 @@
         elif qb2 is not None:
             self._bexfil(qb2)
             if strip:  # assumes bytearray
                 del qb2[:self.fullSize * 3 // 4]
 
         else:
             raise EmptyMaterialError(f"Improper initialization need either "
-                                     f"(raw and code) or qb64b or qb64 or qb2.")
+                                         f"(raw not None and code) or "
+                                         f"(code and soft) or "
+                                         f"qb64b or qb64 or qb2.")
+
 
     @classmethod
     def _rawSize(cls, code):
         """
         Returns raw size in bytes not including leader for a given code
         Parameters:
             code (str): derivation code Base64
         """
         hs, ss, fs, ls = cls.Sizes[code]  # get sizes
         cs = hs + ss  # both hard + soft code size
         if fs is None:
             raise InvalidCodeSizeError(f"Non-fixed raw size code {code}.")
+        # assumes .Sizes only has valid entries, cs % 4 != 3, and fs % 4 == 0
         return (((fs - cs) * 3 // 4) - ls)
 
+
     @classmethod
     def _leadSize(cls, code):
         """
         Returns lead size in bytes for a given code
         Parameters:
             code (str): derivation code Base64
         """
         _, _, _, ls = cls.Sizes[code]  # get lead size from .Sizes table
         return ls
 
+
+    @classmethod
+    def _special(cls, code):
+        """
+        Returns:
+            special (bool): True when code has special soft i.e. when
+                    fs is not None and ss > 0
+                False otherwise
+
+        """
+        hs, ss, fs, ls = cls.Sizes[code]
+
+        return (fs is not None and ss > 0)
+
+
     @property
     def code(self):
         """
-        Returns ._code which is the hard part only of full text code.
-        Some codes only have a hard part. Soft part is for variable sized matter.
-        Makes .code read only
+        Returns:
+            code (str): hard part only of full text code.
+
+        Getter for ._code. Makes ._code read only
+
+        Some codes only have a hard part. Soft part may be for variable sized
+        matter or for special codes that are code only (raw is empty)
         """
         return self._code
 
+
     @property
-    def both(self):
+    def hard(self):
+        """
+        Returns:
+            hard (str): hard part only of full text code. Alias for .code.
+
         """
-        Returns both hard and soft parts of full text code
+        return self.code
+
+
+    @property
+    def soft(self):
+        """
+        Returns:
+            soft (str): soft part only of full text code.
+
+        Getter for ._soft. Make ._soft read only
         """
-        _, ss, _, _ = self.Sizes[self.code]
-        return (f"{self.code}{intToB64(self.size, l=ss)}")
+        return self._soft
 
 
     @property
     def size(self):
         """
-        Returns ._size int or None if not variable sized matter
-        Makes .size read only
+        Returns:
+            size(int | None): Number of variably sized b64 quadlets/b2 triplets
+                                in primitive when varibly sized
+                              None when not variably sized when (fs!=None)
+
+        Number of quadlets/triplets of chars/bytes of variable sized material or
+        None when not variably sized.
 
-        Number of triplets of bytes including lead bytes (quadlets of chars)
-        of variable sized material. Value of soft size, ss, part of full text code.
+        Converted qb64 value to int of soft ss portion of full text code
+        when variably sized primitive material (fs == None).
         """
-        return self._size
+        return (b64ToInt(self.soft) if self.soft else None)
+
+
+    @property
+    def both(self):
+        """
+        Returns:
+            both (str):  hard + soft parts of full text code
+        """
+        #_, ss, _, _ = self.Sizes[self.code]
+
+        #if self.size is not None:
+            #return (f"{self.code}{intToB64(self.size, l=ss)}")
+        #else:
+            #return (f"{self.code}{self.soft}")
+
+        return (f"{self.code}{self.soft}")
 
 
     @property
     def fullSize(self):
         """
         Returns full size of matter in bytes
         Fixed size codes returns fs from .Sizes
@@ -1082,57 +1149,63 @@
         """
         hs, ss, fs, _ = self.Sizes[self.code]  # get sizes
 
         if fs is None:  # compute fs from ss characters in code
             fs = hs + ss + (self.size * 4)
         return fs
 
+
     @property
     def raw(self):
         """
         Returns ._raw
         Makes .raw read only
         """
         return self._raw
 
+
     @property
     def qb64b(self):
         """
         Property qb64b:
         Returns Fully Qualified Base64 Version encoded as bytes
         Assumes self.raw and self.code are correctly populated
         """
         return self._infil()
 
+
     @property
     def qb64(self):
         """
         Property qb64:
         Returns Fully Qualified Base64 Version
         Assumes self.raw and self.code are correctly populated
         """
         return self.qb64b.decode("utf-8")
 
+
     @property
     def qb2(self):
         """
         Property qb2:
         Returns Fully Qualified Binary Version Bytes
         """
         return self._binfil()
 
+
     @property
     def transferable(self):
         """
         Property transferable:
         Returns True if identifier does not have non-transferable derivation code,
                 False otherwise
         """
         return (self.code not in NonTransDex)
 
+
     @property
     def digestive(self):
         """
         Property digestable:
         Returns True if identifier has digest derivation code,
                 False otherwise
         """
@@ -1145,108 +1218,134 @@
         Property prefixive:
         Returns True if identifier has prefix derivation code,
                 False otherwise
         """
         return (self.code in PreDex)
 
 
-    def _infil(self):
+    @property
+    def special(self):
         """
-        Returns bytes of fully qualified base64 characters
-        self.code + converted self.raw to Base64 with pad chars stripped
-
-        cs = hs + ss
-        fs = (size * 4) + cs
+        special (bool): True when self.code has special self.soft i.e. when
+                    fs is not None and ss > 0  and fs = hs + ss and ls = 0
+                    i.e. (fs fixed and soft not empty and raw is empty and no lead)
+                False otherwise
+        """
+        return self._special(self.code)
 
+    @property
+    def composable(self):
         """
-        code = self.code  # hard size codex value
-        size = self.size  # size if variable length, None otherwise
-        raw = self.raw  # bytes or bytearray
+        composable (bool): True when both .qb64b and .qb2 are 24 bit aligned and
+                           round trip using encodeB64 and decodeB64.
+                           False otherwise
+        """
+        qb64b = self.qb64b
+        qb2 = self.qb2
+        return (len(qb64b) % 4 == 0 and len(qb2) % 3 == 0 and
+                encodeB64(qb2) == qb64b and decodeB64(qb64b) == qb2)
+
 
-        ps = ((3 - (len(raw) % 3)) % 3)  # pad size chars or lead size bytes
+    def _infil(self):
+        """
+        Returns:
+            primitive (bytes): fully qualified base64 characters.
+        """
+        code = self.code  # hard part of full code == codex value
+        both = self.both  # code + soft, soft may be empty
+        raw = self.raw  # bytes or bytearray, raw may be empty
+        rs = len(raw)  # raw size
         hs, ss, fs, ls = self.Sizes[code]
-        if not fs:  # variable sized, compute code ss value from .size
-            cs = hs + ss  # both hard + soft size
-            if cs % 4:
-                raise InvalidCodeSizeError(f"Whole code size not multiple of 4 for "
-                                           f"variable length material. cs={cs}.")
-
-            if size < 0 or size > (64 ** ss - 1):
-                raise InvalidVarSizeError("Invalid size={} for code={}."
-                                          "".format(size, code))
-            # both is hard code + size converted to ss B64 chars
-            both = f"{code}{intToB64(size, l=ss)}"
-
-            if len(both) % 4 != ps - ls:  # adjusted pad given lead bytes
-                raise InvalidCodeSizeError(f"Invalid code={both} for converted"
-                                           f" raw pad size={ps}.")
-            # prepad, convert, and prepend
-            return (both.encode("utf-8") + encodeB64(bytes([0] * ls) + raw))
-
-        else:  # fixed size so prepad but lead ls may not be zero
-            both = code
-            cs = len(both)
-            if (cs % 4) != ps - ls:  # adjusted pad given lead bytes
-                raise InvalidCodeSizeError(f"Invalid code={both} for converted"
-                                           f" raw pad size={ps}.")
-            # prepad, convert, and replace upfront
-            # when fixed and ls != 0 then cs % 4 is zero and ps==ls
-            # otherwise  fixed and ls == 0 then cs % 4 == ps
-            return (both.encode("utf-8") + encodeB64(bytes([0] * ps) + raw)[cs % 4:])
+        cs = hs + ss
+        # assumes unit tests on Matter.Sizes ensure valid size entries
+
+        if cs != len(both):
+            InvalidCodeSizeError(f"Invalid full code={both} for sizes {hs=} and"
+                                f" {ss=}.")
+
+        if not fs:  # variable sized
+            # Tests on .Sizes table must ensure ls in (0,1,2) and cs % 4 == 0 but
+            # can't know the variable size. So instance methods must ensure that
+            # (ls + rs) % 3 == 0 i.e. both full code (B64) and lead+raw (B2)
+            # are both 24 bit aligned.
+            # If so then should not need following check.
+            if (ls + rs) % 3 or cs % 4:
+                raise InvalidCodeSizeError(f"Invalid full code{both=} with "
+                                           f"variable raw size={rs} given "
+                                           f" {cs=}, {hs=}, {ss=}, {fs=}, and "
+                                           f"{ls=}.")
+
+            # When ls+rs is 24 bit aligned then encodeB64 has no trailing
+            # pad chars that need to be stripped. So simply prepad raw with
+            # ls zero bytes and convert (encodeB64).
+            full = (both.encode("utf-8") + encodeB64(bytes([0] * ls) + raw))
+
+        else:  # fixed size
+            ps = (3 - ((rs + ls) % 3)) % 3  # net pad size given raw with lead
+            # net pad size must equal both code size remainder so that primitive
+            # both + converted padded raw is fs long. Assumes ls in (0,1,2) and
+            # cs % 4 != 3, fs % 4 == 0. Sizes table test must ensure these properties.
+            # If so then should not need following check.
+            if ps != (cs % 4):  # given cs % 4 != 3 then cs % 4 is pad size
+                raise InvalidCodeSizeError(f"Invalid full code{both=} with "
+                                           f"fixed raw size={rs} given "
+                                           f" {cs=}, {hs=}, {ss=}, {fs=}, and "
+                                           f"{ls=}.")
+
+            # Predpad raw so we midpad the full primitive. Prepad with ps+ls
+            # zero bytes ensures encodeB64 of prepad+lead+raw has no trailing
+            # pad characters. Finally skip first ps == cs % 4 of the converted
+            # characters to ensure that when full code is prepended, the full
+            # primitive size is fs but midpad bits are zeros.
+            full = (both.encode("utf-8") + encodeB64(bytes([0] * (ps + ls)) + raw)[ps:])
+
+        if (len(full) % 4) or (fs and len(full) != fs):
+            raise InvalidCodeSizeError(f"Invalid full size given code{both=} "
+                                       f" with raw size={rs}, {cs=}, {hs=}, "
+                                       f"{ss=}, {fs=}, and {ls=}.")
+
+        return full
 
 
     def _binfil(self):
         """
         Returns bytes of fully qualified base2 bytes, that is .qb2
         self.code converted to Base2 + self.raw left shifted with pad bits
         equivalent of Base64 decode of .qb64 into .qb2
         """
-        code = self.code  # codex value
-        size = self.size  # optional size if variable length
-        raw = self.raw  # bytes or bytearray
+        code = self.code  # hard part of full code == codex value
+        both = self.both  # code + soft, soft may be empty
+        raw = self.raw  # bytes or bytearray may be empty
 
         hs, ss, fs, ls = self.Sizes[code]
         cs = hs + ss
-
-        if not fs:  # compute both and fs from size
-            if cs % 4:
-                raise InvalidCodeSizeError("Whole code size not multiple of 4 for "
-                                           "variable length material. cs={}.".format(cs))
-
-            if size < 0 or size > (64 ** ss - 1):
-                raise InvalidVarSizeError("Invalid size={} for code={}."
-                                          "".format(size, code))
-            # both is hard code + converted index
-            both = f"{code}{intToB64(size, l=ss)}"
-            fs = hs + ss + (size * 4)
-        else:
-            both = code
-
-        if len(both) != cs:
-            raise InvalidCodeSizeError("Mismatch code size = {} with table = {}."
-                                       .format(cs, len(code)))
-
+        # assumes unit tests on Matter.Sizes ensure valid size entries
         n = sceil(cs * 3 / 4)  # number of b2 bytes to hold b64 code
         # convert code both to right align b2 int then left shift in pad bits
         # then convert to bytes
         bcode = (b64ToInt(both) << (2 * (cs % 4))).to_bytes(n, 'big')
-        full = bcode + bytes([0] * ls) + raw
+        full = bcode + bytes([0] * ls) + raw  # includes lead bytes
+
         bfs = len(full)
+        if not fs:  # compute fs
+            fs = hs + ss + (len(raw) + ls) * 4 // 3 # hs + ss + (size * 4)
         if bfs % 3 or (bfs * 4 // 3) != fs:  # invalid size
-            raise InvalidCodeSizeError(f"Invalid code={both} for raw size={len(raw)}.")
-
+            raise InvalidCodeSizeError(f"Invalid full code={both} for raw size"
+                                       f"={len(raw)}.")
         return full
 
 
     def _exfil(self, qb64b):
         """
-        Extracts self.code and self.raw from qualified base64 bytes qb64b
+        Extracts self.code and self.raw from qualified base64 str or bytes qb64b
+        Detects is str and converts to bytes
+
+        Parameters:
+            qb64b (str | bytes | bytearray): fully qualified base64 from stream
 
-        cs = hs + ss
-        fs = (size * 4) + cs
         """
         if not qb64b:  # empty need more bytes
             raise ShortageError("Empty material.")
 
         first = qb64b[:1]  # extract first char code selector
         if hasattr(first, "decode"):
             first = first.decode("utf-8")
@@ -1268,68 +1367,53 @@
         if hasattr(hard, "decode"):
             hard = hard.decode("utf-8")  # converts bytes/bytearray to str
         if hard not in self.Sizes:
             raise UnexpectedCodeError(f"Unsupported code ={hard}.")
 
         hs, ss, fs, ls = self.Sizes[hard]  # assumes hs in both tables match
         cs = hs + ss  # both hs and ss
-        size = None
-        if not fs:  # compute fs from size chars in ss part of code
-            if cs % 4:
-                raise ValidationError(f"Whole code size not multiple of 4 for "
-                                      f"variable length material. cs={cs}.")
-            size = qb64b[hs:hs + ss]  # extract size chars
-            if hasattr(size, "decode"):
-                size = size.decode("utf-8")
-            size = b64ToInt(size)  # compute int size
-            fs = (size * 4) + cs
-
-        # assumes that unit tests on Matter and MatterCodex ensure that
-        # .Codes and .Sizes are well formed.
-        # hs consistent and ss == 0 and not fs % 4 and hs > 0 and fs >= hs + ss
-        # unless fs is None
+        # assumes that unit tests on Matter .Sizes .Hards and .Bards ensure that
+        # these are well formed.
+        # when fs is None then ss > 0 otherwise fs > hs + ss when ss > 0
+
+        soft = qb64b[hs:hs + ss]  # extract soft chars, empty when ss==0
+        if hasattr(soft, "decode"):
+            soft = soft.decode("utf-8")
+
+        if not fs:  # compute fs from soft from ss part which provides size B64
+            # compute variable size as int may have value 0
+            fs = (b64ToInt(soft) * 4) + cs
 
         if len(qb64b) < fs:  # need more bytes
             raise ShortageError(f"Need {fs - len(qb64b)} more chars.")
 
         qb64b = qb64b[:fs]  # fully qualified primitive code plus material
         if hasattr(qb64b, "encode"):  # only convert extracted chars from stream
             qb64b = qb64b.encode("utf-8")
 
-        # check for non-zeroed pad bits or lead bytes
-        ps = cs % 4  # code pad size ps = cs mod 4
-        pbs = 2 * (ps if ps else ls)  # pad bit size in bits
-        if ps:  # ps. IF ps THEN not ls (lead) and vice versa OR not ps and not ls
-            base = ps * b'A' + qb64b[cs:]  # replace pre code with prepad chars of zero
-            paw = decodeB64(base)  # decode base to leave prepadded raw
-            pi = (int.from_bytes(paw[:ps], "big"))  # prepad as int
-            if pi & (2 ** pbs - 1 ):  # masked pad bits non-zero
-                raise ValueError(f"Non zeroed prepad bits = "
-                                 f"{pi & (2 ** pbs - 1 ):<06b} in {qb64b[cs:cs+1]}.")
-            raw = paw[ps:]  # strip off ps prepad paw bytes
-
-        else:  # not ps. IF not ps THEN may or may not be ls (lead)
-            base = qb64b[cs:]  # strip off code leaving lead chars if any and value
-            # decode lead chars + val leaving lead bytes + raw bytes
-            # then strip off ls lead bytes leaving raw
-            paw = decodeB64(base) # decode base to leave prepadded paw bytes
-            li = int.from_bytes(paw[:ls], "big")  # lead as int
-            if li:  # pre pad lead bytes must be zero
-                if ls == 1:
-                    raise ValueError(f"Non zeroed lead byte = 0x{li:02x}.")
-                else:
-                    raise ValueError(f"Non zeroed lead bytes = 0x{li:04x}.")
-            raw = paw[ls:]  # paw is bytes so raw is bytes
+        # check for non-zeroed pad bits and/or lead bytes
+        # net prepad ps == cs % 4 (remainer).  Assumes ps != 3 i.e ps in (0,1,2)
+        # To ensure number of prepad bytes and prepad chars are same.
+        # need net prepad chars ps to invert using decodeB64 of lead + raw
+
+        ps = cs % 4  # net prepad bytes to ensure 24 bit align when encodeB64
+        base =  ps * b'A' + qb64b[cs:]  # prepad ps 'A's to  B64 of (lead + raw)
+        paw = decodeB64(base)  # now should have ps + ls leading sextexts of zeros
+        raw = paw[ps+ls:]  # remove prepad midpat bytes to invert back to raw
+        # ensure midpad bytes are zero
+        pi = int.from_bytes(paw[:ps+ls], "big")
+        if pi != 0:
+            raise ConversionError(f"Nonzero midpad bytes=0x{pi:0{(ps + ls) * 2}x}.")
 
         if len(raw) != ((len(qb64b) - cs) * 3 // 4) - ls:  # exact lengths
             raise ConversionError(f"Improperly qualified material = {qb64b}")
 
         self._code = hard  # hard only
-        self._size = size
-        self._raw = raw  # ensure bytes so immutable and for crypto ops
+        self._soft = soft  # soft only
+        self._raw = raw  # ensure bytes for crypto ops, may be empty
 
 
     def _bexfil(self, qb2):
         """
         Extracts self.code and self.raw from qualified base2 qb2
 
         Parameters:
@@ -1356,76 +1440,75 @@
 
         hard = codeB2ToB64(qb2, hs)  # extract and convert hard part of code
         if hard not in self.Sizes:
             raise UnexpectedCodeError(f"Unsupported code ={hard}.")
 
         hs, ss, fs, ls = self.Sizes[hard]
         cs = hs + ss  # both hs and ss
+        # assumes that unit tests on Matter .Sizes .Hards and .Bards ensure that
+        # these are well formed.
+        # when fs is None then ss > 0 otherwise fs > hs + ss when ss > 0
+
         bcs = sceil(cs * 3 / 4)  # bcs is min bytes to hold cs sextets
-        size = None
-        if not fs:  # compute fs from size chars in ss part of code
-            if cs % 4:
-                raise ValidationError("Whole code size not multiple of 4 for "
-                                      "variable length material. cs={}.".format(cs))
+        if len(qb2) < bcs:  # need more bytes
+            raise ShortageError("Need {} more bytes.".format(bcs - len(qb2)))
+
+        both = codeB2ToB64(qb2, cs)  # extract and convert both hard and soft part of code
+        soft = both[hs:hs + ss]  # get soft may be empty
 
+        if not fs:  # compute fs from size chars in ss part of code
             if len(qb2) < bcs:  # need more bytes
                 raise ShortageError("Need {} more bytes.".format(bcs - len(qb2)))
 
-            both = codeB2ToB64(qb2, cs)  # extract and convert both hard and soft part of code
-            size = b64ToInt(both[hs:hs + ss])  # get size
-            fs = (size * 4) + cs
-
-        # assumes that unit tests on Matter and MatterCodex ensure that
-        # .Codes and .Sizes are well formed.
-        # hs consistent and ss == 0 and not fs % 4 and hs > 0 and
-        # (fs >= hs + ss if fs is not None else True)
+            # compute size as int from soft part given by ss B64 chars
+            fs = (b64ToInt(soft) * 4) + cs  # compute fs
 
         bfs = sceil(fs * 3 / 4)  # bfs is min bytes to hold fs sextets
         if len(qb2) < bfs:  # need more bytes
             raise ShortageError("Need {} more bytes.".format(bfs - len(qb2)))
 
         qb2 = qb2[:bfs]  # extract qb2 fully qualified primitive code plus material
-        # check for non-zeroed prepad bits or lead bytes
-        ps = cs % 4  # code pad size ps = cs mod 4
-        pbs = 2 * (ps if ps else ls)  # pad bit size in bits
-        if ps:  # ps. IF ps THEN not ls (lead) and vice versa OR not ps and not ls
-            # convert last byte of code bytes in which are pad bits to int
-            pi = (int.from_bytes(qb2[bcs-1:bcs], "big"))
-            if pi & (2 ** pbs - 1 ):  # masked pad bits non-zero
-                raise ValueError(f"Non zeroed pad bits = "
-                                 f"{pi & (2 ** pbs - 1 ):>08b} in 0x{pi:02x}.")
-        else:  # not ps. IF not ps THEN may or may not be ls (lead)
-            li = int.from_bytes(qb2[bcs:bcs+ls], "big")  # lead as int
-            if li:  # pre pad lead bytes must be zero
-                if ls == 1:
-                    raise ValueError(f"Non zeroed lead byte = 0x{li:02x}.")
-                else:
-                    raise ValueError(f"Non zeroed lead bytes = 0x{li:02x}.")
 
-        raw = qb2[(bcs + ls):]  # strip code and leader bytes from qb2 to get raw
+        # check for nonzero trailing full code mid pad bits
+        ps = cs % 4  # full code (both) net pad size for 24 bit alignment
+        pbs = 2 * ps  # mid pad bits = 2 per net pad
+        # get pad bits in last byte of full code
+        pi = (int.from_bytes(qb2[bcs-1:bcs], "big")) # convert byte to int
+        pi = pi & (2 ** pbs - 1 ) # mask with 1's in pad bit locations
+        if pi:  # not zero so raise error
+            raise ConversionError(f"Nonzero code mid pad bits=0b{pi:0{pbs}b}.")
+
+        # check nonzero leading mid pad lead bytes in lead + raw
+        li = int.from_bytes(qb2[bcs:bcs+ls], "big")  # lead as int
+        if li:  # midpad lead bytes must be zero
+            raise ConversionError(f"Nonzero lead midpad bytes=0x{li:0{ls*2}x}.")
+
+        # strip code and leader bytes from qb2 to get raw
+        raw = qb2[(bcs + ls):]  # may be empty
 
         if len(raw) != (len(qb2) - bcs - ls):  # exact lengths
             raise ConversionError(r"Improperly qualified material = {qb2}")
 
-        self._code = hard
-        self._size = size
-        self._raw = bytes(raw)  # ensure bytes so immutable and crypto operations
+        self._code = hard  # hard only
+        self._soft = soft  # soft only may be empty
+        self._raw = bytes(raw)  # ensure bytes for crypto ops may be empty
 
 
 class Seqner(Matter):
     """
-    Seqner is subclass of Matter, cryptographic material, for ordinal numbers
-    such as sequence numbers or first seen ordering numbers.
-    Seqner provides fully qualified format for ordinals (sequence numbers etc)
-    when provided as attached cryptographic material elements.
+    Seqner is subclass of Matter, cryptographic material, for fully qualified
+    fixed serialization sized ordinal numbers such as sequence numbers or
+    first seen numbers.
+
+    The serialization is forced to a fixed size (single code) so that it may be
+    used  for lexocographically ordered namespaces such as database indices.
+    That code is MtrDex.Salt_128
 
-    Useful when parsing attached receipt groupings with sn from stream or database
-
-    Uses default initialization code = CryTwoDex.Salt_128
-    Raises error on init if code not CryTwoDex.Salt_128
+    Default initialization code = MtrDex.Salt_128
+    Raises error on init if code is not MtrDex.Salt_128
 
     Attributes:
 
     Inherited Properties:  (See Matter)
         .pad  is int number of pad chars given raw
         .code is  str derivation code to indicate cypher suite
         .raw is bytes crypto material only without code
@@ -1443,18 +1526,16 @@
         ._pad is method to compute  .pad property
         ._code is str value for .code property
         ._raw is bytes value for .raw property
         ._index is int value for .index property
         ._infil is method to compute fully qualified Base64 from .raw and .code
         ._exfil is method to extract .code and .raw from fully qualified Base64
 
-
     Methods:
 
-
     """
 
     def __init__(self, raw=None, qb64b=None, qb64=None, qb2=None,
                  code=MtrDex.Salt_128, sn=None, snh=None, **kwa):
         """
         Inherited Parameters:  (see Matter)
             raw is bytes of unqualified crypto material usable for crypto operations
@@ -1462,34 +1543,51 @@
             qb64 is str or bytes  of fully qualified crypto material
             qb2 is bytes of fully qualified crypto material
             code is str of derivation code
             index is int of count of attached receipts for CryCntDex codes
 
 
         Parameters:
-            sn is int sequence number or some form of ordinal number
-            snh is hex string of sequence number
+            sn (int | str | None): some form of ordinal number int or hex str
+            snh (str | None): hex string of ordinal number
 
         """
         if raw is None and qb64b is None and qb64 is None and qb2 is None:
-            if sn is None:
-                if snh is None:
-                    sn = 0
-                else:
-                    sn = int(snh, 16)
+            try:
+                if sn is None:
+                    if snh is None or snh == '':
+                        sn = 0
+                    else:
+                        sn = int(snh, 16)
+
+                else:  # sn is not None but so may be hex str
+                    if isinstance(sn, str):  # is it a hex str
+                        if sn == '':
+                            sn = 0
+                        else:
+                            sn = int(sn, 16)
+            except ValueError as ex:
+                raise InvalidValueError(f"Not whole number={sn} .") from ex
+
+            if not isinstance(sn, int) or sn < 0:
+                raise InvalidValueError(f"Not whole number={sn}.")
+
+            if sn > MaxON:  # too big for ordinal 256 ** 16 - 1
+                raise ValidationError(f"Non-ordinal {sn} exceeds {MaxON}.")
 
             raw = sn.to_bytes(Matter._rawSize(MtrDex.Salt_128), 'big')
 
         super(Seqner, self).__init__(raw=raw, qb64b=qb64b, qb64=qb64, qb2=qb2,
                                      code=code, **kwa)
 
         if self.code != MtrDex.Salt_128:
             raise ValidationError("Invalid code = {} for Seqner."
                                   "".format(self.code))
 
+
     @property
     def sn(self):
         """
         Property sn: sequence number as int
         Returns .raw converted to int
         """
         return int.from_bytes(self.raw, 'big')
@@ -1499,14 +1597,15 @@
         """
         Property snh:  sequence number as hex
         Returns .sn int converted to hex str
         """
         return f"{self.sn:x}"  # "{:x}".format(self.sn)
 
 
+
 class Number(Matter):
     """
     Number is subclass of Matter, cryptographic material, for ordinal counting
     whole numbers  (non-negative integers) up to a maximum size of 16 bytes,
     256 ** 16 - 1.
     Examples uses are sequence numbers or first seen ordering numbers or thresholds.
     Seqner provides fully qualified format for ordinals (sequence numbers etc)
@@ -1579,43 +1678,45 @@
         """
         if raw is None and qb64b is None and qb64 is None and qb2 is None:
             try:
                 if num is None:
                     if numh is None or numh == '':
                         num = 0
                     else:
-                        #if len(numh) > 32:
-                            #raise InvalidValueError(f"Hex numh={numh} str too long.")
                         num = int(numh, 16)
 
                 else:  # handle case where num is hex str'
                     if isinstance(num, str):
                         if num == '':
                             num = 0
                         else:
-                            #if len(num) > 32:
-                                #raise InvalidValueError(f"Hex num={num} str too long.")
                             num = int(num, 16)
             except ValueError as ex:
-                raise InvalidValueError(f"Invalid whole number={num} .") from ex
+                raise InvalidValueError(f"Not whole number={num} .") from ex
 
             if not isinstance(num, int) or num < 0:
-                raise InvalidValueError(f"Invalid whole number={num}.")
+                raise InvalidValueError(f"Not whole number={num}.")
 
             if num <= (256 ** 2 - 1):  # make short version of code
                 code = NumDex.Short
 
-            elif num <= (256 ** 4 - 1):  # make long version of code
-                code = code = NumDex.Long
+            elif num <= (256 ** 5 - 1):  # make tall version of code
+                code = code = NumDex.Tall
 
             elif num <= (256 ** 8 - 1):  # make big version of code
                 code = code = NumDex.Big
 
-            elif num <= (256 ** 16 - 1):  # make huge version of code
-                code = code = NumDex.Huge
+            elif num <= (256 ** 11 - 1):  # make large version of code
+                code = code = NumDex.Large
+
+            elif num <= (256 ** 14 - 1):  # make great version of code
+                code = code = NumDex.Great
+
+            elif num <= (256 ** 17 - 1):  # make vast version of code
+                code = code = NumDex.Vast
 
             else:
                 raise InvalidValueError(f"Invalid num = {num}, too large to encode.")
 
             # default to_bytes parameter signed is False. If negative raises
             # OverflowError: can't convert negative int to unsigned
             raw = num.to_bytes(Matter._rawSize(code), 'big')  # big endian unsigned
@@ -1623,14 +1724,52 @@
         super(Number, self).__init__(raw=raw, qb64b=qb64b, qb64=qb64, qb2=qb2,
                                      code=code, **kwa)
 
         if self.code not in NumDex:
             raise ValidationError(f"Invalid code = {self.code} for Number.")
 
 
+    def validate(self, inceptive=None):
+        """
+        Returns:
+            self (Number):
+
+        Raises:
+            ValidationError: when .num is invalid ordinal such as
+               sequence number or first seen number etc.
+
+        Parameters:
+           inceptive(bool): raise ValidationError whan .num invalid
+                            None means exception when .num < 0
+                            True means exception when .num != 0
+                            False means exception when .num < 1
+
+        """
+        num = self.num
+
+        if num > MaxON:  # too big for ordinal 256 ** 16 - 1
+            raise ValidationError(f"Non-ordinal {num} exceeds {MaxON}.")
+
+        if inceptive is not None:
+            if inceptive:
+                if num != 0:
+                    raise ValidationError(f"Nonzero num = {num} non-inceptive"
+                                          f" ordinal.")
+            else:
+                if num < 1:
+                    raise ValidationError(f"Non-positive num = {num} not "
+                                          f"non-inceptive ordinal.")
+        else:
+            if num < 0:
+                raise ValidationError(f"Negative num = {num} non-ordinal.")
+
+        return self
+
+
+
     @property
     def num(self):
         """
         Property num: number as int
         Returns .raw converted to int
         """
         return int.from_bytes(self.raw, 'big')
@@ -1658,34 +1797,43 @@
         """Sequence number hex str, snh property getter to mimic Seqner interface
         Returns:
             snh (hex str): alias for numh
         """
         return self.numh
 
 
-
     @property
     def positive(self):
         """
         Returns True if .num is strictly positive non-zero False otherwise.
         Because valid number .num must be non-negative, positive False also means
         that .num is zero.
         """
         return True if self.num > 0 else False
 
+
     @property
     def inceptive(self):
         """
         Returns True if .num == 0 False otherwise.
-        Because valid number .num must be non-negative, positive False means
-        that .num is zero.
+        Valid number .num must be non-negative,
         """
         return True if self.num == 0 else False
 
 
+    @property
+    def seqner(self):
+        """Seqner getter.
+
+        Returns:
+            seqner (Seqner): instance made from number
+        """
+        return Seqner(sn=self.sn)
+
+
 class Dater(Matter):
     """
     Dater is subclass of Matter, cryptographic material, for RFC-3339 profile of
     ISO-8601 formatted datetimes.
 
     Dater provides a custom Base64 coding of an ASCII RFC-3339 profile of an
     ISO-8601 datetime by replacing (using translate) the three non-Base64 characters,
@@ -1770,16 +1918,15 @@
 
         Parameters:
             dts is the ISO-8601 datetime as str or bytes
         """
         if raw is None and qb64b is None and qb64 is None and qb2 is None:
             if dts is None:  # defaults to now
                 dts = helping.nowIso8601()
-            # if len(dts) != 32:
-            #     raise ValueError("Invalid length of date time string")
+
             if hasattr(dts, "decode"):
                 dts = dts.decode("utf-8")
             qb64 = MtrDex.DateTime + dts.translate(self.ToB64)
 
         super(Dater, self).__init__(raw=raw, qb64b=qb64b, qb64=qb64, qb2=qb2,
                                     code=code, **kwa)
         if self.code != MtrDex.DateTime:
@@ -1807,14 +1954,599 @@
         """
         Property datetime:
         Returns datetime.datetime instance converted from .dts
         """
         return helping.fromIso8601(self.dts)
 
 
+class Tagger(Matter):
+    """
+    Tagger is subclass of Matter, cryptographic material, for compact special
+    fixed size primitive with non-empty soft part and empty raw part.
+
+    Tagger provides a more compact representation of small Base64 values in
+    as soft part of code rather than would be obtained by by using a small raw
+    part whose ASCII representation is converted to Base64.
+
+    Attributes:
+
+    Inherited Properties:  (See Matter)
+        code (str): hard part of derivation code to indicate cypher suite
+        hard (str): hard part of derivation code. alias for code
+        soft (str): soft part of derivation code fs any.
+                    Empty when ss = 0.
+        both (str): hard + soft parts of full text code
+        size (int | None): Number of quadlets/triplets of chars/bytes including
+                            lead bytes of variable sized material (fs = None).
+                            Converted value of the soft part (of len ss) of full
+                            derivation code.
+                          Otherwise None when not variably sized (fs != None)
+        fullSize (int): full size of primitive
+        raw (bytes): crypto material only. Not derivation code or lead bytes.
+        qb64 (str): Base64 fully qualified with derivation code + crypto mat
+        qb64b (bytes): Base64 fully qualified with derivation code + crypto mat
+        qb2  (bytes): binary with derivation code + crypto material
+        transferable (bool): True means transferable derivation code False otherwise
+        digestive (bool): True means digest derivation code False otherwise
+        prefixive (bool): True means identifier prefix derivation code False otherwise
+        special (bool): True when soft is special raw is empty and fixed size
+        composable (bool): True when .qb64b and .qb2 are 24 bit aligned and round trip
+
+    Properties:
+        tag (str): B64 primitive without prepad (strips prepad from soft)
+
+
+    Inherited Hidden:  (See Matter)
+        _code (str): value for .code property
+        _soft (str): soft value of full code
+        _raw (bytes): value for .raw property
+        _rawSize():
+        _leadSize():
+        _special():
+        _infil(): creates qb64b from .raw and .code (fully qualified Base64)
+        _binfil(): creates qb2 from .raw and .code (fully qualified Base2)
+        _exfil(): extracts .code and .raw from qb64b (fully qualified Base64)
+        _bexfil(): extracts .code and .raw from qb2 (fully qualified Base2)
+
+
+    Hidden:
+
+
+    Methods:
+
+    def __init__(self, raw=None, code=MtrDex.Ed25519N, soft='', rize=None,
+                 qb64b=None, qb64=None, qb2=None, strip=False):
+
+    """
+    Pad = '_'  # B64 pad char for tag codes with pre-padded soft values
+
+    def __init__(self, tag='', soft='', code=None, **kwa):
+        """
+        Inherited Parameters:  (see Matter)
+            raw (bytes | bytearray | None): unqualified crypto material usable
+                    for crypto operations.
+            code (str): stable (hard) part of derivation code
+            soft (str | bytes): soft part for special codes
+            rize (int | None): raw size in bytes when variable sized material not
+                        including lead bytes if any
+                        Otherwise None
+            qb64b (bytes | None): fully qualified crypto material Base64
+            qb64 (str | bytes | None):  fully qualified crypto material Base64
+            qb2 (bytes | None): fully qualified crypto material Base2
+            strip (bool): True means strip (delete) matter from input stream
+                bytearray after parsing qb64b or qb2. False means do not strip
+
+        Parameters:
+            tag (str | bytes):  Base64 plain. Prepad is added as needed.
+
+        """
+        if tag:
+            if hasattr(tag, "decode"):  # make tag str
+                tag = tag.decode("utf-8")
+            if not Reb64.match(tag.encode("utf-8")):
+                raise InvalidSoftError(f"Non Base64 chars in {tag=}.")
+            codes = astuple(TagDex)
+            l = len(tag)  # soft not empty so l > 0
+            if l > len(codes):
+                raise InvalidSoftError("Oversized tag={soft}.")
+            code = codes[l-1]  # get code for size of soft
+            if code in PadTagDex:
+                soft = self.Pad + tag # pre pad for those that need it
+            else:
+                soft = tag
+
+
+        super(Tagger, self).__init__(soft=soft, code=code, **kwa)
+
+        if (not self._special(self.code)) or self.code not in TagDex:
+            raise InvalidCodeError(f"Invalid code={self.code} for Tagger.")
+
+    @property
+    def tag(self):
+        """Returns:
+                tag (str): B64 primitive without prepad (strips prepad from soft)
+
+        """
+        tag = self.soft
+        if self.code in PadTagDex:
+            pad = self.soft[0]
+            tag = self.soft[1:]
+            if pad != self.Pad:
+                raise  InvalidSoftError("Invaid pre {pad=} for {tag=}.")
+
+        return tag
+
+
+class Ilker(Tagger):
+    """
+    Ilker is subclass of Tagger, cryptographic material, for formatted
+    message types (ilks) in Base64. Leverages Tagger support compact special
+    fixed size primitives with non-empty soft part and empty raw part.
+
+    Ilker provides a more compact representation than would be obtained by
+    converting the raw ASCII representation to Base64.
+
+    Attributes:
+
+    Inherited Properties:  (See Tagger)
+        code (str): hard part of derivation code to indicate cypher suite
+        hard (str): hard part of derivation code. alias for code
+        soft (str): soft part of derivation code fs any.
+                    Empty when ss = 0.
+        both (str): hard + soft parts of full text code
+        size (int | None): Number of quadlets/triplets of chars/bytes including
+                            lead bytes of variable sized material (fs = None).
+                            Converted value of the soft part (of len ss) of full
+                            derivation code.
+                          Otherwise None when not variably sized (fs != None)
+        fullSize (int): full size of primitive
+        raw (bytes): crypto material only. Not derivation code or lead bytes.
+        qb64 (str): Base64 fully qualified with derivation code + crypto mat
+        qb64b (bytes): Base64 fully qualified with derivation code + crypto mat
+        qb2  (bytes): binary with derivation code + crypto material
+        transferable (bool): True means transferable derivation code False otherwise
+        digestive (bool): True means digest derivation code False otherwise
+        prefixive (bool): True means identifier prefix derivation code False otherwise
+        special (bool): True when soft is special raw is empty and fixed size
+        composable (bool): True when .qb64b and .qb2 are 24 bit aligned and round trip
+        tag (str): B64 primitive without prepad (strips prepad from soft)
+
+
+    Properties:
+        ilk (str):  message type from Ilks of Ilkage
+
+    Inherited Hidden:  (See Tagger)
+        _code (str): value for .code property
+        _soft (str): soft value of full code
+        _raw (bytes): value for .raw property
+        _rawSize():
+        _leadSize():
+        _special():
+        _infil(): creates qb64b from .raw and .code (fully qualified Base64)
+        _binfil(): creates qb2 from .raw and .code (fully qualified Base2)
+        _exfil(): extracts .code and .raw from qb64b (fully qualified Base64)
+        _bexfil(): extracts .code and .raw from qb2 (fully qualified Base2)
+
+    Hidden:
+
+
+    Methods:
+
+    """
+
+
+    def __init__(self, qb64b=None, qb64=None, qb2=None, tag='', ilk='', **kwa):
+        """
+        Inherited Parameters:  (see Tagger)
+            raw (bytes | bytearray | None): unqualified crypto material usable
+                    for crypto operations.
+            code (str): stable (hard) part of derivation code
+            soft (str | bytes): soft part for special codes
+            rize (int | None): raw size in bytes when variable sized material not
+                        including lead bytes if any
+                        Otherwise None
+            qb64b (bytes | None): fully qualified crypto material Base64
+            qb64 (str | bytes | None):  fully qualified crypto material Base64
+            qb2 (bytes | None): fully qualified crypto material Base2
+            strip (bool): True means strip (delete) matter from input stream
+                bytearray after parsing qb64b or qb2. False means do not strip
+            tag (str | bytes):  Base64 plain. Prepad is added as needed.
+
+        Parameters:
+            ilk (str):  message type from Ilks of Ilkage
+
+        """
+        if not (qb64b or qb64 or qb2):
+            if ilk:
+                tag = ilk
+
+
+        super(Ilker, self).__init__(qb64b=qb64b, qb64=qb64, qb2=qb2, tag=tag, **kwa)
+
+        if self.code not in (MtrDex.Tag3, ):
+            raise InvalidCodeError(f"Invalid code={self.code} for Ilker "
+                                   f"{self.ilk=}.")
+        if self.ilk not in Ilks:
+            raise InvalidSoftError(f"Ivalid ilk={self.ilk} for Ilker.")
+
+
+
+    @property
+    def ilk(self):
+        """Returns:
+                tag (str): B64 primitive without prepad (strips prepad from soft)
+
+        Alias for self.tag
+
+        """
+        return self.tag
+
+
+class Traitor(Tagger):
+    """
+    Traitor is subclass of Tagger, cryptographic material, for formatted
+    configuration traits for key events in Base64. Leverages Tagger support of
+    compact special fixed size primitives with non-empty soft part and empty raw part.
+
+    Traitor provides a more compact representation than would be obtained by
+    converting the raw ASCII representation to Base64.
+
+    Attributes:
+
+    Inherited Properties:  (See Tagger)
+        code (str): hard part of derivation code to indicate cypher suite
+        hard (str): hard part of derivation code. alias for code
+        soft (str): soft part of derivation code fs any.
+                    Empty when ss = 0.
+        both (str): hard + soft parts of full text code
+        size (int | None): Number of quadlets/triplets of chars/bytes including
+                            lead bytes of variable sized material (fs = None).
+                            Converted value of the soft part (of len ss) of full
+                            derivation code.
+                          Otherwise None when not variably sized (fs != None)
+        fullSize (int): full size of primitive
+        raw (bytes): crypto material only. Not derivation code or lead bytes.
+        qb64 (str): Base64 fully qualified with derivation code + crypto mat
+        qb64b (bytes): Base64 fully qualified with derivation code + crypto mat
+        qb2  (bytes): binary with derivation code + crypto material
+        transferable (bool): True means transferable derivation code False otherwise
+        digestive (bool): True means digest derivation code False otherwise
+        prefixive (bool): True means identifier prefix derivation code False otherwise
+        special (bool): True when soft is special raw is empty and fixed size
+        composable (bool): True when .qb64b and .qb2 are 24 bit aligned and round trip
+        tag (str): B64 primitive without prepad (strips prepad from soft)
+
+
+    Properties:
+        trait (str):  configuration trait B64 from TraitDex
+
+    Inherited Hidden:  (See Tagger)
+        _code (str): value for .code property
+        _soft (str): soft value of full code
+        _raw (bytes): value for .raw property
+        _rawSize():
+        _leadSize():
+        _special():
+        _infil(): creates qb64b from .raw and .code (fully qualified Base64)
+        _binfil(): creates qb2 from .raw and .code (fully qualified Base2)
+        _exfil(): extracts .code and .raw from qb64b (fully qualified Base64)
+        _bexfil(): extracts .code and .raw from qb2 (fully qualified Base2)
+
+    Hidden:
+
+
+    Methods:
+
+    """
+
+
+    def __init__(self, qb64b=None, qb64=None, qb2=None, tag='', trait='', **kwa):
+        """
+        Inherited Parameters:  (see Tagger)
+            raw (bytes | bytearray | None): unqualified crypto material usable
+                    for crypto operations.
+            code (str): stable (hard) part of derivation code
+            soft (str | bytes): soft part for special codes
+            rize (int | None): raw size in bytes when variable sized material not
+                        including lead bytes if any
+                        Otherwise None
+            qb64b (bytes | None): fully qualified crypto material Base64
+            qb64 (str | bytes | None):  fully qualified crypto material Base64
+            qb2 (bytes | None): fully qualified crypto material Base2
+            strip (bool): True means strip (delete) matter from input stream
+                bytearray after parsing qb64b or qb2. False means do not strip
+            tag (str | bytes):  Base64 plain. Prepad is added as needed.
+
+        Parameters:
+            trait (str):  configuration trait B64 from TraitDex
+
+        """
+        if not (qb64b or qb64 or qb2):
+            if trait:
+                tag = trait
+
+
+        super(Traitor, self).__init__(qb64b=qb64b, qb64=qb64, qb2=qb2, tag=tag, **kwa)
+
+
+        if self.trait not in TraitDex:
+            raise InvalidSoftError(f"Invalid trait={self.trait} for Traitor.")
+
+
+
+    @property
+    def trait(self):
+        """Returns:
+                trait (str): B64 primitive without prepad (strips prepad from soft)
+
+        Alias for self.tag
+
+        """
+        return self.tag
+
+
+
+
+# Versage namedtuple
+# proto (str): protocol element of Protocols
+# vrsn (Versionage): instance protocol version namedtuple (major, minor) ints
+# vrsn (Versionage | None): instance genus version namedtuple (major, minor) ints
+Versage = namedtuple("Versage", "proto vrsn gvrsn", defaults=(None, ))
+
+
+class Verser(Tagger):
+    """
+    Verser is subclass of Tagger, cryptographic material, for formatted
+    version primitives in Base64. Leverages Tagger support compact special
+    fixed size primitives with non-empty soft part and empty raw part.
+
+    Verser provides a more compact representation than would be obtained by
+    converting the raw ASCII representation to Base64.
+
+    Attributes:
+
+    Inherited Properties:  (See Tagger)
+        code (str): hard part of derivation code to indicate cypher suite
+        hard (str): hard part of derivation code. alias for code
+        soft (str): soft part of derivation code fs any.
+                    Empty when ss = 0.
+        both (str): hard + soft parts of full text code
+        size (int | None): Number of quadlets/triplets of chars/bytes including
+                            lead bytes of variable sized material (fs = None).
+                            Converted value of the soft part (of len ss) of full
+                            derivation code.
+                          Otherwise None when not variably sized (fs != None)
+        fullSize (int): full size of primitive
+        raw (bytes): crypto material only. Not derivation code or lead bytes.
+        qb64 (str): Base64 fully qualified with derivation code + crypto mat
+        qb64b (bytes): Base64 fully qualified with derivation code + crypto mat
+        qb2  (bytes): binary with derivation code + crypto material
+        transferable (bool): True means transferable derivation code False otherwise
+        digestive (bool): True means digest derivation code False otherwise
+        prefixive (bool): True means identifier prefix derivation code False otherwise
+        special (bool): True when soft is special raw is empty and fixed size
+        composable (bool): True when .qb64b and .qb2 are 24 bit aligned and round trip
+        tag (str): B64 primitive without prepad (strips prepad from soft)
+
+
+    Properties:
+        versage (Versage):  named tuple of (proto, vrsn, gvrsn)
+
+    Inherited Hidden:  (See Tagger)
+        _code (str): value for .code property
+        _soft (str): soft value of full code
+        _raw (bytes): value for .raw property
+        _rawSize():
+        _leadSize():
+        _special():
+        _infil(): creates qb64b from .raw and .code (fully qualified Base64)
+        _binfil(): creates qb2 from .raw and .code (fully qualified Base2)
+        _exfil(): extracts .code and .raw from qb64b (fully qualified Base64)
+        _bexfil(): extracts .code and .raw from qb2 (fully qualified Base2)
+
+    Hidden:
+
+
+    Methods:
+
+    """
+
+
+    def __init__(self, qb64b=None, qb64=None, qb2=None, versage=None,
+                 proto=Protocols.keri, vrsn=Vrsn_2_0, gvrsn=None, tag='', **kwa):
+        """
+        Inherited Parameters:  (see Tagger)
+            raw (bytes | bytearray | None): unqualified crypto material usable
+                    for crypto operations.
+            code (str): stable (hard) part of derivation code
+            soft (str | bytes): soft part for special codes
+            rize (int | None): raw size in bytes when variable sized material not
+                        including lead bytes if any
+                        Otherwise None
+            qb64b (bytes | None): fully qualified crypto material Base64
+            qb64 (str | bytes | None):  fully qualified crypto material Base64
+            qb2 (bytes | None): fully qualified crypto material Base2
+            strip (bool): True means strip (delete) matter from input stream
+                bytearray after parsing qb64b or qb2. False means do not strip
+            tag (str | bytes):  Base64 plain. Prepad is added as needed.
+
+        Parameters:
+            versage (Versage | None): namedtuple of (proto, vrsn, gvrsn)
+            proto (str | None): protocol from Protocols
+            vrsn  (Versionage | None): instance protocol version.
+               namedtuple (major, minor) of ints
+            gvrsn (Versionage | None): instance genus version.
+               namedtuple (major, minor) of ints
+
+        """
+        if not (qb64b or qb64 or qb2):
+            if versage:
+                proto, vrsn, gvrsn = versage
+
+            tag = proto + self.verToB64(vrsn)
+
+            if gvrsn:
+                tag += self.verToB64(gvrsn)
+
+        super(Verser, self).__init__(qb64b=qb64b, qb64=qb64, qb2=qb2, tag=tag, **kwa)
+
+        if self.code not in (MtrDex.Tag7, MtrDex.Tag10, ):
+            raise InvalidCodeError(f"Invalid code={self.code} for "
+                                   f"Verser={self.tag}.")
+
+
+    @property
+    def versage(self):
+        """Returns:
+            versage (Versage):  named tuple of (proto, vrsn, gvrsn)
+
+        """
+        gvrsn = None
+        proto = self.tag[:4]
+        vrsn = self.b64ToVer(self.tag[4:7])
+        gvrsn = self.b64ToVer(self.tag[7:10]) if len(self.tag) == 10 else None
+
+        return Versage(proto=proto, vrsn=vrsn, gvrsn=gvrsn)
+
+
+    @staticmethod
+    def verToB64(version=None, *, text="", major=0, minor=0):
+        """ Converts version to Base64 representation
+
+        Returns:
+            verB64 (str):
+
+        Example:
+            Verser.verToB64(verstr = "1.0"))
+
+        Parameters:
+            version (Versionage): instange of namedtuple
+                         Versionage(major=major,minor=minor)
+            text (str): text format of version as dotted decimal "major.minor"
+            major (int): When version is None and verstr is empty then use major minor
+                        range [0, 63] for one Base64 character
+            minor (int): When version is None and verstr is  empty then use major minor
+                        range [0, 4095] for two Base64 characters
+
+        """
+        if version:
+            major = version.major
+            minor = version.minor
+
+        elif text:
+            splits = text.split(".", maxsplit=2)
+            splits = [(int(s) if s else 0) for s in splits]
+            parts = [major, minor]
+            for i in range(2-len(splits),0, -1):  # append missing minor and/or major
+                splits.append(parts[-i])
+            major = splits[0]
+            minor = splits[1]
+
+        if major < 0 or major > 63 or minor < 0 or minor > 4095:
+                raise ValueError(f"Out of bounds version = {major}.{minor}.")
+
+        return (f"{intToB64(major)}{intToB64(minor, l=2)}")
+
+
+    @staticmethod
+    def b64ToVer(b64, *, texted=False):
+        """ Converts Base64 representation of version to Versionage or
+        text dotted decimal format
+
+        default is Versionage
+
+        Returns:
+            version (Versionage | str):
+
+        Example:
+            .b64ToVer("BAA"))
+
+        Parameters:
+            b64 (str): base64 string of three characters Mmm for Major minor
+            texted (bool): return text format dotted decimal string
+
+
+        """
+        if not Reb64.match(b64.encode("utf-8")):
+            raise ValueError("Invalid Base64.")
+
+        if texted:
+            return ".".join([f"{b64ToInt(b64[0])}", f"{b64ToInt(b64[1:3])}"])
+
+        return Versionage(major=b64ToInt(b64[0]), minor=b64ToInt(b64[1:3]))
+
+
+
+
+
+class Texter(Matter):
+    """
+    Texter is subclass of Matter, cryptographic material, for variable length
+    text strings as bytes not unicode. Unicode strings converted to bytes.
+
+
+    Attributes:
+
+    Inherited Properties:  (See Matter)
+
+    Properties:
+        .text is bytes value with CESR code and leader removed.
+        .uext is str value with CESR code and leader removed unicode of .text
+
+    Inherited Hidden Properties:  (See Matter)
+
+    Methods:
+
+    Codes:
+        Bytes_L0:     str = '4B'  # Byte String lead size 0
+        Bytes_L1:     str = '5B'  # Byte String lead size 1
+        Bytes_L2:     str = '6B'  # Byte String lead size 2
+        Bytes_Big_L0: str = '7AAB'  # Byte String big lead size 0
+        Bytes_Big_L1: str = '8AAB'  # Byte String big lead size 1
+        Bytes_Big_L2: str = '9AAB'  # Byte String big lead size 2
+
+    """
+
+    def __init__(self, raw=None, qb64b=None, qb64=None, qb2=None,
+                 code=MtrDex.Bytes_L0, text=None, **kwa):
+        """
+        Inherited Parameters:  (see Matter)
+            raw is bytes of unqualified crypto material usable for crypto operations
+            qb64b is bytes of fully qualified crypto material
+            qb64 is str or bytes  of fully qualified crypto material
+            qb2 is bytes of fully qualified crypto material
+            code is str of derivation code
+            index is int of count of attached receipts for CryCntDex codes
+
+        Parameters:
+            text is the variable sized text string as either bytes or str
+
+        """
+        if raw is None and qb64b is None and qb64 is None and qb2 is None:
+            if text is None:
+                raise EmptyMaterialError("Missing text string.")
+            if hasattr(text, "encode"):
+                text = text.encode("utf-8")
+            raw = text
+
+        super(Texter, self).__init__(raw=raw, qb64b=qb64b, qb64=qb64, qb2=qb2,
+                                     code=code, **kwa)
+        if self.code not in TexDex:
+            raise ValidationError("Invalid code = {} for Texter."
+                                  "".format(self.code))
+
+
+    @property
+    def text(self):
+        """
+        Property text: raw as str
+        """
+        return self.raw.decode('utf-8')
+
+
 class Bexter(Matter):
     """
     Bexter is subclass of Matter, cryptographic material, for variable length
     strings that only contain Base64 URL safe characters, i.e. Base64 text (bext).
     When created using the 'bext' paramaeter, the encoded matter in qb64 format
     in the text domain is more compact than would be the case if the string were
     passed in as raw bytes. The text is used as is to form the value part of the
@@ -1855,36 +2587,30 @@
         CESR encoded paths for nested SADs and SAIDs
         CESR encoded fractionally weighted threshold expressions
 
 
     Attributes:
 
     Inherited Properties:  (See Matter)
-        .pad  is int number of pad chars given raw
-
-        .code is  str derivation code to indicate cypher suite
-        .raw is bytes crypto material only without code
-        .index is int count of attached crypto material by context (receipts)
-        .qb64 is str in Base64 fully qualified with derivation code + crypto mat
-        .qb64b is bytes in Base64 fully qualified with derivation code + crypto mat
-        .qb2  is bytes in binary with derivation code + crypto material
-        .transferable is Boolean, True when transferable derivation code False otherwise
 
     Properties:
-        .text is the Base64 text value, .qb64 with text code and leader removed.
+        .bext is the Base64 text value, .qb64 with text code and leader removed.
 
-    Hidden:
-        ._pad is method to compute  .pad property
-        ._code is str value for .code property
-        ._raw is bytes value for .raw property
-        ._index is int value for .index property
-        ._infil is method to compute fully qualified Base64 from .raw and .code
-        ._exfil is method to extract .code and .raw from fully qualified Base64
+    Inherited Hidden Properties:  (See Matter)
 
     Methods:
+        ._rawify(self, bext)
+
+    Codes:
+        StrB64_L0:     str = '4A'  # String Base64 Only Leader Size 0
+        StrB64_L1:     str = '5A'  # String Base64 Only Leader Size 1
+        StrB64_L2:     str = '6A'  # String Base64 Only Leader Size 2
+        StrB64_Big_L0: str = '7AAA'  # String Base64 Only Big Leader Size 0
+        StrB64_Big_L1: str = '8AAA'  # String Base64 Only Big Leader Size 1
+        StrB64_Big_L2: str = '9AAA'  # String Base64 Only Big Leader Size 2
 
     """
 
     def __init__(self, raw=None, qb64b=None, qb64=None, qb2=None,
                  code=MtrDex.StrB64_L0, bext=None, **kwa):
         """
         Inherited Parameters:  (see Matter)
@@ -1898,18 +2624,18 @@
         Parameters:
             bext is the variable sized Base64 text string
         """
         if raw is None and qb64b is None and qb64 is None and qb2 is None:
             if bext is None:
                 raise EmptyMaterialError("Missing bext string.")
             if hasattr(bext, "encode"):
-                bext = bext.encode("utf-8")
+                bext = bext.encode("utf-8")  # convert to bytes
             if not Reb64.match(bext):
                 raise ValueError("Invalid Base64.")
-            raw = self._rawify(bext)
+            raw = self._rawify(bext)  # convert bytes to raw with padding
 
         super(Bexter, self).__init__(raw=raw, qb64b=qb64b, qb64=qb64, qb2=qb2,
                                      code=code, **kwa)
         if self.code not in BexDex:
             raise ValidationError("Invalid code = {} for Bexter."
                                   "".format(self.code))
 
@@ -2516,30 +3242,30 @@
         if index is None:  # Must be Cigar i.e. non-indexed signature
             return Cigar(raw=sig, code=MtrDex.Ed25519_Sig, verfer=verfer)
         else:  # Must be Siger i.e. indexed signature
             # should add Indexer class method to get ms main index size for given code
             if only:  # only main index ondex not used
                 ondex = None
                 if index <= 63: # (64 ** ms - 1) where ms is main index size
-                    code = IdrDex.Ed25519_Crt_Sig  # use small current only
+                    code = indexing.IdrDex.Ed25519_Crt_Sig  # use small current only
                 else:
-                    code = IdrDex.Ed25519_Big_Crt_Sig  # use big current only
+                    code = indexing.IdrDex.Ed25519_Big_Crt_Sig  # use big current only
             else:  # both
                 if ondex == None:
                     ondex = index  # enable default to be same
                 if ondex == index and index <= 63:  # both same and small
-                    code = IdrDex.Ed25519_Sig  # use  small both same
+                    code = indexing.IdrDex.Ed25519_Sig  # use  small both same
                 else:  # otherwise big or both not same so use big both
-                    code = IdrDex.Ed25519_Big_Sig  # use use big both
+                    code = indexing.IdrDex.Ed25519_Big_Sig  # use use big both
 
-            return Siger(raw=sig,
-                         code=code,
-                         index=index,
-                         ondex=ondex,
-                         verfer=verfer,)
+            return indexing.Siger(raw=sig,
+                                    code=code,
+                                    index=index,
+                                    ondex=ondex,
+                                    verfer=verfer,)
 
     @staticmethod
     def _secp256r1(ser, seed, verfer, index, only=False, ondex=None, **kwa):
         """
         Returns signature as either Cigar or Siger instance as appropriate for
         Ed25519 digital signatures given index and ondex values
 
@@ -2575,30 +3301,30 @@
         if index is None:  # Must be Cigar i.e. non-indexed signature
             return Cigar(raw=sig, code=MtrDex.ECDSA_256r1_Sig, verfer=verfer)
         else:  # Must be Siger i.e. indexed signature
             # should add Indexer class method to get ms main index size for given code
             if only:  # only main index ondex not used
                 ondex = None
                 if index <= 63: # (64 ** ms - 1) where ms is main index size
-                    code = IdrDex.ECDSA_256r1_Crt_Sig  # use small current only
+                    code = indexing.IdrDex.ECDSA_256r1_Crt_Sig  # use small current only
                 else:
-                    code = IdrDex.ECDSA_256r1_Big_Crt_Sig  # use big current only
+                    code = indexing.IdrDex.ECDSA_256r1_Big_Crt_Sig  # use big current only
             else:  # both
                 if ondex == None:
                     ondex = index  # enable default to be same
                 if ondex == index and index <= 63:  # both same and small
-                    code = IdrDex.ECDSA_256r1_Sig  # use  small both same
+                    code = indexing.IdrDex.ECDSA_256r1_Sig  # use  small both same
                 else:  # otherwise big or both not same so use big both
-                    code = IdrDex.ECDSA_256r1_Big_Sig  # use use big both
+                    code = indexing.IdrDex.ECDSA_256r1_Big_Sig  # use use big both
 
-            return Siger(raw=sig,
-                         code=code,
-                         index=index,
-                         ondex=ondex,
-                         verfer=verfer,)
+            return indexing.Siger(raw=sig,
+                                    code=code,
+                                    index=index,
+                                    ondex=ondex,
+                                    verfer=verfer,)
 
     @staticmethod
     def _secp256k1(ser, seed, verfer, index, only=False, ondex=None, **kwa):
         """
         Returns signature as either Cigar or Siger instance as appropriate for
         secp256k1 digital signatures given index and ondex values
 
@@ -2634,76 +3360,31 @@
         if index is None:  # Must be Cigar i.e. non-indexed signature
             return Cigar(raw=sig, code=MtrDex.ECDSA_256k1_Sig, verfer=verfer)
         else:  # Must be Siger i.e. indexed signature
             # should add Indexer class method to get ms main index size for given code
             if only:  # only main index ondex not used
                 ondex = None
                 if index <= 63: # (64 ** ms - 1) where ms is main index size
-                    code = IdrDex.ECDSA_256k1_Crt_Sig  # use small current only
+                    code = indexing.IdrDex.ECDSA_256k1_Crt_Sig  # use small current only
                 else:
-                    code = IdrDex.ECDSA_256k1_Big_Crt_Sig  # use big current only
+                    code = indexing.IdrDex.ECDSA_256k1_Big_Crt_Sig  # use big current only
             else:  # both
                 if ondex == None:
                     ondex = index  # enable default to be same
                 if ondex == index and index <= 63:  # both same and small
-                    code = IdrDex.ECDSA_256k1_Sig  # use  small both same
+                    code = indexing.IdrDex.ECDSA_256k1_Sig  # use  small both same
                 else:  # otherwise big or both not same so use big both
-                    code = IdrDex.ECDSA_256k1_Big_Sig  # use use big both
+                    code = indexing.IdrDex.ECDSA_256k1_Big_Sig  # use use big both
 
-            return Siger(raw=sig,
-                         code=code,
-                         index=index,
-                         ondex=ondex,
-                         verfer=verfer,)
-
-    # def derive_index_code(code, index, only=False, ondex=None, **kwa):
-    #     # should add Indexer class method to get ms main index size for given code
-    #     if only:  # only main index ondex not used
-    #         ondex = None
-    #         if index <= 63: # (64 ** ms - 1) where ms is main index size,  use small current only
-    #             if code == MtrDex.Ed25519_Seed:
-    #                 indxSigCode = IdrDex.Ed25519_Crt_Sig
-    #             elif code == MtrDex.ECDSA_256r1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256r1_Crt_Sig
-    #             elif code == MtrDex.ECDSA_256k1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256k1_Crt_Sig
-    #             else:
-    #                 raise ValueError("Unsupported signer code = {}.".format(code))
-    #         else:    # use big current only
-    #             if code == MtrDex.Ed25519_Seed:
-    #                 indxSigCode = IdrDex.Ed25519_Big_Crt_Sig
-    #             elif code == MtrDex.ECDSA_256r1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256r1_Big_Crt_Sig
-    #             elif code == MtrDex.ECDSA_256k1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256k1_Big_Crt_Sig
-    #             else:
-    #                 raise ValueError("Unsupported signer code = {}.".format(code))
-    #     else:  # both
-    #         if ondex == None:
-    #             ondex = index  # enable default to be same
-    #         if ondex == index and index <= 63:  # both same and small so use small both same
-    #             if code == MtrDex.Ed25519_Seed:
-    #                 indxSigCode = IdrDex.Ed25519_Sig
-    #             elif code == MtrDex.ECDSA_256r1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256r1_Sig
-    #             elif code == MtrDex.ECDSA_256k1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256k1_Sig
-    #             else:
-    #                 raise ValueError("Unsupported signer code = {}.".format(code))
-    #         else:  # otherwise big or both not same so use big both
-    #             if code == MtrDex.Ed25519_Seed:
-    #                 indxSigCode = IdrDex.Ed25519_Big_Sig
-    #             elif code == MtrDex.ECDSA_256r1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256r1_Big_Sig
-    #             elif code == MtrDex.ECDSA_256k1_Seed:
-    #                 indxSigCode = IdrDex.ECDSA_256k1_Big_Sig
-    #             else:
-    #                 raise ValueError("Unsupported signer code = {}.".format(code))
+            return indexing.Siger(raw=sig,
+                                code=code,
+                                index=index,
+                                ondex=ondex,
+                                verfer=verfer,)
 
-    #     return (indxSigCode, ondex)
 
 class Salter(Matter):
     """
     Salter is Matter subclass to maintain random salt for secrets (private keys)
     Its .raw is random salt, .code as cipher suite for salt
 
     Attributes:
@@ -3294,46 +3975,14 @@
         Parameters:
             ser is bytes serialization
             dig is bytes reference digest
         """
         return (hashlib.sha256(ser).digest() == raw)
 
 
-
-@dataclass(frozen=True)
-class PreCodex:
-    """
-    PreCodex is codex all identifier prefix derivation codes.
-    This is needed to verify valid inception events.
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Ed25519N:      str = 'B'  # Ed25519 verification key non-transferable, basic derivation.
-    Ed25519:       str = 'D'  # Ed25519 verification key basic derivation
-    Blake3_256:    str = 'E'  # Blake3 256 bit digest self-addressing derivation.
-    Blake2b_256:   str = 'F'  # Blake2b 256 bit digest self-addressing derivation.
-    Blake2s_256:   str = 'G'  # Blake2s 256 bit digest self-addressing derivation.
-    SHA3_256:      str = 'H'  # SHA3 256 bit digest self-addressing derivation.
-    SHA2_256:      str = 'I'  # SHA2 256 bit digest self-addressing derivation.
-    Blake3_512:    str = '0D'  # Blake3 512 bit digest self-addressing derivation.
-    Blake2b_512:   str = '0E'  # Blake2b 512 bit digest self-addressing derivation.
-    SHA3_512:      str = '0F'  # SHA3 512 bit digest self-addressing derivation.
-    SHA2_512:      str = '0G'  # SHA2 512 bit digest self-addressing derivation.
-    ECDSA_256k1N:  str = '1AAA'  # ECDSA secp256k1 verification key non-transferable, basic derivation.
-    ECDSA_256k1:   str = '1AAB'  # ECDSA public verification or encryption key, basic derivation
-    ECDSA_256r1N:  str = "1AAI"  # ECDSA secp256r1 verification key non-transferable, basic derivation.
-    ECDSA_256r1:   str = "1AAJ"  # ECDSA secp256r1 verification or encryption key, basic derivation
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-
-PreDex = PreCodex()  # Make instance
-
-
 class Prefixer(Matter):
     """
     Prefixer is Matter subclass for autonomic identifier prefix using
     derivation as determined by code from ked
 
     Attributes:
 
@@ -3429,19 +4078,20 @@
             seed is only used for sig derivation it is the secret key/secret
 
         """
         ilk = ked["t"]
         if ilk not in (Ilks.icp, Ilks.dip, Ilks.vcp, Ilks.iss):
             raise ValueError("Nonincepting ilk={} for prefix derivation.".format(ilk))
 
-        labels = getattr(Labels, ilk)
-        for k in labels:
-            if k not in ked:
-                raise ValidationError("Missing element = {} from {} event for "
-                                      "evt = {}.".format(k, ilk, ked))
+        # Serder now does this check
+        #labels = getattr(Labels, ilk)
+        #for k in labels:
+            #if k not in ked:
+                #raise ValidationError("Missing element = {} from {} event for "
+                                      #"evt = {}.".format(k, ilk, ked))
 
         return (self._derive(ked=ked))
 
     def verify(self, ked, prefixed=False):
         """
         Returns True if derivation from ked for .code matches .qb64 and
                 If prefixed also verifies ked["i"] matches .qb64
@@ -3450,19 +4100,20 @@
         Parameters:
             ked is inception key event dict
         """
         ilk = ked["t"]
         if ilk not in (Ilks.icp, Ilks.dip, Ilks.vcp, Ilks.iss):
             raise ValueError("Nonincepting ilk={} for prefix derivation.".format(ilk))
 
-        labels = getattr(Labels, ilk)
-        for k in labels:
-            if k not in ked:
-                raise ValidationError("Missing element = {} from {} event for "
-                                      "evt = {}.".format(k, ilk, ked))
+        # Serder now does this check
+        #labels = getattr(Labels, ilk)
+        #for k in labels:
+            #if k not in ked:
+                #raise ValidationError("Missing element = {} from {} event for "
+                                      #"evt = {}.".format(k, ilk, ked))
 
         return (self._verify(ked=ked, pre=self.qb64, prefixed=prefixed))
 
     def _derive_non_transferable(self, ked):
         """
         Returns tuple (raw, code) of basic nontransferable Ed25519 prefix (qb64)
             as derived from inception key event dict ked keys[0]
@@ -3736,15 +4387,15 @@
            kind (str): serialization algorithm of sad, one of Serials
                         used to override that given by 'v' field if any in sad
                         otherwise default is Serials.json
 
         """
         knd = Serials.json
         if 'v' in sad:  # versioned sad
-            _, _, knd, _ = deversify(sad['v'])
+            _, _, knd, _, _ = deversify(sad['v'])
 
         if not kind:  # match logic of Serder for kind
             kind = knd
 
         return dumps(sad, kind=kind)
 
     @classmethod
@@ -3894,864 +4545,54 @@
         except Exception as ex:
             return False
 
         return True
 
 
 @dataclass(frozen=True)
-class IndexerCodex:
-    """ IndexerCodex is codex hard (stable) part of all indexer derivation codes.
-
-    Codes indicate which list of keys, current and/or prior next, index is for:
-
-        _Sig:           Indices in code may appear in both current signing and
-                        prior next key lists when event has both current and prior
-                        next key lists. Two character code table has only one index
-                        so must be the same for both lists. Other index if for
-                        prior next.
-                        The indices may be different in those code tables which
-                        have two sets of indices.
-
-        _Crt_Sig:       Index in code for current signing key list only.
-
-        _Big_:          Big index values
-
-
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-
-    Ed25519_Sig: str = 'A'  # Ed25519 sig appears same in both lists if any.
-    Ed25519_Crt_Sig: str = 'B'  # Ed25519 sig appears in current list only.
-    ECDSA_256k1_Sig: str = 'C'  # ECDSA secp256k1 sig appears same in both lists if any.
-    ECDSA_256k1_Crt_Sig: str = 'D'  # ECDSA secp256k1 sig appears in current list.
-    ECDSA_256r1_Sig: str = "E"  # ECDSA secp256r1 sig appears same in both lists if any.
-    ECDSA_256r1_Crt_Sig: str = "F"  # ECDSA secp256r1 sig appears in current list.
-    Ed448_Sig: str = '0A'  # Ed448 signature appears in both lists.
-    Ed448_Crt_Sig: str = '0B'  # Ed448 signature appears in current list only.
-    Ed25519_Big_Sig: str = '2A'  # Ed25519 sig appears in both lists.
-    Ed25519_Big_Crt_Sig: str = '2B'  # Ed25519 sig appears in current list only.
-    ECDSA_256k1_Big_Sig: str = '2C'  # ECDSA secp256k1 sig appears in both lists.
-    ECDSA_256k1_Big_Crt_Sig: str = '2D'  # ECDSA secp256k1 sig appears in current list only.
-    ECDSA_256r1_Big_Sig: str = "2E"  # ECDSA secp256r1 sig appears in both lists.
-    ECDSA_256r1_Big_Crt_Sig: str = "2F"  # ECDSA secp256r1 sig appears in current list only.
-    Ed448_Big_Sig: str = '3A'  # Ed448 signature appears in both lists.
-    Ed448_Big_Crt_Sig: str = '3B'  # Ed448 signature appears in current list only.
-    TBD0: str = '0z'  # Test of Var len label L=N*4 <= 4095 char quadlets includes code
-    TBD1: str = '1z'  # Test of index sig lead 1
-    TBD4: str = '4z'  # Test of index sig lead 1 big
-
-    def __iter__(self):
-        return iter(astuple(self))  # enables inclusion test with "in"
-
-IdrDex = IndexerCodex()
-
-
-@dataclass(frozen=True)
-class IndexedSigCodex:
-    """IndexedSigCodex is codex all indexed signature derivation codes.
-
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Ed25519_Sig: str = 'A'  # Ed25519 sig appears same in both lists if any.
-    Ed25519_Crt_Sig: str = 'B'  # Ed25519 sig appears in current list only.
-    ECDSA_256k1_Sig: str = 'C'  # ECDSA secp256k1 sig appears same in both lists if any.
-    ECDSA_256k1_Crt_Sig: str = 'D'  # ECDSA secp256k1 sig appears in current list.
-    ECDSA_256r1_Sig: str = "E"  # ECDSA secp256r1 sig appears same in both lists if any.
-    ECDSA_256r1_Crt_Sig: str = "F"  # ECDSA secp256r1 sig appears in current list.
-    Ed448_Sig: str = '0A'  # Ed448 signature appears in both lists.
-    Ed448_Crt_Sig: str = '0B'  # Ed448 signature appears in current list only.
-    Ed25519_Big_Sig: str = '2A'  # Ed25519 sig appears in both lists.
-    Ed25519_Big_Crt_Sig: str = '2B'  # Ed25519 sig appears in current list only.
-    ECDSA_256k1_Big_Sig: str = '2C'  # ECDSA secp256k1 sig appears in both lists.
-    ECDSA_256k1_Big_Crt_Sig: str = '2D'  # ECDSA secp256k1 sig appears in current list only.
-    ECDSA_256r1_Big_Sig: str = "2E"  # ECDSA secp256r1 sig appears in both lists.
-    ECDSA_256r1_Big_Crt_Sig: str = "2F"  # ECDSA secp256r1 sig appears in current list only.
-    Ed448_Big_Sig: str = '3A'  # Ed448 signature appears in both lists.
-    Ed448_Big_Crt_Sig: str = '3B'  # Ed448 signature appears in current list only.
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-IdxSigDex = IndexedSigCodex()  # Make instance
-
-
-@dataclass(frozen=True)
-class IndexedCurrentSigCodex:
-    """IndexedCurrentSigCodex is codex indexed signature codes for current list.
-
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Ed25519_Crt_Sig: str = 'B'  # Ed25519 sig appears in current list only.
-    ECDSA_256k1_Crt_Sig: str = 'D'  # ECDSA secp256k1 sig appears in current list only.
-    ECDSA_256r1_Crt_Sig: str = "F"  # ECDSA secp256r1 sig appears in current list.
-    Ed448_Crt_Sig: str = '0B'  # Ed448 signature appears in current list only.
-    Ed25519_Big_Crt_Sig: str = '2B'  # Ed25519 sig appears in current list only.
-    ECDSA_256k1_Big_Crt_Sig: str = '2D'  # ECDSA secp256k1 sig appears in current list only.
-    ECDSA_256r1_Big_Crt_Sig: str = "2F"  # ECDSA secp256r1 sig appears in current list only.
-    Ed448_Big_Crt_Sig: str = '3B'  # Ed448 signature appears in current list only.
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-IdxCrtSigDex = IndexedCurrentSigCodex()  # Make instance
-
-
-
-@dataclass(frozen=True)
-class IndexedBothSigCodex:
-    """IndexedBothSigCodex is codex indexed signature codes for both lists.
-
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    Ed25519_Sig: str = 'A'  # Ed25519 sig appears same in both lists if any.
-    ECDSA_256k1_Sig: str = 'C'  # ECDSA secp256k1 sig appears same in both lists if any.
-    ECDSA_256r1_Sig: str = "E"  # ECDSA secp256r1 sig appears same in both lists if any.
-    Ed448_Sig: str = '0A'  # Ed448 signature appears in both lists.
-    Ed25519_Big_Sig: str = '2A'  # Ed25519 sig appears in both listsy.
-    ECDSA_256k1_Big_Sig: str = '2C'  # ECDSA secp256k1 sig appears in both lists.
-    ECDSA_256r1_Big_Sig: str = "2E"  # ECDSA secp256r1 sig appears in both lists.
-    Ed448_Big_Sig: str = '3A'  # Ed448 signature appears in both lists.
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-IdxBthSigDex = IndexedBothSigCodex()  # Make instance
-
-# namedtuple for size entries in Incexer derivation code tables
-# hs is the hard size int number of chars in hard (stable) part of code
-# ss is the soft size int number of chars in soft (unstable) part of code
-# os is the other size int number of chars in other index part of soft
-#     ms = ss - os main index size computed
-# fs is the full size int number of chars in code plus appended material if any
-# ls is the lead size int number of bytes to pre-pad pre-converted raw binary
-Xizage = namedtuple("Xizage", "hs ss os fs ls")
-
-class Indexer:
-    """ Indexer is fully qualified cryptographic material primitive base class for
-    indexed primitives. In special cases some codes in the Index code table
-    may be of variable length (i.e. not indexed) when the full size table entry
-    is None. In that case the index is used instread as the length.
-
-    Sub classes are derivation code and key event element context specific.
-
-    Includes the following attributes and properties:
-
-    Attributes:
-
-    Properties:
-        code is str of stable (hard) part of derivation code
-        raw (bytes): unqualified crypto material usable for crypto operations
-        index (int): main index offset into list or length of material
-        ondex (int | None): other index offset into list or length of material
-        qb64b (bytes): fully qualified Base64 crypto material
-        qb64 (str | bytes):  fully qualified Base64 crypto material
-        qb2 (bytes): fully qualified binary crypto material
-
-    Hidden:
-        ._code (str): value for .code property
-        ._raw (bytes): value for .raw property
-        ._index (int): value for .index property
-        ._ondex (int): value for .ondex property
-        ._infil is method to compute fully qualified Base64 from .raw and .code
-        ._binfil is method to compute fully qualified Base2 from .raw and .code
-        ._exfil is method to extract .code and .raw from fully qualified Base64
-        ._bexfil is method to extract .code and .raw from fully qualified Base2
-
-    """
-    Codex = IdrDex
-    # Hards table maps from bytes Base64 first code char to int of hard size, hs,
-    # (stable) of code. The soft size, ss, (unstable) is always > 0 for Indexer.
-    Hards = ({chr(c): 1 for c in range(65, 65 + 26)})
-    Hards.update({chr(c): 1 for c in range(97, 97 + 26)})
-    Hards.update([('0', 2), ('1', 2), ('2', 2), ('3', 2), ('4', 2)])
-    # Sizes table maps hs chars of code to Xizage namedtuple of (hs, ss, os, fs, ls)
-    # where hs is hard size, ss is soft size, os is other index size,
-    # and fs is full size, ls is lead size.
-    # where ss includes os, so main index size ms = ss - os
-    # soft size, ss, should always be  > 0 for Indexer
-    Sizes = {
-        'A': Xizage(hs=1, ss=1, os=0, fs=88, ls=0),
-        'B': Xizage(hs=1, ss=1, os=0, fs=88, ls=0),
-        'C': Xizage(hs=1, ss=1, os=0, fs=88, ls=0),
-        'D': Xizage(hs=1, ss=1, os=0, fs=88, ls=0),
-        'E': Xizage(hs=1, ss=1, os=0, fs=88, ls=0),
-        'F': Xizage(hs=1, ss=1, os=0, fs=88, ls=0),
-        '0A': Xizage(hs=2, ss=2, os=1, fs=156, ls=0),
-        '0B': Xizage(hs=2, ss=2, os=1, fs=156, ls=0),
-        '2A': Xizage(hs=2, ss=4, os=2, fs=92, ls=0),
-        '2B': Xizage(hs=2, ss=4, os=2, fs=92, ls=0),
-        '2C': Xizage(hs=2, ss=4, os=2, fs=92, ls=0),
-        '2D': Xizage(hs=2, ss=4, os=2, fs=92, ls=0),
-        '2E': Xizage(hs=2, ss=4, os=2, fs=92, ls=0),
-        '2F': Xizage(hs=2, ss=4, os=2, fs=92, ls=0),
-        '3A': Xizage(hs=2, ss=6, os=3, fs=160, ls=0),
-        '3B': Xizage(hs=2, ss=6, os=3, fs=160, ls=0),
-        '0z': Xizage(hs=2, ss=2, os=0, fs=None, ls=0),
-        '1z': Xizage(hs=2, ss=2, os=1, fs=76, ls=1),
-        '4z': Xizage(hs=2, ss=6, os=3, fs=80, ls=1),
-    }
-    # Bards table maps to hard size, hs, of code from bytes holding sextets
-    # converted from first code char. Used for ._bexfil.
-    Bards = ({codeB64ToB2(c): hs for c, hs in Hards.items()})
-
-    def __init__(self, raw=None, code=IdrDex.Ed25519_Sig, index=0, ondex=None,
-                 qb64b=None, qb64=None, qb2=None, strip=False):
-        """
-        Validate as fully qualified
-        Parameters:
-            raw (bytes): unqualified crypto material usable for crypto operations
-            code is str of stable (hard) part of derivation code
-            index (int): main index offset into list or length of material
-            ondex (int | None): other index offset into list or length of material
-            qb64b (bytes): fully qualified Base64 crypto material
-            qb64 (str | bytes):  fully qualified Base64 crypto material
-            qb2 (bytes): fully qualified binary crypto material
-            strip (bool): True means strip counter contents from input stream
-                bytearray after parsing qb64b or qb2. False means do not strip
-
-        Needs either (raw and code and index) or qb64b or qb64 or qb2
-        Otherwise raises EmptyMaterialError
-        When raw and code provided then validate that code is correct
-        for length of raw  and assign .raw
-        Else when qb64b or qb64 or qb2 provided extract and assign
-        .raw, .code, .index, .ondex.
-
-        """
-        if raw is not None:  # raw provided
-            if not code:
-                raise EmptyMaterialError("Improper initialization need either "
-                                         "(raw and code) or qb64b or qb64 or qb2.")
-            if not isinstance(raw, (bytes, bytearray)):
-                raise TypeError(f"Not a bytes or bytearray, raw={raw}.")
-
-            if code not in self.Sizes:
-                raise UnexpectedCodeError(f"Unsupported code={code}.")
-
-            hs, ss, os, fs, ls = self.Sizes[code]  # get sizes for code
-            cs = hs + ss  # both hard + soft code size
-            ms = ss - os
-
-            if not isinstance(index, int) or index < 0 or index > (64 ** ms - 1):
-                raise InvalidVarIndexError(f"Invalid index={index} for code={code}.")
-
-            if isinstance(ondex, int) and os and not (ondex >= 0 and ondex <= (64 ** os - 1)):
-                raise InvalidVarIndexError(f"Invalid ondex={ondex} for code={code}.")
-
-            if code in IdxCrtSigDex and ondex is not None:
-                raise InvalidVarIndexError(f"Non None ondex={ondex} for code={code}.")
-
-            if code in IdxBthSigDex:
-                if ondex is None:  # set default
-                    ondex = index  # when not provided make ondex match index
-                else:
-                    if ondex != index and os == 0:  # must match if os == 0
-                        raise InvalidVarIndexError(f"Non matching ondex={ondex}"
-                                                   f" and index={index} for "
-                                                   f"code={code}.")
-
-
-            if not fs:  # compute fs from index
-                if cs % 4:
-                    raise InvalidCodeSizeError(f"Whole code size not multiple of 4 for "
-                                               f"variable length material. cs={cs}.")
-                if os != 0:
-                    raise InvalidCodeSizeError(f"Non-zero other index size for "
-                                               f"variable length material. os={os}.")
-                fs = (index * 4) + cs
-
-            rawsize = (fs - cs) * 3 // 4
-
-            raw = raw[:rawsize]  # copy rawsize from stream, may be less
-            if len(raw) != rawsize:  # forbids shorter
-                raise RawMaterialError(f"Not enougth raw bytes for code={code}"
-                                       f"and index={index} ,expected {rawsize} "
-                                       f"got {len(raw)}.")
-
-            self._code = code
-            self._index = index
-            self._ondex = ondex
-            self._raw = bytes(raw)  # crypto ops require bytes not bytearray
-
-        elif qb64b is not None:
-            self._exfil(qb64b)
-            if strip:  # assumes bytearray
-                del qb64b[:len(self.qb64b)]  # may be variable length fs
-
-        elif qb64 is not None:
-            self._exfil(qb64)
-
-        elif qb2 is not None:
-            self._bexfil(qb2)
-            if strip:  # assumes bytearray
-                del qb2[:len(self.qb2)]  # may be variable length fs
-
-        else:
-            raise EmptyMaterialError("Improper initialization need either "
-                                     "(raw and code and index) or qb64b or "
-                                     "qb64 or qb2.")
-
-    @classmethod
-    def _rawSize(cls, code):
-        """
-        Returns expected raw size in bytes for a given code. Not applicable to
-        codes with fs = None
-        """
-        hs, ss, os, fs, ls = cls.Sizes[code]  # get sizes
-        return ((fs - (hs + ss)) * 3 // 4)
-
-    @property
-    def code(self):
-        """
-        Returns ._code
-        Makes .code read only
-        """
-        return self._code
-
-    @property
-    def raw(self):
-        """
-        Returns ._raw
-        Makes .raw read only
-        """
-        return self._raw
-
-    @property
-    def index(self):
-        """
-        Returns ._index
-        Makes .index read only
-        """
-        return self._index
-
-    @property
-    def ondex(self):
-        """
-        Returns ._ondex
-        Makes .ondex read only
-        """
-        return self._ondex
-
-    @property
-    def qb64b(self):
-        """
-        Property qb64b:
-        Returns Fully Qualified Base64 Version encoded as bytes
-        Assumes self.raw and self.code are correctly populated
-        """
-        return self._infil()
-
-    @property
-    def qb64(self):
-        """
-        Property qb64:
-        Returns Fully Qualified Base64 Version
-        Assumes self.raw and self.code are correctly populated
-        """
-        return self.qb64b.decode("utf-8")
-
-    @property
-    def qb2(self):
-        """
-        Property qb2:
-        Returns Fully Qualified Binary Version Bytes
-        """
-        return self._binfil()
-
-    def _infil(self):
-        """
-        Returns fully qualified attached sig base64 bytes computed from
-        self.raw, self.code and self.index.
-
-        cs = hs + ss
-        os = ss - ms (main index size)
-        when fs None then size computed & fs = size * 4 + cs
-
-        """
-        code = self.code  # codex value chars hard code
-        index = self.index  # main index value
-        ondex = self.ondex  # other index value
-        raw = self.raw  # bytes or bytearray
-
-        ps = (3 - (len(raw) % 3)) % 3  # if lead then same pad size chars & lead size bytes
-        hs, ss, os, fs, ls = self.Sizes[code]
-        cs = hs + ss
-        ms = ss - os
-
-        if not fs:  # compute fs from index
-            if cs % 4:
-                raise InvalidCodeSizeError(f"Whole code size not multiple of 4 for "
-                                           f"variable length material. cs={cs}.")
-            if os != 0:
-                raise InvalidCodeSizeError(f"Non-zero other index size for "
-                                           f"variable length material. os={os}.")
-            fs = (index * 4) + cs
-
-        if index < 0 or index > (64 ** ms - 1):
-            raise InvalidVarIndexError(f"Invalid index={index} for code={code}.")
-
-        if (isinstance(ondex, int) and os and
-                not (ondex >= 0 and ondex <= (64 ** os - 1))):
-            raise InvalidVarIndexError(f"Invalid ondex={ondex} for os={os} and "
-                                       f"code={code}.")
-
-        # both is hard code + converted index + converted ondex
-        both = (f"{code}{intToB64(index, l=ms)}"
-                f"{intToB64(ondex if ondex is not None else 0, l=os)}")
-
-        # check valid pad size for whole code size, assumes ls is zero
-        if len(both) != cs:
-            raise InvalidCodeSizeError("Mismatch code size = {} with table = {}."
-                                       .format(cs, len(both)))
-
-        if (cs % 4) != ps - ls:  # adjusted pad given lead bytes
-            raise InvalidCodeSizeError(f"Invalid code={both} for converted"
-                                       f" raw pad size={ps}.")
-
-        # prepend pad bytes, convert, then replace pad chars with full derivation
-        # code including index,
-        full = both.encode("utf-8") + encodeB64(bytes([0] * ps) + raw)[ps - ls:]
-
-        if len(full) != fs:  # invalid size
-            raise InvalidCodeSizeError(f"Invalid code={both} for raw size={len(raw)}.")
-
-        return full
-
-
-    def _binfil(self):
-        """
-        Returns bytes of fully qualified base2 bytes, that is .qb2
-        self.code and self.index  converted to Base2 + self.raw left shifted
-        with pad bits equivalent of Base64 decode of .qb64 into .qb2
-        """
-        code = self.code  # codex chars hard code
-        index = self.index  # main index value
-        ondex = self.ondex  # other index value
-        raw = self.raw  # bytes or bytearray
-
-        ps = (3 - (len(raw) % 3)) % 3  # same pad size chars & lead size bytes
-        hs, ss, os, fs, ls = self.Sizes[code]
-        cs = hs + ss
-        ms = ss - os
-
-        if index < 0 or index > (64 ** ss - 1):
-            raise InvalidVarIndexError(f"Invalid index={index} for code={code}.")
-
-        if (isinstance(ondex, int) and os and
-                not (ondex >= 0 and ondex <= (64 ** os - 1))):
-            raise InvalidVarIndexError(f"Invalid ondex={ondex} for os={os} and "
-                                       f"code={code}.")
-
-        if not fs:  # compute fs from index
-            if cs % 4:
-                raise InvalidCodeSizeError(f"Whole code size not multiple of 4 for "
-                                           f"variable length material. cs={cs}.")
-            if os != 0:
-                raise InvalidCodeSizeError(f"Non-zero other index size for "
-                                           f"variable length material. os={os}.")
-            fs = (index * 4) + cs
-
-        # both is hard code + converted index
-        both = (f"{code}{intToB64(index, l=ms)}"
-                f"{intToB64(ondex if ondex is not None else 0, l=os)}")
-
-        if len(both) != cs:
-            raise InvalidCodeSizeError("Mismatch code size = {} with table = {}."
-                                       .format(cs, len(both)))
-
-        if (cs % 4) != ps - ls:  # adjusted pad given lead bytes
-                    raise InvalidCodeSizeError(f"Invalid code={both} for converted"
-                                               f" raw pad size={ps}.")
-
-        n = sceil(cs * 3 / 4)  # number of b2 bytes to hold b64 code + index
-        # convert code both to right align b2 int then left shift in pad bits
-        # then convert to bytes
-        bcode = (b64ToInt(both) << (2 * (ps - ls))).to_bytes(n, 'big')
-        full = bcode + bytes([0] * ls) + raw
-
-        bfs = len(full)  # binary full size
-        if bfs % 3 or (bfs * 4 // 3) != fs:  # invalid size
-            raise InvalidCodeSizeError(f"Invalid code={both} for raw size={len(raw)}.")
-
-        return full
-
-
-    def _exfil(self, qb64b):
-        """
-        Extracts self.code, self.index, and self.raw from qualified base64 bytes qb64b
-
-        cs = hs + ss
-        ms = ss - os (main index size)
-        when fs None then size computed & fs = size * 4 + cs
-        """
-        if not qb64b:  # empty need more bytes
-            raise ShortageError("Empty material.")
-
-        first = qb64b[:1]  # extract first char code selector
-        if hasattr(first, "decode"):
-            first = first.decode("utf-8")
-        if first not in self.Hards:
-            if first[0] == '-':
-                raise UnexpectedCountCodeError("Unexpected count code start"
-                                               "while extracing Indexer.")
-            elif first[0] == '_':
-                raise UnexpectedOpCodeError("Unexpected  op code start"
-                                            "while extracing Indexer.")
-            else:
-                raise UnexpectedCodeError(f"Unsupported code start char={first}.")
-
-        hs = self.Hards[first]  # get hard code size
-        if len(qb64b) < hs:  # need more bytes
-            raise ShortageError(f"Need {hs - len(qb64b)} more characters.")
-
-        hard = qb64b[:hs]  # get hard code
-        if hasattr(hard, "decode"):
-            hard = hard.decode("utf-8")
-        if hard not in self.Sizes:
-            raise UnexpectedCodeError(f"Unsupported code ={hard}.")
-
-        hs, ss, os, fs, ls = self.Sizes[hard]  # assumes hs in both tables consistent
-        cs = hs + ss  # both hard + soft code size
-        ms = ss - os
-        # assumes that unit tests on Indexer and IndexerCodex ensure that
-        # .Codes and .Sizes are well formed.
-        # hs consistent and hs > 0 and ss > 0 and (fs >= hs + ss if fs is not None else True)
-        # assumes no variable length indexed codes so fs is not None
-
-        if len(qb64b) < cs:  # need more bytes
-            raise ShortageError(f"Need {cs - len(qb64b)} more characters.")
-
-        index = qb64b[hs:hs+ms]  # extract index/size chars
-        if hasattr(index, "decode"):
-            index = index.decode("utf-8")
-        index = b64ToInt(index)  # compute int index
-
-        ondex = qb64b[hs+ms:hs+ms+os]  # extract ondex chars
-        if hasattr(ondex, "decode"):
-            ondex = ondex.decode("utf-8")
-
-        if hard in IdxCrtSigDex:  # if current sig then ondex from code must be 0
-            ondex = b64ToInt(ondex) if os else None  # compute ondex from code
-            if ondex:  # not zero or None so error
-                raise ValueError(f"Invalid ondex={ondex} for code={hard}.")
-            else:
-                ondex = None  # zero so set to None when current only
-        else:
-            ondex = b64ToInt(ondex) if os else index
-
-        # index is index for some codes and variable length for others
-        if not fs:  # compute fs from index which means variable length
-            if cs % 4:
-                raise ValidationError(f"Whole code size not multiple of 4 for "
-                                      f"variable length material. cs={cs}.")
-            if os != 0:
-                raise ValidationError(f"Non-zero other index size for "
-                                      f"variable length material. os={os}.")
-            fs = (index * 4) + cs
-
-        if len(qb64b) < fs:  # need more bytes
-            raise ShortageError(f"Need {fs - len(qb64b)} more chars.")
-
-        qb64b = qb64b[:fs]  # fully qualified primitive code plus material
-        if hasattr(qb64b, "encode"):  # only convert extracted chars from stream
-            qb64b = qb64b.encode("utf-8")
-
-        # strip off prepended code and append pad characters
-        #ps = cs % 4  # pad size ps = cs mod 4, same pad chars and lead bytes
-        #base = ps * b'A' + qb64b[cs:]  # replace prepend code with prepad zeros
-        #raw = decodeB64(base)[ps+ls:]  # decode and strip off ps+ls prepad bytes
-
-        # check for non-zeroed pad bits or lead bytes
-        ps = cs % 4  # code pad size ps = cs mod 4
-        pbs = 2 * (ps if ps else ls)  # pad bit size in bits
-        if ps:  # ps. IF ps THEN not ls (lead) and vice versa OR not ps and not ls
-            base = ps * b'A' + qb64b[cs:]  # replace pre code with prepad chars of zero
-            paw = decodeB64(base)  # decode base to leave prepadded raw
-            pi = (int.from_bytes(paw[:ps], "big"))  # prepad as int
-            if pi & (2 ** pbs - 1 ):  # masked pad bits non-zero
-                raise ValueError(f"Non zeroed prepad bits = "
-                                 f"{pi & (2 ** pbs - 1 ):<06b} in {qb64b[cs:cs+1]}.")
-            raw = paw[ps:]  # strip off ps prepad paw bytes
-        else:  # not ps. IF not ps THEN may or may not be ls (lead)
-            base = qb64b[cs:]  # strip off code leaving lead chars if any and value
-            # decode lead chars + val leaving lead bytes + raw bytes
-            # then strip off ls lead bytes leaving raw
-            paw = decodeB64(base) # decode base to leave prepadded paw bytes
-            li = int.from_bytes(paw[:ls], "big")  # lead as int
-            if li:  # pre pad lead bytes must be zero
-                if ls == 1:
-                    raise ValueError(f"Non zeroed lead byte = 0x{li:02x}.")
-                else:
-                    raise ValueError(f"Non zeroed lead bytes = 0x{li:04x}.")
-
-            raw = paw[ls:]
-
-        if len(raw) != (len(qb64b) - cs) * 3 // 4:  # exact lengths
-            raise ConversionError(f"Improperly qualified material = {qb64b}")
-
-        self._code = hard
-        self._index = index
-        self._ondex = ondex
-        self._raw = raw  # must be bytes for crpto opts and immutable not bytearray
-
-
-
-    def _bexfil(self, qb2):
-        """
-        Extracts self.code, self.index, and self.raw from qualified base2 bytes qb2
-
-        cs = hs + ss
-        ms = ss - os (main index size)
-        when fs None then size computed & fs = size * 4 + cs
-        """
-        if not qb2:  # empty need more bytes
-            raise ShortageError("Empty material, Need more bytes.")
-
-        first = nabSextets(qb2, 1)  # extract first sextet as code selector
-        if first not in self.Bards:
-            if first[0] == b'\xf8':  # b64ToB2('-')
-                raise UnexpectedCountCodeError("Unexpected count code start"
-                                               "while extracing Matter.")
-            elif first[0] == b'\xfc':  # b64ToB2('_')
-                raise UnexpectedOpCodeError("Unexpected  op code start"
-                                            "while extracing Matter.")
-            else:
-                raise UnexpectedCodeError(f"Unsupported code start sextet={first}.")
-
-        hs = self.Bards[first]  # get code hard size equvalent sextets
-        bhs = sceil(hs * 3 / 4)  # bhs is min bytes to hold hs sextets
-        if len(qb2) < bhs:  # need more bytes
-            raise ShortageError(f"Need {bhs - len(qb2)} more bytes.")
-
-        hard = codeB2ToB64(qb2, hs)  # extract and convert hard part of code
-        if hard not in self.Sizes:
-            raise UnexpectedCodeError(f"Unsupported code ={hard}.")
-
-        hs, ss, os, fs, ls = self.Sizes[hard]
-        cs = hs + ss  # both hs and ss
-        ms = ss - os
-        # assumes that unit tests on Indexer and IndexerCodex ensure that
-        # .Codes and .Sizes are well formed.
-        # hs consistent and hs > 0 and ss > 0 and (fs >= hs + ss if fs is not None else True)
-
-        bcs = sceil(cs * 3 / 4)  # bcs is min bytes to hold cs sextets
-        if len(qb2) < bcs:  # need more bytes
-            raise ShortageError("Need {} more bytes.".format(bcs - len(qb2)))
-
-        both = codeB2ToB64(qb2, cs)  # extract and convert both hard and soft part of code
-        index = b64ToInt(both[hs:hs+ms])  # compute index
-
-        if hard in IdxCrtSigDex:  # if current sig then ondex from code must be 0
-            ondex = b64ToInt(both[hs+ms:hs+ms+os]) if os else None  # compute ondex from code
-            if ondex:  # not zero or None so error
-                raise ValueError(f"Invalid ondex={ondex} for code={hard}.")
-            else:
-                ondex = None  # zero so set to None when current only
-        else:
-            ondex = b64ToInt(both[hs+ms:hs+ms+os]) if os else index
-
-        if hard in IdxCrtSigDex:  # if current sig then ondex from code must be 0
-            if ondex:  # not zero so error
-                raise ValueError(f"Invalid ondex={ondex} for code={hard}.")
-            else:  # zero so set to None
-                ondex = None
-
-        if not fs:  # compute fs from size chars in ss part of code
-            if cs % 4:
-                raise ValidationError(f"Whole code size not multiple of 4 for "
-                                      f"variable length material. cs={cs}.")
-            if os != 0:
-                raise ValidationError(f"Non-zero other index size for "
-                                      f"variable length material. os={os}.")
-            fs = (index * 4) + cs
-
-        bfs = sceil(fs * 3 / 4)  # bfs is min bytes to hold fs sextets
-        if len(qb2) < bfs:  # need more bytes
-            raise ShortageError("Need {} more bytes.".format(bfs - len(qb2)))
-
-        qb2 = qb2[:bfs]  # extract qb2 fully qualified primitive code plus material
-
-        # check for non-zeroed prepad bits or lead bytes
-        ps = cs % 4  # code pad size ps = cs mod 4
-        pbs = 2 * (ps if ps else ls)  # pad bit size in bits
-        if ps:  # ps. IF ps THEN not ls (lead) and vice versa OR not ps and not ls
-            # convert last byte of code bytes in which are pad bits to int
-            pi = (int.from_bytes(qb2[bcs-1:bcs], "big"))
-            if pi & (2 ** pbs - 1 ):  # masked pad bits non-zero
-                raise ValueError(f"Non zeroed pad bits = "
-                                 f"{pi & (2 ** pbs - 1 ):>08b} in 0x{pi:02x}.")
-        else:  # not ps. IF not ps THEN may or may not be ls (lead)
-            li = int.from_bytes(qb2[bcs:bcs+ls], "big")  # lead as int
-            if li:  # pre pad lead bytes must be zero
-                if ls == 1:
-                    raise ValueError(f"Non zeroed lead byte = 0x{li:02x}.")
-                else:
-                    raise ValueError(f"Non zeroed lead bytes = 0x{li:02x}.")
-
-
-        raw = qb2[(bcs + ls):]  # strip code and leader bytes from qb2 to get raw
-
-        if len(raw) != (len(qb2) - bcs - ls):  # exact lengths
-            raise ConversionError(f"Improperly qualified material = {qb2}")
-
-        self._code = hard
-        self._index = index
-        self._ondex = ondex
-        self._raw = bytes(raw)  # must be bytes for crypto ops and not bytearray mutable
-
-
-class Siger(Indexer):
-    """
-    Siger is subclass of Indexer, indexed signature material,
-
-    Adds .verfer property which is instance of Verfer that provides
-          associated signature verifier.
-
-    See Indexer for inherited attributes and properties:
-
-    Attributes:
-
-    Properties:
-        verfer (Verfer): instance if any provides public verification key
-
-    Methods:
-
-    Hidden:
-        _verfer (Verfer): value for .verfer property
-
-
-    """
-
-    def __init__(self, verfer=None, **kwa):
-        """Initialze instance
-
-        Parameters:  See Matter for inherted parameters
-            verfer (Verfer): instance if any provides public verification key
-
-        """
-        super(Siger, self).__init__(**kwa)
-        if self.code not in IdxSigDex:
-            raise ValidationError("Invalid code = {} for Siger."
-                                  "".format(self.code))
-        self.verfer = verfer
-
-    @property
-    def verfer(self):
-        """
-        Property verfer:
-        Returns Verfer instance
-        Assumes ._verfer is correctly assigned
-        """
-        return self._verfer
-
-    @verfer.setter
-    def verfer(self, verfer):
-        """ verfer property setter """
-        self._verfer = verfer
-
-
-@dataclass(frozen=True)
 class CounterCodex:
     """
     CounterCodex is codex hard (stable) part of all counter derivation codes.
     Only provide defined codes.
     Undefined are left out so that inclusion(exclusion) via 'in' operator works.
     """
 
     ControllerIdxSigs: str = '-A'  # Qualified Base64 Indexed Signature.
     WitnessIdxSigs: str = '-B'  # Qualified Base64 Indexed Signature.
     NonTransReceiptCouples: str = '-C'  # Composed Base64 Couple, pre+cig.
     TransReceiptQuadruples: str = '-D'  # Composed Base64 Quadruple, pre+snu+dig+sig.
     FirstSeenReplayCouples: str = '-E'  # Composed Base64 Couple, fnu+dts.
     TransIdxSigGroups: str = '-F'  # Composed Base64 Group, pre+snu+dig+ControllerIdxSigs group.
-    SealSourceCouples: str = '-G'  # Composed Base64 couple, snu+dig of given delegators or issuers event
+    SealSourceCouples: str = '-G'  # Composed Base64 couple, snu+dig of given delegator/issuer/transaction event
     TransLastIdxSigGroups: str = '-H'  # Composed Base64 Group, pre+ControllerIdxSigs group.
     SealSourceTriples: str = '-I'  # Composed Base64 triple, pre+snu+dig of anchoring source event
-    SadPathSig: str = '-J'  # Composed Base64 Group path+TransIdxSigGroup of SAID of content
-    SadPathSigGroup: str = '-K'  # Composed Base64 Group, root(path)+SaidPathCouples
-    PathedMaterialQuadlets: str = '-L'  # Composed Grouped Pathed Material Quadlet (4 char each)
-    AttachedMaterialQuadlets: str = '-V'  # Composed Grouped Attached Material Quadlet (4 char each)
-    BigAttachedMaterialQuadlets: str = '-0V'  # Composed Grouped Attached Material Quadlet (4 char each)
-    KERIProtocolStack: str = '--AAA'  # KERI ACDC Protocol Stack CESR Version
+    SadPathSigGroups: str = '-J'  # Composed Base64 Group path+TransIdxSigGroup of SAID of content
+    RootSadPathSigGroups: str = '-K'  # Composed Base64 Group, root(path)+SaidPathCouples
+    PathedMaterialGroup: str = '-L'  # Composed Grouped Pathed Material Quadlet (4 char each)
+    AttachmentGroup: str = '-V'  # Composed Grouped Attached Material Quadlet (4 char each)
+    BigAttachmentGroup: str = '-0V'  # Composed Grouped Attached Material Quadlet (4 char each)
+    KERIACDCGenusVersion: str = '--AAA'  # KERI ACDC Protocol Stack CESR Version
 
     def __iter__(self):
         return iter(astuple(self))  # enables inclusion test with "in"
 
 CtrDex = CounterCodex()
 
 
-@dataclass(frozen=True)
-class ProtocolGenusCodex:
-    """ProtocolGenusCodex is codex of protocol genera for code table.
-
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-    KERI: str = '--AAA'  # KERI and ACDC Protocol Stacks share the same tables
-    ACDC: str = '--AAA'  # KERI and ACDC Protocol Stacks share the same tables
-
-
-    def __iter__(self):
-        return iter(astuple(self))  # enables inclusion test with "in"
-        # duplicate values above just result in multiple entries in tuple so
-        # in inclusion still works
-
-ProDex = ProtocolGenusCodex()  # Make instance
-
-
-@dataclass(frozen=True)
-class AltCounterCodex:
-    """
-    CounterCodex is codex hard (stable) part of all counter derivation codes.
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-    """
-
-    ControllerIdxSigs: str = '-A'  # Qualified Base64 Indexed Signature.
-    WitnessIdxSigs: str = '-B'  # Qualified Base64 Indexed Signature.
-    NonTransReceiptCouples: str = '-C'  # Composed Base64 Couple, pre+cig.
-    TransReceiptQuadruples: str = '-D'  # Composed Base64 Quadruple, pre+snu+dig+sig.
-    FirstSeenReplayCouples: str = '-E'  # Composed Base64 Couple, fnu+dts.
-    TransIdxSigGroups: str = '-F'  # Composed Base64 Group, pre+snu+dig+ControllerIdxSigs group.
-    SealSourceCouples: str = '-G'  # Composed Base64 couple, snu+dig of given delegators or issuers event
-    TransLastIdxSigGroups: str = '-H'  # Composed Base64 Group, pre+ControllerIdxSigs group.
-    SealSourceTriples: str = '-I'  # Composed Base64 triple, pre+snu+dig of anchoring source event
-    SadPathSig: str = '-J'  # Composed Base64 Group path+TransIdxSigGroup of SAID of content
-    SadPathSigGroup: str = '-K'  # Composed Base64 Group, root(path)+SaidPathCouples
-    PathedMaterialQuadlets: str = '-L'  # Composed Grouped Pathed Material Quadlet (4 char each)
-    MessageDataGroups: str = '-U'  # Composed Message Data Group or Primitive
-    AttachedMaterialQuadlets: str = '-V'  # Composed Grouped Attached Material Quadlet (4 char each)
-    MessageDataMaterialQuadlets: str = '-W'  # Composed Grouped Message Data Quadlet (4 char each)
-    CombinedMaterialQuadlets: str = '-X'  # Combined Message Data + Attachments Quadlet (4 char each)
-    MaterialGroups: str = '-Y'  # Composed Generic Material Group or Primitive
-    MaterialQuadlets: str = '-Z'  # Composed Generic Material Quadlet (4 char each)
-    BigMessageDataGroups: str = '-0U'  # Composed Message Data Group or Primitive
-    BigAttachedMaterialQuadlets: str = '-0V'  # Composed Grouped Attached Material Quadlet (4 char each)
-    BigMessageDataMaterialQuadlets: str = '-0W'  # Composed Grouped Message Data Quadlet (4 char each)
-    BigCombinedMaterialQuadlets: str = '-0X'  # Combined Message Data + Attachments Quadlet (4 char each)
-    BigMaterialGroups: str = '-0Y'  # Composed Generic Material Group or Primitive
-    BigMaterialQuadlets: str = '-0Z'  # Composed Generic Material Quadlet (4 char each)
-
-
-    def __iter__(self):
-        return iter(astuple(self))  # enables inclusion test with "in"
-
-
 class Counter:
     """
     Counter is fully qualified cryptographic material primitive base class for
     counter primitives (framing composition grouping count codes).
 
     Sub classes are derivation code and key event element context specific.
 
     Includes the following attributes and properties:
 
+    Class Attributes:
+
     Attributes:
 
     Properties:
         .code is  str derivation code to indicate cypher suite
         .raw is bytes crypto material only without code
         .pad  is int number of pad chars given raw
         .count is int count of grouped following material (not part of counter)
@@ -4764,22 +4605,26 @@
         ._raw is bytes value for .raw property
         ._pad is method to compute  .pad property
         ._count is int value for .count property
         ._infil is method to compute fully qualified Base64 from .raw and .code
         ._exfil is method to extract .code and .raw from fully qualified Base64
 
     """
-    Codex = CtrDex
     # Hards table maps from bytes Base64 first two code chars to int of
     # hard size, hs,(stable) of code. The soft size, ss, (unstable) for Counter
     # is always > 0 and hs + ss = fs always
     Hards = ({('-' + chr(c)): 2 for c in range(65, 65 + 26)})
     Hards.update({('-' + chr(c)): 2 for c in range(97, 97 + 26)})
     Hards.update([('-0', 3)])
     Hards.update([('--', 5)])
+
+    # Bards table maps to hard size, hs, of code from bytes holding sextets
+    # converted from first two code char. Used for ._bexfil.
+    Bards = ({codeB64ToB2(c): hs for c, hs in Hards.items()})
+
     # Sizes table maps hs chars of code to Sizage namedtuple of (hs, ss, fs)
     # where hs is hard size, ss is soft size, and fs is full size
     # soft size, ss, should always be  > 0 and hs+ss=fs for Counter
     Sizes = {
         '-A': Sizage(hs=2, ss=2, fs=4, ls=0),
         '-B': Sizage(hs=2, ss=2, fs=4, ls=0),
         '-C': Sizage(hs=2, ss=2, fs=4, ls=0),
@@ -4792,17 +4637,17 @@
         '-J': Sizage(hs=2, ss=2, fs=4, ls=0),
         '-K': Sizage(hs=2, ss=2, fs=4, ls=0),
         '-L': Sizage(hs=2, ss=2, fs=4, ls=0),
         '-V': Sizage(hs=2, ss=2, fs=4, ls=0),
         '-0V': Sizage(hs=3, ss=5, fs=8, ls=0),
         '--AAA': Sizage(hs=5, ss=3, fs=8, ls=0),
     }
-    # Bards table maps to hard size, hs, of code from bytes holding sextets
-    # converted from first two code char. Used for ._bexfil.
-    Bards = ({codeB64ToB2(c): hs for c, hs in Hards.items()})
+
+    Codex = CtrDex
+
 
     def __init__(self, code=None, count=None, countB64=None,
                  qb64b=None, qb64=None, qb2=None, strip=False):
         """
         Validate as fully qualified
         Parameters:
             code (str | None):  stable (hard) part of derivation code
@@ -5097,282 +4942,14 @@
         both = codeB2ToB64(qb2, cs)  # extract and convert both hard and soft part of code
         count = b64ToInt(both[hs:hs + ss])  # get count
 
         self._code = hard
         self._count = count
 
 
-class Sadder:
-    """
-    Sadder is self addressed data (SAD) serializer-deserializer class
-
-    Instance creation of a Sadder does not verifiy it .said property it merely
-    extracts it. In order to ensure Sadder instance has a verified .said then
-    must call .saider.verify(sad=self.ked)
-
-    Has the following public properties:
-
-    Properties:
-        raw (bytes): of serialized event only
-        ked (dict): self addressed data dict
-        kind (str): serialization kind coring.Serials such as JSON, CBOR, MGPK, CESR
-        size (int): number of bytes in serialization
-        version (Versionage): protocol version (Major, Minor)
-        proto (str): Protocolage value as protocol identifier such as KERI, ACDC
-        label (str): Saidage value as said field label
-        saider (Saider): of SAID of this SAD .ked['d'] if present
-        said (str): SAID of .saider qb64
-        saidb (bytes): SAID of .saider  qb64b
-        pretty (str): Pretty JSON of this SAD
-
-    Hidden Attributes:
-        ._raw is bytes of serialized event only
-        ._ked is key event dict
-        ._kind is serialization kind string value (see namedtuple coring.Serials)
-          supported kinds are 'json', 'cbor', 'msgpack', 'binary'
-        ._size is int of number of bytes in serialed event only
-        ._version is Versionage instance of event version
-        ._proto (str):  Protocolage value as protocol type identifier
-        ._saider (Saider): instance for this Sadder's SAID
-
-    Note:
-        loads and jumps of json use str whereas cbor and msgpack use bytes
-
-    """
-
-    def __init__(self, raw=b'', ked=None, sad=None, kind=None, saidify=False,
-                 code=MtrDex.Blake3_256):
-        """
-        Deserialize if raw provided does not verify assumes embedded said is valid
-        Serialize if ked provided but not raw verifies if verify is True?
-        When serializing if kind provided then use kind instead of field in ked
-
-        Parameters:
-          raw (bytes): serialized event
-          ked is key event dict or None
-            if None its deserialized from raw
-          kind is serialization kind string value or None (see namedtuple coring.Serials)
-            supported kinds are 'json', 'cbor', 'msgpack', 'binary'
-            if kind is None then its extracted from ked or raw
-          saidify (bool): True means compute said for ked
-          code is .diger default digest code for computing said .saider
-
-        """
-        self._code = code  # need default code for .saider
-        if raw:  # deserialize raw using property setter
-            self.raw = raw  # raw property setter does the deserialization
-        elif ked:  # serialize ked using property setter
-            #ToDo  when pass in ked and saidify True then compute said
-            self._kind = kind
-            self.ked = ked  # ked property setter does the serialization
-        elif sad:
-            # ToDo do we need this or should we be using ked above with saidify flag
-            self._clone(sad=sad)  # copy fields from sad
-        else:
-            raise ValueError("Improper initialization need sad, raw or ked.")
-
-
-    def _clone(self, sad):
-        """ copy hidden attributes from sad """
-        self._raw = sad.raw
-        self._ked = sad.ked
-        self._kind = sad.kind
-        self._size = sad.size
-        self._version = sad.version
-        self._proto = sad.proto
-        self._saider = sad.saider
-
-
-    def _inhale(self, raw):
-        """
-        Parses serilized event ser of serialization kind and assigns to
-        instance attributes.
-
-        Parameters:
-          raw is bytes of serialized event
-          kind is str of raw serialization kind (see namedtuple Serials)
-          size is int size of raw to be deserialized
-
-        Note:
-          loads and jumps of json use str whereas cbor and msgpack use bytes
-
-        """
-        proto, kind, version, size = sniff(raw)
-        if version != Version:
-            raise VersionError("Unsupported version = {}.{}, expected {}."
-                               "".format(version.major, version.minor, Version))
-        if len(raw) < size:
-            raise ShortageError("Need more bytes.")
-
-        ked = loads(raw=raw, size=size, kind=kind)
-
-        return ked, proto, kind, version, size
-
-
-    def _exhale(self, ked, kind=None):
-        """
-        Returns sizeify(ked, kind)
-
-        From sizeify
-        Returns tuple of (raw, proto, kind, ked, version) where:
-            raw (str): serialized event as bytes of kind
-            proto (str): protocol type as value of Protocolage
-            kind (str): serialzation kind as value of Serialage
-            ked (dict): key event dict or sad dict
-            version (Versionage): instance
-
-        Parameters:
-            ked (dict): key event dict or sad dict
-            kind (str): value of Serials serialization kind.
-                When not provided use
-
-        Assumes only supports Version
-        """
-        return sizeify(ked=ked, kind=kind)
-
-
-    def compare(self, said=None):
-        """
-        Returns True  if said and either .saider.qb64 or .saider.qb64b match
-        via string equality ==
-
-        Convenience method to allow comparison of own .saider digest self.raw
-        with some other purported said of self.raw
-
-        Parameters:
-            said is qb64b or qb64 SAID of ser to compare with .said
-
-        """
-
-        if said is not None:
-            if hasattr(said, "encode"):
-                said = said.encode('utf-8')  # makes bytes
-
-            return said == self.saidb  # matching
-
-        else:
-            raise ValueError("Both said and saider may not be None.")
-
-
-    @property
-    def raw(self):
-        """ raw property getter """
-        return self._raw
-
-    @raw.setter
-    def raw(self, raw):
-        """ raw property setter """
-        ked, proto, kind, version, size = self._inhale(raw=raw)
-        self._raw = bytes(raw[:size])  # crypto ops require bytes not bytearray
-        self._ked = ked
-        self._proto = proto
-        self._kind = kind
-        self._version = version
-        self._size = size
-        self._saider = Saider(qb64=ked["d"], code=self._code)
-
-    @property
-    def ked(self):
-        """ ked property getter"""
-        return self._ked
-
-    @ked.setter
-    def ked(self, ked):
-        """ ked property setter  assumes ._kind """
-        raw, proto, kind, ked, version = self._exhale(ked=ked, kind=self._kind)
-        size = len(raw)
-        self._raw = raw[:size]
-        self._ked = ked
-        self._proto = proto
-        self._kind = kind
-        self._size = size
-        self._version = version
-        self._saider = Saider(qb64=ked["d"], code=self._code)
-
-    @property
-    def kind(self):
-        """ kind property getter"""
-        return self._kind
-
-    @kind.setter
-    def kind(self, kind):
-        """ kind property setter Assumes ._ked. Serialization kind. """
-        raw, proto, kind, ked, version = self._exhale(ked=self._ked, kind=kind)
-        size = len(raw)
-        self._raw = raw[:size]
-        self._proto = proto
-        self._ked = ked
-        self._kind = kind
-        self._size = size
-        self._version = version
-        self._saider = Saider(qb64=ked["d"], code=self._code)
-
-
-    @property
-    def size(self):
-        """ size property getter"""
-        return self._size
-
-
-    @property
-    def version(self):
-        """
-        version property getter
-
-        Returns:
-            (Versionage):
-        """
-        return self._version
-
-
-    @property
-    def proto(self):
-        """ proto property getter
-        protocol identifier type value of Protocolage such as 'KERI' or 'ACDC'
-
-        Returns:
-            (str): Protocolage value as protocol type
-        """
-        return self._proto
-
-
-    @property
-    def saider(self):
-        """
-        Returns Diger of digest of self.raw
-        diger (digest material) property getter
-        """
-        return self._saider
-
-    @property
-    def said(self):
-        """
-        Returns str qb64  of .ked["d"] (said when ked is SAD)
-        said (self-addressing identifier) property getter
-        """
-        return self.saider.qb64
-
-    @property
-    def saidb(self):
-        """
-        Returns bytes qb64b of .ked["d"] (said when ked is SAD)
-        said (self-addressing identifier) property getter
-        """
-        return self.saider.qb64b
-
-    def pretty(self, *, size=1024):
-        """
-        Returns str JSON of .ked with pretty formatting
-
-        ToDo: add default size limit on pretty when used for syslog UDP MCU
-        like 1024 for ogler.logger
-        """
-        return json.dumps(self.ked, indent=1)[:size if size is not None else None]
-
-
 
 class Tholder:
     """
     Tholder is KERI Signing Threshold Satisfaction class
     .satisfy method evaluates satisfaction based on ordered list of indices of
     verified signatures where indices correspond to offsets in key list of
     associated signatures.
@@ -5387,30 +4964,38 @@
                         to know size of keys list in this case
 
         .limen is qualified b64 signing threshold suitable for CESR serialization.
             either Number.qb64b or Bexter.qb64b.
             The b64 portion of limen  with code stripped (Bexter.bext) of
               [["1/2", "1/2", "1/4", "1/4", "1/4"], ["1", "1"]]
               is '1s2c1s2c1s4c1s4c1s4a1c1' basically slash is 's', comma is 'c',
-              and ANDed clauses are delimited by 'a'.
+            ANDed clauses are delimited by 'a'.
+            Each clause top level weight may be optionally a weighted set of weights
+            delimited by 'k' for the weight on the set and 'v' for the weights in
+            the set.
+            [[{'1/3': ['1/2', '1/2', '1/2']}, '1/2', {'1/2': ['1', '1']}],
+                            ['1/2', {'1/2': ['1', '1']}]]
+            b'4AAKA1s3k1s2v1s2v1s2c1s2c1s2k1v1a1s2c1s2k1v1'
+
 
         .sith is original signing threshold suitable for value to be serialized
             as json, cbor, mgpk in key event message as either:
                 non-negative hex number str or
                 list of str rational number fractions >= 0 and <= 1 or
                 list of list of str rational number fractions >= 0 and <= 1
+                list of list of weighted map of weights
 
         .thold is parsed signing threshold suitable for calculating satisfaction.
             either as int or list of Fractions
 
         .num is int signing threshold when not ._weighted
 
     Methods:
-        .satisfy returns bool, True means ilist of verified signature key indices satisfies
-             threshold, False otherwise.
+        .satisfy returns bool, True means list of verified signature key indices
+        satisfies the threshold, False otherwise.
 
     Static Methods:
         weight (str): converts weight str expression into either int or Fraction
                     else raises ValueError must satisfy 0 <= w <= 1
                     Ensures strict proper rational number fraction of ints or
                     0 or 1
 
@@ -5429,50 +5014,58 @@
     """
 
     def __init__(self, *, thold=None , limen=None, sith=None, **kwa):
         """
         Accepts signing threshold in various forms so that may output correct
         forms for serialization and/or calculation of satisfaction.
 
-        Parameters:
-            sith is signing threshold (current or next) expressed as either:
-                non-negative int of threshold number (M-of-N threshold)
-                    next threshold may be zero
-                non-negative hex string of threshold number (M-of-N threshold)
-                    next threshold may be zero
-                fractional weight clauses which may be expressed as either:
-                    an iterable of rational number fraction strings  >= 0 and <= 1
-                    an iterable of iterables of rational number fraction strings >= 0 and <= 1
-                JSON serialized str of either:
-                   list of rational number fraction strings >= 0 and <= 1  or
-                   list of list of rational number fraction strings >= 0 and <= 1
+        The thold representation is meant to accept thresholds from computable
+        expressions for satisfaction of a threshold
 
+        The limen representation is meant to parse threshold expressions from
+        CESR serializations of key event message fields or attachments.
 
-            limen is qualified signing threshold (current or next) expressed as either:
-                Number.qb64 or .qb64b of integer threshold or
-                Bexter.qb64 or .qb64b of fractional weight clauses which may be either:
-                    Base64 delimited clauses of fractions
-                    Base64 delimited clauses of fractions
+        The sith representation is meant to parse threhold expressions from
+        deserializations of JSON, CBOR, or MGPK key event message fields  or
+        the command line or configuration files.
+
+
+        Parameters:
 
             thold is signing threshold (current or next) is suitable for computing
                 the satisfaction of a threshold and is expressed as either:
                     int of threshold number (M of N)
                     fractional weight clauses which may be expressed as either:
-                        an iterable of Fractions or
-                        an iterable of iterables of Fractions.
+                        sequence of either Fractions or tuples of Fraction and
+                            sequence of Fractions
+                        sequence of sequence of either Fractions or tuples of
+                            Fraction and sequence of Fractions
 
-        The sith representation is meant to parse threhold expressions from
-           deserializations of JSON, CBOR, or MGPK key event message fields  or
-           the command line or configuration files.
-
-        The limen representation is meant to parse threshold expressions from
-           CESR serializations of key event message fields or attachments.
+            limen is qualified signing threshold (current or next) expressed as either:
+                Number.qb64 or .qb64b of integer threshold or
+                Bexter.qb64 or .qb64b of fractional weight clauses which may be either:
+                    Base64 delimited clauses of fractions
+                    Base64 delimited clauses of fractions
 
-        The thold representation is meant to accept thresholds from computable
-            expressions for satisfaction of a threshold
+            sith is signing threshold (current or next) expressed as either:
+                non-negative int of threshold number (M-of-N threshold)
+                    next threshold may be zero
+                non-negative hex string of threshold number (M-of-N threshold)
+                    next threshold may be zero
+                fractional weight clauses which may be expressed as either:
+                    sequence of rational number fraction strings  >= 0 and <= 1
+                    sequence of either rational number fraction strings  >= 0 and <= 1 or
+                    map with key rational number string and value as sequence
+                    of rational number fraction strings
+                    rational number fraction string
+                    sequence of sequences of rational number fraction strings >= 0 and <= 1
+                    sequence of sequnces of either rational number fraction strings or
+                    map with key rational number fraction string with value sequence of
+                    rationaly number fraction strings
+                JSON serialized str of the above:
 
 
         """
         if thold is not None:
             self._processThold(thold=thold)
 
         elif limen is not None:
@@ -5509,17 +5102,32 @@
         return self._bexter.qb64b if self._weighted else self._number.qb64b
 
     @property
     def sith(self):
         """ sith property getter """
         # make sith expression of thold
         if self.weighted:
-            sith = [[f"{f.numerator}/{f.denominator}" if (0 < f < 1) else f"{int(f)}"
-                                           for f in clause]
-                                                   for clause in self.thold]
+            sith = []
+            for c in self.thold:
+                clause = []
+                for e in c:
+                    if isinstance(e, tuple):
+                        f = e[0]
+                        k = f"{f.numerator}/{f.denominator}" if (0 < f < 1) else f"{int(f)}"
+                        v = [f"{f.numerator}/{f.denominator}" if (0 < f < 1) else f"{int(f)}"
+                                for f in e[1]]
+                        clause.append({k: v})
+                    else:
+                        f = e
+                        clause.append(f"{f.numerator}/{f.denominator}" if (0 < f < 1) else f"{int(f)}")
+                sith.append(clause)
+
+            #sith = [[f"{f.numerator}/{f.denominator}" if (0 < f < 1) else f"{int(f)}"
+                                           #for f in clause]
+                                                   #for clause in self.thold]
             if len(sith) == 1:
                 sith = sith[0]  # simplify list of one clause to clause
         else:
             sith = f"{self.thold:x}"
 
         return sith
 
@@ -5535,19 +5143,19 @@
     @property
     def num(self):
         """ sith property getter """
         return self.thold if not self._weighted else None
 
 
 
-    def _processThold(self, thold: int | Iterable):
+    def _processThold(self, thold: int | Sequence):
         """Process thold input
 
         Parameters:
-            thold (int | Iterable): computable thold expression
+            thold (int | Sequence): computable thold expression
         """
         if isinstance(thold, int):
             self._processUnweighted(thold=thold)
 
         else:
             self._processWeighted(thold=thold)
 
@@ -5564,36 +5172,48 @@
             self._processUnweighted(thold=number.num)
 
         elif matter.code in BexDex:
             # Convert to fractional thold expression
             bexter = Bexter(raw=matter.raw, code=matter.code, **kwa)
             t = bexter.bext.replace('s', '/')
             # get clauses
-            thold = [clause.split('c') for clause in t.split('a')]
-            thold = [[self.weight(w) for w in clause] for clause in thold]
+            clauses = [clause.split('c') for clause in t.split('a')]
+
+            thold = []
+            for c in clauses:
+                clause = []
+                for e in c:
+                    k, s, v = e.partition("k")
+                    if s:  #not empty
+                        clause.append((self.weight(k), [self.weight(w) for w in v.split("v")]))
+                    else:
+                        clause.append(self.weight(k))
+
+                thold.append(clause)
+
             self._processWeighted(thold=thold)
 
         else:
             raise InvalidCodeError(f"Invalid code for limen = {matter.code}.")
 
 
-    def _processSith(self, sith: int | str | Iterable):
+    def _processSith(self, sith: int | str | Sequence):
         """
         Process attributes for fractionall weighted threshold sith
 
         Parameters:
             sith is signing threshold (current or next) expressed as either:
                 non-negative int of threshold number (M-of-N threshold)
                     next threshold may be zero
                 non-negative hex string of threshold number (M-of-N threshold)
                     next threshold may be zero
                 fractional weight clauses which may be expressed as either:
-                    an iterable of rational number fraction weight str or int str
+                    an sequence of rational number fraction weight str or int str
                         each denoted w where 0 <= w <= 1
-                    an iterable of iterables of rational number fraction weight
+                    an sequence of sequences of rational number fraction weight
                        or int str
                        each denoted w where 0 <= w <= 1>= 0
                 JSON serialized str of either:
                     list of rational number fraction weight strings
                         each denoted w where 0 <= w <= 1
                     list of lists of rational number fraction weight strings
                         each denoted w where 0 <= w <= 1
@@ -5602,40 +5222,55 @@
         """
         if isinstance(sith, int):
             self._processUnweighted(thold=sith)
 
         elif isinstance(sith, str) and '[' not in sith:
             self._processUnweighted(thold=int(sith, 16))
 
-        else:  # assumes iterable of weights or iterable of iterables of weights
+        else:  # assumes sequence of weights or sequence of sequence of weights
             if isinstance(sith, str):  # json of weighted sith from cli
                 sith = json.loads(sith)  # deserialize
 
-            if not sith:  # empty iterable
+            if not sith:  # empty or None
                 raise ValueError(f"Empty weight list = {sith}.")
 
-            # because all([]) == True  have to also test for emply mask
-            # is it non str iterable of non str iterable of strs
-            mask = [nonStringIterable(c) for c in sith]
-            if mask and not all(mask):  # not empty and not iterable of iterables
-                sith = [sith]  # attempt to make Iterable of Iterables
+            # is it non str sequence of sequences? or non str sequnce of strs?
+            # must test for emply mask because all([]) == True
+            mask = [nonStringSequence(c) for c in sith]  # check each element
+            if mask and not all(mask):  # not empty and not sequence of sequenes
+                sith = [sith]  # attempt to make sequnce of sequqnces of strs
 
             for c in sith:  # get each clause
-                mask = [isinstance(w, str) for w in c]  # must be all strs
-                if mask and not all(mask):  # not empty and not iterable of strs?
+                # each element of a clause must be a str or dict
+                mask = [(isinstance(w, str) or isinstance(w, Mapping)) for w in c]
+                if mask and not all(mask):  # not empty and not sequence of str or dicts
                     raise ValueError(f"Invalid sith = {sith} some weights in"
                                      f"clause {c} are non string.")
 
-
             # replace weight str expression, int str or fractional strings with
             # int or fraction as appropriate.
             thold = []
-            for clause in sith:  # convert string fractions to Fractions
-                # append list of weights converted fromnn str expression
-                thold.append([self.weight(w) for w in clause])
+            for c in sith:  # convert string fractions to Fractions
+                # append list of where each element is either bare weight or
+                # single key map with value as list of weights
+                # each weight is converted from its  str expression
+                clause = []
+                for e in c:  # each element of clause c
+                    if isinstance(e, Mapping):
+                        if len(e) != 1:
+                            raise ValueError(f"Invalid sith = {sith} nested "
+                                             f"weight map {e} in clause {c} "
+                                             f" not single key value.")
+                        k = list(e)[0]  # zeroth key is used
+                        # convert to tuple of (weight, [list of weights])
+                        clause.append((self.weight(k), [self.weight(w) for w in e[k]]))
+                    else:
+                        clause.append(self.weight(e))
+
+                thold.append(clause)
 
             self._processWeighted(thold=thold)
 
 
     def _processUnweighted(self, thold=0):
         """
         Process attributes for unweighted (numeric) threshold thold
@@ -5659,42 +5294,62 @@
         Process attributes for fractionall weighted threshold thold
 
         Parameters:
             thold (iterable):  iterable or iterable or iterables of
                 rational number fraction strings  >= 0 and <= 1
 
         """
-        for clause in thold:  # sum of fractions in clause must be >= 1
-            if not (sum(clause) >= 1):
-                raise ValueError(f"Invalid sith clause = {thold}, all "
+        for clause in thold:  # sum of top level weights in clause must be >= 1
+            # When element is dict then sum of value's weights must be >= 1
+            top = []  # top level weights
+            for e in clause:
+                if isinstance(e, tuple):
+                    top.append(e[0])
+                    if not (sum(e[1]) >= 1):
+                        raise ValueError(f"Invalid sith clause = {clause}, "
+                                         f"element = {e}. All nested clause "
+                                         f"weight sums must be >= 1.")
+                else:
+                    top.append(e)
+            if not (sum(top) >= 1):
+                raise ValueError(f"Invalid sith clause = {clause}, all top level"
                                  f"clause weight sums must be >= 1.")
 
         self._thold = thold
         self._weighted = True
-        self._size = sum(len(clause) for clause in thold)
+        #self._size = sum(len(clause) for clause in thold)
+        s = 0
+        for clause in thold:
+            for e in clause:
+                if isinstance(e, tuple):
+                    s += len(e[1])
+                else:
+                    s += 1
+        self._size = s
+
         self._satisfy = self._satisfy_weighted
         # make bext str of thold for .bexter for limen
-        bext = [[f"{f.numerator}s{f.denominator}" if (0 < f < 1) else f"{int(f)}"
-                                           for f in clause]
-                                                           for clause in thold]
-        bext = "a".join(["c".join(clause) for clause in bext])
-        self._number = None
-        self._bexter = Bexter(bext=bext)
-
+        ta = []  # list of list of fractions and/or single element map of fractions
+        for c in thold:
+            bc = []  # list of fractions and/or single element map of fractions
+            for e in c:
+                if isinstance(e, tuple):
+                    f = e[0]
+                    k = f"{f.numerator}s{f.denominator}" if (0 < f < 1) else f"{int(f)}"
+                    v = "v".join([f"{f.numerator}s{f.denominator}" if (0 < f < 1) else f"{int(f)}" for f in e[1]])
+                    kv = "k".join([k, v])
+                    bc.append(kv)
+                else:
+                    bc.append(f"{e.numerator}s{e.denominator}" if (0 < e < 1) else f"{int(e)}")
 
-    @staticmethod
-    def _oldcheckWeight(w: Fraction) -> Fraction:
-        """Returns w if 0 <= w <= 1 Else raises ValueError
+            ta.append(bc)
 
-        Parameters:
-            w (Fraction): Threshold weight Fraction
-        """
-        if not 0 <= w <= 1:
-            raise ValueError(f"Invalid weight not 0 <= {w} <= 1.")
-        return w
+        bext = "a".join(["c".join(bc) for bc in ta])
+        self._number = None
+        self._bexter = Bexter(bext=bext)
 
 
     @staticmethod
     def weight(w: str) -> Fraction:
         """Returns valid weight from w else raises error (ValueError or TypeError).
         w expression must evaluate to 0, 1, or strict proper rational fraction.
         w expression must be 0 <= w <= 1 Else raises ValueError
@@ -5769,30 +5424,377 @@
             sats = [False] * self.size  # default all satifactions to False
             for idx in indices:
                 sats[idx] = True  # set verified signature index to True
 
             wio = 0  # weight index offset
             for clause in self.thold:
                 cw = 0  # init clause weight
-                for w in clause:
-                    if sats[wio]:  # verified signature so weight applies
-                        cw += w
-                    wio += 1
+                for e in clause:
+                    if isinstance(e, tuple):
+                        vw = 0  # init element value weight
+                        for w in e[1]:   # sum weights of value
+                            if sats[wio]:
+                                vw += w
+                            wio += 1
+                        if vw >= 1:  # element true
+                            cw += e[0]  # add element key weight to clause weight
+                    else:
+                        w = e
+                        if sats[wio]:  # verified signature so weight applies
+                            cw += w
+                        wio += 1
                 if cw < 1:  # each clause must sum to at least 1
                     return False
 
-            return True  # all clauses including final one cw >= 1
+            return True  # all clauses have cw >= 1 including final one, AND true
 
         except Exception as ex:
             return False
 
         return False
 
 
 
+class Streamer:
+    """
+    Streamer is CESR sniffable stream class
+
+
+    Has the following public properties:
+
+    Properties:
+
+
+    Methods:
+
+
+    Hidden:
+
+
+
+    """
+
+    def __init__(self, stream):
+        """Initialize instance
+
+
+        Parameters:
+            stream (bytes | bytearray): sniffable CESR stream
+
+
+        """
+        self._stream = bytes(stream)
+
+
+    @property
+    def stream(self):
+        """stream property getter
+        """
+        return self._stream
+
+    @property
+    def text(self):
+        """expanded stream as qb64 text
+        Returns:
+           stream (bytes): expanded text qb64 version of stream
+
+        """
+        return self._stream
+
+    @property
+    def binary(self):
+        """compacted stream as qb2 binary
+        Returns:
+           stream (bytes): compacted binary qb2 version of stream
+
+        """
+        return self._stream
+
+    @property
+    def texter(self):
+        """expanded stream as Texter instance
+        Returns:
+           texter (Texter): Texter primitive of stream suitable wrapping
+
+        """
+        return self._stream
+
+
+
+
+class Sadder:
+    """
+    Sadder is self addressed data (SAD) serializer-deserializer class
+
+    Instance creation of a Sadder does not verifiy it .said property it merely
+    extracts it. In order to ensure Sadder instance has a verified .said then
+    must call .saider.verify(sad=self.ked)
+
+    Has the following public properties:
+
+    Properties:
+        raw (bytes): of serialized event only
+        ked (dict): self addressed data dict
+        kind (str): serialization kind coring.Serials such as JSON, CBOR, MGPK, CESR
+        size (int): number of bytes in serialization
+        version (Versionage): protocol version (Major, Minor)
+        proto (str): Protocolage value as protocol identifier such as KERI, ACDC
+        label (str): Saidage value as said field label
+        saider (Saider): of SAID of this SAD .ked['d'] if present
+        said (str): SAID of .saider qb64
+        saidb (bytes): SAID of .saider  qb64b
+        pretty (str): Pretty JSON of this SAD
+
+    Hidden Attributes:
+        ._raw is bytes of serialized event only
+        ._ked is key event dict
+        ._kind is serialization kind string value (see namedtuple coring.Serials)
+          supported kinds are 'json', 'cbor', 'msgpack', 'binary'
+        ._size is int of number of bytes in serialed event only
+        ._version is Versionage instance of event version
+        ._proto (str):  Protocolage value as protocol type identifier
+        ._saider (Saider): instance for this Sadder's SAID
+
+    Note:
+        loads and jumps of json use str whereas cbor and msgpack use bytes
+
+    """
+    MaxVSOffset = 12
+    SmellSize = MaxVSOffset + MAXVERFULLSPAN  # min buffer size to inhale
+
+    def __init__(self, raw=b'', ked=None, sad=None, kind=None, saidify=False,
+                 code=MtrDex.Blake3_256):
+        """
+        Deserialize if raw provided does not verify assumes embedded said is valid
+        Serialize if ked provided but not raw verifies if verify is True?
+        When serializing if kind provided then use kind instead of field in ked
+
+        Parameters:
+          raw (bytes): serialized event
+          ked is key event dict or None
+            if None its deserialized from raw
+          kind is serialization kind string value or None (see namedtuple coring.Serials)
+            supported kinds are 'json', 'cbor', 'msgpack', 'binary'
+            if kind is None then its extracted from ked or raw
+          saidify (bool): True means compute said for ked
+          code is .diger default digest code for computing said .saider
+
+        """
+        self._code = code  # need default code for .saider
+        if raw:  # deserialize raw using property setter
+            self.raw = raw  # raw property setter does the deserialization
+        elif ked:  # serialize ked using property setter
+            #ToDo  when pass in ked and saidify True then compute said
+            self._kind = kind
+            self.ked = ked  # ked property setter does the serialization
+        elif sad:
+            # ToDo do we need this or should we be using ked above with saidify flag
+            self._clone(sad=sad)  # copy fields from sad
+        else:
+            raise ValueError("Improper initialization need sad, raw or ked.")
+
+
+    def _clone(self, sad):
+        """ copy hidden attributes from sad """
+        self._raw = sad.raw
+        self._ked = sad.ked
+        self._kind = sad.kind
+        self._size = sad.size
+        self._version = sad.version
+        self._proto = sad.proto
+        self._saider = sad.saider
+
+
+    def _inhale(self, raw):
+        """
+        Parses serilized event ser of serialization kind and assigns to
+        instance attributes.
+
+        Parameters:
+          raw is bytes of serialized event
+          kind is str of raw serialization kind (see namedtuple Serials)
+          size is int size of raw to be deserialized
+
+        Note:
+          loads and jumps of json use str whereas cbor and msgpack use bytes
+
+        """
+        proto, vrsn, kind, size, _ = smell(raw)
+        if vrsn != Version:
+            raise VersionError("Unsupported version = {}.{}, expected {}."
+                               "".format(vrsn.major, vrsn.minor, Version))
+
+        ked = loads(raw=raw, size=size, kind=kind)
+
+        return ked, proto, kind, vrsn, size
+
+
+    def _exhale(self, ked, kind=None):
+        """
+        Returns sizeify(ked, kind)
+
+        From sizeify
+        Returns tuple of (raw, proto, kind, ked, version) where:
+            raw (str): serialized event as bytes of kind
+            proto (str): protocol type as value of Protocolage
+            kind (str): serialzation kind as value of Serialage
+            ked (dict): key event dict or sad dict
+            version (Versionage): instance
+
+        Parameters:
+            ked (dict): key event dict or sad dict
+            kind (str): value of Serials serialization kind.
+                When not provided use
+
+        Assumes only supports Version
+        """
+        return sizeify(ked=ked, kind=kind)
+
+
+    def compare(self, said=None):
+        """
+        Returns True  if said and either .saider.qb64 or .saider.qb64b match
+        via string equality ==
+
+        Convenience method to allow comparison of own .saider digest self.raw
+        with some other purported said of self.raw
+
+        Parameters:
+            said is qb64b or qb64 SAID of ser to compare with .said
+
+        """
+
+        if said is not None:
+            if hasattr(said, "encode"):
+                said = said.encode('utf-8')  # makes bytes
+
+            return said == self.saidb  # matching
+
+        else:
+            raise ValueError("Both said and saider may not be None.")
+
+
+    @property
+    def raw(self):
+        """ raw property getter """
+        return self._raw
+
+    @raw.setter
+    def raw(self, raw):
+        """ raw property setter """
+        ked, proto, kind, version, size = self._inhale(raw=raw)
+        self._raw = bytes(raw[:size])  # crypto ops require bytes not bytearray
+        self._ked = ked
+        self._proto = proto
+        self._kind = kind
+        self._version = version
+        self._size = size
+        self._saider = Saider(qb64=ked["d"], code=self._code)
+
+    @property
+    def ked(self):
+        """ ked property getter"""
+        return self._ked
+
+    @ked.setter
+    def ked(self, ked):
+        """ ked property setter  assumes ._kind """
+        raw, proto, kind, ked, version = self._exhale(ked=ked, kind=self._kind)
+        size = len(raw)
+        self._raw = raw[:size]
+        self._ked = ked
+        self._proto = proto
+        self._kind = kind
+        self._size = size
+        self._version = version
+        self._saider = Saider(qb64=ked["d"], code=self._code)
+
+    @property
+    def kind(self):
+        """ kind property getter"""
+        return self._kind
+
+    @kind.setter
+    def kind(self, kind):
+        """ kind property setter Assumes ._ked. Serialization kind. """
+        raw, proto, kind, ked, version = self._exhale(ked=self._ked, kind=kind)
+        size = len(raw)
+        self._raw = raw[:size]
+        self._proto = proto
+        self._ked = ked
+        self._kind = kind
+        self._size = size
+        self._version = version
+        self._saider = Saider(qb64=ked["d"], code=self._code)
+
+
+    @property
+    def size(self):
+        """ size property getter"""
+        return self._size
+
+
+    @property
+    def version(self):
+        """
+        version property getter
+
+        Returns:
+            (Versionage):
+        """
+        return self._version
+
+
+    @property
+    def proto(self):
+        """ proto property getter
+        protocol identifier type value of Protocolage such as 'KERI' or 'ACDC'
+
+        Returns:
+            (str): Protocolage value as protocol type
+        """
+        return self._proto
+
+
+    @property
+    def saider(self):
+        """
+        Returns Diger of digest of self.raw
+        diger (digest material) property getter
+        """
+        return self._saider
+
+    @property
+    def said(self):
+        """
+        Returns str qb64  of .ked["d"] (said when ked is SAD)
+        said (self-addressing identifier) property getter
+        """
+        return self.saider.qb64
+
+    @property
+    def saidb(self):
+        """
+        Returns bytes qb64b of .ked["d"] (said when ked is SAD)
+        said (self-addressing identifier) property getter
+        """
+        return self.saider.qb64b
+
+    def pretty(self, *, size=1024):
+        """
+        Returns str JSON of .ked with pretty formatting
+
+        ToDo: add default size limit on pretty when used for syslog UDP MCU
+        like 1024 for ogler.logger
+        """
+        return json.dumps(self.ked, indent=1)[:size if size is not None else None]
+
+
+
+
 class Dicter:
     """ Dicter class is base class for objects that can be stored in a Suber
 
     Dicter classes can be initialized by a dict and then expose bytes of JSON
     in the .raw property  Subclasses can add semantically appropriate properties
     that extract / add specific keys to the underlying dict .pad
 
@@ -5863,16 +5865,7 @@
 
         ToDo: add default size limit on pretty when used for syslog UDP MCU
         like 1024 for ogler.logger
         """
         return json.dumps(self.pad, indent=1)[:size if size is not None else None]
 
 
-def randomNonce():
-    """ Generate a random ed25519 seed and encode as qb64
-
-    Returns:
-        str: qb64 encoded ed25519 random seed
-    """
-    preseed = pysodium.randombytes(pysodium.crypto_sign_SEEDBYTES)
-    seedqb64 = Matter(raw=preseed, code=MtrDex.Ed25519_Seed).qb64
-    return seedqb64
```

### Comparing `keri-1.1.9/src/keri/core/eventing.py` & `keri-1.2.dev0/src/keri/core/eventing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,71 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 """
 keri.core.eventing module
 
 """
 import datetime
 import json
 import logging
 from collections import namedtuple
 from dataclasses import dataclass, astuple, asdict, field
 from urllib.parse import urlsplit
 from math import ceil
 from ordered_set import OrderedSet as oset
 from hio.help import decking
 
-from . import coring, serdering
-from .coring import (versify, Serials, Ilks, MtrDex, PreDex, DigDex,
-                     NonTransDex, CtrDex, Counter,
-                     Number, Seqner, Siger, Cigar, Dater, Indexer, IdrDex,
-                     Verfer, Diger, Prefixer, Tholder, Saider)
-from . import serdering
-from .. import help
-from .. import kering
-from ..db import basing, dbing
-from ..db.basing import KeyStateRecord, StateEERecord
-from ..db.dbing import dgKey, snKey, fnKey, splitKeySN, splitKey
 
+from .. import kering
 from ..kering import (MissingEntryError,
                       ValidationError, DerivationError, MissingSignatureError,
                       MissingWitnessSignatureError, UnverifiedReplyError,
                       MissingDelegationError, OutOfOrderError,
                       LikelyDuplicitousError, UnverifiedWitnessReceiptError,
-                      UnverifiedReceiptError, UnverifiedTransferableReceiptError, QueryNotFoundError)
-from ..kering import Version, Versionage
-from ..kering import (ICP_LABELS, DIP_LABELS, ROT_LABELS, DRT_LABELS, IXN_LABELS,
-                       RPY_LABELS)
+                      UnverifiedReceiptError, UnverifiedTransferableReceiptError,
+                      QueryNotFoundError, MisfitEventSourceError,
+                      MissingDelegableApprovalError)
+from ..kering import Version, Versionage, TraitCodex, TraitDex
+from ..kering import Coldage, Colds, ColdDex
 
+from .. import help
 from ..help import helping
 
-logger = help.ogler.getLogger()
+from . import coring
+from .coring import (versify, Serials, Ilks, MtrDex, PreDex, DigDex,
+                     NonTransDex, CtrDex, Counter,
+                     Number, Seqner, Cigar, Dater,
+                     Verfer, Diger, Prefixer, Tholder, Saider)
 
-EscrowTimeoutPS = 3600  # seconds for partial signed escrow timeout
+from . import indexing
+from .indexing import (IdrDex, Indexer, Siger)
 
-MaxIntThold = 2 ** 32 - 1
+from . import serdering
 
-@dataclass(frozen=True)
-class TraitCodex:
-    """
-    TraitCodex is codex of inception configuration trait code strings
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
+from ..db import basing, dbing
+from ..db.basing import KeyStateRecord, StateEERecord
+from ..db.dbing import dgKey, snKey, fnKey, splitKeySN, splitKey
 
-    """
-    EstOnly: str = 'EO'  # Only allow establishment events
-    DoNotDelegate: str = 'DND'  # Dot not allow delegated identifiers
-    NoBackers: str = 'NB'  # Do not allow any registrar backers
-    Backers: str = 'RB' # Registrar backer provided in Registrar seal
 
-    def __iter__(self):
-        return iter(astuple(self))
+logger = help.ogler.getLogger()
 
+EscrowTimeoutPS = 3600  # seconds for partial signed escrow timeout
 
-TraitDex = TraitCodex()  # Make instance
+MaxIntThold = 2 ** 32 - 1
 
 # Location of last establishment key event: sn is int, dig is qb64 digest
 LastEstLoc = namedtuple("LastEstLoc", 's d')
 
 #  for the following Seal namedtuples use the ._asdict() method to convert to dict
 #  when using in events
 # to convert seal namedtuple to dict use namedtuple._asdict()
 # seal == SealEvent(i="abc",s="1",d="efg")
 # sealdict =seal._asdict()
 # to convet dict to namedtuple use ** unpacking as in seal = SealDigest(**sealdict)
 # to check if dict of seal matches fields of associted namedtuple
-# if tuple(sealdict.keys()) == SealEvent._fields:
+# if tuple(sealdict) == SealEvent._fields:
 
 # Digest Seal: uniple (d,)
 # d = digest qb64 of data  (usually SAID)
 SealDigest = namedtuple("SealDigest", 'd')
 
 # Root Seal: uniple (rd,)
 # rd = Merkle tree root digest qb64 digest of anchored (sealed) data in Merkle tree
@@ -94,82 +83,36 @@
 SealEvent = namedtuple("SealEvent", 'i s d')
 
 # Last Estalishment Event Seal: uniple (i,)
 # i = pre is qb64 of identifier prefix of KEL from which to get last est, event
 # used to indicate to get the latest keys available from KEL for 'i'
 SealLast = namedtuple("SealLast", 'i')
 
-# Establishment Event for Source of Message: duple (s, d)
-# s = sn of event as lowercase hex string  no leading zeros,
-# d = SAID digest qb64 of event
-# the pre is provided in the 'i' field of the message itself which is the qb64
-# of identifier prefix of KEL from which to get  est, event given by 's d'
-# use SealSourceCouples count code for attachment
-SealEst = namedtuple("SealEst", 's d')
-
-# State (latest current) Event: triple (s, t, d)
-# s = sn of latest event as lowercase hex string  no leading zeros,
-# t = message type of latest event (ilk)
-# d = SAID digest qb64 of latest event
-StateEvent = namedtuple("StateEvent", 's t d')
-
-# State (latest current) Establishment Event: quadruple (s, d, br, ba)
+# State Establishment Event (latest current) : quadruple (s, d, br, ba)
 # s = sn of latest est event as lowercase hex string  no leading zeros,
 # d = SAID digest qb64  of latest establishment event
 # br = backer (witness) remove list (cuts) from latest est event
 # ba = backer (witness) add list (adds) from latest est event
 StateEstEvent = namedtuple("StateEstEvent", 's d br ba')
 
+# Transaction Event Seal for Transaction Event: duple (s, d)
+# s = sn of transaction event as lowercase hex string  no leading zeros,
+# d = SAID digest qb64 of transaction event
+# the pre is provided in the 'i' field  qb64 of identifier prefix of KEL
+# key event that this seal appears.
+# use SealSourceCouples count code for attachment
+SealTrans = namedtuple("SealTrans", 's d')
 
-@dataclass(frozen=True)
-class ColdCodex:
-    """
-    ColdCodex is codex of cold stream start tritets of first byte
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-
-    First three bits:
-        0o0 = 000 free
-        0o1 = 001 cntcode B64
-        0o2 = 010 opcode B64
-        0o3 = 011 json
-        0o4 = 100 mgpk
-        0o5 = 101 cbor
-        0o6 = 110 mgpk
-        007 = 111 cntcode or opcode B2
-
-    status is one of ('evt', 'txt', 'bny' )
-    'evt' if tritet in (ColdDex.JSON, ColdDex.MGPK1, ColdDex.CBOR, ColdDex.MGPK2)
-    'txt' if tritet in (ColdDex.CtB64, ColdDex.OpB64)
-    'bny' if tritet in (ColdDex.CtOpB2,)
-
-    otherwise raise ColdStartError
-
-    x = bytearray([0x2d, 0x5f])
-    x == bytearray(b'-_')
-    x[0] >> 5 == 0o1
-    True
-    """
-    Free: int = 0o0  # not taken
-    CtB64: int = 0o1  # CountCode Base64
-    OpB64: int = 0o2  # OpCode Base64
-    JSON: int = 0o3  # JSON Map Event Start
-    MGPK1: int = 0o4  # MGPK Fixed Map Event Start
-    CBOR: int = 0o5  # CBOR Map Event Start
-    MGPK2: int = 0o6  # MGPK Big 16 or 32 Map Event Start
-    CtOpB2: int = 0o7  # CountCode or OpCode Base2
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-
-ColdDex = ColdCodex()  # Make instance
+# not used should this be depricated
+# State Event (latest current) : triple (s, t, d)
+# s = sn of latest event as lowercase hex string  no leading zeros,
+# t = message type of latest event (ilk)
+# d = SAID digest qb64 of latest event
+StateEvent = namedtuple("StateEvent", 's t d')
 
-Coldage = namedtuple("Coldage", 'msg txt bny')  # stream cold start status
-Colds = Coldage(msg='msg', txt='txt', bny='bny')
 
 
 # Future make Cues dataclasses  instead of dicts. Dataclasses so may be converted
 # to/from dicts easily  example: dict(kin="receipt", serder=serder)
 
 
 def simple(n):
@@ -410,52 +353,14 @@
     if not strip:
         data = data[len(ssaider.qb64b):]
     siger = Siger(qb64b=data, strip=strip)  # indexed siger of event
 
     return esaider, sprefixer, sseqner, ssaider, siger
 
 
-def validateSN(sn, inceptive=None):
-    """
-    Returns:
-        sn (int): converted from sn hex str
-
-    Raises ValueError if invalid sn
-
-    Parameters:
-       sn (str): hex char sequence number of event or seal in an event
-       inceptive(bool): Check sn value and raise ValueError if invalid
-                        None means check for sn < 0
-                        True means check for sn != 0
-                        False means check for sn < 1
-
-    """
-    if len(sn) > 32:
-        raise ValueError("Invalid sn = {} too large.".format(sn))
-
-    try:
-        sn = int(sn, 16)
-    except Exception as ex:
-        raise ValueError("Invalid sn = {}.".format(sn))
-
-    if inceptive is not None:
-        if inceptive:
-            if sn != 0:
-                raise ValidationError("Nonzero sn = {} for inception evt."
-                                      "".format(sn))
-        else:
-            if sn < 1:
-                raise ValidationError("Zero or less sn = {} for non-inception evt."
-                                      "".format(sn))
-    else:
-        if sn < 0:
-            raise ValidationError("Negative sn = {} for event.".format(sn))
-
-    return sn
-
 
 def verifySigs(raw, sigers, verfers):
     """
     Returns tuple of (vsigers, vindices) where:
         vsigers is list  of unique verified sigers with assigned verfer
         vindices is list of indices from those verified sigers
 
@@ -851,40 +756,14 @@
     if code is not None and code in PreDex:  # use code to override all else
         saids = {'i': code}
 
     serder = serdering.SerderKERI(sad=ked, makify=True, saids=saids)
     serder._verify()  # raises error if fails verifications
     return serder
 
-    #if delpre is not None:  # delegated inception with ilk = dip
-        #ked['di'] = delpre
-        #if code is None:
-            #code = MtrDex.Blake3_256  # force digestive
-
-    #if delpre is None and code is None and len(keys) == 1:
-        #prefixer = Prefixer(qb64=keys[0])  # defaults to not digestive code
-        #if prefixer.digestive:
-            #raise ValueError("Invalid code, digestive={}, must be derived from"
-                             #" ked.".format(prefixer.code))
-    #else:  # digestive
-        ## raises derivation error if non-empty nxt but ephemeral code
-        #prefixer = Prefixer(ked=ked, code=code)  # Derive AID from ked and code
-
-        #if delpre is not None:
-            #if not prefixer.digestive:
-                #raise ValueError(f"Invalid derivation code = {prefixer.code} "
-                                 #f"for delegation. Must be digestive")
-
-    #ked["i"] = prefixer.qb64  # update pre element in ked with pre qb64
-    #if prefixer.digestive:
-        #ked["d"] = prefixer.qb64
-    #else:
-        #_, ked = coring.Saider.saidify(sad=ked)
-
-    #return Serder(ked=ked)  # return serialized ked
 
 def delcept(keys, delpre, **kwa):
     """
     Returns serder of delegated inception event message.
     Utility function to automate creation of delegated inception events.
     Syntactic suger that calls incept but with delpre so ilk is dip.
 
@@ -1462,15 +1341,15 @@
             atc.extend(cigar.verfer.qb64b)
             atc.extend(cigar.qb64b)
 
     if pipelined:
         if len(atc) % 4:
             raise ValueError("Invalid attachments size={}, nonintegral"
                              " quadlets.".format(len(atc)))
-        msg.extend(Counter(code=CtrDex.AttachedMaterialQuadlets,
+        msg.extend(Counter(code=CtrDex.AttachmentGroup,
                            count=(len(atc) // 4)).qb64b)
 
     msg.extend(atc)
     return msg
 
 
 def proofize(sadtsgs=None, *, sadsigers=None, sadcigars=None, pipelined=False):
@@ -1494,38 +1373,38 @@
     sadtsgs = [] if sadtsgs is None else sadtsgs
     sadsigers = [] if sadsigers is None else sadsigers
     sadcigars = [] if sadcigars is None else sadcigars
 
     count = 0
     for (pather, sigers) in sadsigers:
         count += 1
-        atc.extend(coring.Counter(coring.CtrDex.SadPathSig, count=1).qb64b)
+        atc.extend(coring.Counter(coring.CtrDex.SadPathSigGroups, count=1).qb64b)
         atc.extend(pather.qb64b)
 
         atc.extend(coring.Counter(code=coring.CtrDex.ControllerIdxSigs, count=len(sigers)).qb64b)
         for siger in sigers:
             atc.extend(siger.qb64b)
 
     for (pather, prefixer, seqner, saider, sigers) in sadtsgs:
         count += 1
-        atc.extend(coring.Counter(coring.CtrDex.SadPathSig, count=1).qb64b)
+        atc.extend(coring.Counter(coring.CtrDex.SadPathSigGroups, count=1).qb64b)
         atc.extend(pather.qb64b)
 
         atc.extend(coring.Counter(coring.CtrDex.TransIdxSigGroups, count=1).qb64b)
         atc.extend(prefixer.qb64b)
         atc.extend(seqner.qb64b)
         atc.extend(saider.qb64b)
 
         atc.extend(coring.Counter(code=coring.CtrDex.ControllerIdxSigs, count=len(sigers)).qb64b)
         for siger in sigers:
             atc.extend(siger.qb64b)
 
     for (pather, cigars) in sadcigars:
         count += 1
-        atc.extend(coring.Counter(coring.CtrDex.SadPathSig, count=1).qb64b)
+        atc.extend(coring.Counter(coring.CtrDex.SadPathSigGroups, count=1).qb64b)
         atc.extend(pather.qb64b)
 
         atc.extend(coring.Counter(code=coring.CtrDex.NonTransReceiptCouples, count=len(sadcigars)).qb64b)
         for cigar in cigars:
             if cigar.verfer.code not in coring.NonTransDex:
                 raise ValueError("Attempt to use tranferable prefix={} for "
                                  "receipt.".format(cigar.verfer.qb64))
@@ -1534,20 +1413,20 @@
 
     msg = bytearray()
 
     if pipelined:
         if len(atc) % 4:
             raise ValueError("Invalid attachments size={}, nonintegral"
                              " quadlets.".format(len(atc)))
-        msg.extend(coring.Counter(code=coring.CtrDex.AttachedMaterialQuadlets,
+        msg.extend(coring.Counter(code=coring.CtrDex.AttachmentGroup,
                                   count=(len(atc) // 4)).qb64b)
 
     if count > 1:
         root = coring.Pather(bext="-")
-        msg.extend(coring.Counter(code=coring.CtrDex.SadPathSigGroup, count=count).qb64b)
+        msg.extend(coring.Counter(code=coring.CtrDex.RootSadPathSigGroups, count=count).qb64b)
         msg.extend(root.qb64b)
 
     msg.extend(atc)
     return msg
 
 
 class Kever:
@@ -1569,18 +1448,14 @@
         db (Baser | None): instance that manages the LMDB database when provided.
             When None provided then create and assign vacuous instance of Baser.
         cues (deque | None): Injected Kevery.cues when provided. Default None.
         prefixes (list | None): Injected from Kevery when provided.
             qb64 identifier prefixes of own habitat identifiers.
             Assign db.prefixes when None
             When empty operate in promiscuous mode
-        local (bool): Injected from kevery when provided.
-            True means only process msgs for own events when .prefixes is not empty
-            False means only process msgs for not own events when .prefixes is not empty
-                Default is False.
         version (Versionage): serder.version instance of current event state version
         prefixer (Prefixer):  instance for current event state
         sner (Number): instance of sequence number
         fner (Number): instance of first seen ordinal number
         dater (Dater): instance of first seen datetime
         serder (SerderKERI): instance of current event with .serder.diger for digest
         ilk (str): from Ilks for current event type
@@ -1598,15 +1473,15 @@
         estOnly (bool): config trait True means only allow establishment events
             Default False. Corresponds to config trait string "EO"
         doNotDelegate (bool): config trait True means do not allow delegation
             Default False. Corresponds to config trait string "DND"
 
         lastEst (LastEstLoc): namedtuple of int sn .s and qb64 digest .d of last est event
         delegated (bool): True means delegated identifier, False not delegated
-        delgator (str): qb64 of delegator's prefix
+        delpre(str): qb64 of delegator's prefix
 
 
     Properties:
         sn (int): sequence number property that returns .sner.num
         fn (int): first seen ordinal number property the returns .fner.num
         ndigs (list): of digests qb64 of .digers
         kevers (dict): reference to self.db.kevers
@@ -1622,15 +1497,15 @@
 
     """
     EstOnly = False
     DoNotDelegate = False
 
     def __init__(self, *, state=None, serder=None, sigers=None, wigers=None,
                  db=None, estOnly=None, delseqner=None, delsaider=None, firner=None,
-                 dater=None, cues=None, prefixes=None, local=False, check=False):
+                 dater=None, cues=None, local=True, check=False):
         """
         Create incepting kever and state from inception serder
         Verify incepting serder against sigers raises ValidationError if not
 
         Parameters:
             state (KeyStateRecord | None): instance for key state notice
             serder (SerderKERI | None): instance of inception event
@@ -1650,38 +1525,32 @@
                 When firner provided then compare fn of dater and database and
                 first seen if not match then log and add cue notify problem
             dater (Dater | None): optional instance of cloned replay datetime
                 If cloned mode then dater maybe provided (not None)
                 When dater provided then use dater for first seen datetime
             cues (Deck | None): reference to Kevery.cues Deck when provided
                 i.e. notices of events or requests to respond to
-            prefixes (list | None): own prefixes for own local habitats.
-                May not include the prefix of this Kever's event when inception
-                has not yet been accepted into KEL
-                Some restrictions if present
-                If empty then effectively in promiscuous mode
-            local (bool): True means only process msgs for own controller's
-                              events if .prefixes is not empty.
-                          False means only process msgs for not own events
-                              if .prefixes is not empty
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
             check (bool): True means do not update the database in any
                 non-idempotent way. Useful for reinitializing the Kevers from
                 a persisted KEL without updating non-idempotent first seen .fels
                 and timestamps.
         """
         if not (state or (serder and sigers)):
             raise ValueError("Missing required arguments. Need state or serder"
                              " and sigers")
 
         if db is None:
             db = basing.Baser(reopen=True)  # default name = "main"
         self.db = db
         self.cues = cues
-        self.prefixes = prefixes if prefixes is not None else db.prefixes
-        self.local = True if local else False
+        local = True if local else False
 
         if state:  # preload from state
             self.reload(state)
             return
 
         # may update state as we go because if invalid we fail to finish init
         self.version = serder.version  # version dispatch ?
@@ -1689,47 +1558,42 @@
         ilk = serder.ilk # serder.ked["t"]
         if ilk not in (Ilks.icp, Ilks.dip):
             raise ValidationError("Expected ilk = {} or {} got {} for evt = {}."
                                   "".format(Ilks.icp, Ilks.dip,
                                             ilk, serder.ked))
         self.ilk = ilk
 
-        labels = DIP_LABELS if ilk == Ilks.dip else ICP_LABELS
-        for k in labels:
-            if k not in serder.ked:
-                raise ValidationError("Missing element = {} from {} event for "
-                                      "evt = {}.".format(k, ilk, serder.ked))
-
         self.incept(serder=serder)  # do major event validation and state setting
 
         self.config(serder=serder, estOnly=estOnly)  # assign config traits perms
 
         # Validates signers, delegation if any, and witnessing when applicable
         # If does not validate then escrows as needed and raises ValidationError
-        sigers, delegator, wigers = self.valSigsDelWigs(serder=serder,
+        sigers, wigers, delpre = self.valSigsWigsDel(serder=serder,
                                                         sigers=sigers,
                                                         verfers=serder.verfers,
                                                         tholder=self.tholder,
                                                         wigers=wigers,
                                                         toader=self.toader,
                                                         wits=self.wits,
+                                                        local=local,
                                                         delseqner=delseqner,
                                                         delsaider=delsaider)
 
-        self.delegator = delegator
-        self.delegated = True if self.delegator else False
+        self.delpre = delpre  # may be None
+        self.delegated = True if self.delpre else False
 
         wits = serder.backs  # serder.ked["b"]
         # .validateSigsDelWigs above ensures thresholds met otherwise raises exception
         # all validated above so may add to KEL and FEL logs as first seen
         # returns fn == None if already logged fn log is non idempotent
         fn, dts = self.logEvent(serder=serder, sigers=sigers, wigers=wigers, wits=wits,
                                 first=True if not check else False,
                                 seqner=delseqner, saider=delsaider,
-                                firner=firner, dater=dater)
+                                firner=firner, dater=dater, local=local)
         if fn is not None:  # first is non-idempotent for fn check mode fn is None
             self.fner = Number(num=fn)
             self.dater = Dater(dts=dts)
             self.db.states.pin(keys=self.prefixer.qb64,
                                val=self.state())
 
 
@@ -1765,50 +1629,124 @@
         """
         Returns .baser.kevers
         """
         return self.db.kevers
 
 
     @property
+    def prefixes(self):
+        """
+        Returns .db.prefixes
+        """
+        return self.db.prefixes
+
+
+    @property
+    def groups(self):
+        """
+        Returns .db.gids oset of group hab ids (prefixes)
+        """
+        return self.db.groups
+
+
+    @property
     def transferable(self):
         """
         Property transferable:
         Returns True if identifier does not have non-transferable derivation code
                 and .nextor is not None
                 False otherwise
         """
         return True if self.ndigers and self.prefixer.transferable else False
 
 
-    def locallyOwned(self, pre=''):
-        """Returns True if pre is in .prefixes False otherwise. Indicates that
-        provided identifier prefix is controlled by a local controller from
-        .prefixes
+    def locallyOwned(self, pre: str | None = None):
+        """Returns True if pre is in .prefixes and not in .groups
+        False otherwise.
+        Indicates that provided identifier prefix is controlled by a local
+        controller from .prefixes but is not a group with local member.
         i.e pre is a locally owned (controlled) AID (identifier prefix)
 
+        Returns:
+            (bool): True if pre is local hab but not group hab
+
         Parameters:
-           pre (str): qb64 identifier prefix
+            pre (str|None): qb64 identifier prefix if any. Default None
+                    None means use self.prefixer.qb64
 
         """
-        return pre in self.prefixes
+        pre = pre if pre is not None else self.prefixer.qb64
+        return pre in self.prefixes and pre not in self.groups
 
 
-    def locallyWitnessed(self, serder=None):
+    def locallyWitnessed(self, *, wits: list[str]=None, serder: (str)=None):
         """Returns True if a local controller is a witness of this Kever's KEL
            of wits in serder of if None then current wits for this Kever.
            i.e.  self is witnessd by locally owned (controlled) AID (identifier prefix)
 
         Parameters:
+           wits (list[str]): qb64 identifier prefixes of witnesses
            serder ( SerderKERI | None): SerderKERI instace if any
 
         """
-        if serder and serder.pre != self.prefixer.qb64:  # same KEL as self
-            return False
-        wits = serder.backs if serder is not None else self.wits
-        return (oset(self.prefixes) & oset(wits))
+        if not wits:
+            if not serder:
+                wits = self.wits
+            else:
+                if serder.pre != self.prefixer.qb64:  # not same KEL as self
+                    return False
+                wits, _, _ = self.deriveBacks(serder=serder)
+
+        return True if (self.prefixes & oset(wits)) else False
+
+
+    def locallyMembered(self, pre: str | None = None):
+        """Returns True if group hab identifier prefix pre has as a contributing
+        member a locally owned prefix by virture of pre in .groups
+
+        Returns:
+            (bool): True if pre is group hab identifier in .groups
+                    False otherwise
+
+        Parameters:
+            pre (str|None): qb64 identifier prefix if any or None
+                           When None default to use self.prefixer.qb64
+
+        """
+        # assumes stale group membership is taken care of by presence of groups
+        # i.e where once a local member but no more.
+        pre = pre if pre is not None else self.prefixer.qb64
+        return pre in self.groups  # groups
+
+
+    def locallyContributedIndices(self, verfers: list[Verfer]):
+        """Returns list of indices of public keys contributed by local members
+        to the KEL with current signing keys represented by verfers
+
+        Using the pubs index to find members of a signing group
+
+        Parameters:
+            verfers (list[Verfer]): instance for each current signing key
+
+        Returns:
+            indices list[int]: list of indices of keys contributed by local members
+
+        """
+        indices = []
+
+        for i, verfer in enumerate(verfers):
+            if (couples := self.pubs.get(keys=(verfer.qb64,))) is None:
+                continue
+
+            for (prefixer, seqner) in couples:
+                if self.locallyOwned(prefixer.qb64):  # only member not group aid
+                    indices.append(i)
+                    break  # only need one local member to exclude signature
+
+        return indices
 
 
     def reload(self, state):
         """
         Reload Kever attributes (aka its state) from state (KeyStateRecord)
 
         Parameters:
@@ -1826,20 +1764,20 @@
         self.verfers = [Verfer(qb64=key) for key in state.k]
         self.ndigers = [Diger(qb64=dig) for dig in state.n]
         self.toader = Number(numh=state.bt)  # auto converts from hex num
         self.wits = state.b
         self.cuts = state.ee.br
         self.adds = state.ee.ba
         self.estOnly = False
-        self.doNotDelegate = True if TraitCodex.DoNotDelegate in state.c else False
-        self.estOnly = True if TraitCodex.EstOnly in state.c else False
+        self.doNotDelegate = True if TraitDex.DoNotDelegate in state.c else False
+        self.estOnly = True if TraitDex.EstOnly in state.c else False
         self.lastEst = LastEstLoc(s=int(state.ee.s, 16),
                                   d=state.ee.d)
-        self.delegator = state.di if state.di else None
-        self.delegated = True if self.delegator else False
+        self.delpre = state.di if state.di else None
+        self.delegated = True if self.delpre else False
 
         if (raw := self.db.getEvt(key=dgKey(pre=self.prefixer.qb64,
                                             dig=state.d))) is None:
             raise MissingEntryError(f"Corresponding event not found for state="
                                     f"{state}.")
         self.serder = serdering.SerderKERI(raw=bytes(raw))
         # May want to do additional checks here
@@ -1936,15 +1874,15 @@
         if TraitDex.EstOnly in cnfg:
             self.estOnly = True
         if TraitDex.DoNotDelegate in cnfg:
             self.doNotDelegate = True
 
 
     def update(self, serder, sigers, wigers=None, delseqner=None, delsaider=None,
-               firner=None, dater=None, check=False):
+               firner=None, dater=None, local=True, check=False):
         """
         Not an inception event. Verify event serder and indexed signatures
         in sigers and update state
 
         Parameters:
             serder (SerderKERI): instance of  event
             sigers (list): of SigMat instances of indexed signatures of controller
@@ -1960,14 +1898,18 @@
             firner (Seqner | None): Seqner instance of cloned first seen ordinal
                 If cloned mode then firner maybe provided (not None)
                 When firner provided then compare fn of dater and database and
                 first seen if not match then log and add cue notify problem
             dater (Dater | None): Dater instance of cloned replay datetime
                 If cloned mode then dater maybe provided (not None)
                 When dater provided then use dater for first seen datetime
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
             check (bool): True means do not update the database in any
                 non-idempotent way. Useful for reinitializing the Kevers from
                 a persisted KEL without updating non-idempotent first seen .fels
                 and timestamps.
 
         """
         ked = serder.ked
@@ -1977,14 +1919,15 @@
 
         if serder.pre != self.prefixer.qb64:
             raise ValidationError("Mismatch event aid prefix = {} expecting"
                                   " = {} for evt = {}.".format(serder.pre,
                                                                self.prefixer.qb64,
                                                                ked))
 
+        local = True if local else False
 
         sner = serder.sner  # Number instance ensures whole number for sequence number
         ilk = serder.ilk # ked["t"]
 
         if ilk in (Ilks.rot, Ilks.drt):  # rotation (or delegated rotation) event
             if self.delegated and ilk != Ilks.drt:
                 raise ValidationError("Attempted non delegated rotation on "
@@ -1992,43 +1935,32 @@
                                       "".format(serder.pre, ked))
 
             tholder, toader, wits, cuts, adds = self.rotate(serder)
 
             # Validates signers, delegation if any, and witnessing when applicable
             # returned sigers and wigers are verified signatures
             # If does not validate then escrows as needed and raises ValidationError
-            sigers, delegator, wigers = self.valSigsDelWigs(serder=serder,
+            sigers, wigers, delpre = self.valSigsWigsDel(serder=serder,
                                                             sigers=sigers,
                                                             verfers=serder.verfers,
                                                             tholder=tholder,
                                                             wigers=wigers,
                                                             toader=toader,
                                                             wits=wits,
+                                                            local=local,
                                                             delseqner=delseqner,
                                                             delsaider=delsaider)
 
 
-            # rotation so check rotation threshold against exposed sigers versus
-            # prior next digers in .ndigers
-            #ondices = self.exposeds(sigers)
-            #if not self.ntholder.satisfy(indices=ondices):
-                #self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers)
-                #if delseqner and delsaider:  # save in case not attached later
-                    #self.escrowPACouple(serder=serder, seqner=delseqner, saider=delsaider)
-                #raise MissingSignatureError(f"Failure satisfying nsith="
-                                            #f"{self.ntholder.sith} on sigs="
-                                            #f"{[siger.qb64 for siger in sigers]}"
-                                            #f" for evt={serder.ked}.")
 
-
-            # .validateSigsDelWigs above ensures thresholds met otherwise raises exception
+            # .valSigWigsDel above ensures thresholds met otherwise raises exception
             # all validated above so may add to KEL and FEL logs as first seen
             fn, dts = self.logEvent(serder=serder, sigers=sigers, wigers=wigers, wits=wits,
                                     first=True if not check else False, seqner=delseqner, saider=delsaider,
-                                    firner=firner, dater=dater)
+                                    firner=firner, dater=dater, local=local)
 
             # nxt and signatures verify so update state
             self.sner = sner  # sequence number Number instance
             self.serder = serder  # need whole serder for digest agility compare
             self.ilk = ilk
             self.tholder = tholder
             self.verfers = serder.verfers
@@ -2049,18 +1981,18 @@
 
 
         elif ilk == Ilks.ixn:  # subsequent interaction event
             if self.estOnly:
                 raise ValidationError("Unexpected non-establishment event = {}."
                                       "".format(serder.ked))
 
-            for k in IXN_LABELS:
-                if k not in ked:
-                    raise ValidationError("Missing element = {} from {} event."
-                                          " evt = {}.".format(k, Ilks.ixn, ked))
+            #for k in IXN_LABELS:
+                #if k not in ked:
+                    #raise ValidationError("Missing element = {} from {} event."
+                                          #" evt = {}.".format(k, Ilks.ixn, ked))
 
             if not sner.num == (self.sner.num + 1):  # sn not in order
                 raise ValidationError("Invalid sn = {} expecting = {} for evt "
                                       "= {}.".format(sner.num, self.sner.num + 1, ked))
 
             if not self.serder.compare(said=ked["p"]):  # prior event dig not match
                 raise ValidationError("Mismatch event dig = {} with state dig"
@@ -2068,21 +2000,22 @@
                                                                    self.serder.said,
                                                                    ked))
 
             # interaction event use keys, sith, toad, and wits from pre-existing Kever state
 
             # Validates signers, delegation if any, and witnessing when applicable
             # If does not validate then escrows as needed and raises ValidationError
-            sigers, delegator, wigers = self.valSigsDelWigs(serder=serder,
+            sigers, wigers, delpre = self.valSigsWigsDel(serder=serder,
                                                             sigers=sigers,
                                                             verfers=self.verfers,
                                                             tholder=self.tholder,
                                                             wigers=wigers,
                                                             toader=self.toader,
-                                                            wits=self.wits)
+                                                            wits=self.wits,
+                                                            local=local)
 
             # .validateSigsDelWigs above ensures thresholds met otherwise raises exception
             # all validated above so may add to KEL and FEL logs as first seen
             fn, dts = self.logEvent(serder=serder, sigers=sigers, wigers=wigers,
                                     first=True if not check else False)  # First seen accepted
 
             # validates so update state
@@ -2184,69 +2117,88 @@
 
 
 
         # compute wits from existing .wits with new cuts and adds from event
         # use ordered set math ops to verify and ensure strict ordering of wits
         # cuts and add to ensure that indexed signatures on indexed witness
         # receipts work
+        wits, cuts, adds = self.deriveBacks(serder)
+
+        toader = serder.bner # Number(num=ked["bt"])  # auto converts hex num to int
+        if wits:
+            if toader.num < 1 or toader.num > len(wits):  # out of bounds toad
+                raise ValueError(f"Invalid toad = {toader.num} for backers "
+                                 f"(wits)={wits} for event={ked}.")
+        else:
+            if toader.num != 0:  # invalid toad
+                raise ValueError(f"Invalid toad = {toader.num} for backers "
+                                 "(wits)={wits} for event={ked}.")
+
+        return tholder, toader, wits, cuts, adds
+
+
+    def deriveBacks(self, serder):
+        """Derives and return tuple of (wits, cuts, adds) for backers  given
+        current set and any changes provided by serder.
+
+        Returns:
+            wca (tuple): of
+               wits (list[str]): prefixes of witnesses full list (backers)
+               cuts (list[str]): prefixes of witnesses removed in latest est evt
+               adds (list[str]): prefixes of witnesses added in latest est evt
+
+        Parameters:
+            serder (SerderKeri): instance of current event
+        """
+        if serder.ilk not in (Ilks.rot, Ilks.drt):  # no changes
+            return (self.wits, self.cuts, self.adds)
+
         witset = oset(self.wits)
-        cuts = serder.cuts # ked["br"]
+        cuts = serder.cuts
         cutset = oset(cuts)
         if len(cutset) != len(cuts):
-            raise ValidationError("Invalid cuts = {}, has duplicates for evt = "
-                                  "{}.".format(cuts, ked))
+            raise ValidationError("Invalid cuts = {cuts}, has duplicates for "
+                                  f"evt = {serder.ked}.")
 
         if (witset & cutset) != cutset:  # some cuts not in wits
-            raise ValidationError("Invalid cuts = {}, not all members in wits"
-                                  " for evt = {}.".format(cuts, ked))
+            raise ValidationError(f"Invalid cuts = {cuts}, not all members in "
+                                  f"wits for evt = {serder.ked}.")
 
-        adds = serder.adds # ked["ba"]
+        adds = serder.adds
         addset = oset(adds)
         if len(addset) != len(adds):
-            raise ValidationError("Invalid adds = {}, has duplicates for evt = "
-                                  "{}.".format(adds, ked))
+            raise ValidationError(f"Invalid adds = {adds}, has duplicates for "
+                                  f"evt = {serder.ked}.")
 
         if cutset & addset:  # non empty intersection
-            raise ValidationError("Intersecting cuts = {} and  adds = {} for "
-                                  "evt = {}.".format(cuts, adds, ked))
+            raise ValidationError(f"Intersecting cuts = {cuts} and adds = {adds}"
+                                  f"for evt = {serder.ked}.")
 
         if witset & addset:  # non empty intersection
-            raise ValidationError("Intersecting wits = {} and  adds = {} for "
-                                  "evt = {}.".format(self.wits, adds, ked))
+            raise ValidationError(f"Intersecting wits = {self.wits} and  adds ="
+                                  f"{adds} for evt = {serder.ked}.")
 
         wits = list((witset - cutset) | addset)
 
         if len(wits) != (len(self.wits) - len(cuts) + len(adds)):  # redundant?
-            raise ValidationError("Invalid member combination among wits = {}, cuts ={}, "
-                                  "and adds = {} for evt = {}.".format(self.wits,
-                                                                       cuts,
-                                                                       adds,
-                                                                       ked))
-
-        toader = serder.bner # Number(num=ked["bt"])  # auto converts hex num to int
-        if wits:
-            if toader.num < 1 or toader.num > len(wits):  # out of bounds toad
-                raise ValueError(f"Invalid toad = {toader.num} for backers "
-                                 f"(wits)={wits} for event={ked}.")
-        else:
-            if toader.num != 0:  # invalid toad
-                raise ValueError(f"Invalid toad = {toader.num} for backers "
-                                 "(wits)={wits} for event={ked}.")
+            raise ValidationError(f"Invalid member combination among wits = "
+                                  f"{self.wits}, cuts ={cuts}, and adds = "
+                                  f"{adds,} for evt = {serder.ked}.")
+        return (wits, cuts, adds)
 
-        return tholder, toader, wits, cuts, adds
 
 
-    def valSigsDelWigs(self, serder, sigers, verfers, tholder,
-                       wigers, toader, wits,
+    def valSigsWigsDel(self, serder, sigers, verfers, tholder,
+                       wigers, toader, wits, local=True,
                        delseqner=None, delsaider=None):
         """
-        Returns triple (sigers, delegator, wigers) where:
+        Returns triple (sigers, wigers, delegator) where:
         sigers is unique validated signature verified members of inputed sigers
-        delegator is qb64 delegator prefix if delegated else None
         wigers is unique validated signature verified members of inputed wigers
+        delegator is qb64 delegator prefix if delegated else None
 
         Validates sigers signatures by validating indexes, verifying signatures, and
             validating threshold sith.
         Validate witness receipts by validating indexes, verifying
             witness signatures and validating toad.
         Witness validation is a function of wits .prefixes and .local
 
@@ -2258,93 +2210,141 @@
             tholder (Tholder): instance of sith threshold
             wigers (list): of Siger instances of indexed witness signatures.
                 Index is offset into wits list of associated witness nontrans pre
                 from which public key may be derived.
             toader (Number): instance of backer witness threshold
             wits (list): of qb64 non-transferable prefixes of witnesses used to
                 derive werfers for wigers
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
             delseqner (Seqner | None): instance of delegating event sequence number.
                 If this event is not delegated then seqner is ignored
             delsaider (Saider | None): instance of of delegating event said.
                 If this event is not delegated then saider is ignored
 
         """
         if len(verfers) < tholder.size:
             raise ValidationError("Invalid sith = {} for keys = {} for evt = {}."
                                   "".format(tholder.sith,
                                             [verfer.qb64 for verfer in verfers],
                                             serder.ked))
 
+        # Filters sigers to remove any signatures from locally membered groups
+        # when not local (remote) event source. So that attacker can't source
+        # compromised signature remotely to satisfy threshold.
+
+        if not local and self.locallyMembered():  # is this Kever's pre a local group
+            if (indices := self.locallyContributedIndices(verfers)):
+                for siger in list(sigers):  # copy so clean del on original elements
+                    if siger.index in indices:
+                        del sigers[siger.index]
+                        self.cues.push(dict(kin="remoteMemberedSig",
+                                            serder=serder,
+                                              index=siger.index))
+
         # get unique verified sigers and indices lists from sigers list
         sigers, indices = verifySigs(raw=serder.raw, sigers=sigers, verfers=verfers)
         # sigers  now have .verfer assigned
 
         # check if minimally signed in order to continue processing
         if not indices:  # must have a least one verified sig
             raise ValidationError("No verified signatures for evt = {}."
                                   "".format(serder.ked))
 
-        werfers = [Verfer(qb64=wit) for wit in wits]  # get witnes signatures
+        # Misfit check events that must be locally sourced (protected) get
+        # escrowed in order to repair the protection when appropriate
+        if (not local and
+                (self.locallyOwned() or
+                 self.locallyWitnessed(wits=wits))):
+
+            self.escrowMFEvent(serder=serder, sigers=sigers, wigers=wigers,
+                                   seqner=delseqner, saider=delsaider, local=local)
+            raise MisfitEventSourceError(f"Nonlocal source for locally owned"
+                                             f"or locally witnessed event"
+                                                 f" = {serder.ked}.")
 
+
+        werfers = [Verfer(qb64=wit) for wit in wits]  # get witness public key verifiers
         # get unique verified wigers and windices lists from wigers list
         wigers, windices = verifySigs(raw=serder.raw, sigers=wigers, verfers=werfers)
         # each wiger now has added to it a werfer of its wit in its .verfer property
 
-        # escrow if not fully signed vs threshold
+        # escrow if not fully signed vs signing threshold
         if not tholder.satisfy(indices):  # at least one but not enough
-            self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers)
+            self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
             if delseqner and delsaider:
                 self.escrowPACouple(serder=serder, seqner=delseqner, saider=delsaider)
             raise MissingSignatureError(f"Failure satisfying sith = {tholder.sith}"
                                         f" on sigs for {[siger.qb64 for siger in sigers]}"
                                         f" for evt = {serder.ked}.")
 
+        # escrow if not fully signed vs prior next rotation threshold
         if serder.ilk in (Ilks.rot, Ilks.drt):  # rotation so check prior next threshold
             # prior next threshold in .ntholder and digers in .ndigers
             ondices = self.exposeds(sigers)
             if not self.ntholder.satisfy(indices=ondices):
-                self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers)
+                self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
                 if delseqner and delsaider:  # save in case not attached later
                     self.escrowPACouple(serder=serder, seqner=delseqner, saider=delsaider)
                 raise MissingSignatureError(f"Failure satisfying prior nsith="
                                             f"{self.ntholder.sith} with exposed "
                                             f"sigs= {[siger.qb64 for siger in sigers]}"
                                             f" for new est evt={serder.ked}.")
 
 
-        delegator = self.validateDelegation(serder, sigers=sigers, wigers=wigers,
-                                            delseqner=delseqner, delsaider=delsaider)
-
-        # Kevery .process event logic does not prevent this from seeing event when
-        # not local and event pre is own pre
-        if not self.locallyOwned(serder.pre):  # not in self.prefixes
-            if ((wits and not self.prefixes) or  # in promiscuous mode so assume must verify toad
-                    (wits and self.prefixes and not self.local and  # not promiscuous nonlocal
-                     not (oset(self.prefixes) & oset(wits)))):  # own prefix is not a witness
-                # validate that event is fully witnessed
-
-                if wits:
-                    if toader.num < 1 or toader.num > len(wits):  # out of bounds toad
-                        raise ValidationError(f"Invalid toad = {toader.num} for wits = {wits}")
-                else:
-                    if toader.num != 0:  # invalid toad
-                        raise ValidationError(f"Invalid toad = {toader.num} for wits = {wits}")
-
-                if len(windices) < toader.num:  # not fully witnessed yet
-                    if self.escrowPWEvent(serder=serder, wigers=wigers, sigers=sigers,
-                                          seqner=delseqner, saider=delsaider):
-                        # cue to query for witness receipts
-                        self.cues.push(dict(kin="query", q=dict(pre=serder.pre, sn=serder.snh)))
-                    raise MissingWitnessSignatureError(f"Failure satisfying toad={toader.num} "
-                                                       f"on witness sigs="
-                                                       f"{[siger.qb64 for siger in wigers]} "
-                                                       f"for event={serder.ked}.")
-
+        # get delegator if any
+        if serder.ilk == Ilks.dip:
+            delpre = serder.delpre  # delegator from dip event
+            if not delpre:  # empty or None
+                raise ValidationError(f"Empty or missing delegator for delegated"
+                                          f" inception event = {serder.ked}.")
+        elif serder.ilk == Ilks.drt:  # serder.ilk == Ilks.drt so rotation
+            delpre = self.delpre
+        else:  # not delegable event icp, rot, ixn
+            delpre = None
+
+        # delpre maybe None so ensure not None to pass into .locallyOwned which
+        # defaults to self.prefixer.qb64 when None
+        if not local and self.locallyOwned(delpre if delpre is not None else ''):
+            self.escrowMFEvent(serder=serder, sigers=sigers, wigers=wigers,
+                               seqner=delseqner, saider=delsaider, local=local)
+            raise MisfitEventSourceError(f"Nonlocal source  for locally"
+                                                 f" delegated by {delpre} of"
+                                                 f"event = {serder.ked}.")
+
+        # short circuit witness validation when either locallyOwned or locallyWitnessed
+        # otherwise must validate fully witnessed
+        if not (self.locallyOwned() or self.locallyWitnessed(wits=wits)):
+            if wits:  # is witnessed
+                if toader.num < 1 or toader.num > len(wits):  # out of bounds toad
+                    raise ValidationError(f"Invalid toad = {toader.num} for wits = {wits}")
+            else:  # not witnessed
+                if toader.num != 0:  # invalid toad
+                    raise ValidationError(f"Invalid toad = {toader.num} for wits = {wits}")
+
+            if len(windices) < toader.num:  # not fully witnessed yet
+                if self.escrowPWEvent(serder=serder, wigers=wigers, sigers=sigers,
+                                      seqner=delseqner, saider=delsaider,
+                                      local=local):
+                    # cue to query for witness receipts
+                    self.cues.push(dict(kin="query", q=dict(pre=serder.pre, sn=serder.snh)))
+                raise MissingWitnessSignatureError(f"Failure satisfying toad={toader.num} "
+                                                   f"on witness sigs="
+                                                   f"{[siger.qb64 for siger in wigers]} "
+                                                   f"for event={serder.ked}.")
+
+        if delpre:
+            self.validateDelegation(serder, sigers=sigers,
+                                    wigers=wigers, wits=wits,
+                                    local=local, delpre=delpre,
+                                    delseqner=delseqner, delsaider=delsaider)
 
-        return sigers, delegator, wigers
+        return sigers, wigers, delpre
 
 
     def exposeds(self, sigers):
         """Returns list of ondices (indices) suitable for Tholder.satisfy
         from self.ndigers (prior next key digests ) as exposed by event sigers.
         Uses dual index feature of siger. Assumes that each siger.verfer is
         from the correct key given by siger.index and the signature has been verified.
@@ -2386,43 +2386,153 @@
             kdig = Diger(ser=siger.verfer.qb64b, code=diger.code).qb64
             if kdig == diger.qb64:
                 odxs.append(siger.ondex)
 
         return odxs
 
 
-    def validateDelegation(self, serder, sigers, wigers=None, delseqner=None, delsaider=None):
+    def validateDelegation(self, serder, sigers, wigers, wits, local=True,
+                           delpre=None, delseqner=None, delsaider=None):
         """
         Returns delegator's qb64 identifier prefix if validation successful.
+        Assumes that local vs remote source checks have been applied before
+        this function is called.
+
         Rules:
             If event is not a delegated event then not valid delegation
             If delegatee's own event (.mine) then valid delegation
             If delegation seal found in delgator's KEL then valid delegation given
                 valid superseding rules below
             Otherwise escrow or reject if error condition
 
         seal validates with respect to Delegator's KEL
         Location Seal is from Delegate's establishment event
         Assumes state setup
 
         Parameters:
             serder (SerderKERI): instance of delegated event serder
-            sigers (list): of Siger instances of indexed controller sigs of
+            sigers (list[Siger]): of Siger instances of indexed controller sigs of
                 delegated event. Assumes sigers is list of unique verified sigs
-            wigers (list | None): of optional Siger instance of indexed witness sigs of
+            wigers (list[Siger]): of optional Siger instance of indexed witness sigs of
                 delegated event. Assumes wigers is list of unique verified sigs
+            wits (list[str]): of qb64 non-transferable prefixes of witnesses used to
+                derive werfers for wigers
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
+            delpre (str | None): qb64 prefix of delegator if any
             delseqner (Seqner | None): instance of delegating event sequence number.
                 If this event is not delegated then ignored
             delsaider (Saider | None): instance of of delegating event digest.
                 If this event is not delegated ignored
 
         Returns:
             (str | None): qb64 delegator prefix or None if not delegated
 
-        Superseding Recovery
+        Process Logic:
+            A delegative event is processed differently for each of four different
+            parties, namely, controller of event, witness to controller of event,
+            delegator of event , and validator of event that is not controller,
+            witness or delegator. Events are processed as either local (protected)
+            or remote. A local event may assume that the event only came via a
+            protected transmission path. This might be because the event is
+            functions locally on a device under the supervision of the controller
+            or was received via some protected channel using some form of MFA.
+            A remote event is received in an unprotected manner. The purpose of
+            local and remote is to allow increased security on local events where
+            a threshold structure is imposed.
+
+            A witness pool may act a threshold structure for enchanced security
+            when each witness only accepts local events that are protected
+            by a unique authentication factor thereby making the controller's
+            signature(s) the first factor and the set of unique witness factors
+            a secondary threshold factor. An attacker therefore has to compromise
+            not merely the controller's private key(s) but also the unique second factor
+            on each of a threshold satisfycing number of witnesses.
+
+            Likewise a delegator may act as a threshold structure for enhanced security
+            when the delegator only accepts local events for delegation that are
+            protected by a unique authentication factor thereby making the
+            controller's signatures the first factor, a threshold satisfycing
+            number of unique witness factors the second layer of factors, and
+            the delegator's unique authentication factor as the third factor.
+            An attacker therefore has to compromise not merely the controller's
+            private key(s) but also the unique second factor
+            on each of a threshold satisfycing number of witnesses and the unique
+            third factor for the delegator.
+
+            Controller as delegatee must accept its own delegated event prior
+            to full witnessing or delegator approval (anchored seal) by signing the
+            event in order to trigger the logic to get witness receipts and
+            delegator approval. This means a local (protected) event may be
+            accepted into controller's KEL when fully signed by controller.
+
+            Witness must accept a controller's delegated event it witnesses prior to
+            full witnessing or delegator approval in order to trigger its
+            witnessing logic. This means a local (protected) event may be
+            accepted into  a witness' KEL when fully signed by its controller.
+
+            Delegator may escrow or sandbox a delegated event prior to it anchoring
+            a seal of the event in its KEL in order to trigger its approval logic.
+            Alternatively the approval logic may be triggered immediately after
+            it is received and authenticated on it its local (protected) channel
+            but before it is submitted to its local Kevery for processing.
+
+            The delegator MUST NOT accept a delegable event unless it is locally
+            sourced, fully signed by its controller, and fully witnessed by its
+            controller's designated witness pool.
+            A Delegator may impose additional validation logic prior to approval.
+            The approval logic may be handled by an escrow that only runs if
+            the delegable event is sourced as local. This may require a
+            sandboxed kel for the delegatee in order to not corrupt its pristine
+            copy of the delegatee's KEL with a valid delegable event from a
+            malicious source. The sandboxing logic may create a virtual
+            delegation event with seal for the purpose of checking the delegated
+            event superseding logic prior to acceptance.
+
+            A malicious attacker that compromises the pre-rotated keys of the
+            delegatee may issue a rotation that changes its witness pool in order
+            to bypass the local security logic of the witness pool. The approval
+            logic of the delegator may choose to not automatically approve a
+            delegable rotation event unliess the change to the witness pool is
+            below the threshold.
+
+            The logic for superseded events is NOT a requirement for acceptance in
+            either a delegated event controller's KEL or its witness' KEL. The
+            delegator's kel creates a virtual (provisional) delegating interaction
+            event in order to evaluate correct superseding logic so as not to
+            accept an invalid supderseding delegated event into its local copy
+            of the delegated KEL. This virtual event is needed because superseding
+            logic requires an anchoring seal be present before the rules can
+            be fully evaluated.
+
+            Should the actual anchor be via a superseding rotation in the
+            delegator's KEL not via an interaction event then the delegator must
+            check the logic for a virtual delegating rotation instead.
+            In either case the delegated event does not change so the virtual
+            delegating checks are sufficient to accept the delegated event
+            into the delegator's local copy of the delegatee's KEL.
+
+
+            Any of delegated controller, delegated witness, or delegator
+            of delegated event may after the fact fully validate event by
+            processing it as a remote event.
+            Then the logic applied is same as validator below.
+
+            A validator of a delegated event that is not the event's controller,
+            witness, or delegator must not accept the event until is is fully
+            signed by the controller (threshold), fully witnessed by the witness
+            pool (threshold) and its seal anchored in the delegator's KEL. The
+            rules for event superseding in the delegated controller's kel must
+            also be satisfied. The logic should be the same for both local and
+            remote event because the validator is not one of the protected parties
+            to the event.
+
+        Superseding Recovery:
 
         Supersede means that after an event has already been accepted as first seen
         into a KEL that a different event with the same sequence number is accepted
         that supersedes the pre-existing event at that sn. This enables the recovery of
         events signed by compromised keys. The result of superseded recovery is that
         the KEL is forked at the sn of the superseding event. All events in the
         superseded branch of the fork still exist but, by virtue of being superseded,
@@ -2434,193 +2544,262 @@
         The fn is not the same as the sn (sequence number).
         Each event accepted into a KEL has a unique fn but multiple events due to
         recovery forks may share the same sn.
 
 
         Superseding Rules for Recovery at given SN (sequence number)
 
-        A0. Any rotation event may supersede an interaction event at the same sn. (existing rule)
-        A1. A non-delegated rotation may not supersede another rotation at the same sn.  (modified rule)
+        A0. Any rotation event may supersede an interaction event at the same sn.
+            where that interaction event is not before any other rotation event.
+            (existing rule)
+        A1. A non-delegated rotation may not supersede another rotation at the
+            same sn.  (modified rule)
         A2. An interaction event may not supersede any event. ( existing rule).
 
         (B. and C. below provide the new rules)
 
-        B.  A delegated rotation may supersede another delegated rotation at the same sn
-        under either of the following conditions:
+        B.  A delegated rotation may supersede the latest seen delegated rotation
+            at the same sn under either of the following conditions:
+
             B1.  The superseding rotation's delegating event is later than
             the superseded rotation's delegating event in the delegator's KEL, i.e. the
             sn of the superseding event's delegation is higher than the superseded event's
             delegation.
+
             B2. The sn of the superseding rotation's delegating event is the same as
             the sn of the superseded rotation's delegating event in the delegator's KEL
             and the superseding rotation's delegating event is a rotation and the
             superseded rotation's delegating event is an interaction,
             i.e. the superseding rotation's delegating event is itself a superseding
             rotation of the superseded rotations delegating interaction event in the
             delgator's KEL
 
         C. IF Neither A nor B is satisfied, then recursively apply rules A. and B. to
-        the delegating events of those delegating events and so on until either  A. or B.
-        is satisfied, or the root KEL of the delegation has been reached.
-          C1. If neither A. nor B. is satisfied by recursive application on the
-          delegator's KEL (i.e. the root KEL of the delegation has been reached without
-          satisfaction) then the superseding rotation is discarded. The terminal case of
-          the recursive application will occur at the root KEL which by defintion is
-          non-delegated wherefore either A. or B. must be satisfied, or else the
-          superseding rotation must be discarded.
+            the delegating events of those delegating events and so on until
+            either  A. or B. is satisfied, or the root KEL of the delegation
+            which must be undelegated has been reached.
+
+            C1. If neither A. nor B. is satisfied by recursive application on the
+            delegator's KEL (i.e. the root KEL of the delegation has been reached
+            without satisfaction) then the superseding rotation is discarded.
+            The terminal case of the recursive application will occur at the
+            root KEL which by defintion is non-delegated wherefore either
+            A. or B. must be satisfied, or else the superseding rotation must
+            be discarded.
+
+        Note: The latest seen deleagated rotation constraint means that any earlier
+        delegated rotations can NOT be superseded. This greatly simplifies the
+        validation logic and avoids a potential infinite regress of forks in the
+        delegated identifier's KEL.
+
+        In order to capture control of a delegated identifier the attacker must
+        issue a delegated rotation that rotates to keys under the control of the
+        attacker that must be approved by the delegator. A recovery rotation must
+        therefore superseded the compromised rotation. If the attacker is able
+        to issue and get approved by the delegator a second rotation
+        that follows but does not supersede the compromising rotation then
+        recovery is no longer possible because the delegatee would no longer
+        control the privete keys needed to verifiably sign a recovery rotation.
 
         """
-        if serder.ilk not in (Ilks.dip, Ilks.drt):  # not delegated
-            return None  # delegator is None
-
-        # verify delegator and attachment pointing to delegating event
-        if serder.ilk == Ilks.dip:
-            delegator = serder.delpre  # delegator from dip event
-            if not delegator:
-                raise ValidationError(f"Empty or missing delegator for delegated"
-                                      f" inception event = {serder.ked}.")
-        else:  # serder.ilk == Ilks.drt so rotation
-            delegator = self.delegator
-
+        if not delpre:  # not delegable so no delegation validation needed
+            return
 
         # if we are the delegatee, accept the event without requiring the
         # delegator validation via an anchored delegation seal or by requiring
-        # it to be witnessed
-        # ToDo XXXX add local lax check after figure out dist multisig group
-        # ToDo XXXX add check for witness to accept so that witness will
-        # add to its KEL without waiting for delegation seal to be anchored in
-        # delegator's KEL  witness cue in Kevery will then generate reciept
-        if self.locallyOwned(serder.pre) or self.locallyWitnessed(serder=serder):
-            return delegator
-
-        # during initial delegation we just escrow the delcept event
-        if delseqner is None and delsaider is None and delegator is not None:
-            self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers)
-            raise MissingDelegationError("No delegation seal for delegator {} "
-                                         "with evt = {}.".format(delegator, serder.ked))
+        # it to be witnessed. Query witness cue in Kevery will then request witnessing.
+        # Controller accepts without waiting for witnessor nor for the delegation
+        # seal to be anchored in delegator's KEL.
+        # Witness accepts without waiting for delegation seal to be anchored in
+        # delegator's KEL.  Witness cue in Kevery will then generate receipt
+        if self.locallyOwned() or self.locallyWitnessed(wits=wits):
+            return
+
 
-        ssn = validateSN(sn=delseqner.snh, inceptive=False)  # delseqner Number should already do this
-        #ssn = sner.num sner is Number seqner is Seqner need to replace Seqners with Numbers
+        if self.kevers is None or delpre not in self.kevers:   # drop event
+            # ToDo XXXX cue a trigger to get the KEL of the delegator
+            # the processDelegableEvent should also cue a trigger to get KEL
+            # of delegator if still missing when processing escrow later.
+            self.escrowDelegableEvent(serder=serder, sigers=sigers,
+                                              wigers=wigers,local=local)
+            raise MissingDelegableApprovalError(f"Missing Kever for delegator"
+                                                f" = {delpre} of event"
+                                                f" = {serder.ked}.")
+
+        dkever = self.kevers[delpre]
+        if dkever.doNotDelegate:  # drop event if delegation not allowed
+            raise ValidationError(f"Delegator = {delpre} for evt = {serder.ked},"
+                                  f" does not allow delegation.")
+
+
+        # Delegator accepts here without waiting for delegation seal to be anchored in
+        # delegator's KEL. But has already waited for fully receipted above.
+        # Once fully receipted, cue in Kevery will then trigger cue to approve
+        # delegation
+
+        if delseqner is None or delsaider is None:
+            if self.locallyOwned(delpre):  # local delegator so escrow.
+                # Won't get to here if not local and locallyOwned(delpre) because
+                # valSigsWigsDel will send nonlocal sourced delegable event to
+                # misfit escrow first. Mistfit escrow must first
+                # promote to local and reprocess event before we get to here
+                self.escrowDelegableEvent(serder=serder, sigers=sigers,
+                                          wigers=wigers,local=local)
+                raise MissingDelegableApprovalError(f"Missing approval for "
+                                                    f" delegation by {delpre} of"
+                                                         f"event = {serder.ked}.")
+
+                # ToDo XXXX This logic moves to the Delegable escrow processing
+                # ToDo XXXX create process escrow for delegable events "dees."
+                #in order to get delegator approval
+                # any virtual delegation or sandboxing logic happens there
+                # create virtual anchor seal so local delegator can evaluate
+                # superseding logic with provisional virtual seal
+                #dkever = self.kevers[delpre]
+                #dseal = SealEvent(i=serder.pre, s=serder.snh, d=serder.said)
+                #dserder = interact(pre=dkever.prefixer.qb64,
+                                           #dig=dkever.serder.said,
+                                           #sn=dkever.sner.num + 1,
+                                           #data=[dseal._asdict()])
+                #delseqner = coring.Seqner(snh=dserder.snh)
+                #delsaider = coring.Saider(qb64=dserder.said)
+                # ToDo XXXX  need to cue task here  to approve delegation by generating
+                # an anchoring SealEvent of serder in delegators KEL
+                # may include MFA and or business logic for the delegator i.e. is local
+                # event that designates this controller as delegator triggers
+                # this cue to approave delegation
+                #self.cues.push(dict(kin="approveDelegation",
+                                        #delegator=kever.delpre,
+                                        #serder=serder))
+
+
+            else:  # not local delegator so escrow
+                self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
+                raise MissingDelegationError(f"No delegation seal for delegator "
+                                         "{delpre} of evt = {serder.ked}.")
+
+        #ssn = validateSN(sn=delseqner.snh, inceptive=False)  # delseqner Number should already do this
+        ssn = Number(num=delseqner.sn).validate(inceptive=False).sn
+        #ssn = sner.num sner is Number seqner is Seqner
+        # ToDo XXXX need to replace Seqners with Numbers
 
         # get the dig of the delegating event. Using getKeLast ensures delegating
         #  event has not already been superceded
-        key = snKey(pre=delegator, sn=ssn)  # database key
+        key = snKey(pre=delpre, sn=ssn)  # database key
         raw = self.db.getKeLast(key)  # get dig of delegating event
 
         if raw is None:  # no delegating event at key pre, sn
-            # ToDo XXXX create cue to send query to fetch delegating event from
+            # ToDo XXXX process  this cue of query to fetch delegating event from
             # delegator
-            self.cues.push(dict(kin="query", q=dict(pre=delegator,
+            self.cues.push(dict(kin="query", q=dict(pre=delpre,
                                                               sn=delseqner.snh,
                                                               dig=delsaider.qb64)))
 
             #  escrow event here
             inceptive = True if serder.ilk in (Ilks.icp, Ilks.dip) else False
-            sn = validateSN(sn=serder.snh, inceptive=inceptive)
-            self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers)
+            #sn = validateSN(sn=serder.snh, inceptive=inceptive)
+            sn = Number(num=serder.sn).validate(inceptive=inceptive).sn
+            self.escrowPSEvent(serder=serder, sigers=sigers, wigers=wigers, local=local)
             self.escrowPACouple(serder=serder, seqner=delseqner, saider=delsaider)
             raise MissingDelegationError("No delegating event from {} at {} for "
-                                         "evt = {}.".format(delegator,
+                                         "evt = {}.".format(delpre,
                                                             delsaider.qb64,
                                                             serder.ked))
 
         # get the delegating event from dig
         ddig = bytes(raw)
-        key = dgKey(pre=delegator, dig=ddig)  # database key
+        key = dgKey(pre=delpre, dig=ddig)  # database key
         raw = self.db.getEvt(key)
         if raw is None:   # drop event
             raise ValidationError("Missing delegation from {} at event dig = {} for evt = {}."
-                                  "".format(delegator, ddig, serder.ked))
+                                  "".format(delpre, ddig, serder.ked))
 
         dserder = serdering.SerderKERI(raw=bytes(raw))  # delegating event
+
+
         # compare digests to make sure they match here
         if not dserder.compare(said=delsaider.qb64):  # drop event
             raise ValidationError("Invalid delegation from {} at event dig = {} for evt = {}."
-                                  "".format(delegator, ddig, serder.ked))
-
-        if self.kevers is None or delegator not in self.kevers:   # drop event
-            raise ValidationError("Missing Kever for delegator = {} for evt = {}."
-                                  "".format(delegator, serder.ked))
-
-        dkever = self.kevers[delegator]
-        if dkever.doNotDelegate:  # drop event
-            raise ValidationError("Delegator = {} for evt = {},"
-                                  " does not allow delegation.".format(delegator,
-                                                                       serder.ked))
+                                  "".format(delpre, ddig, serder.ked))
 
 
         found = False  # find event seal of delegated event in delegating data
         # XXXX ToDo need to change logic here to support native CESR seals not just dicts
         # for JSON, CBOR, MGPK
+        # may want to try harder here by walking KEL
         for dseal in dserder.seals:  # find delegating seal anchor
-            if tuple(dseal.keys()) == SealEvent._fields:
+            if tuple(dseal) == SealEvent._fields:
                 seal = SealEvent(**dseal)
                 if (seal.i == serder.pre and
                     seal.s == serder.sner.numh and
                     serder.compare(said=seal.d)):
                         found = True
                         break
 
         if not found:  # drop event
-            raise ValidationError("Missing delegation from {} in {} for evt = {}."
-                                  "".format(delegator, dserder.seals, serder.ked))
-
-        # Assumes database is reverified each bootup chain-of-custody of dic broken.
+            raise ValidationError(f"Missing delegation seal in designated event"
+                                  f"from {delpre} in {dserder.seals} for "
+                                  f"evt = {serder.ked}.")
+
+        # Found anchor so can assume delegation successful unless its one of
+        # the superseding condidtions.
+        # Assumes database is reverified each bootup chain-of-custody of disc broken.
         # Rule for non-supeding delegated rotation of rotation.
         # Returning delegator indicates success and eventually results acceptance
         # via Kever.logEvent which also writes the delgating event source couple to
         # db.aess so we can find it later
         if ((serder.ilk == Ilks.dip) or  # delegated inception
             (serder.sner.num == self.sner.num + 1) or  # inorder event
-            (serder.sner.num == self.sner.num and
-                self.ilk == Ilks.ixn and
+            (serder.sner.num == self.sner.num and  # superseding event
+                self.ilk == Ilks.ixn and  # superseded is ixn
                 serder.ilk == Ilks.drt)):  # recovery rotation superseding ixn
-                    return delegator  # indicates delegation valid with return of delegator
+                    return  # delegator  # indicates delegation valid with return of delegator
 
+        # get to here means drt rotation superseding another drt rotation
         # Kever.logEvent saves authorizer (delegator) seal source couple in
         # db.aess data base so can use it here to recusively look up delegating
         # events
 
         # set up recursive search for superseding delegations
         serfn = serder  # new potentially superseding delegated event i.e. serf new
         bossn = dserder # new delegating event of superseding delegated event i.e. boss new
         serfo = self.serder  # original delegated event i.e. serf original
-        bosso = self.fetchDelegatingEvent(delegator, serfo)
+        bosso = self.fetchDelegatingEvent(delpre, serfo)
 
         while (True):  # superseding delegated rotation of rotation recovery rules
             # Only get to here if same sn for drt existing and drt superseding
 
             if (bossn.sn > bosso.sn or  # later supersedes
                 (bossn.Ilk == Ilks.drt and
                  bosso.Ilk == Ilks.ixn) ): # drt supersedes ixn
-                    return delegator  # valid superseding delegation
+                    return  # delegator  # valid superseding delegation
 
             if bossn.said == bosso.said: # same delegating event
                 nseals = [SealEvent(**seal) for seal in bossn.seals
-                                  if tuple(seal.keys()) == SealEvent._fields]
+                                  if tuple(seal) == SealEvent._fields]
                 nindex = nseals.index(SealEvent(i=serfn.pre, s=serfn.snh, d=serfn.said))
                 oseals = [SealEvent(**seal) for seal in bosso.seals
-                                      if tuple(seal.keys()) == SealEvent._fields]
+                                      if tuple(seal) == SealEvent._fields]
                 oindex = oseals.index(SealEvent(i=serfo.pre, s=serfo.snh, d=serfo.said))
 
                 if nindex > oindex:  # later seal supersedes
                     # assumes index can't be None
-                    return delegator  # valid superseding delegation
+                    return  # delegator  # valid superseding delegation
 
                 else:
                     # ToDo: XXXX may want to cue up business logic for delegator
                     # if self.mine(delegator):  # failed attempt at recovery
                     raise ValidationError(f"Invalid delegation recovery rotation"
                                           f"of {serfo.ked} by {serfn.ked}")
 
             # tie condition same sn and drt so need to climb delegation chain
             serfn = bossn
-            bossn = self.fetchDelegatingEvent(delegator, serfn)
+            bossn = self.fetchDelegatingEvent(delpre, serfn)
             serfo = bosso
-            bosso = self.fetchDelegatingEvent(delegator, serfo)
+            bosso = self.fetchDelegatingEvent(delpre, serfo)
             # repeat
 
 
     def fetchDelegatingEvent(self, delegator, serder):
         """Returns delegating event by delegator of delegated event given by
         serder otherwise raises ValidationError.
         Assumes serder is already delegated event
@@ -2647,15 +2826,15 @@
                 # database broken this should never happen so do not supersede
                 raise ValidationError(f"Missing delegation source seal for {serder.ked}")
 
         return dserder
 
 
     def logEvent(self, serder, sigers=None, wigers=None, wits=None, first=False,
-                 seqner=None, saider=None, firner=None, dater=None):
+                 seqner=None, saider=None, firner=None, dater=None, local=True):
         """
         Update associated logs for verified event.
         Update is idempotent. Logs will not write dup at key if already exists.
 
         Parameters:
             serder is SerderKERI instance of current event
             sigers is optional list of Siger instance for current event
@@ -2671,31 +2850,43 @@
             firner is optional Seqner instance of cloned first seen ordinal
                 If cloned mode then firner maybe provided (not None)
                 When firner provided then compare fn of dater and database and
                 first seen if not match then log and add cue notify problem
             dater is optional Dater instance of cloned replay datetime
                 If cloned mode then dater maybe provided (not None)
                 When dater provided then use dater for first seen datetime
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
         """
+        local = True if local else False
         fn = None  # None means not a first seen log event so does not return an fn
+        dgkeys = (serder.pre, serder.said)
         dgkey = dgKey(serder.preb, serder.saidb)
         dtsb = helping.nowIso8601().encode("utf-8")
         self.db.putDts(dgkey, dtsb)  # idempotent do not change dts if already
         if sigers:
             self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])  # idempotent
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         if wits:
             self.db.wits.put(keys=dgkey, vals=[coring.Prefixer(qb64=w) for w in wits])
+
         self.db.putEvt(dgkey, serder.raw)  # idempotent (maybe already excrowed)
-        val = (coring.Prefixer(qb64b=serder.preb), coring.Seqner(sn=serder.sn))
-        for verfer in (serder.verfers if serder.verfers is not None else []):
-            self.db.pubs.add(keys=(verfer.qb64,), val=val)
-        for diger in (serder.ndigers if serder.ndigers is not None else []):
-            self.db.digs.add(keys=(diger.qb64,), val=val)
+        # update event source
+        if (esr := self.db.esrs.get(keys=dgkeys)):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkeys, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkeys, val=esr)
+
         if first:  # append event dig to first seen database in order
             if seqner and saider:  # delegation for authorized delegated or issued event
                 couple = seqner.qb64b + saider.qb64b
                 self.db.setAes(dgkey, couple)  # authorizer (delegator/issuer) event seal
             fn = self.db.appendFe(serder.preb, serder.saidb)
             if firner and fn != firner.sn:  # cloned replay but replay fn not match
                 if self.cues is not None:  # cue to notice BadCloneFN
@@ -2711,79 +2902,199 @@
             logger.info("Kever state: %s First seen ordinal %s at %s\nEvent=\n%s\n",
                         serder.preb, fn, dtsb.decode("utf-8"), serder.pretty())
         self.db.addKe(snKey(serder.preb, serder.sn), serder.saidb)
         logger.info("Kever state: %s Added to KEL valid event=\n%s\n",
                     serder.preb, serder.pretty())
         return (fn, dtsb.decode("utf-8"))  # (fn int, dts str) if first else (None, dts str)
 
-    def escrowPSEvent(self, serder, sigers, wigers=None):
+
+    def escrowMFEvent(self, serder, sigers, wigers=None,
+                      seqner=None, saider=None, local=True):
+        """
+        Update associated logs for escrow of MisFit event
+
+        Parameters:
+            serder (SerderKERI): instance of  event
+            sigers (list): of Siger instance for  event
+            wigers (list): of witness signatures
+            seqner (Seqner): instance of sn of event delegatint/issuing event if any
+            saider (Saider): instance of dig of event delegatint/issuing event if any
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
+        """
+        local = True if local else False
+        dgkey = dgKey(serder.preb, serder.saidb)
+        if esr := self.db.esrs.get(keys=dgkey):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
+        self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
+        self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
+        self.db.putEvt(dgkey, serder.raw)
+        if wigers:
+            self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
+        if seqner and saider:
+            couple = seqner.qb64b + saider.qb64b
+            self.db.putPde(dgkey, couple)  # idempotent
+        self.db.misfits.add(snKey(serder.preb, serder.sn), serder.saidb)
+        # log escrowed
+        logger.info("Kever state: escrowed misfit event=\n%s\n",
+                    json.dumps(serder.ked, indent=1))
+
+
+    def escrowDelegableEvent(self, serder, sigers, wigers=None, local=True):
+        """
+        Update associated logs for escrow of Delegable event that needs delegation
+        via an anchored seal in delegator's KEl
+
+        Parameters:
+            serder (SerderKERI): instance of  event
+            sigers (list): of Siger instance for  event
+            wigers (list): of witness signatures
+            seqner (Seqner): instance of sn of event delegatint/issuing event if any
+            saider (Saider): instance of dig of event delegatint/issuing event if any
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
+        """
+        local = True if local else False
+        dgkey = dgKey(serder.preb, serder.saidb)
+        if esr := self.db.esrs.get(keys=dgkey):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
+        self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
+        self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
+        self.db.putEvt(dgkey, serder.raw)
+        if wigers:
+            self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
+        self.db.delegables.add(snKey(serder.preb, serder.sn), serder.saidb)
+        # log escrowed
+        logger.info("Kever state: escrowed delegable event=\n%s\n",
+                    json.dumps(serder.ked, indent=1))
+
+
+    def escrowPSEvent(self, serder, sigers, wigers=None, local=True):
         """
         Update associated logs for escrow of partially signed event
         or fully signed delegated event but not yet verified delegation.
 
         Parameters:
             serder is SerderKERI instance of event
             sigers is list of Siger instances of indexed controller sigs
             wigers is optional list of Siger instance of indexed witness sigs
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
         """
+        local = True if local else False
         dgkey = dgKey(serder.preb, serder.saidb)
         self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))  # idempotent
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
+
         self.db.putEvt(dgkey, serder.raw)
+        # update event source
+        if esr := self.db.esrs.get(keys=dgkey):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
         snkey = snKey(serder.preb, serder.sn)
         self.db.addPse(snkey, serder.saidb)  # b'EOWwyMU3XA7RtWdelFt-6waurOTH_aW_Z9VTaU-CshGk.00000000000000000000000000000001'
         logger.info("Kever state: Escrowed partially signed or delegated "
                     "event = %s\n", serder.ked)
 
-    def escrowPACouple(self, serder, seqner, saider):
+
+    def escrowPACouple(self, serder, seqner, saider, local=True):
         """
         Update associated logs for escrow of partially authenticated issued event.
         Assuming signatures are provided elsewhere. Partial authentication results
         from either a partially signed event or a fully signed delegated event
         but whose delegation is not yet verified.
 
         Escrow allows escrow processor to retrieve serder from key and source
         couple from val in order to to re-verify authentication status. Sigs
         are escrowed elsewhere.
 
         Parameters:
             serder is SerderKERI instance of delegated or issued event
             seqner is Seqner instance of sn of seal source event of delegator/issuer
             saider is Saider instance of said of delegator/issuer
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
         """
+        local = True if local else False  # ignored since not escrowing serder here
         dgkey = dgKey(serder.preb, serder.saidb)
         couple = seqner.qb64b + saider.qb64b
         self.db.putPde(dgkey, couple)  # idempotent
         logger.info("Kever state: Escrowed source couple for partially signed "
                     "or delegated event = %s\n", serder.ked)
 
-    def escrowPWEvent(self, serder, wigers, sigers=None, seqner=None, saider=None):
+
+    def escrowPWEvent(self, serder, wigers, sigers=None,
+                      seqner=None, saider=None, local=True):
         """
         Update associated logs for escrow of partially witnessed event
 
         Parameters:
             serder is SerderKERI instance of  event
             wigers is list of Siger instance of indexed witness sigs
             sigers is optional list of Siger instances of indexed controller sigs
             seqner is Seqner instance of sn of seal source event of delegator/issuer
             saider is Diger instance of digest of delegator/issuer
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
+
         """
+        local = True if local else False
         dgkey = dgKey(serder.preb, serder.saidb)
         self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))  # idempotent
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         if sigers:
             self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         if seqner and saider:
             couple = seqner.qb64b + saider.qb64b
             self.db.putPde(dgkey, couple)
 
         self.db.putEvt(dgkey, serder.raw)
+        # update event source
+        if (esr := self.db.esrs.get(keys=dgkey)):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else: # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
         logger.info("Kever state: Escrowed partially witnessed "
                     "event = %s\n", serder.ked)
         return self.db.addPwe(snKey(serder.preb, serder.sn), serder.saidb)
 
 
     def state(self):
         """
@@ -2812,15 +3123,15 @@
                       eevt=eevt,
                       sith=self.tholder.sith,
                       nsith=self.ntholder.sith if self.ntholder else '0',
                       ndigs=[diger.qb64 for diger in self.ndigers],
                       toad=self.toader.num,
                       wits=self.wits,
                       cnfg=cnfg,
-                      dpre=self.delegator,
+                      dpre=self.delpre,
                       )
                 )
 
 
     def fetchPriorDigers(self, sn: int | None = None) -> list | None:
         """ Returns either the most recent prior list of digers before .lastEst or None
 
@@ -2890,15 +3201,15 @@
             sn = self.lastEst.s
 
         keys = [verfer.qb64 for verfer in verfers]
 
         for digb in self.db.getKelBackIter(pre, sn):
             dgkey = dgKey(pre, digb)
             raw = self.db.getEvt(dgkey)
-            serder = serdering.SerderKERI(raw=bytes(raw))
+            serder = serdering.SerderKERI(raw=bytes(raw), verify=False)
             if serder.estive:  # establishment event
                 key = serder.verfers[0].qb64
                 try:
                     i = keys.index(key)  # find index of key in keys
                 except ValueError:  # not found
                     continue
 
@@ -2943,15 +3254,15 @@
             sn = self.lastEst.s
 
         key = verfer.qb64
 
         for digb in self.db.getKelBackIter(pre, sn):
             dgkey = dgKey(pre, digb)
             raw = self.db.getEvt(dgkey)
-            serder = serdering.SerderKERI(raw=bytes(raw))
+            serder = serdering.SerderKERI(raw=bytes(raw), verify=False)
             if serder.estive:  # establishment event
                 keys = [verfer.qb64 for verfer in serder.verfers]
                 try:
                     i = keys.index(key) # find index of key in keys
                 except ValueError:  # not found
                     continue
 
@@ -3022,16 +3333,16 @@
         Parameters:
             cues (Deck)  notices to create responses to evts
             kevers is dict of Kever instances of key state in db
             db (Baser): instance of database
             lax (bool): True means operate in promiscuous (unrestricted) mode,
                            False means operate in nonpromiscuous (restricted) mode
                               as determined by local and prefixes
-            local (bool): True means only process msgs for own events if not lax
-                         False means only process msgs for not own events if not lax
+            local (bool): True means event source is local (protected) for validation
+                         False means event source is remote (unprotected) for validation
             cloned (bool): True means cloned message stream so use attached
                          datetimes from clone source not own.
                          False means use current datetime
             direct (bool): True means direct mode so cue notices for receipts etc
                           False means indirect mode so don't cue notices
             check (bool): True means do not update the database in any
                 non-idempotent way. Useful for reinitializing the Kevers from
@@ -3040,15 +3351,15 @@
         """
         self.cues = cues if cues is not None else decking.Deck()  # subclass of deque
         if db is None:
             db = basing.Baser(reopen=True)  # default name = "main"
         self.db = db
         self.rvy = rvy
         self.lax = True if lax else False  # promiscuous mode
-        self.local = True if local else False  # local vs nonlocal restrictions
+        self.local = True if local else False  # local vs nonlocal default
         self.cloned = True if cloned else False  # process as cloned
         self.direct = True if direct else False  # process as direct mode
         self.check = True if check else False  # process as check mode
 
     @property
     def kevers(self):
         """
@@ -3090,47 +3401,54 @@
                 return wits
 
         return []
 
 
     def processEvent(self, serder, sigers, *, wigers=None,
                      delseqner=None, delsaider=None,
-                     firner=None, dater=None):
+                     firner=None, dater=None, local=None):
         """
         Process one event serder with attached indexd signatures sigers
 
         Parameters:
-            serder is SerderKERI instance of event to process
-            sigers is list of Siger instances of attached controller indexed sigs
-            wigers is optional list of Siger instances of attached witness indexed sigs
-            delseqner is Seqner instance of delegating event sequence number.
+            serder (SerderKERI): instance of event to process
+            sigers (list[Siger]): instances of attached controller indexed sigs
+            wigers (list[Siger]|None): instances of attached witness indexed sigs
+                otherwise None
+            delseqner (Seqner|None): instance of delegating event sequence number.
                 If this event is not delegated then seqner is ignored
-            delsaider is Saider instance of of delegating event SAID.
+            delsaider (Saider|None): instance of of delegating event SAID.
                 If this event is not delegated then saider is ignored
-            firner is optional Seqner instance of cloned first seen ordinal
+            firner (Seqner|None): instance of cloned first seen ordinal
                 If cloned mode then firner maybe provided (not None)
                 When firner provided then compare fn of dater and database and
                 first seen if not match then log and add cue notify problem
-            dater is optional Dater instance of cloned replay datetime
+            dater (Dater|None): instance of cloned replay datetime
                 If cloned mode then dater maybe provided (not None)
                 When dater provided then use dater for first seen datetime
+            local (bool|None): True means local (protected) event source.
+                               False means remote (unprotected).
+                               None means use default .local .
         """
+        local = local if local is not None else self.local
+        local = True if local else False  # force boolean
+
         # fetch ked ilk  pre, sn, dig to see how to process
         pre = serder.pre
         ked = serder.ked
 
         # See todo for Prefixer fix redundancy XXX
         try:  # see if code of pre is supported and matches size of pre
             Prefixer(qb64=pre)
         except Exception as ex:  # if unsupported code or bad size raises error
             raise ValidationError("Invalid pre = {} for evt = {}."
                                   "".format(pre, ked)) from ex
 
         sn = serder.sn
-        ilk = serder.ilk # ked["t"]
+        ilk = serder.ilk  # ked["t"]
         said = serder.said
 
 
         if pre not in self.kevers:  # first seen event for pre
             if ilk in (Ilks.icp, Ilks.dip):  # first seen and inception so verify event keys
                 # kever init verifies basic inception stuff and signatures
                 # raises exception if problem
@@ -3141,37 +3459,61 @@
                               wigers=wigers,
                               db=self.db,
                               delseqner=delseqner,
                               delsaider=delsaider,
                               firner=firner if self.cloned else None,
                               dater=dater if self.cloned else None,
                               cues=self.cues,
-                              prefixes=self.prefixes,
-                              local=self.local,
+                              local=local,
                               check=self.check)
                 self.kevers[pre] = kever  # not exception so add to kevers
 
+                # At this point  the inceptive event (icp or dip) given by serder
+                # together with its attachments has been accepted as valid with finality.
+                # Events that don't get to here have either been dropped as
+                # invalid by raising an error or have been escrowed as not
+                # yet complete enough to decide their validity, i.e. are
+                # missing signatures, or witness receipts or delegations.
+                # Any actions that should be triggered as a result of final
+                # acceptance should follow from here.
+
                 if self.direct or self.lax or pre not in self.prefixes:  # not own event when owned
                     # create cue for receipt  controller or watcher
                     #  receipt of actual type is dependent on own type of identifier
                     self.cues.push(dict(kin="receipt", serder=serder))
                 elif not self.direct:  # notice of new  event
                     self.cues.push(dict(kin="notice", serder=serder))
 
-                if kever.locallyWitnessed():
-                    # ToDo XXXX  need to cue task here kin = "witness"
+                if self.local and kever.locallyWitnessed():  #
+                    # ToDo XXXX  need to cue task here kin = "witness" and process
+                    # cued witness and then combine with reciept above so only
+                    # one receipt is generated not two
                     self.cues.push(dict(kin="witness", serder=serder))
 
-                if kever.locallyOwned(kever.delegator):  # delegator may be None
-                    # ToDo XXXX  need to cue task here  to approve delegation by generating
-                    # and anchoring SealEvent of serder in delegators KEL
-                    # may include MFA business logic for the delegator i.e. is local
-                    self.cues.push(dict(kin="approveDelegation",
-                                            delegator=kever.delegator,
-                                            serder=serder))
+                if self.local and kever.locallyOwned():
+                    # ToDo XXXX process  this cue of query to send event to delegator
+                    # to trigger generation of anchor in delegating event
+                    # note for remote validators there is query cue in
+                    # validateDelegation to query for anchoring event seal
+                    pass
+
+                # Moved logic to kever.validateDelegation trigger for delegation escrow
+                #if (self.local and
+                    #kever.locallyOwned(kever.delpre if kever.delpre is not None else '')):  # delpre may be None
+                    ## ToDo XXXX  need to cue task here  to approve delegation by generating
+                    ## an anchoring SealEvent of serder in delegators KEL
+                    ## may include MFA and or business logic for the delegator i.e. is local
+                    ## event that designates this controller as delegator triggers
+                    ## this cue to approave delegation
+                    #self.cues.push(dict(kin="approveDelegation",
+                                            #delegator=kever.delpre,
+                                            #serder=serder))
+
+
+
 
 
             else:  # not inception so can't verify sigs etc, add to out-of-order escrow
                 self.escrowOOEvent(serder=serder, sigers=sigers,
                                    seqner=delseqner, saider=delsaider, wigers=wigers)
                 raise OutOfOrderError("Out-of-order event={}.".format(ked))
 
@@ -3194,16 +3536,17 @@
                     wigers, windices = verifySigs(raw=serder.raw,
                                                   sigers=wigers,
                                                   verfers=eserder.berfers)
 
                     if sigers or wigers:  # at least one verified sig or wig so log evt
                         # this allows late arriving witness receipts or controller
                         # signatures to be added to the databse
-                        # not first seen inception so ignore return
-                        kever.logEvent(serder, sigers=sigers, wigers=wigers)  # idempotent update db logs
+                        # Not first seen version of event so ignore return
+                        # idempotent update db logs
+                        kever.logEvent(serder, sigers=sigers, wigers=wigers)
 
                 else:  # escrow likely duplicitous event
                     self.escrowLDEvent(serder=serder, sigers=sigers)
                     raise LikelyDuplicitousError("Likely Duplicitous event={}.".format(ked))
 
             else:  # rot, drt, or ixn, so sn matters
                 kever = self.kevers[pre]  # get existing kever for pre
@@ -3224,35 +3567,57 @@
                     # verify signatures etc and update state if valid
                     # raise exception if problem.
                     # Otherwise adds to KELs
                     kever.update(serder=serder, sigers=sigers, wigers=wigers,
                                  delseqner=delseqner, delsaider=delsaider,
                                  firner=firner if self.cloned else None,
                                  dater=dater if self.cloned else None,
-                                 check=self.check)
+                                 local=local, check=self.check)
+
+                    # At this point the non-inceptive event (rot, drt, or ixn)
+                    # given by serder together with its attachments has been
+                    # accepted as valid with finality.
+                    # Events that don't get to here have either been dropped as
+                    # invalid by raising an error or have been escrowed as not
+                    # yet complete enough to decide their validity, i.e. are
+                    # missing signatures, or witness receipts or delegations.
+                    # Any actions that should be triggered as a result of final
+                    # acceptance should follow from here.
 
                     if self.direct or self.lax or pre not in self.prefixes:  # not own event when owned
                         # create cue for receipt  controller or watcher
                         #  receipt of actual type is dependent on own type of identifier
                         self.cues.push(dict(kin="receipt", serder=serder))
                     elif not self.direct:  # notice of new  event
                         self.cues.push(dict(kin="notice", serder=serder))
 
-                    if kever.locallyWitnessed():
-                        # ToDo XXXX  need to cue task here kin = "witness"
+                    if self.local and kever.locallyWitnessed():  #
+                        # ToDo XXXX  need to cue task here kin = "witness" and process
+                        # cued witness and then combine with reciept above so only
+                        # one receipt is generated not two
                         self.cues.push(dict(kin="witness", serder=serder))
 
-                    if kever.locallyOwned(kever.delegator):  # delegator may be None
-                        # ToDo XXXX  need to cue task here  to approve delegation by generating
-                        # and anchoring SealEvent of serder in delegators KEL
-                        # may include MFA business logic   for the delegator i.e. is local
-                        self.cues.push(dict(kin="approveDelegation",
-                                            delegator=kever.delegator,
-                                            serder=serder))
-
+                    if self.local and kever.locallyOwned():
+                        # ToDo XXXX process  this cue of query to send event to delegator
+                        # to trigger generation of anchor in delegating event
+                        # note for remote validators there is query cue in
+                        # validateDelegation to query for anchoring event seal
+                        pass
+
+                    # Moved logic to kever.validateDelegation trigger for delegation escrow
+                    #if (self.local and
+                        #kever.locallyOwned(kever.delpre if kever.delpre is not None else '')):  # delpre may be None
+                        ## ToDo XXXX  need to cue task here  to approve delegation by generating
+                        ## an anchoring SealEvent of serder in delegators KEL
+                        ## may include MFA and or business logic for the delegator i.e. is local
+                        ## event that designates this controller as delegator triggers
+                        ## this cue to approave delegation
+                        #self.cues.push(dict(kin="approveDelegation",
+                                                #delegator=kever.delpre,
+                                                #serder=serder))
 
                 else:  # maybe duplicitous
                     # check if duplicate of existing valid accepted event
                     ddig = bytes(self.db.getKeLast(key=snKey(pre, sn))).decode("utf-8")
                     if ddig == said:  # event is a duplicate but not duplicitous
                         eserder = self.fetchEstEvent(pre, sn)  # latest est event wrt sn
                         # may have attached valid signature not yet logged
@@ -3266,43 +3631,53 @@
                         wits = [wit.qb64 for wit in self.fetchWitnessState(pre, sn)]
                         werfers = [Verfer(qb64=wit) for wit in wits]
                         wigers, windices = verifySigs(raw=serder.raw,
                                                       sigers=wigers,
                                                       verfers=werfers)
 
                         if sigers or wigers:  # at least one verified sig or wig so log evt
-                            # not first seen update so ignore return
+                            # this allows late arriving witness receipts or controller
+                            # signatures to be added to the databse
+                            # Not first seen version of event so ignore return
+                            # idempotent update db logs
                             kever.logEvent(serder, sigers=sigers, wigers=wigers)  # idempotent update db logs
 
                     else:  # escrow likely duplicitous event
                         self.escrowLDEvent(serder=serder, sigers=sigers)
                         raise LikelyDuplicitousError("Likely Duplicitous event={}.".format(ked))
 
-    def processReceiptWitness(self, serder, wigers):
+
+    def processReceiptWitness(self, serder, wigers, local=None):
         """
-        Process one witness receipt serder with attached witness sigers
+        Process one witness receipt serder with attached witness wigers
+        (indexed signatures)
 
         Parameters:
-            serder is SerderKERI instance of serialized receipt message not receipted event
-            sigers is list of Siger instances that with witness indexed signatures
+            serder (SerderKERI): instance of serialized receipt message not receipted event
+            wigers (list[Siger]): instances that with witness indexed signatures
                 signature in .raw. Index is offset into witness list of latest
                 establishment event for receipted event. Signature uses key pair
                 derived from nontrans witness prefix in associated witness list.
+            local (bool|None): True means local (protected) event source.
+                               False means remote (unprotected).
+                               None means use default .local .
 
         Receipt dict labels
             vs  # version string
             pre  # qb64 prefix
             sn  # hex string sequence number
             ilk  # rct
             dig  # qb64 digest of receipted event
         """
+        local = local if local is not None else self.local
+        local = True if local else False  # force boolean
+
         # fetch  pre dig to process
         ked = serder.ked
         pre = serder.pre
-
         sn = serder.sn
 
         # Only accept receipt if for last seen version of event at sn
         snkey = snKey(pre=pre, sn=sn)
         ldig = self.db.getKeLast(key=snkey)  # retrieve dig of last event at sn.
         if ldig is not None:  # verify digs match
             ldig = bytes(ldig).decode("utf-8")
@@ -3322,51 +3697,60 @@
                 # assign verfers from witness list
                 if wiger.index >= len(wits):
                     continue  # skip invalid witness index
                 wiger.verfer = Verfer(qb64=wits[wiger.index])  # assign verfer
                 if wiger.verfer.transferable:  # skip transferable verfers
                     continue  # skip invalid witness prefix
 
-                if not self.lax and wiger.verfer.qb64 in self.prefixes:  # own is receiptor
+                if not self.lax and wiger.verfer.qb64 in self.prefixes:  # own is witness
                     if pre in self.prefixes:  # skip own receiptor of own event
                         # sign own events not receipt them
                         logger.info("Kevery process: skipped own receipt attachment"
                                     " on own event receipt=\n%s\n", serder.pretty())
                         continue  # skip own receipt attachment on own event
-                    if not self.local:  # own receipt on other event when not local
+                    if not local:  # so skip own receipt on other event when non-local source
                         logger.info("Kevery process: skipped own receipt attachment"
                                     " on nonlocal event receipt=\n%s\n", serder.pretty())
                         continue  # skip own receipt attachment on non-local event
 
                 if wiger.verfer.verify(wiger.raw, lserder.raw):
                     # write receipt indexed sig to database
                     self.db.addWig(key=dgkey, val=wiger.qb64b)
 
         else:  # no events to be receipted yet at that sn so escrow
             # get digest from receipt message not receipted event
             self.escrowUWReceipt(serder=serder, wigers=wigers, said=ked["d"])
             raise UnverifiedWitnessReceiptError("Unverified witness receipt={}."
                                                 "".format(ked))
 
-    def processReceipt(self, serder, cigars):
+    def processReceipt(self, serder, cigars, local=None):
         """
         Process one receipt serder with attached cigars
+        may or may not be a witness receipt. If prefix matches witness then
+        promote to indexed witness signature and store appropriately. Otherwise
+        signature is nontrans nonwitness endorser (watcher etc)
 
         Parameters:
-            serder is SerderKERI instance of serialized receipt message not receipted message
-            cigars is list of Cigar instances that contain receipt couple
+            serder (SerderKERI): rct instance of serialized receipt message
+            cigars (list[Cigar]): instances that contain receipt couple
                 signature in .raw and public key in .verfer
+            local (bool|None): True means local (protected) event source.
+                               False means remote (unprotected).
+                               None means use default .local .
 
         Receipt dict labels
             vs  # version string
             pre  # qb64 prefix
             sn  # hex string sequence number
             ilk  # rct
             dig  # qb64 digest of receipted event
         """
+        local = local if local is not None else self.local
+        local = True if local else False  # force boolean
+
         # fetch  pre dig to process
         ked = serder.ked
         pre = serder.pre
         sn = serder.sn
 
         # Only accept receipt if for last seen version of event at sn
         snkey = snKey(pre=pre, sn=sn)
@@ -3391,48 +3775,61 @@
 
                 if not self.lax and cigar.verfer.qb64 in self.prefixes:  # own is receiptor
                     if pre in self.prefixes:  # skip own receipter of own event
                         # sign own events not receipt them
                         logger.info("Kevery process: skipped own receipt attachment"
                                     " on own event receipt=\n%s\n", serder.pretty())
                         continue  # skip own receipt attachment on own event
-                    if not self.local:  # own receipt on other event when not local
+                    if not local:  # skip own receipt on other event when not local
                         logger.info("Kevery process: skipped own receipt attachment"
                                     " on nonlocal event receipt=\n%s\n", serder.pretty())
                         continue  # skip own receipt attachment on non-local event
 
                 if cigar.verfer.verify(cigar.raw, lserder.raw):
                     wits = [wit.qb64 for wit in self.fetchWitnessState(pre, sn)]
                     rpre = cigar.verfer.qb64  # prefix of receiptor
-                    if rpre in wits:  # its a witness receipt
+                    if rpre in wits:  # its a witness receipt write in .wigs
                         index = wits.index(rpre)
                         # create witness indexed signature
                         wiger = Siger(raw=cigar.raw, index=index, verfer=cigar.verfer)
                         self.db.addWig(key=dgkey, val=wiger.qb64b)  # write to db
-                    else:  # write receipt couple to database
+                    else:  # not witness rect write receipt couple to database .rcts
                         couple = cigar.verfer.qb64b + cigar.qb64b
                         self.db.addRct(key=dgkey, val=couple)
 
         else:  # no events to be receipted yet at that sn so escrow
             self.escrowUReceipt(serder, cigars, said=ked["d"])  # digest in receipt
             raise UnverifiedReceiptError("Unverified receipt={}.".format(ked))
 
-    def processReceiptCouples(self, serder, cigars, firner=None):
+
+    def processAttachedReceiptCouples(self, serder, cigars, firner=None, local=None):
         """
-        Process attachment with receipt couple
+        Process one attachment couple that represents an endorsement from
+        a nontransferable AID  that may or may not be a witness, maybe a watcher.
+        Originally may have been a non-transferable receipt or key event attachment
+        if signature is for witness then promote to indexed sig and store
+        appropriately.
+        The is the attachment version of .processReceipt
 
         Parameters:
-            serder is SerderKERI instance of receipted serialized event message
-                to which receipts are attached from replay
-            cigars is list of Cigar instances that contain receipt couple
+            serder (SerderKERI): instance serialized event message to which
+                attachments come from replay (clone)
+            cigars (list[Cigar]): instances that contain receipt couple
                 signature in .raw and public key in .verfer
-            firner is Seqner instance of first seen ordinal,
+            firner (Seqner): instance of first seen ordinal,
                 if provided lookup event by fn = firner.sn
+                used when in cloned replay mode
+            local (bool|None): True means local (protected) event source.
+                               False means remote (unprotected).
+                               None means use default .local .
 
         """
+        local = local if local is not None else self.local
+        local = True if local else False  # force boolean
+
         # fetch  pre dig to process
         ked = serder.ked
         pre = serder.pre
         sn = serder.sn
 
         # Only accept receipt if event is latest event at sn. Means its been
         # first seen and is the most recent first seen with that sn
@@ -3459,15 +3856,15 @@
                 continue  # skip invalid couplets
             if not self.lax and cigar.verfer.qb64 in self.prefixes:  # own is receiptor
                 if pre in self.prefixes:  # skip own receipter on own event
                     # sign own events not receipt them
                     logger.info("Kevery process: skipped own receipt attachment"
                                 " on own event receipt=\n%s\n", serder.pretty())
                     continue  # skip own receipt attachment on own event
-                if not self.local:  # own receipt on other event when not local
+                if not local:  # own receipt on other event when not local
                     logger.info("Kevery process: skipped own receipt attachment"
                                 " on nonlocal event receipt=\n%s\n", serder.pretty())
                     continue  # skip own receipt attachment on non-local event
 
             if cigar.verfer.verify(cigar.raw, serder.raw):
                 wits = self.fetchWitnessState(pre, sn)
                 rpre = cigar.verfer.qb64  # prefix of receiptor
@@ -3476,31 +3873,39 @@
                     # create witness indexed signature and write to db
                     wiger = Siger(raw=cigar.raw, index=index, verfer=cigar.verfer)
                     self.db.addWig(key=dgKey(pre, ldig), val=wiger.qb64b)
                 else:  # write receipt couple to database
                     couple = cigar.verfer.qb64b + cigar.qb64b
                     self.db.addRct(key=dgKey(pre, ldig), val=couple)
 
-    def processReceiptTrans(self, serder, tsgs):
+    def processReceiptTrans(self, serder, tsgs, local=None):
         """
         Process one transferable validator receipt (chit) serder with attached sigers
+        (indexed signatures) who are not controllers. Controllers may only attach signatures to
+        the associated event not by sending signature attached to receipt of event.
 
         Parameters:
-            serder is chit serder (transferable validator receipt message)
-            tsgs is tist of tuples from extracted transferable indexed sig groups
+            serder (serderKERI): rct (transferable validator receipt message)
+            tsgs (list[tuple]): from extracted transferable indexed sig groups
                 each converted group is tuple of (i,s,d) triple plus list of sigs
+            local (bool|None): True means local (protected) event source.
+                               False means remote (unprotected).
+                               None means use default .local .
 
         Receipt dict labels
             vs  # version string
             pre  # qb64 prefix
             sn  # hex string sequence number
             ilk  # rct
             dig  # qb64 digest of receipted event
 
         """
+        local = local if local is not None else self.local
+        local = True if local else False  # force boolean
+
         # fetch  pre, dig,seal to process
         ked = serder.ked
         pre = serder.pre
         sn = serder.sn
 
         # Only accept receipt if for last seen version of event at sn
         ldig = self.db.getKeLast(key=snKey(pre=pre, sn=sn))  # retrieve dig of last event at sn.
@@ -3518,34 +3923,34 @@
         if not lserder.compare(said=ldig):  # mismatch events problem with replay
             raise ValidationError("Mismatch receipt of event at sn = {} with db."
                                   "".format(sn))
 
         for sprefixer, sseqner, saider, sigers in tsgs:  # iterate over each tsg
             if not self.lax and sprefixer.qb64 in self.prefixes:  # own is receipter
                 if pre in self.prefixes:  # skip own receipter of own event
-                    # sign own events not receipt them
+                    # sign own events as controller not endorse them via receipt
                     raise ValidationError("Own pre={} receipter of own event"
                                           " {}.".format(self.prefixes, serder.pretty()))
-                if not self.local:  # skip own receipts of nonlocal events
+                if not local:  # skip own receipts of nonlocal events
                     raise ValidationError("Own pre={} receipter of nonlocal event "
                                           "{}.".format(self.prefixes, serder.pretty()))
 
             # receipted event in db so attempt to get receipter est evt
-            # retrieve dig of last event at sn of est evt of receipter.
+            # retrieve dig of last event at sn of est evt of receiptor.
             sdig = self.db.getKeLast(key=snKey(pre=sprefixer.qb64b, sn=sseqner.sn))
             if sdig is None:
-                # receipter's est event not yet in receipters's KEL
+                # receiptor's est event not yet in receiptors's KEL
                 # so need cue to discover est evt KEL for receipter from watcher etc
                 self.escrowTReceipts(serder, sprefixer, sseqner, saider, sigers)
                 raise UnverifiedTransferableReceiptError("Unverified receipt: "
                                                          "missing establishment event of transferable "
                                                          "receipter for event={}."
                                                          "".format(ked))
 
-            # retrieve last event itself of receipter est evt from sdig.
+            # retrieve last event itself of receiptor est evt from sdig.
             sraw = self.db.getEvt(key=dgKey(pre=sprefixer.qb64b, dig=bytes(sdig)))
             # assumes db ensures that sraw must not be none because sdig was in KE
             sserder = serdering.SerderKERI(raw=bytes(sraw))
             if not sserder.compare(said=saider.qb64):  # endorser's dig not match event
                 raise ValidationError("Bad trans indexed sig group at sn = {}"
                                       " for ksn = {}."
                                       "".format(sseqner.sn, sserder.ked))
@@ -3553,42 +3958,53 @@
             # verify sigs and if so write receipt to database
             sverfers = sserder.verfers
             if not sverfers:
                 raise ValidationError("Invalid receipter's est. event"
                                       " dig = {}  from pre ={}, no keys."
                                       "".format(saider.qb64, sprefixer.qb64))
 
-            for siger in sigers:
+            for siger in sigers:  # endorser (non-controller) signatures
                 if siger.index >= len(sverfers):
                     raise ValidationError("Index = {} to large for keys."
                                           "".format(siger.index))
                 siger.verfer = sverfers[siger.index]  # assign verfer
                 if siger.verfer.verify(siger.raw, lserder.raw):  # verify sig
                     # good sig so write receipt quadruple to database
                     quadruple = sprefixer.qb64b + sseqner.qb64b + saider.qb64b + siger.qb64b
                     self.db.addVrc(key=dgKey(pre=pre, dig=ldig),
                                    val=quadruple)  # dups kept
 
-    def processReceiptQuadruples(self, serder, trqs, firner=None):
+    def processAttachedReceiptQuadruples(self, serder, trqs, firner=None, local=None):
         """
-        Process one attachment quadruple that comprises a transferable receipt
+        Process one attachment quadruple that represents an endorsement from
+        a transferable AID that is not the controller. Maybe a watcher.
+        Originally may have been a transferable receipt or key event attachment
+
+        This is the attachement version of .processReceiptTrans
 
         Parameters:
-            serder is chit serder (transferable validator receipt message)
-            trqs is list of tuples (quadruples) of form
-                (prefixer, seqner, diger, siger)
-            firner is Seqner instance of first seen ordinal,
+            serder (serderKERI):  instance serialized event message to which
+                attachments come from replay (clone)
+            trqs (list[tuple]): quadruples of (prefixer, seqner, diger, siger)
+            firner (Seqner): instance of first seen ordinal,
                if provided lookup event by fn = firner.sn
+               used when in cloned replay mode
+            local (bool|None): True means local (protected) event source.
+                               False means remote (unprotected).
+                               None means use default .local .
 
         Seal labels
             i pre  # qb64 prefix of receipter
             s sn   # hex of sequence number of est event for receipter keys
             d dig  # qb64 digest of est event for receipter keys
 
         """
+        local = local if local is not None else self.local
+        local = True if local else False  # force boolean
+
         # fetch  pre, dig,seal to process
         ked = serder.ked
         pre = serder.pre
         sn = serder.sn
 
         if firner:  # retrieve last event by fn ordinal
             ldig = self.db.getFe(key=fnKey(pre=pre, sn=firner.sn))
@@ -3598,15 +4014,15 @@
 
         for sprefixer, sseqner, saider, siger in trqs:  # iterate over each trq
             if not self.lax and sprefixer.qb64 in self.prefixes:  # own trans receipt quadruple (chit)
                 if pre in self.prefixes:  # skip own trans receipts of own events
                     raise ValidationError("Own pre={} replay attached transferable "
                                           "receipt quadruple of own event {}."
                                           "".format(self.prefixes, serder.pretty()))
-                if not self.local:  # skip own trans receipt quadruples of nonlocal events
+                if not local:  # skip own trans receipt quadruples of nonlocal events
                     raise ValidationError("Own pre={} seal in replay attached "
                                           "transferable receipt quadruples of nonlocal"
                                           " event {}.".format(self.prefixes, serder.pretty()))
 
             if ldig is not None and sprefixer.qb64 in self.kevers:
                 # both receipted event and receipter in database so retreive
                 if isinstance(ldig, memoryview):
@@ -4121,16 +4537,16 @@
                     self.escrowQueryNotFoundEvent(serder=serder, prefixer=source, sigers=sigers, cigars=cigars)
                     raise QueryNotFoundError("Query not found error={}.".format(ked))
 
             msgs = list()  # outgoing messages
             for msg in self.db.clonePreIter(pre=pre, fn=0):
                 msgs.append(msg)
 
-            if kever.delegator:
-                cloner = self.db.clonePreIter(pre=kever.delegator, fn=0)  # create iterator at 0
+            if kever.delpre:
+                cloner = self.db.clonePreIter(pre=kever.delpre, fn=0)  # create iterator at 0
                 for msg in cloner:
                     msgs.append(msg)
 
             if msgs:
                 self.cues.push(dict(kin="replay", src=src, msgs=msgs, dest=source.qb64))
 
         elif route == "ksn":
@@ -4199,35 +4615,91 @@
             if serder.ked["t"] in (Ilks.icp, Ilks.dip, Ilks.rot, Ilks.drt):
                 return serder  # establishment event so return
 
             sn = int(serder.ked["s"], 16) - 1  # set sn to previous event
             if sn < 0:  # no more events
                 return None
 
-    def escrowOOEvent(self, serder, sigers, seqner=None, saider=None, wigers=None):
+
+    def escrowMFEvent(self, serder, sigers, wigers=None,
+                      seqner=None, saider=None, local=True):
+        """
+        Update associated logs for escrow of MisFit event
+
+        Parameters:
+            serder (SerderKERI): instance of  event
+            sigers (list): of Siger instance for  event
+            seqner (Seqner): instance of sn of event delegatint/issuing event if any
+            saider (Saider): instance of dig of event delegatint/issuing event if any
+            wigers (list): of witness signatures
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
+        """
+        local = True if local else False
+        dgkey = dgKey(serder.preb, serder.saidb)
+        if esr := self.db.esrs.get(keys=dgkey):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
+        self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
+        self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
+        self.db.putEvt(dgkey, serder.raw)
+        if wigers:
+            self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
+        if seqner and saider:
+            couple = seqner.qb64b + saider.qb64b
+            self.db.putPde(dgkey, couple)  # idempotent
+        self.db.misfits.add(snKey(serder.preb, serder.sn), serder.saidb)
+        # log escrowed
+        logger.info("Kevery process: escrowed misfit event=\n%s\n",
+                    json.dumps(serder.ked, indent=1))
+
+
+    def escrowOOEvent(self, serder, sigers, seqner=None, saider=None, wigers=None, local=True):
         """
         Update associated logs for escrow of Out-of-Order event
 
         Parameters:
             serder (SerderKERI): instance of  event
             sigers (list): of Siger instance for  event
             seqner (Seqner): instance of sn of event delegatint/issuing event if any
             saider (Saider): instance of dig of event delegatint/issuing event if any
             wigers (list): of witness signatures
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
         """
+        local = True if local else False
         dgkey = dgKey(serder.preb, serder.saidb)
+        if esr := self.db.esrs.get(keys=dgkey):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
         self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         self.db.putEvt(dgkey, serder.raw)
-        self.db.addOoe(snKey(serder.preb, serder.sn), serder.saidb)
         if wigers:
             self.db.putWigs(dgkey, [siger.qb64b for siger in wigers])
         if seqner and saider:
             couple = seqner.qb64b + saider.qb64b
             self.db.putPde(dgkey, couple)  # idempotent
+        self.db.addOoe(snKey(serder.preb, serder.sn), serder.saidb)
         # log escrowed
         logger.info("Kevery process: escrowed out of order event=\n%s\n",
                     json.dumps(serder.ked, indent=1))
 
     def escrowQueryNotFoundEvent(self, prefixer, serder, sigers, cigars=None):
         """
         Update associated logs for escrow of Out-of-Order event
@@ -4248,23 +4720,37 @@
         for cigar in cigars:
             self.db.addRct(key=dgkey, val=cigar.verfer.qb64b + cigar.qb64b)
 
         # log escrowed
         logger.info("Kevery process: escrowed query not found event=\n%s\n",
                     json.dumps(serder.ked, indent=1))
 
-    def escrowLDEvent(self, serder, sigers):
+    def escrowLDEvent(self, serder, sigers, local=True):
         """
         Update associated logs for escrow of Likely Duplicitous event
 
         Parameters:
             serder is SerderKERI instance of  event
             sigers is list of Siger instance for  event
+            local (bool): event source for validation logic
+                True means event source is local (protected).
+                False means event source is remote (unprotected).
+                Event validation logic is a function of local or remote
         """
+        local = True if local else False
         dgkey = dgKey(serder.preb, serder.saidb)
+        if esr := self.db.esrs.get(keys=dgkey):  # preexisting esr
+            if local and not esr.local:  # local overwrites prexisting remote
+                esr.local = local
+                self.db.esrs.pin(keys=dgkey, val=esr)
+            # otherwise don't change
+        else:  # not preexisting so put
+            esr = basing.EventSourceRecord(local=local)
+            self.db.esrs.put(keys=dgkey, val=esr)
+
         self.db.putDts(dgkey, helping.nowIso8601().encode("utf-8"))
         self.db.putSigs(dgkey, [siger.qb64b for siger in sigers])
         self.db.putEvt(dgkey, serder.raw)
         self.db.addLde(snKey(serder.preb, serder.sn), serder.saidb)
         # log duplicitous
         logger.info("Kevery process: escrowed likely duplicitous event=\n%s\n",
                     json.dumps(serder.ked, indent=1))
@@ -4519,16 +5005,22 @@
         """
 
         key = ekey = b''  # both start same. when not same means escrows found
         while True:  # break when done
             for ekey, edig in self.db.getOoeItemsNextIter(key=key):
                 try:
                     pre, sn = splitKeySN(ekey)  # get pre and sn from escrow item
+                    dgkey = dgKey(pre, bytes(edig))
+                    if not (esr := self.db.esrs.get(keys=dgkey)):  # get event source, otherwise error
+                        # no local sourde so raise ValidationError which unescrows below
+                        raise ValidationError("Missing escrowed event source "
+                                              "at dig = {}.".format(bytes(edig)))
+
                     # check date if expired then remove escrow.
-                    dtb = self.db.getDts(dgKey(pre, bytes(edig)))
+                    dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
                                     " at dig = %s\n", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
@@ -4569,15 +5061,15 @@
                     # process event
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
 
                     #  get wigs
                     wigs = self.db.getWigs(dgKey(pre, bytes(edig)))  # list of wigs
                     wigers = [Siger(qb64b=bytes(wig)) for wig in wigs]
 
-                    self.processEvent(serder=eserder, sigers=sigers, wigers=wigers)
+                    self.processEvent(serder=eserder, sigers=sigers, wigers=wigers, local=esr.local)
 
                     # If process does NOT validate event with sigs, becasue it is
                     # still out of order then process will attempt to re-escrow
                     # and then raise OutOfOrderError (subclass of ValidationError)
                     # so we can distinquish between ValidationErrors that are
                     # re-escrow vs non re-escrow. We want process to be idempotent
                     # with respect to processing events that result in escrow items.
@@ -4654,14 +5146,19 @@
         key = ekey = b''  # both start same. when not same means escrows found
         while True:  # break when done
             for ekey, edig in self.db.getPseItemsNextIter(key=key):
                 eserder = None
                 try:
                     pre, sn = splitKeySN(ekey)  # get pre and sn from escrow item
                     dgkey = dgKey(pre, bytes(edig))
+                    if not (esr := self.db.esrs.get(keys=dgkey)):  # get event source, otherwise error
+                        # no local sourde so raise ValidationError which unescrows below
+                        raise ValidationError("Missing escrowed event source "
+                                              "at dig = {}.".format(bytes(edig)))
+
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
                                     " at dig = %s\n", bytes(edig))
 
@@ -4703,30 +5200,30 @@
                     # seal source (delegator issuer if any)
                     delseqner = delsaider = None
                     couple = self.db.getPde(dgkey)
                     if couple is not None:
                         delseqner, delsaider = deSourceCouple(couple)
                     elif eserder.ked["t"] in (Ilks.dip, Ilks.drt,):
                         if eserder.pre in self.kevers:
-                            delpre = self.kevers[eserder.pre].delegator
+                            delpre = self.kevers[eserder.pre].delpre
                         else:
                             delpre = eserder.ked["di"]
 
                         seal = dict(i=eserder.ked["i"], s=eserder.snh, d=eserder.said)
                         srdr = self.db.findAnchoringSealEvent(pre=delpre, seal=seal)
                         if srdr is not None:
                             delseqner = coring.Seqner(sn=srdr.sn)
                             delsaider = coring.Saider(qb64=srdr.said)
                             couple = delseqner.qb64b + delsaider.qb64b
                             self.db.putPde(dgkey, couple)
 
                     # process event
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
                     self.processEvent(serder=eserder, sigers=sigers,
-                                      delseqner=delseqner, delsaider=delsaider)
+                                      delseqner=delseqner, delsaider=delsaider, local=esr.local)
 
                     # If process does NOT validate sigs or delegation seal (when delegated),
                     # but there is still one valid signature then process will
                     # attempt to re-escrow and then raise MissingSignatureError
                     # or MissingDelegationSealError (subclass of ValidationError)
                     # so we can distinquish between ValidationErrors that are
                     # re-escrow vs non re-escrow. We want process to be idempotent
@@ -4813,16 +5310,22 @@
         """
 
         key = ekey = b''  # both start same. when not same means escrows found
         while True:  # break when done
             for ekey, edig in self.db.getPweItemsNextIter(key=key):
                 try:
                     pre, sn = splitKeySN(ekey)  # get pre and sn from escrow item
+                    dgkey = dgKey(pre, bytes(edig))
+                    if not (esr := self.db.esrs.get(keys=dgkey)):  # get event source, otherwise error
+                        # no local sourde so raise ValidationError which unescrows below
+                        raise ValidationError("Missing escrowed event source "
+                                              "at dig = {}.".format(bytes(edig)))
+
                     # check date if expired then remove escrow.
-                    dtb = self.db.getDts(dgKey(pre, bytes(edig)))
+                    dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
                                     " at dig = %s\n", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
@@ -4881,15 +5384,15 @@
                     # seal source (delegator issuer if any)
                     delseqner = delsaider = None
                     couple = self.db.getPde(dgKey(pre, bytes(edig)))
                     if couple is not None:
                         delseqner, delsaider = deSourceCouple(couple)
 
                     self.processEvent(serder=eserder, sigers=sigers, wigers=wigers,
-                                      delseqner=delseqner, delsaider=delsaider)
+                                      delseqner=delseqner, delsaider=delsaider, local=esr.local)
 
                     # If process does NOT validate wigs then process will attempt
                     # to re-escrow and then raise MissingWitnessSignatureError
                     # (subclass of ValidationError)
                     # so we can distinquish between ValidationErrors that are
                     # re-escrow vs non re-escrow. We want process to be idempotent
                     # with respect to processing events that result in escrow items.
@@ -4982,14 +5485,15 @@
 
         ims = bytearray()
         key = ekey = b''  # both start same. when not same means escrows found
         while True:  # break when done
             for ekey, ecouple in self.db.getUweItemsNextIter(key=key):
                 try:
                     pre, sn = splitKeySN(ekey)  # get pre and sn from escrow db key
+
                     #  get escrowed receipt's rdiger of receipted event and
                     # wiger indexed signature of receipted event
                     rdiger, wiger = deWitnessCouple(ecouple)
 
                     # check date if expired then remove escrow.
                     dtb = self.db.getDts(dgKey(pre, bytes(rdiger.qb64b)))
                     if dtb is None:  # othewise is a datetime as bytes
@@ -5301,15 +5805,21 @@
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     # process event
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
 
-                    #  get wigs
+                    # ToDo XXXX get wigs and attach
+                    # getWigs
+
+                    # ToDo XXXX get trans endorsements
+                    # getVrcs
+
+                    #  get nontrans endorsements
                     cigars = []
                     cigs = self.db.getRcts(dgKey(pre, bytes(edig)))  # list of wigs
                     for cig in cigs:
                         (_, cigar) = deReceiptCouple(cig)
                         cigars.append(cigar)
 
                     source = coring.Prefixer(qb64b=pre)
@@ -5668,16 +6178,22 @@
                         If successful then remove from escrow table
         """
         key = ekey = b''  # both start same. when not same means escrows found
         while True:  # break when done
             for ekey, edig in self.db.getLdeItemsNextIter(key=key):
                 try:
                     pre, sn = splitKeySN(ekey)  # get pre and sn from escrow item
+                    dgkey = dgKey(pre, bytes(edig))
+                    if not (esr := self.db.esrs.get(keys=dgkey)):  # get event source, otherwise error
+                        # no local sourde so raise ValidationError which unescrows below
+                        raise ValidationError("Missing escrowed event source "
+                                              "at dig = {}.".format(bytes(edig)))
+
                     # check date if expired then remove escrow.
-                    dtb = self.db.getDts(dgKey(pre, bytes(edig)))
+                    dtb = self.db.getDts(dgkey)
                     if dtb is None:  # othewise is a datetime as bytes
                         # no date time so raise ValidationError which unescrows below
                         logger.info("Kevery unescrow error: Missing event datetime"
                                     " at dig = %s\n", bytes(edig))
 
                         raise ValidationError("Missing escrowed event datetime "
                                               "at dig = {}.".format(bytes(edig)))
@@ -5712,15 +6228,15 @@
                         logger.info("Kevery unescrow error: Missing event sigs at."
                                     "dig = %s\n", bytes(edig))
 
                         raise ValidationError("Missing escrowed evt sigs at "
                                               "dig = {}.".format(bytes(edig)))
 
                     sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
-                    self.processEvent(serder=eserder, sigers=sigers)
+                    self.processEvent(serder=eserder, sigers=sigers, local=esr.local)
 
                     # If process does NOT validate event with sigs, becasue it is
                     # still out of order then process will attempt to re-escrow
                     # and then raise OutOfOrderError (subclass of ValidationError)
                     # so we can distinquish between ValidationErrors that are
                     # re-escrow vs non re-escrow. We want process to be idempotent
                     # with respect to processing events that result in escrow items.
@@ -5798,27 +6314,27 @@
     if sdig is not None:
         event["stored"] = True
 
     # add indexed signatures to attachments
     sigs = db.getSigs(key=dgkey)
     dsigs = []
     for s in sigs:
-        sig = coring.Siger(qb64b=bytes(s))
+        sig = indexing.Siger(qb64b=bytes(s))
         dsigs.append(dict(index=sig.index, signature=sig.qb64))
     event["signatures"] = dsigs
 
     # add witness state at this event
     wits = db.wits.get(dgkey) if serder.estive else []
     event["witnesses"] = [wit.qb64 for wit in wits]
 
     # add indexed witness signatures to attachments
     dwigs = []
     if wigs := db.getWigs(key=dgkey):
         for w in wigs:
-            sig = coring.Siger(qb64b=bytes(w))
+            sig = indexing.Siger(qb64b=bytes(w))
             dwigs.append(dict(index=sig.index, signature=sig.qb64))
     event["witness_signatures"] = dwigs
 
     # add authorizer (delegator/issuer) source seal event couple to attachments
     couple = db.getAes(dgkey)
     if couple is not None:
         raw = bytearray(couple)
@@ -5832,15 +6348,15 @@
         trans = []
         for quad in quads:
             raw = bytearray(quad)
             trans.append(dict(
                 prefix=coring.Prefixer(qb64b=raw, strip=True).qb64,
                 sequence=coring.Seqner(qb64b=raw, strip=True).qb64,
                 said=coring.Saider(qb64b=raw, strip=True).qb64,
-                signature=coring.Siger(qb64b=raw, strip=True).qb64,
+                signature=indexing.Siger(qb64b=raw, strip=True).qb64,
             ))
 
         receipts["transferable"] = trans
 
     # add nontrans receipts couples
     if coups := db.getRcts(key=dgkey):
         nontrans = []
```

### Comparing `keri-1.1.9/src/keri/core/parsing.py` & `keri-1.2.dev0/src/keri/core/parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,71 +6,25 @@
 """
 
 import logging
 import traceback
 from collections import namedtuple
 from dataclasses import dataclass, astuple
 
-from .coring import (Ilks, CtrDex, Counter, Seqner, Siger, Cigar,
-                     Dater, Verfer, Prefixer, Saider, Pather, Protos )
+from .coring import (Ilks, CtrDex, Counter, Seqner, Cigar,
+                     Dater, Verfer, Prefixer, Saider, Pather, Protocols )
+from .indexing import (Siger, )
 from . import serdering
 from .. import help
 from .. import kering
+from ..kering import ColdDex, Colds, sniff
 
 logger = help.ogler.getLogger()
 
 
-@dataclass(frozen=True)
-class ColdCodex:
-    """
-    ColdCodex is codex of cold stream start tritets of first byte
-    Only provide defined codes.
-    Undefined are left out so that inclusion(exclusion) via 'in' operator works.
-
-    First three bits:
-        0o0 = 000 free
-        0o1 = 001 cntcode B64
-        0o2 = 010 opcode B64
-        0o3 = 011 json
-        0o4 = 100 mgpk
-        0o5 = 101 cbor
-        0o6 = 110 mgpk
-        007 = 111 cntcode or opcode B2
-
-    status is one of ('evt', 'txt', 'bny' )
-    'evt' if tritet in (ColdDex.JSON, ColdDex.MGPK1, ColdDex.CBOR, ColdDex.MGPK2)
-    'txt' if tritet in (ColdDex.CtB64, ColdDex.OpB64)
-    'bny' if tritet in (ColdDex.CtOpB2,)
-
-    otherwise raise ColdStartError
-
-    x = bytearray([0x2d, 0x5f])
-    x == bytearray(b'-_')
-    x[0] >> 5 == 0o1
-    True
-    """
-    Free: int = 0o0  # not taken
-    CtB64: int = 0o1  # CountCode Base64
-    OpB64: int = 0o2  # OpCode Base64
-    JSON: int = 0o3  # JSON Map Event Start
-    MGPK1: int = 0o4  # MGPK Fixed Map Event Start
-    CBOR: int = 0o5  # CBOR Map Event Start
-    MGPK2: int = 0o6  # MGPK Big 16 or 32 Map Event Start
-    CtOpB2: int = 0o7  # CountCode or OpCode Base2
-
-    def __iter__(self):
-        return iter(astuple(self))
-
-
-ColdDex = ColdCodex()  # Make instance
-
-Coldage = namedtuple("Coldage", 'msg txt bny')  # stream cold start status
-Colds = Coldage(msg='msg', txt='txt', bny='bny')
-
-
 class Parser:
     """
     Parser is stream parser that processes an incoming message stream.
     Each message in the stream is composed of a message body with a message foot
     The message body includes a version string. The message foot is composed of
     composable concatenated attachments encoded in CESR (Composable Event
     Streaming Representation)  CESR supports both binary and text formats where
@@ -85,81 +39,51 @@
     Attributes:
         ims (bytearray): incoming message stream
         framed (bool): True means stream is packet framed
         pipeline (bool): True means use pipeline processor to process
                 whenever stream includes pipelined count codes.
         kvy (Kevery): route KEL message types to this instance
         tvy (Tevery): route TEL message types to this instance
+        exc (Exchanger): route EXN message types to this instance
+        rvy (Revery): reply (RPY) message handler
+        vry (Verfifier): credential verifier with wallet storage
+        local (bool): True means event source is local (protected) for validation
+                         False means event source is remote (unprotected) for validation
 
     """
 
-    def __init__(self, ims=None, framed=True, pipeline=False, kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+    def __init__(self, ims=None, framed=True, pipeline=False, kvy=None,
+                 tvy=None, exc=None, rvy=None, vry=None, local=False):
         """
         Initialize instance:
 
         Parameters:
             ims (bytearray): incoming message stream
             framed (bool): True means ims contains only one msg body plus
                 its foot of attachments, not multiple sets of msg body plus foot
             pipeline (bool): True means use pipeline processor to process
                 ims msgs when stream includes pipelined count codes.
             kvy (Kevery): route KEL message types to this instance
             tvy (Tevery): route TEL message types to this instance
             exc (Exchanger): route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
             vry (Verfifier): credential verifier with wallet storage
+            local (bool): True means event source is local (protected) for validation
+                         False means event source is remote (unprotected) for validation
         """
         self.ims = ims if ims is not None else bytearray()
         self.framed = True if framed else False  # extract until end-of-stream
         self.pipeline = True if pipeline else False  # process as pipelined
         self.kvy = kvy
         self.tvy = tvy
         self.exc = exc
         self.rvy = rvy
         self.vry = vry
+        self.local = True if local else False
 
-    @staticmethod
-    def sniff(ims):
-        """
-        Returns status string of cold start of stream ims bytearray by looking
-        at first triplet of first byte to determin if message or counter code
-        and if counter code whether Base64 or Base2 representation
-
-        First three bits:
-        0o0 = 000 free
-        0o1 = 001 cntcode B64
-        0o2 = 010 opcode B64
-        0o3 = 011 json
-        0o4 = 100 mgpk
-        0o5 = 101 cbor
-        0o6 = 110 mgpk
-        007 = 111 cntcode or opcode B2
-
-        counter B64 in (0o1, 0o2) return 'txt'
-        counter B2 in (0o7)  return 'bny'
-        event in (0o3, 0o4, 0o5, 0o6)  return 'evt'
-        unexpected in (0o0)  raise ColdStartError
-        Colds = Coldage(msg='msg', txt='txt', bny='bny')
-
-        'msg' if tritet in (ColdDex.JSON, ColdDex.MGPK1, ColdDex.CBOR, ColdDex.MGPK2)
-        'txt' if tritet in (ColdDex.CtB64, ColdDex.OpB64)
-        'bny' if tritet in (ColdDex.CtOpB2,)
-        """
-        if not ims:
-            raise kering.ShortageError("Need more bytes.")
-
-        tritet = ims[0] >> 5
-        if tritet in (ColdDex.JSON, ColdDex.MGPK1, ColdDex.CBOR, ColdDex.MGPK2):
-            return Colds.msg
-        if tritet in (ColdDex.CtB64, ColdDex.OpB64):
-            return Colds.txt
-        if tritet in (ColdDex.CtOpB2,):
-            return Colds.bny
-
-        raise kering.ColdStartError("Unexpected tritet={} at stream start.".format(tritet))
 
     @staticmethod
     def extract(ims, klas, cold=Colds.txt):
         """
         Extract and return instance of klas from input message stream, ims, given
         stream state, cold, is txt or bny. Inits klas from ims using qb64b or
         qb2 parameter based on cold.
@@ -167,14 +91,15 @@
         if cold == Colds.txt:
             return klas(qb64b=ims, strip=True)
         elif cold == Colds.bny:
             return klas(qb2=ims, strip=True)
         else:
             raise kering.ColdStartError("Invalid stream state cold={}.".format(cold))
 
+
     @staticmethod
     def _extractor(ims, klas, cold=Colds.txt, abort=False):
         """
         Returns generator to extract and return instance of klas from input
         message stream, ims, given stream state, cold, is txt or bny.
         If wait is True then yield when not enough bytes in stream otherwise
         raise ShortageError
@@ -194,14 +119,15 @@
                 else:
                     raise kering.ColdStartError("Invalid stream state cold={}.".format(cold))
             except kering.ShortageError as ex:
                 if abort:  # pipelined pre-collects full frame before extracting
                     raise  # bad pipelined frame so abort by raising error
                 yield
 
+
     def _sadPathSigGroup(self, ctr, ims, root=None, cold=Colds.txt, pipelined=False):
         """
 
         Args:
             ctr (Counter): group type counter
             ims (bytearray) of serialized incoming message stream.
                 May contain one or more sets each of a serialized message with
@@ -210,15 +136,15 @@
             cold (str): next charater Coldage type indicayor
             pipelined (bool) True means use pipeline processor to process
                 ims msgs when stream includes pipelined count codes.
 
         Returns:
 
         """
-        if ctr.code != CtrDex.SadPathSig:
+        if ctr.code != CtrDex.SadPathSigGroups:
             raise kering.UnexpectedCountCodeError("Wrong "
                                                   "count code={}.Expected code={}."
                                                   "".format(ctr.code, CtrDex.ControllerIdxSigs))
 
         subpath = yield from self._extractor(ims,
                                              klas=Pather,
                                              cold=cold,
@@ -246,14 +172,15 @@
             for cigar in self._nonTransReceiptCouples(ctr=sctr, ims=ims, cold=cold, pipelined=pipelined):
                 yield sctr.code, (subpath, cigar)
         else:
             raise kering.UnexpectedCountCodeError("Wrong "
                                                   "count code={}.Expected code={}."
                                                   "".format(ctr.code, CtrDex.ControllerIdxSigs))
 
+
     def _transIdxSigGroups(self, ctr, ims, cold=Colds.txt, pipelined=False):
         """
         Extract attaced trans indexed sig groups each made of
         triple pre+snu+dig plus indexed sig group
         pre is pre of signer (endorser) of msg
         snu is sn of signer's est evt when signed
         dig is dig of signer's est event when signed
@@ -300,14 +227,15 @@
                                                     klas=Siger,
                                                     cold=cold,
                                                     abort=pipelined)
                 isigers.append(isiger)
 
             yield prefixer, seqner, saider, isigers
 
+
     def _nonTransReceiptCouples(self, ctr, ims, cold=Colds.txt, pipelined=False):
         """
         Extract attached rct couplets into list of sigvers
         verfer property of cigar is the identifier prefix
         cigar itself has the attached signature
 
         Parameters:
@@ -332,15 +260,17 @@
                                                klas=Cigar,
                                                cold=cold,
                                                abort=pipelined)
             cigar.verfer = verfer
 
             yield cigar
 
-    def parse(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+
+    def parse(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None,
+              exc=None, rvy=None, vry=None, local=None):
         """
         Processes all messages from incoming message stream, ims,
         when provided. Otherwise process messages from .ims
         Returns when ims is empty.
         Convenience executor for .processAllGen when ims is not live, i.e. fixed
 
         Parameters:
@@ -355,35 +285,45 @@
                 ims msgs when stream incpyludes pipelined count codes.
 
             kvy (Kevery): route KERI KEL message types to this instance
             tvy (Tevery): route TEL message types to this instance
             exc (Exchanger) route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
             vry (Verfifier): credential verifier with wallet storage
+            local (bool): True means event source is local (protected) for validation
+                          False means event source is remote (unprotected) for validation
+                          None means use default .local
 
         New Logic:
             Attachments must all have counters so know if txt or bny format for
             attachments. So even when framed==True must still have counters.
         """
+        local = local if local is not None else self.local
+        local = True if local else False
+
+
         parsator = self.allParsator(ims=ims,
                                     framed=framed,
                                     pipeline=pipeline,
                                     kvy=kvy,
                                     tvy=tvy,
                                     exc=exc,
                                     rvy=rvy,
-                                    vry=vry)
+                                    vry=vry,
+                                    local=local)
 
         while True:
             try:
                 next(parsator)
             except StopIteration:
                 break
 
-    def parseOne(self, ims=None, framed=True, pipeline=False, kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+
+    def parseOne(self, ims=None, framed=True, pipeline=False, kvy=None, tvy=None,
+                 exc=None, rvy=None, vry=None, local=None):
         """
         Processes one messages from incoming message stream, ims,
         when provided. Otherwise process message from .ims
         Returns once one message is processed.
         Convenience executor for .processOneGen when ims is not live, i.e. fixed
 
         Parameters:
@@ -397,34 +337,43 @@
             pipeline is Boolean, True means use pipeline processor to process
                 ims msgs when stream includes pipelined count codes.
 
             kvy (Kevery): route KERI KEL message types to this instance
             tvy (Tevery): route TEL message types to this instance
             exc (Exchanger) route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
+            local (bool): True means event source is local (protected) for validation
+                          False means event source is remote (unprotected) for validation
+                          None means use default .local
 
         New Logic:
             Attachments must all have counters so know if txt or bny format for
             attachments. So even when framed==True must still have counters.
         """
+        local = local if local is not None else self.local
+        local = True if local else False
+
         parsator = self.onceParsator(ims=ims,
                                      framed=framed,
                                      pipeline=pipeline,
                                      kvy=kvy,
                                      tvy=tvy,
                                      exc=exc,
                                      rvy=rvy,
-                                     vry=vry)
+                                     vry=vry,
+                                     local=local)
         while True:
             try:
                 next(parsator)
             except StopIteration:
                 break
 
-    def allParsator(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+
+    def allParsator(self, ims=None, framed=None, pipeline=None, kvy=None,
+                    tvy=None, exc=None, rvy=None, vry=None, local=None):
         """
         Returns generator to parse all messages from incoming message stream,
         ims until ims is exhausted (empty) then returns.
         Generator completes as soon as ims is empty.
         If ims not provided then parse messages from .ims
 
         Parameters:
@@ -439,14 +388,17 @@
                 ims msgs when stream includes pipelined count codes.
 
             kvy (Kevery): route KERI KEL message types to this instance
             tvy (Tevery): route TEL message types to this instance
             exc (Exchanger) route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
             vry (Verfifier): credential verifier with wallet storage
+            local (bool): True means event source is local (protected) for validation
+                          False means event source is remote (unprotected) for validation
+                          None means use default .local
 
         New Logic:
             Attachments must all have counters so know if txt or bny format for
             attachments. So even when framed==True must still have counters.
         """
         if ims is not None:  # needs bytearray not bytes since deletes as processes
             if not isinstance(ims, bytearray):
@@ -457,25 +409,28 @@
         framed = framed if framed is not None else self.framed
         pipeline = pipeline if pipeline is not None else self.pipeline
         kvy = kvy if kvy is not None else self.kvy
         tvy = tvy if tvy is not None else self.tvy
         exc = exc if exc is not None else self.exc
         rvy = rvy if rvy is not None else self.rvy
         vry = vry if vry is not None else self.vry
+        local = local if local is not None else self.local
+        local = True if local else False
 
         while ims:  # only process until ims empty
             try:
                 done = yield from self.msgParsator(ims=ims,
                                                    framed=framed,
                                                    pipeline=pipeline,
                                                    kvy=kvy,
                                                    tvy=tvy,
                                                    exc=exc,
                                                    rvy=rvy,
-                                                   vry=vry)
+                                                   vry=vry,
+                                                   local=local)
 
             except kering.SizedGroupError as ex:  # error inside sized group
                 # processOneIter already flushed group so do not flush stream
                 if logger.isEnabledFor(logging.ERROR):
                     logger.exception("Parser msg extraction error: %s\n", ex.args[0])
                 else:
                     logger.error("Parser msg extraction error: %s\n", ex.args[0])
@@ -494,15 +449,17 @@
                     logger.exception("Parser msg non-extraction error: %s\n", ex)
                 else:
                     logger.error("Parser msg non-extraction error: %s\n", ex)
             yield
 
         return True
 
-    def onceParsator(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+
+    def onceParsator(self, ims=None, framed=None, pipeline=None, kvy=None,
+                     tvy=None, exc=None, rvy=None, vry=None, local=None):
         """
         Returns generator to parse one message from incoming message stream, ims.
         If ims not provided parse messages from .ims
 
         Parameters:
             ims is bytearray of incoming message stream. May contain one or more
                 sets each of a serialized message with attached cryptographic
@@ -515,14 +472,17 @@
                 ims msgs when stream includes pipelined count codes.
 
             kvy (Kevery): route KERI KEL message types to this instance
             tvy (Tevery): route TEL message types to this instance
             exc (Exchanger) route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
             vry (Verfifier): credential verifier with wallet storage
+            local (bool): True means event source is local (protected) for validation
+                          False means event source is remote (unprotected) for validation
+                          None means use default .local
 
         New Logic:
             Attachments must all have counters so know if txt or bny format for
             attachments. So even when framed==True must still have counters.
         """
         if ims is not None:  # needs bytearray not bytes since deletes as processes
             if not isinstance(ims, bytearray):
@@ -533,26 +493,29 @@
         framed = framed if framed is not None else self.framed
         pipeline = pipeline if pipeline is not None else self.pipeline
         kvy = kvy if kvy is not None else self.kvy
         tvy = tvy if tvy is not None else self.tvy
         exc = exc if exc is not None else self.exc
         rvy = rvy if rvy is not None else self.rvy
         vry = vry if vry is not None else self.vry
+        local = local if local is not None else self.local
+        local = True if local else False
 
         done = False
         while not done:
             try:
                 done = yield from self.msgParsator(ims=ims,
                                                    framed=framed,
                                                    pipeline=pipeline,
                                                    kvy=kvy,
                                                    tvy=tvy,
                                                    exc=exc,
                                                    rvy=rvy,
-                                                   vry=vry)
+                                                   vry=vry,
+                                                   local=local)
 
             except kering.SizedGroupError as ex:  # error inside sized group
                 # processOneIter already flushed group so do not flush stream
                 if logger.isEnabledFor(logging.ERROR):
                     logger.exception("Kevery msg extraction error: %s\n", ex.args[0])
                 else:
                     logger.error("Kevery msg extraction error: %s\n", ex.args[0])
@@ -572,21 +535,23 @@
                 else:
                     logger.error("Kevery msg non-extraction error: %s\n", ex.args[0])
             finally:
                 done = True
 
         return done
 
-    def parsator(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+
+    def parsator(self, ims=None, framed=None, pipeline=None, kvy=None, tvy=None,
+                 exc=None, rvy=None, vry=None, local=None):
         """
         Returns generator to continually parse messages from incoming message
-        stream, ims. Empty yields when ims is emply.
+        stream, ims. Empty yields when ims is emply. Does not return.
         Useful for always running servers.
         One yield from per each message if any.
-        Continually yields while ims is empty.
+        Continually yields while ims is empty, i.e. does not return.
         If ims not provided then parse messages from .ims
 
         Parameters:
             ims is bytearray of incoming message stream. May contain one or more
                 sets each of a serialized message with attached cryptographic
                 material such as signatures or receipts.
 
@@ -597,14 +562,18 @@
                 ims msgs when stream includes pipelined count codes.
 
             kvy (Kevery): route KERI KEL message types to this instance
             tvy (Tevery): route TEL message types to this instance
             exc (Exchanger) route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
             vry (Verifier): credential processor
+            local (bool): True means event source is local (protected) for validation
+                          False means event source is remote (unprotected) for validation
+                          None means use default .local
+
 
         New Logic:
             Attachments must all have counters so know if txt or bny format for
             attachments. So even when framed==True must still have counters.
         """
         if ims is not None:  # needs bytearray not bytes since deletes as processes
             if not isinstance(ims, bytearray):
@@ -615,25 +584,28 @@
         framed = framed if framed is not None else self.framed
         pipeline = pipeline if pipeline is not None else self.pipeline
         kvy = kvy if kvy is not None else self.kvy
         tvy = tvy if tvy is not None else self.tvy
         exc = exc if exc is not None else self.exc
         rvy = rvy if rvy is not None else self.rvy
         vry = vry if vry is not None else self.vry
+        local = local if local is not None else self.local
+        local = True if local else False
 
         while True:  # continuous stream processing never stop
             try:
                 done = yield from self.msgParsator(ims=ims,
                                                    framed=framed,
                                                    pipeline=pipeline,
                                                    kvy=kvy,
                                                    tvy=tvy,
                                                    exc=exc,
                                                    rvy=rvy,
-                                                   vry=vry)
+                                                   vry=vry,
+                                                   local=local)
 
             except kering.SizedGroupError as ex:  # error inside sized group
                 # processOneIter already flushed group so do not flush stream
                 if logger.isEnabledFor(logging.ERROR):
                     logger.exception("Parser msg extraction error: %s\n", ex.args[0])
                 else:
                     logger.error("Parser msg extraction error: %s\n", ex.args[0])
@@ -654,15 +626,15 @@
                     logger.error("Parser msg non-extraction error: %s\n", ex.args[0])
             yield
 
         return True  # should never return
 
 
     def msgParsator(self, ims=None, framed=True, pipeline=False,
-                    kvy=None, tvy=None, exc=None, rvy=None, vry=None):
+                    kvy=None, tvy=None, exc=None, rvy=None, vry=None, local=None):
         """
         Returns generator that upon each iteration extracts and parses msg
         with attached crypto material (signature etc) from incoming message
         stream, ims, and dispatches processing of message with attachments.
 
         Uses .ims when ims is not provided.
 
@@ -681,14 +653,17 @@
                 ims msgs when stream includes pipelined count codes.
 
             kvy (Kevery) route KERI KEL message types to this instance
             tvy (Tevery) route TEL message types to this instance
             exc (Exchanger) route EXN message types to this instance
             rvy (Revery): reply (RPY) message handler
             vry (Verifier) ACDC credential processor
+            local (bool): True means event source is local (protected) for validation
+                          False means event source is remote (unprotected) for validation
+                          None means use default .local
 
         Logic:
             Currently only support couters on attachments not on combined or
             on message
             Attachments must all have counters so know if txt or bny format for
             attachments. So even when framed==True must still have counter.
             Do While loop
@@ -699,47 +674,40 @@
                sniff for counter
                if group counter extract and discard but keep track of count
                so if error while processing attachments then only need to flush
                attachment count not full stream.
 
 
         """
+        local = local if local is not None else self.local
+        local = True if local else False
+
         serdery = serdering.Serdery(version=kering.Version)
 
         if ims is None:
             ims = self.ims
 
         while not ims:
             yield
 
-        cold = self.sniff(ims)  # check for spurious counters at front of stream
+        cold = sniff(ims)  # check for spurious counters at front of stream
         if cold in (Colds.txt, Colds.bny):  # not message error out to flush stream
             # replace with pipelining here once CESR message format supported.
             raise kering.ColdStartError("Expecting message counter tritet={}"
                                         "".format(cold))
         # Otherwise its a message cold start
 
         while True:  # extract, deserialize, and strip message from ims
             try:
                 serder = serdery.reap(ims=ims)  # can set version here
             except kering.ShortageError as ex:  # need more bytes
                 yield
             else: # extracted and stripped successfully
                 break  # break out of while loop
 
-
-        #while True:  # extract and deserialize message from ims
-            #try:
-                #sadder = Sadder(raw=ims)
-            #except kering.ShortageError as ex:  # need more bytes
-                #yield
-            #else:  # extracted successfully
-                #del ims[:sadder.size]  # strip off event from front of ims
-                #break
-
         sigers = []  # list of Siger instances of attached indexed controller signatures
         wigers = []  # list of Siger instance of attached indexed witness signatures
         cigars = []  # List of cigars to hold nontrans rct couplets
         # List of tuples from extracted transferable receipt (vrc) quadruples
         trqs = []  # each converted quadruple is (prefixer, seqner, diger, siger)
         # List of tuples from extracted transferable indexed sig groups
         tsgs = []  # each converted group is tuple of (i,s,d) triple plus list of sigs
@@ -758,18 +726,18 @@
         pathed = []  # grouped attachments targetting a subpath
         pipelined = False  # all attachments in one big pipeline counted group
         # extract and deserialize attachments
         try:  # catch errors here to flush only counted part of stream
             # extract attachments must start with counter so know if txt or bny.
             while not ims:
                 yield
-            cold = self.sniff(ims)  # expect counter at front of attachments
+            cold = sniff(ims)  # expect counter at front of attachments
             if cold != Colds.msg:  # not new message so process attachments
                 ctr = yield from self._extractor(ims=ims, klas=Counter, cold=cold)
-                if ctr.code == CtrDex.AttachedMaterialQuadlets:  # pipeline ctr?
+                if ctr.code == CtrDex.AttachmentGroup:  # pipeline ctr?
                     pipelined = True
                     # compute pipelined attached group size based on txt or bny
                     pags = ctr.count * 4 if cold == Colds.txt else ctr.count * 3
                     while len(ims) < pags:  # wait until rx full pipelned group
                         yield
 
                     pims = ims[:pags]  # copy out substream pipeline group
@@ -930,15 +898,15 @@
                                                                 abort=pipelined)
                             saider = yield from self._extractor(ims,
                                                                 klas=Saider,
                                                                 cold=cold,
                                                                 abort=pipelined)
                             ssts.append((prefixer, seqner, saider))
 
-                    elif ctr.code == CtrDex.SadPathSigGroup:
+                    elif ctr.code == CtrDex.SadPathSigGroups:
                         path = yield from self._extractor(ims,
                                                           klas=Pather,
                                                           cold=cold,
                                                           abort=pipelined)
                         for i in range(ctr.count):
                             ictr = yield from self._extractor(ims=ims,
                                                               klas=Counter,
@@ -950,25 +918,25 @@
                                                                     cold=cold,
                                                                     pipelined=pipelined):
                                 if code == CtrDex.TransIdxSigGroups:
                                     sadtsgs.append(sigs)
                                 else:
                                     sadcigs.append(sigs)
 
-                    elif ctr.code == CtrDex.SadPathSig:
+                    elif ctr.code == CtrDex.SadPathSigGroups:
                         for code, sigs in self._sadPathSigGroup(ctr=ctr,
                                                                 ims=ims,
                                                                 cold=cold,
                                                                 pipelined=pipelined):
                             if code == CtrDex.TransIdxSigGroups:
                                 sadtsgs.append(sigs)
                             else:
                                 sadcigs.append(sigs)
 
-                    elif ctr.code == CtrDex.PathedMaterialQuadlets:  # pathed ctr?
+                    elif ctr.code == CtrDex.PathedMaterialGroup:  # pathed ctr?
                         # compute pipelined attached group size based on txt or bny
                         pags = ctr.count * 4 if cold == Colds.txt else ctr.count * 3
                         while len(ims) < pags:  # wait until rx full pipelned group
                             yield
 
                         pims = ims[:pags]  # copy out substream pipeline group
                         del ims[:pags]  # strip off from ims
@@ -983,81 +951,82 @@
                             break
 
                     elif framed:
                         # because not all in one pipeline group, each attachment
                         # group may switch stream state txt or bny
                         if not ims:  # end of frame
                             break
-                        cold = self.sniff(ims)
+                        cold = sniff(ims)
                         if cold == Colds.msg:  # new message so attachments done
                             break  # finished attachments since new message
                     else:  # process until next message
                         # because not all in one pipeline group, each attachment
                         # group may switch stream state txt or bny
                         while not ims:
                             yield  # no frame so must wait for next message
-                        cold = self.sniff(ims)  # ctr or msg
+                        cold = sniff(ims)  # ctr or msg
                         if cold == Colds.msg:  # new message
                             break  # finished attachments since new message
 
                     ctr = yield from self._extractor(ims=ims, klas=Counter, cold=cold)
 
         except kering.ExtractionError as ex:
             if pipelined:  # extracted pipelined group is preflushed
                 raise kering.SizedGroupError("Error processing pipelined size"
                                              "attachment group of size={}.".format(pags))
             raise  # no pipeline group so can't preflush, must flush stream
 
         if isinstance(serder, serdering.SerderKERI):
             ilk = serder.ilk  # dispatch abased on ilk
 
-        #if sadder.proto == Protos.keri:
-            #serder = Serder(sad=sadder)
-
-            #ilk = serder.ked["t"]  # dispatch abased on ilk
-
             if ilk in [Ilks.icp, Ilks.rot, Ilks.ixn, Ilks.dip, Ilks.drt]:  # event msg
                 firner, dater = frcs[-1] if frcs else (None, None)  # use last one if more than one
                 # when present assumes this is source seal of delegating event in delegator's KEL
                 delseqner, delsaider = sscs[-1] if sscs else (None, None)  # use last one if more than one
                 if not sigers:
                     raise kering.ValidationError("Missing attached signature(s) for evt "
                                                  "= {}.".format(serder.ked))
                 try:
                     kvy.processEvent(serder=serder,
                                      sigers=sigers,
                                      wigers=wigers,
                                      delseqner=delseqner,
                                      delsaider=delsaider,
                                      firner=firner,
-                                     dater=dater)
+                                     dater=dater,
+                                     local=local)
 
                     if cigars:
-                        kvy.processReceiptCouples(serder, cigars, firner=firner)
+                        kvy.processAttachedReceiptCouples(serder, cigars,
+                                                    firner=firner, local=local)
                     if trqs:
-                        kvy.processReceiptQuadruples(serder, trqs, firner=firner)
+                        kvy.processAttachedReceiptQuadruples(serder, trqs,
+                                                    firner=firner, local=local)
 
                 except AttributeError as ex:
                     raise kering.ValidationError("No kevery to process so dropped msg"
                                                  "= {}.".format(serder.pretty())) from ex
 
             elif ilk in [Ilks.rct]:  # event receipt msg (nontransferable)
                 if not (cigars or wigers or tsgs):
                     raise kering.ValidationError("Missing attached signatures on receipt"
                                                  "msg = {}.".format(serder.ked))
 
                 try:
                     if cigars:
-                        kvy.processReceipt(serder=serder, cigars=cigars)
+                        kvy.processReceipt(serder=serder, cigars=cigars,
+                                           local=local)
 
                     if wigers:
-                        kvy.processReceiptWitness(serder=serder, wigers=wigers)
+                        kvy.processReceiptWitness(serder=serder, wigers=wigers,
+                                                  local=local)
 
                     if tsgs:
-                        kvy.processReceiptTrans(serder=serder, tsgs=tsgs)
+                        kvy.processReceiptTrans(serder=serder, tsgs=tsgs,
+                                                local=local)
 
                 except AttributeError:
                     raise kering.ValidationError("No kevery to process so dropped msg"
                                                  "= {}.".format(serder.pretty()))
 
             elif ilk in (Ilks.rpy,):  # reply message
                 if not (cigars or tsgs):
```

### Comparing `keri-1.1.9/src/keri/core/routing.py` & `keri-1.2.dev0/src/keri/core/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,29 +179,30 @@
 
          If nontrans and last Est Evt is not yet accepted then escrow.
          If nontrans and partially signed then escrow.
 
          Escrow process logic is route dependent and is dispatched by route,
          i.e. route is address of buffer with route specific handler of escrow.
         """
-        for k in eventing.RPY_LABELS:
-            if k not in serder.ked:
-                raise kering.ValidationError(f"Missing element={k} from {coring.Ilks.rpy}"
-                                             f" msg={serder.ked}.")
+        #for k in eventing.RPY_LABELS:
+            #if k not in serder.ked:
+                #raise kering.ValidationError(f"Missing element={k} from {coring.Ilks.rpy}"
+                                             #f" msg={serder.ked}.")
         # fetch from serder to process
         ked = serder.ked
 
         # verify said of reply
         saider = coring.Saider(qb64=ked["d"])
         if not saider.verify(sad=ked, prefixed=True):
             raise kering.ValidationError(f"Invalid said = {saider.qb64} for reply "
                                          f"msg={ked}.")
 
         self.rtr.dispatch(serder=serder, saider=saider, cigars=cigars, tsgs=tsgs)
 
+
     def acceptReply(self, serder, saider, route, aid, osaider=None,
                     cigars=None, tsgs=None):
         """ Applies Best Available Data Acceptance policy to reply and signatures
 
         Returns:
             bool: True is successfully accepted. False otherwise
```

### Comparing `keri-1.1.9/src/keri/core/scheming.py` & `keri-1.2.dev0/src/keri/core/scheming.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/core/serdering.py` & `keri-1.2.dev0/src/keri/core/serdering.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,111 +1,246 @@
-# -*- encoding: utf-8 -*-
+# -*- coding: utf-8 -*-
 """
 keri.core.serdering module
 
 """
 import copy
 import json
 from collections import namedtuple
+from collections.abc import Mapping
+from dataclasses import dataclass, asdict, field
 
 import cbor2 as cbor
 import msgpack
 import pysodium
 import blake3
 import hashlib
+from  ordered_set import OrderedSet as oset
+
 
 from .. import kering
-from ..kering import (ValidationError,  MissingFieldError,
+from ..kering import (ValidationError,  MissingFieldError, ExtraFieldError,
+                      AlternateFieldError,
                       ShortageError, VersionError, ProtocolError, KindError,
                       DeserializeError, FieldError, SerializeError)
-from ..kering import (Versionage, Version, Vrsn_1_0, Vrsn_1_1,
-                      VERRAWSIZE, VERFMT, VERFULLSIZE)
-from ..kering import Protos, Serials, Rever, versify, deversify, Ilks
+from ..kering import (Versionage, Version, Vrsn_1_0, Vrsn_2_0,
+                      VERRAWSIZE, VERFMT,
+                      MAXVERFULLSPAN, VER1FULLSPAN,  VER2FULLSPAN)
+from ..kering import SMELLSIZE, Smellage, smell
+
+from ..kering import Protocols, Serials, Rever, versify, deversify, Ilks
 from ..core import coring
 from .coring import MtrDex, DigDex, PreDex, Saids,  Digestage
-from .coring import Matter, Saider, Verfer, Diger, Number, Tholder
+from .coring import (Matter, Saider, Verfer, Diger, Number, Tholder, Tagger,
+                     Ilker, Traitor, Verser, )
+
+from ..core import counting
+from ..core.counting import GenDex, AllTags, Counter
 
 from .. import help
 from ..help import helping
+from ..help.helping import nonStringSequence
 
 logger = help.ogler.getLogger()
 
-"""
-Fieldage
-    saids (dict): keyed by saidive field labels with values as default codes
-    alls (dict): keyed by all field labels including saidive ones
-                   with values as default codes
-
-Example:
-    Fields = Labelage(saids={'d': DigDex.Blake3_256},
-                      alls={'v': '','d':''})
-"""
-Fieldage = namedtuple("Fieldage", "saids alls")  #values are dicts
 
 
-"""
-Reapage
-    proto (str): protocol type value of Protos examples 'KERI', 'ACDC'
-    major (str): single char hex string of major version number
-    minor (str): single char hex string of minor version number
-    kind (str): serialization value of Serials examples 'JSON', 'CBOR', 'MGPK'
+
+@dataclass
+class FieldDom:
+    """
+    Field configuration dataclass for Serder messages. Provides field labels
+    and default field values for a given ilk (message type).
+
+    Attributes:
+        alls (dict): Allowed fields (not extra)
+                    alls must not be empty since at least version string
+                    or protocol version filed is always required.
+                    Fields in alls that appear must appear in order.
+
+        opts (dict): Optional fields within alls.
+                    opts defaults to empty.
+                    When opts is empty than all alls are required.
+                    Any fields in alls but not in opts are required.
+                    opts is a subset of alls
+
+        alts (dict): Alternate fields within alls.
+                    alts defaults to empty.
+                    An alt field means that one or the other of two fields is
+                    allowed but not both. Two entries in alts are required, one
+                    for each field in an alt pair. the alt pair key value are
+                    the two labels. One entry for each order.
+                    all alts must be in opts since both can't be required.
+                    Suppose 'a' and 'A' are an alternate pair then alts =
+                    { 'a': 'A', 'A': 'a'}. This allows the presence of one to
+                    block the presence of the other by looking up the one present
+                    as key to see the value of the one to block.
+
+        saids (dict): are saidive fields whose value may be computed as a said of the message.
+                    saids defaults to empty
+                    when provided a field in saids indicates the field value is saidive.
+                    A simple SAID field value is always computed.
+                    An AID SAID field value is only computed when its code indicates.
+                    saids is a subset of alls
+
+        strict (bool): determines if alls is strict, no extra fields are allowed
+                       strict defaults to True.
+                       True means no extra fields are allowed, only those in alls.
+                       False means extra fields are allowed besides thos in alls.
+                       Extra fields are fields not in alls.
+                       Extra fields may appear in any order after the last field
+                       in alls.
+
+
+        When strict:  no extras allowed
+           Any fields not in alls raise error
+           If opts is empty then all alls are required in order
+           If opts is not empty then fields in opts are optional but the rest of
+                the fields in alls are required
+
+        When not strict: extras allowed
+           Any fields not in alls must appear after all fields in alls
+           If opts is empty then all alls are required in order
+           If opts is not empty then fields in opts are optional but the rest of
+                the fields in alls are required
+
+    """
+    alls: dict  # all allowed fields when strict
+    opts: dict = field(default_factory=dict)  # optional fields
+    alts:  dict = field(default_factory=dict)  # alternate optional fields
+    saids: dict = field(default_factory=dict)  # saidive fields
+    strict: bool = True  # only alls allowed no extras
+
+    def __iter__(self):
+        return iter(asdict(self))
+
+"""Design Notes:
+
+Problems is that sniff only determines if counter not which type of
+counter. Then smell does regex lookahead to find out which serialization
+when not count code but extractor does not look ahead but strips from
+stream. So when possibility that CESR message is next either need to
+not strip from stream when extracting or if counter is message
+then grab rest of frame and reattach so raw in Serder includes the
+message counter. Latter is better since always keep counter around
+until later. So need to check counter type and if message then
+extract rest of counter frame (message) and reattach counter raw.
+Then can call Serder with raw and smellage that indicates CESR kind
+
+But this does not solve the problem of using the Serder subclass
+for the given protocol. Merely knowing is a CESR message is not
+enough also have to know the protocol which comes in the version
+field (not version string).
+
+One solution is to modify smell so that it also can lookahead and
+see the version field. Or lookahead and see the version field with
+count codes in front. Problem is that the Regexes don't separate
+cleanly.
+
+Another solution is to use distinct function for cesr native called
+snuff like smell but regex only for CESR native. Reap can be told which
+because sniff tells which it is.
+So question for snuff is should it be searching over the counter or should it
+start at version field. This changes regex so forced start at front of raw.
+so if reattach counter but use skip then can snuff at start of string.
+Begine regex with b'^' or b'\A' to match at start of string.
+
+So change Smellage to return extra field that has gvrsn when used by snuff
+so can use Smellage for both smell and snuff in both reap and inhale
+where smellage is used. Change egacy uses of smell to ignore extra value.
+
+
+
+Lets try that as it works the best.
+
+while True:  # extract, deserialize, and strip message from ims
+    try:
+        serder = serdery.reap(ims=ims)  # can set version here
+    except kering.ShortageError as ex:  # need more bytes
+        yield
+    else: # extracted and stripped successfully
+        break  # break out of while loop
+
+ctr = yield from self._extractor(ims=ims, klas=Counter, cold=cold)
+if ctr.code == CtrDex.AttachmentGroup:  # pipeline ctr?
+    pipelined = True
+
+@staticmethod
+def _extractor(ims, klas, cold=Colds.txt, abort=False):
+    while True:
+        try:
+            if cold == Colds.txt:
+                return klas(qb64b=ims, strip=True)
+            elif cold == Colds.bny:
+                return klas(qb2=ims, strip=True)
+            else:
+                raise kering.ColdStartError("Invalid stream state cold={}.".format(cold))
+        except kering.ShortageError as ex:
+            if abort:  # pipelined pre-collects full frame before extracting
+                raise  # bad pipelined frame so abort by raising error
+            yield
+
+
 
 """
-Reapage = namedtuple("Reapage", "proto major minor kind size")
 
 
 class Serdery:
     """Serder factory class for generating serder instances by protocol type
     from an incoming message stream.
-
-
     """
 
-    def __init__(self, *, version=None):
+    def __init__(self, *pa, **kwa):
         """Init instance
 
         Parameters:
-            version (Versionage | None): instance supported protocol version
-                     None means do not enforce a supported version
+
         """
-        self.version = version  # default version
+        pass
 
 
-    def reap(self, ims, *, version=None):
+    def reap(self, ims, genus=GenDex.KERI, gvrsn=Vrsn_2_0, native=False, skip=0):
         """Extract and return Serder subclass based on protocol type reaped from
         version string inside serialized raw of Serder.
 
         Returns:
             serder (Serder): instance of Serder subclass where subclass is
                 determined by the protocol type of its version string.
 
         Parameters:
             ims (bytearray) of serialized incoming message stream. Assumes start
                 of stream is raw Serder.
-            version (Versionage | None): instance supported protocol version
-                None means do not enforce a supported version
-        """
-        version = version if version is not None else self.version
-
-        if len(ims) < Serder.InhaleSize:
-            raise ShortageError(f"Need more raw bytes for Serdery to reap.")
+            genus (str): CESR genus code from stream parser.
+                    Provides genus of enclosing stream top-level or nested group
+            gvrsn (Versionage): instance CESR genus code table version (Major, Minor)
+                    Provides genus of enclosing stream top-level or nested group
+            native (bool): True means sniff determined may be CESR native message
+                           so snuff instead of smell.
+                           False means sniff determined not CESR native i.e
+                           JSON, CBOR, MGPK field map. so use smell. Default False
+             skip (int): bytes to skip at front of ims. Useful when CESR native
+                serialization where skip is size of the message counter so smell
+                does need to see counter
+
+        """
+        if native:
+            pass
+            #smellage = smell(memoryview(ims)[skip:])  # does not copy to skip
 
-        match = Rever.search(ims)  # Rever regex takes bytes/bytearray not str
-        if not match or match.start() > Serder.MaxVSOffset:
-            raise VersionError(f"Invalid version string for Serder raw = "
-                               f"{ims[: Serder.InhaleSize]}.")
-
-        reaped = Reapage(*match.group("proto", "major", "minor", "kind", "size"))
+        else:
+            smellage = smell(ims)
 
-        if reaped.proto == Protos.keri.encode("utf-8"):
-            return SerderKERI(raw=ims, strip=True, version=version, reaped=reaped)
-        elif reaped.proto == Protos.acdc.encode("utf-8"):
-            return SerderACDC(raw=ims, strip=True, version=version, reaped=reaped)
+        if smellage.proto == Protocols.keri:
+            return SerderKERI(raw=ims, strip=True, smellage=smellage,
+                              genus=genus, gvrsn=gvrsn)
+        elif smellage.proto == Protocols.acdc:
+            return SerderACDC(raw=ims, strip=True, smellage=smellage,
+                              genus=genus, gvrsn=gvrsn)
         else:
-            raise ProtocolError(f"Unsupported protocol type = {reaped.proto}.")
+            raise ProtocolError(f"Unsupported protocol type = {smellage.proto}.")
 
 
 
 class Serder:
     """Serder is serializer-deserializer class for saidified  over-the-wire
     messages that deserializes to a field map (label value pairs) from
     either a serialized field map or an unlabeled fixed field structure with
@@ -128,37 +263,53 @@
     override the Labels class attribute, and if necessary the .verify and
     .saidify methods and define any protocol specific properties. If necessary
     define ilk specific subclasses of a given protocol (ilk is packet type).
     The .Labels class attributes configures the field label(s) for said
     generation and verification in addition to the required fields.
 
     Class Attributes:
-        MaxVSOffset (int): Maximum Version String Offset in bytes/chars
-        InhaleSize (int): Minimum raw buffer size needed to inhale
-        Labels (dict): Protocol specific dict of field labels keyed by ilk
-            (packet type string value). None is default key when no ilk needed.
-            Each entry is a
+        Dummy (str): dummy character for computing SAIDs
+        Spans (dict): version string spans keyed by version
+        Digests (dict): map of digestive codes. Should be same set of codes as
+            in coring.DigestCodex coring.DigDex so that .digestive property works.
+            Use unit tests to ensure codex sets match
+        Protocol (str): class specific message protocol
+        Proto (str): default message protocol
+        Vrsn (Versionage): default version
+        Kind (str): default serialization kind one of Serials
+        Fields (dict): nested dict of field labels keyed by protocol, version,
+            and message type (ilk). Felds labels are provided with a Fieldage
+            named tuple (saids, reqs, alls) that governs field type and presence.
+            None is default message type (ilk) when no ilk needed in a message.
+            See below for detailed logic associated with Fields class attribute
 
     Properties:
         raw (bytes): of serialized event only
         sad (dict): self addressed data dict
+        genus (str): CESR genus code
+        gvrsn (Versionage): instance CESR genus code table version (Major, Minor)
         proto (str): Protocolage value as protocol identifier such as KERI, ACDC
-        version (Versionage): protocol version (Major, Minor)
+                     alias of .protocol
+        protocol (str): Protocolage value as protocol identifier such as KERI, ACDC
+                        alias of .proto
+        vrsn (Versionage): protocol version (Major, Minor) alias of .version
+        version (Versionage): protocol version (Major, Minor) alias of .vrsn
         kind (str): serialization kind coring.Serials such as JSON, CBOR, MGPK, CESR
         size (int): number of bytes in serialization
         said (str): qb64 said of .raw given by appropriate field
         saidb (bytes): qb64b of .said
         ilk (str | None): packet type for this Serder if any (may be None)
 
 
     Hidden Attributes:
-        ._raw is bytes of serialized event only
-        ._sad is key event dict
+        ._raw (bytes): serialized message
+        ._sad (dict): sad dict (key event dict)
+        ._cvrsn (Versionage): CESR code table version
         ._proto (str):  Protocolage value as protocol type identifier
-        ._version is Versionage instance of event version
+        ._vrsn is Versionage instance of event version
         ._kind is serialization kind string value (see namedtuple coring.Serials)
             supported kinds are 'json', 'cbor', 'msgpack', 'binary'
         ._size is int of number of bytes in serialed event only
         ._said (str): qb64 given by appropriate saidive field
 
     Methods:
         verify()
@@ -174,20 +325,27 @@
     StaticMethods:
         loads()
         dumps()
 
     Note:
         loads and jumps of json use str whereas cbor and msgpack use bytes
 
-    """
 
-    MaxVSOffset = 12
-    InhaleSize = MaxVSOffset + VERFULLSIZE  # min buffer size to inhale
+    Fields:
+        Each element of Fields is a FieldDom dataclass instance with four attributes:
+            alls (dict):
+            opts (dict):
+            saids (dict):
+            strict (bool):
+
+    """
+    Dummy = "#"  # dummy spaceholder char for SAID. Must not be a valid Base64 char
 
-    Dummy = "#"  # dummy spaceholder char for said. Must not be a valid Base64 char
+    # Spans dict keyed by version (Versionage instance) of version string span (size)
+    Spans = {Vrsn_1_0: VER1FULLSPAN, Vrsn_2_0: VER2FULLSPAN}
 
     # should be same set of codes as in coring.DigestCodex coring.DigDex so
     # .digestive property works. Use unit tests to ensure codex sets match
     Digests = {
         DigDex.Blake3_256: Digestage(klas=blake3.blake3, size=None, length=None),
         DigDex.Blake2b_256: Digestage(klas=hashlib.blake2b, size=32, length=None),
         DigDex.Blake2s_256: Digestage(klas=hashlib.blake2s, size=None, length=None),
@@ -196,195 +354,219 @@
         DigDex.Blake3_512: Digestage(klas=blake3.blake3, size=None, length=64),
         DigDex.Blake2b_512: Digestage(klas=hashlib.blake2b, size=None, length=None),
         DigDex.SHA3_512: Digestage(klas=hashlib.sha3_512, size=None, length=None),
         DigDex.SHA2_512: Digestage(klas=hashlib.sha512, size=None, length=None),
     }
 
     #override in subclass to enforce specific protocol
-    Protocol = None  # required protocol, None means any in Protos is ok
-
-    Proto = Protos.keri  # default protocol type
+    Protocol = None  # class based message protocol, None means any in Protocols is ok
+    Proto = Protocols.keri  # default message protocol type for makify on base Serder
     Vrsn = Vrsn_1_0  # default protocol version for protocol type
     Kind = Serials.json  # default serialization kind
+    CVrsn = Vrsn_2_0  # default CESR code table version
 
 
     # Nested dict keyed by protocol.
     # Each protocol value is a dict keyed by ilk.
     # Each ilk value is a Labelage named tuple with saids, codes and fields
     # ilk value of None is default for protocols that support ilkless packets
-    Fields = {
-            Protos.keri:
+    Fields = \
+    {
+        Protocols.keri:
+        {
+            Vrsn_1_0:
             {
-                Vrsn_1_0:
-                {
-                    Ilks.icp: Fieldage(saids={Saids.d: DigDex.Blake3_256,
-                                              Saids.i: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', kt='0',
-                            k=[], nt='0', n=[], bt='0', b=[], c=[], a=[])),
-                    Ilks.rot: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', s='0', p='',
-                            kt='0',k=[], nt='0', n=[], bt='0', br=[],
-                            ba=[], a=[])),
-                    Ilks.ixn: Fieldage({Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', s='0', p='', a=[])),
-                    Ilks.dip: Fieldage(saids={Saids.d: DigDex.Blake3_256,
-                                              Saids.i: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', kt='0',
-                            k=[], nt='0', n=[], bt='0', b=[], c=[], a=[],
-                            di='')),
-                    Ilks.drt: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', s='0', p='',
-                            kt='0',k=[], nt='0', n=[], bt='0', br=[],
-                            ba=[], a=[])),
-                    Ilks.rct: Fieldage(saids={},
-                        alls=dict(v='', t='',d='', i='', s='0')),
-                    Ilks.qry: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', dt='', r='', rr='',
-                                    q={})),
-                    Ilks.rpy: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', dt='', r='',a=[])),
-                    Ilks.pro: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', dt='', r='', rr='',
-                                    q={})),
-                    Ilks.bar: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', dt='', r='',a=[])),
-                    Ilks.exn: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='', d='', i="", p="", dt='', r='',q={},
-                                    a=[], e={})),
-                    Ilks.vcp: Fieldage(saids={Saids.d: DigDex.Blake3_256,
-                                              Saids.i: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', ii='', s='0', c=[],
-                                    bt='0', b=[], n='')),
-                    Ilks.vrt: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', p='', s='0',
-                                    bt='0', br=[], ba=[])),
-                    Ilks.iss: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', ri='',
-                                  dt='')),
-                    Ilks.rev: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', ri='',
-                                  p='', dt='')),
-                    Ilks.bis: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', ii='', s='0', ra={},
-                                  dt='')),
-                    Ilks.brv: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', p='', ra={},
-                                  dt='')),
-                },
-                Vrsn_1_1:
-                {
-                    Ilks.icp: Fieldage(saids={Saids.d: DigDex.Blake3_256,
-                                              Saids.i: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', kt='0',
-                            k=[], nt='0', n=[], bt='0', b=[], c=[], a=[])),
-                    Ilks.rot: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', s='0', p='',
-                            kt='0',k=[], nt='0', n=[], bt='0', br=[],
-                            ba=[], c=[], a=[])),
-                    Ilks.ixn: Fieldage({Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', s='0', p='', a=[])),
-                    Ilks.dip: Fieldage(saids={Saids.d: DigDex.Blake3_256,
-                                              Saids.i: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', kt='0',
-                            k=[], nt='0', n=[], bt='0', b=[], c=[], a=[],
-                            di='')),
-                    Ilks.drt: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', s='0', p='',
-                            kt='0',k=[], nt='0', n=[], bt='0', br=[],
-                            ba=[], c=[], a=[])),
-                    Ilks.rct: Fieldage(saids={},
-                        alls=dict(v='', t='',d='', i='', s='0')),
-                    Ilks.qry: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', dt='', r='', rr='',
-                                    q={})),
-                    Ilks.rpy: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', dt='', r='',a=[])),
-                    Ilks.pro: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', dt='', r='', rr='',
-                                    q={})),
-                    Ilks.bar: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='',d='', i='', dt='', r='',a=[])),
-                    Ilks.exn: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                        alls=dict(v='', t='', d='', i="", p="", dt='', r='', q={},
-                                    a=[], e={})),
-                },
+                Ilks.icp: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        kt='0',k=[], nt='0', n=[], bt='0', b=[], c=[],
+                        a=[]),
+                    saids={Saids.d: DigDex.Blake3_256,
+                           Saids.i: DigDex.Blake3_256,}),
+                Ilks.rot: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                            p='', kt='0',k=[], nt='0', n=[], bt='0', br=[],
+                            ba=[], a=[]),
+                        saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.ixn: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        p='', a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.dip: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        kt='0', k=[], nt='0', n=[], bt='0', b=[], c=[],
+                        a=[], di=''),
+                    saids={Saids.d: DigDex.Blake3_256,
+                           Saids.i: DigDex.Blake3_256,}),
+                Ilks.drt: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        p='', kt='0',k=[], nt='0', n=[], bt='0', br=[],
+                        ba=[], a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.rct: FieldDom(alls=dict(v='', t='',d='', i='', s='0')),
+                Ilks.qry: FieldDom(alls=dict(v='', t='',d='', dt='', r='',
+                        rr='',q={}),
+                    saids={Saids.d: DigDex.Blake3_256},),
+                Ilks.rpy: FieldDom(alls=dict(v='', t='',d='', dt='', r='',
+                        a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.pro: FieldDom(alls=dict(v='', t='',d='', dt='', r='',
+                        rr='',q={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.bar: FieldDom(alls=dict(v='', t='',d='', dt='', r='',
+                        a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.exn: FieldDom(alls=dict(v='', t='', d='', i="", p="",
+                        dt='', r='',q={}, a=[], e={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.vcp: FieldDom(alls=dict(v='', t='',d='', i='', ii='',
+                        s='0', c=[], bt='0', b=[], n=''),
+                    saids={Saids.d: DigDex.Blake3_256,
+                           Saids.i: DigDex.Blake3_256,}),
+                Ilks.vrt: FieldDom(alls=dict(v='', t='',d='', i='', p='',
+                        s='0', bt='0', br=[], ba=[]),
+                    saids={Saids.d: DigDex.Blake3_256,}),
+                Ilks.iss: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        ri='', dt=''),
+                    saids={Saids.d: DigDex.Blake3_256,}),
+                Ilks.rev: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        ri='', p='', dt=''),
+                    saids={Saids.d: DigDex.Blake3_256,}),
+                Ilks.bis: FieldDom(alls=dict(v='', t='',d='', i='', ii='',
+                        s='0', ra={}, dt=''),
+                    saids={Saids.d: DigDex.Blake3_256,}),
+                Ilks.brv: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                         p='', ra={}, dt=''),
+                    saids={Saids.d: DigDex.Blake3_256,}),
             },
-            Protos.crel:
+            Vrsn_2_0:
             {
-                Vrsn_1_1:
-                {
-                    Ilks.vcp: Fieldage(saids={Saids.d: DigDex.Blake3_256,
-                                              Saids.i: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', ii='', s='0', c=[],
-                                    bt='0', b=[], u='')),
-                    Ilks.vrt: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', p='', s='0',
-                                    bt='0', br=[], ba=[])),
-                    Ilks.iss: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', ri='',
-                                  dt='')),
-                    Ilks.rev: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', ri='',
-                                  p='', dt='')),
-                    Ilks.bis: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', ii='', s='0', ra={},
-                                  dt='')),
-                    Ilks.brv: Fieldage(saids={Saids.d: DigDex.Blake3_256,},
-                        alls=dict(v='', t='',d='', i='', s='0', p='', ra={},
-                                  dt='')),
-                },
+                Ilks.icp: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                         kt='0', k=[], nt='0', n=[], bt='0', b=[], c=[],
+                         a=[]),
+                    saids={Saids.d: DigDex.Blake3_256,
+                           Saids.i: DigDex.Blake3_256,}),
+                Ilks.rot: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        p='', kt='0',k=[], nt='0', n=[], bt='0', br=[],
+                        ba=[], c=[], a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.ixn: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        p='', a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.dip: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                        kt='0', k=[], nt='0', n=[], bt='0', b=[], c=[],
+                        a=[], di=''),
+                    saids={Saids.d: DigDex.Blake3_256,
+                           Saids.i: DigDex.Blake3_256,}),
+                Ilks.drt: FieldDom(alls=dict(v='', t='',d='', i='', s='0',
+                         p='', kt='0',k=[], nt='0', n=[], bt='0', br=[],
+                        ba=[], c=[], a=[]),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.rct: FieldDom(alls=dict(v='', t='',d='', i='', s='0')),
+                Ilks.qry: FieldDom(alls=dict(v='', t='',d='', i='', dt='',
+                        r='', rr='', q={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.rpy: FieldDom(alls=dict(v='', t='',d='', i='', dt='',
+                        r='',a={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.pro: FieldDom(alls=dict(v='', t='',d='', i='', dt='',
+                        r='', rr='', q={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.bar: FieldDom(alls=dict(v='', t='',d='', i='', dt='',
+                        r='',a={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.xip: FieldDom(alls=dict(v='', t='', d='', i="", dt='',
+                                             r='', q={}, a={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.exn: FieldDom(alls=dict(v='', t='', d='', i="", x="",
+                        p="", dt='', r='', q={}, a={}),
+                    saids={Saids.d: DigDex.Blake3_256}),
             },
-            Protos.acdc:
+        },
+        Protocols.acdc:
+        {
+            Vrsn_1_0:
             {
-                Vrsn_1_0:
-                {
-                    None: Fieldage(saids={Saids.d: DigDex.Blake3_256},
-                                   alls=dict(v='', d='', i='', s='')),
-                }
+                None: FieldDom(alls=dict(v='', d='', u='', i='',
+                        ri='', s='', a='', A='', e='', r=''),
+                    opts=dict(u='', ri='', a='', A='', e='', r=''),
+                    alts=dict(a="A", A="a"),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.ace: FieldDom(alls=dict(v='', t='', d='', u='', i='',
+                        ri='', s='', a='', A='', e='', r=''),
+                    opts=dict(u='', ri='', a='', A='', e='', r=''),
+                    alts=dict(a="A", A="a"),
+                    saids={Saids.d: DigDex.Blake3_256},
+                    strict=False),
             },
-        }
-
-
-    # default ilk for each protocol at default version is zeroth ilk in dict
-    Ilks = dict()
-    for key, val in Fields.items():
-        Ilks[key] = list(list(val.values())[0].keys())[0]
+            Vrsn_2_0:
+            {
+                None: FieldDom(alls=dict(v='', d='', u='', i='',
+                        rd='', s='', a='', A='', e='', r=''),
+                    opts=dict(u='', rd='', a='', A='', e='', r=''),
+                    alts=dict(a="A", A="a"),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.acd: FieldDom(alls=dict(v='', t='', d='', u='', i='',
+                        rd='', s='', a='', A='', e='', r=''),
+                    opts=dict(u='', rd='', a='', A='', e='', r=''),
+                    alts=dict(a="A", A="a"),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.ace: FieldDom(alls=dict(v='', t='', d='', u='', i='',
+                        rd='', s='', a='', A='', e='', r=''),
+                    opts=dict(u='', rd='', a='', A='', e='', r=''),
+                    alts=dict(a="A", A="a"),
+                    saids={Saids.d: DigDex.Blake3_256},
+                    strict=False),
+                Ilks.sch: FieldDom(alls=dict(v='', t='', d='', s=''),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.att: FieldDom(alls=dict(v='', t='', d='', a=''),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.agg: FieldDom(alls=dict(v='', t='', d='', A=''),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.rul: FieldDom(alls=dict(v='', t='', d='', e=''),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.rip: FieldDom(alls=dict(v='', t='', d='', u='', i='',
+                                              s='', dt=''),
+                    saids={Saids.d: DigDex.Blake3_256}),
+                Ilks.upd: FieldDom(alls=dict(v='', t='', d='', r='', s='',
+                                              p='', dt='', a=''),
+                    saids={Saids.d: DigDex.Blake3_256}),
+            },
+        },
+    }
 
 
-    def __init__(self, *, raw=b'', sad=None, strip=False, version=Version,
-                 reaped=None, verify=True, makify=False,
+    def __init__(self, *, raw=b'', sad=None, strip=False, smellage=None,
+                 genus=GenDex.KERI, gvrsn=Vrsn_2_0, verify=True, makify=False,
                  proto=None, vrsn=None, kind=None, ilk=None, saids=None):
         """Deserialize raw if provided. Update properties from deserialized raw.
             Verifies said(s) embedded in sad as given by labels.
             When verify is True then verify said(s) in deserialized raw as
             given by label(s) according to proto and ilk and code
         If raw not provided then serialize .raw from sad with kind and code.
             When kind not provided use kind embedded in sad['v'] version string.
             When saidify is True then compute and update said(s) in sad as
             given by label(s) according to proto and ilk and code.
 
         Parameters:
-            raw (bytes): serialized event
+            raw (bytes | bytearray): serialized event
             sad (dict): serializable saidified field map of message.
                 Ignored if raw provided
             strip (bool): True means strip (delete) raw from input stream
                 bytearray after parsing. False means do not strip.
                 Assumes that raw is bytearray when strip is True.
-            version (Versionage | None): instance supported protocol version
-                None means do not enforce a supported version
-            reaped (Reapage | None): instance of deconstructed version string
-                elements. If none or empty ignore otherwise assume that raw
-                already had its version string extracted (reaped) into the
-                elements of reaped.
+            smellage (Smellage | None): instance of deconstructed and converted
+                version string elements. If none or empty ignore otherwise assume
+                that raw already had its version string extracted (reaped) into the
+                elements of smellage.
+            genus (str):  CESR genus str. Either provided by parser from stream
+                or generated by Serder to stream
+            gvrsn (Versionage): instance CESR genus code table version
+                Either provided by parser from stream genus version or desired when
+                generating Serder instance to stream
             verify (bool): True means verify said(s) of given raw or sad.
                 Raises ValidationError if verification fails
                 Ignore when raw not provided or when raw and saidify is True
             makify (bool): True means compute fields for sad including size and
                 saids.
-            proto (str | None): desired protocol type str value of Protos
+            proto (str | None): desired protocol type str value of Protocols
                 If None then its extracted from sad or uses default .Proto
             vrsn (Versionage | None): instance desired protocol version
                 If None then its extracted from sad or uses default .Vrsn
             kind (str None): serialization kind string value of Serials
                 supported kinds are 'json', 'cbor', 'msgpack', 'binary'
                 If None then its extracted from sad or uses default .Kind
             ilk (str | None): desired ilk packet type str value of Ilks
@@ -395,82 +577,72 @@
                 Code assignment for each saidive field in desending priority:
                    - the code provided in saids when not None
                    - the code extracted from sad[said label] when valid CESR
                    - the code provided in .Fields...saids
 
 
         """
+        self._gvrsn = gvrsn
+        self._genus = genus
 
         if raw:  # deserialize raw using property setter
-            # self._inhale works because it only references class attributes
-            sad, proto, vrsn, kind, size = self._inhale(raw=raw,
-                                                        version=version,
-                                                        reaped=reaped)
-            self._raw = bytes(raw[:size])  # crypto ops require bytes not bytearray
-            self._sad = sad
-            self._proto = proto
-            self._vrsn = vrsn
-            self._kind = kind
-            self._size = size
+            self._inhale(raw=raw, smellage=smellage)
+            # ._inhale updates ._raw, ._sad, ._proto, ._vrsn, ._kind, ._size
+
             # primary said field label
             try:
-                label = list(self.Fields[self.proto][self.vrsn][self.ilk].saids.keys())[0]
+                label = list(self.Fields[self.proto][self.vrsn][self.ilk].saids)[0]
                 if label not in self._sad:
                     raise FieldError(f"Missing primary said field in {self._sad}.")
                 self._said = self._sad[label]  # not verified
             except Exception as ex:
                 self._said = None  # no saidive field
 
             if strip:  #only when raw is bytearray
                 try:
                     del raw[:self._size]
                 except TypeError:
                     pass  # ignore if bytes
 
-            if verify:  # verify the said(s) provided in raw
+            if verify:  # verify fields including the said(s) provided in raw
                 try:
                     self._verify()  # raises exception when not verify
                 except Exception as ex:
                     logger.error("Invalid raw for Serder %s\n%s",
                                  self.pretty(), ex.args[0])
                     raise ValidationError(f"Invalid raw for Serder = "
                                           f"{self._sad}. {ex.args[0]}") from ex
 
         elif sad or makify:  # serialize sad into raw or make sad
             if makify:  # recompute properties and said(s) and reset sad
-                # makify resets sad, raw, proto, version, kind, and size
-                self.makify(sad=sad, version=version,
-                        proto=proto, vrsn=vrsn, kind=kind, ilk=ilk, saids=saids)
+                # makify resets sad, raw, proto, vrsn, kind, ilk, and size
+                self.makify(sad=sad, proto=proto, vrsn=vrsn, kind=kind,
+                            ilk=ilk, saids=saids)
+                # .makify updates ._raw, ._sad, ._proto, ._vrsn, ._kind, ._size
 
             else:
-                # self._exhale works because it only access class attributes
-                raw, sad, proto, vrsn, kind, size = self._exhale(sad=sad,
-                                                                 version=version)
-                self._raw = raw
-                self._sad = sad
-                self._proto = proto
-                self._vrsn = vrsn
-                self._kind = kind
-                self._size = size
-                # primary said field label
-                try:
-                    label = list(self.Fields[self.proto][self.vrsn][self.ilk].saids.keys())[0]
-                    if label not in self._sad:
-                        raise DeserializeError(f"Missing primary said field in {self._sad}.")
-                    self._said = self._sad[label]  # not verified
-                except Exception:
-                    self._said = None  # no saidive field
+                self._exhale(sad=sad)
+                # .exhale updates ._raw, ._sad, ._proto, ._vrsn, ._kind, ._size
 
-                if verify:  # verify the said(s) provided in sad
-                    try:
-                        self._verify()  # raises exception when not verify
-                    except Exception as ex:
-                        logger.error("Invalid sad for Serder %s\n%s",
-                                     self.pretty(), ex.args[0])
-                        raise ValidationError(f"Invalid sad for Serder ="
+            # primary said field label
+            try:
+                label = list(self.Fields[self.proto][self.vrsn][self.ilk].saids)[0]
+                if label not in self._sad:
+                    raise DeserializeError(f"Missing primary said field in {self._sad}.")
+                self._said = self._sad[label]  # not verified
+            except Exception:
+                self._said = None  # no saidive field
+
+            if verify:  # verify fields including the said(s) provided in sad
+                try:
+                    self._verify()  # raises exception when not verify
+                except Exception as ex:
+                    logger.error("Invalid sad for Serder %s\n%s",
+                                 self.pretty(), ex.args[0])
+                    raise ValidationError(f"Invalid sad for Serder ="
                                               f"{self._sad}.") from ex
 
         else:
             raise ValueError("Improper initialization need raw or sad or makify.")
 
 
 
@@ -499,61 +671,94 @@
         Override for protocol and ilk specific verification behavior. Especially
         for inceptive ilks that have more than one said field like a said derived
         identifier prefix.
 
         Raises a ValidationError (or subclass) if any verification fails
 
         """
-        if self.Protocol and self.proto != self.Protocol:
-            raise ValidationError(f"Expected protocol = {self.Protocol}, got "
+        if self.Protocol and self.proto != self.Protocol:  # class required
+            raise ValidationError(f"Required protocol = {self.Protocol}, got "
                                  f"{self.proto} instead.")
 
         if self.proto not in self.Fields:
             raise ValidationError(f"Invalid protocol type = {self.proto}.")
 
+        if self.genus not in GenDex:  # ensures self.genus != None
+            raise SerializeError(f"Invalid genus={self.genus}.")
+
+        if getattr(GenDex, self.proto, None) != self.genus:
+            raise SerializeError(f"Incompatible protocol={self.proto} with "
+                                 f"genus={self.genus}.")
+
+        if self.vrsn.major > self.gvrsn.major:
+            raise SerializeError(f"Incompatible major protocol version={self.vrsn}"
+                                 f" with major genus version={self.gvrsn}.")
+
+        if self.vrsn not in self.Fields[self.proto]:
+            raise SerializeError(f"Invalid version={self.vrsn} for "
+                                 f"protocol={self.proto}.")
+
         if self.ilk not in self.Fields[self.proto][self.vrsn]:
             raise ValidationError(f"Invalid packet type (ilk) = {self.ilk} for"
                                   f"protocol = {self.proto}.")
 
+
+
         fields = self.Fields[self.proto][self.vrsn][self.ilk]  # get labelage
-        # ensure all required fields in alls are in sad
-        alls = fields.alls  # dict of all field labels with default values
-        keys = list(self._sad)  # get list of keys of self.sad
-        for key in list(keys):  # make copy to mutate
-            if key not in alls:
-                del keys[keys.index(key)]  # remove non required fields
-
-        if list(alls.keys()) != keys:  # forces ordering of labels in .sad
-            raise MissingFieldError(f"Missing one or more required fields from"
-                                    f"= {list(alls.keys())} in sad = "
-                                    f"{self._sad}.")
+
+        alls = fields.alls  # faster local reference
+        oalls = oset(alls)  # ordereset of field labels
+        oopts = oset(fields.opts)  # ordereset of field labels
+        oreqs = oalls - oopts  # required fields
+
+        oskeys = oset(self._sad)  # ordered set of keys in sad (skeys)
+        osexts = oskeys - oalls  # get ordered set of extras in sad (sexts)
+        if osexts and fields.strict:
+            raise ExtraFieldError(f"Unallowed extra field(s) = {list(osexts)} "
+                                     f"in sad.")
+
+        osopts = oskeys - oreqs - osexts  # subset of opts in sad
+
+        osalls = oalls - (oopts - osopts)  # subset of alls without missing opts in sad
+
+        for k, v in fields.alts.items():
+            if k in osopts and v in osopts:
+                raise AlternateFieldError(f"Unallowed, alternate fields '{k}' "
+                                          f"and '{v}' both present in sad.")
+
+        # can't do set math osalls == oskeys - osexts becasue of osexts might be
+        # out-of-order so have to iterate to ensure osexts if any appear in oskeys
+        # after all fields in osalls
+        for i, label in enumerate(osalls):
+            if oskeys[i] != label:
+                raise MissingFieldError(f"Missing or out-of-order field = {label} "
+                                         f"from = {list(osalls)} in sad.")
 
         # said field labels are not order dependent with respect to all fields
         # in sad so use set() to test inclusion
         saids = copy.copy(fields.saids)  # get copy of saidive field labels and defaults values
-        if not (set(saids.keys()) <= set(alls.keys())):
+        if not (set(saids) <= set(alls)):
             raise MissingFieldError(f"Missing one or more required said fields"
-                                    f" from {list(saids.keys())} in sad = "
+                                    f" from {list(saids)} in sad = "
                                     f"{self._sad}.")
 
         sad = self.sad  # make shallow copy so don't clobber original .sad
-        for label in saids.keys():
+        for label in saids:
             try:  # replace default code with code of value from sad
                 saids[label] = Matter(qb64=sad[label]).code
             except Exception as ex:
                 if saids[label] in DigDex:  # digestive but invalid
                     raise ValidationError(f"Invalid said field '{label}' in sad\n"
                                       f" = {self._sad}.") from ex
 
             if saids[label] in DigDex:  # if digestive then replace with dummy
                 sad[label] = self.Dummy * len(sad[label])
 
-
+        # compute saidive digestive field values using raw from sized dummied sad
         raw = self.dumps(sad, kind=self.kind)  # serialize dummied sad copy
-
         for label, code in saids.items():
             if code in DigDex:  # subclass override if non digestive allowed
                 klas, size, length = self.Digests[code]  # digest algo size & length
                 ikwa = dict()  # digest algo class initi keyword args
                 if size:
                     ikwa.update(digest_size=size)  # optional digest_size
                 dkwa = dict()  # digest method keyword args
@@ -561,23 +766,46 @@
                     dkwa.update(length=length)
                 dig = Matter(raw=klas(raw, **ikwa).digest(**dkwa), code=code).qb64
                 if dig != self._sad[label]:  # compare to original
                     raise ValidationError(f"Invalid said field '{label}' in sad"
                                           f" = {self._sad}, should be {dig}.")
                 sad[label] = dig
 
-        raw = self.dumps(sad, kind=self.kind)
+        raw = self.dumps(sad, kind=self.kind)  # compute final raw
+
         if raw != self.raw:
             raise ValidationError(f"Invalid round trip of {sad} != \n"
                                   f"{self.sad}.")
+
+        if "v" not in sad:
+            raise ValidationError(f"Missing version string field in {sad}.")
+
+        # extract version string elements to verify consistency with attributes
+        proto, vrsn, kind, size, opt = deversify(sad["v"])
+        if self.proto != proto:
+            raise ValidationError(f"Inconsistent protocol={self.proto} in {sad}.")
+
+        if self.vrsn != vrsn:
+            raise ValidationError(f"Inconsistent version={self.vrsn} in {sad}.")
+
+        if self.kind != kind:
+            raise ValidationError(f"Inconsistent kind={self.kind} in {sad}.")
+
+        if self.kind in (Serials.json, Serials.cbor, Serials.mgpk):
+            if size != self.size != len(raw):
+                raise ValidationError(f"Inconsistent size={self.size} in {sad}.")
+        else:  # size is not set in version string when kind is CESR
+            if self.size != len(raw):
+                raise ValidationError(f"Inconsistent size={self.size} in {sad}.")
+
         # verified successfully since no exception
 
 
-    def makify(self, sad, *, version=None,
-               proto=None, vrsn=None, kind=None, ilk=None, saids=None):
+    def makify(self, sad, *, proto=None, vrsn=None, kind=None,
+               ilk=None, saids=None):
         """Makify given sad dict makes the versions string and computes the said
         field values and sets associated properties:
         raw, sad, proto, version, kind, size
 
         Override for protocol and ilk specific saidification behavior. Especially
         for inceptive ilks that have more than one said field like a said derived
         identifier prefix.
@@ -587,17 +815,15 @@
            Else use provided version string if valid
            Otherwise use class attribute
 
 
         Parameters:
             sad (dict): serializable saidified field map of message.
                 Ignored if raw provided
-            version (Versionage): instance supported protocol version
-                None means do not enforce version
-            proto (str | None): desired protocol type str value of Protos
+            proto (str | None): desired protocol type str value of Protocols
                 If None then its extracted from sad or uses default .Proto
             vrsn (Versionage | None): instance desired protocol version
                 If None then its extracted from sad or uses default .Vrsn
             kind (str None): serialization kind string value of Serials
                 supported kinds are 'json', 'cbor', 'msgpack', 'binary'
                 If None then its extracted from sad or uses default .Kind
             ilk (str | None): desired ilk packet type str value of Ilks
@@ -609,88 +835,123 @@
                    - the code provided in saids when not None
                    - the code extracted from sad[said label] when valid CESR
                    - the code provided in .Fields...saids
         """
         sproto = svrsn = skind = silk = None
         if sad and 'v' in sad:  # attempt to get from vs in sad
             try:  # extract version string elements as defaults if provided
-                sproto, svrsn, skind, _ = deversify(sad["v"], version=version)
+                sproto, svrsn, skind, _, _ = deversify(sad["v"])
             except ValueError as ex:
                 pass
             else:
-                silk = sad.get('t')  # if not in get returns None which may be valid
+                silk = sad.get('t')  # if 't' not in sad .get returns None which may be valid
 
         if proto is None:
             proto = sproto if sproto is not None else self.Proto
 
-        if vrsn is None:
-            vrsn = svrsn if svrsn is not None else self.Vrsn
-
-        if kind is None:
-            kind = skind if skind is not None else self.Kind
+        if proto not in self.Fields:
+            raise SerializeError(f"Invalid protocol={proto}.")
 
-        if ilk is None:
-            ilk = silk if silk is not None else self.Ilks[proto]
+        if self.Protocol and proto != self.Protocol:  # required by class
+            raise SerializeError(f"Required protocol={self.Protocol}, got "
+                                 f"protocol={proto} instead.")
+
+        if self.genus not in GenDex:  # ensures self.genus != None
+            raise SerializeError(f"Invalid genus={self.genus}.")
+
+        if getattr(GenDex, proto, None) != self.genus:
+            raise SerializeError(f"Incompatible protocol={proto} with "
+                                 f"genus={self.genus}.")
 
+        if vrsn is None:
+            vrsn = svrsn if svrsn is not None else self.Vrsn
 
-        if proto not in self.Fields:
-            raise SerializeError(f"Invalid protocol type = {proto}.")
+        if vrsn not in self.Fields[proto]:
+            raise SerializeError(f"Invalid version={vrsn} for protocol={proto}.")
 
+        if vrsn.major > self.gvrsn.major:
+            raise SerializeError(f"Incompatible major protocol version={vrsn} "
+                                 f"with major genus version={self.gvrsn}.")
 
-        if self.Protocol and proto != self.Protocol:
-            raise SerializeError(f"Expected protocol = {self.Protocol}, got "
-                                 f"{proto} instead.")
+        if kind is None:
+            kind = skind if skind is not None else self.Kind
 
-        if version is not None and vrsn != version:
-            raise SerializeError(f"Expected version = {version}, got "
-                               f"{vrsn.major}.{vrsn.minor}.")
+        if ilk is None:  # default is first ilk in Fields for given proto vrsn
+            ilk = (silk if silk is not None else
+                   list(self.Fields[proto][vrsn])[0])  # list(dict) gives list of keys
 
         if kind not in Serials:
             raise SerializeError(f"Invalid serialization kind = {kind}")
 
-
         if ilk not in self.Fields[proto][vrsn]:
             raise SerializeError(f"Invalid packet type (ilk) = {ilk} for"
                                   f"protocol = {proto}.")
 
-        fields = self.Fields[proto][vrsn][ilk]  # get Fieldage of fields
+        fields = self.Fields[proto][vrsn][ilk]  # get FieldDom of fields
+
+        alls = fields.alls  # faster local reference
+        oalls = oset(alls)  # ordereset of field labels
+        oopts = oset(fields.opts)  # ordereset of field labels
+        oreqs = oalls - oopts  # required fields
 
-        if not sad:  # empty or None so create from defaults
-            sad = {}
-            for label, value in fields.alls.items():
-                if helping.nonStringIterable(value):  # copy iterable defaults
-                    value = copy.copy(value)
-                sad[label] = value
 
-            if 't' in sad:  # packet type (ilk) requried so set value to ilk
-                sad['t'] = ilk
+        if not sad:  # empty or None so create sad dict
+            sad = {}
 
-        # ensure all required fields in alls are in sad
-        alls = fields.alls  # all field labels
-        for label, value in alls.items():  # ensure provided sad as all required fields
-            if label not in sad:  # supply default
-                if helping.nonStringIterable(value):  # copy iterable defaults
-                    value = copy.copy(value)
+        # ensure all required fields are in sad. If not provide default
+        for label in oreqs:
+            if label not in sad:
+                value = alls[label]
+                if helping.nonStringIterable(value):
+                    value = copy.copy(value)  # copy iterable defaults
                 sad[label] = value
 
-        keys = list(sad)  # get list of keys of self.sad
-        for key in list(keys):  # make copy to mutate
-            if key not in alls:
-                del keys[keys.index(key)]  # remove non required fields
-
-        if list(alls.keys()) != keys:  # ensure ordering of fields matches alls
-            raise SerializeError(f"Mismatch one or more of all required fields "
-                                 f" = {list(alls.keys())} in sad = {sad}.")
+        sadold = sad
+        sad = {}
+        for label in oalls:  # make sure all fields are in correct order
+            if label in sadold:
+                sad[label] = sadold[label]
+
+        for label in sadold:  # copy extras if any
+            if label not in sad:
+                sad[label] = sadold[label]
+
+        if 't' in sad:  # when packet type field then force ilk
+            sad['t'] = ilk  # assign ilk
+
+        # ensure required fields are present and all fields are ordered wrt alls
+        oskeys = oset(sad)  # ordered set of keys in sad (skeys)
+        osexts = oskeys - oalls  # get ordered set of extras in sad (sexts)
+        if osexts and fields.strict:
+            raise SerializeError(f"Unallowed extra field(s) = {list(osexts)} "
+                                 f"in sad.")
+
+        osopts = oskeys - oreqs - osexts  # subset of opts in sad
+
+        osalls = oalls - (oopts - osopts)  # subset of alls without missing opts in sad
+
+        for k, v in fields.alts.items():
+            if k in osopts and v in osopts:
+                raise SerializeError(f"Unallowed, alternate fields '{k}' "
+                                          f"and '{v}' both present in sad.")
+
+        # can't do set math osalls == oskeys - osexts becasue of osexts might be
+        # out-of-order so have to iterate to ensure osexts if any appear in oskeys
+        # after all fields in osalls
+        for i, label in enumerate(osalls):
+            if oskeys[i] != label:
+                raise SerializeError(f"Missing or out-of-order field = {label} "
+                                            f"from = {list(osalls)} in sad.")
 
         # said field labels are not order dependent with respect to all fields
         # in sad so use set() to test inclusion
         _saids = copy.copy(fields.saids)  # get copy of defaults
-        if not (set(_saids.keys()) <= set(alls.keys())):
+        if not (set(_saids) <= set(alls)):
             raise SerializeError(f"Missing one or more required said fields "
-                                 f"from {list(_saids.keys())} in sad = {sad}.")
+                                 f"from {list(_saids)} in sad = {sad}.")
 
         # override saidive defaults
         for label in _saids:
             if saids and label in saids:  # use parameter override
                 _saids[label] = saids[label]
             else:
                 try:  # use sad field override
@@ -702,144 +963,120 @@
                 sad[label] = self.Dummy * Matter.Sizes[_saids[label]].fs
 
 
         if 'v' not in sad:  # ensures that 'v' is always required by .Labels
             raise SerializeError(f"Missing requires version string field 'v'"
                                           f" in sad = {sad}.")
 
-        sad['v'] = self.Dummy * VERFULLSIZE  # ensure size of vs
+        if kind in (Serials.json, Serials.cbor, Serials.mgpk):
+            # this size of sad needs to be computed based on actual version string span
+            # since not same for all versions
+            sad['v'] = self.Dummy * self.Spans[vrsn]  # ensure span of vs is dummied MAXVERFULLSPAN
 
-        raw = self.dumps(sad, kind)  # get size of fully dummied sad
-        size = len(raw)
+            raw = self.dumps(sad, kind)  # get size of sad with fully dummied vs and saids
+            size = len(raw)
 
-        # generate new version string with correct size
-        vs = versify(proto=proto, version=vrsn, kind=kind, size=size)
-        sad["v"] = vs  # update version string in sad
+            # generate new version string with correct size
+            vs = versify(protocol=proto, version=vrsn, kind=kind, size=size)
+            sad["v"] = vs  # update version string in sad
+            # now have correctly sized version string in sad
 
-        # now have correctly sized version string in sad
-        # now compute saidive digestive field values using sized dummied sad
-        raw = self.dumps(sad, kind=kind)  # serialize sized dummied sad
 
+        # compute saidive digestive field values using raw from sized dummied sad
+        raw = self.dumps(sad, kind=kind)  # serialize sized dummied sad
         for label, code in _saids.items():
             if code in DigDex:  # subclass override if non digestive allowed
                 klas, dsize, dlen = self.Digests[code]  # digest algo size & length
                 ikwa = dict()  # digest algo class initi keyword args
                 if dsize:
                     ikwa.update(digest_size=dsize)  # optional digest_size
                 dkwa = dict()  # digest method keyword args
                 if dlen:
                     dkwa.update(length=dlen)
                 dig = Matter(raw=klas(raw, **ikwa).digest(**dkwa), code=code).qb64
                 sad[label] = dig
 
         raw = self.dumps(sad, kind=kind)  # compute final raw
+        if kind == Serials.cesr:# cesr kind version string does not set size
+            size = len(raw) # size of whole message
 
         self._raw = raw
         self._sad = sad
         self._proto = proto
         self._vrsn = vrsn
         self._kind = kind
         self._size = size
-        # primary said field label
-        try:
-            label = list(self.Fields[self.proto][self.vrsn][self.ilk].saids.keys())[0]
-            if label not in self._sad:
-                raise SerializeError(f"Missing primary said field in {self._sad}.")
-            self._said = self._sad[label]  # implicitly verified
-        except Exception:
-            self._said = None  # no saidive field
-
 
 
-    @classmethod
-    def _inhale(clas, raw, version=Version, reaped=None):
+    def _inhale(self, raw, *, smellage=None):
         """Deserializes raw.
         Parses serilized event ser of serialization kind and assigns to
         instance attributes and returns tuple of associated elements.
 
         As classmethod enables testing parsing raw serder values. This can be
         called on self as well because it only ever accesses clas attributes
         not instance attributes.
 
         Returns: tuple (sad, proto, vrsn, kind, size) where:
             sad (dict): serializable attribute dict of saidified data
-            proto (str): value of Protos (Protocolage) protocol type
+            proto (str): value of Protocols (Protocolage) protocol type
             vrsn (Versionage | None): tuple of (major, minor) version ints
                 None means do not enforce version
             kind (str): value of Serials (Serialage) serialization kind
 
         Parameters:
+            clas (Serder): class reference
             raw (bytes): serialized sad message
-            version (Versionage): instance supported protocol version
-            reaped (Reapage | None): instance of deconstructed version string
+            smellage (Smellage | None): instance of deconstructed version string
                 elements. If none or empty ignore otherwise assume that raw
                 already had its version string extracted (reaped) into the
-                elements of reaped.
+                elements of smellage.
 
-        Note:
-            loads and jumps of json use str whereas cbor and msgpack use bytes
-            Assumes only supports Version
 
-        """
-        if reaped:
-            proto, major, minor, kind, size = reaped  # tuple unpack
-        else:
-            if len(raw) < clas.InhaleSize:
-                raise ShortageError(f"Need more raw bytes for Serder to inhale.")
 
-            match = Rever.search(raw)  # Rever regex takes bytes/bytearray not str
-            if not match or match.start() > clas.MaxVSOffset:
-                raise VersionError(f"Invalid version string in raw = "
-                                   f"{raw[:clas.InhaleSize]}.")
-
-            proto, major, minor, kind, size = match.group("proto",
-                                                          "major",
-                                                          "minor",
-                                                          "kind",
-                                                          "size")
-
-        proto = proto.decode("utf-8")
-        if proto not in Protos:
-            raise ProtocolError(f"Invalid protocol type = {proto}.")
-
-        vrsn = Versionage(major=int(major, 16), minor=int(minor, 16))
-        if version is not None and vrsn != version:
-            raise VersionError(f"Expected version = {version}, got "
-                               f"{vrsn.major}.{vrsn.minor}.")
-
-        kind = kind.decode("utf-8")
-        if kind not in Serials:
-            raise KindError(f"Invalid serialization kind = {kind}.")
-
-        size = int(size, 16)
-        if len(raw) < size:
-            raise ShortageError(f"Need more bytes.")
+        """
+        if smellage:  # passed in so don't need to smell raw again
+            proto, vrsn, kind, size, gvrsn = smellage  # tuple unpack
+        else:  # not passed in so smell raw
+            proto, vrsn, kind, size, gvrsn = smell(raw)
 
-        sad = clas.loads(raw=raw, size=size, kind=kind)
+        sad = self.loads(raw=raw, size=size, kind=kind)
+        # ._gvrsn may be set in loads when CESR native deserialization provides _gvrsn
 
-        if "v" not in sad:
+        if "v" not in sad:  # Regex does not check for version string label itself
             raise FieldError(f"Missing version string field in {sad}.")
 
-        return sad, proto, vrsn, kind, size
+        # cypto opts want bytes not bytearray
+        self._raw = bytes(raw[:size])  # make copy so strip not affect
+        self._sad = sad
+        self._proto = proto
+        self._vrsn = vrsn
+        self._kind = kind
+        self._size = size
+
 
 
-    @staticmethod
-    def loads(raw, size=None, kind=Serials.json):
-        """Utility static method to handle deserialization by kind
+    def loads(self, raw, size=None, kind=Serials.json):
+        """method to handle deserialization by kind
+        assumes already sniffed and smelled to determine
+        serialization size and kind
 
         Returns:
            sad (dict | list): deserialized dict or list. Assumes attribute
                 dict of saidified data.
 
         Parameters:
-           raw (bytes |bytearray): raw serialization to deserialze as dict
+           raw (bytes | bytearray): raw serialization to deserialze as dict
            size (int): number of bytes to consume for the deserialization.
                        If None then consume all bytes in raw
            kind (str): value of Serials (Serialage) serialization kind
                        "JSON", "MGPK", "CBOR"
+
+        Notes:
+            loads of json uses str whereas loads of cbor and msgpack use bytes
         """
         if kind == Serials.json:
             try:
                 sad = json.loads(raw[:size].decode("utf-8"))
             except Exception as ex:
                 raise DeserializeError(f"Error deserializing JSON: "
                     f"{raw[:size].decode('utf-8')}") from ex
@@ -860,91 +1097,253 @@
 
         else:
             raise DeserializeError(f"Invalid deserialization kind: {kind}")
 
         return sad
 
 
-    @classmethod
-    def _exhale(clas, sad, version=None):
-        """Serializes sad given kind and version and sets the serialized size
-        in the version string.
-
-        As classmethod enables bootstrap of valid sad dict that has correct size
-        in version string. This obviates sizeify. This can be called on self as
-        well because it only ever accesses clas attributes not instance attributes.
-
-        Returns tuple of (raw, proto, kind, sad, vrsn) where:
-            raw (str): serialized event as bytes of kind
-            proto (str): protocol type as value of Protocolage
-            kind (str): serialzation kind as value of Serialage
-            sad (dict): modified serializable attribute dict of saidified data
-            vrsn (Versionage): tuple value (major, minor)
+    def _loads(self, raw, size=None):
+        """CESR native desserialization of raw
+
+        Returns:
+           sad (dict): deserialized dict of CESR native serialization.
 
         Parameters:
-            sad (dict): serializable attribute dict of saidified data
-            version (Versionage | None): supported protocol version for message
-                None means do not enforce a supported version
+           clas (Serder): class reference
+           raw (bytes |bytearray): raw serialization to deserialze as dict
+           size (int): number of bytes to consume for the deserialization.
+                       If None then consume all bytes in raw
+        """
+        # ._gvrsn may be set in loads when CESR native deserialization provides _gvrsn
+        pass
+
 
+    def _exhale(self, sad):
+        """Serializes sad and assigns attributes.
+        Asssumes all field values in sad are valid.
+        Call .verify to otherwise
 
+        Parameters:
+            sad (dict): serializable attribute dict of saidified data
         """
         if "v" not in sad:
             raise SerializeError(f"Missing version string field in {sad}.")
 
         # extract elements so can replace size element but keep others
-        proto, vrsn, kind, size = deversify(sad["v"], version=version)
-
-        raw = clas.dumps(sad, kind)
-        size = len(raw)
-
-        # generate new version string with correct size
-        vs = versify(proto=proto, version=vrsn, kind=kind, size=size)
+        proto, vrsn, kind, size, opt = deversify(sad["v"])
 
-        # find location of old version string inside raw
-        match = Rever.search(raw)  # Rever's regex takes bytes
-        if not match or match.start() > 12:
-            raise SerializeError(f"Invalid version string in raw = {raw}.")
-        fore, back = match.span()  # start and end positions of version string
+        raw = self.dumps(sad, kind)
 
-        # replace old version string in raw with new one
-        raw = b'%b%b%b' % (raw[:fore], vs.encode("utf-8"), raw[back:])
-        if size != len(raw):  # substitution messed up
-            raise SerializeError(f"Malformed size of raw in version string == {vs}")
-        sad["v"] = vs  # update sad
+        if kind in (Serials.cesr):  # cesr kind version string does not set size
+            size = len(raw) # size of whole message
 
-        return raw, sad, proto, vrsn, kind, size
+        # must call .verify to ensure these are compatible
+        self._raw = raw  # crypto opts want bytes not bytearray
+        self._sad = sad
+        self._proto = proto
+        self._vrsn = vrsn
+        self._kind = kind
+        self._size = size
 
 
-    @staticmethod
-    def dumps(sad, kind=Serials.json):
-        """Utility static method to handle serialization by kind
+    def dumps(self, sad, kind=Serials.json):
+        """Method to handle serialization by kind
+        Assumes sad fields are properly filled out for serialization kind.
 
         Returns:
            raw (bytes): serialization of sad dict using serialization kind
 
         Parameters:
            sad (dict | list)): serializable dict or list to serialize
            kind (str): value of Serials (Serialage) serialization kind
-                "JSON", "MGPK", "CBOR"
+                "JSON", "MGPK", "CBOR", "CSER"
+
+        Notes:
+            dumps of json uses str whereas dumps of cbor and msgpack use bytes
+            crypto opts want bytes not bytearray
         """
         if kind == Serials.json:
             raw = json.dumps(sad, separators=(",", ":"),
                              ensure_ascii=False).encode("utf-8")
 
         elif kind == Serials.mgpk:
             raw = msgpack.dumps(sad)
 
         elif kind == Serials.cbor:
             raw = cbor.dumps(sad)
+
+        elif kind == Serials.cser:
+            raw = self._dumps(sad)
+
         else:
             raise SerializeError(f"Invalid serialization kind = {kind}")
 
         return raw
 
 
+    def _dumps(self, sad):
+        """CESR native serialization of sad
+
+        Returns:
+            raw (bytes): CESR native serialization of sad dict
+
+        Parameters:
+            sad (dict | list)): serializable dict or list to serialize
+
+        Versioning:
+            CESR native serialization includes in its fixed version field
+            a version primitive that includes message protocol+protocol version
+            +genus version: 0NPPPPMmmMmm (12 B64 characters)
+
+            This assumes that genus is compatible with message
+            protocol so genus is not needed. This protects from malleability attack
+            and ensure compatible cesr codes especially count (group) codes.
+            Primitive codes are less problematic since so far all primitive codes
+            tables are backwards compatible across major versions.
+
+        """
+        if (self.gvrsn.major < Vrsn_2_0.major or
+            self.vrsn.major < Vrsn_2_0.major):
+                raise SerializeError(f"Invalid major genus version={self.gvrsn}"
+                                f"or Invalid major protocol version={self.vrsn}"
+                                f" for native CESR serialization.")
+
+        if self.genus not in GenDex:  # ensures self.genus != None
+            raise SerializeError(f"Invalid genus={self.genus}.")
+
+        if getattr(GenDex, self.proto, None) != self.genus:
+            raise SerializeError(f"Incompatible protocol={self.proto} with "
+                                 f"genus={self.genus}.")
+
+
+        fixed = True  # True = use fixed field, False= use field map
+
+        raw = bytearray()
+        ilks = self.Fields[self.proto][self.vrsn]  # get fields keyed by ilk
+
+        ilk = sad.get('t')  # returns None if missing message type (ilk)
+        if ilk not in ilks:  #
+            raise SerializeError(f"Missing message type field "
+                                 f"'t' for protocol={self.proto} "
+                                 f"version={self.vrsn} with {sad=}.")
+
+        fields = ilks[ilk]  # FieldDom for given protocol and ilk
+
+        if fields.opts or not fields.strict:  # optional or extra fields allowed
+            fixed = False  # so must use field map
+
+
+        # assumes that sad's field ordering and field inclusion is correct
+        # so can serialize in order to compute saidive fields
+        # need to fix ._verify and .makify to account for CESR native serialization
+
+        if self.proto == Protocols.keri:
+            for l, v in sad.items():  # assumes valid field order & presence
+                if not fixed:  # prepend label
+                    pass
+
+                # should dispatch or use match instead of big if else
+                match l:  # label
+                    case "v":  # protocol+version  do not use version string itself
+                        val = Verser(proto=self.proto, vrsn=self.vrsn).qb64b
+
+                    case "t":  # message type (ilk), already got ilk
+                        val = Ilker(ilk=v).qb64b  # assumes same
+
+                    case "d" | "i" | "p" | "di":  # said or aid
+                        val = v.encode("utf-8")  # already primitive qb64 make qb6b
+
+                    case "s" | "bt":  # sequence number or numeric threshold
+                        val = coring.Number(numh=v).qb64b  # convert hex str
+
+                    case "kt" | "nt": # current or next signing threshold
+                        val = coring.Tholder(sith=v).limen  # convert sith str
+
+                    case "k" | "n" | "b" | "ba" | "br":  # list of primitives
+                        frame = bytearray()
+                        for e in v:  # list
+                            frame.extend(e.encode("utf-8"))
+
+                        val = bytearray(Counter(tag=AllTags.GenericListGroup,
+                                                count=len(frame) % 4).qb64b)
+                        val.extend(frame)
+
+                    case "c":  # list of config traits strings
+                        frame = bytearray()
+                        for e in v:  # list
+                            frame.extend(Traitor(trait=e).qb64n)
+
+                        val = bytearray(Counter(tag=AllTags.GenericListGroup,
+                                                count=len(frame) % 4).qb64b)
+                        val.extend(frame)
+
+                    case "a":  # list of seals or field map of attributes
+                        frame = bytearray()
+                        for e in v:  # list of seal dicts
+                            pass
+                            #if tuple(v) == eventing.SealEvent._fields:
+                                #eseal = eventing.SealEvent(**v)  # convert to namedtuple
+                                #SealSourceCouples: str = '-Q'  # Seal Source Couple(s), snu+dig of source sealing or sealed event.
+                                #SealSourceTriples: str = '-R'  # Seal Source Triple(s), pre+snu+dig of source sealing or sealed event.
+                                #DigestSealSingles: str = '-V'  # Digest Seal Single(s), dig of sealed data.
+                                #MerkleRootSealSingles: str = '-W'  # Merkle Tree Root Digest Seal Single(s), dig of sealed data.
+                                #BackerRegistrarSealCouples: str = '-X'  # Backer Registrar Seal Couple(s), brid+dig of sealed data.
+
+                                # SealMark == tuple of seal dict field names tuple(dict)
+                                #d = dict(a=1, b=2)
+                                #tuple(d)
+                                #('a', 'b')
+
+                            #frame.extend(Anchor(seal=e).qb64b)
+                            # else:  generic seal no count type (v, Mapping):
+                                #for l, e in v.items():
+                                    #pass
+                                #val = bytearray(Counter(tag=AllTags.GenericMapGroup,
+                                               # count=len(frame) % 4).qb64b)
+                                #val.extend(mapframe)
+
+                        val = bytearray(Counter(tag=AllTags.GenericListGroup,
+                                                count=len(frame) % 4).qb64b)
+                        val.extend(frame)
+
+
+                    case _:  # if extra fields this is where logic would be
+                        raise SerializeError(f"Unsupported protocol field label"
+                                             f"='{l}' for protocol={self.proto}"
+                                             f" version={self.vrsn}.")
+
+
+                raw.extend(val)
+
+
+        elif self.protocol == Protocols.acdc:
+            for l, val in sad.items():  # assumes valid field order & presence
+                if not fixed:
+                    pass  # prepend label
+
+
+
+        else:
+            raise SerializeError(f"Unsupported protocol={self.proto}.")
+
+
+        # prepend count code for message
+        if fixed:
+
+            val = bytearray(Counter(tag=AllTags.FixedMessageBodyGroup,
+                                    count=len(raw) % 4).qb64b)
+            val.extend(raw)
+        else:
+            pass
+
+
+        return raw
+
+
+
     def compare(self, said=None):
         """Utility method to allow comparison of own .said digest of .raw
         with some other purported said of .raw
 
         Returns:
             success (bool): True if said matches self.saidb  via string
                equality. Converts said to bytes if unicode
@@ -999,44 +1398,74 @@
         Returns:
             sad (dict): serializable attribute dict (saidified data)
         """
         return dict(self._sad)  # return copy
 
 
     @property
+    def genus(self):
+        """genus (CESR genu code) property getter
+
+        Returns:
+            genus (stre): CESR genus code for this Serder
+        """
+        return self._genus
+
+
+    @property
+    def gvrsn(self):
+        """gvrsn (CESR genus version) property getter
+
+        Returns:
+            gvrsn (Versionage): instance, CESR genus code table version for this Serder
+        """
+        return self._gvrsn
+
+
+    @property
     def kind(self):
         """kind property getter
         Returns:
             kind (str): value of Serials (Serialage)"""
         return self._kind
 
 
     @property
     def proto(self):
-        """proto property getter
+        """proto property getter,
         protocol identifier type value of Protocolage such as 'KERI' or 'ACDC'
 
         Returns:
             proto (str): Protocolage value as protocol type
         """
         return self._proto
 
+    @property
+    def protocol(self):
+        """protocp; property getter, alias of .proto
+        protocol identifier type value of Protocolage such as 'KERI' or 'ACDC'
+
+        Returns:
+            protocol (str): Protocolage value as protocol type
+        """
+        return self.proto
+
 
     @property
     def vrsn(self):
         """vrsn (version) property getter
 
         Returns:
             vrsn (Versionage): instance of protocol version for this Serder
         """
         return self._vrsn
 
     @property
     def version(self):
-        """version property getter alias of .vrsn
+        """version property getter, alias of .vrsn
 
         Returns:
             version (Versionage): instance of protocol version for this Serder
         """
         return self.vrsn
 
 
@@ -1051,15 +1480,15 @@
 
     @property
     def said(self):
         """said property getter
         Returns:
            said (str): qb64
         """
-        if not self.Fields[self.proto][self.vrsn][self.ilk].saids.keys() and 'd' in self._sad:
+        if not self.Fields[self.proto][self.vrsn][self.ilk].saids and 'd' in self._sad:
             return self._sad['d']  # special case for non-saidive messages like rct
         return self._said
 
 
     @property
     def saidb(self):
         """saidb property getter
@@ -1082,32 +1511,32 @@
 class SerderKERI(Serder):
     """SerderKERI is Serder subclass with Labels for KERI packet types (ilks) and
        properties for exposing field values of KERI messages
 
        See docs for Serder
     """
     #override in subclass to enforce specific protocol
-    Protocol = Protos.keri  # required protocol, None means any in Protos is ok
-    Proto = Protos.keri  # default protocol type
+    Protocol = Protocols.keri  # required protocol, None means any in Protocols is ok
+    Proto = Protocols.keri  # default protocol type
 
 
 
     def _verify(self, **kwa):
         """Verifies said(s) in sad against raw
         Override for protocol and ilk specific verification behavior. Especially
         for inceptive ilks that have more than one said field like a said derived
         identifier prefix.
 
         Raises a ValidationError (or subclass) if any verification fails
 
         """
         super(SerderKERI, self)._verify(**kwa)
 
-        allkeys = list(self.Fields[self.proto][self.vrsn][self.ilk].alls.keys())
-        keys = list(self.sad.keys())
+        allkeys = list(self.Fields[self.proto][self.vrsn][self.ilk].alls)
+        keys = list(self.sad)
         if allkeys != keys:
             raise ValidationError(f"Invalid top level field list. Expected "
                                   f"{allkeys} got {keys}.")
 
         if (self.vrsn.major < 2 and self.vrsn.minor < 1 and
             self.ilk in (Ilks.qry, Ilks.rpy, Ilks.pro, Ilks.bar, Ilks.exn)):
                 pass
@@ -1444,76 +1873,24 @@
         """
         if self.vrsn.major < 2 and self.vrsn.minor < 1 and self.ilk == Ilks.vcp:
             return self._sad.get("n")
         else:
             return self.uuid
 
 
-class SerderCREL(Serder):
-    """SerderCREL is Serder subclass with Labels for CREL packet types (ilks) and
-       properties for exposing field values of CREL messages
-       Container Registry Event Log for issuance, revocation, etc registries of
-       ACDC
-
-       See docs for Serder
-    """
-    #override in subclass to enforce specific protocol
-    Protocol = Protos.crel  # required protocol, None means any in Protos is ok
-    Proto = Protos.crel  # default protocol type
-    Vrsn = Vrsn_1_1  # default protocol version for protocol type
-
-
-    def _verify(self, **kwa):
-        """Verifies said(s) in sad against raw
-        Override for protocol and ilk specific verification behavior. Especially
-        for inceptive ilks that have more than one said field like a said derived
-        identifier prefix.
-
-        Raises a ValidationError (or subclass) if any verification fails
-
-        """
-        super(SerderCREL, self)._verify(**kwa)
-
-        try:
-            code = Matter(qb64=self.issuer).code
-        except Exception as ex:
-            raise ValidationError(f"Invalid issuer AID = "
-                                  f"{self.issuer}.") from ex
-
-        if code not in PreDex:
-            raise ValidationError(f"Invalid issuer AID code = {code}.")
-
-
-    @property
-    def issuer(self):
-        """
-        Returns:
-           issuer (str): qb64  of .sad["i"] issuer AID property getter
-        """
-        return self._sad.get('i')
-
-
-    @property
-    def issuerb(self):
-        """
-        Returns:
-        issuerb (bytes): qb64b  of .issuer property getter as bytes
-        """
-        return self.issuer.encode("utf-8") if self.issuer is not None else None
-
 
 class SerderACDC(Serder):
     """SerderACDC is Serder subclass with Labels for ACDC packet types (ilks) and
        properties for exposing field values of ACDC messages
 
        See docs for Serder
     """
     #override in subclass to enforce specific protocol
-    Protocol = Protos.acdc  # required protocol, None means any in Protos is ok
-    Proto = Protos.acdc  # default protocol type
+    Protocol = Protocols.acdc  # required protocol, None means any in Protocols is ok
+    Proto = Protocols.acdc  # default protocol type
 
 
 
     def _verify(self, **kwa):
         """Verifies said(s) in sad against raw
         Override for protocol and ilk specific verification behavior. Especially
         for inceptive ilks that have more than one said field like a said derived
```

### Comparing `keri-1.1.9/src/keri/db/basing.py` & `keri-1.2.dev0/src/keri/db/basing.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,42 +14,75 @@
 See _Database.flags() to view the state of those options for an opened database.
 A consequence of the immutability of these flags is that the default non-named
 database will never have these flags set.
 
 So only need to set dupsort first time opened each other opening does not
 need to call it
 """
-
+import importlib
 import os
 import shutil
 from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass, asdict, field
 import json
 
 
 import cbor2 as cbor
 import msgpack
 import lmdb
+import semver
 from ordered_set import OrderedSet as oset
 
 from hio.base import doing
 
+import keri
 from . import dbing, koming, subing
 from .. import kering
 
-from ..core import coring, eventing, parsing, serdering
+from ..core import coring, eventing, parsing, serdering, indexing
 
 from .. import help
 from ..help import helping
 
 
 logger = help.ogler.getLogger()
 
 
+MIGRATIONS = [
+    ("1.1.0", ["rekey_habs"])
+]
+
+
+# ToDo XXXX maybe
+'''
+class komerdict(dict):
+    """
+    Subclass of dict that has db as attribute and employs read through cache
+    from db Baser.stts of kever states to reload kever from state in database
+    when not found in memory as dict item.
+
+    add method that answers is a given pre a group hab pre .localGroup(pre)
+
+    ToDo XXXX change name of dbdict to stateDict since now have differen types
+    and can't subclass dict with init parameters.
+    but can change function by manually assigning attributes but that is ugly
+    need wrapper decorator to do that. So can update attributes with wrapper
+    on class that injects instance attributes when class is instanced
+    one of the injected parameters is function that that maps returned Komer to
+    object class
+    parameters are subdb (must be Komer) and function that maps retrieved dataclass
+    record  from dataabase to class instance. if no mapping function then just
+    return the dataclass record as value.
+    """
+
+'''
+
+
+# ToDo XXXX change name to statedict since not a generic dbdict
 class dbdict(dict):
     """
     Subclass of dict that has db as attribute and employs read through cache
     from db Baser.stts of kever states to reload kever from state in database
     when not found in memory as dict item.
     """
     __slots__ = ('db')  # no .__dict__ just for db reference
@@ -96,14 +129,17 @@
         """
         if not super(dbdict, self).__contains__(k):
             return default
         else:
             return self.__getitem__(k)
 
 
+
+
+
 @dataclass
 class RawRecord:
     """RawRecord is base class for dataclasses that provides private utility
     methods for representing the dataclass as some other format like dict,
     json bytes, cbor bytes, mgpk bytes as a raw format. Typically uses case
     is to transform dataclass into dict or serialization of its transformation
     into dict so that it can be included in messages or stored in a database.
@@ -211,14 +247,26 @@
     bt: str = '0'  # backer threshold hex num str
     b: list = field(default_factory=list)  # backer AID list qb64
     c: list[str] =  field(default_factory=list)  # config trait list
     ee: StateEERecord = field(default_factory=StateEERecord)
     di: str = '' # delegator aid qb64 if any otherwise empty '' str
 
 
+@dataclass
+class EventSourceRecord:  # tracks source of event local or remote
+    """
+    Keyed by dig (said) of serder of event
+
+    Usage:
+
+    """
+    local: bool = True  # True of local (protected) else False for remote (unprotected)
+
+    def __iter__(self):
+        return iter(asdict(self))
 
 
 @dataclass
 class HabitatRecord:  # baser.habs
     """
     Habitat application state information keyed by habitat name (baser.habs)
 
@@ -228,14 +276,16 @@
         smids (list | None): group signing member identifiers qb64 when hid is group
         rmids (list | None): group signing member identifiers qb64 when hid is group
         watchers: (list[str]) = list of id prefixes qb64 of watchers
 
 
     """
     hid: str  # hab own identifier prefix qb64
+    name: str | None = None
+    domain: str | None = None
     mid: str | None = None  # group member identifier qb64 when hid is group
     smids: list | None = None  # group signing member ids when hid is group
     rmids: list | None = None  # group rotating member ids when hid is group
     sid: str | None = None  # Signify identifier qb64 when hid is Signify
     watchers: list[str] = field(default_factory=list)  # id prefixes qb64 of watchers
 
 
@@ -267,15 +317,15 @@
 
     This functionality is aspirational for now. It is likely that we need an
     endpoint identity constraint graph to properly model the endpoint relationship
     permissing constraint structure. For now we just operate with a promiscuous
     constraint policy for endpoint discovery .
 
     Usage:
-        oobiqs: dict[str, OobiQueryRecord] = field(default_factory=dict)
+
     """
     cid: str = None  # qb64
     role: str = None  # one of kering.Roles None is any or all
     eids: list[str] = field(default_factory=list)  # of qb64  empty is any
     scheme: str = None  # one of kering.Schemes None is any or all
 
     def __iter__(self):
@@ -505,14 +555,54 @@
         prefixes (OrderedSet): local prefixes corresponding to habitats for this db
 
         .evts is named sub DB whose values are serialized events
             dgKey
             DB is keyed by identifier prefix plus digest of serialized event
             Only one value per DB key is allowed
 
+        .esrs is named sub DB instance of Komer of EventSourceRecord
+            dgKey
+            DB is keyed by identifier prefix plus digest (said) of serialized event
+            Value is serialized instance of EventSourceRecord dataclass.
+            Only one value per DB key is allowed.
+            Keeps track of the source of the event. When .local is Truthy the
+            event was sourced in a protected way such as being generated
+            locally or via a protected path. When .local is Falsey the event was
+            NOT sourced in a protected way. The value of .local determines what
+            validation logic to run on the event. This database is used to track
+            the source when processing escrows that would otherwise be decoupled
+            from the original source of the event.
+
+        .misfits is named sub DB instance of CesrIoSetSuber for misfit escrows
+            subkey "mfes."
+            snKey
+            DB is keyed by event controller prefix plus sn of serialized event
+            where sn is 32 char hex string with leading zeros
+            Value is serialized qb64b dig (said) of event
+            Misfit escrows are events with remote (nonlocal) sources that are
+            inappropriate (i.e. would be dropped) unless they can be promoted
+            to local source via some extra after the fact authentication.
+            Escrow processing determines if and how to promote event source to
+            local and then reprocess
+
+        .delegables is named sub DB instance of CesrIoSetSuber for delegable escrows
+            subkey "dees."
+            snKey
+            DB is keyed by event controller prefix plus sn of serialized event
+            where sn is 32 char hex string with leading zeros
+            Value is serialized qb64b dig (said) of event
+            Delegable event escrows are events with local delegator that need
+            to be approved via the anchoring of the delegated event seal in
+            the delegator's KEL. Event source must be local. A nonlocal (remote)
+            source for a delegable event of a local delegator must first pass
+            through the misfit escrow and get promoted to local source.
+
+        # delegable events escrows. events with local delegator that need approval
+        self.delegables = subing.CesrIoSetSuber(db=self, subkey='dees.', klas=coring.Diger)
+
         .fels is named sub DB of first seen event log table (FEL) of digests
             that indexes events in first 'seen' accepted order for replay and
             cloning of event log. Only one value per DB key is allowed.
             Provides append only ordering of accepted first seen events.
             Uses first seen order number or fn.
             fnKey
             DB is keyed by identifier prefix plus monotonically increasing first
@@ -538,45 +628,53 @@
             Only one value per DB key is allowed
 
         .sigs is named sub DB of fully qualified indexed event signatures
             dgKey
             DB is keyed by identifier prefix plus digest of serialized event
             More than one value per DB key is allowed
 
-        .wigs is named sub DB of indexed witness signatures of event
-            Witnesses always have nontransferable indetifier prefixes.
+        .wigs is named sub DB of indexed witness signatures of event that may
+            come directly or derived from a witness receipt message.
+            Witnesses always have nontransferable identifier prefixes.
             The index is the offset of the witness into the witness list
             of the most recent establishment event wrt the receipted event.
             dgKey
             DB is keyed by identifier prefix plus digest of serialized event
             More than one value per DB key is allowed
 
         .rcts is named sub DB of event receipt couplets from nontransferable
-            signers. Each couple is concatenation of fully qualified items.
+            signers.
+            These are endorsements from nontrasferable signers who are not witnesses
+            May be watchers or other
+            Each couple is concatenation of fully qualified items.
             These are: non-transferale prefix plus non-indexed event signature
             by that prefix.
             dgKey
             DB is keyed by identifier prefix plus digest of serialized event
             More than one value per DB key is allowed
 
         .ures is named sub DB of unverified event receipt escrowed triples from
             non-transferable signers. Each triple is concatenation of fully
             qualified items. These are: receipted event digest,
             non-transferable receiptor identifier prefix,
             plus nonindexed receipt event signature by that prefix.
+             Used to manage out of order events such as escrowing
+            receipt couple until event receipted shows up.
             snKey
             DB is keyed by receipted event controller prefix plus sn
             of serialized event
             More than one value per DB key is allowed
 
         .vrcs is named sub DB of event validator receipt quadruples from transferable
             signers. Each quadruple is concatenation of  four fully qualified items
             of validator. These are: transferable prefix, plus latest establishment
             event sequence number plus latest establishment event digest,
             plus indexed event signature.
+            These are endorsements by transferable AIDs that are not the controller
+            may be watchers or others.
             When latest establishment event is multisig then there will
             be multiple quadruples one per signing key, each a dup at same db key.
             dgKey
             DB is keyed by identifier prefix plus digest of serialized event
             More than one value per DB key is allowed
 
         .vres is named sub DB of unverified event validator receipt escrowed
@@ -659,15 +757,15 @@
             More than one value per DB key is allowed
 
         .fons is named subDB instance of MatterSuber that maps
             (prefix, digest) e.g. dgKey to fn value (first seen ordinal number) of
             the associated event. So one can lookup event digest, get its fn here
             and then use fn to fetch event by fn from .fels.
 
-        .states (stts) is named subDB instance of SerderSuber that maps a prefix
+        .states (subkey stts.) is named subDB instance of SerderSuber that maps a prefix
             to the latest keystate for that prefix. Used by ._kevers.db for read
             through cache of key state to reload kevers in memory
 
         .habs is named subDB instance of Komer that maps habitat names to habitat
             application state. Includes habitat identifier prefix
             key is habitat name str
             value is serialized HabitatRecord dataclass
@@ -742,14 +840,28 @@
             value is serialized GroupIdentifier dataclass
 
         .mpids is named subDB instance of CesrIoSetSuber mapping payload SAID (of 'e' block)
             to the SAID of the `exn` messages is was contained in.  This aggregates
             identical message bodies across participants in group multisig body trying
             to reach concensus on events or credentials.
 
+        .pubs is CatCesrIoSetSuber with subkey="pubs." of concatenated tuples
+        (qb64 pre, qb64 snh) indexed by qb64 of public key. Maps each signing
+        public key from establishment event to the events's prefix and sequence number
+        so can look up an event by any of its signing keys. Updated by Kever.logEvent
+
+        .digs is CatCesrIoSetSuber with subkey="digs." of of concatenated tuples
+        (qb64 pre, qb64 snh) indexed by qb64 of digest of next signing public key.
+        Maps each next signing public key digest from establishment event to
+        the events's prefix and sequence number so can look up an event by any
+        of its next public signing key digests. Updated by Kever.logEvent
+
+        Missing ToDo XXXX other attributes as sub dbs not documented here
+            such as .wits etc
+
     Properties:
         kevers (dbdict): read through cache of kevers of states for KELs in db
 
     """
 
     def __init__(self, headDirPath=None, reopen=False, **kwa):
         """
@@ -765,15 +877,16 @@
             headDirPath is optional str head directory pathname for main database
                 If not provided use default .HeadDirpath
             mode is int numeric os dir permissions for database directory
             reopen (bool): True means database will be reopened by this init
 
 
         """
-        self.prefixes = oset()
+        self.prefixes = oset()  # should change to hids for hab ids
+        self.groups = oset()  # group hab ids
         self._kevers = dbdict()
         self._kevers.db = self  # assign db for read through cache of kevers
 
         super(Baser, self).__init__(headDirPath=headDirPath, reopen=reopen, **kwa)
 
     @property
     def kevers(self):
@@ -820,80 +933,95 @@
         self.pwes = self.env.open_db(key=b'pwes.', dupsort=True)
         self.uwes = self.env.open_db(key=b'uwes.', dupsort=True)
         self.ooes = self.env.open_db(key=b'ooes.', dupsort=True)
         self.dels = self.env.open_db(key=b'dels.', dupsort=True)
         self.ldes = self.env.open_db(key=b'ldes.', dupsort=True)
         self.qnfs = self.env.open_db(key=b'qnfs.', dupsort=True)
 
+        self.migs = subing.CesrSuber(db=self, subkey="migs.", klas=coring.Dater)
+        self.vers = subing.Suber(db=self, subkey="vers.")
+
+        # event source local (protected) or non-local (remote not protected)
+        self.esrs = koming.Komer(db=self,
+                                   schema=EventSourceRecord,
+                                   subkey='esrs.')
+
+        # misfit escrows whose processing may change the .esrs event source record
+        self.misfits = subing.CesrIoSetSuber(db=self, subkey='mfes.', klas=coring.Diger)
+
+        # delegable events escrows. events with local delegator that need approval
+        self.delegables = subing.CesrIoSetSuber(db=self, subkey='dees.', klas=coring.Diger)
+
         # events as ordered by first seen ordinals
         self.fons = subing.CesrSuber(db=self, subkey='fons.', klas=coring.Seqner)
         # Kever state made of KeyStateRecord key states
+        # TODO: clean
         self.states = koming.Komer(db=self,
                                    schema=KeyStateRecord,
                                    subkey='stts.')
 
         self.wits = subing.CesrIoSetSuber(db=self, subkey="wits.", klas=coring.Prefixer)
 
         # habitat application state keyed by habitat name, includes prefix
         self.habs = koming.Komer(db=self,
                                  subkey='habs.',
                                  schema=HabitatRecord, )
-
-        # habitat application state keyed by habitat namespace + b'\x00' + name, includes prefix
-        self.nmsp = koming.Komer(db=self,
-                                 subkey='nmsp.',
-                                 schema=HabitatRecord, )
+        # habitat name database mapping (domain,name) as key to Prefixer
+        self.names = subing.Suber(db=self, subkey='names.', sep="^")
 
         # SAD support datetime stamps and signatures indexed and not-indexed
         # all sad  sdts (sad datetime serializations) maps said to date-time
         self.sdts = subing.CesrSuber(db=self, subkey='sdts.', klas=coring.Dater)
 
         # all sad ssgs (sad indexed signature serializations) maps SAD quadkeys
         # given by quadruple (saider.qb64, prefixer.qb64, seqner.q64, diger.qb64)
         #  of reply and trans signer's key state est evt to val Siger for each
         # signature.
-        self.ssgs = subing.CesrIoSetSuber(db=self, subkey='ssgs.', klas=coring.Siger)
+        self.ssgs = subing.CesrIoSetSuber(db=self, subkey='ssgs.', klas=indexing.Siger)
 
         # all sad scgs  (sad non-indexed signature serializations) maps SAD SAID
         # to couple (Verfer, Cigar) of nontrans signer of signature in Cigar
         # nontrans qb64 of Prefixer is same as Verfer
         self.scgs = subing.CatCesrIoSetSuber(db=self, subkey='scgs.',
                                              klas=(coring.Verfer, coring.Cigar))
 
         # all reply messages. Maps reply said to serialization. Replys are
         # versioned sads ( with version string) so use Serder to deserialize and
         # use  .sdts, .ssgs, and .scgs for datetimes and signatures
+        # TODO: clean
         self.rpys = subing.SerderSuber(db=self, subkey='rpys.')
 
         # all reply escrows indices of partially signed reply messages. Maps
         # route in reply to single (Saider,)  of escrowed reply.
         # Routes such as /end/role  /loc/schema
         self.rpes = subing.CesrIoSetSuber(db=self, subkey='rpes.',
                                           klas=coring.Saider)
 
         # auth AuthN/AuthZ by controller at cid of endpoint provider at eid
         # maps key=cid.role.eid to val=said of end reply
+        # TODO: clean
         self.eans = subing.CesrSuber(db=self, subkey='eans.', klas=coring.Saider)
 
         # auth AuthN/AuthZ by endpoint provider at eid of location at scheme url
         # maps key=cid.role.eid to val=said of end reply
         self.lans = subing.CesrSuber(db=self, subkey='lans.', klas=coring.Saider)
 
         # service endpoint identifier (eid) auths keyed by controller cid.role.eid
         # data extracted from reply /end/role/add or /end/role/cut
         self.ends = koming.Komer(db=self, subkey='ends.',
                                  schema=EndpointRecord, )
 
-        # service endpont locations keyed by eid.scheme  (endpoint identifier)
+        # service endpoint locations keyed by eid.scheme  (endpoint identifier)
         # data extracted from reply loc
         self.locs = koming.Komer(db=self,
                                  subkey='locs.',
                                  schema=LocationRecord, )
 
         # index of last retrieved message from witness mailbox
+        # TODO: clean
         self.tops = koming.Komer(db=self,
                                  subkey='witm.',
                                  schema=TopicsRecord, )
 
         # group partial signature escrow
         self.gpse = subing.CatCesrIoSetSuber(db=self, subkey='gpse.',
                                              klas=(coring.Seqner, coring.Saider))
@@ -903,65 +1031,74 @@
                                              klas=(coring.Seqner, coring.Saider))
 
         # group partial witness escrow
         self.gpwe = subing.CatCesrIoSetSuber(db=self, subkey='gdwe.',
                                              klas=(coring.Seqner, coring.Saider))
 
         # completed group multisig
+        # TODO: clean
         self.cgms = subing.CesrSuber(db=self, subkey='cgms.',
                                      klas=coring.Saider)
 
         # exchange message partial signature escrow
         self.epse = subing.SerderSuber(db=self, subkey="epse.")
 
         # exchange messages
+        # TODO: clean
         self.exns = subing.SerderSuber(db=self, subkey="exns.")
 
         # Forward pointer to a provided reply message
+        # TODO: clean
         self.erpy = subing.CesrSuber(db=self, subkey="erpy.", klas=coring.Saider)
 
-        # exchange messages
-        self.sxns = subing.SerderSuber(db=self, subkey="sxns.")
-
         # exchange message signatures
-        self.esigs = subing.CesrIoSetSuber(db=self, subkey='esigs.', klas=coring.Siger)
+        # TODO: clean
+        self.esigs = subing.CesrIoSetSuber(db=self, subkey='esigs.', klas=indexing.Siger)
 
         # exchange message signatures
+        # TODO: clean
         self.ecigs = subing.CatCesrIoSetSuber(db=self, subkey='ecigs.',
                                               klas=(coring.Verfer, coring.Cigar))
 
         # exchange pathed attachments
+        # TODO: clean
         self.epath = subing.IoSetSuber(db=self, subkey=".epath")
 
         # accepted signed 12-word challenge response exn messages keys by prefix of signer
+        # TODO: clean
         self.chas = subing.CesrIoSetSuber(db=self, subkey='chas.', klas=coring.Saider)
 
         # successfull signed 12-word challenge response exn messages keys by prefix of signer
+        # TODO: clean
         self.reps = subing.CesrIoSetSuber(db=self, subkey='reps.', klas=coring.Saider)
 
         # authorzied well known OOBIs
+        # TODO: clean
         self.wkas = koming.IoSetKomer(db=self, subkey='wkas.', schema=WellKnownAuthN)
 
         # KSN support datetime stamps and signatures indexed and not-indexed
         # all ksn  kdts (key state datetime serializations) maps said to date-time
+        # TODO: clean
         self.kdts = subing.CesrSuber(db=self, subkey='kdts.', klas=coring.Dater)
 
         # all key state messages. Maps key state said to serialization. ksns are
         # KeyStateRecords so use ._asdict or ._asjson as appropriate
         # use  .kdts, .ksgs, and .kcgs for datetimes and signatures
+        # TODO: clean
         self.ksns = koming.Komer(db=self,
                                 schema=KeyStateRecord,
                                 subkey='ksns.')
-        #self.ksns = subing.SerderSuber(db=self, subkey='ksns.')
 
         # key state SAID database for successfully saved key state notices
         # maps key=(prefix, aid) to val=said of key state
+        # TODO: clean
         self.knas = subing.CesrSuber(db=self, subkey='knas.', klas=coring.Saider)
 
         # config loaded oobis to be processed asynchronously, keyed by oobi URL
+        # TODO: clean
         self.oobis = koming.Komer(db=self,
                                   subkey='oobis.',
                                   schema=OobiRecord,
                                   sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # escrow OOBIs that failed to load, retriable, keyed by oobi URL
         self.eoobi = koming.Komer(db=self,
@@ -972,135 +1109,209 @@
         # OOBIs with outstand client requests.
         self.coobi = koming.Komer(db=self,
                                   subkey='coobi.',
                                   schema=OobiRecord,
                                   sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # Resolved OOBIs (those that have been processed successfully for this database.
+        # TODO: clean
         self.roobi = koming.Komer(db=self,
                                   subkey='roobi.',
                                   schema=OobiRecord,
                                   sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # Well known OOBIs that are to be used for mfa against a resolved OOBI.
+        # TODO: clean
         self.woobi = koming.Komer(db=self,
                                   subkey='woobi.',
                                   schema=OobiRecord,
                                   sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # Well known OOBIs that are to be used for mfa against a resolved OOBI.
+        # TODO: clean
         self.moobi = koming.Komer(db=self,
                                   subkey='moobi.',
                                   schema=OobiRecord,
                                   sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # Multifactor well known OOBI auth records to process.  Keys by controller URL
+        # TODO: clean
         self.mfa = koming.Komer(db=self,
                                 subkey='mfa.',
                                 schema=OobiRecord,
                                 sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # Resolved multifactor well known OOBI auth records.  Keys by controller URL
+        # TODO: clean
         self.rmfa = koming.Komer(db=self,
-                                 subkey='mfa.',
+                                 subkey='rmfa.',
                                  schema=OobiRecord,
                                  sep=">")  # Use seperator not a allowed in URLs so no splitting occurs.
 
         # JSON schema SADs keys by the SAID
+        # TODO: clean
         self.schema = subing.SchemerSuber(db=self,
                                           subkey='schema.')
 
         # Field values for contact information for remote identifiers.  Keyed by prefix/field
+        # TODO: clean
         self.cfld = subing.Suber(db=self,
                                  subkey="cfld.")
 
         # Global settings for the Habery environment
         self.hbys = subing.Suber(db=self, subkey='hbys.')
+
         # Signed contact data, keys by prefix
+        # TODO: clean
         self.cons = subing.Suber(db=self,
                                  subkey="cons.")
 
         # Transferable signatures on contact data
+        # TODO: clean
         self.ccigs = subing.CesrSuber(db=self, subkey='ccigs.', klas=coring.Cigar)
+
         # Chunked image data for contact information for remote identifiers
+        # TODO: clean
         self.imgs = self.env.open_db(key=b'imgs.')
 
         # Delegation escrow dbs #
         # delegated partial witness escrow
         self.dpwe = subing.SerderSuber(db=self, subkey='dpwe.')
 
         # delegated unanchored escrow
         self.dune = subing.SerderSuber(db=self, subkey='dune.')
 
-        # completed group multisig
+        # completed group delegated AIDs
+        # TODO: clean
         self.cdel = subing.CesrSuber(db=self, subkey='cdel.',
                                      klas=coring.Saider)
 
-        # public keys mapped to the AID and event seq no they appeared in
-        self.pubs = subing.CatCesrIoSetSuber(db=self, subkey="pubs.",
-                                             klas=(coring.Prefixer, coring.Seqner))
-
-        # next key digests mapped to the AID and event seq no they appeared in
-        self.digs = subing.CatCesrIoSetSuber(db=self, subkey="digs.",
-                                             klas=(coring.Prefixer, coring.Seqner))
-
         # multisig sig embed payload SAID mapped to containing exn messages across group multisig participants
+        # TODO: clean
         self.meids = subing.CesrIoSetSuber(db=self, subkey="meids.", klas=coring.Saider)
 
         # multisig sig embed payload SAID mapped to group multisig participants AIDs
+        # TODO: clean
         self.maids = subing.CesrIoSetSuber(db=self, subkey="maids.", klas=coring.Prefixer)
 
         self.reload()
 
         return self.env
 
     def reload(self):
         """
         Reload stored prefixes and Kevers from .habs
 
         """
+        # Check migrations to see if this database is up to date.  Error otherwise
+        if not self.current:
+            raise kering.DatabaseError("Database migrations must be run.")
+
         removes = []
         for keys, data in self.habs.getItemIter():
             if (ksr := self.states.get(keys=data.hid)) is not None:
                 try:
                     kever = eventing.Kever(state=ksr,
                                            db=self,
-                                           prefixes=self.prefixes,
                                            local=True)
                 except kering.MissingEntryError as ex:  # no kel event for keystate
                     removes.append(keys)  # remove from .habs
                     continue
                 self.kevers[kever.prefixer.qb64] = kever
                 self.prefixes.add(kever.prefixer.qb64)
+                if data.mid:  # group hab
+                    self.groups.add(data.hid)
+
             elif data.mid is None:  # in .habs but no corresponding key state and not a group so remove
                 removes.append(keys)  # no key state or KEL event for .hab record
 
         for keys in removes:  # remove bare .habs records
             self.habs.rem(keys=keys)
 
-        # Load namespaced Habs
-        removes = []
-        for keys, data in self.nmsp.getItemIter():
-            if (ksr := self.states.get(keys=data.hid)) is not None:
-                try:
-                    kever = eventing.Kever(state=ksr,
-                                           db=self,
-                                           prefixes=self.prefixes,
-                                           local=True)
-                except kering.MissingEntryError as ex:  # no kel event for keystate
-                    removes.append(keys)  # remove from .habs
+    def migrate(self):
+        """ Run all migrations required
+
+        Run all migrations  that are required from the current version of database up to the current version
+         of the software that have not already been run.
+
+         Sets the version of the database to the current version of the software after successful completion
+         of required migrations
+
+        """
+        for (version, migrations) in MIGRATIONS:
+            # Check to see if this is for an older version
+            if self.version is not None and semver.compare(version, self.version) != 1:
+                continue
+
+            for migration in migrations:
+                modName = f"keri.db.migrations.{migration}"
+                if self.migs.get(keys=(migration,)) is not None:
                     continue
-                self.kevers[kever.prefixer.qb64] = kever
-                self.prefixes.add(kever.prefixer.qb64)
-            elif data.mid is None:  # in .habs but no corresponding key state and not a group so remove
-                removes.append(keys)  # no key state or KEL event for .hab record
 
-        for keys in removes:  # remove bare .habs records
-            self.nmsp.rem(keys=keys)
+                mod = importlib.import_module(modName)
+                try:
+                    print(f"running migration {modName}")
+                    mod.migrate(self)
+                except Exception as e:
+                    print(f"\nAbandoning migration {migration} with error: {e}")
+                    return
+
+                self.migs.pin(keys=(migration,), val=coring.Dater())
 
+        self.version = keri.__version__
+
+    @property
+    def current(self):
+        """ Current property determines if we are at the current database migration state.
+
+         If the database version matches the library version return True
+         If the current database version is behind the current library version, check for migrations
+            - If there are migrations to run, return False
+            - If there are no migrations to run, reset database version to library version and return True
+         If the current database version is ahead of the current library version, raise exception
+
+         """
+        if self.version == keri.__version__:
+            return True
+
+        # If database version is ahead of library version, throw exception
+        if self.version is not None and semver.compare(self.version, keri.__version__) == 1:
+            raise kering.ConfigurationError(
+                f"Database version={self.version} is ahead of library version={keri.__version__}")
+
+        last = MIGRATIONS[-1]
+        # If we aren't at latest version, but there are no outstanding migrations, reset version to latest
+        if self.migs.get(keys=(last[1][0],)) is not None:
+            return True
+
+        # We have migrations to run
+        return False
+
+    def complete(self, name=None):
+        """ Returns list of tuples of migrations completed with date of completion
+
+        Parameters:
+            name(str): optional name of migration to check completeness
+
+        Returns:
+            list: tuples of migration,date of completed migration names and the date of completion
+
+        """
+        migrations = []
+        if not name:
+            for version, migs in MIGRATIONS:
+                for mig in migs:
+                    dater = self.migs.get(keys=(mig,))
+                    migrations.append((mig, dater))
+        else:
+            if name not in MIGRATIONS or not self.migs.get(keys=(name,)):
+                raise ValueError(f"No migration named {name}")
+            migrations.append((name, self.migs.get(keys=(name,))))
+
+        return migrations
 
     def clean(self):
         """
         Clean database by creating re-verified cleaned cloned copy
         and then replacing original with cleaned cloned copy
 
         Database usage should be offline during cleaning as it will be cloned in
@@ -1108,15 +1319,15 @@
 
         """
         # create copy to clone into
         with openDB(name=self.name,
                     temp=self.temp,
                     headDirPath=self.headDirPath,
                     perm=self.perm,
-                    clean=True) as copy:
+                    clean=True) as copy:  # copy is Baser instance
 
             with reopenDB(db=self, reuse=True, readonly=True):  # reopen as readonly
                 if not os.path.exists(self.path):
                     raise ValueError("Error while cleaning, no orig at {}."
                                      "".format(self.path))
 
                 kvy = eventing.Kevery(db=copy)  # promiscuous mode
@@ -1126,35 +1337,62 @@
                 # need new method cloneObjAllPreIter()
                 # process event doesn't capture exceptions so we can more easily
                 # detect in the cloning that some events did not make it through
                 psr = parsing.Parser(kvy=kvy)
                 for msg in self.cloneAllPreIter():  # clone into copy
                     psr.parseOne(ims=msg)
 
+                # This is the list of non-set based databases that are not created as part of event processing.
+                # for now we are just copying them from self to copy without worrying about being able to
+                # reprocess them.  We need a more secure method in the future
+                unsecured = ["hbys", "schema", "states", "rpys", "eans", "tops", "cgms", "exns", "erpy",
+                             "kdts", "ksns", "knas", "oobis", "roobi", "woobi", "moobi", "mfa", "rmfa",
+                             "cfld", "cons", "ccigs", "cdel", "migs"]
+
+                for name in unsecured:
+                    srcdb = getattr(self, name)
+                    cpydb = getattr(copy, name)
+                    for keys, val in srcdb.getItemIter():
+                        cpydb.put(keys=keys, val=val)
+
+                # This is the list of set based databases that are not created as part of event processing.
+                # for now we are just copying them from self to copy without worrying about being able to
+                # reprocess them.  We need a more secure method in the future
+                sets = ["esigs", "ecigs", "epath", "chas", "reps", "wkas", "meids", "maids"]
+                for name in sets:
+                    srcdb = getattr(self, name)
+                    cpydb = getattr(copy, name)
+                    for keys, val in srcdb.getItemIter():
+                        cpydb.add(keys=keys, val=val)
+
+                # Insecure raw imgs database copy.
+                for (key, val) in self.getAllItemIter(self.imgs):
+                    copy.imgs.setVal(key=key, val=val)
+
                 # clone .habs  habitat name prefix Komer subdb
                 # copy.habs = koming.Komer(db=copy, schema=HabitatRecord, subkey='habs.')  # copy
                 for keys, val in self.habs.getItemIter():
                     if val.hid in copy.kevers:  # only copy habs that verified
                         copy.habs.put(keys=keys, val=val)
+                        ns = "" if val.domain is None else val.domain
+                        copy.names.put(keys=(ns, val.name), val=val.hid)
                         copy.prefixes.add(val.hid)
-
-                if not copy.habs.get(keys=(self.name,)):
-                    raise ValueError("Error cloning habs, missing orig name={}."
-                                     "".format(self.name))
+                        if val.mid:  # a group hab
+                            copy.groups.add(val.hid)
 
                 # clone .ends and .locs databases
-                for keys, val in self.ends.getItemIter():
+                for (cid, role, eid), val in self.ends.getItemIter():
                     exists = False  # only copy if entries in both .ends and .locs
                     for scheme in ("https", "http", "tcp"):  # all supported schemes
-                        lval = self.locs.get(keys=(val.eid, scheme))
-                        if lval and lval.cid == keys[0] and lval.role == keys[1]:
+                        lval = self.locs.get(keys=(eid, scheme))
+                        if lval:
                             exists = True  # loc with matching cid and rol
-                            copy.locs.put(keys=(val.eid, scheme), val=lval)
+                            copy.locs.put(keys=(eid, scheme), val=lval)
                     if exists:  # only copy end if has at least one matching loc
-                        copy.ends.put(keys=keys, vals=[val])
+                        copy.ends.put(keys=(cid, role, eid), val=val)
 
             # remove own db directory replace with clean clone copy
             if os.path.exists(self.path):
                 shutil.rmtree(self.path)
 
             dst = shutil.move(copy.path, self.path)  # move copy back to orig
             if not dst:  # move failed leave new in place so can manually fix
@@ -1169,24 +1407,27 @@
 
             # replace prefixes with cloned copy prefixes
 
             # clear and clone .prefixes
             self.prefixes.clear()
             self.prefixes.update(copy.prefixes)
 
+            # clear and clone .gids
+            self.groups.clear()
+            self.groups.update(copy.groups)
+
             with reopenDB(db=self, reuse=True):  # make sure can reopen
                 if not isinstance(self.env, lmdb.Environment):
                     raise ValueError("Error cloning, unable to reopen."
                                      "".format(self.path))
 
         # clone success so remove if still there
         if os.path.exists(copy.path):
             shutil.rmtree(copy.path)
 
-
     def clonePreIter(self, pre, fn=0):
         """
         Returns iterator of first seen event messages with attachments for the
         identifier prefix pre starting at first seen order number, fn.
         Essentially a replay in first seen order with attachments
         """
         if hasattr(pre, 'encode'):
@@ -1256,22 +1497,24 @@
         # add authorizer (delegator/issuer) source seal event couple to attachments
         couple = self.getAes(dgkey)
         if couple is not None:
             atc.extend(coring.Counter(code=coring.CtrDex.SealSourceCouples,
                                       count=1).qb64b)
             atc.extend(couple)
 
-        # add trans receipts quadruples to attachments
+        # add trans endorsement quadruples to attachments not controller
+        # may have been originally key event attachments or receipted endorsements
         if quads := self.getVrcs(key=dgkey):
             atc.extend(coring.Counter(code=coring.CtrDex.TransReceiptQuadruples,
                                       count=len(quads)).qb64b)
             for quad in quads:
                 atc.extend(quad)
 
-        # add nontrans receipts couples to attachments
+        # add nontrans endorsement couples to attachments not witnesses
+        # may have been originally key event attachments or receipted endorsements
         if coups := self.getRcts(key=dgkey):
             atc.extend(coring.Counter(code=coring.CtrDex.NonTransReceiptCouples,
                                       count=len(coups)).qb64b)
             for coup in coups:
                 atc.extend(coup)
 
         # add first seen replay couple to attachments
@@ -1282,15 +1525,15 @@
         atc.extend(coring.Seqner(sn=fn).qb64b)
         atc.extend(coring.Dater(dts=bytes(dts)).qb64b)
 
         # prepend pipelining counter to attachments
         if len(atc) % 4:
             raise ValueError("Invalid attachments size={}, nonintegral"
                              " quadlets.".format(len(atc)))
-        pcnt = coring.Counter(code=coring.CtrDex.AttachedMaterialQuadlets,
+        pcnt = coring.Counter(code=coring.CtrDex.AttachmentGroup,
                               count=(len(atc) // 4)).qb64b
         msg.extend(pcnt)
         msg.extend(atc)
         return msg
 
 
     def cloneDelegation(self, kever):
@@ -1298,18 +1541,18 @@
         Recursively clone delegation chain from AID of Kever if one exits.
 
         Parameters:
             kever (Kever): Kever from which to clone the delegator's AID.
 
         """
         if kever.delegated:
-            dkever = self.kevers[kever.delegator]
+            dkever = self.kevers[kever.delpre]
             yield from self.cloneDelegation(dkever)
 
-            for dmsg in self.clonePreIter(pre=kever.delegator, fn=0):
+            for dmsg in self.clonePreIter(pre=kever.delpre, fn=0):
                 yield dmsg
 
 
     def findAnchoringSealEvent(self, pre, seal, sn=0):
         """
         Search through a KEL for the event that contains a specific anchored
         SealEvent type of provided seal but in dict form and is also fully
@@ -1322,23 +1565,23 @@
         Parameters:
             pre (bytes|str): identifier of the KEL to search
             seal (dict): dict form of Seal of any type SealEvent to find in anchored
                 seals list of each event
             sn (int): beginning sn to search
 
         """
-        if tuple(seal.keys()) != eventing.SealEvent._fields:  # wrong type of seal
+        if tuple(seal) != eventing.SealEvent._fields:  # wrong type of seal
             return None
 
         seal = eventing.SealEvent(**seal)  #convert to namedtuple
 
         for evt in self.getEvtPreIter(pre=pre, sn=sn):  # includes disputed & superseded
             srdr = serdering.SerderKERI(raw=evt.tobytes())
             for eseal in srdr.seals or []:
-                if tuple(eseal.keys()) == eventing.SealEvent._fields:
+                if tuple(eseal) == eventing.SealEvent._fields:
                     eseal = eventing.SealEvent(**eseal)  # convert to namedtuple
                     if seal == eseal and self.fullyWitnessed(srdr):
                         return srdr
         return None
 
 
     def findAnchoringSeal(self, pre, seal, sn=0):
@@ -1354,149 +1597,57 @@
             pre (bytes|str): identifier of the KEL to search
             seal (dict): dict form of Seal of any type to find in anchored
                 seals list of each event
             sn (int): beginning sn to search
 
         """
         # create generic Seal namedtuple class using keys from provided seal dict
-        Seal = namedtuple('Seal', seal.keys())  # matching type
+        Seal = namedtuple('Seal', list(seal))  # matching type
 
         for evt in self.getEvtLastPreIter(pre=pre, sn=sn):  # only last evt at sn
             srdr = serdering.SerderKERI(raw=evt.tobytes())
             for eseal in srdr.seals or []:
-                if tuple(eseal.keys()) == Seal._fields:  # same type of seal
+                if tuple(eseal) == Seal._fields:  # same type of seal
                     eseal = Seal(**eseal)  #convert to namedtuple
                     if seal == eseal and self.fullyWitnessed(srdr):
                         return srdr
         return None
 
-
-
-    def findAnchoringSealEventClone(self, pre, seal):
-        """
-        Search through a KEL for the event that contains a specific anchored
-        SealEvent type of provided seal but in dict form.
-        Returns the Serder of the first event with the anchored SealEvent seal,
-            None if not found
-        Searchs from inception forward
-
-        Parameters:
-            pre is qb64 identifier of the KEL to search
-            seal is dict form of SealEvent to find in anchored seals list of each event
-
-        """
-        if tuple(seal.keys()) != eventing.SealEvent._fields:  # wrong type of seal
-            return None
-            #raise ValueError(f"Expected SealEvent got {seal}.")
-
-        seal = eventing.SealEvent(**seal)  #convert to namedtuple
-
-        # getEvtPreIter getEvtLastPreIter
-
-        for evt in self.clonePreIter(pre=pre):  # all events including superseded
-            srdr = serdering.SerderKERI(raw=evt)
-            for eseal in srdr.seals or []:
-                if tuple(eseal.keys()) == eventing.SealEvent._fields:
-                    eseal = eventing.SealEvent(**eseal)  #convert to namedtuple
-                    if seal == eseal and self.fullyWitnessed(srdr):
-                        return srdr
-                #spre = anc["i"]
-                #ssn = int(anc["s"], 16)
-                #sdig = anc["d"]
-
-                #if spre == seal["i"] and ssn == int(seal["s"], 16) \
-                        #and seal["d"] == sdig and self.fullyWitnessed(srdr):
-                    #return srdr
-
-        return None
-
-
-    def findAnchoringSealClone(self, pre, seal):
-        """
-        Search through a KEL for the event that contains an anchored
-        Seal with same Seal type as provided seal but in dict form.
-        Returns the Serder of the first event with the anchored Seal seal,
-            None if not found
-        Searchs from inception forward
-
-        Parameters:
-            pre is qb64 identifier of the KEL to search
-            seal is dict form of Seal of any type to find in anchored seals list of each event
-
-        """
-        # create generic Seal namedtuple class using keys from provided seal dict
-        Seal = namedtuple('Seal', seal.keys())  # matching type
-
-        # getEvtPreIter getEvtLastPreIter
-
-        for evt in self.clonePreIter(pre=pre):  # all events including superseded
-            srdr = serdering.SerderKERI(raw=evt)
-            for eseal in srdr.seals or []:
-                if tuple(eseal.keys()) == Seal._fields:  # same type of seal
-                    eseal = Seal(**eseal)  #convert to namedtuple
-                    if seal == eseal and self.fullyWitnessed(srdr):
-                        return srdr
-        return None
-
-
     def signingMembers(self, pre: str):
         """ Find signing members of a multisig group aid.
 
         Using the pubs index to find members of a signing group
 
         Parameters:
             pre (str): qb64 identifier prefix to find members
 
         Returns:
             list: qb64 identifier prefixes of signing members for provided aid
 
         """
-        members = []
-        if pre not in self.kevers:
-            return members
-
-        kever = self.kevers[pre]
-        for verfer in kever.verfers:
-            if (couples := self.pubs.get(keys=(verfer.qb64,))) is None:
-                continue
-
-            for couple in couples:
-                prefixer, seqner = couple
-                if prefixer.qb64 != pre:  # Rule out aid being queried
-                    members.append(prefixer.qb64)
-
-        return members
+        if (habord := self.habs.get(keys=(pre,))) is None:
+            return None
 
+        return habord.smids
 
     def rotationMembers(self, pre: str):
         """ Find rotation members of a multisig group aid.
 
         Using the digs index to lookup member pres of a group aid
 
         Parameters:
             pre (str): qb64 identifier prefix to find members
 
         Returns:
             list: qb64 identifier prefixes of rotation members for provided aid
         """
-        members = []
-        if pre not in self.kevers:
-            return members
-
-        kever = self.kevers[pre]
-        for diger in kever.ndigers:
-            if (couples := self.digs.get(keys=(diger.qb64,))) is None:
-                continue
-
-            for couple in couples:
-                prefixer, seqner = couple
-                if prefixer.qb64 != pre:  # Rule out aid being queried
-                    members.append(prefixer.qb64)
+        if (habord := self.habs.get(keys=(pre,))) is None:
+            return None
 
-        return members
+        return habord.rmids
 
     def fullyWitnessed(self, serder):
         """ Verify the witness threshold on the event
 
         Parameters:
             serder (Serder): event serder to validate witness threshold
```

### Comparing `keri-1.1.9/src/keri/db/dbing.py` & `keri-1.2.dev0/src/keri/db/dbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,23 @@
 import shutil
 import stat
 from collections import abc
 from contextlib import contextmanager
 from typing import Union
 
 import lmdb
-from  ordered_set import OrderedSet as oset
-
-from hio.base import filing
-
+from ordered_set import OrderedSet as oset
 from hio.base import filing
 
+import keri
+from ..kering import MaxON  # maximum ordinal number for seqence or first seen
 from ..help import helping
 
 ProemSize = 32  # does not include trailing separator
 MaxProem = int("f"*(ProemSize), 16)
-MaxON = int("f"*32, 16)  # largest possible ordinal number, sequence or first seen
-
 SuffixSize = 32  # does not include trailing separator
 MaxSuffix = int("f"*(SuffixSize), 16)
 
 def dgKey(pre, dig):
     """
     Returns bytes DB key from concatenation of '.' with qualified Base64 prefix
     bytes pre and qualified Base64 bytes digest of serialized event
@@ -303,15 +300,14 @@
     AltCleanTailDirPath = ".keri/clean/db"
     TempHeadDir = "/tmp"
     TempPrefix = "keri_lmdb_"
     TempSuffix = "_test"
     Perm = stat.S_ISVTX | stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR  # 0o1700==960
     MaxNamedDBs = 96
 
-
     def __init__(self, readonly=False, **kwa):
         """
         Setup main database directory at .dirpath.
         Create main database environment at .env using .path.
 
         Parameters:
             name (str): directory path name differentiator directory/file
@@ -340,19 +336,20 @@
             mode (str): File open mode when filed
             fext (str): File extension when filed
 
             readonly (bool): True means open database in readonly mode
                                 False means open database in read/write mode
 
         """
+
         self.env = None
+        self._version = None
         self.readonly = True if readonly else False
         super(LMDBer, self).__init__(**kwa)
 
-
     def reopen(self, readonly=False, **kwa):
         """
         Open if closed or close and reopen if opened or create and open if not
         if not preexistent, directory path for lmdb at .path and then
         Open lmdb and assign to .env
 
         Parameters:
@@ -370,25 +367,59 @@
             clean (bool): True means path uses clean tail variant
                              False means path uses normal tail variant
             mode (str): file open mode when .filed
             fext (str): File extension when .filed
             readonly (bool): True means open database in readonly mode
                                 False means open database in read/write mode
         """
+        exists = self.exists(name=self.name, base=self.base)
         opened = super(LMDBer, self).reopen(**kwa)
         if readonly is not None:
             self.readonly = readonly
 
         # open lmdb major database instance
         # creates files data.mdb and lock.mdb in .dbDirPath
         self.env = lmdb.open(self.path, max_dbs=self.MaxNamedDBs, map_size=104857600,
                              mode=self.perm, readonly=self.readonly)
+
         self.opened = True if opened and self.env else False
+
+        if self.opened and not self.readonly and (not exists or self.temp):
+            self.version = keri.__version__
+
         return self.opened
 
+    @property
+    def version(self):
+        """ Return the version of database stored in __version__ key.
+
+        This value is read through cached in memory
+
+        Returns:
+            str: the version of the database or None if not set in the database
+
+        """
+        if self._version is None:
+            self._version = self.getVer()
+
+        return self._version
+
+    @version.setter
+    def version(self, val):
+        """  Set the version of the database in memory and in the __version__ key
+
+        Parameters:
+            val (str): The new semver formatted version of the database
+
+        """
+        if hasattr(val, "decode"):
+            val = val.decode("utf-8")  # convert bytes to str
+
+        self._version = val
+        self.setVer(self._version)
 
     def close(self, clear=False):
         """
         Close lmdb at .env and if clear or .temp then remove lmdb directory at .path
         Parameters:
            clear is boolean, True means clear lmdb directory
         """
@@ -396,16 +427,41 @@
             try:
                 self.env.close()
             except:
                 pass
 
         self.env = None
 
-        return(super(LMDBer, self).close(clear=clear))
+        return super(LMDBer, self).close(clear=clear)
+
+    def getVer(self):
+        """ Returns the value of the the semver formatted version in the __version__ key in this database
+
+        Returns:
+            str: semver formatted version of the database
+
+        """
+        with self.env.begin() as txn:
+            cursor = txn.cursor()
+            version = cursor.get(b'__version__')
+            return version.decode("utf-8") if version is not None else None
+
+    def setVer(self, val):
+        """  Set the version of the database in the __version__ key
+
+        Parameters:
+            val (str): The new semver formatted version of the database
+
+        """
+        if hasattr(val, "encode"):
+            val = val.encode("utf-8")  # convert str to bytes
 
+        with self.env.begin(write=True) as txn:
+            cursor = txn.cursor()
+            cursor.replace(b'__version__', val)
 
     # For subdbs with no duplicate values allowed at each key. (dupsort==False)
     def putVal(self, db, key, val):
         """
         Write serialized bytes val to location key in db
         Does not overwrite.
         Returns True If val successfully written Else False
```

### Comparing `keri-1.1.9/src/keri/db/escrowing.py` & `keri-1.2.dev0/src/keri/db/escrowing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 keri.core.escrowing module
 
 """
 import datetime
 import logging
 from typing import Type
 
-from keri.core import coring
-from keri import help
+
 from keri import kering
-from keri.core import eventing
-from keri.db import subing
+from keri import help
 from keri.help import helping
 
+from keri.core import coring, eventing, indexing
+from keri.db import subing
+
+
 logger = help.ogler.getLogger()
 
 
 class Broker:
 
     def __init__(self, db, subkey, timeout=3600):
         self.db = db
@@ -38,15 +40,15 @@
                                    #schema=viring.RegStateRecord,
                                    #subkey=subkey + '-sns.')
 
         # all key state ksgs (ksn indexed signature serializations) maps ksn quadkeys
         # given by quadruple (saider.qb64, subkeyer.qb64, seqner.q64, diger.qb64)
         #  of reply and trans signer's key state est evt to val Siger for each
         # signature.
-        self.tigerdb = subing.CesrIoSetSuber(db=self.db, subkey=subkey + '-sgs.', klas=coring.Siger)
+        self.tigerdb = subing.CesrIoSetSuber(db=self.db, subkey=subkey + '-sgs.', klas=indexing.Siger)
 
         # all key state kcgs  (ksn non-indexed signature serializations) maps ksn SAID
         # to couple (Verfer, Cigar) of nontrans signer of signature in Cigar
         # nontrans qb64 of subkeyer is same as Verfer
         self.cigardb = subing.CatCesrIoSetSuber(db=self.db, subkey=subkey + '-cgs.',
                                                 klas=(coring.Verfer, coring.Cigar))
```

### Comparing `keri-1.1.9/src/keri/db/koming.py` & `keri-1.2.dev0/src/keri/db/koming.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/db/subing.py` & `keri-1.2.dev0/src/keri/db/subing.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,36 +55,41 @@
     Provides common methods for subclasses
     Do not instantiate but use a subclass
 
     Attributes:
         db (dbing.LMDBer): base LMDB db
         sdb (lmdb._Database): instance of lmdb named sub db for this Suber
         sep (str): separator for combining keys tuple of strs into key bytes
+        verify (bool): some subclasses want to re-verify when deser from db
+                       default false
     """
     Sep = '.'  # separator for combining key iterables
 
     def __init__(self, db: dbing.LMDBer, *,
                        subkey: str='docs.',
                        dupsort: bool=False,
                        sep: str=None,
+                       verify: bool=False,
                        **kwa):
         """
         Parameters:
             db (dbing.LMDBer): base db
             subkey (str):  LMDB sub database key
             dupsort (bool): True means enable duplicates at each key
                                False (default) means do not enable duplicates at
                                each key
             sep (str): separator to convert keys iterator to key bytes for db key
                        default is self.Sep == '.'
         """
-        super(SuberBase, self).__init__()
+        super(SuberBase, self).__init__()  # for multi inheritance
         self.db = db
         self.sdb = self.db.env.open_db(key=subkey.encode("utf-8"), dupsort=dupsort)
         self.sep = sep if sep is not None else self.Sep
+        self.verify = True if verify else False
+
 
 
     def _tokey(self, keys: Union[str, bytes, memoryview, Iterable],
                 top: bool=False):
         """
         Converts keys to key str with proper separators and returns key bytes.
         If keys is already str then returns. Else If keys is iterable (non-str)
@@ -274,15 +279,15 @@
 
 
 class CesrSuberBase(SuberBase):
     """
     Sub class of Suber where data is CESR encode/decode ducktyped subclass
     instance such as Matter, Indexer, Counter with .qb64b property when provided
     as fully qualified serialization
-    Automatically serializes and deserializes from qb64b to/from CESR instances
+    Automatically serializes and deserializes from qb64b to/from CESR instance
 
     """
 
     def __init__(self, *pa, klas: Type[coring.Matter] = coring.Matter, **kwa):
         """
         Parameters:
             db (dbing.LMDBer): base db
@@ -315,15 +320,15 @@
 
 
 class CesrSuber(CesrSuberBase, Suber):
     """
     Sub class of Suber where data is CESR encode/decode ducktyped subclass
     instance such as Matter, Indexer, Counter with .qb64b property when provided
     as fully qualified serialization.
-    Extents Suber to support val that are ducktyped CESR serializable .qb64 .qb64b
+    Extends Suber to support val that are ducktyped CESR serializable .qb64 .qb64b
     subclasses such as coring.Matter, coring.Indexer, coring.Counter.
     Automatically serializes and deserializes from qb64b to/from CESR instances
 
     """
 
     def __init__(self, *pa, **kwa):
         """
@@ -505,16 +510,16 @@
         that is not already in set of vals at key. Does not overwrite.
 
         Parameters:
             keys (Iterable): of key strs to be combined in order to form key
             val (Union[bytes, str]): serialization
 
         Returns:
-            result (bool): True means unique value among duplications,
-                              False means duplicte of same value already exists.
+            result (bool): True means unique value added among duplications,
+                            False means duplicate of same value already exists.
 
         """
         return (self.db.addIoSetVal(db=self.sdb,
                                     key=self._tokey(keys),
                                     val=self._ser(val),
                                     sep=self.sep))
 
@@ -738,18 +743,17 @@
         """
         return self.db.delIoSetIokey(db=self.sdb, iokey=self._tokey(iokeys))
 
 
 class CesrIoSetSuber(CesrSuberBase, IoSetSuber):
     """
     Subclass of CesrSuber and IoSetSuber.
-    Class whose values stored in db are a concatenation of the  .qb64b property
-    from one or more  subclass instances (qb64b is bytes of fully qualified
-    serialization) that support CESR encode/decode ducktyped subclass instance
-    such as Matter, Indexer, Counter
+    Sub class of Suber where data is CESR encode/decode ducktyped subclass
+    instance such as Matter, Indexer, Counter with .qb64b property when provided
+    as fully qualified serialization
     Automatically serializes and deserializes from qb64b to/from CESR instances
 
     Extends IoSetSuber with mixin methods ._ser and ._des from CesrSuberBase
     so that all IoSetSuber methods now work with CESR subclass for each val.
 
     IoSetSuber stores at each effective key a set of distinct values that
     share that same effective key where each member of the set is retrieved in
@@ -777,16 +781,16 @@
             db (dbing.LMDBer): base db
             subkey (str):  LMDB sub database key
             dupsort (bool): True means enable duplicates at each key
                                False (default) means do not enable duplicates at
                                each key
             sep (str): separator to convert keys iterator to key bytes for db key
                        default is self.Sep == '.'
-            klas (Iterable): of Class references to subclasses of Matter, each
-                of to Type[coring.Matter]
+            klas (Type[coring.Matter]): Class reference to subclass of Matter or
+                Indexer or Counter or any ducktyped class of Matter
 
         """
         super(CesrIoSetSuber, self).__init__(*pa, **kwa)
 
 
 
 class CatCesrIoSetSuber(CatCesrSuberBase, IoSetSuber):
@@ -1110,15 +1114,15 @@
             Use walrus operator to catch and raise missing entry
             if (srder := mydb.get(keys)) is None:
                 raise ExceptionHere
             use srdr here
 
         """
         val = self.db.getVal(db=self.sdb, key=self._tokey(keys))
-        return self.klas(raw=bytes(val)) if val is not None else None
+        return self.klas(raw=bytes(val), verify=self.verify) if val is not None else None
 
 
     def rem(self, keys: Union[str, Iterable]):
         """
         Removes entry at keys
 
         Parameters:
@@ -1142,15 +1146,15 @@
             keys (Iterator): tuple of bytes or strs that may be a truncation of
                 a full keys tuple in  in order to get all the items from
                 multiple branches of the key space. If keys is empty then gets
                 all items in database.
 
         """
         for iokey, val in self.db.getTopItemIter(db=self.sdb, key=self._tokey(keys)):
-            yield self._tokeys(iokey), self.klas(raw=bytes(val))
+            yield self._tokeys(iokey), self.klas(raw=bytes(val), verify=self.verify)
 
 
 class SchemerSuber(Suber):
     """
     Sub class of Suber where data is serialized Schemer instance
     Automatically serializes and deserializes using Schemer methods
```

### Comparing `keri-1.1.9/src/keri/demo/demo_bob.py` & `keri-1.2.dev0/src/keri/demo/demo_bob.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/demo/demo_eve.py` & `keri-1.2.dev0/src/keri/demo/demo_eve.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/demo/demo_kev.py` & `keri-1.2.dev0/src/keri/demo/demo_kev.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/demo/demo_sam.py` & `keri-1.2.dev0/src/keri/demo/demo_sam.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/demo/demoing.py` & `keri-1.2.dev0/src/keri/demo/demoing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/end/ending.py` & `keri-1.2.dev0/src/keri/end/ending.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import falcon
 from hio import base
 from hio.core import http, wiring
 
 from .. import help
 from .. import kering
 from ..app import habbing
-from ..core import coring
+from ..core import coring, indexing
 from ..help import helping
 
 logger = help.ogler.getLogger()
 
 Mimage = namedtuple("Mimage", "json mgpk cbor cesr")
 
 Mimes = Mimage(json="application/json",
@@ -78,20 +78,20 @@
 
     Parameters:
         signages (list): items are Signage namedtuples,
                            (markers, indexed, signer, ordinal, kind)
             where:
                 markers (Union[list, dict]): When dict each item (key, val) has
                     key as str identifier of marker and has val as instance of
-                    either coring.Siger or coring.Cigar.
-                    When list each item is instance of either coring.Siger or
+                    either indexing.Siger or coring.Cigar.
+                    When list each item is instance of either indexing.Siger or
                     coring.Cigar.
                     All markers must be of same class
                 indexed (bool): True means marker values are indexed signatures
-                    using coring.Siger. False means marker values are unindexed
+                    using indexing.Siger. False means marker values are unindexed
                     signatures using coring.Cigar. None means auto detect from
                     first marker value class. All markers must be of same class.
                 signer (str): optional identifier of signage. May be a
                     multi-sig group identifier. Default is None. When None or
                     empty signer is not included in header value
                 ordinal (str): optional ordinal hex str of int that is an ordinal
                                such as sequence number to further identify the
@@ -184,20 +184,20 @@
 
     Returns:
        signages (list): items are Signage namedtuples,
                            (markers, indexed, signer, ordinal, kind)
             where:
                 markers (Union[list, dict]): When dict each item (key, val) has
                     key as str identifier of marker and has val as instance of
-                    either coring.Siger or coring.Cigar.
-                    When list each item is instance of either coring.Siger or
+                    either indexing.Siger or coring.Cigar.
+                    When list each item is instance of either indexing.Siger or
                     coring.Cigar.
                     All markers must be of same class
                 indexed (bool): True means marker values are indexed signatures
-                    using coring.Siger. False means marker values are unindexed
+                    using indexing.Siger. False means marker values are unindexed
                     signatures using coring.Cigar. None means auto detect from
                     first marker value class. All markers must be of same class.
                 signer (str): optional identifier of signage. May be a
                     multi-sig group identifier. Default is None. When None or
                     empty signer is not included in header value
                 ordinal (str): optional ordinal hex str of int that is an ordinal
                                such as sequence number to further identify the
@@ -216,15 +216,15 @@
         items = {}
         for item in value.split(";"):
             key, val = item.split("=", maxsplit=1)
             items[key] = val.strip('"')
 
         if "indexed" not in items:
             raise ValueError("Missing indexed field in Signature header signage.")
-        indexed = items["indexed"] not in kering.FALSEY  # make bool
+        indexed = items["indexed"] not in helping.FALSEY  # make bool
         del items["indexed"]
 
         if "signer" in items:
             signer = items["signer"]
             del items["signer"]
         else:
             signer = None
@@ -246,15 +246,15 @@
             del items["kind"]
         else:
             kind = "CESR"  # default is empty or missing
 
         if kind == "CESR":  # convert to Siger or Cigar instances
             for key, val in items.items():
                 if indexed:
-                    items[key] = coring.Siger(qb64=val)
+                    items[key] = indexing.Siger(qb64=val)
                 else:
                     items[key] = coring.Cigar(qb64=val)
 
         signages.append(Signage(markers=items, indexed=indexed, signer=signer,
                                 ordinal=ordinal, digest=digest, kind=kind))
 
     return signages
```

### Comparing `keri-1.1.9/src/keri/end/priming.py` & `keri-1.2.dev0/src/keri/end/priming.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/help/__init__.py` & `keri-1.2.dev0/src/keri/help/__init__.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/peer/exchanging.py` & `keri-1.2.dev0/src/keri/peer/exchanging.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         if not atc:
             continue
 
         pathed = bytearray()
         pather = coring.Pather(path=["e", label])
         pathed.extend(pather.qb64b)
         pathed.extend(atc)
-        end.extend(coring.Counter(code=coring.CtrDex.PathedMaterialQuadlets,
+        end.extend(coring.Counter(code=coring.CtrDex.PathedMaterialGroup,
                                   count=(len(pathed) // 4)).qb64b)
         end.extend(pathed)
 
     if e:
         e["d"] = ""
         _, e = coring.Saider.saidify(sad=e, label=coring.Saids.d)
 
@@ -407,25 +407,25 @@
                 raise ValueError("Attempt to use tranferable prefix={} for "
                                  "receipt.".format(cigar.verfer.qb64))
             atc.extend(cigar.verfer.qb64b)
             atc.extend(cigar.qb64b)
 
     # Smash the pathed components on the end
     for p in hby.db.epath.get(keys=(exn.said,)):
-        atc.extend(coring.Counter(code=coring.CtrDex.PathedMaterialQuadlets,
+        atc.extend(coring.Counter(code=coring.CtrDex.PathedMaterialGroup,
                                   count=(len(p) // 4)).qb64b)
         atc.extend(p.encode("utf-8"))
 
     msg = bytearray()
 
     if pipelined:
         if len(atc) % 4:
             raise ValueError("Invalid attachments size={}, nonintegral"
                              " quadlets.".format(len(atc)))
-        msg.extend(coring.Counter(code=coring.CtrDex.AttachedMaterialQuadlets,
+        msg.extend(coring.Counter(code=coring.CtrDex.AttachmentGroup,
                                   count=(len(atc) // 4)).qb64b)
 
     msg.extend(atc)
     return msg
 
 
 def nesting(paths, acc, val):
```

### Comparing `keri-1.1.9/src/keri/vc/protocoling.py` & `keri-1.2.dev0/src/keri/vc/protocoling.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/vc/proving.py` & `keri-1.2.dev0/src/keri/vc/proving.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         version (Version): version instance
         kind (Serials): serialization kind
 
     Returns:
         SerderACDC: credential instance
 
     """
-    vs = versify(proto=coring.Protos.acdc, version=version, kind=kind, size=0)
+    vs = versify(protocol=coring.Protocols.acdc, version=version, kind=kind, size=0)
 
     vc = dict(
         v=vs,
         d="",
     )
 
     subject = dict(
```

### Comparing `keri-1.1.9/src/keri/vc/walleting.py` & `keri-1.2.dev0/src/keri/vc/walleting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/vdr/credentialing.py` & `keri-1.2.dev0/src/keri/vdr/credentialing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.9/src/keri/vdr/eventing.py` & `keri-1.2.dev0/src/keri/vdr/eventing.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 from  ordered_set import OrderedSet as oset
 
 from hio.help import decking
 
 from keri import kering
 from .. import core
 from .. import help
-from ..core import serdering, coring
+from ..core import serdering, coring, indexing
 from ..core.coring import (MtrDex, Serials, versify, Prefixer,
-                           Ilks, Seqner, Verfer)
-from ..core.eventing import SealEvent, ample, TraitDex, verifySigs, validateSN
+                           Ilks, Seqner, Verfer, Number)
+from ..core.eventing import SealEvent, ample, TraitDex, verifySigs
 from ..db import basing, dbing
 from ..db.dbing import dgKey, snKey
 from ..help import helping
 from ..kering import (MissingWitnessSignatureError, Version,
                       MissingAnchorError, ValidationError, OutOfOrderError, LikelyDuplicitousError)
-from ..kering import (VCP_LABELS, VRT_LABELS, ISS_LABELS, BIS_LABELS, REV_LABELS,
-                      BRV_LABELS, TSN_LABELS, CRED_TSN_LABELS)
 from ..vdr import viring
 
 logger = help.ogler.getLogger()
 
 
 def incept(
         pre,
@@ -640,15 +638,15 @@
     """
     Tever is KERI/ACDC transaction event log verifier class
     Only supports current version VERSION
 
     Has the following public attributes and properties:
 
     Class Attributes:
-        .NoBackers is Boolean
+        .NoRegistrarBackers is Boolean
                 True means do not allow backers (default to witnesses of controlling KEL)
                 False means allow backers (ignore witnesses of controlling KEL)
 
     Attributes:
         .db is reference to Baser instance that managers the LMDB database
         .reg is regerence to Registry instance that manages VC LMDB database
         .regk is fully qualified base64 identifier prefix of own Registry if any
@@ -662,15 +660,15 @@
         .toad is int threshold of accountable duplicity
         .baks is list of qualified qb64 aids for backers
         .cuts is list of qualified qb64 aids for backers cut from prev wits list
         .adds is list of qualified qb64 aids for backers added to prev wits list
         .noBackers is boolean trait True means do not allow backers
 
     """
-    NoBackers = False
+    NoRegistrarBackers = False
 
     def __init__(self, cues=None, rsr=None, serder=None, seqner=None, saider=None,
                  bigers=None, db=None, reger=None, noBackers=None, estOnly=None,
                  regk=None, local=False):
         """ Create incepting tever and state from registry inception serder
 
         Create incepting tever and state from registry inception serder
@@ -714,19 +712,19 @@
         self.regk = regk
 
         ilk = serder.ked["t"]
         if ilk not in [Ilks.vcp]:
             raise ValidationError("Expected ilk {} got {} for evt: {}".format(Ilks.vcp, ilk, serder))
 
         self.ilk = ilk
-        labels = VCP_LABELS
-        for k in labels:
-            if k not in serder.ked:
-                raise ValidationError("Missing element = {} from {} event for "
-                                      "evt = {}.".format(k, ilk, serder.ked))
+        #labels = VCP_LABELS
+        #for k in labels:
+            #if k not in serder.ked:
+                #raise ValidationError("Missing element = {} from {} event for "
+                                      #"evt = {}.".format(k, ilk, serder.ked))
 
         self.incept(serder=serder)
         self.config(serder=serder, noBackers=noBackers, estOnly=estOnly)
 
         bigers = self.valAnchorBigs(serder=serder,
                                     seqner=seqner,
                                     saider=saider,
@@ -822,16 +820,17 @@
         ked = serder.ked
         self.pre = ked["ii"]
         self.prefixer = Prefixer(qb64=serder.pre)
         if not self.prefixer.verify(ked=ked, prefixed=True):  # invalid prefix
             raise ValidationError("Invalid prefix = {} for registry inception evt = {}."
                                   .format(self.prefixer.qb64, ked))
 
-        sn = ked["s"]
-        self.sn = validateSN(sn, inceptive=True)
+        #sn = ked["s"]
+        #self.sn = validateSN(sn, inceptive=True)
+        self.sn = Number(numh=ked["s"]).validate(inceptive=True).sn
 
         self.cuts = []  # always empty at inception since no prev event
         self.adds = []  # always empty at inception since no prev event
         baks = ked["b"]
         if len(oset(baks)) != len(baks):
             raise ValidationError("Invalid baks = {}, has duplicates for evt = {}."
                                   "".format(baks, ked))
@@ -860,15 +859,15 @@
             noBackers (bool): override flag for specifying a registry with no additional backers
                               beyond the controlling KEL's witnesses
 
 
         """
         # assign traits
         self.noBackers = (True if (noBackers if noBackers is not None
-                                   else self.NoBackers)
+                                   else self.NoRegistrarBackers)
                           else False)  # ensure default noBackers is boolean
 
         self.estOnly = (True if (estOnly if estOnly is not None
                                    else False)
                           else False)  # ensure default estOnly is boolean
 
         cnfg = serder.ked["c"]  # process cnfg for traits
@@ -891,20 +890,21 @@
                 Index is offset into wits list of associated witness nontrans pre
                 from which public key may be derived.
 
         """
 
         ked = serder.ked
         ilk = ked["t"]
-        sn = ked["s"]
+        #sn = ked["s"]
 
         icp = ilk in (Ilks.iss, Ilks.bis)
 
         # validate SN for
-        sn = validateSN(sn, inceptive=icp)
+        #sn = validateSN(sn, inceptive=icp)
+        sn = Number(numh=ked["s"]).validate(inceptive=icp).sn
 
         if ilk in (Ilks.vrt,):
             if self.noBackers is True:
                 raise ValidationError("invalid rotation evt {} against backerless registry {}".
                                       format(ked, self.regk))
 
             toad, baks, cuts, adds = self.rotate(serder, sn=sn)
@@ -957,16 +957,16 @@
 
         """
 
         ked = serder.ked
         ilk = ked["t"]
         dig = ked["p"]
 
-        # XXXX should there be validation of labels here
-        labels = VRT_LABELS  # assumes ilk == Ilks.vrt
+
+        #labels = VRT_LABELS  # assumes ilk == Ilks.vrt
         #for k in labels:
             #if k not in ked:
                 #raise ValidationError("Missing element = {} from {} event for "
                                       #"evt = {}.".format(k, ilk, ked))
 
         if serder.pre != self.prefixer.qb64:
             raise ValidationError("Mismatch event aid prefix = {} expecting"
@@ -1047,20 +1047,19 @@
         """
 
         ked = serder.ked
         vcpre = ked["i"]
         ilk = ked["t"]
         vci = vcpre
 
-        labels = ISS_LABELS if ilk == Ilks.iss else BIS_LABELS
-
-        for k in labels:
-            if k not in ked:
-                raise ValidationError("Missing element = {} from {} event for "
-                                      "evt = {}.".format(k, ilk, ked))
+        #labels = ISS_LABELS if ilk == Ilks.iss else BIS_LABELS
+        #for k in labels:
+            #if k not in ked:
+                #raise ValidationError("Missing element = {} from {} event for "
+                                      #"evt = {}.".format(k, ilk, ked))
 
         if ilk == Ilks.iss:  # simple issue
             if self.noBackers is False:
                 raise ValidationError("invalid simple issue evt {} against backer based registry {}".
                                       format(ked, self.regk))
 
             regi = ked["ri"]
@@ -1114,20 +1113,19 @@
 
         """
 
         ked = serder.ked
         vcpre = ked["i"]
         ilk = ked["t"]
 
-        labels = REV_LABELS if ilk == Ilks.rev else BRV_LABELS
-
-        for k in labels:
-            if k not in ked:
-                raise ValidationError("Missing element = {} from {} event for "
-                                      "evt = {}.".format(k, ilk, ked))
+        #labels = REV_LABELS if ilk == Ilks.rev else BRV_LABELS
+        #for k in labels:
+            #if k not in ked:
+                #raise ValidationError("Missing element = {} from {} event for "
+                                      #"evt = {}.".format(k, ilk, ked))
 
         # have to compare with VC issuance serder
         vci = vcpre
 
         dig = self.reger.getTel(snKey(pre=vci, sn=sn - 1))
         ievt = self.reger.getTvt(dgKey(pre=vci, dig=dig))
         if ievt is None:
@@ -1539,21 +1537,22 @@
         except Exception:  # if unsupported code or bad size raises error
             raise ValidationError("Invalid pre = {} for evt = {}."
                                   "".format(serder.pre, ked))
 
         regk = self.registryKey(serder)
         pre = serder.pre
         ked = serder.ked
-        sn = ked["s"]
+        #sn = ked["s"]
         ilk = ked["t"]
 
         inceptive = ilk in (Ilks.vcp, Ilks.iss, Ilks.bis)
 
         # validate SN for
-        sn = validateSN(sn, inceptive=inceptive)
+        #sn = validateSN(sn, inceptive=inceptive)
+        sn = Number(numh=ked["s"]).validate(inceptive=inceptive).sn
 
         if not self.lax:
             if self.local:
                 if regk not in self.registries:  # nonlocal event when in local mode
                     raise ValueError("Nonlocal event regk={} when local mode for registries={}."
                                      "".format(regk, self.registries))
             else:
@@ -2056,15 +2055,15 @@
                     raise ValidationError("Missing escrowed evt at dig = {}."
                                           "".format(bytes(digb)))
 
                 tserder = serdering.SerderKERI(raw=bytes(traw))  # escrowed event
 
                 bigers = None
                 if tibs := self.reger.getTibs(key=dgkey):
-                    bigers = [coring.Siger(qb64b=tib) for tib in tibs]
+                    bigers = [indexing.Siger(qb64b=tib) for tib in tibs]
 
                 couple = self.reger.getAnc(dgkey)
                 if couple is None:
                     logger.info("Tevery unescrow error: Missing anchor at."
                                 "dig = %s\n", bytes(digb))
 
                     raise ValidationError("Missing escrowed anchor at dig = {}."
@@ -2123,15 +2122,15 @@
                     raise ValidationError("Missing escrowed evt at dig = {}."
                                           "".format(bytes(digb)))
 
                 tserder = serdering.SerderKERI(raw=bytes(traw))  # escrowed event
 
                 bigers = None
                 if tibs := self.reger.getTibs(key=dgkey):
-                    bigers = [coring.Siger(qb64b=tib) for tib in tibs]
+                    bigers = [indexing.Siger(qb64b=tib) for tib in tibs]
 
                 couple = self.reger.getAnc(dgkey)
                 if couple is None:
                     logger.info("Tevery unescrow error: Missing anchor at."
                                 "dig = %s\n", bytes(digb))
 
                     raise MissingAnchorError("Missing escrowed anchor at dig = {}."
```

### Comparing `keri-1.1.9/src/keri/vdr/verifying.py` & `keri-1.2.dev0/src/keri/vdr/verifying.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
 
         # Look up indicies
         saider = coring.Saider(qb64=creder.said)
         self.reger.saved.pin(keys=saider.qb64b, val=saider)
         self.reger.issus.add(keys=issuer, val=saider)
         self.reger.schms.add(keys=schema, val=saider)
 
-        if 'i' in creder.attrib:
+        if not isinstance(creder.attrib, str) and 'i' in creder.attrib:
             subject = creder.attrib["i"].encode("utf-8")
             self.reger.subjs.add(keys=subject, val=saider)
 
     def query(self, pre, regk, vcid, *, dt=None, dta=None, dtb=None, **kwa):
         """ Returns query message for querying registry
         """
```

### Comparing `keri-1.1.9/src/keri/vdr/viring.py` & `keri-1.2.dev0/src/keri/vdr/viring.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from dataclasses import dataclass, field, asdict
 from  ordered_set import OrderedSet as oset
 
 from ..db import koming, subing, escrowing
 
 from .. import kering
 from ..app import signing
-from ..core import coring, serdering
+from ..core import coring, serdering, indexing
 from ..db import dbing, basing
 from ..db.dbing import snKey
 from ..help import helping
 from ..vc import proving
 from ..vdr import eventing
 
 
@@ -324,15 +324,15 @@
         self.cancs = subing.CatCesrSuber(db=self, subkey='cancs.',
                                          klas=(coring.Prefixer, coring.Seqner, coring.Saider))
 
         # all sad path ssgs (sad pathed indexed signature serializations) maps SAD quinkeys
         # given by quintuple (saider.qb64, path, prefixer.qb64, seqner.q64, diger.qb64)
         # of credential and trans signer's key state est evt to val Siger for each
         # signature.
-        self.spsgs = subing.CesrIoSetSuber(db=self, subkey='ssgs.', klas=coring.Siger)
+        self.spsgs = subing.CesrIoSetSuber(db=self, subkey='ssgs.', klas=indexing.Siger)
 
         # all sad path scgs  (sad pathed non-indexed signature serializations) maps
         # couple (SAD SAID, path) to couple (Verfer, Cigar) of nontrans signer of signature in Cigar
         # nontrans qb64 of Prefixer is same as Verfer
         self.spcgs = subing.CatCesrIoSetSuber(db=self, subkey='scgs.',
                                               klas=(coring.Verfer, coring.Cigar))
 
@@ -436,15 +436,15 @@
                     pre=prefixer.qb64,
                     sn=seqner.sn,
                     d=asaider.qb64
                 )
             )
 
             ctr = coring.Counter(qb64b=iss, strip=True)
-            if ctr.code == coring.CtrDex.AttachedMaterialQuadlets:
+            if ctr.code == coring.CtrDex.AttachmentGroup:
                 ctr = coring.Counter(qb64b=iss, strip=True)
 
             if ctr.code == coring.CtrDex.SealSourceCouples:
                 coring.Seqner(qb64b=iss, strip=True)
                 saider = coring.Saider(qb64b=iss)
 
                 anc = db.cloneEvtMsg(pre=creder.issuer, fn=0, dig=saider.qb64b)
@@ -537,15 +537,15 @@
                                       count=1).qb64b)
             atc.extend(couple)
 
         # prepend pipelining counter to attachments
         if len(atc) % 4:
             raise ValueError("Invalid attachments size={}, nonintegral"
                              " quadlets.".format(len(atc)))
-        pcnt = coring.Counter(code=coring.CtrDex.AttachedMaterialQuadlets,
+        pcnt = coring.Counter(code=coring.CtrDex.AttachmentGroup,
                               count=(len(atc) // 4)).qb64b
         msg.extend(pcnt)
         msg.extend(atc)
         return msg
 
     def sources(self, db, creder):
         """ Returns raw bytes of any source ('e') credential that is in our database
@@ -1005,12 +1005,12 @@
 
     """
 
     craw = bytearray(creder.raw)
     if len(proof) % 4:
         raise ValueError("Invalid attachments size={}, nonintegral"
                          " quadlets.".format(len(proof)))
-    craw.extend(coring.Counter(code=coring.CtrDex.AttachedMaterialQuadlets,
+    craw.extend(coring.Counter(code=coring.CtrDex.AttachmentGroup,
                                count=(len(proof) // 4)).qb64b)
     craw.extend(proof)
 
     return craw
```

### Comparing `keri-1.1.9/src/keri.egg-info/PKG-INFO` & `keri-1.2.dev0/src/keri.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.1.9
+Version: 1.2.dev0
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/WebOfTrust/keripy/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10.4
+Requires-Python: >=3.12.2
 License-File: LICENSE
-Requires-Dist: lmdb>=1.3.0
-Requires-Dist: pysodium>=0.7.12
-Requires-Dist: blake3>=0.3.1
-Requires-Dist: msgpack>=1.0.4
-Requires-Dist: cbor2>=5.4.3
-Requires-Dist: multidict>=6.0.2
+Requires-Dist: lmdb>=1.4.1
+Requires-Dist: pysodium>=0.7.17
+Requires-Dist: blake3>=0.4.1
+Requires-Dist: msgpack>=1.0.8
+Requires-Dist: cbor2>=5.6.2
+Requires-Dist: multidict>=6.0.5
 Requires-Dist: ordered-set>=4.1.0
-Requires-Dist: hio>=0.6.9
+Requires-Dist: hio>=0.6.12
 Requires-Dist: multicommand>=1.0.0
-Requires-Dist: jsonschema>=4.17.0
-Requires-Dist: falcon>=3.1.0
-Requires-Dist: hjson>=3.0.2
-Requires-Dist: PyYaml>=6.0
-Requires-Dist: apispec>=6.0.0
-Requires-Dist: mnemonic>=0.20
-Requires-Dist: PrettyTable>=3.5.0
-Requires-Dist: http_sfv>=0.9.8
-Requires-Dist: cryptography>=39.0.2
+Requires-Dist: jsonschema>=4.21.1
+Requires-Dist: falcon>=3.1.3
+Requires-Dist: hjson>=3.1.0
+Requires-Dist: PyYaml>=6.0.1
+Requires-Dist: apispec>=6.6.0
+Requires-Dist: mnemonic>=0.21
+Requires-Dist: PrettyTable>=3.10.0
+Requires-Dist: http_sfv>=0.9.9
+Requires-Dist: cryptography>=42.0.5
+Requires-Dist: semver>=3.0.2
 
 KERI Decentralized Key Management Infrastructure
```

### Comparing `keri-1.1.9/src/keri.egg-info/SOURCES.txt` & `keri-1.2.dev0/src/keri.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/keri/app/signaling.py
 src/keri/app/signing.py
 src/keri/app/specing.py
 src/keri/app/storing.py
 src/keri/app/cli/__init__.py
 src/keri/app/cli/kli.py
 src/keri/app/cli/commands/__init__.py
+src/keri/app/cli/commands/clean.py
 src/keri/app/cli/commands/escrow.py
 src/keri/app/cli/commands/export.py
 src/keri/app/cli/commands/incept.py
 src/keri/app/cli/commands/init.py
 src/keri/app/cli/commands/interact.py
 src/keri/app/cli/commands/kevers.py
 src/keri/app/cli/commands/list.py
@@ -80,14 +81,18 @@
 src/keri/app/cli/commands/ipex/offer.py
 src/keri/app/cli/commands/ipex/spurn.py
 src/keri/app/cli/commands/local/__init__.py
 src/keri/app/cli/commands/local/watch.py
 src/keri/app/cli/commands/mailbox/__init__.py
 src/keri/app/cli/commands/mailbox/debug.py
 src/keri/app/cli/commands/mailbox/update.py
+src/keri/app/cli/commands/migrate/__init__.py
+src/keri/app/cli/commands/migrate/list.py
+src/keri/app/cli/commands/migrate/run.py
+src/keri/app/cli/commands/migrate/show.py
 src/keri/app/cli/commands/multisig/__init__.py
 src/keri/app/cli/commands/multisig/continue.py
 src/keri/app/cli/commands/multisig/demo.py
 src/keri/app/cli/commands/multisig/incept.py
 src/keri/app/cli/commands/multisig/interact.py
 src/keri/app/cli/commands/multisig/join.py
 src/keri/app/cli/commands/multisig/notice.py
@@ -109,42 +114,42 @@
 src/keri/app/cli/commands/vc/export.py
 src/keri/app/cli/commands/vc/list.py
 src/keri/app/cli/commands/vc/revoke.py
 src/keri/app/cli/commands/vc/registry/__init__.py
 src/keri/app/cli/commands/vc/registry/incept.py
 src/keri/app/cli/commands/vc/registry/list.py
 src/keri/app/cli/commands/vc/registry/status.py
-src/keri/app/cli/commands/watcher/__init__.py
-src/keri/app/cli/commands/watcher/list.py
-src/keri/app/cli/commands/watcher/start.py
-src/keri/app/cli/commands/watcher/update.py
 src/keri/app/cli/commands/witness/__init__.py
 src/keri/app/cli/commands/witness/demo.py
 src/keri/app/cli/commands/witness/start.py
 src/keri/app/cli/commands/witness/submit.py
 src/keri/app/cli/common/__init__.py
 src/keri/app/cli/common/config.py
 src/keri/app/cli/common/displaying.py
 src/keri/app/cli/common/existing.py
 src/keri/app/cli/common/incepting.py
 src/keri/app/cli/common/rotating.py
 src/keri/app/cli/common/terming.py
 src/keri/core/__init__.py
 src/keri/core/coring.py
+src/keri/core/counting.py
 src/keri/core/eventing.py
+src/keri/core/indexing.py
 src/keri/core/parsing.py
 src/keri/core/routing.py
 src/keri/core/scheming.py
 src/keri/core/serdering.py
 src/keri/db/__init__.py
 src/keri/db/basing.py
 src/keri/db/dbing.py
 src/keri/db/escrowing.py
 src/keri/db/koming.py
 src/keri/db/subing.py
+src/keri/db/migrations/__init__.py
+src/keri/db/migrations/rekey_habs.py
 src/keri/demo/__init__.py
 src/keri/demo/demo_bob.py
 src/keri/demo/demo_eve.py
 src/keri/demo/demo_kev.py
 src/keri/demo/demo_sam.py
 src/keri/demo/demoing.py
 src/keri/end/__init__.py
@@ -158,8 +163,9 @@
 src/keri/vc/protocoling.py
 src/keri/vc/proving.py
 src/keri/vc/walleting.py
 src/keri/vdr/__init__.py
 src/keri/vdr/credentialing.py
 src/keri/vdr/eventing.py
 src/keri/vdr/verifying.py
-src/keri/vdr/viring.py
+src/keri/vdr/viring.py
+tests/test_kering.py
```

