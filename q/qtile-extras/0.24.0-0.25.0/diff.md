# Comparing `tmp/qtile-extras-0.24.0.tar.gz` & `tmp/qtile-extras-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtile-extras-0.24.0.tar", last modified: Sat Jan 20 20:27:19 2024, max compression
+gzip compressed data, was "qtile-extras-0.25.0.tar", last modified: Sat Apr  6 16:50:59 2024, max compression
```

## Comparing `qtile-extras-0.24.0.tar` & `qtile-extras-0.25.0.tar`

### file list

```diff
@@ -1,241 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.829917 qtile-extras-0.24.0/.github/
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.github/check_for_changes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.829917 qtile-extras-0.24.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.829917 qtile-extras-0.24.0/qtile_extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.833917 qtile-extras-0.24.0/qtile_extras/popup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/popup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/popup/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.833917 qtile-extras-0.24.0/qtile_extras/popup/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/popup/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/popup/templates/mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/popup/templates/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    51843 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/popup/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.833917 qtile-extras-0.24.0/qtile_extras/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.833917 qtile-extras-0.24.0/qtile_extras/resources/dbusmenu/
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/dbusmenu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/dbusmenu/dbusmenu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.833917 qtile-extras-0.24.0/qtile_extras/resources/footballscores/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/fixtures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24538 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/footballmatch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/league.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3551 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/matchdict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2382 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/matchevent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/morphlinks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/playeraction.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1317 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/footballscores/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.833917 qtile-extras-0.24.0/qtile_extras/resources/github-icons/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/github-icons/github.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/global_menu/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/global_menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/global_menu/registrar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/media-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/media-icons/default.png
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/media-icons/default.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/media-icons/next.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/media-icons/play_pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/media-icons/previous.svg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/media-icons/stop.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/snapcast-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/snapcast-icons/snapcast.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/stravadata/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/stravadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/stravadata/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/stravadata/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/syncthing/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/syncthing/syncthing.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/tvheadend-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/tvheadend-icons/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.837917 qtile-extras-0.24.0/qtile_extras/resources/visualiser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/visualiser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5038 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/visualiser/cava_draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.841917 qtile-extras-0.24.0/qtile_extras/resources/wallpapers/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wallpapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wallpapers/qte_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)   326251 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wallpapers/qte_triangles.png
--rw-r--r--   0 runner    (1001) docker     (127)   330247 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.841917 qtile-extras-0.24.0/qtile_extras/resources/wordclock/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/dutch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/english.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/finnish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/french.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/portuguese.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/spanish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/resources/wordclock/swedish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/qtile_extras/widget/
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/alsavolumecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/analogueclock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/brightnesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/continuous_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/currentlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/decorations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/githubnotifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/globalmenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    33152 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/groupbox2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/iwd.py
--rw-r--r--   0 runner    (1001) docker     (127)    22797 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/livefootballscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/qtile_extras/widget/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)    24996 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/mpris2widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/pulse_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/pulse_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/scriptexit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/snapcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/statusnotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/strava.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/syncthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/systray.py
--rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/tvheadend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/unitstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/upower.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/visualiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/qtile_extras/widget/wordclock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/qtile_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-20 20:27:19.000000 qtile-extras-0.24.0/qtile_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-01-20 20:27:19.000000 qtile-extras-0.24.0/qtile_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 20:27:19.000000 qtile-extras-0.24.0/qtile_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-20 20:27:19.000000 qtile-extras-0.24.0/qtile_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-20 20:27:19.869917 qtile-extras-0.24.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/test/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/test/backend/wayland/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/backend/wayland/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/backend/wayland/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/test/backend/x11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/backend/x11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/backend/x11/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/test/popup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/popup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/popup/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/popup/test_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.825917 qtile-extras-0.24.0/test/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.849917 qtile-extras-0.24.0/test/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/icons/audio-volume-high.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/icons/audio-volume-low.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/icons/audio-volume-medium.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/icons/audio-volume-muted.svg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/icons/menuitem.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.857917 qtile-extras-0.24.0/test/resources/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-default-grouped-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-default-grouped-padding_x.png
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-default-grouped-padding_y.png
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-default-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-default-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-E-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-E.png
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-N-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-N.png
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-S-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-S.png
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-W-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-single-W.png
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-stacked-grouped.png
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-stacked-same-position.png
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/border-stacked.png
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/combo-rect-plus-powerline.png
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_left-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_left.png
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_right-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_right.png
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-back_slash-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-back_slash.png
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-custom-path.png
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-forward_slash-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-forward_slash.png
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_left-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_left.png
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_right-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_right.png
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-zig_zag-padding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/powerline-zig_zag.png
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-default-filled.png
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-default-group-filled-no-radius.png
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-default-group-filled-widget-background.png
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-default-group-filled.png
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-default-line.png
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/resources/test_images/rect-stacked.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.857917 qtile-extras-0.24.0/test/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/scripts/cpoll.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/scripts/exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/scripts/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/test_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/test_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/test/widget/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/test/widget/decorations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/decorations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/decorations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/decorations/test_decoration_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/decorations/test_widget_decorations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/test/widget/docs_screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/docs_screenshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/docs_screenshots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/docs_screenshots/ss_groupbox2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/docs_screenshots/ss_iwd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:19.865917 qtile-extras-0.24.0/test/widget/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47648 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/resources/lfs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_alsawidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_analogueclock.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_brightness_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_continuous_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_currentlayouticon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_githubnotifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_global_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_groupbox2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_init_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_injection_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_iwd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_livefootballscores.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_mpris2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_popup_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_scriptexit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_snapcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_statusnotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_strava.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_syncthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_tvhwidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_unitstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_upower.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_visualiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_widget_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/test/widget/test_wordclock.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-20 20:27:09.000000 qtile-extras-0.24.0/whitelist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.382254 qtile-extras-0.25.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/check_for_changes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 16:50:59.382254 qtile-extras-0.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/popup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/popup/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/templates/mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/templates/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51899 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/popup/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.346254 qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/dbusmenu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/footballscores/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/fixtures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24538 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/footballmatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/league.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3551 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchdict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2382 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/morphlinks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/playeraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1317 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/footballscores/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/github-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/github-icons/github.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/global_menu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/global_menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/global_menu/registrar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/media-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/next.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/play_pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/previous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/media-icons/stop.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/snapcast-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/snapcast-icons/snapcast.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/stravadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/stravadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/stravadata/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/stravadata/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/syncthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/syncthing/syncthing.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.350254 qtile-extras-0.25.0/qtile_extras/resources/tvheadend-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/tvheadend-icons/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.354254 qtile-extras-0.25.0/qtile_extras/resources/visualiser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/visualiser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5038 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/visualiser/cava_draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.354254 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   326251 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   330247 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.354254 qtile-extras-0.25.0/qtile_extras/resources/wordclock/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/dutch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/english.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/finnish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/french.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/portuguese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/spanish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/resources/wordclock/swedish.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/qtile_extras/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/alsavolumecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/analogueclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/animatedimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/brightnesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/continuous_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/currentlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/decorations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/githubnotifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/globalmenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33152 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/groupbox2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23460 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/iwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23089 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/livefootballscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/qtile_extras/widget/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/mpris2widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/pulse_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/pulse_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/scriptexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/snapcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/statusnotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/strava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/syncthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/systray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/tvheadend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/unitstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/upower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/qtile_extras/widget/wordclock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/qtile_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 16:50:59.000000 qtile-extras-0.25.0/qtile_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-06 16:50:59.382254 qtile-extras-0.25.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/backend/wayland/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/wayland/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/wayland/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/backend/x11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/x11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/backend/x11/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.362254 qtile-extras-0.25.0/test/popup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/popup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/popup/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/popup/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.342254 qtile-extras-0.25.0/test/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.366254 qtile-extras-0.25.0/test/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-high.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-low.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-medium.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/audio-volume-muted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/icons/menuitem.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.370254 qtile-extras-0.25.0/test/resources/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-E-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-E.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-N-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-N.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-S-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-S.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-W-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-single-W.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-stacked-grouped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-stacked-same-position.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/border-stacked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/combo-rect-plus-powerline.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-custom-path.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag-padding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-filled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-no-radius.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-widget-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default-line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/resources/test_images/rect-stacked.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.370254 qtile-extras-0.25.0/test/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/cpoll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/scripts/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/test_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/test_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/decorations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/test_decoration_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/decorations/test_widget_decorations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/docs_screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/ss_groupbox2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/docs_screenshots/ss_iwd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:59.378254 qtile-extras-0.25.0/test/widget/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47648 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/resources/lfs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_alsawidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_analogueclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_animated_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_brightness_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_continuous_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_currentlayouticon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_githubnotifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_global_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_groupbox2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_init_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_injection_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_iwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_livefootballscores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_mpris2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_popup_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_scriptexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_snapcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_statusnotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_strava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_syncthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_tvhwidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_unitstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_upower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_widget_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/test/widget/test_wordclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-06 16:50:54.000000 qtile-extras-0.25.0/whitelist.py
```

### Comparing `qtile-extras-0.24.0/.github/workflows/changelog.yml` & `qtile-extras-0.25.0/.github/workflows/changelog.yml`

 * *Files 19% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     pull_request:
 
 jobs:
     build:
         runs-on: ubuntu-20.04
         name: "Check CHANGELOG"
         steps:
-            - uses: actions/checkout@v2
+            - uses: actions/checkout@v4
             - name: Install dependencies
               run: |
                 sudo apt update
                 sudo apt install --no-install-recommends jq
-            - uses: lots0logs/gh-action-get-changed-files@2.1.4
+            - uses: lots0logs/gh-action-get-changed-files@2.2.2
               with:
                 token: ${{ secrets.GITHUB_TOKEN }}
             - name: Check changed files
               run: .github/check_for_changes
             - uses: ouzi-dev/commit-status-updater@v1.1.0
               with:
                 status: ${{ env.CHANGELOG_STATUS }}
```

