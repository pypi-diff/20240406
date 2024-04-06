# Comparing `tmp/music-dragon-0.8.tar.gz` & `tmp/music-dragon-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-dragon-0.8.tar", last modified: Sat Jun  4 13:53:48 2022, max compression
+gzip compressed data, was "music-dragon-0.9.tar", last modified: Sat Jul  9 14:16:22 2022, max compression
```

## Comparing `music-dragon-0.8.tar` & `music-dragon-0.9.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-06-04 13:53:48.821782 music-dragon-0.8/
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1058 2022-05-31 13:37:53.000000 music-dragon-0.8/LICENSE.txt
--rw-r--r--   0 stefano   (1000) stefano   (1000)       37 2022-06-01 07:16:22.000000 music-dragon-0.8/MANIFEST.in
--rw-r--r--   0 stefano   (1000) stefano   (1000)     2494 2022-06-04 13:53:48.821782 music-dragon-0.8/PKG-INFO
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1984 2022-06-04 13:53:40.000000 music-dragon-0.8/README.md
-drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-06-04 13:53:48.806782 music-dragon-0.8/music_dragon/
--rw-r--r--   0 stefano   (1000) stefano   (1000)      117 2022-06-04 13:45:23.000000 music-dragon-0.8/music_dragon/__init__.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)      864 2022-06-04 13:37:17.000000 music-dragon-0.8/music_dragon/audioplayer.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     3649 2022-05-31 14:06:53.000000 music-dragon-0.8/music_dragon/cache.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     6899 2022-06-03 19:20:24.000000 music-dragon-0.8/music_dragon/localsongs.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)      850 2022-05-31 14:17:10.000000 music-dragon-0.8/music_dragon/log.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1587 2022-06-01 20:32:12.000000 music-dragon-0.8/music_dragon/main.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    17172 2022-06-02 08:47:19.000000 music-dragon-0.8/music_dragon/musicbrainz.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     2194 2022-06-01 07:27:40.000000 music-dragon-0.8/music_dragon/preferences.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    59485 2022-06-04 07:50:33.000000 music-dragon-0.8/music_dragon/repository.py
-drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-06-04 13:53:48.816782 music-dragon-0.8/music_dragon/ui/
--rw-r--r--   0 stefano   (1000) stefano   (1000)        0 2022-05-31 13:49:02.000000 music-dragon-0.8/music_dragon/ui/__init__.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    10236 2022-06-03 12:55:17.000000 music-dragon-0.8/music_dragon/ui/albumtrackswidget.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     3952 2022-05-31 14:06:53.000000 music-dragon-0.8/music_dragon/ui/artistalbumswidget.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     2006 2022-05-20 15:30:44.000000 music-dragon-0.8/music_dragon/ui/clickablelabel.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)      255 2022-05-14 08:54:46.000000 music-dragon-0.8/music_dragon/ui/clickablewidget.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)      649 2022-06-03 19:12:31.000000 music-dragon-0.8/music_dragon/ui/clickslider.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    10025 2022-06-02 08:27:59.000000 music-dragon-0.8/music_dragon/ui/downloadswidget.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1523 2022-05-31 22:15:55.000000 music-dragon-0.8/music_dragon/ui/imagepreviewwindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     3815 2022-06-01 08:49:52.000000 music-dragon-0.8/music_dragon/ui/listwidgetmodelview.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     8362 2022-05-31 14:06:53.000000 music-dragon-0.8/music_dragon/ui/localalbumsview.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     9124 2022-05-31 14:06:53.000000 music-dragon-0.8/music_dragon/ui/localartistsview.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    10974 2022-06-04 07:33:48.000000 music-dragon-0.8/music_dragon/ui/localsongsview.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    56722 2022-06-03 20:26:47.000000 music-dragon-0.8/music_dragon/ui/mainwindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     3937 2022-05-31 14:08:11.000000 music-dragon-0.8/music_dragon/ui/preferenceswindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)   316253 2022-06-04 10:18:46.000000 music-dragon-0.8/music_dragon/ui/res_rc.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     2242 2022-06-03 14:36:23.000000 music-dragon-0.8/music_dragon/ui/resources.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     8840 2022-06-01 07:59:48.000000 music-dragon-0.8/music_dragon/ui/searchresultswidget.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1895 2022-06-04 10:18:46.000000 music-dragon-0.8/music_dragon/ui/ui_imagepreviewwindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    37504 2022-06-04 10:18:46.000000 music-dragon-0.8/music_dragon/ui/ui_mainwindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    16544 2022-06-04 10:18:45.000000 music-dragon-0.8/music_dragon/ui/ui_preferenceswindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     2194 2022-05-31 14:08:11.000000 music-dragon-0.8/music_dragon/ui/ytmusicsetupwindow.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     4907 2022-06-04 09:18:12.000000 music-dragon-0.8/music_dragon/utils.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     3329 2022-05-31 14:06:53.000000 music-dragon-0.8/music_dragon/wiki.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    10985 2022-06-02 08:25:42.000000 music-dragon-0.8/music_dragon/workers.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1735 2022-05-31 10:06:33.000000 music-dragon-0.8/music_dragon/ytcommons.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)    18770 2022-05-31 20:52:44.000000 music-dragon-0.8/music_dragon/ytdownloader.py
--rw-r--r--   0 stefano   (1000) stefano   (1000)     7906 2022-06-04 07:39:49.000000 music-dragon-0.8/music_dragon/ytmusic.py
-drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-06-04 13:53:48.807782 music-dragon-0.8/music_dragon.egg-info/
--rw-r--r--   0 stefano   (1000) stefano   (1000)     2494 2022-06-04 13:53:48.000000 music-dragon-0.8/music_dragon.egg-info/PKG-INFO
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1654 2022-06-04 13:53:48.000000 music-dragon-0.8/music_dragon.egg-info/SOURCES.txt
--rw-r--r--   0 stefano   (1000) stefano   (1000)        1 2022-06-04 13:53:48.000000 music-dragon-0.8/music_dragon.egg-info/dependency_links.txt
--rw-r--r--   0 stefano   (1000) stefano   (1000)       56 2022-06-04 13:53:48.000000 music-dragon-0.8/music_dragon.egg-info/entry_points.txt
--rw-r--r--   0 stefano   (1000) stefano   (1000)       90 2022-06-04 13:53:48.000000 music-dragon-0.8/music_dragon.egg-info/requires.txt
--rw-r--r--   0 stefano   (1000) stefano   (1000)       13 2022-06-04 13:53:48.000000 music-dragon-0.8/music_dragon.egg-info/top_level.txt
-drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-06-04 13:53:48.804782 music-dragon-0.8/res/
-drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-06-04 13:53:48.820782 music-dragon-0.8/res/images/
--rw-r--r--   0 stefano   (1000) stefano   (1000)     4038 2022-05-10 13:59:31.000000 music-dragon-0.8/res/images/back.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      414 2022-05-28 08:56:03.000000 music-dragon-0.8/res/images/delete.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      415 2022-05-11 09:02:58.000000 music-dragon-0.8/res/images/download.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)     4523 2022-05-14 13:57:43.000000 music-dragon-0.8/res/images/forward.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      746 2022-05-20 13:51:49.000000 music-dragon-0.8/res/images/left.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)     4671 2022-05-12 22:45:24.000000 music-dragon-0.8/res/images/loader.gif
--rw-r--r--   0 stefano   (1000) stefano   (1000)    26166 2022-05-31 14:15:23.000000 music-dragon-0.8/res/images/logo.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      877 2022-05-23 09:03:10.000000 music-dragon-0.8/res/images/openfolder.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      900 2022-05-21 13:09:05.000000 music-dragon-0.8/res/images/openlink.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)    26201 2022-05-15 14:39:12.000000 music-dragon-0.8/res/images/person.jpg
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1147 2022-05-09 22:38:27.000000 music-dragon-0.8/res/images/questionmark.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      704 2022-05-20 13:51:11.000000 music-dragon-0.8/res/images/right.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)      567 2022-05-23 14:19:52.000000 music-dragon-0.8/res/images/x.png
--rw-r--r--   0 stefano   (1000) stefano   (1000)       38 2022-06-04 13:53:48.821782 music-dragon-0.8/setup.cfg
--rw-r--r--   0 stefano   (1000) stefano   (1000)     1284 2022-06-03 13:07:49.000000 music-dragon-0.8/setup.py
+drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-07-09 14:16:22.242740 music-dragon-0.9/
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1058 2022-05-31 13:37:53.000000 music-dragon-0.9/LICENSE.txt
+-rw-r--r--   0 stefano   (1000) stefano   (1000)       37 2022-06-01 07:16:22.000000 music-dragon-0.9/MANIFEST.in
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2494 2022-07-09 14:16:22.242740 music-dragon-0.9/PKG-INFO
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1984 2022-06-04 13:53:40.000000 music-dragon-0.9/README.md
+drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-07-09 14:16:22.227740 music-dragon-0.9/music_dragon/
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      184 2022-07-09 14:16:01.000000 music-dragon-0.9/music_dragon/__init__.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      979 2022-06-22 10:00:42.000000 music-dragon-0.9/music_dragon/audioplayer.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     5604 2022-06-27 09:58:54.000000 music-dragon-0.9/music_dragon/cache.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    10250 2022-06-27 08:30:12.000000 music-dragon-0.9/music_dragon/localsongs.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      850 2022-05-31 14:17:10.000000 music-dragon-0.9/music_dragon/log.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2300 2022-06-22 08:12:12.000000 music-dragon-0.9/music_dragon/main.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    19840 2022-06-27 13:46:57.000000 music-dragon-0.9/music_dragon/musicbrainz.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     3573 2022-07-05 06:30:39.000000 music-dragon-0.9/music_dragon/preferences.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    64645 2022-07-05 06:30:39.000000 music-dragon-0.9/music_dragon/repository.py
+drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-07-09 14:16:22.237740 music-dragon-0.9/music_dragon/ui/
+-rw-r--r--   0 stefano   (1000) stefano   (1000)        0 2022-05-31 13:49:02.000000 music-dragon-0.9/music_dragon/ui/__init__.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     9718 2022-06-28 13:59:29.000000 music-dragon-0.9/music_dragon/ui/albumtrackswidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     3952 2022-06-21 15:23:22.000000 music-dragon-0.9/music_dragon/ui/artistalbumswidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2006 2022-05-20 15:30:44.000000 music-dragon-0.9/music_dragon/ui/clickablelabel.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      255 2022-05-14 08:54:46.000000 music-dragon-0.9/music_dragon/ui/clickablewidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      775 2022-07-06 13:08:34.000000 music-dragon-0.9/music_dragon/ui/clickslider.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    10282 2022-06-28 14:23:00.000000 music-dragon-0.9/music_dragon/ui/downloadswidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      554 2022-06-28 13:32:01.000000 music-dragon-0.9/music_dragon/ui/editlinkwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1607 2022-06-28 14:32:36.000000 music-dragon-0.9/music_dragon/ui/imagepreviewwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      293 2022-07-03 13:43:33.000000 music-dragon-0.9/music_dragon/ui/listproxyview.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     3865 2022-06-08 06:40:35.000000 music-dragon-0.9/music_dragon/ui/listwidgetmodelview.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     9905 2022-07-03 13:54:16.000000 music-dragon-0.9/music_dragon/ui/localalbumsview.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2716 2022-06-22 14:36:43.000000 music-dragon-0.9/music_dragon/ui/localalbumtrackswidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     3692 2022-06-24 09:58:57.000000 music-dragon-0.9/music_dragon/ui/localartistalbumswidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    10103 2022-07-03 13:54:16.000000 music-dragon-0.9/music_dragon/ui/localartistsview.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    12283 2022-07-03 13:50:26.000000 music-dragon-0.9/music_dragon/ui/localsongsview.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    75617 2022-07-09 13:40:54.000000 music-dragon-0.9/music_dragon/ui/mainwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     6201 2022-07-05 06:30:39.000000 music-dragon-0.9/music_dragon/ui/preferenceswindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)   325921 2022-07-09 13:40:55.000000 music-dragon-0.9/music_dragon/ui/res_rc.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2466 2022-06-28 13:08:02.000000 music-dragon-0.9/music_dragon/ui/resources.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     8840 2022-06-01 07:59:48.000000 music-dragon-0.9/music_dragon/ui/searchresultswidget.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2016 2022-07-09 13:40:55.000000 music-dragon-0.9/music_dragon/ui/ui_editlinkwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1895 2022-07-09 13:40:55.000000 music-dragon-0.9/music_dragon/ui/ui_imagepreviewwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    55273 2022-07-09 13:40:55.000000 music-dragon-0.9/music_dragon/ui/ui_mainwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    23631 2022-07-09 13:40:55.000000 music-dragon-0.9/music_dragon/ui/ui_preferenceswindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     3686 2022-07-09 13:40:55.000000 music-dragon-0.9/music_dragon/ui/ui_youtubesigninwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      866 2022-06-08 07:11:18.000000 music-dragon-0.9/music_dragon/ui/youtubesigninwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2194 2022-05-31 14:08:11.000000 music-dragon-0.9/music_dragon/ui/ytmusicsetupwindow.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     5129 2022-07-05 06:22:53.000000 music-dragon-0.9/music_dragon/utils.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     3329 2022-05-31 14:06:53.000000 music-dragon-0.9/music_dragon/wiki.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    11559 2022-07-07 23:43:23.000000 music-dragon-0.9/music_dragon/workers.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1735 2022-05-31 10:06:33.000000 music-dragon-0.9/music_dragon/ytcommons.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    20572 2022-07-08 08:05:47.000000 music-dragon-0.9/music_dragon/ytdownloader.py
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    34249 2022-07-07 06:59:04.000000 music-dragon-0.9/music_dragon/ytmusic.py
+drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-07-09 14:16:22.228740 music-dragon-0.9/music_dragon.egg-info/
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     2494 2022-07-09 14:16:22.000000 music-dragon-0.9/music_dragon.egg-info/PKG-INFO
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1924 2022-07-09 14:16:22.000000 music-dragon-0.9/music_dragon.egg-info/SOURCES.txt
+-rw-r--r--   0 stefano   (1000) stefano   (1000)        1 2022-07-09 14:16:22.000000 music-dragon-0.9/music_dragon.egg-info/dependency_links.txt
+-rw-r--r--   0 stefano   (1000) stefano   (1000)       56 2022-07-09 14:16:22.000000 music-dragon-0.9/music_dragon.egg-info/entry_points.txt
+-rw-r--r--   0 stefano   (1000) stefano   (1000)       86 2022-07-09 14:16:22.000000 music-dragon-0.9/music_dragon.egg-info/requires.txt
+-rw-r--r--   0 stefano   (1000) stefano   (1000)       13 2022-07-09 14:16:22.000000 music-dragon-0.9/music_dragon.egg-info/top_level.txt
+drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-07-09 14:16:22.222740 music-dragon-0.9/res/
+drwxr-xr-x   0 stefano   (1000) stefano   (1000)        0 2022-07-09 14:16:22.242740 music-dragon-0.9/res/images/
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     4038 2022-05-10 13:59:31.000000 music-dragon-0.9/res/images/back.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      414 2022-05-28 08:56:03.000000 music-dragon-0.9/res/images/delete.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      415 2022-05-11 09:02:58.000000 music-dragon-0.9/res/images/download.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     4523 2022-05-14 13:57:43.000000 music-dragon-0.9/res/images/forward.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      746 2022-05-20 13:51:49.000000 music-dragon-0.9/res/images/left.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     4671 2022-05-12 22:45:24.000000 music-dragon-0.9/res/images/loader.gif
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    26166 2022-05-31 14:15:23.000000 music-dragon-0.9/res/images/logo.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      877 2022-05-23 09:03:10.000000 music-dragon-0.9/res/images/openfolder.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      900 2022-05-21 13:09:05.000000 music-dragon-0.9/res/images/openlink.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)    26201 2022-05-15 14:39:12.000000 music-dragon-0.9/res/images/person.jpg
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1147 2022-05-09 22:38:27.000000 music-dragon-0.9/res/images/questionmark.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      704 2022-05-20 13:51:11.000000 music-dragon-0.9/res/images/right.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)      567 2022-05-23 14:19:52.000000 music-dragon-0.9/res/images/x.png
+-rw-r--r--   0 stefano   (1000) stefano   (1000)       38 2022-07-09 14:16:22.242740 music-dragon-0.9/setup.cfg
+-rw-r--r--   0 stefano   (1000) stefano   (1000)     1280 2022-06-08 07:42:14.000000 music-dragon-0.9/setup.py
```

### Comparing `music-dragon-0.8/LICENSE.txt` & `music-dragon-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/PKG-INFO` & `music-dragon-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-dragon
-Version: 0.8
+Version: 0.9
 Summary: All-in-one music manager: scrapes albums, artists and songs from musicbrainz and automatically download them from youtube.
 Home-page: https://github.com/Docheinstein/music-dragon
 Author: Stefano Dottore
 Author-email: docheinstein@gmail.com
 License: MIT
 Keywords: music manager youtube spotify musicbrainz musicbrainzngs tag cover eyed3 ytmusicapi youtube_dl
 Requires-Python: >=3
```

### Comparing `music-dragon-0.8/README.md` & `music-dragon-0.9/README.md`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/audioplayer.py` & `music-dragon-0.9/music_dragon/audioplayer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from music_dragon.log import debug
 import vlc
 
 _vlc_instance = vlc.Instance()
 media_player = _vlc_instance.media_player_new()
 
 def open_stream(url: str):
-    debug(f"Opening audio stream from url: {url}")
-    media_player.set_media(_vlc_instance.media_new(url))
+    debug(f"Opening audio stream at: {url}")
+    if url.startswith("http"):
+        media_player.set_media(_vlc_instance.media_new_location(url))
+    else:
+        media_player.set_media(_vlc_instance.media_new_path(url))
+
 
 def stream_is_open():
     return media_player.get_media() is not None
 
 def play():
     debug("PLAY")
     media_player.play()
```

### Comparing `music-dragon-0.8/music_dragon/localsongs.py` & `music-dragon-0.9/music_dragon/localsongs.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,107 +4,197 @@
 
 import eyed3
 from PyQt5.QtCore import pyqtSignal
 from eyed3.core import AudioFile
 
 from music_dragon import workers
 from music_dragon.log import debug
+from music_dragon.utils import crc32
 from music_dragon.workers import Worker
 
 MP3_IMAGE_TAG_INDEX_FRONT_COVER = 3
 
 mp3s_indexes_by_metadata = {}
 mp3s = []
 
 class Mp3:
     def __init__(self):
         # tag
-        self.length = None
         self.tag = None
+        self.length = None
         self.artist = None
         self.album = None
         self.song = None
         self.track_num = None
         self.image = None
+        self.image_path = None # only available if cached
+        self.size = None
+        self.year = None
 
         self.path: Optional[Path] = None
 
         #
         self.fetched_release_group = False
         self.release_group_id = None
 
         self.fetched_artist = False
         self.artist_id = None
 
         self.fetched_track = False
         self.track_id = None
 
+    def title(self):
+        if self.song:
+            return self.song
+        print(f"WARN: no song attribute for mp3 {self.path}")
+        return self.path.stem
+
     def load_from_file(self, file: str, load_image=True):
         p = Path(file)
 
         if not p.is_file():
             print(f"ERROR: cannot load file '{file}': not a file")
             return False
 
         if p.suffix != ".mp3":
             return False
 
         self.path = p.absolute()
+        self.tag = None
 
         try:
+            self.size = os.stat(self.path).st_size
+
             mp3: AudioFile = eyed3.load(self.path)
             if mp3:
                 if not mp3.tag:
                     print(f"WARN: no mp3 tag found for file '{file}', skipping")
                     return False
                 self.length = 1000 * mp3.info.time_secs
                 self.tag = mp3.tag
                 self.artist = mp3.tag.artist
                 self.album = mp3.tag.album
                 self.song = mp3.tag.title
-                self.track_num = mp3.tag.track_num
+                self.track_num = mp3.tag.track_num[0]
+                try:
+                    self.year = mp3.tag.getBestDate().year
+                except:
+                    pass
+
                 if load_image:
                     self._load_image_from_tag()
 
                 debug(f"Loaded {self.path}: "
-                      f"(artist={self.artist}, album={self.album}, "
-                      f"title={self.album}, image={'yes' if self.image else 'no'})")
+                      f"(artist={self.artist}, "
+                      f"album={self.album}, "
+                      f"title={self.song}, "
+                      f"year={self.year}, "
+                      f"track_num={self.track_num}, "
+                      f"image={'yes' if self.image else 'no'})")
                 return True
         except Exception as e:
             print(f"WARN: failed to load mp3 from '{file}': {e}")
 
         return False
 
+    def load_from_info(self, info: dict, load_image=True):
+        self.size = info.get("size")
+        self.path = Path(info.get("path"))
+        self.length = info.get("length")
+        self.artist = info.get("artist")
+        self.album = info.get("album")
+        self.song = info.get("song")
+        self.track_num = info.get("track_num")
+        self.year = info.get("year")
+        self.image_path = info.get("image")
+        self.tag = None
+
+        if load_image:
+            if self.image_path:
+                self._load_image_from_path(self.image_path)
+
+                debug(f"Loaded [cached] {self.path}: "
+                      f"(artist={self.artist}, "
+                      f"album={self.album}, "
+                      f"title={self.song}, "
+                      f"year={self.year}, "
+                      f"track_num={self.track_num}, "
+                      f"image={'yes' if self.image else 'no'})")
+
+        return True
+
+
+    def load_image(self):
+        if self.image:
+            return
+
+        if self.image_path is not None:
+            self._load_image_from_path(self.image_path)
+        else:
+            self._load_image_from_tag()
+
+
     def _load_image_from_tag(self):
+        # Eventually load tag
+        if not self.tag:
+            try:
+                mp3: AudioFile = eyed3.load(self.path)
+                if mp3:
+                    self.tag = mp3.tag
+            except Exception as e:
+                print(f"WARN: failed to load mp3 from '{self.path}': {e}")
+
+        if not self.tag:
+            print(f"WARN: no tag for mp3 {self.path}")
+            return
+
         for img in self.tag.images:
             if img.picture_type == MP3_IMAGE_TAG_INDEX_FRONT_COVER:
                 self.image = img.image_data
                 debug(f"Loaded image of {self}")
 
+
+    def _load_image_from_path(self, image_path):
+        with Path(image_path).open("rb") as img:
+            self.image = img.read()
+            debug(f"Loaded [cached] image of {self}")
+
+
     def __str__(self):
         return f"{self.artist} - {self.album} - {self.song}"
 
 
-def get_by_metadata(artist: str, album: str, song: str):
+def get_by_metadata(artist: str, album: str, song: str) -> Optional[Mp3]:
     idx = mp3s_indexes_by_metadata.get((artist, album, song))
     debug(f"Checking availability of ({artist}, {album}, {song})")
     if idx is not None and 0 <= idx < len(mp3s):
         debug("-> found")
         return mp3s[idx]
+    else:
+        debug("-> not found")
     return None
 
+
 def load_mp3(file: str, load_image=True):
     mp3: Mp3 = Mp3()
     if mp3.load_from_file(file, load_image=load_image):
-        mp3s_indexes_by_metadata[(mp3.artist, mp3.album, mp3.song)] = len(mp3s)
+        mp3s_indexes_by_metadata[(mp3.artist, mp3.album, mp3.title())] = len(mp3s)
         mp3s.append(mp3)
         return mp3
     return None
 
-def load_mp3s(directory: str, load_images=True, mp3_loaded_callback=None):
+def load_mp3_from_info(mp3_info: dict, load_image=True):
+    mp3: Mp3 = Mp3()
+    if mp3.load_from_info(mp3_info, load_image=load_image):
+        mp3s_indexes_by_metadata[(mp3.artist, mp3.album, mp3.title())] = len(mp3s)
+        mp3s.append(mp3)
+        return mp3
+    return None
+
+def load_mp3s(directory: str, info=None, load_images=True, mp3_loaded_callback=None):
     root = Path(directory)
     if not root.exists():
         print(f"WARN: cannot load mp3s from directory '{directory}': does not exist")
         return
     if not root.is_dir():
         print(f"WARN: cannot load mp3s from directory '{directory}': not a directory")
         return
@@ -112,58 +202,78 @@
     file_count = 0
     loaded_file_count = 0
     for root, dirs, files in os.walk(str(root.absolute()), topdown=False):
         for file in files:
             if not file.endswith(".mp3"):
                 continue # skip non mp3
             file_count += 1
-            mp3 = load_mp3(os.path.join(root, file), load_image=load_images)
+
+            full_path = os.path.join(root, file)
+
+            mp3 = None
+
+            # check whether we already know this file
+            if info and full_path in info:
+                mp3_info =  info[full_path]
+                stat = os.stat(full_path)
+                # TODO: md5, crc32 would be more reliable
+                if mp3_info.get("size", 0) == stat.st_size:
+                    mp3 = load_mp3_from_info(mp3_info)
+
+            if not mp3:
+                mp3 = load_mp3(full_path, load_image=load_images)
+
             if mp3:
                 loaded_file_count += 1
                 if callable(mp3_loaded_callback):
                     mp3_loaded_callback(mp3)
+
     debug(f"Loaded {loaded_file_count}/{file_count} mp3 files")
 
 def clear_mp3s():
     mp3s_indexes_by_metadata.clear()
     mp3s.clear()
 
 # ============ LOAD MP3s  ===============
 # Load mp3s and their tags from directory
 # =======================================
 
 class LoadMp3sWorker(Worker):
     mp3_loaded = pyqtSignal(Mp3)
 
-    def __init__(self, directory: str, load_images):
+    def __init__(self, directory: str, info: dict, load_images):
         super().__init__()
         self.directory = directory
+        self.info = info
         self.load_images = load_images
 
     def run(self):
         # Fetch all the releases and releases tracks for the release groups
         debug(f"LOCALSONGS: load_mp3s: '{self.directory}'")
 
-        load_mp3s(self.directory, mp3_loaded_callback=self._on_mp3_loaded, load_images=self.load_images)
+        load_mp3s(self.directory, info=self.info, mp3_loaded_callback=self._on_mp3_loaded, load_images=self.load_images)
         # TODO: sort?
 
     def _on_mp3_loaded(self, mp3: Mp3):
         self.mp3_loaded.emit(mp3)
 
 
-def load_mp3s_background(directory, mp3_loaded_callback=None, finished_callback=None,
+def load_mp3s_background(directory,
+                         info: dict=None,
+                         mp3_loaded_callback=None, finished_callback=None,
                          load_images=True, priority=workers.Worker.PRIORITY_BELOW_NORMAL):
-    worker = LoadMp3sWorker(directory, load_images=load_images)
+    worker = LoadMp3sWorker(directory, info=info, load_images=load_images)
     worker.priority = priority
     if mp3_loaded_callback:
         worker.mp3_loaded.connect(mp3_loaded_callback)
     if finished_callback:
         worker.finished.connect(lambda: finished_callback(load_images))
     workers.schedule(worker)
 
+
 # ============ LOAD MP3  ===============
 # Load mp3 and its tags from file
 # =======================================
 
 class LoadMp3Worker(Worker):
     mp3_loaded = pyqtSignal(Mp3)
 
@@ -199,15 +309,15 @@
     def __init__(self):
         super().__init__()
 
     def run(self):
         debug(f"LOCALSONGS: load_mp3s_images: ({len(mp3s)})")
 
         for mp3 in mp3s:
-            mp3._load_image_from_tag()
+            mp3.load_image()
             self.mp3_image_loaded.emit(mp3)
 
 
 def load_mp3s_images_background(
         mp3_image_loaded_callback=None, finished_callback=None,
         priority=workers.Worker.PRIORITY_LOW):
     worker = LoadMp3sImagesWorker()
```

### Comparing `music-dragon-0.8/music_dragon/log.py` & `music-dragon-0.9/music_dragon/log.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/musicbrainz.py` & `music-dragon-0.9/music_dragon/musicbrainz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import musicbrainzngs as mb
 from PyQt5.QtCore import pyqtSignal
 
 from music_dragon import workers, APP_DISPLAY_NAME, APP_VERSION
 from music_dragon.log import debug
 from music_dragon.utils import j
 from music_dragon.workers import Worker
-
+from musicbrainzngs import musicbrainz
 
 def initialize():
     mb.set_useragent(APP_DISPLAY_NAME, APP_VERSION)
 
 def release_belongs_to_official_album(mb_release: dict):
     # return mb_release.get("status", "").lower() == "official" and \
     return "release-group" in mb_release and release_group_is_official_album(mb_release["release-group"])
 
 def release_group_is_official_album(mb_release_group: dict):
     return "primary-type" in mb_release_group and mb_release_group.get("primary-type") in ["Album", "EP"] \
-           and ("secondary-type-list" not in mb_release_group or not mb_release_group.get("secondary-type-list"))
+           and ("secondary-type-list" not in mb_release_group or not mb_release_group["secondary-type-list"] or
+                (len(mb_release_group["secondary-type-list"]) == 1 and
+                 mb_release_group["secondary-type-list"][0] in ["Soundtrack"]))
 
 #
 # class MbTrack: # recording belonging to a release
 #     def __init__(self, mb_track=None, release_id=None):
 #         self.id = None
 #         self.title = None
 #         self.length = 0
@@ -99,15 +101,15 @@
 #
 #         self.artists = []
 #         self.releases = []
 #
 #         if mb_release_group:
 #             self.id: str = mb_release_group["id"]
 #             self.title: str = mb_release_group["title"]
-#             self.date = mb_release_group.get("first-release-date", "")
+#             self.date = mb_release_group.get("first-release-date", "9999-99-99")
 #             self.score: int = int(mb_release_group.get("ext-score", 0))
 #
 #
 #             if "artist-credit" in mb_release_group:
 #                 self.artists = [{
 #                     "id": artist_credit["artist"]["id"],
 #                     "name": artist_credit["artist"]["name"],
@@ -208,14 +210,15 @@
 
     def run(self):
         if not self.query:
             return
         debug(f"MUSICBRAINZ: search_release_groups: '{self.query}'")
         result = mb.search_release_groups(
             self.query, limit=self.limit, primarytype="Album", status="Official"
+            # self.query, limit=self.limit, primarytype="Album"
         )["release-group-list"]
         debug(
             "=== search_release_groups ==="
             f"{j(result)}"
             "======================"
         )
         # release_groups = [MbReleaseGroup(release_group) for release_group in result
@@ -396,27 +399,80 @@
         super().__init__()
         self.artist_id = artist_id
 
     def run(self):
         # Fetch all the releases and releases tracks for the release groups
         # result = mb.get_artist_by_id(self.artist_id, includes=["aliases", "release-groups", "url-rels", "annotation", "releases", "isrcs"])
         debug(f"MUSICBRAINZ: get_artist_by_id: '{self.artist_id}'")
+
+        # def get_artist_by_id_ext(id, includes=[], release_status=[], release_type=[], limit=25):
+        #     params = musicbrainz._check_filter_and_make_params("artist", includes,
+        #                                            release_status, release_type)
+        #     params["limit"] = limit
+        #     return musicbrainz._do_mb_query("artist", id, includes, params)
+
         result = mb.get_artist_by_id(
             self.artist_id,
-            includes=["aliases", "release-groups", "release-group-rels", "releases", "url-rels"],
-            release_status=["official"],
-            release_type=["album"],
+            # includes=["aliases", "release-groups", "release-group-rels", "releases", "url-rels"],
+            includes=["aliases", "release-groups", "release-group-rels", "url-rels"],
+            # release_status=["official"],
+            release_type=["album", "ep"],
         )["artist"]
         debug(
             "=== get_artist_by_id ==="
             f"{j(result)}"
             "======================"
         )
 
-        # self.result.emit(self.artist_id, MbArtist(result))
+        release_group_list = result["release-group-list"]
+        release_group_count = result["release-group-count"]
+
+        if len(release_group_list) < release_group_count:
+            debug("Too many release groups, browsing them...")
+
+            release_group_list = []
+            while len(release_group_list) < release_group_count:
+                offset = len(release_group_list)
+                # debug(f"browse_release_groups(artist={self.artist_id},offset={offset},limit={25}) [COUNT is {release_group_count}]")
+                # rgs_result = browse_release_groups(artist=self.artist_id,
+                #                         includes=["release-rels", "release-group-rels"],
+                #                         release_type=["album"],
+                #                         limit=25,
+                #                         offset=offset)
+                debug(f"search_release_groups(artist={self.artist_id},offset={offset},limit={25}) [COUNT is {release_group_count}]")
+
+                rgs_result = mb.search_release_groups(
+                    query="",
+                    limit=100,
+                    offset=offset,
+                    strict=True,
+                    arid=self.artist_id,
+                    primarytype="album",
+                    status="official"
+                )
+
+                debug(
+                    f"=== search_release_groups (offset={offset}) ==="
+                    f"{j(rgs_result)}"
+                    "======================"
+                )
+
+                release_group_list += rgs_result["release-group-list"]
+                release_group_count = rgs_result["release-group-count"]
+
+            release_group_list = sorted(release_group_list, key=lambda rg: rg.get("first-release-date", "9999-99-99"))
+            result["release-group-list"] = release_group_list
+
+        debug(
+            "=== get_artist_by_id EXTENDED ==="
+            f"{j(result)}"
+            "======================"
+        )
+
+
         self.result.emit(self.artist_id, result)
 
 def fetch_artist(artist_id, callback, priority=workers.Worker.PRIORITY_NORMAL):
     worker = FetchArtistWorker(artist_id)
     worker.priority = priority
     worker.result.connect(callback)
     workers.schedule(worker)
```

### Comparing `music-dragon-0.8/music_dragon/repository.py` & `music-dragon-0.9/music_dragon/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import json
 from difflib import get_close_matches
 from statistics import mean, multimode
-from typing import List, Dict, Optional, Union
+from typing import List, Dict, Optional, Union, Tuple
 
 import Levenshtein as levenshtein
 import requests
 
 from music_dragon import cache, localsongs, musicbrainz, preferences, wiki, workers, ytdownloader, ytmusic
 from music_dragon.localsongs import Mp3
 from music_dragon.log import debug
-from music_dragon.utils import Mergeable, min_index, stable_hash, normalize_metadata
+from music_dragon.utils import Mergeable, min_index, stable_hash, normalize_metadata, j, crc32
+from music_dragon.workers import Worker
 from music_dragon.ytmusic import YtTrack
 
 _artists: Dict[str, 'Artist'] = {}
 _release_groups: Dict[str, 'ReleaseGroup'] = {}
 _releases: Dict[str, 'Release'] = {}
 _tracks: Dict[str, 'Track'] = {}
 _youtube_tracks: Dict[str, 'YtTrack'] = {}
@@ -42,18 +44,23 @@
             if "release-group-list" in mb_artist:
                 for mb_rg in mb_artist["release-group-list"]:
                     if not musicbrainz.release_group_is_official_album(mb_rg):
                         debug(f"Skipping release group: {mb_rg['title']}")
                         continue
 
                     release_group = ReleaseGroup(mb_rg)
-                    # TODO: what if there is more than an artist?
-                    release_group.artist_ids.append(self.id)
+                    # TODO: dict/set?
+                    if self.id not in release_group.artist_ids:
+                        # TODO: what if there is more than an artist?
+                        release_group.artist_ids.append(self.id)
+
                     _add_release_group(release_group)
-                    self.release_group_ids.append(release_group.id)
+                    if release_group.id not in self.release_group_ids:
+                        self.release_group_ids.append(release_group.id)
+                self.release_group_ids = sorted(self.release_group_ids, key=lambda rgid: f"{get_release_group(rgid).year() or 9999}@{get_release_group(rgid).title}")
 
     def merge(self, other):
         # handle flags apart
         fetched = self.fetched or other.fetched
         fetched_image = self.fetched_image or other.fetched_image
         super().merge(other)
         self.fetched = fetched
@@ -84,21 +91,29 @@
         self.youtube_playlist_id = None
 
         if mb_release_group:
             self.id = mb_release_group["id"]
             self.title = normalize_metadata(mb_release_group["title"])
             self.date = mb_release_group.get("first-release-date", "")
             if "artist-credit" in mb_release_group:
+                # debug(f"mb_release_group['artist-credit'] len is {len(mb_release_group['artist-credit'])}")
+                # debug(f"self.artist_ids before is {self.artist_ids}")
                 for artist_credit in mb_release_group["artist-credit"]:
                     if not isinstance(artist_credit, dict):
                         continue
 
                     artist = Artist(artist_credit["artist"])
                     _add_artist(artist)
-                    self.artist_ids.append(artist.id)
+
+                    if artist.id not in self.artist_ids:
+                        self.artist_ids.append(artist.id)
+                    else:
+                        debug("WARN: duplicate artist id")
+
+                # debug(f"self.artist_ids after is {self.artist_ids}")
 
             if "release-list" in mb_release_group:
                 self.release_ids = [{
                     "id": release["id"],
                     "title": normalize_metadata(release["title"]),
                 } for release in mb_release_group["release-list"]]
 
@@ -169,22 +184,53 @@
         self.track_ids = []
         self.front_cover = None
         self.fetched_front_cover = False
 
         if mb_release:
             self.id = mb_release["id"]
             self.title = normalize_metadata(mb_release["title"]) # should match the release group title
-            if "format" in mb_release["medium-list"][0]:
+            # print(j(mb_release))
+            if mb_release["medium-list"] and "format" in mb_release["medium-list"][0]:
                 self.format = mb_release["medium-list"][0]["format"]
             self.release_group_id = mb_release["release-group"]["id"]
 
             track_names = {}
 
-            if len(mb_release["medium-list"][0]["track-list"]) == mb_release["medium-list"][0]["track-count"]:
+            if mb_release["medium-list"] and len(mb_release["medium-list"][0]["track-list"]) == mb_release["medium-list"][0]["track-count"]:
                 for mb_track in mb_release["medium-list"][0]["track-list"]:
+                    # expected
+                    # {
+                    #     "id": "896b4283-ff19-3b07-bb45-dced0f884a2f",
+                    #     "position": "11",
+                    #     "number": "11",
+                    #     "length": "217000",
+                    #     "recording": {
+                    #         "id": "81e4c357-3918-4c16-8a2a-80286759eec4",
+                    #         "title": "All Because of You",
+                    #         "length": "216236"
+                    #     },
+                    #     "track_or_recording_length": "217000"
+                    # },
+                    # found
+                    # {
+                    #     "id": "47793e9c-7c42-33e1-8bb9-47480b4e67d9",
+                    #     "number": "2",
+                    #     "title": "Shadow of the Moon",
+                    #     "length": "242466",
+                    #     "track_or_recording_length": "242466"
+                    # }
+                    if "recording" not in mb_track:
+                        mb_track["recording"] = {
+                            "id": mb_track["id"],
+                            "title": mb_track["title"],
+                            "length": mb_track.get("length", 0)
+                        }
+                    if "position" not in mb_track and "number" in mb_track:
+                        mb_track["position"] = mb_track["number"]
+
                     t = Track(mb_track, self.id)
                     if t.title not in track_names:
                         track_names[t.title] = 1
                     else:
                         track_names[t.title] += 1
                         print(f"WARN: found duplicate track title: '{t.title}', renaming it to '{t.title} ({track_names[t.title]})'")
                         t.title = f"{t.title} ({track_names[t.title]})"
@@ -224,19 +270,23 @@
         self.youtube_track_id = None
         self.fetched_youtube_track = False
         self.youtube_track_is_official = False
         self.downloading = False
         self.title_aliases = []
 
         if mb_track:
+            # print(f"MB_TRACK = {mb_track}")
+            # try:
             self.id = f'{mb_track["recording"]["id"]}@{release_id}'
             self.title = normalize_metadata(mb_track["recording"]["title"])
             self.length = int(mb_track["recording"].get("length", 0))
             self.track_number = int(mb_track["position"])
             self.release_id = release_id
+            # except:
+            #     print(f"WARN: invalid musicbrainz track: {mb_track}")
 
     def merge(self, other):
         # TODO: youtube_track_is_official is not handled well probably
         # handle flags apart
         fetched_youtube_track = self.fetched_youtube_track or other.fetched_youtube_track
         super().merge(other)
         self.fetched_youtube_track = fetched_youtube_track
@@ -254,14 +304,25 @@
             return True
         for alias in self.title_aliases:
             mp3 = localsongs.get_by_metadata(rg.artists_string(), rg.title, alias)
             if mp3:
                 return True
         return False
 
+    def get_local(self) -> Optional[Mp3]:
+        mp3, idx = self.get_local_ext()
+        return mp3
+
+    def get_local_ext(self) -> Tuple[Optional[Mp3], Optional[int]]:
+        rg = self.release().release_group()
+        idx = localsongs.mp3s_indexes_by_metadata.get((rg.artists_string(), rg.title, self.title))
+        if idx is not None:
+            return localsongs.mp3s[idx], idx
+        return None, None
+
 def _add_artist(artist: Artist):
     debug(f"add_artist({artist.id})")
 
     if  artist.id not in _artists:
         _artists[artist.id] = artist
     else:
         _artists[artist.id].merge(artist)
@@ -504,15 +565,15 @@
     else:
         if not mp3.album:
             print("WARN: no album for mp3")
             mp3.fetched_release_group = True
             # TODO: ... callback?
             return
 
-        def release_groups_callback_wrapper(query_, result: List[dict]):
+        def release_groups_callback_wrapper(_1, _2, result: List[dict]):
             if not cache_hit:
                 cache.put_request(request_name, result)
 
             release_groups = [ReleaseGroup(rg) for rg in result]
             for rg in release_groups:
                 _add_release_group(rg)
 
@@ -545,18 +606,18 @@
                     fetch_release_group_cover(best_release_group.id, mp3_release_group_image_callback)
 
 
         req = cache.get_request(request_name)
         if req:
             # storage cached
             cache_hit = True
-            release_groups_callback_wrapper(mp3.album, req)
+            release_groups_callback_wrapper(mp3.artist, mp3.album, req)
         else:
             # actually fetch
-            musicbrainz.search_release_groups(mp3.album, release_groups_callback_wrapper, limit=limit)
+            musicbrainz.search_release_group(mp3.artist, mp3.album, release_groups_callback_wrapper)
 
 
 def fetch_release_group_by_name(release_group_name: str, artist_name_hint: str, release_group_callback, release_group_image_callback):
     debug(f"fetch_mp3_release_group({release_group_name})")
     limit = 15
 
     request_name = f"mb-search-release-groups-{stable_hash(release_group_name)}-{limit}"
@@ -782,218 +843,33 @@
             # 2. Take the release with the number of track nearest to the mean
             # 3. Take the release with the number of track nearest to the mode
 
             request_name2 = f"ytmusic-search-youtube-album-{stable_hash(rg.artists_string())}-{stable_hash(rg.title)}"
             cache_hit2 = False
 
             def search_youtube_album_tracks_callback(_1, _2, album: dict):
-
-                yttracks = album.get("tracks", [])
-
-                # if len(yttracks) == 0:
-                #     return
-
                 if not cache_hit2:
                     cache.put_request(request_name2, album)
-                yttracks = [YtTrack(yttrack) for yttrack in yttracks]
-
-                _search_youtube_album_tracks_callback(_1, _2, album.get("audioPlaylistId"), yttracks)
-
-            def _search_youtube_album_tracks_callback(_1, _2, playlist_id, yttracks: List[YtTrack]):
-                if playlist_id:
-                    rg.fetched_youtube_video_ids = True
-                    rg.youtube_playlist_id = playlist_id
-                    rg.youtube_video_ids = [yt.id for yt in yttracks]
-
-                release_candidates = releases
-
-                releases_track_count = [r.track_count() for r in release_candidates]
-                yt_track_count = len(yttracks)
-                track_count_modes = multimode(releases_track_count)
-                track_count_mean = mean(releases_track_count)
-
-                debug(f"releases_track_count={releases_track_count}")
-                debug(f"mean_track_count={track_count_modes}")
-                debug(f"modes_track_count={track_count_mean}")
-
-                best_release_candidate = None
-
-                TRACK_NUMBER_FACTOR = 50
-                EDIT_DISTANCE_FACTOR = 1
-                TRACK_POSITION_DISTANCE_FACTOR = 5
-
-                def get_close_matches_smart(word, possibilities):
-                    res = get_close_matches(word, possibilities)
-                    for p in possibilities:
-                        if p in res:
-                            continue # already there
-                        debug(f"Smart check of {word} with {p}")
-                        p_ = p.lower()
-                        w_ = word.lower()
-                        if p_ in w_ or w_ in p_:
-                            debug("-> yes")
-                            res.insert(0, p)
-                    return res
-
-                def compute_track_yttrack_score(t_: Track, yt_: YtTrack):
-                    debug(f"compute_track_yttrack_score({t_.title}, {yt_.song})")
-
-                    # hack special characters
-                    t_title = t_.title.lower()
-                    yt_title = yt_.song.lower()
-
-                    t_title = t_title.replace("’", "'")
-                    yt_title = yt_title.replace("’", "'")
-
-                    t_title = t_title.replace("-", " ")
-                    yt_title = yt_title.replace("-", " ")
-
-                    t_title = t_title.replace("‐", " ")
-                    yt_title = yt_title.replace("‐", " ")
-
-                    t_title = t_title.replace("_", " ")
-                    yt_title = yt_title.replace("_", " ")
-
-                    if t_title in yt_.song or yt_title in t_title:
-                        edit_distance_component = 0
-                    else:
-                        edit_distance_component = levenshtein.distance(t_title, yt_title)
-
-                    track_position_component = 0
-                    if t_.track_number is not None and yt_.track_number is not None:
-                        track_position_component += abs(t_.track_number - yt_.track_number)
-
-                    edit_distance_component *= EDIT_DISTANCE_FACTOR
-                    track_position_component *= TRACK_POSITION_DISTANCE_FACTOR
-
-                    scr = edit_distance_component + track_position_component
-                    debug(
-                        f"-> {scr} (edit_distance={edit_distance_component} + track_pos={track_position_component}){' *************' if scr == 0 else ''}")
-                    return scr
-
-                if yt_track_count:
-                    debug(f"Taking main release with tracks more similar to youtube one = {yt_track_count}")
-
-                    def compute_release_score(r: Release):
-                        debug(f"Computing release score of {r.title} ({r.id}): {r.track_count()} tracks)")
-
-                        # 1. Same number of track is better
-                        # 2. Consider edit distance between the tracks
-                        # 3. Consider the difference between the position of the tracks
-
-                        debug("")
-                        release_score = abs(r.track_count() - len(yttracks)) * TRACK_NUMBER_FACTOR
-                        debug(f"ReleaseScore after track number counting: {release_score}")
-
-                        # compute score based on tracks similarity
-                        for t in r.tracks():
-                            best_yt_track_score = min([compute_track_yttrack_score(t, y) for y in yttracks])
-                            release_score += best_yt_track_score
-                            debug(f"Score now is {release_score}")
 
-                        debug(f"Computed release score of {r.title} ({r.id}) = {release_score}")
-
-                        return release_score
-
-                    scores = [compute_release_score(r) for r in release_candidates]
-
-                    for i, sc in enumerate(scores):
-                        rc = release_candidates[i]
-                        debug(
-                            f"Release candidate {rc.title} ({rc.id}) with {release_candidates[i].track_count()} tracks has score = {sc}")
-
-                    best_release_candidate = release_candidates[min_index(scores)]
-
-                    if min(scores) > 0:
-                        print(
-                            f"WARN: youtube release does not match perfectly musicbrainz release (off by {min(scores)} points)")
-                    else:
-                        debug(f"Youtube release does match perfectly musicbrainz release")
-                else:
-                    # fallback: no youtube available
-
-                    # consider only CDs, if possible
-                    has_cds = [r.format == "CD" for r in releases].count(True) > 0
-
-                    release_candidates = []
-
-                    if has_cds:
-                        for r in releases:
-                            candidate = r.format == "CD"
-                            debug(
-                                f"Release: {r.title}, format={r.format}, track_count={r.track_count()}: candidate {candidate}")
-
-                            if candidate:
-                                release_candidates.append(r)
-                    else:
-                        release_candidates = releases
-
-                    if len(track_count_modes) == 1:
-                        # There is only a mode (there could be multiple), take a release with that mode
-                        track_count_mode = track_count_modes[0]
-                        debug(f"Taking main release with track count equal to the only mode = {track_count_mode}")
-                        for r in release_candidates:
-                            if r.track_count() == track_count_mode:
-                                best_release_candidate = r
-                                break
-                    else:
-                        # Fallback: take the release with the number of track nearest to the mean
-                        debug(f"Taking main release with track count nearest to mean = {track_count_mean}")
-                        mean_deltas = [abs(tc - track_count_mean) for tc in releases_track_count]
-                        best_release_candidate = release_candidates[min_index(mean_deltas)]
-
-                if best_release_candidate:
-                    debug(
-                        f"Best release candidate: {best_release_candidate.title} ({best_release_candidate.id}) with {best_release_candidate.track_count()} tracks")
-                    release_group.main_release_id = best_release_candidate.id
-
-                # Tag track with yttrack ids
-
-                tracks = release_group.main_release().tracks()
-                track_names = [t.title for t in tracks]
-
-                debug("Associating yttracks <===> tracks")
-                for yttrack_ in yttracks:
-                    yttrack = _add_youtube_track(yttrack_)
-
-                    # debug(f"Handling yttrack: {yttrack.song}")
-
-                    closest_track_names = get_close_matches_smart(yttrack.song, track_names)
-                    debug(f"closest_track_names={closest_track_names}")
-                    if closest_track_names:
-                        closest_tracks = []
-                        for closest_track_name in closest_track_names:
-                            for t in tracks:
-                                if t.title == closest_track_name:
-                                    closest_tracks.append(t)
-                        closest_tracks_scores = [compute_track_yttrack_score(t, yttrack) for t in closest_tracks]
-                        closest_track = closest_tracks[min_index(closest_tracks_scores)]
-                        # debug(f"Closest track found: {closest_track.title}")
-                        closest_track.fetched_youtube_track = True
-                        closest_track.youtube_track_is_official = True
-                        closest_track.youtube_track_id = yttrack.id
-                        # add the yt title as an alias
-                        if yttrack.song != closest_track.title and yttrack.song not in closest_track.title_aliases:
-                            closest_track.title_aliases.append(yttrack.song)
-                        # _track_id_by_video_id[yttrack.video_id] = closest_track.id
-                        debug(
-                            f"'{yttrack.song} (#{yttrack.track_number})' <==> '{closest_track.title} (#{closest_track.track_number})' (association score {min(closest_tracks_scores)})")
-                    else:
-                        print(f"WARN: no close track found for youtube track with title {yttrack.song}")
+                yttracks = album.get("tracks", [])
+                yttracks = [YtTrack(yttrack) for yttrack in yttracks]
 
-                release_group_releases_callback(release_group_id_, releases)
+                _set_release_group_tracks(release_group_id_, album.get("audioPlaylistId"), yttracks,
+                                          release_group_releases_callback, release_group_youtube_tracks_callback)
+                # _search_youtube_album_tracks_callback(_1, _2, album.get("audioPlaylistId"), yttracks)
 
-                if release_group_youtube_tracks_callback:
-                    release_group_youtube_tracks_callback(release_group_id_, yttracks)
 
             if rg.fetched_youtube_video_ids:
                 # memory cached
                 debug("Video ids already fetched")
-                _search_youtube_album_tracks_callback(None, None, rg.youtube_playlist_id,
-                                                     [get_youtube_track(video_id) for video_id in rg.youtube_video_ids])
+                _set_release_group_tracks(release_group_id_, rg.youtube_playlist_id,
+                                          [get_youtube_track(video_id) for video_id in rg.youtube_video_ids],
+                                          release_group_releases_callback, release_group_youtube_tracks_callback)
+                # _search_youtube_album_tracks_callback(None, None, rg.youtube_playlist_id,
+                #                                      [get_youtube_track(video_id) for video_id in rg.youtube_video_ids])
             else:
                 req2 = cache.get_request(request_name2)
                 if req2:
                     # storage cached
                     cache_hit2 = True
                     search_youtube_album_tracks_callback(rg.artists_string(), rg.title, req2)
                 else:
@@ -1103,14 +979,254 @@
                 release.front_cover = image
                 cache.put_image(f"{r_id}", image)
                 release_cover_callback(r_id, image)
 
             musicbrainz.fetch_release_cover(release_id, preferences.cover_size(), release_cover_callback_wrapper,
                                             priority=workers.Worker.PRIORITY_LOW)
 
+def set_release_group_playlist_id(release_group_id: str, playlist_id: str,
+                                  release_group_releases_callback, release_group_youtube_tracks_callback):
+    debug(f"set_release_group_playlist_id(release_group_id={release_group_id}, playlist_id={playlist_id})")
+
+    request_name = f"ytmusic-fetch-playlist-{stable_hash(playlist_id)}"
+    cache_hit = False
+
+    req = cache.get_request(request_name)
+
+    def release_group_youtube_tracks_callback_wrapper(playlist_id_, result: dict):
+        if not cache_hit:
+            cache.put_request(request_name, result)
+
+        yttracks = result.get("tracks", [])
+        yttracks = [YtTrack(yttrack) for yttrack in yttracks]
+
+        _set_release_group_tracks(release_group_id, playlist_id, yttracks,
+                                  release_group_releases_callback, release_group_youtube_tracks_callback)
+
+    if req:
+        # storage cached
+        cache_hit = True
+        release_group_youtube_tracks_callback_wrapper(playlist_id, req)
+    else:
+        # actually fetch
+        ytmusic.fetch_album_or_playlist_info(playlist_id, release_group_youtube_tracks_callback_wrapper)
+
+
+def _set_release_group_tracks(release_group_id, playlist_id, yttracks: List[YtTrack],
+                              release_group_releases_callback, release_group_youtube_tracks_callback):
+# def _set_release_group_tracks(_1, _2, playlist_id, yttracks: List[YtTrack]):
+    rg = get_release_group(release_group_id)
+
+    # if playlist_id:
+    rg.fetched_youtube_video_ids = True
+    rg.youtube_playlist_id = playlist_id
+    rg.youtube_video_ids = [yt.id for yt in yttracks]
+
+    releases = rg.releases()
+    release_candidates = rg.releases()
+
+    if not release_candidates:
+        print("WARN: no releases")
+        return
+
+    releases_track_count = [r.track_count() for r in release_candidates]
+    yt_track_count = len(yttracks)
+    track_count_modes = multimode(releases_track_count)
+    track_count_mean = mean(releases_track_count)
+
+    debug(f"releases_track_count={releases_track_count}")
+    debug(f"mean_track_count={track_count_modes}")
+    debug(f"modes_track_count={track_count_mean}")
+
+    best_release_candidate = None
+
+    TRACK_NUMBER_FACTOR = 50
+    EDIT_DISTANCE_FACTOR = 1
+    TRACK_POSITION_DISTANCE_FACTOR = 5
+
+    def get_close_matches_smart(word, possibilities):
+        res = get_close_matches(word, possibilities)
+        for p in possibilities:
+            if p in res:
+                continue  # already there
+            debug(f"Smart check of {word} with {p}")
+            p_ = p.lower()
+            w_ = word.lower()
+            if p_ in w_ or w_ in p_:
+                debug("-> yes")
+                res.insert(0, p)
+        return res
+
+    def compute_track_yttrack_score(t_: Track, yt_: YtTrack):
+        debug(f"compute_track_yttrack_score({t_.title}, {yt_.song})")
+
+        # hack special characters
+        t_title = t_.title.lower()
+        yt_title = yt_.song.lower()
+
+        t_title = t_title.replace("’", "'")
+        yt_title = yt_title.replace("’", "'")
+
+        t_title = t_title.replace("-", " ")
+        yt_title = yt_title.replace("-", " ")
+
+        t_title = t_title.replace("‐", " ")
+        yt_title = yt_title.replace("‐", " ")
+
+        t_title = t_title.replace("_", " ")
+        yt_title = yt_title.replace("_", " ")
+
+        if t_title in yt_.song or yt_title in t_title:
+            edit_distance_component = 0
+        else:
+            edit_distance_component = levenshtein.distance(t_title, yt_title)
+
+        track_position_component = 0
+        if t_.track_number is not None and yt_.track_number is not None:
+            track_position_component += abs(t_.track_number - yt_.track_number)
+
+        edit_distance_component *= EDIT_DISTANCE_FACTOR
+        track_position_component *= TRACK_POSITION_DISTANCE_FACTOR
+
+        scr = edit_distance_component + track_position_component
+        debug(
+            f"-> {scr} (edit_distance={edit_distance_component} + track_pos={track_position_component}){' *************' if scr == 0 else ''}")
+        return scr
+
+    if yt_track_count:
+        debug(f"Taking main release with tracks more similar to youtube one = {yt_track_count}")
+
+        def compute_release_score(r: Release):
+            debug(f"Computing release score of {r.title} ({r.id}): {r.track_count()} tracks)")
+
+            # 1. Same number of track is better
+            # 2. Consider edit distance between the tracks
+            # 3. Consider the difference between the position of the tracks
+
+            debug("")
+            release_score = abs(r.track_count() - len(yttracks)) * TRACK_NUMBER_FACTOR
+            debug(f"ReleaseScore after track number counting: {release_score}")
+
+            # compute score based on tracks similarity
+            for t in r.tracks():
+                best_yt_track_score = min([compute_track_yttrack_score(t, y) for y in yttracks])
+                release_score += best_yt_track_score
+                debug(f"Score now is {release_score}")
+
+            debug(f"Computed release score of {r.title} ({r.id}) = {release_score}")
+
+            return release_score
+
+        scores = [compute_release_score(r) for r in release_candidates]
+
+        for i, sc in enumerate(scores):
+            rc = release_candidates[i]
+            debug(
+                f"Release candidate {rc.title} ({rc.id}) with {release_candidates[i].track_count()} tracks has score = {sc}")
+
+        best_release_candidate = release_candidates[min_index(scores)]
+
+        if min(scores) > 0:
+            print(
+                f"WARN: youtube release does not match perfectly musicbrainz release (off by {min(scores)} points)")
+        else:
+            debug(f"Youtube release does match perfectly musicbrainz release")
+    else:
+        # fallback: no youtube available
+
+        # consider only CDs, if possible
+        has_cds = [r.format == "CD" for r in releases].count(True) > 0
+
+        release_candidates = []
+
+        if has_cds:
+            for r in releases:
+                candidate = r.format == "CD"
+                debug(
+                    f"Release: {r.title}, format={r.format}, track_count={r.track_count()}: candidate {candidate}")
+
+                if candidate:
+                    release_candidates.append(r)
+        else:
+            release_candidates = releases
+
+        if len(track_count_modes) == 1:
+            # There is only a mode (there could be multiple), take a release with that mode
+            track_count_mode = track_count_modes[0]
+            debug(f"Taking main release with track count equal to the only mode = {track_count_mode}")
+            for r in release_candidates:
+                if r.track_count() == track_count_mode:
+                    best_release_candidate = r
+                    break
+        else:
+            # Fallback: take the release with the number of track nearest to the mean
+            debug(f"Taking main release with track count nearest to mean = {track_count_mean}")
+            mean_deltas = [abs(tc - track_count_mean) for tc in releases_track_count]
+            best_release_candidate = release_candidates[min_index(mean_deltas)]
+
+    if best_release_candidate:
+        debug(
+            f"Best release candidate: {best_release_candidate.title} ({best_release_candidate.id}) with {best_release_candidate.track_count()} tracks")
+        rg.main_release_id = best_release_candidate.id
+
+    for track in rg.main_release().tracks():
+        track.youtube_track_id = None
+        track.youtube_track_is_official = False
+        track.fetched_youtube_track = False
+
+    # Tag track with yttrack ids
+
+    # tracks = release_group.main_release().tracks()
+    # track_names = [t.title for t in tracks]
+
+    # Greedy algorithm
+    remaining_tracks = set([t for t in rg.main_release().tracks()])
+    remaining_track_names = set([t.title for t in remaining_tracks])
+
+    debug(f"Associating yttracks <===> tracks for album {rg.title}")
+
+    for yttrack_ in yttracks:
+        yttrack = _add_youtube_track(yttrack_)
+        debug(f"YtTrack '{yttrack.song}' at position {yttrack.track_number}")
+
+        closest_track_names = get_close_matches_smart(yttrack.song, remaining_track_names)
+        debug(f"YtTrack '{yttrack.song}': closest_track_names={closest_track_names}")
+        if closest_track_names:
+            closest_tracks = []
+            for closest_track_name in closest_track_names:
+                for t in remaining_tracks:
+                    if t.title == closest_track_name:
+                        closest_tracks.append(t)
+            debug(f"YtTrack '{yttrack.song}': closest tracks: {[t.title for t in closest_tracks]}")
+            closest_tracks_scores = [compute_track_yttrack_score(t, yttrack) for t in closest_tracks]
+            closest_track = closest_tracks[min_index(closest_tracks_scores)]
+            debug(f"YtTrack '{yttrack.song}': closest track found: {closest_track.title}")
+
+            closest_track.fetched_youtube_track = True
+            closest_track.youtube_track_is_official = True
+            closest_track.youtube_track_id = yttrack.id
+
+            remaining_tracks.remove(closest_track)
+            remaining_track_names.remove(closest_track.title)
+
+            # add the yt title as an alias
+            if yttrack.song != closest_track.title and yttrack.song not in closest_track.title_aliases:
+                closest_track.title_aliases.append(yttrack.song)
+            # _track_id_by_video_id[yttrack.video_id] = closest_track.id
+            debug(
+                f"YtTrack '{yttrack.song} (#{yttrack.track_number})' <==> '{closest_track.title} (#{closest_track.track_number})' (association score {min(closest_tracks_scores)})")
+        else:
+            print(f"WARN: no close track found for youtube track with title {yttrack.song}")
+
+    release_group_releases_callback(release_group_id, releases)
+
+    if release_group_youtube_tracks_callback:
+        release_group_youtube_tracks_callback(release_group_id, yttracks)
+
+
 def search_track_youtube_track(track_id: str, track_youtube_track_callback):
     debug(f"search_track_youtube_track(track_id={track_id})")
 
     t = get_track(track_id)
     if t.fetched_youtube_track:
         # memory cached
         track_youtube_track_callback(track_id, t.youtube_track())
@@ -1171,15 +1287,16 @@
 
 
 
 
 
 def download_youtube_track_manual(video_id: str,
                            queued_callback, started_callback, progress_callback,
-                           finished_callback, canceled_callback, error_callback):
+                           finished_callback, canceled_callback, error_callback,
+                            track_number_hint: int=None):
     # TODO: fetch official from MB?
 
     # no cache needed here, since should be one shot
 
     def queued_callback_wrapper(down: dict):
         queued_callback(down)
 
@@ -1217,14 +1334,15 @@
 
 
         def best_yt_thumbnail(thumbs, preferred_size):
             if not thumbs:
                 return None
             # keep only square thumbs if there at least one
             debug("Choosing best yt thumbnail")
+            thumbs = [t for t in thumbs if "height" in t and "width" in t]
             at_least_one_squared = [t["width"] == t["height"] for t in thumbs].count(True) > 0
             filtered_thumbs =  [t for t in thumbs if t["width"] == t["height"]] if at_least_one_squared else thumbs
 
             preferred_area = preferred_size ** 2
             areas = [thumb["width"] * thumb["height"] for thumb in filtered_thumbs]
             deltas = [abs(preferred_area - a) for a in areas]
             thumb_idx = min_index(deltas)
@@ -1238,14 +1356,16 @@
         all_thumbnails = []
 
         yttrack = YtTrack(ytdownloader_result)
         if "videoDetails" in ytmusic_result and "title" in ytmusic_result["videoDetails"]:
             # heuristic: usually is better
             yttrack.song = ytmusic_result["videoDetails"]["title"]
 
+        if yttrack.track_number is None:
+            yttrack.track_number = track_number_hint
         _add_youtube_track(yttrack)
 
         # TODO: mb?
         # if mb_result:
         #     best_rg = mb_result[0]
         #     debug("Got MB result, using it?")
         #     pass
@@ -1277,28 +1397,29 @@
 
         ytdownloader.enqueue_track_download(
             video_id=video_id,
             artist=yttrack.artists[0],
             album=yttrack.album,
             song=yttrack.song,
             track_num=yttrack.track_number,
+            year=yttrack.year,
             image=best_cover,
-            output_directory=preferences.directory(),
-            output_format=preferences.output_format(),
+            output_directory=preferences.manual_download_directory(),
+            output_format=preferences.manual_output_format(),
             queued_callback=queued_callback_wrapper,
             started_callback=started_callback_wrapper,
             progress_callback=progress_callback_wrapper,
             finished_callback=finished_callback_wrapper,
             canceled_callback=canceled_callback_wrapper,
             error_callback=error_callback_wrapper,
             metadata=True,
             user_data={
-            "type": "manual",
-            "id": video_id
-        })
+                "type": "manual",
+                "id": video_id
+            })
 
     # def mb_release_group_result(artist_, album_, result):
     #     nonlocal mb_done, mb_result
     #
     #     mb_done = True
     #     mb_result = result
     #
@@ -1367,65 +1488,39 @@
     #     # track.downloading = False
     #     error_callback(down, error_msg)
 
     # track.downloading = True
     def playlist_info_result(playlist_id_, result, user_data):
         debug(f"playlist_info_result")
 
-        for entry in result["entries"]:
-            video_id = entry["id"]
-
-            download_youtube_track_manual(video_id,
-                                          queued_callback, started_callback, progress_callback,
-                                          finished_callback, canceled_callback, error_callback)
-            #
-            # # fetch image, eventually
-            # image = None
-            # if entry.get("thumbnails"):
-            #     preferred_area = preferences.cover_size() ** 2
-            #     areas = [thumb["width"] * thumb["height"] for thumb in entry["thumbnails"]]
-            #     deltas = [abs(preferred_area - a) for a in areas]
-            #     thumb_idx = min_index(deltas)
-            #     best_thumb = entry["thumbnails"][thumb_idx]
-            #
-            #     debug(f"Image will be retrieved from {best_thumb['url']}")
-            #     image = requests.get(best_thumb["url"], headers={
-            #         "User-Agent": "MusicDragonBot/1.0 (docheinstein@gmail.com) MusicDragon/1.0",
-            #     }).content
-            #     debug(f"Retrieved image data size: {len(image)}")
-            #
-            # yttrack = YtTrack(entry)
-            # _add_youtube_track(yttrack)
-            #
-            # ytdownloader.enqueue_track_download(
-            #     video_id=video_id,
-            #     artist=yttrack.artists[0],
-            #     album=yttrack.album,
-            #     song=yttrack.song,
-            #     track_num=yttrack.track_number,
-            #     image=image,
-            #     output_directory=preferences.directory(),
-            #     output_format=preferences.output_format(),
-            #     queued_callback=queued_callback_wrapper,
-            #     started_callback=started_callback_wrapper,
-            #     progress_callback=progress_callback_wrapper,
-            #     finished_callback=finished_callback_wrapper,
-            #     canceled_callback=canceled_callback_wrapper,
-            #     error_callback=error_callback_wrapper,
-            #     metadata=True,
-            #     user_data={
-            #     "type": "manual",
-            #     "id": video_id
-            # })
+        for track_num, entry in enumerate(result["entries"]):
+            try:
+                video_id = entry["id"]
+                download_youtube_track_manual(video_id,
+                                              queued_callback, started_callback, progress_callback,
+                                              finished_callback, canceled_callback, error_callback,
+                                              track_number_hint=track_num + 1)
+            except:
+                print(f"WARN: track {track_num} download failed")
 
     ytdownloader.fetch_playlist_info(
         playlist_id, playlist_info_result, user_data={}
     )
 
 
+def set_track_youtube_video_id(track_id: str, video_id: str):
+    debug(f"set_track_youtube_video_id(track_id={track_id}, video_id={video_id})")
+    track = get_track(track_id)
+    track.youtube_track_id = video_id
+    track.youtube_track_is_official = False
+    track.fetched_youtube_track = True
+    yttrack = YtTrack({})
+    yttrack.id = video_id
+    yttrack.video_id = video_id
+    _add_youtube_track(yttrack)
 
 def download_youtube_track(track_id: str,
                            queued_callback, started_callback, progress_callback,
                            finished_callback, canceled_callback, error_callback):
     track = get_track(track_id)
     rg = track.release().release_group()
 
@@ -1461,14 +1556,15 @@
     track.downloading = True
     ytdownloader.enqueue_track_download(
         video_id=track.youtube_track().video_id,
         artist=rg.artists_string(),
         album=rg.title,
         song=track.title,
         track_num=track.track_number,
+        year=rg.year(),
         image=rg.preferred_front_cover(),
         output_directory=preferences.directory(),
         output_format=preferences.output_format(),
         queued_callback=queued_callback_wrapper,
         started_callback=started_callback_wrapper,
         progress_callback=progress_callback_wrapper,
         finished_callback=finished_callback_wrapper,
@@ -1479,7 +1575,73 @@
             "type": "official",
             "id": track.id
         }
     )
 
 def cancel_youtube_track_download(video_id: str):
     ytdownloader.cancel_track_download(video_id)
+
+def load_mp3s(directory: str,
+              mp3_loaded_callback,
+              mp3_image_loaded_callback,
+              mp3s_loaded_callback,
+              mp3s_images_loaded_callback):
+
+    def update_localsongs_cache(*args, **kwargs):
+        debug("Computing local songs info...")
+        info = {}
+
+        for mp3 in localsongs.mp3s:
+            img_fingerprint_ = str(crc32(mp3.image)) if mp3.image else None
+
+            # Add info
+            info[str(mp3.path)] = {
+                "path": str(mp3.path),
+                "length": mp3.length,
+                "artist": mp3.artist,
+                "album": mp3.album,
+                "song": mp3.song,
+                "track_num": mp3.track_num,
+                "year": mp3.year,
+                "size": mp3.size,
+                "image_fingerprint": img_fingerprint_,
+            }
+
+            # Save image
+            if img_fingerprint_ is not None and not cache.has_file(img_fingerprint_):
+                cache.put_image(img_fingerprint_, mp3.image)
+
+        debug("Local songs info computed")
+        cache.put_localsongs(info)
+
+    def mp3s_images_loaded_callback_wrapper():
+        mp3s_images_loaded_callback()
+
+        # Update cache
+        workers.schedule_function(update_localsongs_cache)
+
+    def mp3s_loaded_callback_wrapper(_1):
+        mp3s_loaded_callback(_1)
+
+        # Load images
+        debug("Loading images now")
+        localsongs.load_mp3s_images_background(
+            mp3_image_loaded_callback=mp3_image_loaded_callback,
+            finished_callback=mp3s_images_loaded_callback_wrapper)
+
+    # Load local songs info
+    localsongs_info = cache.get_localsongs()
+
+    if localsongs_info:
+        # Link mp3s info with images
+        for _1, mp3_info in localsongs_info.items():
+            img_fingerprint = mp3_info.get("image_fingerprint")
+            if img_fingerprint is not None:
+                mp3_info["image"] = cache._cache_path / img_fingerprint
+
+    # Load mp3s from info
+    localsongs.load_mp3s_background(directory,
+                                    info=localsongs_info,
+                                    mp3_loaded_callback=mp3_loaded_callback,
+                                    finished_callback=mp3s_loaded_callback_wrapper,
+                                    load_images=False)
+
```

### Comparing `music-dragon-0.8/music_dragon/ui/albumtrackswidget.py` & `music-dragon-0.9/music_dragon/ui/albumtrackswidget.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 from music_dragon.log import debug
 from music_dragon.repository import Track, get_release, get_track, get_youtube_track
 from music_dragon.ui.listwidgetmodelview import ListWidgetModel, ListWidgetModelViewItem, ListWidgetModelView
 from music_dragon.utils import make_pixmap_from_data
 
 
 class AlbumTracksItemWidget(ListWidgetModelViewItem):
+    link_button_clicked = pyqtSignal(str)
     download_button_clicked = pyqtSignal(str)
     open_video_button_clicked = pyqtSignal(str)
 
     class Ui:
         def __init__(self):
             self.cover: Optional[QLabel] = None
             self.title: Optional[QLabel] = None
+            self.subtitle: Optional[QLabel] = None
+            self.link_button: Optional[QPushButton] = None
             self.download_button: Optional[QPushButton] = None
             self.open_video_button: Optional[QPushButton] = None
             self.download_progress: Optional[QProgressBar] = None
 
-    def __init__(self, track_id: str):
+    def __init__(self, track_id: str, show_youtube_titles=False):
         super().__init__(entry=track_id)
 
+        self.show_youtube_title = show_youtube_titles
         self.track_id = track_id
         self.track: Track = get_track(self.track_id)
         if not self.track:
             print(f"WARN: no track for id '{self.track_id}'")
             return
 
         self.ui = AlbumTracksItemWidget.Ui()
@@ -39,21 +43,42 @@
         self.invalidate()
 
 
     def setup(self):
         # cover
         self.ui.cover = QLabel()
         self.ui.cover.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
-        self.ui.cover.setMaximumSize(QSize(64, 64))
+        self.ui.cover.setMaximumSize(QSize(48, 48))
         self.ui.cover.setScaledContents(True)
 
         # title
         self.ui.title = QLabel()
         self.ui.title.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
-        self.ui.title.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
+
+        # subtitle
+        self.ui.subtitle = QLabel()
+        self.ui.subtitle.setVisible(True)
+        f = self.ui.subtitle.font()
+        f.setItalic(True)
+        f.setPointSize(f.pointSize() - 2)
+        self.ui.subtitle.setFont(f)
+        self.ui.subtitle.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
+
+        # download button
+        self.ui.link_button = QPushButton()
+        # self.ui.link_button.setVisible(False)
+        self.ui.link_button.setIcon(resources.LINK_ICON)
+        self.ui.link_button.setFlat(True)
+        self.ui.link_button.setCursor(Qt.PointingHandCursor)
+        self.ui.link_button.setIconSize(QSize(24, 24))
+        self.ui.link_button.setToolTip(f"Set YouTube URL")
+        self.ui.link_button.clicked.connect(self._on_link_button_clicked)
+        # szp = self.ui.link_button.sizePolicy()
+        # szp.setRetainSizeWhenHidden(True)
+        # self.ui.link_button.setSizePolicy(szp)
 
         # download button
         self.ui.download_button = QPushButton()
         self.ui.download_button.setVisible(False)
         self.ui.download_button.setIcon(resources.DOWNLOAD_ICON)
         self.ui.download_button.setFlat(True)
         self.ui.download_button.setCursor(Qt.PointingHandCursor)
@@ -88,18 +113,20 @@
         layout = QHBoxLayout()
         layout.setSpacing(4)
         layout.addWidget(self.ui.cover)
 
         inner_layout = QGridLayout()
         inner_layout.setContentsMargins(8, 0, 0, 0)
         inner_layout.addWidget(self.ui.title, 0, 0)
+        inner_layout.addWidget(self.ui.subtitle, 0, 0, alignment=Qt.AlignBottom)
         inner_layout.addWidget(self.ui.download_progress, 0, 0, alignment=Qt.AlignBottom)
         layout.addLayout(inner_layout)
 
 
+        layout.addWidget(self.ui.link_button)
         layout.addWidget(self.ui.open_video_button)
         layout.addWidget(self.ui.download_button)
 
         self.setLayout(layout)
 
     def invalidate(self):
         if self.track_id is None:
@@ -122,14 +149,17 @@
         self.ui.title.setText(self.track.title)
 
         # download
         youtube_track = get_youtube_track(self.track.youtube_track_id)
         download = ytdownloader.get_download(youtube_track.video_id) if youtube_track else None
 
         if youtube_track:
+            self.ui.subtitle.setText(youtube_track.video_title)
+            self.ui.subtitle.setVisible(True)
+
             self.ui.open_video_button.setVisible(True)
 
             if download and download["user_data"]["type"] == "official":
                 self.ui.download_progress.setVisible(download["status"] == "downloading")
                 self.ui.download_progress.setValue(round(download["progress"]))
 
                 self.ui.download_button.setVisible(False)
@@ -143,19 +173,28 @@
                     # self.ui.open_video_button.setVisible(False)
                 else:
                     self.ui.download_button.setVisible(True)
 
                     # self.ui.open_video_button.setVisible(True)
                     # self.ui.open_video_button.setToolTip(f"Open")
         else:
+            self.ui.subtitle.setVisible(False)
             self.ui.download_progress.setVisible(False)
             self.ui.download_button.setVisible(False)
             self.ui.open_video_button.setVisible(False)
 
+        if self.ui.download_progress.isVisible():
+            self.ui.subtitle.setVisible(False)
+
+        if not self.show_youtube_title:
+            self.ui.subtitle.setVisible(False)
 
+    def _on_link_button_clicked(self):
+        debug(f"_on_link_button_clicked({self._on_link_button_clicked})")
+        self.link_button_clicked.emit(self.track_id)
 
     def _on_download_button_clicked(self):
         debug(f"on_download_button_clicked({self.track_id})")
         self.download_button_clicked.emit(self.track_id)
 
     def _on_open_video_button_clicked(self):
         debug(f"on_open_video_button_clicked({self.track_id})")
@@ -171,88 +210,39 @@
         return release.track_ids if release else []
 
     def entry_count(self) -> int:
         release = get_release(self.release_id)
         return release.track_count() if release else 0
 
 class AlbumTracksWidget(ListWidgetModelView):
+    link_button_clicked = pyqtSignal(int)
     download_button_clicked = pyqtSignal(int)
     open_video_button_clicked = pyqtSignal(int)
 
     def __init__(self, parent=None):
         super().__init__(parent)
+        self.show_youtube_titles = False
+
+    def set_show_youtube_titles(self, show):
+        if show == self.show_youtube_titles:
+            return
+        self.show_youtube_titles = show
+        self.invalidate()
 
     def make_item_widget(self, entry) -> ListWidgetModelViewItem:
-        w = AlbumTracksItemWidget(entry)
+        w = AlbumTracksItemWidget(entry, self.show_youtube_titles)
+        w.link_button_clicked.connect(self._on_link_button_clicked)
         w.download_button_clicked.connect(self._on_download_button_clicked)
         w.open_video_button_clicked.connect(self._on_open_video_button_clicked)
         return w
 
+    def _on_link_button_clicked(self, entry: str):
+        row = self.model.index(entry)
+        self.link_button_clicked.emit(row)
+
     def _on_download_button_clicked(self, entry: str):
         row = self.model.index(entry)
         self.download_button_clicked.emit(row)
 
     def _on_open_video_button_clicked(self, entry: str):
         row = self.model.index(entry)
-        self.open_video_button_clicked.emit(row)
-
-    #
-    # def add_track(self, track: MbTrack):
-    #     self.tracks.append(track)
-    #
-    #     item = QListWidgetItem()
-    #     widget = AlbumTracksItemWidget(track)
-    #     widget.download_track_clicked.connect(self.on_download_track_clicked)
-    #     item.setSizeHint(widget.sizeHint())
-    #
-    #     self.addItem(item)
-    #     self.setItemWidget(item, widget)
-    #
-    # def set_cover(self, cover):
-    #     for idx, track in enumerate(self.tracks):
-    #         item = self.item(idx)
-    #         track_widget: AlbumTracksItemWidget = self.itemWidget(item)
-    #         if cover:
-    #             track_widget.ui.cover.setPixmap(make_pixmap_from_data(cover))
-    #         else:
-    #             track_widget.ui.cover.setPixmap(QPixmap(resources.DEFAULT_COVER_PLACEHOLDER_IMAGE_PATH))
-    #
-    # def set_youtube_track(self, mbtrack: MbTrack, yttrack: YtTrack):
-    #     for idx, track in enumerate(self.tracks):
-    #         if track.id == mbtrack.id:
-    #             item = self.item(idx)
-    #             track_widget: AlbumTracksItemWidget = self.itemWidget(item)
-    #
-    #             track.youtube_track = yttrack
-    #             track_widget.ui.download_button.setVisible(True)
-    #             track_widget.ui.download_button.setToolTip(f"Download {yttrack.video_title}  [{yttrack.video_id}]")
-    #
-    # def set_download_enabled(self, mbtrack: MbTrack, enabled):
-    #     for idx, track in enumerate(self.tracks):
-    #         if track.id == mbtrack.id:
-    #             item = self.item(idx)
-    #             track_widget: AlbumTracksItemWidget = self.itemWidget(item)
-    #
-    #             track_widget.ui.download_button.setVisible(enabled)
-    #
-    # def set_download_progress_visible(self, mbtrack: MbTrack, visibile):
-    #     for idx, track in enumerate(self.tracks):
-    #         if track.id == mbtrack.id:
-    #             item = self.item(idx)
-    #             track_widget: AlbumTracksItemWidget = self.itemWidget(item)
-    #
-    #             track_widget.ui.download_progress.setVisible(visibile)
-    #
-    # def set_download_progress(self, mbtrack: MbTrack, percentage: int):
-    #     for idx, track in enumerate(self.tracks):
-    #         if track.id == mbtrack.id:
-    #             item = self.item(idx)
-    #             track_widget: AlbumTracksItemWidget = self.itemWidget(item)
-    #
-    #             track_widget.ui.download_progress.setValue(percentage)
-    #
-    # def on_download_track_clicked(self, track: MbTrack):
-    #     self.download_track_clicked.emit(track)
-    #
-    # def on_item_clicked(self, item: QListWidgetItem):
-    #     debug(f"on_item_clicked at row {self.row(item)}")
-    #     self.row_clicked.emit(self.row(item))
+        self.open_video_button_clicked.emit(row)
```

### Comparing `music-dragon-0.8/music_dragon/ui/artistalbumswidget.py` & `music-dragon-0.9/music_dragon/ui/artistalbumswidget.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/ui/clickablelabel.py` & `music-dragon-0.9/music_dragon/ui/clickablelabel.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/ui/clickslider.py` & `music-dragon-0.9/music_dragon/ui/clickslider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from PyQt5.QtGui import QMouseEvent
 from PyQt5.QtWidgets import QSlider
 
+from music_dragon.log import debug
+
 
 class ClickSlider(QSlider):
 
     def __init__(self, parent):
         super().__init__(parent)
 
     def mouseReleaseEvent(self, e: QMouseEvent):
         e.accept()
         x = e.pos().x()
         value = int((self.maximum() - self.minimum()) * x / self.width() + self.minimum())
-        self.setValue(value, notify=True)
+        self.set_value(value, notify=True)
 
-    def setValue(self, value: int, notify: bool=True):
+    def set_value(self, value: int, notify: bool=True):
+        debug(f"set_value({value})")
+        if self.value() == value:
+            return
         was_blocked = False
         if not notify:
             was_blocked = self.blockSignals(True)
-        super().setValue(value)
+        self.setValue(value)
         if not notify:
             self.blockSignals(was_blocked)
+
```

### Comparing `music-dragon-0.8/music_dragon/ui/downloadswidget.py` & `music-dragon-0.9/music_dragon/ui/downloadswidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional
 
 from PyQt5.QtCore import QSize, Qt, pyqtSignal
 from PyQt5.QtWidgets import QLabel, QSizePolicy, QHBoxLayout, QGridLayout, QProgressBar, QPushButton, QVBoxLayout, \
     QSpacerItem
 
-from music_dragon import ytdownloader
+from music_dragon import ytdownloader, UNKNOWN_ARTIST, UNKNOWN_ALBUM
 from music_dragon.log import debug
 from music_dragon.repository import get_track, get_youtube_track
 from music_dragon.ui import resources
 from music_dragon.ui.clickablelabel import ClickableLabel
 from music_dragon.ui.listwidgetmodelview import ListWidgetModelView, ListWidgetModelViewItem, ListWidgetModel
 from music_dragon.utils import make_pixmap_from_data
 
@@ -151,27 +151,34 @@
         # cover
         self.ui.cover.setPixmap(make_pixmap_from_data(cover, default=resources.COVER_PLACEHOLDER_PIXMAP))
 
         # title
         self.ui.artist.setVisible(True)
         self.ui.title.setText(title)
 
-        # artist
-        if artist:
-            self.ui.artist.setVisible(True)
-            self.ui.artist.setText(artist)
-        else:
-            self.ui.artist.setVisible(False)
+        # # artist
+        # if artist:
+        #     self.ui.artist.setVisible(True)
+        #     self.ui.artist.setText(artist)
+        # else:
+        #     self.ui.artist.setVisible(False)
+        #
+        # # album
+        # if artist:
+        #     self.ui.album.setVisible(True)
+        #     self.ui.album.setText(album)
+        # else:
+        #     self.ui.album.setVisible(False)
+
+        self.ui.artist.setVisible(True)
+        self.ui.artist.setText(artist or UNKNOWN_ARTIST)
+
+        self.ui.album.setVisible(True)
+        self.ui.album.setText(album or UNKNOWN_ALBUM)
 
-        # album
-        if artist:
-            self.ui.album.setVisible(True)
-            self.ui.album.setText(album)
-        else:
-            self.ui.album.setVisible(False)
 
         # error
         if self.download:
             if self.download["status"] == "queued":
                 self.ui.download_progress.setVisible(False)
                 self.ui.download_error.setVisible(False)
                 self.ui.cancel_button.setVisible(True)
```

### Comparing `music-dragon-0.8/music_dragon/ui/imagepreviewwindow.py` & `music-dragon-0.9/music_dragon/ui/imagepreviewwindow.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,19 @@
         self.ui = Ui_ImagePreviewWindow()
         self.ui.setupUi(self)
 
         self.ui.saveButton.clicked.connect(self._on_save_button_clicked)
 
     def set_image(self, image: bytes):
         debug("Setting preview image")
-        self.image = image
-        self.ui.image.setPixmap(make_pixmap_from_data(image))
+        if image:
+            self.image = image
+            self.ui.image.setPixmap(make_pixmap_from_data(image))
+        else:
+            print("WARN: no image to show")
 
     def _on_save_button_clicked(self):
         directory_picker = QFileDialog()
 
         result = directory_picker.getSaveFileName(self, "Save file", "", "")
         if result:
             filename = result[0]
```

### Comparing `music-dragon-0.8/music_dragon/ui/listwidgetmodelview.py` & `music-dragon-0.9/music_dragon/ui/listwidgetmodelview.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,16 @@
         widget: ListWidgetModelViewItem = self.itemWidget(item)
         if widget:
             widget.invalidate()
         else:
             print(f"WARN: no widget at index {idx}")
 
     def add_row(self, entry: Any):
-        debug(f"{type(self).__name__}.add_row({entry})")
+        # debug(f"{type(self).__name__}.add_row({entry})")
+        debug(f"{type(self).__name__}.add_row")
         item = QListWidgetItem()
         widget = self.make_item_widget(entry)
         item.setSizeHint(widget.sizeHint())
 
         self.addItem(item)
         self.setItemWidget(item, widget)
```

### Comparing `music-dragon-0.8/music_dragon/ui/localalbumsview.py` & `music-dragon-0.9/music_dragon/ui/localalbumsview.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from typing import Any, Optional
 
-from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QModelIndex, QAbstractListModel, QVariant, pyqtSignal
+from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QModelIndex, QAbstractListModel, QVariant, pyqtSignal, \
+    QSortFilterProxyModel
 from PyQt5.QtGui import QPainter, QMouseEvent
 from PyQt5.QtWidgets import QStyledItemDelegate, QWidget, QLabel, QSizePolicy, QHBoxLayout, QVBoxLayout, QSpacerItem, \
     QGridLayout, QListView
 
-from music_dragon import localsongs
+from music_dragon import localsongs, UNKNOWN_ALBUM, UNKNOWN_ARTIST
+from music_dragon.localsongs import Mp3
 from music_dragon.log import debug
 from music_dragon.ui import resources
 from music_dragon.ui.clickablelabel import ClickableLabel
+from music_dragon.ui.listproxyview import ListProxyView
 from music_dragon.utils import make_icon_from_data
 
-
 class LocalAlbumsItemRole:
     TITLE = Qt.DisplayRole
     IMAGE = Qt.DecorationRole
     ARTIST = Qt.UserRole
 
 
 class LocalAlbumsItemWidget(QWidget):
-    artist_clicked = pyqtSignal(int)
-    album_clicked = pyqtSignal(int)
+    artist_clicked = pyqtSignal(QModelIndex)
+    album_clicked = pyqtSignal(QModelIndex)
 
     class Ui:
         def __init__(self):
             self.cover: Optional[QLabel] = None
             self.title: Optional[QLabel] = None
             self.artist: Optional[QLabel] = None
 
-    def __init__(self, parent, row, title, artist, image):
+    def __init__(self, parent, index, title, artist, image):
         super().__init__(parent)
 
-        self.row = row
+        self.index = index
         self.title = title
         self.artist = artist
         self.image = image
 
         self.ui = LocalAlbumsItemWidget.Ui()
         self.setup()
         self.setAutoFillBackground(True)
@@ -90,24 +92,29 @@
         self.ui.title.setText(self.title)
 
         # artist
         self.ui.artist.setText(self.artist)
 
     def _on_artist_clicked(self):
         debug(f"_on_artist_clicked({self.artist})")
-        self.artist_clicked.emit(self.row)
+        self.artist_clicked.emit(self.index)
 
     def sizeHint(self) -> QSize:
         sz = super().sizeHint()
         return QSize(sz.width(), 48)
 
 
 class LocalAlbumsItemDelegate(QStyledItemDelegate):
     artist_clicked = pyqtSignal(int)
 
+    def __init__(self, proxy: Optional[QSortFilterProxyModel] = None):
+        super().__init__()
+        self.proxy = proxy
+
+
     def paint(self, painter: QPainter, option: 'QStyleOptionViewItem', index: QModelIndex) -> None:
         ICON_TO_TEXT_SPACING = 9
 
         painter.save()
 
         title: str = index.data(LocalAlbumsItemRole.TITLE)
         artist: str = index.data(LocalAlbumsItemRole.ARTIST)
@@ -150,44 +157,67 @@
 
     def createEditor(self, parent: QWidget, option: 'QStyleOptionViewItem', index: QModelIndex) -> QWidget:
         title: str = index.data(LocalAlbumsItemRole.TITLE)
         artist: str = index.data(LocalAlbumsItemRole.ARTIST)
         image: bytes = index.data(LocalAlbumsItemRole.IMAGE)
 
         debug(f"Create editor for row with (title={title}, artist={artist})")
-        editor = LocalAlbumsItemWidget(parent=parent, row=index.row(), title=title, artist=artist, image=image)
+        editor = LocalAlbumsItemWidget(parent=parent, index=index, title=title, artist=artist, image=image)
 
         editor.artist_clicked.connect(self._on_artist_clicked)
         editor.adjustSize()
         return editor
 
     def updateEditorGeometry(self, editor: QWidget, option: 'QStyleOptionViewItem', index: QModelIndex) -> None:
         # debug("updateEditorGeometry")
         rect = option.rect
         rect.setX(rect.x() + 48)
         rect.setY(rect.y())
         editor.setGeometry(rect)
 
-    def _on_artist_clicked(self, row: int):
+    def _on_artist_clicked(self, index: QModelIndex):
+        index = self.proxy.mapToSource(index) if self.proxy else index
+        row = index.row()
         debug(f"_on_artist_clicked at row {row}")
         self.artist_clicked.emit(row)
 
 
+class LocalAlbumsProxyModel(QSortFilterProxyModel):
+    def filterAcceptsRow(self, source_row: int, source_parent: QModelIndex) -> bool:
+        src = self.sourceModel()
+        index = src.index(source_row, 0, source_parent)
+        album = src.data(index, LocalAlbumsItemRole.TITLE)
+        artist = src.data(index, LocalAlbumsItemRole.ARTIST)
+        reg_exp = self.filterRegularExpression()
+        return reg_exp.match(album).hasMatch() or reg_exp.match(artist).hasMatch()
+
 class LocalAlbumsModel(QAbstractListModel):
     def __init__(self):
         super().__init__()
         self.localalbums = []
 
     def reload(self):
+        def is_better(m1: Mp3, m2: Mp3):
+            if m1.year and not m2.year:
+                return True
+            if m1.image and not m2.image:
+                return True
+            if m1.year and m2.year and m1.year < m2.year:
+                return True
+            return False
+
         mp3s_by_albums = {}
         for mp3 in localsongs.mp3s:
-            if mp3.album and (mp3.album not in mp3s_by_albums or not mp3s_by_albums[mp3.album].image):
+            if not mp3.album and (UNKNOWN_ALBUM not in mp3s_by_albums or is_better(mp3, mp3s_by_albums[UNKNOWN_ALBUM])):
+                mp3s_by_albums[UNKNOWN_ALBUM] = mp3
+            if mp3.album and (mp3.album not in mp3s_by_albums or is_better(mp3, mp3s_by_albums[mp3.album])):
                 mp3s_by_albums[mp3.album] = mp3
 
         self.localalbums = list(mp3s_by_albums.values())
+        self.localalbums = sorted(self.localalbums, key=lambda mp3: (mp3.album or "ZZZZZZZZZZZZZZZZZZZZZZZ").lower())
 
     def flags(self, index: QModelIndex) -> Qt.ItemFlags:
         return super().flags(index) | Qt.ItemIsEditable | Qt.ItemIsSelectable
 
     def rowCount(self, parent: QModelIndex = ...) -> int:
         return len(self.localalbums)
 
@@ -204,35 +234,35 @@
             return QVariant()
 
         mp3: localsongs.Mp3 = self.localalbums[row]
 
         if role == LocalAlbumsItemRole.TITLE:
             if mp3.album:
                 return mp3.album
-            return ""
+            return UNKNOWN_ALBUM
 
         if role == LocalAlbumsItemRole.ARTIST:
             if mp3.artist:
                 return mp3.artist
-            return ""
+            return UNKNOWN_ARTIST
 
         if role == LocalAlbumsItemRole.IMAGE:
             return mp3.image
 
         return QVariant()
 
     def update_row(self, row, roles=None):
         if row < 0 or row >= self.rowCount():
             return
 
         index = self.index(row)
 
         self.dataChanged.emit(index, index, roles or [])
 
-class LocalAlbumsView(QListView):
+class LocalAlbumsView(ListProxyView):
     row_clicked = pyqtSignal(int)
     row_double_clicked = pyqtSignal(int)
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.edit_index = None
         self.setMouseTracking(True)
@@ -248,11 +278,11 @@
         if self.edit_index and self.edit_index != index:
             self.closePersistentEditor(self.edit_index)
 
         self.edit_index = index
         self.openPersistentEditor(self.edit_index)
 
     def _on_item_clicked(self, idx: QModelIndex):
-        self.row_clicked.emit(idx.row())
+        self.row_clicked.emit(self._source_index(idx).row())
 
     def _on_item_double_clicked(self, idx: QModelIndex):
-        self.row_double_clicked.emit(idx.row())
+        self.row_double_clicked.emit(self._source_index(idx).row())
```

### Comparing `music-dragon-0.8/music_dragon/ui/localartistsview.py` & `music-dragon-0.9/music_dragon/ui/localartistsview.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Any
+from typing import Any, Optional
 
-from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QModelIndex, QAbstractListModel, QVariant, pyqtSignal
+from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QModelIndex, QAbstractListModel, QVariant, pyqtSignal, \
+    QSortFilterProxyModel
 from PyQt5.QtGui import QPainter
 from PyQt5.QtWidgets import QStyledItemDelegate, QListView
 
-from music_dragon import localsongs
+from music_dragon import localsongs, UNKNOWN_ARTIST
+from music_dragon.localsongs import Mp3
 from music_dragon.ui import resources
+from music_dragon.ui.listproxyview import ListProxyView
 from music_dragon.utils import make_icon_from_data
 
-
 class LocalArtistsItemRole:
     NAME = Qt.DisplayRole
     IMAGE = Qt.DecorationRole
 
 #
 # class LocalArtistsItemWidget(QWidget):
 #     artist_clicked = pyqtSignal(int)
@@ -124,14 +126,18 @@
 #         return QSize(sz.width(), 48)
 
 
 class LocalArtistsItemDelegate(QStyledItemDelegate):
     # clicked = pyqtSignal(int)
     # album_clicked = pyqtSignal(int)
 
+    def __init__(self, proxy: Optional[QSortFilterProxyModel] = None):
+        super().__init__()
+        self.proxy = proxy
+
     def paint(self, painter: QPainter, option: 'QStyleOptionViewItem', index: QModelIndex) -> None:
         ICON_TO_TEXT_SPACING = 9
 
         painter.save()
 
         name: str = index.data(LocalArtistsItemRole.NAME)
         image: bytes = index.data(LocalArtistsItemRole.IMAGE)
@@ -186,27 +192,42 @@
     #     debug(f"_on_artist_clicked at row {row}")
     #     self.artist_clicked.emit(row)
     #
     # def _on_album_clicked(self, row: int):
     #     debug(f"_on_album_clicked at row {row}")
     #     self.album_clicked.emit(row)
 
+class LocalArtistsProxyModel(QSortFilterProxyModel):
+    pass
 
 class LocalArtistsModel(QAbstractListModel):
     def __init__(self):
         super().__init__()
         self.localartists = []
 
     def reload(self):
+        def is_better(m1: Mp3, m2: Mp3):
+            if m1.year and not m2.year:
+                return True
+            if m1.image and not m2.image:
+                return True
+            if m1.year and m2.year and m1.year < m2.year:
+                return True
+            return False
+
         mp3s_by_artists = {}
         for mp3 in localsongs.mp3s:
-            if mp3.artist and (mp3.artist not in mp3s_by_artists or not mp3s_by_artists[mp3.artist].image):
+            if not mp3.artist and (UNKNOWN_ARTIST not in mp3s_by_artists or is_better(mp3, mp3s_by_artists[UNKNOWN_ARTIST])):
+                mp3s_by_artists[UNKNOWN_ARTIST] = mp3
+            if mp3.artist and (mp3.artist not in mp3s_by_artists or is_better(mp3, mp3s_by_artists[mp3.artist])):
                 mp3s_by_artists[mp3.artist] = mp3
 
+
         self.localartists = list(mp3s_by_artists.values())
+        self.localartists = sorted(self.localartists, key=lambda mp3: (mp3.artist or "ZZZZZZZZZZZZZZZZZZZZZZZ").lower())
 
     # def flags(self, index: QModelIndex) -> Qt.ItemFlags:
     #     return super().flags(index) | Qt.ItemIsEditable | Qt.ItemIsSelectable
 
     def rowCount(self, parent: QModelIndex = ...) -> int:
         return len(self.localartists)
 
@@ -222,30 +243,30 @@
         if row < 0 or row >= self.rowCount():
             return QVariant()
 
         mp3_group: localsongs.Mp3 = self.localartists[row]
         artist_name = mp3_group.artist
 
         if role == LocalArtistsItemRole.NAME:
-            return artist_name
+            return artist_name or UNKNOWN_ARTIST
 
         if role == LocalArtistsItemRole.IMAGE:
             return mp3_group.image
 
         return QVariant()
 
     def update_row(self, row, roles=None):
         if row < 0 or row >= self.rowCount():
             return
 
         index = self.index(row)
 
         self.dataChanged.emit(index, index, roles or [])
 
-class LocalArtistsView(QListView):
+class LocalArtistsView(ListProxyView):
     row_clicked = pyqtSignal(int)
     # row_double_clicked = pyqtSignal(int)
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.edit_index = None
         self.setMouseTracking(True)
@@ -261,11 +282,11 @@
     #     if self.edit_index and self.edit_index != index:
     #         self.closePersistentEditor(self.edit_index)
     #
     #     self.edit_index = index
     #     self.openPersistentEditor(self.edit_index)
 
     def _on_item_clicked(self, idx: QModelIndex):
-        self.row_clicked.emit(idx.row())
+        self.row_clicked.emit(self._source_index(idx).row())
 
     # def _on_item_double_clicked(self, idx: QModelIndex):
     #     self.row_double_clicked.emit(idx.row())
```

### Comparing `music-dragon-0.8/music_dragon/ui/localsongsview.py` & `music-dragon-0.9/music_dragon/ui/localsongsview.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from typing import Any, Optional
 
-from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QModelIndex, QAbstractListModel, QVariant, pyqtSignal
+from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QModelIndex, QAbstractListModel, QVariant, pyqtSignal, \
+    QSortFilterProxyModel
 from PyQt5.QtGui import QPainter, QMouseEvent
 from PyQt5.QtWidgets import QStyledItemDelegate, QWidget, QLabel, QSizePolicy, QHBoxLayout, QVBoxLayout, QSpacerItem, \
     QGridLayout, QListView
 
 from music_dragon import localsongs
 from music_dragon.log import debug
 from music_dragon.ui import resources
 from music_dragon.ui.clickablelabel import ClickableLabel
+from music_dragon.ui.listproxyview import ListProxyView
 from music_dragon.utils import make_icon_from_data
 
 
 class LocalSongsItemRole:
     SONG = Qt.DisplayRole
     IMAGE = Qt.DecorationRole
     ARTIST = Qt.UserRole
     ALBUM = Qt.UserRole + 1
 
 
 class LocalSongsItemWidget(QWidget):
-    artist_clicked = pyqtSignal(int)
-    album_clicked = pyqtSignal(int)
+    artist_clicked = pyqtSignal(QModelIndex)
+    album_clicked = pyqtSignal(QModelIndex)
 
     class Ui:
         def __init__(self):
             self.cover: Optional[QLabel] = None
             self.title: Optional[QLabel] = None
             self.dash: Optional[QLabel] = None
             self.artist: Optional[QLabel] = None
             self.album: Optional[QLabel] = None
             self.subtitle_widget: Optional[QWidget] = None
 
-    def __init__(self, parent, row, artist, album, song, image):
+    def __init__(self, parent, index, artist, album, song, image):
         super().__init__(parent)
 
-        self.row = row
+        self.index = index
         self.artist = artist
         self.album = album
         self.song = song
         self.image = image
 
         self.ui = LocalSongsItemWidget.Ui()
         self.setup()
@@ -138,29 +140,33 @@
         else:
             self.ui.subtitle_widget.setVisible(False)
             self.ui.dash.setVisible(False)
             self.ui.title.setAlignment(Qt.AlignLeft | Qt.AlignVCenter)
 
     def _on_artist_clicked(self):
         debug(f"_on_artist_clicked({self.artist})")
-        self.artist_clicked.emit(self.row)
+        self.artist_clicked.emit(self.index)
 
     def _on_album_clicked(self):
         debug(f"_on_album_clicked({self.album})")
-        self.album_clicked.emit(self.row)
+        self.album_clicked.emit(self.index)
 
     def sizeHint(self) -> QSize:
         sz = super().sizeHint()
         return QSize(sz.width(), 48)
 
 
 class LocalSongsItemDelegate(QStyledItemDelegate):
     artist_clicked = pyqtSignal(int)
     album_clicked = pyqtSignal(int)
 
+    def __init__(self, proxy: Optional[QSortFilterProxyModel] = None):
+        super().__init__()
+        self.proxy = proxy
+
     def paint(self, painter: QPainter, option: 'QStyleOptionViewItem', index: QModelIndex) -> None:
         ICON_TO_TEXT_SPACING = 9
 
         painter.save()
 
         song: str = index.data(LocalSongsItemRole.SONG)
         artist: str = index.data(LocalSongsItemRole.ARTIST)
@@ -219,60 +225,82 @@
     def createEditor(self, parent: QWidget, option: 'QStyleOptionViewItem', index: QModelIndex) -> QWidget:
         song: str = index.data(LocalSongsItemRole.SONG)
         artist: str = index.data(LocalSongsItemRole.ARTIST)
         album: str = index.data(LocalSongsItemRole.ALBUM)
         image: bytes = index.data(LocalSongsItemRole.IMAGE)
 
         debug(f"Create editor for row with (song={song}, artist={artist}, album={album})")
-        editor = LocalSongsItemWidget(parent=parent, row=index.row(), artist=artist, album=album, song=song, image=image)
+        editor = LocalSongsItemWidget(parent=parent, index=index, artist=artist, album=album, song=song, image=image)
 
         editor.artist_clicked.connect(self._on_artist_clicked)
         editor.album_clicked.connect(self._on_album_clicked)
         editor.adjustSize()
         return editor
 
     def updateEditorGeometry(self, editor: QWidget, option: 'QStyleOptionViewItem', index: QModelIndex) -> None:
         # debug("updateEditorGeometry")
         rect = option.rect
         rect.setX(rect.x() + 48)
         rect.setY(rect.y())
         editor.setGeometry(rect)
 
-    def _on_artist_clicked(self, row: int):
+    def _on_artist_clicked(self, index: QModelIndex):
+        index = self.proxy.mapToSource(index) if self.proxy else index
+        row = index.row()
         debug(f"_on_artist_clicked at row {row}")
         self.artist_clicked.emit(row)
 
-    def _on_album_clicked(self, row: int):
+    def _on_album_clicked(self, index: QModelIndex):
+        index = self.proxy.mapToSource(index) if self.proxy else index
+        row = index.row()
         debug(f"_on_album_clicked at row {row}")
         self.album_clicked.emit(row)
 
 
+class LocalSongsProxyModel(QSortFilterProxyModel):
+    def filterAcceptsRow(self, source_row: int, source_parent: QModelIndex) -> bool:
+        src = self.sourceModel()
+        index = src.index(source_row, 0, source_parent)
+        song = src.data(index, LocalSongsItemRole.SONG)
+        artist = src.data(index, LocalSongsItemRole.ARTIST)
+        album = src.data(index, LocalSongsItemRole.ALBUM)
+        reg_exp = self.filterRegularExpression()
+        return reg_exp.match(song).hasMatch() or reg_exp.match(artist).hasMatch() or reg_exp.match(album).hasMatch()
+
 class LocalSongsModel(QAbstractListModel):
     def __init__(self):
         super().__init__()
+        self.localsongs = []
+
+    def reload(self):
+        self.localsongs = [mp3 for mp3 in localsongs.mp3s]
+        self.localsongs = sorted(self.localsongs, key=lambda mp3: mp3.title().lower())
 
     def flags(self, index: QModelIndex) -> Qt.ItemFlags:
         return super().flags(index) | Qt.ItemIsEditable | Qt.ItemIsSelectable
 
     def rowCount(self, parent: QModelIndex = ...) -> int:
-        return len(localsongs.mp3s)
+        return len(self.localsongs)
+
+    def entry(self, row: int):
+        return self.localsongs[row]
 
     def data(self, index: QModelIndex, role: int = ...) -> Any:
         if not index.isValid():
             return QVariant()
 
         row = index.row()
 
         if row < 0 or row >= self.rowCount():
             return QVariant()
 
-        mp3 = localsongs.mp3s[row]
+        mp3 = self.localsongs[row]
 
         if role == LocalSongsItemRole.SONG:
-            return mp3.song or str(mp3.path)
+            return mp3.title()
 
         if role == LocalSongsItemRole.ARTIST:
             if mp3.artist:
                 return mp3.artist
             return ""
 
         if role == LocalSongsItemRole.ALBUM:
@@ -289,15 +317,15 @@
         if row < 0 or row >= self.rowCount():
             return
 
         index = self.index(row)
 
         self.dataChanged.emit(index, index, roles or [])
 
-class LocalSongsView(QListView):
+class LocalSongsView(ListProxyView):
     row_clicked = pyqtSignal(int)
     row_double_clicked = pyqtSignal(int)
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.edit_index = None
         self.setMouseTracking(True)
@@ -313,11 +341,11 @@
         if self.edit_index and self.edit_index != index:
             self.closePersistentEditor(self.edit_index)
 
         self.edit_index = index
         self.openPersistentEditor(self.edit_index)
 
     def _on_item_clicked(self, idx: QModelIndex):
-        self.row_clicked.emit(idx.row())
+        self.row_clicked.emit(self._source_index(idx).row())
 
     def _on_item_double_clicked(self, idx: QModelIndex):
-        self.row_double_clicked.emit(idx.row())
+        self.row_double_clicked.emit(self._source_index(idx).row())
```

### Comparing `music-dragon-0.8/music_dragon/ui/mainwindow.py` & `music-dragon-0.9/music_dragon/ui/mainwindow.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,55 @@
+import random
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import List, Union, Optional
 
-from PyQt5.QtCore import QTimer
-from PyQt5.QtGui import QFont, QMouseEvent
+from PyQt5.QtCore import QTimer, QSortFilterProxyModel, QRegularExpression
+from PyQt5.QtGui import QFont, QMouseEvent, QCloseEvent
 from PyQt5.QtWidgets import QMainWindow, QLabel, QMessageBox
-from music_dragon import localsongs, repository, workers, ytcommons, ytdownloader, preferences, audioplayer
+
+from music_dragon import localsongs, repository, workers, ytcommons, ytdownloader, preferences, audioplayer, cache, \
+    UNKNOWN_ARTIST, UNKNOWN_ALBUM
 from music_dragon.localsongs import Mp3
 from music_dragon.log import debug
 from music_dragon.repository import Artist, ReleaseGroup, Release, Track, get_artist, \
     get_release_group, get_entity, get_track, get_release, get_youtube_track
 from music_dragon.ui import resources
 from music_dragon.ui.albumtrackswidget import AlbumTracksModel
 from music_dragon.ui.artistalbumswidget import ArtistAlbumsModel
 from music_dragon.ui.downloadswidget import DownloadsModel, FinishedDownloadsModel
+from music_dragon.ui.editlinkwindow import EditLinkWindow
 from music_dragon.ui.imagepreviewwindow import ImagePreviewWindow
-from music_dragon.ui.localalbumsview import LocalAlbumsModel, LocalAlbumsItemDelegate
-from music_dragon.ui.localartistsview import LocalArtistsModel, LocalArtistsItemDelegate
-from music_dragon.ui.localsongsview import LocalSongsModel, LocalSongsItemDelegate
+from music_dragon.ui.localalbumsview import LocalAlbumsModel, LocalAlbumsItemDelegate, LocalAlbumsProxyModel
+from music_dragon.ui.localalbumtrackswidget import LocalAlbumTracksModel
+from music_dragon.ui.localartistalbumswidget import LocalArtistAlbumsModel
+from music_dragon.ui.localartistsview import LocalArtistsModel, LocalArtistsItemDelegate, LocalArtistsProxyModel
+from music_dragon.ui.localsongsview import LocalSongsModel, LocalSongsItemDelegate, LocalSongsProxyModel
 from music_dragon.ui.preferenceswindow import PreferencesWindow
 from music_dragon.ui.searchresultswidget import SearchResultsModel
 from music_dragon.ui.ui_mainwindow import Ui_MainWindow
 from music_dragon.utils import make_pixmap_from_data, open_url, open_folder, is_dark_mode, millis_to_long_string, \
     millis_to_short_string, rangify
+from music_dragon.ytcommons import youtube_playlist_id_to_youtube_url, youtube_url_to_playlist_id
 from music_dragon.ytmusic import YtTrack
 
 SEARCH_DEBOUNCE_MS = 800
 
 DOWNLOADS_TABS_QUEUED_INDEX = 0
 DOWNLOADS_TABS_COMPLETED_INDEX = 1
 
-# class Mp3PlayInfo:
-#     def __init__(self):
-#         self.mp3 = None
-#
-# class TrackPlayInfo:
-#     def __init__(self):
-#         self.track = None
+
+class PlayingInfo:
+    def __init__(self):
+        self.index = 0
+        self.queue: List[Union[Track, Mp3]] = []
+
+    def in_play(self) -> Optional[Union[Track, Mp3]]:
+        if 0 <= self.index < len(self.queue):
+            return self.queue[self.index]
+        return None
 
 class MainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
 
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
@@ -94,39 +104,94 @@
         self.ui.albumCover.double_clicked.connect(self.on_album_cover_double_clicked)
         self.ui.albumCover.set_clickable(False)
         self.ui.albumCover.set_double_clickable(True)
         self.album_cover_data = None
         self.ui.albumCoverPrevButton.clicked.connect(self.on_album_cover_prev_button_clicked)
         self.ui.albumCoverNextButton.clicked.connect(self.on_album_cover_next_button_clicked)
         self.album_change_cover_empty_image_callback = None
+        self.album_change_cover_initial_index = None
 
+        self.ui.albumTracks.link_button_clicked.connect(self.on_track_link_button_clicked)
         self.ui.albumTracks.download_button_clicked.connect(self.on_track_download_button_clicked)
         self.ui.albumTracks.open_video_button_clicked.connect(self.on_track_open_video_button_clicked)
         self.ui.albumTracks.row_double_clicked.connect(self.on_track_double_clicked)
         self.ui.albumDownloadAllButton.clicked.connect(self.on_download_missing_album_tracks_clicked)
+        self.ui.albumDownloadAllVerifiedCheck.stateChanged.connect(self.on_download_missing_album_tracks_verified_check_changed)
         self.ui.albumOpenButton.clicked.connect(self.on_open_album_button_clicked)
 
+        self.ui.albumLinkButton.clicked.connect(self.on_album_link_button_clicked)
+        self.ui.albumLinkOkButton.clicked.connect(self.on_album_link_ok_button_clicked)
+        self.ui.albumLinkCancelButton.clicked.connect(self.on_album_link_cancel_button_clicked)
+
+        self.ui.albumLinkButton.setVisible(True)
+        self.ui.albumLinkButton.setToolTip("Edit YouTube URL")
+        sz = self.ui.albumLinkContainer.sizePolicy()
+        sz.setRetainSizeWhenHidden(True)
+        self.ui.albumLinkContainer.setSizePolicy(sz)
+        self.ui.albumLinkContainer.setVisible(False)
+
+        self.ui.showYouTubeTitlesCheck.stateChanged.connect(self.on_show_album_tracks_youtube_titles_check_changed)
+
+        self.ui.albumOpenLocalButton.clicked.connect(self.on_album_open_local_button_clicked)
+
         # Artist
         self.current_artist_id = None
         self.artist_albums_model = ArtistAlbumsModel()
         self.ui.artistAlbums.set_model(self.artist_albums_model)
         self.ui.artistAlbums.row_clicked.connect(self.on_artist_album_clicked)
         self.ui.artistCover.double_clicked.connect(self.on_artist_image_double_clicked)
+        self.ui.artistCover.set_clickable(False)
+        self.ui.artistCover.set_double_clickable(True)
         self.artist_cover_data = None
 
+        self.ui.artistOpenLocalButton.clicked.connect(self.on_artist_open_local_button_clicked)
+
+        # Local Album
+        self.current_local_album_mp3_group_leader = None
+        self.local_album_tracks_model = LocalAlbumTracksModel()
+        self.ui.localAlbumTracks.set_model(self.local_album_tracks_model)
+        self.ui.localAlbumTracks.row_clicked.connect(self.on_local_album_track_clicked)
+
+        self.ui.localAlbumArtist.set_underline_on_hover(True)
+        self.ui.localAlbumArtist.clicked.connect(self.on_local_album_artist_clicked_2)
+
+        self.ui.localAlbumCover.double_clicked.connect(self.on_local_album_cover_double_clicked)
+        self.ui.localAlbumCover.set_clickable(False)
+        self.ui.localAlbumCover.set_double_clickable(True)
+        self.album_cover_data = None
+
+        self.ui.localAlbumTracks.row_double_clicked.connect(self.on_local_track_double_clicked)
+        self.ui.localAlbumOpenRemoteButton.clicked.connect(self.on_local_album_open_remote_button_clicked)
+        self.ui.localAlbumRandomPlayButton.clicked.connect(self.on_local_album_random_play_button_clicked)
+
+        # Local Artist
+        self.current_local_artist_mp3_group_leader = None
+
+        self.local_artist_albums_model = LocalArtistAlbumsModel()
+        self.ui.localArtistAlbums.set_model(self.local_artist_albums_model)
+        self.ui.localArtistAlbums.row_clicked.connect(self.on_local_artist_album_clicked)
+        self.ui.localArtistCover.double_clicked.connect(self.on_local_artist_image_double_clicked)
+        self.ui.localArtistCover.set_clickable(False)
+        self.ui.localArtistCover.set_double_clickable(True)
+
+        self.ui.localArtistOpenRemoteButton.clicked.connect(self.on_local_artist_open_remote_button_clicked)
+        self.ui.localArtistRandomPlayButton.clicked.connect(self.on_local_artist_random_play_button_clicked)
+
         # Menu
         self.ui.actionPreferences.triggered.connect(self.on_action_preferences)
+        self.ui.actionRefresh.triggered.connect(self.on_action_refresh)
         self.ui.actionReload.triggered.connect(self.on_action_reload)
 
-        # Queued ownloads
+        # Queued downloads
         self.downloads_model = DownloadsModel()
         self.ui.queuedDownloads.set_model(self.downloads_model)
         self.ui.queuedDownloads.cancel_button_clicked.connect(self.on_download_cancel_button_clicked)
         self.ui.queuedDownloads.artist_clicked.connect(self.on_download_artist_clicked)
         self.ui.queuedDownloads.album_clicked.connect(self.on_download_album_clicked)
+        self.ui.autoDownloadQueuedCheck.stateChanged.connect(self.on_auto_download_queued_check_changed)
 
         # Completed downloads
         self.finished_downloads_model = FinishedDownloadsModel()
         self.ui.finishedDownloads.set_model(self.finished_downloads_model)
         self.ui.finishedDownloads.artist_clicked.connect(self.on_finished_download_artist_clicked)
         self.ui.finishedDownloads.album_clicked.connect(self.on_finished_download_album_clicked)
         self.ui.finishedDownloads.row_double_clicked.connect(self.on_finished_download_double_clicked)
@@ -136,69 +201,94 @@
         # self.downloader = YtDownloader()
         # self.downloader.track_download_started.connect(self.on_track_download_started)
         # self.downloader.track_download_progress.connect(self.on_track_download_progress)
         # self.downloader.track_download_finished.connect(self.on_track_download_finished)
 
         # Local songs
         self.local_songs_model = LocalSongsModel()
-        self.local_songs_delegate = LocalSongsItemDelegate()
+        self.local_songs_proxy_model = LocalSongsProxyModel()
+        self.local_songs_proxy_model.setSourceModel(self.local_songs_model)
+        self.local_songs_proxy_model.setFilterCaseSensitivity(0)
+        self.local_songs_delegate = LocalSongsItemDelegate(self.local_songs_proxy_model)
         self.local_songs_delegate.artist_clicked.connect(self.on_local_song_artist_clicked)
         self.local_songs_delegate.album_clicked.connect(self.on_local_song_album_clicked)
         self.ui.localSongs.row_clicked.connect(self.on_local_song_clicked)
         self.ui.localSongs.row_double_clicked.connect(self.on_local_song_double_clicked)
         self.ui.localSongs.setSpacing(6)
-        self.ui.localSongs.setModel(self.local_songs_model)
+        self.ui.localSongs.setModel(self.local_songs_proxy_model)
         self.ui.localSongs.setItemDelegate(self.local_songs_delegate)
+        self.ui.localSongsFilter.textChanged.connect(self.on_local_songs_filter_changed)
 
         self.local_artists_model = LocalArtistsModel()
-        self.local_artists_delegate = LocalArtistsItemDelegate()
+        self.local_artists_proxy_model = LocalArtistsProxyModel()
+        self.local_artists_proxy_model.setSourceModel(self.local_artists_model)
+        self.local_artists_proxy_model.setFilterCaseSensitivity(0)
+        self.local_artists_delegate = LocalArtistsItemDelegate(self.local_artists_proxy_model)
         self.ui.localArtists.row_clicked.connect(self.on_local_artist_clicked)
         self.ui.localArtists.setSpacing(6)
-        self.ui.localArtists.setModel(self.local_artists_model)
+        self.ui.localArtists.setModel(self.local_artists_proxy_model)
         self.ui.localArtists.setItemDelegate(self.local_artists_delegate)
+        self.ui.localArtistsFilter.textChanged.connect(self.on_local_artists_filter_changed)
 
         self.local_albums_model = LocalAlbumsModel()
-        self.local_albums_delegate = LocalAlbumsItemDelegate()
+        self.local_albums_proxy_model = LocalAlbumsProxyModel()
+        self.local_albums_proxy_model.setSourceModel(self.local_albums_model)
+        self.local_albums_proxy_model.setFilterCaseSensitivity(0)
+        self.local_albums_delegate = LocalAlbumsItemDelegate(self.local_albums_proxy_model)
         self.local_albums_delegate.artist_clicked.connect(self.on_local_album_artist_clicked)
         # self.local_albums_delegate.album_clicked.connect(self.on_local_album_clicked)
         self.ui.localAlbums.row_clicked.connect(self.on_local_album_clicked)
         # self.ui.localAlbums.row_double_clicked.connect(self.on_local_song_double_clicked)
         self.ui.localAlbums.setSpacing(6)
-        self.ui.localAlbums.setModel(self.local_albums_model)
+        self.ui.localAlbums.setModel(self.local_albums_proxy_model)
         self.ui.localAlbums.setItemDelegate(self.local_albums_delegate)
+        self.ui.localAlbumsFilter.textChanged.connect(self.on_local_albums_filter_changed)
 
         self.ui.localSongsButton.clicked.connect(self.on_local_songs_button_clicked)
         self.ui.localArtistsButton.clicked.connect(self.on_local_artists_button_clicked)
         self.ui.localAlbumsButton.clicked.connect(self.on_local_albums_button_clicked)
         self.on_local_songs_button_clicked()
 
+        self.ui.localSongsRandomPlayButton.clicked.connect(self.on_local_songs_random_play_button_clicked)
+
+
         # Load local songs
         # TODO: preferences flag?
-        localsongs.load_mp3s_background(
-            preferences.directory(),
-            mp3_loaded_callback=self.on_mp3_loaded,
-            finished_callback=self.on_mp3s_loaded,
-            load_images=False
-        )
+        repository.load_mp3s(preferences.directory(),
+                                        mp3_loaded_callback=self.on_mp3_loaded,
+                                        mp3_image_loaded_callback=self.on_mp3_image_loaded,
+                                        mp3s_loaded_callback=self.on_mp3s_loaded,
+                                        mp3s_images_loaded_callback=self.on_mp3s_images_loaded)
 
         # Play
         self.ui.playPauseButton.clicked.connect(self.on_play_pause_button_clicked)
         self.ui.playArtist.set_underline_on_hover(True)
         self.ui.playArtist.clicked.connect(self.on_play_artist_clicked)
         self.ui.playAlbum.set_underline_on_hover(True)
         self.ui.playAlbum.clicked.connect(self.on_play_album_clicked)
         self.ui.playContainer.setVisible(False)
         self.ui.playBar.valueChanged.connect(self.on_play_bar_changed)
         self.ui.prevSongButton.clicked.connect(self.on_prev_song_button_clicked)
         self.ui.nextSongButton.clicked.connect(self.on_next_song_button_clicked)
 
-        self.playing: Optional[Union[Track, Mp3]] = None
+        self.playing = PlayingInfo()
         self.playTimer = QTimer(self)
         self.playTimer.timeout.connect(self.on_play_timer_tick)
 
+        # Restore geometry
+        geometry, state = preferences.geometry_and_state()
+        if geometry:
+            self.restoreGeometry(geometry)
+        if state:
+            self.restoreState(state)
+
+    def closeEvent(self, ev: QCloseEvent) -> None:
+        debug("Closing window")
+        # Save geometry
+        preferences.set_geometry_and_state(self.saveGeometry(), self.saveState())
 
     def set_local_page(self):
         self.push_page(self.ui.localPage)
 
     def set_search_page(self):
         self.push_page(self.ui.searchPage)
 
@@ -207,14 +297,20 @@
 
     def set_album_page(self):
         self.push_page(self.ui.albumPage)
 
     def set_artist_page(self):
         self.push_page(self.ui.artistPage)
 
+    def set_local_album_page(self):
+        self.push_page(self.ui.localAlbumPage)
+
+    def set_local_artist_page(self):
+        self.push_page(self.ui.localArtistPage)
+
     def current_page(self):
         return self.pages_stack[self.pages_stack_cursor] if 0 <= self.pages_stack_cursor <= len(self.pages_stack) - 1 else None
 
     def push_page(self, page):
         if self.current_page() == page:
             return
 
@@ -239,14 +335,18 @@
                 return "search"
             if p == self.ui.downloadsPage:
                 return "downloads"
             if p == self.ui.albumPage:
                 return "album"
             if p == self.ui.artistPage:
                 return "artist"
+            if p == self.ui.localAlbumPage:
+                return "local_album"
+            if p == self.ui.localArtistsPage:
+                return "local_artist"
         next_page = self.pages_stack[self.pages_stack_cursor]
         debug(f"Updating current page to {page_to_string(next_page)}")
         debug(f"Page stack is ",
             [(f'{page_to_string(p)} (ACTIVE)' if idx == self.pages_stack_cursor else page_to_string(p))
              for idx, p in enumerate(self.pages_stack)])
         self.unselect_pages_buttons()
 
@@ -256,14 +356,18 @@
             self.select_page_button(self.ui.searchPageButton)
         elif next_page == self.ui.downloadsPage:
             self.select_page_button(self.ui.downloadsPageButton)
         elif next_page == self.ui.albumPage:
             pass
         elif next_page == self.ui.artistPage:
             pass
+        elif next_page == self.ui.localAlbumPage:
+            pass
+        elif next_page == self.ui.localArtistPage:
+            pass
 
         self.ui.pages.setCurrentWidget(next_page)
 
         self.ui.backButton.setEnabled(self.pages_stack_cursor > 0)
         self.ui.forwardButton.setEnabled(self.pages_stack_cursor < len(self.pages_stack) - 1)
 
     def unselect_pages_buttons(self):
@@ -320,27 +424,52 @@
         self.set_album_page()
 
         # fetch the main release and its tracks
         repository.fetch_release_group_releases(release_group.id, self.on_release_group_releases_result, self.on_release_group_youtube_tracks_result)
 
 
     def open_mp3_release_group(self, mp3: Mp3):
+        self.current_local_album_mp3_group_leader = mp3
+
+        # title
+        self.ui.localAlbumTitle.setText(mp3.album or UNKNOWN_ALBUM)
+
+        # artist
+        self.ui.localAlbumArtist.setText(mp3.artist or UNKNOWN_ARTIST)
+
+        # icon
+        self.ui.localAlbumCover.setPixmap(make_pixmap_from_data(mp3.image, default=resources.COVER_PLACEHOLDER_PIXMAP))
+        self.album_cover_data = mp3.image
+
+        # tracks
+        self.local_album_tracks_model.set(mp3)
+        self.ui.localAlbumTracks.invalidate()
+
+        # length
+        self.ui.localAlbumSongCount.setText(
+            f"{len(self.local_album_tracks_model.mp3s)} songs - "
+            f"{millis_to_long_string(sum([mp3.length for mp3 in self.local_album_tracks_model.mp3s]))}")
+
+        # switch page
+        self.set_local_album_page()
+
+    def open_mp3_release_group_remote(self, mp3: Mp3):
         # already fetched: open directly
         if mp3.fetched_release_group and mp3.release_group_id:
             self.open_release_group(get_release_group(mp3.release_group_id))
             return
 
         # fetch it by name
         self.current_release_group_id = None
 
         # title
         self.ui.albumTitle.setText(mp3.album)
 
         # artist
-        self.ui.albumArtist.setText(mp3.artist or "")
+        self.ui.albumArtist.setText(mp3.artist or UNKNOWN_ARTIST)
 
         # icon
         self.ui.albumCover.setPixmap(make_pixmap_from_data(mp3.image, default=resources.COVER_PLACEHOLDER_PIXMAP))
         self.album_cover_data = mp3.image
         self.ui.albumCoverNumber.setText("")
 
         # download
@@ -387,14 +516,15 @@
         self.ui.albumDownloadStatus.setText("")
         self.ui.albumOpenButton.setVisible(False)
 
         # tracks
         self.album_tracks_model.release_id = None
         self.ui.albumTracks.invalidate()
 
+
         # switch page
         self.set_album_page()
 
         # TODO: handle image blink
 
         def release_group_callback(release_group_name_, release_group):
             self.open_release_group(release_group)
@@ -429,14 +559,32 @@
         self.set_artist_page()
 
         # fetch the artist details (e.g. artist release groups)
         repository.fetch_artist(artist.id, self.on_artist_result, self.on_artist_image_result)
 
 
     def open_mp3_artist(self, mp3: Mp3):
+        self.current_local_artist_mp3_group_leader = mp3
+
+        # title
+        self.ui.localArtistName.setText(mp3.artist or UNKNOWN_ARTIST)
+
+        # icon
+        self.ui.localArtistCover.setPixmap(make_pixmap_from_data(mp3.image, default=resources.COVER_PLACEHOLDER_PIXMAP))
+        self.album_cover_data = mp3.image
+
+        # tracks
+        self.local_artist_albums_model.set(mp3)
+        self.ui.localArtistAlbums.invalidate()
+
+        # switch page
+        self.set_local_artist_page()
+
+
+    def open_mp3_artist_remote(self, mp3: Mp3):
         # already fetched: open directly
         if mp3.fetched_artist and mp3.artist_id:
             self.open_artist(get_artist(mp3.artist_id))
             return
 
         self.current_artist_id = None
 
@@ -577,21 +725,29 @@
     def on_release_group_releases_result(self, release_group_id: str, releases: List[Release]):
         debug(f"on_search_release_group_releases_result(release_group_id={release_group_id})")
 
         rg = get_release_group(release_group_id)
         if rg and self.current_release_group_id == rg.id:
             main_release_id = rg.main_release_id
             main_release = get_release(main_release_id)
+
+            # link
+            if rg.youtube_playlist_id:
+                self.ui.albumLink.setText(youtube_playlist_id_to_youtube_url(rg.youtube_playlist_id))
+            else:
+                self.ui.albumLink.setText("")
+
             if main_release:
                 self.album_tracks_model.release_id = main_release_id
                 self.ui.albumTracks.invalidate()
                 self.ui.albumYear.setText(rg.year())
                 self.ui.albumSongCount.setText(f"{main_release.track_count()} songs - {millis_to_long_string(main_release.length())}")
 
                 self.set_album_cover(release_group_id)
+
                 self.update_album_download_widgets()
 
         self.ui.artistAlbums.update_row(release_group_id)
 
         # repository.search_release_youtube_tracks(main_release_id, self.on_release_youtube_tracks_result)
 
 
@@ -702,42 +858,74 @@
 
         if not release_group:
             print(f"WARN: no release group found for id {release_group_id}")
             return
 
         self.open_release_group(release_group)
 
+    def on_local_artist_album_clicked(self, row: int):
+        debug(f"on_local_artist_album_clicked(row={row})")
+        album_group_leader = self.local_artist_albums_model.entry(row)
+        self.open_mp3_release_group(album_group_leader)
+
     def on_album_track_clicked(self, row: int):
         track_id = self.album_tracks_model.entry(row)
         track = get_track(track_id)
 
         if not track:
             print(f"WARN: no release group found for id {track_id}")
             return
 
+
     def on_album_artist_clicked(self):
         debug("on_album_artist_clicked")
         release_group = get_release_group(self.current_release_group_id)
         release_group_artists = release_group.artists()
         if not release_group_artists:
             print(f"WARN: no artist found for release group {self.current_release_group_id}")
         # TODO: more than an artist
         self.open_artist(release_group_artists[0])
 
     def on_album_cover_prev_button_clicked(self):
         debug("on_album_cover_prev_button_clicked")
-        self.album_change_cover_empty_image_callback = self.on_album_cover_prev_button_clicked
-        self.handle_album_cover_change_request(direction="prev")
+        self.album_change_cover_empty_image_callback = self.set_album_cover_prev_prevent_loop
+        release_group = get_release_group(self.current_release_group_id)
+        self.album_change_cover_initial_index = release_group.preferred_front_cover_index
+        self.set_album_cover_prev()
 
 
     def on_album_cover_next_button_clicked(self):
         debug("on_album_cover_next_button_clicked")
-        self.album_change_cover_empty_image_callback = self.on_album_cover_next_button_clicked
+        self.album_change_cover_empty_image_callback = self.set_album_cover_next_prevent_loop
+        release_group = get_release_group(self.current_release_group_id)
+        self.album_change_cover_initial_index = release_group.preferred_front_cover_index
+        self.set_album_cover_next()
+
+
+    def set_album_cover_prev_prevent_loop(self, force=False):
+        release_group = get_release_group(self.current_release_group_id)
+        if not force and self.album_change_cover_initial_index == release_group.preferred_front_cover_index:
+            return
+        self.set_album_cover_prev()
+
+
+    def set_album_cover_next_prevent_loop(self, force=False):
+        release_group = get_release_group(self.current_release_group_id)
+        if not force and self.album_change_cover_initial_index == release_group.preferred_front_cover_index:
+            return
+        self.set_album_cover_next()
+
+    def set_album_cover_prev(self):
+        self.handle_album_cover_change_request(direction="prev")
+
+
+    def set_album_cover_next(self):
         self.handle_album_cover_change_request(direction="next")
 
+
     def handle_album_cover_change_request(self, direction):
         if direction == "next":
             delta = 1
         elif direction == "prev":
             delta = -1
         else:
             raise ValueError(f"Unexpected direction: {direction}")
@@ -832,45 +1020,87 @@
 
     def on_album_cover_double_clicked(self, ev: QMouseEvent):
         debug("on_album_cover_double_clicked")
         image_preview_window = ImagePreviewWindow()
         image_preview_window.set_image(self.album_cover_data)
         image_preview_window.exec()
 
+    def on_local_album_cover_double_clicked(self, ev: QMouseEvent):
+        debug("on_local_album_cover_double_clicked")
+        image_preview_window = ImagePreviewWindow()
+        image_preview_window.set_image(self.album_cover_data)
+        image_preview_window.exec()
+
     def on_artist_image_double_clicked(self, ev: QMouseEvent):
         debug("on_artist_image_double_clicked")
         image_preview_window = ImagePreviewWindow()
         image_preview_window.set_image(self.artist_cover_data)
         image_preview_window.exec()
 
+    def on_local_artist_image_double_clicked(self, ev: QMouseEvent):
+        debug("on_local_artist_image_double_clicked")
+        image_preview_window = ImagePreviewWindow()
+        image_preview_window.set_image(self.artist_cover_data)
+        image_preview_window.exec()
+
+
+    def on_local_album_track_clicked(self, row: int):
+        pass
+
+    def on_local_album_artist_clicked_2(self):
+        debug("on_local_album_artist_clicked_2")
+        self.open_mp3_artist(self.current_local_album_mp3_group_leader)
+
     def on_release_group_youtube_tracks_result(self, release_group_id: str, yttracks: List[YtTrack]):
         debug("on_release_group_youtube_tracks_result")
 
         # fetch missing ones
-        release = get_release_group(release_group_id).main_release()
+        release_group = get_release_group(release_group_id)
+        release = release_group.main_release()
 
         missing = 0
         for t in release.tracks():
             if not t.fetched_youtube_track:
                 missing += 1
                 repository.search_track_youtube_track(t.id, self.on_track_youtube_track_result)
 
         if missing:
             debug(f"After release tracks fetching there was still {missing} "
                   f"missing tracks missing youtube video, searching now")
 
         self.handle_youtube_tracks_update(release.id)
 
+        if self.current_release_group_id == release.release_group_id:
+            self.ui.albumLink.setText(youtube_playlist_id_to_youtube_url(release_group.youtube_playlist_id))
+
 
     def on_track_youtube_track_result(self, track_id: str, yttrack: YtTrack):
         track = get_track(track_id)
         # self.ui.albumTracks.update_row(track_id) # would be more precise
         self.handle_youtube_tracks_update(track.release_id)
 
 
+    def on_track_link_button_clicked(self, row: int):
+        debug("on_track_link_button_clicked")
+        track_id = self.album_tracks_model.entry(row)
+        track = get_track(track_id)
+        video_id = get_youtube_track(track.youtube_track_id).video_id if track.youtube_track_id else None
+        edit_link_window = EditLinkWindow(ytcommons.youtube_video_id_to_youtube_url(video_id))
+        edit_link_window.exec()
+        if edit_link_window.link:
+            debug(f"New link set for track {track_id}: {edit_link_window.link}")
+            video_id = ytcommons.youtube_url_to_video_id(edit_link_window.link)
+            if video_id:
+                repository.set_track_youtube_video_id(track_id, video_id)
+            else:
+                print("WARN: invalid youtube URL")
+                QMessageBox.warning(self, "Invalid YouTube URL", f"Invalid YouTube URL")
+
+
+
     def on_track_download_button_clicked(self, row: int):
         debug("on_track_download_button_clicked")
         track_id = self.album_tracks_model.entry(row)
         self.do_download_youtube_track(track_id)
 
     def on_track_open_video_button_clicked(self, row: int):
         debug("on_track_open_video_button_clicked")
@@ -896,21 +1126,23 @@
         release = get_release_group(self.current_release_group_id).main_release()
         if not release:
             debug("update_album_download_widgets: no main release for release group")
             return
 
         tracks = release.tracks()
         # Download missing tracks button
+        verified_only = self.ui.albumDownloadAllVerifiedCheck.isChecked()
         missing_downloadable = 0
         verified = 0
         for track in tracks:
             if track.fetched_youtube_track and track.youtube_track_id:
                 if track.youtube_track_is_official:
                     verified += 1
-                if not track.is_locally_available() and not track.downloading:
+                if not track.is_locally_available() and not track.downloading and \
+                        (not verified_only or track.youtube_track_is_official):
                     missing_downloadable += 1
 
         self.ui.albumDownloadAllButton.setEnabled(missing_downloadable > 0)
         if missing_downloadable > 0:
             self.ui.albumDownloadAllButton.setText(f"Download missing songs ({missing_downloadable})")
         else:
             self.ui.albumDownloadAllButton.setText(f"Download missing songs")
@@ -944,31 +1176,39 @@
         if down["user_data"]["type"] == "official":
             track_id = down["user_data"]["id"]
             self.ui.albumTracks.update_row(track_id)
 
     def on_youtube_track_download_progress(self, down: dict, progress: float):
         debug(f"on_youtube_track_download_progress(video_id={down['video_id']}, progress={progress})")
         video_id = down["video_id"]
-        self.ui.queuedDownloads.update_row(video_id)
 
-        if down["user_data"]["type"] == "official":
-            track_id = down["user_data"]["id"]
-            self.ui.albumTracks.update_row(track_id)
+        # TODO: skipping the update in this way is a little bit superficial
+        # at least the stuff should be invalidated when reentering download/album/...
+        cur_page = self.pages_stack[-1]
+
+        if cur_page == self.ui.downloadsPage:
+            self.ui.queuedDownloads.update_row(video_id)
+
+        if cur_page == self.ui.albumPage:
+            if down["user_data"]["type"] == "official":
+                track_id = down["user_data"]["id"]
+                self.ui.albumTracks.update_row(track_id)
 
     def on_youtube_track_download_finished(self, down: dict):
         debug(f"on_youtube_track_download_finished(video_id={down['video_id']})")
         self.ui.queuedDownloads.invalidate()
         self.ui.finishedDownloads.invalidate()
         self.update_downloads_count()
         self.update_album_download_widgets()
         self.update_album_cover_state()
 
         debug("Reloading mp3s model")
         self.update_local_song_count()
         self.local_songs_model.beginResetModel()
+        self.local_songs_model.reload()
         self.local_songs_model.endResetModel()
 
         if down["user_data"]["type"] == "official":
             track_id = down["user_data"]["id"]
             self.ui.albumTracks.update_row(track_id)
 
             t = get_track(track_id)
@@ -995,43 +1235,115 @@
         self.ui.finishedDownloads.invalidate()
         self.update_downloads_count()
         self.update_album_download_widgets()
         if down["user_data"]["type"] == "official":
             track_id = down["user_data"]["id"]
             self.ui.albumTracks.update_row(track_id)
 
+        error_managed = False
+
+        # if "age" in error_msg:
+        #     debug("Age problem, eventually showing sign in window")
+        #     # Show sign in alert
+        #     if not ytdownloader.is_signed_in():
+        #         error_managed = True
+        #         sign_in_window = YouTubeSignInWindow()
+        #         sign_in_window.exec()
+        #         if ytdownloader.is_signed_in():
+        #             # Now we are signed in, try again
+        #             debug("Now we are signed in, trying again to download song")
+        #             if down["user_data"]["type"] == "official":
+        #                 track_id = down["user_data"]["id"]
+        #                 self.do_download_youtube_track(track_id)
+        #             elif down["user_data"]["type"] == "manual":
+        #                 video_id = down["user_data"]["id"]
+        #                 self.do_download_youtube_track_manual(video_id)
+
+        if not error_managed:
+            artist = down["artist"]
+            album = down["album"]
+            song = down["song"]
+            QMessageBox.warning(self, "Download failed",
+                                f"Download of {artist} - {album} - {song} failed\n"
+                                f"Reason: {error_msg}",
+                                QMessageBox.Ok)
+
     def update_downloads_count(self):
         queued_count = ytdownloader.download_count()
         finished_count = ytdownloader.finished_download_count()
         self.ui.downloadsPageButton.setText(f"Downloads ({queued_count})" if queued_count else "Downloads")
         self.ui.downloadsTabs.setTabText(DOWNLOADS_TABS_QUEUED_INDEX, f"Queue ({queued_count})" if queued_count else "Queue")
         self.ui.downloadsTabs.setTabText(DOWNLOADS_TABS_COMPLETED_INDEX, f"Completed ({finished_count})" if finished_count else "Completed")
 
     def on_download_missing_album_tracks_clicked(self):
-        debug("on_download_all_album_tracks_clicked")
+        verified_only = self.ui.albumDownloadAllVerifiedCheck.isChecked()
+        debug(f"on_download_missing_album_tracks_clicked (verified_only={verified_only})")
         rg = get_release_group(self.current_release_group_id)
         for track in rg.main_release().tracks():
             if not track.is_locally_available() and not track.downloading:
-                self.do_download_youtube_track(track.id)
+                if not verified_only or track.youtube_track_is_official:
+                    self.do_download_youtube_track(track.id)
+
+    def on_download_missing_album_tracks_verified_check_changed(self):
+        debug(f"on_download_missing_album_tracks_verified_check_changed")
+        self.update_album_download_widgets()
 
     def on_open_album_button_clicked(self):
         debug("on_open_album_button_clicked")
         rg = get_release_group(self.current_release_group_id)
         if rg.youtube_playlist_id:
             open_url(ytcommons.youtube_playlist_id_to_youtube_url(rg.youtube_playlist_id))
+        else:
+            print(f"WARN: no playlist id available for release group {rg.title}")
+
+    def on_local_album_open_remote_button_clicked(self):
+        debug("on_local_album_open_remote_button_clicked")
+        self.open_mp3_release_group_remote(self.current_local_album_mp3_group_leader)
+
+    def on_local_artist_open_remote_button_clicked(self):
+        debug("on_local_artist_open_remote_button_clicked")
+        self.open_mp3_artist_remote(self.current_local_artist_mp3_group_leader)
+
+    def on_local_album_random_play_button_clicked(self):
+        artist = self.current_local_album_mp3_group_leader.artist
+        album = self.current_local_album_mp3_group_leader.album
+        queue = [mp3 for mp3 in localsongs.mp3s if mp3.artist == artist and mp3.album == album]
+        random.shuffle(queue)
+        self.play(0, queue)
+
+
+    def on_local_artist_random_play_button_clicked(self):
+        artist = self.current_local_artist_mp3_group_leader.artist
+        queue = [mp3 for mp3 in localsongs.mp3s if mp3.artist == artist]
+        random.shuffle(queue)
+        self.play(0, queue)
+
+    def on_local_songs_random_play_button_clicked(self):
+        queue = list(localsongs.mp3s)
+        random.shuffle(queue)
+        self.play(0, queue)
 
     def do_download_youtube_track(self, track_id):
         repository.download_youtube_track(track_id,
                                           queued_callback=self.on_youtube_track_download_queued,
                                           started_callback=self.on_youtube_track_download_started,
                                           progress_callback=self.on_youtube_track_download_progress,
                                           finished_callback=self.on_youtube_track_download_finished,
                                           canceled_callback=self.on_youtube_track_download_canceled,
                                           error_callback=self.on_youtube_track_download_error)
 
+    def do_download_youtube_track_manual(self, video_id):
+        repository.download_youtube_track(video_id,
+                                          queued_callback=self.on_youtube_track_download_queued,
+                                          started_callback=self.on_youtube_track_download_started,
+                                          progress_callback=self.on_youtube_track_download_progress,
+                                          finished_callback=self.on_youtube_track_download_finished,
+                                          canceled_callback=self.on_youtube_track_download_canceled,
+                                          error_callback=self.on_youtube_track_download_error)
+
     def on_download_cancel_button_clicked(self, row: int):
         debug("on_download_cancel_button_clicked")
         down = self.downloads_model.entry(row)
         repository.cancel_youtube_track_download(down["video_id"])
 
     def on_download_artist_clicked(self, row: int):
         debug("on_download_artist_clicked")
@@ -1083,43 +1395,42 @@
     def on_mp3_loaded(self, mp3: Mp3):
         self.update_local_song_count()
 
     def on_mp3s_loaded(self, with_images):
         # self.ui.localSongs.invalidate()
         debug("Reloading mp3s model")
         self.reload_local_songs_artists_albums()
-        if not with_images:
-            debug("Loading images now")
-            localsongs.load_mp3s_images_background(
-                mp3_image_loaded_callback=self.on_mp3_image_loaded,
-                finished_callback=self.on_mp3s_images_loaded)
-
 
     def on_mp3_image_loaded(self, mp3: Mp3):
         pass
 
     def on_mp3s_images_loaded(self):
         debug("Reloading mp3s model")
         # self.ui.localSongs.invalidate()
         self.reload_local_songs_artists_albums()
 
-    def on_action_reload(self):
-        # Reload mp3s
+    def on_action_refresh(self):
         localsongs.clear_mp3s()
 
         self.reload_local_songs_artists_albums()
 
         self.update_local_song_count()
-        localsongs.load_mp3s_background(preferences.directory(),
+        repository.load_mp3s(preferences.directory(),
                                         mp3_loaded_callback=self.on_mp3_loaded,
-                                        finished_callback=self.on_mp3s_loaded,
-                                        load_images=False)
+                                        mp3_image_loaded_callback=self.on_mp3_image_loaded,
+                                        mp3s_loaded_callback=self.on_mp3s_loaded,
+                                        mp3s_images_loaded_callback=self.on_mp3s_images_loaded)
+
+    def on_action_reload(self):
+        cache.clear_localsongs()
+        self.on_action_refresh()
 
     def reload_local_songs_artists_albums(self):
         self.local_songs_model.beginResetModel()
+        self.local_songs_model.reload()
         self.local_songs_model.endResetModel()
 
         self.local_artists_model.beginResetModel()
         self.local_artists_model.reload()
         self.local_artists_model.endResetModel()
 
         self.local_albums_model.beginResetModel()
@@ -1170,32 +1481,32 @@
                 finished_callback=self.on_youtube_track_download_finished,
                 canceled_callback=self.on_youtube_track_download_canceled,
                 error_callback=self.on_youtube_track_download_error,
             )
 
 
     def on_local_song_artist_clicked(self, row: int):
-        mp3 = localsongs.mp3s[row]
+        mp3 = self.local_songs_model.entry(row)
         debug(f"on_local_song_artist_clicked: {mp3}")
         self.open_mp3_artist(mp3)
 
     def on_local_song_album_clicked(self, row: int):
-        mp3 = localsongs.mp3s[row]
+        mp3 = self.local_songs_model.entry(row)
         debug(f"on_local_song_album_clicked: {mp3}")
         self.open_mp3_release_group(mp3)
 
     def on_local_song_clicked(self, row: int):
-        mp3 = localsongs.mp3s[row]
+        mp3 = self.local_songs_model.entry(row)
         debug(f"on_local_song_clicked: {mp3}")
 
     def on_local_song_double_clicked(self, row: int):
-        mp3 = localsongs.mp3s[row]
+        mp3 = self.local_songs_model.entry(row)
         debug(f"on_local_song_double_clicked: {mp3}")
         if mp3.path:
-            self.play_local_song(mp3)
+            self.play(row, list(self.local_songs_model.localsongs))
 
     def on_finished_download_double_clicked(self, row: int):
         debug("on_finished_download_double_clicked")
         down = self.finished_downloads_model.entry(row)
         if down:
             # debug(f"Associated download: {down}")
             folder = down.get("file")
@@ -1225,73 +1536,96 @@
         self.ui.localAlbumsButton.setStyleSheet(resources.PILL_HIGHLIGHTED_STYLESHEET)
 
     def on_local_artist_clicked(self, row: int):
         debug("on_local_artist_clicked")
         mp3_group_leader = self.local_artists_model.entry(row)
         self.open_mp3_artist(mp3_group_leader)
 
-        # self.on_local_artist_clicked()
-
     def on_local_album_clicked(self, row: int):
         debug("on_local_album_clicked")
         mp3_group_leader = self.local_albums_model.entry(row)
         self.open_mp3_release_group(mp3_group_leader)
 
     def on_local_album_artist_clicked(self, row: int):
         debug("on_local_album_artist_clicked")
         mp3_group_leader = self.local_albums_model.entry(row)
         self.open_mp3_artist(mp3_group_leader)
 
     def on_track_double_clicked(self, row: int):
         debug("on_track_double_clicked")
         track_id = self.album_tracks_model.entry(row)
-        self.play_track(track_id)
+        self.play(row, list(get_release(self.album_tracks_model.release_id).tracks()))
+
+    def on_local_track_double_clicked(self, row: int):
+        debug("on_local_track_double_clicked")
+        mp3 = self.local_album_tracks_model.entry(row)
+        self.play(row, list(self.local_album_tracks_model.mp3s))
+
+    def play(self, index: int, queue=None):
+        if queue is not None:
+            self.playing.queue = queue
+
+        if index < 0 or index >= len(self.playing.queue):
+            debug("Nothing to play")
+            return
+
+        self.playing.index = index
+        song = self.playing.queue[index]
 
-    def play_local_song(self, mp3: Mp3):
+        if isinstance(song, Mp3):
+            self.play_mp3(song)
+        elif isinstance(song, Track):
+            self.play_track(song)
+
+    def play_mp3(self, mp3: Mp3):
         self.ui.playContainer.setVisible(False)
 
         self.ui.playCover.setPixmap(make_pixmap_from_data(mp3.image, default=resources.COVER_PLACEHOLDER_PIXMAP))
-        self.ui.playTitle.setText(mp3.song)
-        self.ui.playArtist.setText(mp3.artist)
-        self.ui.playAlbum.setText(mp3.album)
+        self.ui.playTitle.setText(mp3.title())
+        self.ui.playArtist.setText(mp3.artist or UNKNOWN_ARTIST)
+        self.ui.playAlbum.setText(mp3.album or UNKNOWN_ALBUM)
 
-        self.ui.playBar.setValue(0, notify=False)
+        self.ui.playBar.set_value(0, notify=False)
         self.ui.playCurrentTime.setText(millis_to_short_string(0))
         self.ui.playMaxTime.setText(millis_to_short_string(mp3.length))
 
-        self.playing = mp3
         self.play_audio(str(mp3.path))
 
-    def play_track(self, track_id):
-        track = get_track(track_id)
+    def play_track(self, track: Track):
+        local_mp3, local_mp3_idx = track.get_local_ext()
+        if local_mp3:
+            # play locally if available
+            self.play_mp3(local_mp3)
+            return
+
+        # play from url
         self.ui.playContainer.setVisible(False)
 
         rg = track.release().release_group()
         self.ui.playCover.setPixmap(make_pixmap_from_data(rg.preferred_front_cover(), default=resources.COVER_PLACEHOLDER_PIXMAP))
         self.ui.playTitle.setText(track.title)
-        self.ui.playArtist.setText(rg.artists_string())
-        self.ui.playAlbum.setText(rg.title)
+        self.ui.playArtist.setText(rg.artists_string() or UNKNOWN_ARTIST)
+        self.ui.playAlbum.setText(rg.title or UNKNOWN_ALBUM)
 
-        self.ui.playBar.setValue(0, notify=False)
+        self.ui.playBar.set_value(0, notify=False)
         self.ui.playCurrentTime.setText(millis_to_short_string(0))
         self.ui.playMaxTime.setText(millis_to_short_string(track.length))
 
         def track_streams_fetched(_1, _2):
             yttrack = get_youtube_track(track.youtube_track_id)
 
             audios = sorted([s for s in yttrack.streams if s["type"] == "audio"], key=lambda s: s["size"])
             if audios:
-                self.playing = track
                 self.play_audio(audios[0]["url"])
 
-        repository.fetch_youtube_track_streams(track_id, track_streams_fetched)
+        repository.fetch_youtube_track_streams(track.id, track_streams_fetched)
 
-    def play_audio(self, audio_url: str):
+    def play_audio(self, audio_url_or_path: str):
         audioplayer.set_time(0)
-        audioplayer.open_stream(audio_url)
+        audioplayer.open_stream(audio_url_or_path)
         audioplayer.play()
 
         self.ui.playContainer.setVisible(True)
         self.ui.playPauseButton.setIcon(resources.PAUSE_ICON)
         self.playTimer.start(200)
 
     def on_play_pause_button_clicked(self):
@@ -1300,84 +1634,145 @@
             return
 
         if audioplayer.is_playing():
             audioplayer.pause()
             self.ui.playPauseButton.setIcon(resources.PLAY_ICON)
         elif audioplayer.is_paused():
             audioplayer.play()
+            self.playTimer.start(200)
             self.ui.playPauseButton.setIcon(resources.PAUSE_ICON)
         elif audioplayer.is_ended():
             audioplayer.set_time(0)
             audioplayer.play()
             self.ui.playPauseButton.setIcon(resources.PAUSE_ICON)
             self.update_play_progress()
         else:
             print(f"WARN: unexpected audio player state: {audioplayer.get_state()}")
 
     def on_play_artist_clicked(self):
-        # TODO: more than an artist
-        if isinstance(self.playing, Track):
-            self.open_artist(self.playing.release().release_group().artists()[0])
-        elif isinstance(self.playing, Mp3):
-            self.open_mp3_artist(self.playing)
+        in_play = self.playing.in_play()
+        if isinstance(in_play, Mp3):
+            self.open_mp3_artist(in_play)
+        elif isinstance(in_play, Track):
+            # TODO: more than an artist
+            self.open_artist(in_play.release().release_group().artists()[0])
 
     def on_play_album_clicked(self):
-        if isinstance(self.playing, Track):
-            self.open_release_group(self.playing.release().release_group())
-        elif isinstance(self.playing, Mp3):
-            self.open_mp3_release_group(self.playing)
+        in_play = self.playing.in_play()
+        if isinstance(in_play, Mp3):
+            self.open_mp3_release_group(in_play)
+        elif isinstance(in_play, Track):
+            self.open_release_group(in_play.release().release_group())
 
     def on_play_timer_tick(self):
         self.update_play_progress()
 
     def update_play_progress(self):
         if audioplayer.is_playing():
             t = audioplayer.get_time()
             self.ui.playCurrentTime.setText(millis_to_short_string(t))
-            self.ui.playBar.setValue(int(100 * t / self.playing.length), notify=False)
+            try:
+                self.ui.playBar.set_value(int(100 * t / self.playing.in_play().length), notify=False)
+            except:
+                self.ui.playBar.set_value(0, notify=False)
         elif audioplayer.is_paused():
             self.playTimer.stop()
         elif audioplayer.is_ended():
             self.playTimer.stop()
             self.ui.playPauseButton.setIcon(resources.PLAY_ICON)
             self.ui.playCurrentTime.setText(millis_to_short_string(0))
-            self.ui.playBar.setValue(0, notify=False)
+            self.ui.playBar.set_value(0, notify=False)
             self.play_next()
 
 
     def play_by_offset(self, delta):
         debug("play_next")
-        if isinstance(self.playing, Track):
-            rg = self.playing.release().release_group()
-            main_release = rg.main_release()
-            next_idx = main_release.track_ids.index(self.playing.id) + delta
-            if 0 <= next_idx < main_release.track_count():
-                self.play_track(main_release.track_ids[next_idx])
-            else:
-                print("Nothing else to play")
-        elif isinstance(self.playing, Mp3):
-            next_idx = localsongs.mp3s.index(self.playing) + delta
-            if 0 <= next_idx < len(localsongs.mp3s):
-                self.play_local_song(localsongs.mp3s[next_idx])
-            else:
-                print("Nothing else to play")
+        self.play(self.playing.index + delta)
 
     def play_next(self):
         debug("play_next")
         self.play_by_offset(1)
 
     def play_prev(self):
         debug("play_prev")
         self.play_by_offset(-1)
 
     def on_play_bar_changed(self):
         debug(f"on_play_bar_changed, value = {self.ui.playBar.value()}")
         # t : length = value : 100
-        t = rangify(0, int(self.ui.playBar.value() * self.playing.length / 100), self.playing.length)
+        t = rangify(0, int(self.ui.playBar.value() * self.playing.in_play().length / 100), self.playing.in_play().length)
         audioplayer.set_time(t)
         self.update_play_progress()
 
     def on_prev_song_button_clicked(self):
         self.play_prev()
 
     def on_next_song_button_clicked(self):
         self.play_next()
+
+    def on_album_link_button_clicked(self):
+        debug("on_album_link_button_clicked")
+        self.ui.albumLinkButton.setVisible(False)
+        self.ui.albumLinkContainer.setVisible(True)
+
+    def on_album_link_ok_button_clicked(self):
+        debug("on_album_link_ok_button_clicked")
+        self.ui.albumLinkButton.setVisible(True)
+        self.ui.albumLinkContainer.setVisible(False)
+        playlist_id = youtube_url_to_playlist_id(self.ui.albumLink.text())
+        if not playlist_id:
+            print("WARN: invalid youtube url")
+            QMessageBox.warning(self, "Invalid URL",
+                                "Invalid YouTube URL",
+                                QMessageBox.Ok)
+            return
+
+        repository.set_release_group_playlist_id(self.current_release_group_id, playlist_id,
+                                                 self.on_release_group_releases_result, self.on_release_group_youtube_tracks_result)
+
+    def on_album_link_cancel_button_clicked(self):
+        debug("on_album_link_cancel_button_clicked")
+        self.ui.albumLinkButton.setVisible(True)
+        self.ui.albumLinkContainer.setVisible(False)
+
+    def on_show_album_tracks_youtube_titles_check_changed(self):
+        debug("on_show_album_tracks_youtube_titles_check_changed")
+        self.ui.albumTracks.set_show_youtube_titles(self.ui.showYouTubeTitlesCheck.isChecked())
+
+    def on_album_open_local_button_clicked(self):
+        debug("on_album_open_local_button_clicked")
+        album = get_release_group(self.current_release_group_id)
+        for mp3 in localsongs.mp3s:
+            if mp3.artist and mp3.artist.lower() == album.artists_string().lower() and mp3.album and mp3.album.lower() == album.title.lower():
+                self.open_mp3_release_group(mp3)
+                return
+        print(f"WARN: album '{album.title}' not locally available")
+
+    def on_artist_open_local_button_clicked(self):
+        debug("on_artist_open_local_button_clicked")
+        artist = get_artist(self.current_artist_id)
+        for mp3 in localsongs.mp3s:
+            if mp3.artist and mp3.artist.lower() == artist.name.lower():
+                self.open_mp3_artist(mp3)
+                return
+        print(f"WARN: artist '{artist.name}' not locally available")
+
+    def on_local_songs_filter_changed(self):
+        filter_text = self.ui.localSongsFilter.text()
+        debug(f"on_local_songs_filter_changed({filter_text})")
+        self.local_songs_proxy_model.setFilterRegularExpression(QRegularExpression(filter_text, QRegularExpression.CaseInsensitiveOption))
+
+
+    def on_local_artists_filter_changed(self):
+        filter_text = self.ui.localArtistsFilter.text()
+        debug(f"on_local_artists_filter_changed({filter_text})")
+        self.local_artists_proxy_model.setFilterRegularExpression(QRegularExpression(filter_text, QRegularExpression.CaseInsensitiveOption))
+
+
+    def on_local_albums_filter_changed(self):
+        filter_text = self.ui.localAlbumsFilter.text()
+        debug(f"on_local_albums_filter_changed({filter_text})")
+        self.local_albums_proxy_model.setFilterRegularExpression(QRegularExpression(filter_text, QRegularExpression.CaseInsensitiveOption))
+
+    def on_auto_download_queued_check_changed(self):
+        debug(f"on_auto_download_queued_check_changed={self.ui.autoDownloadQueuedCheck.isChecked()}")
+        ytdownloader.set_auto_download(self.ui.autoDownloadQueuedCheck.isChecked())
```

### Comparing `music-dragon-0.8/music_dragon/ui/preferenceswindow.py` & `music-dragon-0.9/music_dragon/ui/preferenceswindow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from PyQt5.QtWidgets import QDialog, QFileDialog
 
-from music_dragon import cache, preferences
+from music_dragon import cache, preferences, ytdownloader
 from music_dragon.log import debug
 from music_dragon.ui.ui_preferenceswindow import Ui_PreferencesWindow
 from music_dragon.utils import open_folder, app_cache_path
 
 
 class PreferencesWindow(QDialog):
     COVER_SIZE_VALUES = [
@@ -28,54 +28,75 @@
         self.ui = Ui_PreferencesWindow()
         self.ui.setupUi(self)
 
         # Directory
         self.ui.directory.clicked.connect(self.on_directory_clicked)
         self.ui.browseDirectoryButton.clicked.connect(self.on_browse_directory_button_clicked)
 
+        # Download directory
+        self.ui.manualDownloadDirectory.clicked.connect(self.on_manual_download_directory_clicked)
+        self.ui.browseManualDownloadDirectoryButton.clicked.connect(self.on_browse_manual_download_directory_button_clicked)
+
         # Cache
         self.ui.cache.clicked.connect(self.on_cache_clicked)
         self.ui.cacheClearButton.clicked.connect(self.on_clear_cache_button_clicked)
         self.update_cache_size()
 
         # OK / CANCEL
         self.accepted.connect(self.on_accepted)
         self.rejected.connect(self.on_rejected)
 
         # Actually load settings
         self.load_settings()
 
+        # HACK
+        self.ui.tabWidget.removeTab(3)
+
     def on_accepted(self):
         debug("Saving preferences")
         self.save_settings()
 
     def on_rejected(self):
         debug("Closing preferences window without saving")
 
     def load_settings(self):
         self.ui.directory.setText(preferences.directory())
+        self.ui.manualDownloadDirectory.setText(preferences.manual_download_directory())
         self.ui.coverSize.setCurrentIndex(PreferencesWindow.COVER_SIZE_INDEXES[preferences.cover_size()])
         self.ui.outputFormat.setText(preferences.output_format())
+        self.ui.manualOutputFormat.setText(preferences.manual_output_format())
         self.ui.threadNumber.setValue(preferences.thread_number())
         self.ui.maxSimultaneousDownloads.setValue(preferences.max_simultaneous_downloads())
         self.ui.cacheImagesCheck.setChecked(preferences.is_images_cache_enabled())
         self.ui.cacheRequestsBox.setChecked(preferences.is_requests_cache_enabled())
+        self.ui.cacheLocalSongs.setChecked(preferences.is_localsongs_cache_enabled())
         self.ui.cache.setText(str(app_cache_path().absolute()))
+        self.ui.youtubeEmail.setText(preferences.get_youtube_email())
+        self.ui.youtubePassword.setText(preferences.get_youtube_password())
 
     def save_settings(self):
         preferences.set_directory(self.ui.directory.text())
+        preferences.set_manual_download_directory(self.ui.manualDownloadDirectory.text())
         preferences.set_cover_size(PreferencesWindow.COVER_SIZE_VALUES[self.ui.coverSize.currentIndex()])
         preferences.set_output_format(self.ui.outputFormat.text())
+        preferences.set_manual_output_format(self.ui.manualOutputFormat.text())
         preferences.set_thread_number(self.ui.threadNumber.value())
         preferences.set_max_simultaneous_downloads(self.ui.maxSimultaneousDownloads.value())
+
         preferences.set_images_cache_enabled(self.ui.cacheImagesCheck.isChecked())
         preferences.set_requests_cache_enabled(self.ui.cacheRequestsBox.isChecked())
+        preferences.set_localsongs_cache_enabled(self.ui.cacheLocalSongs.isChecked())
+        preferences.set_youtube_email(self.ui.youtubeEmail.text())
+        preferences.set_youtube_password(self.ui.youtubePassword.text())
 
         cache.enable_images_cache(preferences.is_images_cache_enabled())
         cache.enable_requests_cache(preferences.is_requests_cache_enabled())
+        cache.enable_localsongs_cache(preferences.is_localsongs_cache_enabled())
+
+        ytdownloader.set_credentials(preferences.get_youtube_email(), preferences.get_youtube_password())
 
     def on_directory_clicked(self):
         directory_str = self.ui.directory.text()
         debug(f"Opening directory: {directory_str}")
         directory = Path(directory_str)
         if not directory.exists():
             print(f"WARN: cannot open directory: '{directory_str}' does not exist")
@@ -93,14 +114,39 @@
                 return
 
             result = results[0]
             debug(f"Selected directory: {result}")
             self.ui.directory.setText(result)
 
 
+
+    def on_manual_download_directory_clicked(self):
+        directory_str = self.ui.manualDownloadDirectory.text()
+        debug(f"Opening download_directory: {directory_str}")
+        directory = Path(directory_str)
+        if not directory.exists():
+            print(f"WARN: cannot open directory: '{directory_str}' does not exist")
+            return
+        open_folder(directory)
+
+    def on_browse_manual_download_directory_button_clicked(self):
+        debug("Opening download directory picker")
+        directory_picker = QFileDialog()
+        directory_picker.setFileMode(QFileDialog.Directory)
+        if directory_picker.exec():
+            results = directory_picker.selectedFiles()
+            if not results:
+                print("WARN: no directory has been selected")
+                return
+
+            result = results[0]
+            debug(f"Selected directory: {result}")
+            self.ui.manualDownloadDirectory.setText(result)
+
+
     def on_cache_clicked(self):
         open_folder(app_cache_path())
 
     def on_clear_cache_button_clicked(self):
         cache.clear()
         self.update_cache_size()
```

### Comparing `music-dragon-0.8/music_dragon/ui/res_rc.py` & `music-dragon-0.9/music_dragon/ui/res_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,307 @@
 # -*- coding: utf-8 -*-
 
 # Resource object code
 #
-# Created by: The Resource Compiler for PyQt5 (Qt v5.15.2)
+# Created by: The Resource Compiler for PyQt5 (Qt v5.15.4)
 #
 # WARNING! All changes made in this file will be lost!
 
 from PyQt5 import QtCore
 
 qt_resource_data = b"\
+\x00\x00\x03\x6d\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
+\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
+\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
+\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
+\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
+\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
+\x6b\x42\xcf\x00\x00\x02\x6f\x49\x44\x41\x54\x78\xda\xed\x9a\x3f\
+\x6b\x14\x41\x18\x87\x1f\x4f\x09\xb1\x0b\x24\x95\x20\x84\x58\x68\
+\xa3\x10\x49\xa5\x41\xf0\x34\x0a\xd6\x62\xe1\x87\x10\xac\x6c\x2d\
+\xad\xc4\x6f\x60\x23\x16\x8a\x1f\x40\xd7\xa8\x10\x04\xb5\xd0\x46\
+\x88\x08\xd1\x42\xc1\x26\x01\xa3\x01\xff\x85\x9c\xc5\xec\x42\x38\
+\xde\xb9\xdd\xd9\x99\xb9\x99\xcb\xbd\x0f\x0c\xdc\x0d\x73\x77\xfb\
+\x7b\xee\x9d\xd9\xbb\x61\x40\x51\x14\x45\x51\x14\x45\x19\x4f\xf6\
+\x35\x1c\x73\x02\x98\x05\x26\x3c\x3e\xeb\x07\xf0\x38\x75\x60\x57\
+\x2e\x02\x1f\x80\x5e\xa0\x76\x33\x75\x20\x17\xae\x00\xdb\x01\xc3\
+\x8f\x94\x84\x19\x60\x33\x42\xf8\x91\x91\x70\x2d\x62\xf8\x91\x90\
+\x70\x77\x08\x02\x7a\xc0\xad\xd4\x41\x6d\x3c\x18\x92\x80\xd0\xed\
+\x1b\x70\x1f\x73\xd7\x1a\x4b\x01\x55\xfb\x03\x5c\x6d\x12\xb4\xe3\
+\x5d\x2b\x79\x32\x81\x99\xc6\xb5\x95\xb0\x57\x05\x54\x12\x6e\x8c\
+\xb3\x00\x80\x6e\xdd\x80\x03\x0e\x6f\xf6\x0a\xb8\x9d\x3a\x91\x23\
+\xbd\x90\x02\xbe\x00\x0f\x53\x27\x0a\xcd\x5e\x9f\x02\x2a\x40\x05\
+\xd4\xe0\xb2\x06\xd8\xe8\x02\xd3\xa9\x83\x38\xb2\x09\x3c\x09\x21\
+\x60\x3f\xf0\x08\x98\x4a\x9d\xc8\x91\x7b\x95\x00\xdf\x29\xb0\x30\
+\x82\xe1\x01\x8a\xea\x81\xaf\x80\x73\xa9\x93\xb4\xe4\xd9\x38\x0b\
+\x78\x0f\x7c\x0d\x21\x60\x12\x38\x95\x3a\x4d\x0b\x8a\xdd\x4f\x7c\
+\x04\x2c\x96\x12\xfa\x39\x82\xd9\x49\x4e\xdd\x16\x62\x0b\x90\xca\
+\x7f\x0d\xf8\xe4\xf1\x9e\x21\x59\x12\xfa\xfe\x02\x2b\x31\x05\x3c\
+\x4d\x9d\xba\xe6\xfa\x5e\x02\x5b\x21\x04\x4c\x01\x27\x85\xfe\xe5\
+\xd4\xa9\x4b\x26\x81\xd3\x42\x7f\xd1\xdf\xd1\x56\xc0\x59\xcc\x8f\
+\xa0\xdd\xec\x00\xcf\x53\x27\x2f\x59\x04\x0e\xc6\x14\x20\x95\xd7\
+\x5b\x60\x3d\x75\xf2\x92\xf3\x42\xdf\x46\x79\x8d\xd1\x04\xe4\x34\
+\xff\x25\x01\xcb\x98\x2a\xf5\x16\x70\x08\x38\x66\xf9\x80\x1c\x98\
+\x06\xe6\x85\xfe\x42\x1a\xdc\x46\x80\xf4\xed\xff\xc6\xac\xb0\x39\
+\xd0\xb5\xe4\x12\xbf\xa0\x50\x02\x56\x80\x5f\xa9\x93\x97\x48\xe5\
+\xff\x11\xf8\x1c\x4a\x80\xb4\xd3\x9a\x4b\xf9\xdb\x04\x14\xb6\xc1\
+\xae\x02\x8e\x02\x87\x85\xfe\x5c\x16\xc0\x59\x60\x2e\xa6\x00\xa9\
+\xfc\x37\x80\x77\xa9\x93\x97\x5c\x10\xfa\xb6\x81\x17\x31\x05\x88\
+\xb7\x97\x44\x48\xe5\xff\x1a\xb3\x05\xe6\x2d\xa0\x03\x9c\xb1\x08\
+\xc8\x81\x0e\xe6\x17\x6a\x3f\x45\xdd\x8b\x9a\x32\x8f\x39\x39\xd2\
+\x4f\x2e\xf3\xbf\xd5\xf5\xd9\x36\x45\xb7\x84\xbe\x39\xcb\xd8\xb5\
+\xd4\xc9\x07\xf0\x13\x78\x33\x68\x80\xad\x02\x72\x59\xd4\x7c\x29\
+\x80\x7f\x6d\x5e\x38\x03\x7c\x27\xfd\x41\x07\xdf\x76\xc9\xc7\xde\
+\x65\xe2\x1c\x93\x1b\x56\xbb\xe3\x13\xbe\x62\x09\x58\xcd\x20\x8c\
+\x4b\x5b\x07\xae\xd3\x70\x81\x6f\x72\x54\x16\xe0\x38\x66\x11\xf4\
+\x39\x2a\x1b\x9b\x1d\xcc\x7e\xe4\x2a\xe6\xcf\x99\xa2\x28\x8a\xa2\
+\x28\x8a\xa2\x0c\xe0\x3f\x94\xab\xaa\x38\x29\x07\x4f\xa2\x00\x00\
+\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\
+\x65\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x33\x54\x30\x39\x3a\
+\x30\x33\x3a\x31\x30\x2b\x30\x30\x3a\x30\x30\x41\xba\xb7\x88\x00\
+\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\
+\x66\x79\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x33\x54\x30\x39\
+\x3a\x30\x33\x3a\x31\x30\x2b\x30\x30\x3a\x30\x30\x30\xe7\x0f\x34\
+\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x02\xb8\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
+\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
+\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
+\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
+\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
+\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
+\x6b\x42\xcf\x00\x00\x01\xba\x49\x44\x41\x54\x78\xda\xed\x99\xbb\
+\x2e\x45\x41\x14\x86\xbf\x25\x1a\x8d\x42\xa2\xd0\x68\x34\x1a\x11\
+\x97\x84\x53\x48\x44\x21\x2a\x2a\x3a\xc7\x23\xf0\x08\x3c\x02\xb5\
+\x82\xe3\x52\xd0\xa9\x44\x25\x51\x68\x5c\x0a\x8d\x82\x46\xa3\x90\
+\x28\x24\x22\x11\xf2\x2b\xce\x14\xbb\xd0\xc8\xd9\x7b\xcf\x3e\x66\
+\x7d\x0f\x30\x6b\xff\x5f\xd6\xcc\xac\xc9\x06\xc7\x71\x1c\xc7\x71\
+\x1c\xc7\x71\x1c\xc7\x71\x9c\x3f\xa2\xdf\x59\x2c\xa1\x6e\xb7\xa4\
+\x46\xab\xeb\x74\x94\xa3\x29\xf7\xf0\x35\xe0\x06\x58\x4e\x4a\x80\
+\xa4\x4e\x49\xeb\xc0\x05\x30\x90\xc7\x9a\x9d\xb1\x43\xfd\x21\xfc\
+\x20\xb0\x0f\x8c\xe5\xb9\x6e\x5b\x74\x80\xa4\x3a\x70\x95\x77\x78\
+\xa8\x78\x07\x48\xea\x05\xb6\x81\xf9\xa2\x6a\x54\x56\x80\xa4\x59\
+\x60\x07\xe8\x2b\xb2\x4e\xe5\xb6\x80\xa4\x2e\x49\x9b\xc0\x69\xd1\
+\xe1\xa1\x62\x1d\x20\x69\x08\x38\x00\x86\xca\xaa\x59\x89\x0e\x90\
+\x64\x92\x56\x69\x1e\x74\xa5\x85\x87\x0a\x74\x80\xa4\x7e\x60\x17\
+\x98\x8e\x51\x3f\x6a\x07\x84\x91\xf9\x36\x56\xf8\x68\x02\x32\x73\
+\xfc\x11\xd0\x13\x2b\x3c\x44\xd8\x02\x61\x8e\xdf\x23\xa7\x51\xb6\
+\x55\x4a\xeb\x80\x22\xe6\xf8\x3c\x28\xa5\x03\x8a\x9a\xe3\xf3\xa0\
+\x12\xd7\xe0\xbf\x17\x60\x66\xf7\xc0\x24\xb0\x01\x7c\xc7\x0e\x5d\
+\xba\x80\x20\xe1\xcb\xcc\xd6\x81\x29\xe0\x31\x76\xf0\xd2\x05\x64\
+\x44\x5c\x02\xa3\x34\x6f\x82\xe8\x44\x39\x03\xcc\xec\xcd\xcc\xea\
+\xc0\x12\xf0\x9a\x9c\x80\x8c\x88\x63\x60\x04\x38\x4f\x52\x40\x90\
+\xf0\x04\xcc\x00\x6b\xc0\x67\x72\x02\x82\x04\x99\xd9\x26\x30\x0e\
+\xdc\x25\x27\x20\x23\xe2\x0e\x98\x00\xb6\x00\x25\x27\x20\x48\xf8\
+\x30\xb3\x55\x60\x0e\x78\x4e\x4e\x40\x46\xc4\x19\x30\x0c\x9c\x24\
+\x29\x20\x48\x78\x31\xb3\x05\x60\x05\x78\x4f\x4e\x40\x46\x44\x83\
+\xe6\x01\x79\x9d\xa4\x80\x20\xa1\x9a\xef\x89\x18\x7f\x87\x25\xd5\
+\x24\x3d\x48\x6a\xf9\xa6\x68\x9b\x0e\xc8\x12\xde\x13\x63\xc0\x61\
+\xec\x6f\x71\x1c\xc7\x71\x1c\xc7\x71\x1c\xc7\x71\x1c\xa7\xfd\xf8\
+\x01\x73\xbb\xad\xea\xb8\xa9\x09\x48\x00\x00\x00\x25\x74\x45\x58\
+\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\
+\x32\x2d\x30\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x30\x33\
+\x2b\x30\x30\x3a\x30\x30\xcc\xfd\x4d\xd2\x00\x00\x00\x25\x74\x45\
+\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\
+\x32\x32\x2d\x30\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x30\
+\x33\x2b\x30\x30\x3a\x30\x30\xbd\xa0\xf5\x6e\x00\x00\x00\x00\x49\
+\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x01\x9e\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x30\x00\x00\x00\x30\x08\x06\x00\x00\x00\x57\x02\xf9\x87\
+\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
+\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
+\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
+\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
+\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
+\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
+\x6b\x42\xcf\x00\x00\x00\xa0\x49\x44\x41\x54\x68\xde\xed\xd9\x31\
+\x0e\x82\x40\x00\x05\xd1\xd1\x73\x68\xed\x35\x2d\xbd\x8a\xde\xc0\
+\xc2\x1b\x19\x13\xc2\x01\xb0\x30\xda\xca\xca\xee\xfe\xa8\xf3\x12\
+\x3a\x42\xfe\x40\xa0\x01\x24\xe9\x57\xec\x81\x69\xe6\x71\x48\x8f\
+\x5d\x32\xbe\x6a\xc4\xaa\xe0\xdc\xa9\xf3\x4d\x99\xb5\x6d\xdd\x79\
+\x54\x75\x06\xe8\xdf\x95\x7c\x85\x9e\x5a\x7f\x8d\x8a\x36\x7d\xfd\
+\x3b\x60\x40\x9a\x01\x69\x06\xa4\x19\x90\x66\x40\x9a\x01\x69\x06\
+\xa4\x19\x90\x66\x40\x9a\x01\x69\x06\xa4\x7d\x12\x30\x36\xdc\x33\
+\xf4\x08\xb8\x34\x0c\x38\x37\xbc\xf6\xcb\x0e\xb8\x51\xfe\x43\xe3\
+\xdd\x71\x05\x36\x3d\x02\x00\xb6\xc0\x89\xc7\x23\x5f\x3a\x7c\x00\
+\x8e\x3d\xc7\x4b\x52\x3d\x77\x26\x42\x46\xf6\xa2\xc9\xef\x56\x00\
+\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\
+\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x38\x54\x30\x38\
+\x3a\x35\x36\x3a\x30\x33\x2b\x30\x30\x3a\x30\x30\xac\xcb\x38\xb5\
+\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\
+\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x38\x54\x30\
+\x38\x3a\x35\x36\x3a\x30\x33\x2b\x30\x30\x3a\x30\x30\xdd\x96\x80\
+\x09\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x05\x14\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
+\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
+\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
+\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
+\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
+\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
+\x6b\x42\xcf\x00\x00\x04\x16\x49\x44\x41\x54\x78\xda\xed\x9b\x4b\
+\x68\x1e\x55\x18\x86\x9f\x2f\x74\x21\xad\x4d\xef\x56\x17\x5a\x2f\
+\xa0\x29\xa9\x2b\x4b\x11\x05\x4b\xac\xa2\x88\x28\x8a\x1b\x29\x9a\
+\x76\x2f\x16\xdc\x08\x82\x78\x59\x89\x88\xd0\x42\x8b\x0b\xef\x0b\
+\xa5\x2e\xda\x8d\xb8\x11\xba\xd0\x4d\x05\x71\x63\x5a\x53\x6b\x4b\
+\xd3\x82\x36\xa6\x86\x9a\xa4\xea\xaa\x8f\x8b\x99\x60\x1a\x66\xfe\
+\x7f\x26\x99\x4b\x6a\xff\x77\xf9\xcf\x99\x7f\xce\xf3\xce\xf7\xcd\
+\x9c\xf3\x9d\x33\xd0\x53\x4f\x3d\xf5\x74\x0d\x2b\x9a\xba\x90\xba\
+\x11\xd8\x02\xdc\x05\x6c\x02\x56\x03\xd7\xa7\x87\x67\x80\x8b\xc0\
+\x18\x70\x02\x18\x89\x88\xf1\xb6\xcd\x59\x2c\x70\x9f\xfa\xb0\x7a\
+\x40\xfd\xc9\xf2\x3a\xae\xee\x57\x77\xa8\x7d\x6d\xf3\x94\x01\xdf\
+\xa0\xbe\xa9\x9e\x5b\x00\x74\x9e\xce\xaa\x6f\xa8\xeb\xdb\xe6\xeb\
+\x04\xbe\x46\x7d\x57\x9d\xa9\x10\x7c\xbe\x66\xd4\x77\xd4\xd5\x6d\
+\xf3\xce\x05\x0f\x75\x58\x1d\xaf\x11\x7c\xbe\xce\xab\xcf\xb5\xcd\
+\x8e\xda\xaf\x1e\x6c\x10\x7c\xbe\x0e\xab\x6b\xda\x82\x1f\x54\x4f\
+\xb7\x08\x3f\xab\x53\xea\xe6\xa6\xe1\xb7\xa9\x13\x6d\x93\xcf\xd1\
+\xa4\x7a\xff\x42\x58\x4a\x8f\x03\xd4\xfb\x80\xaf\x81\xe5\x8d\xba\
+\xde\x5d\x97\x80\x87\x22\xe2\x68\x6d\x06\xa8\x83\xc0\x37\xc0\xda\
+\xb6\x69\x73\xf4\x07\xf0\x40\x44\x1c\xaf\xdc\x00\x93\x57\xcf\x0f\
+\xc0\x6d\x6d\x53\x76\xd1\x29\xe0\x9e\x88\xf8\xb3\x48\xe3\x32\x23\
+\xac\x0f\xae\x02\x78\x80\x3b\x80\xf7\x8b\x36\x2e\x64\x80\x3a\x0c\
+\x3c\xdd\x36\x59\x09\x3d\xa3\xee\x2c\xd2\xb0\x6b\x0a\x98\xbc\x67\
+\x47\x81\x1b\xda\xa6\x2a\xa9\x71\x60\x20\x22\x2e\x76\x6a\x54\x24\
+\x02\x5e\xbd\x0a\xe1\x01\x36\x02\xaf\x74\x6b\xd4\x31\x02\xd4\x75\
+\xc0\x19\xfe\x9b\xb6\x2e\x46\x5f\x02\xa7\x81\x17\x1b\x34\xe1\x12\
+\x70\x6b\x44\x5c\xc8\x6b\xd0\x2d\x02\xf6\x54\x04\x0f\xf0\x77\x44\
+\xec\x01\x76\xa5\x1d\x6b\x42\x2b\x80\x17\x3a\x35\xc8\x35\xc0\x64\
+\x0e\xbe\xab\xea\x1e\x45\xc4\x27\xc0\x56\xe0\xc7\x86\x4c\xd8\x6d\
+\x87\x7a\x42\xa7\x08\xd8\x01\xdc\x5c\x47\x8f\x22\x62\x14\xd8\x06\
+\xec\x6b\xc0\x80\x5b\x80\xed\x0b\x31\xe0\xa9\x3a\x7b\x15\x11\xff\
+\x34\x98\x12\xb9\x2c\x9d\x0c\x78\xb0\xe6\x4e\xcd\x1a\xd1\x44\x4a\
+\x0c\x95\x32\x40\xbd\x91\xa4\x78\xd9\x88\xd2\x94\xb8\x17\xf8\xb8\
+\xa6\x4b\x0c\xaa\x99\xaf\xf2\xbc\x08\xd8\xd2\x14\xfc\x1c\x13\xfe\
+\x8a\x88\xdd\xc0\x30\xd5\xa7\x44\x00\x83\x65\x0c\x68\xec\xee\x67\
+\x18\xf1\x29\xf5\xa4\x44\x26\x53\x9e\x01\x9b\xda\x32\x20\x35\xa1\
+\x8e\x94\xc8\x9c\xc8\xe5\x19\xd0\xdf\xa6\x01\xa9\x09\x55\xa7\xc4\
+\xca\x32\x06\x54\x35\xfa\xab\xc2\x88\xaa\x52\xa2\x94\x01\xd7\x8c\
+\xf2\x0c\x98\x69\xbb\x63\xb3\x52\x9f\x07\xbe\x07\xee\x5e\xe4\x5f\
+\x4d\x67\xfd\xb8\x2c\xa7\xf1\xd4\x12\x00\x5f\x0e\xec\xa7\xba\xf9\
+\x48\x26\x53\x9e\x01\x63\x2d\xc3\x0f\x00\x5f\xb0\xf8\xbb\x3e\x57\
+\x67\xb2\x7e\xcc\x4b\x81\xd1\x16\xe1\xab\x0a\xf9\x42\x4c\x79\x11\
+\x30\x02\x48\xb3\xfb\x07\xaa\x0e\xf9\x2b\xfe\x1e\x38\x96\x75\x20\
+\x33\x02\xd2\xcd\x09\x27\x1a\x84\x1f\x00\x8e\xd6\x04\x0f\x70\x2c\
+\x22\x26\x0a\x1b\x90\xea\x48\x43\xf0\xc3\xd4\x13\xf2\x85\x58\x3a\
+\x19\x70\xb8\x66\xf0\xeb\xd4\xbd\x24\xc3\xdd\x15\x75\x5e\x0b\x38\
+\x94\x77\x60\x59\x87\x93\x8e\x00\xe7\xa8\xa1\x2a\x54\xd3\x53\x3e\
+\x4f\x67\x81\x6f\xf3\x0e\xe6\x46\x40\x44\x5c\x06\x3e\xaa\x01\xbe\
+\x89\x90\x9f\xab\x0f\x53\x96\x6c\xce\x2e\x9d\x5d\x4f\xf2\xfe\xac\
+\x22\x44\xbf\x02\x7e\xa7\xbe\x07\x5d\x96\xa6\x49\xca\xe2\x93\x79\
+\x0d\x3a\xce\x05\xd2\x7a\xfa\x7b\x15\x75\xe6\xb1\x86\xe1\x01\x0e\
+\x74\x82\x87\x62\x4b\x63\xfd\x24\x83\x88\x9b\x1a\xee\xfc\x62\x75\
+\x9e\x64\x69\xac\xe3\x2a\x71\xd7\xd9\x60\x44\x4c\x01\x2f\xb7\x4d\
+\xb3\x00\xbd\x54\x74\x89\xbc\x90\xd4\xcf\xda\xde\x07\x53\x42\x07\
+\x8b\x72\x95\xd9\x20\xb1\x8a\x64\x83\xc4\xed\x8d\xde\xc7\xf2\x3a\
+\x09\x6c\x4d\x23\xb7\xab\x0a\x17\x44\xd2\x70\x7a\x94\xe4\x49\xbe\
+\x54\x75\x01\x78\xa2\x28\x7c\x29\x03\x52\x13\x4e\x02\x4f\xd2\xdc\
+\xe2\x66\x19\xcd\x00\x8f\xa7\x05\xd5\xc2\x2a\x5d\x12\x4b\x77\x61\
+\x0d\x01\x13\x65\xcf\xad\x51\x93\xc0\x23\x11\xf1\x5d\x63\x57\x54\
+\x37\xab\xbf\xb4\xfd\xb4\x53\x7f\x56\xdb\x59\xc7\x50\x57\xaa\x9f\
+\xb7\x08\x7f\xc8\xa5\xb0\x71\x5a\xdd\xa9\xfe\xd6\x20\xf8\xaf\xea\
+\xb3\x6d\x73\xcf\x37\x61\x95\xfa\xb6\x3a\x5d\x23\xf8\x94\xfa\x96\
+\xc9\xe8\x74\x69\x4a\x5d\xa7\xbe\xae\x8e\x55\x08\x3e\xa6\xbe\xa6\
+\x2e\xd5\x1d\xaa\x99\x46\xf4\xa9\x43\xea\x3e\x75\xa4\x24\xf0\xe5\
+\xf4\x9c\xbd\xea\x76\x6b\xfc\x64\xa6\xc9\xa2\xe7\x06\x92\x1a\xc0\
+\x9d\x24\xdb\x56\xd6\x72\xe5\x47\x53\x93\x24\xc5\x8b\xd9\x8f\xa6\
+\x96\xd2\x6b\xb6\xa7\x9e\x7a\xea\xe9\xff\xa9\x7f\x01\x81\x26\x51\
+\x3c\x61\xb0\x0b\xa4\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\
+\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x36\
+\x2d\x30\x33\x54\x31\x39\x3a\x35\x31\x3a\x35\x38\x2b\x30\x30\x3a\
+\x30\x30\x69\xd8\x7c\x72\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\
+\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\
+\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x31\x3a\x35\x38\x2b\x30\x30\
+\x3a\x30\x30\x18\x85\xc4\xce\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
+\x42\x60\x82\
+\x00\x00\x04\x7b\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\xe1\x00\x00\x00\xe1\x08\x03\x00\x00\x00\x09\x6d\x22\x48\
+\x00\x00\x00\x75\x50\x4c\x54\x45\x00\x00\x00\xff\xff\xff\xe7\xe7\
+\xe7\xf2\xf2\xf2\x0b\x0b\x0b\xdd\xdd\xdd\xe3\xe3\xe3\xcb\xcb\xcb\
+\xf9\xf9\xf9\xbf\xbf\xbf\xae\xae\xae\xce\xce\xce\x8b\x8b\x8b\xe0\
+\xe0\xe0\xf5\xf5\xf5\x0f\x0f\x0f\xa3\xa3\xa3\x5b\x5b\x5b\x22\x22\
+\x22\x94\x94\x94\x71\x71\x71\xc4\xc4\xc4\x36\x36\x36\x1c\x1c\x1c\
+\x47\x47\x47\x18\x18\x18\xba\xba\xba\x8d\x8d\x8d\x4f\x4f\x4f\x62\
+\x62\x62\xd4\xd4\xd4\x82\x82\x82\x41\x41\x41\x69\x69\x69\x2b\x2b\
+\x2b\x9c\x9c\x9c\x7d\x7d\x7d\x4d\x4d\x4d\x2f\x2f\x2f\x8a\x37\xee\
+\x59\x00\x00\x03\xc1\x49\x44\x41\x54\x78\x9c\xed\xdd\x6b\x53\xea\
+\x40\x0c\x06\x60\x5b\xee\x20\x48\x05\x04\x41\x50\x41\xfd\xff\x3f\
+\xf1\x50\xe6\x78\x46\x93\xc0\x5e\xe8\x21\xbb\x99\xf7\xf9\x6c\x67\
+\x92\xa1\xdd\x6b\x76\xbd\xbb\x03\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x49\x75\
+\x3f\x1d\x8c\x3a\xdd\xb2\x2c\xc7\xbb\xde\x7a\xfa\x5a\x3d\x68\x47\
+\xd4\xa0\xa7\xcd\xa2\x55\x70\x93\xd1\xe1\x45\x3b\xb4\x26\xec\xa7\
+\xa5\x90\xdd\xb7\xfe\x60\xab\x1d\xe0\x95\xb6\xbb\x0b\xe9\xfd\x4d\
+\xf2\xd0\xd6\x8e\x32\x5e\xd5\x75\xe6\x77\x32\xd4\x0e\x34\xd2\x72\
+\xe4\x97\x5f\xed\x5e\x3b\xd8\x18\x1f\xfe\xf9\x1d\x8d\x1f\xb5\xe3\
+\x0d\x36\x08\x4a\xf0\xe8\x5d\x3b\xe2\x40\xe3\xd0\x04\x73\x7b\x53\
+\xa5\xfe\xcf\x69\xa6\x1d\x75\x80\xa8\x04\x8b\xe2\x55\x3b\x6e\x6f\
+\x9d\xb8\x04\x8b\x22\x97\x31\xce\x3a\x36\xc1\xa2\xaf\x1d\xba\x9f\
+\x79\x74\x82\x45\xb1\xd0\x0e\xde\xcb\x15\x09\xe6\xf1\x9e\x06\x77\
+\x84\xbf\x8c\xb5\xc3\x77\xfb\xbc\x2a\xc1\xa2\xa8\xb4\x13\x70\x3a\
+\x37\x99\x28\x07\xb3\x79\xb5\x5a\xad\xaa\xf9\x6c\x7d\x69\x38\x30\
+\xd2\x4e\xc0\x65\x25\xa7\xb7\x21\xc3\xce\x79\xef\x6c\x8a\xa9\xcf\
+\xa5\x16\x52\x7e\xd2\x2c\xf7\xf1\xdc\xf7\xba\xb9\x79\xcc\x41\xda\
+\x42\xc8\xd3\x33\x7f\xfb\xd2\xcf\xf1\x35\xbd\xe7\x11\x5f\x98\x33\
+\xc8\xeb\x1b\xb7\x8b\x36\x06\x6f\x67\x2e\xae\xc3\x4c\xa4\x0c\xdf\
+\x6e\x13\x6a\x24\x16\xee\xe5\xf9\xc2\x9b\x94\xe1\xc7\x8d\x62\x8d\
+\xc2\x06\x6c\x1d\xc7\x03\x43\x21\xc3\x73\xdf\x6d\x12\x58\xc0\x2b\
+\xd7\x13\x42\x86\x83\x5b\x44\x1a\x8b\x76\xe5\x3b\xe7\x13\x42\xef\
+\x92\x74\x63\x4a\x83\x75\xaf\xbd\x08\x13\x11\xd7\x9b\xad\xe9\x89\
+\x06\xeb\x7e\x64\xc9\x33\x4c\x79\xf0\xfd\x4e\x62\xed\x79\x3c\xc3\
+\xbb\xfd\xee\x7f\x8f\x33\xde\x86\xc4\xea\xb3\xb4\xc4\x7b\xfd\x94\
+\xdf\xd2\x29\x89\xd5\x67\x26\xc4\xd7\x74\xdc\xcd\x93\x1e\xba\x40\
+\xb3\xf7\x78\x86\x67\x98\xf2\x4a\x06\x6d\xfa\x7d\x9e\xe1\x9b\x37\
+\x29\xef\xd3\xac\xbb\xdd\x7a\x93\xb7\x2c\x5b\x47\x93\xc9\xc4\xe7\
+\x19\xbe\xb4\x9a\xf8\xf4\x29\x18\x4b\x30\x83\x75\x8c\x20\xac\x0b\
+\x4d\x7f\x92\x1f\xe8\x95\x25\x58\x6a\x87\xd4\x30\xbe\x96\x91\x72\
+\x43\x13\xc3\xfc\x67\xc8\x07\xde\x5e\x0d\x70\x46\x78\x7f\x9f\xf4\
+\xfc\x37\x5c\xc5\x5f\xd2\xa5\x76\x4c\xcd\xe2\xc3\xee\xb5\x76\x48\
+\xcd\xa2\x73\x91\xa3\x67\xed\x98\x1a\xf5\xc5\x13\x34\xf6\x15\xf2\
+\x77\xb4\xa5\x1d\x52\xb3\x84\xcd\x99\x1c\xf6\x47\xfd\x09\x4b\xa5\
+\xb6\xde\x51\xa1\x95\x49\x79\x72\x1f\x8e\x8f\xb8\x8d\x7d\x84\x52\
+\x59\x9f\xcf\x9a\x47\x36\xa4\x82\x14\xe7\x06\x40\x4e\xa4\x04\x4d\
+\x4d\x29\xb6\x42\x82\xb9\x97\x7b\xff\x22\x0c\xb7\x6d\xfd\x82\xd2\
+\xae\xa8\xa9\x04\x85\xad\x18\x5b\x09\x4a\xd5\x09\xb6\xc6\x6a\xc2\
+\x60\xf4\x53\x3b\xa6\x46\x09\xd5\x28\xb6\x7e\x41\x61\x46\x68\xeb\
+\x1b\x14\x16\x9e\xe6\xda\x21\x35\x8b\x8f\x46\xad\xed\xc2\xb0\x12\
+\x28\x63\xeb\x4e\xbc\x99\xb1\xb6\x45\xc1\x7f\xc2\x2f\xed\x88\x1a\
+\xf6\x4e\x13\xcc\xe9\x8c\x8c\x17\xda\xd9\xdb\x9a\xd3\xd7\xe8\x4f\
+\x98\xdb\x61\x35\x27\x3a\xed\x35\xd7\xcc\xb0\x52\x94\x7c\x8e\x71\
+\xf9\xa2\x93\x0a\xed\x78\x9a\x47\x12\xf4\xa9\x79\xcb\x0b\x3d\x88\
+\x91\xd7\x89\x51\x1f\x74\x4c\xfa\xa4\x1d\x50\xe3\x66\xe6\x3f\x43\
+\xb2\x11\x63\xaf\xaf\xa0\x9d\x85\xad\x5d\x98\x13\x52\xb7\x98\x72\
+\x89\x65\xa4\x9d\xf9\x0c\x97\xcb\xe7\xa3\x87\xa3\x76\x4d\x3b\x1c\
+\x00\x00\x00\x00\x00\x00\x00\xb8\xc2\x76\xd8\xeb\xec\x16\x07\x53\
+\x75\x96\x3f\x6d\xfe\x1d\x4c\x2f\xcd\x6d\xac\xd5\x1e\xba\xc6\x17\
+\xa2\x1e\xc9\xcd\x02\x29\x1f\xba\x8f\xc3\x0a\xf6\x92\xbe\xc1\x24\
+\x02\xbd\x8b\xa0\x30\x56\x15\x2c\x5e\x43\x93\xf2\xf5\x17\xe1\x84\
+\x92\xc4\xd4\xef\x83\x0a\x24\xde\x0a\x7d\xd0\x8e\xaa\x49\xe2\x9d\
+\xb4\xa6\xf6\xb9\xa5\x04\x93\xbe\x69\x27\x98\x98\xa1\xa9\x4d\x52\
+\xfb\xbf\xa1\x78\xb7\x9e\xa9\xef\x50\xbc\xd4\xd4\xd4\x79\x4a\x5a\
+\x88\x71\x62\xaa\x48\xff\x59\x48\xd0\x58\xf1\xa5\x70\xc5\xb7\xb5\
+\xca\x3d\xdb\x2d\x69\x8d\x1e\xc9\xeb\x1b\xbb\xff\xe2\x8e\x1e\xab\
+\x9c\x58\x2b\x62\xaf\xed\x7f\x1c\x98\xb1\x36\xfd\xfd\x56\x0d\x4e\
+\x23\xf0\x72\x68\xaf\x2e\xf1\x87\x7d\x7e\xff\x4f\x06\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\xe0\x96\xfe\x00\xef\xff\x1f\x4f\xab\x8f\xe8\xa8\x00\x00\
+\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
 \x00\x00\x04\x9d\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
 \x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
 \x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
 \x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
@@ -81,120 +370,67 @@
 \x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\
 \x65\x00\x32\x30\x32\x32\x2d\x30\x36\x2d\x30\x33\x54\x31\x39\x3a\
 \x35\x32\x3a\x31\x39\x2b\x30\x30\x3a\x30\x30\xa0\xd2\xc2\x3f\x00\
 \x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\
 \x66\x79\x00\x32\x30\x32\x32\x2d\x30\x36\x2d\x30\x33\x54\x31\x39\
 \x3a\x35\x32\x3a\x31\x39\x2b\x30\x30\x3a\x30\x30\xd1\x8f\x7a\x83\
 \x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x03\x6d\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
-\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
-\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
-\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
-\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
-\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
-\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
-\x6b\x42\xcf\x00\x00\x02\x6f\x49\x44\x41\x54\x78\xda\xed\x9a\x3f\
-\x6b\x14\x41\x18\x87\x1f\x4f\x09\xb1\x0b\x24\x95\x20\x84\x58\x68\
-\xa3\x10\x49\xa5\x41\xf0\x34\x0a\xd6\x62\xe1\x87\x10\xac\x6c\x2d\
-\xad\xc4\x6f\x60\x23\x16\x8a\x1f\x40\xd7\xa8\x10\x04\xb5\xd0\x46\
-\x88\x08\xd1\x42\xc1\x26\x01\xa3\x01\xff\x85\x9c\xc5\xec\x42\x38\
-\xde\xb9\xdd\xd9\x99\xb9\x99\xcb\xbd\x0f\x0c\xdc\x0d\x73\x77\xfb\
-\x7b\xee\x9d\xd9\xbb\x61\x40\x51\x14\x45\x51\x14\x45\x19\x4f\xf6\
-\x35\x1c\x73\x02\x98\x05\x26\x3c\x3e\xeb\x07\xf0\x38\x75\x60\x57\
-\x2e\x02\x1f\x80\x5e\xa0\x76\x33\x75\x20\x17\xae\x00\xdb\x01\xc3\
-\x8f\x94\x84\x19\x60\x33\x42\xf8\x91\x91\x70\x2d\x62\xf8\x91\x90\
-\x70\x77\x08\x02\x7a\xc0\xad\xd4\x41\x6d\x3c\x18\x92\x80\xd0\xed\
-\x1b\x70\x1f\x73\xd7\x1a\x4b\x01\x55\xfb\x03\x5c\x6d\x12\xb4\xe3\
-\x5d\x2b\x79\x32\x81\x99\xc6\xb5\x95\xb0\x57\x05\x54\x12\x6e\x8c\
-\xb3\x00\x80\x6e\xdd\x80\x03\x0e\x6f\xf6\x0a\xb8\x9d\x3a\x91\x23\
-\xbd\x90\x02\xbe\x00\x0f\x53\x27\x0a\xcd\x5e\x9f\x02\x2a\x40\x05\
-\xd4\xe0\xb2\x06\xd8\xe8\x02\xd3\xa9\x83\x38\xb2\x09\x3c\x09\x21\
-\x60\x3f\xf0\x08\x98\x4a\x9d\xc8\x91\x7b\x95\x00\xdf\x29\xb0\x30\
-\x82\xe1\x01\x8a\xea\x81\xaf\x80\x73\xa9\x93\xb4\xe4\xd9\x38\x0b\
-\x78\x0f\x7c\x0d\x21\x60\x12\x38\x95\x3a\x4d\x0b\x8a\xdd\x4f\x7c\
-\x04\x2c\x96\x12\xfa\x39\x82\xd9\x49\x4e\xdd\x16\x62\x0b\x90\xca\
-\x7f\x0d\xf8\xe4\xf1\x9e\x21\x59\x12\xfa\xfe\x02\x2b\x31\x05\x3c\
-\x4d\x9d\xba\xe6\xfa\x5e\x02\x5b\x21\x04\x4c\x01\x27\x85\xfe\xe5\
-\xd4\xa9\x4b\x26\x81\xd3\x42\x7f\xd1\xdf\xd1\x56\xc0\x59\xcc\x8f\
-\xa0\xdd\xec\x00\xcf\x53\x27\x2f\x59\x04\x0e\xc6\x14\x20\x95\xd7\
-\x5b\x60\x3d\x75\xf2\x92\xf3\x42\xdf\x46\x79\x8d\xd1\x04\xe4\x34\
-\xff\x25\x01\xcb\x98\x2a\xf5\x16\x70\x08\x38\x66\xf9\x80\x1c\x98\
-\x06\xe6\x85\xfe\x42\x1a\xdc\x46\x80\xf4\xed\xff\xc6\xac\xb0\x39\
-\xd0\xb5\xe4\x12\xbf\xa0\x50\x02\x56\x80\x5f\xa9\x93\x97\x48\xe5\
-\xff\x11\xf8\x1c\x4a\x80\xb4\xd3\x9a\x4b\xf9\xdb\x04\x14\xb6\xc1\
-\xae\x02\x8e\x02\x87\x85\xfe\x5c\x16\xc0\x59\x60\x2e\xa6\x00\xa9\
-\xfc\x37\x80\x77\xa9\x93\x97\x5c\x10\xfa\xb6\x81\x17\x31\x05\x88\
-\xb7\x97\x44\x48\xe5\xff\x1a\xb3\x05\xe6\x2d\xa0\x03\x9c\xb1\x08\
-\xc8\x81\x0e\xe6\x17\x6a\x3f\x45\xdd\x8b\x9a\x32\x8f\x39\x39\xd2\
-\x4f\x2e\xf3\xbf\xd5\xf5\xd9\x36\x45\xb7\x84\xbe\x39\xcb\xd8\xb5\
-\xd4\xc9\x07\xf0\x13\x78\x33\x68\x80\xad\x02\x72\x59\xd4\x7c\x29\
-\x80\x7f\x6d\x5e\x38\x03\x7c\x27\xfd\x41\x07\xdf\x76\xc9\xc7\xde\
-\x65\xe2\x1c\x93\x1b\x56\xbb\xe3\x13\xbe\x62\x09\x58\xcd\x20\x8c\
-\x4b\x5b\x07\xae\xd3\x70\x81\x6f\x72\x54\x16\xe0\x38\x66\x11\xf4\
-\x39\x2a\x1b\x9b\x1d\xcc\x7e\xe4\x2a\xe6\xcf\x99\xa2\x28\x8a\xa2\
-\x28\x8a\xa2\x0c\xe0\x3f\x94\xab\xaa\x38\x29\x07\x4f\xa2\x00\x00\
-\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\
-\x65\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x33\x54\x30\x39\x3a\
-\x30\x33\x3a\x31\x30\x2b\x30\x30\x3a\x30\x30\x41\xba\xb7\x88\x00\
-\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\
-\x66\x79\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x33\x54\x30\x39\
-\x3a\x30\x33\x3a\x31\x30\x2b\x30\x30\x3a\x30\x30\x30\xe7\x0f\x34\
-\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x02\xa4\
+\x00\x00\x02\xea\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
-\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
-\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
-\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
-\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
-\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
-\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
-\x6b\x42\xcf\x00\x00\x01\xa6\x49\x44\x41\x54\x78\xda\xed\xd7\xbf\
-\x2b\x86\x51\x18\xc6\xf1\xef\xcd\x9b\x92\x32\x28\x8b\xc1\x62\xb1\
-\x50\x62\x31\x28\x93\x4c\x36\x16\x24\x25\x36\xfc\x07\xf8\x0f\xb0\
-\x59\x29\x03\x13\x93\x0c\x52\x06\x94\x5f\x65\xb1\x58\x0c\x16\x65\
-\xb0\x58\xd4\x65\x78\x7b\xca\xc0\x20\xcf\x7b\xee\xa3\xf7\xfe\xfc\
-\x01\xcf\x39\xd7\xd5\xfd\x3c\xcf\x39\x10\x42\x08\x21\x84\x10\x42\
-\x08\x21\x84\xf0\x4b\x92\xf6\x24\xb5\x25\x58\x67\x5c\xdf\xf8\xeb\
-\x73\x1b\x4a\xd8\xdb\x38\x70\x2b\x69\xb8\xd6\x25\xd4\x42\x19\x05\
-\x00\x74\x02\x27\x92\x36\x24\x35\x79\x87\xf2\x28\x00\xc0\x80\x45\
-\xe0\x4a\x52\x8f\x77\x30\x8f\x02\x0a\x3d\xc0\xa5\xa4\x25\x49\xe6\
-\x1d\xd0\xa3\x00\x80\x66\x60\x1d\x38\x92\xd4\xe1\x1d\xd2\xa3\x80\
-\xc2\x08\x70\x27\x69\xcc\x3b\xa8\x57\x01\x00\xed\xc0\x81\xa4\x6d\
-\x49\x2d\xde\x81\x3d\x0a\x28\x4c\x53\xfd\x40\xf6\x7b\x87\xf6\x2a\
-\x00\xa0\x1b\xb8\x90\xb4\x2a\xa9\xd1\x3b\xbc\x47\x01\x00\x15\x60\
-\x05\x38\x93\xd4\x55\x8f\x05\x14\x06\x81\x1b\x49\xf3\xf5\x5a\x00\
-\x40\x2b\xb0\x95\xea\x3e\x91\x63\x01\x05\xb7\xfb\x44\x2e\x05\x80\
-\xd3\x7d\x22\xa7\x02\xc0\xe1\x3e\x91\x5b\x01\xc9\xe5\x56\x80\x80\
-\x4d\x60\xc0\xcc\xee\x53\x2c\x58\xf1\x4e\xfc\xc5\x13\x30\x63\x66\
-\xa7\x29\x17\xcd\x65\x02\xf6\x81\xbe\xd4\xe1\x73\x28\xe0\x0d\x58\
-\x30\xb3\x09\x33\x7b\xf5\xd8\x80\xe7\x2b\x70\x0e\x4c\x9b\xd9\xa3\
-\xe3\x1e\x5c\x26\xe0\x03\x58\x03\x86\xbc\xc3\x43\xfa\x09\x78\x00\
-\xa6\xcc\xec\xda\x3b\x78\x21\xe5\x04\xec\x50\xfd\xbd\x65\x13\x1e\
-\xd2\x4c\xc0\x0b\x30\x67\x66\x87\xde\x61\x3d\x0a\x38\x06\x66\xcd\
-\xec\xd9\x3b\xe8\x4f\x6a\xf5\x0a\xbc\x03\xcb\xc0\x68\xce\xe1\xa1\
-\x36\x13\x70\x0f\x4c\xa6\x3a\xca\xfe\x55\x99\x13\x90\xfc\x1c\x5f\
-\x86\xb2\x26\xc0\xe5\x1c\x5f\x86\x32\x26\x60\x17\xe8\xfd\x8f\xe1\
-\x43\x08\x21\x84\x10\x42\x08\x21\x84\x50\x9f\x3e\x01\x96\x0e\x92\
-\x34\x47\x8e\x42\xcf\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\
-\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x36\
-\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x32\x32\x2b\x30\x30\x3a\
-\x30\x30\x28\xaf\x41\x1b\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\
-\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\
-\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x32\x32\x2b\x30\x30\
-\x3a\x30\x30\x59\xf2\xf9\xa7\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
-\x42\x60\x82\
-\x00\x00\x03\x84\
+\x00\x00\x50\x00\x00\x00\x50\x08\x06\x00\x00\x00\x8e\x11\xf2\xad\
+\x00\x00\x00\xca\x69\x43\x43\x50\x43\x75\x73\x74\x6f\x6d\x00\x00\
+\x18\x95\x63\x60\x60\xdc\xce\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\
+\x45\x41\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\
+\x01\x37\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\
+\xe5\xc7\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\
+\x98\xcd\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\
+\xad\x03\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\
+\x03\xd9\x3e\x40\xb6\x40\x3a\x12\x3b\x09\x89\x9d\x92\x5a\x9c\x0c\
+\x64\xc7\x00\xd9\xd1\x08\xbf\xe5\xcf\x67\x60\xb0\xf8\xc2\xc0\xc0\
+\x3c\x11\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x6d\x84\x98\
+\xca\x42\x06\x06\xfe\x56\x06\x86\x6d\x57\x10\x62\x9f\x03\xc1\xfe\
+\x65\x14\x3b\x53\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\
+\x4a\x84\xfb\x8a\xc9\xd8\x08\x62\x2f\x2c\x8c\xa8\x0a\x00\x67\xd9\
+\x31\x35\xdc\xee\x19\x62\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\
+\x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\x00\x25\x74\
+\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\
+\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x35\x31\x3a\
+\x32\x36\x2b\x30\x30\x3a\x30\x30\x57\xdf\xca\x8c\x00\x00\x00\x25\
+\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\
+\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x35\x31\
+\x3a\x32\x36\x2b\x30\x30\x3a\x30\x30\x26\x82\x72\x30\x00\x00\x01\
+\x64\x49\x44\x41\x54\x78\x9c\xed\xdb\xbd\x4a\xc4\x40\x18\x46\xe1\
+\xa3\x9d\x08\xb9\x1a\xff\x2a\x0b\xb5\xf3\xe7\x7a\x05\x2b\x1b\xbd\
+\x12\x6d\x37\x82\x8a\x0a\xa2\x55\x60\x91\x35\x26\xf9\x3e\x26\xb3\
+\xee\x79\x60\xca\x90\x97\xc3\xb4\x03\x92\x24\x49\x52\xfd\x1a\xe0\
+\x06\x38\x9e\x7b\xc8\x3a\x6a\x80\x7b\xe0\x0b\x78\xc6\x88\xa3\x2c\
+\xc7\xeb\x8e\x11\x07\x5a\x15\xcf\x88\x03\xf5\xc5\x33\xe2\x1f\x86\
+\xc4\x33\xe2\x2f\xc6\xc4\x33\xe2\x0f\x0d\x70\xc7\xb8\x78\xdd\x79\
+\x04\x76\xca\x4f\xae\xc7\x94\x9b\xd7\x9d\x17\xe0\xa4\xfc\xe4\x7a\
+\x18\x2f\xc0\x78\x01\xc6\x0b\x88\xc6\x3b\x2d\x3f\xb9\x1e\xc6\x0b\
+\x30\x5e\x40\x24\xde\x2b\xc6\x0b\xc5\x3b\x2b\x3f\xb9\x1e\xc6\x0b\
+\x30\x5e\x80\xf1\x02\x22\xf1\xde\x80\xf3\xf2\x93\xeb\x61\xbc\x00\
+\xe3\x05\x18\x2f\xc0\x78\x01\x91\x78\xef\xc0\x45\xf9\xc9\xf5\x30\
+\x5e\x80\xf1\x02\xa2\xf1\x2e\xcb\x4f\xae\x87\xf1\x02\x8c\x17\x60\
+\xbc\x25\xdb\x13\xbe\xf9\x04\x3e\x02\xff\xdc\x0a\x7c\xfb\x6f\xec\
+\x02\xb7\x4c\xbf\x85\x57\xe5\x27\xd7\xc7\x88\x09\x8c\x98\xc0\x88\
+\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\
+\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\
+\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\
+\x20\xf2\xe0\xfa\x81\x0d\x7f\x70\xdd\x99\x72\x13\x17\xc0\xde\x1c\
+\x63\x6b\x35\x26\xe2\x02\xd8\x9f\x67\x66\xdd\x86\x44\x6c\x31\x5e\
+\xaf\xbe\x88\x2d\x70\x30\xdf\xb4\xf5\xb1\x2a\x62\x0b\x1c\xce\x39\
+\x6a\xdd\x2c\x47\x7c\xc2\x78\x93\x34\xc0\x35\x70\x34\xf7\x10\x49\
+\x92\x24\x6d\xb6\x6f\xa1\xa7\x43\x48\x8a\xcb\xd9\x64\x00\x00\x00\
+\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x02\xc0\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x50\x00\x00\x00\x50\x08\x06\x00\x00\x00\x8e\x11\xf2\xad\
 \x00\x00\x00\xca\x69\x43\x43\x50\x43\x75\x73\x74\x6f\x6d\x00\x00\
 \x18\x95\x63\x60\x60\xdc\xce\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\
 \x45\x41\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\
 \x01\x37\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\
 \xe5\xc7\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\
 \x98\xcd\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\
 \xad\x03\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\
@@ -203,91 +439,580 @@
 \x3c\x11\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x6d\x84\x98\
 \xca\x42\x06\x06\xfe\x56\x06\x86\x6d\x57\x10\x62\x9f\x03\xc1\xfe\
 \x65\x14\x3b\x53\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\
 \x4a\x84\xfb\x8a\xc9\xd8\x08\x62\x2f\x2c\x8c\xa8\x0a\x00\x67\xd9\
 \x31\x35\xdc\xee\x19\x62\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\
 \x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\x00\x25\x74\
 \x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\
-\x30\x32\x32\x2d\x30\x35\x2d\x32\x31\x54\x31\x33\x3a\x30\x37\x3a\
-\x32\x39\x2b\x30\x30\x3a\x30\x30\x73\xb6\xf7\xf1\x00\x00\x00\x25\
+\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x34\x39\x3a\
+\x35\x39\x2b\x30\x30\x3a\x30\x30\x79\x0b\x2c\x48\x00\x00\x00\x25\
 \x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\
-\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x31\x54\x31\x33\x3a\x30\x37\
-\x3a\x32\x39\x2b\x30\x30\x3a\x30\x30\x02\xeb\x4f\x4d\x00\x00\x01\
-\xfe\x49\x44\x41\x54\x78\x9c\xed\xda\x3d\x6e\x13\x41\x18\x87\xf1\
-\x1f\x08\x21\x6e\x40\xc5\x09\x80\xd4\xa9\x69\x1c\x51\x82\x22\x10\
-\x05\x0d\x12\x67\xe0\x14\x1c\x01\x9a\xc8\x05\x08\x41\x05\x34\x50\
-\x73\x0f\x24\x3e\x0e\x80\xe2\xc6\x81\xc2\x31\x44\xca\x7a\x77\xb0\
-\x67\x66\xdf\x8d\xe6\x91\xa6\xb1\xc6\xaf\xdf\xff\xb3\x9f\xb3\x5e\
-\x1a\x8d\x46\xa3\xd1\x68\x34\x86\xd9\xc3\x1c\x3f\xb0\xc4\xef\x4c\
-\xa3\x8b\x57\x85\xeb\xff\xe5\x4a\x62\xf8\x47\x78\x89\xab\x89\xf3\
-\x27\xc3\xe5\x84\x39\x7b\x2e\x68\x78\xd2\x04\x3c\x73\x41\xc3\x93\
-\x26\xe0\x4e\xf1\x2e\x46\xe4\x52\xc2\x9c\xa5\xf3\xa2\x9e\xe3\x4b\
-\xa6\x1e\x5e\x77\x7c\xb6\x8f\x1b\x03\xdf\x9b\xe1\x49\x42\xfd\x94\
-\x8c\xbd\x74\x9d\x59\x0f\x77\x2d\xba\x23\x33\x1c\xcb\x70\x15\x48\
-\x39\x04\xa2\x31\xc3\x3b\x5c\xcb\x51\x6c\x6a\x02\xb2\x86\x67\x5a\
-\x02\x0e\x6c\x0e\xbf\xc0\x8b\x6d\x8a\x4e\x45\xc0\x0c\x6f\x6d\x0e\
-\x7f\x1f\x1f\xb7\x29\x3c\x05\x01\x7d\xbb\xfd\x3a\xfc\xfb\x6d\x8b\
-\x47\x17\x50\x34\x3c\xb1\x05\x14\x0f\x4f\x5c\x01\x55\xc2\x13\x53\
-\x40\xb5\xf0\xc4\x13\x50\x35\x3c\xb1\x04\x54\x0f\x4f\xfa\x03\x91\
-\xd2\x1c\xe8\xbf\xce\xdf\xc3\x87\x81\x1a\x5f\x75\x2f\xac\x76\xa6\
-\xf4\x62\xa8\x6f\x61\x73\x8c\xbb\x19\x7f\x6b\x2b\x4a\x0a\x08\x1f\
-\x9e\x72\x02\x26\x11\x9e\x32\x02\x26\x13\x9e\xfc\x02\x26\x15\x9e\
-\xbc\x02\x4a\x86\x3f\xdc\x50\xb7\x97\x9a\xf7\x01\xa3\x5c\xe7\x87\
-\xa8\x25\x20\x64\x78\xea\x08\x08\x1b\x9e\xf2\x02\x42\x87\xa7\xac\
-\x80\xf0\xe1\x29\x27\x60\x12\xe1\x29\xb3\x18\xba\x8e\x37\x76\x5b\
-\xd8\x54\xa3\xc4\x1e\xf0\x13\x4f\xad\xfe\x52\x3b\xcb\x7a\xcb\x87\
-\x09\x4f\xb9\x43\x60\x8e\xc7\xfe\x49\x08\xb5\xdb\x9f\xa5\xe4\x49\
-\x70\x2d\xe1\x97\xa0\xe1\x29\xff\x40\x64\x8e\x4f\x56\x87\x45\x48\
-\x6a\xdc\x08\x85\x0d\x4f\xac\x67\x82\xa3\xd0\x04\x8c\xdd\xc0\xd8\
-\x34\x01\x63\x37\x30\x36\x29\x97\xc1\x13\xe7\x45\xed\x17\xe8\x65\
-\x57\xba\x7a\x3a\xc9\x51\xf8\xbb\x7c\xaf\xad\xd6\x1e\xdf\x86\xc2\
-\xa5\x1c\x02\x9f\x13\xe6\x44\x25\x4b\xef\xb7\xad\xee\xe5\xc7\xde\
-\x9a\xff\x3b\x16\xb8\x99\x43\x00\x3c\x90\xfe\x5e\x5e\x84\xb1\xc0\
-\xc3\x5c\xe1\xd7\xdc\xc2\x91\xd5\x39\x21\xe7\xeb\xf2\xb9\xc6\xf2\
-\xb4\xb7\xa3\xd3\x5e\x1b\x8d\x46\xa3\xd1\x68\x34\x7a\xf9\x03\xe9\
-\xbb\x8b\x97\x75\xe0\x93\x8a\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
-\x42\x60\x82\
-\x00\x00\x02\x37\
+\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x34\x39\
+\x3a\x35\x39\x2b\x30\x30\x3a\x30\x30\x08\x56\x94\xf4\x00\x00\x01\
+\x3a\x49\x44\x41\x54\x78\x9c\xed\xda\x31\x4a\x43\x51\x10\x46\xe1\
+\x63\xba\x34\x82\x3b\x89\xa9\x0c\x68\xba\xa8\x4b\xb6\xb2\xb4\x72\
+\x1b\x5a\xa9\x20\x86\x08\x82\x68\x63\x40\xd4\xa7\xef\xe6\x1f\x62\
+\xa2\xe7\x83\x29\x2f\x0c\x87\x29\x2f\x48\x92\x24\xa9\xc0\x04\x38\
+\x07\xf6\x7e\x7b\x91\x6d\x34\x01\xee\x81\x17\xe0\x12\x23\x36\x79\
+\x1f\x6f\x39\x46\xec\xe9\xab\x78\x46\xec\xe9\xbb\x78\x46\xfc\x41\
+\x9f\x78\x46\xec\xd0\x12\xcf\x88\x1f\x0c\x81\x6b\xda\xe2\x2d\xe7\
+\x02\xd8\x5d\xff\xca\x9b\xe7\x10\x78\x60\xb5\x88\x5e\xe2\x1b\x23\
+\x16\x30\x62\x81\x23\x8c\x18\x33\x62\x01\x23\x16\x30\x62\x01\x23\
+\x16\x98\x62\xc4\xd8\x14\x98\x63\xc4\x88\x11\x0b\x18\xb1\xc0\x0c\
+\x58\x60\xc4\x88\x11\x0b\x18\xb1\x80\x11\x0b\x18\xb1\xc0\x31\xf0\
+\x88\x11\x23\x46\x2c\x60\xc4\x02\x46\x2c\x60\xc4\x02\x27\x18\x31\
+\xb6\xd6\x88\x83\xaa\xad\x37\xc8\x4e\xf0\xf6\x09\x78\xae\x5a\x64\
+\x1b\x9d\xb2\xfa\xf5\xfd\xfb\x5f\x0f\xc6\x0b\x18\x2f\x60\xbc\x80\
+\xf1\x02\xc6\x0b\x18\x2f\x60\xbc\x80\xf1\x02\xc6\x0b\x18\x2f\x60\
+\xbc\x80\xf1\x02\xc6\x0b\x18\x2f\x60\xbc\x80\xf1\x02\xc6\x0b\x18\
+\x2f\x60\xbc\x80\xf1\x02\xc6\x0b\x18\x2f\x30\x04\xae\x30\x5e\x64\
+\x04\xdc\x60\xbc\x48\x4b\x44\xe3\x75\x18\x01\xb7\x18\x2f\xb2\x4f\
+\x77\x44\xe3\xf5\x34\xe6\x73\x44\xe3\x35\x1a\x03\x77\x18\x2f\x72\
+\x00\x9c\x61\x3c\x49\x92\x24\xe9\x6f\x7b\x05\xbd\x94\x43\x47\x66\
+\xec\x2a\x6b\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x11\xab\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x03\xd4\x00\x00\x03\xd8\x08\x03\x00\x00\x00\x0c\xc8\x41\xcd\
+\x00\x00\x00\xe1\x69\x43\x43\x50\x73\x52\x47\x42\x00\x00\x18\x95\
+\x63\x60\x60\x3c\xcd\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\x45\x41\
+\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\x01\x37\
+\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\xe5\xc7\
+\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\x98\xcd\
+\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\xad\x03\
+\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\x03\xd9\
+\x3e\x40\xb6\x42\x3a\x12\x3b\x09\x89\x9d\x92\x5a\x9c\x0c\x64\xe7\
+\x00\xd9\xf1\x08\xbf\xe5\xcf\x67\x60\xb0\xf8\xc2\xc0\xc0\x3c\x11\
+\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x1d\x84\x98\xca\x42\
+\x06\x06\xfe\x56\x06\x86\x6d\x97\x11\x62\x9f\xfd\xc1\xfe\x65\x14\
+\x3b\x54\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\x4a\x04\
+\x4b\x33\x83\x02\x34\x2d\x8d\x81\xe1\xd3\x72\x06\x06\xde\x48\x06\
+\x06\xe1\x0b\x0c\x0c\x5c\xd1\x10\x77\x80\x01\x6b\x31\x30\xa0\x49\
+\x0c\x27\x42\x00\x00\x72\xd8\x36\x84\xa3\x1f\x47\xb3\x00\x00\x00\
+\x57\x50\x4c\x54\x45\xff\xff\xff\xe8\xe8\xe8\x7f\x7f\x7f\x11\x11\
+\x11\xcc\xcc\xcc\x00\x00\x00\x15\x15\x15\xd1\xd1\xd1\x30\x30\x30\
+\x55\x55\x55\x88\x88\x88\x33\x33\x33\x66\x66\x66\x0a\x0a\x0a\xbe\
+\xbe\xbe\xbf\xbf\xbf\x0b\x0b\x0b\xc0\xc0\xc0\xc1\xc1\xc1\x0e\x0e\
+\x0e\xc7\xc7\xc7\x0f\x0f\x0f\xc8\xc8\xc8\xc9\xc9\xc9\x10\x10\x10\
+\xca\xca\xca\xcb\xcb\xcb\xff\xff\xff\x00\x00\x00\x2d\x21\xd7\x57\
+\x00\x00\x00\x1d\x74\x52\x4e\x53\x00\xff\xff\xff\xff\xff\xff\xff\
+\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\
+\xff\xff\xff\xff\x00\xce\xc7\xf9\x42\x00\x00\x00\x09\x70\x48\x59\
+\x73\x00\x00\x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\
+\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\
+\x65\x00\x32\x30\x31\x37\x2d\x30\x36\x2d\x31\x32\x54\x30\x33\x3a\
+\x33\x34\x3a\x35\x31\x2b\x30\x38\x3a\x30\x30\x84\x9a\x03\x36\x00\
+\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\
+\x66\x79\x00\x32\x30\x31\x36\x2d\x30\x34\x2d\x31\x36\x54\x31\x35\
+\x3a\x35\x32\x3a\x31\x38\x2b\x30\x38\x3a\x30\x30\x8b\xf9\x5a\xba\
+\x00\x00\x00\x58\x7a\x54\x58\x74\x73\x76\x67\x3a\x62\x61\x73\x65\
+\x2d\x75\x72\x69\x00\x00\x08\x99\x4b\xcb\xcc\x49\xb5\xd2\xd7\xd7\
+\xcf\xc8\xcf\x4d\xd5\x4f\x49\xd2\x2f\x2e\x4b\x8f\xcf\xcc\x4b\xcb\
+\x07\x31\xf4\x4d\x8d\xf5\x4d\x4d\x80\xa4\xa9\x49\x9a\x91\x79\x92\
+\xa9\x81\xa1\xb1\x99\x79\xb2\x59\x8a\xb1\x71\xb2\xb9\xa1\xb1\x85\
+\x79\x9a\x45\x92\xb1\x41\xa2\xb1\x1e\x50\x29\x00\x17\x9a\x14\xea\
+\xbe\x3f\x86\x2f\x00\x00\x0f\x1e\x49\x44\x41\x54\x78\x9c\xed\xdb\
+\x59\x8e\x2b\xc7\x15\x45\x51\xb9\xd4\xd9\xcf\x7d\x6f\x6b\xfe\x03\
+\x35\x04\x43\xd2\x6b\xaa\x8a\xd9\x31\x23\x62\x6b\xad\x11\x9c\xfb\
+\xb1\x41\x82\x99\xfc\xea\x2b\x7e\x15\x7e\x33\x7a\x00\x70\xa9\x6f\
+\xbe\x7e\x19\x3d\x01\xb8\xd0\x37\x5f\x7f\xfb\xad\xaa\xa1\xe3\xc7\
+\xa6\x55\x0d\x1d\xff\x6f\x5a\xd5\x50\xf1\x53\xd3\xaa\x86\x86\x5f\
+\x9a\x56\x35\x14\x7c\xdc\xb4\xaa\x61\x7d\x9f\x36\xad\x6a\x58\xdd\
+\xe7\x4d\xab\x1a\xd6\xf6\x65\xd3\xaa\x86\x95\xbd\xd6\xb4\xaa\x61\
+\x5d\xaf\x37\xad\x6a\x58\xd5\x5b\x4d\xab\x1a\xd6\xf4\x76\xd3\xaa\
+\x86\x15\xbd\xd7\xb4\xaa\x61\x3d\xef\x37\xad\x6a\x58\xcd\xa3\xa6\
+\x55\x0d\x6b\x79\xdc\xb4\xaa\x61\x25\x5b\x9a\x56\x35\xac\x63\x5b\
+\xd3\xaa\x86\x55\x6c\x6d\x5a\xd5\xb0\x86\xed\x4d\xab\x1a\x56\xb0\
+\xa7\x69\x55\xc3\xfc\xf6\x35\xad\x6a\x98\xdd\xde\xa6\x55\x0d\x73\
+\xdb\xdf\xb4\xaa\x61\x66\x47\x9a\x56\x35\xcc\xeb\x58\xd3\xaa\x86\
+\x59\x1d\x6d\x5a\xd5\x30\xa7\xe3\x4d\xab\x1a\x66\x74\xa6\x69\x55\
+\xc3\x7c\xce\x35\xad\x6a\x98\xcd\xd9\xa6\x55\x0d\x73\x39\xdf\xb4\
+\xaa\x61\x26\x57\x34\xad\x6a\x98\xc7\x35\x4d\xab\x1a\x66\x71\x55\
+\xd3\xaa\x86\x39\x5c\xd7\xb4\xaa\x61\x06\x57\x36\xad\x6a\x18\xef\
+\xda\xa6\x55\x0d\xa3\x5d\xdd\xb4\xaa\x61\xac\xeb\x9b\x56\x35\x8c\
+\xf4\x8c\xa6\x55\x0d\xe3\x3c\xa7\x69\x55\xc3\x28\xcf\x6a\x5a\xd5\
+\x30\xc6\xf3\x9a\x56\x35\x8c\xf0\xcc\xa6\x55\x0d\xf7\x7b\x6e\xd3\
+\xaa\x86\xbb\x3d\xbb\x69\x55\xc3\xbd\x9e\xdf\xb4\xaa\xe1\x4e\x77\
+\x34\xad\x6a\xb8\xcf\x3d\x4d\xab\x1a\xee\x72\x57\xd3\xaa\x86\x7b\
+\xdc\xd7\xb4\xaa\xe1\x0e\x77\x36\xad\x6a\x78\xbe\x7b\x9b\x56\x35\
+\x3c\xdb\xdd\x4d\xab\x1a\x9e\xeb\xfe\xa6\x55\x0d\xcf\x34\xa2\x69\
+\x55\xc3\xf3\x8c\x69\x5a\xd5\xf0\x2c\xa3\x9a\x56\x35\x3c\xc7\xb8\
+\xa6\x55\x0d\xcf\x30\xb2\x69\x55\xc3\xf5\xc6\x36\xad\x6a\xb8\xda\
+\xe8\xa6\x55\x0d\xd7\x1a\xdf\xb4\xaa\xe1\x4a\x33\x34\xad\x6a\xb8\
+\xce\x1c\x4d\xab\x1a\xae\x32\x4b\xd3\xaa\x86\x6b\xcc\xd3\xb4\xaa\
+\xe1\x0a\x33\x35\xad\x6a\x38\x6f\xae\xa6\x55\x0d\x67\xcd\xd6\xb4\
+\xaa\xe1\x9c\xf9\x9a\x56\x35\x9c\x31\x63\xd3\xaa\x86\xe3\xe6\x6c\
+\x5a\xd5\x70\xd4\xac\x4d\xab\x1a\x8e\x99\xb7\x69\x55\xc3\x11\x33\
+\x37\xad\x6a\xd8\x6f\xee\xa6\x55\x0d\x7b\xcd\xde\xb4\xaa\x61\x9f\
+\xf9\x9b\x56\x35\xec\xb1\x42\xd3\xaa\x86\xed\xd6\x68\x5a\xd5\xb0\
+\xd5\x2a\x4d\xab\x1a\xb6\x59\xa7\x69\x55\xc3\x26\xdf\x7f\x37\x3a\
+\xd5\x1d\x54\x0d\x1b\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
+\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
+\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
+\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
+\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
+\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
+\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
+\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
+\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
+\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
+\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
+\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
+\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\
+\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
+\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
+\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
+\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\
+\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
+\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
+\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
+\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
+\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
+\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
+\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
+\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
+\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
+\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
+\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
+\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
+\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
+\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
+\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
+\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
+\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\
+\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
+\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
+\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
+\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\
+\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
+\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
+\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
+\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
+\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
+\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
+\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
+\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
+\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
+\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
+\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
+\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
+\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
+\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
+\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
+\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\xcd\
+\xaf\xb3\xea\xdf\x41\xd8\x6f\x47\x97\xba\xc7\x55\x55\x8f\xbe\x03\
+\xf8\xc9\x45\x55\x8f\x3e\x03\xf8\xd9\x35\x55\x8f\xbe\x02\xf8\xc5\
+\x25\x55\x8f\x3e\x02\xf8\xc8\x15\x55\x8f\xbe\x01\xf8\xd8\x05\x55\
+\x8f\x3e\x01\xf8\xc4\xf9\xaa\x47\x5f\x00\x7c\xea\x74\xd5\xa3\x0f\
+\x00\x3e\x73\xb6\xea\xd1\xfb\x81\xcf\x9d\xac\x7a\xf4\x7c\xe0\x0b\
+\xe7\xaa\x1e\xbd\x1e\xf8\xd2\xa9\xaa\x47\x8f\x07\x5e\x71\xa6\xea\
+\xd1\xdb\x81\xd7\x9c\xa8\x7a\xf4\x74\xe0\x55\xc7\xab\x1e\xbd\x1c\
+\x78\xdd\xe1\xaa\x47\x0f\x07\xde\x70\xb4\xea\xd1\xbb\x81\xb7\x1c\
+\xac\x7a\xf4\x6c\xe0\x4d\xc7\xaa\x1e\xbd\x1a\x78\xdb\xa1\xaa\x47\
+\x8f\x06\xde\x71\xa4\xea\xd1\x9b\x81\xf7\x1c\xa8\x7a\xf4\x64\xe0\
+\x5d\xfb\xab\x1e\xbd\x18\x78\xdf\xee\xaa\x47\x0f\x06\x1e\xd8\x5b\
+\xf5\xe8\xbd\xc0\x23\x3b\xab\x1e\x3d\x17\x78\x68\x5f\xd5\xa3\xd7\
+\x02\x8f\xed\xaa\x7a\xf4\x58\x60\x83\x3d\x55\x8f\xde\x0a\x6c\xb1\
+\xa3\xea\xd1\x53\x81\x4d\xb6\x57\x3d\x7a\x29\xb0\xcd\xe6\xaa\x47\
+\x0f\x05\x36\xda\x5a\xf5\xe8\x9d\xc0\x56\x1b\xab\x1e\x3d\x13\xd8\
+\x6c\x5b\xd5\xa3\x57\x02\xdb\x6d\xaa\x7a\xf4\x48\x60\x87\x2d\x55\
+\x8f\xde\x08\xec\xb1\xa1\xea\xd1\x13\x81\x5d\x1e\x57\x3d\x7a\x21\
+\xb0\xcf\xc3\xaa\x47\x0f\x04\x76\x7a\x54\xf5\xe8\x7d\xc0\x5e\x0f\
+\xaa\x1e\x3d\x0f\xd8\xed\xfd\xaa\x47\xaf\x03\xf6\x7b\xb7\xea\xd1\
+\xe3\x80\x03\xde\xab\x7a\xf4\x36\xe0\x88\x77\xaa\x1e\x3d\x0d\x38\
+\xe4\xed\xaa\x47\x2f\x03\x8e\x79\xb3\xea\xd1\xc3\x80\x83\xde\xaa\
+\x7a\xf4\x2e\xe0\xa8\x37\xaa\x1e\x3d\x0b\x38\xec\xf5\xaa\x47\xaf\
+\x02\x8e\x7b\xb5\xea\xd1\xa3\x80\x13\x5e\xab\x7a\xf4\x26\xe0\x8c\
+\x57\xaa\x1e\x3d\x09\x38\xe5\xcb\xaa\x47\x2f\x02\xce\xf9\xa2\xea\
+\xd1\x83\x80\x93\x3e\xaf\x7a\xf4\x1e\xe0\xac\x17\x51\x43\xcc\x8b\
+\xa8\x21\xe6\x45\xd4\x10\xf3\x22\x6a\x88\x79\x11\x35\xc4\xbc\x88\
+\x1a\x62\x5e\x44\x0d\x31\x2f\xa2\x86\x98\x17\x51\x43\xcc\x8b\xa8\
+\x21\xe6\x45\xd4\x10\xf3\x22\x6a\x88\x79\x11\x35\xc4\xbc\x88\x1a\
+\x5a\x3e\x88\x1a\x52\x3e\xf8\xfa\x0d\x29\x1f\xfc\x50\x06\x29\x1f\
+\x3c\xd2\x82\x94\x0f\x5e\x3e\x81\x94\x0f\x5e\x13\x85\x94\x0f\xfe\
+\xd0\x01\x29\x3f\x35\x2d\x6a\x68\xf8\xb9\x69\x51\x43\xc2\x2f\x4d\
+\x8b\x1a\x0a\x3e\x6a\x5a\xd4\x10\xf0\x71\xd3\xa2\x86\xf5\x7d\xd2\
+\xb4\xa8\x61\x79\x9f\x36\x2d\x6a\x58\xdd\x67\x4d\x8b\x1a\x16\xf7\
+\x79\xd3\xa2\x86\xb5\x7d\xd1\xb4\xa8\x61\x69\x5f\x36\x2d\x6a\x58\
+\xd9\x2b\x4d\x8b\x1a\x16\xf6\x5a\xd3\xa2\x86\x75\xbd\xda\xb4\xa8\
+\x61\x59\xaf\x37\x2d\x6a\x58\xd5\x1b\x4d\x8b\x1a\x16\xf5\x56\xd3\
+\xa2\x86\x35\xbd\xd9\xb4\xa8\x61\x49\x6f\x37\x2d\x6a\x58\xd1\x3b\
+\x4d\x8b\x1a\x16\xf4\x5e\xd3\xa2\x86\xf5\xbc\xdb\xb4\xa8\x61\x39\
+\xef\x37\x2d\x6a\x58\xcd\x83\xa6\x45\x0d\x8b\x79\xd4\xb4\xa8\x61\
+\x2d\x0f\x9b\x16\x35\x2c\xe5\x71\xd3\xa2\x86\x95\x6c\x68\x5a\xd4\
+\xb0\x90\x2d\x4d\x8b\x1a\xd6\xb1\xa9\x69\x51\xc3\x32\xb6\x35\x2d\
+\x6a\x58\xc5\xc6\xa6\x45\x0d\x8b\xd8\xda\xb4\xa8\x61\x0d\x9b\x9b\
+\x16\x35\x2c\x61\x7b\xd3\xa2\x86\x15\xec\x68\x5a\xd4\xb0\x80\x3d\
+\x4d\x8b\x1a\xe6\xb7\xab\x69\x51\xc3\xf4\xf6\x35\x2d\x6a\x98\xdd\
+\xce\xa6\x45\x0d\x93\xdb\xdb\xb4\xa8\x61\x6e\xbb\x9b\x16\x35\x4c\
+\x6d\x7f\xd3\xa2\x86\x99\x1d\x68\x5a\xd4\x30\xb1\x23\x4d\x8b\x1a\
+\xe6\x75\xa8\x69\x51\xc3\xb4\x8e\x35\x2d\x6a\x98\xd5\xc1\xa6\x45\
+\x0d\x93\x3a\xda\xb4\xa8\x61\x4e\x87\x9b\x16\x35\x4c\xe9\x78\xd3\
+\xa2\x86\x19\x9d\x68\x5a\xd4\x30\xa1\x33\x4d\x8b\x1a\xe6\x73\xaa\
+\x69\x51\xc3\x74\xce\x35\x2d\x6a\x98\xcd\xc9\xa6\x45\x0d\x93\x39\
+\xdb\xb4\xa8\x61\x2e\xa7\x9b\x16\x35\x4c\xe5\x7c\xd3\xa2\x86\x99\
+\x5c\xd0\xb4\xa8\x61\x22\x57\x34\x2d\x6a\x98\xc7\x25\x4d\x7f\xf5\
+\x07\x28\xfb\xfd\xe8\x4e\xf7\x78\xb9\xa4\x69\x48\xfb\xd3\x1f\x47\
+\x87\xba\xc3\x35\x9f\xd3\x90\xa6\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
+\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
+\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
+\x45\xd3\xd0\xf2\x67\x4d\x43\xca\x9f\xff\x32\x3a\xd4\x1d\x34\x0d\
+\x0f\x69\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
+\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
+\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
+\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
+\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xf2\x57\
+\x4d\x43\x8a\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\
+\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\
+\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\
+\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
+\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xf2\x37\x4d\
+\x43\x8a\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\xe5\x1f\x7f\x1f\x1d\xea\x0e\x9a\x86\x87\x34\x0d\x2d\x9a\
+\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
+\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
+\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
+\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xf9\xc7\x3f\x47\x87\
+\xba\x83\xa6\xe1\x21\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
+\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
+\xa1\x45\xd3\xd0\xf2\x2f\x4d\x43\x8a\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
+\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
+\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
+\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
+\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
+\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\xcb\xbf\x35\x0d\x29\
+\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
+\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
+\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
+\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\xcb\xbf\xff\x33\x3a\xd4\
+\x1d\x34\x0d\x0f\x69\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
+\x2d\x9a\x86\x16\x4d\x43\xcb\x7f\x35\x0d\x29\x9a\x86\x16\x4d\x43\
+\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
+\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
+\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
+\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
+\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
+\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
+\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x7e\xd0\x34\xa4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
+\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
+\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x96\x1f\xbe\x1e\
+\x1d\xea\x0e\x9a\x86\x87\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
+\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
+\x9a\x86\x16\x4d\x43\xcb\x37\x9a\x86\x14\x4d\x43\x8b\xa6\xa1\x45\
+\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
+\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
+\xa2\x69\x88\xf9\xfe\xbb\xd1\xa5\x6e\xa7\x69\xd8\x62\x9d\xaa\x35\
+\x0d\xdb\xac\x52\xb5\xa6\x61\xab\x35\xaa\xd6\x34\x6c\xb7\x42\xd5\
+\x9a\x86\x3d\xe6\xaf\x5a\xd3\xb0\xcf\xec\x55\x6b\x1a\xf6\x9a\xbb\
+\x6a\x4d\xc3\x7e\x33\x57\xad\x69\x38\x62\xde\xaa\x35\x0d\xc7\xcc\
+\x5a\xb5\xa6\xe1\xa8\x39\xab\xd6\x34\x1c\x37\x63\xd5\x9a\x86\x33\
+\xe6\xab\x5a\xd3\x70\xce\x6c\x55\x6b\x1a\xce\x9a\xab\x6a\x4d\xc3\
+\x79\x33\x55\xad\x69\xb8\xc2\x3c\x55\x6b\x1a\xae\x31\x4b\xd5\x9a\
+\x86\xab\xcc\x51\xb5\xa6\xe1\x3a\x33\x54\xad\x69\xb8\xd2\xf8\xaa\
+\x35\x0d\xd7\x1a\x5d\xb5\xa6\xe1\x6a\x63\xab\xd6\x34\x5c\x6f\x64\
+\xd5\x9a\x86\x67\x18\x57\xb5\xa6\xe1\x39\x46\x55\xad\x69\x78\x96\
+\x31\x55\x6b\x1a\x9e\x67\x44\xd5\x9a\x86\x67\xba\xbf\x6a\x4d\xc3\
+\x73\xdd\x5d\xb5\xa6\xe1\xd9\xee\xad\x5a\xd3\xf0\x7c\x77\x56\xad\
+\x69\xb8\xc3\x7d\x55\x6b\x1a\xee\x71\x57\xd5\x9a\x86\xbb\xdc\x53\
+\xb5\xa6\xe1\x3e\x77\x54\xad\x69\xb8\xd3\xf3\xab\xd6\x34\xdc\xeb\
+\xd9\x55\x6b\x1a\xee\xf6\xdc\xaa\x35\x0d\xf7\x7b\x66\xd5\x9a\x86\
+\x11\x9e\x57\xb5\xa6\x61\x8c\x67\x55\xad\x69\x18\xe5\x39\x55\x6b\
+\x1a\xc6\x79\x46\xd5\x9a\x86\x91\xae\xaf\x5a\xd3\x30\xd6\xd5\x55\
+\x6b\x1a\x46\xbb\xb6\x6a\x4d\xc3\x78\x57\x56\xad\x69\x98\xc1\x75\
+\x55\x6b\x1a\xe6\x70\x55\xd5\x9a\x86\x59\x5c\x53\xb5\xa6\x61\x1e\
+\x57\x54\xad\x69\x98\xc9\xf9\xaa\x35\x0d\x73\x39\x5b\xb5\xa6\x61\
+\x36\xe7\xaa\xd6\x34\xcc\xe7\x4c\xd5\x9a\x86\x19\x1d\xaf\x5a\xd3\
+\x30\xa7\xa3\x55\x6b\x1a\x66\x75\xac\x6a\x4d\xc3\xbc\x8e\x54\xad\
+\x69\x98\xd9\xfe\xaa\x35\x0d\x73\xdb\x5b\xb5\xa6\x61\x76\xfb\xaa\
+\xd6\x34\xcc\x6f\x4f\xd5\x9a\x86\x15\x6c\xaf\x5a\xd3\xb0\x86\xad\
+\x55\x6b\x1a\x56\xb1\xad\x6a\x4d\xc3\x3a\xb6\x54\xad\x69\x58\xc9\
+\xe3\xaa\x35\x0d\x6b\x79\x54\xb5\xa6\x61\x35\xef\x57\xad\x69\x58\
+\xcf\x7b\x55\x6b\x1a\x56\xf4\x76\xd5\x9a\x86\x35\xbd\x55\xb5\xa6\
+\x61\x55\xaf\x57\xad\x69\x58\xd7\x6b\x55\x6b\x1a\x56\xf6\x65\xd5\
+\x9a\x86\xb5\x7d\x5e\xb5\xa6\x61\x75\x9f\x56\xad\x69\x58\xdf\xc7\
+\x55\x6b\x1a\x0a\x7e\xa9\x5a\xd3\xd0\xf0\x53\xd5\x9a\x86\x8a\xff\
+\x57\xad\x69\xe8\xf8\xb1\x6a\x4d\x43\xc9\xf7\xdf\x69\x1a\x5a\x7e\
+\x33\x7a\x00\xb7\xf9\x1f\x60\x09\x80\x64\x76\x94\x1f\xe0\x00\x00\
+\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x0f\xc6\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x03\xd4\x00\x00\x03\xd8\x08\x03\x00\x00\x00\x0c\xc8\x41\xcd\
 \x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
-\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
-\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
-\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
-\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
-\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
-\x6b\x42\xcf\x00\x00\x01\x39\x49\x44\x41\x54\x78\xda\xed\x9a\x4d\
-\x0a\xc2\x30\x10\x85\x9f\x5e\x46\x10\xef\x61\x29\xe8\xfd\x4f\x20\
-\x78\x02\x75\x55\x37\xcd\xa6\xf4\xcf\x9a\xbc\xcc\x4c\xdf\x07\xdd\
-\x48\x61\x7c\x5f\x42\x9b\x4c\x03\x08\x21\x84\x10\x42\x08\x21\x84\
-\xd8\xc4\x19\x40\x53\xa1\x6e\xd3\xd7\xae\xca\x09\xc0\x03\xc0\x07\
-\xc0\x9d\x1c\xfe\x05\xe0\x09\xe0\x52\x3b\x7c\xd7\x5f\x2c\x09\x29\
-\x7c\xaa\x5b\x45\xc2\x30\x3c\x4b\xc2\x30\x7c\x35\x09\x0d\x80\xf7\
-\xc8\x1f\xe9\xfa\xdf\xdb\x02\x35\xdb\x85\x9a\xf4\xe7\xd0\x15\xe3\
-\xa3\x51\x62\x26\x4c\x8d\x7c\xaa\x75\x63\x87\x67\x4a\x30\x1b\x9e\
-\x21\xc1\x7c\xf8\x92\x12\xdc\x84\x2f\x21\xc1\x5d\xf8\x9c\x12\xdc\
-\x86\xcf\x21\xc1\x7d\xf8\x7f\x24\x84\x09\xbf\x45\x42\xb8\xf0\xbf\
-\x48\x08\x1b\x3e\xb1\xb4\x84\x65\x2f\xa9\xab\x30\x37\x13\xc2\x8e\
-\xfc\x56\x09\x21\xc3\xaf\x95\x40\x0f\x7f\x24\x0b\x38\x64\xba\xc7\
-\x25\x73\x4f\x7b\x66\x53\xc5\x74\xf8\x90\x12\x76\xfd\x1a\x5c\xb3\
-\xc8\x61\x76\x96\xcc\x85\x4f\x84\x93\xb0\x65\x79\x1b\x46\xc2\x3f\
-\x6b\x7b\xf7\x12\x72\x6c\x6c\xdc\x4a\xc8\xb9\xab\x73\x27\xa1\xc4\
-\x96\xd6\x8d\x84\x92\xfb\x79\xf3\x12\x18\xcd\x0c\xb3\x12\x98\x9d\
-\x1c\x73\x12\x76\xff\x71\x74\xee\xf3\x78\xc9\xfd\xfc\xd4\x4c\x30\
-\x71\x46\x80\xd5\xcc\x18\x4a\x30\x71\x4a\x84\xdd\xc9\x49\x12\xaa\
-\x86\x4f\xec\xfa\x90\x94\x10\x42\x08\x21\x84\x10\x42\xb8\xe4\x0b\
-\x51\xb4\xd2\xe4\x46\xbd\x95\xba\x00\x00\x00\x25\x74\x45\x58\x74\
-\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\
-\x2d\x30\x35\x2d\x32\x33\x54\x31\x34\x3a\x31\x39\x3a\x35\x32\x2b\
-\x30\x30\x3a\x30\x30\x5e\xe0\x66\x5a\x00\x00\x00\x25\x74\x45\x58\
-\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\
-\x32\x2d\x30\x35\x2d\x32\x33\x54\x31\x34\x3a\x31\x39\x3a\x35\x32\
-\x2b\x30\x30\x3a\x30\x30\x2f\xbd\xde\xe6\x00\x00\x00\x00\x49\x45\
-\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x00\x01\x73\x52\x47\x42\x00\xae\xce\x1c\xe9\x00\x00\x00\
+\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\x00\x00\xfa\
+\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\x00\x00\x3a\
+\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x54\x50\x4c\x54\
+\x45\xff\xff\xff\xe8\xe8\xe8\x7f\x7f\x7f\x11\x11\x11\xcc\xcc\xcc\
+\x00\x00\x00\x15\x15\x15\xd1\xd1\xd1\x30\x30\x30\x55\x55\x55\x88\
+\x88\x88\x33\x33\x33\x66\x66\x66\x0a\x0a\x0a\xbe\xbe\xbe\xbf\xbf\
+\xbf\x0b\x0b\x0b\xc0\xc0\xc0\xc1\xc1\xc1\x0e\x0e\x0e\xc7\xc7\xc7\
+\x0f\x0f\x0f\xc8\xc8\xc8\xc9\xc9\xc9\x10\x10\x10\xca\xca\xca\xcb\
+\xcb\xcb\xff\xff\xff\xef\x09\x36\x35\x00\x00\x00\x01\x74\x52\x4e\
+\x53\x00\x40\xe6\xd8\x66\x00\x00\x00\x01\x62\x4b\x47\x44\x00\x88\
+\x05\x1d\x48\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x00\x48\x00\
+\x00\x00\x48\x00\x46\xc9\x6b\x3e\x00\x00\x0d\xf3\x49\x44\x41\x54\
+\x78\xda\xed\xd5\x09\xae\xed\x46\x19\x46\x51\xe7\x25\x2f\x81\x43\
+\x17\xfa\x66\xfe\x03\x05\x21\x14\x01\x69\xae\xed\x63\xbb\xaa\x76\
+\xd6\x1a\xc1\x5f\x9f\xb4\x55\xdb\xc6\xcf\xc5\x17\xa3\x0f\x00\x2e\
+\xf5\xe9\xcb\xaf\x46\x9f\x00\x5c\xe8\xd3\xe7\xcf\xaa\x86\x90\x7f\
+\x35\xad\x6a\x08\xf9\x77\xd3\xaa\x86\x8c\xff\x34\xad\x6a\x88\xf8\
+\xae\x69\x55\x43\xc2\x7f\x35\xad\x6a\x08\xf8\x9f\xa6\x55\x0d\xcb\
+\xfb\xbf\xa6\x55\x0d\x8b\xfb\x5e\xd3\xaa\x86\xa5\xfd\x40\xd3\xaa\
+\x86\x85\xfd\x60\xd3\xaa\x86\x65\xfd\x48\xd3\xaa\x86\x45\xfd\x68\
+\xd3\xaa\x86\x25\xfd\x44\xd3\xaa\x86\x05\xfd\x64\xd3\xaa\x86\xe5\
+\x7c\xd0\xb4\xaa\x61\x31\x1f\x36\xad\x6a\x58\xca\x8e\xa6\x55\x0d\
+\x0b\xd9\xd5\xb4\xaa\x61\x19\x3b\x9b\x56\x35\x2c\x62\x77\xd3\xaa\
+\x86\x25\x1c\x68\x5a\xd5\xb0\x80\x43\x4d\xab\x1a\xa6\x77\xb0\x69\
+\x55\xc3\xe4\x0e\x37\xad\x6a\x98\xda\x89\xa6\x55\x0d\x13\x3b\xd5\
+\xb4\xaa\x61\x5a\x27\x9b\x56\x35\x4c\xea\x74\xd3\xaa\x86\x29\xbd\
+\xd1\xb4\xaa\x61\x42\x6f\x35\xad\x6a\x98\xce\x9b\x4d\xab\x1a\x26\
+\xf3\x76\xd3\xaa\x86\xa9\x5c\xd0\xb4\xaa\x61\x22\x97\x34\xad\x6a\
+\x98\xc6\x45\x4d\xab\x1a\x26\x71\x59\xd3\xaa\x86\x29\x5c\xd8\xb4\
+\xaa\x61\x02\x97\x36\xad\x6a\x18\xee\xe2\xa6\x55\x0d\x83\x5d\xde\
+\xb4\xaa\x61\xa8\x1b\x9a\x56\x35\x0c\x74\x4b\xd3\xaa\x86\x61\x6e\
+\x6a\x5a\xd5\x30\xc8\x6d\x4d\xab\x1a\x86\xb8\xb1\x69\x55\xc3\x00\
+\xb7\x36\xad\x6a\x78\xdc\xcd\x4d\xab\x1a\x1e\x76\x7b\xd3\xaa\x86\
+\x47\x3d\xd0\xb4\xaa\xe1\x41\x8f\x34\xad\x6a\x78\xcc\x43\x4d\xab\
+\x1a\x1e\xf2\x58\xd3\xaa\x86\x47\x3c\xd8\xb4\xaa\xe1\x01\x8f\x36\
+\xad\x6a\xb8\xdd\xc3\x4d\xab\x1a\x6e\xf6\x78\xd3\xaa\x86\x5b\x0d\
+\x68\x5a\xd5\x70\xa3\x21\x4d\xab\x1a\x6e\x33\xa8\x69\x55\xc3\x4d\
+\x86\x35\xad\x6a\xb8\xc5\xc0\xa6\x55\x0d\x37\x18\xda\xb4\xaa\xe1\
+\x72\x83\x9b\x56\x35\x5c\x6c\x78\xd3\xaa\x86\x4b\x4d\xd0\xb4\xaa\
+\xe1\x42\x53\x34\xad\x6a\xb8\xcc\x24\x4d\xab\x1a\x2e\x32\x4d\xd3\
+\xaa\x86\x4b\x4c\xd4\xb4\xaa\xe1\x02\x53\x35\xad\x6a\x78\xdb\x64\
+\x4d\xab\x1a\xde\x34\x5d\xd3\xaa\x86\xb7\x4c\xd8\xb4\xaa\xe1\x0d\
+\x53\x36\xad\x6a\x38\x6d\xd2\xa6\x55\x0d\x27\x4d\xdb\xb4\xaa\xe1\
+\x94\x89\x9b\x56\x35\x9c\x30\x75\xd3\xaa\x86\xc3\x26\x6f\x5a\xd5\
+\x70\xd0\xf4\x4d\xab\x1a\x0e\x59\xa0\x69\x55\xc3\x01\x4b\x34\xad\
+\x6a\xd8\x6d\x91\xa6\x55\x0d\x3b\x2d\xd3\xb4\xaa\x61\x97\x85\x9a\
+\xfe\xfc\xf5\x37\xa3\xd7\x82\xf9\x69\x1a\x5a\x34\x0d\x2d\x9a\x86\
+\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
+\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
+\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
+\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
+\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
+\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
+\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
+\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
+\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
+\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\
+\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\
+\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\
+\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
+\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
+\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
+\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
+\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
+\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
+\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
+\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
+\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
+\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
+\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
+\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
+\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
+\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
+\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
+\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
+\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\
+\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\
+\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\
+\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
+\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
+\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
+\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
+\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
+\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
+\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
+\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
+\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
+\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
+\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
+\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
+\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
+\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
+\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
+\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
+\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
+\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
+\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
+\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
+\x4d\x43\x8b\xa6\xa1\x65\xa5\xa6\x3f\xff\xe2\x97\x10\xf6\x33\x6c\
+\x1a\xda\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\
+\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\
+\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\
+\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\
+\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\
+\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\
+\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\
+\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\
+\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\
+\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\
+\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\
+\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\
+\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xb3\xbd\x46\x5f\x00\x5c\x6a\x53\
+\x35\xb4\x6c\xaa\x86\x96\x4d\xd5\xd0\xb2\xa9\x1a\x5a\x36\x55\x43\
+\xcb\xa6\x6a\x68\xd9\x54\x0d\x2d\x9b\xaa\xa1\x65\x53\x35\xb4\x6c\
+\xaa\x86\x96\x4d\xd5\xd0\xb2\xa9\x1a\x5a\x36\x55\x43\xcb\xa6\x6a\
+\x68\xd9\x54\x0d\x2d\x9b\xaa\xa1\x65\x53\x35\xb4\x6c\xaa\x86\x96\
+\x4d\xd5\xd0\xb2\xa9\x1a\x5a\x36\x55\x43\xcb\xa6\x6a\x68\xd9\x54\
+\x0d\x2d\x9b\xaa\xa1\x65\x53\x35\xb4\x6c\xaa\x86\x96\x4d\xd5\xd0\
+\xb2\xa9\x1a\x5a\x36\x55\x43\xcb\xa6\x6a\x68\xd9\x54\x0d\x2d\x1f\
+\x45\xad\x6a\x58\xcc\x87\x51\xab\x1a\xd6\xf2\x71\xd4\xaa\x86\xa5\
+\xec\x88\x5a\xd5\xb0\x92\x3d\x51\xab\x1a\x16\xb2\x2b\x6a\x55\xc3\
+\x3a\xf6\x45\xad\x6a\x58\xc6\xce\xa8\x55\x0d\xab\xd8\x1b\xb5\xaa\
+\x61\x11\xbb\xa3\x56\x35\xac\x61\x7f\xd4\xaa\x86\x25\x1c\x88\x5a\
+\xd5\xb0\x82\x23\x51\xab\x1a\x16\x70\x28\x6a\x55\xc3\xfc\x8e\x45\
+\xad\x6a\x98\xde\xc1\xa8\x55\x0d\xb3\x3b\x1a\xb5\xaa\x61\x72\x87\
+\xa3\x56\x35\xcc\xed\x78\xd4\xaa\x86\xa9\x9d\x88\x5a\xd5\x30\xb3\
+\x33\x51\xab\x1a\x26\x76\x2a\x6a\x55\xc3\xbc\xce\x45\xad\x6a\x98\
+\xd6\xc9\xa8\x55\x0d\xb3\x3a\x1b\xb5\xaa\x61\x52\xa7\xa3\x56\x35\
+\xcc\xe9\x7c\xd4\xaa\x86\x29\xbd\x11\xb5\xaa\x61\x46\xef\x44\xad\
+\x6a\x98\xd0\x5b\x51\xab\x1a\xe6\xf3\x5e\xd4\xaa\x86\xe9\xbc\x19\
+\xb5\xaa\x61\x36\xef\x46\xad\x6a\x98\xcc\xdb\x51\xab\x1a\xe6\xf2\
+\x7e\xd4\xaa\x86\xa9\x5c\x10\xb5\xaa\x61\x26\x57\x44\xad\x6a\x98\
+\xc8\x25\x51\x6f\x9f\x46\x3f\xe3\x88\x5f\xfd\x1a\xca\xae\x89\x7a\
+\xa9\xbf\xfa\x37\xbf\xbd\xe8\xd1\x90\xa6\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
+\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
+\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
+\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
+\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
+\xaa\xa1\x46\xd5\x50\xb3\x54\xd5\xbf\x1b\xbd\x16\xac\x60\xa5\xaa\
+\xbf\x55\x35\xec\xa0\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
+\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
+\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
+\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
+\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
+\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
+\x43\xcd\x52\x55\xff\x7e\xf4\x5a\xb0\x02\x55\x43\x8d\xaa\xa1\x46\
+\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
+\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
+\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
+\x43\x8d\xaa\xa1\x66\xa9\xaa\xff\x30\x7a\x2d\x58\x81\xaa\xa1\x46\
+\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
+\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
+\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x66\xa5\xaa\
+\xff\xf8\xa7\xd1\x6b\xc1\x0a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
+\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\
+\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
+\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
+\x46\xd5\x50\xa3\x6a\xa8\x59\xa9\xea\x3f\xab\x1a\x76\x50\x35\xd4\
+\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
+\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\x4b\x55\xfd\
+\x97\xd1\x6b\xc1\x0a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
+\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
+\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\
+\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
+\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
+\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
+\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
+\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x96\xaa\xfa\xaf\xa3\xd7\x82\x15\
+\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
+\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
+\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
+\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
+\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\x2b\x55\xfd\x37\x55\
+\xc3\x0e\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
+\xa1\x46\xd5\x50\xb3\x54\xd5\x7f\x1f\xbd\x16\xac\x40\xd5\x50\xa3\
+\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
+\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
+\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
+\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
+\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
+\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\xcd\x52\x55\xff\
+\x63\xf4\x5a\xb0\x02\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
+\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
+\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
+\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
+\xd5\x50\xb3\x52\xd5\x5f\xaa\x1a\x76\x50\x35\xd4\xa8\x1a\x6a\x54\
+\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
+\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\x4b\x55\xfd\xd5\xe8\xb5\x60\
+\x05\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
+\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
+\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
+\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xb3\x50\xd5\x5f\x7f\x33\
+\x7a\x2c\x58\xc2\x32\x55\x6b\x1a\x76\x5a\xa4\x6a\x4d\xc3\x6e\x4b\
+\x54\xad\x69\x38\x60\x81\xaa\x35\x0d\x87\x4c\x5f\xb5\xa6\xe1\xa0\
+\xc9\xab\xd6\x34\x1c\x36\x75\xd5\x9a\x86\x13\x26\xae\x5a\xd3\x70\
+\xca\xb4\x55\x6b\x1a\x4e\x9a\xb4\x6a\x4d\xc3\x69\x53\x56\xad\x69\
+\x78\xc3\x84\x55\x6b\x1a\xde\x32\x5d\xd5\x9a\x86\x37\x4d\x56\xb5\
+\xa6\xe1\x6d\x53\x55\xad\x69\xb8\xc0\x44\x55\x6b\x1a\x2e\x31\x4d\
+\xd5\x9a\x86\x8b\x4c\x52\xb5\xa6\xe1\x32\x53\x54\xad\x69\xb8\xd0\
+\x04\x55\x6b\x1a\x2e\x35\xbc\x6a\x4d\xc3\xc5\x06\x57\xad\x69\xb8\
+\xdc\xd0\xaa\x35\x0d\x37\x18\x58\xb5\xa6\xe1\x16\xc3\xaa\xd6\x34\
+\xdc\x64\x50\xd5\x9a\x86\xdb\x0c\xa9\x5a\xd3\x70\xa3\x01\x55\x6b\
+\x1a\x6e\xf5\x78\xd5\x9a\x86\x9b\x3d\x5c\xb5\xa6\xe1\x76\x8f\x56\
+\xad\x69\x78\xc0\x83\x55\x6b\x1a\x1e\xf1\x58\xd5\x9a\x86\x87\x3c\
+\x54\xb5\xa6\xe1\x31\x8f\x54\xad\x69\x78\xd0\x03\x55\x6b\x1a\x1e\
+\x75\x7b\xd5\x9a\x86\x87\xdd\x5c\xb5\xa6\xe1\x71\xb7\x56\xad\x69\
+\x18\xe0\xc6\xaa\x35\x0d\x43\xdc\x56\xb5\xa6\x61\x90\x9b\xaa\xd6\
+\x34\x0c\x73\x4b\xd5\x9a\x86\x81\x6e\xa8\x5a\xd3\x30\xd4\xe5\x55\
+\x6b\x1a\x06\xbb\xb8\x6a\x4d\xc3\x70\x97\x56\xad\x69\x98\xc0\x85\
+\x55\x6b\x1a\xa6\x70\x59\xd5\x9a\x86\x49\x5c\x54\xb5\xa6\x61\x1a\
+\x97\x54\xad\x69\x98\xc8\x05\x55\x6b\x1a\xa6\xf2\x76\xd5\x9a\x86\
+\xc9\xbc\x59\xb5\xa6\x61\x3a\x6f\x55\xad\x69\x98\xd0\x1b\x55\x6b\
+\x1a\xa6\x74\xba\x6a\x4d\xc3\xa4\x4e\x56\xad\x69\x98\xd6\xa9\xaa\
+\x35\x0d\x13\x3b\x51\xb5\xa6\x61\x6a\x87\xab\xd6\x34\x4c\xee\x60\
+\xd5\x9a\x86\xe9\x1d\xaa\x5a\xd3\xb0\x80\x03\x55\x6b\x1a\x96\xb0\
+\xbb\x6a\x4d\xc3\x22\x76\x56\xad\x69\x58\xc6\xae\xaa\x35\x0d\x0b\
+\xd9\x51\xb5\xa6\x61\x29\x1f\x56\xad\x69\x58\xcc\x4b\xd3\x10\xf3\
+\xd2\x34\xc4\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x4b\xd3\x10\xf3\xd2\
+\x34\xc4\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x4b\xd3\x10\xf3\xd2\x34\
+\xc4\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x4b\xd3\x10\xf3\xd2\x34\xc4\
+\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x17\xa3\x0f\xe0\x19\xff\x04\x21\
+\xd0\x80\x64\x8d\x91\x64\x11\x00\x00\x00\x25\x74\x45\x58\x74\x64\
+\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x31\x37\x2d\
+\x30\x36\x2d\x31\x32\x54\x30\x33\x3a\x33\x34\x3a\x35\x31\x2b\x30\
+\x38\x3a\x30\x30\x84\x9a\x03\x36\x00\x00\x00\x25\x74\x45\x58\x74\
+\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x31\x36\
+\x2d\x30\x34\x2d\x31\x36\x54\x31\x35\x3a\x35\x32\x3a\x31\x38\x2b\
+\x30\x38\x3a\x30\x30\x8b\xf9\x5a\xba\x00\x00\x00\x54\x74\x45\x58\
+\x74\x73\x76\x67\x3a\x62\x61\x73\x65\x2d\x75\x72\x69\x00\x66\x69\
+\x6c\x65\x3a\x2f\x2f\x2f\x68\x6f\x6d\x65\x2f\x64\x62\x2f\x73\x76\
+\x67\x5f\x69\x6e\x66\x6f\x2f\x73\x76\x67\x2f\x35\x33\x2f\x35\x34\
+\x2f\x35\x33\x35\x34\x66\x32\x37\x62\x35\x30\x31\x33\x36\x37\x63\
+\x36\x64\x33\x33\x63\x37\x31\x33\x38\x37\x66\x38\x62\x33\x30\x61\
+\x33\x2e\x73\x76\x67\xf7\x2c\xcc\x83\x00\x00\x00\x00\x49\x45\x4e\
+\x44\xae\x42\x60\x82\
 \x00\x00\x66\x59\
 \xff\
 \xd8\xff\xe1\x00\x18\x45\x78\x69\x66\x00\x00\x49\x49\x2a\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xff\xec\x00\x11\x44\
 \x75\x63\x6b\x79\x00\x01\x00\x04\x00\x00\x00\x64\x00\x00\xff\xe1\
 \x03\x7c\x68\x74\x74\x70\x3a\x2f\x2f\x6e\x73\x2e\x61\x64\x6f\x62\
 \x65\x2e\x63\x6f\x6d\x2f\x78\x61\x70\x2f\x31\x2e\x30\x2f\x00\x3c\
@@ -1920,14 +2645,532 @@
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x01\xa2\x7d\x09\xe1\xfa\x3f\xdb\xff\x00\x4f\xed\
 \x03\x50\x00\x3e\xbf\xe3\xe8\xff\x00\x9f\x40\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x3f\xff\xd9\
+\x00\x00\x03\x84\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\xca\x69\x43\x43\x50\x43\x75\x73\x74\x6f\x6d\x00\x00\
+\x18\x95\x63\x60\x60\xdc\xce\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\
+\x45\x41\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\
+\x01\x37\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\
+\xe5\xc7\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\
+\x98\xcd\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\
+\xad\x03\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\
+\x03\xd9\x3e\x40\xb6\x40\x3a\x12\x3b\x09\x89\x9d\x92\x5a\x9c\x0c\
+\x64\xc7\x00\xd9\xd1\x08\xbf\xe5\xcf\x67\x60\xb0\xf8\xc2\xc0\xc0\
+\x3c\x11\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x6d\x84\x98\
+\xca\x42\x06\x06\xfe\x56\x06\x86\x6d\x57\x10\x62\x9f\x03\xc1\xfe\
+\x65\x14\x3b\x53\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\
+\x4a\x84\xfb\x8a\xc9\xd8\x08\x62\x2f\x2c\x8c\xa8\x0a\x00\x67\xd9\
+\x31\x35\xdc\xee\x19\x62\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\
+\x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\x00\x25\x74\
+\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\
+\x30\x32\x32\x2d\x30\x35\x2d\x32\x31\x54\x31\x33\x3a\x30\x37\x3a\
+\x32\x39\x2b\x30\x30\x3a\x30\x30\x73\xb6\xf7\xf1\x00\x00\x00\x25\
+\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\
+\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x31\x54\x31\x33\x3a\x30\x37\
+\x3a\x32\x39\x2b\x30\x30\x3a\x30\x30\x02\xeb\x4f\x4d\x00\x00\x01\
+\xfe\x49\x44\x41\x54\x78\x9c\xed\xda\x3d\x6e\x13\x41\x18\x87\xf1\
+\x1f\x08\x21\x6e\x40\xc5\x09\x80\xd4\xa9\x69\x1c\x51\x82\x22\x10\
+\x05\x0d\x12\x67\xe0\x14\x1c\x01\x9a\xc8\x05\x08\x41\x05\x34\x50\
+\x73\x0f\x24\x3e\x0e\x80\xe2\xc6\x81\xc2\x31\x44\xca\x7a\x77\xb0\
+\x67\x66\xdf\x8d\xe6\x91\xa6\xb1\xc6\xaf\xdf\xff\xb3\x9f\xb3\x5e\
+\x1a\x8d\x46\xa3\xd1\x68\x34\x86\xd9\xc3\x1c\x3f\xb0\xc4\xef\x4c\
+\xa3\x8b\x57\x85\xeb\xff\xe5\x4a\x62\xf8\x47\x78\x89\xab\x89\xf3\
+\x27\xc3\xe5\x84\x39\x7b\x2e\x68\x78\xd2\x04\x3c\x73\x41\xc3\x93\
+\x26\xe0\x4e\xf1\x2e\x46\xe4\x52\xc2\x9c\xa5\xf3\xa2\x9e\xe3\x4b\
+\xa6\x1e\x5e\x77\x7c\xb6\x8f\x1b\x03\xdf\x9b\xe1\x49\x42\xfd\x94\
+\x8c\xbd\x74\x9d\x59\x0f\x77\x2d\xba\x23\x33\x1c\xcb\x70\x15\x48\
+\x39\x04\xa2\x31\xc3\x3b\x5c\xcb\x51\x6c\x6a\x02\xb2\x86\x67\x5a\
+\x02\x0e\x6c\x0e\xbf\xc0\x8b\x6d\x8a\x4e\x45\xc0\x0c\x6f\x6d\x0e\
+\x7f\x1f\x1f\xb7\x29\x3c\x05\x01\x7d\xbb\xfd\x3a\xfc\xfb\x6d\x8b\
+\x47\x17\x50\x34\x3c\xb1\x05\x14\x0f\x4f\x5c\x01\x55\xc2\x13\x53\
+\x40\xb5\xf0\xc4\x13\x50\x35\x3c\xb1\x04\x54\x0f\x4f\xfa\x03\x91\
+\xd2\x1c\xe8\xbf\xce\xdf\xc3\x87\x81\x1a\x5f\x75\x2f\xac\x76\xa6\
+\xf4\x62\xa8\x6f\x61\x73\x8c\xbb\x19\x7f\x6b\x2b\x4a\x0a\x08\x1f\
+\x9e\x72\x02\x26\x11\x9e\x32\x02\x26\x13\x9e\xfc\x02\x26\x15\x9e\
+\xbc\x02\x4a\x86\x3f\xdc\x50\xb7\x97\x9a\xf7\x01\xa3\x5c\xe7\x87\
+\xa8\x25\x20\x64\x78\xea\x08\x08\x1b\x9e\xf2\x02\x42\x87\xa7\xac\
+\x80\xf0\xe1\x29\x27\x60\x12\xe1\x29\xb3\x18\xba\x8e\x37\x76\x5b\
+\xd8\x54\xa3\xc4\x1e\xf0\x13\x4f\xad\xfe\x52\x3b\xcb\x7a\xcb\x87\
+\x09\x4f\xb9\x43\x60\x8e\xc7\xfe\x49\x08\xb5\xdb\x9f\xa5\xe4\x49\
+\x70\x2d\xe1\x97\xa0\xe1\x29\xff\x40\x64\x8e\x4f\x56\x87\x45\x48\
+\x6a\xdc\x08\x85\x0d\x4f\xac\x67\x82\xa3\xd0\x04\x8c\xdd\xc0\xd8\
+\x34\x01\x63\x37\x30\x36\x29\x97\xc1\x13\xe7\x45\xed\x17\xe8\x65\
+\x57\xba\x7a\x3a\xc9\x51\xf8\xbb\x7c\xaf\xad\xd6\x1e\xdf\x86\xc2\
+\xa5\x1c\x02\x9f\x13\xe6\x44\x25\x4b\xef\xb7\xad\xee\xe5\xc7\xde\
+\x9a\xff\x3b\x16\xb8\x99\x43\x00\x3c\x90\xfe\x5e\x5e\x84\xb1\xc0\
+\xc3\x5c\xe1\xd7\xdc\xc2\x91\xd5\x39\x21\xe7\xeb\xf2\xb9\xc6\xf2\
+\xb4\xb7\xa3\xd3\x5e\x1b\x8d\x46\xa3\xd1\x68\x34\x7a\xf9\x03\xe9\
+\xbb\x8b\x97\x75\xe0\x93\x8a\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
+\x42\x60\x82\
+\x00\x00\x12\x3f\
+\x47\
+\x49\x46\x38\x39\x61\x20\x00\x20\x00\xf3\x00\x00\xca\xca\xca\x88\
+\x88\x88\xb1\xb1\xb1\xeb\xeb\xeb\xbf\xbf\xbf\xd4\xd4\xd4\x7f\x7f\
+\x7f\x3f\x3f\x3f\x6a\x6a\x6a\x55\x55\x55\x2a\x2a\x2a\x94\x94\x94\
+\xa9\xa9\xa9\x15\x15\x15\xff\xff\xff\x00\x00\x00\x21\xff\x0b\x4e\
+\x45\x54\x53\x43\x41\x50\x45\x32\x2e\x30\x03\x01\x00\x00\x00\x21\
+\xff\x0b\x58\x4d\x50\x20\x44\x61\x74\x61\x58\x4d\x50\x3c\x3f\x78\
+\x70\x61\x63\x6b\x65\x74\x20\x62\x65\x67\x69\x6e\x3d\x22\xef\xbb\
+\xbf\x22\x20\x69\x64\x3d\x22\x57\x35\x4d\x30\x4d\x70\x43\x65\x68\
+\x69\x48\x7a\x72\x65\x53\x7a\x4e\x54\x63\x7a\x6b\x63\x39\x64\x22\
+\x3f\x3e\x20\x3c\x78\x3a\x78\x6d\x70\x6d\x65\x74\x61\x20\x78\x6d\
+\x6c\x6e\x73\x3a\x78\x3d\x22\x61\x64\x6f\x62\x65\x3a\x6e\x73\x3a\
+\x6d\x65\x74\x61\x2f\x22\x20\x78\x3a\x78\x6d\x70\x74\x6b\x3d\x22\
+\x41\x64\x6f\x62\x65\x20\x58\x4d\x50\x20\x43\x6f\x72\x65\x20\x35\
+\x2e\x36\x2d\x63\x31\x31\x31\x20\x37\x39\x2e\x31\x35\x38\x33\x32\
+\x35\x2c\x20\x32\x30\x31\x35\x2f\x30\x39\x2f\x31\x30\x2d\x30\x31\
+\x3a\x31\x30\x3a\x32\x30\x20\x20\x20\x20\x20\x20\x20\x20\x22\x3e\
+\x20\x3c\x72\x64\x66\x3a\x52\x44\x46\x20\x78\x6d\x6c\x6e\x73\x3a\
+\x72\x64\x66\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\
+\x77\x33\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\x30\x32\x2f\x32\
+\x32\x2d\x72\x64\x66\x2d\x73\x79\x6e\x74\x61\x78\x2d\x6e\x73\x23\
+\x22\x3e\x20\x3c\x72\x64\x66\x3a\x44\x65\x73\x63\x72\x69\x70\x74\
+\x69\x6f\x6e\x20\x72\x64\x66\x3a\x61\x62\x6f\x75\x74\x3d\x22\x22\
+\x20\x78\x6d\x6c\x6e\x73\x3a\x78\x6d\x70\x3d\x22\x68\x74\x74\x70\
+\x3a\x2f\x2f\x6e\x73\x2e\x61\x64\x6f\x62\x65\x2e\x63\x6f\x6d\x2f\
+\x78\x61\x70\x2f\x31\x2e\x30\x2f\x22\x20\x78\x6d\x6c\x6e\x73\x3a\
+\x78\x6d\x70\x4d\x4d\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x6e\x73\
+\x2e\x61\x64\x6f\x62\x65\x2e\x63\x6f\x6d\x2f\x78\x61\x70\x2f\x31\
+\x2e\x30\x2f\x6d\x6d\x2f\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x74\
+\x52\x65\x66\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x6e\x73\x2e\x61\
+\x64\x6f\x62\x65\x2e\x63\x6f\x6d\x2f\x78\x61\x70\x2f\x31\x2e\x30\
+\x2f\x73\x54\x79\x70\x65\x2f\x52\x65\x73\x6f\x75\x72\x63\x65\x52\
+\x65\x66\x23\x22\x20\x78\x6d\x70\x3a\x43\x72\x65\x61\x74\x6f\x72\
+\x54\x6f\x6f\x6c\x3d\x22\x41\x64\x6f\x62\x65\x20\x50\x68\x6f\x74\
+\x6f\x73\x68\x6f\x70\x20\x43\x43\x20\x32\x30\x31\x35\x20\x28\x4d\
+\x61\x63\x69\x6e\x74\x6f\x73\x68\x29\x22\x20\x78\x6d\x70\x4d\x4d\
+\x3a\x49\x6e\x73\x74\x61\x6e\x63\x65\x49\x44\x3d\x22\x78\x6d\x70\
+\x2e\x69\x69\x64\x3a\x41\x45\x38\x30\x41\x41\x45\x34\x31\x42\x41\
+\x42\x31\x31\x45\x36\x39\x32\x45\x32\x44\x34\x41\x36\x32\x38\x30\
+\x37\x35\x33\x35\x45\x22\x20\x78\x6d\x70\x4d\x4d\x3a\x44\x6f\x63\
+\x75\x6d\x65\x6e\x74\x49\x44\x3d\x22\x78\x6d\x70\x2e\x64\x69\x64\
+\x3a\x41\x45\x38\x30\x41\x41\x45\x35\x31\x42\x41\x42\x31\x31\x45\
+\x36\x39\x32\x45\x32\x44\x34\x41\x36\x32\x38\x30\x37\x35\x33\x35\
+\x45\x22\x3e\x20\x3c\x78\x6d\x70\x4d\x4d\x3a\x44\x65\x72\x69\x76\
+\x65\x64\x46\x72\x6f\x6d\x20\x73\x74\x52\x65\x66\x3a\x69\x6e\x73\
+\x74\x61\x6e\x63\x65\x49\x44\x3d\x22\x78\x6d\x70\x2e\x69\x69\x64\
+\x3a\x41\x45\x38\x30\x41\x41\x45\x32\x31\x42\x41\x42\x31\x31\x45\
+\x36\x39\x32\x45\x32\x44\x34\x41\x36\x32\x38\x30\x37\x35\x33\x35\
+\x45\x22\x20\x73\x74\x52\x65\x66\x3a\x64\x6f\x63\x75\x6d\x65\x6e\
+\x74\x49\x44\x3d\x22\x78\x6d\x70\x2e\x64\x69\x64\x3a\x41\x45\x38\
+\x30\x41\x41\x45\x33\x31\x42\x41\x42\x31\x31\x45\x36\x39\x32\x45\
+\x32\x44\x34\x41\x36\x32\x38\x30\x37\x35\x33\x35\x45\x22\x2f\x3e\
+\x20\x3c\x2f\x72\x64\x66\x3a\x44\x65\x73\x63\x72\x69\x70\x74\x69\
+\x6f\x6e\x3e\x20\x3c\x2f\x72\x64\x66\x3a\x52\x44\x46\x3e\x20\x3c\
+\x2f\x78\x3a\x78\x6d\x70\x6d\x65\x74\x61\x3e\x20\x3c\x3f\x78\x70\
+\x61\x63\x6b\x65\x74\x20\x65\x6e\x64\x3d\x22\x72\x22\x3f\x3e\x01\
+\xff\xfe\xfd\xfc\xfb\xfa\xf9\xf8\xf7\xf6\xf5\xf4\xf3\xf2\xf1\xf0\
+\xef\xee\xed\xec\xeb\xea\xe9\xe8\xe7\xe6\xe5\xe4\xe3\xe2\xe1\xe0\
+\xdf\xde\xdd\xdc\xdb\xda\xd9\xd8\xd7\xd6\xd5\xd4\xd3\xd2\xd1\xd0\
+\xcf\xce\xcd\xcc\xcb\xca\xc9\xc8\xc7\xc6\xc5\xc4\xc3\xc2\xc1\xc0\
+\xbf\xbe\xbd\xbc\xbb\xba\xb9\xb8\xb7\xb6\xb5\xb4\xb3\xb2\xb1\xb0\
+\xaf\xae\xad\xac\xab\xaa\xa9\xa8\xa7\xa6\xa5\xa4\xa3\xa2\xa1\xa0\
+\x9f\x9e\x9d\x9c\x9b\x9a\x99\x98\x97\x96\x95\x94\x93\x92\x91\x90\
+\x8f\x8e\x8d\x8c\x8b\x8a\x89\x88\x87\x86\x85\x84\x83\x82\x81\x80\
+\x7f\x7e\x7d\x7c\x7b\x7a\x79\x78\x77\x76\x75\x74\x73\x72\x71\x70\
+\x6f\x6e\x6d\x6c\x6b\x6a\x69\x68\x67\x66\x65\x64\x63\x62\x61\x60\
+\x5f\x5e\x5d\x5c\x5b\x5a\x59\x58\x57\x56\x55\x54\x53\x52\x51\x50\
+\x4f\x4e\x4d\x4c\x4b\x4a\x49\x48\x47\x46\x45\x44\x43\x42\x41\x40\
+\x3f\x3e\x3d\x3c\x3b\x3a\x39\x38\x37\x36\x35\x34\x33\x32\x31\x30\
+\x2f\x2e\x2d\x2c\x2b\x2a\x29\x28\x27\x26\x25\x24\x23\x22\x21\x20\
+\x1f\x1e\x1d\x1c\x1b\x1a\x19\x18\x17\x16\x15\x14\x13\x12\x11\x10\
+\x0f\x0e\x0d\x0c\x0b\x0a\x09\x08\x07\x06\x05\x04\x03\x02\x01\x00\
+\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x21\xfe\x27\x47\x49\x46\x20\
+\x72\x65\x73\x69\x7a\x65\x64\x20\x6f\x6e\x20\x68\x74\x74\x70\x73\
+\x3a\x2f\x2f\x65\x7a\x67\x69\x66\x2e\x63\x6f\x6d\x2f\x72\x65\x73\
+\x69\x7a\x65\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdb\
+\xf0\xc9\x49\x2b\x21\x35\xeb\x3d\xef\xe5\xe0\xc4\x30\x94\xe0\x51\
+\x45\x11\x52\xe3\x38\x99\x9f\x94\xa6\xab\xd4\x92\x12\x8c\xc9\x73\
+\x6d\xb7\xb9\xd3\x63\xa6\xf2\xfd\x70\x3a\x5e\x01\x10\x5a\x2c\x58\
+\xc0\x24\x91\x32\x18\x54\x9c\x4e\xe8\x48\x37\x9d\x54\xab\x14\x2c\
+\xf6\x48\xfa\x74\xbf\xdf\xab\x38\x0b\x9c\xf4\xd0\x69\xcd\xfa\xc9\
+\x81\x5b\x41\x6b\x10\xdc\x37\xae\x83\x37\x06\x81\x82\x81\x3e\x76\
+\x60\x83\x88\x06\x2b\x0e\x8c\x8d\x8e\x89\x83\x8b\x8e\x93\x0f\x90\
+\x8a\x35\x93\x8d\x1c\x08\x9c\x21\x0d\x0d\x46\x9c\x9d\x1c\x9f\x9f\
+\x2b\xa2\xa2\x20\xa5\xa5\x1b\xa8\xa9\x09\xb0\x15\x0a\x0a\x0f\xab\
+\xac\x14\xae\x08\x12\xb0\xb1\x07\x07\x0f\xb3\xb3\x12\xb6\xa0\x13\
+\xae\x13\xbc\x09\xbe\xbe\xc1\xb4\x13\xab\x15\xa3\xbb\xbc\x0f\xcb\
+\xbf\xcd\x14\xa6\x21\xc9\xd5\xcb\x12\xc1\x46\xd3\xb1\xdd\xbe\xdf\
+\xe0\x3e\xdc\x12\xd6\x13\xd8\x35\xe9\xe4\xbf\xe6\xc2\xe8\x09\x14\
+\xeb\xec\xce\xe1\xf6\xde\xfa\x21\xe5\x3e\x11\x00\x21\xf9\x04\x09\
+\x04\x00\x0f\x00\x2c\x05\x00\x00\x00\x1b\x00\x20\x00\x00\x04\x1f\
+\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\
+\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x78\x3e\x45\x00\
+\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\
+\x00\x00\x04\xdd\xf0\xc9\x49\x2b\x63\x35\xeb\x3d\xef\xe5\xe0\xb4\
+\x2c\x94\x87\x4d\x04\x11\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\
+\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x73\x3d\x72\xc1\x5d\xc8\
+\x60\x60\xb5\x8e\x30\x21\xa5\x50\xa8\x30\x99\xce\x91\x49\x3a\xa1\
+\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\xbd\xd6\x30\xf6\xa9\x7b\x9c\xd1\
+\x1a\x75\x93\xf3\xae\x82\xd4\xa0\x37\x4f\x4c\xff\x6e\x10\x80\x81\
+\x80\x3c\x03\x85\x86\x85\x0f\x82\x8a\x08\x2b\x87\x8e\x03\x8b\x82\
+\x8d\x8f\x86\x89\x91\x84\x94\x1c\x09\x9b\x20\x0e\x0e\x03\x44\x9b\
+\x9c\x1c\x9e\x9e\x2b\xa2\xa2\x9d\xa5\xa6\x1a\xa8\xa9\x07\xb0\x15\
+\x0d\x0d\x0f\xab\xa5\x15\xae\x09\x12\xb0\xb1\x0a\x0a\x0f\xb3\xb3\
+\x12\xb6\x0e\x14\xae\x13\xbc\x07\xbe\xbe\xc1\xb4\x12\x03\xab\xb8\
+\xba\xc8\xbc\x0f\xcb\xbf\xcd\x14\xac\x20\xc9\xd6\xcb\x12\xc1\x44\
+\xbb\xd5\xde\xbe\xe0\xe1\x3c\xdd\x12\xd7\x13\xd9\x34\xea\xe5\xbf\
+\xe7\xc2\xe9\x07\x14\xec\xed\xce\xe2\xf7\xdf\xfb\x21\xe6\x3c\x22\
+\x00\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x01\x00\x01\x00\x1f\
+\x00\x1e\x00\x00\x04\x20\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\
+\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\
+\x6d\xdf\x78\xae\xaf\x11\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\
+\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdf\xf0\xc9\x49\xeb\x5a\
+\x35\xeb\x3d\xef\xe5\xe0\x64\x18\x94\x87\x4d\x0c\x13\x52\xe3\xd8\
+\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\
+\x57\x73\x3d\x72\xc1\x5d\x08\x81\x60\xb5\x8e\x30\x21\x85\x40\xa8\
+\x30\x99\xce\x91\x49\x3a\xa1\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\xbd\
+\xd6\x30\xf6\xa9\x7b\x9c\xd1\x1a\x75\x93\xf3\xae\x82\xd4\xa0\x37\
+\x4f\x4c\xff\x6e\x12\x72\x09\x3c\x05\x84\x85\x84\x0f\x09\x89\x8a\
+\x8b\x2b\x86\x8e\x05\x8b\x91\x82\x21\x8f\x86\x88\x92\x93\x8d\x95\
+\x1c\x07\x9d\x20\x03\xa0\x44\x9d\x9e\x1c\xa0\xa1\x21\xa3\xa3\x9f\
+\xa6\xa7\x19\xa9\xaa\x0a\xb1\x14\x0e\xb4\x0f\xac\xa6\x15\xaf\x07\
+\x12\xb1\xb2\x0d\x0d\x0f\xb4\xb5\xb6\xb7\x14\xa9\x14\xbd\x0a\xbf\
+\xbf\xc2\x0e\x13\xc5\xc6\xbb\x13\xc9\x0f\xca\x0d\x0a\xc1\xc2\x14\
+\xad\x1c\xd4\xd6\xd8\x03\xda\x44\xd5\xbd\xbc\xbf\xd8\xd9\xc3\x34\
+\xd4\xe6\xd7\x13\xcd\x3c\xec\xd5\xe7\xef\xe2\xeb\xe8\xed\xf8\xd9\
+\xe3\x19\xcb\xfa\xfc\x1b\x7e\x11\x89\x00\x00\x21\xf9\x04\x09\x04\
+\x00\x0f\x00\x2c\x01\x00\x03\x00\x1e\x00\x1b\x00\x00\x04\x1e\xf0\
+\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\
+\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x6e\x04\x00\x21\xf9\
+\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\
+\x04\xde\xf0\xc9\x49\xab\x31\x35\xeb\x3d\xef\xe5\xe0\x84\x20\x94\
+\x87\x4d\xcb\x12\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\
+\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x73\x3d\x72\xc1\x5d\x28\x91\x60\
+\xb5\x8e\x30\x21\x85\xc1\xa8\x30\x99\xce\x91\x49\x3a\xa1\x52\x29\
+\xd7\x6b\xef\xf9\xe1\x7a\xbd\xd6\x30\xf6\xa9\x7b\x9c\xd1\x1a\x75\
+\x93\xf3\xae\x82\xd4\xa0\x37\x4f\x4c\xff\x6e\x0e\x80\x81\x80\x3c\
+\x02\x85\x86\x85\x0f\x82\x8a\x07\x2b\x04\x8e\x8f\x90\x8b\x82\x8d\
+\x90\x95\x89\x92\x3c\x95\x8f\x1c\x0a\x9d\x20\x00\x05\x05\x44\x9d\
+\x9e\x1c\xa1\xa1\x2b\xa4\xa4\x20\xa7\xa7\x1b\xaa\xab\x0d\xb2\x14\
+\x03\xb5\x0f\xad\xae\x14\xb0\x0a\x12\xb2\xb3\x0e\x0e\x0f\xb5\xb6\
+\xb7\xb8\xba\xab\x13\xbe\x0d\xc0\x0e\xc3\xc4\x12\xad\x15\xa5\xbd\
+\xbe\x0f\xcc\x03\xc2\xc3\x14\xa8\x21\xd5\xd6\xc0\xd8\xce\x44\xd4\
+\xb3\xdf\xcd\x12\xe2\x3c\xca\x13\xd7\x13\xe9\x2b\xeb\x12\xed\xe8\
+\xda\xea\x0d\x14\xf3\xf4\xe3\x19\xcc\xc1\xfb\x21\xc0\x88\x44\x00\
+\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x00\x00\x04\x00\x20\x00\
+\x1c\x00\x00\x04\x1f\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\
+\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\
+\xdf\x78\x3e\x47\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\
+\x00\x00\x20\x00\x20\x00\x00\x04\xd9\xf0\xc9\x49\x2b\x42\x35\xeb\
+\x3d\xef\xe5\xe0\x94\x24\x94\x87\x4d\x86\x11\x52\xe3\xd8\x79\x68\
+\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x73\
+\x3d\x72\xc1\x5d\xe8\x70\x60\xb5\x8e\x30\x21\x65\xb1\xa8\x30\x99\
+\xce\x91\x49\x3a\xa1\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\xbd\xd6\x30\
+\xf6\xa9\x7b\x9c\xd1\x1a\x75\x93\xf3\xae\x2e\xc5\xf4\x33\x0f\xbf\
+\x81\x6b\x14\x80\x81\x80\x3c\x0c\x85\x86\x85\x0f\x82\x8a\x0a\x2b\
+\x87\x8e\x0c\x8b\x82\x8d\x8f\x86\x89\x91\x84\x94\x1c\x0d\x9b\x20\
+\x04\x9e\x44\x9b\x9c\x1c\x9e\x9f\x21\xa1\xa1\x9d\xa4\xa5\x19\xa7\
+\xa8\x0e\xaf\x14\x05\xb2\x0f\xaa\xa4\x15\xad\x0d\x12\xaf\xb0\x03\
+\x03\x0f\xb2\xb3\xb4\xb5\x14\xa7\x14\xbb\x0e\xbd\xbd\xc0\x05\x14\
+\xaa\xb7\xb9\x13\xc7\x0f\xc9\xbe\xcb\xcd\x04\x2b\xbb\xbe\xd4\xbf\
+\xc0\x44\xba\xbb\x12\xdc\xdd\xc1\x34\xd2\xe2\xc9\x13\xd6\xe6\xe1\
+\xe8\xbd\xea\xde\x3c\xb0\x13\xe3\x12\xe5\xdf\xf4\xe9\xf8\x21\xef\
+\x3c\x11\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x00\x00\x01\x00\
+\x1e\x00\x1f\x00\x00\x04\x20\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\
+\xff\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\
+\x74\x6d\xdf\x78\xae\xaf\x11\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\
+\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xda\xf0\xc9\x49\x6b\
+\x4a\x35\xeb\x3d\xef\xe5\xe0\x74\x1c\x94\x87\x4d\x08\x12\x52\xe3\
+\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\
+\x8c\x57\x73\x3d\x72\xc1\x5d\x48\xa1\x60\xb5\x8e\x30\x21\xc5\x60\
+\xa8\x30\x99\xce\x91\x49\x3a\xa1\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\
+\xbd\xd6\x30\xf6\xa9\x7b\x9c\xd1\x1a\x75\x93\xf3\xae\x2e\xc5\x74\
+\x38\x0d\xbf\xd1\x67\x1a\x72\x73\x2b\x0b\x84\x85\x84\x0f\x0d\x89\
+\x8a\x8b\x83\x86\x8e\x8b\x90\x0d\x8d\x8e\x85\x88\x81\x3c\x94\x87\
+\x1b\x0e\x9c\x20\x0c\x9f\x44\x9c\x9d\x1c\x9f\xa0\x21\xa2\xa2\x9e\
+\xa5\xa6\x19\xa8\xa9\x03\xb0\x14\x04\xb3\x0f\xab\xa5\x15\xae\x0e\
+\x12\xb0\xb1\x05\x05\x0f\xb3\xb4\xb5\xb6\x14\xa8\x14\xbc\x03\xbe\
+\xbe\xc1\x04\x14\xab\xb8\x03\xc7\xbc\x0f\xca\xbf\xcc\xce\x0c\x2b\
+\xc8\xd4\xca\x12\xc1\x44\xbb\xd3\xdc\xbe\xde\xdf\x3c\xdb\x12\xd5\
+\x13\xd7\x34\xe8\xe3\xbf\xe5\xc2\xed\xd1\x13\xea\xeb\xcd\xe0\x15\
+\xf6\xf9\x20\xe4\x3c\x11\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\
+\x02\x00\x00\x00\x1b\x00\x20\x00\x00\x04\x1f\xf0\xc9\x49\xab\xbd\
+\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\
+\xbe\x70\x2c\xcf\x74\x6d\xdf\x78\x3e\x45\x00\x21\xf9\x04\x05\x04\
+\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdb\xf0\
+\xc9\x49\xeb\x39\x35\xeb\x3d\xef\xe5\xe0\xa4\x28\x94\x87\x4d\x49\
+\x12\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\
+\xc3\x0f\xd9\x8c\x57\x6b\x3d\x72\xc1\x5d\xa8\xd1\x60\x19\x73\x42\
+\x0a\x02\x51\x61\x32\x9d\x23\x53\x74\x32\x9d\x52\xac\xd6\xde\x13\
+\xb3\xed\x76\xab\xe0\xab\x51\xf7\x30\x9f\x35\xe9\x26\xc7\x4d\x5d\
+\x86\xe7\x6f\xda\x7d\x93\xcf\x0c\x1c\x80\x81\x0e\x3c\x06\x85\x86\
+\x85\x0f\x82\x8a\x83\x21\x87\x8e\x06\x8b\x82\x2b\x8f\x87\x89\x03\
+\x97\x98\x03\x84\x94\x1c\x98\x20\x0b\xa0\x44\x99\x9f\xa0\xa1\x20\
+\x99\x97\xa4\xa5\x0b\x1b\xa8\xa9\x05\xb0\x14\x0c\xb3\x0f\xab\xa5\
+\x15\xae\x12\xb0\xb1\x04\x04\x0f\xb3\xb4\xb5\xb6\x14\xa3\x13\xbb\
+\x05\xbd\xbd\xc0\x0c\x14\xab\xb8\x9a\xc6\xbb\x0f\x02\xc9\xbf\xc0\
+\xcd\xac\x21\xc7\xd3\xd5\xd6\xcc\x44\x0f\xdb\xdc\xbd\x12\xcb\x44\
+\xe2\xe3\xbe\xe5\xd7\x34\xe8\xd4\xe4\xeb\xc1\xed\x05\x14\xef\xea\
+\xeb\xe0\x19\xc9\xf7\xf9\x1c\xf0\x34\x11\x00\x21\xf9\x04\x09\x04\
+\x00\x0f\x00\x2c\x00\x00\x00\x00\x1c\x00\x1e\x00\x00\x04\x1f\xf0\
+\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\
+\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x38\x19\x01\x00\x21\
+\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\
+\x00\x04\xd9\xf0\xc9\x49\xab\x52\x35\xeb\x3d\xef\xe5\xe0\xd4\x34\
+\x94\x87\x4d\xc7\x11\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\
+\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x6b\x3d\x72\xc1\x5d\xc8\xe1\
+\x60\x19\x73\x42\x4a\x22\x51\x61\x32\x9d\x23\x53\x74\x32\x9d\x52\
+\xac\xd6\xde\x13\xb3\xed\x76\xab\xe0\xab\x51\xf7\x30\x9f\x35\xe9\
+\x26\xc7\x4d\x5d\x86\xe7\x66\xde\x7d\xf3\xd6\x0c\xfe\x80\x7f\x3c\
+\x08\x84\x85\x84\x0f\x81\x89\x03\x2b\x86\x8d\x08\x8a\x81\x8c\x8e\
+\x85\x88\x90\x83\x93\x1c\x05\x9a\x20\x01\x06\x06\x44\x9a\x9b\x1c\
+\x9e\xa4\x21\xa1\xa1\x20\xa4\xa5\x1a\xa7\xa8\x04\xaf\x14\x0b\xb2\
+\x0f\xaa\xab\x13\xad\x05\x12\xaf\xb0\x0c\x0c\x0f\xb2\xb3\xb4\xb5\
+\x14\xa7\x14\xbb\x04\xbd\xbd\xc0\x0b\x14\xaa\x15\xa2\xba\xbb\x0f\
+\xc9\xbe\xcb\xcd\x9f\x21\xc7\xd3\xc9\x12\xc0\x44\xd1\xb0\xdb\xbd\
+\xdd\xde\x3c\xda\x12\xd4\x13\xd6\x34\xe7\xe2\xbe\xe4\xc1\xec\x04\
+\x14\xe9\xea\xcc\xdf\x15\xf5\xf8\x20\xe3\x3c\x11\x00\x21\xf9\x04\
+\x09\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x1c\x00\x20\x00\x00\x04\
+\x1f\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\
+\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x78\x3e\x47\
+\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\
+\x20\x00\x00\x04\xdd\xf0\xc9\x49\x6b\x6b\x35\xeb\x3d\xd5\xc5\x5c\
+\x28\x39\x0e\xe5\x5d\xa6\x22\x52\x24\xd9\x7d\x9d\x22\xaf\x63\xfb\
+\xa2\x92\x3c\xd3\x4f\x5b\x3e\x27\x90\x4e\xc5\xab\x39\x06\x40\x18\
+\x50\x27\x1a\x20\x27\xbe\x24\x6a\x48\x39\x1c\x2a\x4e\x27\xab\x15\
+\xa4\x4e\xac\x56\x4a\x36\x6b\x2c\x4d\x99\x0f\x30\x18\x3b\xd6\xda\
+\x62\x2a\xf5\x5a\xd3\x7e\x6e\xe4\xd7\x26\x99\x23\xe7\xed\xef\x61\
+\x1b\x05\x83\x84\x83\x3c\x09\x88\x89\x88\x0f\x85\x8d\x05\x2b\x8a\
+\x91\x09\x8e\x85\x90\x92\x89\x8c\x94\x87\x97\x1c\x04\x9e\x21\x08\
+\xa1\x45\x9e\x9f\x1c\xa1\xa7\x22\xa4\xa4\xa0\xa7\xa2\x1a\xaa\xab\
+\x0c\xb2\x14\x06\xb5\x0f\xad\xa8\x14\xb0\x04\x12\xb2\xb3\x0b\x0b\
+\x0f\xb5\xb6\xb7\xb8\xba\xab\x13\xbe\x0c\xc0\xc0\xc3\x06\x14\xad\
+\x15\xa5\xbd\xbe\x0f\xcc\xc1\xce\xd0\x08\x2b\xca\xd6\xcc\x12\xc3\
+\x45\xd4\xb3\xde\xc0\xe0\xe1\x3c\xdd\x12\xd7\x13\xd9\x34\xea\xe5\
+\xc1\xe7\xc4\xef\x0c\x14\xec\xed\xcf\xe2\x15\xf8\xfb\x21\xe6\x3c\
+\x22\x00\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x00\x00\x02\x00\
+\x1f\x00\x1d\x00\x00\x04\x1f\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\
+\xff\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\
+\x74\x6d\xdf\x78\x6e\x47\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\
+\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdf\xf0\xc9\x49\xab\x73\
+\x35\xeb\x3d\xc7\xc5\x5c\x28\x0d\x03\xe5\x5d\x54\xd3\x88\x26\x59\
+\x8e\xdf\xa4\xaa\xec\xe8\x76\xb1\x34\xaf\xf5\xe3\xbe\x27\xd0\xae\
+\xd7\xb9\x05\x75\x33\x51\xa1\xd0\x22\xf9\x62\xc3\x89\x42\x51\x59\
+\x2e\x9b\xa4\x4f\x54\x32\x9d\x52\xac\x56\x9b\x13\x15\xed\x76\xab\
+\xe0\xeb\x4d\x46\x33\x9f\x35\x69\x26\xc7\x4d\x55\x86\xe7\xe6\xde\
+\x7d\xf3\xd6\x10\x04\x80\x81\x02\x3d\x07\x85\x86\x85\x0f\x04\x8a\
+\x8b\x8c\x2c\x87\x8f\x07\x8c\x92\x04\x8e\x90\x86\x89\x93\x94\x35\
+\x96\x07\x1c\x0c\x9f\x22\x09\x09\x44\x9f\xa0\x1c\xa2\xa2\x2c\xa5\
+\xa5\x21\xa8\xa8\x1b\xab\xac\x0b\xb3\x15\x08\x08\x0f\xae\xaf\x14\
+\xb1\x0c\x12\xb3\xb4\x06\x06\x0f\xb6\xb6\x12\xb9\xa3\x13\xb1\x13\
+\xbf\x0b\xc1\xc1\xc4\xb7\x13\xae\x15\xa6\xbe\xbf\x0f\xce\xc2\xd0\
+\x14\xa9\x22\xcc\xd8\xce\x12\xc4\x44\xd6\xb4\xe0\xc1\xe2\xe3\x3d\
+\xdf\x12\xd9\x13\xdb\x35\xec\xe7\xc2\xe9\xc5\xeb\x0b\x14\xee\xef\
+\xd1\xe4\xf9\xe1\xfd\x22\xd0\xf5\x88\x00\x00\x21\xf9\x04\x09\x04\
+\x00\x0f\x00\x2c\x00\x00\x00\x00\x1d\x00\x1c\x00\x00\x04\x1e\xf0\
+\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\
+\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x70\x04\x00\x21\xf9\
+\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\
+\x04\xdd\xf0\xc9\x49\xeb\x18\x35\xeb\x3d\xef\xe5\xe0\x54\x14\x94\
+\x87\x4d\x8e\x13\x52\xe3\xd8\x79\x5d\xaa\xae\x4f\x4b\x4a\x26\x2a\
+\xd3\x92\x8d\xc3\x0f\xd9\x8c\x57\x6b\x3d\x72\xc1\xd4\x89\x43\x20\
+\xb0\x8c\x39\x21\xa5\xd1\xa8\x34\x9b\xcf\x91\x69\xb0\x9b\x50\xa9\
+\x94\xeb\xb5\x07\xc5\x48\x1f\xdf\xaf\x55\x8c\x35\xea\x54\x69\xb5\
+\x86\xed\xe4\xc4\xab\x21\x31\x28\xce\x1b\xdb\xc1\x1b\x0c\x82\x83\
+\x82\x3c\x0a\x87\x88\x87\x0f\x84\x8c\x0c\x2b\x89\x90\x0a\x8d\x84\
+\x8f\x91\x88\x8b\x93\x86\x96\x1c\x0b\x9d\x21\x07\x07\x44\x9d\x9e\
+\x1c\xa0\xa0\x2b\xa3\xa3\x20\xa6\xa6\x1b\xa9\xaa\x06\xb1\x15\x09\
+\x09\x0f\xac\xad\x14\xaf\x0b\x12\xb1\xb2\x08\x08\x0f\xb4\xb4\x12\
+\xb7\xa1\x13\xaf\x13\xbd\x06\xbf\xbf\xc2\xb5\x13\xac\x15\xa4\xbc\
+\xbd\x0f\xcc\xc0\xce\x14\xa7\x21\xca\xd6\xcc\x12\xc2\x44\xd4\xb2\
+\xde\xbf\xe0\xe1\x3c\xdd\x12\xd7\x13\xd9\x34\xea\xe5\xc0\xe7\xc3\
+\xe9\x06\x14\xec\xed\xcf\xe2\xf7\xdf\xfb\x21\xe6\x3c\x22\x00\x00\
+\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x03\x00\x00\x00\x1d\x00\x1c\
+\x00\x00\x04\x1e\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\
+\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\
+\x70\x04\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\
+\x20\x00\x20\x00\x00\x04\xde\xf0\xc9\x49\x6b\x29\x35\xeb\x3d\xef\
+\xe5\xe0\x44\x10\x94\x87\x4d\xc3\x10\x52\xe3\xd8\x79\x68\xaa\xae\
+\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x1b\x09\x1e\
+\xb9\xa0\x2c\xc4\x60\xb0\x5a\x48\x98\x90\x32\x70\x54\x9a\xcd\xe7\
+\xc8\x34\x9d\x38\xbe\xd6\x09\x16\xdb\x83\x7e\xba\x60\xf0\x75\x9c\
+\x85\xea\x1e\x69\xb5\x86\xed\xe4\xc4\xc3\x1c\x36\x28\x3d\x64\x66\
+\xed\x5f\x1c\x0b\x83\x84\x83\x3c\x0a\x88\x89\x88\x0f\x85\x8d\x0b\
+\x2b\x0d\x91\x92\x93\x8e\x85\x90\x93\x98\x8c\x95\x3c\x98\x92\x1c\
+\x06\xa0\x21\x8b\x3c\xa0\xa1\x1c\x8a\x2b\xa5\xa5\x20\x8a\xa3\x19\
+\xaa\xab\x08\xb2\x15\x07\x07\x0f\xad\xae\x12\xb0\x06\x12\xb2\xb3\
+\x09\x09\x0f\xb5\xb5\x12\xb8\x14\xb0\x13\xbe\x08\xc0\xc0\xc3\xb6\
+\x13\xa8\xc7\xbc\xc9\xbe\x0f\xcb\xc0\xc2\xc3\x14\xb9\x1b\xca\xd6\
+\xcc\x12\xda\x44\xd6\xd5\xdf\xd8\xd9\xc4\x3c\xde\xbd\xe0\xe1\xe2\
+\x2b\xeb\x12\xed\xe8\xcf\x34\xb3\x14\xf3\xd9\xe3\x19\xcc\xc1\xfb\
+\x21\xe7\x68\x44\x00\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\
+\x00\x00\x00\x01\x00\x01\x00\x00\x04\x02\xf0\x45\x00\x3b\
+\x00\x00\x02\x37\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
+\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
+\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
+\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
+\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
+\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
+\x6b\x42\xcf\x00\x00\x01\x39\x49\x44\x41\x54\x78\xda\xed\x9a\x4d\
+\x0a\xc2\x30\x10\x85\x9f\x5e\x46\x10\xef\x61\x29\xe8\xfd\x4f\x20\
+\x78\x02\x75\x55\x37\xcd\xa6\xf4\xcf\x9a\xbc\xcc\x4c\xdf\x07\xdd\
+\x48\x61\x7c\x5f\x42\x9b\x4c\x03\x08\x21\x84\x10\x42\x08\x21\x84\
+\xd8\xc4\x19\x40\x53\xa1\x6e\xd3\xd7\xae\xca\x09\xc0\x03\xc0\x07\
+\xc0\x9d\x1c\xfe\x05\xe0\x09\xe0\x52\x3b\x7c\xd7\x5f\x2c\x09\x29\
+\x7c\xaa\x5b\x45\xc2\x30\x3c\x4b\xc2\x30\x7c\x35\x09\x0d\x80\xf7\
+\xc8\x1f\xe9\xfa\xdf\xdb\x02\x35\xdb\x85\x9a\xf4\xe7\xd0\x15\xe3\
+\xa3\x51\x62\x26\x4c\x8d\x7c\xaa\x75\x63\x87\x67\x4a\x30\x1b\x9e\
+\x21\xc1\x7c\xf8\x92\x12\xdc\x84\x2f\x21\xc1\x5d\xf8\x9c\x12\xdc\
+\x86\xcf\x21\xc1\x7d\xf8\x7f\x24\x84\x09\xbf\x45\x42\xb8\xf0\xbf\
+\x48\x08\x1b\x3e\xb1\xb4\x84\x65\x2f\xa9\xab\x30\x37\x13\xc2\x8e\
+\xfc\x56\x09\x21\xc3\xaf\x95\x40\x0f\x7f\x24\x0b\x38\x64\xba\xc7\
+\x25\x73\x4f\x7b\x66\x53\xc5\x74\xf8\x90\x12\x76\xfd\x1a\x5c\xb3\
+\xc8\x61\x76\x96\xcc\x85\x4f\x84\x93\xb0\x65\x79\x1b\x46\xc2\x3f\
+\x6b\x7b\xf7\x12\x72\x6c\x6c\xdc\x4a\xc8\xb9\xab\x73\x27\xa1\xc4\
+\x96\xd6\x8d\x84\x92\xfb\x79\xf3\x12\x18\xcd\x0c\xb3\x12\x98\x9d\
+\x1c\x73\x12\x76\xff\x71\x74\xee\xf3\x78\xc9\xfd\xfc\xd4\x4c\x30\
+\x71\x46\x80\xd5\xcc\x18\x4a\x30\x71\x4a\x84\xdd\xc9\x49\x12\xaa\
+\x86\x4f\xec\xfa\x90\x94\x10\x42\x08\x21\x84\x10\x42\xb8\xe4\x0b\
+\x51\xb4\xd2\xe4\x46\xbd\x95\xba\x00\x00\x00\x25\x74\x45\x58\x74\
+\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\
+\x2d\x30\x35\x2d\x32\x33\x54\x31\x34\x3a\x31\x39\x3a\x35\x32\x2b\
+\x30\x30\x3a\x30\x30\x5e\xe0\x66\x5a\x00\x00\x00\x25\x74\x45\x58\
+\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\
+\x32\x2d\x30\x35\x2d\x32\x33\x54\x31\x34\x3a\x31\x39\x3a\x35\x32\
+\x2b\x30\x30\x3a\x30\x30\x2f\xbd\xde\xe6\x00\x00\x00\x00\x49\x45\
+\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x02\xb8\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x0e\xc4\x00\x00\x0e\xc4\
+\x01\x95\x2b\x0e\x1b\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\
+\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x35\
+\x2d\x32\x31\x54\x31\x33\x3a\x30\x37\x3a\x32\x39\x2b\x30\x30\x3a\
+\x30\x30\x73\xb6\xf7\xf1\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\
+\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\
+\x35\x2d\x32\x31\x54\x31\x33\x3a\x30\x37\x3a\x32\x39\x2b\x30\x30\
+\x3a\x30\x30\x02\xeb\x4f\x4d\x00\x00\x02\x08\x49\x44\x41\x54\x78\
+\x9c\xed\x9a\xb1\x4e\x02\x31\x18\xc7\x7f\x8a\x83\x93\xab\x0f\xa1\
+\xee\xbc\x81\x7a\x93\xc6\x10\x8d\x9b\xaf\xe0\x53\x30\xf9\x00\x26\
+\x2e\x06\x1c\x34\xba\xbb\x38\x3b\xbb\x3b\x99\x88\xc6\x07\x80\x90\
+\x80\x0e\x07\x09\x62\xe1\xca\xd1\xf2\x7d\xc5\xef\x97\x74\x69\x7a\
+\x6d\xff\x3f\x9a\xbb\x96\x3b\x30\x0c\xc3\x30\x0c\xc3\x28\x66\x1b\
+\x68\x00\x2d\xa0\x07\x7c\x2b\x2b\xbd\xc1\xdc\x1a\x83\xb9\x06\xe5\
+\x04\xe8\x28\x08\xe9\x5b\xda\xc0\x71\xa8\xf0\x5b\x89\x85\x1f\x96\
+\x0e\xb0\x13\x42\x40\x43\x41\x98\xb2\xa5\x19\x42\xc0\xbb\x82\x20\
+\x65\x4b\xab\x28\xdc\x8a\x87\x80\x1e\xb0\x3a\x56\x77\x01\x3c\x7b\
+\x5c\xbb\x48\xaa\xc0\xf9\x58\x5d\x1f\xa8\x4c\xbb\x68\xcd\xa3\xe3\
+\xf1\xf0\x90\x87\xbf\xf3\x9b\x97\x28\xae\xb9\xcf\xd6\x60\xd9\x31\
+\x01\xd2\x13\x90\xc6\x04\x48\x4f\x40\x1a\xed\x02\x36\x63\x0f\xa0\
+\x59\x40\x06\xbc\x02\xa7\x31\x07\xf1\xd9\x07\x48\x90\x01\xf7\xc0\
+\x3a\x70\x3d\xa8\xbb\x89\x31\x90\xc6\x15\x30\x1a\x1e\xf2\x9d\xdc\
+\x35\x91\x56\x82\x36\x01\xfb\xfc\x0e\x3f\xa4\x02\x5c\x12\xe1\x9e\
+\xa0\x49\x40\x06\x3c\xf0\x37\x3c\xe4\x47\xdb\x23\xe0\x33\xf4\xa0\
+\x5a\x04\x8c\x2f\xfb\x51\x3a\xc0\x01\xf0\x18\x63\x60\x0d\x02\xc4\
+\xc2\x83\xbc\x00\xd1\xf0\x20\x2b\x40\x3c\x3c\xc8\x09\x50\x11\x1e\
+\x64\x04\xa8\x09\x2f\x41\x46\xfe\x97\xb5\xeb\xff\xbb\x36\xb0\x3b\
+\x47\xdf\xb5\x09\xfd\xaa\x21\x66\x78\x50\x2e\x20\x76\x78\x50\x2c\
+\x60\x11\xe1\x41\xa9\x80\x45\x85\x87\x92\x02\x7c\x8e\xc3\xb7\x8e\
+\x3a\x9f\xf7\x02\x93\x0e\x36\x90\xdf\xed\x0f\x49\xe4\x6e\xef\xb2\
+\x5a\x2b\xb8\x66\x91\xbf\xfc\x90\x52\x2b\x20\xc6\x3e\x20\xa9\xe7\
+\x7c\x68\x01\x49\x85\x87\xb0\x02\x92\x0b\x0f\xe1\x04\x24\x19\x1e\
+\xc2\x08\x48\x36\x3c\xcc\x2f\x20\xe9\xf0\x30\x9f\x80\xe4\xc3\xfb\
+\xe2\x7a\xb6\x5e\x31\xfd\x39\xbf\x27\x30\xcf\x68\x5b\xe1\x59\x3e\
+\x49\x89\xb5\xc9\xf1\x41\x7c\x23\x94\xe4\xb2\x0f\x25\x20\xc9\xf0\
+\x10\xee\xdd\x60\x13\xd8\x60\xfa\x19\xe1\x0d\xf7\x01\xaa\xe8\x5c\
+\xe1\x4b\xd5\x51\xd7\x0f\xd1\x71\xa8\x4f\xd6\x5c\xa7\xca\x90\xfd\
+\xbb\xca\x47\x51\x38\xe9\xf7\x02\xb1\x79\x2a\x6a\xb0\xcc\x02\xba\
+\x40\xbd\xa8\xd1\xb2\x0a\xe8\x02\x67\xc0\x4b\x51\x43\xad\x1f\x48\
+\x94\xa1\x0f\x7c\x91\x2f\xfb\x3a\x1e\xe1\x0d\xc3\x30\x0c\xc3\xf8\
+\xdf\xfc\x00\x90\xf0\xcf\xe4\x10\x19\x96\x29\x00\x00\x00\x00\x49\
+\x45\x4e\x44\xae\x42\x60\x82\
+\x00\x00\x02\x14\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x30\x00\x00\x00\x30\x08\x06\x00\x00\x00\x57\x02\xf9\x87\
+\x00\x00\x01\xdb\x49\x44\x41\x54\x68\x43\xed\x98\xe1\x4d\xc3\x30\
+\x10\x85\xdb\x09\xe8\x28\x8c\x90\x4d\x68\x27\x00\x26\x20\x6c\x50\
+\x26\xa0\x4c\x42\xd9\x80\x11\x60\x03\x98\xa0\xdc\x93\x72\x92\x65\
+\xc5\xb1\x2f\x7e\x67\x54\xc9\x96\xfc\x23\xf1\xf9\xee\x7d\x77\x8e\
+\x13\x67\xbb\xb9\xf2\xb6\xbd\x72\xfd\x9b\x0e\xf0\xdf\x15\xec\x15\
+\xe8\x15\xa8\xcc\x40\xe9\x12\x1a\x24\xce\xb9\x32\x56\x38\xfd\xc9\
+\xe0\xeb\x63\x29\x76\x09\xc0\x5e\x1c\xbc\x4a\x3f\x49\x3f\x18\x02\
+\x2f\x99\x5e\x0c\x7e\x9e\xc5\x76\x4c\xd9\xe7\x00\x90\xf9\xf7\x60\
+\x32\x0b\xa2\x19\x00\xb4\x43\xf4\x1d\x19\x22\x95\xd1\x7b\x89\xb3\
+\x8b\xb2\x5d\x55\x01\xf5\xe5\x01\x11\xaf\x0a\x2c\x53\x2c\xd7\xb8\
+\x51\x00\xbc\x2a\xa1\x62\x63\xf1\xbf\x32\x70\x33\x0d\xd2\x00\xbc\
+\x20\x62\xf1\x6f\x12\xe8\x4b\xba\xee\x54\x54\x00\x36\xc4\x9c\x78\
+\x2c\x23\x3c\x23\x6e\x00\x2c\x88\x94\x78\xf8\x77\x07\xa8\x85\x58\
+\x12\xdf\x0c\x60\x2d\x44\x4e\x7c\x53\x00\x2b\x44\x89\xf8\xe6\x00\
+\x73\x10\x2f\x72\xf3\x21\xda\xd0\x4b\xc5\xcf\xbc\x0a\xd2\xb7\x72\
+\x9f\x12\x16\x67\x27\x31\xc6\x1b\x1b\x7b\xf8\x20\xfd\x33\x98\xec\
+\x22\x1e\xfe\x99\x00\xf0\x77\x94\x0e\x90\x26\xe2\x3d\x00\xe2\x8a\
+\xb9\x65\x5e\x03\xb1\x2b\x10\x02\xb8\x8b\xf7\xac\x40\x13\xf1\x5e\
+\x00\xcd\xc4\x7b\x00\xe4\xc4\xdf\x4e\x3b\xd5\xa3\x65\x7b\x5b\xb2\
+\x65\x3e\x03\x25\xe2\x71\xba\xc3\x81\x05\x3b\x15\xe5\x78\xca\x02\
+\xc8\x89\xd7\x2d\x16\x27\x2e\x6d\x14\x08\x06\x40\x89\xf8\x50\x74\
+\xc9\xf1\x74\x94\x09\xae\x9f\xd3\x2a\xc8\x22\xde\x02\xd1\x04\x60\
+\x8d\xf8\x52\x08\x77\x80\x1a\xf1\x25\x10\xae\x00\x0c\xf1\x39\x08\
+\x37\x00\xa6\xf8\x25\x88\x6f\x8f\x87\xd8\x43\x7c\x0a\xe2\x67\x7a\
+\x5f\x60\x9c\xf2\x57\xc2\x53\x7c\x0a\x42\xef\x57\x03\x78\x88\xd7\
+\x3d\x3e\xfe\x4a\xc0\x29\x8e\xfa\x6b\x71\x10\x87\x78\xfd\x6b\xc3\
+\x4f\xa7\x7d\x1c\x75\xc5\xf5\xc5\x30\xa7\xba\x02\x10\x8c\x2a\xb0\
+\xc4\x43\x7b\x53\x00\x04\x44\x25\xce\x86\xac\xe5\x4c\xc7\x9c\x41\
+\x30\x8e\xb8\xc9\xd8\x8c\x6f\x21\x83\x16\xbe\x69\x07\xe0\xe7\xd4\
+\xe6\xb1\x57\xc0\x96\x2f\xbe\x75\xaf\x00\x3f\xa7\x36\x8f\x7f\x22\
+\xc9\x98\x31\xaa\xe7\x39\xdc\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
+\x42\x60\x82\
+\x00\x00\x02\xa4\
+\x89\
+\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
+\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
+\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
+\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
+\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
+\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
+\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
+\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
+\x6b\x42\xcf\x00\x00\x01\xa6\x49\x44\x41\x54\x78\xda\xed\xd7\xbf\
+\x2b\x86\x51\x18\xc6\xf1\xef\xcd\x9b\x92\x32\x28\x8b\xc1\x62\xb1\
+\x50\x62\x31\x28\x93\x4c\x36\x16\x24\x25\x36\xfc\x07\xf8\x0f\xb0\
+\x59\x29\x03\x13\x93\x0c\x52\x06\x94\x5f\x65\xb1\x58\x0c\x16\x65\
+\xb0\x58\xd4\x65\x78\x7b\xca\xc0\x20\xcf\x7b\xee\xa3\xf7\xfe\xfc\
+\x01\xcf\x39\xd7\xd5\xfd\x3c\xcf\x39\x10\x42\x08\x21\x84\x10\x42\
+\x08\x21\x84\xf0\x4b\x92\xf6\x24\xb5\x25\x58\x67\x5c\xdf\xf8\xeb\
+\x73\x1b\x4a\xd8\xdb\x38\x70\x2b\x69\xb8\xd6\x25\xd4\x42\x19\x05\
+\x00\x74\x02\x27\x92\x36\x24\x35\x79\x87\xf2\x28\x00\xc0\x80\x45\
+\xe0\x4a\x52\x8f\x77\x30\x8f\x02\x0a\x3d\xc0\xa5\xa4\x25\x49\xe6\
+\x1d\xd0\xa3\x00\x80\x66\x60\x1d\x38\x92\xd4\xe1\x1d\xd2\xa3\x80\
+\xc2\x08\x70\x27\x69\xcc\x3b\xa8\x57\x01\x00\xed\xc0\x81\xa4\x6d\
+\x49\x2d\xde\x81\x3d\x0a\x28\x4c\x53\xfd\x40\xf6\x7b\x87\xf6\x2a\
+\x00\xa0\x1b\xb8\x90\xb4\x2a\xa9\xd1\x3b\xbc\x47\x01\x00\x15\x60\
+\x05\x38\x93\xd4\x55\x8f\x05\x14\x06\x81\x1b\x49\xf3\xf5\x5a\x00\
+\x40\x2b\xb0\x95\xea\x3e\x91\x63\x01\x05\xb7\xfb\x44\x2e\x05\x80\
+\xd3\x7d\x22\xa7\x02\xc0\xe1\x3e\x91\x5b\x01\xc9\xe5\x56\x80\x80\
+\x4d\x60\xc0\xcc\xee\x53\x2c\x58\xf1\x4e\xfc\xc5\x13\x30\x63\x66\
+\xa7\x29\x17\xcd\x65\x02\xf6\x81\xbe\xd4\xe1\x73\x28\xe0\x0d\x58\
+\x30\xb3\x09\x33\x7b\xf5\xd8\x80\xe7\x2b\x70\x0e\x4c\x9b\xd9\xa3\
+\xe3\x1e\x5c\x26\xe0\x03\x58\x03\x86\xbc\xc3\x43\xfa\x09\x78\x00\
+\xa6\xcc\xec\xda\x3b\x78\x21\xe5\x04\xec\x50\xfd\xbd\x65\x13\x1e\
+\xd2\x4c\xc0\x0b\x30\x67\x66\x87\xde\x61\x3d\x0a\x38\x06\x66\xcd\
+\xec\xd9\x3b\xe8\x4f\x6a\xf5\x0a\xbc\x03\xcb\xc0\x68\xce\xe1\xa1\
+\x36\x13\x70\x0f\x4c\xa6\x3a\xca\xfe\x55\x99\x13\x90\xfc\x1c\x5f\
+\x86\xb2\x26\xc0\xe5\x1c\x5f\x86\x32\x26\x60\x17\xe8\xfd\x8f\xe1\
+\x43\x08\x21\x84\x10\x42\x08\x21\x84\x50\x9f\x3e\x01\x96\x0e\x92\
+\x34\x47\x8e\x42\xcf\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\
+\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x36\
+\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x32\x32\x2b\x30\x30\x3a\
+\x30\x30\x28\xaf\x41\x1b\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\
+\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\
+\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x32\x32\x2b\x30\x30\
+\x3a\x30\x30\x59\xf2\xf9\xa7\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
+\x42\x60\x82\
 \x00\x00\x01\x9f\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x30\x00\x00\x00\x30\x08\x06\x00\x00\x00\x57\x02\xf9\x87\
 \x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
 \x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
 \x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
@@ -1948,437 +3191,72 @@
 \x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\
 \x61\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x31\x31\x54\x30\
 \x39\x3a\x30\x32\x3a\x35\x38\x2b\x30\x30\x3a\x30\x30\xcd\xe7\xe2\
 \xcc\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\
 \x64\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x31\x31\x54\
 \x30\x39\x3a\x30\x32\x3a\x35\x38\x2b\x30\x30\x3a\x30\x30\xbc\xba\
 \x5a\x70\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x0f\xc6\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x03\xd4\x00\x00\x03\xd8\x08\x03\x00\x00\x00\x0c\xc8\x41\xcd\
-\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
-\x00\x00\x00\x01\x73\x52\x47\x42\x00\xae\xce\x1c\xe9\x00\x00\x00\
-\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\x00\x00\xfa\
-\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\x00\x00\x3a\
-\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x54\x50\x4c\x54\
-\x45\xff\xff\xff\xe8\xe8\xe8\x7f\x7f\x7f\x11\x11\x11\xcc\xcc\xcc\
-\x00\x00\x00\x15\x15\x15\xd1\xd1\xd1\x30\x30\x30\x55\x55\x55\x88\
-\x88\x88\x33\x33\x33\x66\x66\x66\x0a\x0a\x0a\xbe\xbe\xbe\xbf\xbf\
-\xbf\x0b\x0b\x0b\xc0\xc0\xc0\xc1\xc1\xc1\x0e\x0e\x0e\xc7\xc7\xc7\
-\x0f\x0f\x0f\xc8\xc8\xc8\xc9\xc9\xc9\x10\x10\x10\xca\xca\xca\xcb\
-\xcb\xcb\xff\xff\xff\xef\x09\x36\x35\x00\x00\x00\x01\x74\x52\x4e\
-\x53\x00\x40\xe6\xd8\x66\x00\x00\x00\x01\x62\x4b\x47\x44\x00\x88\
-\x05\x1d\x48\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x00\x48\x00\
-\x00\x00\x48\x00\x46\xc9\x6b\x3e\x00\x00\x0d\xf3\x49\x44\x41\x54\
-\x78\xda\xed\xd5\x09\xae\xed\x46\x19\x46\x51\xe7\x25\x2f\x81\x43\
-\x17\xfa\x66\xfe\x03\x05\x21\x14\x01\x69\xae\xed\x63\xbb\xaa\x76\
-\xd6\x1a\xc1\x5f\x9f\xb4\x55\xdb\xc6\xcf\xc5\x17\xa3\x0f\x00\x2e\
-\xf5\xe9\xcb\xaf\x46\x9f\x00\x5c\xe8\xd3\xe7\xcf\xaa\x86\x90\x7f\
-\x35\xad\x6a\x08\xf9\x77\xd3\xaa\x86\x8c\xff\x34\xad\x6a\x88\xf8\
-\xae\x69\x55\x43\xc2\x7f\x35\xad\x6a\x08\xf8\x9f\xa6\x55\x0d\xcb\
-\xfb\xbf\xa6\x55\x0d\x8b\xfb\x5e\xd3\xaa\x86\xa5\xfd\x40\xd3\xaa\
-\x86\x85\xfd\x60\xd3\xaa\x86\x65\xfd\x48\xd3\xaa\x86\x45\xfd\x68\
-\xd3\xaa\x86\x25\xfd\x44\xd3\xaa\x86\x05\xfd\x64\xd3\xaa\x86\xe5\
-\x7c\xd0\xb4\xaa\x61\x31\x1f\x36\xad\x6a\x58\xca\x8e\xa6\x55\x0d\
-\x0b\xd9\xd5\xb4\xaa\x61\x19\x3b\x9b\x56\x35\x2c\x62\x77\xd3\xaa\
-\x86\x25\x1c\x68\x5a\xd5\xb0\x80\x43\x4d\xab\x1a\xa6\x77\xb0\x69\
-\x55\xc3\xe4\x0e\x37\xad\x6a\x98\xda\x89\xa6\x55\x0d\x13\x3b\xd5\
-\xb4\xaa\x61\x5a\x27\x9b\x56\x35\x4c\xea\x74\xd3\xaa\x86\x29\xbd\
-\xd1\xb4\xaa\x61\x42\x6f\x35\xad\x6a\x98\xce\x9b\x4d\xab\x1a\x26\
-\xf3\x76\xd3\xaa\x86\xa9\x5c\xd0\xb4\xaa\x61\x22\x97\x34\xad\x6a\
-\x98\xc6\x45\x4d\xab\x1a\x26\x71\x59\xd3\xaa\x86\x29\x5c\xd8\xb4\
-\xaa\x61\x02\x97\x36\xad\x6a\x18\xee\xe2\xa6\x55\x0d\x83\x5d\xde\
-\xb4\xaa\x61\xa8\x1b\x9a\x56\x35\x0c\x74\x4b\xd3\xaa\x86\x61\x6e\
-\x6a\x5a\xd5\x30\xc8\x6d\x4d\xab\x1a\x86\xb8\xb1\x69\x55\xc3\x00\
-\xb7\x36\xad\x6a\x78\xdc\xcd\x4d\xab\x1a\x1e\x76\x7b\xd3\xaa\x86\
-\x47\x3d\xd0\xb4\xaa\xe1\x41\x8f\x34\xad\x6a\x78\xcc\x43\x4d\xab\
-\x1a\x1e\xf2\x58\xd3\xaa\x86\x47\x3c\xd8\xb4\xaa\xe1\x01\x8f\x36\
-\xad\x6a\xb8\xdd\xc3\x4d\xab\x1a\x6e\xf6\x78\xd3\xaa\x86\x5b\x0d\
-\x68\x5a\xd5\x70\xa3\x21\x4d\xab\x1a\x6e\x33\xa8\x69\x55\xc3\x4d\
-\x86\x35\xad\x6a\xb8\xc5\xc0\xa6\x55\x0d\x37\x18\xda\xb4\xaa\xe1\
-\x72\x83\x9b\x56\x35\x5c\x6c\x78\xd3\xaa\x86\x4b\x4d\xd0\xb4\xaa\
-\xe1\x42\x53\x34\xad\x6a\xb8\xcc\x24\x4d\xab\x1a\x2e\x32\x4d\xd3\
-\xaa\x86\x4b\x4c\xd4\xb4\xaa\xe1\x02\x53\x35\xad\x6a\x78\xdb\x64\
-\x4d\xab\x1a\xde\x34\x5d\xd3\xaa\x86\xb7\x4c\xd8\xb4\xaa\xe1\x0d\
-\x53\x36\xad\x6a\x38\x6d\xd2\xa6\x55\x0d\x27\x4d\xdb\xb4\xaa\xe1\
-\x94\x89\x9b\x56\x35\x9c\x30\x75\xd3\xaa\x86\xc3\x26\x6f\x5a\xd5\
-\x70\xd0\xf4\x4d\xab\x1a\x0e\x59\xa0\x69\x55\xc3\x01\x4b\x34\xad\
-\x6a\xd8\x6d\x91\xa6\x55\x0d\x3b\x2d\xd3\xb4\xaa\x61\x97\x85\x9a\
-\xfe\xfc\xf5\x37\xa3\xd7\x82\xf9\x69\x1a\x5a\x34\x0d\x2d\x9a\x86\
-\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
-\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
-\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
-\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
-\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
-\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
-\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
-\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
-\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
-\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\
-\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\
-\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\
-\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
-\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
-\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
-\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
-\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
-\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
-\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
-\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
-\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
-\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
-\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
-\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
-\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
-\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
-\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
-\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
-\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\
-\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\
-\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\
-\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
-\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
-\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
-\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
-\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
-\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
-\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
-\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
-\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
-\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
-\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
-\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
-\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
-\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
-\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
-\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
-\x4d\x43\x8b\xa6\xa1\x65\xa5\xa6\x3f\xff\xe2\x97\x10\xf6\x33\x6c\
-\x1a\xda\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\
-\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\
-\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\
-\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\
-\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\
-\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\
-\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\
-\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\
-\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\
-\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xa3\x69\x88\xd1\x34\xc4\
-\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\x4d\x43\x8c\xa6\x21\x46\xd3\
-\x10\xa3\x69\x88\xd1\x34\xc4\x68\x1a\x62\x34\x0d\x31\x9a\x86\x18\
-\x4d\x43\x8c\xa6\x21\x46\xd3\x10\xb3\xbd\x46\x5f\x00\x5c\x6a\x53\
-\x35\xb4\x6c\xaa\x86\x96\x4d\xd5\xd0\xb2\xa9\x1a\x5a\x36\x55\x43\
-\xcb\xa6\x6a\x68\xd9\x54\x0d\x2d\x9b\xaa\xa1\x65\x53\x35\xb4\x6c\
-\xaa\x86\x96\x4d\xd5\xd0\xb2\xa9\x1a\x5a\x36\x55\x43\xcb\xa6\x6a\
-\x68\xd9\x54\x0d\x2d\x9b\xaa\xa1\x65\x53\x35\xb4\x6c\xaa\x86\x96\
-\x4d\xd5\xd0\xb2\xa9\x1a\x5a\x36\x55\x43\xcb\xa6\x6a\x68\xd9\x54\
-\x0d\x2d\x9b\xaa\xa1\x65\x53\x35\xb4\x6c\xaa\x86\x96\x4d\xd5\xd0\
-\xb2\xa9\x1a\x5a\x36\x55\x43\xcb\xa6\x6a\x68\xd9\x54\x0d\x2d\x1f\
-\x45\xad\x6a\x58\xcc\x87\x51\xab\x1a\xd6\xf2\x71\xd4\xaa\x86\xa5\
-\xec\x88\x5a\xd5\xb0\x92\x3d\x51\xab\x1a\x16\xb2\x2b\x6a\x55\xc3\
-\x3a\xf6\x45\xad\x6a\x58\xc6\xce\xa8\x55\x0d\xab\xd8\x1b\xb5\xaa\
-\x61\x11\xbb\xa3\x56\x35\xac\x61\x7f\xd4\xaa\x86\x25\x1c\x88\x5a\
-\xd5\xb0\x82\x23\x51\xab\x1a\x16\x70\x28\x6a\x55\xc3\xfc\x8e\x45\
-\xad\x6a\x98\xde\xc1\xa8\x55\x0d\xb3\x3b\x1a\xb5\xaa\x61\x72\x87\
-\xa3\x56\x35\xcc\xed\x78\xd4\xaa\x86\xa9\x9d\x88\x5a\xd5\x30\xb3\
-\x33\x51\xab\x1a\x26\x76\x2a\x6a\x55\xc3\xbc\xce\x45\xad\x6a\x98\
-\xd6\xc9\xa8\x55\x0d\xb3\x3a\x1b\xb5\xaa\x61\x52\xa7\xa3\x56\x35\
-\xcc\xe9\x7c\xd4\xaa\x86\x29\xbd\x11\xb5\xaa\x61\x46\xef\x44\xad\
-\x6a\x98\xd0\x5b\x51\xab\x1a\xe6\xf3\x5e\xd4\xaa\x86\xe9\xbc\x19\
-\xb5\xaa\x61\x36\xef\x46\xad\x6a\x98\xcc\xdb\x51\xab\x1a\xe6\xf2\
-\x7e\xd4\xaa\x86\xa9\x5c\x10\xb5\xaa\x61\x26\x57\x44\xad\x6a\x98\
-\xc8\x25\x51\x6f\x9f\x46\x3f\xe3\x88\x5f\xfd\x1a\xca\xae\x89\x7a\
-\xa9\xbf\xfa\x37\xbf\xbd\xe8\xd1\x90\xa6\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
-\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
-\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
-\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
-\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
-\xaa\xa1\x46\xd5\x50\xb3\x54\xd5\xbf\x1b\xbd\x16\xac\x60\xa5\xaa\
-\xbf\x55\x35\xec\xa0\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
-\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
-\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
-\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
-\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
-\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
-\x43\xcd\x52\x55\xff\x7e\xf4\x5a\xb0\x02\x55\x43\x8d\xaa\xa1\x46\
-\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
-\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
-\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
-\x43\x8d\xaa\xa1\x66\xa9\xaa\xff\x30\x7a\x2d\x58\x81\xaa\xa1\x46\
-\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
-\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x66\xa5\xaa\
-\xff\xf8\xa7\xd1\x6b\xc1\x0a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
-\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\
-\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
-\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
-\x46\xd5\x50\xa3\x6a\xa8\x59\xa9\xea\x3f\xab\x1a\x76\x50\x35\xd4\
-\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
-\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\x4b\x55\xfd\
-\x97\xd1\x6b\xc1\x0a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
-\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
-\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\
-\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
-\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
-\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
-\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
-\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x96\xaa\xfa\xaf\xa3\xd7\x82\x15\
-\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
-\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
-\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
-\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
-\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\x2b\x55\xfd\x37\x55\
-\xc3\x0e\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
-\xa1\x46\xd5\x50\xb3\x54\xd5\x7f\x1f\xbd\x16\xac\x40\xd5\x50\xa3\
-\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
-\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
-\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
-\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
-\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
-\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\xcd\x52\x55\xff\
-\x63\xf4\x5a\xb0\x02\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
-\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
-\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
-\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
-\xd5\x50\xb3\x52\xd5\x5f\xaa\x1a\x76\x50\x35\xd4\xa8\x1a\x6a\x54\
-\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\x4b\x55\xfd\xd5\xe8\xb5\x60\
-\x05\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
-\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
-\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
-\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xb3\x50\xd5\x5f\x7f\x33\
-\x7a\x2c\x58\xc2\x32\x55\x6b\x1a\x76\x5a\xa4\x6a\x4d\xc3\x6e\x4b\
-\x54\xad\x69\x38\x60\x81\xaa\x35\x0d\x87\x4c\x5f\xb5\xa6\xe1\xa0\
-\xc9\xab\xd6\x34\x1c\x36\x75\xd5\x9a\x86\x13\x26\xae\x5a\xd3\x70\
-\xca\xb4\x55\x6b\x1a\x4e\x9a\xb4\x6a\x4d\xc3\x69\x53\x56\xad\x69\
-\x78\xc3\x84\x55\x6b\x1a\xde\x32\x5d\xd5\x9a\x86\x37\x4d\x56\xb5\
-\xa6\xe1\x6d\x53\x55\xad\x69\xb8\xc0\x44\x55\x6b\x1a\x2e\x31\x4d\
-\xd5\x9a\x86\x8b\x4c\x52\xb5\xa6\xe1\x32\x53\x54\xad\x69\xb8\xd0\
-\x04\x55\x6b\x1a\x2e\x35\xbc\x6a\x4d\xc3\xc5\x06\x57\xad\x69\xb8\
-\xdc\xd0\xaa\x35\x0d\x37\x18\x58\xb5\xa6\xe1\x16\xc3\xaa\xd6\x34\
-\xdc\x64\x50\xd5\x9a\x86\xdb\x0c\xa9\x5a\xd3\x70\xa3\x01\x55\x6b\
-\x1a\x6e\xf5\x78\xd5\x9a\x86\x9b\x3d\x5c\xb5\xa6\xe1\x76\x8f\x56\
-\xad\x69\x78\xc0\x83\x55\x6b\x1a\x1e\xf1\x58\xd5\x9a\x86\x87\x3c\
-\x54\xb5\xa6\xe1\x31\x8f\x54\xad\x69\x78\xd0\x03\x55\x6b\x1a\x1e\
-\x75\x7b\xd5\x9a\x86\x87\xdd\x5c\xb5\xa6\xe1\x71\xb7\x56\xad\x69\
-\x18\xe0\xc6\xaa\x35\x0d\x43\xdc\x56\xb5\xa6\x61\x90\x9b\xaa\xd6\
-\x34\x0c\x73\x4b\xd5\x9a\x86\x81\x6e\xa8\x5a\xd3\x30\xd4\xe5\x55\
-\x6b\x1a\x06\xbb\xb8\x6a\x4d\xc3\x70\x97\x56\xad\x69\x98\xc0\x85\
-\x55\x6b\x1a\xa6\x70\x59\xd5\x9a\x86\x49\x5c\x54\xb5\xa6\x61\x1a\
-\x97\x54\xad\x69\x98\xc8\x05\x55\x6b\x1a\xa6\xf2\x76\xd5\x9a\x86\
-\xc9\xbc\x59\xb5\xa6\x61\x3a\x6f\x55\xad\x69\x98\xd0\x1b\x55\x6b\
-\x1a\xa6\x74\xba\x6a\x4d\xc3\xa4\x4e\x56\xad\x69\x98\xd6\xa9\xaa\
-\x35\x0d\x13\x3b\x51\xb5\xa6\x61\x6a\x87\xab\xd6\x34\x4c\xee\x60\
-\xd5\x9a\x86\xe9\x1d\xaa\x5a\xd3\xb0\x80\x03\x55\x6b\x1a\x96\xb0\
-\xbb\x6a\x4d\xc3\x22\x76\x56\xad\x69\x58\xc6\xae\xaa\x35\x0d\x0b\
-\xd9\x51\xb5\xa6\x61\x29\x1f\x56\xad\x69\x58\xcc\x4b\xd3\x10\xf3\
-\xd2\x34\xc4\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x4b\xd3\x10\xf3\xd2\
-\x34\xc4\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x4b\xd3\x10\xf3\xd2\x34\
-\xc4\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x4b\xd3\x10\xf3\xd2\x34\xc4\
-\xbc\x34\x0d\x31\x2f\x4d\x43\xcc\x17\xa3\x0f\xe0\x19\xff\x04\x21\
-\xd0\x80\x64\x8d\x91\x64\x11\x00\x00\x00\x25\x74\x45\x58\x74\x64\
-\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x31\x37\x2d\
-\x30\x36\x2d\x31\x32\x54\x30\x33\x3a\x33\x34\x3a\x35\x31\x2b\x30\
-\x38\x3a\x30\x30\x84\x9a\x03\x36\x00\x00\x00\x25\x74\x45\x58\x74\
-\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x31\x36\
-\x2d\x30\x34\x2d\x31\x36\x54\x31\x35\x3a\x35\x32\x3a\x31\x38\x2b\
-\x30\x38\x3a\x30\x30\x8b\xf9\x5a\xba\x00\x00\x00\x54\x74\x45\x58\
-\x74\x73\x76\x67\x3a\x62\x61\x73\x65\x2d\x75\x72\x69\x00\x66\x69\
-\x6c\x65\x3a\x2f\x2f\x2f\x68\x6f\x6d\x65\x2f\x64\x62\x2f\x73\x76\
-\x67\x5f\x69\x6e\x66\x6f\x2f\x73\x76\x67\x2f\x35\x33\x2f\x35\x34\
-\x2f\x35\x33\x35\x34\x66\x32\x37\x62\x35\x30\x31\x33\x36\x37\x63\
-\x36\x64\x33\x33\x63\x37\x31\x33\x38\x37\x66\x38\x62\x33\x30\x61\
-\x33\x2e\x73\x76\x67\xf7\x2c\xcc\x83\x00\x00\x00\x00\x49\x45\x4e\
-\x44\xae\x42\x60\x82\
-\x00\x00\x02\xb8\
+\x00\x00\x03\x8a\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
 \x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
 \x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
 \x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
 \x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
 \x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
 \x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
-\x6b\x42\xcf\x00\x00\x01\xba\x49\x44\x41\x54\x78\xda\xed\x99\xbb\
-\x2e\x45\x41\x14\x86\xbf\x25\x1a\x8d\x42\xa2\xd0\x68\x34\x1a\x11\
-\x97\x84\x53\x48\x44\x21\x2a\x2a\x3a\xc7\x23\xf0\x08\x3c\x02\xb5\
-\x82\xe3\x52\xd0\xa9\x44\x25\x51\x68\x5c\x0a\x8d\x82\x46\xa3\x90\
-\x28\x24\x22\x11\xf2\x2b\xce\x14\xbb\xd0\xc8\xd9\x7b\xcf\x3e\x66\
-\x7d\x0f\x30\x6b\xff\x5f\xd6\xcc\xac\xc9\x06\xc7\x71\x1c\xc7\x71\
-\x1c\xc7\x71\x1c\xc7\x71\x9c\x3f\xa2\xdf\x59\x2c\xa1\x6e\xb7\xa4\
-\x46\xab\xeb\x74\x94\xa3\x29\xf7\xf0\x35\xe0\x06\x58\x4e\x4a\x80\
-\xa4\x4e\x49\xeb\xc0\x05\x30\x90\xc7\x9a\x9d\xb1\x43\xfd\x21\xfc\
-\x20\xb0\x0f\x8c\xe5\xb9\x6e\x5b\x74\x80\xa4\x3a\x70\x95\x77\x78\
-\xa8\x78\x07\x48\xea\x05\xb6\x81\xf9\xa2\x6a\x54\x56\x80\xa4\x59\
-\x60\x07\xe8\x2b\xb2\x4e\xe5\xb6\x80\xa4\x2e\x49\x9b\xc0\x69\xd1\
-\xe1\xa1\x62\x1d\x20\x69\x08\x38\x00\x86\xca\xaa\x59\x89\x0e\x90\
-\x64\x92\x56\x69\x1e\x74\xa5\x85\x87\x0a\x74\x80\xa4\x7e\x60\x17\
-\x98\x8e\x51\x3f\x6a\x07\x84\x91\xf9\x36\x56\xf8\x68\x02\x32\x73\
-\xfc\x11\xd0\x13\x2b\x3c\x44\xd8\x02\x61\x8e\xdf\x23\xa7\x51\xb6\
-\x55\x4a\xeb\x80\x22\xe6\xf8\x3c\x28\xa5\x03\x8a\x9a\xe3\xf3\xa0\
-\x12\xd7\xe0\xbf\x17\x60\x66\xf7\xc0\x24\xb0\x01\x7c\xc7\x0e\x5d\
-\xba\x80\x20\xe1\xcb\xcc\xd6\x81\x29\xe0\x31\x76\xf0\xd2\x05\x64\
-\x44\x5c\x02\xa3\x34\x6f\x82\xe8\x44\x39\x03\xcc\xec\xcd\xcc\xea\
-\xc0\x12\xf0\x9a\x9c\x80\x8c\x88\x63\x60\x04\x38\x4f\x52\x40\x90\
-\xf0\x04\xcc\x00\x6b\xc0\x67\x72\x02\x82\x04\x99\xd9\x26\x30\x0e\
-\xdc\x25\x27\x20\x23\xe2\x0e\x98\x00\xb6\x00\x25\x27\x20\x48\xf8\
-\x30\xb3\x55\x60\x0e\x78\x4e\x4e\x40\x46\xc4\x19\x30\x0c\x9c\x24\
-\x29\x20\x48\x78\x31\xb3\x05\x60\x05\x78\x4f\x4e\x40\x46\x44\x83\
-\xe6\x01\x79\x9d\xa4\x80\x20\xa1\x9a\xef\x89\x18\x7f\x87\x25\xd5\
-\x24\x3d\x48\x6a\xf9\xa6\x68\x9b\x0e\xc8\x12\xde\x13\x63\xc0\x61\
-\xec\x6f\x71\x1c\xc7\x71\x1c\xc7\x71\x1c\xc7\x71\x1c\xa7\xfd\xf8\
-\x01\x73\xbb\xad\xea\xb8\xa9\x09\x48\x00\x00\x00\x25\x74\x45\x58\
-\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\
-\x32\x2d\x30\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x30\x33\
-\x2b\x30\x30\x3a\x30\x30\xcc\xfd\x4d\xd2\x00\x00\x00\x25\x74\x45\
-\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\
-\x32\x32\x2d\x30\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x30\x3a\x30\
-\x33\x2b\x30\x30\x3a\x30\x30\xbd\xa0\xf5\x6e\x00\x00\x00\x00\x49\
-\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x04\x7b\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\xe1\x00\x00\x00\xe1\x08\x03\x00\x00\x00\x09\x6d\x22\x48\
-\x00\x00\x00\x75\x50\x4c\x54\x45\x00\x00\x00\xff\xff\xff\xe7\xe7\
-\xe7\xf2\xf2\xf2\x0b\x0b\x0b\xdd\xdd\xdd\xe3\xe3\xe3\xcb\xcb\xcb\
-\xf9\xf9\xf9\xbf\xbf\xbf\xae\xae\xae\xce\xce\xce\x8b\x8b\x8b\xe0\
-\xe0\xe0\xf5\xf5\xf5\x0f\x0f\x0f\xa3\xa3\xa3\x5b\x5b\x5b\x22\x22\
-\x22\x94\x94\x94\x71\x71\x71\xc4\xc4\xc4\x36\x36\x36\x1c\x1c\x1c\
-\x47\x47\x47\x18\x18\x18\xba\xba\xba\x8d\x8d\x8d\x4f\x4f\x4f\x62\
-\x62\x62\xd4\xd4\xd4\x82\x82\x82\x41\x41\x41\x69\x69\x69\x2b\x2b\
-\x2b\x9c\x9c\x9c\x7d\x7d\x7d\x4d\x4d\x4d\x2f\x2f\x2f\x8a\x37\xee\
-\x59\x00\x00\x03\xc1\x49\x44\x41\x54\x78\x9c\xed\xdd\x6b\x53\xea\
-\x40\x0c\x06\x60\x5b\xee\x20\x48\x05\x04\x41\x50\x41\xfd\xff\x3f\
-\xf1\x50\xe6\x78\x46\x93\xc0\x5e\xe8\x21\xbb\x99\xf7\xf9\x6c\x67\
-\x92\xa1\xdd\x6b\x76\xbd\xbb\x03\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x49\x75\
-\x3f\x1d\x8c\x3a\xdd\xb2\x2c\xc7\xbb\xde\x7a\xfa\x5a\x3d\x68\x47\
-\xd4\xa0\xa7\xcd\xa2\x55\x70\x93\xd1\xe1\x45\x3b\xb4\x26\xec\xa7\
-\xa5\x90\xdd\xb7\xfe\x60\xab\x1d\xe0\x95\xb6\xbb\x0b\xe9\xfd\x4d\
-\xf2\xd0\xd6\x8e\x32\x5e\xd5\x75\xe6\x77\x32\xd4\x0e\x34\xd2\x72\
-\xe4\x97\x5f\xed\x5e\x3b\xd8\x18\x1f\xfe\xf9\x1d\x8d\x1f\xb5\xe3\
-\x0d\x36\x08\x4a\xf0\xe8\x5d\x3b\xe2\x40\xe3\xd0\x04\x73\x7b\x53\
-\xa5\xfe\xcf\x69\xa6\x1d\x75\x80\xa8\x04\x8b\xe2\x55\x3b\x6e\x6f\
-\x9d\xb8\x04\x8b\x22\x97\x31\xce\x3a\x36\xc1\xa2\xaf\x1d\xba\x9f\
-\x79\x74\x82\x45\xb1\xd0\x0e\xde\xcb\x15\x09\xe6\xf1\x9e\x06\x77\
-\x84\xbf\x8c\xb5\xc3\x77\xfb\xbc\x2a\xc1\xa2\xa8\xb4\x13\x70\x3a\
-\x37\x99\x28\x07\xb3\x79\xb5\x5a\xad\xaa\xf9\x6c\x7d\x69\x38\x30\
-\xd2\x4e\xc0\x65\x25\xa7\xb7\x21\xc3\xce\x79\xef\x6c\x8a\xa9\xcf\
-\xa5\x16\x52\x7e\xd2\x2c\xf7\xf1\xdc\xf7\xba\xb9\x79\xcc\x41\xda\
-\x42\xc8\xd3\x33\x7f\xfb\xd2\xcf\xf1\x35\xbd\xe7\x11\x5f\x98\x33\
-\xc8\xeb\x1b\xb7\x8b\x36\x06\x6f\x67\x2e\xae\xc3\x4c\xa4\x0c\xdf\
-\x6e\x13\x6a\x24\x16\xee\xe5\xf9\xc2\x9b\x94\xe1\xc7\x8d\x62\x8d\
-\xc2\x06\x6c\x1d\xc7\x03\x43\x21\xc3\x73\xdf\x6d\x12\x58\xc0\x2b\
-\xd7\x13\x42\x86\x83\x5b\x44\x1a\x8b\x76\xe5\x3b\xe7\x13\x42\xef\
-\x92\x74\x63\x4a\x83\x75\xaf\xbd\x08\x13\x11\xd7\x9b\xad\xe9\x89\
-\x06\xeb\x7e\x64\xc9\x33\x4c\x79\xf0\xfd\x4e\x62\xed\x79\x3c\xc3\
-\xbb\xfd\xee\x7f\x8f\x33\xde\x86\xc4\xea\xb3\xb4\xc4\x7b\xfd\x94\
-\xdf\xd2\x29\x89\xd5\x67\x26\xc4\xd7\x74\xdc\xcd\x93\x1e\xba\x40\
-\xb3\xf7\x78\x86\x67\x98\xf2\x4a\x06\x6d\xfa\x7d\x9e\xe1\x9b\x37\
-\x29\xef\xd3\xac\xbb\xdd\x7a\x93\xb7\x2c\x5b\x47\x93\xc9\xc4\xe7\
-\x19\xbe\xb4\x9a\xf8\xf4\x29\x18\x4b\x30\x83\x75\x8c\x20\xac\x0b\
-\x4d\x7f\x92\x1f\xe8\x95\x25\x58\x6a\x87\xd4\x30\xbe\x96\x91\x72\
-\x43\x13\xc3\xfc\x67\xc8\x07\xde\x5e\x0d\x70\x46\x78\x7f\x9f\xf4\
-\xfc\x37\x5c\xc5\x5f\xd2\xa5\x76\x4c\xcd\xe2\xc3\xee\xb5\x76\x48\
-\xcd\xa2\x73\x91\xa3\x67\xed\x98\x1a\xf5\xc5\x13\x34\xf6\x15\xf2\
-\x77\xb4\xa5\x1d\x52\xb3\x84\xcd\x99\x1c\xf6\x47\xfd\x09\x4b\xa5\
-\xb6\xde\x51\xa1\x95\x49\x79\x72\x1f\x8e\x8f\xb8\x8d\x7d\x84\x52\
-\x59\x9f\xcf\x9a\x47\x36\xa4\x82\x14\xe7\x06\x40\x4e\xa4\x04\x4d\
-\x4d\x29\xb6\x42\x82\xb9\x97\x7b\xff\x22\x0c\xb7\x6d\xfd\x82\xd2\
-\xae\xa8\xa9\x04\x85\xad\x18\x5b\x09\x4a\xd5\x09\xb6\xc6\x6a\xc2\
-\x60\xf4\x53\x3b\xa6\x46\x09\xd5\x28\xb6\x7e\x41\x61\x46\x68\xeb\
-\x1b\x14\x16\x9e\xe6\xda\x21\x35\x8b\x8f\x46\xad\xed\xc2\xb0\x12\
-\x28\x63\xeb\x4e\xbc\x99\xb1\xb6\x45\xc1\x7f\xc2\x2f\xed\x88\x1a\
-\xf6\x4e\x13\xcc\xe9\x8c\x8c\x17\xda\xd9\xdb\x9a\xd3\xd7\xe8\x4f\
-\x98\xdb\x61\x35\x27\x3a\xed\x35\xd7\xcc\xb0\x52\x94\x7c\x8e\x71\
-\xf9\xa2\x93\x0a\xed\x78\x9a\x47\x12\xf4\xa9\x79\xcb\x0b\x3d\x88\
-\x91\xd7\x89\x51\x1f\x74\x4c\xfa\xa4\x1d\x50\xe3\x66\xe6\x3f\x43\
-\xb2\x11\x63\xaf\xaf\xa0\x9d\x85\xad\x5d\x98\x13\x52\xb7\x98\x72\
-\x89\x65\xa4\x9d\xf9\x0c\x97\xcb\xe7\xa3\x87\xa3\x76\x4d\x3b\x1c\
-\x00\x00\x00\x00\x00\x00\x00\xb8\xc2\x76\xd8\xeb\xec\x16\x07\x53\
-\x75\x96\x3f\x6d\xfe\x1d\x4c\x2f\xcd\x6d\xac\xd5\x1e\xba\xc6\x17\
-\xa2\x1e\xc9\xcd\x02\x29\x1f\xba\x8f\xc3\x0a\xf6\x92\xbe\xc1\x24\
-\x02\xbd\x8b\xa0\x30\x56\x15\x2c\x5e\x43\x93\xf2\xf5\x17\xe1\x84\
-\x92\xc4\xd4\xef\x83\x0a\x24\xde\x0a\x7d\xd0\x8e\xaa\x49\xe2\x9d\
-\xb4\xa6\xf6\xb9\xa5\x04\x93\xbe\x69\x27\x98\x98\xa1\xa9\x4d\x52\
-\xfb\xbf\xa1\x78\xb7\x9e\xa9\xef\x50\xbc\xd4\xd4\xd4\x79\x4a\x5a\
-\x88\x71\x62\xaa\x48\xff\x59\x48\xd0\x58\xf1\xa5\x70\xc5\xb7\xb5\
-\xca\x3d\xdb\x2d\x69\x8d\x1e\xc9\xeb\x1b\xbb\xff\xe2\x8e\x1e\xab\
-\x9c\x58\x2b\x62\xaf\xed\x7f\x1c\x98\xb1\x36\xfd\xfd\x56\x0d\x4e\
-\x23\xf0\x72\x68\xaf\x2e\xf1\x87\x7d\x7e\xff\x4f\x06\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\xe0\x96\xfe\x00\xef\xff\x1f\x4f\xab\x8f\xe8\xa8\x00\x00\
-\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x02\xea\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x50\x00\x00\x00\x50\x08\x06\x00\x00\x00\x8e\x11\xf2\xad\
-\x00\x00\x00\xca\x69\x43\x43\x50\x43\x75\x73\x74\x6f\x6d\x00\x00\
-\x18\x95\x63\x60\x60\xdc\xce\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\
-\x45\x41\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\
-\x01\x37\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\
-\xe5\xc7\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\
-\x98\xcd\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\
-\xad\x03\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\
-\x03\xd9\x3e\x40\xb6\x40\x3a\x12\x3b\x09\x89\x9d\x92\x5a\x9c\x0c\
-\x64\xc7\x00\xd9\xd1\x08\xbf\xe5\xcf\x67\x60\xb0\xf8\xc2\xc0\xc0\
-\x3c\x11\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x6d\x84\x98\
-\xca\x42\x06\x06\xfe\x56\x06\x86\x6d\x57\x10\x62\x9f\x03\xc1\xfe\
-\x65\x14\x3b\x53\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\
-\x4a\x84\xfb\x8a\xc9\xd8\x08\x62\x2f\x2c\x8c\xa8\x0a\x00\x67\xd9\
-\x31\x35\xdc\xee\x19\x62\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\
-\x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\x00\x25\x74\
+\x6b\x42\xcf\x00\x00\x02\x8c\x49\x44\x41\x54\x78\xda\xed\x99\xcd\
+\x6f\x8c\x51\x14\x87\x1f\x43\xc6\xac\x4b\x7c\xd4\x74\xa5\x58\xd8\
+\xd2\xea\xc6\x82\xea\x5a\xc4\xd8\x21\xe2\x63\x4b\xca\x42\x84\x84\
+\x88\x34\x4d\xc3\x96\xb2\x10\xfd\x3b\x1a\x54\x24\x1a\xb1\xf3\xb1\
+\xf1\x4d\x75\xa6\xfe\x84\x46\x67\x2c\xee\x5b\x99\xc8\xb9\xaf\xf3\
+\x7e\xbf\x13\xe7\x49\xde\xcd\x7d\xef\xfd\xcd\xef\x9c\x99\x7b\xee\
+\xc7\x80\x61\x18\x86\x61\x18\x86\x61\x18\x86\x61\x18\x86\xf1\x7f\
+\xb1\x26\xe1\xf8\x0a\xb0\x0d\xa8\x03\x9b\x80\xaa\x72\xdc\x0b\x60\
+\xe1\xaf\xb6\x3a\x30\xa2\x1c\xbf\x0c\xfc\x0c\x34\x7e\x00\xed\x3c\
+\x92\xd5\xcd\x18\xf0\x00\x58\x02\x3a\x31\x9e\x86\xa0\xd9\x88\xa9\
+\xd5\x02\xee\x03\xa3\x79\x04\x3e\x02\x3c\x8b\x69\x34\xab\x04\x74\
+\x3f\x73\xc0\x70\x56\xc1\x9f\x07\x56\x52\x30\x99\x65\x02\x3a\xb8\
+\xe9\x70\x9d\xe4\xd3\xfb\x0f\x15\x60\x26\x25\x73\x79\x24\x60\xf5\
+\x79\x14\x78\x0f\x65\x9d\x22\x01\x13\xc0\xf1\x90\xf7\xbf\x80\x0f\
+\xb8\xa2\xb4\xac\x4c\xea\x92\xa7\x6d\x56\x39\xbe\x8a\x2b\xba\x83\
+\x21\x31\x9c\xc0\x15\xc8\x2b\x4a\x4d\x91\x63\xf8\x33\xfc\x11\x38\
+\x0d\xf4\x25\xf9\x80\x84\xf4\x01\x67\x80\x4f\xf8\xa7\xc3\x91\xb8\
+\xe2\x35\xe0\x9b\x47\xf8\x2e\xfa\x25\x2f\x0f\xd6\x03\xf7\x3c\x5e\
+\xbf\x04\xb1\x44\xe6\x92\x47\x70\xb2\xe8\x68\x43\x98\xf2\x78\x1e\
+\x8f\x23\xf6\x4e\x10\x7a\x82\xa2\xb0\x14\xc8\x5a\xe4\x65\xfa\x6d\
+\x54\xa1\x5d\xc8\x99\xdc\x53\x74\x84\x0a\x86\x3c\xde\x77\x48\x9d\
+\x7d\x15\xf4\x80\xd0\xf6\x1a\x78\xa5\x34\x31\x0e\xec\x4b\x39\xb0\
+\x79\xe0\x8e\xa2\xdf\x4b\xdc\x37\xbe\x5b\x88\xe9\xbd\x36\x01\x75\
+\xa1\x4d\xbb\x44\x11\x04\xdf\x88\xd0\x3f\x6d\x66\x85\x04\x0c\x48\
+\x1d\x7d\xf3\xb9\x5f\x68\xfb\x5e\x60\x40\x51\x91\xbc\x6e\x8d\x92\
+\x80\x8e\xd0\x96\xda\xd6\x32\x07\x24\xaf\x52\x4c\xde\x04\x2c\x0a\
+\x6d\x03\xf4\x0e\xd2\x14\x6e\x4a\x1d\x7d\x35\x60\x41\x68\x8b\x72\
+\xdc\x9c\xcf\x20\xa8\x28\x9a\x87\x94\x31\x79\xd9\x89\xbc\x94\xec\
+\xcd\x20\xb0\xb4\x19\xf6\x78\x1f\x8c\x2a\x24\x6d\x84\xe6\x28\xff\
+\x46\xe8\xb9\xe0\xfb\x4d\x1c\xb1\x8b\xc8\x99\x9c\x2a\x3a\xca\x10\
+\x6e\x7b\x3c\x5f\x88\x23\x56\x03\xbe\x7a\x04\xa7\x71\x07\x90\xb2\
+\x50\xc3\x5d\xd1\x49\x5e\x3f\x27\xf1\x7a\xd4\x23\xba\x7a\xca\x3a\
+\x0b\x6c\x28\x30\xf0\x8d\xc0\x39\xfc\x5f\x54\x1b\x38\x1c\x26\xa0\
+\x59\xdb\x27\x80\xcb\x21\xef\x57\x70\x77\x03\x2d\xf4\x17\x22\x37\
+\x71\x87\x96\x6e\xf6\x03\xd7\x94\xe3\xab\xc0\x16\x60\x3b\x6e\xde\
+\xfb\xb8\x05\x5c\xd5\xe7\x53\xa6\x82\xbb\x5e\xea\xb5\x2b\xb1\x87\
+\x28\x0a\xb6\xa6\xa2\xb7\x81\x93\xb8\x42\x92\xfb\xfd\x7b\x0c\x3a\
+\xc0\x0d\xe0\x54\x16\x7e\x87\x80\xa7\x94\xf7\x17\xf0\x98\x9c\xf6\
+\x2a\x07\x71\x2b\x41\xb3\x04\x09\x58\xc4\x5d\x87\x49\x47\xf8\x7f\
+\x92\xc6\x5f\x63\xfd\xb8\xbd\xf7\x66\xf2\xfd\x6b\xac\x15\x68\x34\
+\xe9\x8d\xa9\x69\x18\x86\x61\x18\x86\x61\x18\x86\x61\x18\x86\x61\
+\x94\x82\xdf\x05\xaa\xaa\x63\x48\xd7\xde\xb7\x00\x00\x00\x25\x74\
 \x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\
-\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x35\x31\x3a\
-\x32\x36\x2b\x30\x30\x3a\x30\x30\x57\xdf\xca\x8c\x00\x00\x00\x25\
+\x30\x32\x32\x2d\x30\x36\x2d\x31\x30\x54\x30\x37\x3a\x34\x36\x3a\
+\x34\x34\x2b\x30\x30\x3a\x30\x30\x88\x07\x40\x56\x00\x00\x00\x25\
 \x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\
-\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x35\x31\
-\x3a\x32\x36\x2b\x30\x30\x3a\x30\x30\x26\x82\x72\x30\x00\x00\x01\
-\x64\x49\x44\x41\x54\x78\x9c\xed\xdb\xbd\x4a\xc4\x40\x18\x46\xe1\
-\xa3\x9d\x08\xb9\x1a\xff\x2a\x0b\xb5\xf3\xe7\x7a\x05\x2b\x1b\xbd\
-\x12\x6d\x37\x82\x8a\x0a\xa2\x55\x60\x91\x35\x26\xf9\x3e\x26\xb3\
-\xee\x79\x60\xca\x90\x97\xc3\xb4\x03\x92\x24\x49\x52\xfd\x1a\xe0\
-\x06\x38\x9e\x7b\xc8\x3a\x6a\x80\x7b\xe0\x0b\x78\xc6\x88\xa3\x2c\
-\xc7\xeb\x8e\x11\x07\x5a\x15\xcf\x88\x03\xf5\xc5\x33\xe2\x1f\x86\
-\xc4\x33\xe2\x2f\xc6\xc4\x33\xe2\x0f\x0d\x70\xc7\xb8\x78\xdd\x79\
-\x04\x76\xca\x4f\xae\xc7\x94\x9b\xd7\x9d\x17\xe0\xa4\xfc\xe4\x7a\
-\x18\x2f\xc0\x78\x01\xc6\x0b\x88\xc6\x3b\x2d\x3f\xb9\x1e\xc6\x0b\
-\x30\x5e\x40\x24\xde\x2b\xc6\x0b\xc5\x3b\x2b\x3f\xb9\x1e\xc6\x0b\
-\x30\x5e\x80\xf1\x02\x22\xf1\xde\x80\xf3\xf2\x93\xeb\x61\xbc\x00\
-\xe3\x05\x18\x2f\xc0\x78\x01\x91\x78\xef\xc0\x45\xf9\xc9\xf5\x30\
-\x5e\x80\xf1\x02\xa2\xf1\x2e\xcb\x4f\xae\x87\xf1\x02\x8c\x17\x60\
-\xbc\x25\xdb\x13\xbe\xf9\x04\x3e\x02\xff\xdc\x0a\x7c\xfb\x6f\xec\
-\x02\xb7\x4c\xbf\x85\x57\xe5\x27\xd7\xc7\x88\x09\x8c\x98\xc0\x88\
-\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\
-\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\
-\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\xc0\x88\x09\x8c\x98\
-\x20\xf2\xe0\xfa\x81\x0d\x7f\x70\xdd\x99\x72\x13\x17\xc0\xde\x1c\
-\x63\x6b\x35\x26\xe2\x02\xd8\x9f\x67\x66\xdd\x86\x44\x6c\x31\x5e\
-\xaf\xbe\x88\x2d\x70\x30\xdf\xb4\xf5\xb1\x2a\x62\x0b\x1c\xce\x39\
-\x6a\xdd\x2c\x47\x7c\xc2\x78\x93\x34\xc0\x35\x70\x34\xf7\x10\x49\
-\x92\x24\x6d\xb6\x6f\xa1\xa7\x43\x48\x8a\xcb\xd9\x64\x00\x00\x00\
+\x32\x30\x32\x32\x2d\x30\x36\x2d\x31\x30\x54\x30\x37\x3a\x34\x36\
+\x3a\x34\x34\x2b\x30\x30\x3a\x30\x30\xf9\x5a\xf8\xea\x00\x00\x00\
 \x00\x49\x45\x4e\x44\xae\x42\x60\x82\
 \x00\x00\x66\x36\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x02\x00\x00\x00\x02\x00\x08\x06\x00\x00\x00\xf4\x78\xd4\xfa\
 \x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\x0d\xd7\x00\x00\x0d\xd7\
 \x01\x42\x28\x9b\x78\x00\x00\x00\x19\x74\x45\x58\x74\x53\x6f\x66\
@@ -4010,888 +4888,172 @@
 \x4c\x64\x59\x56\xcf\xb2\xac\x96\x65\x59\x00\xa0\x92\x65\x99\x9f\
 \x65\x99\x97\x65\x99\x93\xa6\xa9\x31\xc6\xc0\x18\x93\x01\x48\x8d\
 \x31\xa9\x31\x26\x31\xc6\x24\x00\x62\x63\x4c\x6c\x8c\xe9\x02\xe8\
 \x1a\x63\x3a\x00\xda\xc6\x98\x36\x80\x45\x63\xcc\xa3\xc6\x98\x79\
 \x63\xcc\x1d\xc6\x98\x5b\xc2\x30\x7c\x48\xe9\x3f\x07\x91\xf5\xfe\
 \x3f\xbd\x14\x5c\x2a\xa2\x77\xbe\x90\x00\x00\x00\x00\x49\x45\x4e\
 \x44\xae\x42\x60\x82\
-\x00\x00\x01\x9e\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x30\x00\x00\x00\x30\x08\x06\x00\x00\x00\x57\x02\xf9\x87\
-\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
-\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
-\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
-\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
-\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
-\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
-\x6b\x42\xcf\x00\x00\x00\xa0\x49\x44\x41\x54\x68\xde\xed\xd9\x31\
-\x0e\x82\x40\x00\x05\xd1\xd1\x73\x68\xed\x35\x2d\xbd\x8a\xde\xc0\
-\xc2\x1b\x19\x13\xc2\x01\xb0\x30\xda\xca\xca\xee\xfe\xa8\xf3\x12\
-\x3a\x42\xfe\x40\xa0\x01\x24\xe9\x57\xec\x81\x69\xe6\x71\x48\x8f\
-\x5d\x32\xbe\x6a\xc4\xaa\xe0\xdc\xa9\xf3\x4d\x99\xb5\x6d\xdd\x79\
-\x54\x75\x06\xe8\xdf\x95\x7c\x85\x9e\x5a\x7f\x8d\x8a\x36\x7d\xfd\
-\x3b\x60\x40\x9a\x01\x69\x06\xa4\x19\x90\x66\x40\x9a\x01\x69\x06\
-\xa4\x19\x90\x66\x40\x9a\x01\x69\x06\xa4\x7d\x12\x30\x36\xdc\x33\
-\xf4\x08\xb8\x34\x0c\x38\x37\xbc\xf6\xcb\x0e\xb8\x51\xfe\x43\xe3\
-\xdd\x71\x05\x36\x3d\x02\x00\xb6\xc0\x89\xc7\x23\x5f\x3a\x7c\x00\
-\x8e\x3d\xc7\x4b\x52\x3d\x77\x26\x42\x46\xf6\xa2\xc9\xef\x56\x00\
-\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\
-\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x38\x54\x30\x38\
-\x3a\x35\x36\x3a\x30\x33\x2b\x30\x30\x3a\x30\x30\xac\xcb\x38\xb5\
-\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\
-\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x38\x54\x30\
-\x38\x3a\x35\x36\x3a\x30\x33\x2b\x30\x30\x3a\x30\x30\xdd\x96\x80\
-\x09\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x11\xab\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x03\xd4\x00\x00\x03\xd8\x08\x03\x00\x00\x00\x0c\xc8\x41\xcd\
-\x00\x00\x00\xe1\x69\x43\x43\x50\x73\x52\x47\x42\x00\x00\x18\x95\
-\x63\x60\x60\x3c\xcd\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\x45\x41\
-\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\x01\x37\
-\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\xe5\xc7\
-\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\x98\xcd\
-\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\xad\x03\
-\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\x03\xd9\
-\x3e\x40\xb6\x42\x3a\x12\x3b\x09\x89\x9d\x92\x5a\x9c\x0c\x64\xe7\
-\x00\xd9\xf1\x08\xbf\xe5\xcf\x67\x60\xb0\xf8\xc2\xc0\xc0\x3c\x11\
-\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x1d\x84\x98\xca\x42\
-\x06\x06\xfe\x56\x06\x86\x6d\x97\x11\x62\x9f\xfd\xc1\xfe\x65\x14\
-\x3b\x54\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\x4a\x04\
-\x4b\x33\x83\x02\x34\x2d\x8d\x81\xe1\xd3\x72\x06\x06\xde\x48\x06\
-\x06\xe1\x0b\x0c\x0c\x5c\xd1\x10\x77\x80\x01\x6b\x31\x30\xa0\x49\
-\x0c\x27\x42\x00\x00\x72\xd8\x36\x84\xa3\x1f\x47\xb3\x00\x00\x00\
-\x57\x50\x4c\x54\x45\xff\xff\xff\xe8\xe8\xe8\x7f\x7f\x7f\x11\x11\
-\x11\xcc\xcc\xcc\x00\x00\x00\x15\x15\x15\xd1\xd1\xd1\x30\x30\x30\
-\x55\x55\x55\x88\x88\x88\x33\x33\x33\x66\x66\x66\x0a\x0a\x0a\xbe\
-\xbe\xbe\xbf\xbf\xbf\x0b\x0b\x0b\xc0\xc0\xc0\xc1\xc1\xc1\x0e\x0e\
-\x0e\xc7\xc7\xc7\x0f\x0f\x0f\xc8\xc8\xc8\xc9\xc9\xc9\x10\x10\x10\
-\xca\xca\xca\xcb\xcb\xcb\xff\xff\xff\x00\x00\x00\x2d\x21\xd7\x57\
-\x00\x00\x00\x1d\x74\x52\x4e\x53\x00\xff\xff\xff\xff\xff\xff\xff\
-\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\
-\xff\xff\xff\xff\x00\xce\xc7\xf9\x42\x00\x00\x00\x09\x70\x48\x59\
-\x73\x00\x00\x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\
-\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\
-\x65\x00\x32\x30\x31\x37\x2d\x30\x36\x2d\x31\x32\x54\x30\x33\x3a\
-\x33\x34\x3a\x35\x31\x2b\x30\x38\x3a\x30\x30\x84\x9a\x03\x36\x00\
-\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\
-\x66\x79\x00\x32\x30\x31\x36\x2d\x30\x34\x2d\x31\x36\x54\x31\x35\
-\x3a\x35\x32\x3a\x31\x38\x2b\x30\x38\x3a\x30\x30\x8b\xf9\x5a\xba\
-\x00\x00\x00\x58\x7a\x54\x58\x74\x73\x76\x67\x3a\x62\x61\x73\x65\
-\x2d\x75\x72\x69\x00\x00\x08\x99\x4b\xcb\xcc\x49\xb5\xd2\xd7\xd7\
-\xcf\xc8\xcf\x4d\xd5\x4f\x49\xd2\x2f\x2e\x4b\x8f\xcf\xcc\x4b\xcb\
-\x07\x31\xf4\x4d\x8d\xf5\x4d\x4d\x80\xa4\xa9\x49\x9a\x91\x79\x92\
-\xa9\x81\xa1\xb1\x99\x79\xb2\x59\x8a\xb1\x71\xb2\xb9\xa1\xb1\x85\
-\x79\x9a\x45\x92\xb1\x41\xa2\xb1\x1e\x50\x29\x00\x17\x9a\x14\xea\
-\xbe\x3f\x86\x2f\x00\x00\x0f\x1e\x49\x44\x41\x54\x78\x9c\xed\xdb\
-\x59\x8e\x2b\xc7\x15\x45\x51\xb9\xd4\xd9\xcf\x7d\x6f\x6b\xfe\x03\
-\x35\x04\x43\xd2\x6b\xaa\x8a\xd9\x31\x23\x62\x6b\xad\x11\x9c\xfb\
-\xb1\x41\x82\x99\xfc\xea\x2b\x7e\x15\x7e\x33\x7a\x00\x70\xa9\x6f\
-\xbe\x7e\x19\x3d\x01\xb8\xd0\x37\x5f\x7f\xfb\xad\xaa\xa1\xe3\xc7\
-\xa6\x55\x0d\x1d\xff\x6f\x5a\xd5\x50\xf1\x53\xd3\xaa\x86\x86\x5f\
-\x9a\x56\x35\x14\x7c\xdc\xb4\xaa\x61\x7d\x9f\x36\xad\x6a\x58\xdd\
-\xe7\x4d\xab\x1a\xd6\xf6\x65\xd3\xaa\x86\x95\xbd\xd6\xb4\xaa\x61\
-\x5d\xaf\x37\xad\x6a\x58\xd5\x5b\x4d\xab\x1a\xd6\xf4\x76\xd3\xaa\
-\x86\x15\xbd\xd7\xb4\xaa\x61\x3d\xef\x37\xad\x6a\x58\xcd\xa3\xa6\
-\x55\x0d\x6b\x79\xdc\xb4\xaa\x61\x25\x5b\x9a\x56\x35\xac\x63\x5b\
-\xd3\xaa\x86\x55\x6c\x6d\x5a\xd5\xb0\x86\xed\x4d\xab\x1a\x56\xb0\
-\xa7\x69\x55\xc3\xfc\xf6\x35\xad\x6a\x98\xdd\xde\xa6\x55\x0d\x73\
-\xdb\xdf\xb4\xaa\x61\x66\x47\x9a\x56\x35\xcc\xeb\x58\xd3\xaa\x86\
-\x59\x1d\x6d\x5a\xd5\x30\xa7\xe3\x4d\xab\x1a\x66\x74\xa6\x69\x55\
-\xc3\x7c\xce\x35\xad\x6a\x98\xcd\xd9\xa6\x55\x0d\x73\x39\xdf\xb4\
-\xaa\x61\x26\x57\x34\xad\x6a\x98\xc7\x35\x4d\xab\x1a\x66\x71\x55\
-\xd3\xaa\x86\x39\x5c\xd7\xb4\xaa\x61\x06\x57\x36\xad\x6a\x18\xef\
-\xda\xa6\x55\x0d\xa3\x5d\xdd\xb4\xaa\x61\xac\xeb\x9b\x56\x35\x8c\
-\xf4\x8c\xa6\x55\x0d\xe3\x3c\xa7\x69\x55\xc3\x28\xcf\x6a\x5a\xd5\
-\x30\xc6\xf3\x9a\x56\x35\x8c\xf0\xcc\xa6\x55\x0d\xf7\x7b\x6e\xd3\
-\xaa\x86\xbb\x3d\xbb\x69\x55\xc3\xbd\x9e\xdf\xb4\xaa\xe1\x4e\x77\
-\x34\xad\x6a\xb8\xcf\x3d\x4d\xab\x1a\xee\x72\x57\xd3\xaa\x86\x7b\
-\xdc\xd7\xb4\xaa\xe1\x0e\x77\x36\xad\x6a\x78\xbe\x7b\x9b\x56\x35\
-\x3c\xdb\xdd\x4d\xab\x1a\x9e\xeb\xfe\xa6\x55\x0d\xcf\x34\xa2\x69\
-\x55\xc3\xf3\x8c\x69\x5a\xd5\xf0\x2c\xa3\x9a\x56\x35\x3c\xc7\xb8\
-\xa6\x55\x0d\xcf\x30\xb2\x69\x55\xc3\xf5\xc6\x36\xad\x6a\xb8\xda\
-\xe8\xa6\x55\x0d\xd7\x1a\xdf\xb4\xaa\xe1\x4a\x33\x34\xad\x6a\xb8\
-\xce\x1c\x4d\xab\x1a\xae\x32\x4b\xd3\xaa\x86\x6b\xcc\xd3\xb4\xaa\
-\xe1\x0a\x33\x35\xad\x6a\x38\x6f\xae\xa6\x55\x0d\x67\xcd\xd6\xb4\
-\xaa\xe1\x9c\xf9\x9a\x56\x35\x9c\x31\x63\xd3\xaa\x86\xe3\xe6\x6c\
-\x5a\xd5\x70\xd4\xac\x4d\xab\x1a\x8e\x99\xb7\x69\x55\xc3\x11\x33\
-\x37\xad\x6a\xd8\x6f\xee\xa6\x55\x0d\x7b\xcd\xde\xb4\xaa\x61\x9f\
-\xf9\x9b\x56\x35\xec\xb1\x42\xd3\xaa\x86\xed\xd6\x68\x5a\xd5\xb0\
-\xd5\x2a\x4d\xab\x1a\xb6\x59\xa7\x69\x55\xc3\x26\xdf\x7f\x37\x3a\
-\xd5\x1d\x54\x0d\x1b\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
-\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
-\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
-\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
-\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
-\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
-\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
-\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
-\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
-\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
-\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
-\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
-\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\
-\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
-\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
-\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
-\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\
-\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
-\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
-\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
-\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
-\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
-\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
-\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
-\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
-\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
-\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
-\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
-\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
-\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
-\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
-\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
-\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\
-\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\
-\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\
-\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\
-\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\
-\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\
-\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\
-\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\
-\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\
-\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\
-\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\
-\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\
-\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\
-\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\
-\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\
-\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\
-\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\
-\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\
-\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\
-\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\
-\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\
-\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\xa8\x51\x35\xd4\xa8\x1a\x6a\
-\x54\x0d\x35\xaa\x86\x1a\x55\x43\x8d\xaa\xa1\x46\xd5\x50\xa3\x6a\
-\xa8\x51\x35\xd4\xa8\x1a\x6a\x54\x0d\x35\xaa\x86\x1a\x55\x43\xcd\
-\xaf\xb3\xea\xdf\x41\xd8\x6f\x47\x97\xba\xc7\x55\x55\x8f\xbe\x03\
-\xf8\xc9\x45\x55\x8f\x3e\x03\xf8\xd9\x35\x55\x8f\xbe\x02\xf8\xc5\
-\x25\x55\x8f\x3e\x02\xf8\xc8\x15\x55\x8f\xbe\x01\xf8\xd8\x05\x55\
-\x8f\x3e\x01\xf8\xc4\xf9\xaa\x47\x5f\x00\x7c\xea\x74\xd5\xa3\x0f\
-\x00\x3e\x73\xb6\xea\xd1\xfb\x81\xcf\x9d\xac\x7a\xf4\x7c\xe0\x0b\
-\xe7\xaa\x1e\xbd\x1e\xf8\xd2\xa9\xaa\x47\x8f\x07\x5e\x71\xa6\xea\
-\xd1\xdb\x81\xd7\x9c\xa8\x7a\xf4\x74\xe0\x55\xc7\xab\x1e\xbd\x1c\
-\x78\xdd\xe1\xaa\x47\x0f\x07\xde\x70\xb4\xea\xd1\xbb\x81\xb7\x1c\
-\xac\x7a\xf4\x6c\xe0\x4d\xc7\xaa\x1e\xbd\x1a\x78\xdb\xa1\xaa\x47\
-\x8f\x06\xde\x71\xa4\xea\xd1\x9b\x81\xf7\x1c\xa8\x7a\xf4\x64\xe0\
-\x5d\xfb\xab\x1e\xbd\x18\x78\xdf\xee\xaa\x47\x0f\x06\x1e\xd8\x5b\
-\xf5\xe8\xbd\xc0\x23\x3b\xab\x1e\x3d\x17\x78\x68\x5f\xd5\xa3\xd7\
-\x02\x8f\xed\xaa\x7a\xf4\x58\x60\x83\x3d\x55\x8f\xde\x0a\x6c\xb1\
-\xa3\xea\xd1\x53\x81\x4d\xb6\x57\x3d\x7a\x29\xb0\xcd\xe6\xaa\x47\
-\x0f\x05\x36\xda\x5a\xf5\xe8\x9d\xc0\x56\x1b\xab\x1e\x3d\x13\xd8\
-\x6c\x5b\xd5\xa3\x57\x02\xdb\x6d\xaa\x7a\xf4\x48\x60\x87\x2d\x55\
-\x8f\xde\x08\xec\xb1\xa1\xea\xd1\x13\x81\x5d\x1e\x57\x3d\x7a\x21\
-\xb0\xcf\xc3\xaa\x47\x0f\x04\x76\x7a\x54\xf5\xe8\x7d\xc0\x5e\x0f\
-\xaa\x1e\x3d\x0f\xd8\xed\xfd\xaa\x47\xaf\x03\xf6\x7b\xb7\xea\xd1\
-\xe3\x80\x03\xde\xab\x7a\xf4\x36\xe0\x88\x77\xaa\x1e\x3d\x0d\x38\
-\xe4\xed\xaa\x47\x2f\x03\x8e\x79\xb3\xea\xd1\xc3\x80\x83\xde\xaa\
-\x7a\xf4\x2e\xe0\xa8\x37\xaa\x1e\x3d\x0b\x38\xec\xf5\xaa\x47\xaf\
-\x02\x8e\x7b\xb5\xea\xd1\xa3\x80\x13\x5e\xab\x7a\xf4\x26\xe0\x8c\
-\x57\xaa\x1e\x3d\x09\x38\xe5\xcb\xaa\x47\x2f\x02\xce\xf9\xa2\xea\
-\xd1\x83\x80\x93\x3e\xaf\x7a\xf4\x1e\xe0\xac\x17\x51\x43\xcc\x8b\
-\xa8\x21\xe6\x45\xd4\x10\xf3\x22\x6a\x88\x79\x11\x35\xc4\xbc\x88\
-\x1a\x62\x5e\x44\x0d\x31\x2f\xa2\x86\x98\x17\x51\x43\xcc\x8b\xa8\
-\x21\xe6\x45\xd4\x10\xf3\x22\x6a\x88\x79\x11\x35\xc4\xbc\x88\x1a\
-\x5a\x3e\x88\x1a\x52\x3e\xf8\xfa\x0d\x29\x1f\xfc\x50\x06\x29\x1f\
-\x3c\xd2\x82\x94\x0f\x5e\x3e\x81\x94\x0f\x5e\x13\x85\x94\x0f\xfe\
-\xd0\x01\x29\x3f\x35\x2d\x6a\x68\xf8\xb9\x69\x51\x43\xc2\x2f\x4d\
-\x8b\x1a\x0a\x3e\x6a\x5a\xd4\x10\xf0\x71\xd3\xa2\x86\xf5\x7d\xd2\
-\xb4\xa8\x61\x79\x9f\x36\x2d\x6a\x58\xdd\x67\x4d\x8b\x1a\x16\xf7\
-\x79\xd3\xa2\x86\xb5\x7d\xd1\xb4\xa8\x61\x69\x5f\x36\x2d\x6a\x58\
-\xd9\x2b\x4d\x8b\x1a\x16\xf6\x5a\xd3\xa2\x86\x75\xbd\xda\xb4\xa8\
-\x61\x59\xaf\x37\x2d\x6a\x58\xd5\x1b\x4d\x8b\x1a\x16\xf5\x56\xd3\
-\xa2\x86\x35\xbd\xd9\xb4\xa8\x61\x49\x6f\x37\x2d\x6a\x58\xd1\x3b\
-\x4d\x8b\x1a\x16\xf4\x5e\xd3\xa2\x86\xf5\xbc\xdb\xb4\xa8\x61\x39\
-\xef\x37\x2d\x6a\x58\xcd\x83\xa6\x45\x0d\x8b\x79\xd4\xb4\xa8\x61\
-\x2d\x0f\x9b\x16\x35\x2c\xe5\x71\xd3\xa2\x86\x95\x6c\x68\x5a\xd4\
-\xb0\x90\x2d\x4d\x8b\x1a\xd6\xb1\xa9\x69\x51\xc3\x32\xb6\x35\x2d\
-\x6a\x58\xc5\xc6\xa6\x45\x0d\x8b\xd8\xda\xb4\xa8\x61\x0d\x9b\x9b\
-\x16\x35\x2c\x61\x7b\xd3\xa2\x86\x15\xec\x68\x5a\xd4\xb0\x80\x3d\
-\x4d\x8b\x1a\xe6\xb7\xab\x69\x51\xc3\xf4\xf6\x35\x2d\x6a\x98\xdd\
-\xce\xa6\x45\x0d\x93\xdb\xdb\xb4\xa8\x61\x6e\xbb\x9b\x16\x35\x4c\
-\x6d\x7f\xd3\xa2\x86\x99\x1d\x68\x5a\xd4\x30\xb1\x23\x4d\x8b\x1a\
-\xe6\x75\xa8\x69\x51\xc3\xb4\x8e\x35\x2d\x6a\x98\xd5\xc1\xa6\x45\
-\x0d\x93\x3a\xda\xb4\xa8\x61\x4e\x87\x9b\x16\x35\x4c\xe9\x78\xd3\
-\xa2\x86\x19\x9d\x68\x5a\xd4\x30\xa1\x33\x4d\x8b\x1a\xe6\x73\xaa\
-\x69\x51\xc3\x74\xce\x35\x2d\x6a\x98\xcd\xc9\xa6\x45\x0d\x93\x39\
-\xdb\xb4\xa8\x61\x2e\xa7\x9b\x16\x35\x4c\xe5\x7c\xd3\xa2\x86\x99\
-\x5c\xd0\xb4\xa8\x61\x22\x57\x34\x2d\x6a\x98\xc7\x25\x4d\x7f\xf5\
-\x07\x28\xfb\xfd\xe8\x4e\xf7\x78\xb9\xa4\x69\x48\xfb\xd3\x1f\x47\
-\x87\xba\xc3\x35\x9f\xd3\x90\xa6\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
-\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
-\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
-\x45\xd3\xd0\xf2\x67\x4d\x43\xca\x9f\xff\x32\x3a\xd4\x1d\x34\x0d\
-\x0f\x69\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
-\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
-\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
-\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
-\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xf2\x57\
-\x4d\x43\x8a\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\
-\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\
-\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\
-\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
-\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xf2\x37\x4d\
-\x43\x8a\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\xe5\x1f\x7f\x1f\x1d\xea\x0e\x9a\x86\x87\x34\x0d\x2d\x9a\
-\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
-\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\
-\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\
-\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xf9\xc7\x3f\x47\x87\
-\xba\x83\xa6\xe1\x21\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
-\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
-\xa1\x45\xd3\xd0\xf2\x2f\x4d\x43\x8a\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
-\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\
-\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\
-\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\
-\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\
-\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\xcb\xbf\x35\x0d\x29\
-\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
-\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
-\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
-\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\xcb\xbf\xff\x33\x3a\xd4\
-\x1d\x34\x0d\x0f\x69\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\
-\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\
-\x2d\x9a\x86\x16\x4d\x43\xcb\x7f\x35\x0d\x29\x9a\x86\x16\x4d\x43\
-\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\
-\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\
-\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
-\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
-\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\
-\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\
-\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x7e\xd0\x34\xa4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
-\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\
-\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\
-\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\
-\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\x96\x1f\xbe\x1e\
-\x1d\xea\x0e\x9a\x86\x87\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\
-\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\
-\x9a\x86\x16\x4d\x43\xcb\x37\x9a\x86\x14\x4d\x43\x8b\xa6\xa1\x45\
-\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\x1a\x5a\x34\x0d\x2d\x9a\x86\
-\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\xa2\x69\x68\xd1\x34\xb4\x68\
-\x1a\x5a\x34\x0d\x2d\x9a\x86\x16\x4d\x43\x8b\xa6\xa1\x45\xd3\xd0\
-\xa2\x69\x88\xf9\xfe\xbb\xd1\xa5\x6e\xa7\x69\xd8\x62\x9d\xaa\x35\
-\x0d\xdb\xac\x52\xb5\xa6\x61\xab\x35\xaa\xd6\x34\x6c\xb7\x42\xd5\
-\x9a\x86\x3d\xe6\xaf\x5a\xd3\xb0\xcf\xec\x55\x6b\x1a\xf6\x9a\xbb\
-\x6a\x4d\xc3\x7e\x33\x57\xad\x69\x38\x62\xde\xaa\x35\x0d\xc7\xcc\
-\x5a\xb5\xa6\xe1\xa8\x39\xab\xd6\x34\x1c\x37\x63\xd5\x9a\x86\x33\
-\xe6\xab\x5a\xd3\x70\xce\x6c\x55\x6b\x1a\xce\x9a\xab\x6a\x4d\xc3\
-\x79\x33\x55\xad\x69\xb8\xc2\x3c\x55\x6b\x1a\xae\x31\x4b\xd5\x9a\
-\x86\xab\xcc\x51\xb5\xa6\xe1\x3a\x33\x54\xad\x69\xb8\xd2\xf8\xaa\
-\x35\x0d\xd7\x1a\x5d\xb5\xa6\xe1\x6a\x63\xab\xd6\x34\x5c\x6f\x64\
-\xd5\x9a\x86\x67\x18\x57\xb5\xa6\xe1\x39\x46\x55\xad\x69\x78\x96\
-\x31\x55\x6b\x1a\x9e\x67\x44\xd5\x9a\x86\x67\xba\xbf\x6a\x4d\xc3\
-\x73\xdd\x5d\xb5\xa6\xe1\xd9\xee\xad\x5a\xd3\xf0\x7c\x77\x56\xad\
-\x69\xb8\xc3\x7d\x55\x6b\x1a\xee\x71\x57\xd5\x9a\x86\xbb\xdc\x53\
-\xb5\xa6\xe1\x3e\x77\x54\xad\x69\xb8\xd3\xf3\xab\xd6\x34\xdc\xeb\
-\xd9\x55\x6b\x1a\xee\xf6\xdc\xaa\x35\x0d\xf7\x7b\x66\xd5\x9a\x86\
-\x11\x9e\x57\xb5\xa6\x61\x8c\x67\x55\xad\x69\x18\xe5\x39\x55\x6b\
-\x1a\xc6\x79\x46\xd5\x9a\x86\x91\xae\xaf\x5a\xd3\x30\xd6\xd5\x55\
-\x6b\x1a\x46\xbb\xb6\x6a\x4d\xc3\x78\x57\x56\xad\x69\x98\xc1\x75\
-\x55\x6b\x1a\xe6\x70\x55\xd5\x9a\x86\x59\x5c\x53\xb5\xa6\x61\x1e\
-\x57\x54\xad\x69\x98\xc9\xf9\xaa\x35\x0d\x73\x39\x5b\xb5\xa6\x61\
-\x36\xe7\xaa\xd6\x34\xcc\xe7\x4c\xd5\x9a\x86\x19\x1d\xaf\x5a\xd3\
-\x30\xa7\xa3\x55\x6b\x1a\x66\x75\xac\x6a\x4d\xc3\xbc\x8e\x54\xad\
-\x69\x98\xd9\xfe\xaa\x35\x0d\x73\xdb\x5b\xb5\xa6\x61\x76\xfb\xaa\
-\xd6\x34\xcc\x6f\x4f\xd5\x9a\x86\x15\x6c\xaf\x5a\xd3\xb0\x86\xad\
-\x55\x6b\x1a\x56\xb1\xad\x6a\x4d\xc3\x3a\xb6\x54\xad\x69\x58\xc9\
-\xe3\xaa\x35\x0d\x6b\x79\x54\xb5\xa6\x61\x35\xef\x57\xad\x69\x58\
-\xcf\x7b\x55\x6b\x1a\x56\xf4\x76\xd5\x9a\x86\x35\xbd\x55\xb5\xa6\
-\x61\x55\xaf\x57\xad\x69\x58\xd7\x6b\x55\x6b\x1a\x56\xf6\x65\xd5\
-\x9a\x86\xb5\x7d\x5e\xb5\xa6\x61\x75\x9f\x56\xad\x69\x58\xdf\xc7\
-\x55\x6b\x1a\x0a\x7e\xa9\x5a\xd3\xd0\xf0\x53\xd5\x9a\x86\x8a\xff\
-\x57\xad\x69\xe8\xf8\xb1\x6a\x4d\x43\xc9\xf7\xdf\x69\x1a\x5a\x7e\
-\x33\x7a\x00\xb7\xf9\x1f\x60\x09\x80\x64\x76\x94\x1f\xe0\x00\x00\
-\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
-\x00\x00\x05\x14\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x40\x00\x00\x00\x40\x08\x06\x00\x00\x00\xaa\x69\x71\xde\
-\x00\x00\x00\x04\x67\x41\x4d\x41\x00\x00\xb1\x8f\x0b\xfc\x61\x05\
-\x00\x00\x00\x20\x63\x48\x52\x4d\x00\x00\x7a\x26\x00\x00\x80\x84\
-\x00\x00\xfa\x00\x00\x00\x80\xe8\x00\x00\x75\x30\x00\x00\xea\x60\
-\x00\x00\x3a\x98\x00\x00\x17\x70\x9c\xba\x51\x3c\x00\x00\x00\x06\
-\x62\x4b\x47\x44\x00\x00\x00\x00\x00\x00\xf9\x43\xbb\x7f\x00\x00\
-\x00\x09\x70\x48\x59\x73\x00\x00\x00\x60\x00\x00\x00\x60\x00\xf0\
-\x6b\x42\xcf\x00\x00\x04\x16\x49\x44\x41\x54\x78\xda\xed\x9b\x4b\
-\x68\x1e\x55\x18\x86\x9f\x2f\x74\x21\xad\x4d\xef\x56\x17\x5a\x2f\
-\xa0\x29\xa9\x2b\x4b\x11\x05\x4b\xac\xa2\x88\x28\x8a\x1b\x29\x9a\
-\x76\x2f\x16\xdc\x08\x82\x78\x59\x89\x88\xd0\x42\x8b\x0b\xef\x0b\
-\xa5\x2e\xda\x8d\xb8\x11\xba\xd0\x4d\x05\x71\x63\x5a\x53\x6b\x4b\
-\xd3\x82\x36\xa6\x86\x9a\xa4\xea\xaa\x8f\x8b\x99\x60\x1a\x66\xfe\
-\x7f\x26\x99\x4b\x6a\xff\x77\xf9\xcf\x99\x7f\xce\xf3\xce\xf7\xcd\
-\x9c\xf3\x9d\x33\xd0\x53\x4f\x3d\xf5\x74\x0d\x2b\x9a\xba\x90\xba\
-\x11\xd8\x02\xdc\x05\x6c\x02\x56\x03\xd7\xa7\x87\x67\x80\x8b\xc0\
-\x18\x70\x02\x18\x89\x88\xf1\xb6\xcd\x59\x2c\x70\x9f\xfa\xb0\x7a\
-\x40\xfd\xc9\xf2\x3a\xae\xee\x57\x77\xa8\x7d\x6d\xf3\x94\x01\xdf\
-\xa0\xbe\xa9\x9e\x5b\x00\x74\x9e\xce\xaa\x6f\xa8\xeb\xdb\xe6\xeb\
-\x04\xbe\x46\x7d\x57\x9d\xa9\x10\x7c\xbe\x66\xd4\x77\xd4\xd5\x6d\
-\xf3\xce\x05\x0f\x75\x58\x1d\xaf\x11\x7c\xbe\xce\xab\xcf\xb5\xcd\
-\x8e\xda\xaf\x1e\x6c\x10\x7c\xbe\x0e\xab\x6b\xda\x82\x1f\x54\x4f\
-\xb7\x08\x3f\xab\x53\xea\xe6\xa6\xe1\xb7\xa9\x13\x6d\x93\xcf\xd1\
-\xa4\x7a\xff\x42\x58\x4a\x8f\x03\xd4\xfb\x80\xaf\x81\xe5\x8d\xba\
-\xde\x5d\x97\x80\x87\x22\xe2\x68\x6d\x06\xa8\x83\xc0\x37\xc0\xda\
-\xb6\x69\x73\xf4\x07\xf0\x40\x44\x1c\xaf\xdc\x00\x93\x57\xcf\x0f\
-\xc0\x6d\x6d\x53\x76\xd1\x29\xe0\x9e\x88\xf8\xb3\x48\xe3\x32\x23\
-\xac\x0f\xae\x02\x78\x80\x3b\x80\xf7\x8b\x36\x2e\x64\x80\x3a\x0c\
-\x3c\xdd\x36\x59\x09\x3d\xa3\xee\x2c\xd2\xb0\x6b\x0a\x98\xbc\x67\
-\x47\x81\x1b\xda\xa6\x2a\xa9\x71\x60\x20\x22\x2e\x76\x6a\x54\x24\
-\x02\x5e\xbd\x0a\xe1\x01\x36\x02\xaf\x74\x6b\xd4\x31\x02\xd4\x75\
-\xc0\x19\xfe\x9b\xb6\x2e\x46\x5f\x02\xa7\x81\x17\x1b\x34\xe1\x12\
-\x70\x6b\x44\x5c\xc8\x6b\xd0\x2d\x02\xf6\x54\x04\x0f\xf0\x77\x44\
-\xec\x01\x76\xa5\x1d\x6b\x42\x2b\x80\x17\x3a\x35\xc8\x35\xc0\x64\
-\x0e\xbe\xab\xea\x1e\x45\xc4\x27\xc0\x56\xe0\xc7\x86\x4c\xd8\x6d\
-\x87\x7a\x42\xa7\x08\xd8\x01\xdc\x5c\x47\x8f\x22\x62\x14\xd8\x06\
-\xec\x6b\xc0\x80\x5b\x80\xed\x0b\x31\xe0\xa9\x3a\x7b\x15\x11\xff\
-\x34\x98\x12\xb9\x2c\x9d\x0c\x78\xb0\xe6\x4e\xcd\x1a\xd1\x44\x4a\
-\x0c\x95\x32\x40\xbd\x91\xa4\x78\xd9\x88\xd2\x94\xb8\x17\xf8\xb8\
-\xa6\x4b\x0c\xaa\x99\xaf\xf2\xbc\x08\xd8\xd2\x14\xfc\x1c\x13\xfe\
-\x8a\x88\xdd\xc0\x30\xd5\xa7\x44\x00\x83\x65\x0c\x68\xec\xee\x67\
-\x18\xf1\x29\xf5\xa4\x44\x26\x53\x9e\x01\x9b\xda\x32\x20\x35\xa1\
-\x8e\x94\xc8\x9c\xc8\xe5\x19\xd0\xdf\xa6\x01\xa9\x09\x55\xa7\xc4\
-\xca\x32\x06\x54\x35\xfa\xab\xc2\x88\xaa\x52\xa2\x94\x01\xd7\x8c\
-\xf2\x0c\x98\x69\xbb\x63\xb3\x52\x9f\x07\xbe\x07\xee\x5e\xe4\x5f\
-\x4d\x67\xfd\xb8\x2c\xa7\xf1\xd4\x12\x00\x5f\x0e\xec\xa7\xba\xf9\
-\x48\x26\x53\x9e\x01\x63\x2d\xc3\x0f\x00\x5f\xb0\xf8\xbb\x3e\x57\
-\x67\xb2\x7e\xcc\x4b\x81\xd1\x16\xe1\xab\x0a\xf9\x42\x4c\x79\x11\
-\x30\x02\x48\xb3\xfb\x07\xaa\x0e\xf9\x2b\xfe\x1e\x38\x96\x75\x20\
-\x33\x02\xd2\xcd\x09\x27\x1a\x84\x1f\x00\x8e\xd6\x04\x0f\x70\x2c\
-\x22\x26\x0a\x1b\x90\xea\x48\x43\xf0\xc3\xd4\x13\xf2\x85\x58\x3a\
-\x19\x70\xb8\x66\xf0\xeb\xd4\xbd\x24\xc3\xdd\x15\x75\x5e\x0b\x38\
-\x94\x77\x60\x59\x87\x93\x8e\x00\xe7\xa8\xa1\x2a\x54\xd3\x53\x3e\
-\x4f\x67\x81\x6f\xf3\x0e\xe6\x46\x40\x44\x5c\x06\x3e\xaa\x01\xbe\
-\x89\x90\x9f\xab\x0f\x53\x96\x6c\xce\x2e\x9d\x5d\x4f\xf2\xfe\xac\
-\x22\x44\xbf\x02\x7e\xa7\xbe\x07\x5d\x96\xa6\x49\xca\xe2\x93\x79\
-\x0d\x3a\xce\x05\xd2\x7a\xfa\x7b\x15\x75\xe6\xb1\x86\xe1\x01\x0e\
-\x74\x82\x87\x62\x4b\x63\xfd\x24\x83\x88\x9b\x1a\xee\xfc\x62\x75\
-\x9e\x64\x69\xac\xe3\x2a\x71\xd7\xd9\x60\x44\x4c\x01\x2f\xb7\x4d\
-\xb3\x00\xbd\x54\x74\x89\xbc\x90\xd4\xcf\xda\xde\x07\x53\x42\x07\
-\x8b\x72\x95\xd9\x20\xb1\x8a\x64\x83\xc4\xed\x8d\xde\xc7\xf2\x3a\
-\x09\x6c\x4d\x23\xb7\xab\x0a\x17\x44\xd2\x70\x7a\x94\xe4\x49\xbe\
-\x54\x75\x01\x78\xa2\x28\x7c\x29\x03\x52\x13\x4e\x02\x4f\xd2\xdc\
-\xe2\x66\x19\xcd\x00\x8f\xa7\x05\xd5\xc2\x2a\x5d\x12\x4b\x77\x61\
-\x0d\x01\x13\x65\xcf\xad\x51\x93\xc0\x23\x11\xf1\x5d\x63\x57\x54\
-\x37\xab\xbf\xb4\xfd\xb4\x53\x7f\x56\xdb\x59\xc7\x50\x57\xaa\x9f\
-\xb7\x08\x7f\xc8\xa5\xb0\x71\x5a\xdd\xa9\xfe\xd6\x20\xf8\xaf\xea\
-\xb3\x6d\x73\xcf\x37\x61\x95\xfa\xb6\x3a\x5d\x23\xf8\x94\xfa\x96\
-\xc9\xe8\x74\x69\x4a\x5d\xa7\xbe\xae\x8e\x55\x08\x3e\xa6\xbe\xa6\
-\x2e\xd5\x1d\xaa\x99\x46\xf4\xa9\x43\xea\x3e\x75\xa4\x24\xf0\xe5\
-\xf4\x9c\xbd\xea\x76\x6b\xfc\x64\xa6\xc9\xa2\xe7\x06\x92\x1a\xc0\
-\x9d\x24\xdb\x56\xd6\x72\xe5\x47\x53\x93\x24\xc5\x8b\xd9\x8f\xa6\
-\x96\xd2\x6b\xb6\xa7\x9e\x7a\xea\xe9\xff\xa9\x7f\x01\x81\x26\x51\
-\x3c\x61\xb0\x0b\xa4\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\x74\
-\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\x30\x32\x32\x2d\x30\x36\
-\x2d\x30\x33\x54\x31\x39\x3a\x35\x31\x3a\x35\x38\x2b\x30\x30\x3a\
-\x30\x30\x69\xd8\x7c\x72\x00\x00\x00\x25\x74\x45\x58\x74\x64\x61\
-\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\x32\x30\x32\x32\x2d\x30\
-\x36\x2d\x30\x33\x54\x31\x39\x3a\x35\x31\x3a\x35\x38\x2b\x30\x30\
-\x3a\x30\x30\x18\x85\xc4\xce\x00\x00\x00\x00\x49\x45\x4e\x44\xae\
-\x42\x60\x82\
-\x00\x00\x12\x3f\
-\x47\
-\x49\x46\x38\x39\x61\x20\x00\x20\x00\xf3\x00\x00\xca\xca\xca\x88\
-\x88\x88\xb1\xb1\xb1\xeb\xeb\xeb\xbf\xbf\xbf\xd4\xd4\xd4\x7f\x7f\
-\x7f\x3f\x3f\x3f\x6a\x6a\x6a\x55\x55\x55\x2a\x2a\x2a\x94\x94\x94\
-\xa9\xa9\xa9\x15\x15\x15\xff\xff\xff\x00\x00\x00\x21\xff\x0b\x4e\
-\x45\x54\x53\x43\x41\x50\x45\x32\x2e\x30\x03\x01\x00\x00\x00\x21\
-\xff\x0b\x58\x4d\x50\x20\x44\x61\x74\x61\x58\x4d\x50\x3c\x3f\x78\
-\x70\x61\x63\x6b\x65\x74\x20\x62\x65\x67\x69\x6e\x3d\x22\xef\xbb\
-\xbf\x22\x20\x69\x64\x3d\x22\x57\x35\x4d\x30\x4d\x70\x43\x65\x68\
-\x69\x48\x7a\x72\x65\x53\x7a\x4e\x54\x63\x7a\x6b\x63\x39\x64\x22\
-\x3f\x3e\x20\x3c\x78\x3a\x78\x6d\x70\x6d\x65\x74\x61\x20\x78\x6d\
-\x6c\x6e\x73\x3a\x78\x3d\x22\x61\x64\x6f\x62\x65\x3a\x6e\x73\x3a\
-\x6d\x65\x74\x61\x2f\x22\x20\x78\x3a\x78\x6d\x70\x74\x6b\x3d\x22\
-\x41\x64\x6f\x62\x65\x20\x58\x4d\x50\x20\x43\x6f\x72\x65\x20\x35\
-\x2e\x36\x2d\x63\x31\x31\x31\x20\x37\x39\x2e\x31\x35\x38\x33\x32\
-\x35\x2c\x20\x32\x30\x31\x35\x2f\x30\x39\x2f\x31\x30\x2d\x30\x31\
-\x3a\x31\x30\x3a\x32\x30\x20\x20\x20\x20\x20\x20\x20\x20\x22\x3e\
-\x20\x3c\x72\x64\x66\x3a\x52\x44\x46\x20\x78\x6d\x6c\x6e\x73\x3a\
-\x72\x64\x66\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x77\x77\x77\x2e\
-\x77\x33\x2e\x6f\x72\x67\x2f\x31\x39\x39\x39\x2f\x30\x32\x2f\x32\
-\x32\x2d\x72\x64\x66\x2d\x73\x79\x6e\x74\x61\x78\x2d\x6e\x73\x23\
-\x22\x3e\x20\x3c\x72\x64\x66\x3a\x44\x65\x73\x63\x72\x69\x70\x74\
-\x69\x6f\x6e\x20\x72\x64\x66\x3a\x61\x62\x6f\x75\x74\x3d\x22\x22\
-\x20\x78\x6d\x6c\x6e\x73\x3a\x78\x6d\x70\x3d\x22\x68\x74\x74\x70\
-\x3a\x2f\x2f\x6e\x73\x2e\x61\x64\x6f\x62\x65\x2e\x63\x6f\x6d\x2f\
-\x78\x61\x70\x2f\x31\x2e\x30\x2f\x22\x20\x78\x6d\x6c\x6e\x73\x3a\
-\x78\x6d\x70\x4d\x4d\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x6e\x73\
-\x2e\x61\x64\x6f\x62\x65\x2e\x63\x6f\x6d\x2f\x78\x61\x70\x2f\x31\
-\x2e\x30\x2f\x6d\x6d\x2f\x22\x20\x78\x6d\x6c\x6e\x73\x3a\x73\x74\
-\x52\x65\x66\x3d\x22\x68\x74\x74\x70\x3a\x2f\x2f\x6e\x73\x2e\x61\
-\x64\x6f\x62\x65\x2e\x63\x6f\x6d\x2f\x78\x61\x70\x2f\x31\x2e\x30\
-\x2f\x73\x54\x79\x70\x65\x2f\x52\x65\x73\x6f\x75\x72\x63\x65\x52\
-\x65\x66\x23\x22\x20\x78\x6d\x70\x3a\x43\x72\x65\x61\x74\x6f\x72\
-\x54\x6f\x6f\x6c\x3d\x22\x41\x64\x6f\x62\x65\x20\x50\x68\x6f\x74\
-\x6f\x73\x68\x6f\x70\x20\x43\x43\x20\x32\x30\x31\x35\x20\x28\x4d\
-\x61\x63\x69\x6e\x74\x6f\x73\x68\x29\x22\x20\x78\x6d\x70\x4d\x4d\
-\x3a\x49\x6e\x73\x74\x61\x6e\x63\x65\x49\x44\x3d\x22\x78\x6d\x70\
-\x2e\x69\x69\x64\x3a\x41\x45\x38\x30\x41\x41\x45\x34\x31\x42\x41\
-\x42\x31\x31\x45\x36\x39\x32\x45\x32\x44\x34\x41\x36\x32\x38\x30\
-\x37\x35\x33\x35\x45\x22\x20\x78\x6d\x70\x4d\x4d\x3a\x44\x6f\x63\
-\x75\x6d\x65\x6e\x74\x49\x44\x3d\x22\x78\x6d\x70\x2e\x64\x69\x64\
-\x3a\x41\x45\x38\x30\x41\x41\x45\x35\x31\x42\x41\x42\x31\x31\x45\
-\x36\x39\x32\x45\x32\x44\x34\x41\x36\x32\x38\x30\x37\x35\x33\x35\
-\x45\x22\x3e\x20\x3c\x78\x6d\x70\x4d\x4d\x3a\x44\x65\x72\x69\x76\
-\x65\x64\x46\x72\x6f\x6d\x20\x73\x74\x52\x65\x66\x3a\x69\x6e\x73\
-\x74\x61\x6e\x63\x65\x49\x44\x3d\x22\x78\x6d\x70\x2e\x69\x69\x64\
-\x3a\x41\x45\x38\x30\x41\x41\x45\x32\x31\x42\x41\x42\x31\x31\x45\
-\x36\x39\x32\x45\x32\x44\x34\x41\x36\x32\x38\x30\x37\x35\x33\x35\
-\x45\x22\x20\x73\x74\x52\x65\x66\x3a\x64\x6f\x63\x75\x6d\x65\x6e\
-\x74\x49\x44\x3d\x22\x78\x6d\x70\x2e\x64\x69\x64\x3a\x41\x45\x38\
-\x30\x41\x41\x45\x33\x31\x42\x41\x42\x31\x31\x45\x36\x39\x32\x45\
-\x32\x44\x34\x41\x36\x32\x38\x30\x37\x35\x33\x35\x45\x22\x2f\x3e\
-\x20\x3c\x2f\x72\x64\x66\x3a\x44\x65\x73\x63\x72\x69\x70\x74\x69\
-\x6f\x6e\x3e\x20\x3c\x2f\x72\x64\x66\x3a\x52\x44\x46\x3e\x20\x3c\
-\x2f\x78\x3a\x78\x6d\x70\x6d\x65\x74\x61\x3e\x20\x3c\x3f\x78\x70\
-\x61\x63\x6b\x65\x74\x20\x65\x6e\x64\x3d\x22\x72\x22\x3f\x3e\x01\
-\xff\xfe\xfd\xfc\xfb\xfa\xf9\xf8\xf7\xf6\xf5\xf4\xf3\xf2\xf1\xf0\
-\xef\xee\xed\xec\xeb\xea\xe9\xe8\xe7\xe6\xe5\xe4\xe3\xe2\xe1\xe0\
-\xdf\xde\xdd\xdc\xdb\xda\xd9\xd8\xd7\xd6\xd5\xd4\xd3\xd2\xd1\xd0\
-\xcf\xce\xcd\xcc\xcb\xca\xc9\xc8\xc7\xc6\xc5\xc4\xc3\xc2\xc1\xc0\
-\xbf\xbe\xbd\xbc\xbb\xba\xb9\xb8\xb7\xb6\xb5\xb4\xb3\xb2\xb1\xb0\
-\xaf\xae\xad\xac\xab\xaa\xa9\xa8\xa7\xa6\xa5\xa4\xa3\xa2\xa1\xa0\
-\x9f\x9e\x9d\x9c\x9b\x9a\x99\x98\x97\x96\x95\x94\x93\x92\x91\x90\
-\x8f\x8e\x8d\x8c\x8b\x8a\x89\x88\x87\x86\x85\x84\x83\x82\x81\x80\
-\x7f\x7e\x7d\x7c\x7b\x7a\x79\x78\x77\x76\x75\x74\x73\x72\x71\x70\
-\x6f\x6e\x6d\x6c\x6b\x6a\x69\x68\x67\x66\x65\x64\x63\x62\x61\x60\
-\x5f\x5e\x5d\x5c\x5b\x5a\x59\x58\x57\x56\x55\x54\x53\x52\x51\x50\
-\x4f\x4e\x4d\x4c\x4b\x4a\x49\x48\x47\x46\x45\x44\x43\x42\x41\x40\
-\x3f\x3e\x3d\x3c\x3b\x3a\x39\x38\x37\x36\x35\x34\x33\x32\x31\x30\
-\x2f\x2e\x2d\x2c\x2b\x2a\x29\x28\x27\x26\x25\x24\x23\x22\x21\x20\
-\x1f\x1e\x1d\x1c\x1b\x1a\x19\x18\x17\x16\x15\x14\x13\x12\x11\x10\
-\x0f\x0e\x0d\x0c\x0b\x0a\x09\x08\x07\x06\x05\x04\x03\x02\x01\x00\
-\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x21\xfe\x27\x47\x49\x46\x20\
-\x72\x65\x73\x69\x7a\x65\x64\x20\x6f\x6e\x20\x68\x74\x74\x70\x73\
-\x3a\x2f\x2f\x65\x7a\x67\x69\x66\x2e\x63\x6f\x6d\x2f\x72\x65\x73\
-\x69\x7a\x65\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdb\
-\xf0\xc9\x49\x2b\x21\x35\xeb\x3d\xef\xe5\xe0\xc4\x30\x94\xe0\x51\
-\x45\x11\x52\xe3\x38\x99\x9f\x94\xa6\xab\xd4\x92\x12\x8c\xc9\x73\
-\x6d\xb7\xb9\xd3\x63\xa6\xf2\xfd\x70\x3a\x5e\x01\x10\x5a\x2c\x58\
-\xc0\x24\x91\x32\x18\x54\x9c\x4e\xe8\x48\x37\x9d\x54\xab\x14\x2c\
-\xf6\x48\xfa\x74\xbf\xdf\xab\x38\x0b\x9c\xf4\xd0\x69\xcd\xfa\xc9\
-\x81\x5b\x41\x6b\x10\xdc\x37\xae\x83\x37\x06\x81\x82\x81\x3e\x76\
-\x60\x83\x88\x06\x2b\x0e\x8c\x8d\x8e\x89\x83\x8b\x8e\x93\x0f\x90\
-\x8a\x35\x93\x8d\x1c\x08\x9c\x21\x0d\x0d\x46\x9c\x9d\x1c\x9f\x9f\
-\x2b\xa2\xa2\x20\xa5\xa5\x1b\xa8\xa9\x09\xb0\x15\x0a\x0a\x0f\xab\
-\xac\x14\xae\x08\x12\xb0\xb1\x07\x07\x0f\xb3\xb3\x12\xb6\xa0\x13\
-\xae\x13\xbc\x09\xbe\xbe\xc1\xb4\x13\xab\x15\xa3\xbb\xbc\x0f\xcb\
-\xbf\xcd\x14\xa6\x21\xc9\xd5\xcb\x12\xc1\x46\xd3\xb1\xdd\xbe\xdf\
-\xe0\x3e\xdc\x12\xd6\x13\xd8\x35\xe9\xe4\xbf\xe6\xc2\xe8\x09\x14\
-\xeb\xec\xce\xe1\xf6\xde\xfa\x21\xe5\x3e\x11\x00\x21\xf9\x04\x09\
-\x04\x00\x0f\x00\x2c\x05\x00\x00\x00\x1b\x00\x20\x00\x00\x04\x1f\
-\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\
-\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x78\x3e\x45\x00\
-\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\
-\x00\x00\x04\xdd\xf0\xc9\x49\x2b\x63\x35\xeb\x3d\xef\xe5\xe0\xb4\
-\x2c\x94\x87\x4d\x04\x11\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\
-\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x73\x3d\x72\xc1\x5d\xc8\
-\x60\x60\xb5\x8e\x30\x21\xa5\x50\xa8\x30\x99\xce\x91\x49\x3a\xa1\
-\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\xbd\xd6\x30\xf6\xa9\x7b\x9c\xd1\
-\x1a\x75\x93\xf3\xae\x82\xd4\xa0\x37\x4f\x4c\xff\x6e\x10\x80\x81\
-\x80\x3c\x03\x85\x86\x85\x0f\x82\x8a\x08\x2b\x87\x8e\x03\x8b\x82\
-\x8d\x8f\x86\x89\x91\x84\x94\x1c\x09\x9b\x20\x0e\x0e\x03\x44\x9b\
-\x9c\x1c\x9e\x9e\x2b\xa2\xa2\x9d\xa5\xa6\x1a\xa8\xa9\x07\xb0\x15\
-\x0d\x0d\x0f\xab\xa5\x15\xae\x09\x12\xb0\xb1\x0a\x0a\x0f\xb3\xb3\
-\x12\xb6\x0e\x14\xae\x13\xbc\x07\xbe\xbe\xc1\xb4\x12\x03\xab\xb8\
-\xba\xc8\xbc\x0f\xcb\xbf\xcd\x14\xac\x20\xc9\xd6\xcb\x12\xc1\x44\
-\xbb\xd5\xde\xbe\xe0\xe1\x3c\xdd\x12\xd7\x13\xd9\x34\xea\xe5\xbf\
-\xe7\xc2\xe9\x07\x14\xec\xed\xce\xe2\xf7\xdf\xfb\x21\xe6\x3c\x22\
-\x00\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x01\x00\x01\x00\x1f\
-\x00\x1e\x00\x00\x04\x20\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\
-\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\
-\x6d\xdf\x78\xae\xaf\x11\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\
-\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdf\xf0\xc9\x49\xeb\x5a\
-\x35\xeb\x3d\xef\xe5\xe0\x64\x18\x94\x87\x4d\x0c\x13\x52\xe3\xd8\
-\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\
-\x57\x73\x3d\x72\xc1\x5d\x08\x81\x60\xb5\x8e\x30\x21\x85\x40\xa8\
-\x30\x99\xce\x91\x49\x3a\xa1\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\xbd\
-\xd6\x30\xf6\xa9\x7b\x9c\xd1\x1a\x75\x93\xf3\xae\x82\xd4\xa0\x37\
-\x4f\x4c\xff\x6e\x12\x72\x09\x3c\x05\x84\x85\x84\x0f\x09\x89\x8a\
-\x8b\x2b\x86\x8e\x05\x8b\x91\x82\x21\x8f\x86\x88\x92\x93\x8d\x95\
-\x1c\x07\x9d\x20\x03\xa0\x44\x9d\x9e\x1c\xa0\xa1\x21\xa3\xa3\x9f\
-\xa6\xa7\x19\xa9\xaa\x0a\xb1\x14\x0e\xb4\x0f\xac\xa6\x15\xaf\x07\
-\x12\xb1\xb2\x0d\x0d\x0f\xb4\xb5\xb6\xb7\x14\xa9\x14\xbd\x0a\xbf\
-\xbf\xc2\x0e\x13\xc5\xc6\xbb\x13\xc9\x0f\xca\x0d\x0a\xc1\xc2\x14\
-\xad\x1c\xd4\xd6\xd8\x03\xda\x44\xd5\xbd\xbc\xbf\xd8\xd9\xc3\x34\
-\xd4\xe6\xd7\x13\xcd\x3c\xec\xd5\xe7\xef\xe2\xeb\xe8\xed\xf8\xd9\
-\xe3\x19\xcb\xfa\xfc\x1b\x7e\x11\x89\x00\x00\x21\xf9\x04\x09\x04\
-\x00\x0f\x00\x2c\x01\x00\x03\x00\x1e\x00\x1b\x00\x00\x04\x1e\xf0\
-\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\
-\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x6e\x04\x00\x21\xf9\
-\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\
-\x04\xde\xf0\xc9\x49\xab\x31\x35\xeb\x3d\xef\xe5\xe0\x84\x20\x94\
-\x87\x4d\xcb\x12\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\
-\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x73\x3d\x72\xc1\x5d\x28\x91\x60\
-\xb5\x8e\x30\x21\x85\xc1\xa8\x30\x99\xce\x91\x49\x3a\xa1\x52\x29\
-\xd7\x6b\xef\xf9\xe1\x7a\xbd\xd6\x30\xf6\xa9\x7b\x9c\xd1\x1a\x75\
-\x93\xf3\xae\x82\xd4\xa0\x37\x4f\x4c\xff\x6e\x0e\x80\x81\x80\x3c\
-\x02\x85\x86\x85\x0f\x82\x8a\x07\x2b\x04\x8e\x8f\x90\x8b\x82\x8d\
-\x90\x95\x89\x92\x3c\x95\x8f\x1c\x0a\x9d\x20\x00\x05\x05\x44\x9d\
-\x9e\x1c\xa1\xa1\x2b\xa4\xa4\x20\xa7\xa7\x1b\xaa\xab\x0d\xb2\x14\
-\x03\xb5\x0f\xad\xae\x14\xb0\x0a\x12\xb2\xb3\x0e\x0e\x0f\xb5\xb6\
-\xb7\xb8\xba\xab\x13\xbe\x0d\xc0\x0e\xc3\xc4\x12\xad\x15\xa5\xbd\
-\xbe\x0f\xcc\x03\xc2\xc3\x14\xa8\x21\xd5\xd6\xc0\xd8\xce\x44\xd4\
-\xb3\xdf\xcd\x12\xe2\x3c\xca\x13\xd7\x13\xe9\x2b\xeb\x12\xed\xe8\
-\xda\xea\x0d\x14\xf3\xf4\xe3\x19\xcc\xc1\xfb\x21\xc0\x88\x44\x00\
-\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x00\x00\x04\x00\x20\x00\
-\x1c\x00\x00\x04\x1f\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\
-\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\
-\xdf\x78\x3e\x47\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\
-\x00\x00\x20\x00\x20\x00\x00\x04\xd9\xf0\xc9\x49\x2b\x42\x35\xeb\
-\x3d\xef\xe5\xe0\x94\x24\x94\x87\x4d\x86\x11\x52\xe3\xd8\x79\x68\
-\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x73\
-\x3d\x72\xc1\x5d\xe8\x70\x60\xb5\x8e\x30\x21\x65\xb1\xa8\x30\x99\
-\xce\x91\x49\x3a\xa1\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\xbd\xd6\x30\
-\xf6\xa9\x7b\x9c\xd1\x1a\x75\x93\xf3\xae\x2e\xc5\xf4\x33\x0f\xbf\
-\x81\x6b\x14\x80\x81\x80\x3c\x0c\x85\x86\x85\x0f\x82\x8a\x0a\x2b\
-\x87\x8e\x0c\x8b\x82\x8d\x8f\x86\x89\x91\x84\x94\x1c\x0d\x9b\x20\
-\x04\x9e\x44\x9b\x9c\x1c\x9e\x9f\x21\xa1\xa1\x9d\xa4\xa5\x19\xa7\
-\xa8\x0e\xaf\x14\x05\xb2\x0f\xaa\xa4\x15\xad\x0d\x12\xaf\xb0\x03\
-\x03\x0f\xb2\xb3\xb4\xb5\x14\xa7\x14\xbb\x0e\xbd\xbd\xc0\x05\x14\
-\xaa\xb7\xb9\x13\xc7\x0f\xc9\xbe\xcb\xcd\x04\x2b\xbb\xbe\xd4\xbf\
-\xc0\x44\xba\xbb\x12\xdc\xdd\xc1\x34\xd2\xe2\xc9\x13\xd6\xe6\xe1\
-\xe8\xbd\xea\xde\x3c\xb0\x13\xe3\x12\xe5\xdf\xf4\xe9\xf8\x21\xef\
-\x3c\x11\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x00\x00\x01\x00\
-\x1e\x00\x1f\x00\x00\x04\x20\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\
-\xff\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\
-\x74\x6d\xdf\x78\xae\xaf\x11\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\
-\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xda\xf0\xc9\x49\x6b\
-\x4a\x35\xeb\x3d\xef\xe5\xe0\x74\x1c\x94\x87\x4d\x08\x12\x52\xe3\
-\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\
-\x8c\x57\x73\x3d\x72\xc1\x5d\x48\xa1\x60\xb5\x8e\x30\x21\xc5\x60\
-\xa8\x30\x99\xce\x91\x49\x3a\xa1\x52\x29\xd7\x6b\xef\xf9\xe1\x7a\
-\xbd\xd6\x30\xf6\xa9\x7b\x9c\xd1\x1a\x75\x93\xf3\xae\x2e\xc5\x74\
-\x38\x0d\xbf\xd1\x67\x1a\x72\x73\x2b\x0b\x84\x85\x84\x0f\x0d\x89\
-\x8a\x8b\x83\x86\x8e\x8b\x90\x0d\x8d\x8e\x85\x88\x81\x3c\x94\x87\
-\x1b\x0e\x9c\x20\x0c\x9f\x44\x9c\x9d\x1c\x9f\xa0\x21\xa2\xa2\x9e\
-\xa5\xa6\x19\xa8\xa9\x03\xb0\x14\x04\xb3\x0f\xab\xa5\x15\xae\x0e\
-\x12\xb0\xb1\x05\x05\x0f\xb3\xb4\xb5\xb6\x14\xa8\x14\xbc\x03\xbe\
-\xbe\xc1\x04\x14\xab\xb8\x03\xc7\xbc\x0f\xca\xbf\xcc\xce\x0c\x2b\
-\xc8\xd4\xca\x12\xc1\x44\xbb\xd3\xdc\xbe\xde\xdf\x3c\xdb\x12\xd5\
-\x13\xd7\x34\xe8\xe3\xbf\xe5\xc2\xed\xd1\x13\xea\xeb\xcd\xe0\x15\
-\xf6\xf9\x20\xe4\x3c\x11\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\
-\x02\x00\x00\x00\x1b\x00\x20\x00\x00\x04\x1f\xf0\xc9\x49\xab\xbd\
-\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\
-\xbe\x70\x2c\xcf\x74\x6d\xdf\x78\x3e\x45\x00\x21\xf9\x04\x05\x04\
-\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdb\xf0\
-\xc9\x49\xeb\x39\x35\xeb\x3d\xef\xe5\xe0\xa4\x28\x94\x87\x4d\x49\
-\x12\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\
-\xc3\x0f\xd9\x8c\x57\x6b\x3d\x72\xc1\x5d\xa8\xd1\x60\x19\x73\x42\
-\x0a\x02\x51\x61\x32\x9d\x23\x53\x74\x32\x9d\x52\xac\xd6\xde\x13\
-\xb3\xed\x76\xab\xe0\xab\x51\xf7\x30\x9f\x35\xe9\x26\xc7\x4d\x5d\
-\x86\xe7\x6f\xda\x7d\x93\xcf\x0c\x1c\x80\x81\x0e\x3c\x06\x85\x86\
-\x85\x0f\x82\x8a\x83\x21\x87\x8e\x06\x8b\x82\x2b\x8f\x87\x89\x03\
-\x97\x98\x03\x84\x94\x1c\x98\x20\x0b\xa0\x44\x99\x9f\xa0\xa1\x20\
-\x99\x97\xa4\xa5\x0b\x1b\xa8\xa9\x05\xb0\x14\x0c\xb3\x0f\xab\xa5\
-\x15\xae\x12\xb0\xb1\x04\x04\x0f\xb3\xb4\xb5\xb6\x14\xa3\x13\xbb\
-\x05\xbd\xbd\xc0\x0c\x14\xab\xb8\x9a\xc6\xbb\x0f\x02\xc9\xbf\xc0\
-\xcd\xac\x21\xc7\xd3\xd5\xd6\xcc\x44\x0f\xdb\xdc\xbd\x12\xcb\x44\
-\xe2\xe3\xbe\xe5\xd7\x34\xe8\xd4\xe4\xeb\xc1\xed\x05\x14\xef\xea\
-\xeb\xe0\x19\xc9\xf7\xf9\x1c\xf0\x34\x11\x00\x21\xf9\x04\x09\x04\
-\x00\x0f\x00\x2c\x00\x00\x00\x00\x1c\x00\x1e\x00\x00\x04\x1f\xf0\
-\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\
-\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x38\x19\x01\x00\x21\
-\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\
-\x00\x04\xd9\xf0\xc9\x49\xab\x52\x35\xeb\x3d\xef\xe5\xe0\xd4\x34\
-\x94\x87\x4d\xc7\x11\x52\xe3\xd8\x79\x68\xaa\xae\x4f\x4b\x4a\x66\
-\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x6b\x3d\x72\xc1\x5d\xc8\xe1\
-\x60\x19\x73\x42\x4a\x22\x51\x61\x32\x9d\x23\x53\x74\x32\x9d\x52\
-\xac\xd6\xde\x13\xb3\xed\x76\xab\xe0\xab\x51\xf7\x30\x9f\x35\xe9\
-\x26\xc7\x4d\x5d\x86\xe7\x66\xde\x7d\xf3\xd6\x0c\xfe\x80\x7f\x3c\
-\x08\x84\x85\x84\x0f\x81\x89\x03\x2b\x86\x8d\x08\x8a\x81\x8c\x8e\
-\x85\x88\x90\x83\x93\x1c\x05\x9a\x20\x01\x06\x06\x44\x9a\x9b\x1c\
-\x9e\xa4\x21\xa1\xa1\x20\xa4\xa5\x1a\xa7\xa8\x04\xaf\x14\x0b\xb2\
-\x0f\xaa\xab\x13\xad\x05\x12\xaf\xb0\x0c\x0c\x0f\xb2\xb3\xb4\xb5\
-\x14\xa7\x14\xbb\x04\xbd\xbd\xc0\x0b\x14\xaa\x15\xa2\xba\xbb\x0f\
-\xc9\xbe\xcb\xcd\x9f\x21\xc7\xd3\xc9\x12\xc0\x44\xd1\xb0\xdb\xbd\
-\xdd\xde\x3c\xda\x12\xd4\x13\xd6\x34\xe7\xe2\xbe\xe4\xc1\xec\x04\
-\x14\xe9\xea\xcc\xdf\x15\xf5\xf8\x20\xe3\x3c\x11\x00\x21\xf9\x04\
-\x09\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x1c\x00\x20\x00\x00\x04\
-\x1f\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\
-\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x78\x3e\x47\
-\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\
-\x20\x00\x00\x04\xdd\xf0\xc9\x49\x6b\x6b\x35\xeb\x3d\xd5\xc5\x5c\
-\x28\x39\x0e\xe5\x5d\xa6\x22\x52\x24\xd9\x7d\x9d\x22\xaf\x63\xfb\
-\xa2\x92\x3c\xd3\x4f\x5b\x3e\x27\x90\x4e\xc5\xab\x39\x06\x40\x18\
-\x50\x27\x1a\x20\x27\xbe\x24\x6a\x48\x39\x1c\x2a\x4e\x27\xab\x15\
-\xa4\x4e\xac\x56\x4a\x36\x6b\x2c\x4d\x99\x0f\x30\x18\x3b\xd6\xda\
-\x62\x2a\xf5\x5a\xd3\x7e\x6e\xe4\xd7\x26\x99\x23\xe7\xed\xef\x61\
-\x1b\x05\x83\x84\x83\x3c\x09\x88\x89\x88\x0f\x85\x8d\x05\x2b\x8a\
-\x91\x09\x8e\x85\x90\x92\x89\x8c\x94\x87\x97\x1c\x04\x9e\x21\x08\
-\xa1\x45\x9e\x9f\x1c\xa1\xa7\x22\xa4\xa4\xa0\xa7\xa2\x1a\xaa\xab\
-\x0c\xb2\x14\x06\xb5\x0f\xad\xa8\x14\xb0\x04\x12\xb2\xb3\x0b\x0b\
-\x0f\xb5\xb6\xb7\xb8\xba\xab\x13\xbe\x0c\xc0\xc0\xc3\x06\x14\xad\
-\x15\xa5\xbd\xbe\x0f\xcc\xc1\xce\xd0\x08\x2b\xca\xd6\xcc\x12\xc3\
-\x45\xd4\xb3\xde\xc0\xe0\xe1\x3c\xdd\x12\xd7\x13\xd9\x34\xea\xe5\
-\xc1\xe7\xc4\xef\x0c\x14\xec\xed\xcf\xe2\x15\xf8\xfb\x21\xe6\x3c\
-\x22\x00\x00\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x00\x00\x02\x00\
-\x1f\x00\x1d\x00\x00\x04\x1f\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\
-\xff\x60\x28\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\
-\x74\x6d\xdf\x78\x6e\x47\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\
-\x00\x00\x00\x00\x20\x00\x20\x00\x00\x04\xdf\xf0\xc9\x49\xab\x73\
-\x35\xeb\x3d\xc7\xc5\x5c\x28\x0d\x03\xe5\x5d\x54\xd3\x88\x26\x59\
-\x8e\xdf\xa4\xaa\xec\xe8\x76\xb1\x34\xaf\xf5\xe3\xbe\x27\xd0\xae\
-\xd7\xb9\x05\x75\x33\x51\xa1\xd0\x22\xf9\x62\xc3\x89\x42\x51\x59\
-\x2e\x9b\xa4\x4f\x54\x32\x9d\x52\xac\x56\x9b\x13\x15\xed\x76\xab\
-\xe0\xeb\x4d\x46\x33\x9f\x35\x69\x26\xc7\x4d\x55\x86\xe7\xe6\xde\
-\x7d\xf3\xd6\x10\x04\x80\x81\x02\x3d\x07\x85\x86\x85\x0f\x04\x8a\
-\x8b\x8c\x2c\x87\x8f\x07\x8c\x92\x04\x8e\x90\x86\x89\x93\x94\x35\
-\x96\x07\x1c\x0c\x9f\x22\x09\x09\x44\x9f\xa0\x1c\xa2\xa2\x2c\xa5\
-\xa5\x21\xa8\xa8\x1b\xab\xac\x0b\xb3\x15\x08\x08\x0f\xae\xaf\x14\
-\xb1\x0c\x12\xb3\xb4\x06\x06\x0f\xb6\xb6\x12\xb9\xa3\x13\xb1\x13\
-\xbf\x0b\xc1\xc1\xc4\xb7\x13\xae\x15\xa6\xbe\xbf\x0f\xce\xc2\xd0\
-\x14\xa9\x22\xcc\xd8\xce\x12\xc4\x44\xd6\xb4\xe0\xc1\xe2\xe3\x3d\
-\xdf\x12\xd9\x13\xdb\x35\xec\xe7\xc2\xe9\xc5\xeb\x0b\x14\xee\xef\
-\xd1\xe4\xf9\xe1\xfd\x22\xd0\xf5\x88\x00\x00\x21\xf9\x04\x09\x04\
-\x00\x0f\x00\x2c\x00\x00\x00\x00\x1d\x00\x1c\x00\x00\x04\x1e\xf0\
-\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\x8e\x64\x69\x9e\x68\
-\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\x70\x04\x00\x21\xf9\
-\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\x20\x00\x20\x00\x00\
-\x04\xdd\xf0\xc9\x49\xeb\x18\x35\xeb\x3d\xef\xe5\xe0\x54\x14\x94\
-\x87\x4d\x8e\x13\x52\xe3\xd8\x79\x5d\xaa\xae\x4f\x4b\x4a\x26\x2a\
-\xd3\x92\x8d\xc3\x0f\xd9\x8c\x57\x6b\x3d\x72\xc1\xd4\x89\x43\x20\
-\xb0\x8c\x39\x21\xa5\xd1\xa8\x34\x9b\xcf\x91\x69\xb0\x9b\x50\xa9\
-\x94\xeb\xb5\x07\xc5\x48\x1f\xdf\xaf\x55\x8c\x35\xea\x54\x69\xb5\
-\x86\xed\xe4\xc4\xab\x21\x31\x28\xce\x1b\xdb\xc1\x1b\x0c\x82\x83\
-\x82\x3c\x0a\x87\x88\x87\x0f\x84\x8c\x0c\x2b\x89\x90\x0a\x8d\x84\
-\x8f\x91\x88\x8b\x93\x86\x96\x1c\x0b\x9d\x21\x07\x07\x44\x9d\x9e\
-\x1c\xa0\xa0\x2b\xa3\xa3\x20\xa6\xa6\x1b\xa9\xaa\x06\xb1\x15\x09\
-\x09\x0f\xac\xad\x14\xaf\x0b\x12\xb1\xb2\x08\x08\x0f\xb4\xb4\x12\
-\xb7\xa1\x13\xaf\x13\xbd\x06\xbf\xbf\xc2\xb5\x13\xac\x15\xa4\xbc\
-\xbd\x0f\xcc\xc0\xce\x14\xa7\x21\xca\xd6\xcc\x12\xc2\x44\xd4\xb2\
-\xde\xbf\xe0\xe1\x3c\xdd\x12\xd7\x13\xd9\x34\xea\xe5\xc0\xe7\xc3\
-\xe9\x06\x14\xec\xed\xcf\xe2\xf7\xdf\xfb\x21\xe6\x3c\x22\x00\x00\
-\x21\xf9\x04\x09\x04\x00\x0f\x00\x2c\x03\x00\x00\x00\x1d\x00\x1c\
-\x00\x00\x04\x1e\xf0\xc9\x49\xab\xbd\x38\xeb\xcd\xbb\xff\x60\x28\
-\x8e\x64\x69\x9e\x68\xaa\xae\x6c\xeb\xbe\x70\x2c\xcf\x74\x6d\xdf\
-\x70\x04\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\x00\x00\x00\
-\x20\x00\x20\x00\x00\x04\xde\xf0\xc9\x49\x6b\x29\x35\xeb\x3d\xef\
-\xe5\xe0\x44\x10\x94\x87\x4d\xc3\x10\x52\xe3\xd8\x79\x68\xaa\xae\
-\x4f\x4b\x4a\x66\x9c\xd2\x92\x8d\xc3\x0f\xd9\x8c\x57\x1b\x09\x1e\
-\xb9\xa0\x2c\xc4\x60\xb0\x5a\x48\x98\x90\x32\x70\x54\x9a\xcd\xe7\
-\xc8\x34\x9d\x38\xbe\xd6\x09\x16\xdb\x83\x7e\xba\x60\xf0\x75\x9c\
-\x85\xea\x1e\x69\xb5\x86\xed\xe4\xc4\xc3\x1c\x36\x28\x3d\x64\x66\
-\xed\x5f\x1c\x0b\x83\x84\x83\x3c\x0a\x88\x89\x88\x0f\x85\x8d\x0b\
-\x2b\x0d\x91\x92\x93\x8e\x85\x90\x93\x98\x8c\x95\x3c\x98\x92\x1c\
-\x06\xa0\x21\x8b\x3c\xa0\xa1\x1c\x8a\x2b\xa5\xa5\x20\x8a\xa3\x19\
-\xaa\xab\x08\xb2\x15\x07\x07\x0f\xad\xae\x12\xb0\x06\x12\xb2\xb3\
-\x09\x09\x0f\xb5\xb5\x12\xb8\x14\xb0\x13\xbe\x08\xc0\xc0\xc3\xb6\
-\x13\xa8\xc7\xbc\xc9\xbe\x0f\xcb\xc0\xc2\xc3\x14\xb9\x1b\xca\xd6\
-\xcc\x12\xda\x44\xd6\xd5\xdf\xd8\xd9\xc4\x3c\xde\xbd\xe0\xe1\xe2\
-\x2b\xeb\x12\xed\xe8\xcf\x34\xb3\x14\xf3\xd9\xe3\x19\xcc\xc1\xfb\
-\x21\xe7\x68\x44\x00\x00\x21\xf9\x04\x05\x04\x00\x0f\x00\x2c\x00\
-\x00\x00\x00\x01\x00\x01\x00\x00\x04\x02\xf0\x45\x00\x3b\
-\x00\x00\x02\xc0\
-\x89\
-\x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
-\x00\x00\x50\x00\x00\x00\x50\x08\x06\x00\x00\x00\x8e\x11\xf2\xad\
-\x00\x00\x00\xca\x69\x43\x43\x50\x43\x75\x73\x74\x6f\x6d\x00\x00\
-\x18\x95\x63\x60\x60\xdc\xce\x00\x04\x4c\x0e\x0c\x0c\xb9\x79\x25\
-\x45\x41\xee\x4e\x0a\x11\x91\x51\x0a\x0c\x48\x20\x31\xb9\xb8\x80\
-\x01\x37\x60\x64\x60\xf8\x76\x0d\x44\x32\x30\x5c\xd6\x0d\x2c\x61\
-\xe5\xc7\xa3\x16\x1b\xe0\x2c\x02\x5a\x08\xa4\x3f\x00\xb1\x48\x3a\
-\x98\xcd\xc8\x02\x62\x27\x41\xd8\x12\x20\x76\x79\x49\x41\x09\x90\
-\xad\x03\x62\x27\x17\x14\x81\xd8\x40\x17\x33\xf0\x14\x85\x04\x39\
-\x03\xd9\x3e\x40\xb6\x40\x3a\x12\x3b\x09\x89\x9d\x92\x5a\x9c\x0c\
-\x64\xc7\x00\xd9\xd1\x08\xbf\xe5\xcf\x67\x60\xb0\xf8\xc2\xc0\xc0\
-\x3c\x11\x21\x96\x34\x8d\x81\x61\x7b\x3b\x03\x83\xc4\x6d\x84\x98\
-\xca\x42\x06\x06\xfe\x56\x06\x86\x6d\x57\x10\x62\x9f\x03\xc1\xfe\
-\x65\x14\x3b\x53\x92\x5a\x51\x02\x12\xf1\xd3\x77\x64\x28\x48\x2c\
-\x4a\x84\xfb\x8a\xc9\xd8\x08\x62\x2f\x2c\x8c\xa8\x0a\x00\x67\xd9\
-\x31\x35\xdc\xee\x19\x62\x00\x00\x00\x09\x70\x48\x59\x73\x00\x00\
-\x0e\xc4\x00\x00\x0e\xc4\x01\x95\x2b\x0e\x1b\x00\x00\x00\x25\x74\
-\x45\x58\x74\x64\x61\x74\x65\x3a\x63\x72\x65\x61\x74\x65\x00\x32\
-\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x34\x39\x3a\
-\x35\x39\x2b\x30\x30\x3a\x30\x30\x79\x0b\x2c\x48\x00\x00\x00\x25\
-\x74\x45\x58\x74\x64\x61\x74\x65\x3a\x6d\x6f\x64\x69\x66\x79\x00\
-\x32\x30\x32\x32\x2d\x30\x35\x2d\x32\x30\x54\x31\x33\x3a\x34\x39\
-\x3a\x35\x39\x2b\x30\x30\x3a\x30\x30\x08\x56\x94\xf4\x00\x00\x01\
-\x3a\x49\x44\x41\x54\x78\x9c\xed\xda\x31\x4a\x43\x51\x10\x46\xe1\
-\x63\xba\x34\x82\x3b\x89\xa9\x0c\x68\xba\xa8\x4b\xb6\xb2\xb4\x72\
-\x1b\x5a\xa9\x20\x86\x08\x82\x68\x63\x40\xd4\xa7\xef\xe6\x1f\x62\
-\xa2\xe7\x83\x29\x2f\x0c\x87\x29\x2f\x48\x92\x24\xa9\xc0\x04\x38\
-\x07\xf6\x7e\x7b\x91\x6d\x34\x01\xee\x81\x17\xe0\x12\x23\x36\x79\
-\x1f\x6f\x39\x46\xec\xe9\xab\x78\x46\xec\xe9\xbb\x78\x46\xfc\x41\
-\x9f\x78\x46\xec\xd0\x12\xcf\x88\x1f\x0c\x81\x6b\xda\xe2\x2d\xe7\
-\x02\xd8\x5d\xff\xca\x9b\xe7\x10\x78\x60\xb5\x88\x5e\xe2\x1b\x23\
-\x16\x30\x62\x81\x23\x8c\x18\x33\x62\x01\x23\x16\x30\x62\x01\x23\
-\x16\x98\x62\xc4\xd8\x14\x98\x63\xc4\x88\x11\x0b\x18\xb1\xc0\x0c\
-\x58\x60\xc4\x88\x11\x0b\x18\xb1\x80\x11\x0b\x18\xb1\xc0\x31\xf0\
-\x88\x11\x23\x46\x2c\x60\xc4\x02\x46\x2c\x60\xc4\x02\x27\x18\x31\
-\xb6\xd6\x88\x83\xaa\xad\x37\xc8\x4e\xf0\xf6\x09\x78\xae\x5a\x64\
-\x1b\x9d\xb2\xfa\xf5\xfd\xfb\x5f\x0f\xc6\x0b\x18\x2f\x60\xbc\x80\
-\xf1\x02\xc6\x0b\x18\x2f\x60\xbc\x80\xf1\x02\xc6\x0b\x18\x2f\x60\
-\xbc\x80\xf1\x02\xc6\x0b\x18\x2f\x60\xbc\x80\xf1\x02\xc6\x0b\x18\
-\x2f\x60\xbc\x80\xf1\x02\xc6\x0b\x18\x2f\x30\x04\xae\x30\x5e\x64\
-\x04\xdc\x60\xbc\x48\x4b\x44\xe3\x75\x18\x01\xb7\x18\x2f\xb2\x4f\
-\x77\x44\xe3\xf5\x34\xe6\x73\x44\xe3\x35\x1a\x03\x77\x18\x2f\x72\
-\x00\x9c\x61\x3c\x49\x92\x24\xe9\x6f\x7b\x05\xbd\x94\x43\x47\x66\
-\xec\x2a\x6b\x00\x00\x00\x00\x49\x45\x4e\x44\xae\x42\x60\x82\
 "
 
 qt_resource_name = b"\
 \x00\x06\
 \x07\x03\x7d\xc3\
 \x00\x69\
 \x00\x6d\x00\x61\x00\x67\x00\x65\x00\x73\
-\x00\x09\
-\x0c\x98\xba\x47\
-\x00\x70\
-\x00\x61\x00\x75\x00\x73\x00\x65\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x0e\
 \x07\x4c\xee\x87\
 \x00\x6f\
 \x00\x70\x00\x65\x00\x6e\x00\x66\x00\x6f\x00\x6c\x00\x64\x00\x65\x00\x72\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x08\
-\x0c\xf7\x59\xc7\
-\x00\x6e\
-\x00\x65\x00\x78\x00\x74\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x0c\
-\x02\x83\xdd\x07\
-\x00\x6f\
-\x00\x70\x00\x65\x00\x6e\x00\x6c\x00\x69\x00\x6e\x00\x6b\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x05\
-\x00\x7b\x57\x47\
-\x00\x78\
-\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x0a\
-\x0a\x6f\x88\x47\
+\x08\xc9\x59\xa7\
 \x00\x70\
-\x00\x65\x00\x72\x00\x73\x00\x6f\x00\x6e\x00\x2e\x00\x6a\x00\x70\x00\x67\
-\x00\x0c\
-\x08\x1a\x9d\x27\
+\x00\x72\x00\x65\x00\x76\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x0a\
+\x0c\xad\x0f\x07\
 \x00\x64\
-\x00\x6f\x00\x77\x00\x6e\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x08\
-\x07\x9e\x5a\x47\
-\x00\x62\
-\x00\x61\x00\x63\x00\x6b\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x65\x00\x6c\x00\x65\x00\x74\x00\x65\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x08\
-\x08\xc9\x59\xa7\
+\x02\x8c\x59\xa7\
 \x00\x70\
-\x00\x72\x00\x65\x00\x76\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x6c\x00\x61\x00\x79\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x10\
 \x0d\xcc\xb2\x07\
 \x00\x71\
 \x00\x75\x00\x65\x00\x73\x00\x74\x00\x69\x00\x6f\x00\x6e\x00\x6d\x00\x61\x00\x72\x00\x6b\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x09\
+\x0c\x98\xba\x47\
+\x00\x70\
+\x00\x61\x00\x75\x00\x73\x00\x65\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x08\
 \x0b\xd7\x59\x07\
 \x00\x6c\
 \x00\x65\x00\x66\x00\x74\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x08\
-\x05\xe2\x59\x27\
-\x00\x6c\
-\x00\x6f\x00\x67\x00\x6f\x00\x2e\x00\x70\x00\x6e\x00\x67\
-\x00\x0a\
-\x0c\xad\x0f\x07\
-\x00\x64\
-\x00\x65\x00\x6c\x00\x65\x00\x74\x00\x65\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x09\
+\x0d\xf7\xa6\xa7\
+\x00\x72\
+\x00\x69\x00\x67\x00\x68\x00\x74\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x0b\
 \x08\x5d\x84\xe7\
 \x00\x66\
 \x00\x6f\x00\x72\x00\x77\x00\x61\x00\x72\x00\x64\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x08\
-\x02\x8c\x59\xa7\
+\x07\x9e\x5a\x47\
+\x00\x62\
+\x00\x61\x00\x63\x00\x6b\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x0a\
+\x0a\x6f\x88\x47\
 \x00\x70\
-\x00\x6c\x00\x61\x00\x79\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x65\x00\x72\x00\x73\x00\x6f\x00\x6e\x00\x2e\x00\x6a\x00\x70\x00\x67\
+\x00\x0c\
+\x02\x83\xdd\x07\
+\x00\x6f\
+\x00\x70\x00\x65\x00\x6e\x00\x6c\x00\x69\x00\x6e\x00\x6b\x00\x2e\x00\x70\x00\x6e\x00\x67\
 \x00\x0a\
 \x0a\xcb\x27\x16\
 \x00\x6c\
 \x00\x6f\x00\x61\x00\x64\x00\x65\x00\x72\x00\x2e\x00\x67\x00\x69\x00\x66\
-\x00\x09\
-\x0d\xf7\xa6\xa7\
-\x00\x72\
-\x00\x69\x00\x67\x00\x68\x00\x74\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x05\
+\x00\x7b\x57\x47\
+\x00\x78\
+\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x0d\
+\x05\xa7\xf0\x27\
+\x00\x6f\
+\x00\x70\x00\x65\x00\x6e\x00\x6c\x00\x6f\x00\x63\x00\x61\x00\x6c\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x0b\
+\x0d\xd7\xa0\xc7\
+\x00\x73\
+\x00\x68\x00\x75\x00\x66\x00\x66\x00\x6c\x00\x65\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x08\
+\x0c\xf7\x59\xc7\
+\x00\x6e\
+\x00\x65\x00\x78\x00\x74\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x0c\
+\x08\x1a\x9d\x27\
+\x00\x64\
+\x00\x6f\x00\x77\x00\x6e\x00\x6c\x00\x6f\x00\x61\x00\x64\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x08\
+\x00\x4e\x59\x27\
+\x00\x6c\
+\x00\x69\x00\x6e\x00\x6b\x00\x2e\x00\x70\x00\x6e\x00\x67\
+\x00\x08\
+\x05\xe2\x59\x27\
+\x00\x6c\
+\x00\x6f\x00\x67\x00\x6f\x00\x2e\x00\x70\x00\x6e\x00\x67\
 "
 
 qt_resource_struct_v1 = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x11\x00\x00\x00\x02\
-\x00\x00\x00\x80\x00\x00\x00\x00\x00\x01\x00\x00\x0e\x42\
-\x00\x00\x00\x62\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xba\
-\x00\x00\x01\x7c\x00\x00\x00\x00\x00\x01\x00\x01\x0b\xfb\
-\x00\x00\x01\x30\x00\x00\x00\x00\x00\x01\x00\x00\x92\x70\
-\x00\x00\x00\x2a\x00\x00\x00\x00\x00\x01\x00\x00\x04\xa1\
-\x00\x00\x00\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x78\x7d\
-\x00\x00\x00\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x76\xda\
-\x00\x00\x01\x60\x00\x00\x00\x00\x00\x01\x00\x00\xfa\x4c\
-\x00\x00\x00\xde\x00\x00\x00\x00\x00\x01\x00\x00\x88\x47\
-\x00\x00\x00\x90\x00\x00\x00\x00\x00\x01\x00\x00\x10\x7d\
-\x00\x00\x01\x92\x00\x00\x00\x00\x00\x01\x00\x01\x11\x13\
-\x00\x00\x01\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x8f\x82\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x14\x00\x00\x00\x02\
+\x00\x00\x01\xea\x00\x00\x00\x00\x00\x01\x00\x00\xc4\xb4\
+\x00\x00\x01\x6a\x00\x00\x00\x00\x00\x01\x00\x00\xb9\x5a\
+\x00\x00\x01\x32\x00\x00\x00\x00\x00\x01\x00\x00\xa3\x8f\
+\x00\x00\x00\x64\x00\x00\x00\x00\x00\x01\x00\x00\x07\xcf\
+\x00\x00\x01\x7a\x00\x00\x00\x00\x00\x01\x00\x00\xbb\x95\
+\x00\x00\x02\x00\x00\x00\x00\x00\x00\x01\x00\x00\xc8\x42\
 \x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x46\x00\x00\x00\x00\x00\x01\x00\x00\xf8\xaa\
-\x00\x00\x00\x4c\x00\x00\x00\x00\x00\x01\x00\x00\x08\x12\
-\x00\x00\x00\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x03\
-\x00\x00\x01\xac\x00\x00\x00\x00\x00\x01\x00\x01\x23\x56\
+\x00\x00\x01\x02\x00\x00\x00\x00\x00\x01\x00\x00\x2d\x68\
+\x00\x00\x01\xcc\x00\x00\x00\x00\x00\x01\x00\x00\xc3\x11\
+\x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x1b\xb9\
+\x00\x00\x00\x34\x00\x00\x00\x00\x00\x01\x00\x00\x03\x71\
+\x00\x00\x01\x18\x00\x00\x00\x00\x00\x01\x00\x00\x3d\x32\
+\x00\x00\x01\x50\x00\x00\x00\x00\x00\x01\x00\x00\xa7\x17\
+\x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00\x16\x07\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x11\x66\
+\x00\x00\x00\x4a\x00\x00\x00\x00\x00\x01\x00\x00\x06\x2d\
+\x00\x00\x01\xb6\x00\x00\x00\x00\x00\x01\x00\x00\xc0\x69\
+\x00\x00\x00\x7a\x00\x00\x00\x00\x00\x01\x00\x00\x0c\xe7\
+\x00\x00\x01\x9a\x00\x00\x00\x00\x00\x01\x00\x00\xbe\x51\
+\x00\x00\x00\xce\x00\x00\x00\x00\x00\x01\x00\x00\x18\xf5\
 "
 
 qt_resource_struct_v2 = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x11\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x14\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x80\x00\x00\x00\x00\x00\x01\x00\x00\x0e\x42\
+\x00\x00\x01\xea\x00\x00\x00\x00\x00\x01\x00\x00\xc4\xb4\
+\x00\x00\x01\x81\x4c\x94\x6c\x78\
+\x00\x00\x01\x6a\x00\x00\x00\x00\x00\x01\x00\x00\xb9\x5a\
 \x00\x00\x01\x80\xf1\x49\xe1\x72\
-\x00\x00\x00\x62\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xba\
+\x00\x00\x01\x32\x00\x00\x00\x00\x00\x01\x00\x00\xa3\x8f\
 \x00\x00\x01\x80\xe6\xbc\x5a\xd9\
-\x00\x00\x01\x7c\x00\x00\x00\x00\x00\x01\x00\x01\x0b\xfb\
+\x00\x00\x00\x64\x00\x00\x00\x00\x00\x01\x00\x00\x07\xcf\
 \x00\x00\x01\x81\x2b\x1f\xe3\x0d\
-\x00\x00\x01\x30\x00\x00\x00\x00\x00\x01\x00\x00\x92\x70\
+\x00\x00\x01\x7a\x00\x00\x00\x00\x00\x01\x00\x00\xbb\x95\
+\x00\x00\x01\x81\xb8\x89\x38\xcc\
+\x00\x00\x02\x00\x00\x00\x00\x00\x00\x01\x00\x00\xc8\x42\
 \x00\x00\x01\x81\x1a\x78\xa5\x11\
-\x00\x00\x00\x2a\x00\x00\x00\x00\x00\x01\x00\x00\x04\xa1\
+\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x80\xf0\x27\xef\x23\
-\x00\x00\x00\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x78\x7d\
+\x00\x00\x01\x02\x00\x00\x00\x00\x00\x01\x00\x00\x2d\x68\
 \x00\x00\x01\x80\xae\x44\x94\x14\
-\x00\x00\x00\xaa\x00\x00\x00\x00\x00\x01\x00\x00\x76\xda\
+\x00\x00\x01\xcc\x00\x00\x00\x00\x00\x01\x00\x00\xc3\x11\
 \x00\x00\x01\x80\xb2\x5b\x71\x3c\
-\x00\x00\x01\x60\x00\x00\x00\x00\x00\x01\x00\x00\xfa\x4c\
+\x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x1b\xb9\
 \x00\x00\x01\x80\xc2\xdc\x5f\x68\
-\x00\x00\x00\xde\x00\x00\x00\x00\x00\x01\x00\x00\x88\x47\
+\x00\x00\x00\x34\x00\x00\x00\x00\x00\x01\x00\x00\x03\x71\
 \x00\x00\x01\x81\x2b\x1e\x21\xba\
-\x00\x00\x00\x90\x00\x00\x00\x00\x00\x01\x00\x00\x10\x7d\
+\x00\x00\x01\x18\x00\x00\x00\x00\x00\x01\x00\x00\x3d\x32\
 \x00\x00\x01\x80\xc8\x28\xb4\x92\
-\x00\x00\x01\x92\x00\x00\x00\x00\x00\x01\x00\x01\x11\x13\
+\x00\x00\x01\x50\x00\x00\x00\x00\x00\x01\x00\x00\xa7\x17\
 \x00\x00\x01\x80\xba\x72\xc1\x6f\
-\x00\x00\x01\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x8f\x82\
+\x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00\x16\x07\
 \x00\x00\x01\x80\xe1\xbd\x1f\x72\
-\x00\x00\x00\x12\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x11\x66\
 \x00\x00\x01\x81\x2b\x20\x34\x53\
-\x00\x00\x01\x46\x00\x00\x00\x00\x00\x01\x00\x00\xf8\xaa\
+\x00\x00\x00\x4a\x00\x00\x00\x00\x00\x01\x00\x00\x06\x2d\
 \x00\x00\x01\x81\x09\xe1\x35\x77\
-\x00\x00\x00\x4c\x00\x00\x00\x00\x00\x01\x00\x00\x08\x12\
+\x00\x00\x01\xb6\x00\x00\x00\x00\x00\x01\x00\x00\xc0\x69\
 \x00\x00\x01\x81\x2b\x1e\x69\x31\
-\x00\x00\x00\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x03\
+\x00\x00\x00\x7a\x00\x00\x00\x00\x00\x01\x00\x00\x0c\xe7\
 \x00\x00\x01\x80\xaa\xf9\x51\x13\
-\x00\x00\x01\xac\x00\x00\x00\x00\x00\x01\x00\x01\x23\x56\
+\x00\x00\x01\x9a\x00\x00\x00\x00\x00\x01\x00\x00\xbe\x51\
+\x00\x00\x01\x81\x9f\xff\xc6\xbb\
+\x00\x00\x00\xce\x00\x00\x00\x00\x00\x01\x00\x00\x18\xf5\
 \x00\x00\x01\x80\xe1\xbc\x8a\xaa\
 "
 
 qt_version = [int(v) for v in QtCore.qVersion().split('.')]
 if qt_version < [5, 8, 0]:
     rcc_version = 1
     qt_resource_struct = qt_resource_struct_v1
```

### Comparing `music-dragon-0.8/music_dragon/ui/resources.py` & `music-dragon-0.9/music_dragon/ui/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,49 +15,56 @@
 COVER_PLACEHOLDER_PATH = f"{IMAGES_PATH}/questionmark.png"
 PERSON_PLACEHOLDER_PATH = f"{IMAGES_PATH}/person.jpg"
 DOWNLOAD_PATH = f"{IMAGES_PATH}/download.png"
 X_PATH = f"{IMAGES_PATH}/x.png"
 OPEN_LINK_PATH = f"{IMAGES_PATH}/openlink.png"
 PLAY_PATH = f"{IMAGES_PATH}/play.png"
 PAUSE_PATH = f"{IMAGES_PATH}/pause.png"
+LINK_PATH = f"{IMAGES_PATH}/link.png"
 
 COVER_PLACEHOLDER_PIXMAP: Optional[QPixmap] = None
 PERSON_PLACEHOLDER_PIXMAP: Optional[QPixmap] = None
 DOWNLOAD_PIXMAP: Optional[QPixmap] = None
 X_PIXMAP: Optional[QPixmap] = None
 OPEN_LINK_PIXMAP: Optional[QPixmap] = None
+LINK_PIXMAP: Optional[QPixmap] = None
 
 COVER_PLACEHOLDER_ICON: Optional[QIcon] = None
 PERSON_PLACEHOLDER_ICON: Optional[QIcon] = None
 DOWNLOAD_ICON: Optional[QIcon] = None
 X_ICON: Optional[QIcon] = None
 OPEN_LINK_ICON: Optional[QIcon] = None
 PLAY_ICON: Optional[QIcon] = None
 PAUSE_ICON: Optional[QIcon] = None
+LINK_ICON: Optional[QIcon] = None
 
 def initialize():
     global COVER_PLACEHOLDER_PIXMAP
     global PERSON_PLACEHOLDER_PIXMAP
     global DOWNLOAD_PIXMAP
     global OPEN_LINK_PIXMAP
     global X_PIXMAP
+    global LINK_PIXMAP
     global COVER_PLACEHOLDER_ICON
     global PERSON_PLACEHOLDER_ICON
     global DOWNLOAD_ICON
     global OPEN_LINK_ICON
     global X_ICON
     global PLAY_ICON
     global PAUSE_ICON
+    global LINK_ICON
 
     COVER_PLACEHOLDER_PIXMAP = QPixmap(COVER_PLACEHOLDER_PATH)
     PERSON_PLACEHOLDER_PIXMAP = QPixmap(PERSON_PLACEHOLDER_PATH)
     DOWNLOAD_PIXMAP = QPixmap(DOWNLOAD_PATH)
     OPEN_LINK_PIXMAP = QPixmap(OPEN_LINK_PATH)
     X_PIXMAP = QPixmap(X_PATH)
+    LINK_PIXMAP = QPixmap(LINK_PATH)
 
     COVER_PLACEHOLDER_ICON = QIcon(COVER_PLACEHOLDER_PATH)
     PERSON_PLACEHOLDER_ICON = QIcon(COVER_PLACEHOLDER_PATH)
     DOWNLOAD_ICON = QIcon(DOWNLOAD_PATH)
     OPEN_LINK_ICON = QIcon(OPEN_LINK_PATH)
     X_ICON = QIcon(X_PATH)
     PLAY_ICON = QIcon(PLAY_PATH)
-    PAUSE_ICON = QIcon(PAUSE_PATH)
+    PAUSE_ICON = QIcon(PAUSE_PATH)
+    LINK_ICON = QIcon(LINK_PATH)
```

### Comparing `music-dragon-0.8/music_dragon/ui/searchresultswidget.py` & `music-dragon-0.9/music_dragon/ui/searchresultswidget.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/ui/ui_imagepreviewwindow.py` & `music-dragon-0.9/music_dragon/ui/ui_imagepreviewwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file './res/ui/imagepreviewwindow.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.7
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
```

### Comparing `music-dragon-0.8/music_dragon/ui/ui_mainwindow.py` & `music-dragon-0.9/music_dragon/ui/ui_mainwindow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file './res/ui/mainwindow.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.7
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
-        MainWindow.resize(964, 693)
+        MainWindow.resize(1005, 693)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout_16 = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout_16.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_16.setSpacing(6)
         self.verticalLayout_16.setObjectName("verticalLayout_16")
         self.horizontalLayout_5 = QtWidgets.QHBoxLayout()
@@ -141,51 +141,73 @@
         self.verticalLayout_4.addWidget(self.widget_2)
         self.localPages = QtWidgets.QStackedWidget(self.localPage)
         self.localPages.setObjectName("localPages")
         self.localSongsPage = QtWidgets.QWidget()
         self.localSongsPage.setObjectName("localSongsPage")
         self.verticalLayout_13 = QtWidgets.QVBoxLayout(self.localSongsPage)
         self.verticalLayout_13.setObjectName("verticalLayout_13")
+        self.localSongsFilter = QtWidgets.QLineEdit(self.localSongsPage)
+        self.localSongsFilter.setObjectName("localSongsFilter")
+        self.verticalLayout_13.addWidget(self.localSongsFilter)
         self.localSongs = LocalSongsView(self.localSongsPage)
         self.localSongs.setMouseTracking(True)
         self.localSongs.setIconSize(QtCore.QSize(64, 64))
         self.localSongs.setUniformItemSizes(True)
         self.localSongs.setObjectName("localSongs")
         self.verticalLayout_13.addWidget(self.localSongs)
         self.localPages.addWidget(self.localSongsPage)
         self.localArtistsPage = QtWidgets.QWidget()
         self.localArtistsPage.setObjectName("localArtistsPage")
         self.verticalLayout_14 = QtWidgets.QVBoxLayout(self.localArtistsPage)
         self.verticalLayout_14.setObjectName("verticalLayout_14")
+        self.localArtistsFilter = QtWidgets.QLineEdit(self.localArtistsPage)
+        self.localArtistsFilter.setObjectName("localArtistsFilter")
+        self.verticalLayout_14.addWidget(self.localArtistsFilter)
         self.localArtists = LocalArtistsView(self.localArtistsPage)
         self.localArtists.setMouseTracking(True)
         self.localArtists.setIconSize(QtCore.QSize(64, 64))
         self.localArtists.setUniformItemSizes(True)
         self.localArtists.setObjectName("localArtists")
         self.verticalLayout_14.addWidget(self.localArtists)
         self.localPages.addWidget(self.localArtistsPage)
         self.localAlbumsPage = QtWidgets.QWidget()
         self.localAlbumsPage.setObjectName("localAlbumsPage")
         self.verticalLayout_15 = QtWidgets.QVBoxLayout(self.localAlbumsPage)
         self.verticalLayout_15.setObjectName("verticalLayout_15")
+        self.localAlbumsFilter = QtWidgets.QLineEdit(self.localAlbumsPage)
+        self.localAlbumsFilter.setObjectName("localAlbumsFilter")
+        self.verticalLayout_15.addWidget(self.localAlbumsFilter)
         self.localAlbums = LocalAlbumsView(self.localAlbumsPage)
         self.localAlbums.setMouseTracking(True)
         self.localAlbums.setIconSize(QtCore.QSize(64, 64))
         self.localAlbums.setUniformItemSizes(True)
         self.localAlbums.setObjectName("localAlbums")
         self.verticalLayout_15.addWidget(self.localAlbums)
         self.localPages.addWidget(self.localAlbumsPage)
         self.verticalLayout_4.addWidget(self.localPages)
+        self.horizontalLayout_19 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_19.setObjectName("horizontalLayout_19")
         self.localSongCount = QtWidgets.QLabel(self.localPage)
         font = QtGui.QFont()
         font.setPointSize(10)
         self.localSongCount.setFont(font)
         self.localSongCount.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
         self.localSongCount.setObjectName("localSongCount")
-        self.verticalLayout_4.addWidget(self.localSongCount)
+        self.horizontalLayout_19.addWidget(self.localSongCount)
+        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_19.addItem(spacerItem2)
+        self.localSongsRandomPlayButton = QtWidgets.QPushButton(self.localPage)
+        self.localSongsRandomPlayButton.setText("")
+        icon2 = QtGui.QIcon()
+        icon2.addPixmap(QtGui.QPixmap(":/images/shuffle.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.localSongsRandomPlayButton.setIcon(icon2)
+        self.localSongsRandomPlayButton.setIconSize(QtCore.QSize(24, 24))
+        self.localSongsRandomPlayButton.setObjectName("localSongsRandomPlayButton")
+        self.horizontalLayout_19.addWidget(self.localSongsRandomPlayButton)
+        self.verticalLayout_4.addLayout(self.horizontalLayout_19)
         self.pages.addWidget(self.localPage)
         self.downloadsPage = QtWidgets.QWidget()
         self.downloadsPage.setObjectName("downloadsPage")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.downloadsPage)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
         self.horizontalLayout_7 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_7.setObjectName("horizontalLayout_7")
@@ -193,14 +215,18 @@
         self.manualDownloadURL.setText("")
         self.manualDownloadURL.setObjectName("manualDownloadURL")
         self.horizontalLayout_7.addWidget(self.manualDownloadURL)
         self.manualDownloadButton = QtWidgets.QPushButton(self.downloadsPage)
         self.manualDownloadButton.setObjectName("manualDownloadButton")
         self.horizontalLayout_7.addWidget(self.manualDownloadButton)
         self.verticalLayout_11.addLayout(self.horizontalLayout_7)
+        self.autoDownloadQueuedCheck = QtWidgets.QCheckBox(self.downloadsPage)
+        self.autoDownloadQueuedCheck.setChecked(True)
+        self.autoDownloadQueuedCheck.setObjectName("autoDownloadQueuedCheck")
+        self.verticalLayout_11.addWidget(self.autoDownloadQueuedCheck)
         self.downloadsTabs = QtWidgets.QTabWidget(self.downloadsPage)
         self.downloadsTabs.setObjectName("downloadsTabs")
         self.downloadsQueuedTab = QtWidgets.QWidget()
         self.downloadsQueuedTab.setObjectName("downloadsQueuedTab")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.downloadsQueuedTab)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.queuedDownloads = DownloadsWidget(self.downloadsQueuedTab)
@@ -215,18 +241,18 @@
         self.finishedDownloads.setObjectName("finishedDownloads")
         self.verticalLayout_12.addWidget(self.finishedDownloads)
         self.downloadsTabs.addTab(self.downloadsFinishedTab, "")
         self.verticalLayout_11.addWidget(self.downloadsTabs)
         self.pages.addWidget(self.downloadsPage)
         self.albumPage = QtWidgets.QWidget()
         self.albumPage.setObjectName("albumPage")
-        self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.albumPage)
-        self.verticalLayout_10.setObjectName("verticalLayout_10")
-        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
+        self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.albumPage)
+        self.verticalLayout_24.setObjectName("verticalLayout_24")
+        self.horizontalLayout_21 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_21.setObjectName("horizontalLayout_21")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setSpacing(6)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.albumCover = ClickableLabel(self.albumPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
@@ -246,17 +272,17 @@
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.albumCoverPrevButton.sizePolicy().hasHeightForWidth())
         self.albumCoverPrevButton.setSizePolicy(sizePolicy)
         self.albumCoverPrevButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.albumCoverPrevButton.setText("")
-        icon2 = QtGui.QIcon()
-        icon2.addPixmap(QtGui.QPixmap(":/images/left.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.albumCoverPrevButton.setIcon(icon2)
+        icon3 = QtGui.QIcon()
+        icon3.addPixmap(QtGui.QPixmap(":/images/left.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.albumCoverPrevButton.setIcon(icon3)
         self.albumCoverPrevButton.setIconSize(QtCore.QSize(20, 20))
         self.albumCoverPrevButton.setFlat(True)
         self.albumCoverPrevButton.setObjectName("albumCoverPrevButton")
         self.horizontalLayout.addWidget(self.albumCoverPrevButton)
         self.albumCoverNumber = QtWidgets.QLabel(self.albumPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
@@ -270,40 +296,54 @@
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.albumCoverNextButton.sizePolicy().hasHeightForWidth())
         self.albumCoverNextButton.setSizePolicy(sizePolicy)
         self.albumCoverNextButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.albumCoverNextButton.setText("")
-        icon3 = QtGui.QIcon()
-        icon3.addPixmap(QtGui.QPixmap(":/images/right.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.albumCoverNextButton.setIcon(icon3)
+        icon4 = QtGui.QIcon()
+        icon4.addPixmap(QtGui.QPixmap(":/images/right.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.albumCoverNextButton.setIcon(icon4)
         self.albumCoverNextButton.setIconSize(QtCore.QSize(20, 20))
         self.albumCoverNextButton.setFlat(True)
         self.albumCoverNextButton.setObjectName("albumCoverNextButton")
         self.horizontalLayout.addWidget(self.albumCoverNextButton)
         self.verticalLayout_2.addLayout(self.horizontalLayout)
-        self.horizontalLayout_3.addLayout(self.verticalLayout_2)
+        self.horizontalLayout_21.addLayout(self.verticalLayout_2)
         self.verticalLayout_5 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_5.setContentsMargins(16, -1, -1, -1)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
+        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
         self.albumTitle = QtWidgets.QLabel(self.albumPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(3)
         sizePolicy.setHeightForWidth(self.albumTitle.sizePolicy().hasHeightForWidth())
         self.albumTitle.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(18)
         font.setBold(True)
         font.setWeight(75)
         self.albumTitle.setFont(font)
-        self.albumTitle.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft)
+        self.albumTitle.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
         self.albumTitle.setObjectName("albumTitle")
-        self.verticalLayout_5.addWidget(self.albumTitle)
+        self.horizontalLayout_3.addWidget(self.albumTitle)
+        self.albumOpenLocalButton = QtWidgets.QPushButton(self.albumPage)
+        self.albumOpenLocalButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
+        self.albumOpenLocalButton.setText("")
+        icon5 = QtGui.QIcon()
+        icon5.addPixmap(QtGui.QPixmap(":/images/openlocal.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.albumOpenLocalButton.setIcon(icon5)
+        self.albumOpenLocalButton.setIconSize(QtCore.QSize(24, 24))
+        self.albumOpenLocalButton.setFlat(True)
+        self.albumOpenLocalButton.setObjectName("albumOpenLocalButton")
+        self.horizontalLayout_3.addWidget(self.albumOpenLocalButton)
+        spacerItem3 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_3.addItem(spacerItem3)
+        self.verticalLayout_5.addLayout(self.horizontalLayout_3)
         self.albumArtist = ClickableLabel(self.albumPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(2)
         sizePolicy.setHeightForWidth(self.albumArtist.sizePolicy().hasHeightForWidth())
         self.albumArtist.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
@@ -321,122 +361,312 @@
         self.albumSongCount = QtWidgets.QLabel(self.albumPage)
         font = QtGui.QFont()
         font.setPointSize(10)
         self.albumSongCount.setFont(font)
         self.albumSongCount.setObjectName("albumSongCount")
         self.verticalLayout_5.addWidget(self.albumSongCount)
         self.widget = QtWidgets.QWidget(self.albumPage)
-        self.widget.setMinimumSize(QtCore.QSize(0, 40))
-        self.widget.setMaximumSize(QtCore.QSize(16777215, 40))
         self.widget.setObjectName("widget")
+        self.horizontalLayout_15 = QtWidgets.QHBoxLayout(self.widget)
+        self.horizontalLayout_15.setContentsMargins(0, 0, 0, 0)
+        self.horizontalLayout_15.setObjectName("horizontalLayout_15")
+        self.albumLinkContainer = QtWidgets.QWidget(self.widget)
+        self.albumLinkContainer.setObjectName("albumLinkContainer")
+        self.horizontalLayout_16 = QtWidgets.QHBoxLayout(self.albumLinkContainer)
+        self.horizontalLayout_16.setObjectName("horizontalLayout_16")
+        self.albumLink = QtWidgets.QLineEdit(self.albumLinkContainer)
+        self.albumLink.setObjectName("albumLink")
+        self.horizontalLayout_16.addWidget(self.albumLink)
+        self.albumLinkCancelButton = QtWidgets.QPushButton(self.albumLinkContainer)
+        self.albumLinkCancelButton.setObjectName("albumLinkCancelButton")
+        self.horizontalLayout_16.addWidget(self.albumLinkCancelButton)
+        self.albumLinkOkButton = QtWidgets.QPushButton(self.albumLinkContainer)
+        self.albumLinkOkButton.setObjectName("albumLinkOkButton")
+        self.horizontalLayout_16.addWidget(self.albumLinkOkButton)
+        self.horizontalLayout_15.addWidget(self.albumLinkContainer)
+        self.albumLinkButton = QtWidgets.QPushButton(self.widget)
+        self.albumLinkButton.setToolTip("")
+        self.albumLinkButton.setText("")
+        icon6 = QtGui.QIcon()
+        icon6.addPixmap(QtGui.QPixmap(":/images/link.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.albumLinkButton.setIcon(icon6)
+        self.albumLinkButton.setIconSize(QtCore.QSize(24, 24))
+        self.albumLinkButton.setObjectName("albumLinkButton")
+        self.horizontalLayout_15.addWidget(self.albumLinkButton)
         self.verticalLayout_5.addWidget(self.widget)
-        self.horizontalLayout_3.addLayout(self.verticalLayout_5)
-        spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_3.addItem(spacerItem2)
-        self.verticalLayout_10.addLayout(self.horizontalLayout_3)
-        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
+        self.horizontalLayout_21.addLayout(self.verticalLayout_5)
+        self.verticalLayout_24.addLayout(self.horizontalLayout_21)
+        self.horizontalLayout_20 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_20.setObjectName("horizontalLayout_20")
+        self.verticalLayout_10 = QtWidgets.QVBoxLayout()
+        self.verticalLayout_10.setSpacing(0)
+        self.verticalLayout_10.setObjectName("verticalLayout_10")
         self.albumDownloadAllButton = QtWidgets.QPushButton(self.albumPage)
         self.albumDownloadAllButton.setEnabled(False)
         self.albumDownloadAllButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.albumDownloadAllButton.setStyleSheet("padding: 8px")
-        icon4 = QtGui.QIcon()
-        icon4.addPixmap(QtGui.QPixmap(":/images/download.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.albumDownloadAllButton.setIcon(icon4)
+        icon7 = QtGui.QIcon()
+        icon7.addPixmap(QtGui.QPixmap(":/images/download.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.albumDownloadAllButton.setIcon(icon7)
         self.albumDownloadAllButton.setIconSize(QtCore.QSize(26, 26))
         self.albumDownloadAllButton.setFlat(False)
         self.albumDownloadAllButton.setObjectName("albumDownloadAllButton")
-        self.horizontalLayout_2.addWidget(self.albumDownloadAllButton)
-        spacerItem3 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_2.addItem(spacerItem3)
+        self.verticalLayout_10.addWidget(self.albumDownloadAllButton)
+        self.albumDownloadAllVerifiedCheck = QtWidgets.QCheckBox(self.albumPage)
+        self.albumDownloadAllVerifiedCheck.setObjectName("albumDownloadAllVerifiedCheck")
+        self.verticalLayout_10.addWidget(self.albumDownloadAllVerifiedCheck)
+        self.horizontalLayout_20.addLayout(self.verticalLayout_10)
+        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_20.addItem(spacerItem4)
+        self.verticalLayout_26 = QtWidgets.QVBoxLayout()
+        self.verticalLayout_26.setObjectName("verticalLayout_26")
+        self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_2.setObjectName("horizontalLayout_2")
         self.albumDownloadStatus = QtWidgets.QLabel(self.albumPage)
         self.albumDownloadStatus.setText("")
         self.albumDownloadStatus.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
         self.albumDownloadStatus.setObjectName("albumDownloadStatus")
         self.horizontalLayout_2.addWidget(self.albumDownloadStatus)
         self.albumOpenButton = QtWidgets.QPushButton(self.albumPage)
         self.albumOpenButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.albumOpenButton.setText("")
-        icon5 = QtGui.QIcon()
-        icon5.addPixmap(QtGui.QPixmap(":/images/openlink.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.albumOpenButton.setIcon(icon5)
+        icon8 = QtGui.QIcon()
+        icon8.addPixmap(QtGui.QPixmap(":/images/openlink.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.albumOpenButton.setIcon(icon8)
         self.albumOpenButton.setIconSize(QtCore.QSize(24, 24))
         self.albumOpenButton.setFlat(True)
         self.albumOpenButton.setObjectName("albumOpenButton")
         self.horizontalLayout_2.addWidget(self.albumOpenButton)
-        self.verticalLayout_10.addLayout(self.horizontalLayout_2)
+        self.verticalLayout_26.addLayout(self.horizontalLayout_2)
+        self.showYouTubeTitlesCheck = QtWidgets.QCheckBox(self.albumPage)
+        self.showYouTubeTitlesCheck.setObjectName("showYouTubeTitlesCheck")
+        self.verticalLayout_26.addWidget(self.showYouTubeTitlesCheck)
+        self.horizontalLayout_20.addLayout(self.verticalLayout_26)
+        self.verticalLayout_24.addLayout(self.horizontalLayout_20)
         self.albumTracks = AlbumTracksWidget(self.albumPage)
         self.albumTracks.setObjectName("albumTracks")
-        self.verticalLayout_10.addWidget(self.albumTracks)
+        self.verticalLayout_24.addWidget(self.albumTracks)
         self.pages.addWidget(self.albumPage)
         self.artistPage = QtWidgets.QWidget()
         self.artistPage.setObjectName("artistPage")
-        self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.artistPage)
-        self.verticalLayout_9.setObjectName("verticalLayout_9")
+        self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.artistPage)
+        self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_6.setSpacing(0)
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
         self.artistCover = ClickableLabel(self.artistPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.artistCover.sizePolicy().hasHeightForWidth())
         self.artistCover.setSizePolicy(sizePolicy)
         self.artistCover.setMinimumSize(QtCore.QSize(160, 160))
         self.artistCover.setMaximumSize(QtCore.QSize(160, 160))
         self.artistCover.setText("")
         self.artistCover.setPixmap(QtGui.QPixmap(":/images/questionmark.png"))
         self.artistCover.setScaledContents(True)
         self.artistCover.setObjectName("artistCover")
         self.horizontalLayout_6.addWidget(self.artistCover)
-        self.verticalLayout_8 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_8.setContentsMargins(16, -1, -1, -1)
-        self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.artistName = QtWidgets.QLabel(self.artistPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(3)
         sizePolicy.setHeightForWidth(self.artistName.sizePolicy().hasHeightForWidth())
         self.artistName.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(18)
         font.setBold(True)
         font.setWeight(75)
         self.artistName.setFont(font)
         self.artistName.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
         self.artistName.setObjectName("artistName")
-        self.verticalLayout_8.addWidget(self.artistName)
-        self.horizontalLayout_6.addLayout(self.verticalLayout_8)
-        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_6.addItem(spacerItem4)
-        self.verticalLayout_9.addLayout(self.horizontalLayout_6)
+        self.horizontalLayout_6.addWidget(self.artistName)
+        self.artistOpenLocalButton = QtWidgets.QPushButton(self.artistPage)
+        self.artistOpenLocalButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
+        self.artistOpenLocalButton.setText("")
+        self.artistOpenLocalButton.setIcon(icon5)
+        self.artistOpenLocalButton.setIconSize(QtCore.QSize(24, 24))
+        self.artistOpenLocalButton.setFlat(True)
+        self.artistOpenLocalButton.setObjectName("artistOpenLocalButton")
+        self.horizontalLayout_6.addWidget(self.artistOpenLocalButton)
+        spacerItem5 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_6.addItem(spacerItem5)
+        self.verticalLayout_8.addLayout(self.horizontalLayout_6)
         self.artistAlbums = ArtistAlbumsWidget(self.artistPage)
         self.artistAlbums.setObjectName("artistAlbums")
-        self.verticalLayout_9.addWidget(self.artistAlbums)
+        self.verticalLayout_8.addWidget(self.artistAlbums)
         self.pages.addWidget(self.artistPage)
+        self.localAlbumPage = QtWidgets.QWidget()
+        self.localAlbumPage.setObjectName("localAlbumPage")
+        self.verticalLayout_23 = QtWidgets.QVBoxLayout(self.localAlbumPage)
+        self.verticalLayout_23.setObjectName("verticalLayout_23")
+        self.horizontalLayout_17 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_17.setObjectName("horizontalLayout_17")
+        self.verticalLayout_21 = QtWidgets.QVBoxLayout()
+        self.verticalLayout_21.setSpacing(6)
+        self.verticalLayout_21.setObjectName("verticalLayout_21")
+        self.localAlbumCover = ClickableLabel(self.localAlbumPage)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.localAlbumCover.sizePolicy().hasHeightForWidth())
+        self.localAlbumCover.setSizePolicy(sizePolicy)
+        self.localAlbumCover.setMinimumSize(QtCore.QSize(160, 160))
+        self.localAlbumCover.setMaximumSize(QtCore.QSize(160, 160))
+        self.localAlbumCover.setStyleSheet("")
+        self.localAlbumCover.setText("")
+        self.localAlbumCover.setPixmap(QtGui.QPixmap(":/images/questionmark.png"))
+        self.localAlbumCover.setScaledContents(True)
+        self.localAlbumCover.setObjectName("localAlbumCover")
+        self.verticalLayout_21.addWidget(self.localAlbumCover)
+        self.horizontalLayout_17.addLayout(self.verticalLayout_21)
+        self.verticalLayout_22 = QtWidgets.QVBoxLayout()
+        self.verticalLayout_22.setContentsMargins(16, -1, -1, -1)
+        self.verticalLayout_22.setObjectName("verticalLayout_22")
+        self.horizontalLayout_14 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_14.setObjectName("horizontalLayout_14")
+        self.localAlbumTitle = QtWidgets.QLabel(self.localAlbumPage)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(3)
+        sizePolicy.setHeightForWidth(self.localAlbumTitle.sizePolicy().hasHeightForWidth())
+        self.localAlbumTitle.setSizePolicy(sizePolicy)
+        font = QtGui.QFont()
+        font.setPointSize(18)
+        font.setBold(True)
+        font.setWeight(75)
+        self.localAlbumTitle.setFont(font)
+        self.localAlbumTitle.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.localAlbumTitle.setObjectName("localAlbumTitle")
+        self.horizontalLayout_14.addWidget(self.localAlbumTitle)
+        self.localAlbumOpenRemoteButton = QtWidgets.QPushButton(self.localAlbumPage)
+        self.localAlbumOpenRemoteButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
+        self.localAlbumOpenRemoteButton.setText("")
+        self.localAlbumOpenRemoteButton.setIcon(icon8)
+        self.localAlbumOpenRemoteButton.setIconSize(QtCore.QSize(24, 24))
+        self.localAlbumOpenRemoteButton.setFlat(True)
+        self.localAlbumOpenRemoteButton.setObjectName("localAlbumOpenRemoteButton")
+        self.horizontalLayout_14.addWidget(self.localAlbumOpenRemoteButton)
+        spacerItem6 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_14.addItem(spacerItem6)
+        self.localAlbumRandomPlayButton = QtWidgets.QPushButton(self.localAlbumPage)
+        self.localAlbumRandomPlayButton.setText("")
+        self.localAlbumRandomPlayButton.setIcon(icon2)
+        self.localAlbumRandomPlayButton.setIconSize(QtCore.QSize(24, 24))
+        self.localAlbumRandomPlayButton.setFlat(False)
+        self.localAlbumRandomPlayButton.setObjectName("localAlbumRandomPlayButton")
+        self.horizontalLayout_14.addWidget(self.localAlbumRandomPlayButton)
+        self.verticalLayout_22.addLayout(self.horizontalLayout_14)
+        self.localAlbumArtist = ClickableLabel(self.localAlbumPage)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(2)
+        sizePolicy.setHeightForWidth(self.localAlbumArtist.sizePolicy().hasHeightForWidth())
+        self.localAlbumArtist.setSizePolicy(sizePolicy)
+        font = QtGui.QFont()
+        font.setPointSize(12)
+        self.localAlbumArtist.setFont(font)
+        self.localAlbumArtist.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignTop)
+        self.localAlbumArtist.setObjectName("localAlbumArtist")
+        self.verticalLayout_22.addWidget(self.localAlbumArtist)
+        self.localAlbumSongCount = QtWidgets.QLabel(self.localAlbumPage)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        self.localAlbumSongCount.setFont(font)
+        self.localAlbumSongCount.setObjectName("localAlbumSongCount")
+        self.verticalLayout_22.addWidget(self.localAlbumSongCount)
+        spacerItem7 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_22.addItem(spacerItem7)
+        self.horizontalLayout_17.addLayout(self.verticalLayout_22)
+        self.verticalLayout_23.addLayout(self.horizontalLayout_17)
+        self.localAlbumTracks = LocalAlbumTracksWidget(self.localAlbumPage)
+        self.localAlbumTracks.setObjectName("localAlbumTracks")
+        self.verticalLayout_23.addWidget(self.localAlbumTracks)
+        self.pages.addWidget(self.localAlbumPage)
+        self.localArtistPage = QtWidgets.QWidget()
+        self.localArtistPage.setObjectName("localArtistPage")
+        self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.localArtistPage)
+        self.verticalLayout_9.setObjectName("verticalLayout_9")
+        self.horizontalLayout_18 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_18.setObjectName("horizontalLayout_18")
+        self.localArtistCover = ClickableLabel(self.localArtistPage)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.localArtistCover.sizePolicy().hasHeightForWidth())
+        self.localArtistCover.setSizePolicy(sizePolicy)
+        self.localArtistCover.setMinimumSize(QtCore.QSize(160, 160))
+        self.localArtistCover.setMaximumSize(QtCore.QSize(160, 160))
+        self.localArtistCover.setText("")
+        self.localArtistCover.setPixmap(QtGui.QPixmap(":/images/questionmark.png"))
+        self.localArtistCover.setScaledContents(True)
+        self.localArtistCover.setObjectName("localArtistCover")
+        self.horizontalLayout_18.addWidget(self.localArtistCover)
+        self.localArtistName = QtWidgets.QLabel(self.localArtistPage)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(3)
+        sizePolicy.setHeightForWidth(self.localArtistName.sizePolicy().hasHeightForWidth())
+        self.localArtistName.setSizePolicy(sizePolicy)
+        font = QtGui.QFont()
+        font.setPointSize(18)
+        font.setBold(True)
+        font.setWeight(75)
+        self.localArtistName.setFont(font)
+        self.localArtistName.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.localArtistName.setObjectName("localArtistName")
+        self.horizontalLayout_18.addWidget(self.localArtistName)
+        self.localArtistOpenRemoteButton = QtWidgets.QPushButton(self.localArtistPage)
+        self.localArtistOpenRemoteButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
+        self.localArtistOpenRemoteButton.setText("")
+        self.localArtistOpenRemoteButton.setIcon(icon8)
+        self.localArtistOpenRemoteButton.setIconSize(QtCore.QSize(24, 24))
+        self.localArtistOpenRemoteButton.setFlat(True)
+        self.localArtistOpenRemoteButton.setObjectName("localArtistOpenRemoteButton")
+        self.horizontalLayout_18.addWidget(self.localArtistOpenRemoteButton)
+        spacerItem8 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_18.addItem(spacerItem8)
+        self.localArtistRandomPlayButton = QtWidgets.QPushButton(self.localArtistPage)
+        self.localArtistRandomPlayButton.setText("")
+        self.localArtistRandomPlayButton.setIcon(icon2)
+        self.localArtistRandomPlayButton.setIconSize(QtCore.QSize(24, 24))
+        self.localArtistRandomPlayButton.setObjectName("localArtistRandomPlayButton")
+        self.horizontalLayout_18.addWidget(self.localArtistRandomPlayButton)
+        self.verticalLayout_9.addLayout(self.horizontalLayout_18)
+        self.localArtistAlbums = LocalArtistAlbumsWidget(self.localArtistPage)
+        self.localArtistAlbums.setObjectName("localArtistAlbums")
+        self.verticalLayout_9.addWidget(self.localArtistAlbums)
+        self.pages.addWidget(self.localArtistPage)
         self.verticalLayout_7.addWidget(self.pages)
         self.horizontalLayout_5.addLayout(self.verticalLayout_7)
         self.verticalLayout_16.addLayout(self.horizontalLayout_5)
         self.playContainer = QtWidgets.QWidget(self.centralwidget)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.playContainer.sizePolicy().hasHeightForWidth())
         self.playContainer.setSizePolicy(sizePolicy)
         self.playContainer.setMinimumSize(QtCore.QSize(0, 100))
         self.playContainer.setMaximumSize(QtCore.QSize(16777215, 100))
-        self.playContainer.setStyleSheet(".QWidget { background-color:  #252626; border-top: 1px solid #929696;}")
+        self.playContainer.setStyleSheet("QWidget#playContainer { background-color:  #252626; border-top: 1px solid #929696;}")
         self.playContainer.setObjectName("playContainer")
         self.horizontalLayout_13 = QtWidgets.QHBoxLayout(self.playContainer)
-        self.horizontalLayout_13.setContentsMargins(12, 12, 12, 0)
         self.horizontalLayout_13.setObjectName("horizontalLayout_13")
+        self.playSongContainer = QtWidgets.QWidget(self.playContainer)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Ignored, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.playSongContainer.sizePolicy().hasHeightForWidth())
+        self.playSongContainer.setSizePolicy(sizePolicy)
+        self.playSongContainer.setObjectName("playSongContainer")
+        self.verticalLayout_19 = QtWidgets.QVBoxLayout(self.playSongContainer)
+        self.verticalLayout_19.setObjectName("verticalLayout_19")
         self.horizontalLayout_10 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_10.setSpacing(12)
         self.horizontalLayout_10.setObjectName("horizontalLayout_10")
-        self.playCover = ClickableLabel(self.playContainer)
+        self.playCover = ClickableLabel(self.playSongContainer)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.playCover.sizePolicy().hasHeightForWidth())
         self.playCover.setSizePolicy(sizePolicy)
         self.playCover.setMinimumSize(QtCore.QSize(64, 64))
         self.playCover.setMaximumSize(QtCore.QSize(64, 64))
@@ -445,187 +675,220 @@
         self.playCover.setPixmap(QtGui.QPixmap(":/images/questionmark.png"))
         self.playCover.setScaledContents(True)
         self.playCover.setObjectName("playCover")
         self.horizontalLayout_10.addWidget(self.playCover)
         self.verticalLayout_17 = QtWidgets.QVBoxLayout()
         self.verticalLayout_17.setSpacing(0)
         self.verticalLayout_17.setObjectName("verticalLayout_17")
-        self.playTitle = QtWidgets.QLabel(self.playContainer)
+        self.playTitle = QtWidgets.QLabel(self.playSongContainer)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.playTitle.setFont(font)
         self.playTitle.setStyleSheet("color: white")
         self.playTitle.setAlignment(QtCore.Qt.AlignBottom|QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft)
         self.playTitle.setObjectName("playTitle")
         self.verticalLayout_17.addWidget(self.playTitle)
         self.horizontalLayout_9 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_9.setSpacing(0)
         self.horizontalLayout_9.setObjectName("horizontalLayout_9")
-        self.playArtist = ClickableLabel(self.playContainer)
+        self.playArtist = ClickableLabel(self.playSongContainer)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.playArtist.sizePolicy().hasHeightForWidth())
+        self.playArtist.setSizePolicy(sizePolicy)
         self.playArtist.setStyleSheet("color: white")
         self.playArtist.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignTop)
         self.playArtist.setObjectName("playArtist")
         self.horizontalLayout_9.addWidget(self.playArtist)
-        self.label_3 = QtWidgets.QLabel(self.playContainer)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        self.label_3 = QtWidgets.QLabel(self.playSongContainer)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_3.sizePolicy().hasHeightForWidth())
         self.label_3.setSizePolicy(sizePolicy)
         self.label_3.setStyleSheet("color: white")
         self.label_3.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignTop)
         self.label_3.setObjectName("label_3")
         self.horizontalLayout_9.addWidget(self.label_3)
-        self.playAlbum = ClickableLabel(self.playContainer)
+        self.playAlbum = ClickableLabel(self.playSongContainer)
         font = QtGui.QFont()
         font.setUnderline(False)
         self.playAlbum.setFont(font)
         self.playAlbum.setStyleSheet("color: white")
         self.playAlbum.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignTop)
         self.playAlbum.setObjectName("playAlbum")
         self.horizontalLayout_9.addWidget(self.playAlbum)
         self.verticalLayout_17.addLayout(self.horizontalLayout_9)
         self.horizontalLayout_10.addLayout(self.verticalLayout_17)
-        self.horizontalLayout_13.addLayout(self.horizontalLayout_10)
-        spacerItem5 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_13.addItem(spacerItem5)
+        self.verticalLayout_19.addLayout(self.horizontalLayout_10)
+        self.horizontalLayout_13.addWidget(self.playSongContainer)
+        spacerItem9 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_13.addItem(spacerItem9)
+        self.playControlsContainer = QtWidgets.QWidget(self.playContainer)
+        self.playControlsContainer.setMinimumSize(QtCore.QSize(600, 0))
+        self.playControlsContainer.setMaximumSize(QtCore.QSize(600, 16777215))
+        self.playControlsContainer.setObjectName("playControlsContainer")
+        self.verticalLayout_20 = QtWidgets.QVBoxLayout(self.playControlsContainer)
+        self.verticalLayout_20.setObjectName("verticalLayout_20")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout()
         self.verticalLayout_18.setSpacing(0)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.horizontalLayout_12 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_12.setObjectName("horizontalLayout_12")
-        spacerItem6 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_12.addItem(spacerItem6)
-        self.prevSongButton = QtWidgets.QPushButton(self.playContainer)
+        spacerItem10 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_12.addItem(spacerItem10)
+        self.prevSongButton = QtWidgets.QPushButton(self.playControlsContainer)
         self.prevSongButton.setMinimumSize(QtCore.QSize(32, 32))
         self.prevSongButton.setMaximumSize(QtCore.QSize(32, 32))
         self.prevSongButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.prevSongButton.setText("")
-        icon6 = QtGui.QIcon()
-        icon6.addPixmap(QtGui.QPixmap(":/images/prev.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.prevSongButton.setIcon(icon6)
+        icon9 = QtGui.QIcon()
+        icon9.addPixmap(QtGui.QPixmap(":/images/prev.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.prevSongButton.setIcon(icon9)
         self.prevSongButton.setIconSize(QtCore.QSize(32, 32))
         self.prevSongButton.setFlat(True)
         self.prevSongButton.setObjectName("prevSongButton")
         self.horizontalLayout_12.addWidget(self.prevSongButton)
-        self.playPauseButton = QtWidgets.QPushButton(self.playContainer)
+        self.playPauseButton = QtWidgets.QPushButton(self.playControlsContainer)
         self.playPauseButton.setMinimumSize(QtCore.QSize(48, 48))
         self.playPauseButton.setMaximumSize(QtCore.QSize(48, 48))
         self.playPauseButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.playPauseButton.setText("")
-        icon7 = QtGui.QIcon()
-        icon7.addPixmap(QtGui.QPixmap(":/images/play.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.playPauseButton.setIcon(icon7)
+        icon10 = QtGui.QIcon()
+        icon10.addPixmap(QtGui.QPixmap(":/images/play.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.playPauseButton.setIcon(icon10)
         self.playPauseButton.setIconSize(QtCore.QSize(48, 48))
         self.playPauseButton.setFlat(True)
         self.playPauseButton.setObjectName("playPauseButton")
         self.horizontalLayout_12.addWidget(self.playPauseButton)
-        self.nextSongButton = QtWidgets.QPushButton(self.playContainer)
+        self.nextSongButton = QtWidgets.QPushButton(self.playControlsContainer)
         self.nextSongButton.setMinimumSize(QtCore.QSize(32, 32))
         self.nextSongButton.setMaximumSize(QtCore.QSize(32, 32))
         self.nextSongButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.nextSongButton.setText("")
-        icon8 = QtGui.QIcon()
-        icon8.addPixmap(QtGui.QPixmap(":/images/next.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
-        self.nextSongButton.setIcon(icon8)
+        icon11 = QtGui.QIcon()
+        icon11.addPixmap(QtGui.QPixmap(":/images/next.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        self.nextSongButton.setIcon(icon11)
         self.nextSongButton.setIconSize(QtCore.QSize(32, 32))
         self.nextSongButton.setFlat(True)
         self.nextSongButton.setObjectName("nextSongButton")
         self.horizontalLayout_12.addWidget(self.nextSongButton)
-        spacerItem7 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.horizontalLayout_12.addItem(spacerItem7)
+        spacerItem11 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.horizontalLayout_12.addItem(spacerItem11)
         self.verticalLayout_18.addLayout(self.horizontalLayout_12)
         self.horizontalLayout_11 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_11.setSpacing(12)
         self.horizontalLayout_11.setObjectName("horizontalLayout_11")
-        self.playCurrentTime = QtWidgets.QLabel(self.playContainer)
+        self.playCurrentTime = QtWidgets.QLabel(self.playControlsContainer)
         self.playCurrentTime.setStyleSheet("color: white")
         self.playCurrentTime.setObjectName("playCurrentTime")
         self.horizontalLayout_11.addWidget(self.playCurrentTime)
-        self.playBar = ClickSlider(self.playContainer)
+        self.playBar = ClickSlider(self.playControlsContainer)
         self.playBar.setMaximum(100)
         self.playBar.setSliderPosition(0)
         self.playBar.setOrientation(QtCore.Qt.Horizontal)
         self.playBar.setObjectName("playBar")
         self.horizontalLayout_11.addWidget(self.playBar)
-        self.playMaxTime = QtWidgets.QLabel(self.playContainer)
+        self.playMaxTime = QtWidgets.QLabel(self.playControlsContainer)
         self.playMaxTime.setStyleSheet("color: white")
         self.playMaxTime.setObjectName("playMaxTime")
         self.horizontalLayout_11.addWidget(self.playMaxTime)
         self.verticalLayout_18.addLayout(self.horizontalLayout_11)
-        self.horizontalLayout_13.addLayout(self.verticalLayout_18)
+        self.verticalLayout_20.addLayout(self.verticalLayout_18)
+        self.horizontalLayout_13.addWidget(self.playControlsContainer)
         self.verticalLayout_16.addWidget(self.playContainer)
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QtWidgets.QMenuBar(MainWindow)
-        self.menubar.setGeometry(QtCore.QRect(0, 0, 964, 34))
+        self.menubar.setGeometry(QtCore.QRect(0, 0, 1005, 34))
         self.menubar.setObjectName("menubar")
         self.menuFile = QtWidgets.QMenu(self.menubar)
         self.menuFile.setObjectName("menuFile")
         self.menuEdit = QtWidgets.QMenu(self.menubar)
         self.menuEdit.setObjectName("menuEdit")
         self.menuTools = QtWidgets.QMenu(self.menubar)
         self.menuTools.setObjectName("menuTools")
         MainWindow.setMenuBar(self.menubar)
         self.actionPreferences = QtWidgets.QAction(MainWindow)
         self.actionPreferences.setObjectName("actionPreferences")
-        self.actionReload = QtWidgets.QAction(MainWindow)
-        self.actionReload.setObjectName("actionReload")
+        self.actionRefresh = QtWidgets.QAction(MainWindow)
+        self.actionRefresh.setObjectName("actionRefresh")
         self.actionYtMusicSetup = QtWidgets.QAction(MainWindow)
         self.actionYtMusicSetup.setObjectName("actionYtMusicSetup")
+        self.actionReload = QtWidgets.QAction(MainWindow)
+        self.actionReload.setObjectName("actionReload")
+        self.menuFile.addAction(self.actionRefresh)
         self.menuFile.addAction(self.actionReload)
         self.menuEdit.addAction(self.actionPreferences)
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuEdit.menuAction())
         self.menubar.addAction(self.menuTools.menuAction())
 
         self.retranslateUi(MainWindow)
-        self.pages.setCurrentIndex(3)
+        self.pages.setCurrentIndex(2)
         self.localPages.setCurrentIndex(0)
         self.downloadsTabs.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "Music Dragon"))
         self.searchPageButton.setText(_translate("MainWindow", "Search"))
         self.localPageButton.setText(_translate("MainWindow", "Local"))
         self.downloadsPageButton.setText(_translate("MainWindow", "Downloads"))
         self.searchBar.setPlaceholderText(_translate("MainWindow", "Search for artists, album, songs..."))
         self.localSongsButton.setText(_translate("MainWindow", "Songs"))
         self.localArtistsButton.setText(_translate("MainWindow", "Artists"))
         self.localAlbumsButton.setText(_translate("MainWindow", "Albums"))
+        self.localSongsFilter.setPlaceholderText(_translate("MainWindow", "Filter by song..."))
+        self.localArtistsFilter.setPlaceholderText(_translate("MainWindow", "Filter by artist..."))
+        self.localAlbumsFilter.setPlaceholderText(_translate("MainWindow", "Filter by album..."))
         self.localSongCount.setText(_translate("MainWindow", "0 Songs"))
         self.manualDownloadURL.setPlaceholderText(_translate("MainWindow", "YouTube video or playlist URL..."))
         self.manualDownloadButton.setText(_translate("MainWindow", "Download"))
+        self.autoDownloadQueuedCheck.setText(_translate("MainWindow", "Automatically download queued songs"))
         self.downloadsTabs.setTabText(self.downloadsTabs.indexOf(self.downloadsQueuedTab), _translate("MainWindow", "Queue"))
         self.downloadsTabs.setTabText(self.downloadsTabs.indexOf(self.downloadsFinishedTab), _translate("MainWindow", "Completed"))
         self.albumCoverNumber.setText(_translate("MainWindow", "1/2"))
         self.albumTitle.setText(_translate("MainWindow", "Fear of the Dark"))
         self.albumArtist.setText(_translate("MainWindow", "Iron Maiden"))
         self.albumYear.setText(_translate("MainWindow", "1992"))
         self.albumSongCount.setText(_translate("MainWindow", "8 songs - 58 min 37 sec"))
+        self.albumLink.setPlaceholderText(_translate("MainWindow", "YouTube playlist URL"))
+        self.albumLinkCancelButton.setText(_translate("MainWindow", "Cancel"))
+        self.albumLinkOkButton.setText(_translate("MainWindow", "OK"))
         self.albumDownloadAllButton.setText(_translate("MainWindow", "Download missing songs"))
+        self.albumDownloadAllVerifiedCheck.setText(_translate("MainWindow", "Download only verified"))
+        self.showYouTubeTitlesCheck.setText(_translate("MainWindow", "Show YouTube titles"))
         self.artistName.setText(_translate("MainWindow", "Iron Maiden"))
+        self.localAlbumTitle.setText(_translate("MainWindow", "Fear of the Dark"))
+        self.localAlbumArtist.setText(_translate("MainWindow", "Iron Maiden"))
+        self.localAlbumSongCount.setText(_translate("MainWindow", "8 songs - 58 min 37 sec"))
+        self.localArtistName.setText(_translate("MainWindow", "Iron Maiden"))
         self.playTitle.setText(_translate("MainWindow", "Be Quick or Be Dead"))
         self.playArtist.setText(_translate("MainWindow", "Iron Maiden"))
         self.label_3.setText(_translate("MainWindow", " - "))
         self.playAlbum.setText(_translate("MainWindow", "Fear of the Dark"))
         self.playCurrentTime.setText(_translate("MainWindow", "0:00"))
         self.playMaxTime.setText(_translate("MainWindow", "4:17"))
         self.menuFile.setTitle(_translate("MainWindow", "File"))
         self.menuEdit.setTitle(_translate("MainWindow", "Edit"))
         self.menuTools.setTitle(_translate("MainWindow", "Tools"))
         self.actionPreferences.setText(_translate("MainWindow", "Preferences"))
-        self.actionReload.setText(_translate("MainWindow", "Reload"))
-        self.actionReload.setShortcut(_translate("MainWindow", "F5"))
+        self.actionRefresh.setText(_translate("MainWindow", "Refresh"))
+        self.actionRefresh.setShortcut(_translate("MainWindow", "F5"))
         self.actionYtMusicSetup.setText(_translate("MainWindow", "YtMusic Setup"))
+        self.actionReload.setText(_translate("MainWindow", "Reload"))
+        self.actionReload.setShortcut(_translate("MainWindow", "Ctrl+F5"))
 from music_dragon.ui.albumtrackswidget import AlbumTracksWidget
 from music_dragon.ui.artistalbumswidget import ArtistAlbumsWidget
 from music_dragon.ui.clickablelabel import ClickableLabel
 from music_dragon.ui.clickslider import ClickSlider
 from music_dragon.ui.downloadswidget import DownloadsWidget
 from music_dragon.ui.localalbumsview import LocalAlbumsView
+from music_dragon.ui.localalbumtrackswidget import LocalAlbumTracksWidget
+from music_dragon.ui.localartistalbumswidget import LocalArtistAlbumsWidget
 from music_dragon.ui.localartistsview import LocalArtistsView
 from music_dragon.ui.localsongsview import LocalSongsView
 from music_dragon.ui.searchresultswidget import SearchResultsWidget
 from . import res_rc
```

### Comparing `music-dragon-0.8/music_dragon/ui/ui_preferenceswindow.py` & `music-dragon-0.9/music_dragon/ui/ui_preferenceswindow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 
 # Form implementation generated from reading ui file './res/ui/preferenceswindow.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.7
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_PreferencesWindow(object):
     def setupUi(self, PreferencesWindow):
         PreferencesWindow.setObjectName("PreferencesWindow")
-        PreferencesWindow.resize(474, 642)
+        PreferencesWindow.resize(624, 821)
         self.verticalLayout = QtWidgets.QVBoxLayout(PreferencesWindow)
         self.verticalLayout.setObjectName("verticalLayout")
         self.tabWidget = QtWidgets.QTabWidget(PreferencesWindow)
         self.tabWidget.setObjectName("tabWidget")
         self.tab = QtWidgets.QWidget()
         self.tab.setObjectName("tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.tab)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.scrollArea = QtWidgets.QScrollArea(self.tab)
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 438, 533))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 588, 712))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.scrollAreaWidgetContents)
         self.verticalLayout_4.setSpacing(12)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.directoryWidget = QtWidgets.QWidget(self.scrollAreaWidgetContents)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum)
         sizePolicy.setHorizontalStretch(0)
@@ -69,14 +69,55 @@
         self.browseDirectoryButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
         self.browseDirectoryButton.setIconSize(QtCore.QSize(24, 24))
         self.browseDirectoryButton.setFlat(False)
         self.browseDirectoryButton.setObjectName("browseDirectoryButton")
         self.horizontalLayout.addWidget(self.browseDirectoryButton)
         self.verticalLayout_3.addLayout(self.horizontalLayout)
         self.verticalLayout_4.addWidget(self.directoryWidget)
+        self.directoryWidget_2 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.directoryWidget_2.sizePolicy().hasHeightForWidth())
+        self.directoryWidget_2.setSizePolicy(sizePolicy)
+        self.directoryWidget_2.setObjectName("directoryWidget_2")
+        self.verticalLayout_16 = QtWidgets.QVBoxLayout(self.directoryWidget_2)
+        self.verticalLayout_16.setObjectName("verticalLayout_16")
+        self.label_11 = QtWidgets.QLabel(self.directoryWidget_2)
+        font = QtGui.QFont()
+        font.setPointSize(14)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_11.setFont(font)
+        self.label_11.setObjectName("label_11")
+        self.verticalLayout_16.addWidget(self.label_11)
+        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
+        self.manualDownloadDirectory = ClickableLabel(self.directoryWidget_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.manualDownloadDirectory.sizePolicy().hasHeightForWidth())
+        self.manualDownloadDirectory.setSizePolicy(sizePolicy)
+        self.manualDownloadDirectory.setMinimumSize(QtCore.QSize(0, 40))
+        self.manualDownloadDirectory.setObjectName("manualDownloadDirectory")
+        self.horizontalLayout_3.addWidget(self.manualDownloadDirectory)
+        self.browseManualDownloadDirectoryButton = QtWidgets.QPushButton(self.directoryWidget_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.browseManualDownloadDirectoryButton.sizePolicy().hasHeightForWidth())
+        self.browseManualDownloadDirectoryButton.setSizePolicy(sizePolicy)
+        self.browseManualDownloadDirectoryButton.setCursor(QtGui.QCursor(QtCore.Qt.PointingHandCursor))
+        self.browseManualDownloadDirectoryButton.setIconSize(QtCore.QSize(24, 24))
+        self.browseManualDownloadDirectoryButton.setFlat(False)
+        self.browseManualDownloadDirectoryButton.setObjectName("browseManualDownloadDirectoryButton")
+        self.horizontalLayout_3.addWidget(self.browseManualDownloadDirectoryButton)
+        self.verticalLayout_16.addLayout(self.horizontalLayout_3)
+        self.verticalLayout_4.addWidget(self.directoryWidget_2)
         self.widget = QtWidgets.QWidget(self.scrollAreaWidgetContents)
         self.widget.setObjectName("widget")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.widget)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.label_2 = QtWidgets.QLabel(self.widget)
         font = QtGui.QFont()
         font.setPointSize(14)
@@ -104,33 +145,54 @@
         font.setWeight(75)
         self.label_3.setFont(font)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_6.addWidget(self.label_3)
         self.outputFormat = QtWidgets.QLineEdit(self.widget_2)
         self.outputFormat.setObjectName("outputFormat")
         self.verticalLayout_6.addWidget(self.outputFormat)
-        self.label_4 = QtWidgets.QLabel(self.widget_2)
+        self.verticalLayout_4.addWidget(self.widget_2)
+        self.widget_5 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
+        self.widget_5.setObjectName("widget_5")
+        self.verticalLayout_17 = QtWidgets.QVBoxLayout(self.widget_5)
+        self.verticalLayout_17.setObjectName("verticalLayout_17")
+        self.label_12 = QtWidgets.QLabel(self.widget_5)
+        font = QtGui.QFont()
+        font.setPointSize(14)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_12.setFont(font)
+        self.label_12.setObjectName("label_12")
+        self.verticalLayout_17.addWidget(self.label_12)
+        self.manualOutputFormat = QtWidgets.QLineEdit(self.widget_5)
+        self.manualOutputFormat.setObjectName("manualOutputFormat")
+        self.verticalLayout_17.addWidget(self.manualOutputFormat)
+        self.verticalLayout_4.addWidget(self.widget_5)
+        self.widget_6 = QtWidgets.QWidget(self.scrollAreaWidgetContents)
+        self.widget_6.setObjectName("widget_6")
+        self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.widget_6)
+        self.verticalLayout_18.setObjectName("verticalLayout_18")
+        self.label_4 = QtWidgets.QLabel(self.widget_6)
         self.label_4.setWordWrap(True)
         self.label_4.setObjectName("label_4")
-        self.verticalLayout_6.addWidget(self.label_4)
-        self.verticalLayout_4.addWidget(self.widget_2)
+        self.verticalLayout_18.addWidget(self.label_4)
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_4.addItem(spacerItem)
+        self.verticalLayout_18.addItem(spacerItem)
+        self.verticalLayout_4.addWidget(self.widget_6)
         self.scrollArea.setWidget(self.scrollAreaWidgetContents)
         self.verticalLayout_2.addWidget(self.scrollArea)
         self.tabWidget.addTab(self.tab, "")
         self.tab_3 = QtWidgets.QWidget()
         self.tab_3.setObjectName("tab_3")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.tab_3)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
         self.scrollArea_3 = QtWidgets.QScrollArea(self.tab_3)
         self.scrollArea_3.setWidgetResizable(True)
         self.scrollArea_3.setObjectName("scrollArea_3")
         self.scrollAreaWidgetContents_3 = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents_3.setGeometry(QtCore.QRect(0, 0, 438, 533))
+        self.scrollAreaWidgetContents_3.setGeometry(QtCore.QRect(0, 0, 588, 712))
         self.scrollAreaWidgetContents_3.setObjectName("scrollAreaWidgetContents_3")
         self.verticalLayout_12 = QtWidgets.QVBoxLayout(self.scrollAreaWidgetContents_3)
         self.verticalLayout_12.setObjectName("verticalLayout_12")
         self.cacheWidget = QtWidgets.QWidget(self.scrollAreaWidgetContents_3)
         self.cacheWidget.setObjectName("cacheWidget")
         self.verticalLayout_13 = QtWidgets.QVBoxLayout(self.cacheWidget)
         self.verticalLayout_13.setObjectName("verticalLayout_13")
@@ -153,14 +215,17 @@
         self.verticalLayout_13.addWidget(self.cache)
         self.cacheImagesCheck = QtWidgets.QCheckBox(self.cacheWidget)
         self.cacheImagesCheck.setObjectName("cacheImagesCheck")
         self.verticalLayout_13.addWidget(self.cacheImagesCheck)
         self.cacheRequestsBox = QtWidgets.QCheckBox(self.cacheWidget)
         self.cacheRequestsBox.setObjectName("cacheRequestsBox")
         self.verticalLayout_13.addWidget(self.cacheRequestsBox)
+        self.cacheLocalSongs = QtWidgets.QCheckBox(self.cacheWidget)
+        self.cacheLocalSongs.setObjectName("cacheLocalSongs")
+        self.verticalLayout_13.addWidget(self.cacheLocalSongs)
         self.cacheSize = QtWidgets.QLabel(self.cacheWidget)
         self.cacheSize.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
         self.cacheSize.setObjectName("cacheSize")
         self.verticalLayout_13.addWidget(self.cacheSize)
         self.cacheClearButton = QtWidgets.QPushButton(self.cacheWidget)
         icon = QtGui.QIcon()
         icon.addPixmap(QtGui.QPixmap(":/images/delete.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
@@ -178,15 +243,15 @@
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.scrollArea_2 = QtWidgets.QScrollArea(self.tab_2)
         self.scrollArea_2.setWidgetResizable(True)
         self.scrollArea_2.setObjectName("scrollArea_2")
         self.scrollAreaWidgetContents_2 = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents_2.setGeometry(QtCore.QRect(0, 0, 438, 533))
+        self.scrollAreaWidgetContents_2.setGeometry(QtCore.QRect(0, 0, 588, 712))
         self.scrollAreaWidgetContents_2.setObjectName("scrollAreaWidgetContents_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.scrollAreaWidgetContents_2)
         self.verticalLayout_7.setSpacing(12)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.widget_3 = QtWidgets.QWidget(self.scrollAreaWidgetContents_2)
         self.widget_3.setObjectName("widget_3")
         self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.widget_3)
@@ -234,14 +299,48 @@
         self.verticalLayout_10.addWidget(self.label_7)
         self.verticalLayout_7.addWidget(self.widget_4)
         spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_7.addItem(spacerItem2)
         self.scrollArea_2.setWidget(self.scrollAreaWidgetContents_2)
         self.verticalLayout_8.addWidget(self.scrollArea_2)
         self.tabWidget.addTab(self.tab_2, "")
+        self.tab_4 = QtWidgets.QWidget()
+        self.tab_4.setObjectName("tab_4")
+        self.verticalLayout_14 = QtWidgets.QVBoxLayout(self.tab_4)
+        self.verticalLayout_14.setObjectName("verticalLayout_14")
+        self.scrollArea_4 = QtWidgets.QScrollArea(self.tab_4)
+        self.scrollArea_4.setWidgetResizable(True)
+        self.scrollArea_4.setObjectName("scrollArea_4")
+        self.scrollAreaWidgetContents_4 = QtWidgets.QWidget()
+        self.scrollAreaWidgetContents_4.setGeometry(QtCore.QRect(0, 0, 588, 712))
+        self.scrollAreaWidgetContents_4.setObjectName("scrollAreaWidgetContents_4")
+        self.verticalLayout_15 = QtWidgets.QVBoxLayout(self.scrollAreaWidgetContents_4)
+        self.verticalLayout_15.setObjectName("verticalLayout_15")
+        self.label_10 = QtWidgets.QLabel(self.scrollAreaWidgetContents_4)
+        font = QtGui.QFont()
+        font.setPointSize(14)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_10.setFont(font)
+        self.label_10.setObjectName("label_10")
+        self.verticalLayout_15.addWidget(self.label_10)
+        self.youtubeEmail = QtWidgets.QLineEdit(self.scrollAreaWidgetContents_4)
+        self.youtubeEmail.setInputMethodHints(QtCore.Qt.ImhEmailCharactersOnly)
+        self.youtubeEmail.setObjectName("youtubeEmail")
+        self.verticalLayout_15.addWidget(self.youtubeEmail)
+        self.youtubePassword = QtWidgets.QLineEdit(self.scrollAreaWidgetContents_4)
+        self.youtubePassword.setInputMethodHints(QtCore.Qt.ImhHiddenText|QtCore.Qt.ImhNoAutoUppercase|QtCore.Qt.ImhNoPredictiveText|QtCore.Qt.ImhSensitiveData)
+        self.youtubePassword.setEchoMode(QtWidgets.QLineEdit.Password)
+        self.youtubePassword.setObjectName("youtubePassword")
+        self.verticalLayout_15.addWidget(self.youtubePassword)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_15.addItem(spacerItem3)
+        self.scrollArea_4.setWidget(self.scrollAreaWidgetContents_4)
+        self.verticalLayout_14.addWidget(self.scrollArea_4)
+        self.tabWidget.addTab(self.tab_4, "")
         self.verticalLayout.addWidget(self.tabWidget)
         self.buttonBox = QtWidgets.QDialogButtonBox(PreferencesWindow)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.verticalLayout.addWidget(self.buttonBox)
 
@@ -253,29 +352,38 @@
 
     def retranslateUi(self, PreferencesWindow):
         _translate = QtCore.QCoreApplication.translate
         PreferencesWindow.setWindowTitle(_translate("PreferencesWindow", "Preferences"))
         self.label.setText(_translate("PreferencesWindow", "Directory"))
         self.directory.setText(_translate("PreferencesWindow", "~/MusicDragon"))
         self.browseDirectoryButton.setText(_translate("PreferencesWindow", "Browse"))
+        self.label_11.setText(_translate("PreferencesWindow", "Manual download directory"))
+        self.manualDownloadDirectory.setText(_translate("PreferencesWindow", "~/MusicDragon"))
+        self.browseManualDownloadDirectoryButton.setText(_translate("PreferencesWindow", "Browse"))
         self.label_2.setText(_translate("PreferencesWindow", "Cover size"))
         self.coverSize.setItemText(0, _translate("PreferencesWindow", "Small (250)"))
         self.coverSize.setItemText(1, _translate("PreferencesWindow", "Medium (500)"))
         self.coverSize.setItemText(2, _translate("PreferencesWindow", "Large (1200)"))
         self.coverSize.setItemText(3, _translate("PreferencesWindow", "Largest"))
         self.label_3.setText(_translate("PreferencesWindow", "Output format"))
+        self.label_12.setText(_translate("PreferencesWindow", "Manual output format"))
         self.label_4.setText(_translate("PreferencesWindow", "<html><head/><body><p><span style=\" font-size:10pt;\">{artist}: </span><span style=\" font-size:10pt; font-style:italic;\">artist name</span><span style=\" font-size:10pt;\"><br/>{album}: </span><span style=\" font-size:10pt; font-style:italic;\">album title</span><span style=\" font-size:10pt;\"><br/>{song}: </span><span style=\" font-size:10pt; font-style:italic;\">song name</span><span style=\" font-size:10pt;\"><br/>{ext}: </span><span style=\" font-size:10pt; font-style:italic;\">extension</span></p></body></html>"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab), _translate("PreferencesWindow", "General"))
         self.label_9.setText(_translate("PreferencesWindow", "Cache"))
         self.cache.setText(_translate("PreferencesWindow", " ~/MusicDragon"))
         self.cacheImagesCheck.setText(_translate("PreferencesWindow", "Cache images"))
         self.cacheRequestsBox.setText(_translate("PreferencesWindow", "Cache requests"))
+        self.cacheLocalSongs.setText(_translate("PreferencesWindow", "Cache local songs"))
         self.cacheSize.setText(_translate("PreferencesWindow", "Size: 0MB"))
         self.cacheClearButton.setText(_translate("PreferencesWindow", "Clear Cache"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_3), _translate("PreferencesWindow", "Cache"))
         self.label_6.setText(_translate("PreferencesWindow", "Thread number"))
         self.label_5.setText(_translate("PreferencesWindow", "This option requires an application restart to take effect."))
         self.label_8.setText(_translate("PreferencesWindow", "Maximum simultaneous downloads"))
         self.label_7.setText(_translate("PreferencesWindow", "This option requires an application restart to take effect."))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("PreferencesWindow", "Threads"))
+        self.label_10.setText(_translate("PreferencesWindow", "Sign in"))
+        self.youtubeEmail.setPlaceholderText(_translate("PreferencesWindow", "Email"))
+        self.youtubePassword.setPlaceholderText(_translate("PreferencesWindow", "Password"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_4), _translate("PreferencesWindow", "YouTube"))
 from music_dragon.ui.clickablelabel import ClickableLabel
 from . import res_rc
```

### Comparing `music-dragon-0.8/music_dragon/ui/ytmusicsetupwindow.py` & `music-dragon-0.9/music_dragon/ui/ytmusicsetupwindow.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/utils.py` & `music-dragon-0.9/music_dragon/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import hashlib
 import json
 import os
 import sys
 import time
+import zlib
 from pathlib import Path
 from typing import Sequence, Optional, Union
 
 from PyQt5.QtCore import QUrl, QStandardPaths
 from PyQt5.QtGui import QPixmap, QIcon, QDesktopServices, QPalette
 
 application_start_time: Optional[int] = None
@@ -70,16 +71,22 @@
     return [idx for idx, element in enumerate(sequence) if element == m]
 
 def max_indexes(sequence: Sequence):
     m = max(sequence)
     return [idx for idx, element in enumerate(sequence) if element == m]
 
 def sanitize_filename(f: str):
-    if f:
-        return f.replace("/", "-")
+    if not f:
+        return f
+    f = f.replace("/", "-")
+    f = f.replace("? ", " ")
+    f = f.replace("?", " ")
+    f = f.replace(": ", ", ")
+    f = f.replace(":", " ")
+    f = f.replace("\"", "")
     return f
 
 def normalize_metadata(something: str):
     if not something:
         return something
     something = something.replace("’", "'")
     something = something.replace("‐", "-")
@@ -127,14 +134,17 @@
 def rangify(a, x, b):
     return max(a, min(x, b))
 
 def is_win():
     return sys.platform.startswith("win")
 
 
+def crc32(data: bytes):
+    return zlib.crc32(data)
+
 class Mergeable:
     def merge(self, other):
         # debug("===== merging =====\n"
         #       f"{(vars(self))}\n"
         #       "------ with -----\n"
         #       f"{(vars(other))}\n"
         # )
```

### Comparing `music-dragon-0.8/music_dragon/wiki.py` & `music-dragon-0.9/music_dragon/wiki.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/workers.py` & `music-dragon-0.9/music_dragon/workers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List
+from typing import Optional, List, Callable, Union
 
 from PyQt5.QtCore import QObject, QThread, pyqtSlot, pyqtSignal, QMetaObject, Qt
 
 from music_dragon.log import debug
 from music_dragon.utils import current_execution_millis
 
 worker_scheduler: Optional['WorkerScheduler'] = None
@@ -181,14 +181,17 @@
         debug(f"Inserting Worker {worker.worker_id} into the scheduler queue with priority {worker.priority}")
 
         # Push in the queue or dispatch if possible
         worker.status = Worker.STATUS_WAITING
         self.workers[worker.worker_id] = worker
         self._dispatch_job_while_possible()
 
+    def dispatch(self): # usually not needed since called by schedule
+        self._dispatch_job_while_possible()
+
     def _on_worker_started(self, worker_id):
         pass
 
     def _on_worker_canceled(self, worker_id):
         self._on_worker_finished(worker_id)
 
     def _on_worker_finished(self, worker_id):
@@ -319,9 +322,25 @@
         for wid in canceled_worker_ids:
             try:
                 w = self.workers.pop(wid)
                 debug(f"Removed {w} from {self}")
             except KeyError:
                 print(f"WARN: no worker with id {wid} among workers of {self}")
 
+    def __str__(self):
+        return self.__class__.__name__
+
 def schedule(worker: Worker):
+    worker_scheduler.schedule(worker)
+
+def schedule_function(func: Callable, *args, **kwargs):
+    class FunctionWorker(Worker):
+        def __init__(self, *args_, **kwargs_):
+            super().__init__()
+            self.args = args_
+            self.kwargs = kwargs_
+
+        def run(self):
+            func(self.args, self.kwargs)
+
+    worker = FunctionWorker(args, kwargs)
     worker_scheduler.schedule(worker)
```

### Comparing `music-dragon-0.8/music_dragon/ytcommons.py` & `music-dragon-0.9/music_dragon/ytcommons.py`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/music_dragon/ytdownloader.py` & `music-dragon-0.9/music_dragon/ytdownloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,123 @@
 import json
 import os.path
 import sys
 from pathlib import Path
 
 import eyed3
-import youtube_dl
+import yt_dlp
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
 from eyed3.core import AudioFile
 from eyed3.id3 import Tag
-from youtube_dl import YoutubeDL
+from yt_dlp import YoutubeDL
 
 import music_dragon.log
 from music_dragon import preferences, workers, ytcommons
 from music_dragon.log import debug
 from music_dragon.utils import j, sanitize_filename
 from music_dragon.workers import Worker
 
 MP3_IMAGE_TAG_INDEX_FRONT_COVER = 3
-YOUTUBE_DL_MAX_DOWNLOAD_ATTEMPTS = 10
+YOUTUBE_DL_MAX_DOWNLOAD_ATTEMPTS = 2
 
 YDL_DEFAULT_OPTS = {
     'format': 'bestaudio/best',
+    'postprocessors': [
+        {
+            'key': 'FFmpegExtractAudio',
+            'preferredcodec': 'mp3',
+            'preferredquality': '320',
+        }
+    ],
+    'verbose': music_dragon.log.debug_enabled,
+}
+YDL_DEFAULT_PLAYLIST_OPTS = {
+    'format': 'bestaudio/best',
     'postprocessors': [{
         'key': 'FFmpegExtractAudio',
         'preferredcodec': 'mp3',
         'preferredquality': '320',
     }],
     'verbose': music_dragon.log.debug_enabled,
+    'ignoreerrors': True
+
 }
 
 downloads = {}
 finished_downloads = {}
 
+email = None
+password = None
+
+auto_download = True
+
+def set_credentials(ytemail: str, ytpassword: str):
+    if ytemail and ytpassword:
+        sign_in(ytemail, ytpassword)
+    else:
+        sign_out()
+
+def sign_in(ytemail: str, ytpassword: str):
+    global email, password
+    debug(f"YT Sign in: username={ytemail}, password={'*' * len(ytpassword)}")
+    email = ytemail
+    password = ytpassword
+
+def sign_out():
+    global email, password
+    debug(f"YT Sign out")
+    email = None
+    password = None
+
+def is_signed_in():
+    return True if (email and password) else False
+
 def download_count():
     return len(downloads)
 
 def get_download(video_id: str):
     return downloads.get(video_id)
 
 def finished_download_count():
     return len(finished_downloads)
 
 def get_finished_download(video_id: str):
     return finished_downloads.get(video_id)
 
+def set_auto_download(yes: bool):
+    global auto_download
+    auto_download = yes
+    if auto_download:
+        workers.worker_scheduler.dispatch()
+
 def ytdl_download(ytdl, url_list):
     """Download a given list of URLs."""
-    outtmpl = ytdl.params.get('outtmpl', youtube_dl.DEFAULT_OUTTMPL)
+    outtmpl = ytdl.outtmpl_dict['default']
     if (len(url_list) > 1
             and outtmpl != '-'
             and '%' not in outtmpl
             and ytdl.params.get('max_downloads') != 1):
-        raise youtube_dl.SameFileError(outtmpl)
+        raise yt_dlp.SameFileError(outtmpl)
 
     res = None
 
     for url in url_list:
         try:
-            # It also downloads the videos
             res = ytdl.extract_info(
                 url, force_generic_extractor=ytdl.params.get('force_generic_extractor', False))
-        except youtube_dl.utils.UnavailableVideoError:
-            ytdl.report_error('unable to download video')
-        except youtube_dl.MaxDownloadsReached:
-            ytdl.to_screen('[info] Maximum number of downloaded files reached.')
-            raise
+        except yt_dlp.utils.UnavailableVideoError as e:
+            ytdl.report_error(e)
+        except yt_dlp.DownloadCancelled as e:
+            ytdl.to_screen(f'[info] {e}')
+            if not ytdl.params.get('break_per_url'):
+                raise
         else:
             if ytdl.params.get('dump_single_json', False):
-                ytdl.to_stdout(json.dumps(res))
+                ytdl.post_extract(res)
+                ytdl.to_stdout(json.dumps(ytdl.sanitize_info(res)))
 
     res["_filename"] = ytdl.prepare_filename(res) # as performed internally
     return res
 
 class CancelException(Exception):
     def __init__(self):
         super(CancelException, self).__init__("canceled by user")
@@ -86,23 +132,24 @@
     output_destination_known = pyqtSignal(str, str)
     download_finished = pyqtSignal(str)
     conversion_finished = pyqtSignal(str)
     tagging_finished = pyqtSignal(str)
 
     def __init__(self,
                  video_id: str,
-                 artist: str, album: str, song: str, track_num: int, image: bytes,
+                 artist: str, album: str, song: str, track_num: int, year: int, image: bytes,
                  output_directory: str, output_format: str,
                  metadata=True):
         super().__init__()
         self.video_id = video_id
         self.artist = artist
         self.album = album
         self.song = song
         self.track_num = track_num
+        self.year = year
         self.image = image
         self.metadata = metadata
         self.output_directory = output_directory
         self.output_format = output_format
 
 
     @pyqtSlot()
@@ -156,64 +203,77 @@
         outtmpl = os.path.join(self.output_directory, outtmpl)
 
         debug(f"Destination template: '{outtmpl}'")
         # debug(f"Destination [real]: '{output}'")
 
         ydl_opts = {
             'format': 'bestaudio/best',
-            'postprocessors': [{
-                'key': 'FFmpegExtractAudio',
-                'preferredcodec': 'mp3',
-                'preferredquality': '320',
-            }],
+            'postprocessors': [
+                {
+                    'key': 'FFmpegExtractAudio',
+                    'preferredcodec': 'mp3',
+                    'preferredquality': '320',
+                }
+            ],
             'logger': YoutubeDLLogger(),
             'progress_hooks': [progress_hook],
             'outtmpl': outtmpl,
             'cachedir': False,
             'verbose': music_dragon.log.debug_enabled,
         }
 
+        if is_signed_in():
+            debug("Adding youtube credentials")
+            ydl_opts["username"] = email
+            ydl_opts["password"] = password
+
         # TODO: download speed up?
 
         last_error = None
         for attempt in range(YOUTUBE_DL_MAX_DOWNLOAD_ATTEMPTS):
             debug(f"Download attempt n. {attempt} for {self.video_id}")
             try:
                 with YoutubeDL(ydl_opts) as ydl:
                     yt_url = ytcommons.youtube_video_id_to_youtube_music_url(self.video_id)
                     debug(f"Going to download from '{yt_url}'")
 
                     debug(f"YOUTUBE_DL: download: '{self.video_id}'")
                     result = ytdl_download(ydl, [yt_url])
-                    debug(
-                        "=== ytdl_download ==="
-                        f"{j(result)}"
-                        "======================"
-                    )
+                    # Fix for "Object of type FFmpegFixupM4aPP is not JSON serializable"
+                    try:
+                        debug(
+                            "=== ytdl_download ==="
+                            f"{j(result)}"
+                            "======================"
+                        )
+                    except Exception as e:
+                        debug(f"WARN: ytdl_download dump failed: {e}")
 
                     output = str(Path(result['_filename']).with_suffix(".mp3").absolute())
                     debug(f"Download destination: {output}")
                     self.output_destination_known.emit(self.video_id, output)
 
                     debug("Conversion completed")
 
                     self.conversion_finished.emit(self.video_id)
 
                     if self.metadata is True:
                         artist = self.artist
                         album = self.album
                         song = self.song
                         track_num = self.track_num
+                        year = self.year
                         image = self.image
 
                         debug(f"Applying mp3 tags to {output}\n"
                               f"artist={artist}\n"
                               f"album={album}\n"
                               f"song={song}\n"
                               f"track_num={track_num}\n"
+                              f"year={year}\n"
                               f"image={'yes' if image else 'no'}"
                           )
 
                         try:
                             f: AudioFile = eyed3.load(output)
                             if f:
                                 if not f.tag:
@@ -224,44 +284,45 @@
                                     tag.artist = artist
                                 if album is not None:
                                     tag.album = album
                                 if song is not None:
                                     tag.title = song
                                 if track_num is not None:
                                     tag.track_num = track_num
+                                if year is not None:
+                                    tag.recording_date = eyed3.core.Date(int(year))
                                 if image:
                                     tag.images.set(MP3_IMAGE_TAG_INDEX_FRONT_COVER, image, "image/jpeg")
                                 tag.save()
                                 debug("Tagging completed")
                                 self.tagging_finished.emit(self.video_id)
                             else:
                                 print(f"WARN: failed to apply mp3 tags to {output}: cannot load mp3")
                         except Exception as e:
                             print(f"WARN: failed to apply mp3 tags to {output}: {e}")
                 return # download done
-
             except CancelException as ce:
                 print(f"WARN: cancel request received during attempt n. {attempt} for video {self.video_id}")
                 return
-
             except Exception as e:
-                print(f"WARN: download attempt n. {attempt} failed for video {self.video_id}: {e}")
+                print(f"WARN: download attempt n. {attempt} failed for video {self.video_id}: {type(e).__name__} {e}")
                 last_error = e
 
         print(f"ERROR: all download attempts ({YOUTUBE_DL_MAX_DOWNLOAD_ATTEMPTS} "
-              f"failed for video {self.video_id}: {last_error}", file=sys.stderr)
+              f"fails for video {self.video_id}: {last_error}", file=sys.stderr)
         self.error.emit(self.video_id, f"ERROR: {last_error}")
 
     def can_execute(self):
         # Can execute only if there are less running (or dispatched) workers than max_simultaneous_downloads
         # This would be enough if the workers_scheduler would schedule the jobs
         # as a queue, but since the jobs are scheduled as a stack (on purpose)#
         # we have to return True only if this worker is actually the earlier one
 
-        earlier_worker = None
+        if not auto_download:
+            return
         downloading_count = 0
         for w in workers.worker_scheduler.workers.values():
             if isinstance(w, TrackDownloaderWorker):
                 # if w.status == Worker.STATUS_WAITING and (earlier_worker is None or w.born < earlier_worker.born):
                 #     earlier_worker = w
 
                 if w.status == Worker.STATUS_DISPATCHED or w.status == Worker.STATUS_RUNNING:
@@ -277,15 +338,15 @@
 
     def __lt__(self, other):
         # FIFO: earlier is better
         return self.born < other.born
 
 def enqueue_track_download(
         video_id: str,
-        artist: str, album: str, song: str, track_num: int, image: bytes,
+        artist: str, album: str, song: str, track_num: int, year: int, image: bytes,
         output_directory: str, output_format: str,
         queued_callback,
         started_callback,
         progress_callback,
         finished_callback,
         canceled_callback,
         error_callback,
@@ -297,25 +358,26 @@
         "status": "queued",
         "progress": 0,
         "attempt": 0,
         "artist": artist,
         "album": album,
         "song": song,
         "track_num": track_num,
+        "year": year,
         "image": image,
         "user_data": user_data,
     }
 
     if video_id in downloads:
         print(f"WARN: already download video with id {video_id}")
         error_callback(down, "Already downloading video")
         return False
 
     worker = TrackDownloaderWorker(
-        video_id, artist, album, song, track_num, image,
+        video_id, artist, album, song, track_num, year, image,
         output_directory, output_format,
         metadata)
     worker.priority = Worker.PRIORITY_BELOW_NORMAL
     down["worker"] = worker
 
     def internal_started_callback():
         d = downloads.get(video_id)
@@ -468,15 +530,15 @@
     def run(self) -> None:
 
         # TODO: download speed up?
         last_error = None
         for attempt in range(YOUTUBE_DL_MAX_DOWNLOAD_ATTEMPTS):
             debug(f"Retrieval attempt n. {attempt} for playlist {self.playlist_id}")
             try:
-                with YoutubeDL(YDL_DEFAULT_OPTS) as ydl:
+                with YoutubeDL(YDL_DEFAULT_PLAYLIST_OPTS) as ydl:
                     yt_url = ytcommons.youtube_playlist_id_to_youtube_url(self.playlist_id)
                     debug(f"YOUTUBE_DL: extract_info: '{self.playlist_id}'")
                     info = ydl.extract_info(yt_url, download=False)
                     debug(
                         "=== extract_info (playlist) ==="
                         f"{j(info)}"
                         "======================"
```

### Comparing `music-dragon-0.8/music_dragon.egg-info/PKG-INFO` & `music-dragon-0.9/music_dragon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-dragon
-Version: 0.8
+Version: 0.9
 Summary: All-in-one music manager: scrapes albums, artists and songs from musicbrainz and automatically download them from youtube.
 Home-page: https://github.com/Docheinstein/music-dragon
 Author: Stefano Dottore
 Author-email: docheinstein@gmail.com
 License: MIT
 Keywords: music manager youtube spotify musicbrainz musicbrainzngs tag cover eyed3 ytmusicapi youtube_dl
 Requires-Python: >=3
```

### Comparing `music-dragon-0.8/music_dragon.egg-info/SOURCES.txt` & `music-dragon-0.9/music_dragon.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,34 @@
 music_dragon/ui/__init__.py
 music_dragon/ui/albumtrackswidget.py
 music_dragon/ui/artistalbumswidget.py
 music_dragon/ui/clickablelabel.py
 music_dragon/ui/clickablewidget.py
 music_dragon/ui/clickslider.py
 music_dragon/ui/downloadswidget.py
+music_dragon/ui/editlinkwindow.py
 music_dragon/ui/imagepreviewwindow.py
+music_dragon/ui/listproxyview.py
 music_dragon/ui/listwidgetmodelview.py
 music_dragon/ui/localalbumsview.py
+music_dragon/ui/localalbumtrackswidget.py
+music_dragon/ui/localartistalbumswidget.py
 music_dragon/ui/localartistsview.py
 music_dragon/ui/localsongsview.py
 music_dragon/ui/mainwindow.py
 music_dragon/ui/preferenceswindow.py
 music_dragon/ui/res_rc.py
 music_dragon/ui/resources.py
 music_dragon/ui/searchresultswidget.py
+music_dragon/ui/ui_editlinkwindow.py
 music_dragon/ui/ui_imagepreviewwindow.py
 music_dragon/ui/ui_mainwindow.py
 music_dragon/ui/ui_preferenceswindow.py
+music_dragon/ui/ui_youtubesigninwindow.py
+music_dragon/ui/youtubesigninwindow.py
 music_dragon/ui/ytmusicsetupwindow.py
 res/images/back.png
 res/images/delete.png
 res/images/download.png
 res/images/forward.png
 res/images/left.png
 res/images/loader.gif
```

### Comparing `music-dragon-0.8/res/images/back.png` & `music-dragon-0.9/res/images/back.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/forward.png` & `music-dragon-0.9/res/images/forward.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/left.png` & `music-dragon-0.9/res/images/left.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/loader.gif` & `music-dragon-0.9/res/images/loader.gif`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/logo.png` & `music-dragon-0.9/res/images/logo.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/openfolder.png` & `music-dragon-0.9/res/images/openfolder.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/openlink.png` & `music-dragon-0.9/res/images/openlink.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/person.jpg` & `music-dragon-0.9/res/images/person.jpg`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/questionmark.png` & `music-dragon-0.9/res/images/questionmark.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/right.png` & `music-dragon-0.9/res/images/right.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/res/images/x.png` & `music-dragon-0.9/res/images/x.png`

 * *Files identical despite different names*

### Comparing `music-dragon-0.8/setup.py` & `music-dragon-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             'music-dragon = music_dragon.main:main',
         ]
     },
 
     # Dependencies
     install_requires=[
         "musicbrainzngs",
-        "youtube_dl",
+        "yt_dlp",
         "ytmusicapi",
         "python-vlc",
         "eyed3",
         "PyQt5",
         "wikidata",
         "requests",
         "levenshtein",
```

