# Comparing `tmp/ffconverter-2.3.2.tar.gz` & `tmp/ffconverter-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffconverter-2.3.2.tar", last modified: Tue Feb  6 16:41:30 2024, max compression
+gzip compressed data, was "ffconverter-2.4.0.tar", last modified: Sat Apr  6 19:16:58 2024, max compression
```

## Comparing `ffconverter-2.3.2.tar` & `ffconverter-2.4.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.112059 ffconverter-2.3.2/
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      102 2024-02-06 16:31:25.000000 ffconverter-2.3.2/.gitignore
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)       50 2024-02-06 16:31:25.000000 ffconverter-2.3.2/AUTHORS
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    34665 2024-02-06 16:31:25.000000 ffconverter-2.3.2/COPYING
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     6198 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ChangeLog
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      211 2024-02-06 16:31:25.000000 ffconverter-2.3.2/MANIFEST.in
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     2511 2024-02-06 16:41:30.112059 ffconverter-2.3.2/PKG-INFO
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     3619 2024-02-06 16:31:25.000000 ffconverter-2.3.2/README.md
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      982 2024-02-06 16:31:25.000000 ffconverter-2.3.2/TRANSLATORS
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.108726 ffconverter-2.3.2/bin/
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)      114 2024-02-06 16:31:25.000000 ffconverter-2.3.2/bin/ffconverter
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.108726 ffconverter-2.3.2/ffconverter/
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      602 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/__init__.py
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)     3107 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/about_dlg.py
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)    23183 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/audiovideotab.py
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)     5253 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/config.py
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     2402 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/dynamictab.py
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    28966 2024-02-06 16:41:09.000000 ffconverter-2.3.2/ffconverter/ffconverter.py
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)     4728 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/imagetab.py
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    16574 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/preferences_dlg.py
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)    18633 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/presets_dlgs.py
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    24958 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/progress.py
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)  1251243 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/qrc_resources.py
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    26640 2024-02-06 16:31:25.000000 ffconverter-2.3.2/ffconverter/utils.py
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.112059 ffconverter-2.3.2/ffconverter.egg-info/
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     2511 2024-02-06 16:41:30.000000 ffconverter-2.3.2/ffconverter.egg-info/PKG-INFO
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     1273 2024-02-06 16:41:30.000000 ffconverter-2.3.2/ffconverter.egg-info/SOURCES.txt
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)        1 2024-02-06 16:41:30.000000 ffconverter-2.3.2/ffconverter.egg-info/dependency_links.txt
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)       12 2024-02-06 16:41:30.000000 ffconverter-2.3.2/ffconverter.egg-info/top_level.txt
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)      114 2024-02-06 16:31:25.000000 ffconverter-2.3.2/launcher
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.112059 ffconverter-2.3.2/locale/
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      862 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter.pro
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    45600 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_bg.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    35525 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_ca.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    35959 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_cs.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    36320 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_de_DE.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    38690 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_el.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    33999 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_en.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    35421 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_es.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    43549 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_fr.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    42403 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_gl.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    42406 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_gl_ES.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    41592 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_hu.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    42338 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_it.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    37555 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_ms_MY.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    39570 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_pl_PL.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    38218 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_pt.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    39782 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_pt_BR.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    38131 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_ro_RO.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    45091 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_ru.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    40891 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_tr.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    43700 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_vi.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    42125 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_zh_CN.ts
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    41525 2024-02-06 16:31:25.000000 ffconverter-2.3.2/locale/ffconverter_zh_TW.ts
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.112059 ffconverter-2.3.2/man/
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      730 2024-02-06 16:31:25.000000 ffconverter-2.3.2/man/ffconverter.1.gz
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)     1517 2024-02-06 16:31:25.000000 ffconverter-2.3.2/resources.qrc
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)       38 2024-02-06 16:41:30.112059 ffconverter-2.3.2/setup.cfg
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)     3392 2024-02-06 16:31:25.000000 ffconverter-2.3.2/setup.py
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.112059 ffconverter-2.3.2/share/
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)      404 2024-02-06 16:31:25.000000 ffconverter-2.3.2/share/ffconverter.desktop
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    30976 2024-02-06 16:31:25.000000 ffconverter-2.3.2/share/ffconverter.png
--rw-r--r--   0 lorenz    (1000) lorenz    (1000)    39299 2024-02-06 16:31:25.000000 ffconverter-2.3.2/share/presets.xml
-drwxr-xr-x   0 lorenz    (1000) lorenz    (1000)        0 2024-02-06 16:41:30.112059 ffconverter-2.3.2/test/
--rwxr-xr-x   0 lorenz    (1000) lorenz    (1000)      816 2024-02-06 16:31:25.000000 ffconverter-2.3.2/test/test_dialogs.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.377552 ffconverter-2.4.0/
+-rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.0/AUTHORS
+-rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.0/COPYING
+-rw-r--r--   0 luna      (1000) luna      (1000)     6438 2024-04-06 19:15:18.000000 ffconverter-2.4.0/ChangeLog
+-rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.0/MANIFEST.in
+-rw-r--r--   0 luna      (1000) luna      (1000)     2511 2024-04-06 19:16:58.377552 ffconverter-2.4.0/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     3731 2024-04-06 19:16:14.000000 ffconverter-2.4.0/README.md
+-rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.0/TRANSLATORS
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.370885 ffconverter-2.4.0/bin/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.0/bin/ffconverter
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.370885 ffconverter-2.4.0/ffconverter/
+-rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-06 19:12:53.000000 ffconverter-2.4.0/ffconverter/__init__.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/about_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/audiovideotab.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/config.py
+-rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.0/ffconverter/dynamictab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    29084 2024-04-04 20:10:23.000000 ffconverter-2.4.0/ffconverter/ffconverter.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/imagetab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/preferences_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/presets_dlgs.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    26813 2024-04-04 19:50:46.000000 ffconverter-2.4.0/ffconverter/progress.py
+-rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/qrc_resources.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    27171 2024-04-04 16:33:34.000000 ffconverter-2.4.0/ffconverter/utils.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/ffconverter.egg-info/
+-rw-r--r--   0 luna      (1000) luna      (1000)     2511 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     1262 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/top_level.txt
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.0/launcher
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/locale/
+-rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter.pro
+-rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_bg.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ca.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_cs.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_de_DE.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_el.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_en.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_es.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_fr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_gl.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_gl_ES.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_hu.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_it.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ms_MY.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_pl_PL.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_pt.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_pt_BR.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ro_RO.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ru.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_tr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_vi.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_zh_CN.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_zh_TW.ts
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/man/
+-rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.0/man/ffconverter.1.gz
+-rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.0/resources.qrc
+-rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-06 19:16:58.377552 ffconverter-2.4.0/setup.cfg
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3392 2024-03-02 10:15:40.000000 ffconverter-2.4.0/setup.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/share/
+-rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-06 19:12:59.000000 ffconverter-2.4.0/share/ffconverter.desktop
+-rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.0/share/ffconverter.png
+-rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.0/share/presets.xml
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/test/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.0/test/test_dialogs.py
```

### Comparing `ffconverter-2.3.2/COPYING` & `ffconverter-2.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ChangeLog` & `ffconverter-2.4.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Version 2.4.0
+-------------
+
+* Added trimesh/gmsh to support 3D-Models (close #11)
+
+* Fixed crash when using drag-and-drop (close #12)
+
+* When set to only show common file types, still show uncommon ones
+  if no common types are available
+
 Version 2.3.2
 -------------
 
 * Added Caching to all_supported_conversions and missing to make
   starting the program faster.
 
 * Fix Issue #10: Will now no longer freeze if the external program is
```

### Comparing `ffconverter-2.3.2/PKG-INFO` & `ffconverter-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.3.2
+Version: 2.4.0
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
```

### Comparing `ffconverter-2.3.2/README.md` & `ffconverter-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,29 @@
 
 On Linux, use your distributions package manager or pip to install these.  
 On Windows, use [python.org](https://python.org) to get python (the version  
 in the Microsoft Store is [worse in some regards](https://docs.python.org/3/using/windows.html#known-issues)), then use  
 `python -m pip install PyQt5` to get PyQt5.  
 
 #### Optional dependencies:
-(Without these some conversions will not work)  
+Without these some conversions will not work.  
+
+System Packages:  
 
 * ffmpeg (Audio and Video)  
 * imagemagick (Images)  
 * unoconv (Office formats)  
 * pandoc (Markdown)  
 * squashfs-tools, zip, unzip, binutils, tar, gzip, bzip2 (Compressed files)  
 
+Python packages:  
+
+* trimesh _AND_ gmsh (python packages, used for 3D Models)  
+
+
 On Linux, use your distributions Package manager to install these.  
 On Windows, either get .exe files and place them on the $PATH , use [scoop](https://scoop.sh),  
 or (for everything but ffmpeg) install the dependencies in WSL.  
 You could also try other third-party package managers  
 or even the Microsoft Store, the program only needs the command  
 (e.g. `unoconv`) to be available on the CMD.  
 
@@ -47,15 +54,15 @@
 
 #### Troubleshooting
 If a optional dependency is installed after the program, you might  
 need to restart the program twice to ensure the cache gets overwritten.  
 If this does not work, delete the cache (Preferences -> Delete Cache).  
 
 #### Troubleshooting (Linux)
-On some distros (externally managed environments, Arch, Debian),  
+On some distros ("externally managed environments", like Arch and Debian),  
 `pip` will not work. In this case, you should use `pipx`.  
 
 ```sh
 sudo PIPX_HOME=/usr/local/pipx PIPX_BIN_DIR=/usr/local/bin pipx install --system-site-packages ffconverter
 sudo ln -sf /usr/local/pipx/venvs/ffconverter/share/applications/ffconverter.desktop /usr/local/share/applications/ffconverter.desktop
 sudo ln -sf /usr/local/pipx/venvs/ffconverter/share/pixmaps/ffconverter.png /usr/local/share/icons/ffconverter.png
 ```
```

### Comparing `ffconverter-2.3.2/TRANSLATORS` & `ffconverter-2.4.0/TRANSLATORS`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/__init__.py` & `ffconverter-2.4.0/ffconverter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 GUI File Format Converter
 """
 
 # version
 __major__ = 2
-__minor__ = 3
-__patch__ = 2
+__minor__ = 4
+__patch__ = 0
 __prerelease__ = "" # alpha, beta, rc etc.
 
 # package information
 __name__ = "ffconverter"
 __version__ = "{0}.{1}.{2}".format(__major__, __minor__, __patch__)
 __version__ += __prerelease__
 __description__ = "File Format Converter with Qt GUI"
```

### Comparing `ffconverter-2.3.2/ffconverter/about_dlg.py` & `ffconverter-2.4.0/ffconverter/about_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/audiovideotab.py` & `ffconverter-2.4.0/ffconverter/audiovideotab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/config.py` & `ffconverter-2.4.0/ffconverter/config.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/dynamictab.py` & `ffconverter-2.4.0/ffconverter/dynamictab.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,11 +52,12 @@
     def fill_extension_combobox(self, list_of_files, all_supported_conversions):
         self.extQCB.clear()
         common = []
         if self.commonformatQChB.isChecked():
             common = (self.parent.settings.value('extraformats_common') or []) + config.common_formats
         outputs = utils.get_combobox_content(self, list_of_files, all_supported_conversions,
                                              common=common)
+
         self.extQCB.addItems(outputs)
 
     def ok_to_continue(self):
         return True
```

### Comparing `ffconverter-2.3.2/ffconverter/ffconverter.py` & `ffconverter-2.4.0/ffconverter/ffconverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,22 +376,22 @@
         mobile_ui = self.settings.value('mobile_ui', type=bool)
         if not utils.is_installed(self.ffmpeg_path, use_wsl):
             self.ffmpeg_path = utils.is_installed('ffmpeg', use_wsl)
             QSettings().setValue('ffmpeg_path', self.ffmpeg_path)
         self.unoconv = utils.is_installed('unoconv', use_wsl)
         self.imagemagick = utils.is_installed('magick', use_wsl)
         self.pandoc = utils.is_installed('pandoc', use_wsl)
-
         self.compress_zip = utils.is_installed('zip', use_wsl)
         self.compress_unzip = utils.is_installed('unzip', use_wsl)
         self.compress_tar = utils.is_installed('tar', use_wsl)
         self.compress_squash = utils.is_installed('mksquashfs', use_wsl) and utils.is_installed('unsquashfs', use_wsl)
         self.compress_ar = utils.is_installed('ar', use_wsl)
         self.compress_gzip = utils.is_installed('gzip', use_wsl)
         self.compress_bzip2 = utils.is_installed('bzip2', use_wsl)
+        self.trimesh = utils.is_installed('trimesh', use_wsl)
 
         self.missing = []
         if not self.ffmpeg_path:
             self.missing.append('ffmpeg')
         if not self.unoconv:
             self.missing.append('unoconv')
         if not self.imagemagick:
@@ -408,25 +408,26 @@
             self.missing.append('squashfs-tools')
         if not self.compress_ar:
             self.missing.append('binutils/ar')
         if not self.compress_gzip:
             self.missing.append('gzip')
         if not self.compress_bzip2:
             self.missing.append('bzip2')
+        if not self.trimesh:
+            self.missing.append('trimesh')
 
         if self.missing:
             status = ', '.join(self.missing)
             status = self.tr('Missing dependencies:') + ' ' + status
             if mobile_ui:
                 print(status)
             else:
                 self.dependenciesQL.setText(status)
 
     def load_settings(self, settings):
-
         self.mobile_ui = settings.value('mobile_ui', type=bool)
         self.overwrite_existing = settings.value('overwrite_existing', type=bool)
         self.default_output = settings.value('default_output', type=str)
         self.prefix = settings.value('prefix', type=str)
         self.suffix = settings.value('suffix', type=str)
         self.ffmpeg_path = settings.value('ffmpeg_path', type=str)
         self.default_command = (settings.value('default_command', type=str) or
@@ -495,19 +496,18 @@
                 self.toQLE.setText(dir_of_first_file)
 
     def filesList_add_dragged(self, links):
         for path in links:
             if os.path.isfile(path) and not path in self.fnames:
                 self.fnames.append(path)
         self.filesList_update()
-        if fnames:
-            # Set toQLE to the dir of the first file, if toQLE not set
-            if self.toQLE.text() == "":
-                dir_of_first_file = os.path.dirname(os.path.abspath(fnames[0]))
-                self.toQLE.setText(dir_of_first_file)
+        # Set toQLE to the dir of the first file, if toQLE not set
+        if self.fnames and self.toQLE.text() == "":
+            dir_of_first_file = os.path.dirname(os.path.abspath(self.fnames[0]))
+            self.toQLE.setText(dir_of_first_file)
 
     def filesList_delete(self):
         items = self.filesList.selectedItems()
         if items:
             for i in items:
                 self.fnames.remove(i.text())
             self.filesList_update()
```

### Comparing `ffconverter-2.3.2/ffconverter/imagetab.py` & `ffconverter-2.4.0/ffconverter/imagetab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/preferences_dlg.py` & `ffconverter-2.4.0/ffconverter/preferences_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/presets_dlgs.py` & `ffconverter-2.4.0/ffconverter/presets_dlgs.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/progress.py` & `ffconverter-2.4.0/ffconverter/progress.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import io
 import signal
 import threading
 import subprocess
 import shlex
 import shutil
 import logging
+import sys
 from pathlib import Path
 
 from PyQt5.QtCore import pyqtSignal, QTimer
 from PyQt5.QtGui import QTextCursor
 from PyQt5.QtWidgets import (
         QApplication, QDialog, QFrame, QLabel, QPushButton, QProgressBar,
         QMessageBox, QTextEdit, QCommandLinkButton, QSizePolicy, QCheckBox
@@ -261,35 +262,51 @@
                 conv_func = self.convert_compression
                 params = (from_file, to_file)
             elif self._type == "Documents":
                 conv_func = self.convert_document
                 params = (from_file, to_file)
             else:
                 conv_func = self.convert_dynamic
-                params = (from_file, to_file)
+                params = (from_file, to_file, converter)
 
             try:
                 if conv_func(*params):
                     self.ok += 1
                     if self.delete and not from_file == to_file:
                         try:
                             os.remove(from_file[1:-1])
                         except OSError:
                             pass
                 else:
                     self.error += 1
             except Exception as e:
                 # convert() caused a exception, likely a wrong command was used.
-                print(f"convert() thread exception: {e}")
+                self.update_text_edit_signal.emit(f"Exception in convert(): {e}\n")
                 self.error += 1
 
             self.file_converted_signal.emit()
 
-        self.thread = threading.Thread(target=convert)
-        self.thread.start()
+        force_no_thread = False
+        # trimesh doesn't work with threads
+        if self._type not in ['AudioVideo', 'Images', 'Markdown', 'Compression', 'Documents']:
+            from_file_ext = utils.get_extension(from_file)
+            to_file_ext = utils.get_extension(to_file)
+            converter = utils.get_all_conversions(self.parent.settings, 
+                                                get_conv_for_ext=True,
+                                                ext=[from_file_ext,to_file_ext],
+                                                missing=self.parent.missing,
+                                                use_wsl=self.parent.use_wsl)
+            if converter == "trimesh":
+                convert()
+            else:
+                self.thread = threading.Thread(target=convert)
+                self.thread.start()
+        else:
+            self.thread = threading.Thread(target=convert)
+            self.thread.start()
 
     def convert_video(self, from_file, to_file, command):
         """
         Create the ffmpeg command and execute it in a new process using the
         subprocess module. While the process is alive, parse ffmpeg output,
         estimate conversion progress using video's duration.
         With the result, emit the corresponding signal in order progress bar
@@ -599,28 +616,47 @@
         log_lvl(final_output, extra=log_data)
 
         if to_file_ext not in ['[Folder]']:
             shutil.rmtree(decompress_dir)
             pass
         return return_code == 0
 
-    def convert_dynamic(self, from_file, to_file):
-        from_file_ext = utils.get_extension(from_file)
-        to_file_ext = utils.get_extension(to_file)
-        converter = utils.get_all_conversions(self.parent.settings,
-                                              get_conv_for_ext=True,
-                                              ext=[from_file_ext,to_file_ext],
-                                              missing=self.parent.missing,
-                                              use_wsl=self.parent.use_wsl)
+    def convert_model(self, from_file, to_file):
+        # can't be imported at the start because its a optional dependency
+        import trimesh
+        # python library doesn't need escaped paths, we can undo that
+        from_file = from_file.replace('"', '').replace('\\', '')
+        to_file   =   to_file.replace('"', '').replace('\\', '')
+        
+        needs_gmsh = utils.get_extension(from_file) in ['iges', 'stp', 'step', 'brep']
+        try:
+            if utils.get_extension(from_file) in ['iges', 'stp', 'step', 'brep']:
+                self.update_text_edit_signal.emit(f"Loading file from {from_file} using trimesh.gmsh\n")
+                mesh = trimesh.Trimesh(**trimesh.interfaces.gmsh.load_gmsh(file_name=from_file))
+            else:
+                self.update_text_edit_signal.emit(f"Loading file from {from_file} using trimesh.default\n")
+                mesh = trimesh.load(from_file)
+            self.update_text_edit_signal.emit(f"Saving File to {to_file}\n")
+            mesh.export(to_file)
+        except Exception as e:
+            self.update_text_edit_signal.emit(f"Failed: {e}\n")
+            return False
+        return True
+
+    def convert_dynamic(self, from_file, to_file, converter):
         if converter == "ffmpeg":
             return self.convert_video(from_file, to_file, "")
         elif converter == "pandoc":
             return self.convert_markdown(from_file, to_file)
         elif converter == "magick":
             return self.convert_image(from_file, to_file, "", "", "")
         elif converter == "soffice":
             return self.convert_document(from_file, to_file)
         elif converter == "compression":
             return self.convert_compression(from_file, to_file)
-        else:
+        elif converter == "trimesh":
+            return self.convert_model(from_file, to_file)
+        elif converter == "unsupported":
             print("Error: Did not find suitable converter for dynamic conversion!")
-            return False
+        else:
+            print(f"Error: Found converter \"{converter}\", but it does not implement conversion yet!")
+        return False
```

### Comparing `ffconverter-2.3.2/ffconverter/qrc_resources.py` & `ffconverter-2.4.0/ffconverter/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/ffconverter/utils.py` & `ffconverter-2.4.0/ffconverter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import re
 import sys
 import shlex
 import subprocess
 import time
 import string
 import threading
+import importlib.util
 
 from PyQt5.QtCore import pyqtSignal, QSize, Qt, QSettings
 from PyQt5.QtWidgets import (
         QAction, QLayout, QLineEdit, QListWidget, QListWidgetItem, QMenu,
         QSpacerItem, QWidget, QHBoxLayout, QVBoxLayout, QGridLayout
         )
 from ffconverter import config
@@ -56,14 +57,18 @@
 
     If program is an absolute path, returns the path if it's executable, else
     empty string.
     """
 
     if program.startswith('wsl'): return program # do not resolve WSL paths
 
+    if program == 'trimesh':
+        is_installed = importlib.util.find_spec(program) is not None
+        return is_installed
+
     # wsl_only is used to not get "convert" on a windows system
     if wsl_only == False:
         path_env = os.getenv('PATH').split(os.pathsep)
         for path in path_env:
             fpath = os.path.join(path, program)
             if os.name == 'nt':
                 fpath_ls = [fpath, fpath+'.exe', fpath+'.cmd', fpath+'.bat']
@@ -290,14 +295,21 @@
         compression_exts[0] += ['deb', 'a', 'ar', 'o', 'so']
         compression_exts[1] += ['ar']
     if compression_exts != [[], []]: # if any of the tools work
         compression_exts[0] += extraformats_compression
         compression_exts[1] += extraformats_compression + ['[Folder]']
     supported_tmp.append(compression_exts)
 
+    model_exts = [[], []]
+    if 'trimesh' not in missing:
+        # TODO: trimesh can load/export far more types, add these
+        model_exts[0] += ['step']
+        model_exts[1] += ['stl']
+    supported_tmp.append(model_exts)
+
     # if the function is meant to return a converter for a in/output pair
     if get_conv_for_ext:
         if ext[0] in ffmpeg_conversions[0] and ext[1] in ffmpeg_conversions[1]:
             return "ffmpeg"
         elif ext[0] in pandoc_conversions[0] and ext[1] in pandoc_conversions[1]:
             return "pandoc"
         elif ext[0] in magick_conversions[0] and ext[1] in magick_conversions[1]:
@@ -308,14 +320,16 @@
             return "soffice"
         elif ext[0] in slide[0] and ext[1] in slide[1]:
             return "soffice"
         elif ext[0] in text[0] and ext[1] in text[1]:
             return "soffice"
         elif ext[0] in compression_exts[0] and ext[1] in compression_exts[1]:
             return "compression"
+        elif ext[0] in model_exts[0] and ext[1] in model_exts[1]:
+            return "trimesh"
         else:
             return "unsupported"
     else:
         return supported_tmp
 
 def get_extension(file_path):
     """
@@ -333,16 +347,16 @@
     remainder, first_ext = os.path.splitext(file_path)
     first_ext = first_ext[1:]
     second_ext = os.path.splitext(remainder)[-1][1:] # '' if only one ext there
     joined_ext = second_ext + '.' + first_ext
 
     all_double = config.double_formats + (settings.value('extraformats_double') or [])
     if joined_ext in all_double:
-        return joined_ext
-    return first_ext
+        return joined_ext.lower()
+    return first_ext.lower()
 
 def get_combobox_content(self, list_of_files, all_supported_conversions,
                          common=[]):
     possible_outputs = []
     for input_file in list_of_files:
         file_outputs = []
         input_file_ext = get_extension(input_file)
@@ -364,15 +378,15 @@
             if available and extension not in valid_outputs:
                 valid_outputs.append(extension)
     else:
         # flatten and deduplicate
         first_output_list = possible_outputs[0] if possible_outputs else []
         valid_outputs = list(dict.fromkeys(first_output_list))
 
-    if common != []:
+    if [ext for ext in valid_outputs if ext in common] != []:
         # remove all uncommon formats from the list
         valid_outputs[:] = [ext for ext in valid_outputs if ext in common]
     return valid_outputs
 
 def start_office_listener():
     """
     Start a openoffice/libreoffice listener.
```

### Comparing `ffconverter-2.3.2/ffconverter.egg-info/PKG-INFO` & `ffconverter-2.4.0/ffconverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.3.2
+Version: 2.4.0
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
```

### Comparing `ffconverter-2.3.2/ffconverter.egg-info/SOURCES.txt` & `ffconverter-2.4.0/ffconverter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.gitignore
 AUTHORS
 COPYING
 ChangeLog
 MANIFEST.in
 README.md
 TRANSLATORS
 launcher
```

### Comparing `ffconverter-2.3.2/locale/ffconverter.pro` & `ffconverter-2.4.0/locale/ffconverter.pro`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_bg.ts` & `ffconverter-2.4.0/locale/ffconverter_bg.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_ca.ts` & `ffconverter-2.4.0/locale/ffconverter_ca.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_cs.ts` & `ffconverter-2.4.0/locale/ffconverter_cs.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_de_DE.ts` & `ffconverter-2.4.0/locale/ffconverter_de_DE.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_el.ts` & `ffconverter-2.4.0/locale/ffconverter_el.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_en.ts` & `ffconverter-2.4.0/locale/ffconverter_en.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_es.ts` & `ffconverter-2.4.0/locale/ffconverter_es.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_fr.ts` & `ffconverter-2.4.0/locale/ffconverter_fr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_gl.ts` & `ffconverter-2.4.0/locale/ffconverter_gl.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_gl_ES.ts` & `ffconverter-2.4.0/locale/ffconverter_gl_ES.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_hu.ts` & `ffconverter-2.4.0/locale/ffconverter_hu.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_it.ts` & `ffconverter-2.4.0/locale/ffconverter_it.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_ms_MY.ts` & `ffconverter-2.4.0/locale/ffconverter_ms_MY.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_pl_PL.ts` & `ffconverter-2.4.0/locale/ffconverter_pl_PL.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_pt.ts` & `ffconverter-2.4.0/locale/ffconverter_pt.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_pt_BR.ts` & `ffconverter-2.4.0/locale/ffconverter_pt_BR.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_ro_RO.ts` & `ffconverter-2.4.0/locale/ffconverter_ro_RO.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_ru.ts` & `ffconverter-2.4.0/locale/ffconverter_ru.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_tr.ts` & `ffconverter-2.4.0/locale/ffconverter_tr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_vi.ts` & `ffconverter-2.4.0/locale/ffconverter_vi.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_zh_CN.ts` & `ffconverter-2.4.0/locale/ffconverter_zh_CN.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/locale/ffconverter_zh_TW.ts` & `ffconverter-2.4.0/locale/ffconverter_zh_TW.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/man/ffconverter.1.gz` & `ffconverter-2.4.0/man/ffconverter.1.gz`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/resources.qrc` & `ffconverter-2.4.0/resources.qrc`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/setup.py` & `ffconverter-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/share/ffconverter.png` & `ffconverter-2.4.0/share/ffconverter.png`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/share/presets.xml` & `ffconverter-2.4.0/share/presets.xml`

 * *Files identical despite different names*

### Comparing `ffconverter-2.3.2/test/test_dialogs.py` & `ffconverter-2.4.0/test/test_dialogs.py`

 * *Files identical despite different names*

