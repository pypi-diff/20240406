# Comparing `tmp/pygobject-3.48.1.tar.gz` & `tmp/pygobject-3.48.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygobject-3.48.1.tar", last modified: Sun Mar 10 07:49:27 2024, max compression
+gzip compressed data, was "pygobject-3.48.2.tar", last modified: Sat Apr  6 07:19:30 2024, max compression
```

## Comparing `pygobject-3.48.1.tar` & `pygobject-3.48.2.tar`

### file list

```diff
@@ -1,323 +1,323 @@
--rw-rw-rw-   0        0        0       91 2024-03-10 07:33:55.000000 pygobject-3.48.1/.coveragerc
--rw-rw-rw-   0        0        0       77 2024-03-10 07:33:55.000000 pygobject-3.48.1/.flake8
--rw-rw-rw-   0        0        0      262 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitignore
--rw-rw-rw-   0        0        0     1792 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/Dockerfile
--rw-rw-rw-   0        0        0      749 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/Dockerfile.old
--rw-rw-rw-   0        0        0      625 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/README.rst
--rwxrwxrwx   0        0        0      927 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/build-sdists.sh
--rwxrwxrwx   0        0        0      762 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/coverage-docker.sh
--rw-rw-rw-   0        0        0     1204 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/fixup-lcov-paths.py
--rw-rw-rw-   0        0        0      578 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/lcovrc
--rwxrwxrwx   0        0        0      333 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/run-docker-old.sh
--rwxrwxrwx   0        0        0      409 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/run-docker-runtime.sh
--rwxrwxrwx   0        0        0      331 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/run-docker.sh
--rwxrwxrwx   0        0        0      105 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/set_env.sh
--rwxrwxrwx   0        0        0      616 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/test-docker-old.sh
--rwxrwxrwx   0        0        0     1567 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/test-docker.sh
--rwxrwxrwx   0        0        0      882 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/test-flatpak.sh
--rwxrwxrwx   0        0        0     1571 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci/test-msys2.sh
--rw-rw-rw-   0        0        0     3275 2024-03-10 07:33:55.000000 pygobject-3.48.1/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      165 2024-03-10 07:33:55.000000 pygobject-3.48.1/.readthedocs.yaml
--rw-rw-rw-   0        0        0    26440 2024-03-10 07:33:55.000000 pygobject-3.48.1/COPYING
--rw-rw-rw-   0        0        0   182929 2024-03-10 07:33:55.000000 pygobject-3.48.1/NEWS
--rw-rw-rw-   0        0        0      854 2024-03-10 07:33:55.000000 pygobject-3.48.1/PKG-INFO.in
--rw-rw-rw-   0        0        0      792 2024-03-10 07:33:55.000000 pygobject-3.48.1/README.rst
--rw-rw-rw-   0        0        0      387 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/Makefile
--rw-rw-rw-   0        0        0      824 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/bugs_repo.rst
--rw-rw-rw-   0        0        0      316 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/changelog.rst
--rw-rw-rw-   0        0        0     1638 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/conf.py
--rw-rw-rw-   0        0        0     1009 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/contact.rst
--rw-rw-rw-   0        0        0     5505 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/devguide/dev_environ.rst
--rw-rw-rw-   0        0        0      172 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/devguide/index.rst
--rw-rw-rw-   0        0        0     4024 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/devguide/override_guidelines.rst
--rw-rw-rw-   0        0        0      375 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/devguide/overview.rst
--rw-rw-rw-   0        0        0     3688 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/devguide/style_guide.rst
--rw-rw-rw-   0        0        0      977 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/extra.css
--rw-rw-rw-   0        0        0      596 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/further.rst
--rw-rw-rw-   0        0        0     6672 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/getting_started.rst
--rw-rw-rw-   0        0        0     2038 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/api.rst
--rw-rw-rw-   0        0        0     1174 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/basic_types.rst
--rw-rw-rw-   0        0        0     1796 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/error_handling.rst
--rw-rw-rw-   0        0        0     1052 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/flags_enums.rst
--rw-rw-rw-   0        0        0     2224 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/gobject.rst
--rw-rw-rw-   0        0        0      162 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/index.rst
--rw-rw-rw-   0        0        0     3700 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/properties.rst
--rw-rw-rw-   0        0        0     2842 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/signals.rst
--rw-rw-rw-   0        0        0      974 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/api/weakrefs.rst
--rw-rw-rw-   0        0        0     1098 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/cairo_integration.rst
--rwxrwxrwx   0        0        0     3097 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/code/cairo-demo.py
--rw-rw-rw-   0        0        0     2845 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/debug_profile.rst
--rw-rw-rw-   0        0        0     2590 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/deploy.rst
--rw-rw-rw-   0        0        0      483 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/faq.rst
--rw-rw-rw-   0        0        0     2978 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/gtk_template.rst
--rw-rw-rw-   0        0        0    24418 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/images/cairo_integration.png
--rw-rw-rw-   0        0        0      223 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/index.rst
--rw-rw-rw-   0        0        0     3791 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/porting.rst
--rw-rw-rw-   0        0        0      711 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/sysdeps.rst
--rw-rw-rw-   0        0        0      445 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/testing.rst
--rw-rw-rw-   0        0        0    10814 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/guide/threading.rst
--rw-rw-rw-   0        0        0      806 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/icons.rst
--rw-rw-rw-   0        0        0      196 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/LICENSE
--rw-rw-rw-   0        0        0    34494 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/favicon.ico
--rw-rw-rw-   0        0        0     8609 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/logo.svg
--rw-rw-rw-   0        0        0     8499 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/overview-dark.svg
--rw-rw-rw-   0        0        0     1885 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/overview.dia
--rw-rw-rw-   0        0        0     8224 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/overview.svg
--rw-rw-rw-   0        0        0     8777 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/pygobject-small.svg
--rw-rw-rw-   0        0        0    14723 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/pygobject.svg
--rw-rw-rw-   0        0        0     9893 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/start_linux.png
--rw-rw-rw-   0        0        0    13949 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/start_macos.png
--rw-rw-rw-   0        0        0    11454 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/images/start_windows.png
--rw-rw-rw-   0        0        0     5671 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/index.rst
--rw-rw-rw-   0        0        0     1164 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/maintguide.rst
--rw-rw-rw-   0        0        0     1198 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/packagingguide.rst
--rw-rw-rw-   0        0        0       34 2024-03-10 07:33:55.000000 pygobject-3.48.1/docs/requirements.txt
--rwxrwxrwx   0        0        0     2578 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/cairo-demo.py
--rwxrwxrwx   0        0        0    12450 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demo.py
--rw-rw-rw-   0        0        0        0 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Css/__init__.py
--rw-rw-rw-   0        0        0     2678 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Css/css_accordion.py
--rw-rw-rw-   0        0        0     5599 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Css/css_basics.py
--rw-rw-rw-   0        0        0     7128 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Css/css_multiplebgs.py
--rw-rw-rw-   0        0        0        0 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Entry/__init__.py
--rw-rw-rw-   0        0        0     2277 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Entry/entry_buffer.py
--rw-rw-rw-   0        0        0     2655 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Entry/entry_completion.py
--rw-rw-rw-   0        0        0     8983 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/Entry/search_entry.py
--rw-rw-rw-   0        0        0        0 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/IconView/__init__.py
--rw-rw-rw-   0        0        0     7150 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/IconView/iconviewbasics.py
--rw-rw-rw-   0        0        0     3310 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/IconView/iconviewedit.py
--rw-rw-rw-   0        0        0        0 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/TreeView/__init__.py
--rw-rw-rw-   0        0        0     7727 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/TreeView/liststore.py
--rw-rw-rw-   0        0        0     6115 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/TreeView/treemodel_filelist.py
--rw-rw-rw-   0        0        0     8145 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/TreeView/treemodel_filetree.py
--rw-rw-rw-   0        0        0     4372 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/TreeView/treemodel_large.py
--rw-rw-rw-   0        0        0        0 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/__init__.py
--rw-rw-rw-   0        0        0    13908 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/appwindow.py
--rw-rw-rw-   0        0        0     4750 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/assistant.py
--rw-rw-rw-   0        0        0     1865 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/builder.py
--rw-rw-rw-   0        0        0     3664 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/button_box.py
--rw-rw-rw-   0        0        0     8037 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/clipboard.py
--rw-rw-rw-   0        0        0     3558 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/colorselector.py
--rw-rw-rw-   0        0        0    11099 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/combobox.py
--rw-rw-rw-   0        0        0    26529 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/alphatest.png
--rw-rw-rw-   0        0        0     3545 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/apple-red.png
--rw-rw-rw-   0        0        0    22219 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/background.jpg
--rw-rw-rw-   0        0        0     5043 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/brick.png
--rw-rw-rw-   0        0        0    10713 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/brick2.png
--rw-rw-rw-   0        0        0     1334 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/css_accordion.css
--rw-rw-rw-   0        0        0      549 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/css_basics.css
--rw-rw-rw-   0        0        0     5825 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/css_multiplebgs.css
--rw-rw-rw-   0        0        0      908 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/cssview.css
--rw-rw-rw-   0        0        0    31110 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/demo.gresource
--rw-rw-rw-   0        0        0      493 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/demo.gresource.xml
--rw-rw-rw-   0        0        0    12169 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/demo.ui
--rw-rw-rw-   0        0        0     5216 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/floppybuddy.gif
--rw-rw-rw-   0        0        0     3090 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-applets.png
--rw-rw-rw-   0        0        0     2755 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-calendar.png
--rw-rw-rw-   0        0        0     2916 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-foot.png
--rw-rw-rw-   0        0        0     2044 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-fs-directory.png
--rw-rw-rw-   0        0        0     1795 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-fs-regular.png
--rw-rw-rw-   0        0        0     3410 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-gimp.png
--rw-rw-rw-   0        0        0     3244 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-gmush.png
--rw-rw-rw-   0        0        0     4263 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnome-gsame.png
--rw-rw-rw-   0        0        0     3852 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gnu-keys.png
--rw-rw-rw-   0        0        0     6427 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/gtk-logo-rgb.gif
--rw-rw-rw-   0        0        0     1990 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/data/reset.css
--rw-rw-rw-   0        0        0     5434 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/dialogs.py
--rw-rw-rw-   0        0        0     6910 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/drawingarea.py
--rw-rw-rw-   0        0        0     2079 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/expander.py
--rwxrwxrwx   0        0        0    18770 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/flowbox.py
--rw-rw-rw-   0        0        0    11297 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/images.py
--rw-rw-rw-   0        0        0     3918 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/infobars.py
--rw-rw-rw-   0        0        0     2664 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/links.py
--rw-rw-rw-   0        0        0     4704 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/menus.py
--rw-rw-rw-   0        0        0     2686 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/pickers.py
--rw-rw-rw-   0        0        0     6183 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/pixbuf.py
--rw-rw-rw-   0        0        0     6247 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/printing.py
--rw-rw-rw-   0        0        0     6741 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/rotatedtext.py
--rw-rw-rw-   0        0        0      260 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/demo/demos/test.py
--rw-rw-rw-   0        0        0     1009 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/option.py
--rw-rw-rw-   0        0        0      619 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/properties.py
--rw-rw-rw-   0        0        0     1236 2024-03-10 07:33:55.000000 pygobject-3.48.1/examples/signal.py
--rw-rw-rw-   0        0        0     5754 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/__init__.py
--rw-rw-rw-   0        0        0     1969 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_constants.py
--rw-rw-rw-   0        0        0     2082 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_error.py
--rw-rw-rw-   0        0        0    10193 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_gtktemplate.py
--rw-rw-rw-   0        0        0    13714 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_option.py
--rw-rw-rw-   0        0        0     7615 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_ossighelper.py
--rw-rw-rw-   0        0        0    14163 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_propertyhelper.py
--rw-rw-rw-   0        0        0     9303 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/_signalhelper.py
--rw-rw-rw-   0        0        0     6726 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/docstring.py
--rw-rw-rw-   0        0        0    77172 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/gimodule.c
--rw-rw-rw-   0        0        0      602 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/gimodule.h
--rw-rw-rw-   0        0        0     5412 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/importer.py
--rw-rw-rw-   0        0        0     1988 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/meson.build
--rw-rw-rw-   0        0        0     9949 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/module.py
--rw-rw-rw-   0        0        0     2242 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/GIMarshallingTests.py
--rw-rw-rw-   0        0        0    29960 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/GLib.py
--rw-rw-rw-   0        0        0    24215 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/GObject.py
--rw-rw-rw-   0        0        0    17630 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/Gdk.py
--rw-rw-rw-   0        0        0     1724 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/GdkPixbuf.py
--rw-rw-rw-   0        0        0    18777 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/Gio.py
--rw-rw-rw-   0        0        0    62808 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/Gtk.py
--rw-rw-rw-   0        0        0     1774 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/Pango.py
--rw-rw-rw-   0        0        0    12730 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/__init__.py
--rw-rw-rw-   0        0        0     1705 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/keysyms.py
--rw-rw-rw-   0        0        0      259 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/overrides/meson.build
--rw-rw-rw-   0        0        0     7640 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygboxed.c
--rw-rw-rw-   0        0        0     1347 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygboxed.h
--rw-rw-rw-   0        0        0    11403 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygenum.c
--rw-rw-rw-   0        0        0     1706 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygenum.h
--rw-rw-rw-   0        0        0    14985 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygflags.c
--rw-rw-rw-   0        0        0     1764 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygflags.h
--rw-rw-rw-   0        0        0    45784 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-argument.c
--rw-rw-rw-   0        0        0     2706 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-argument.h
--rw-rw-rw-   0        0        0    36014 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-array.c
--rw-rw-rw-   0        0        0     1844 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-array.h
--rw-rw-rw-   0        0        0    34776 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-basictype.c
--rw-rw-rw-   0        0        0     4665 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-basictype.h
--rw-rw-rw-   0        0        0     7014 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-boxed.c
--rw-rw-rw-   0        0        0     1458 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-boxed.h
--rw-rw-rw-   0        0        0    41232 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-cache.c
--rw-rw-rw-   0        0        0    11245 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-cache.h
--rw-rw-rw-   0        0        0     3305 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-ccallback.c
--rw-rw-rw-   0        0        0     1600 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-ccallback.h
--rw-rw-rw-   0        0        0    35381 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-closure.c
--rw-rw-rw-   0        0        0     2176 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-closure.h
--rw-rw-rw-   0        0        0    13728 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-enum-marshal.c
--rw-rw-rw-   0        0        0     1766 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-enum-marshal.h
--rw-rw-rw-   0        0        0    10728 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-error.c
--rw-rw-rw-   0        0        0     1773 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-error.h
--rw-rw-rw-   0        0        0     3091 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-foreign-api.h
--rw-rw-rw-   0        0        0    19799 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-foreign-cairo.c
--rw-rw-rw-   0        0        0     7056 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-foreign.c
--rw-rw-rw-   0        0        0     2688 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-foreign.h
--rw-rw-rw-   0        0        0     8089 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-fundamental.c
--rw-rw-rw-   0        0        0     2067 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-fundamental.h
--rw-rw-rw-   0        0        0    13983 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-hashtable.c
--rw-rw-rw-   0        0        0     1410 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-hashtable.h
--rw-rw-rw-   0        0        0    80798 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-info.c
--rw-rw-rw-   0        0        0     3003 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-info.h
--rw-rw-rw-   0        0        0     1790 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-invoke-state-struct.h
--rw-rw-rw-   0        0        0    30200 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-invoke.c
--rw-rw-rw-   0        0        0     1729 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-invoke.h
--rw-rw-rw-   0        0        0    16430 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-list.c
--rw-rw-rw-   0        0        0     1484 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-list.h
--rw-rw-rw-   0        0        0     9263 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-marshal-cleanup.c
--rw-rw-rw-   0        0        0     2045 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-marshal-cleanup.h
--rw-rw-rw-   0        0        0    15885 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-object.c
--rw-rw-rw-   0        0        0     1802 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-object.h
--rw-rw-rw-   0        0        0    13624 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-property.c
--rw-rw-rw-   0        0        0     1863 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-property.h
--rw-rw-rw-   0        0        0    12750 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-repository.c
--rw-rw-rw-   0        0        0     1218 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-repository.h
--rw-rw-rw-   0        0        0    11465 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-resulttuple.c
--rw-rw-rw-   0        0        0     1165 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-resulttuple.h
--rw-rw-rw-   0        0        0    10540 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-signal-closure.c
--rw-rw-rw-   0        0        0     1837 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-signal-closure.h
--rw-rw-rw-   0        0        0     6624 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-source.c
--rw-rw-rw-   0        0        0     1401 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-source.h
--rw-rw-rw-   0        0        0    23770 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-struct-marshal.c
--rw-rw-rw-   0        0        0     3421 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-struct-marshal.h
--rw-rw-rw-   0        0        0     6929 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-struct.c
--rw-rw-rw-   0        0        0     1466 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-struct.h
--rw-rw-rw-   0        0        0    37505 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-type.c
--rw-rw-rw-   0        0        0     2415 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-type.h
--rw-rw-rw-   0        0        0     3652 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-util.c
--rw-rw-rw-   0        0        0     1895 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-util.h
--rw-rw-rw-   0        0        0    31572 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-value.c
--rw-rw-rw-   0        0        0     2148 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygi-value.h
--rw-rw-rw-   0        0        0     4183 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pyginterface.c
--rw-rw-rw-   0        0        0     1441 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pyginterface.h
--rw-rw-rw-   0        0        0      148 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygobject-internal.h
--rw-rw-rw-   0        0        0    75597 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygobject-object.c
--rw-rw-rw-   0        0        0     1963 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygobject-object.h
--rw-rw-rw-   0        0        0    24983 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygobject.h
--rw-rw-rw-   0        0        0    11605 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygoptioncontext.c
--rw-rw-rw-   0        0        0     1252 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygoptioncontext.h
--rw-rw-rw-   0        0        0     9094 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygoptiongroup.c
--rw-rw-rw-   0        0        0     1399 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygoptiongroup.h
--rw-rw-rw-   0        0        0    16573 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygparamspec.c
--rw-rw-rw-   0        0        0     1176 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygparamspec.h
--rw-rw-rw-   0        0        0     6018 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygpointer.c
--rw-rw-rw-   0        0        0     1314 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygpointer.h
--rw-rw-rw-   0        0        0     8411 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygspawn.c
--rw-rw-rw-   0        0        0     1081 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygspawn.h
--rw-rw-rw-   0        0        0      727 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/pygtkcompat.py
--rw-rw-rw-   0        0        0     1002 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/repository/__init__.py
--rw-rw-rw-   0        0        0      117 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/repository/meson.build
--rw-rw-rw-   0        0        0    13543 2024-03-10 07:33:55.000000 pygobject-3.48.1/gi/types.py
--rw-rw-rw-   0        0        0     6650 2024-03-10 07:33:55.000000 pygobject-3.48.1/meson.build
--rw-rw-rw-   0        0        0      326 2024-03-10 07:33:55.000000 pygobject-3.48.1/meson_options.txt
--rw-rw-rw-   0        0        0      705 2024-03-10 07:33:55.000000 pygobject-3.48.1/pygobject-3.0.pc.in
--rw-rw-rw-   0        0        0     2400 2024-03-10 07:33:55.000000 pygobject-3.48.1/pygobject.doap
--rw-rw-rw-   0        0        0      547 2024-03-10 07:33:55.000000 pygobject-3.48.1/pygtkcompat/__init__.py
--rw-rw-rw-   0        0        0    14383 2024-03-10 07:33:55.000000 pygobject-3.48.1/pygtkcompat/generictreemodel.py
--rw-rw-rw-   0        0        0      148 2024-03-10 07:33:55.000000 pygobject-3.48.1/pygtkcompat/meson.build
--rw-rw-rw-   0        0        0    20826 2024-03-10 07:33:55.000000 pygobject-3.48.1/pygtkcompat/pygtkcompat.py
--rw-r--r--   0        0        0     1536 2024-03-10 07:33:55.000000 pygobject-3.48.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-10 07:33:55.000000 pygobject-3.48.1/subprojects/.gitignore
--rw-rw-rw-   0        0        0      137 2024-03-10 07:33:55.000000 pygobject-3.48.1/subprojects/glib.wrap
--rw-rw-rw-   0        0        0      188 2024-03-10 07:33:55.000000 pygobject-3.48.1/subprojects/gobject-introspection.wrap
--rw-rw-rw-   0        0        0      147 2024-03-10 07:33:55.000000 pygobject-3.48.1/subprojects/libffi.wrap
--rw-rw-rw-   0        0        0       96 2024-03-10 07:33:55.000000 pygobject-3.48.1/subprojects/pycairo.wrap
--rw-rw-rw-   0        0        0     5276 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/conftest.py
--rw-rw-rw-   0        0        0     1007 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/gi/overrides/Regress.py
--rw-rw-rw-   0        0        0       75 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/gi/overrides/__init__.py
--rw-rw-rw-   0        0        0     5584 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/gimarshallingtestsextra.c
--rw-rw-rw-   0        0        0     2390 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/gimarshallingtestsextra.h
--rw-rw-rw-   0        0        0     3697 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/helper.py
--rw-rw-rw-   0        0        0     4392 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/meson.build
--rw-rw-rw-   0        0        0      948 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/org.gnome.test.gschema.xml
--rw-rw-rw-   0        0        0    10985 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/regressextra.c
--rw-rw-rw-   0        0        0     3215 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/regressextra.h
--rw-rw-rw-   0        0        0     3250 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test-floating.c
--rw-rw-rw-   0        0        0     3730 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test-floating.h
--rw-rw-rw-   0        0        0     1554 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test-thread.c
--rw-rw-rw-   0        0        0      847 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test-thread.h
--rw-rw-rw-   0        0        0     2882 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test-unknown.c
--rw-rw-rw-   0        0        0     1509 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test-unknown.h
--rw-rw-rw-   0        0        0     3634 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_atoms.py
--rw-rw-rw-   0        0        0    11911 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_cairo.py
--rw-rw-rw-   0        0        0     5080 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_docstring.py
--rw-rw-rw-   0        0        0     6484 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_error.py
--rw-rw-rw-   0        0        0    56951 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_everything.py
--rw-rw-rw-   0        0        0     5364 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_fields.py
--rw-rw-rw-   0        0        0     4493 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_fundamental.py
--rw-rw-rw-   0        0        0    10385 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_gdbus.py
--rw-rw-rw-   0        0        0    14971 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_generictreemodel.py
--rw-rw-rw-   0        0        0   126524 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_gi.py
--rw-rw-rw-   0        0        0    12688 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_gio.py
--rw-rw-rw-   0        0        0    10884 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_glib.py
--rw-rw-rw-   0        0        0    33702 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_gobject.py
--rw-rw-rw-   0        0        0    19208 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_gtk_template.py
--rw-rw-rw-   0        0        0     4434 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_gtype.py
--rw-rw-rw-   0        0        0     5420 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_import_machinery.py
--rw-rw-rw-   0        0        0     1077 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_interface.py
--rw-rw-rw-   0        0        0     4084 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_internal_api.py
--rw-rw-rw-   0        0        0    16023 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_iochannel.py
--rw-rw-rw-   0        0        0     1841 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_mainloop.py
--rw-rw-rw-   0        0        0    23258 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_object_marshaling.py
--rw-rw-rw-   0        0        0     4551 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_option.py
--rw-rw-rw-   0        0        0     6461 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_ossig.py
--rw-rw-rw-   0        0        0    12301 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_gdk.py
--rw-rw-rw-   0        0        0     1936 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_gdkpixbuf.py
--rw-rw-rw-   0        0        0     9498 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_gio.py
--rw-rw-rw-   0        0        0    27814 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_glib.py
--rw-rw-rw-   0        0        0    10158 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_gobject.py
--rw-rw-rw-   0        0        0   112729 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_gtk.py
--rw-rw-rw-   0        0        0     2291 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_overrides_pango.py
--rw-rw-rw-   0        0        0    53769 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_properties.py
--rw-rw-rw-   0        0        0     1082 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_pycapi.py
--rw-rw-rw-   0        0        0     9991 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_pygtkcompat.py
--rw-rw-rw-   0        0        0    20579 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_repository.py
--rw-rw-rw-   0        0        0     3055 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_resulttuple.py
--rw-rw-rw-   0        0        0    55202 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_signal.py
--rw-rw-rw-   0        0        0    13045 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_source.py
--rw-rw-rw-   0        0        0     6608 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_subprocess.py
--rw-rw-rw-   0        0        0      828 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_thread.py
--rw-rw-rw-   0        0        0     3100 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_typeclass.py
--rw-rw-rw-   0        0        0      893 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/test_unknown.py
--rw-rw-rw-   0        0        0    22527 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/testhelpermodule.c
--rw-rw-rw-   0        0        0      496 2024-03-10 07:33:55.000000 pygobject-3.48.1/tests/valgrind.supp
--rwxrwxrwx   0        0        0    21387 2024-03-10 07:33:55.000000 pygobject-3.48.1/tools/pygi-convert.sh
--rw-r--r--   0        0        0     1286 2024-03-10 07:49:27.695437 pygobject-3.48.1/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2024-04-06 07:08:23.000000 pygobject-3.48.2/.coveragerc
+-rw-rw-rw-   0        0        0       77 2024-04-06 07:08:23.000000 pygobject-3.48.2/.flake8
+-rw-rw-rw-   0        0        0      262 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitignore
+-rw-rw-rw-   0        0        0     1792 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/Dockerfile
+-rw-rw-rw-   0        0        0      749 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/Dockerfile.old
+-rw-rw-rw-   0        0        0      625 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/README.rst
+-rwxrwxrwx   0        0        0      927 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/build-sdists.sh
+-rwxrwxrwx   0        0        0      762 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/coverage-docker.sh
+-rw-rw-rw-   0        0        0     1204 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/fixup-lcov-paths.py
+-rw-rw-rw-   0        0        0      578 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/lcovrc
+-rwxrwxrwx   0        0        0      333 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/run-docker-old.sh
+-rwxrwxrwx   0        0        0      409 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/run-docker-runtime.sh
+-rwxrwxrwx   0        0        0      331 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/run-docker.sh
+-rwxrwxrwx   0        0        0      105 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/set_env.sh
+-rwxrwxrwx   0        0        0      616 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/test-docker-old.sh
+-rwxrwxrwx   0        0        0     1567 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/test-docker.sh
+-rwxrwxrwx   0        0        0      882 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/test-flatpak.sh
+-rwxrwxrwx   0        0        0     1571 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci/test-msys2.sh
+-rw-rw-rw-   0        0        0     3275 2024-04-06 07:08:23.000000 pygobject-3.48.2/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      165 2024-04-06 07:08:23.000000 pygobject-3.48.2/.readthedocs.yaml
+-rw-rw-rw-   0        0        0    26440 2024-04-06 07:08:23.000000 pygobject-3.48.2/COPYING
+-rw-rw-rw-   0        0        0   183065 2024-04-06 07:08:23.000000 pygobject-3.48.2/NEWS
+-rw-rw-rw-   0        0        0      854 2024-04-06 07:08:23.000000 pygobject-3.48.2/PKG-INFO.in
+-rw-rw-rw-   0        0        0      792 2024-04-06 07:08:23.000000 pygobject-3.48.2/README.rst
+-rw-rw-rw-   0        0        0      387 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/Makefile
+-rw-rw-rw-   0        0        0      824 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/bugs_repo.rst
+-rw-rw-rw-   0        0        0      316 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1638 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/conf.py
+-rw-rw-rw-   0        0        0     1009 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/contact.rst
+-rw-rw-rw-   0        0        0     5505 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/devguide/dev_environ.rst
+-rw-rw-rw-   0        0        0      172 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/devguide/index.rst
+-rw-rw-rw-   0        0        0     4024 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/devguide/override_guidelines.rst
+-rw-rw-rw-   0        0        0      375 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/devguide/overview.rst
+-rw-rw-rw-   0        0        0     3688 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/devguide/style_guide.rst
+-rw-rw-rw-   0        0        0      977 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/extra.css
+-rw-rw-rw-   0        0        0      596 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/further.rst
+-rw-rw-rw-   0        0        0     6672 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/getting_started.rst
+-rw-rw-rw-   0        0        0     2038 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/api.rst
+-rw-rw-rw-   0        0        0     1174 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/basic_types.rst
+-rw-rw-rw-   0        0        0     1796 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/error_handling.rst
+-rw-rw-rw-   0        0        0     1052 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/flags_enums.rst
+-rw-rw-rw-   0        0        0     2224 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/gobject.rst
+-rw-rw-rw-   0        0        0      162 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/index.rst
+-rw-rw-rw-   0        0        0     3700 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/properties.rst
+-rw-rw-rw-   0        0        0     2842 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/signals.rst
+-rw-rw-rw-   0        0        0      974 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/api/weakrefs.rst
+-rw-rw-rw-   0        0        0     1098 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/cairo_integration.rst
+-rwxrwxrwx   0        0        0     3097 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/code/cairo-demo.py
+-rw-rw-rw-   0        0        0     2845 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/debug_profile.rst
+-rw-rw-rw-   0        0        0     2590 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/deploy.rst
+-rw-rw-rw-   0        0        0      483 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/faq.rst
+-rw-rw-rw-   0        0        0     2978 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/gtk_template.rst
+-rw-rw-rw-   0        0        0    24418 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/images/cairo_integration.png
+-rw-rw-rw-   0        0        0      223 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/index.rst
+-rw-rw-rw-   0        0        0     3791 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/porting.rst
+-rw-rw-rw-   0        0        0      711 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/sysdeps.rst
+-rw-rw-rw-   0        0        0      445 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/testing.rst
+-rw-rw-rw-   0        0        0    10814 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/guide/threading.rst
+-rw-rw-rw-   0        0        0      806 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/icons.rst
+-rw-rw-rw-   0        0        0      196 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/LICENSE
+-rw-rw-rw-   0        0        0    34494 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/favicon.ico
+-rw-rw-rw-   0        0        0     8609 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/logo.svg
+-rw-rw-rw-   0        0        0     8499 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/overview-dark.svg
+-rw-rw-rw-   0        0        0     1885 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/overview.dia
+-rw-rw-rw-   0        0        0     8224 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/overview.svg
+-rw-rw-rw-   0        0        0     8777 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/pygobject-small.svg
+-rw-rw-rw-   0        0        0    14723 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/pygobject.svg
+-rw-rw-rw-   0        0        0     9893 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/start_linux.png
+-rw-rw-rw-   0        0        0    13949 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/start_macos.png
+-rw-rw-rw-   0        0        0    11454 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/images/start_windows.png
+-rw-rw-rw-   0        0        0     5671 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1164 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/maintguide.rst
+-rw-rw-rw-   0        0        0     1198 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/packagingguide.rst
+-rw-rw-rw-   0        0        0       34 2024-04-06 07:08:23.000000 pygobject-3.48.2/docs/requirements.txt
+-rwxrwxrwx   0        0        0     2578 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/cairo-demo.py
+-rwxrwxrwx   0        0        0    12450 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demo.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Css/__init__.py
+-rw-rw-rw-   0        0        0     2678 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Css/css_accordion.py
+-rw-rw-rw-   0        0        0     5599 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Css/css_basics.py
+-rw-rw-rw-   0        0        0     7128 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Css/css_multiplebgs.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Entry/__init__.py
+-rw-rw-rw-   0        0        0     2277 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Entry/entry_buffer.py
+-rw-rw-rw-   0        0        0     2655 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Entry/entry_completion.py
+-rw-rw-rw-   0        0        0     8983 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/Entry/search_entry.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/IconView/__init__.py
+-rw-rw-rw-   0        0        0     7150 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/IconView/iconviewbasics.py
+-rw-rw-rw-   0        0        0     3310 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/IconView/iconviewedit.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/TreeView/__init__.py
+-rw-rw-rw-   0        0        0     7727 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/TreeView/liststore.py
+-rw-rw-rw-   0        0        0     6115 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/TreeView/treemodel_filelist.py
+-rw-rw-rw-   0        0        0     8145 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/TreeView/treemodel_filetree.py
+-rw-rw-rw-   0        0        0     4372 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/TreeView/treemodel_large.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/__init__.py
+-rw-rw-rw-   0        0        0    13908 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/appwindow.py
+-rw-rw-rw-   0        0        0     4750 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/assistant.py
+-rw-rw-rw-   0        0        0     1865 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/builder.py
+-rw-rw-rw-   0        0        0     3664 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/button_box.py
+-rw-rw-rw-   0        0        0     8037 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/clipboard.py
+-rw-rw-rw-   0        0        0     3558 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/colorselector.py
+-rw-rw-rw-   0        0        0    11099 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/combobox.py
+-rw-rw-rw-   0        0        0    26529 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/alphatest.png
+-rw-rw-rw-   0        0        0     3545 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/apple-red.png
+-rw-rw-rw-   0        0        0    22219 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/background.jpg
+-rw-rw-rw-   0        0        0     5043 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/brick.png
+-rw-rw-rw-   0        0        0    10713 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/brick2.png
+-rw-rw-rw-   0        0        0     1334 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/css_accordion.css
+-rw-rw-rw-   0        0        0      549 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/css_basics.css
+-rw-rw-rw-   0        0        0     5825 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/css_multiplebgs.css
+-rw-rw-rw-   0        0        0      908 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/cssview.css
+-rw-rw-rw-   0        0        0    31110 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/demo.gresource
+-rw-rw-rw-   0        0        0      493 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/demo.gresource.xml
+-rw-rw-rw-   0        0        0    12169 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/demo.ui
+-rw-rw-rw-   0        0        0     5216 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/floppybuddy.gif
+-rw-rw-rw-   0        0        0     3090 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-applets.png
+-rw-rw-rw-   0        0        0     2755 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-calendar.png
+-rw-rw-rw-   0        0        0     2916 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-foot.png
+-rw-rw-rw-   0        0        0     2044 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-fs-directory.png
+-rw-rw-rw-   0        0        0     1795 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-fs-regular.png
+-rw-rw-rw-   0        0        0     3410 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-gimp.png
+-rw-rw-rw-   0        0        0     3244 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-gmush.png
+-rw-rw-rw-   0        0        0     4263 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnome-gsame.png
+-rw-rw-rw-   0        0        0     3852 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gnu-keys.png
+-rw-rw-rw-   0        0        0     6427 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/gtk-logo-rgb.gif
+-rw-rw-rw-   0        0        0     1990 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/data/reset.css
+-rw-rw-rw-   0        0        0     5434 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/dialogs.py
+-rw-rw-rw-   0        0        0     6910 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/drawingarea.py
+-rw-rw-rw-   0        0        0     2079 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/expander.py
+-rwxrwxrwx   0        0        0    18770 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/flowbox.py
+-rw-rw-rw-   0        0        0    11297 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/images.py
+-rw-rw-rw-   0        0        0     3918 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/infobars.py
+-rw-rw-rw-   0        0        0     2664 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/links.py
+-rw-rw-rw-   0        0        0     4704 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/menus.py
+-rw-rw-rw-   0        0        0     2686 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/pickers.py
+-rw-rw-rw-   0        0        0     6183 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/pixbuf.py
+-rw-rw-rw-   0        0        0     6247 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/printing.py
+-rw-rw-rw-   0        0        0     6741 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/rotatedtext.py
+-rw-rw-rw-   0        0        0      260 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/demo/demos/test.py
+-rw-rw-rw-   0        0        0     1009 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/option.py
+-rw-rw-rw-   0        0        0      619 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/properties.py
+-rw-rw-rw-   0        0        0     1236 2024-04-06 07:08:23.000000 pygobject-3.48.2/examples/signal.py
+-rw-rw-rw-   0        0        0     5754 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/__init__.py
+-rw-rw-rw-   0        0        0     1969 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_constants.py
+-rw-rw-rw-   0        0        0     2082 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_error.py
+-rw-rw-rw-   0        0        0    10193 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_gtktemplate.py
+-rw-rw-rw-   0        0        0    13714 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_option.py
+-rw-rw-rw-   0        0        0     7615 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_ossighelper.py
+-rw-rw-rw-   0        0        0    14163 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_propertyhelper.py
+-rw-rw-rw-   0        0        0     9303 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/_signalhelper.py
+-rw-rw-rw-   0        0        0     6726 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/docstring.py
+-rw-rw-rw-   0        0        0    77172 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/gimodule.c
+-rw-rw-rw-   0        0        0      602 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/gimodule.h
+-rw-rw-rw-   0        0        0     5412 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/importer.py
+-rw-rw-rw-   0        0        0     1988 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/meson.build
+-rw-rw-rw-   0        0        0     9979 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/module.py
+-rw-rw-rw-   0        0        0     2242 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/GIMarshallingTests.py
+-rw-rw-rw-   0        0        0    29960 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/GLib.py
+-rw-rw-rw-   0        0        0    24215 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/GObject.py
+-rw-rw-rw-   0        0        0    17630 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/Gdk.py
+-rw-rw-rw-   0        0        0     1724 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/GdkPixbuf.py
+-rw-rw-rw-   0        0        0    18777 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/Gio.py
+-rw-rw-rw-   0        0        0    62808 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/Gtk.py
+-rw-rw-rw-   0        0        0     1774 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/Pango.py
+-rw-rw-rw-   0        0        0    12730 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/__init__.py
+-rw-rw-rw-   0        0        0     1705 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/keysyms.py
+-rw-rw-rw-   0        0        0      259 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/overrides/meson.build
+-rw-rw-rw-   0        0        0     7640 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygboxed.c
+-rw-rw-rw-   0        0        0     1347 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygboxed.h
+-rw-rw-rw-   0        0        0    11403 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygenum.c
+-rw-rw-rw-   0        0        0     1706 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygenum.h
+-rw-rw-rw-   0        0        0    14985 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygflags.c
+-rw-rw-rw-   0        0        0     1764 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygflags.h
+-rw-rw-rw-   0        0        0    45784 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-argument.c
+-rw-rw-rw-   0        0        0     2706 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-argument.h
+-rw-rw-rw-   0        0        0    36014 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-array.c
+-rw-rw-rw-   0        0        0     1844 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-array.h
+-rw-rw-rw-   0        0        0    34776 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-basictype.c
+-rw-rw-rw-   0        0        0     4665 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-basictype.h
+-rw-rw-rw-   0        0        0     7014 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-boxed.c
+-rw-rw-rw-   0        0        0     1458 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-boxed.h
+-rw-rw-rw-   0        0        0    41232 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-cache.c
+-rw-rw-rw-   0        0        0    11245 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-cache.h
+-rw-rw-rw-   0        0        0     3305 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-ccallback.c
+-rw-rw-rw-   0        0        0     1600 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-ccallback.h
+-rw-rw-rw-   0        0        0    35381 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-closure.c
+-rw-rw-rw-   0        0        0     2176 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-closure.h
+-rw-rw-rw-   0        0        0    13728 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-enum-marshal.c
+-rw-rw-rw-   0        0        0     1766 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-enum-marshal.h
+-rw-rw-rw-   0        0        0    10728 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-error.c
+-rw-rw-rw-   0        0        0     1773 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-error.h
+-rw-rw-rw-   0        0        0     3091 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-foreign-api.h
+-rw-rw-rw-   0        0        0    19799 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-foreign-cairo.c
+-rw-rw-rw-   0        0        0     7056 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-foreign.c
+-rw-rw-rw-   0        0        0     2688 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-foreign.h
+-rw-rw-rw-   0        0        0     8314 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-fundamental.c
+-rw-rw-rw-   0        0        0     2067 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-fundamental.h
+-rw-rw-rw-   0        0        0    13983 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-hashtable.c
+-rw-rw-rw-   0        0        0     1410 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-hashtable.h
+-rw-rw-rw-   0        0        0    80798 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-info.c
+-rw-rw-rw-   0        0        0     3003 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-info.h
+-rw-rw-rw-   0        0        0     1790 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-invoke-state-struct.h
+-rw-rw-rw-   0        0        0    30200 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-invoke.c
+-rw-rw-rw-   0        0        0     1729 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-invoke.h
+-rw-rw-rw-   0        0        0    16430 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-list.c
+-rw-rw-rw-   0        0        0     1484 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-list.h
+-rw-rw-rw-   0        0        0     9263 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-marshal-cleanup.c
+-rw-rw-rw-   0        0        0     2045 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-marshal-cleanup.h
+-rw-rw-rw-   0        0        0    15885 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-object.c
+-rw-rw-rw-   0        0        0     1802 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-object.h
+-rw-rw-rw-   0        0        0    13624 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-property.c
+-rw-rw-rw-   0        0        0     1863 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-property.h
+-rw-rw-rw-   0        0        0    12750 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-repository.c
+-rw-rw-rw-   0        0        0     1218 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-repository.h
+-rw-rw-rw-   0        0        0    11465 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-resulttuple.c
+-rw-rw-rw-   0        0        0     1165 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-resulttuple.h
+-rw-rw-rw-   0        0        0    10540 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-signal-closure.c
+-rw-rw-rw-   0        0        0     1837 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-signal-closure.h
+-rw-rw-rw-   0        0        0     6624 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-source.c
+-rw-rw-rw-   0        0        0     1401 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-source.h
+-rw-rw-rw-   0        0        0    23770 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-struct-marshal.c
+-rw-rw-rw-   0        0        0     3421 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-struct-marshal.h
+-rw-rw-rw-   0        0        0     6929 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-struct.c
+-rw-rw-rw-   0        0        0     1466 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-struct.h
+-rw-rw-rw-   0        0        0    37505 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-type.c
+-rw-rw-rw-   0        0        0     2415 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-type.h
+-rw-rw-rw-   0        0        0     3652 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-util.c
+-rw-rw-rw-   0        0        0     1895 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-util.h
+-rw-rw-rw-   0        0        0    31572 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-value.c
+-rw-rw-rw-   0        0        0     2148 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygi-value.h
+-rw-rw-rw-   0        0        0     4183 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pyginterface.c
+-rw-rw-rw-   0        0        0     1441 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pyginterface.h
+-rw-rw-rw-   0        0        0      148 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygobject-internal.h
+-rw-rw-rw-   0        0        0    75597 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygobject-object.c
+-rw-rw-rw-   0        0        0     1963 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygobject-object.h
+-rw-rw-rw-   0        0        0    24983 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygobject.h
+-rw-rw-rw-   0        0        0    11605 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygoptioncontext.c
+-rw-rw-rw-   0        0        0     1252 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygoptioncontext.h
+-rw-rw-rw-   0        0        0     9094 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygoptiongroup.c
+-rw-rw-rw-   0        0        0     1399 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygoptiongroup.h
+-rw-rw-rw-   0        0        0    16573 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygparamspec.c
+-rw-rw-rw-   0        0        0     1176 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygparamspec.h
+-rw-rw-rw-   0        0        0     6018 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygpointer.c
+-rw-rw-rw-   0        0        0     1314 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygpointer.h
+-rw-rw-rw-   0        0        0     8411 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygspawn.c
+-rw-rw-rw-   0        0        0     1081 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygspawn.h
+-rw-rw-rw-   0        0        0      727 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/pygtkcompat.py
+-rw-rw-rw-   0        0        0     1002 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/repository/__init__.py
+-rw-rw-rw-   0        0        0      117 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/repository/meson.build
+-rw-rw-rw-   0        0        0    13543 2024-04-06 07:08:23.000000 pygobject-3.48.2/gi/types.py
+-rw-rw-rw-   0        0        0     6650 2024-04-06 07:08:23.000000 pygobject-3.48.2/meson.build
+-rw-rw-rw-   0        0        0      326 2024-04-06 07:08:23.000000 pygobject-3.48.2/meson_options.txt
+-rw-rw-rw-   0        0        0      705 2024-04-06 07:08:23.000000 pygobject-3.48.2/pygobject-3.0.pc.in
+-rw-rw-rw-   0        0        0     2400 2024-04-06 07:08:23.000000 pygobject-3.48.2/pygobject.doap
+-rw-rw-rw-   0        0        0      547 2024-04-06 07:08:23.000000 pygobject-3.48.2/pygtkcompat/__init__.py
+-rw-rw-rw-   0        0        0    14383 2024-04-06 07:08:23.000000 pygobject-3.48.2/pygtkcompat/generictreemodel.py
+-rw-rw-rw-   0        0        0      148 2024-04-06 07:08:23.000000 pygobject-3.48.2/pygtkcompat/meson.build
+-rw-rw-rw-   0        0        0    20826 2024-04-06 07:08:23.000000 pygobject-3.48.2/pygtkcompat/pygtkcompat.py
+-rw-r--r--   0        0        0     1536 2024-04-06 07:08:23.000000 pygobject-3.48.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 07:08:23.000000 pygobject-3.48.2/subprojects/.gitignore
+-rw-rw-rw-   0        0        0      137 2024-04-06 07:08:23.000000 pygobject-3.48.2/subprojects/glib.wrap
+-rw-rw-rw-   0        0        0      188 2024-04-06 07:08:23.000000 pygobject-3.48.2/subprojects/gobject-introspection.wrap
+-rw-rw-rw-   0        0        0      147 2024-04-06 07:08:23.000000 pygobject-3.48.2/subprojects/libffi.wrap
+-rw-rw-rw-   0        0        0       96 2024-04-06 07:08:23.000000 pygobject-3.48.2/subprojects/pycairo.wrap
+-rw-rw-rw-   0        0        0     5276 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/conftest.py
+-rw-rw-rw-   0        0        0     1461 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/gi/overrides/Regress.py
+-rw-rw-rw-   0        0        0       75 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/gi/overrides/__init__.py
+-rw-rw-rw-   0        0        0     5584 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/gimarshallingtestsextra.c
+-rw-rw-rw-   0        0        0     2390 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/gimarshallingtestsextra.h
+-rw-rw-rw-   0        0        0     3697 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/helper.py
+-rw-rw-rw-   0        0        0     4392 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/meson.build
+-rw-rw-rw-   0        0        0      948 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/org.gnome.test.gschema.xml
+-rw-rw-rw-   0        0        0    12572 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/regressextra.c
+-rw-rw-rw-   0        0        0     3650 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/regressextra.h
+-rw-rw-rw-   0        0        0     3250 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test-floating.c
+-rw-rw-rw-   0        0        0     3730 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test-floating.h
+-rw-rw-rw-   0        0        0     1554 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test-thread.c
+-rw-rw-rw-   0        0        0      847 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test-thread.h
+-rw-rw-rw-   0        0        0     2882 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test-unknown.c
+-rw-rw-rw-   0        0        0     1509 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test-unknown.h
+-rw-rw-rw-   0        0        0     3634 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_atoms.py
+-rw-rw-rw-   0        0        0    11911 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_cairo.py
+-rw-rw-rw-   0        0        0     5080 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_docstring.py
+-rw-rw-rw-   0        0        0     6484 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_error.py
+-rw-rw-rw-   0        0        0    56951 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_everything.py
+-rw-rw-rw-   0        0        0     5364 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_fields.py
+-rw-rw-rw-   0        0        0     4596 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_fundamental.py
+-rw-rw-rw-   0        0        0    10385 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_gdbus.py
+-rw-rw-rw-   0        0        0    14971 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_generictreemodel.py
+-rw-rw-rw-   0        0        0   126524 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_gi.py
+-rw-rw-rw-   0        0        0    12688 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_gio.py
+-rw-rw-rw-   0        0        0    10884 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_glib.py
+-rw-rw-rw-   0        0        0    33702 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_gobject.py
+-rw-rw-rw-   0        0        0    19208 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_gtk_template.py
+-rw-rw-rw-   0        0        0     4434 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_gtype.py
+-rw-rw-rw-   0        0        0     5420 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_import_machinery.py
+-rw-rw-rw-   0        0        0     1077 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_interface.py
+-rw-rw-rw-   0        0        0     4084 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_internal_api.py
+-rw-rw-rw-   0        0        0    16023 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_iochannel.py
+-rw-rw-rw-   0        0        0     1841 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_mainloop.py
+-rw-rw-rw-   0        0        0    23258 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_object_marshaling.py
+-rw-rw-rw-   0        0        0     4551 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_option.py
+-rw-rw-rw-   0        0        0     6461 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_ossig.py
+-rw-rw-rw-   0        0        0    12301 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_gdk.py
+-rw-rw-rw-   0        0        0     1936 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_gdkpixbuf.py
+-rw-rw-rw-   0        0        0     9498 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_gio.py
+-rw-rw-rw-   0        0        0    27814 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_glib.py
+-rw-rw-rw-   0        0        0    10158 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_gobject.py
+-rw-rw-rw-   0        0        0   112729 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_gtk.py
+-rw-rw-rw-   0        0        0     2291 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_overrides_pango.py
+-rw-rw-rw-   0        0        0    53769 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_properties.py
+-rw-rw-rw-   0        0        0     1082 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_pycapi.py
+-rw-rw-rw-   0        0        0     9991 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_pygtkcompat.py
+-rw-rw-rw-   0        0        0    20579 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_repository.py
+-rw-rw-rw-   0        0        0     3055 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_resulttuple.py
+-rw-rw-rw-   0        0        0    55202 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_signal.py
+-rw-rw-rw-   0        0        0    13045 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_source.py
+-rw-rw-rw-   0        0        0     6608 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0      828 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_thread.py
+-rw-rw-rw-   0        0        0     3100 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_typeclass.py
+-rw-rw-rw-   0        0        0      893 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/test_unknown.py
+-rw-rw-rw-   0        0        0    22527 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/testhelpermodule.c
+-rw-rw-rw-   0        0        0      496 2024-04-06 07:08:23.000000 pygobject-3.48.2/tests/valgrind.supp
+-rwxrwxrwx   0        0        0    21387 2024-04-06 07:08:23.000000 pygobject-3.48.2/tools/pygi-convert.sh
+-rw-r--r--   0        0        0     1286 2024-04-06 07:19:31.548129 pygobject-3.48.2/PKG-INFO
```

### Comparing `pygobject-3.48.1/.gitlab-ci/Dockerfile` & `pygobject-3.48.2/.gitlab-ci/Dockerfile`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/Dockerfile.old` & `pygobject-3.48.2/.gitlab-ci/Dockerfile.old`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/README.rst` & `pygobject-3.48.2/.gitlab-ci/README.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/build-sdists.sh` & `pygobject-3.48.2/.gitlab-ci/build-sdists.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/coverage-docker.sh` & `pygobject-3.48.2/.gitlab-ci/coverage-docker.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/fixup-lcov-paths.py` & `pygobject-3.48.2/.gitlab-ci/fixup-lcov-paths.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/lcovrc` & `pygobject-3.48.2/.gitlab-ci/lcovrc`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/test-docker-old.sh` & `pygobject-3.48.2/.gitlab-ci/test-docker-old.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/test-docker.sh` & `pygobject-3.48.2/.gitlab-ci/test-docker.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/test-flatpak.sh` & `pygobject-3.48.2/.gitlab-ci/test-flatpak.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci/test-msys2.sh` & `pygobject-3.48.2/.gitlab-ci/test-msys2.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/.gitlab-ci.yml` & `pygobject-3.48.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/COPYING` & `pygobject-3.48.2/COPYING`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/NEWS` & `pygobject-3.48.2/NEWS`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+3.48.2 - 2024-04-06
+-------------------
+
+* Fix support for fundamental (primitive) types, such as Gst.Bitmask
+  :issue:`624` :mr:`304`
+
 3.48.1 - 2024-03-10
 -------------------
 
 * Fix installation with pip failing in some environments with
   ModuleNotFoundError in g-ir-scanner :issue:`622` :mr:`302`
 
 3.48.0 - 2024-03-09
```

