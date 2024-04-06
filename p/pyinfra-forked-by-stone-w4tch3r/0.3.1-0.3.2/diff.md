# Comparing `tmp/pyinfra_forked_by_stone-w4tch3r-0.3.1.tar.gz` & `tmp/pyinfra_forked_by_stone-w4tch3r-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinfra_forked_by_stone-w4tch3r-0.3.1.tar", last modified: Fri Apr  5 21:01:35 2024, max compression
+gzip compressed data, was "pyinfra_forked_by_stone-w4tch3r-0.3.2.tar", last modified: Sat Apr  6 14:57:11 2024, max compression
```

## Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1.tar` & `pyinfra_forked_by_stone-w4tch3r-0.3.2.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.611055 pyinfra_forked_by_stone-w4tch3r-0.3.1/
--rw-rw-r--   0 user1     (1000) user1     (1000)     1659 2024-04-05 21:01:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/CHANGELOG.md
--rw-rw-r--   0 user1     (1000) user1     (1000)     1076 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/LICENSE.md
--rw-rw-r--   0 user1     (1000) user1     (1000)       59 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/MANIFEST.in
--rw-r--r--   0 user1     (1000) user1     (1000)     8076 2024-04-05 21:01:35.611055 pyinfra_forked_by_stone-w4tch3r-0.3.1/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4526 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/README.md
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.575039 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/
--rw-rw-r--   0 user1     (1000) user1     (1000)      535 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)       47 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/__main__.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.579041 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/
--rw-rw-r--   0 user1     (1000) user1     (1000)      942 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9748 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/arguments.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2254 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/arguments_typed.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     7176 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/command.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4221 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/config.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1416 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/connect.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      544 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/connectors.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2756 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/deploy.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1861 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/exceptions.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10282 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/facts.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    13164 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/host.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     7663 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/inventory.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    14374 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/operation.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10942 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/operations.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    12622 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/state.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11977 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.579041 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3756 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/base.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5931 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/chroot.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8964 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/docker.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8919 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/dockerssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6929 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/local.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    21018 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/ssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3683 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/ssh_util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.583043 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/sshuserclient/
--rw-rw-r--   0 user1     (1000) user1     (1000)       44 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/sshuserclient/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9720 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/sshuserclient/client.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2721 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/sshuserclient/config.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3617 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/terraform.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11321 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4722 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/vagrant.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3394 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/context.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.587045 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/
--rw-rw-r--   0 user1     (1000) user1     (1000)      347 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      482 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/apk.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1999 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/apt.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2266 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/brew.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      490 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/bsdinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      531 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/cargo.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      703 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/choco.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1666 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/deb.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      862 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/dnf.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1678 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/docker.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11475 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      473 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/gem.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1294 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/git.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3729 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/gpg.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11402 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/hardware.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3374 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/iptables.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      668 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/launchd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      337 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/lxd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5936 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/mysql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      674 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/npm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1350 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/openrc.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1001 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/pacman.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      702 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/pip.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      452 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/pkg.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      481 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/pkgin.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4146 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/postgres.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      187 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/postgresql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1973 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/rpm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4272 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/selinux.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    19982 2024-04-05 20:59:46.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/server.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1910 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/snap.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3927 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/systemd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1490 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/sysvinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      543 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/upstart.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.587045 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/
--rw-rw-r--   0 user1     (1000) user1     (1000)      521 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      730 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/databases.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1161 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/packaging.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2561 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/win_files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      591 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/vzctl.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      481 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/xbps.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      827 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/yum.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      766 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/zypper.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2751 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/local.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.595048 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/
--rw-rw-r--   0 user1     (1000) user1     (1000)      357 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2068 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/apk.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    13621 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/apt.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5086 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/brew.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1598 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/bsdinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1061 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/cargo.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1472 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/choco.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5546 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/dnf.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    53012 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1089 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/gem.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11669 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/git.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9180 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/iptables.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1134 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/launchd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1727 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/lxd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    19530 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/mysql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1430 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/npm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1530 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/openrc.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1691 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pacman.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5771 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pip.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2248 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pkg.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1949 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pkgin.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9401 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/postgres.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      797 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/postgresql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      811 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/puppet.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1959 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/python.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5768 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/selinux.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    36016 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/server.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3006 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/snap.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5563 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/ssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3866 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/systemd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4028 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/sysvinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1928 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/upstart.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.595048 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/
--rw-rw-r--   0 user1     (1000) user1     (1000)      366 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3521 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8637 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/packaging.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1146 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/service.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3067 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/vzctl.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1465 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/xbps.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5548 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/yum.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5477 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/zypper.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4193 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/progress.py
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/py.typed
--rw-rw-r--   0 user1     (1000) user1     (1000)      153 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/version.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.595048 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/
--rw-rw-r--   0 user1     (1000) user1     (1000)      284 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      881 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/__main__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1832 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/commands.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4806 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/exceptions.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9513 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/inventory.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2201 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/log.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    19715 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/main.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11859 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/prints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6322 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2466 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/virtualenv.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.603052 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/
--rw-r--r--   0 user1     (1000) user1     (1000)     8076 2024-04-05 21:01:35.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4839 2024-04-05 21:01:35.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2024-04-05 21:01:35.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)      471 2024-04-05 21:01:35.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/entry_points.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)      884 2024-04-05 21:01:35.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       26 2024-04-05 21:01:35.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)      381 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/pyproject.toml
--rw-rw-r--   0 user1     (1000) user1     (1000)      663 2024-04-05 21:01:35.611055 pyinfra_forked_by_stone-w4tch3r-0.3.1/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)     4714 2024-04-05 20:59:32.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/setup.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.599050 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.599050 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2413 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1961 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_arguments.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3204 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_command.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      708 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_config.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4200 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_deploys.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10687 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_facts.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1119 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_host.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2013 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_inventory.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    20162 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_operations.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1716 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.599050 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6045 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4858 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli_deploy.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3088 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli_exceptions.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2562 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli_util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2130 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_context_objects.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      338 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 21:01:35.603052 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5907 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_chroot.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6566 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_docker.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9303 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_dockerssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     7442 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_local.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    38399 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_ssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5734 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_sshuserclient.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3743 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_terraform.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4647 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3646 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_vagrant.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3308 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_facts.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1696 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_global_arguments.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6074 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_operations.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      557 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_operations_utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.414672 pyinfra_forked_by_stone-w4tch3r-0.3.2/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1700 2024-04-06 14:56:55.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/CHANGELOG.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1076 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/LICENSE.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)       59 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/MANIFEST.in
+-rw-r--r--   0 user1     (1000) user1     (1000)     8076 2024-04-06 14:57:11.414672 pyinfra_forked_by_stone-w4tch3r-0.3.2/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4526 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/README.md
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.382658 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      535 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)       47 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/__main__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.386660 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      942 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9748 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/arguments.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2254 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/arguments_typed.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7176 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/command.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4221 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/config.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1416 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/connect.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      544 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/connectors.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2756 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/deploy.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1861 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/exceptions.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10282 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/facts.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    13164 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/host.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7663 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/inventory.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    14374 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/operation.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10942 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/operations.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    12622 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/state.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11977 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.386660 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3756 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/base.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5931 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/chroot.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8964 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/docker.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8919 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/dockerssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6929 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/local.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    21018 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/ssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3683 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/ssh_util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.386660 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/sshuserclient/
+-rw-rw-r--   0 user1     (1000) user1     (1000)       44 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/sshuserclient/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9720 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/sshuserclient/client.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2721 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/sshuserclient/config.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3617 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/terraform.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11321 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4722 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/vagrant.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3394 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/context.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.394663 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      347 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      482 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/apk.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1999 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/apt.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2266 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/brew.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      490 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/bsdinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      531 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/cargo.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      703 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/choco.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1666 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/deb.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      862 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/dnf.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1678 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/docker.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    12247 2024-04-06 14:55:31.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      473 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/gem.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1294 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/git.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3729 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/gpg.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11402 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/hardware.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3374 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/iptables.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      668 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/launchd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      337 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/lxd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5936 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/mysql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      674 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/npm.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1350 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/openrc.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1001 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/pacman.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      702 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/pip.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      452 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/pkg.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      481 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/pkgin.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4146 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/postgres.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      187 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/postgresql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1973 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/rpm.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4272 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/selinux.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    19982 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/server.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1910 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/snap.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3927 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/systemd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1490 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/sysvinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      543 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/upstart.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.394663 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      521 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      730 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/databases.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1161 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/packaging.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2561 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/win_files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      591 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/vzctl.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      481 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/xbps.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      827 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/yum.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      766 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/zypper.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2751 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/local.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.398665 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      357 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2068 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/apk.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    13621 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/apt.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5086 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/brew.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1598 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/bsdinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1061 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/cargo.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1472 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/choco.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5546 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/dnf.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    53019 2024-04-06 14:55:38.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1089 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/gem.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11669 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/git.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9180 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/iptables.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1134 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/launchd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1727 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/lxd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    19530 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/mysql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1430 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/npm.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1530 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/openrc.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1691 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pacman.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5771 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pip.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2248 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pkg.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1949 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pkgin.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9401 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/postgres.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      797 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/postgresql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      811 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/puppet.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1959 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/python.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5768 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/selinux.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    36016 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/server.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3006 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/snap.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5563 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/ssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3866 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/systemd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4028 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/sysvinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1928 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/upstart.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.402667 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      366 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3521 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8637 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/packaging.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1146 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/service.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3067 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/vzctl.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1465 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/xbps.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5548 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/yum.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5477 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/zypper.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4193 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/progress.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/py.typed
+-rw-rw-r--   0 user1     (1000) user1     (1000)      153 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/version.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.402667 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      284 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      881 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/__main__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1832 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/commands.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4806 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/exceptions.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9513 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/inventory.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2201 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/log.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    19715 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/main.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11859 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/prints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6322 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2466 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/virtualenv.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.410670 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/
+-rw-r--r--   0 user1     (1000) user1     (1000)     8076 2024-04-06 14:57:11.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4839 2024-04-06 14:57:11.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2024-04-06 14:57:11.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      471 2024-04-06 14:57:11.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/entry_points.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      884 2024-04-06 14:57:11.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       26 2024-04-06 14:57:11.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      381 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/pyproject.toml
+-rw-rw-r--   0 user1     (1000) user1     (1000)      663 2024-04-06 14:57:11.414672 pyinfra_forked_by_stone-w4tch3r-0.3.2/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4714 2024-04-06 14:55:25.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.402667 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.406668 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2413 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1961 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_arguments.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3204 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_command.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      708 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_config.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4200 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_deploys.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10687 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_facts.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1119 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_host.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2013 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_inventory.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    20162 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_operations.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1716 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.406668 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6045 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4858 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli_deploy.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3088 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli_exceptions.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2562 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli_util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2130 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_context_objects.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      338 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-06 14:57:11.410670 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5907 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_chroot.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6566 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_docker.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9303 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_dockerssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7442 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_local.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    38399 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_ssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5734 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_sshuserclient.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3743 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_terraform.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4647 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3646 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_vagrant.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3308 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_facts.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1696 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_global_arguments.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6074 2024-04-06 14:15:21.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_operations.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      557 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_operations_utils.py
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/CHANGELOG.md` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# v0.3.2
+
+FileContent fact, minor fixes
+
 # v0.3.1
 
 Added EnvVar fact
 
 # v0.3.0
 
 Move to v3, type hints for operations
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/LICENSE.md` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/PKG-INFO` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinfra_forked_by_stone-w4tch3r
-Version: 0.3.1
+Version: 0.3.2
 Summary: Custom version for developing pyinfra
 Home-page: https://pyinfra.com
 Author: stone-w4tch3r
 Author-email: 100294019+stone-w4tch3r@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com
 Project-URL: GitHub, https://github.com/stone-w4tch3r/pyinfra_fork
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyinfra_forked_by_stone-w4tch3r Version: 0.3.1
+Metadata-Version: 2.1 Name: pyinfra_forked_by_stone-w4tch3r Version: 0.3.2
 Summary: Custom version for developing pyinfra Home-page: https://pyinfra.com
 Author: stone-w4tch3r Author-email: 100294019+stone-
 w4tch3r@users.noreply.github.com License: MIT Project-URL: Documentation,
 https://docs.pyinfra.com Project-URL: GitHub, https://github.com/stone-w4tch3r/
 pyinfra_fork Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Intended
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/README.md` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/__init__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/__init__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/arguments.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/arguments_typed.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/arguments_typed.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/command.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/command.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/config.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/connect.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/connect.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/connectors.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/connectors.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/deploy.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/deploy.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/exceptions.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/facts.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/host.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/host.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/inventory.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/operation.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/operation.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/operations.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/operations.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/state.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/state.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/api/util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/api/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/base.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/base.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/chroot.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/chroot.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/docker.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/dockerssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/dockerssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/local.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/local.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/ssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/ssh_util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/ssh_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/sshuserclient/client.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/sshuserclient/client.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/sshuserclient/config.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/sshuserclient/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/terraform.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/terraform.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/connectors/vagrant.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/connectors/vagrant.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/context.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/context.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/apt.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/brew.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/cargo.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/cargo.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/choco.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/choco.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/deb.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/deb.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/dnf.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/docker.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,7 +416,33 @@
 
     def process(self, output):
         if output and (output[0] == f"{EXISTS}{self.path}"):
             return []
         if output and (output[0] == f"{MISSING}{self.path}"):
             return None
         return output
+
+
+class FileContent(FactBase[Optional[str]]):
+    """
+    Returns the content of a file as a single string.
+    """
+    path: str = None
+
+    def command(self, path):
+        cmd = f"cat {path}"
+        self.path = path
+
+        backstop = make_formatted_string_command(
+            "(find {0} -type f > /dev/null && echo {1} || echo {2} )",
+            QuoteString(path),
+            QuoteString(f"{EXISTS}{path}"),
+            QuoteString(f"{MISSING}{path}"),
+        )
+        return f"{cmd} || {backstop}"
+
+    def process(self, output: List[str]) -> Optional[str]:
+        if output and (output[0] == f"{EXISTS}{self.path}"):
+            return ""
+        if output and (output[0] == f"{MISSING}{self.path}"):
+            return None
+        return '\n'.join(output)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/git.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/git.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/gpg.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/gpg.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/hardware.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/hardware.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/iptables.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/iptables.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/launchd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/mysql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/mysql.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/npm.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/openrc.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/pacman.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/pip.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/pip.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/postgres.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/postgres.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/rpm.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/rpm.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/selinux.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/selinux.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/server.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/server.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/snap.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/systemd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/systemd.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/sysvinit.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/sysvinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/upstart.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/__init__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/databases.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/databases.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/packaging.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/packaging.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/util/win_files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/util/win_files.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/vzctl.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/yum.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/facts/zypper.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/facts/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/local.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/local.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/apk.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/apk.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/apt.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/brew.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/bsdinit.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/bsdinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/cargo.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/cargo.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/choco.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/choco.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/dnf.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
 
 @operation()
 def put(
     src: str | IO[Any],
     dest: str,
     user: str = None,
     group: str = None,
-    mode: str = None,
+    mode: str | bool = None,
     add_deploy_dir=True,
     create_remote_dir=True,
     force=False,
     assume_exists=False,
 ):
     """
     Upload a local file, or file-like object, to the remote system.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/gem.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/gem.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/git.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/git.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/iptables.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/iptables.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/launchd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/lxd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/lxd.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/mysql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/mysql.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/npm.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/openrc.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pacman.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pip.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pip.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pkg.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pkg.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/pkgin.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/pkgin.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/postgres.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/postgres.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/postgresql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/puppet.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/puppet.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/python.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/python.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/selinux.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/selinux.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/server.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/server.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/snap.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/ssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/ssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/systemd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/systemd.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/sysvinit.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/sysvinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/upstart.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/files.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/packaging.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/packaging.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/util/service.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/util/service.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/vzctl.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/xbps.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/xbps.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/yum.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/operations/zypper.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/operations/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra/progress.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra/progress.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/__main__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/commands.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/commands.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/exceptions.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/inventory.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/log.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/log.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/main.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/main.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/prints.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/prints.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_cli/virtualenv.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_cli/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinfra_forked_by_stone-w4tch3r
-Version: 0.3.1
+Version: 0.3.2
 Summary: Custom version for developing pyinfra
 Home-page: https://pyinfra.com
 Author: stone-w4tch3r
 Author-email: 100294019+stone-w4tch3r@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com
 Project-URL: GitHub, https://github.com/stone-w4tch3r/pyinfra_fork
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyinfra_forked_by_stone-w4tch3r Version: 0.3.1
+Metadata-Version: 2.1 Name: pyinfra_forked_by_stone-w4tch3r Version: 0.3.2
 Summary: Custom version for developing pyinfra Home-page: https://pyinfra.com
 Author: stone-w4tch3r Author-email: 100294019+stone-
 w4tch3r@users.noreply.github.com License: MIT Project-URL: Documentation,
 https://docs.pyinfra.com Project-URL: GitHub, https://github.com/stone-w4tch3r/
 pyinfra_fork Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Intended
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/pyinfra_forked_by_stone_w4tch3r.egg-info/requires.txt` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/pyinfra_forked_by_stone_w4tch3r.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/setup.cfg` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/setup.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_arguments.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_command.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_command.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_config.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_config.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_deploys.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_deploys.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_facts.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_host.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_host.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_inventory.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_operations.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_operations.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_api/test_api_util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_api/test_api_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli_deploy.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli_exceptions.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_cli_util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_cli/test_context_objects.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_cli/test_context_objects.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_chroot.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_chroot.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_docker.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_dockerssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_dockerssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_local.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_ssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_ssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_sshuserclient.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_sshuserclient.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_terraform.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_terraform.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_connectors/test_vagrant.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_connectors/test_vagrant.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_facts.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_global_arguments.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_global_arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_operations.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.3.1/tests/test_operations_utils.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.2/tests/test_operations_utils.py`

 * *Files identical despite different names*