### Comparing `qtile-extras-0.24.0/.github/workflows/ci.yml` & `qtile-extras-0.25.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     build:
         runs-on: ubuntu-22.04
         name: "python ${{ matrix.python-version }}"
         strategy:
             matrix:
                 python-version: [3.9, '3.10', '3.11', '3.12']
         steps:
-            - uses: actions/checkout@v2
+            - uses: actions/checkout@v4
             - name: Set up python ${{ matrix.python-version }}
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v5
               with:
                   python-version: ${{ matrix.python-version }}
             - name: Install dependencies
               run: |
                 sudo apt update
                 sudo apt install --no-install-recommends \
                   libdbus-1-dev libgirepository1.0-dev gir1.2-gtk-3.0 gir1.2-notify-0.7 gir1.2-gudev-1.0 \
@@ -36,15 +36,15 @@
                 tox
             - name: Test widget decoration output
               if: ${{ matrix.python-version == '3.11' }}
               run: |
                 tox -e decorations
             - name: Upload generated images
               if: ${{ always() && matrix.python-version == '3.11' }}
-              uses: actions/upload-artifact@v3
+              uses: actions/upload-artifact@v4
               with:
                 name: generated-images
                 path: decoration_images/
                 retention-days: 5
             - name: Push coverage to Coveralls
               run: |
                 pip -q install coveralls
```

### Comparing `qtile-extras-0.24.0/.github/workflows/release.yml` & `qtile-extras-0.25.0/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,27 @@
   build:
     name: Build qtile-extras pure python distribution
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Install pypa/build
       run: >-
         python3 -m
         pip install
         build
         --user
     - name: Build a binary wheel and a source tarball
       run: python3 -m build
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: >-
       Publish to PyPI
@@ -43,15 +43,15 @@
       name: pypi
       url: https://pypi.org/p/qtile-extras
     permissions:
       id-token: write
 
     steps:
     - name: Download built artifacts
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   publish-to-testpypi:
@@ -66,15 +66,15 @@
       url: https://test.pypi.org/p/qtile-extras
 
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish qtile-extras to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
```

### Comparing `qtile-extras-0.24.0/.gitignore` & `qtile-extras-0.25.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/.pre-commit-config.yaml` & `qtile-extras-0.25.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/CHANGELOG` & `qtile-extras-0.25.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2024-04-08: [RELEASE] v0.25.0 release - compatible with qtile 0.25.0
+2024-03-10: [FEATURE] Expose widget popup menu commands and allow custom positioning
+2024-03-02: [BUGFIX] Fix bug for volume widgets where bar crashes if volume is greater than 100%
+2024-03-02: [BUGFIX] Fix popup menus ignoring config
+2024-02-17: [FEATURE] Add `AnimatedImage` widget
+2024-02-16: [FEATURE] Allow pango markup in `PopupText` controls
+2024-02-09: [BUGFIX] Handle connection errors in `GithubNotifications` widget
 2024-01-20: [RELEASE] v0.24.0 - compatible with qtile 0.24.0
 2024-01-20: [PYPI] Enable release workflow to push future releases to PyPI
 2024-01-20: [BUGFIX] Fix `Visualiser` bug with `hide=True`
 2024-01-20: [FEATURE] Add `GroupBox2` widget
 2023-12-21: [FEATURE] Add `IWD` widget
 2023-11-17: [BUGFIX] Prevent double hooks for Mpris2 widget
 2023-11-13: [BUGFIX] A neater fix for the `Visualiser` CPU bug
```

### Comparing `qtile-extras-0.24.0/LICENSE` & `qtile-extras-0.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/PKG-INFO` & `qtile-extras-0.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtile-extras
-Version: 0.24.0
+Version: 0.25.0
 Summary: Extra items for qtile that are unlikely to be maintained in the main repo.
 Author: elParaguayo
 License: MIT
 Project-URL: homepage, https://github.com/elParaguayo/qtile-extras
 Project-URL: documentation, https://qtile-extras.readthedocs.io/en/stable/
 Project-URL: changelog, https://qtile-extras.readthedocs.io/en/stable/changelog.html
 Project-URL: issues, https://github.com/elParaguayo/qtile-extras/issues
