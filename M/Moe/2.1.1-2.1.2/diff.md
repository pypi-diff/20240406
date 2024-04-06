# Comparing `tmp/moe-2.1.1.tar.gz` & `tmp/moe-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moe-2.1.1.tar", max compression
+gzip compressed data, was "moe-2.1.2.tar", max compression
```

## Comparing `moe-2.1.1.tar` & `moe-2.1.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1066 2023-05-22 16:39:36.033294 moe-2.1.1/LICENSE
--rw-r--r--   0        0        0     3256 2023-05-22 16:39:36.033294 moe-2.1.1/README.rst
--rw-r--r--   0        0        0       38 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/README
--rw-r--r--   0        0        0     2008 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/alembic.ini
--rw-r--r--   0        0        0     2704 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/env.py
--rw-r--r--   0        0        0      495 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/script.py.mako
--rw-r--r--   0        0        0      744 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/0ce5960a081e_new_field_catalog_nums.py
--rw-r--r--   0        0        0      587 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/30668259fcd6_new_field_country.py
--rw-r--r--   0        0        0      599 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/32e9fea590b7_new_field_track_total.py
--rw-r--r--   0        0        0      581 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/60608d9d2908_new_field_media.py
--rw-r--r--   0        0        0     3185 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/6d4e785df5cb_initial_generation.py
--rw-r--r--   0        0        0      581 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/817440447857_new_field_label.py
--rw-r--r--   0        0        0      605 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/880c5a2d80ed_remove_audio_format_field.py
--rw-r--r--   0        0        0      601 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/ab11c34c1d0b_new_field_audio_format.py
--rw-r--r--   0        0        0     1154 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/ab5db9861d30_rename_custom_fields.py
--rw-r--r--   0        0        0     5698 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/bf49ac6805f7_json_multi_value_fields.py
--rw-r--r--   0        0        0      597 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/db3a470892c6_new_field_og_date.py
--rw-r--r--   0        0        0      586 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/eb8c7e20a080_new_field_barcode.py
--rw-r--r--   0        0        0      723 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/fe0956c93730_new_field_artists.py
--rw-r--r--   0        0        0      443 2023-05-22 16:39:36.037294 moe-2.1.1/moe/__init__.py
--rw-r--r--   0        0        0      430 2023-05-22 16:39:36.037294 moe-2.1.1/moe/add/__init__.py
--rw-r--r--   0        0        0     3736 2023-05-22 16:39:36.037294 moe-2.1.1/moe/add/add_cli.py
--rw-r--r--   0        0        0     2154 2023-05-22 16:39:36.037294 moe-2.1.1/moe/add/add_core.py
--rwxr-xr-x   0        0        0     4870 2023-05-22 16:39:36.037294 moe-2.1.1/moe/cli.py
--rw-r--r--   0        0        0    15584 2023-05-22 16:39:36.037294 moe-2.1.1/moe/config.py
--rw-r--r--   0        0        0      514 2023-05-22 16:39:36.037294 moe-2.1.1/moe/duplicate/__init__.py
--rw-r--r--   0        0        0     7141 2023-05-22 16:39:36.037294 moe-2.1.1/moe/duplicate/dup_cli.py
--rw-r--r--   0        0        0     5827 2023-05-22 16:39:36.037294 moe-2.1.1/moe/duplicate/dup_core.py
--rw-r--r--   0        0        0      454 2023-05-22 16:39:36.037294 moe-2.1.1/moe/edit/__init__.py
--rw-r--r--   0        0        0     2135 2023-05-22 16:39:36.037294 moe-2.1.1/moe/edit/edit_cli.py
--rw-r--r--   0        0        0     1801 2023-05-22 16:39:36.037294 moe-2.1.1/moe/edit/edit_core.py
--rw-r--r--   0        0        0      311 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/__init__.py
--rw-r--r--   0        0        0    19001 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/album.py
--rw-r--r--   0        0        0     5497 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/extra.py
--rw-r--r--   0        0        0    10090 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/lib_item.py
--rw-r--r--   0        0        0    16982 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/track.py
--rw-r--r--   0        0        0     4421 2023-05-22 16:39:36.037294 moe-2.1.1/moe/list.py
--rw-r--r--   0        0        0      544 2023-05-22 16:39:36.037294 moe-2.1.1/moe/moe_import/__init__.py
--rw-r--r--   0        0        0    12282 2023-05-22 16:39:36.037294 moe-2.1.1/moe/moe_import/import_cli.py
--rw-r--r--   0        0        0     3852 2023-05-22 16:39:36.037294 moe-2.1.1/moe/moe_import/import_core.py
--rw-r--r--   0        0        0      472 2023-05-22 16:39:36.037294 moe-2.1.1/moe/move/__init__.py
--rw-r--r--   0        0        0     2506 2023-05-22 16:39:36.037294 moe-2.1.1/moe/move/move_cli.py
--rw-r--r--   0        0        0    10415 2023-05-22 16:39:36.037294 moe-2.1.1/moe/move/move_core.py
--rw-r--r--   0        0        0        0 2023-05-22 16:39:36.037294 moe-2.1.1/moe/py.typed
--rw-r--r--   0        0        0     7053 2023-05-22 16:39:36.037294 moe-2.1.1/moe/query.py
--rw-r--r--   0        0        0      462 2023-05-22 16:39:36.037294 moe-2.1.1/moe/read/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-22 16:39:36.037294 moe-2.1.1/moe/read/read_cli.py
--rw-r--r--   0        0        0      818 2023-05-22 16:39:36.037294 moe-2.1.1/moe/read/read_core.py
--rw-r--r--   0        0        0      450 2023-05-22 16:39:36.037294 moe-2.1.1/moe/remove/__init__.py
--rw-r--r--   0        0        0     1475 2023-05-22 16:39:36.037294 moe-2.1.1/moe/remove/rm_cli.py
--rw-r--r--   0        0        0     1228 2023-05-22 16:39:36.037294 moe-2.1.1/moe/remove/rm_core.py
--rw-r--r--   0        0        0       62 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/__init__.py
--rw-r--r--   0        0        0      209 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/cli/__init__.py
--rw-r--r--   0        0        0     2131 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/cli/prompt.py
--rw-r--r--   0        0        0     2609 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/cli/query.py
--rw-r--r--   0        0        0      153 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/core/__init__.py
--rw-r--r--   0        0        0     5651 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/core/match.py
--rw-r--r--   0        0        0     3033 2023-05-22 16:39:36.037294 moe-2.1.1/moe/write.py
--rw-r--r--   0        0        0     2114 2023-05-22 16:39:36.041294 moe-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 moe-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-06 19:51:12.110586 moe-2.1.2/LICENSE
+-rw-r--r--   0        0        0     3244 2024-04-06 19:51:12.110586 moe-2.1.2/README.rst
+-rw-r--r--   0        0        0       38 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/README
+-rw-r--r--   0        0        0     2008 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/alembic.ini
+-rw-r--r--   0        0        0     2704 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/env.py
+-rw-r--r--   0        0        0      495 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/script.py.mako
+-rw-r--r--   0        0        0      745 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/0ce5960a081e_new_field_catalog_nums.py
+-rw-r--r--   0        0        0      588 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/30668259fcd6_new_field_country.py
+-rw-r--r--   0        0        0      600 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/32e9fea590b7_new_field_track_total.py
+-rw-r--r--   0        0        0      582 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/60608d9d2908_new_field_media.py
+-rw-r--r--   0        0        0     3186 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/6d4e785df5cb_initial_generation.py
+-rw-r--r--   0        0        0      582 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/817440447857_new_field_label.py
+-rw-r--r--   0        0        0      606 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/880c5a2d80ed_remove_audio_format_field.py
+-rw-r--r--   0        0        0      602 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/ab11c34c1d0b_new_field_audio_format.py
+-rw-r--r--   0        0        0     1155 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/ab5db9861d30_rename_custom_fields.py
+-rw-r--r--   0        0        0     5699 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/bf49ac6805f7_json_multi_value_fields.py
+-rw-r--r--   0        0        0      598 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/db3a470892c6_new_field_og_date.py
+-rw-r--r--   0        0        0      587 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/eb8c7e20a080_new_field_barcode.py
+-rw-r--r--   0        0        0      724 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/fe0956c93730_new_field_artists.py
+-rw-r--r--   0        0        0      443 2024-04-06 19:51:12.114586 moe-2.1.2/moe/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-06 19:51:12.114586 moe-2.1.2/moe/add/__init__.py
+-rw-r--r--   0        0        0     3736 2024-04-06 19:51:12.114586 moe-2.1.2/moe/add/add_cli.py
+-rw-r--r--   0        0        0     2154 2024-04-06 19:51:12.114586 moe-2.1.2/moe/add/add_core.py
+-rwxr-xr-x   0        0        0     4863 2024-04-06 19:51:12.114586 moe-2.1.2/moe/cli.py
+-rw-r--r--   0        0        0    15593 2024-04-06 19:51:12.114586 moe-2.1.2/moe/config.py
+-rw-r--r--   0        0        0      514 2024-04-06 19:51:12.114586 moe-2.1.2/moe/duplicate/__init__.py
+-rw-r--r--   0        0        0     7141 2024-04-06 19:51:12.114586 moe-2.1.2/moe/duplicate/dup_cli.py
+-rw-r--r--   0        0        0     5841 2024-04-06 19:51:12.114586 moe-2.1.2/moe/duplicate/dup_core.py
+-rw-r--r--   0        0        0      454 2024-04-06 19:51:12.114586 moe-2.1.2/moe/edit/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-06 19:51:12.114586 moe-2.1.2/moe/edit/edit_cli.py
+-rw-r--r--   0        0        0     1801 2024-04-06 19:51:12.114586 moe-2.1.2/moe/edit/edit_core.py
+-rw-r--r--   0        0        0      311 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/__init__.py
+-rw-r--r--   0        0        0    19002 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/album.py
+-rw-r--r--   0        0        0     5499 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/extra.py
+-rw-r--r--   0        0        0    10209 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/lib_item.py
+-rw-r--r--   0        0        0    16985 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/track.py
+-rw-r--r--   0        0        0     4421 2024-04-06 19:51:12.114586 moe-2.1.2/moe/list.py
+-rw-r--r--   0        0        0      544 2024-04-06 19:51:12.114586 moe-2.1.2/moe/moe_import/__init__.py
+-rw-r--r--   0        0        0    12282 2024-04-06 19:51:12.114586 moe-2.1.2/moe/moe_import/import_cli.py
+-rw-r--r--   0        0        0     3852 2024-04-06 19:51:12.114586 moe-2.1.2/moe/moe_import/import_core.py
+-rw-r--r--   0        0        0      472 2024-04-06 19:51:12.114586 moe-2.1.2/moe/move/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-06 19:51:12.114586 moe-2.1.2/moe/move/move_cli.py
+-rw-r--r--   0        0        0    10415 2024-04-06 19:51:12.114586 moe-2.1.2/moe/move/move_core.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:51:12.114586 moe-2.1.2/moe/py.typed
+-rw-r--r--   0        0        0     7053 2024-04-06 19:51:12.114586 moe-2.1.2/moe/query.py
+-rw-r--r--   0        0        0      462 2024-04-06 19:51:12.114586 moe-2.1.2/moe/read/__init__.py
+-rw-r--r--   0        0        0     1619 2024-04-06 19:51:12.114586 moe-2.1.2/moe/read/read_cli.py
+-rw-r--r--   0        0        0      818 2024-04-06 19:51:12.114586 moe-2.1.2/moe/read/read_core.py
+-rw-r--r--   0        0        0      450 2024-04-06 19:51:12.114586 moe-2.1.2/moe/remove/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-06 19:51:12.118586 moe-2.1.2/moe/remove/rm_cli.py
+-rw-r--r--   0        0        0     1228 2024-04-06 19:51:12.118586 moe-2.1.2/moe/remove/rm_core.py
+-rw-r--r--   0        0        0       62 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/cli/__init__.py
+-rw-r--r--   0        0        0     2131 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/cli/prompt.py
+-rw-r--r--   0        0        0     2609 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/cli/query.py
+-rw-r--r--   0        0        0      153 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/core/__init__.py
+-rw-r--r--   0        0        0     5651 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/core/match.py
+-rw-r--r--   0        0        0     3033 2024-04-06 19:51:12.118586 moe-2.1.2/moe/write.py
+-rw-r--r--   0        0        0     2144 2024-04-06 19:51:12.118586 moe-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 moe-2.1.2/PKG-INFO
```

### Comparing `moe-2.1.1/LICENSE` & `moe-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/README.rst` & `moe-2.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,35 +23,35 @@
 As previously mentioned, all of Moe's music management logic and functionality is also available as a python library. As an example, below is a standalone script that takes an album directory and Musicbrainz release ID from the command-line, and then updates the underlying files' tags with any changes from Musicbrainz.
 
 .. code:: python
 
     #!/usr/bin/env python3
 
     import argparse