### Comparing `pygobject-3.48.1/PKG-INFO.in` & `pygobject-3.48.2/PKG-INFO.in`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/README.rst` & `pygobject-3.48.2/README.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/bugs_repo.rst` & `pygobject-3.48.2/docs/bugs_repo.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/conf.py` & `pygobject-3.48.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/contact.rst` & `pygobject-3.48.2/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/devguide/dev_environ.rst` & `pygobject-3.48.2/docs/devguide/dev_environ.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/devguide/override_guidelines.rst` & `pygobject-3.48.2/docs/devguide/override_guidelines.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/devguide/style_guide.rst` & `pygobject-3.48.2/docs/devguide/style_guide.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/extra.css` & `pygobject-3.48.2/docs/extra.css`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/further.rst` & `pygobject-3.48.2/docs/further.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/getting_started.rst` & `pygobject-3.48.2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/api.rst` & `pygobject-3.48.2/docs/guide/api/api.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/basic_types.rst` & `pygobject-3.48.2/docs/guide/api/basic_types.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/error_handling.rst` & `pygobject-3.48.2/docs/guide/api/error_handling.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/flags_enums.rst` & `pygobject-3.48.2/docs/guide/api/flags_enums.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/gobject.rst` & `pygobject-3.48.2/docs/guide/api/gobject.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/properties.rst` & `pygobject-3.48.2/docs/guide/api/properties.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/signals.rst` & `pygobject-3.48.2/docs/guide/api/signals.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/api/weakrefs.rst` & `pygobject-3.48.2/docs/guide/api/weakrefs.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/cairo_integration.rst` & `pygobject-3.48.2/docs/guide/cairo_integration.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/code/cairo-demo.py` & `pygobject-3.48.2/docs/guide/code/cairo-demo.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/debug_profile.rst` & `pygobject-3.48.2/docs/guide/debug_profile.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/deploy.rst` & `pygobject-3.48.2/docs/guide/deploy.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/gtk_template.rst` & `pygobject-3.48.2/docs/guide/gtk_template.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/images/cairo_integration.png` & `pygobject-3.48.2/docs/guide/images/cairo_integration.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/porting.rst` & `pygobject-3.48.2/docs/guide/porting.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/sysdeps.rst` & `pygobject-3.48.2/docs/guide/sysdeps.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/guide/threading.rst` & `pygobject-3.48.2/docs/guide/threading.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/icons.rst` & `pygobject-3.48.2/docs/icons.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/favicon.ico` & `pygobject-3.48.2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/logo.svg` & `pygobject-3.48.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/overview-dark.svg` & `pygobject-3.48.2/docs/images/overview-dark.svg`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/overview.dia` & `pygobject-3.48.2/docs/images/overview.dia`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/overview.svg` & `pygobject-3.48.2/docs/images/overview.svg`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/pygobject-small.svg` & `pygobject-3.48.2/docs/images/pygobject-small.svg`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/pygobject.svg` & `pygobject-3.48.2/docs/images/pygobject.svg`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/start_linux.png` & `pygobject-3.48.2/docs/images/start_linux.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/start_macos.png` & `pygobject-3.48.2/docs/images/start_macos.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/images/start_windows.png` & `pygobject-3.48.2/docs/images/start_windows.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/index.rst` & `pygobject-3.48.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/maintguide.rst` & `pygobject-3.48.2/docs/maintguide.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/docs/packagingguide.rst` & `pygobject-3.48.2/docs/packagingguide.rst`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/cairo-demo.py` & `pygobject-3.48.2/examples/cairo-demo.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demo.py` & `pygobject-3.48.2/examples/demo/demo.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/Css/css_accordion.py` & `pygobject-3.48.2/examples/demo/demos/Css/css_accordion.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/Css/css_basics.py` & `pygobject-3.48.2/examples/demo/demos/Css/css_basics.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/Css/css_multiplebgs.py` & `pygobject-3.48.2/examples/demo/demos/Css/css_multiplebgs.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/Entry/entry_buffer.py` & `pygobject-3.48.2/examples/demo/demos/Entry/entry_buffer.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/Entry/entry_completion.py` & `pygobject-3.48.2/examples/demo/demos/Entry/entry_completion.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/Entry/search_entry.py` & `pygobject-3.48.2/examples/demo/demos/Entry/search_entry.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/IconView/iconviewbasics.py` & `pygobject-3.48.2/examples/demo/demos/IconView/iconviewbasics.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/IconView/iconviewedit.py` & `pygobject-3.48.2/examples/demo/demos/IconView/iconviewedit.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/TreeView/liststore.py` & `pygobject-3.48.2/examples/demo/demos/TreeView/liststore.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/TreeView/treemodel_filelist.py` & `pygobject-3.48.2/examples/demo/demos/TreeView/treemodel_filelist.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/TreeView/treemodel_filetree.py` & `pygobject-3.48.2/examples/demo/demos/TreeView/treemodel_filetree.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/TreeView/treemodel_large.py` & `pygobject-3.48.2/examples/demo/demos/TreeView/treemodel_large.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/appwindow.py` & `pygobject-3.48.2/examples/demo/demos/appwindow.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/assistant.py` & `pygobject-3.48.2/examples/demo/demos/assistant.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/builder.py` & `pygobject-3.48.2/examples/demo/demos/builder.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/button_box.py` & `pygobject-3.48.2/examples/demo/demos/button_box.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/clipboard.py` & `pygobject-3.48.2/examples/demo/demos/clipboard.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/colorselector.py` & `pygobject-3.48.2/examples/demo/demos/colorselector.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/combobox.py` & `pygobject-3.48.2/examples/demo/demos/combobox.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/alphatest.png` & `pygobject-3.48.2/examples/demo/demos/data/alphatest.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/apple-red.png` & `pygobject-3.48.2/examples/demo/demos/data/apple-red.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/background.jpg` & `pygobject-3.48.2/examples/demo/demos/data/background.jpg`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/brick.png` & `pygobject-3.48.2/examples/demo/demos/data/brick.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/brick2.png` & `pygobject-3.48.2/examples/demo/demos/data/brick2.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/css_accordion.css` & `pygobject-3.48.2/examples/demo/demos/data/css_accordion.css`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/css_basics.css` & `pygobject-3.48.2/examples/demo/demos/data/css_basics.css`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/css_multiplebgs.css` & `pygobject-3.48.2/examples/demo/demos/data/css_multiplebgs.css`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/cssview.css` & `pygobject-3.48.2/examples/demo/demos/data/cssview.css`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/demo.gresource` & `pygobject-3.48.2/examples/demo/demos/data/demo.gresource`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/demo.ui` & `pygobject-3.48.2/examples/demo/demos/data/demo.ui`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/floppybuddy.gif` & `pygobject-3.48.2/examples/demo/demos/data/floppybuddy.gif`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-applets.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-applets.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-calendar.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-calendar.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-foot.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-foot.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-fs-directory.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-fs-directory.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-fs-regular.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-fs-regular.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-gimp.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-gimp.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-gmush.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-gmush.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnome-gsame.png` & `pygobject-3.48.2/examples/demo/demos/data/gnome-gsame.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gnu-keys.png` & `pygobject-3.48.2/examples/demo/demos/data/gnu-keys.png`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/gtk-logo-rgb.gif` & `pygobject-3.48.2/examples/demo/demos/data/gtk-logo-rgb.gif`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/data/reset.css` & `pygobject-3.48.2/examples/demo/demos/data/reset.css`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/dialogs.py` & `pygobject-3.48.2/examples/demo/demos/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/drawingarea.py` & `pygobject-3.48.2/examples/demo/demos/drawingarea.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/expander.py` & `pygobject-3.48.2/examples/demo/demos/expander.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/flowbox.py` & `pygobject-3.48.2/examples/demo/demos/flowbox.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/images.py` & `pygobject-3.48.2/examples/demo/demos/images.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/infobars.py` & `pygobject-3.48.2/examples/demo/demos/infobars.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/links.py` & `pygobject-3.48.2/examples/demo/demos/links.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/menus.py` & `pygobject-3.48.2/examples/demo/demos/menus.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/pickers.py` & `pygobject-3.48.2/examples/demo/demos/pickers.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/pixbuf.py` & `pygobject-3.48.2/examples/demo/demos/pixbuf.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/printing.py` & `pygobject-3.48.2/examples/demo/demos/printing.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/demo/demos/rotatedtext.py` & `pygobject-3.48.2/examples/demo/demos/rotatedtext.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/option.py` & `pygobject-3.48.2/examples/option.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/properties.py` & `pygobject-3.48.2/examples/properties.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/examples/signal.py` & `pygobject-3.48.2/examples/signal.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/__init__.py` & `pygobject-3.48.2/gi/__init__.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_constants.py` & `pygobject-3.48.2/gi/_constants.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_error.py` & `pygobject-3.48.2/gi/_error.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_gtktemplate.py` & `pygobject-3.48.2/gi/_gtktemplate.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_option.py` & `pygobject-3.48.2/gi/_option.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_ossighelper.py` & `pygobject-3.48.2/gi/_ossighelper.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_propertyhelper.py` & `pygobject-3.48.2/gi/_propertyhelper.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/_signalhelper.py` & `pygobject-3.48.2/gi/_signalhelper.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/docstring.py` & `pygobject-3.48.2/gi/docstring.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/gimodule.c` & `pygobject-3.48.2/gi/gimodule.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/gimodule.h` & `pygobject-3.48.2/gi/gimodule.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/importer.py` & `pygobject-3.48.2/gi/importer.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/meson.build` & `pygobject-3.48.2/gi/meson.build`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/module.py` & `pygobject-3.48.2/gi/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         # new introspection wrapper. This allows static C wrappers already
         # registered with the GType to be used as the introspection base
         # (_gi.GObject for example)
         gtype = object_info.get_g_type()
         if gtype and gtype.pytype:
             return gtype.pytype
 
