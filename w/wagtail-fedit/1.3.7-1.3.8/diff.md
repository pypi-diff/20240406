# Comparing `tmp/wagtail_fedit-1.3.7.tar.gz` & `tmp/wagtail_fedit-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.7.tar", last modified: Fri Apr  5 20:42:48 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.8.tar", last modified: Fri Apr  5 20:58:56 2024, max compression
```

## Comparing `wagtail_fedit-1.3.7.tar` & `wagtail_fedit-1.3.8.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.485573 wagtail_fedit-1.3.7/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7538 2024-04-05 20:42:48.485573 wagtail_fedit-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.7/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 20:42:48.493452 wagtail_fedit-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.388682 wagtail_fedit-1.3.7/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.7/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.7/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.7/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.413884 wagtail_fedit-1.3.7/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.7/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.7/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.7/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.7/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.414889 wagtail_fedit-1.3.7/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.7/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.415881 wagtail_fedit-1.3.7/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.3.7/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.357157 wagtail_fedit-1.3.7/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.358765 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.420867 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.422782 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.360772 wagtail_fedit-1.3.7/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.362770 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.423967 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.425958 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.434527 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.436529 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.438806 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.441991 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.443990 wagtail_fedit-1.3.7/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.7/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.446987 wagtail_fedit-1.3.7/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.7/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.449770 wagtail_fedit-1.3.7/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.453779 wagtail_fedit-1.3.7/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.458253 wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.466595 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6996 2024-04-05 20:03:30.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     2755 2024-04-05 20:42:15.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.471858 wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.7/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.7/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.7/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.475866 wagtail_fedit-1.3.7/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.7/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.7/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    14326 2024-04-05 20:33:13.000000 wagtail_fedit-1.3.7/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.7/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1456 2024-04-05 18:16:06.000000 wagtail_fedit-1.3.7/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.484579 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:42:48.410009 wagtail_fedit-1.3.7/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7538 2024-04-05 20:42:48.000000 wagtail_fedit-1.3.7/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3499 2024-04-05 20:42:48.000000 wagtail_fedit-1.3.7/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:42:48.000000 wagtail_fedit-1.3.7/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 20:42:48.000000 wagtail_fedit-1.3.7/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 20:42:48.000000 wagtail_fedit-1.3.7/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.960336 wagtail_fedit-1.3.8/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     7538 2024-04-05 20:58:56.960336 wagtail_fedit-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.8/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 20:58:56.969103 wagtail_fedit-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.818622 wagtail_fedit-1.3.8/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.8/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.8/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.8/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.844609 wagtail_fedit-1.3.8/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.8/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.8/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.8/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.8/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.845687 wagtail_fedit-1.3.8/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.8/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.845687 wagtail_fedit-1.3.8/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.3.8/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.798645 wagtail_fedit-1.3.8/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.799694 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.845687 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.864385 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.800703 wagtail_fedit-1.3.8/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.801703 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.864385 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.864385 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-05 20:57:10.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.879321 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.879321 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.879321 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.892627 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.894601 wagtail_fedit-1.3.8/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.8/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.896767 wagtail_fedit-1.3.8/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16816 2024-04-05 20:58:14.000000 wagtail_fedit-1.3.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13781 2024-04-05 20:58:12.000000 wagtail_fedit-1.3.8/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.896767 wagtail_fedit-1.3.8/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.896767 wagtail_fedit-1.3.8/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.896767 wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.913094 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6996 2024-04-05 20:03:30.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 20:42:15.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.913094 wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.8/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.8/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.8/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.946576 wagtail_fedit-1.3.8/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.8/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.8/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    14407 2024-04-05 20:53:33.000000 wagtail_fedit-1.3.8/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.8/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.3.8/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.959286 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:58:56.842669 wagtail_fedit-1.3.8/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7538 2024-04-05 20:58:56.000000 wagtail_fedit-1.3.8/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3499 2024-04-05 20:58:56.000000 wagtail_fedit-1.3.8/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:58:56.000000 wagtail_fedit-1.3.8/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 20:58:56.000000 wagtail_fedit-1.3.8/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 20:58:56.000000 wagtail_fedit-1.3.8/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.7/LICENSE` & `wagtail_fedit-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/PKG-INFO` & `wagtail_fedit-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.7
+Version: 1.3.8
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.7 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.8 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.7/README.md` & `wagtail_fedit-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/setup.cfg` & `wagtail_fedit-1.3.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
+00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.8/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.8/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.8/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/models.py` & `wagtail_fedit-1.3.8/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa1fe0f66 (Fri Apr  5 13:37:37 2024 UTC)
-files sz: 13783
+moddate:  0xe4651066 (Fri Apr  5 20:58:12 2024 UTC)
+files sz: 13781
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -221,32 +221,32 @@
    
    290         456 STORE_NAME              47 (do_render_fedit_field)
    
    340         458 LOAD_CONST              33 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 340>)
                460 MAKE_FUNCTION            0
                462 STORE_NAME              48 (render_editable_field)
    
