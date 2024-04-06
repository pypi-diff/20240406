# Comparing `tmp/avtomat_aws-0.0.3.tar.gz` & `tmp/avtomat_aws-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.0.3.tar", max compression
+gzip compressed data, was "avtomat_aws-0.1.1.tar", max compression
```

## Comparing `avtomat_aws-0.0.3.tar` & `avtomat_aws-0.1.1.tar`

### file list

```diff
@@ -1,115 +1,117 @@
--rw-r--r--   0        0        0      128 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/LICENSE
--rw-r--r--   0        0        0     3512 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/README.md
--rw-r--r--   0        0        0       69 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1495 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      833 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      897 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1125 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1114 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1269 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      824 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0      687 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      657 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      803 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      472 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      451 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1203 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1369 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      634 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1401 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1172 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      481 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1207 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      899 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      823 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1220 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1100 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      793 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      816 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      760 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      750 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      468 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      701 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      732 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      735 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      715 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1231 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1333 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      593 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     2006 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1211 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      864 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1194 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1337 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      391 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      963 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      610 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0      288 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2502 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      890 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2784 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3383 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3252 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1052 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2771 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0     1532 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     2929 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3662 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3247 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5192 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     2625 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4818 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3417 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      496 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1733 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 avtomat_aws-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3838 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/README.md
+-rw-r--r--   0        0        0       69 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      833 2024-04-06 20:19:09.958304 avtomat_aws-0.1.1/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      897 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1125 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1114 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1269 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      680 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/create_snapshots.py
+-rw-r--r--   0        0        0      824 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0      687 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      657 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      803 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      472 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      451 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1203 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1369 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      634 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1401 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1172 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      481 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1348 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      899 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      823 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1220 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1100 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      793 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      816 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      760 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      750 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      468 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      701 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      732 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      735 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      715 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1231 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1333 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      593 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     2006 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1211 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      864 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1194 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1365 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0     1375 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      391 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      615 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2636 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      728 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2784 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3383 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3252 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1099 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2625 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     1988 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/create_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0     1532 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     2929 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3662 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3247 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5192 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     3322 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4818 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      618 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     2808 2024-04-06 20:19:09.962304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3423 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      497 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1743 2024-04-06 20:19:09.966304 avtomat_aws-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 avtomat_aws-0.1.1/PKG-INFO
```

### Comparing `avtomat_aws-0.0.3/LICENSE` & `avtomat_aws-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/README.md` & `avtomat_aws-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,46 +14,40 @@
 
 [![homepage](https://img.shields.io/website?url=https%3A%2F%2Favtomat.io&style=flat-square)](https://avtomat.io)
 [![documentation](https://img.shields.io/badge/documentation-yes-brightgreen.svg?style=flat-square)](https://docs.avtomat.io/aws/get_started)
 [![contributing](https://img.shields.io/badge/contributing-guide-blue?style=flat-square)](/docs/CONTRIBUTING.md)
 <br/>
 [![version](https://img.shields.io/pypi/v/avtomat-aws?style=flat-square&label=version&color=blue)](https://github.com/avtomat-hub/avtomat-aws)
 [![build](https://img.shields.io/github/actions/workflow/status/avtomat-hub/avtomat-aws/publish-to-pypi.yml?style=flat-square)](https://github.com/avtomat-hub/avtomat-aws/actions/workflows/publish-to-pypi.yml)
-[![python](https://img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https://pypi.org/p/avtomat-aws)
 [![status](https://img.shields.io/pypi/status/avtomat-aws?style=flat-square)](https://pypi.org/p/avtomat-aws)
+[![downloads](https://img.shields.io/pypi/dm/avtomat-aws?style=flat-square)](https://pypi.org/project/avtomat-aws/)
+[![python](https://img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https://pypi.org/p/avtomat-aws)
 [![license](https://img.shields.io/github/license/avtomat-hub/avtomat-aws?style=flat-square)](https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE)
 
 </div>
 
-> </br><h4 align="center">**A Python collection of Amazon Web Services actions. </br> 
-> Built on top of Boto3.**</h4></br>
-
----
+> </br><h4 align="center">**A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations. </br> 
+> Written in Python. Built on top of Boto3.**</h4></br>
 
 ## Table of Contents
 
 - [Overview](#overview)
 - [Installation](#installation)
   - [PyPi](#pypi)
 - [Requirements](#requirements)
 - [Contributing](#contributing)
-  - [Affiliates](#affiliates)
 - [License](#license)
 
----
-
 ## Overview
 
-This repository is home to the Avtomat AWS collection. It includes pre-defined actions for automating cloud operations on Amazon Web Services. </br> 
-The actions are written in Python and can be used as standalone scripts or incorporated into your own projects. </br> 
-Additionally, the entire collection has a CLI interface, providing easy access to actions. </br> </br>
+This repository features a collection of pre-written AWS scripts (called actions), designed to streamline daily operations - from information gathering to infrastructure changes. </br> 
+Actions are written in Python and can be used as standalone scripts, chained together to form workflows or incorporated into your own projects. </br> 
+The collection has a CLI interface, providing easy access to each action. </br> </br>
 For a list of available actions or usage instructions, see the [documentation](https://docs.avtomat.io/aws/get_started).
 
----
-
 ## Installation
 
 Currently, this collection can only be installed from PyPi.
 
 ### PyPi
 
 If you already have Python3 and pip3 installed, you can perform:
@@ -63,29 +57,26 @@
 ```shell 
 python3 -m venv venv
 source venv/bin/activate
 pip install avtomat-aws
 aaws --help
 ```
 
-#### System-wide Installation (recommended: pipx)
+#### Global Installation (recommended: pipx)
 
 ```shell
 pipx install avtomat-aws
 aaws --help
 ```
 
 ## Requirements
 
-To run this collection, you only need [Python3](https://www.python.org/) and [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html).
-
----
+This collection only requires [Python3](https://www.python.org/) and [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html). </br>
+AWS configuration files (`~/.aws/credentials` and `~/.aws/config`) are optional but highly recommended for falling back to Boto3 authentication flow.
 
 ## Contributing
 
 Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/avtomat-hub/avtomat-aws/issues). <br>If you are interested in contributing or would like to make some modifications, please take a look at the [contributing guide](/docs/CONTRIBUTING.md).
 
----
-
 ## License
 
 Copyright © 2024 [Avtomat Ltd](https://avtomat.io). This project is [GPLv2](https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE) licensed.
```

#### html2text {}

```diff
@@ -7,39 +7,44 @@
 brightgreen.svg?style=flat-square)](https://docs.avtomat.io/aws/get_started) [!
 [contributing](https://img.shields.io/badge/contributing-guide-blue?style=flat-
                        square)](/docs/CONTRIBUTING.md)
        [![version](https://img.shields.io/pypi/v/avtomat-aws?style=flat-
 square&label=version&color=blue)](https://github.com/avtomat-hub/avtomat-aws)
  [![build](https://img.shields.io/github/actions/workflow/status/avtomat-hub/
 avtomat-aws/publish-to-pypi.yml?style=flat-square)](https://github.com/avtomat-
-  hub/avtomat-aws/actions/workflows/publish-to-pypi.yml) [![python](https://
-    img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https://
-pypi.org/p/avtomat-aws) [![status](https://img.shields.io/pypi/status/avtomat-
- aws?style=flat-square)](https://pypi.org/p/avtomat-aws) [![license](https://
-   img.shields.io/github/license/avtomat-hub/avtomat-aws?style=flat-square)]
-        (https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE)
+  hub/avtomat-aws/actions/workflows/publish-to-pypi.yml) [![status](https://
+img.shields.io/pypi/status/avtomat-aws?style=flat-square)](https://pypi.org/p/
+      avtomat-aws) [![downloads](https://img.shields.io/pypi/dm/avtomat-
+   aws?style=flat-square)](https://pypi.org/project/avtomat-aws/) [![python]
+(https://img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https:/
+  /pypi.org/p/avtomat-aws) [![license](https://img.shields.io/github/license/
+  avtomat-hub/avtomat-aws?style=flat-square)](https://github.com/avtomat-hub/
+                        avtomat-aws/blob/main/LICENSE)
 >
-  ****** ****AA PPyytthhoonn ccoolllleeccttiioonn ooff AAmmaazzoonn WWeebb SSeerrvviicceess aaccttiioonnss.. >> BBuuiilltt oonn ttoopp ooff
-                                 BBoottoo33..**** ******
---- ## Table of Contents - [Overview](#overview) - [Installation]
-(#installation) - [PyPi](#pypi) - [Requirements](#requirements) -
-[Contributing](#contributing) - [Affiliates](#affiliates) - [License](#license)
---- ## Overview This repository is home to the Avtomat AWS collection. It
-includes pre-defined actions for automating cloud operations on Amazon Web
-Services. The actions are written in Python and can be used as standalone
-scripts or incorporated into your own projects. Additionally, the entire
-collection has a CLI interface, providing easy access to actions. For a list of
-available actions or usage instructions, see the [documentation](https://
-docs.avtomat.io/aws/get_started). --- ## Installation Currently, this
-collection can only be installed from PyPi. ### PyPi If you already have
-Python3 and pip3 installed, you can perform: #### Virtual Environment
-Installation (pip) ```shell python3 -m venv venv source venv/bin/activate pip
-install avtomat-aws aaws --help ``` #### System-wide Installation (recommended:
-pipx) ```shell pipx install avtomat-aws aaws --help ``` ## Requirements To run
-this collection, you only need [Python3](https://www.python.org/) and [Boto3]
-(https://boto3.amazonaws.com/v1/documentation/api/latest/index.html). --- ##
-Contributing Contributions, issues, and feature requests are welcome! Feel free
-to check the [issues page](https://github.com/avtomat-hub/avtomat-aws/issues).
+****** ****AA ccoolllleeccttiioonn ooff rreeuussaabbllee AAmmaazzoonn WWeebb SSeerrvviicceess aaccttiioonnss,, bbrriinnggiinngg ssppeeeedd aanndd
+ cceerrttaaiinnttyy ttoo cclloouudd ooppeerraattiioonnss.. >> WWrriitttteenn iinn PPyytthhoonn.. BBuuiilltt oonn ttoopp ooff BBoottoo33..****
+                                      ******
+## Table of Contents - [Overview](#overview) - [Installation](#installation) -
+[PyPi](#pypi) - [Requirements](#requirements) - [Contributing](#contributing) -
+[License](#license) ## Overview This repository features a collection of pre-
+written AWS scripts (called actions), designed to streamline daily operations -
+from information gathering to infrastructure changes. Actions are written in
+Python and can be used as standalone scripts, chained together to form
+workflows or incorporated into your own projects. The collection has a CLI
+interface, providing easy access to each action. For a list of available
+actions or usage instructions, see the [documentation](https://docs.avtomat.io/
+aws/get_started). ## Installation Currently, this collection can only be
+installed from PyPi. ### PyPi If you already have Python3 and pip3 installed,
+you can perform: #### Virtual Environment Installation (pip) ```shell python3 -
+m venv venv source venv/bin/activate pip install avtomat-aws aaws --help ```
+#### Global Installation (recommended: pipx) ```shell pipx install avtomat-aws
+aaws --help ``` ## Requirements This collection only requires [Python3](https:/
+/www.python.org/) and [Boto3](https://boto3.amazonaws.com/v1/documentation/api/
+latest/index.html). AWS configuration files (`~/.aws/credentials` and `~/.aws/
+config`) are optional but highly recommended for falling back to Boto3
+authentication flow. ## Contributing Contributions, issues, and feature
+requests are welcome! Feel free to check the [issues page](https://github.com/
+avtomat-hub/avtomat-aws/issues).
 If you are interested in contributing or would like to make some modifications,
-please take a look at the [contributing guide](/docs/CONTRIBUTING.md). --- ##
+please take a look at the [contributing guide](/docs/CONTRIBUTING.md). ##
 License Copyright Â© 2024 [Avtomat Ltd](https://avtomat.io). This project is
 [GPLv2](https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE) licensed.
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_security_groups.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,20 @@
     )
     parser.add_argument(
         "--types",
         nargs="+",
         help="Volume types to check, separated by space.",
         required=False,
     )
+    parser.add_argument(
+        "--root",
+        action="store_true",
+        help="Get only root volumes.",
+        required=False,
+    )
 
 
 def cli(args):
     """Command-line interface function"""
 
     inputs = vars(args)
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/share_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_password_users.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/main.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/main.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/s3/delete_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/s3/discover_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/services.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     "cloudtrail": [
         "discover_user_events",
         "discover_resource_events",
         "discover_events",
     ],
     "ec2": [
         "copy_snapshots",
+        "create_snapshots",
         "delete_images",
         "delete_security_groups",
         "delete_snapshots",
         "delete_volumes",
         "discover_active_regions",
         "discover_default_ebs_encryption",
         "discover_images",
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/cli/sts/create_session.py` & `avtomat_aws-0.1.1/avtomat_aws/cli/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.1.1/avtomat_aws/decorators/authenticate.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 
 
 def authenticate():
     """Decorator to authenticate with AWS and set a region for the action."""
 
     def decorator(func):
         def wrapper(**kwargs):
-            # Check if session is not provided and create one if necessary
-            if not kwargs.get("session"):
-                kwargs["session"] = set_session(
-                    debug=kwargs.get("debug"), silent=kwargs.get("silent")
-                )
+            # Create a session
+            kwargs["session"] = set_session(**kwargs)
             # Set the region for the session
             kwargs["region"] = set_region(
                 region=kwargs.get("region"),
                 session=kwargs.get("session"),
                 debug=kwargs.get("debug"),
                 silent=kwargs.get("silent"),
             )
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.1.1/avtomat_aws/decorators/set_logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def set_logger():
     """Decorator to set a logger for the action."""
 
     def decorator(func):
         def wrapper(**kwargs):
             # Setup logger
             set_logging()
-            logger = logging.getLogger(__name__)
+            logger = logging.getLogger("avtomat_aws")
             # Set log level
             if kwargs.get("debug"):
                 logger.setLevel(logging.DEBUG)
             if kwargs.get("silent"):
                 logger.setLevel(logging.WARNING)
             # Call the action
             return func(**kwargs)
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.1.1/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.1.1/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.1.1/avtomat_aws/helpers/set_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,30 @@
 
     # Set logging level
     if kwargs.get("debug"):
         logger.setLevel(logging.DEBUG)
     if kwargs.get("silent"):
         logger.setLevel(logging.WARNING)
 
-    if kwargs.get("profile"):
+    if kwargs.get("session"):
+        logger.debug("Session explicitly supplied.")
+        session = kwargs["session"]
+    elif kwargs.get("profile"):
         session = authenticate_profile(kwargs["profile"])
     elif kwargs.get("role_arn"):
         session = authenticate_role(
             kwargs["role_arn"], kwargs["mfa_serial"], kwargs["mfa_token"]
         )
     elif kwargs.get("access_key") and kwargs.get("secret_key"):
         session = authenticate_credentials(
             kwargs["access_key"], kwargs["secret_key"], kwargs["session_token"]
         )
     else:
         logger.debug(
-            "No 'profile' or 'role_arn' or 'access_key' + 'secret_key' parameters supplied. "
+            "No 'session' or 'profile' or 'role_arn' or 'access_key' + 'secret_key' parameters supplied. "
             "Falling back to default credentials."
         )
         session = authenticate_default()
 
     sts_client = session.client("sts")
     response = sts_client.get_caller_identity()
     logger.debug(f"Session created: {response['Arn']}")
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/helpers/set_session_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,19 @@
 
 def set_session_objects(session, region, clients=None, resources=None):
     """Set the session objects(clients and resources)."""
 
     session_objects = {}
 
     if clients:
-        logger.debug("Initializing clients:")
         for client in clients:
             session_objects[f"{client}_client"] = session.client(
                 client, region_name=region, config=config
             )
-            logger.debug(client)
 
     if resources:
-        logger.debug("Initializing resources:")
         for resource in resources:
             session_objects[f"{resource}_resource"] = session.resource(
                 resource, region_name=region, config=config
             )
-            logger.debug(resource)
 
     return session_objects
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.1.1/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.1.1/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.1.1/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .copy_snapshots import copy_snapshots
+from .create_snapshots import create_snapshots
 from .delete_images import delete_images
 from .delete_security_groups import delete_security_groups
 from .delete_snapshots import delete_snapshots
 from .delete_volumes import delete_volumes
 from .discover_active_regions import discover_active_regions
 from .discover_default_ebs_encryption import discover_default_ebs_encryption
 from .discover_images import discover_images
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from avtomat_aws.decorators.validate import validate
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
     "region": None,
-    "pending_limit": None,
+    "pending_limit": 20,
     "encrypt": False,
     "kms_key_id": None,
     "debug": False,
     "silent": False,
 }
 RULES = [{"and": ["encrypt", "kms_key_id"]}]
 
@@ -37,19 +37,16 @@
         kwargs["session"], clients=["ec2"], region=target_region
     )
 
     logger.info(f"Creating snapshot copies in {target_region}")
 
     snapshots = []
     pending_snapshots = set()
-    if kwargs.get("pending_limit"):
-        logger.debug(f"Custom pending limit: {kwargs['pending_limit']}")
-        pending_limit = kwargs["pending_limit"]
-    else:
-        pending_limit = 20  # AWS limit for concurrent snapshot copy operations
+    pending_limit = kwargs["pending_limit"]
+    logger.debug(f"Custom pending limit: {pending_limit}")
 
     for snapshot_id in snapshot_ids:
         while len(pending_snapshots) >= pending_limit:
             logger.debug(f"Reached {pending_limit} pending snapshots, waiting...")
             for snapshot in list(pending_snapshots):
                 status = session_objects["ec2_client"].describe_snapshots(
                     SnapshotIds=[snapshot]
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from avtomat_aws.decorators.set_logger import set_logger
 from avtomat_aws.decorators.validate import validate
 from avtomat_aws.helpers.set_session_objects import set_session_objects
 
 logger = logging.getLogger(__name__)
 
 DEFAULTS = {
-    "instance_ids": None,
+    "instance_ids": [],
     "volume_ids": [],
     "unencrypted": False,
     "detached": False,
     "types": None,
+    "root": False,
     "region": None,
     "debug": False,
     "silent": False,
 }
 RULES = [
-    {"required": ["resource_types", "tags"]},
     {
         "choice": [
             {"types": ["gp2", "gp3", "io1", "io2", "st1", "sc1", "standard"]},
         ]
     },
     {"at_most_one": ["instance_ids", "volume_ids"]},
 ]
@@ -49,14 +49,15 @@
     """Construct filters"""
 
     instance_ids = kwargs.get("instance_ids")
     volume_ids = kwargs.get("volume_ids")
     unencrypted = kwargs.get("unencrypted")
     detached = kwargs.get("detached")
     types = kwargs.get("types")
+    root = kwargs.get("root")
 
     filters = []
     if instance_ids:
         logger.debug(f"Targeting instance volumes: {instance_ids}")
         filters.append({"Name": "attachment.instance-id", "Values": instance_ids})
     elif volume_ids:
         logger.debug(f"Targeting specific volumes: {volume_ids}")
@@ -67,14 +68,18 @@
         filters.append({"Name": "encrypted", "Values": ["false"]})
     if detached:
         logger.debug("Filtering for detached volumes")
         filters.append({"Name": "status", "Values": ["available"]})
     if types:
         logger.debug(f"Filtering for types: {types}")
         filters.append({"Name": "volume-type", "Values": types})
+    if root:
+        logger.debug("Filtering for root volumes")
+        root_devices = get_root_devices(**kwargs)
+        filters.append({"Name": "attachment.device", "Values": root_devices})
 
     return filters
 
 
 def search_volumes(filters, **kwargs):
     """Search for volumes in specified region"""
 
@@ -89,7 +94,25 @@
         Filters=filters, VolumeIds=volume_ids
     )
 
     for volume in response:
         volumes.append(volume.id)
 
     return volumes
+
+
+def get_root_devices(**kwargs):
+    """Get root devices for specified instances"""
+
+    session = kwargs["session"]
+    region = kwargs["region"]
+    instance_ids = kwargs.get("instance_ids")
+
+    session_objects = set_session_objects(session, resources=["ec2"], region=region)
+
+    root_devices = []
+    for instance in session_objects["ec2_resource"].instances.filter(
+        InstanceIds=instance_ids
+    ):
+        root_devices.append(instance.root_device_name)
+
+    return list(set(root_devices))
```

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.1.1/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.1.1/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.1.1/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.1.1/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.1.1/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.1.1/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.3/avtomat_aws/validations/rules.py` & `avtomat_aws-0.1.1/avtomat_aws/validations/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def at_most_one_rule(kwargs, params):
     """Validates that at most one of the parameters is provided."""
 
     if len(params) < 2:
         raise ValueError("Rule 'at_most_one' requires at least two parameters")
 
-    params_defined = sum(kwargs.get(param) is not None for param in params)
+    params_defined = sum(kwargs.get(param) not in (None, []) for param in params)
     if params_defined > 1:
         raise ValueError(
             f"The following parameters cannot be used together, select only one: {params}"
         )
 
 
 def at_least_one_rule(kwargs, params):
```

### Comparing `avtomat_aws-0.0.3/pyproject.toml` & `avtomat_aws-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.0.3"
-description = "Automate AWS cloud operations by using pre-defined actions instead of scripting from scratch."
+version = "0.1.1"
+description = "A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
 include = ["CHANGELOG.md", "LICENSE"]
@@ -39,18 +39,18 @@
 [tool.poetry.scripts]
 aaws = "avtomat_aws.cli.main:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/avtomat-hub/avtomat-aws/issues"
 "GitHub" = "https://github.com/avtomat-hub/avtomat-aws"
 
-
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "semver"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `avtomat_aws-0.0.3/PKG-INFO` & `avtomat_aws-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.0.3
-Summary: Automate AWS cloud operations by using pre-defined actions instead of scripting from scratch.
+Version: 0.1.1
+Summary: A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations.
 Home-page: https://avtomat.io
 License: GPL-2.0-only
 Keywords: aws,cloud,automation,cli,python,boto3
 Author: Dimitar Atanasov
 Author-email: dimitar@avtomat.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -44,46 +44,40 @@
 
 [![homepage](https://img.shields.io/website?url=https%3A%2F%2Favtomat.io&style=flat-square)](https://avtomat.io)
 [![documentation](https://img.shields.io/badge/documentation-yes-brightgreen.svg?style=flat-square)](https://docs.avtomat.io/aws/get_started)
 [![contributing](https://img.shields.io/badge/contributing-guide-blue?style=flat-square)](/docs/CONTRIBUTING.md)
 <br/>
 [![version](https://img.shields.io/pypi/v/avtomat-aws?style=flat-square&label=version&color=blue)](https://github.com/avtomat-hub/avtomat-aws)
 [![build](https://img.shields.io/github/actions/workflow/status/avtomat-hub/avtomat-aws/publish-to-pypi.yml?style=flat-square)](https://github.com/avtomat-hub/avtomat-aws/actions/workflows/publish-to-pypi.yml)
-[![python](https://img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https://pypi.org/p/avtomat-aws)
 [![status](https://img.shields.io/pypi/status/avtomat-aws?style=flat-square)](https://pypi.org/p/avtomat-aws)
+[![downloads](https://img.shields.io/pypi/dm/avtomat-aws?style=flat-square)](https://pypi.org/project/avtomat-aws/)
+[![python](https://img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https://pypi.org/p/avtomat-aws)
 [![license](https://img.shields.io/github/license/avtomat-hub/avtomat-aws?style=flat-square)](https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE)
 
 </div>
 
-> </br><h4 align="center">**A Python collection of Amazon Web Services actions. </br> 
-> Built on top of Boto3.**</h4></br>
-
----
+> </br><h4 align="center">**A collection of reusable Amazon Web Services actions, bringing speed and certainty to cloud operations. </br> 
+> Written in Python. Built on top of Boto3.**</h4></br>
 
 ## Table of Contents
 
 - [Overview](#overview)
 - [Installation](#installation)
   - [PyPi](#pypi)
 - [Requirements](#requirements)
 - [Contributing](#contributing)
-  - [Affiliates](#affiliates)
 - [License](#license)
 
----
-
 ## Overview
 
-This repository is home to the Avtomat AWS collection. It includes pre-defined actions for automating cloud operations on Amazon Web Services. </br> 
-The actions are written in Python and can be used as standalone scripts or incorporated into your own projects. </br> 
-Additionally, the entire collection has a CLI interface, providing easy access to actions. </br> </br>
+This repository features a collection of pre-written AWS scripts (called actions), designed to streamline daily operations - from information gathering to infrastructure changes. </br> 
+Actions are written in Python and can be used as standalone scripts, chained together to form workflows or incorporated into your own projects. </br> 
+The collection has a CLI interface, providing easy access to each action. </br> </br>
 For a list of available actions or usage instructions, see the [documentation](https://docs.avtomat.io/aws/get_started).
 
----
-
 ## Installation
 
 Currently, this collection can only be installed from PyPi.
 
 ### PyPi
 
 If you already have Python3 and pip3 installed, you can perform:
@@ -93,29 +87,26 @@
 ```shell 
 python3 -m venv venv
 source venv/bin/activate
 pip install avtomat-aws
 aaws --help
 ```
 
-#### System-wide Installation (recommended: pipx)
+#### Global Installation (recommended: pipx)
 
 ```shell
 pipx install avtomat-aws
 aaws --help
 ```
 
 ## Requirements
 
-To run this collection, you only need [Python3](https://www.python.org/) and [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html).
-
----
+This collection only requires [Python3](https://www.python.org/) and [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html). </br>
+AWS configuration files (`~/.aws/credentials` and `~/.aws/config`) are optional but highly recommended for falling back to Boto3 authentication flow.
 
 ## Contributing
 
 Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/avtomat-hub/avtomat-aws/issues). <br>If you are interested in contributing or would like to make some modifications, please take a look at the [contributing guide](/docs/CONTRIBUTING.md).
 
----
-
 ## License
 
 Copyright © 2024 [Avtomat Ltd](https://avtomat.io). This project is [GPLv2](https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE) licensed.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.0.3 Summary: Automate AWS
-cloud operations by using pre-defined actions instead of scripting from
-scratch. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.1.1 Summary: A collection of
+reusable Amazon Web Services actions, bringing speed and certainty to cloud
+operations. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -25,39 +25,44 @@
 brightgreen.svg?style=flat-square)](https://docs.avtomat.io/aws/get_started) [!
 [contributing](https://img.shields.io/badge/contributing-guide-blue?style=flat-
                        square)](/docs/CONTRIBUTING.md)
        [![version](https://img.shields.io/pypi/v/avtomat-aws?style=flat-
 square&label=version&color=blue)](https://github.com/avtomat-hub/avtomat-aws)
  [![build](https://img.shields.io/github/actions/workflow/status/avtomat-hub/
 avtomat-aws/publish-to-pypi.yml?style=flat-square)](https://github.com/avtomat-
-  hub/avtomat-aws/actions/workflows/publish-to-pypi.yml) [![python](https://
-    img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https://
-pypi.org/p/avtomat-aws) [![status](https://img.shields.io/pypi/status/avtomat-
- aws?style=flat-square)](https://pypi.org/p/avtomat-aws) [![license](https://
-   img.shields.io/github/license/avtomat-hub/avtomat-aws?style=flat-square)]
-        (https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE)
+  hub/avtomat-aws/actions/workflows/publish-to-pypi.yml) [![status](https://
+img.shields.io/pypi/status/avtomat-aws?style=flat-square)](https://pypi.org/p/
+      avtomat-aws) [![downloads](https://img.shields.io/pypi/dm/avtomat-
+   aws?style=flat-square)](https://pypi.org/project/avtomat-aws/) [![python]
+(https://img.shields.io/pypi/pyversions/avtomat-aws?style=flat-square)](https:/
+  /pypi.org/p/avtomat-aws) [![license](https://img.shields.io/github/license/
+  avtomat-hub/avtomat-aws?style=flat-square)](https://github.com/avtomat-hub/
+                        avtomat-aws/blob/main/LICENSE)
 >
-  ****** ****AA PPyytthhoonn ccoolllleeccttiioonn ooff AAmmaazzoonn WWeebb SSeerrvviicceess aaccttiioonnss.. >> BBuuiilltt oonn ttoopp ooff
-                                 BBoottoo33..**** ******
---- ## Table of Contents - [Overview](#overview) - [Installation]
-(#installation) - [PyPi](#pypi) - [Requirements](#requirements) -
-[Contributing](#contributing) - [Affiliates](#affiliates) - [License](#license)
---- ## Overview This repository is home to the Avtomat AWS collection. It
-includes pre-defined actions for automating cloud operations on Amazon Web
-Services. The actions are written in Python and can be used as standalone
-scripts or incorporated into your own projects. Additionally, the entire
-collection has a CLI interface, providing easy access to actions. For a list of
-available actions or usage instructions, see the [documentation](https://
-docs.avtomat.io/aws/get_started). --- ## Installation Currently, this
-collection can only be installed from PyPi. ### PyPi If you already have
-Python3 and pip3 installed, you can perform: #### Virtual Environment
-Installation (pip) ```shell python3 -m venv venv source venv/bin/activate pip
-install avtomat-aws aaws --help ``` #### System-wide Installation (recommended:
-pipx) ```shell pipx install avtomat-aws aaws --help ``` ## Requirements To run
-this collection, you only need [Python3](https://www.python.org/) and [Boto3]
-(https://boto3.amazonaws.com/v1/documentation/api/latest/index.html). --- ##
-Contributing Contributions, issues, and feature requests are welcome! Feel free
-to check the [issues page](https://github.com/avtomat-hub/avtomat-aws/issues).
+****** ****AA ccoolllleeccttiioonn ooff rreeuussaabbllee AAmmaazzoonn WWeebb SSeerrvviicceess aaccttiioonnss,, bbrriinnggiinngg ssppeeeedd aanndd
+ cceerrttaaiinnttyy ttoo cclloouudd ooppeerraattiioonnss.. >> WWrriitttteenn iinn PPyytthhoonn.. BBuuiilltt oonn ttoopp ooff BBoottoo33..****
+                                      ******
+## Table of Contents - [Overview](#overview) - [Installation](#installation) -
+[PyPi](#pypi) - [Requirements](#requirements) - [Contributing](#contributing) -
+[License](#license) ## Overview This repository features a collection of pre-
+written AWS scripts (called actions), designed to streamline daily operations -
+from information gathering to infrastructure changes. Actions are written in
+Python and can be used as standalone scripts, chained together to form
+workflows or incorporated into your own projects. The collection has a CLI
+interface, providing easy access to each action. For a list of available
+actions or usage instructions, see the [documentation](https://docs.avtomat.io/
+aws/get_started). ## Installation Currently, this collection can only be
+installed from PyPi. ### PyPi If you already have Python3 and pip3 installed,
+you can perform: #### Virtual Environment Installation (pip) ```shell python3 -
+m venv venv source venv/bin/activate pip install avtomat-aws aaws --help ```
+#### Global Installation (recommended: pipx) ```shell pipx install avtomat-aws
+aaws --help ``` ## Requirements This collection only requires [Python3](https:/
+/www.python.org/) and [Boto3](https://boto3.amazonaws.com/v1/documentation/api/
+latest/index.html). AWS configuration files (`~/.aws/credentials` and `~/.aws/
+config`) are optional but highly recommended for falling back to Boto3
+authentication flow. ## Contributing Contributions, issues, and feature
+requests are welcome! Feel free to check the [issues page](https://github.com/
+avtomat-hub/avtomat-aws/issues).
 If you are interested in contributing or would like to make some modifications,
-please take a look at the [contributing guide](/docs/CONTRIBUTING.md). --- ##
+please take a look at the [contributing guide](/docs/CONTRIBUTING.md). ##
 License Copyright Â© 2024 [Avtomat Ltd](https://avtomat.io). This project is
 [GPLv2](https://github.com/avtomat-hub/avtomat-aws/blob/main/LICENSE) licensed.
```