-        if object_info.get_fundamental():
+        if object_info.get_fundamental() and gtype.is_instantiatable():
             return Fundamental
 
         # Otherwise use builtins.object as the base
         return object
 
     namespace = parent_object_info.get_namespace()
     name = parent_object_info.get_name()
```

### Comparing `pygobject-3.48.1/gi/overrides/GIMarshallingTests.py` & `pygobject-3.48.2/gi/overrides/GIMarshallingTests.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/GLib.py` & `pygobject-3.48.2/gi/overrides/GLib.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/GObject.py` & `pygobject-3.48.2/gi/overrides/GObject.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/Gdk.py` & `pygobject-3.48.2/gi/overrides/Gdk.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/GdkPixbuf.py` & `pygobject-3.48.2/gi/overrides/GdkPixbuf.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/Gio.py` & `pygobject-3.48.2/gi/overrides/Gio.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/Gtk.py` & `pygobject-3.48.2/gi/overrides/Gtk.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/Pango.py` & `pygobject-3.48.2/gi/overrides/Pango.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/__init__.py` & `pygobject-3.48.2/gi/overrides/__init__.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/overrides/keysyms.py` & `pygobject-3.48.2/gi/overrides/keysyms.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygboxed.c` & `pygobject-3.48.2/gi/pygboxed.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygboxed.h` & `pygobject-3.48.2/gi/pygboxed.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygenum.c` & `pygobject-3.48.2/gi/pygenum.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygenum.h` & `pygobject-3.48.2/gi/pygenum.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygflags.c` & `pygobject-3.48.2/gi/pygflags.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygflags.h` & `pygobject-3.48.2/gi/pygflags.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-argument.c` & `pygobject-3.48.2/gi/pygi-argument.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-argument.h` & `pygobject-3.48.2/gi/pygi-argument.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-array.c` & `pygobject-3.48.2/gi/pygi-array.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-array.h` & `pygobject-3.48.2/gi/pygi-array.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-basictype.c` & `pygobject-3.48.2/gi/pygi-basictype.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-basictype.h` & `pygobject-3.48.2/gi/pygi-basictype.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-boxed.c` & `pygobject-3.48.2/gi/pygi-boxed.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-boxed.h` & `pygobject-3.48.2/gi/pygi-boxed.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-cache.c` & `pygobject-3.48.2/gi/pygi-cache.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-cache.h` & `pygobject-3.48.2/gi/pygi-cache.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-ccallback.c` & `pygobject-3.48.2/gi/pygi-ccallback.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-ccallback.h` & `pygobject-3.48.2/gi/pygi-ccallback.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-closure.c` & `pygobject-3.48.2/gi/pygi-closure.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-closure.h` & `pygobject-3.48.2/gi/pygi-closure.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-enum-marshal.c` & `pygobject-3.48.2/gi/pygi-enum-marshal.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-enum-marshal.h` & `pygobject-3.48.2/gi/pygi-enum-marshal.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-error.c` & `pygobject-3.48.2/gi/pygi-error.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-error.h` & `pygobject-3.48.2/gi/pygi-error.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-foreign-api.h` & `pygobject-3.48.2/gi/pygi-foreign-api.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-foreign-cairo.c` & `pygobject-3.48.2/gi/pygi-foreign-cairo.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-foreign.c` & `pygobject-3.48.2/gi/pygi-foreign.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-foreign.h` & `pygobject-3.48.2/gi/pygi-foreign.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-fundamental.c` & `pygobject-3.48.2/gi/pygi-fundamental.c`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,19 @@
 }
 
 static PyObject *
 fundamental_new (PyTypeObject *type,
                  PyObject     *args,
                  PyObject     *kwargs)
 {
-    static char *kwlist[] = { NULL };
-
     GIBaseInfo *info;
     gpointer pointer;
     PyGIFundamental *self = NULL;
     GType g_type;
 
-    if (!PyArg_ParseTupleAndKeywords (args, kwargs, "", kwlist)) {
-        return NULL;
-    }
-
     info = _pygi_object_get_gi_info ((PyObject *) type, &PyGIObjectInfo_Type);
     if (info == NULL) {
         if (PyErr_ExceptionMatches (PyExc_AttributeError)) {
             PyErr_Format (PyExc_TypeError, "missing introspection information");
         }
         return NULL;
     }
@@ -95,14 +89,27 @@
 
 out:
     g_base_info_unref (info);
 
     return (PyObject *) self;
 }
 
+static int
+fundamental_init(PyObject     *self,
+                 PyObject     *args,
+                 PyObject     *kwargs)
+{
+    static char *kwlist[] = { NULL };
+
+    if (!PyArg_ParseTupleAndKeywords (args, kwargs, ":Fundamental.__init__", kwlist)) {
+        return -1;
+    }
+    return 0;
+}
+
 static PyObject*
 fundamental_richcompare (PyObject *self,
                          PyObject *other,
                          int op)
 {
     if (Py_TYPE (self) == Py_TYPE (other)) {
         return pyg_ptr_richcompare (((PyGIFundamental*) self)->instance,
@@ -218,14 +225,15 @@
 pygi_fundamental_register_types (PyObject *m)
 {
     Py_SET_TYPE(&PyGIFundamental_Type, &PyType_Type);
     g_assert (Py_TYPE (&PyGIFundamental_Type) != NULL);
 
     PyGIFundamental_Type.tp_alloc = PyType_GenericAlloc;
     PyGIFundamental_Type.tp_new = (newfunc) fundamental_new;
+    PyGIFundamental_Type.tp_init = (initproc) fundamental_init;
     PyGIFundamental_Type.tp_dealloc = (destructor) fundamental_dealloc;
     PyGIFundamental_Type.tp_flags = (Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE);
     PyGIFundamental_Type.tp_richcompare = fundamental_richcompare;
     PyGIFundamental_Type.tp_repr = (reprfunc) fundamental_repr;
     PyGIFundamental_Type.tp_hash = (hashfunc) fundamental_hash;
 
     if (PyType_Ready (&PyGIFundamental_Type))
```

