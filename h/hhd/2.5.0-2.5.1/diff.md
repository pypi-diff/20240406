# Comparing `tmp/hhd-2.5.0.tar.gz` & `tmp/hhd-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhd-2.5.0.tar", last modified: Fri Apr  5 20:38:42 2024, max compression
+gzip compressed data, was "hhd-2.5.1.tar", last modified: Sat Apr  6 13:04:16 2024, max compression
```

## Comparing `hhd-2.5.0.tar` & `hhd-2.5.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.873491 hhd-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 20:38:34.000000 hhd-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 20:38:34.000000 hhd-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-05 20:38:42.869491 hhd-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-05 20:38:34.000000 hhd-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-04-05 20:38:34.000000 hhd-2.5.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:38:42.873491 hhd-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.857491 hhd-2.5.0/src/hhd/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.857491 hhd-2.5.0/src/hhd/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/contrib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.857491 hhd-2.5.0/src/hhd/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/hide.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/lib/uhid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/physical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/evdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/hidraw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/imu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/physical/rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/dualsense/
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/dualsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/dualsense/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/sd/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/sd/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/controller/virtual/uinput/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/uinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/controller/virtual/uinput/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/src/hhd/device/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/device/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/generic/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/src/hhd/device/gpd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.861491 hhd-2.5.0/src/hhd/device/gpd/win/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/gpd/win/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/device/legion_go/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/gyro_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/legion_go/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/device/orange_pi/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/orange_pi/controllers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/device/rog_ally/
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/controllers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/device/rog_ally/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/http/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.865491 hhd-2.5.0/src/hhd/http/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/static/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/http/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/display/
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/display/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/gyro.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/outputs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/overlay/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd/plugins/powerbutton/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/powerbutton/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/touchpad.yml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/sections.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 20:38:34.000000 hhd-2.5.0/src/hhd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/src/hhd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 20:38:42.000000 hhd-2.5.0/src/hhd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/modules-load.d/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/modules-load.d/hhd-user.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/systemd/system/hhd@.service
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/systemd/system/hhd_local@.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/systemd/user/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/systemd/user/hhd-user.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.853491 hhd-2.5.0/usr/lib/udev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/udev/hwdb.d/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/udev/hwdb.d/83-hhd.hwdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:38:42.869491 hhd-2.5.0/usr/lib/udev/rules.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/udev/rules.d/83-hhd-user.rules
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-05 20:38:34.000000 hhd-2.5.0/usr/lib/udev/rules.d/83-hhd.rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.369184 hhd-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 13:04:10.000000 hhd-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 13:04:10.000000 hhd-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-06 13:04:16.369184 hhd-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 13:04:10.000000 hhd-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-04-06 13:04:10.000000 hhd-2.5.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:04:16.369184 hhd-2.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.345184 hhd-2.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.353184 hhd-2.5.1/src/hhd/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.353184 hhd-2.5.1/src/hhd/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/contrib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/contrib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/contrib/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/contrib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/contrib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.353184 hhd-2.5.1/src/hhd/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37040 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/controller/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/lib/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/lib/hide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/lib/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/lib/uhid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/controller/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21658 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/physical/evdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/physical/hidraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/physical/imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/physical/rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/controller/virtual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/controller/virtual/dualsense/
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/dualsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29110 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/dualsense/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/controller/virtual/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/sd/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/controller/virtual/uinput/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/uinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/controller/virtual/uinput/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.349184 hhd-2.5.1/src/hhd/device/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.357184 hhd-2.5.1/src/hhd/device/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/generic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/generic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/generic/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.349184 hhd-2.5.1/src/hhd/device/gpd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.361184 hhd-2.5.1/src/hhd/device/gpd/win/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/gpd/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/gpd/win/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/gpd/win/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/gpd/win/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.361184 hhd-2.5.1/src/hhd/device/legion_go/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/legion_go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17892 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/legion_go/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/legion_go/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/legion_go/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/legion_go/gyro_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/legion_go/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.361184 hhd-2.5.1/src/hhd/device/orange_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/orange_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/orange_pi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/orange_pi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/orange_pi/controllers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.361184 hhd-2.5.1/src/hhd/device/rog_ally/
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/rog_ally/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/rog_ally/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/rog_ally/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/rog_ally/controllers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/device/rog_ally/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.361184 hhd-2.5.1/src/hhd/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/http/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/http/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.361184 hhd-2.5.1/src/hhd/http/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/http/static/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/http/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/src/hhd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/src/hhd/plugins/display/
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/display/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/gyro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/outputs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/src/hhd/plugins/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/overlay/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/overlay/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/overlay/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/overlay/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/src/hhd/plugins/powerbutton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/powerbutton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/powerbutton/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/powerbutton/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/powerbutton/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/touchpad.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/sections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 13:04:10.000000 hhd-2.5.1/src/hhd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/src/hhd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22425 2024-04-06 13:04:16.000000 hhd-2.5.1/src/hhd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-06 13:04:16.000000 hhd-2.5.1/src/hhd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:04:16.000000 hhd-2.5.1/src/hhd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-06 13:04:16.000000 hhd-2.5.1/src/hhd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 13:04:16.000000 hhd-2.5.1/src/hhd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-06 13:04:16.000000 hhd-2.5.1/src/hhd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.349184 hhd-2.5.1/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.349184 hhd-2.5.1/usr/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/usr/lib/modules-load.d/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/modules-load.d/hhd-user.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.349184 hhd-2.5.1/usr/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/usr/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/systemd/system/hhd@.service
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/systemd/system/hhd_local@.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/usr/lib/systemd/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/systemd/user/hhd-user.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.349184 hhd-2.5.1/usr/lib/udev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/usr/lib/udev/hwdb.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/udev/hwdb.d/83-hhd.hwdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:04:16.365184 hhd-2.5.1/usr/lib/udev/rules.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/udev/rules.d/83-hhd-user.rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-06 13:04:10.000000 hhd-2.5.1/usr/lib/udev/rules.d/83-hhd.rules
```

### Comparing `hhd-2.5.0/LICENSE` & `hhd-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/PKG-INFO` & `hhd-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.5.0
+Version: 2.5.1
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `hhd-2.5.0/pyproject.toml` & `hhd-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhd"
-version = "2.5.0"
+version = "2.5.1"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Handheld Daemon, a tool for configuring handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `hhd-2.5.0/readme.md` & `hhd-2.5.1/readme.md`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/__main__.py` & `hhd-2.5.1/src/hhd/__main__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/contrib/dev.py` & `hhd-2.5.1/src/hhd/contrib/dev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/contrib/gs.py` & `hhd-2.5.1/src/hhd/contrib/gs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/contrib/i18n.py` & `hhd-2.5.1/src/hhd/contrib/i18n.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/contrib/main.py` & `hhd-2.5.1/src/hhd/contrib/main.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/__init__.py` & `hhd-2.5.1/src/hhd/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/base.py` & `hhd-2.5.1/src/hhd/controller/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/const.py` & `hhd-2.5.1/src/hhd/controller/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/lib/common.py` & `hhd-2.5.1/src/hhd/controller/lib/common.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/lib/hid.py` & `hhd-2.5.1/src/hhd/controller/lib/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/lib/hide.py` & `hhd-2.5.1/src/hhd/controller/lib/hide.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/lib/ioctl.py` & `hhd-2.5.1/src/hhd/controller/lib/ioctl.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/lib/uhid.py` & `hhd-2.5.1/src/hhd/controller/lib/uhid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/physical/evdev.py` & `hhd-2.5.1/src/hhd/controller/physical/evdev.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/physical/hidraw.py` & `hhd-2.5.1/src/hhd/controller/physical/hidraw.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/physical/imu.py` & `hhd-2.5.1/src/hhd/controller/physical/imu.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/physical/rgb.py` & `hhd-2.5.1/src/hhd/controller/physical/rgb.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/virtual/dualsense/__init__.py` & `hhd-2.5.1/src/hhd/controller/virtual/dualsense/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/virtual/dualsense/const.py` & `hhd-2.5.1/src/hhd/controller/virtual/dualsense/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/virtual/sd/__init__.py` & `hhd-2.5.1/src/hhd/controller/virtual/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/virtual/sd/const.py` & `hhd-2.5.1/src/hhd/controller/virtual/sd/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/virtual/uinput/__init__.py` & `hhd-2.5.1/src/hhd/controller/virtual/uinput/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/controller/virtual/uinput/const.py` & `hhd-2.5.1/src/hhd/controller/virtual/uinput/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/generic/__init__.py` & `hhd-2.5.1/src/hhd/device/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/generic/base.py` & `hhd-2.5.1/src/hhd/device/generic/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/generic/const.py` & `hhd-2.5.1/src/hhd/device/generic/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/generic/controllers.yml` & `hhd-2.5.1/src/hhd/device/generic/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/gpd/win/__init__.py` & `hhd-2.5.1/src/hhd/device/gpd/win/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/gpd/win/base.py` & `hhd-2.5.1/src/hhd/device/gpd/win/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/gpd/win/const.py` & `hhd-2.5.1/src/hhd/device/gpd/win/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/gpd/win/controllers.yml` & `hhd-2.5.1/src/hhd/device/gpd/win/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/legion_go/__init__.py` & `hhd-2.5.1/src/hhd/device/legion_go/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/legion_go/base.py` & `hhd-2.5.1/src/hhd/device/legion_go/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/legion_go/const.py` & `hhd-2.5.1/src/hhd/device/legion_go/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/legion_go/controllers.yml` & `hhd-2.5.1/src/hhd/device/legion_go/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/legion_go/gyro_fix.py` & `hhd-2.5.1/src/hhd/device/legion_go/gyro_fix.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/legion_go/hid.py` & `hhd-2.5.1/src/hhd/device/legion_go/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/orange_pi/__init__.py` & `hhd-2.5.1/src/hhd/device/orange_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/orange_pi/base.py` & `hhd-2.5.1/src/hhd/device/orange_pi/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/orange_pi/const.py` & `hhd-2.5.1/src/hhd/device/orange_pi/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/orange_pi/controllers.yml` & `hhd-2.5.1/src/hhd/device/orange_pi/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/rog_ally/__init__.py` & `hhd-2.5.1/src/hhd/device/rog_ally/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/rog_ally/base.py` & `hhd-2.5.1/src/hhd/device/rog_ally/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/rog_ally/const.py` & `hhd-2.5.1/src/hhd/device/rog_ally/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/rog_ally/controllers.yml` & `hhd-2.5.1/src/hhd/device/rog_ally/controllers.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/device/rog_ally/hid.py` & `hhd-2.5.1/src/hhd/device/rog_ally/hid.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/http/api.py` & `hhd-2.5.1/src/hhd/http/api.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/http/index.html` & `hhd-2.5.1/src/hhd/http/index.html`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/http/static/index.js` & `hhd-2.5.1/src/hhd/http/static/index.js`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/logging.py` & `hhd-2.5.1/src/hhd/logging.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/__init__.py` & `hhd-2.5.1/src/hhd/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/conf.py` & `hhd-2.5.1/src/hhd/plugins/conf.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/display/__init__.py` & `hhd-2.5.1/src/hhd/plugins/display/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/gyro.yml` & `hhd-2.5.1/src/hhd/plugins/gyro.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/inputs.py` & `hhd-2.5.1/src/hhd/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/outputs.py` & `hhd-2.5.1/src/hhd/plugins/outputs.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/outputs.yml` & `hhd-2.5.1/src/hhd/plugins/outputs.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/overlay/__init__.py` & `hhd-2.5.1/src/hhd/plugins/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/overlay/base.py` & `hhd-2.5.1/src/hhd/plugins/overlay/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/overlay/controllers.py` & `hhd-2.5.1/src/hhd/plugins/overlay/controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,24 +139,29 @@
                     if code not in (
                         "a",
                         "b",
                         "x",
                         "y",
                         "rb",
                         "lb",
+                        "mode",
                     ):
                         continue
                     val = ev["value"]
                     if (
                         code not in self.state[cid]
                         or bool(self.state[cid][code]) != val
                     ):
                         changed.append((code, val))
                         self.state[cid][code] = curr + REPEAT_INITIAL if val else None
 
+        # Ignore guide combos
+        if self.state[cid].get("mode", None):
+            return
+
         # Allow holds
         for btn, val in list(self.state[cid].items()):
             if not val:
                 continue
             if val < curr:
                 changed.append((btn, True))
                 self.state[cid][btn] = curr + REPEAT_INTERVAL
```