-    import pathlib
+    from pathlib import Path
 
     from moe.config import Config, ConfigValidationError
     from moe.library import Album
     from moe.write import write_tags
     import moe_musicbrainz
 
     def main():
         try:
-            config.Config(config_dir=Path.home() / ".config" / "my_script", init_db=False)
-        except config.ConfigValidationError as err:
+            Config(config_dir=Path.home() / ".config" / "my_script", init_db=False)
+        except ConfigValidationError as err:
             raise SystemExit(1) from err
 
         parser = argparse.ArgumentParser(
             description="Update an album with musicbrainz tags."
         )
         parser.add_argument("path", help="dir of the album to update")
         parser.add_argument("mb_id", help="musicbrainz id of the album to fetch")
         args = parser.parse_args()
 
-        album = Album.from_dir(pathlib.Path(args.path))
+        album = Album.from_dir(Path(args.path))
 
         album.merge(moe_musicbrainz.get_album_by_id(args.mb_id), overwrite=True)
 
         for track in album.tracks:
             write_tags(track)
```

### Comparing `moe-2.1.1/alembic/alembic.ini` & `moe-2.1.2/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/alembic/env.py` & `moe-2.1.2/alembic/env.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/alembic/versions/0ce5960a081e_new_field_catalog_nums.py` & `moe-2.1.2/alembic/versions/0ce5960a081e_new_field_catalog_nums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """new field catalog_nums.
 
 Revision ID: 0ce5960a081e
 Revises: 32e9fea590b7
 Create Date: 2022-10-12 16:13:33.297005
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "0ce5960a081e"
 down_revision = "32e9fea590b7"
```

### Comparing `moe-2.1.1/alembic/versions/30668259fcd6_new_field_country.py` & `moe-2.1.2/alembic/versions/32e9fea590b7_new_field_track_total.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-"""new field: country.
+"""new field track_total.
 
-Revision ID: 30668259fcd6
-Revises: 60608d9d2908
-Create Date: 2022-10-06 20:35:34.296797
+Revision ID: 32e9fea590b7
+Revises: eb8c7e20a080
+Create Date: 2022-10-12 13:59:57.620933
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
-revision = "30668259fcd6"
-down_revision = "60608d9d2908"
+revision = "32e9fea590b7"
+down_revision = "eb8c7e20a080"
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.add_column(sa.Column("country", sa.String(), nullable=True))
+        batch_op.add_column(sa.Column("track_total", sa.Integer(), nullable=True))
 
 
 def downgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.drop_column("country")
+        batch_op.drop_column("track_total")
```

### Comparing `moe-2.1.1/alembic/versions/32e9fea590b7_new_field_track_total.py` & `moe-2.1.2/alembic/versions/817440447857_new_field_label.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-"""new field track_total.
+"""new field: label.
 
-Revision ID: 32e9fea590b7
-Revises: eb8c7e20a080
-Create Date: 2022-10-12 13:59:57.620933
+Revision ID: 817440447857
+Revises: 30668259fcd6
+Create Date: 2022-10-06 20:39:23.733361
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
-revision = "32e9fea590b7"
-down_revision = "eb8c7e20a080"
+revision = "817440447857"
+down_revision = "30668259fcd6"
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.add_column(sa.Column("track_total", sa.Integer(), nullable=True))
+        batch_op.add_column(sa.Column("label", sa.String(), nullable=True))
 
 
 def downgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.drop_column("track_total")
+        batch_op.drop_column("label")
```

### Comparing `moe-2.1.1/alembic/versions/60608d9d2908_new_field_media.py` & `moe-2.1.2/alembic/versions/60608d9d2908_new_field_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """new field: media.
 
 Revision ID: 60608d9d2908
 Revises: fe0956c93730
 Create Date: 2022-10-06 20:26:02.640360
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "60608d9d2908"
 down_revision = "fe0956c93730"