-   380         464 LOAD_CONST              24 ('parser')
+   379         464 LOAD_CONST              24 ('parser')
                466 LOAD_NAME                7 (Parser)
                468 LOAD_CONST              34 ('kwarg_list')
                470 LOAD_NAME               49 (list)
                472 LOAD_NAME               50 (str)
                474 BINARY_SUBSCR
                484 LOAD_CONST              35 ('tokens')
                486 LOAD_NAME               49 (list)
                488 LOAD_NAME               50 (str)
                490 BINARY_SUBSCR
                500 LOAD_CONST              36 ('return')
                502 LOAD_NAME               51 (dict)
                504 BUILD_TUPLE              8
-               506 LOAD_CONST              37 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 380>)
+               506 LOAD_CONST              37 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 379>)
                508 MAKE_FUNCTION            4 (annotations)
                510 STORE_NAME              52 (get_kwargs)
    
-   407         512 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 407>)
+   406         512 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 406>)
                514 MAKE_FUNCTION            0
                516 STORE_NAME              53 (_get_from_context_or_set)
                518 LOAD_CONST              13 (None)
                520 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
@@ -1814,15 +1814,15 @@
          lnotab
             0x021222011e02040132010c022a010c01020102010201020102fb120804
             0216ff020232fe020364fd02042afc020604020c010401040102fd040402
             fc040502fb
       code
          argcount  : 5
          nlocals   : 10
-         stacksize : 15
+         stacksize : 10
          flags     : 11
          code
             0x8700970074010000000000000000000064017c027c036a010000000000
             0000006a0200000000000000007c036a0100000000000000006a03000000
             00000000007c036a0400000000000000006704ac02a6020000ab02000000
             00000000007d067c057225740b00000000000000000000740d0000000000
             00000000006a070000000000000000640e69007c05a4018e01a6010000ab
@@ -1830,20 +1830,21 @@
             00000000000000a6000000ab00000000000000000067017d087413000000
             000000000000006a0a0000000000000000741600000000000000000000a6
             010000ab01000000000000000044005d117d0902007c0989007c087c037c
             02ac04a6040000ab04000000000000000001008c1288006601640584087c
             084400a6000000ab0000000000000000007d087419000000000000000000
             00741b0000000000000000000064007c08a6020000ab0200000000000000
             00a6010000ab0100000000000000007d087c027c0564063c0000007c037c
-            0564073c000000741d0000000000000000000064087c067c027c037c017c
-            047c08741f000000000000000000007c05a0100000000000000000000000
-            0000000000000000006409640aa6020000ab020000000000000000a60100
-            00ab010000000000000000a0110000000000000000000000000000000000
-            000000a6000000ab000000000000000000640b6b0200000000640c9c077c
-            05a5018900ac0da6030000ab0300000000000000005300
+            0564073c000000741d000000000000000000007c05a00f00000000000000
+            0000000000000000000000000064086409a6020000ab0200000000000000
+            00a6010000ab010000000000000000a01000000000000000000000000000
+            00000000000000a6000000ab000000000000000000640a6b02000000007c
+            0564083c000000742300000000000000000000640b7c067c027c037c017c
+            047c08640c9c067c05a5018900ac0da6030000ab03000000000000000053
+            00
                        0 MAKE_CELL                0 (request)
          
          340           2 RESUME                   0
          
          341           4 LOAD_GLOBAL              1 (NULL + reverse)
          
          342          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
@@ -1943,58 +1944,61 @@
                      382 STORE_SUBSCR
          
          363         386 LOAD_FAST                3 (model)
                      388 LOAD_FAST                5 (kwargs)
                      390 LOAD_CONST               7 ('wagtail_fedit_instance')
                      392 STORE_SUBSCR
          
-         365         396 LOAD_GLOBAL             29 (NULL + render_to_string)
+         364         396 LOAD_GLOBAL             29 (NULL + str)
+                     408 LOAD_FAST                5 (kwargs)
+                     410 LOAD_METHOD             15 (get)
+                     432 LOAD_CONST               8 ('inline')
+                     434 LOAD_CONST               9 (False)
+                     436 PRECALL                  2
+                     440 CALL                     2
+                     450 PRECALL                  1
+                     454 CALL                     1
+                     464 LOAD_METHOD             16 (lower)
+                     486 PRECALL                  0
+                     490 CALL                     0
+                     500 LOAD_CONST              10 ('true')
+                     502 COMPARE_OP               2 (==)
+                     508 LOAD_FAST                5 (kwargs)
+                     510 LOAD_CONST               8 ('inline')
+                     512 STORE_SUBSCR
          
