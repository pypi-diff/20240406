# Comparing `tmp/omnix-0.3.3.tar.gz` & `tmp/omnix-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omnix-0.3.3.tar", last modified: Fri Apr  5 10:49:40 2024, max compression
+gzip compressed data, was "dist/omnix-0.3.4.tar", last modified: Fri Apr  5 21:41:44 2024, max compression
```

## Comparing `omnix-0.3.3.tar` & `omnix-0.3.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:49:36.000000 omnix-0.3.3/src/omnix.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3761 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/util/
--rw-r--r--   0 root         (0) root         (0)     3322 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/logic.py
--rw-r--r--   0 root         (0) root         (0)     2380 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3533 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/image.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2342 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/format.py
--rw-r--r--   0 root         (0) root         (0)    34528 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/business.py
--rw-r--r--   0 root         (0) root         (0)     4362 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/ctt.py
--rw-r--r--   0 root         (0) root         (0)     5615 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/config.py
--rw-r--r--   0 root         (0) root         (0)     7106 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/slave.py
--rw-r--r--   0 root         (0) root         (0)     8985 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/util/supervisor.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/images/
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/down.png
--rw-r--r--   0 root         (0) root         (0)      108 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/equal.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/images/email/
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/email/logo.png
--rw-r--r--   0 root         (0) root         (0)      127 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/up.png
--rw-r--r--   0 root         (0) root         (0)     2771 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/images/login.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/css/
--rw-r--r--   0 root         (0) root         (0)     3930 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/css/layout.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/static/js/
--rw-r--r--   0 root         (0) root         (0)     5109 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/static/js/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/error.html.tpl
--rw-r--r--   0 root         (0) root         (0)      959 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/about.html.tpl
--rw-r--r--   0 root         (0) root         (0)      338 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/index.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/media/
--rw-r--r--   0 root         (0) root         (0)     3043 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/media/edit.html.tpl
--rw-r--r--   0 root         (0) root         (0)      837 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/media/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1977 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/media/show.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/extra/
--rw-r--r--   0 root         (0) root         (0)     1051 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/ctt.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/costs.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3985 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3345 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/template.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/media.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/images.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/prices.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1093 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/inventory.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1445 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/transfers.html.tpl
--rw-r--r--   0 root         (0) root         (0)     2016 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/browser.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/extra/browser/
--rw-r--r--   0 root         (0) root         (0)     3538 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/browser/new_media.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/extra/metadata.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/entity/
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/entity/edit.html.tpl
--rw-r--r--   0 root         (0) root         (0)      852 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/entity/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1720 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/entity/show.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/report/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/report/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)     2311 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/report/sales.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/customer/
--rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/customer/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)      913 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/customer/show.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/partials/
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/doctype.html.tpl
--rw-r--r--   0 root         (0) root         (0)     5710 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout.html.tpl
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/end_doctype.html.tpl
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/content_type.html.tpl
--rw-r--r--   0 root         (0) root         (0)      237 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/messages.html.tpl
--rw-r--r--   0 root         (0) root         (0)      679 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_store.html.tpl
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_simple.html.tpl
--rw-r--r--   0 root         (0) root         (0)      680 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_report.html.tpl
--rw-r--r--   0 root         (0) root         (0)      940 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/includes.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1875 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_employee.html.tpl
--rw-r--r--   0 root         (0) root         (0)      686 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_entity.html.tpl
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/footer.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/partials/layout_media.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/supplier/
--rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/supplier/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/supplier/show.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/email/
--rw-r--r--   0 root         (0) root         (0)     1591 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/layout.pt_pt.html.tpl
--rw-r--r--   0 root         (0) root         (0)      215 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/birthday.pt_pt.html.tpl
--rw-r--r--   0 root         (0) root         (0)      717 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/macros.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1587 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/layout.en_us.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3290 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/activity.en_us.html.tpl
--rw-r--r--   0 root         (0) root         (0)      207 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/birthday.en_us.html.tpl
--rw-r--r--   0 root         (0) root         (0)     3310 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/email/activity.pt_pt.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/employee/
--rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/employee/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)      812 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/employee/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)     4090 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/employee/sales.html.tpl
--rw-r--r--   0 root         (0) root         (0)      480 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/signin.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/templates/store/
--rw-r--r--   0 root         (0) root         (0)      874 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/store/list.html.tpl
--rw-r--r--   0 root         (0) root         (0)      778 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/store/show.html.tpl
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/store/sales.html.tpl
--rw-r--r--   0 root         (0) root         (0)     2790 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/templates/top.html.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/models/
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1584 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/models/base.py
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/models/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/views/
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/views/web/
--rw-r--r--   0 root         (0) root         (0)     2631 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1931 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/supplier.py
--rw-r--r--   0 root         (0) root         (0)    10028 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/base.py
--rw-r--r--   0 root         (0) root         (0)     2413 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/settings.py
--rw-r--r--   0 root         (0) root         (0)     3538 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/media.py
--rw-r--r--   0 root         (0) root         (0)    50263 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/extra.py
--rw-r--r--   0 root         (0) root         (0)     4169 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/store.py
--rw-r--r--   0 root         (0) root         (0)     1500 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/report.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/customer.py
--rw-r--r--   0 root         (0) root         (0)     5180 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/employee.py
--rw-r--r--   0 root         (0) root         (0)     3299 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/web/entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/views/api/
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/views/api/base.py
--rw-r--r--   0 root         (0) root         (0)     1952 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:49:40.000000 omnix-0.3.3/src/omnix/test/util/
--rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12740 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/test/util/business.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 10:49:28.000000 omnix-0.3.3/src/omnix/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3514 2024-04-05 10:49:28.000000 omnix-0.3.3/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 10:49:40.000000 omnix-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4118 2024-04-05 10:49:28.000000 omnix-0.3.3/README.md
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-05 10:49:40.000000 omnix-0.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 21:41:44.000000 omnix-0.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4118 2024-04-05 21:41:32.000000 omnix-0.3.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-04-05 21:41:32.000000 omnix-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3761 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 21:41:40.000000 omnix-0.3.4/src/omnix.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/supplier/
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/supplier/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/supplier/show.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)      940 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/includes.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      679 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout_store.html.tpl
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/doctype.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     5710 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout_simple.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout_media.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      237 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/messages.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      680 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout_report.html.tpl
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/content_type.html.tpl
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/end_doctype.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout_employee.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/footer.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      686 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/partials/layout_entity.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/store/
+-rw-r--r--   0 root         (0) root         (0)      874 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/store/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/store/show.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/store/sales.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/media/
+-rw-r--r--   0 root         (0) root         (0)      837 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/media/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3043 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/media/edit.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/media/show.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/error.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/top.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/customer/
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/customer/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      913 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/customer/show.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/about.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/signin.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/email/
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/activity.pt_pt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      207 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/birthday.en_us.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/activity.en_us.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/layout.en_us.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/birthday.pt_pt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1591 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/layout.pt_pt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      717 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/email/macros.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/report/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/report/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/report/sales.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/employee/
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/employee/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      812 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/employee/show.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     4090 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/employee/sales.html.tpl
+-rw-r--r--   0 root         (0) root         (0)      338 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/index.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/entity/
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/entity/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/entity/edit.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/entity/show.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/extra/
+-rw-r--r--   0 root         (0) root         (0)     3985 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/list.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/ctt.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/costs.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     3345 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/template.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/browser.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/inventory.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/templates/extra/browser/
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/browser/new_media.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/images.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/metadata.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/media.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/prices.html.tpl
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/templates/extra/transfers.html.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/views/web/
+-rw-r--r--   0 root         (0) root         (0)     2413 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/settings.py
+-rw-r--r--   0 root         (0) root         (0)    50263 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/extra.py
+-rw-r--r--   0 root         (0) root         (0)     4169 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/store.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/customer.py
+-rw-r--r--   0 root         (0) root         (0)    10028 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/base.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/entity.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/media.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/supplier.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/report.py
+-rw-r--r--   0 root         (0) root         (0)     5180 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/web/employee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/views/api/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/test/
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/test/util/
+-rw-r--r--   0 root         (0) root         (0)    12740 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/test/util/business.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/test/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/util/
+-rw-r--r--   0 root         (0) root         (0)    34528 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/business.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/image.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/slave.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/logic.py
+-rw-r--r--   0 root         (0) root         (0)     9125 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/supervisor.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/format.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/ctt.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/models/
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/models/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/static/css/
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/css/layout.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/static/js/
+-rw-r--r--   0 root         (0) root         (0)     5109 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/static/images/
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/images/login.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 21:41:44.000000 omnix-0.3.4/src/omnix/static/images/email/
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/images/email/logo.png
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/images/down.png
+-rw-r--r--   0 root         (0) root         (0)      127 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/images/up.png
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-05 21:41:32.000000 omnix-0.3.4/src/omnix/static/images/equal.png
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-05 21:41:44.000000 omnix-0.3.4/PKG-INFO
```

### Comparing `omnix-0.3.3/src/omnix.egg-info/SOURCES.txt` & `omnix-0.3.4/src/omnix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix.egg-info/PKG-INFO` & `omnix-0.3.4/src/omnix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnix
-Version: 0.3.3
+Version: 0.3.4
 Summary: Omnix System
 Home-page: http://omnix.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni (x)Extensions](http://omnix.hive.pt)