```

### Comparing `qtile-extras-0.24.0/README.md` & `qtile-extras-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/pyproject.toml` & `qtile-extras-0.25.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/bar.py` & `qtile-extras-0.25.0/qtile_extras/bar.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/hook.py` & `qtile-extras-0.25.0/qtile_extras/hook.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/images.py` & `qtile-extras-0.25.0/qtile_extras/images.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/popup/menu.py` & `qtile-extras-0.25.0/qtile_extras/popup/menu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/popup/templates/__init__.py` & `qtile-extras-0.25.0/qtile_extras/popup/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/popup/templates/mpris2.py` & `qtile-extras-0.25.0/qtile_extras/popup/templates/mpris2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/popup/templates/volume.py` & `qtile-extras-0.25.0/qtile_extras/popup/templates/volume.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/popup/toolkit.py` & `qtile-extras-0.25.0/qtile_extras/popup/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1030,14 +1030,15 @@
             None,
             "Font colour when highlighted via `block` (None to use foreground value)",
         ),
         ("highlight_method", "block", "Available options: 'border', 'block' or 'text'."),
         ("h_align", "left", "Text alignment: left, center or right."),
         ("v_align", "middle", "Vertical alignment: top, middle or bottom."),
         ("wrap", False, "Wrap text in layout"),
+        ("markup", False, "Enable pango markup"),
     ]
 
     def __init__(self, text="", **config):
         _PopupWidget.__init__(self, **config)
         self.add_defaults(PopupText.defaults)
         self._text = text
 
@@ -1045,15 +1046,15 @@
         _PopupWidget._configure(self, qtile, container)
         self.layout = self.drawer.textlayout(
             self._text,
             self.foreground,
             self.font,
             self.fontsize,
             None,
-            markup=False,
+            markup=self.markup,
             wrap=self.wrap,
         )
         self.layout.layout.set_alignment(pangocffi.ALIGNMENTS[self.h_align])
         self.layout.width = self.width
 
     def _set_layout_colour(self):
         if self.highlight_method == "text" and self._highlight:
```

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/dbusmenu/__init__.py` & `qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/dbusmenu/dbusmenu.py` & `qtile-extras-0.25.0/qtile_extras/resources/dbusmenu/dbusmenu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/__init__.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/exceptions.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/footballmatch.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/footballmatch.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/league.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/league.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/matchdict.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchdict.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/matchevent.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/matchevent.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/morphlinks.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/morphlinks.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/playeraction.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/playeraction.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/footballscores/utils.py` & `qtile-extras-0.25.0/qtile_extras/resources/footballscores/utils.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/github-icons/github.svg` & `qtile-extras-0.25.0/qtile_extras/resources/github-icons/github.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/global_menu/__init__.py` & `qtile-extras-0.25.0/qtile_extras/resources/global_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/global_menu/registrar.py` & `qtile-extras-0.25.0/qtile_extras/resources/global_menu/registrar.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/media-icons/default.png` & `qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/media-icons/default.svg` & `qtile-extras-0.25.0/qtile_extras/resources/media-icons/default.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/media-icons/next.svg` & `qtile-extras-0.25.0/qtile_extras/resources/media-icons/next.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/media-icons/play_pause.svg` & `qtile-extras-0.25.0/qtile_extras/resources/media-icons/play_pause.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/media-icons/previous.svg` & `qtile-extras-0.25.0/qtile_extras/resources/media-icons/previous.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/media-icons/stop.svg` & `qtile-extras-0.25.0/qtile_extras/resources/media-icons/stop.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/snapcast-icons/snapcast.svg` & `qtile-extras-0.25.0/qtile_extras/resources/snapcast-icons/snapcast.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/stravadata/locations.py` & `qtile-extras-0.25.0/qtile_extras/resources/stravadata/locations.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/stravadata/sync.py` & `qtile-extras-0.25.0/qtile_extras/resources/stravadata/sync.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/syncthing/syncthing.svg` & `qtile-extras-0.25.0/qtile_extras/resources/syncthing/syncthing.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/tvheadend-icons/icon.svg` & `qtile-extras-0.25.0/qtile_extras/resources/tvheadend-icons/icon.svg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/visualiser/cava_draw.py` & `qtile-extras-0.25.0/qtile_extras/resources/visualiser/cava_draw.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wallpapers/qte_tiles.png` & `qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_tiles.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wallpapers/qte_triangles.png` & `qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png` & `qtile-extras-0.25.0/qtile_extras/resources/wallpapers/qte_triangles_rounded.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/dutch.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/dutch.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/english.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/english.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/finnish.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/finnish.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/french.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/french.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/portuguese.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/portuguese.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/spanish.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/spanish.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/resources/wordclock/swedish.py` & `qtile-extras-0.25.0/qtile_extras/resources/wordclock/swedish.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/__init__.py` & `qtile-extras-0.25.0/qtile_extras/widget/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from libqtile.widget.import_error import make_error
 
 from qtile_extras.widget.decorations import inject_decorations
 
 widgets = {
     "ALSAWidget": "alsavolumecontrol",
     "AnalogueClock": "analogueclock",
+    "AnimatedImage": "animatedimage",
     "Bluetooth": "bluetooth",
     "BrightnessControl": "brightnesscontrol",
     "ContinuousPoll": "continuous_poll",
     "CurrentLayoutIcon": "currentlayout",
     "CPUGraph": "graph",
     "GithubNotifications": "githubnotifications",
     "GlobalMenu": "globalmenu",
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/alsavolumecontrol.py` & `qtile-extras-0.25.0/qtile_extras/widget/alsavolumecontrol.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/analogueclock.py` & `qtile-extras-0.25.0/qtile_extras/widget/analogueclock.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/base.py` & `qtile-extras-0.25.0/qtile_extras/widget/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,18 @@
             x_offset += self.icon_width
 
         # Does bar need to be displayed
         if self.show_bar and not self.hidden:
             # Text and colour depends on mute status and volume level
             if not self.muted:
                 bar_text = self.text_format.format(volume=self.volume)
-                bar_colour = next(x[1] for x in self.colours if self.volume <= x[0])
+                bar_colour = next(
+                    (x[1] for x in self.colours if self.volume <= x[0]),
+                    self.colours[-1][1],  # Default if volume > 100%
+                )
             else:
                 bar_text = "X"
                 bar_colour = self.bar_colour_mute
 
             bar_value = self.volume / 100.0
             self.draw_bar(
                 x_offset=x_offset, bar_text=bar_text, bar_colour=bar_colour, bar_value=bar_value
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/brightnesscontrol.py` & `qtile-extras-0.25.0/qtile_extras/widget/brightnesscontrol.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/continuous_poll.py` & `qtile-extras-0.25.0/qtile_extras/widget/continuous_poll.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/currentlayout.py` & `qtile-extras-0.25.0/qtile_extras/widget/currentlayout.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/decorations.py` & `qtile-extras-0.25.0/qtile_extras/widget/decorations.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/githubnotifications.py` & `qtile-extras-0.25.0/qtile_extras/widget/githubnotifications.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from pathlib import Path
 
 import requests
 from libqtile import bar
 from libqtile.command.base import expose_command
 from libqtile.log_utils import logger
 from libqtile.widget import base
+from requests.exceptions import ConnectionError
 
 from qtile_extras import hook
 from qtile_extras.images import ImgMask
 
 GITHUB_ICON = Path(__file__).parent / ".." / "resources" / "github-icons" / "github.svg"
 NOTIFICATIONS = "https://api.github.com/notifications"
 
@@ -114,45 +115,61 @@
         if self.error:
             return self.error_colour
         elif self.has_notifications:
             return self.active_colour
         else:
             return self.inactive_colour
 
+    @expose_command()
     def update(self):
+        """Trigger a check for new notifications."""
         if not self.token:
             self.error = True
             logger.error("No access token provided.")
             return
         self._polling = True
         future = self.qtile.run_in_executor(self._get_data)
         future.add_done_callback(self._read_data)
+        if self._timer is not None and not self._timer.cancelled():
+            self._timer.cancel()
 
     def _get_data(self):
         headers = {
             "Accept": "application/vnd.github.v3+json",
             "Authorization": f"token {self.token}",
         }
         return requests.get(NOTIFICATIONS, headers=headers)
 
     def _read_data(self, reply):
-        r = reply.result()
+        self.error = True
+        self._polling = False
 
-        if r.status_code != 200:
-            self.error = True
-            logger.warning("Github returned a %d status code.", r.status_code)
-            self._polling = False
-            return
+        # Check if an exception was raised when trying to retrieve data
+        exc = reply.exception()
+        if exc:
+            if isinstance(exc, ConnectionError):
+                logger.error("Unable to connect to Github API.")
+            else:
+                logger.error(  # noqa: G201
+                    "Unexpected error when connecting to Github.", exc_info=exc
+                )
 
-        self.error = False
-        self.has_notifications = bool(r.json())
-        if self.has_notifications and not self._new_notification:
-            hook.fire("ghn_new_notification")
-        self._new_notification = self.has_notifications
-        self._polling = False
+        # If not, get the result
+        else:
+            r = reply.result()
+
+            if r.status_code != 200:
+                logger.warning("Github returned a %d status code.", r.status_code)
+
+            else:
+                self.error = False
+                self.has_notifications = bool(r.json())
+                if self.has_notifications and not self._new_notification:
+                    hook.fire("ghn_new_notification")
+                self._new_notification = self.has_notifications
 
         self._timer = self.timeout_add(self.update_interval, self.update)
         self.draw()
 
     def calculate_length(self):
         if self.img is None:
             return 0
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/globalmenu.py` & `qtile-extras-0.25.0/qtile_extras/widget/globalmenu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/graph.py` & `qtile-extras-0.25.0/qtile_extras/widget/graph.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/groupbox2.py` & `qtile-extras-0.25.0/qtile_extras/widget/groupbox2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/image.py` & `qtile-extras-0.25.0/qtile_extras/widget/image.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/iwd.py` & `qtile-extras-0.25.0/qtile_extras/widget/iwd.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from dbus_next.errors import DBusError, InterfaceNotFoundError
 from dbus_next.service import ServiceInterface, method
 from libqtile.command.base import expose_command
 from libqtile.log_utils import logger
 from libqtile.utils import create_task
 from libqtile.widget import base
 
-from qtile_extras.popup.menu import PopupMenuItem, PopupMenuSeparator
 from qtile_extras.widget.mixins import ConnectionCheckMixin, GraphicalWifiMixin, MenuMixin
 
 IWD_SERVICE = "net.connman.iwd"
 IWD_DEVICE = IWD_SERVICE + ".Device"
 IWD_STATION = IWD_SERVICE + ".Station"
 IWD_STATION_DIAGNOSTIC = IWD_SERVICE + ".StationDiagnostic"
 IWD_NETWORK = IWD_SERVICE + ".Network"
@@ -303,15 +302,15 @@
         self.device = None
         self.networks = {}
         self.devices = {}
         self._device_tasks = []
         self._network_tasks = []
         self.timer = None
         self._setting_up = False
-        self.add_callbacks({"Button1": self.do_menu})
+        self.add_callbacks({"Button1": self.show_networks})
         self._can_connect = False
         self.percentage = 0
         self._refresh_timer = None
 
     def _configure(self, qtile, bar):
         base._TextBox._configure(self, qtile, bar)
         self.set_wifi_sizes()
@@ -563,71 +562,103 @@
         if self.show_text:
             self.layout.draw(offset, int(self.bar.height / 2.0 - self.layout.height / 2.0) + 1)
 
         self.drawer.draw(
             offsetx=self.offsetx, offsety=self.offsety, width=self.width, height=self.height
         )
 
-    def do_menu(self):
+    def _get_menu_items(self):
         menu_items = []
+        pmi = self.create_menu_item
+        pms = self.create_menu_separator
 
         if self.device.connected_network:
-            menu_items.extend(
-                [
-                    PopupMenuItem("Connected to:"),
-                    PopupMenuItem(self.networks[self.device.connected_network].name),
-                    PopupMenuSeparator(),
-                ]
-            )
+            # We can get a KeyError here if the deivce was suspended while connected
+            # nut resumed when the network is no longer visible.
+            try:
+                name = self.networks[self.device.connected_network].name
+            except KeyError:
+                self.device.connected_network = ""
+            else:
+                menu_items.extend(
+                    [
+                        pmi("Connected to:"),
+                        pmi(name),
+                        pms(),
+                    ]
+                )
 
         networks = []
 
         for path, network in self.networks.items():
             if path == self.device.connected_network:
                 continue
 
             def connect(n):
                 task = create_task(n.connect())
                 task.add_done_callback(self.connect_response)
 
             enabled = (self._can_connect and not network.type == "8021x") or network.known
 
-            item = PopupMenuItem(
+            item = pmi(
                 f"{network.name} ({network.type})",
                 mouse_callbacks={"Button1": lambda n=network: connect(n)} if enabled else {},
                 enabled=enabled,
             )
             networks.append(item)
 
         if networks:
-            networks.insert(0, PopupMenuItem("Visible networks:"))
-            networks.append(PopupMenuSeparator())
+            networks.insert(0, pmi("Visible networks:"))
+            networks.append(pms())
             menu_items.extend(networks)
 
         if self.device.scanning:
-            device_item = PopupMenuItem("Scanning...", enabled=False)
+            device_item = pmi("Scanning...", enabled=False)
         else:
-            device_item = PopupMenuItem(
+            device_item = pmi(
                 "Scan for networks",
                 mouse_callbacks={"Button1": self.scan},
             )
 
         menu_items.append(device_item)
 
-        self.display_menu(menu_items)
+        return menu_items
 
     def connect_response(self, task):
         exc = task.exception()
         if exc is not None:
             if isinstance(exc, Cancelled):
                 logger.info("Password entry cancelled.")
             else:
                 logger.warning("Could not connect: %s", exc)
 
     @expose_command
+    def show_networks(
+        self,
+        x=None,
+        y=None,
+        centered=False,
+        warp_pointer=False,
+        relative_to=1,
+        relative_to_bar=False,
+        hide_on_timeout=None,
+    ):
+        """Show menu with available networks."""
+        self.display_menu(
+            menu_items=self._get_menu_items(),
+            x=x,
+            y=y,
+            centered=centered,
+            warp_pointer=warp_pointer,
+            relative_to=relative_to,
+            relative_to_bar=relative_to_bar,
+            hide_on_timeout=hide_on_timeout,
+        )
+
+    @expose_command
     def scan(self):
         if self.device:
             task = create_task(self.device.scan())
             task.add_done_callback(self._check_scan)
 
     def _check_scan(self, task):
         if task.exception():
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/livefootballscores.py` & `qtile-extras-0.25.0/qtile_extras/widget/livefootballscores.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 from libqtile import bar
 from libqtile.command.base import expose_command
 from libqtile.log_utils import logger
 from libqtile.widget import base
 
 from qtile_extras import hook
-from qtile_extras.popup.menu import PopupMenuItem, PopupMenuSeparator
 from qtile_extras.popup.toolkit import PopupRelativeLayout, PopupText
 from qtile_extras.resources.footballscores import FootballMatch, FSConnectionError, League
 from qtile_extras.widget.mixins import ExtendedPopupMixin, MenuMixin
 
 if TYPE_CHECKING:
     from typing import Any  # noqa: F401
 
@@ -195,15 +194,14 @@
         ("status_halftime", "aaaa00", "Colour when half time"),
         ("status_fulltime", "666666", "Colour when match has ended"),
         (
             "popup_font",
             "monospace",
             "Font to use for displaying upcoming recordings. A monospace font " "is recommended",
         ),
-        ("opacity", 0.8, "Opacity for popup window."),
         ("popup_display_timeout", 10, "Seconds to show recordings."),
         ("menu_width", 300, "Width of menu showing all matches"),
         ("popup_layout", DETAILED_LAYOUT, "Layout to use for extended match information"),
         (
             "popup_show_args",
             {"centered": True, "hide_on_timeout": 5},
             "Arguments to set behaviour of extended popup",
@@ -269,15 +267,15 @@
         self.queue_timer = None
 
         self.popup = None
 
         self.add_callbacks(
             {
                 "Button1": self.loop_match_info,
-                "Button3": self.show_menu,
+                "Button3": self.show_matches,
                 "Button4": self.scroll_up,
                 "Button5": self.scroll_down,
             }
         )
 
     def reset_flags(self):
         for flag in self.flags:
@@ -623,15 +621,15 @@
         self.popup.kill()
         self.popup = None
 
     def toggle_info(self):
         if self.menu and not self.menu._killed:
             self.menu.kill()
         else:
-            self.show_menu()
+            self.show_matches()
 
     @expose_command()
     def popup(self):
         """Display window listing all matches"""
         self.toggle_info()
 
     @expose_command()
@@ -665,46 +663,65 @@
     def select_match(self, match):
         self._selected_match = match
         self.update_or_show_popup()
 
     def _get_match_list(self):
         lines = []
 
+        pmi = self.create_menu_item
+        pms = self.create_menu_separator
+
         def _callback(team):
             return {"mouse_callbacks": {"Button1": lambda team=team: self.select_match(team)}}
 
         for team in [m for m in self.sources[0] if m]:
             lines.extend(
                 [
-                    PopupMenuItem(text=team.competition, enabled=False),
-                    PopupMenuItem(text=team.format_text(self.popup_text), **_callback(team)),
+                    pmi(text=team.competition, enabled=False),
+                    pmi(text=team.format_text(self.popup_text), **_callback(team)),
                 ]
             )
 
         if self.sources[1]:
             if lines and any(m for m in self.sources[1]):
-                lines.append(PopupMenuSeparator())
+                lines.append(pms())
 
-            lines.append(PopupMenuItem(text="Selected Teams:", enabled=False))
+            lines.append(pmi(text="Selected Teams:", enabled=False))
 
             for team in [m for m in self.sources[1] if m]:
-                lines.append(
-                    PopupMenuItem(text=team.format_text(self.popup_text), **_callback(team))
-                )
+                lines.append(pmi(text=team.format_text(self.popup_text), **_callback(team)))
 
         for league in self.sources[2]:
             if lines and league:
-                lines.append(PopupMenuSeparator())
+                lines.append(pms())
             if league:
-                lines.append(PopupMenuItem(text="{}:".format(league.league_name), enabled=False))
+                lines.append(pmi(text="{}:".format(league.league_name), enabled=False))
                 for team in league:
-                    lines.append(
-                        PopupMenuItem(text=team.format_text(self.popup_text), **_callback(team))
-                    )
+                    lines.append(pmi(text=team.format_text(self.popup_text), **_callback(team)))
 
         if not lines:
-            lines.append(PopupMenuItem(text="No matches today", enabled=False))
+            lines.append(pmi(text="No matches today", enabled=False))
 
         return lines
 
-    def show_menu(self):
-        self.display_menu(self._get_match_list())
+    @expose_command
+    def show_matches(
+        self,
+        x=None,
+        y=None,
+        centered=False,
+        warp_pointer=False,
+        relative_to=1,
+        relative_to_bar=False,
+        hide_on_timeout=None,
+    ):
+        """Show menu with followed matchs."""
+        self.display_menu(
+            menu_items=self._get_match_list(),
+            x=x,
+            y=y,
+            centered=centered,
+            warp_pointer=warp_pointer,
+            relative_to=relative_to,
+            relative_to_bar=relative_to_bar,
+            hide_on_timeout=hide_on_timeout,
+        )
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/mirror.py` & `qtile-extras-0.25.0/qtile_extras/widget/mirror.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/mixins/__init__.py` & `qtile-extras-0.25.0/qtile_extras/widget/mixins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+from __future__ import annotations
+
 import math
 import socket
 from contextlib import contextmanager
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 from libqtile.command.base import expose_command
 from libqtile.configurable import Configurable, ExtraFallback
 from libqtile.log_utils import logger
 from libqtile.popup import Popup
 
-from qtile_extras.popup.menu import PopupMenu
+from qtile_extras.popup.menu import PopupMenu, PopupMenuItem, PopupMenuSeparator
+from qtile_extras.resources.dbusmenu import DBusMenuItem
 
 if TYPE_CHECKING:
     from typing import Any, Callable  # noqa: F401
 
 
 PI = math.pi
 
@@ -206,27 +209,27 @@
         ("menu_offset_y", 0, "Fine tune y position of menu"),
         ("separator_colour", "555555", "Colour of menu separator"),
         (
             "highlight_colour",
             "0060A0",
             "Colour of highlight for menu items (None for no highlight)",
         ),
-        ("highlight_radius", 0, "Radius for menu highlight"),
+        ("highlight_radius", 5, "Radius for menu highlight"),
         (
             "menu_row_height",
             None,
             (
                 "Height of menu row (NB text entries are 2 rows tall, separators are 1 row tall.) "
                 '"None" will attempt to calculate height based on font size.'
             ),
         ),
         ("menu_width", 200, "Context menu width"),
         ("show_menu_icons", True, "Show icons in context menu"),
         ("hide_after", 0.5, "Time in seconds before hiding menu atfer mouse leave"),
-        ("opacity", 1, "Menu opactity"),
+        ("opacity", 1, "Menu opacity"),
         ("icon_theme", None, "Icon theme for DBus menu items"),
     ]  # type: list[tuple[str, Any, str]]
 
     def __init__(self, **config):
         self.menu_config = {
             "font": self.menu_font,
             "fontsize": self.menu_fontsize,
@@ -246,32 +249,25 @@
             "hide_after": self.hide_after,
             "opacity": self.opacity,
             "icon_theme": self.icon_theme,
         }
 
         self.menu = None
 
-    def set_menu_position(self, x: int, y: int) -> tuple[int, int]:
-        """
-        Set the x and y coordinates of the menu.
-
-        The method receivs and x and y value which is calculated during
-        ``self.display_menu``. The x and y coordinates place the menu at
-        the start of the widget and adjacent to the bar. The values have also
-        already been adjusted to ensure that the menu will fit on the screen.
-
-        This method can be overriden if menus need to adjust the placement of the menu
-        e.g. if the widget has multiple items with separate menus.
-
-        NB: if a user has defined ``menu_offset_x`` or ``menu_offset_y`` these will
-        be applied after this method and so should not be included here.
-        """
-        return x, y
-
-    def display_menu(self, menu_items):
+    def display_menu(
+        self,
+        menu_items: list[PopupMenuItem | PopupMenuSeparator | DBusMenuItem] = list(),
+        x: int | float | None = None,
+        y: int | float | None = None,
+        centered: bool = False,
+        warp_pointer: bool = False,
+        relative_to: int = 1,
+        relative_to_bar: bool = False,
+        hide_on_timeout: int | float | None = None,
+    ):
         """
         Method to display the menu.
 
         By default, the menu will be placed by the widget using the widget's offset along the bar
         and the bar's size. If the position needs to be adjusted then the x and y coordinates should
         be set by overriding the ``set_menu_position`` method.
         """
@@ -281,37 +277,70 @@
         if self.menu and not self.menu._killed:
             self.menu.kill()
 
         self.menu = self._build_menu(self.qtile, menu_items, **self.menu_config)
 
         screen = self.bar.screen
 
-        if screen.top == self.bar:
-            x = min(self.offsetx, self.bar.width - self.menu.width - 2 * self.menu_border_width)
-            y = self.bar.height
+        custom_x = x
+        custom_y = y
+
+        if screen.top is self.bar:
+            x = min(self.offsetx, screen.width - self.menu.width - 2 * self.menu_border_width)
+            y = self.bar.height + self.bar.margin[0]
 
         elif screen.bottom == self.bar:
-            x = min(self.offsetx, self.bar.width - self.menu.width - 2 * self.menu_border_width)
-            y = screen.height - self.bar.height - self.menu.height - 2 * self.menu_border_width
+            x = min(self.offsetx, screen.width - self.menu.width - 2 * self.menu_border_width)
+            y = (
+                screen.height
+                - (self.bar.height + self.bar.margin[2])
+                - self.menu.height
+                - 2 * self.menu_border_width
+            )
 
         elif screen.left == self.bar:
-            x = self.bar.width
+            x = self.bar.width + self.bar.margin[3]
             y = min(self.offsety, screen.height - self.menu.height - 2 * self.menu_border_width)
 
         else:
-            x = screen.width - self.bar.width - self.menu.width - 2 * self.menu_border_width
+            x = (
+                screen.width
+                - (self.bar.width + self.bar.margin[1])
+                - self.menu.width
+                - 2 * self.menu_border_width
+            )
             y = min(self.offsety, screen.height - self.menu.height - 2 * self.menu_border_width)
 
-        x, y = self.set_menu_position(x, y)
-
         # Adjust the position for any user-defined settings
         x += self.menu_offset_x
         y += self.menu_offset_y
 
-        self.menu.show(x, y)
+        self.menu.show(
+            x=custom_x if custom_x is not None else x,
+            y=custom_y if custom_y is not None else y,
+            centered=centered,
+            warp_pointer=warp_pointer,
+            relative_to=relative_to,
+            relative_to_bar=relative_to_bar,
+            hide_on_timeout=hide_on_timeout,
+        )
+
+    def create_menu_item(self, text, **config):
+        """
+        Create a PopupMenuItem with parameters specified here taking preference over default.
+        """
+        item_config = {**self.menu_config, **config}
+        return PopupMenuItem(text, **item_config)
+
+    def create_menu_separator(self, **config):
+        """
+        Create a PopupMenuSeparator with parameters specified here taking preference over default.
+        """
+        item_config = {**self.menu_config, **config}
+        return PopupMenuSeparator(**item_config)
 
 
 class DbusMenuMixin(MenuMixin):
     """
     Builds a menu from ``qtile_extras.resources.dbusmenu.DBusMenuItem``
     objects.
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/mpris2widget.py` & `qtile-extras-0.25.0/qtile_extras/widget/mpris2widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import asyncio
 
-from dbus_next.constants import MessageType
 from libqtile import widget
 from libqtile.command.base import expose_command
-from libqtile.utils import _send_dbus_message
 
 from qtile_extras import hook
 from qtile_extras.popup.templates.mpris2 import DEFAULT_IMAGE, DEFAULT_LAYOUT
 from qtile_extras.widget.mixins import ExtendedPopupMixin
 
 
 def hms(time):
@@ -155,18 +153,15 @@
             previous={"Button1": self.previous},
             stop={"Button1": self.stop},
         )
 
     def _set_popup_text(self, task):
         if task.exception():
             return
-        bus, msg = task.result()
-
-        if bus:
-            bus.disconnect()
+        msg = task.result()
 
         result = msg.body[0]
 
         metadata = getattr(result.get("Metadata"), "value", dict())
         position = getattr(result.get("Position"), "value", 0)
         title = getattr(metadata.get("xesam:title"), "value", "")
         artist = ", ".join(getattr(metadata.get("xesam:artist"), "value", list()))
@@ -216,17 +211,15 @@
 
         if not getattr(self.extended_popup, "bound_callbacks", False):
             self.bind_callbacks()
             self._popup_values = {}
             self.extended_popup.bound_callbacks = True
 
         task = asyncio.create_task(
-            _send_dbus_message(
-                True,
-                MessageType.METHOD_CALL,
+            self._send_message(
                 self._current_player,
                 "org.freedesktop.DBus.Properties",
                 "/org/mpris/MediaPlayer2",
                 "GetAll",
                 "s",
                 ["org.mpris.MediaPlayer2.Player"],
             )
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/network.py` & `qtile-extras-0.25.0/qtile_extras/widget/network.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/pulse_extra.py` & `qtile-extras-0.25.0/qtile_extras/widget/pulse_extra.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/pulse_volume.py` & `qtile-extras-0.25.0/test/widget/test_popup_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# Copyright (c) 2023 elParaguayo
+# Copyright (c) 2022 elParaguayo
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -14,62 +13,82 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from libqtile.command.base import expose_command
-from libqtile.utils import create_task
-from libqtile.widget.pulse_volume import PulseVolume as QPulseVolume
-from libqtile.widget.pulse_volume import pulse
-
-from qtile_extras.popup.menu import PopupMenuItem
-from qtile_extras.widget.mixins import MenuMixin
-
-
-class PulseVolume(QPulseVolume, MenuMixin):
-    """
-    Same as qtile's ``PulseVolume`` widget but includes the ability to
-    select the default output sink via the ``select_sink()`` command. This is
-    bound to the middle-click button on the widget by default.
-    """
-
-    defaults = [("menu_width", 300, "Width of list showing available sinks.")]
-
-    def __init__(self, **config):
-        QPulseVolume.__init__(self, **config)
-        self.add_defaults(MenuMixin.defaults)
-        self.add_defaults(PulseVolume.defaults)
-        MenuMixin.__init__(self, **config)
-        self.add_callbacks({"Button2": self.select_sink})
-
-    async def set_sink(self, sink):
-        if not pulse.pulse.connected:
-            return
-
-        await pulse.pulse.default_set(sink)
-
-    async def show_sinks(self):
-        if not pulse.pulse.connected:
-            return
-
-        sinks = await pulse.pulse.sink_list()
-        if not sinks:
-            return
-
-        menu_items = [PopupMenuItem(text="Select output sink:", enabled=False)]
-
-        def _callback(team):
-            return {
-                "mouse_callbacks": {"Button1": lambda sink=sink: create_task(self.set_sink(sink))}
-            }
-
-        for sink in sinks:
-            menu_items.append(PopupMenuItem(text=sink.description, **_callback(sink)))
-
-        self.display_menu(menu_items)
-
-    @expose_command()
-    def select_sink(self):
-        """Select output sink from available sinks."""
-        create_task(self.show_sinks())
+import libqtile
+import pytest
+from libqtile import widget
+
+from qtile_extras.popup.toolkit import PopupAbsoluteLayout, PopupText
+from qtile_extras.widget.mixins import ExtendedPopupMixin
+from test.helpers import Retry
+
+
+@Retry(ignore_exceptions=(AssertionError,))
+def assert_window_count(manager, number):
+    assert len(manager.c.internal_windows()) == number
+
+
+class ModdedWidget(widget.TextBox, ExtendedPopupMixin):
+    def __init__(self, text, **config):
+        widget.TextBox.__init__(self, text, **config)
+        ExtendedPopupMixin.__init__(self)
+        self.add_defaults(ExtendedPopupMixin.defaults)
+
+    def _update_popup(self):
+        self.extended_popup.update_controls(textbox1="Text set ok")
+
+    def info(self):
+        return {"text": self.extended_popup.controls[0].text if self.has_popup else ""}
+
+
+class PopupConfig(libqtile.confreader.Config):
+    auto_fullscreen = True
+    mouse = []
+    groups = [
+        libqtile.config.Group("a"),
+    ]
+    layouts = [libqtile.layout.Max()]
+    floating_layout = libqtile.resources.default_config.floating_layout
+    screens = [
+        libqtile.config.Screen(
+            top=libqtile.bar.Bar(
+                [
+                    ModdedWidget(
+                        "",
+                        popup_layout=PopupAbsoluteLayout(controls=[PopupText(name="textbox1")]),
+                        popup_hide_timeout=1,
+                    )
+                ],
+                50,
+            ),
+        )
+    ]
+
+
+@pytest.mark.parametrize("manager", [PopupConfig], indirect=True)
+def test_popup_mixin(manager, backend_name):
+    number = len(manager.c.internal_windows())
+    widget = manager.c.widget["moddedwidget"]
+    assert not widget.info()["text"]
+
+    widget.eval("self.update_or_show_popup()")
+    widget.eval("self.update_or_show_popup()")
+
+    assert_window_count(manager, number + 1)
+    assert widget.info()["text"] == "Text set ok"
+
+    if backend_name == "x11":
+        pytest.xfail("X11 fails last check.")
+
+    # Popup should close automatically
+    assert_window_count(manager, number)
+
+
+def test_popup_missing_method():
+    widget = ModdedWidget("")
+    widget._update_popup = ExtendedPopupMixin._update_popup
+    with pytest.raises(NotImplementedError):
+        widget._update_popup(widget)
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/scriptexit.py` & `qtile-extras-0.25.0/qtile_extras/widget/scriptexit.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/snapcast.py` & `qtile-extras-0.25.0/qtile_extras/widget/snapcast.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import contextlib
 import shlex
 import subprocess
 from pathlib import Path
 
 import requests
 from libqtile import bar
 from libqtile.command.base import expose_command
@@ -165,14 +166,17 @@
         """Toggle Snapcast on and off."""
         if self._proc is None:
             self._proc = subprocess.Popen(
                 self._cmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
             )
         else:
             self._proc.terminate()
+            # Use wait() to prevent zombie process but don't block indefinitely
+            with contextlib.suppress(subprocess.TimeoutExpired):
+                self._proc.wait(timeout=2)
             self._proc = None
 
         self.draw()
 
     def calculate_length(self):
         if self.img is None:
             return 0
```

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/statusnotifier.py` & `qtile-extras-0.25.0/qtile_extras/widget/statusnotifier.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/strava.py` & `qtile-extras-0.25.0/qtile_extras/widget/strava.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/syncthing.py` & `qtile-extras-0.25.0/qtile_extras/widget/syncthing.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/systray.py` & `qtile-extras-0.25.0/qtile_extras/widget/systray.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/tvheadend.py` & `qtile-extras-0.25.0/qtile_extras/widget/tvheadend.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/unitstatus.py` & `qtile-extras-0.25.0/qtile_extras/widget/unitstatus.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/upower.py` & `qtile-extras-0.25.0/qtile_extras/widget/upower.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/visualiser.py` & `qtile-extras-0.25.0/qtile_extras/widget/visualiser.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras/widget/wordclock.py` & `qtile-extras-0.25.0/qtile_extras/widget/wordclock.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/qtile_extras.egg-info/PKG-INFO` & `qtile-extras-0.25.0/qtile_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtile-extras
-Version: 0.24.0
+Version: 0.25.0
 Summary: Extra items for qtile that are unlikely to be maintained in the main repo.
 Author: elParaguayo
 License: MIT
 Project-URL: homepage, https://github.com/elParaguayo/qtile-extras
 Project-URL: documentation, https://qtile-extras.readthedocs.io/en/stable/
 Project-URL: changelog, https://qtile-extras.readthedocs.io/en/stable/changelog.html
 Project-URL: issues, https://github.com/elParaguayo/qtile-extras/issues