-         366         408 LOAD_CONST               8 ('wagtail_fedit/content/editable_field.html')
+         365         516 LOAD_GLOBAL             35 (NULL + render_to_string)
          
-         368         410 LOAD_FAST                6 (edit_url)
+         366         528 LOAD_CONST              11 ('wagtail_fedit/content/editable_field.html')
          
-         369         412 LOAD_FAST                2 (field_name)
+         368         530 LOAD_FAST                6 (edit_url)
          
-         370         414 LOAD_FAST                3 (model)
+         369         532 LOAD_FAST                2 (field_name)
          
-         371         416 LOAD_FAST                1 (content)
+         370         534 LOAD_FAST                3 (model)
          
-         372         418 LOAD_FAST                4 (context)
+         371         536 LOAD_FAST                1 (content)
          
-         373         420 LOAD_FAST                8 (items)
+         372         538 LOAD_FAST                4 (context)
          
-         374         422 LOAD_GLOBAL             31 (NULL + str)
-                     434 LOAD_FAST                5 (kwargs)
-                     436 LOAD_METHOD             16 (get)
-                     458 LOAD_CONST               9 ('inline')
-                     460 LOAD_CONST              10 (False)
-                     462 PRECALL                  2
-                     466 CALL                     2
-                     476 PRECALL                  1
-                     480 CALL                     1
-                     490 LOAD_METHOD             17 (lower)
-                     512 PRECALL                  0
-                     516 CALL                     0
-                     526 LOAD_CONST              11 ('true')
-                     528 COMPARE_OP               2 (==)
+         373         540 LOAD_FAST                8 (items)
          
-         367         534 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items', 'inline'))
-                     536 BUILD_CONST_KEY_MAP      7
+         367         542 LOAD_CONST              12 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
+                     544 BUILD_CONST_KEY_MAP      6
          
-         375         538 LOAD_FAST                5 (kwargs)
+         374         546 LOAD_FAST                5 (kwargs)
          
-         367         540 DICT_UPDATE              1
+         367         548 DICT_UPDATE              1
          
-         377         542 LOAD_DEREF               0 (request)
+         376         550 LOAD_DEREF               0 (request)
          
-         365         544 KW_NAMES                13
-                     546 PRECALL                  3
-                     550 CALL                     3
-                     560 RETURN_VALUE
+         365         552 KW_NAMES                13
+                     554 PRECALL                  3
+                     558 CALL                     3
+                     568 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
             '?'
             ('request', 'items', 'model', 'field_name')
             code
@@ -2027,32 +2031,32 @@
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
                firstlineno 359
                lnotab 0x
             'wagtail_fedit_field_name'
             'wagtail_fedit_instance'
-            'wagtail_fedit/content/editable_field.html'
             'inline'
             False
             'true'
-            ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items', 'inline')
+            'wagtail_fedit/content/editable_field.html'
+            ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
             ('request',)
             ()
-         names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'render_to_string', 'str', 'get', 'lower')
+         names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'str', 'get', 'lower', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
          firstlineno 340
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
-            013a020a010a020c01020202010201020102010201020170f9040802f802
-            0a02f4
+            013a020a010a0178010c0102020201020102010201020102fa040702f902
+            0902f5
       'kwarg_list'
       'tokens'
       'return'
       code
          argcount  : 3
          nlocals   : 9
          stacksize : 5
@@ -2065,89 +2069,89 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         380           0 RESUME                   0
+         379           0 RESUME                   0
          
-         381           2 LOAD_CONST               1 (False)
+         380           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         382           6 BUILD_MAP                0
+         381           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         387          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         386          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         388          50 LOAD_FAST                6 (token)
+         387          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         389          92 LOAD_GLOBAL              5 (NULL + len)
+         388          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         390         130 LOAD_FAST                3 (had_kwargs)
+         389         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         391         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         390         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         393     >>  164 LOAD_FAST                0 (parser)
+         392     >>  164 LOAD_FAST                0 (parser)
                      166 LOAD_METHOD              4 (compile_filter)
                      188 LOAD_FAST                6 (token)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 LOAD_FAST                4 (kwargs)
                      206 LOAD_FAST                1 (kwarg_list)
                      208 LOAD_FAST                5 (i)
                      210 BINARY_SUBSCR
                      220 STORE_SUBSCR
                      224 JUMP_BACKWARD           93 (to 40)
          
-         395     >>  226 LOAD_FAST                7 (split)
+         394     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         399         242 LOAD_FAST                0 (parser)
+         398         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         400         302 LOAD_CONST               6 (True)
+         399         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         402     >>  308 LOAD_FAST                4 (kwargs)
+         401     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -2155,74 +2159,74 @@
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 380
+         firstlineno 379
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 15
          code
             0x97007c017c00760072087c007c01190000000000000000005300740100
             0000000000000000007c02a6010000ab010000000000000000720802007c
             027c0369007c04a4018e017d027c027c007c013c0000007c025300