### Comparing `pygobject-3.48.1/gi/pygi-fundamental.h` & `pygobject-3.48.2/gi/pygi-fundamental.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-hashtable.c` & `pygobject-3.48.2/gi/pygi-hashtable.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-hashtable.h` & `pygobject-3.48.2/gi/pygi-hashtable.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-info.c` & `pygobject-3.48.2/gi/pygi-info.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-info.h` & `pygobject-3.48.2/gi/pygi-info.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-invoke-state-struct.h` & `pygobject-3.48.2/gi/pygi-invoke-state-struct.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-invoke.c` & `pygobject-3.48.2/gi/pygi-invoke.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-invoke.h` & `pygobject-3.48.2/gi/pygi-invoke.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-list.c` & `pygobject-3.48.2/gi/pygi-list.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-list.h` & `pygobject-3.48.2/gi/pygi-list.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-marshal-cleanup.c` & `pygobject-3.48.2/gi/pygi-marshal-cleanup.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-marshal-cleanup.h` & `pygobject-3.48.2/gi/pygi-marshal-cleanup.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-object.c` & `pygobject-3.48.2/gi/pygi-object.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-object.h` & `pygobject-3.48.2/gi/pygi-object.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-property.c` & `pygobject-3.48.2/gi/pygi-property.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-property.h` & `pygobject-3.48.2/gi/pygi-property.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-repository.c` & `pygobject-3.48.2/gi/pygi-repository.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-repository.h` & `pygobject-3.48.2/gi/pygi-repository.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-resulttuple.c` & `pygobject-3.48.2/gi/pygi-resulttuple.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-resulttuple.h` & `pygobject-3.48.2/gi/pygi-resulttuple.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-signal-closure.c` & `pygobject-3.48.2/gi/pygi-signal-closure.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-signal-closure.h` & `pygobject-3.48.2/gi/pygi-signal-closure.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-source.c` & `pygobject-3.48.2/gi/pygi-source.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-source.h` & `pygobject-3.48.2/gi/pygi-source.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-struct-marshal.c` & `pygobject-3.48.2/gi/pygi-struct-marshal.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-struct-marshal.h` & `pygobject-3.48.2/gi/pygi-struct-marshal.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-struct.c` & `pygobject-3.48.2/gi/pygi-struct.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-struct.h` & `pygobject-3.48.2/gi/pygi-struct.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-type.c` & `pygobject-3.48.2/gi/pygi-type.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-type.h` & `pygobject-3.48.2/gi/pygi-type.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-util.c` & `pygobject-3.48.2/gi/pygi-util.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-util.h` & `pygobject-3.48.2/gi/pygi-util.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-value.c` & `pygobject-3.48.2/gi/pygi-value.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygi-value.h` & `pygobject-3.48.2/gi/pygi-value.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pyginterface.c` & `pygobject-3.48.2/gi/pyginterface.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pyginterface.h` & `pygobject-3.48.2/gi/pyginterface.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygobject-object.c` & `pygobject-3.48.2/gi/pygobject-object.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygobject-object.h` & `pygobject-3.48.2/gi/pygobject-object.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygobject.h` & `pygobject-3.48.2/gi/pygobject.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygoptioncontext.c` & `pygobject-3.48.2/gi/pygoptioncontext.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygoptioncontext.h` & `pygobject-3.48.2/gi/pygoptioncontext.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygoptiongroup.c` & `pygobject-3.48.2/gi/pygoptiongroup.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygoptiongroup.h` & `pygobject-3.48.2/gi/pygoptiongroup.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygparamspec.c` & `pygobject-3.48.2/gi/pygparamspec.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygparamspec.h` & `pygobject-3.48.2/gi/pygparamspec.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygpointer.c` & `pygobject-3.48.2/gi/pygpointer.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygpointer.h` & `pygobject-3.48.2/gi/pygpointer.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygspawn.c` & `pygobject-3.48.2/gi/pygspawn.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygspawn.h` & `pygobject-3.48.2/gi/pygspawn.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/pygtkcompat.py` & `pygobject-3.48.2/gi/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/repository/__init__.py` & `pygobject-3.48.2/gi/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/gi/types.py` & `pygobject-3.48.2/gi/types.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/meson.build` & `pygobject-3.48.2/meson.build`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('pygobject', 'c',
-  version : '3.48.1',
+  version : '3.48.2',
   meson_version : '>= 0.64.0',
   default_options : [ 'warning_level=1',
                       'buildtype=debugoptimized'])
 
 pygobject_version = meson.project_version()
 version_arr = pygobject_version.split('.')
 pygobject_version_major = version_arr[0].to_int()