### Comparing `hhd-2.5.0/src/hhd/plugins/overlay/overlay.py` & `hhd-2.5.1/src/hhd/plugins/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/overlay/x11.py` & `hhd-2.5.1/src/hhd/plugins/overlay/x11.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/plugin.py` & `hhd-2.5.1/src/hhd/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/powerbutton/__init__.py` & `hhd-2.5.1/src/hhd/plugins/powerbutton/__init__.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/powerbutton/base.py` & `hhd-2.5.1/src/hhd/plugins/powerbutton/base.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/powerbutton/const.py` & `hhd-2.5.1/src/hhd/plugins/powerbutton/const.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/settings.py` & `hhd-2.5.1/src/hhd/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/touchpad.yml` & `hhd-2.5.1/src/hhd/plugins/touchpad.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/plugins/utils.py` & `hhd-2.5.1/src/hhd/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/settings.yml` & `hhd-2.5.1/src/hhd/settings.yml`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd/utils.py` & `hhd-2.5.1/src/hhd/utils.py`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/src/hhd.egg-info/PKG-INFO` & `hhd-2.5.1/src/hhd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhd
-Version: 2.5.0
+Version: 2.5.1
 Summary: Handheld Daemon, a tool for configuring handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/hhd
 Project-URL: Bug Tracker, https://github.com/hhd-dev/hhd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `hhd-2.5.0/src/hhd.egg-info/SOURCES.txt` & `hhd-2.5.1/src/hhd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/usr/lib/udev/hwdb.d/83-hhd.hwdb` & `hhd-2.5.1/usr/lib/udev/hwdb.d/83-hhd.hwdb`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/usr/lib/udev/rules.d/83-hhd-user.rules` & `hhd-2.5.1/usr/lib/udev/rules.d/83-hhd-user.rules`

 * *Files identical despite different names*

### Comparing `hhd-2.5.0/usr/lib/udev/rules.d/83-hhd.rules` & `hhd-2.5.1/usr/lib/udev/rules.d/83-hhd.rules`

 * *Files identical despite different names*