```

### Comparing `omnix-0.3.3/src/omnix/util/logic.py` & `omnix-0.3.4/src/omnix/util/logic.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/__init__.py` & `omnix-0.3.4/src/omnix/util/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,17 +60,23 @@
     LOCAL_URL,
     REMOTE_URL,
     REDIRECT_URL,
     CLIENT_ID,
     CLIENT_SECRET,
     FIRST_DAY,
     SCOPE,
+    DOCUMENT_INBOUND,
+    DOCUMENT_OUTBOUND,
+    AT_DOCUMENT_TYPES,
     AT_SALE_TYPES,
     AT_TRANSPORT_TYPES,
     AT_SUBMIT_TYPES,
+    AT_SALE_DIGEST_TYPES,
+    AT_TRANSPORT_DIGEST_TYPES,
+    AT_SUBMIT_DIGEST_TYPES,
     REMOTE,
     BASE_URL,
     SENDER_EMAIL,
     USERNAME,
     PASSWORD,
     SCHEDULE,
     COMMISSION_RATE,
```

### Comparing `omnix-0.3.3/src/omnix/util/image.py` & `omnix-0.3.4/src/omnix/util/image.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/scheduling.py` & `omnix-0.3.4/src/omnix/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/format.py` & `omnix-0.3.4/src/omnix/util/format.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/business.py` & `omnix-0.3.4/src/omnix/util/business.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/ctt.py` & `omnix-0.3.4/src/omnix/util/ctt.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/config.py` & `omnix-0.3.4/src/omnix/util/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,26 +102,50 @@
     "inventory.transfer.create",
     "inventory.transactional_merchandise.list",
     "inventory.transactional_merchandise.update",
 )
 """ The list of permissions to be used to create the
 scope string for the OAuth value """
 