```

### Comparing `moe-2.1.1/alembic/versions/6d4e785df5cb_initial_generation.py` & `moe-2.1.2/alembic/versions/6d4e785df5cb_initial_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """initial generation.
 
 Revision ID: 6d4e785df5cb
 Revises: 
 Create Date: 2022-09-27 19:19:39.281403
 
 """
+
 import sqlalchemy as sa
 from sqlalchemy.ext.mutable import MutableDict
 
 import moe
 from alembic import op
 
 # revision identifiers, used by Alembic.
```

### Comparing `moe-2.1.1/alembic/versions/817440447857_new_field_label.py` & `moe-2.1.2/alembic/versions/db3a470892c6_new_field_og_date.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-"""new field: label.
+"""new field: og_date.
 
-Revision ID: 817440447857
-Revises: 30668259fcd6
-Create Date: 2022-10-06 20:39:23.733361
+Revision ID: db3a470892c6
+Revises: 817440447857
+Create Date: 2022-10-08 06:20:42.841502
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
-revision = "817440447857"
-down_revision = "30668259fcd6"
+revision = "db3a470892c6"
+down_revision = "817440447857"
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.add_column(sa.Column("label", sa.String(), nullable=True))
+        batch_op.add_column(sa.Column("original_date", sa.Date(), nullable=True))
 
 
 def downgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.drop_column("label")