```

### Comparing `qtile-extras-0.24.0/qtile_extras.egg-info/SOURCES.txt` & `qtile-extras-0.25.0/qtile_extras.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .github/workflows/ci.yml
 .github/workflows/pre-commit.yml
 .github/workflows/release.yml
 qtile_extras/__init__.py
 qtile_extras/bar.py
 qtile_extras/hook.py
 qtile_extras/images.py
+qtile_extras/py.typed
 qtile_extras.egg-info/PKG-INFO
 qtile_extras.egg-info/SOURCES.txt
 qtile_extras.egg-info/dependency_links.txt
 qtile_extras.egg-info/top_level.txt
 qtile_extras/popup/__init__.py
 qtile_extras/popup/menu.py
 qtile_extras/popup/toolkit.py
@@ -67,14 +68,15 @@
 qtile_extras/resources/wordclock/french.py
 qtile_extras/resources/wordclock/portuguese.py
 qtile_extras/resources/wordclock/spanish.py
 qtile_extras/resources/wordclock/swedish.py
 qtile_extras/widget/__init__.py
 qtile_extras/widget/alsavolumecontrol.py
 qtile_extras/widget/analogueclock.py
+qtile_extras/widget/animatedimage.py
 qtile_extras/widget/base.py
 qtile_extras/widget/bluetooth.py
 qtile_extras/widget/brightnesscontrol.py
 qtile_extras/widget/continuous_poll.py
 qtile_extras/widget/currentlayout.py
 qtile_extras/widget/decorations.py
 qtile_extras/widget/githubnotifications.py