```

### Comparing `pygobject-3.48.1/pygobject-3.0.pc.in` & `pygobject-3.48.2/pygobject-3.0.pc.in`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/pygobject.doap` & `pygobject-3.48.2/pygobject.doap`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/pygtkcompat/__init__.py` & `pygobject-3.48.2/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/pygtkcompat/generictreemodel.py` & `pygobject-3.48.2/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/pygtkcompat/pygtkcompat.py` & `pygobject-3.48.2/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/pyproject.toml` & `pygobject-3.48.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyGObject"
-version = "3.48.1"
+version = "3.48.2"
 description = "Python bindings for GObject Introspection"
 license = { text = "GNU Lesser General Public License v2.1 (LGPLv2.1)" }
 authors = [
     { name="James Henstridge", email="james@daa.com.au" }
 ]
 maintainers = [
     { name="Simon Feltman", email="sfeltman@src.gnome.org" },
```

### Comparing `pygobject-3.48.1/tests/conftest.py` & `pygobject-3.48.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/gimarshallingtestsextra.c` & `pygobject-3.48.2/tests/gimarshallingtestsextra.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/gimarshallingtestsextra.h` & `pygobject-3.48.2/tests/gimarshallingtestsextra.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/helper.py` & `pygobject-3.48.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/meson.build` & `pygobject-3.48.2/tests/meson.build`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/org.gnome.test.gschema.xml` & `pygobject-3.48.2/tests/org.gnome.test.gschema.xml`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/regressextra.c` & `pygobject-3.48.2/tests/regressextra.c`

 * *Files 5% similar despite different names*

```diff
@@ -481,7 +481,73 @@
      */
     regress_test_action_signals[ACTION2_SIGNAL] =
         g_signal_new_class_handler ("action2",
         G_TYPE_FROM_CLASS (klass), G_SIGNAL_RUN_LAST | G_SIGNAL_ACTION,
         G_CALLBACK (regress_test_action_do_action2), NULL, NULL,
         NULL, regress_test_action_get_type (), 0);
 }