+        batch_op.drop_column("original_date")
```

### Comparing `moe-2.1.1/alembic/versions/880c5a2d80ed_remove_audio_format_field.py` & `moe-2.1.2/alembic/versions/880c5a2d80ed_remove_audio_format_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """remove audio_format field.
 
 Revision ID: 880c5a2d80ed
 Revises: bf49ac6805f7
 Create Date: 2022-11-01 13:41:12.407819
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "880c5a2d80ed"
 down_revision = "bf49ac6805f7"
```

### Comparing `moe-2.1.1/alembic/versions/ab11c34c1d0b_new_field_audio_format.py` & `moe-2.1.2/alembic/versions/ab11c34c1d0b_new_field_audio_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """new field audio_format.
 
 Revision ID: ab11c34c1d0b
 Revises: 0ce5960a081e
 Create Date: 2022-10-13 15:55:35.303129
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "ab11c34c1d0b"
 down_revision = "0ce5960a081e"
```

### Comparing `moe-2.1.1/alembic/versions/ab5db9861d30_rename_custom_fields.py` & `moe-2.1.2/alembic/versions/ab5db9861d30_rename_custom_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Rename custom fields.
 
 Revision ID: ab5db9861d30
 Revises: 880c5a2d80ed
 Create Date: 2022-12-11 15:24:10.227924
 
 """
+
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "ab5db9861d30"
 down_revision = "880c5a2d80ed"
 branch_labels = None
 depends_on = None
```

### Comparing `moe-2.1.1/alembic/versions/bf49ac6805f7_json_multi_value_fields.py` & `moe-2.1.2/alembic/versions/bf49ac6805f7_json_multi_value_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """json multi value fields.
 
 Revision ID: bf49ac6805f7
 Revises: ab11c34c1d0b
 Create Date: 2022-10-17 21:09:09.265544
 
 """
+
 import sqlalchemy as sa
 from sqlalchemy.ext.mutable import MutableSet
 from sqlalchemy.orm import Session, declarative_base
 
 from alembic import op
 from moe.library.lib_item import SetType
```

### Comparing `moe-2.1.1/alembic/versions/db3a470892c6_new_field_og_date.py` & `moe-2.1.2/alembic/versions/30668259fcd6_new_field_country.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-"""new field: og_date.
+"""new field: country.
 
-Revision ID: db3a470892c6
-Revises: 817440447857
-Create Date: 2022-10-08 06:20:42.841502
+Revision ID: 30668259fcd6
+Revises: 60608d9d2908
+Create Date: 2022-10-06 20:35:34.296797
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
-revision = "db3a470892c6"
-down_revision = "817440447857"
+revision = "30668259fcd6"
+down_revision = "60608d9d2908"
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.add_column(sa.Column("original_date", sa.Date(), nullable=True))
+        batch_op.add_column(sa.Column("country", sa.String(), nullable=True))
 
 
 def downgrade():
     with op.batch_alter_table("album", schema=None) as batch_op:
-        batch_op.drop_column("original_date")
+        batch_op.drop_column("country")
```

### Comparing `moe-2.1.1/alembic/versions/eb8c7e20a080_new_field_barcode.py` & `moe-2.1.2/alembic/versions/eb8c7e20a080_new_field_barcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """new field barcode.
 
 Revision ID: eb8c7e20a080
 Revises: db3a470892c6
 Create Date: 2022-10-11 14:51:44.788096
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "eb8c7e20a080"
 down_revision = "db3a470892c6"