-         407           0 RESUME                   0
+         406           0 RESUME                   0
          
-         408           2 LOAD_FAST                1 (key)
+         407           2 LOAD_FAST                1 (key)
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
          
-         409          10 LOAD_FAST                0 (context)
+         408          10 LOAD_FAST                0 (context)
                       12 LOAD_FAST                1 (key)
                       14 BINARY_SUBSCR
                       24 RETURN_VALUE
          
-         411     >>   26 LOAD_GLOBAL              1 (NULL + callable)
+         410     >>   26 LOAD_GLOBAL              1 (NULL + callable)
                       38 LOAD_FAST                2 (value)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
          
-         412          56 PUSH_NULL
+         411          56 PUSH_NULL
                       58 LOAD_FAST                2 (value)
                       60 LOAD_FAST                3 (args)
                       62 BUILD_MAP                0
                       64 LOAD_FAST                4 (kwargs)
                       66 DICT_MERGE               1
                       68 CALL_FUNCTION_EX         1
                       70 STORE_FAST               2 (value)
          
-         414     >>   72 LOAD_FAST                2 (value)
+         413     >>   72 LOAD_FAST                2 (value)
                       74 LOAD_FAST                0 (context)
                       76 LOAD_FAST                1 (key)
                       78 STORE_SUBSCR
          
-         415          82 LOAD_FAST                2 (value)
+         414          82 LOAD_FAST                2 (value)
                       84 RETURN_VALUE
          consts
             None
          names      ('callable',)
          varnames   ('context', 'key', 'value', 'args', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_get_from_context_or_set'
-         firstlineno 407
+         firstlineno 406
          lnotab 0x0201080110021e0110020a01
       (None, False)
    names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'TokenType', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'simple_tag', 'bool', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0114010c010c010c010c010c020c010c010c010c0208
       021004100110061e011e03040104031c7f00422a010eff0e01023b2c010c
-      ff0e0102320628301b
+      ff0e0102320627301b
```

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.8/wagtail_fedit/templatetags/fedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,25 +357,24 @@
         hook(request=request, items=items, model=model, field_name=field_name)
 
     items = [item.render(request) for item in items]
     items = list(filter(None, items))
 
     kwargs["wagtail_fedit_field_name"] = field_name
     kwargs["wagtail_fedit_instance"] = model
-
+    kwargs["inline"] = str(kwargs.get("inline", False)).lower() == "true"
     return render_to_string(
         "wagtail_fedit/content/editable_field.html",
         {
             "edit_url": edit_url,
             "field_name": field_name,
             "model": model,
             "content": content,
             "parent_context": context,
             "toolbar_items": items,
-            "inline": str(kwargs.get("inline", False)).lower() == "true",
             **kwargs,
         },
         request=request,
     )
 
 def get_kwargs(parser: Parser, kwarg_list: list[str], tokens: list[str]) -> dict:
     had_kwargs = False
```

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.8/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.8/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/urls.py` & `wagtail_fedit-1.3.8/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.8/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.8/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.8/wagtail_fedit/views/editable.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 )
 from .. import forms as block_forms
 from ..utils import (
     FEDIT_PREVIEW_VAR,
     USERBAR_MODEL_VAR,
     FeditPermissionCheck,
     with_userbar_model,
-    user_can_publish,
-    user_can_unpublish,
-    user_can_submit_for_moderation,
-    lock_info,
+    # user_can_publish,
+    # user_can_unpublish,
+    # user_can_submit_for_moderation,
+    # lock_info,
 )
 
 from .mixins import (
     ObjectViewMixin,
     LockViewMixin,
 )
 
@@ -57,14 +57,16 @@
     if isinstance(object, Page):
         return PublishPageRevisionAction
     return PublishRevisionAction
 
 
 class BaseFeditView(ObjectViewMixin, FeditPermissionCheck, TemplateView):
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
+        if self.error_response:
+            return self.error_response
 
         if not self.has_perms(request, self.object):
             return HttpResponseForbidden("You do not have permission to view this page")
 
         if issubclass(self.model, RevisionMixin) and self.object.latest_revision_id:
             instance: RevisionMixin  = self.object
             revision: RevisionMixin = instance.latest_revision
```

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.8/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.3.8/wagtail_fedit/views/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             self.object = self.model._default_manager.get(pk=object_id)
             self.error_response = None
         except (LookupError):
             self.error_response = HttpResponseBadRequest("Invalid model provided")
         except (self.model.DoesNotExist):
             self.error_response = HttpResponseBadRequest("Model not found")
 
+
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         if self.error_response:
             return self.error_response
 
         return super().dispatch(request, object_id, app_label, model_name)
```

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.8/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.8/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.3.7
+Version: 1.3.8
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.7 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.8 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.7/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.8/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