+
+/*
+ * RegressBitmask
+ *
+ * Mimic a primitive, fundamental type.
+ */
+
+static void
+regress_value_init_bitmask (GValue * value)
+{
+  value->data[0].v_uint64 = 0;
+}
+
+static void
+regress_value_copy_bitmask (const GValue * src_value, GValue * dest_value)
+{
+  dest_value->data[0].v_uint64 = src_value->data[0].v_uint64;
+}
+
+static void
+_value_transform_uint64_bitmask (const GValue * src_value, GValue * dest_value)
+{
+    dest_value->data[0].v_uint64 = src_value->data[0].v_uint64;
+}
+
+static void
+_value_transform_bitmask_uint64 (const GValue * src_value, GValue * dest_value)
+{
+    dest_value->data[0].v_uint64 = src_value->data[0].v_uint64;
+}
+
+static const GTypeValueTable _regress_bitmask_value_table = {
+    regress_value_init_bitmask,
+    NULL,
+    regress_value_copy_bitmask,
+    NULL,
+    (char *) NULL,
+    NULL,
+    (char *) NULL,
+    NULL
+};
+
+GType
+regress_bitmask_get_type (void)
+{
+  static GType regress_bitmask_type = 0;
+
+  if (g_once_init_enter (&regress_bitmask_type)) {
+    GTypeInfo _info = { 0, NULL, NULL, NULL, NULL, NULL, 0, 0, NULL, &_regress_bitmask_value_table };
+    GTypeFundamentalInfo _finfo = { 0 };
+    GType _type = g_type_register_fundamental (
+        g_type_fundamental_next (),
+        "RegressBitmask", &_info, &_finfo, 0);
+
+    g_once_init_leave(&regress_bitmask_type, _type);
+
+    g_value_register_transform_func (
+      REGRESS_TYPE_BITMASK, G_TYPE_UINT64,
+      _value_transform_bitmask_uint64);
+    g_value_register_transform_func (
+      G_TYPE_UINT64, REGRESS_TYPE_BITMASK,
+      _value_transform_uint64_bitmask);
+  }
+
+  return regress_bitmask_type;
+}
```

### Comparing `pygobject-3.48.1/tests/regressextra.h` & `pygobject-3.48.2/tests/regressextra.h`

 * *Files 19% similar despite different names*

```diff
@@ -86,8 +86,30 @@
 typedef struct {
   GInitiallyUnownedClass parent_class;
 } RegressTestActionClass;
 
 _GI_TEST_EXTERN
 GType regress_test_action_get_type (void);
 