```

### Comparing `moe-2.1.1/alembic/versions/fe0956c93730_new_field_artists.py` & `moe-2.1.2/alembic/versions/fe0956c93730_new_field_artists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """new field: artists.
 
 Revision ID: fe0956c93730
 Revises: 6d4e785df5cb
 Create Date: 2022-10-06 18:26:11.939381
 
 """
+
 import sqlalchemy as sa
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = "fe0956c93730"
 down_revision = "6d4e785df5cb"
```

### Comparing `moe-2.1.1/moe/add/add_cli.py` & `moe-2.1.2/moe/add/add_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/add/add_core.py` & `moe-2.1.2/moe/add/add_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/cli.py` & `moe-2.1.2/moe/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """Entry point for the CLI.
 
 This module deals with parsing the arguments of ``moe`` and related functionality.
 For general shared CLI functionality, see the ``moe.util.cli`` package.
 """
 
 import argparse
+import importlib.metadata
 import logging
 import sys
 
-import pkg_resources
 import pluggy
 from rich.console import Console
 
 import moe
 from moe import config
 from moe.config import Config, ConfigValidationError, moe_sessionmaker
 
@@ -114,15 +114,15 @@
         except SystemExit:
             session.commit()
             raise
 
 
 def _create_arg_parser() -> argparse.ArgumentParser:
     """Creates the root argument parser."""
