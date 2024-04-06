# Comparing `tmp/seam-0.0.tar.gz` & `tmp/seam-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seam-0.0.tar", last modified: Mon Jan 27 19:26:17 2014, max compression
+gzip compressed data, was "seam-0.1.0.tar", max compression
```

## Comparing `seam-0.0.tar` & `seam-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,41 @@
-drwxr-xr-x   0 scottburns   (503) staff       (20)        0 2014-01-27 19:26:17.000000 seam-0.0/
--rw-r--r--   0 scottburns   (503) staff       (20)     3000 2014-01-27 19:26:17.000000 seam-0.0/PKG-INFO
-drwxr-xr-x   0 scottburns   (503) staff       (20)        0 2014-01-27 19:26:17.000000 seam-0.0/seam/
--rw-r--r--   0 scottburns   (503) staff       (20)      504 2014-01-27 16:16:13.000000 seam-0.0/seam/__init__.py
-drwxr-xr-x   0 scottburns   (503) staff       (20)        0 2014-01-27 19:26:17.000000 seam-0.0/seam.egg-info/
--rw-r--r--   0 scottburns   (503) staff       (20)        1 2014-01-27 19:26:17.000000 seam-0.0/seam.egg-info/dependency_links.txt
--rw-r--r--   0 scottburns   (503) staff       (20)     3000 2014-01-27 19:26:17.000000 seam-0.0/seam.egg-info/PKG-INFO
--rw-r--r--   0 scottburns   (503) staff       (20)      137 2014-01-27 19:26:17.000000 seam-0.0/seam.egg-info/SOURCES.txt
--rw-r--r--   0 scottburns   (503) staff       (20)        5 2014-01-27 19:26:17.000000 seam-0.0/seam.egg-info/top_level.txt
--rw-r--r--   0 scottburns   (503) staff       (20)       59 2014-01-27 19:26:17.000000 seam-0.0/setup.cfg
--rw-r--r--   0 scottburns   (503) staff       (20)     3109 2014-01-27 19:14:07.000000 seam-0.0/setup.py
+-rw-r--r--   0        0        0     1087 2024-04-06 00:17:02.761351 seam-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4227 2024-04-06 00:17:02.761351 seam-0.1.0/README.rst
+-rw-r--r--   0        0        0      726 2024-04-06 00:17:02.761351 seam-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-04-06 00:17:02.761351 seam-0.1.0/seam/__init__.py
+-rw-r--r--   0        0        0    11938 2024-04-06 00:17:02.761351 seam-0.1.0/seam/access_codes.py
+-rw-r--r--   0        0        0      903 2024-04-06 00:17:02.761351 seam-0.1.0/seam/access_codes_simulate.py
+-rw-r--r--   0        0        0     3979 2024-04-06 00:17:02.761351 seam-0.1.0/seam/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1746 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs.py
+-rw-r--r--   0        0        0     2505 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_access_groups.py
+-rw-r--r--   0        0        0      718 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_credential_pools.py
+-rw-r--r--   0        0        0     1782 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4763 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_credentials.py
+-rw-r--r--   0        0        0     2172 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_entrances.py
+-rw-r--r--   0        0        0      955 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_systems.py
+-rw-r--r--   0        0        0     6476 2024-04-06 00:17:02.761351 seam-0.1.0/seam/acs_users.py
+-rw-r--r--   0        0        0     3169 2024-04-06 00:17:02.761351 seam-0.1.0/seam/action_attempts.py
+-rw-r--r--   0        0        0     5751 2024-04-06 00:17:02.761351 seam-0.1.0/seam/client_sessions.py
+-rw-r--r--   0        0        0     3292 2024-04-06 00:17:02.761351 seam-0.1.0/seam/connect_webviews.py
+-rw-r--r--   0        0        0     2520 2024-04-06 00:17:02.761351 seam-0.1.0/seam/connected_accounts.py
+-rw-r--r--   0        0        0     4761 2024-04-06 00:17:02.761351 seam-0.1.0/seam/devices.py
+-rw-r--r--   0        0        0      517 2024-04-06 00:17:02.761351 seam-0.1.0/seam/devices_simulate.py
+-rw-r--r--   0        0        0     3323 2024-04-06 00:17:02.761351 seam-0.1.0/seam/devices_unmanaged.py
+-rw-r--r--   0        0        0     2385 2024-04-06 00:17:02.761351 seam-0.1.0/seam/events.py
+-rw-r--r--   0        0        0     4181 2024-04-06 00:17:02.761351 seam-0.1.0/seam/locks.py
+-rw-r--r--   0        0        0      765 2024-04-06 00:17:02.761351 seam-0.1.0/seam/networks.py
+-rw-r--r--   0        0        0      714 2024-04-06 00:17:02.761351 seam-0.1.0/seam/noise_sensors.py
+-rw-r--r--   0        0        0     4350 2024-04-06 00:17:02.761351 seam-0.1.0/seam/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      594 2024-04-06 00:17:02.765351 seam-0.1.0/seam/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1063 2024-04-06 00:17:02.765351 seam-0.1.0/seam/phones.py
+-rw-r--r--   0        0        0     1185 2024-04-06 00:17:02.765351 seam-0.1.0/seam/phones_simulate.py
+-rw-r--r--   0        0        0     1535 2024-04-06 00:17:02.765351 seam-0.1.0/seam/routes.py
+-rw-r--r--   0        0        0     3175 2024-04-06 00:17:02.765351 seam-0.1.0/seam/seam.py
+-rw-r--r--   0        0        0     8926 2024-04-06 00:17:02.765351 seam-0.1.0/seam/thermostats.py
+-rw-r--r--   0        0        0     6930 2024-04-06 00:17:02.765351 seam-0.1.0/seam/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64035 2024-04-06 00:17:02.765351 seam-0.1.0/seam/types.py
+-rw-r--r--   0        0        0     6700 2024-04-06 00:17:02.765351 seam-0.1.0/seam/user_identities.py
+-rw-r--r--   0        0        0     2903 2024-04-06 00:17:02.765351 seam-0.1.0/seam/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-04-06 00:17:02.765351 seam-0.1.0/seam/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1815 2024-04-06 00:17:02.765351 seam-0.1.0/seam/webhooks.py
+-rw-r--r--   0        0        0     1845 2024-04-06 00:17:02.765351 seam-0.1.0/seam/workspaces.py
+-rw-r--r--   0        0        0     4977 1970-01-01 00:00:00.000000 seam-0.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

