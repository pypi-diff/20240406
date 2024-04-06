# Comparing `tmp/archey4-4.8.1.tar.gz` & `tmp/archey4-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/archey4-4.8.1.tar", last modified: Sun Oct 11 07:48:36 2020, max compression
+gzip compressed data, was "dist/archey4-4.9.0.tar", last modified: Sat Nov 28 15:08:23 2020, max compression
```

## Comparing `archey4-4.8.1.tar` & `archey4-4.9.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1598 2020-10-11 07:37:36.000000 archey4-4.8.1/COPYRIGHT.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)    35149 2020-07-11 14:32:15.000000 archey4-4.8.1/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1627 2020-10-11 07:48:36.000000 archey4-4.8.1/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)    12778 2020-10-11 07:40:09.000000 archey4-4.8.1/README.md
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/archey/
--rw-r--r--   0 samuel    (1000) samuel    (1000)        0 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5369 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/__main__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)       80 2020-10-11 07:39:53.000000 archey4-4.8.1/archey/_version.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1389 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/api.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1835 2020-10-03 11:55:58.000000 archey4-4.8.1/archey/colors.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3775 2020-10-04 07:25:44.000000 archey4-4.8.1/archey/configuration.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4567 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/constants.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4647 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/distributions.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/archey/entries/
--rw-r--r--   0 samuel    (1000) samuel    (1000)        0 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1574 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/cpu.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1021 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/desktop_environment.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     8381 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/disk.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1539 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/distro.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1967 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/gpu.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      702 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/hostname.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      410 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/kernel.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2299 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/lan_ip.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4718 2020-10-11 07:33:25.000000 archey4-4.8.1/archey/entries/model.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2491 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/packages.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      383 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/processes.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3740 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/ram.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      758 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/shell.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5133 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/temperature.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5356 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/terminal.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7724 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/uptime.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      656 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/user.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3070 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entries/wan_ip.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1756 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/entries/window_manager.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1211 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/entry.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/archey/logos/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1826 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/logos/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1283 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/alpine_linux.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1029 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/android.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1077 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/arch_linux.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1173 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/bunsenlabs.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1789 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/centos.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      983 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/crunchbang.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1019 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/debian.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      977 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/logos/elementary.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1577 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/fedora.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      999 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/freebsd.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1285 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/gentoo.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1521 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/kali_linux.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      919 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/linux.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1238 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/linux_mint.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      879 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/manjaro.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1588 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/nixos.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1013 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/openbsd.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1627 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/opensuse.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1553 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/logos/pop.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1055 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/raspbian.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1259 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/red_hat.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2169 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/slackware.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1394 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/ubuntu.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1304 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/logos/windows.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     6366 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/output.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      897 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/processes.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3817 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/screenshot.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      688 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/singleton.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/archey/test/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/archey/test/entries/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     8009 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2914 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_cpu.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1790 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_desktop_environment.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    14150 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_disk.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2649 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_distro.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4558 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_gpu.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      996 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_hostname.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      593 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_kernel.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     8372 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_lan_ip.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     9164 2020-10-11 07:33:25.000000 archey4-4.8.1/archey/test/entries/test_archey_model.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    10625 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_packages.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5246 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_ram.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1812 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_shell.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    10384 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_temperature.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5204 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_terminal.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    11425 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_uptime.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1757 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_user.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4796 2020-10-11 07:33:10.000000 archey4-4.8.1/archey/test/entries/test_archey_wan_ip.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2297 2020-07-11 14:32:15.000000 archey4-4.8.1/archey/test/entries/test_archey_window_manager.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/archey4.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1627 2020-10-11 07:48:35.000000 archey4-4.8.1/archey4.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2466 2020-10-11 07:48:36.000000 archey4-4.8.1/archey4.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2020-10-11 07:48:35.000000 archey4-4.8.1/archey4.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       49 2020-10-11 07:48:35.000000 archey4-4.8.1/archey4.egg-info/entry_points.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2020-04-19 12:31:02.000000 archey4-4.8.1/archey4.egg-info/not-zip-safe
--rw-r--r--   0 samuel    (1000) samuel    (1000)       17 2020-10-11 07:48:35.000000 archey4-4.8.1/archey4.egg-info/requires.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2020-10-11 07:48:35.000000 archey4-4.8.1/archey4.egg-info/top_level.txt
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-10-11 07:48:36.000000 archey4-4.8.1/dist/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1160 2020-10-11 07:48:23.000000 archey4-4.8.1/dist/archey.1.gz
--rw-r--r--   0 samuel    (1000) samuel    (1000)       38 2020-10-11 07:48:36.000000 archey4-4.8.1/setup.cfg
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2524 2020-10-10 07:04:31.000000 archey4-4.8.1/setup.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1598 2020-11-22 15:35:14.000000 archey4-4.9.0/COPYRIGHT.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    35149 2020-07-11 14:32:15.000000 archey4-4.9.0/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1627 2020-11-28 15:08:23.000000 archey4-4.9.0/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    14231 2020-11-28 14:58:26.000000 archey4-4.9.0/README.md
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/archey/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        0 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6709 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/__main__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       80 2020-11-28 14:55:22.000000 archey4-4.9.0/archey/_version.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1389 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/api.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1835 2020-10-03 11:55:58.000000 archey4-4.9.0/archey/colors.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3743 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/configuration.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3762 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/constants.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4647 2020-11-22 15:35:14.000000 archey4-4.9.0/archey/distributions.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/archey/entries/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        0 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4430 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/cpu.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1021 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/desktop_environment.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8544 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/disk.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1522 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/distro.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1946 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/gpu.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      702 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/hostname.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      410 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/kernel.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2559 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/lan_ip.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4864 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/model.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2491 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/packages.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      383 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/processes.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3674 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/ram.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      758 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/shell.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5076 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/temperature.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5379 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/terminal.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7724 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/uptime.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      656 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/user.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3564 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entries/wan_ip.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1756 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/entries/window_manager.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1540 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/entry.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/archey/logos/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1826 2020-11-22 15:35:14.000000 archey4-4.9.0/archey/logos/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1283 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/alpine_linux.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1029 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/android.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1077 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/arch_linux.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1173 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/bunsenlabs.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1789 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/centos.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      983 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/crunchbang.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1019 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/debian.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      977 2020-11-22 15:35:14.000000 archey4-4.9.0/archey/logos/elementary.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1577 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/fedora.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      999 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/freebsd.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1285 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/gentoo.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1521 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/kali_linux.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      919 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/linux.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1238 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/linux_mint.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      879 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/manjaro.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1588 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/nixos.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1013 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/openbsd.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1627 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/opensuse.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1553 2020-11-22 15:35:14.000000 archey4-4.9.0/archey/logos/pop.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1055 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/raspbian.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1259 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/red_hat.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2169 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/slackware.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1394 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/ubuntu.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1304 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/logos/windows.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6348 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/output.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      897 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/processes.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3816 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/screenshot.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      688 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/singleton.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/archey/test/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/archey/test/entries/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7997 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     9465 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_cpu.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1790 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_desktop_environment.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    13750 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_disk.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2649 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_distro.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4293 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_gpu.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      996 2020-11-22 16:51:23.000000 archey4-4.9.0/archey/test/entries/test_archey_hostname.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      593 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_kernel.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    10147 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_lan_ip.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     9544 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_model.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    10625 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_packages.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4750 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_ram.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1812 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_shell.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     9563 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_temperature.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4768 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_terminal.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    11423 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_uptime.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1757 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_user.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4551 2020-11-28 14:54:40.000000 archey4-4.9.0/archey/test/entries/test_archey_wan_ip.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2297 2020-07-11 14:32:15.000000 archey4-4.9.0/archey/test/entries/test_archey_window_manager.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/archey4.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1627 2020-11-28 15:08:22.000000 archey4-4.9.0/archey4.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2466 2020-11-28 15:08:22.000000 archey4-4.9.0/archey4.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2020-11-28 15:08:22.000000 archey4-4.9.0/archey4.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       49 2020-11-28 15:08:22.000000 archey4-4.9.0/archey4.egg-info/entry_points.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2020-04-19 12:31:02.000000 archey4-4.9.0/archey4.egg-info/not-zip-safe
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       17 2020-11-28 15:08:22.000000 archey4-4.9.0/archey4.egg-info/requires.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2020-11-28 15:08:22.000000 archey4-4.9.0/archey4.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2020-11-28 15:08:23.000000 archey4-4.9.0/dist/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     1164 2020-11-28 15:08:16.000000 archey4-4.9.0/dist/archey.1.gz
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       38 2020-11-28 15:08:23.000000 archey4-4.9.0/setup.cfg
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2525 2020-11-28 14:54:40.000000 archey4-4.9.0/setup.py
```

### Comparing `archey4-4.8.1/COPYRIGHT.md` & `archey4-4.9.0/COPYRIGHT.md`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/LICENSE` & `archey4-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/PKG-INFO` & `archey4-4.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archey4
-Version: 4.8.1
+Version: 4.9.0
 Summary: Archey is a simple system information tool written in Python
 Home-page: https://github.com/HorlogeSkynet/archey4
 Author: Samuel Forestier
 Author-email: dev+archey@samuel.domains
 License: GPLv3
 Description: Archey4 is a **maintained** fork of the original Archey Linux system tool.
         The original Archey program had been written by Melik Manukyan in 2009, and quickly abandoned in 2011.
```

### Comparing `archey4-4.8.1/README.md` & `archey4-4.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Archey 4
 
 > Archey is a simple system information tool written in Python
 
 <p align="center">
-	<!-- GITHUB & TRAVIS CI -->
+	<!-- GITHUB -->
 	<a href="https://github.com/HorlogeSkynet/archey4/releases/latest"><img src="https://img.shields.io/github/release/HorlogeSkynet/archey4.svg?style=for-the-badge"></a>
-	<a href="https://travis-ci.org/HorlogeSkynet/archey4"><img src="https://img.shields.io/travis/HorlogeSkynet/archey4/master.svg?style=for-the-badge"></a>
-	<a href="https://github.com/HorlogeSkynet/archey4/commits/master"><img src="https://img.shields.io/github/last-commit/HorlogeSkynet/archey4.svg?style=for-the-badge"></a>
+	<a href="https://github.com/HorlogeSkynet/archey4/actions"><img src="https://img.shields.io/github/workflow/status/HorlogeSkynet/archey4/Integration/master.svg?style=for-the-badge"></a>
+	<a href="https://github.com/HorlogeSkynet/archey4/commits"><img src="https://img.shields.io/github/last-commit/HorlogeSkynet/archey4.svg?style=for-the-badge"></a>
 	<br />
 	<!-- AUR -->
 	<a href="https://aur.archlinux.org/packages/archey4/"><img src="https://img.shields.io/aur/version/archey4.svg?style=for-the-badge"></a>
 	<a href="https://aur.archlinux.org/packages/archey4/"><img src="https://img.shields.io/aur/license/archey4.svg?style=for-the-badge"></a>
 	<a href="https://aur.archlinux.org/packages/archey4/"><img src="https://img.shields.io/aur/votes/archey4.svg?style=for-the-badge"></a>
 	<a href="https://aur.archlinux.org/packages/archey4/"><img src="https://img.shields.io/aur/last-modified/archey4.svg?style=for-the-badge"></a>
 	<br />