-    version = pkg_resources.get_distribution("moe").version
+    version = importlib.metadata.version("moe")
 
     moe_parser = argparse.ArgumentParser()
     moe_parser.add_argument(
         "--version", action="version", version=f"%(prog)s v{version}"
     )
     moe_parser.add_argument(
         "--verbose",
```

### Comparing `moe-2.1.1/moe/config.py` & `moe-2.1.2/moe/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     * `The sqlalchemy Session docs
       <https://docs.sqlalchemy.org/en/20/orm/session_basics.html#session-basics>`
     * ``moe/cli.py`` for an example on how the CLI handles creating the configuration
       and database connection via the session.
 """
 
 import importlib
-import importlib.metadata
 import importlib.util
 import logging
 import os
 import re
 import sys
 from pathlib import Path
 from types import ModuleType
 from typing import Any, NamedTuple, Optional, Union, cast
 
 import dynaconf
 import dynaconf.base
 import dynaconf.validator
+import importlib_metadata
 import pluggy
 import sqlalchemy
 import sqlalchemy.event
 import sqlalchemy.orm
 
 import alembic.command
 import alembic.config
@@ -400,15 +400,15 @@
         if Path(self.config_dir / "plugins").exists():
             sys.path.append(str(self.config_dir / "plugins"))
             self._register_local_plugins(
                 self.enabled_plugins, self.config_dir / "plugins"
             )
 
         # register all third-party installed plugins
-        plugins = importlib.metadata.entry_points().get("moe.plugins")
+        plugins = importlib_metadata.entry_points().select(group="moe.plugins")
         if plugins:
             for plugin in plugins:
                 if plugin.name in self.enabled_plugins:
                     self.pm.register(plugin.load(), plugin.name)
 
         # register plugin hookimpls for all extra plugins
         for extra_plugin in self._extra_plugins:
```

### Comparing `moe-2.1.1/moe/duplicate/__init__.py` & `moe-2.1.2/moe/duplicate/__init__.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/duplicate/dup_cli.py` & `moe-2.1.2/moe/duplicate/dup_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/duplicate/dup_core.py` & `moe-2.1.2/moe/duplicate/dup_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,13 +158,13 @@
     dup_items = []
     if not others:
         others = query(session, "*", type(item).__name__.lower())
 
     for other in others:
         if (
             item is not other
-            and type(item) == type(other)
+            and type(item) == type(other)  # noqa: E721
             and not item.is_unique(other)
         ):
             dup_items.append(other)
 
     return dup_items
```

### Comparing `moe-2.1.1/moe/edit/edit_cli.py` & `moe-2.1.2/moe/edit/edit_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/edit/edit_core.py` & `moe-2.1.2/moe/edit/edit_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/library/album.py` & `moe-2.1.2/moe/library/album.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,17 +203,17 @@
             ):
                 self.custom[custom_field] = other_value
 
         log.debug(
             f"MetaAlbums merged. [album_a={self!r}, album_b={other!r}, {overwrite=}]"
         )
 
-    def __eq__(self, other: "MetaAlbum") -> bool:
+    def __eq__(self, other) -> bool:
         """Compares MetaAlbums by their fields."""
-        if type(self) != type(other):
+        if type(self) != type(other):  # noqa: E721
             return False
 
         for field in self.fields:
             if not hasattr(other, field) or (
                 getattr(self, field) != getattr(other, field)
             ):
                 return False
```

### Comparing `moe-2.1.1/moe/library/extra.py` & `moe-2.1.2/moe/library/extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return {"album", "path"}
 
     @property
     def rel_path(self) -> PurePath:
         """Returns the extra's path relative to its album's path."""
         return self.path.relative_to(self.album.path)
 
-    def is_unique(self, other: "Extra") -> bool:
+    def is_unique(self, other: "LibItem") -> bool:
         """Returns whether an extra is unique in the library from ``other``."""
         if self.path == other.path:
             return False
 
         custom_uniqueness = config.CONFIG.pm.hook.is_unique_extra(
             extra=self, other=other
         )
```

### Comparing `moe-2.1.1/moe/library/lib_item.py` & `moe-2.1.2/moe/library/lib_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,52 +227,61 @@
     """
 
     impl = sqlalchemy.types.String  # sql type
     cache_ok = True  # expected to produce same bind/result behavior and sql generation
 
     library_path: Path  # will be set on config initialization
 
-    def process_bind_param(self, pathlib_path, dialect):
+    def process_bind_param(self, value, dialect):
         """Normalize pathlib paths as strings for the database.
 
         Args:
-            pathlib_path: Inbound path to the db.
+            value: Inbound path to the db.
             dialect: Database in use.
 
         Returns:
             Relative path from ``library_path`` if possible, otherwise stores the
             absolute path.
         """
+        assert isinstance(value, Path)
+        pathlib_path: Path = value
+
         try:
             return str(pathlib_path.relative_to(self.library_path))
         except ValueError:
             return str(pathlib_path.resolve())
 
-    def process_result_value(self, path_str, dialect):
+    def process_result_value(self, value, dialect):
         """Convert the path back to a Path object on the way out."""
+        path_str = value
+
         if path_str is None:
             return None
 
         return Path(self.library_path / path_str)
 
 
 class SetType(sqlalchemy.types.TypeDecorator):
     """A custom type for storing sets as json in a database."""
 
     impl = sqlalchemy.types.JSON  # sql type
     cache_ok = True  # expected to produce same bind/result behavior and sql generation
 
-    def process_bind_param(self, json_set, dialect):
+    def process_bind_param(self, value, dialect):
         """Convert the set to a list so it's valid json."""
+        json_set = value
+
         if json_set is not None:
             return list(json_set)
         return None
 
-    def process_result_value(self, json_list, dialect):
+    def process_result_value(self, value, dialect):
         """Convert the list in the db back to a set."""
+        json_list = value
+
         if json_list is not None:
             return set(json_list)
         return None
 
 
 class MetaLibItem:
     """Base class for MetaTrack and MetaAlbum objects representing metadata-only.
@@ -302,10 +311,10 @@
 
 class LibItem(MetaLibItem):
     """Base class for library items i.e. Albums, Extras, and Tracks."""
 
     _id: Mapped[int] = mapped_column(Integer, primary_key=True)
     path: Mapped[Path] = mapped_column(PathType, nullable=False, unique=True)
 
-    def is_unique(self, other: "LibItem") -> bool:
+    def is_unique(self, other) -> bool:
         """Returns whether an item is unique in the library from ``other``."""
         raise NotImplementedError
```

### Comparing `moe-2.1.1/moe/library/track.py` & `moe-2.1.2/moe/library/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             ):
                 self.custom[custom_field] = other_value
 
         log.debug(f"Tracks merged. [track_a={self!r}, track_b={other!r}, {overwrite=}]")
 
     def __eq__(self, other) -> bool:
         """Compares Tracks by their fields."""
-        if type(self) != type(other):
+        if not isinstance(other, Track):
             return False
 
         for field in self.fields:
             if not hasattr(other, field) or (
                 getattr(self, field) != getattr(other, field)
             ):
                 return False
```

### Comparing `moe-2.1.1/moe/list.py` & `moe-2.1.2/moe/list.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/moe_import/__init__.py` & `moe-2.1.2/moe/moe_import/__init__.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/moe_import/import_cli.py` & `moe-2.1.2/moe/moe_import/import_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/moe_import/import_core.py` & `moe-2.1.2/moe/moe_import/import_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/move/move_cli.py` & `moe-2.1.2/moe/move/move_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/move/move_core.py` & `moe-2.1.2/moe/move/move_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/query.py` & `moe-2.1.2/moe/query.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/read/read_cli.py` & `moe-2.1.2/moe/read/read_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/read/read_core.py` & `moe-2.1.2/moe/read/read_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/remove/rm_cli.py` & `moe-2.1.2/moe/remove/rm_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/remove/rm_core.py` & `moe-2.1.2/moe/remove/rm_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/util/cli/prompt.py` & `moe-2.1.2/moe/util/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/util/cli/query.py` & `moe-2.1.2/moe/util/cli/query.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/util/core/match.py` & `moe-2.1.2/moe/util/core/match.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/moe/write.py` & `moe-2.1.2/moe/write.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.1/pyproject.toml` & `moe-2.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "Moe"
 include = ["alembic/*", "alembic/versions/*"]
-version = "2.1.1"
+version = "2.1.2"
 description = "The ultimate tool for managing your music library."
 authors = ["Jacob Pavlock <jtpavlock@gmail.com>"]
 repository = "https://github.com/MoeMusic/Moe"
 documentation = "https://mrmoe.readthedocs.io/en/latest/index.html"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -14,56 +14,57 @@
 readme = "README.rst"
 license = "MIT"
 
 [tool.poetry.scripts]
 moe = 'moe.cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.12"
+python = ">=3.9, <3.13"
 alembic = "^1.4.2"
 dynaconf = "^3.1.4"
 mediafile = "^0.11.0"
 musicbrainzngs = "^0.7.1"
-pluggy = "^1.0.0"
+pluggy = "^1.3.0"
 rich = "^13.0.0"
 SQLAlchemy = "^2.0.0"
 Unidecode = "^1.2.0"
-questionary = "^1.9.0"
+questionary = "^2.0.0"
+importlib-metadata = "^7.0.1"
 
 [tool.poetry.group.test.dependencies]
 debugpy = "^1.4.1"
-pytest = "^7.0.0"
+pytest = "^8.0.0"
 pytest-cov = "^4.0.0"
 tox = "^4.0.0"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.0.0"
+black = "^24.0.0"
 commitizen = "^3.0.0"
 darglint = "^1.8.1"
-flake8 = "^6.0.0"
+flake8 = "^7.0.0"
 flake8-alphabetize = "^0.0.19"
-flake8-bugbear = "^23.0.0"
+flake8-bugbear = "^24.0.0"
 flake8-comprehensions = "^3.10.0"
 flake8-docstrings = "^1.5.0"
 flake8-pytest-style = "^1.6.0"
 flake8-use-fstring = "^1.1"
 "github3.py" = "^3.2.0"
 isort = "^5.10.1"
 mccabe = "^0.7.0"
 pre-commit = "^3.0.0"
 pyright = "^1.1.267"
 
 [tool.poetry.group.docs.dependencies]
 furo = "*"
 pypandoc = "^1.9"
-Sphinx = "^6.0.0"
+Sphinx = "^7.0.0"
 
 [tool.commitizen]
 name = "cz_customize"
-version = "2.1.1"
+version = "2.1.2"
 version_files = [
     "pyproject.toml:^version",
 ]
 tag_format = "v$version"
 
 [tool.commitizen.customize]
 schema_pattern = '(build|ci|deprecate|docs|feat|fix|perf|refactor|release|style|test)(\(\w+\))?!?:\s\S.*'
```

### Comparing `moe-2.1.1/PKG-INFO` & `moe-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
-Name: moe
-Version: 2.1.1
+Name: Moe
+Version: 2.1.2
 Summary: The ultimate tool for managing your music library.
 Home-page: https://github.com/MoeMusic/Moe
 License: MIT
 Author: Jacob Pavlock
 Author-email: jtpavlock@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Requires-Dist: SQLAlchemy (>=2.0.0,<3.0.0)
 Requires-Dist: Unidecode (>=1.2.0,<2.0.0)
 Requires-Dist: alembic (>=1.4.2,<2.0.0)
 Requires-Dist: dynaconf (>=3.1.4,<4.0.0)
+Requires-Dist: importlib-metadata (>=7.0.1,<8.0.0)
 Requires-Dist: mediafile (>=0.11.0,<0.12.0)
 Requires-Dist: musicbrainzngs (>=0.7.1,<0.8.0)
-Requires-Dist: pluggy (>=1.0.0,<2.0.0)
-Requires-Dist: questionary (>=1.9.0,<2.0.0)
+Requires-Dist: pluggy (>=1.3.0,<2.0.0)
+Requires-Dist: questionary (>=2.0.0,<3.0.0)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
 Project-URL: Documentation, https://mrmoe.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/MoeMusic/Moe
 Description-Content-Type: text/x-rst
 
 ###############
 Welcome to Moe!
@@ -52,35 +54,35 @@
 As previously mentioned, all of Moe's music management logic and functionality is also available as a python library. As an example, below is a standalone script that takes an album directory and Musicbrainz release ID from the command-line, and then updates the underlying files' tags with any changes from Musicbrainz.
 
 .. code:: python
 
     #!/usr/bin/env python3
 
     import argparse
-    import pathlib
+    from pathlib import Path
 
     from moe.config import Config, ConfigValidationError
     from moe.library import Album
     from moe.write import write_tags
     import moe_musicbrainz
 
     def main():
         try:
-            config.Config(config_dir=Path.home() / ".config" / "my_script", init_db=False)
-        except config.ConfigValidationError as err:
+            Config(config_dir=Path.home() / ".config" / "my_script", init_db=False)
+        except ConfigValidationError as err:
             raise SystemExit(1) from err
 
         parser = argparse.ArgumentParser(
             description="Update an album with musicbrainz tags."
         )
         parser.add_argument("path", help="dir of the album to update")
         parser.add_argument("mb_id", help="musicbrainz id of the album to fetch")
         args = parser.parse_args()
 
-        album = Album.from_dir(pathlib.Path(args.path))
+        album = Album.from_dir(Path(args.path))
 
         album.merge(moe_musicbrainz.get_album_by_id(args.mb_id), overwrite=True)
 
         for track in album.tracks:
             write_tags(track)
```