+
+/**
+ * RegressBitmask:
+ *
+ * A fundamental type that describes a 64-bit bitmask.
+ *
+ * This type resembles GStreamer's Bitmask type.
+ */
+
+/**
+ * REGRESS_TYPE_BITMASK:
+ *
+ * a #GValue type that represents a 64-bit bitmask.
+ *
+ * Returns: the #GType of RegressBitmask (which is not explicitly typed)
+ */
+
+#define REGRESS_TYPE_BITMASK                 (regress_bitmask_get_type())
+
+_GI_TEST_EXTERN
+GType regress_bitmask_get_type (void);
+
 #endif /* REGRESS_EXTRA_H */
```

### Comparing `pygobject-3.48.1/tests/test-floating.c` & `pygobject-3.48.2/tests/test-floating.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test-floating.h` & `pygobject-3.48.2/tests/test-floating.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test-thread.c` & `pygobject-3.48.2/tests/test-thread.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test-thread.h` & `pygobject-3.48.2/tests/test-thread.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test-unknown.c` & `pygobject-3.48.2/tests/test-unknown.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test-unknown.h` & `pygobject-3.48.2/tests/test-unknown.h`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_atoms.py` & `pygobject-3.48.2/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_cairo.py` & `pygobject-3.48.2/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_docstring.py` & `pygobject-3.48.2/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_error.py` & `pygobject-3.48.2/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_everything.py` & `pygobject-3.48.2/tests/test_everything.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_fields.py` & `pygobject-3.48.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_fundamental.py` & `pygobject-3.48.2/tests/test_fundamental.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,20 @@
 def test_multiple_objects():
     obj1 = Regress.TestFundamentalSubObject()
     obj2 = Regress.TestFundamentalSubObject()
 
     assert obj1 != obj2
 
 
+def test_fundamental_primitive_object():
+    bitmask = Regress.Bitmask(2)
+
+    assert bitmask.v == 2
+
+
 def test_custom_fundamental_type_vfunc_override(capsys):
     obj = MyCustomFundamentalObject()
     del obj
 
     out = capsys.readouterr().out
 
     assert "MyCustomFundamentalObject.__init__" in out
```