@@ -33,15 +33,15 @@
 > Nevertheless, **this piece of software is still a fork of [djmelik's Archey project](https://github.com/djmelik/archey.git)**.
 
 ## Features
 
 * Run as quickly as possible
 * Stay as light as possible
 * Keep entries ordered despite parallelism
-* Extensive local IP addresses detection
+* Extensive local and public IP addresses detection
 * General temperature detection
 * JSON output
 * Screen capture ("best effort")
 
 ## Which packages do I need to run this project ?
 
 ### Required packages
@@ -88,77 +88,90 @@
 
 ```bash
 sudo yay -S archey4
 ```
 
 ### Install from source
 
-```bash
-### Step 1 : Fetch the source ###
+#### Step 1 : Fetch sources
 
+```bash
 # If you want the latest release :
-LATEST_VERSION="v4.8.1"
+LATEST_VERSION="v4.9.0"
 wget "https://github.com/HorlogeSkynet/archey4/archive/${LATEST_VERSION}.tar.gz"
 tar xvzf "${LATEST_VERSION}.tar.gz"
 cd "archey4-${LATEST_VERSION}/"
-# _______________________________
 
-# If you want the latest changes :
+# If you want the latest (stable) changes :
 git clone https://github.com/HorlogeSkynet/archey4.git
 cd archey4/
-# _______________________________
-
+```
 
-### Step 2 : Installation ###
+#### Step 2 : Installation
 
+```bash
 # If you have PIP installed on your system :
 sudo pip3 install .
-# _________________________________________
 
 # But if you don't have PIP, no worries :
 sudo python3 setup.py install
-# _______________________________________
+```
 
-### Step 3 (Optional) : Configuration files
+#### Step 3 (optional) : Configuration
 
-# System-wide configuration :
+```bash
+# System-wide configuration file :
 sudo mkdir /etc/archey4
-sudo cp archey/config.json /etc/archey4/config.json
-# ___________________________
-# User-specific configuration :
-mkdir ~/.config/archey4
-cp archey/config.json ~/.config/archey4/config.json
-# _____________________________
+sudo cp config.json /etc/archey4/config.json
 
-### Step 4 (Optional) : I want a standalone script, as before !
+# User-specific configuration file :
+mkdir -p ~/.config/archey4
+cp config.json ~/.config/archey4/config.json
+```
 
-# You can go through StickyTape for this :
+#### Step 4 (optional) : Standalone building
+
+> Some years ago, Archey was a simple and unique Python file.  
+> Project evolved, and now it's a proper module.  
+> Some procedures below walk you through several ways of building Archey as a standalone program.
+
+```bash
+# Using Stickytape :
 sudo pip3 install stickytape
 stickytape \
 	--copy-shebang \
 	--add-python-path . \
 	--output-file dist/archey \
 	archey/__main__.py
 chmod +x dist/archey
-./dist/archey
-# ________________________________________
 
-# You can either use PyInstaller :
+# Using PyInstaller :
 sudo pip3 install pyinstaller
 pyinstaller \
 	--distpath dist \
 	--specpath dist \
 	--name archey \
 	--onefile archey/__main__.py
+
+# Using PEX :
+sudo pip3 install pex
+pex \
+	-o dist/archey \
+	-m archey \
+	.
+```
+
+Resulting program may now be installed system-wide.
+
+```bash
+# Execute program resulting from step 4.
 ./dist/archey
-# ________________________________
 
-# You can now move this script anywhere, as before :
+# You can now move this file for a system-wide install :
 sudo mv dist/archey /usr/local/bin/
-# __________________________________________________
 ```
 
 ## Usage
 
 ```bash
 archey --help
 ```
@@ -168,142 +181,195 @@
 ```bash
 python3 -m archey --help
 ```
 
 ## Configuration (optional)
 
 Since v4.3.0, Archey 4 **may** be "tweaked" a bit with external configuration.  
-You can place a [`config.json`](archey/config.json) file in these locations :
+You can place a [`config.json`](config.json) file in these locations :
 
 1. `/etc/archey4/config.json` (system preferences)
 2. `~/.config/archey4/config.json` (user preferences)
 3. `./config.json` (local preferences)
 
 **If an option is defined in multiple places, it will be overridden according to the order above (local preferences > user preferences > system preferences).**
 
-The [example file](archey/config.json) provided in this repository lists exhaustively the parameters you can set.  
-Below stand further descriptions for each available option :
+Alternatively, you may specify your own configuration file with the `-c` command-line option.
+
+The [example file](config.json) provided in this repository lists exhaustively the parameters you can set.  
+Below stand further descriptions for each available (default) option :
 
 <!-- We use JavaScript syntax coloration below because JSON does not allow the usage of comments in it -->
 ```javascript
 {
 	// If set to `false`, configurations defined afterwards won't be loaded.
-	// Developers running Archey from the original project may keep in there the original `config.json` while having their own external configuration set elsewhere.
+	// Developers running Archey from the original project may keep in there the original `config.json`,
+	//   while having their own external configuration set elsewhere.
 	"allow_overriding": true,
 	// Set to `false` to disable multi-threaded loading of entries.
 	"parallel_loading": true,
 	// If set to `true`, any execution warning or error would be hidden.
-	// It may not apply to configuration parsing warnings.
+	// Configuration parsing warnings **would** still be shown.
 	"suppress_warnings": false,
-	"entries": {
-		// Set to `false` each entry you want to mask.
-	},
-	"colors_palette": {
-		// Leave this option set to `true` to display a beautiful colors palette.
-		// Set it to `false` to allow compatibility with non-Unicode locales.
-		"use_unicode": true,
-		// Set this option to `false` to force Archey to use its own colors palettes.
-		// `true` by default to honor `os-release`'s `ANSI_COLOR` option.
-		"honor_ansi_color": true
-	},
-	"disk": {
-		// Which filesystems to show:
-		// `["local"]` shows only local filesystems.
-		// You can alternatively list specific filesystems as:
-		//  * A list of device paths - e.g. `["/dev/sda1", "/dev/nvme0n1p1"]`
-		//  * A list of mount points - e.g. `["/", "/mnt"]`
-		//  * A combination of the above - e.g. `["/", "/dev/sda2"]`
-		"show_filesystems": ["local"],
-		// Set to `false` to write each filesystem on its own line.
-		"combine_total": true,
-		// Defines which labels to use for each disk (only works if `combine_total` is false!)
-		// The options available are:
-		//  * `"mount_points"`: Shows the mount point of the filesystem.
-		//      e.g. `Disk (/): 10.0 GiB/100.0 GiB`
-		//           `Disk (/mnt): 15.0 GiB / 200.0 GiB`
-		//  * `"device_paths"`: Shows the device path of the filesystem.
-		//      e.g. `Disk (/dev/sda1): 10.0 GiB / 100.0 GiB`
-		//           `Disk (/dev/mmcblk0p1): 15.0 GiB / 200.0 GiB`
-		//  * `false` or `null` (no quote marks!): Don't show any device labels.
-		//      e.g. `Disk: 10.0 GiB / 100.0 GiB`
-		//           `Disk: 15.0 GiB / 200.0 GiB`
-		"disk_labels": null,
-		// Set to `true` to hide the "Disk" entry name from the output.
-		// i.e. null  --> `Disk (/):`
-		//      false --> `Disk (/):`
-		//      true  --> `(/):`
-		"hide_entry_name": null
-	},
-	"default_strings": {
-		// Use this section to override default strings.
-	},
-	"ip_settings": {
-		// The maximum number of local addresses you want to display.
-		// `false` --> Unlimited.
-		"lan_ip_max_count": 2,
-		// `false` would make Archey display IPv4 LAN addresses only.
-		"lan_ip_v6_support": true,
-		// `false` would make Archey display IPv4 WAN addresses only.
-		"wan_ip_v6_support": true
-	},
-	"gpu": {
-		// Display GPUs on multiple lines if set to `false`.
-		"one_line": true,
-		// The maximum number of GPUs you want to display.
-		// `false` --> Unlimited.
-		"max_count": 2
-	},
-	"limits": {
-		// Some threshold values you can adjust affecting disk/ram warning/danger color (percent).
-		"ram": {
-			"warning": 33.3,
-			"danger": 66.7
+	// Set this option to `false` to force Archey to use its own colors palettes.
+	// `true` by default to honor os-release(5) `ANSI_COLOR` option.
+	"honor_ansi_color": true,
+	// Entries list.
+	// Add a `disabled` option set to `true` to temporary hide one.
+	// You may change entry displayed name by adding a `name` option.
+	// You may re-order the entries list as you wish.
+	"entries": [
+		{ "type": "User" },
+		{ "type": "Hostname" },
+		{ "type": "Model" },
+		{ "type": "Distro" },
+		{ "type": "Kernel" },
+		{ "type": "Uptime" },
+		{ "type": "Processes" },
+		{ "type": "WindowManager" },
+		{ "type": "DesktopEnvironment" },
+		{ "type": "Shell" },
+		{
+			"type": "Terminal",
+			// Leave this option set to `true` to display a beautiful colors palette.
+			// Set it to `false` to allow compatibility with non-Unicode locales.
+			"use_unicode": true
+		},
+		{ "type": "Packages" },
+		{
+			"type": "Temperature",
+			// The character to display between the temperature value and the unit (as '°' in 53.2°C).
+			"char_before_unit": " ",
+			"sensors_chipsets": [
+				// White-list of chipset identifiers (strings) passed to LM-SENSORS when computing the average temperature.
+				// Use `sensors -A` to list the available chipsets on your system (e.g. `coretemp-isa-0000`, `acpitz-acpi-0`, ...).
+				// Leaving empty (default) would make Archey process input data from all available chipsets.
+				// Use this option if a sensor happens to return irrelevant values, or if you want to exclude it.
+			],
+			// Display temperature values in Fahrenheit instead of Celsius.
+			"use_fahrenheit": false
+		},
+		{
+			"type": "CPU",
+			// Set to `true` to join all CPUs on the same line.
+			"one_line": false,
+			// Set to `false` to hide the number of cores.
+			"show_cores": true,
+			//
+			// As explained above, you may rename entries as you wish.
+			"name": "Processor"
+		},
+		{
+			"type": "GPU",
+			// Set to `true` to join all GPUs on the same line.
+			"one_line": false,
+			// The maximum number of GPUs you want to display.
+			// `false` --> Unlimited.
+			"max_count": 2
+		},
+		{
+			"type": "RAM",
+			// Some threshold values you can adjust affecting warning/danger colors.
+			"warning_use_percent": 33.3,
+			"danger_use_percent": 66.7
 		},
-		"disk": {
-			"warning": 50,
-			"danger": 75
+		{
+			"type": "LAN_IP",
+			// The maximum number of local addresses you want to display.
+			// `false` --> Unlimited.
+			"max_count": 2,
+			// Set to `false` to only display IPv4 LAN addresses.
+			"ipv6_support": true
+		},
+		{
+			"type": "Disk",
+			// Which filesystems to show:
+			// `["local"]` shows only local filesystems.
+			// You can alternatively list specific filesystems as:
+			//  * A list of device paths - e.g. `["/dev/sda1", "/dev/nvme0n1p1"]`
+			//  * A list of mount points - e.g. `["/", "/mnt"]`
+			//  * A combination of the above - e.g. `["/", "/dev/sda2"]`
+			"show_filesystems": ["local"],
+			// Set to `false` to write each filesystem on its own line.
+			"combine_total": true,
+			// Defines which labels to use for each disk (only works if `combine_total` is false!)
+			// The options available are:
+			//  * `"mount_points"`: Shows the mount point of the filesystem.
+			//      e.g. `Disk (/): 10.0 GiB/100.0 GiB`
+			//           `Disk (/mnt): 15.0 GiB / 200.0 GiB`
+			//  * `"device_paths"`: Shows the device path of the filesystem.
+			//      e.g. `Disk (/dev/sda1): 10.0 GiB / 100.0 GiB`
+			//           `Disk (/dev/mmcblk0p1): 15.0 GiB / 200.0 GiB`
+			//  * `false` or `null` (no quote marks!): Don't show any device labels.
+			//      e.g. `Disk: 10.0 GiB / 100.0 GiB`
+			//           `Disk: 15.0 GiB / 200.0 GiB`
+			"disk_labels": null,
+			// Set to `true` to hide the "Disk" entry name from the output.
+			// i.e. null  --> `Disk (/):`
+			//      false --> `Disk (/):`
+			//      true  --> `(/):`
+			"hide_entry_name": null,
+			// Some threshold values you can adjust affecting warning/danger colors.
+			"warning_use_percent": 50,
+			"danger_use_percent": 75
+		},
+		{
+			"type": "WAN_IP",
+			//
+			// As explained above, you may temporary hide entries as you wish.
+			// See below example to hide your public IP addresses before posting your configuration on Internet.
+			//"disabled": true,
+			//
+			// Below are settings relative to IPv4/IPv6 public addresses retrieval.
+			// I hope options are self-explanatory.
+			// You may set `dns_query` (or `http_url`) to `false` to disable them.
+			// You may directly set `ipv4` or `ipv6` fields to `false` to completely disable them.
+			//
+			// <https://ident.me/> server sources : <https://github.com/pcarrier/identme>.
+			"ipv4": {
+				"dns_query": "myip.opendns.com",
+				"dns_resolver": "resolver1.opendns.com",
+				"dns_timeout": 1,
+				"http_url": "https://v4.ident.me/",
+				"http_timeout": 1
+			},
+			"ipv6": {
+				"dns_query": "myip.opendns.com",
+				"dns_resolver": "resolver1.opendns.com",
+				"dns_timeout": 1,
+				"http_url": "https://v6.ident.me/",
+				"http_timeout": 1
+			}
 		}
-	},
-	"temperature": {
-		// The character to display between the temperature value and the unit (as '°' in 53.2°C).
-		// Set to ' ' (space) by default for backward compatibility with non-Unicode locales.
-		"char_before_unit": " ",
-		"sensors_chipsets": [
-			// White-list of chipset identifiers (strings) passed to LM-SENSORS when computing the average temperature.
-			// Uses `sensors -A` to list the available chipsets on your system (e.g. `coretemp-isa-0000`, `acpitz-acpi-0`, ...).
-			// Leaving empty (default) would make Archey process input data from each existing chipset.
-			// Use this option if a sensor happens to return irrelevant values, or if you want to exclude it.
-		],
-		// Display temperature values in Fahrenheit instead of Celsius.
-		"use_fahrenheit": false
-	},
-	"timeout": {
-		// Some values you can adjust if the default ones look undersized for your system (seconds).
+	],
+	"default_strings": {
+		// Use this section to override default strings (internationalization).
 	}
 }
+
 ```
 
 ## Test cases
 
 An extensive tests suite is available.  
 Here is a short procedure to run them (you'll only need `python3`) :
 
 ```bash
 git clone https://github.com/HorlogeSkynet/archey4.git
 cd archey4/
-# If you got `setuptools` installed
+
+# Run the suite from SetupTools.
 python3 setup.py test
-# But if you don't, no worries !
+
+# Run the suite from the unit testing framework itself.
 python3 -m unittest
 ```
 
 Any improvement would be appreciated.
 
 ## Notes to users
 
 * If you experience any trouble during the installation or usage, please do **[open an issue](https://github.com/HorlogeSkynet/archey4/issues/new)**.
 
 * If you had to tweak this project to make it work on your system, please **[open a pull request](https://github.com/HorlogeSkynet/archey4/pulls)** so as to share your modifications with the rest of the world and participate in this project ! You should also check [Info for contributors](https://github.com/HorlogeSkynet/archey4/wiki/Info-for-contributors).
 
 * If your distribution is not (currently) supported, please check [How do I add a distribution to Archey?](https://github.com/HorlogeSkynet/archey4/wiki/How-do-I-add-a-distribution-to-Archey%3F).
-
-* When looking up your public IP address (**WAN\_IP**), Archey will try at first to run a DNS query for `myip.opendns.com`, against OpenDNS's resolver(s). On error, it would fall back on regular HTTPS request(s) to <https://ident.me> ([server sources](https://github.com/pcarrier/identme)).
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # Archey 4 > Archey is a simple system information tool written in Python
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_H_o_r_l_o_g_e_S_k_y_n_e_t_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
-          _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_r_a_v_i_s_/_H_o_r_l_o_g_e_S_k_y_n_e_t_/_a_r_c_h_e_y_4_/
-  _m_a_s_t_e_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/
-                _H_o_r_l_o_g_e_S_k_y_n_e_t_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
+  _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_H_o_r_l_o_g_e_S_k_y_n_e_t_/_a_r_c_h_e_y_4_/
+_I_n_t_e_g_r_a_t_i_o_n_/_m_a_s_t_e_r_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-
+             _c_o_m_m_i_t_/_H_o_r_l_o_g_e_S_k_y_n_e_t_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_a_u_r_/_v_e_r_s_i_o_n_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
      _i_m_g_._s_h_i_e_l_d_s_._i_o_/_a_u_r_/_l_i_c_e_n_s_e_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
       _i_m_g_._s_h_i_e_l_d_s_._i_o_/_a_u_r_/_v_o_t_e_s_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
        _i_m_g_._s_h_i_e_l_d_s_._i_o_/_a_u_r_/_l_a_s_t_-_m_o_d_i_f_i_e_d_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_a_r_c_h_e_y_4_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_a_r_c_h_e_y_4_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
@@ -14,18 +14,18 @@
 ## Why (again) a f\*cking new Archey fork ? The answer is [here](https://
 blog.samuel.domains/archey4). > Note : Since the 21st September of 2017, you
 may notice that this repository no longer has the official status of fork. >
 Actually, the maintainer decided to separate it from the original one's
 "network" with the help of _GitHub_'s staff. > Nevertheless, **this piece of
 software is still a fork of [djmelik's Archey project](https://github.com/
 djmelik/archey.git)**. ## Features * Run as quickly as possible * Stay as light
-as possible * Keep entries ordered despite parallelism * Extensive local IP
-addresses detection * General temperature detection * JSON output * Screen
-capture ("best effort") ## Which packages do I need to run this project ? ###
-Required packages * `python3` * `python3-distro` (`python-distro` on Arch
+as possible * Keep entries ordered despite parallelism * Extensive local and
+public IP addresses detection * General temperature detection * JSON output *
+Screen capture ("best effort") ## Which packages do I need to run this project
+? ### Required packages * `python3` * `python3-distro` (`python-distro` on Arch
 Linux) * `python3-netifaces` (`python-netifaces` on Arch Linux) * `procps`
 (`procps-ng` on Arch Linux) > PyPy is supported and may replace CPython. ###
 Highly recommended packages | Environments | Packages | Reasons | Notes | | :--
 ------------------ | :-------------------------------- | :---------------------
 ------------------------------ | :--------------------------- | | All |
 `dnsutils` (maybe `bind-tools`) | **WAN\_IP** would be detected faster | Would
 provide `dig` | | All | `lm-sensors` (maybe `lm_sensors`) | **Temperature**
@@ -42,109 +42,125 @@
 based distributions : `dnf install ./archey4-4.Y.Z-R.py??.noarch.rpm` **Note to
 Debian 8 (Jessie) users** : As [`python3-distro`](https://tracker.debian.org/
 pkg/python-distro) is not available in your repositories, **you should opt for
 an [installation from PyPI](#install-from-pypi).** Further information about
 packaging are available [here](https://github.com/HorlogeSkynet/archey4/wiki/
 Packaging). ### Install from [PyPI](https://pypi.org/project/archey4/) ```bash
 sudo pip3 install archey4 ``` ### Install from [AUR](https://aur.archlinux.org/
-packages/archey4/) ```bash sudo yay -S archey4 ``` ### Install from source
-```bash ### Step 1 : Fetch the source ### # If you want the latest release :
-LATEST_VERSION="v4.8.1" wget "https://github.com/HorlogeSkynet/archey4/archive/
+packages/archey4/) ```bash sudo yay -S archey4 ``` ### Install from source ####
+Step 1 : Fetch sources ```bash # If you want the latest release :
+LATEST_VERSION="v4.9.0" wget "https://github.com/HorlogeSkynet/archey4/archive/
 ${LATEST_VERSION}.tar.gz" tar xvzf "${LATEST_VERSION}.tar.gz" cd "archey4-$
-{LATEST_VERSION}/" # _______________________________ # If you want the latest
-changes : git clone https://github.com/HorlogeSkynet/archey4.git cd archey4/ #
-_______________________________ ### Step 2 : Installation ### # If you have PIP
-installed on your system : sudo pip3 install . #
-_________________________________________ # But if you don't have PIP, no
-worries : sudo python3 setup.py install #
-_______________________________________ ### Step 3 (Optional) : Configuration
-files # System-wide configuration : sudo mkdir /etc/archey4 sudo cp archey/
-config.json /etc/archey4/config.json # ___________________________ # User-
-specific configuration : mkdir ~/.config/archey4 cp archey/config.json
-~/.config/archey4/config.json # _____________________________ ### Step 4
-(Optional) : I want a standalone script, as before ! # You can go through
-StickyTape for this : sudo pip3 install stickytape stickytape \ --copy-shebang
-\ --add-python-path . \ --output-file dist/archey \ archey/__main__.py chmod +x
-dist/archey ./dist/archey # ________________________________________ # You can
-either use PyInstaller : sudo pip3 install pyinstaller pyinstaller \ --distpath
-dist \ --specpath dist \ --name archey \ --onefile archey/__main__.py ./dist/
-archey # ________________________________ # You can now move this script
-anywhere, as before : sudo mv dist/archey /usr/local/bin/ #
-__________________________________________________ ``` ## Usage ```bash archey
---help ``` or if you only want to try this out (for instance, from source) :
-```bash python3 -m archey --help ``` ## Configuration (optional) Since v4.3.0,
-Archey 4 **may** be "tweaked" a bit with external configuration. You can place
-a [`config.json`](archey/config.json) file in these locations : 1. `/etc/
-archey4/config.json` (system preferences) 2. `~/.config/archey4/config.json`
-(user preferences) 3. `./config.json` (local preferences) **If an option is
-defined in multiple places, it will be overridden according to the order above
-(local preferences > user preferences > system preferences).** The [example
-file](archey/config.json) provided in this repository lists exhaustively the
-parameters you can set. Below stand further descriptions for each available
-option : ```javascript { // If set to `false`, configurations defined
-afterwards won't be loaded. // Developers running Archey from the original
-project may keep in there the original `config.json` while having their own
-external configuration set elsewhere. "allow_overriding": true, // Set to
-`false` to disable multi-threaded loading of entries. "parallel_loading": true,
-// If set to `true`, any execution warning or error would be hidden. // It may
-not apply to configuration parsing warnings. "suppress_warnings": false,
-"entries": { // Set to `false` each entry you want to mask. },
-"colors_palette": { // Leave this option set to `true` to display a beautiful
-colors palette. // Set it to `false` to allow compatibility with non-Unicode
-locales. "use_unicode": true, // Set this option to `false` to force Archey to
-use its own colors palettes. // `true` by default to honor `os-release`'s
-`ANSI_COLOR` option. "honor_ansi_color": true }, "disk": { // Which filesystems
-to show: // `["local"]` shows only local filesystems. // You can alternatively
+{LATEST_VERSION}/" # If you want the latest (stable) changes : git clone https:
+//github.com/HorlogeSkynet/archey4.git cd archey4/ ``` #### Step 2 :
+Installation ```bash # If you have PIP installed on your system : sudo pip3
+install . # But if you don't have PIP, no worries : sudo python3 setup.py
+install ``` #### Step 3 (optional) : Configuration ```bash # System-wide
+configuration file : sudo mkdir /etc/archey4 sudo cp config.json /etc/archey4/
+config.json # User-specific configuration file : mkdir -p ~/.config/archey4 cp
+config.json ~/.config/archey4/config.json ``` #### Step 4 (optional) :
+Standalone building > Some years ago, Archey was a simple and unique Python
+file. > Project evolved, and now it's a proper module. > Some procedures below
+walk you through several ways of building Archey as a standalone program.
+```bash # Using Stickytape : sudo pip3 install stickytape stickytape \ --copy-
+shebang \ --add-python-path . \ --output-file dist/archey \ archey/__main__.py
+chmod +x dist/archey # Using PyInstaller : sudo pip3 install pyinstaller
+pyinstaller \ --distpath dist \ --specpath dist \ --name archey \ --onefile
+archey/__main__.py # Using PEX : sudo pip3 install pex pex \ -o dist/archey \ -
+m archey \ . ``` Resulting program may now be installed system-wide. ```bash #
+Execute program resulting from step 4. ./dist/archey # You can now move this
+file for a system-wide install : sudo mv dist/archey /usr/local/bin/ ``` ##
+Usage ```bash archey --help ``` or if you only want to try this out (for
+instance, from source) : ```bash python3 -m archey --help ``` ## Configuration
+(optional) Since v4.3.0, Archey 4 **may** be "tweaked" a bit with external
+configuration. You can place a [`config.json`](config.json) file in these
+locations : 1. `/etc/archey4/config.json` (system preferences) 2. `~/.config/
+archey4/config.json` (user preferences) 3. `./config.json` (local preferences)
+**If an option is defined in multiple places, it will be overridden according
+to the order above (local preferences > user preferences > system
+preferences).** Alternatively, you may specify your own configuration file with
+the `-c` command-line option. The [example file](config.json) provided in this
+repository lists exhaustively the parameters you can set. Below stand further
+descriptions for each available (default) option : ```javascript { // If set to
+`false`, configurations defined afterwards won't be loaded. // Developers
+running Archey from the original project may keep in there the original
+`config.json`, // while having their own external configuration set elsewhere.
+"allow_overriding": true, // Set to `false` to disable multi-threaded loading
+of entries. "parallel_loading": true, // If set to `true`, any execution
+warning or error would be hidden. // Configuration parsing warnings **would**
+still be shown. "suppress_warnings": false, // Set this option to `false` to
+force Archey to use its own colors palettes. // `true` by default to honor os-
+release(5) `ANSI_COLOR` option. "honor_ansi_color": true, // Entries list. /
+/ Add a `disabled` option set to `true` to temporary hide one. // You may
+change entry displayed name by adding a `name` option. // You may re-order the
+entries list as you wish. "entries": [ { "type": "User" }, { "type": "Hostname"
+}, { "type": "Model" }, { "type": "Distro" }, { "type": "Kernel" }, { "type":
+"Uptime" }, { "type": "Processes" }, { "type": "WindowManager" }, { "type":
+"DesktopEnvironment" }, { "type": "Shell" }, { "type": "Terminal", // Leave
+this option set to `true` to display a beautiful colors palette. // Set it to
+`false` to allow compatibility with non-Unicode locales. "use_unicode": true },
+{ "type": "Packages" }, { "type": "Temperature", // The character to display
+between the temperature value and the unit (as 'Â°' in 53.2Â°C).
+"char_before_unit": " ", "sensors_chipsets": [ // White-list of chipset
+identifiers (strings) passed to LM-SENSORS when computing the average
+temperature. // Use `sensors -A` to list the available chipsets on your system
+(e.g. `coretemp-isa-0000`, `acpitz-acpi-0`, ...). // Leaving empty (default)
+would make Archey process input data from all available chipsets. // Use this
+option if a sensor happens to return irrelevant values, or if you want to
+exclude it. ], // Display temperature values in Fahrenheit instead of Celsius.
+"use_fahrenheit": false }, { "type": "CPU", // Set to `true` to join all CPUs
+on the same line. "one_line": false, // Set to `false` to hide the number of
+cores. "show_cores": true, // // As explained above, you may rename entries as
+you wish. "name": "Processor" }, { "type": "GPU", // Set to `true` to join all
+GPUs on the same line. "one_line": false, // The maximum number of GPUs you
+want to display. // `false` --> Unlimited. "max_count": 2 }, { "type": "RAM", /
+/ Some threshold values you can adjust affecting warning/danger colors.
+"warning_use_percent": 33.3, "danger_use_percent": 66.7 }, { "type": "LAN_IP",
+// The maximum number of local addresses you want to display. // `false` --
+> Unlimited. "max_count": 2, // Set to `false` to only display IPv4 LAN
+addresses. "ipv6_support": true }, { "type": "Disk", // Which filesystems to
+show: // `["local"]` shows only local filesystems. // You can alternatively
 list specific filesystems as: // * A list of device paths - e.g. `["/dev/sda1",
 "/dev/nvme0n1p1"]` // * A list of mount points - e.g. `["/", "/mnt"]` // * A
 combination of the above - e.g. `["/", "/dev/sda2"]` "show_filesystems":
 ["local"], // Set to `false` to write each filesystem on its own line.
 "combine_total": true, // Defines which labels to use for each disk (only works
 if `combine_total` is false!) // The options available are: // *
 `"mount_points"`: Shows the mount point of the filesystem. // e.g. `Disk (/):
 10.0 GiB/100.0 GiB` // `Disk (/mnt): 15.0 GiB / 200.0 GiB` // *
 `"device_paths"`: Shows the device path of the filesystem. // e.g. `Disk (/dev/
 sda1): 10.0 GiB / 100.0 GiB` // `Disk (/dev/mmcblk0p1): 15.0 GiB / 200.0 GiB` /
 / * `false` or `null` (no quote marks!): Don't show any device labels. // e.g.
 `Disk: 10.0 GiB / 100.0 GiB` // `Disk: 15.0 GiB / 200.0 GiB` "disk_labels":
 null, // Set to `true` to hide the "Disk" entry name from the output. // i.e.
 null --> `Disk (/):` // false --> `Disk (/):` // true --> `(/):
-` "hide_entry_name": null }, "default_strings": { // Use this section to
-override default strings. }, "ip_settings": { // The maximum number of local
-addresses you want to display. // `false` --> Unlimited. "lan_ip_max_count": 2,
-// `false` would make Archey display IPv4 LAN addresses only.
-"lan_ip_v6_support": true, // `false` would make Archey display IPv4 WAN
-addresses only. "wan_ip_v6_support": true }, "gpu": { // Display GPUs on
-multiple lines if set to `false`. "one_line": true, // The maximum number of
-GPUs you want to display. // `false` --> Unlimited. "max_count": 2 }, "limits":
-{ // Some threshold values you can adjust affecting disk/ram warning/danger
-color (percent). "ram": { "warning": 33.3, "danger": 66.7 }, "disk":
-{ "warning": 50, "danger": 75 } }, "temperature": { // The character to display
-between the temperature value and the unit (as 'Â°' in 53.2Â°C). // Set to ' '
-(space) by default for backward compatibility with non-Unicode locales.
-"char_before_unit": " ", "sensors_chipsets": [ // White-list of chipset
-identifiers (strings) passed to LM-SENSORS when computing the average
-temperature. // Uses `sensors -A` to list the available chipsets on your system
-(e.g. `coretemp-isa-0000`, `acpitz-acpi-0`, ...). // Leaving empty (default)
-would make Archey process input data from each existing chipset. // Use this
-option if a sensor happens to return irrelevant values, or if you want to
-exclude it. ], // Display temperature values in Fahrenheit instead of Celsius.
-"use_fahrenheit": false }, "timeout": { // Some values you can adjust if the
-default ones look undersized for your system (seconds). } } ``` ## Test cases
-An extensive tests suite is available. Here is a short procedure to run them
-(you'll only need `python3`) : ```bash git clone https://github.com/
-HorlogeSkynet/archey4.git cd archey4/ # If you got `setuptools` installed
-python3 setup.py test # But if you don't, no worries ! python3 -m unittest ```
-Any improvement would be appreciated. ## Notes to users * If you experience any
-trouble during the installation or usage, please do **[open an issue](https://
-github.com/HorlogeSkynet/archey4/issues/new)**. * If you had to tweak this
-project to make it work on your system, please **[open a pull request](https://
-github.com/HorlogeSkynet/archey4/pulls)** so as to share your modifications
-with the rest of the world and participate in this project ! You should also
-check [Info for contributors](https://github.com/HorlogeSkynet/archey4/wiki/
-Info-for-contributors). * If your distribution is not (currently) supported,
-please check [How do I add a distribution to Archey?](https://github.com/
-HorlogeSkynet/archey4/wiki/How-do-I-add-a-distribution-to-Archey%3F). * When
-looking up your public IP address (**WAN\_IP**), Archey will try at first to
-run a DNS query for `myip.opendns.com`, against OpenDNS's resolver(s). On
-error, it would fall back on regular HTTPS request(s) to
-ident.me> ([server sources](https://github.com/pcarrier/identme)).
+` "hide_entry_name": null, // Some threshold values you can adjust affecting
+warning/danger colors. "warning_use_percent": 50, "danger_use_percent": 75 },
+{ "type": "WAN_IP", // // As explained above, you may temporary hide entries as
+you wish. // See below example to hide your public IP addresses before posting
+your configuration on Internet. //"disabled": true, // // Below are settings
+relative to IPv4/IPv6 public addresses retrieval. // I hope options are self-
+explanatory. // You may set `dns_query` (or `http_url`) to `false` to disable
+them. // You may directly set `ipv4` or `ipv6` fields to `false` to completely
+disable them. // //
+ident.me/> server sources :
+github.com/pcarrier/identme>. "ipv4": { "dns_query": "myip.opendns.com",
+"dns_resolver": "resolver1.opendns.com", "dns_timeout": 1, "http_url": "https:/
+/v4.ident.me/", "http_timeout": 1 }, "ipv6": { "dns_query": "myip.opendns.com",
+"dns_resolver": "resolver1.opendns.com", "dns_timeout": 1, "http_url": "https:/
+/v6.ident.me/", "http_timeout": 1 } } ], "default_strings": { // Use this
+section to override default strings (internationalization). } } ``` ## Test
+cases An extensive tests suite is available. Here is a short procedure to run
+them (you'll only need `python3`) : ```bash git clone https://github.com/
+HorlogeSkynet/archey4.git cd archey4/ # Run the suite from SetupTools. python3
+setup.py test # Run the suite from the unit testing framework itself. python3 -
+m unittest ``` Any improvement would be appreciated. ## Notes to users * If you
+experience any trouble during the installation or usage, please do **[open an
+issue](https://github.com/HorlogeSkynet/archey4/issues/new)**. * If you had to
+tweak this project to make it work on your system, please **[open a pull
+request](https://github.com/HorlogeSkynet/archey4/pulls)** so as to share your
+modifications with the rest of the world and participate in this project ! You
+should also check [Info for contributors](https://github.com/HorlogeSkynet/
+archey4/wiki/Info-for-contributors). * If your distribution is not (currently)
+supported, please check [How do I add a distribution to Archey?](https://
+github.com/HorlogeSkynet/archey4/wiki/How-do-I-add-a-distribution-to-
+Archey%3F).
```

### Comparing `archey4-4.8.1/archey/__main__.py` & `archey4-4.9.0/archey/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Archey main file.
 It loads each entry as a different class coming from the `entries` module.
 Logos are stored under the `logos` module.
 """
 
 import argparse
 import os
+import sys
 
 from enum import Enum
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import ExitStack
 
 from archey._version import __version__
 from archey.output import Output
@@ -32,16 +33,16 @@
 from archey.entries.terminal import Terminal as e_Terminal
 from archey.entries.packages import Packages as e_Packages
 from archey.entries.temperature import Temperature as e_Temperature
 from archey.entries.cpu import CPU as e_CPU
 from archey.entries.gpu import GPU as e_GPU
 from archey.entries.ram import RAM as e_RAM
 from archey.entries.disk import Disk as e_Disk
-from archey.entries.lan_ip import LanIp as e_LanIp
-from archey.entries.wan_ip import WanIp as e_WanIp
+from archey.entries.lan_ip import LanIP as e_LanIP
+from archey.entries.wan_ip import WanIP as e_WanIP
 
 
 class Entries(Enum):
     """
     An enumeration to store and declare each one of our entries.
     The string representation of keys will act as entries names.
     Values will be set under the `value` attribute of each obtained objects.
@@ -59,16 +60,16 @@
     Terminal = e_Terminal
     Packages = e_Packages
     Temperature = e_Temperature
     CPU = e_CPU
     GPU = e_GPU
     RAM = e_RAM
     Disk = e_Disk
-    LAN_IP = e_LanIp
-    WAN_IP = e_WanIp
+    LAN_IP = e_LanIP
+    WAN_IP = e_WanIP
 
 
 def args_parsing():
     """Simple wrapper to `argparse`"""
     parser = argparse.ArgumentParser(prog='archey')
     parser.add_argument(
         '-c', '--config-path',
@@ -107,45 +108,75 @@
 
     # `Processes` is a singleton, let's populate the internal list here.
     Processes()
 
     # `Configuration` is a singleton, let's populate the internal object here.
     configuration = Configuration(config_path=args.config_path)
 
-    # From configuration, gather the entries user-enabled.
-    enabled_entries = [
-        (entry.value, entry.name)
-        for entry in Entries
-        if configuration.get('entries', {}).get(entry.name, True)
-    ]
+    # From configuration, gather the entries user-configured.
+    available_entries = configuration.get('entries')
+    if available_entries is None:
+        # If none were specified, lazy-mimic a full-enabled entries list without any configuration.
+        available_entries = [{'type': entry_name} for entry_name in Entries.__members__.keys()]
+
+    # @deprecated >= v4.10
+    # v4.9.0 introduces a new configuration layout.
+    # This statement performs a transformation to avoid crash if the old layout is being used.
+    # Some user options **WILL** be ignored.
+    elif isinstance(available_entries, dict):
+        print(
+            'Warning: Deprecated configuration layout detected, please update !',
+            file=sys.stderr
+        )
+        available_entries = [
+            {'type': entry_name}
+            for entry_name, is_entry_enabled in available_entries.items()
+            if is_entry_enabled
+        ]
 
     output = Output(
         preferred_distribution=args.distribution,
         format_to_json=args.json
     )
 
     # We will map this function onto our enabled entries to instantiate them.
-    def _entry_instantiator(entry_tuple):
-        return entry_tuple[0](name=entry_tuple[1])
+    def _entry_instantiator(entry):
+        # Based on **required** `type` field, instantiate the corresponding `Entry` object.
+        try:
+            return Entries[entry.pop('type')].value(
+                name=entry.pop('name', None),  # `name` is fully-optional.
+                options=entry                  # Remaining fields should be propagated as options.
+            )
+        except KeyError as key_error:
+            print(
+                'Warning: One entry (misses or) uses an invalid `type` field ({}).'.format(
+                    key_error
+                ),
+                file=sys.stderr
+            )
+            return None
 
     # Let's use a context manager stack to manage conditional use of `TheadPoolExecutor`.
     with ExitStack() as cm_stack:
         if not configuration.get('parallel_loading'):
             mapper = map
         else:
             # Instantiate a threads pool to load our enabled entries in parallel.
             # We use threads (and not processes) since most work done by our entries is IO-bound.
             # `max_workers` is manually computed to mimic Python 3.8+ behaviour, but for our needs.
             #   See <https://github.com/python/cpython/pull/13618>.
             executor = cm_stack.enter_context(ThreadPoolExecutor(
-                max_workers=min(len(enabled_entries) or 1, (os.cpu_count() or 1) + 4)
+                max_workers=min(len(available_entries) or 1, (os.cpu_count() or 1) + 4)
             ))
             mapper = executor.map
 
-        for entry_instance in mapper(_entry_instantiator, enabled_entries):
+        for entry_instance in mapper(_entry_instantiator, available_entries):
+            if not entry_instance:
+                continue
+
             output.add_entry(entry_instance)
 
     output.output()
 
     # Has the screenshot flag been specified ?
     if args.screenshot is not None:
         # If so, but still _falsy_, pass `None` as no output file has been specified by the user.
```

### Comparing `archey4-4.8.1/archey/api.py` & `archey4-4.9.0/archey/api.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/colors.py` & `archey4-4.9.0/archey/colors.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/configuration.py` & `archey4-4.9.0/archey/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         # If a `config_path` has been specified, (try to) load it directly.
         if config_path:
             self._load_configuration(config_path)
         # If not, load each (optional) configuration file in a "regular" order.
         else:
             self._load_configuration('/etc/archey4/')
             self._load_configuration(os.path.expanduser('~/.config/archey4/'))
-            self._load_configuration(os.path.dirname(os.path.realpath(__file__)))
+            self._load_configuration(os.getcwd())
 
     def get(self, key, default=None):
         """
         A binding method to imitate the `dict.get()` behavior.
         """
         return self._config.get(key, default)
```

### Comparing `archey4-4.8.1/archey/distributions.py` & `archey4-4.9.0/archey/distributions.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/desktop_environment.py` & `archey4-4.9.0/archey/entries/desktop_environment.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/disk.py` & `archey4-4.9.0/archey/entries/disk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Disk usage detection class"""
 
 import re
-from subprocess import CalledProcessError, check_output
+from subprocess import DEVNULL, PIPE, Popen
 from csv import reader as csv_reader
 
 from archey.colors import Colors
 from archey.entry import Entry
 
 
 class Disk(Entry):
     """Uses `df` to compute disk usage across devices"""
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Populate an output from `df`
-        self._disk_dict = self.get_df_output_dict()
+        self._disk_dict = self._get_df_output_dict()
 
-        config_filesystems = self._configuration.get('disk')['show_filesystems']
-        # See `Disk.get_df_output_dict` for the format we use in `self.value`.
+        config_filesystems = self.options.get('show_filesystems', ['local'])
+        # See `Disk._get_df_output_dict` for the format we use in `self.value`.
         if config_filesystems == ['local']:
             self.value = self._get_local_filesystems()
         else:
             self.value = self._get_specified_filesystems(config_filesystems)
 
 
     def _get_local_filesystems(self):
@@ -84,15 +84,15 @@
                     # We only need one match, so we can stop when it's found.
                     break
 
         return specified_disk_dict
 
 
     @staticmethod
-    def get_df_output_dict():
+    def _get_df_output_dict():
         """
         Runs `df -P -k` and returns disks in a dict formatted as:
         {
             'mount_point_1': {
                 'device_path': AAA,
                 'used_blocks': BBB,
                 'total_blocks': CCC
@@ -102,19 +102,24 @@
                 'used_blocks': YYY,
                 'total_blocks': ZZZ
             }
         }
         Mount points are used as keys since they are always unique.
         """
         try:
-            df_output = check_output(
+            df_output = Popen(
                 ['df', '-P', '-k'],
-                env={'LANG': 'C'}, universal_newlines=True
-            )
-        except (FileNotFoundError, CalledProcessError):
+                env={'LANG': 'C'}, universal_newlines=True,
+                stdout=PIPE,
+                # On error, `df` may "hold" `EXIT_FAILURE` as exit status code.
+                # Thus, we purposely silence STDERR and ignore its returned status code.
+                # See #92 (related to flatpak/xdg-desktop-portal#512).
+                stderr=DEVNULL
+            ).stdout.read()
+        except FileNotFoundError:
             # `df` isn't available on this system.
             return {}
 
         # Parse this output as a table in SSV (space-separated values) format
         ssv_reader = csv_reader(
             df_output.splitlines()[1:],  # Discard the header row here.
             delimiter=' ',
@@ -155,19 +160,19 @@
 
         if not filesystems:
             # We didn't find any disk, fall back to the default entry behavior.
             super().output(output)
             return
 
         # DRY configuration object for the output.
-        disk_labels = self._configuration.get('disk')['disk_labels']
-        hide_entry_name = self._configuration.get('disk')['hide_entry_name']
+        disk_labels = self.options.get('disk_labels')
+        hide_entry_name = self.options.get('hide_entry_name')
 
         # Combine all entries into one grand-total if configured to do so.
-        if self._configuration.get('disk')['combine_total']:
+        if self.options.get('combine_total', True):
             name = self.name
 
             # Rewrite our `filesystems` object as one combining all of them.
             filesystems = {
                 None: {
                     'device_path': None,
                     'used_blocks': sum([
@@ -187,23 +192,21 @@
             if not hide_entry_name or not disk_labels:
                 name += self.name
             if disk_labels:
                 if not hide_entry_name:
                     name += ' '
                 name += '({disk_label})'
 
-        # Fetch the user-defined limits from the configuration.
-        disk_limits = self._configuration.get('limits')['disk']
-
         # We will only run this loop a single time for combined entries.
         for mount_point, filesystem_data in filesystems.items():
             # Select the corresponding level color based on disk percentage usage.
             level_color = Colors.get_level_color(
                 (filesystem_data['used_blocks'] / filesystem_data['total_blocks']) * 100,
-                disk_limits['warning'], disk_limits['danger']
+                self.options.get('warning_use_percent', 50),
+                self.options.get('danger_use_percent', 75)
             )
 
             # Set the correct disk label
             if disk_labels == 'mount_points':
                 disk_label = mount_point
             elif disk_labels == 'device_paths':
                 disk_label = filesystem_data['device_path']
```

### Comparing `archey4-4.8.1/archey/entries/distro.py` & `archey4-4.9.0/archey/entries/distro.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         return 'Android {0}'.format(release)
 
 
     def output(self, output):
         output.append(
             self.name,
             '{0} [{1}]'.format(
-                (self.value['name'] or self._configuration.get('default_strings')['not_detected']),
+                (self.value['name'] or self._default_strings.get('not_detected')),
                 self.value['arch']
             )
         )
```

### Comparing `archey4-4.8.1/archey/entries/gpu.py` & `archey4-4.9.0/archey/entries/gpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class GPU(Entry):
     """Relies on `lspci` to retrieve graphical device(s) information"""
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        max_count = self._configuration.get('gpu')['max_count']
+        max_count = self.options.get('max_count', 2)
         # Consistency with other entries' configuration: Infinite count if false.
         if max_count is False:
             max_count = None
 
         # Populate our list of devices with the `lspci`-based generator.
         self.value = list(islice(self._gpu_generator(), max_count))
 
@@ -37,16 +37,18 @@
                 if video_key in pci_device:
                     # ... return its name on the next iteration.
                     yield pci_device.partition(': ')[2]
 
 
     def output(self, output):
         """Writes GPUs to `output` based on preferences"""
-        # Even when no GPU device could be detected, be sure to add an "empty" entry to `output`.
-        if self._configuration.get('gpu')['one_line'] or not self.value:
-            output.append(
-                self.name,
-                ', '.join(self.value) or self._configuration.get('default_strings')['not_detected']
-            )
+        # No GPU could be detected.
+        if not self.value:
+            output.append(self.name, self._default_strings.get('not_detected'))
+            return
+
+        # Join the results only if `one_line` option is enabled.
+        if self.options.get('one_line'):
+            output.append(self.name, ', '.join(self.value))
         else:
             for gpu_device in self.value:
                 output.append(self.name, gpu_device)
```

### Comparing `archey4-4.8.1/archey/entries/hostname.py` & `archey4-4.9.0/archey/entries/hostname.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/model.py` & `archey4-4.9.0/archey/entries/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     """Uses multiple methods to retrieve some information about the host hardware"""
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.value = \
             self._fetch_virtual_env_info() \
             or self._fetch_product_info() \
-            or self._fetch_rasperry_pi_revision() \
-            or self._fetch_android_device_model() \
+            or self._fetch_raspberry_pi_revision() \
+            or self._fetch_android_device_model()
 
     def _fetch_virtual_env_info(self):
         """
         Relying on some system tools, tries to gather some details about hypervisor.
         When available, relies on systemd.
         When run as root, `virt-what` and/or `dmidecode` may be called.
         """
@@ -66,40 +66,44 @@
                 pass
         elif not environment:
             # No detection tool is available...
             return None
 
         # If we got there with some info, this _should_ be a virtual environment.
         return '{0} ({1})'.format(
-            product_name or self._configuration.get('default_strings')['virtual_environment'],
+            product_name or self._default_strings.get('virtual_environment'),
             environment
         )
 
     @staticmethod
     def _fetch_product_info():
         """Tries to open specific Linux files, looking for hardware product name and version"""
         try:
             with open('/sys/devices/virtual/dmi/id/product_name') as f_product_name:
                 product_name = f_product_name.read().rstrip()
         except FileNotFoundError:
             return None
 
+        # Stop `/sys/devices/virtual/dmi/id/*` parsing on fuzzy data.
+        if re.search(r'To Be Filled', product_name, re.IGNORECASE):
+            return None
+
         try:
             with open('/sys/devices/virtual/dmi/id/product_version') as f_product_version:
                 product_version = f_product_version.read().rstrip()
         except FileNotFoundError:
             product_version = None
 
         if not product_version:
             return product_name
 
         return "{} {}".format(product_name, product_version)
 
     @staticmethod
-    def _fetch_rasperry_pi_revision():
+    def _fetch_raspberry_pi_revision():
         """Tries to retrieve 'Hardware' and 'Revision IDs' from `/proc/cpuinfo`"""
         try:
             with open('/proc/cpuinfo') as f_cpu_info:
                 cpu_info = f_cpu_info.read()
         except (PermissionError, FileNotFoundError):
             return None
```

### Comparing `archey4-4.8.1/archey/entries/packages.py` & `archey4-4.9.0/archey/entries/packages.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/ram.py` & `archey4-4.9.0/archey/entries/ram.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,21 +94,20 @@
             super().output(output)
             return
 
         # DRY some constants
         used = self.value['used']
         total = self.value['total']
         unit = self.value['unit']
-        # Fetch the user-defined RAM limits from configuration.
-        ram_limits = self._configuration.get('limits')['ram']
 
         # Based on the RAM percentage usage, select the corresponding level color.
         level_color = Colors.get_level_color(
             (used / total) * 100,
-            ram_limits['warning'], ram_limits['danger']
+            self.options.get('warning_use_percent', 33.3),
+            self.options.get('danger_use_percent', 66.7)
         )
 
         output.append(
             self.name,
             '{0}{1} {unit}{2} / {3} {unit}'.format(
                 level_color,
                 int(used),
```

### Comparing `archey4-4.8.1/archey/entries/shell.py` & `archey4-4.9.0/archey/entries/shell.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/temperature.py` & `archey4-4.9.0/archey/entries/temperature.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,30 +17,30 @@
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._temps = []
 
         # Tries `sensors` at first.
-        self._run_sensors(self._configuration.get('temperature')['sensors_chipsets'])
+        self._run_sensors(self.options.get('sensors_chipsets', []))
 
         # On error (list still empty), checks for system thermal zones files.
         if not self._temps:
             self._poll_thermal_zones()
 
         # Tries `vcgencmd` for Raspberry devices.
         self._run_vcgencmd()
 
         # No value could be fetched...
         if not self._temps:
             return
 
         # Let's DRY some constants once.
-        use_fahrenheit = self._configuration.get('temperature')['use_fahrenheit']
-        char_before_unit = self._configuration.get('temperature')['char_before_unit']
+        use_fahrenheit = self.options.get('use_fahrenheit')
+        char_before_unit = self.options.get('char_before_unit', ' ')
 
         # Conversion to Fahrenheit if needed.
         if use_fahrenheit:
             self._temps = list(map(self._convert_to_fahrenheit, self._temps))
 
         # Final average and maximum computations.
         self.value = {
```

### Comparing `archey4-4.8.1/archey/entries/terminal.py` & `archey4-4.9.0/archey/entries/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
         self.value = self._detect_terminal_emulator()
 
     def _get_colors_palette(self):
         """Build and return a 8-color palette, with Unicode characters if allowed"""
         # On systems with non-Unicode locales, we imitate '\u2588' character
         # ... with '#' to display the terminal colors palette.
-        use_unicode = self._configuration.get('colors_palette')['use_unicode']
+        # Archey >= v4.8.0, Unicode is enabled by default.
+        use_unicode = self.options.get('use_unicode', True)
 
         return ' '.join([
             '{normal}{character}{bright}{character}{clear}'.format(
                 normal=Colors((0, i)),
                 bright=Colors((1, i)),
                 character=('\u2588' if use_unicode else '#'),
                 clear=Colors.CLEAR
@@ -113,12 +114,12 @@
         # When nothing of the above matched, falls-back on the regular `TERM` environment variable.
         # Note : It _might_ be `None` in very specific environments.
         return env_term
 
 
     def output(self, output):
         """Adds the entry to `output` after pretty-formatting with colors palette"""
-        text_output = (self.value or self._configuration.get('default_strings')['not_detected'])
+        text_output = (self.value or self._default_strings.get('not_detected'))
         if not NO_COLOR:
             text_output += ' ' + self._get_colors_palette()
 
         output.append(self.name, text_output)
```

### Comparing `archey4-4.8.1/archey/entries/uptime.py` & `archey4-4.9.0/archey/entries/uptime.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/user.py` & `archey4-4.9.0/archey/entries/user.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entries/window_manager.py` & `archey4-4.9.0/archey/entries/window_manager.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/entry.py` & `archey4-4.9.0/archey/entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 
 from archey.configuration import Configuration
 
 
 class Entry(AbstractBaseClass):
     """Module base class"""
     @abstractmethod
-    def __init__(self, name=None, value=None):
+    def __init__(self, name=None, value=None, options=None):
         # Each entry will have always have the following attributes...
-        # `name` (key);
-        # `value` (value of entry as an appropriate object)
-        # ... which are `None` by default.
-        self.name = name
+        # `name`: key (defaults to the instantiated entry class name);
+        # `value`: value of entry as an appropriate object;
+        # `options`: configuration options *specific* to an entry instance;
+        self.name = name or self.__class__.__name__
         self.value = value
+        self.options = options or {}
 
-        # Propagates a reference to `Configuration` singleton to each inheriting class.
-        self._configuration = Configuration()
+        # Propagates a reference to default strings specified in `Configuration`.
+        self._default_strings = Configuration().get('default_strings')
 
+    def __bool__(self):
+        """Makes an `Entry` evaluates to _falsy_ if `disabled` config field is _truthy_"""
+        return not bool(self.options.get('disabled'))
 
     def output(self, output):
         """Output the results to output. Can be overridden by subclasses."""
         if self.value:
             # Let's assume we can just use `__str__` on the object in value,
             # and create a single-line output with it.
             output.append(self.name, str(self.value))
         else:
             # If the value is "falsy" leave a generic "Not detected" message for this entry.
             output.append(
                 self.name,
-                self._configuration.get('default_strings')['not_detected']
+                self._default_strings.get('not_detected')
             )
```

### Comparing `archey4-4.8.1/archey/logos/__init__.py` & `archey4-4.9.0/archey/logos/__init__.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/alpine_linux.py` & `archey4-4.9.0/archey/logos/alpine_linux.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/android.py` & `archey4-4.9.0/archey/logos/android.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/arch_linux.py` & `archey4-4.9.0/archey/logos/arch_linux.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/bunsenlabs.py` & `archey4-4.9.0/archey/logos/bunsenlabs.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/centos.py` & `archey4-4.9.0/archey/logos/centos.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/crunchbang.py` & `archey4-4.9.0/archey/logos/crunchbang.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/debian.py` & `archey4-4.9.0/archey/logos/debian.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/elementary.py` & `archey4-4.9.0/archey/logos/elementary.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/fedora.py` & `archey4-4.9.0/archey/logos/fedora.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/freebsd.py` & `archey4-4.9.0/archey/logos/freebsd.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/gentoo.py` & `archey4-4.9.0/archey/logos/gentoo.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/kali_linux.py` & `archey4-4.9.0/archey/logos/kali_linux.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/linux.py` & `archey4-4.9.0/archey/logos/linux.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/linux_mint.py` & `archey4-4.9.0/archey/logos/linux_mint.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/manjaro.py` & `archey4-4.9.0/archey/logos/manjaro.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/nixos.py` & `archey4-4.9.0/archey/logos/nixos.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/openbsd.py` & `archey4-4.9.0/archey/logos/openbsd.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/opensuse.py` & `archey4-4.9.0/archey/logos/opensuse.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/pop.py` & `archey4-4.9.0/archey/logos/pop.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/raspbian.py` & `archey4-4.9.0/archey/logos/raspbian.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/red_hat.py` & `archey4-4.9.0/archey/logos/red_hat.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/slackware.py` & `archey4-4.9.0/archey/logos/slackware.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/ubuntu.py` & `archey4-4.9.0/archey/logos/ubuntu.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/logos/windows.py` & `archey4-4.9.0/archey/logos/windows.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/output.py` & `archey4-4.9.0/archey/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             self._distribution = Distributions.run_detection()
 
         # Fetch the colors palette related to this distribution.
         self._colors_palette = COLORS_DICT[self._distribution]
 
         # If `os-release`'s `ANSI_COLOR` option is set, honor it.
         ansi_color = Distributions.get_ansi_color()
-        if ansi_color and Configuration().get('colors_palette')['honor_ansi_color']:
+        if ansi_color and Configuration().get('honor_ansi_color'):
             # Replace each Archey integrated colors by `ANSI_COLOR`.
             self._colors_palette = len(self._colors_palette) * \
                 [Colors.escape_code_from_attrs(ansi_color)]
 
         # Each entry will be added to this list
         self._entries = []
         # Each class output will be added in the list below afterwards
```

### Comparing `archey4-4.8.1/archey/processes.py` & `archey4-4.9.0/archey/processes.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/screenshot.py` & `archey4-4.9.0/archey/screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     output_dir = os.path.dirname(output_file)
 
     # Back-end programs that _may_ (?) be available across different platforms.
     screenshot_tools = {
         'Flameshot': ['flameshot', 'full', '-p', output_dir],
         'ImageMagick': ['import', '-window', 'root', output_file],
         'scrot': ['scrot', '-z', output_file],
-        'Shutter': ['shutter', '-f', '-o', output_file, '-e'],
+        'Shutter': ['shutter', '-f', '-o', output_file, '-e']
     }
 
     # Extends the original screenshot tools dictionary according to current platform.
     if sys.platform in ('win32', 'cygwin'):
         screenshot_tools['SnippingTool'] = ['SnippingTool.exe', '/clip']
     elif sys.platform == 'darwin':
         screenshot_tools['ScreenCapture'] = [
```

### Comparing `archey4-4.8.1/archey/singleton.py` & `archey4-4.9.0/archey/singleton.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/__init__.py` & `archey4-4.9.0/archey/test/entries/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,62 +13,64 @@
 
 class HelperMethods:
     """
     This class contains helper methods we commonly use in our entry unit tests.
     We kindly borrow `update_recursive` class method from `Configuration` to DRY its implementation.
     """
     @staticmethod
-    def entry_mock(entry, configuration=None):
+    def entry_mock(entry, options=None, configuration=None):
         """
         Creates a placeholder "instance" of the entry class passed, with a clean default
-        `_configuration` which is optionally updated by `configuration`.
+        `_default_strings` which is optionally updated by `configuration`.
 
         It can be used to very cleanly unit-test instance methods of a class,
         by passing it in (after setting appropriate attributes).
 
         The attributes defined are not instance attributes, however since this isn't
         technically an instance, they are used in place of the respective instance attributes.
         """
         # We spec to the entry so non-existent methods can't be called...
         # ...and wrap it, to inherit its methods.
         instance_mock = MagicMock(spec=entry, wraps=entry)
         # These instance-attributes are quite important, so let's mimic them.
         instance_mock.name = str(entry.__name__)
         instance_mock.value = None  # (entry default)
+        # We don't have default entry options defined outside of entries.
+        instance_mock.options = options or {}
 
         # Let's initially give the entry configuration the defaults.
         # We deep-copy `DEFAULT_CONFIG` to prevent its mutation.
-        entry_configuration = deepcopy(DEFAULT_CONFIG)
+        default_configuration = deepcopy(DEFAULT_CONFIG)
         # Then, let's merge in `configuration` recursively.
-        Configuration.update_recursive(entry_configuration, (configuration or {}))
-        # Finally, replaces the internal (and private!) `_configuration` attribute by...
-        # ... the corresponding configuration object.
-        setattr(instance_mock, '_configuration', entry_configuration)
+        Configuration.update_recursive(default_configuration, (configuration or {}))
+        # Finally, replaces the internal (and private!) `_default_strings` attribute by...
+        # ... the corresponding object from configuration.
+        setattr(instance_mock, '_default_strings', default_configuration.get('default_strings'))
 
         return instance_mock
 
     @staticmethod
     def patch_clean_configuration(method_definition=None, *, configuration=None):
         """
-        Decorator for an entry test definition, which sets the entry's `_configuration` attribute to
-        the Archey defaults, optionally updated with `configuration`.
+        Decorator for an entry test definition, which sets the entry's `_default_strings` attribute
+        to the Archey defaults, optionally updated with `configuration`.
         """
         # Let's initially give the entry configuration the defaults.
         # We deep-copy `DEFAULT_CONFIG` to prevent its mutation.
         entry_configuration = deepcopy(DEFAULT_CONFIG)
         # Then, let's merge in `configuration` recursively.
         Configuration.update_recursive(entry_configuration, (configuration or {}))
 
         def decorator_patch_clean_configuration(method):
             @wraps(method)
             def wrapper_patch_clean_configuration(*args, **kwargs):
                 with patch('archey.entry.Configuration', autospec=True) as config_instance_mock:
                     # Mock "publicly" used methods.
                     config_instance_mock().get = entry_configuration.get
-                    config_instance_mock().__iter__ = lambda _: iter(entry_configuration.items())
+                    config_instance_mock().__iter__ = iter(entry_configuration.items())
                     return method(*args, **kwargs)
 
             return wrapper_patch_clean_configuration
 
         if method_definition is None:
             return decorator_patch_clean_configuration
 
@@ -94,15 +96,18 @@
             return 42
 
     def test_entry_mock_defaults(self):
         """Test `entry_mock`s default attributes."""
         simple_mock_instance = self.entry_mock(TestHelperMethods._SimpleEntry)
         self.assertEqual(simple_mock_instance.name, '_SimpleEntry')
         self.assertIsNone(simple_mock_instance.value)
-        self.assertDictEqual(simple_mock_instance._configuration, DEFAULT_CONFIG)  # pylint: disable=protected-access
+        self.assertDictEqual(
+            simple_mock_instance._default_strings,  # pylint: disable=protected-access
+            DEFAULT_CONFIG.get('default_strings')
+        )
 
     def test_entry_mock_spec(self):
         """Test `entry_mock`s speccing."""
         simple_mock_instance = self.entry_mock(TestHelperMethods._SimpleEntry)
         with self.assertRaises(AttributeError):
             # We shouldn't be able to call methods that don't exist...
             simple_mock_instance.not_a_method()
@@ -122,59 +127,57 @@
     @patch.dict(
         DEFAULT_CONFIG,
         values={
             'a_key': 'a_value',
             'a_dict': {
                 'key_1': 1,
                 'key_2': 2
-            }
+            },
+            'default_strings': {}
         },
         clear=True
     )
     def test_entry_mock_configuration_setting(self):
         """Test `entry_mock`s configuration setting."""
         configuration_dict = {
             'another_key': 'another_value',  # Adding a key-value pair.
             'a_dict': {
                 'key_1': 10  # Updating a nested key-value pair.
             }
         }
-        simple_mock_instance = self.entry_mock(TestHelperMethods._SimpleEntry, configuration_dict)
+        simple_mock_instance = self.entry_mock(
+            TestHelperMethods._SimpleEntry,
+            configuration=configuration_dict
+        )
         self.assertDictEqual(
-            simple_mock_instance._configuration,  # pylint: disable=protected-access
-            {
-                'a_key': 'a_value',
-                'another_key': 'another_value',
-                'a_dict': {
-                    'key_1': 10,
-                    'key_2': 2
-                }
-            }
+            simple_mock_instance._default_strings,  # pylint: disable=protected-access
+            DEFAULT_CONFIG.get('default_strings')
         )
 
     def test_patch_clean_configuration_defaults(self):
         """Test the default configuration-setting of `patch_clean_configuration."""
         @HelperMethods.patch_clean_configuration
         def test(self):
             simple_entry = TestHelperMethods._SimpleEntry()
             self.assertDictEqual(
-                dict(simple_entry._configuration),  # pylint: disable=protected-access
-                DEFAULT_CONFIG
+                simple_entry._default_strings,  # pylint: disable=protected-access
+                DEFAULT_CONFIG.get('default_strings')
             )
 
         test(self)
 
     @patch.dict(
         DEFAULT_CONFIG,
         values={
             'a_key': 'a_value',
             'a_dict': {
                 'key_1': 1,
                 'key_2': 2
-            }
+            },
+            'default_strings': {}
         },
         clear=True
     )
     def test_patch_clean_configuration_setting(self):
         """Test `patch_clean_configuration`s configuration setting."""
         configuration_dict = {
             'another_key': 'another_value',  # Adding a key-value pair.
@@ -184,19 +187,12 @@
         }
         @HelperMethods.patch_clean_configuration(
             configuration=configuration_dict
         )
         def test(self):
             simple_entry = TestHelperMethods._SimpleEntry()
             self.assertDictEqual(
-                dict(simple_entry._configuration),  # pylint: disable=protected-access
-                {
-                    'a_key': 'a_value',
-                    'another_key': 'another_value',
-                    'a_dict': {
-                        'key_1': 10,
-                        'key_2': 2
-                    }
-                }
+                simple_entry._default_strings,  # pylint: disable=protected-access
+                DEFAULT_CONFIG.get('default_strings')
             )
 
         test(self)
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_desktop_environment.py` & `archey4-4.9.0/archey/test/entries/test_archey_desktop_environment.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_disk.py` & `archey4-4.9.0/archey/test/entries/test_archey_disk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Test module for Archey's disks usage detection module"""
 
-import os
 import unittest
 from unittest.mock import call, patch, MagicMock
 
 from archey.colors import Colors
 from archey.entries.disk import Disk
 from archey.test.entries import HelperMethods
 
 
 class TestDiskEntry(unittest.TestCase):
     """
-    Here, we mock `check_output` calls to disk utility tools.
+    Here, we mock `subprocess.run` calls to disk utility tools.
     """
     def setUp(self):
         """We use these mocks so often, it's worth defining them here."""
         self.disk_instance_mock = HelperMethods.entry_mock(Disk)
         self.output_mock = MagicMock()
 
     def test_disk_get_local_filesystems(self):
@@ -125,55 +124,50 @@
             # As long as `device_path` is also correct, this passes.
             self.assertEqual(
                 result_disk_dict[list(result_disk_dict.keys())[0]]['device_path'],
                 '/dev/sda1'
             )
 
 
-    @patch(
-        'archey.entries.disk.check_output',
-        side_effect=[
-            # First `df` call succeeds.
-            os.linesep.join((
+    @patch('archey.entries.disk.Popen')
+    def test_disk_df_output_dict(self, popen_mock):
+        """Test method to get `df` output as a dict by mocking calls to `Popen`"""
+        with self.subTest('`df` regular output.'):
+            popen_mock.return_value.stdout.read.return_value = '\n'.join([
                 "Filesystem               1024-blocks      Used     Available Capacity Mounted on",
                 "/dev/nvme0n1p2             499581952 427458276      67779164      87% /",
                 "tmpfs                        8127236       292       8126944       1% /tmp",
                 "/dev/nvme0n1p1                523248     35908        487340       7% /boot",
                 ""
-            )),
-            # Second `df` call fails (emulating it not being present).
-            FileNotFoundError
-        ]
-    )
-    def test_disk_df_output_dict(self, _):
-        """Test method to get `df` output as a dict by mocking calls to `check_output`."""
-        self.assertDictEqual(
-            Disk.get_df_output_dict(),
-            {
-                '/': {
-                    'device_path': '/dev/nvme0n1p2',
-                    'used_blocks': 427458276,
-                    'total_blocks': 499581952
-                },
-                '/tmp': {
-                    'device_path': 'tmpfs',
-                    'used_blocks': 292,
-                    'total_blocks': 8127236
-                },
-                '/boot': {
-                    'device_path': '/dev/nvme0n1p1',
-                    'used_blocks': 35908,
-                    'total_blocks': 523248
+            ])
+            self.assertDictEqual(
+                Disk._get_df_output_dict(),  # pylint: disable=protected-access
+                {
+                    '/': {
+                        'device_path': '/dev/nvme0n1p2',
+                        'used_blocks': 427458276,
+                        'total_blocks': 499581952
+                    },
+                    '/tmp': {
+                        'device_path': 'tmpfs',
+                        'used_blocks': 292,
+                        'total_blocks': 8127236
+                    },
+                    '/boot': {
+                        'device_path': '/dev/nvme0n1p1',
+                        'used_blocks': 35908,
+                        'total_blocks': 523248
+                    }
                 }
-            }
-        )
+            )
 
-        with self.subTest('Missing `df` from system.'):
+        with self.subTest('`df` missing from system.'):
+            popen_mock.side_effect = FileNotFoundError()
             self.assertDictEqual(
-                Disk.get_df_output_dict(),
+                Disk._get_df_output_dict(),  # pylint: disable=protected-access
                 {}
             )
 
     def test_disk_blocks_to_human_readable(self):
         """Test method to convert 1024-byte blocks to a human readable format."""
         # Each tuple is a number of blocks followed by the expected output.
         test_cases = (
@@ -246,15 +240,15 @@
                 'Disk',
                 '{0}20.0 KiB{1} / 40.0 KiB'.format(Colors.YELLOW_NORMAL, Colors.CLEAR)
             )
 
         self.output_mock.reset_mock()
 
         with self.subTest('Multi-line output'):
-            self.disk_instance_mock._configuration['disk']['combine_total'] = False  # pylint: disable=protected-access
+            self.disk_instance_mock.options['combine_total'] = False
             Disk.output(self.disk_instance_mock, self.output_mock)
             self.assertEqual(self.output_mock.append.call_count, 2)
             self.output_mock.append.assert_has_calls(
                 [
                     call(
                         'Disk',
                         '{0}10.0 KiB{1} / 10.0 KiB'.format(Colors.RED_NORMAL, Colors.CLEAR)
@@ -266,16 +260,18 @@
                 ],
                 any_order=True  # Since Python < 3.6 doesn't have definite `dict` ordering.
             )
 
         self.output_mock.reset_mock()
 
         with self.subTest('Entry name labeling (device path with entry name)'):
-            self.disk_instance_mock._configuration['disk']['combine_total'] = False  # pylint: disable=protected-access
-            self.disk_instance_mock._configuration['disk']['disk_labels'] = 'device_paths'  # pylint: disable=protected-access
+            self.disk_instance_mock.options = {
+                'combine_total': False,
+                'disk_labels': 'device_paths'
+            }
 
             Disk.output(self.disk_instance_mock, self.output_mock)
             self.assertEqual(self.output_mock.append.call_count, 2)
             self.output_mock.append.assert_has_calls(
                 [
                     call(
                         'Disk (/dev/my-cool-disk)',
@@ -288,17 +284,19 @@
                 ],
                 any_order=True  # Since Python < 3.6 doesn't have definite `dict` ordering.
             )
 
         self.output_mock.reset_mock()
 
         with self.subTest('Entry name labeling (mount points without entry name)'):
-            self.disk_instance_mock._configuration['disk']['combine_total'] = False  # pylint: disable=protected-access
-            self.disk_instance_mock._configuration['disk']['disk_labels'] = 'mount_points'  # pylint: disable=protected-access
-            self.disk_instance_mock._configuration['disk']['hide_entry_name'] = True  # pylint: disable=protected-access
+            self.disk_instance_mock.options = {
+                'combine_total': False,
+                'disk_labels': 'mount_points',
+                'hide_entry_name': True
+            }
 
             Disk.output(self.disk_instance_mock, self.output_mock)
             self.assertEqual(self.output_mock.append.call_count, 2)
             self.output_mock.append.assert_has_calls(
                 [
                     call(
                         '(first_mount_point)',
@@ -311,18 +309,20 @@
                 ],
                 any_order=True  # Since Python < 3.6 doesn't have definite `dict` ordering.
             )
 
         self.output_mock.reset_mock()
 
         with self.subTest('Entry name labeling (without disk label nor entry name)'):
-            self.disk_instance_mock._configuration['disk']['combine_total'] = False  # pylint: disable=protected-access
-            self.disk_instance_mock._configuration['disk']['disk_labels'] = False  # pylint: disable=protected-access
-            # `hide_entry_name` is being ignored as `disk_labels` evaluates to "falsy" too.
-            self.disk_instance_mock._configuration['disk']['hide_entry_name'] = True  # pylint: disable=protected-access
+            self.disk_instance_mock.options = {
+                'combine_total': False,
+                'disk_labels': False,
+                # `hide_entry_name` is being ignored as `disk_labels` evaluates to "falsy" too.
+                'hide_entry_name': True
+            }
 
             Disk.output(self.disk_instance_mock, self.output_mock)
             self.assertEqual(self.output_mock.append.call_count, 2)
             self.output_mock.append.assert_has_calls(
                 [
                     call(
                         'Disk',
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_distro.py` & `archey4-4.9.0/archey/test/entries/test_archey_distro.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_gpu.py` & `archey4-4.9.0/archey/test/entries/test_archey_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,43 +17,37 @@
         'archey.entries.gpu.check_output',
         return_value="""\
 XX:YY.H IDE interface: IIIIIIIIIIIIIIII
 XX:YY.H SMBus: BBBBBBBBBBBBBBBB
 XX:YY.H VGA compatible controller: GPU-MODEL-NAME
 XX:YY.H Audio device: DDDDDDDDDDDDDDDD
 """)
-    @HelperMethods.patch_clean_configuration
     def test_match_vga(self, _):
         """Simple 'VGA' device type matching"""
         self.assertListEqual(GPU().value, ['GPU-MODEL-NAME'])
 
     @patch(
         'archey.entries.gpu.check_output',
         return_value="""\
 XX:YY.H IDE interface: IIIIIIIIIIIIIIII
 XX:YY.H SMBus: BBBBBBBBBBBBBBBB
 XX:YY.H VGA compatible controller: GPU-MODEL-NAME
 XX:YY.H Display controller: ANOTHER-MATCHING-VIDEO-CONTROLLER
 XX:YY.H Audio device: DDDDDDDDDDDDDDDD
 XX:YY.H 3D controller: 3D GPU-MODEL-NAME TAKES ADVANTAGE
 """)
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'gpu': {
-                'one_line': True,
-                'max_count': 2
-            }
-        }
-    )
     def test_multi_matches_capped_one_line(self, _):
         """
         Test detection when there are multiple graphical device candidates.
         Check that `max_count` and `one_line` are honored too, including on `output` overriding.
         """
-        gpu = GPU()
+        gpu = GPU(options={
+            'one_line': True,
+            'max_count': 2
+        })
 
         output_mock = MagicMock()
         gpu.output(output_mock)
 
         self.assertListEqual(
             gpu.value,
             ['3D GPU-MODEL-NAME TAKES ADVANTAGE', 'GPU-MODEL-NAME']
@@ -68,28 +62,23 @@
         return_value="""\
 XX:YY.H IDE interface: IIIIIIIIIIIIIIII
 XX:YY.H SMBus: BBBBBBBBBBBBBBBB
 XX:YY.H Display controller: ANOTHER-MATCHING-VIDEO-CONTROLLER
 XX:YY.H Audio device: DDDDDDDDDDDDDDDD
 XX:YY.H 3D controller: 3D GPU-MODEL-NAME TAKES ADVANTAGE
 """)
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'gpu': {
-                'one_line': False,
-                'max_count': False
-            }
-        }
-    )
     def test_multi_matches_uncapped_multiple_lines(self, _):
         """
         Test detection when there are multiple graphical device candidates.
         Check that `max_count` and `one_line` are honored too, including on `output` overriding.
         """
-        gpu = GPU()
+        gpu = GPU(options={
+            'one_line': False,
+            'max_count': False
+        })
 
         output_mock = MagicMock()
         gpu.output(output_mock)
 
         self.assertListEqual(
             gpu.value,
             ['3D GPU-MODEL-NAME TAKES ADVANTAGE', 'ANOTHER-MATCHING-VIDEO-CONTROLLER']
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_hostname.py` & `archey4-4.9.0/archey/test/entries/test_archey_hostname.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_kernel.py` & `archey4-4.9.0/archey/test/entries/test_archey_kernel.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_lan_ip.py` & `archey4-4.9.0/archey/test/entries/test_archey_lan_ip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Test module for Archey's LAN IP addresses detection module"""
 
 import unittest
 from unittest.mock import MagicMock, patch
 
 from netifaces import AF_INET, AF_INET6, AF_LINK
 
-from archey.entries.lan_ip import LanIp
+from archey.entries.lan_ip import LanIP
 from archey.test import CustomAssertions
 from archey.test.entries import HelperMethods
 from archey.constants import DEFAULT_CONFIG
 
 
-class TestLanIpEntry(unittest.TestCase, CustomAssertions):
+class TestLanIPEntry(unittest.TestCase, CustomAssertions):
     """Here, we mock the `netifaces` usages (interfaces and addresses detection calls)"""
     @patch(
         'archey.entries.lan_ip.netifaces.interfaces',
         return_value=['lo', 'en0', 'wlo1']
     )
     @patch(
         'archey.entries.lan_ip.netifaces.ifaddresses',
@@ -44,21 +44,20 @@
                 AF_INET: [{
                     'addr': '172.34.56.78',
                     'broadcast': '172.34.255.255'
                 }]
             }
         ]
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={'ip_settings': {'lan_ip_max_count': False}}
-    )
     def test_multiple_interfaces(self, _, __):
         """Test for multiple interfaces, multiple addresses (including a loopback one)"""
         self.assertListEqual(
-            LanIp().value,
+            LanIP(options={
+                'max_count': False
+            }).value,
             ['192.168.0.11', '192.168.1.11', '172.34.56.78']
         )
 
     @patch(
         'archey.entries.lan_ip.netifaces.interfaces',
         return_value=['lo', 'en0']
     )
@@ -88,54 +87,51 @@
                 AF_INET: [{
                     'addr': '192.168.1.55',
                     'netmask': '255.255.255.0',
                     'broadcast': '192.168.1.255'
                 }],
                 AF_INET6: [
                     {
-                        'addr': '2001::45:6789:abcd:6817',
+                        'addr': '2001:0000:0000:0000:0045:6789:abcd:6817',
                         'netmask': 'ffff:ffff:ffff:ffff::/64'
                     },
                     {
-                        'addr': '2a02::45:6789:abcd:0123/64',
+                        'addr': r'fe80::abcd:ef0:abef:dead%en0',
                         'netmask': 'ffff:ffff:ffff:ffff::/64'
                     },
                     {
-                        'addr': r'fe80::abcd:ef0:abef:dead\%en0',
+                        'addr': '2a02::45:6789:abcd:0123/64',
                         'netmask': 'ffff:ffff:ffff:ffff::/64'
                     }
                 ]
             }
         ]
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'lan_ip_max_count': 2,
-                'lan_ip_v6_support': True
-            }
-        }
-    )
     def test_ipv6_and_limit_and_ether(self, _, __):
         """
         Test for IPv6 support, final set length limit and Ethernet interface filtering.
         Additionally check the `output` method behavior.
+
+        IP address "compression" and interface name splitting will also be tested.
         """
-        lan_ip = LanIp()
+        lan_ip = LanIP(options={
+            'max_count': 3,
+            'ipv6_support': True
+        })
 
         output_mock = MagicMock()
         lan_ip.output(output_mock)
 
         self.assertListEqual(
             lan_ip.value,
-            ['192.168.1.55', '2001::45:6789:abcd:6817']
+            ['192.168.1.55', '2001::45:6789:abcd:6817', 'fe80::abcd:ef0:abef:dead']
         )
         self.assertEqual(
             output_mock.append.call_args[0][1],
-            '192.168.1.55, 2001::45:6789:abcd:6817'
+            '192.168.1.55, 2001::45:6789:abcd:6817, fe80::abcd:ef0:abef:dead'
         )
 
     @patch(
         'archey.entries.lan_ip.netifaces.interfaces',
         return_value=['lo', 'en0']
     )
     @patch(
@@ -164,39 +160,37 @@
                         'netmask': 'ffff:ffff:ffff:ffff::/64'
                     },
                     {
                         'addr': '2a02::45:6789:abcd:0123/64',
                         'netmask': 'ffff:ffff:ffff:ffff::/64'
                     },
                     {
-                        'addr': r'fe80::abcd:ef0:abef:dead\%en0',
+                        'addr': r'fe80::abcd:ef0:abef:dead%en0',
                         'netmask': 'ffff:ffff:ffff:ffff::/64'
                     }
                 ]
             }
         ]
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={'ip_settings': {'lan_ip_v6_support': False}}
-    )
     def test_no_ipv6(self, _, __):
         """Test for IPv6 hiding"""
         self.assertListEqual(
-            LanIp().value,
+            LanIP(options={
+                'ipv6_support': False
+            }).value,
             ['192.168.1.55']
         )
 
     @patch(
         'archey.entries.lan_ip.netifaces.interfaces',
         return_value=[]  # No interface returned by `netifaces`.
     )
-    @HelperMethods.patch_clean_configuration
     def test_no_network_interface(self, _):
         """Test when the device does not have any network interface"""
-        self.assertListEmpty(LanIp().value)
+        self.assertListEmpty(LanIP().value)
 
     @patch(
         'archey.entries.lan_ip.netifaces.interfaces',
         return_value=['lo', 'en0']
     )
     @patch(
         'archey.entries.lan_ip.netifaces.ifaddresses',
@@ -208,30 +202,90 @@
                 }],
                 AF_INET: [{
                     'addr': '127.0.0.1',
                     'netmask': '255.0.0.0',
                     'peer': '127.0.0.1'
                 }],
                 AF_INET6: [{
-                    'addr': '::1',
+                    'addr': '0000:0000:0000:0000:0000:0000:0000:0001',
                     'netmask': 'ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff/128'
                 }]
             },
             {
                 # No address for this one.
             }
         ]
     )
     @HelperMethods.patch_clean_configuration
     def test_no_network_address_output(self, _, __):
         """
         Test when the network interface(s) do not have any IP address.
         Additionally check the `output` method behavior.
         """
-        lan_ip = LanIp()
+        lan_ip = LanIP()
+
+        output_mock = MagicMock()
+        lan_ip.output(output_mock)
+
+        self.assertListEmpty(lan_ip.value)
+        self.assertEqual(
+            output_mock.append.call_args[0][1],
+            DEFAULT_CONFIG['default_strings']['no_address']
+        )
+
+    @patch(
+        'archey.entries.lan_ip.netifaces.interfaces',
+        return_value=['lo', 'en0']
+    )
+    @patch(
+        'archey.entries.lan_ip.netifaces.ifaddresses',
+        side_effect=[
+            {
+                AF_INET: [{
+                    'addr': '127.0.0.1',
+                    'netmask': '255.0.0.0',
+                    'peer': '127.0.0.1'
+                }],
+                AF_INET6: [{
+                    'addr': '::1',
+                    'netmask': 'ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff/128'
+                }]
+            },
+            {
+                AF_INET: [{
+                    'addr': '192.168.1.55',
+                    'netmask': '255.255.255.0',
+                    'broadcast': '192.168.1.255'
+                }],
+                AF_INET6: [
+                    {
+                        'addr': '2001::45:6789:abcd:6817',
+                        'netmask': 'ffff:ffff:ffff:ffff::/64'
+                    },
+                    {
+                        'addr': '2a02::45:6789:abcd:0123/64',
+                        'netmask': 'ffff:ffff:ffff:ffff::/64'
+                    },
+                    {
+                        'addr': r'fe80::abcd:ef0:abef:dead%en0',
+                        'netmask': 'ffff:ffff:ffff:ffff::/64'
+                    }
+                ]
+            }
+        ]
+    )
+    @HelperMethods.patch_clean_configuration
+    def test_user_disabled(self, _, __):
+        """Check behavior on user inputs edge-cases"""
+        lan_ip = LanIP(
+            options={
+                'ipv6_support': True,
+                'max_count': 0
+            }
+        )
 
         output_mock = MagicMock()
         lan_ip.output(output_mock)
 
         self.assertListEmpty(lan_ip.value)
         self.assertEqual(
             output_mock.append.call_args[0][1],
@@ -246,15 +300,15 @@
         'archey.entries.lan_ip.print',
         return_value=None,  # Let's nastily mute class' outputs.
         create=True
     )
     @HelperMethods.patch_clean_configuration
     def test_netifaces_not_available(self, _):
         """Check `netifaces` is really acting as a (soft-)dependency"""
-        lan_ip = LanIp()
+        lan_ip = LanIP()
 
         output_mock = MagicMock()
         lan_ip.output(output_mock)
 
         self.assertIsNone(lan_ip.value)
         self.assertEqual(
             output_mock.append.call_args[0][1],
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_model.py` & `archey4-4.9.0/archey/test/entries/test_archey_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,28 +159,36 @@
             mock.return_value.read.side_effect = [
                 FileNotFoundError(),
                 FileNotFoundError()
             ]
 
             self.assertIsNone(Model._fetch_product_info())  # pylint: disable=protected-access
 
-    def test_fetch_rasperry_pi_revision(self):
-        """Test `_fetch_rasperry_pi_revision` static method"""
+        # Product information are really weird...
+        with patch('archey.entries.model.open', mock_open(), create=True) as mock:
+            mock.return_value.read.side_effect = [
+                'To Be Filled By O.E.M.\n'  # Only `product_name` will be read.
+            ]
+
+            self.assertIsNone(Model._fetch_product_info())  # pylint: disable=protected-access
+
+    def test_fetch_raspberry_pi_revision(self):
+        """Test `_fetch_raspberry_pi_revision` static method"""
         with patch('archey.entries.model.open', mock_open(), create=True) as mock:
             mock.return_value.read.side_effect = [
                 'Hardware\t: HARDWARE\nRevision\t: REVISION\n',
                 'processor   : 0\ncpu family  : X\n'
             ]
 
             self.assertEqual(
-                Model._fetch_rasperry_pi_revision(),  # pylint: disable=protected-access
+                Model._fetch_raspberry_pi_revision(),  # pylint: disable=protected-access
                 'Raspberry Pi HARDWARE (Rev. REVISION)'
             )
             self.assertIsNone(
-                Model._fetch_rasperry_pi_revision()  # pylint: disable=protected-access
+                Model._fetch_raspberry_pi_revision()  # pylint: disable=protected-access
             )
 
     @patch(
         'archey.entries.model.check_output',
         side_effect=[
             'PHONE-BRAND\n',     # First `getprop` call.
             'PHONE-DEVICE\n',    # Second `getprop` call.
@@ -202,15 +210,15 @@
         return_value=None  # Not a virtual environment...
     )
     @patch(
         'archey.entries.model.Model._fetch_product_info',
         return_value=None  # No model name could be retrieved...
     )
     @patch(
-        'archey.entries.model.Model._fetch_rasperry_pi_revision',
+        'archey.entries.model.Model._fetch_raspberry_pi_revision',
         return_value=None  # Not a Raspberry Pi device either...
     )
     @patch(
         'archey.entries.model.Model._fetch_android_device_model',
         return_value=None  # Not an Android device...
     )
     @HelperMethods.patch_clean_configuration
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_packages.py` & `archey4-4.9.0/archey/test/entries/test_archey_packages.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_ram.py` & `archey4-4.9.0/archey/test/entries/test_archey_ram.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,21 @@
     @patch(
         'archey.entries.ram.check_output',
         return_value="""\
               total        used        free      shared  buff/cache   available
 Mem:          15658        2043       10232          12        3382       13268
 Swap:          4095          39        4056
 """)
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'limits': {
-                'ram': {
-                    'warning': 25,
-                    'danger': 45
-                }
-            }
-        }
-    )
     def test_free_dash_m(self, _):
         """Test `free -m` output parsing for low RAM use case"""
         output_mock = MagicMock()
-        RAM().output(output_mock)
+        RAM(options={
+            'warning': 25,
+            'danger': 45
+        }).output(output_mock)
         self.assertEqual(
             output_mock.append.call_args[0][1],
             '{0}2043 MiB{1} / 15658 MiB'.format(
                 Colors.GREEN_NORMAL,
                 Colors.CLEAR
             )
         )
@@ -46,28 +39,21 @@
     @patch(
         'archey.entries.ram.check_output',
         return_value="""\
           total     used    free    shared  buff/cache   available
 Mem:       7412     3341    1503       761        2567        3011
 Swap:      7607        5    7602
 """)
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'limits': {
-                'ram': {
-                    'warning': 33.3,
-                    'danger': 66.7
-                }
-            }
-        }
-    )
     def test_free_dash_m_warning(self, _):
         """Test `free -m` output parsing for warning RAM use case"""
         output_mock = MagicMock()
-        RAM().output(output_mock)
+        RAM(options={
+            'warning': 33.3,
+            'danger': 66.7
+        }).output(output_mock)
         self.assertEqual(
             output_mock.append.call_args[0][1],
             '{0}3341 MiB{1} / 7412 MiB'.format(
                 Colors.YELLOW_NORMAL,
                 Colors.CLEAR
             )
         )
@@ -75,28 +61,21 @@
     @patch(
         'archey.entries.ram.check_output',
         return_value="""\
               total        used        free      shared  buff/cache   available
 Mem:          15658       12341         624         203        2692        2807
 Swap:          4095         160        3935
 """)
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'limits': {
-                'ram': {
-                    'warning': 33.3,
-                    'danger': 66.7
-                }
-            }
-        }
-    )
     def test_free_dash_m_danger(self, _):
         """Test `free -m` output parsing for danger RAM use case"""
         output_mock = MagicMock()
-        RAM().output(output_mock)
+        RAM(options={
+            'warning': 25,
+            'danger': 45
+        }).output(output_mock)
         self.assertEqual(
             output_mock.append.call_args[0][1],
             '{0}12341 MiB{1} / 15658 MiB'.format(
                 Colors.RED_NORMAL,
                 Colors.CLEAR
             )
         )
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_shell.py` & `archey4-4.9.0/archey/test/entries/test_archey_shell.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_temperature.py` & `archey4-4.9.0/archey/test/entries/test_archey_temperature.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from subprocess import CalledProcessError
 
 import unittest
 from unittest.mock import MagicMock, patch
 
 
 from archey.entries.temperature import Temperature
-from archey.test.entries import HelperMethods
 
 
 class TestTemperatureEntry(unittest.TestCase):
     """
     Based on `sensors`, `vcgencmd` and thermal files, this module verifies temperature computations.
     """
 
@@ -45,29 +44,24 @@
             'temp=42.8\'C\n'
         ]
     )
     @patch(
         'archey.entries.temperature.iglob',
         return_value=[]  # No temperature from file will be retrieved
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'temperature': {
-                'sensors_chipsets': [],
-                'use_fahrenheit': False,
-                'char_before_unit': ' '
-            }
-        }
-    )
     def test_vcgencmd_only_no_max(self, _, __):
         """
         Test for `vcgencmd` output only (no sensor files).
         Only one value is retrieved, so no maximum should be displayed (see #39).
         """
-        temperature = Temperature()
+        temperature = Temperature(options={
+            'sensors_chipsets': [],
+            'use_fahrenheit': False,
+            'char_before_unit': ' '
+        })
 
         output_mock = MagicMock()
         temperature.output(output_mock)
 
         self.assertDictEqual(
             temperature.value,
             {
@@ -86,28 +80,23 @@
         'archey.entries.temperature.check_output',
         side_effect=[
             FileNotFoundError(),
             'temp=40.0\'C\n'
         ]
     )
     @patch('archey.entries.temperature.iglob')
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'temperature': {
-                'sensors_chipsets': [],
-                'use_fahrenheit': False,
-                'char_before_unit': ' '
-            }
-        }
-    )
     def test_vcgencmd_and_files(self, iglob_mock, _):
         """Tests `vcgencmd` output AND sensor files"""
         iglob_mock.return_value = iter([file.name for file in self._temp_files])
         self.assertDictEqual(
-            Temperature().value,
+            Temperature(options={
+                'sensors_chipsets': [],
+                'use_fahrenheit': False,
+                'char_before_unit': ' '
+            }).value,
             {
                 'temperature': 45.0,
                 'max_temperature': 50.0,
                 'char_before_unit': ' ',
                 'unit': 'C'
             }
         )
@@ -116,28 +105,23 @@
         'archey.entries.temperature.check_output',
         side_effect=[
             FileNotFoundError(),  # No temperature from `sensors` call
             FileNotFoundError()   # No temperature from `vcgencmd` call
         ]
     )
     @patch('archey.entries.temperature.iglob')
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'temperature': {
-                'sensors_chipsets': [],
-                'use_fahrenheit': True,
-                'char_before_unit': '@'
-            }
-        }
-    )
     def test_files_only_in_fahrenheit(self, iglob_mock, _):
         """Test sensor files only, Fahrenheit (naive) conversion and special degree character"""
         iglob_mock.return_value = iter([file.name for file in self._temp_files])
         self.assertDictEqual(
-            Temperature().value,
+            Temperature(options={
+                'sensors_chipsets': [],
+                'use_fahrenheit': True,
+                'char_before_unit': '@'
+            }).value,
             {
                 'temperature': 116.0,      # 46.7 degrees C in Fahrenheit.
                 'max_temperature': 122.0,  # 50 degrees C in Fahrenheit
                 'char_before_unit': '@',
                 'unit': 'F'
             }
         )
@@ -149,20 +133,19 @@
             FileNotFoundError()   # No temperature from `vcgencmd` call.
         ]
     )
     @patch(
         'archey.entries.temperature.iglob',
         return_value=[]  # No temperature from file will be retrieved.
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={'temperature': {'sensors_chipsets': []}}
-    )
     def test_no_output(self, _, __):
         """Test when no value could be retrieved (anyhow)"""
-        self.assertIsNone(Temperature().value)
+        self.assertIsNone(Temperature(options={
+            'sensors_chipsets': []
+        }).value)
 
     @patch(
         'archey.entries.temperature.check_output',  # Mock the `sensors` call.
         side_effect=[
             """\
 {
    "who-cares-about":{
@@ -217,27 +200,22 @@
       }
    }
 }
 """,
             FileNotFoundError()  # No temperature from `vcgencmd` call.
         ]
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'temperature': {
-                'sensors_chipsets': [],
-                'use_fahrenheit': True,
-                'char_before_unit': ' '
-            }
-        }
-    )
     def test_sensors_only_in_fahrenheit(self, _):
         """Test computations around `sensors` output and Fahrenheit (naive) conversion"""
         self.assertDictEqual(
-            Temperature().value,
+            Temperature(options={
+                'sensors_chipsets': [],
+                'use_fahrenheit': True,
+                'char_before_unit': ' '
+            }).value,
             {
                 'temperature': 126.6,      # (52.6 C in F)
                 'max_temperature': 237.2,  # (114.0 C in F)
                 'char_before_unit': ' ',
                 'unit': 'F'
             }
         )
@@ -246,28 +224,23 @@
         'archey.entries.temperature.check_output',
         side_effect=[
             CalledProcessError(1, 'sensors'),  # `sensors` will hard fail.
             FileNotFoundError()                # No temperature from `vcgencmd` call
         ]
     )
     @patch('archey.entries.temperature.iglob')
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'temperature': {
-                'sensors_chipsets': [],
-                'use_fahrenheit': False,
-                'char_before_unit': 'o'
-            }
-        }
-    )
     def test_sensors_error_1(self, iglob_mock, _):
         """Test `sensors` (hard) failure handling and polling from files in Celsius"""
         iglob_mock.return_value = iter([file.name for file in self._temp_files])
 
-        temperature = Temperature()
+        temperature = Temperature(options={
+            'sensors_chipsets': [],
+            'use_fahrenheit': False,
+            'char_before_unit': 'o'
+        })
 
         output_mock = MagicMock()
         temperature.output(output_mock)
 
         self.assertDictEqual(
             temperature.value,
             {
@@ -292,28 +265,23 @@
     ]
 }
 """,
             FileNotFoundError()  # No temperature from `vcgencmd` call
         ]
     )
     @patch('archey.entries.temperature.iglob')
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'temperature': {
-                'sensors_chipsets': [],
-                'use_fahrenheit': False,
-                'char_before_unit': 'o'
-            }
-        }
-    )
     def test_sensors_error_2(self, iglob_mock, _):
         """Test `sensors` (hard) failure handling and polling from files in Celsius"""
         iglob_mock.return_value = iter([file.name for file in self._temp_files])
         self.assertDictEqual(
-            Temperature().value,
+            Temperature(options={
+                'sensors_chipsets': [],
+                'use_fahrenheit': False,
+                'char_before_unit': 'o'
+            }).value,
             {
                 'temperature': 46.7,
                 'max_temperature': 50.0,
                 'char_before_unit': 'o',
                 'unit': 'C'
             }
         )
@@ -325,15 +293,14 @@
             FileNotFoundError()   # No temperature from `vcgencmd` call.
         ]
     )
     @patch(
         'archey.entries.temperature.iglob',
         return_value=[]  # No temperature from file will be retrieved.
     )
-    @HelperMethods.patch_clean_configuration
     def test_celsius_to_fahrenheit_conversion(self, _, __):
         """Simple tests for the `_convert_to_fahrenheit` static method"""
         test_conversion_cases = [
             (-273.15, -459.67),
             (0.0, 32.0),
             (21.0, 69.8),
             (37.0, 98.6),
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_terminal.py` & `archey4-4.9.0/archey/test/entries/test_archey_terminal.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,60 +22,50 @@
         {
             'TERM': 'xterm-256color',
             'COLORTERM': 'truecolor',
             'TERM_PROGRAM': 'A-COOL-TERMINAL-EMULATOR'
         },
         clear=True
     )
-    @HelperMethods.patch_clean_configuration
     def test_terminal_emulator_term_program(self):
         """Check that `TERM_PROGRAM` is honored even if `TERM` or `COLORTERM` is defined"""
         self.assertEqual(Terminal().value, 'A-COOL-TERMINAL-EMULATOR')
 
     @patch.dict(
         'archey.entries.terminal.os.environ',
         {
             'TERM': 'OH-A-SPECIAL-CASE',
             'TERMINATOR_UUID': 'urn:uuid:xxxxxxxx-yyyy-zzzz-tttt-uuuuuuuuuuuu'  # Ignored.
         },
         clear=True
     )
-    @HelperMethods.patch_clean_configuration
     def test_terminal_emulator_special_term(self):
         """Check that `TERM` is honored even if a "known identifier" could be found"""
         self.assertEqual(Terminal().value, 'OH-A-SPECIAL-CASE')
 
     @patch.dict(
         'archey.entries.terminal.os.environ',
         {
             'TERM': 'xterm-256color',
             'KONSOLE_VERSION': 'X.Y.Z'
         },
         clear=True
     )
-    @HelperMethods.patch_clean_configuration
     def test_terminal_emulator_name_normalization(self):
         """Check that our manual terminal detection as long as name normalization are working"""
         self.assertEqual(Terminal().value, 'Konsole')
 
     @patch.dict(
         'archey.entries.terminal.os.environ',
         {'TERM': 'xterm-256color'},
         clear=True
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'colors_palette': {
-                'use_unicode': True
-            }
-        }
-    )
     def test_terminal_emulator_term_fallback_and_unicode(self):
         """Check that `TERM` is honored if present, and Unicode support for the colors palette"""
-        terminal = Terminal()
+        terminal = Terminal(options={'use_unicode': True})
 
         output_mock = MagicMock()
         terminal.output(output_mock)
 
         self.assertEqual(terminal.value, 'xterm-256color')
         self.assertTrue(
             output_mock.append.call_args[0][1].startswith('xterm-256color')
@@ -86,29 +76,27 @@
         )
 
     @patch.dict(
         'archey.entries.terminal.os.environ',
         {'COLORTERM': 'kmscon'},
         clear=True
     )
-    @HelperMethods.patch_clean_configuration
     def test_terminal_emulator_colorterm(self):
         """Check we can detect terminals using the `COLORTERM` environment variable."""
         self.assertEqual(Terminal().value, 'KMSCON')
 
     @patch.dict(
         'archey.entries.terminal.os.environ',
         {
             'TERM': 'xterm-256color',
             'KONSOLE_VERSION': '200401',
             'COLORTERM': 'kmscon'
         },
         clear=True
     )
-    @HelperMethods.patch_clean_configuration
     def test_terminal_emulator_colorterm_override(self):
         """
         Check we observe terminal using `COLORTERM` even if `TERM` or a "known identifier" is found.
         """
         self.assertEqual(Terminal().value, 'KMSCON')
 
     @patch.dict(
@@ -134,29 +122,25 @@
             )
 
     @patch.dict(
         'archey.entries.terminal.os.environ',
         {},
         clear=True
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'colors_palette': {
-                'use_unicode': False
-            }
-        }
-    )
+    @HelperMethods.patch_clean_configuration
     def test_not_detected(self):
         """Test terminal emulator (non-)detection, without Unicode support"""
-        terminal = Terminal()
+        terminal = Terminal(options={'use_unicode': False})
 
         output_mock = MagicMock()
         terminal.output(output_mock)
         output = output_mock.append.call_args[0][1]
 
         self.assertIsNone(terminal.value)
-        self.assertTrue(output.startswith(DEFAULT_CONFIG['default_strings']['not_detected']))
+        self.assertTrue(
+            output.startswith(DEFAULT_CONFIG['default_strings']['not_detected'])
+        )
         self.assertFalse(output.count('\u2588'))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_uptime.py` & `archey4-4.9.0/archey/test/entries/test_archey_uptime.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             '{time} up 500 days, 0 min, {user_loadavg}': timedelta(days=500),  # Linux
             '{time} up 500 days, 1 min, {user_loadavg}': timedelta(days=500, minutes=1),
             '{time} up 500 days, 12 mins, {user_loadavg}': timedelta(days=500, minutes=12),
             '{time} up 500 day, 12 min, {user_loadavg}': timedelta(days=500, minutes=12),  # Variation without plural minutes
             '{time} up 500 days, 1:00, {user_loadavg}': timedelta(days=500, hours=1),
             '{time} up 500 days, 1:01, {user_loadavg}': timedelta(days=500, hours=1, minutes=1),
             '{time} up 500 days, 1:23, {user_loadavg}': timedelta(days=500, hours=1, minutes=23),
-            '{time} up 500 days, 12:34, {user_loadavg}': timedelta(days=500, hours=12, minutes=34),
+            '{time} up 500 days, 12:34, {user_loadavg}': timedelta(days=500, hours=12, minutes=34)
         }
         # pylint: enable=line-too-long
 
         # Variations of the time in the `{time}` section.
         # These _should_ be avoided when we set the locale in `check_output`,
         # however let's check we can handle them anyway, just in case.
         time_variations = (
@@ -218,15 +218,15 @@
 
         # Variations of the user count and load average section.
         # For this, we'll just combine user variations with a few load average variations.
         user_variations = (
             '1 user ', '1 user  ', ' 1 user, ', ' 1 user,  ',
             '2 users ', '2 users  ', '  2 users, ', '  2 users,  ',
             '15 users ', '15 users  ', ' 15 users, ', ' 15 users,  ',
-            '150 users ', '150 users  ', '150 users, ', '150 users,  ',
+            '150 users ', '150 users  ', '150 users, ', '150 users,  '
         )
         loadavg_variations = (
             'load averages: 1.95 1.28 2.10',
             'load average: 0.13, 0.17, 0.13',
             'we never match this part so the content here',
             '  should not affect our parsing'
         )
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_user.py` & `archey4-4.9.0/archey/test/entries/test_archey_user.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_wan_ip.py` & `archey4-4.9.0/archey/test/entries/test_archey_wan_ip.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,165 +1,132 @@
 """Test module for Archey's public IP address detection module"""
 
 import unittest
 from unittest.mock import MagicMock, patch
 
 from socket import timeout as SocketTimeoutError
 from subprocess import TimeoutExpired
-from urllib.error import URLError
 
 from archey.test import CustomAssertions
-from archey.entries.wan_ip import WanIp
+from archey.entries.wan_ip import WanIP
 from archey.test.entries import HelperMethods
 from archey.constants import DEFAULT_CONFIG
 
-class TestWanIpEntry(unittest.TestCase, CustomAssertions):
+
+class TestWanIPEntry(unittest.TestCase, CustomAssertions):
     """
-    Here, we mock calls to `dig` or `urlopen`.
+    Here, we end up mocking calls to `dig` or `urlopen`.
     """
+    def setUp(self):
+        """We use these mocks so often, it's worth defining them here."""
+        self.wan_ip_mock = HelperMethods.entry_mock(WanIP)
+        self.output_mock = MagicMock()
+
     @patch(
         'archey.entries.wan_ip.check_output',
         side_effect=[
-            'XXX.YY.ZZ.TTT\n',
-            '0123::4567:89a:dead:beef\n'
+            TimeoutExpired('dig', 1),     # `check_output` call will hard-fail.
+            '0123::4567:89a:dead:beef\n'  # `check_output` will work.
         ]
     )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'wan_ip_v6_support': True
-            }
-        }
-    )
-    def test_ipv6_and_ipv4(self, _):
-        """Test the regular case : Both IPv4 and IPv6 are retrieved"""
-        self.assertEqual(
-            WanIp().value,
-            ['XXX.YY.ZZ.TTT', '0123::4567:89a:dead:beef']
+    @patch('archey.entries.wan_ip.urlopen')
+    def test_ipv4_ko_and_ipv6_ok(self, urlopen_mock, _):
+        """Test fallback on HTTP method only when DNS lookup failed"""
+        # `urlopen` will hard-fail.
+        urlopen_mock.return_value.read.side_effect = SocketTimeoutError(0)
+
+        # IPv4 retrieval failed.
+        self.assertFalse(
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 4),  # pylint: disable=protected-access
         )
 
-    @patch(
-        'archey.entries.wan_ip.check_output',
-        return_value='XXX.YY.ZZ.TTT'
-    )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'wan_ip_v6_support': False
-            }
-        }
-    )
-    def test_ipv4_only(self, _):
-        """Test only public IPv4 detection"""
+        # IPv6 worked like a (almost !) charm.
         self.assertEqual(
-            WanIp().value,
-            ['XXX.YY.ZZ.TTT']
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 6),  # pylint: disable=protected-access
+            '0123::4567:89a:dead:beef'
         )
 
     @patch(
         'archey.entries.wan_ip.check_output',
         side_effect=[
-            'XXX.YY.ZZ.TTT',            # The IPv4 address is detected
-            TimeoutExpired('dig', 1)  # `check_output` call will fail
+            '\n',                     # `check_output` call will soft-fail.
+            FileNotFoundError('dig')  # `check_output` call will hard-fail.
         ]
     )
     @patch('archey.entries.wan_ip.urlopen')
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'wan_ip_v6_support': True
-            }
-        }
-    )
-    def test_ipv6_timeout(self, urlopen_mock, _):
-        """
-        Test when `dig` call timeout for the IPv6 detection.
-        Additionally check the `output` method behavior.
-        """
-        urlopen_mock.return_value.read.return_value = b'0123::4567:89a:dead:beef\n'
+    def test_proper_http_fallback(self, urlopen_mock, _):
+        """Test fallback on HTTP method only when DNS lookup failed"""
+        urlopen_mock.return_value.read.return_value = b'XXX.YY.ZZ.TTT\n'
+
+        # HTTP back-end was not called, we trust DNS lookup tool which failed.
+        self.assertFalse(
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 4),  # pylint: disable=protected-access
+        )
 
-        wan_ip = WanIp()
+        # New try: HTTP method has been called !
+        self.assertEqual(
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 4),  # pylint: disable=protected-access
+            'XXX.YY.ZZ.TTT'
+        )
 
-        output_mock = MagicMock()
-        wan_ip.output(output_mock)
+    def test_retrieval_disabled(self):
+        """Test behavior when both IPv4 and IPv6 retrievals are purposely disabled"""
+        self.wan_ip_mock.options = {
+            'ipv4': False,
+            'ipv6': False
+        }
 
-        self.assertListEqual(
-            wan_ip.value,
-            ['XXX.YY.ZZ.TTT', '0123::4567:89a:dead:beef']
+        # Both retrievals fail.
+        self.assertFalse(
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 4)  # pylint: disable=protected-access
         )
-        self.assertEqual(
-            output_mock.append.call_args[0][1],
-            'XXX.YY.ZZ.TTT, 0123::4567:89a:dead:beef'
+        self.assertFalse(
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 6)  # pylint: disable=protected-access
         )
 
-    @patch(
-        'archey.entries.wan_ip.check_output',
-        side_effect=TimeoutExpired('dig', 1)  # `check_output` call will fail
-    )
-    @patch(
-        'archey.entries.wan_ip.urlopen',
-        side_effect=URLError('<urlopen error timed out>')  # `urlopen` call will fail
-    )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'wan_ip_v6_support': False
+    def test_method_disabled(self):
+        """Check whether user could disable resolver back-ends from configuration"""
+        self.wan_ip_mock.options = {
+            'ipv4': {
+                'dns_query': False,
+                'http_url': False
             }
         }
-    )
-    def test_ipv4_timeout_twice(self, _, __):
-        """Test when both `dig` and `URLOpen` trigger timeouts..."""
-        self.assertListEmpty(WanIp().value)
 
-    @patch(
-        'archey.entries.wan_ip.check_output',
-        side_effect=TimeoutExpired('dig', 1)  # `check_output` call will fail
-    )
-    @patch(
-        'archey.entries.wan_ip.urlopen',
-        side_effect=SocketTimeoutError(1)  # `urlopen` call will fail
-    )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'wan_ip_v6_support': False
-            }
-        }
-    )
-    def test_ipv4_timeout_twice_socket_error(self, _, __):
-        """Test when both `dig` timeouts and `URLOpen` raises `socket.timeout`..."""
-        self.assertListEmpty(WanIp().value)
+        # Internal method doesn't return any address.
+        self.assertFalse(
+            WanIP._retrieve_ip_address(self.wan_ip_mock, 4)  # pylint: disable=protected-access
+        )
 
-    @patch(
-        'archey.entries.wan_ip.check_output',
-        return_value=''  # No address will be returned
-    )
-    @patch(
-        'urllib.request.urlopen',
-        return_value=None  # No object will be returned
-    )
-    @HelperMethods.patch_clean_configuration(
-        configuration={
-            'ip_settings': {
-                'wan_ip_v6_support': False
-            }
-        }
-    )
-    def test_no_address(self, _, __):
+    def test_two_addresses(self):
+        """
+        Test when both IPv4 and IPv6 addresses could be retrieved.
+        Additionally check the `output` method behavior.
+        """
+        self.wan_ip_mock.value = ['XXX.YY.ZZ.TTT', '0123::4567:89a:dead:beef']
+
+        WanIP.output(self.wan_ip_mock, self.output_mock)
+
+        self.assertEqual(
+            self.output_mock.append.call_args[0][1],
+            "XXX.YY.ZZ.TTT, 0123::4567:89a:dead:beef"
+        )
+
+    @HelperMethods.patch_clean_configuration
+    def test_no_address(self):
         """
         Test when no address could be retrieved.
         Additionally check the `output` method behavior.
         """
-        wan_ip = WanIp()
+        self.wan_ip_mock.value = []
 
-        output_mock = MagicMock()
-        wan_ip.output(output_mock)
+        WanIP.output(self.wan_ip_mock, self.output_mock)
 
-        self.assertListEmpty(wan_ip.value)
+        self.assertListEmpty(self.wan_ip_mock.value)
         self.assertEqual(
-            output_mock.append.call_args[0][1],
+            self.output_mock.append.call_args[0][1],
             DEFAULT_CONFIG['default_strings']['no_address']
         )
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `archey4-4.8.1/archey/test/entries/test_archey_window_manager.py` & `archey4-4.9.0/archey/test/entries/test_archey_window_manager.py`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/archey4.egg-info/PKG-INFO` & `archey4-4.9.0/archey4.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archey4
-Version: 4.8.1
+Version: 4.9.0
 Summary: Archey is a simple system information tool written in Python
 Home-page: https://github.com/HorlogeSkynet/archey4
 Author: Samuel Forestier
 Author-email: dev+archey@samuel.domains
 License: GPLv3
 Description: Archey4 is a **maintained** fork of the original Archey Linux system tool.
         The original Archey program had been written by Melik Manukyan in 2009, and quickly abandoned in 2011.
```

### Comparing `archey4-4.8.1/archey4.egg-info/SOURCES.txt` & `archey4-4.9.0/archey4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archey4-4.8.1/setup.py` & `archey4-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     version=__version__.lstrip('v'),
     description='Archey is a simple system information tool written in Python',
     keywords='archey python3 linux system-information monitoring screenshot',
     url='https://github.com/HorlogeSkynet/archey4',
     author='Samuel Forestier',  # Not alone
     author_email='dev+archey@samuel.domains',
     license='GPLv3',
-    packages=find_packages(exclude=['archey.test']),
+    packages=find_packages(exclude=['archey.test*']),
     test_suite='archey.test',
     python_requires='>=3.4',
     install_requires=[
         'distro',
         'netifaces'
     ],
     entry_points={
```