@@ -163,14 +165,15 @@
 test/scripts/cpoll.py
 test/scripts/exit.py
 test/scripts/window.py
 test/widget/__init__.py
 test/widget/conftest.py
 test/widget/test_alsawidget.py
 test/widget/test_analogueclock.py
+test/widget/test_animated_image.py
 test/widget/test_brightness_control.py
 test/widget/test_continuous_poll.py
 test/widget/test_currentlayouticon.py
 test/widget/test_githubnotifications.py
 test/widget/test_global_menu.py
 test/widget/test_groupbox2.py
 test/widget/test_image.py
```

### Comparing `qtile-extras-0.24.0/setup.cfg` & `qtile-extras-0.25.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/backend/wayland/conftest.py` & `qtile-extras-0.25.0/test/backend/wayland/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/backend/x11/conftest.py` & `qtile-extras-0.25.0/test/backend/x11/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/conftest.py` & `qtile-extras-0.25.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/helpers.py` & `qtile-extras-0.25.0/test/helpers.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/popup/test_menu.py` & `qtile-extras-0.25.0/test/popup/test_menu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/popup/test_toolkit.py` & `qtile-extras-0.25.0/test/popup/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-default-grouped-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-default-grouped-padding_x.png` & `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_x.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-default-grouped-padding_y.png` & `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped-padding_y.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-default-grouped.png` & `qtile-extras-0.25.0/test/resources/test_images/border-default-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-default-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/border-default-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-default.png` & `qtile-extras-0.25.0/test/resources/test_images/border-default.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-E-grouped.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-E-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-E.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-E.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-N-grouped.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-N-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-N.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-N.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-S-grouped.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-S-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-S.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-S.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-W-grouped.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-W-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-single-W.png` & `qtile-extras-0.25.0/test/resources/test_images/border-single-W.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-stacked-grouped.png` & `qtile-extras-0.25.0/test/resources/test_images/border-stacked-grouped.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-stacked-same-position.png` & `qtile-extras-0.25.0/test/resources/test_images/border-stacked-same-position.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/border-stacked.png` & `qtile-extras-0.25.0/test/resources/test_images/border-stacked.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/combo-rect-plus-powerline.png` & `qtile-extras-0.25.0/test/resources/test_images/combo-rect-plus-powerline.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_left-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_left.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_left.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_right-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-arrow_right.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-arrow_right.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-back_slash-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-back_slash.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-back_slash.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-custom-path.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-custom-path.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-forward_slash-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-forward_slash.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-forward_slash.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_left-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_left.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_left.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_right-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-rounded_right.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-rounded_right.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-zig_zag-padding.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag-padding.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/powerline-zig_zag.png` & `qtile-extras-0.25.0/test/resources/test_images/powerline-zig_zag.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-default-filled.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-default-filled.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-default-group-filled-no-radius.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-no-radius.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-default-group-filled-widget-background.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled-widget-background.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-default-group-filled.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-default-group-filled.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-default-line.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-default-line.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-default.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-default.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/resources/test_images/rect-stacked.png` & `qtile-extras-0.25.0/test/resources/test_images/rect-stacked.png`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/scripts/window.py` & `qtile-extras-0.25.0/test/scripts/window.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/test_bar.py` & `qtile-extras-0.25.0/test/test_bar.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/test_images.py` & `qtile-extras-0.25.0/test/test_images.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/conftest.py` & `qtile-extras-0.25.0/test/widget/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/decorations/conftest.py` & `qtile-extras-0.25.0/test/widget/decorations/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/decorations/test_decoration_output.py` & `qtile-extras-0.25.0/test/widget/decorations/test_decoration_output.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/decorations/test_widget_decorations.py` & `qtile-extras-0.25.0/test/widget/decorations/test_widget_decorations.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/docs_screenshots/conftest.py` & `qtile-extras-0.25.0/test/widget/docs_screenshots/conftest.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/docs_screenshots/ss_groupbox2.py` & `qtile-extras-0.25.0/test/widget/docs_screenshots/ss_groupbox2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/docs_screenshots/ss_iwd.py` & `qtile-extras-0.25.0/test/widget/docs_screenshots/ss_iwd.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/resources/lfs_data.py` & `qtile-extras-0.25.0/test/widget/resources/lfs_data.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_alsawidget.py` & `qtile-extras-0.25.0/test/widget/test_alsawidget.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_analogueclock.py` & `qtile-extras-0.25.0/test/widget/test_analogueclock.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_brightness_control.py` & `qtile-extras-0.25.0/test/widget/test_brightness_control.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_continuous_poll.py` & `qtile-extras-0.25.0/test/widget/test_continuous_poll.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_currentlayouticon.py` & `qtile-extras-0.25.0/test/widget/test_currentlayouticon.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_githubnotifications.py` & `qtile-extras-0.25.0/test/widget/test_githubnotifications.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_global_menu.py` & `qtile-extras-0.25.0/test/widget/test_global_menu.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_groupbox2.py` & `qtile-extras-0.25.0/test/widget/test_groupbox2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_image.py` & `qtile-extras-0.25.0/test/widget/test_image.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_init_configure.py` & `qtile-extras-0.25.0/test/widget/test_init_configure.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_injection_wrapper.py` & `qtile-extras-0.25.0/test/widget/test_injection_wrapper.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_iwd.py` & `qtile-extras-0.25.0/test/widget/test_iwd.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_livefootballscores.py` & `qtile-extras-0.25.0/test/widget/test_livefootballscores.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_mpris2.py` & `qtile-extras-0.25.0/test/widget/test_mpris2.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_network.py` & `qtile-extras-0.25.0/test/widget/test_network.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_scriptexit.py` & `qtile-extras-0.25.0/test/widget/test_scriptexit.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_snapcast.py` & `qtile-extras-0.25.0/test/widget/test_snapcast.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_statusnotifier.py` & `qtile-extras-0.25.0/test/widget/test_statusnotifier.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_strava.py` & `qtile-extras-0.25.0/test/widget/test_strava.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_syncthing.py` & `qtile-extras-0.25.0/test/widget/test_syncthing.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_tooltip.py` & `qtile-extras-0.25.0/test/widget/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_tvhwidget.py` & `qtile-extras-0.25.0/test/widget/test_tvhwidget.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_unitstatus.py` & `qtile-extras-0.25.0/test/widget/test_unitstatus.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_upower.py` & `qtile-extras-0.25.0/test/widget/test_upower.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_visualiser.py` & `qtile-extras-0.25.0/test/widget/test_visualiser.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_widget_init.py` & `qtile-extras-0.25.0/test/widget/test_widget_init.py`

 * *Files identical despite different names*

### Comparing `qtile-extras-0.24.0/test/widget/test_wordclock.py` & `qtile-extras-0.25.0/test/widget/test_wordclock.py`

 * *Files identical despite different names*