### Comparing `pygobject-3.48.1/tests/test_gdbus.py` & `pygobject-3.48.2/tests/test_gdbus.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_generictreemodel.py` & `pygobject-3.48.2/tests/test_generictreemodel.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_gi.py` & `pygobject-3.48.2/tests/test_gi.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_gio.py` & `pygobject-3.48.2/tests/test_gio.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_glib.py` & `pygobject-3.48.2/tests/test_glib.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_gobject.py` & `pygobject-3.48.2/tests/test_gobject.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_gtk_template.py` & `pygobject-3.48.2/tests/test_gtk_template.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_gtype.py` & `pygobject-3.48.2/tests/test_gtype.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_import_machinery.py` & `pygobject-3.48.2/tests/test_import_machinery.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_interface.py` & `pygobject-3.48.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_internal_api.py` & `pygobject-3.48.2/tests/test_internal_api.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_iochannel.py` & `pygobject-3.48.2/tests/test_iochannel.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_mainloop.py` & `pygobject-3.48.2/tests/test_mainloop.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_object_marshaling.py` & `pygobject-3.48.2/tests/test_object_marshaling.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_option.py` & `pygobject-3.48.2/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_ossig.py` & `pygobject-3.48.2/tests/test_ossig.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_gdk.py` & `pygobject-3.48.2/tests/test_overrides_gdk.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_gdkpixbuf.py` & `pygobject-3.48.2/tests/test_overrides_gdkpixbuf.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_gio.py` & `pygobject-3.48.2/tests/test_overrides_gio.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_glib.py` & `pygobject-3.48.2/tests/test_overrides_glib.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_gobject.py` & `pygobject-3.48.2/tests/test_overrides_gobject.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_gtk.py` & `pygobject-3.48.2/tests/test_overrides_gtk.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_overrides_pango.py` & `pygobject-3.48.2/tests/test_overrides_pango.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_properties.py` & `pygobject-3.48.2/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_pycapi.py` & `pygobject-3.48.2/tests/test_pycapi.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_pygtkcompat.py` & `pygobject-3.48.2/tests/test_pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_repository.py` & `pygobject-3.48.2/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_resulttuple.py` & `pygobject-3.48.2/tests/test_resulttuple.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_signal.py` & `pygobject-3.48.2/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_source.py` & `pygobject-3.48.2/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_subprocess.py` & `pygobject-3.48.2/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_thread.py` & `pygobject-3.48.2/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_typeclass.py` & `pygobject-3.48.2/tests/test_typeclass.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/test_unknown.py` & `pygobject-3.48.2/tests/test_unknown.py`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tests/testhelpermodule.c` & `pygobject-3.48.2/tests/testhelpermodule.c`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/tools/pygi-convert.sh` & `pygobject-3.48.2/tools/pygi-convert.sh`

 * *Files identical despite different names*

### Comparing `pygobject-3.48.1/PKG-INFO` & `pygobject-3.48.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGObject
-Version: 3.48.1
+Version: 3.48.2
 Summary: Python bindings for GObject Introspection
 Author-Email: James Henstridge <james@daa.com.au>
 Maintainer: Christoph Reiter
 Maintainer-Email: Simon Feltman <sfeltman@src.gnome.org>
 License: GNU Lesser General Public License v2.1 (LGPLv2.1)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