+DOCUMENT_INBOUND = 2
+""" The inbound document type value, for documents that represent
+actions coming from external entities into the system company """
+
+DOCUMENT_OUTBOUND = 3
+""" The outbound document type value, for documents that represent
+actions going from the system company to external entities """
+
+AT_DOCUMENT_TYPES = (DOCUMENT_INBOUND, DOCUMENT_OUTBOUND)
+""" The multiple document types that are considered to be valid
+for AT submission """
+
 AT_SALE_TYPES = ("MoneySaleSlip", "Invoice", "CreditNote", "DebitNote")
 """ The list containing the complete set of types that
-are considered to be of type sake """
+are considered to be of type sale """
 
 AT_TRANSPORT_TYPES = ("TransportationSlip", "ExpeditionSlip")
 """ The list containing the complete set of types that
 are considered to be of type transport """
 
 AT_SUBMIT_TYPES = AT_SALE_TYPES + AT_TRANSPORT_TYPES
 """ The set of valid types for submission to AT, note
 that this range of values should be changed with care """
 
+AT_SALE_DIGEST_TYPES = ("FS", "FT", "NC", "ND")
+""" The list containing the complete set of digest types that
+are considered to be of type sale """
+
+AT_TRANSPORT_DIGEST_TYPES = ("GT", "GR")
+""" The list containing the complete set of digest types that
+are considered to be of type transport """
+
+AT_SUBMIT_DIGEST_TYPES = AT_SALE_DIGEST_TYPES + AT_TRANSPORT_DIGEST_TYPES
+""" The set of valid digest types for submission to AT, note
+that this range of values should be changed with care """
+
 REMOTE = quorum.conf("REMOTE", False, cast=bool)
 REMOTE = quorum.conf("OMNIX_REMOTE", REMOTE, cast=bool)
 BASE_URL = quorum.conf("BASE_URL", "http://localhost:8181")
 REDIRECT_URL = quorum.conf("REDIRECT_URL", REDIRECT_URL)
 CLIENT_ID = quorum.conf("OMNIX_CLIENT_ID", CLIENT_ID)
 CLIENT_SECRET = quorum.conf("OMNIX_CLIENT_SECRET", CLIENT_SECRET)
 SENDER_EMAIL = quorum.conf("SENDER_EMAIL", "Omnix <no-reply@omnix.com>")
```

### Comparing `omnix-0.3.3/src/omnix/util/slave.py` & `omnix-0.3.4/src/omnix/util/slave.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/util/supervisor.py` & `omnix-0.3.4/src/omnix/util/supervisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,17 @@
             "filter_string": "",
             "start_record": 0,
             "number_records": NUMBER_RECORDS,
             "sort": "issue_date:ascending",
             "filters[]": [
                 "issue_date:greater:1356998400",
                 "submitted_at:equals:2",
-                "document_type:in:1;3",
+                "document_type:in:%s"
+                % ";".join(str(v) for v in config.AT_DOCUMENT_TYPES),
+                "digest_document_type:in:%s" % ";".join(config.AT_SUBMIT_DIGEST_TYPES),
             ],
         }
         documents = self.api.list_signed_documents(**kwargs)
         valid_documents = [
             value for value in documents if value["_class"] in config.AT_SUBMIT_TYPES
         ]
 
@@ -159,15 +161,15 @@
         # the number of messages that have been successfully queued to
         # the remote queueing mechanism (for debugging)
         count = 0
 
         # prints a debug message about the number of valid documents that
         # have been found for submission to the queue
         quorum.debug(
-            "Found %d valid documents for submission, from a total of %d documents"
+            "Found %d (out of %d) valid documents for submission"
             % (len(valid_documents), len(documents))
         )
 
         # iterates over all the valid documents that have been found
         # as not submitted and creates a task for their submission
         # then adds the task to the AMQP queue to be processed
         for document in valid_documents:
```

### Comparing `omnix-0.3.3/src/omnix/__init__.py` & `omnix-0.3.4/src/omnix/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/static/images/email/logo.png` & `omnix-0.3.4/src/omnix/static/images/email/logo.png`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/static/images/login.png` & `omnix-0.3.4/src/omnix/static/images/login.png`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/static/css/layout.css` & `omnix-0.3.4/src/omnix/static/css/layout.css`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/static/js/main.js` & `omnix-0.3.4/src/omnix/static/js/main.js`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/error.html.tpl` & `omnix-0.3.4/src/omnix/templates/error.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/about.html.tpl` & `omnix-0.3.4/src/omnix/templates/about.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/media/edit.html.tpl` & `omnix-0.3.4/src/omnix/templates/media/edit.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/media/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/media/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/media/show.html.tpl` & `omnix-0.3.4/src/omnix/templates/media/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/ctt.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/ctt.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/costs.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/costs.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/template.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/template.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/media.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/media.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/images.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/images.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/prices.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/prices.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/inventory.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/inventory.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/transfers.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/transfers.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/browser.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/browser.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/browser/new_media.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/browser/new_media.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/extra/metadata.html.tpl` & `omnix-0.3.4/src/omnix/templates/extra/metadata.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/entity/edit.html.tpl` & `omnix-0.3.4/src/omnix/templates/entity/edit.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/entity/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/entity/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/entity/show.html.tpl` & `omnix-0.3.4/src/omnix/templates/entity/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/report/sales.html.tpl` & `omnix-0.3.4/src/omnix/templates/report/sales.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/customer/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/customer/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/customer/show.html.tpl` & `omnix-0.3.4/src/omnix/templates/customer/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout_store.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout_store.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout_simple.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout_simple.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout_report.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout_report.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/includes.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/includes.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout_employee.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout_employee.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout_entity.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout_entity.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/partials/layout_media.html.tpl` & `omnix-0.3.4/src/omnix/templates/partials/layout_media.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/supplier/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/supplier/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/supplier/show.html.tpl` & `omnix-0.3.4/src/omnix/templates/supplier/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/email/layout.pt_pt.html.tpl` & `omnix-0.3.4/src/omnix/templates/email/layout.pt_pt.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/email/macros.html.tpl` & `omnix-0.3.4/src/omnix/templates/email/macros.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/email/layout.en_us.html.tpl` & `omnix-0.3.4/src/omnix/templates/email/layout.en_us.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/email/activity.en_us.html.tpl` & `omnix-0.3.4/src/omnix/templates/email/activity.en_us.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/email/activity.pt_pt.html.tpl` & `omnix-0.3.4/src/omnix/templates/email/activity.pt_pt.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/employee/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/employee/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/employee/show.html.tpl` & `omnix-0.3.4/src/omnix/templates/employee/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/employee/sales.html.tpl` & `omnix-0.3.4/src/omnix/templates/employee/sales.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/store/list.html.tpl` & `omnix-0.3.4/src/omnix/templates/store/list.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/store/show.html.tpl` & `omnix-0.3.4/src/omnix/templates/store/show.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/store/sales.html.tpl` & `omnix-0.3.4/src/omnix/templates/store/sales.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/templates/top.html.tpl` & `omnix-0.3.4/src/omnix/templates/top.html.tpl`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/models/__init__.py` & `omnix-0.3.4/src/omnix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/models/base.py` & `omnix-0.3.4/src/omnix/models/base.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/models/settings.py` & `omnix-0.3.4/src/omnix/models/settings.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/__init__.py` & `omnix-0.3.4/src/omnix/views/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/__init__.py` & `omnix-0.3.4/src/omnix/views/web/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/supplier.py` & `omnix-0.3.4/src/omnix/views/web/supplier.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/base.py` & `omnix-0.3.4/src/omnix/views/web/base.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/settings.py` & `omnix-0.3.4/src/omnix/views/web/settings.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/media.py` & `omnix-0.3.4/src/omnix/views/web/media.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/extra.py` & `omnix-0.3.4/src/omnix/views/web/extra.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/store.py` & `omnix-0.3.4/src/omnix/views/web/store.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/report.py` & `omnix-0.3.4/src/omnix/views/web/report.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/customer.py` & `omnix-0.3.4/src/omnix/views/web/customer.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/employee.py` & `omnix-0.3.4/src/omnix/views/web/employee.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/web/entity.py` & `omnix-0.3.4/src/omnix/views/web/entity.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/api/__init__.py` & `omnix-0.3.4/src/omnix/views/api/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/views/api/base.py` & `omnix-0.3.4/src/omnix/views/api/base.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/main.py` & `omnix-0.3.4/src/omnix/main.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/test/util/__init__.py` & `omnix-0.3.4/src/omnix/test/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/test/util/business.py` & `omnix-0.3.4/src/omnix/test/util/business.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/src/omnix/test/__init__.py` & `omnix-0.3.4/src/omnix/test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/setup.py` & `omnix-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name="omnix",
-    version="0.3.3",
+    version="0.3.4",
     author="Hive Solutions Lda.",
     author_email="development@hive.pt",
     description="Omnix System",
     license="Apache License, Version 2.0",
     keywords="omni extensions erp",
     url="http://omnix.hive.pt",
     zip_safe=False,
```

### Comparing `omnix-0.3.3/README.md` & `omnix-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `omnix-0.3.3/PKG-INFO` & `omnix-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnix
-Version: 0.3.3
+Version: 0.3.4
 Summary: Omnix System
 Home-page: http://omnix.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Omni (x)Extensions](http://omnix.hive.pt)
```

