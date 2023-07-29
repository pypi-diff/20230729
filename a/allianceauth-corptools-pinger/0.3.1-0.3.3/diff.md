# Comparing `tmp/allianceauth-corptools-pinger-0.3.1.tar.gz` & `tmp/allianceauth-corptools-pinger-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-corptools-pinger-0.3.1.tar", last modified: Wed May 25 09:55:55 2022, max compression
+gzip compressed data, was "allianceauth-corptools-pinger-0.3.3.tar", last modified: Sat Jul 29 11:07:26 2023, max compression
```

## Comparing `allianceauth-corptools-pinger-0.3.1.tar` & `allianceauth-corptools-pinger-0.3.3.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.489480 allianceauth-corptools-pinger-0.3.1/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       31 2021-11-24 09:23:40.000000 allianceauth-corptools-pinger-0.3.1/MANIFEST.in
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2584 2022-05-25 09:55:55.489480 allianceauth-corptools-pinger-0.3.1/PKG-INFO
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1785 2022-02-19 10:18:43.000000 allianceauth-corptools-pinger-0.3.1/README.md
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.479480 allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2584 2022-05-25 09:55:55.000000 allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/PKG-INFO
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1223 2022-05-25 09:55:55.000000 allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/SOURCES.txt
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        1 2022-05-25 09:55:55.000000 allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/dependency_links.txt
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       50 2022-05-25 09:55:55.000000 allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/requires.txt
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       13 2022-05-25 09:55:55.000000 allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/top_level.txt
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.479480 allianceauth-corptools-pinger-0.3.1/pinger/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       22 2022-05-25 09:55:28.000000 allianceauth-corptools-pinger-0.3.1/pinger/__init__.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     7160 2022-05-14 08:22:48.000000 allianceauth-corptools-pinger-0.3.1/pinger/admin.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      179 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/apps.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      289 2021-11-24 10:14:10.000000 allianceauth-corptools-pinger-0.3.1/pinger/auth_hooks.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     7978 2022-05-14 08:22:48.000000 allianceauth-corptools-pinger-0.3.1/pinger/cogs.py
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.479480 allianceauth-corptools-pinger-0.3.1/pinger/management/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        0 2021-11-24 09:22:09.000000 allianceauth-corptools-pinger-0.3.1/pinger/management/__init__.py
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.479480 allianceauth-corptools-pinger-0.3.1/pinger/management/commands/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        0 2021-11-24 08:51:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/management/commands/__init.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2482 2022-01-03 10:01:17.000000 allianceauth-corptools-pinger-0.3.1/pinger/management/commands/pinger_stats.py
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.489480 allianceauth-corptools-pinger-0.3.1/pinger/migrations/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2669 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0001_initial.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1154 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0002_create_ping_types.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2155 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0003_auto_20211108_0024.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1284 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0004_create_more_types.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1027 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0005_pingerconfig.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      424 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0006_create_settings.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      499 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0007_create_more_types_again.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      612 2022-01-03 08:28:27.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0008_mutedstructure.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1502 2022-01-09 01:56:52.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0009_add_more_types.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      508 2022-01-07 05:22:46.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0010_pingerconfig_discord_mute_channels.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1625 2022-02-03 09:31:36.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0011_auto_20220203_0840.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      407 2022-02-03 08:55:22.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/0012_fuelpingrecord_last_message.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        0 2021-11-07 10:26:32.000000 allianceauth-corptools-pinger-0.3.1/pinger/migrations/__init__.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     9069 2022-05-15 10:48:10.000000 allianceauth-corptools-pinger-0.3.1/pinger/models.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)    68109 2022-05-15 13:58:57.000000 allianceauth-corptools-pinger-0.3.1/pinger/notifications.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      303 2022-01-31 14:20:48.000000 allianceauth-corptools-pinger-0.3.1/pinger/providers.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)    19765 2022-05-15 12:39:12.000000 allianceauth-corptools-pinger-0.3.1/pinger/tasks.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       38 2022-05-25 09:55:55.489480 allianceauth-corptools-pinger-0.3.1/setup.cfg
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1319 2022-05-14 08:26:27.000000 allianceauth-corptools-pinger-0.3.1/setup.py
-drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2022-05-25 09:55:55.489480 allianceauth-corptools-pinger-0.3.1/tests/
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       67 2021-08-11 06:51:26.000000 allianceauth-corptools-pinger-0.3.1/tests/__init__.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      625 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/tests/celery.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1170 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/tests/test_settings.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      347 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.1/tests/urls.py
--rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      103 2021-08-11 06:51:26.000000 allianceauth-corptools-pinger-0.3.1/tests/views.py
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.503087 allianceauth-corptools-pinger-0.3.3/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       31 2021-11-24 09:23:40.000000 allianceauth-corptools-pinger-0.3.3/MANIFEST.in
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2584 2023-07-29 11:07:26.503087 allianceauth-corptools-pinger-0.3.3/PKG-INFO
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1785 2022-02-19 10:18:43.000000 allianceauth-corptools-pinger-0.3.3/README.md
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.493087 allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2584 2023-07-29 11:07:26.000000 allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/PKG-INFO
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1364 2023-07-29 11:07:26.000000 allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        1 2023-07-29 11:07:26.000000 allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       50 2023-07-29 11:07:26.000000 allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/requires.txt
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       13 2023-07-29 11:07:26.000000 allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/top_level.txt
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.493087 allianceauth-corptools-pinger-0.3.3/pinger/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       22 2023-07-29 10:46:05.000000 allianceauth-corptools-pinger-0.3.3/pinger/__init__.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     9753 2023-07-29 10:46:05.000000 allianceauth-corptools-pinger-0.3.3/pinger/admin.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      179 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/apps.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      289 2021-11-24 10:14:10.000000 allianceauth-corptools-pinger-0.3.3/pinger/auth_hooks.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     8022 2023-07-29 10:46:05.000000 allianceauth-corptools-pinger-0.3.3/pinger/cogs.py
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.493087 allianceauth-corptools-pinger-0.3.3/pinger/management/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        0 2021-11-24 09:22:09.000000 allianceauth-corptools-pinger-0.3.3/pinger/management/__init__.py
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.493087 allianceauth-corptools-pinger-0.3.3/pinger/management/commands/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        0 2021-11-24 08:51:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/management/commands/__init.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2481 2023-06-09 13:27:04.000000 allianceauth-corptools-pinger-0.3.3/pinger/management/commands/pinger_stats.py
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.503087 allianceauth-corptools-pinger-0.3.3/pinger/migrations/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2669 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0001_initial.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1154 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0002_create_ping_types.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     2155 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0003_auto_20211108_0024.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1284 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0004_create_more_types.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1027 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0005_pingerconfig.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      424 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0006_create_settings.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      499 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0007_create_more_types_again.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      612 2022-01-03 08:28:27.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0008_mutedstructure.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1502 2022-01-09 01:56:52.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0009_add_more_types.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      508 2022-01-07 05:22:46.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0010_pingerconfig_discord_mute_channels.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1625 2022-02-03 09:31:36.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0011_auto_20220203_0840.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      407 2022-02-03 08:55:22.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0012_fuelpingrecord_last_message.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      408 2022-08-21 15:19:04.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0013_discordwebhook_no_at_pings.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      900 2023-04-16 09:24:12.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0014_structurelothreshold.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      625 2023-06-09 10:32:08.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/0015_add_more_types.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)        0 2021-11-07 10:26:32.000000 allianceauth-corptools-pinger-0.3.3/pinger/migrations/__init__.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     9415 2023-07-29 10:46:05.000000 allianceauth-corptools-pinger-0.3.3/pinger/models.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)    74613 2023-06-09 13:27:25.000000 allianceauth-corptools-pinger-0.3.3/pinger/notifications.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      303 2022-01-31 14:20:48.000000 allianceauth-corptools-pinger-0.3.3/pinger/providers.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)    24788 2023-07-29 10:57:16.000000 allianceauth-corptools-pinger-0.3.3/pinger/tasks.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       38 2023-07-29 11:07:26.503087 allianceauth-corptools-pinger-0.3.3/setup.cfg
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1319 2022-05-14 08:26:27.000000 allianceauth-corptools-pinger-0.3.3/setup.py
+drwxr-xr-x   0 aaronkable  (1000) aaronkable  (1000)        0 2023-07-29 11:07:26.503087 allianceauth-corptools-pinger-0.3.3/tests/
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)       67 2021-08-11 06:51:26.000000 allianceauth-corptools-pinger-0.3.3/tests/__init__.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      625 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/tests/celery.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)     1170 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/tests/test_settings.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      347 2022-01-03 08:28:26.000000 allianceauth-corptools-pinger-0.3.3/tests/urls.py
+-rw-r--r--   0 aaronkable  (1000) aaronkable  (1000)      103 2021-08-11 06:51:26.000000 allianceauth-corptools-pinger-0.3.3/tests/views.py
```

### Comparing `allianceauth-corptools-pinger-0.3.1/PKG-INFO` & `allianceauth-corptools-pinger-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-corptools-pinger
-Version: 0.3.1
+Version: 0.3.3
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/Solar-Helix-Independent-Transport/allianceauth-corp-tools-pinger
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-corptools-pinger-0.3.1/README.md` & `allianceauth-corptools-pinger-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/PKG-INFO` & `allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-corptools-pinger
-Version: 0.3.1
+Version: 0.3.3
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/Solar-Helix-Independent-Transport/allianceauth-corp-tools-pinger
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-corptools-pinger-0.3.1/allianceauth_corptools_pinger.egg-info/SOURCES.txt` & `allianceauth-corptools-pinger-0.3.3/allianceauth_corptools_pinger.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,13 +26,16 @@
 pinger/migrations/0006_create_settings.py
 pinger/migrations/0007_create_more_types_again.py
 pinger/migrations/0008_mutedstructure.py
 pinger/migrations/0009_add_more_types.py
 pinger/migrations/0010_pingerconfig_discord_mute_channels.py
 pinger/migrations/0011_auto_20220203_0840.py
 pinger/migrations/0012_fuelpingrecord_last_message.py
+pinger/migrations/0013_discordwebhook_no_at_pings.py
+pinger/migrations/0014_structurelothreshold.py
+pinger/migrations/0015_add_more_types.py
 pinger/migrations/__init__.py
 tests/__init__.py
 tests/celery.py
 tests/test_settings.py
 tests/urls.py
 tests/views.py
```

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/admin.py` & `allianceauth-corptools-pinger-0.3.3/pinger/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -89,14 +89,82 @@
             logger.warning(msg)
         else:
             msg = f"{w.nickname}: failed ({response.status_code})"
             messages.error(request, msg)
             logger.error(msg)
 
 
+
+@admin.action(description='Send Test Ping')
+def sendTestPing(DiscordWebhook, request, queryset):
+    for w in queryset:
+        types = w.ping_types.all().values_list('name', flat=True)
+        corps = w.corporation_filter.all().values_list('corporation_name', flat=True)
+        if len(corps) == 0:
+            corps = ["None"]
+
+        allis = w.alliance_filter.all().values_list('alliance_name', flat=True)
+        if len(allis) == 0:
+            allis = ["None"]
+
+        regions = w.region_filter.all().values_list('name', flat=True)
+        if len(regions) == 0:
+            regions = ["None"]
+
+        payload = {"embeds": [
+            {
+                "title": "Ping Channel Test",
+                "description": "Configured Notifications:\n\n```{}```".format('\n'.join(types)),
+                "color": 10181046,
+                "fields": [
+                    {
+                        "name": "Fuel Levels",
+                                "value": "Ping Fuel: {}\nPing LO: {}".format(w.fuel_pings, w.lo_pings)
+                    },
+                    {
+                        "name": "Corportaion Filter",
+                                "value": "{}".format('\n'.join(corps))
+                    },
+                    {
+                        "name": "Alliance Filter",
+                                "value": "{}".format('\n'.join(allis))
+                    },
+                    {
+                        "name": "Region Filter",
+                                "value": "{}".format('\n'.join(regions))
+                    }
+                ]
+            }
+        ]
+        }
+        payload = json.dumps(payload)
+        url = w.discord_webhook
+        custom_headers = {'Content-Type': 'application/json'}
+        response = requests.post(url,
+                                 headers=custom_headers,
+                                 data=payload,
+                                 params={'wait': True})
+
+        if response.status_code in [200, 204]:
+            msg = f"{w.nickname}: Test Ping Sent!"
+            messages.success(request, msg)
+            logger.debug(msg)
+        elif response.status_code == 429:
+
+            errors = json.loads(response.content.decode('utf-8'))
+            wh_sleep = (int(errors['retry_after']) / 1000) + 0.15
+            msg = f"{w.nickname}: rate limited: try again in {wh_sleep} seconds..."
+            messages.warning(request, msg)
+            logger.warning(msg)
+        else:
+            msg = f"{w.nickname}: failed ({response.status_code})"
+            messages.error(request, msg)
+            logger.error(msg)
+
+
 class DiscordWebhookAdmin(admin.ModelAdmin):
     filter_horizontal = ('ping_types',
                          'corporation_filter',
                          'region_filter',
                          'alliance_filter')
     actions = [sendTestPing]
```

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/cogs.py` & `allianceauth-corptools-pinger-0.3.3/pinger/cogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from allianceauth.services.modules.discord.models import DiscordUser
 from discord.ext import commands
 from discord.commands import SlashCommandGroup, Option
 
 from discord import AutocompleteContext
 # AA Contexts
 from corptools.models import CharacterAudit, MapSystemMoon
+from corptools.models import CharacterAudit
 from django.conf import settings
 from django.db.models.query_utils import Q
 from allianceauth.eveonline.models import EveCharacter
 import pinger
 
 from pinger.tasks import get_settings, _get_cache_data_for_corp
 from pinger.models import MutedStructure, PingerConfig
```

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/management/commands/pinger_stats.py` & `allianceauth-corptools-pinger-0.3.3/pinger/management/commands/pinger_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class Command(BaseCommand):
     help = 'Spit out stats for pinger'
 
     def handle(self, *args, **options):
         self.stdout.write("Reading Settings!")
 
         allis, corps, _ = get_settings()
-
         self.stdout.write("Looking for Valid Corps:")
 
         # get all new corps not in cache
         all_member_corps_in_audit = CharacterAudit.objects.filter((Q(characterroles__station_manager=True) | Q(characterroles__personnel_manager=True)),
                                                                   character__character_ownership__user__profile__state__name__in=[
                                                                       "Member"],
                                                                   active=True)
```

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0001_initial.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0002_create_ping_types.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0002_create_ping_types.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0003_auto_20211108_0024.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0003_auto_20211108_0024.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0004_create_more_types.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0004_create_more_types.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0005_pingerconfig.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0005_pingerconfig.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0008_mutedstructure.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0008_mutedstructure.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0009_add_more_types.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0009_add_more_types.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/migrations/0011_auto_20220203_0840.py` & `allianceauth-corptools-pinger-0.3.3/pinger/migrations/0011_auto_20220203_0840.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/models.py` & `allianceauth-corptools-pinger-0.3.3/pinger/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from os import nice
+
 from django.core.exceptions import ValidationError
 from django.db import models
 from allianceauth.eveonline.models import EveAllianceInfo, EveCorporationInfo
 from corptools.models import MapRegion, Structure
 from django.db.models.deletion import CASCADE
 from django.utils import timezone
 from datetime import timedelta
@@ -38,14 +38,16 @@
 
     ping_types = models.ManyToManyField(PingType,
                                         blank=True)
 
     fuel_pings = models.BooleanField(default=False)
     lo_pings = models.BooleanField(default=False)
 
+    no_at_pings = models.BooleanField(default=False)
+
     def __str__(self):
         return f"{self.nickname} - {self.discord_webhook[-10:]}"
 
 
 class Ping(models.Model):
     notification_id = models.BigIntegerField()
     hook = models.ForeignKey(DiscordWebhook, on_delete=models.CASCADE)
@@ -218,7 +220,17 @@
     date_added = models.DateTimeField(auto_now=True)
 
     def expired(self):
         return timezone.now() > (self.date_added + timedelta(hours=48))
 
     def __str__(self):
         return f"{self.structure_id}"
+
+
+class StructureLoThreshold(models.Model):
+    structure = models.OneToOneField(
+        Structure, related_name="lo_th", on_delete=models.CASCADE)
+    low = models.IntegerField(default=1500000)
+    critical = models.IntegerField(default=250000)
+
+    def __str__(self):
+        return f"{self.structure.name}"
```

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/notifications.py` & `allianceauth-corptools-pinger-0.3.3/pinger/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from corptools import models as ctm
 from corptools.task_helpers.update_tasks import fetch_location_name
 
 from .models import MutedStructure
 from .providers import cache_client
 
 from django.utils.html import strip_tags
+from django.utils import timezone
 import logging
 from django.apps import apps
 
 logger = logging.getLogger(__name__)
 
 
 def timers_enabled():
@@ -175,15 +176,15 @@
             self._data['typeID'])
         moon_name, _ = ctm.MapSystemMoon.objects.get_or_create_from_esi(
             self._data['moonID'])
 
         owner, _ = ctm.EveName.objects.get_or_create_from_esi(
             self._data['corpID'])
 
-        alliance = "-" if owner.alliance is None else owner.alliance
+        alliance = "-" if owner.alliance is None else owner.alliance.name
 
         title = "Tower Anchoring!"
 
         body = (f"{structure_type.name}\n**{moon_name.name}**\n\n[{owner.name}]"
                 f"(https://zkillboard.com/search/{owner.name.replace(' ', '%20')}/),"
                 f" **[{alliance}](https://zkillboard.com/search/{alliance.replace(' ', '%20')}/)**")
 
@@ -1782,7 +1783,157 @@
                           fields=fields,
                           footer=footer,
                           colour=15158332)
 
         self._corp = self._notification.character.character.corporation_id
         self._alli = self._notification.character.character.alliance_id
         self.force_at_ping = False
+
+
+class OrbitalAttacked(NotificationPing):
+    category = "orbital-attack"  # Structure Alerts
+
+    """
+    aggressorAllianceID: null
+    aggressorCorpID: 98729563
+    aggressorID: 90308296
+    planetID: 40066681
+    planetTypeID: 2016
+    shieldLevel: 0.0
+    solarSystemID: 30001046
+    typeID: 2233
+    """
+
+    def build_ping(self):
+        system_db = ctm.MapSystem.objects.get(
+            system_id=self._data['solarSystemID'])
+        planet_db, _ = ctm.MapSystemPlanet.objects.get_or_create_from_esi(
+            planet_id=self._data['planetID'])
+
+        system_name = system_db.name
+        region_name = system_db.constellation.region.name
+        planet_name = planet_db.name
+
+        system_name = f"[{planet_name}](http://evemaps.dotlan.net/system/{system_name.replace(' ', '_')})"
+        region_name = f"[{region_name}](http://evemaps.dotlan.net/region/{region_name.replace(' ', '_')})"
+
+        structure_type, _ = ctm.EveItemType.objects.get_or_create_from_esi(
+            self._data['typeID'])
+
+        title = "Poco Under Attack"
+        shld = float(self._data['shieldLevel'])*100
+        body = "{} under Attack!\nShield Level: {:.2f}%".format(
+            structure_type.name, shld)
+
+        corp_id = self._notification.character.character.corporation_id
+        corp_ticker = self._notification.character.character.corporation_ticker
+        footer = {"icon_url": "https://imageserver.eveonline.com/Corporation/%s_64.png" % (str(corp_id)),
+                  "text": "%s (%s)" % (self._notification.character.character.corporation_name, corp_ticker)}
+
+        attacking_char, _ = ctm.EveName.objects.get_or_create_from_esi(
+            self._data['aggressorID'])
+        attacking_corp, _ = ctm.EveName.objects.get_or_create_from_esi(
+            self._data['aggressorCorpID'])
+
+        attacking_alli = None
+        if self._data['aggressorAllianceID']:
+            attacking_alli, _ = ctm.EveName.objects.get_or_create_from_esi(
+                self._data['aggressorAllianceID'])
+
+        attackerStr = "*[%s](https://zkillboard.com/search/%s/)*, [%s](https://zkillboard.com/search/%s/), **[%s](https://zkillboard.com/search/%s/)**" % \
+            (attacking_char.name,
+             attacking_char.name.replace(" ", "%20"),
+             attacking_corp.name,
+             attacking_corp.name.replace(" ", "%20"),
+             attacking_alli.name if attacking_alli else "*-*",
+             attacking_alli.name.replace(" ", "%20") if attacking_alli else "")
+
+        fields = [{'name': 'System/Planet', 'value': system_name, 'inline': True},
+                  {'name': 'Region', 'value': region_name, 'inline': True},
+                  {'name': 'Type', 'value': structure_type.name, 'inline': True},
+                  {'name': 'Attacker', 'value': attackerStr, 'inline': False}]
+
+        self.package_ping(title,
+                          body,
+                          self._notification.timestamp,
+                          fields=fields,
+                          footer=footer,
+                          colour=15158332)
+
+        self._corp = self._notification.character.character.corporation_id
+        self._alli = self._notification.character.character.alliance_id
+        self._region = system_db.constellation.region.region_id
+        self.force_at_ping = True
+
+
+class OrbitalReinforced(NotificationPing):
+    category = "orbital-attack"  # orbital-attack
+
+    """
+    aggressorAllianceID: null
+    aggressorCorpID: 98183625
+    aggressorID: 94416120
+    planetID: 40066687
+    planetTypeID: 2016
+    reinforceExitTime: 133307777010000000
+    solarSystemID: 30001046
+    typeID: 2233
+    """
+
+    def build_ping(self):
+        system_db = ctm.MapSystem.objects.get(
+            system_id=self._data['solarSystemID'])
+        planet_db, _ = ctm.MapSystemPlanet.objects.get_or_create_from_esi(
+            planet_id=self._data['planetID'])
+
+        system_name = system_db.name
+        planet_name = planet_db.name
+        system_name = f"[{planet_name}](http://evemaps.dotlan.net/system/{system_name.replace(' ', '_')})"
+        structure_type, _ = ctm.EveItemType.objects.get_or_create_from_esi(
+            self._data['typeID'])
+
+        _timeTill = filetime_to_dt(self._data['reinforceExitTime']).replace(
+            tzinfo=datetime.timezone.utc)
+        _refTimeDelta = _timeTill - timezone.now()
+        tile_till = format_timedelta(_refTimeDelta)
+
+        title = "Poco Reinforced"
+        body = f"{structure_type.name} has lost its Shields"
+
+        corp_id = self._notification.character.character.corporation_id
+        corp_ticker = self._notification.character.character.corporation_ticker
+        corp_name = "[%s](https://zkillboard.com/search/%s/)" % \
+            (self._notification.character.character.corporation_name,
+             self._notification.character.character.corporation_name.replace(" ", "%20"))
+        footer = {"icon_url": "https://imageserver.eveonline.com/Corporation/%s_64.png" % (str(corp_id)),
+                  "text": "%s (%s)" % (self._notification.character.character.corporation_name, corp_ticker)}
+
+        fields = [{'name': 'System', 'value': system_name, 'inline': True},
+                  {'name': 'Type', 'value': structure_type.name, 'inline': True},
+                  {'name': 'Owner', 'value': corp_name, 'inline': False},
+                  {'name': 'Time Till Out', 'value': tile_till, 'inline': False},
+                  {'name': 'Date Out', 'value': _timeTill.strftime("%Y-%m-%d %H:%M"), 'inline': False}]
+
+        self.package_ping(title,
+                          body,
+                          self._notification.timestamp,
+                          fields=fields,
+                          footer=footer,
+                          colour=7419530)
+
+        if timers_enabled():
+            try:
+                self.timer = create_timer(
+                    f"{planet_name} POCO",
+                    structure_type.name,
+                    system_db.name,
+                    TimerType.ARMOR,
+                    _timeTill,
+                    self._notification.character.character.corporation
+                )
+            except Exception as e:
+                logger.exception(
+                    "PINGER: Failed to build timer OrbitalReinforced")
+
+        self._corp = self._notification.character.character.corporation_id
+        self._alli = self._notification.character.character.alliance_id
+        self._region = system_db.constellation.region.region_id
```

### Comparing `allianceauth-corptools-pinger-0.3.1/pinger/tasks.py` & `allianceauth-corptools-pinger-0.3.3/pinger/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import time
 import datetime
 import logging
 import json
 from esi.models import Token
 import requests
+import hashlib
 
 from celery import shared_task
 from django.core.cache import cache
 from allianceauth.services.tasks import QueueOnce
 from django.utils import timezone
+from django.core.exceptions import ObjectDoesNotExist
 
 from oauthlib.oauth2.rfc6749.errors import InvalidGrantError
 
 from corptools.providers import esi
 from corptools.models import CharacterAudit, CorporationAudit, Structure
 
 from django.db.models import Q
 from django.db.models import Max
-from pinger.models import DiscordWebhook, FuelPingRecord, Ping, PingerConfig
+from pinger.models import DiscordWebhook, FuelPingRecord, Ping, PingerConfig, StructureLoThreshold
 
 from http.cookiejar import http2time
 
 from . import notifications
 from .providers import cache_client
 
 TZ_STRING = "%Y-%m-%dT%H:%M:%SZ"
 
 CACHE_TIME_SECONDS = 10*60
 
 TASK_PRIO = 3
 
+LOOK_BACK_HOURS = 6
+
+
 logger = logging.getLogger(__name__)
 
 alliances = []
 corporations = []
 min_time = 60
 last_update = 0
 
@@ -213,18 +218,144 @@
         else:
             old = FuelPingRecord.objects.filter(
                 last_ping_lo_level__isnull=True, structure=struct)
             if old.exists():
                 old.delete()
 
 
+def get_lo_key():
+    return "LO_LEVEL_HASH_KEY"
+
+
+def get_lo_ping_state():
+    return "21"
+
+
+def set_lo_ping_state(hash):
+    return
+
+
+def sort_structure_list(struct_list):
+    return [x.name for x in sorted(struct_list, key=lambda x: x.name)]
+
+
+@shared_task(bind=True, base=QueueOnce, max_retries=None)
+def corporation_lo_check(self, corporation_id):
+    logger.info(
+        f"PINGER: Starting LO Checks")
+    fuel_structures = Structure.objects.filter(
+        type_name_id=35841, corporation__corporation__corporation_id=corporation_id).order_by("name")
+
+    low = []
+    crit = []
+    unknown = []
+
+    for struct in fuel_structures:
+        th_low = 1500000
+        th_crit = 25000
+
+        try:
+            th_low = struct.lo_th.low
+            th_crit = struct.lo_th.critical
+        except ObjectDoesNotExist:
+            pass
+
+        loLeft = struct.ozone_level
+        if loLeft == False:
+            unknown.append(struct)
+            continue
+
+        if loLeft < th_low:
+            if 1 <= loLeft < th_crit:
+                crit.append(struct)
+                continue
+            elif th_crit <= loLeft:
+                low.append(struct)
+                continue
+        else:
+            pass
+
+    if len(crit) or len(low) or len(unknown):
+        # build it!
+        sorted_arrays = (
+            sort_structure_list(crit),
+            sort_structure_list(low),
+            sort_structure_list(unknown)
+        )
+
+        sorted_hash = hashlib.md5(json.dumps(
+            sorted_arrays).encode()).hexdigest()
+
+        if get_lo_ping_state() == sorted_hash:
+            set_lo_ping_state(sorted_hash)
+            return
+        else:
+            # send pings
+            embed = {'color': 15158332,
+                     'title': "Liquid Ozone State",
+                     'description': ""
+                     }
+            gap = "               "
+            desc = []
+            if len(crit):
+                desc.append("\n**Critical Ozone Levels:**")
+                crit_block = [
+                    f"{s.ozone_level:,}{gap[len(f'{s.ozone_level:,}'):15]}{s.name}" for s in crit]
+                crit_block = "\n".join(crit_block)
+                desc.append(f'```Liquid Ozone   Structure\n{crit_block}```')
+            if len(low):
+                desc.append("\n**Low Ozone Levels:**")
+                low_block = [
+                    f"{s.ozone_level:,}{gap[len(f'{s.ozone_level:,}'):15]}{s.name}" for s in low]
+                low_block = "\n".join(low_block)
+                desc.append(f'```Liquid Ozone   Structure\n{low_block}```')
+            if len(unknown):
+                desc.append("\n**Unknown Ozone Levels:**")
+                unknown_block = [f" -             {s.name}" for s in low]
+                unknown_block = "\n".join[unknown_block]
+                desc.append(f'```~~Liquid Ozone~~   Structure\n{low_block}```')
+
+            embed["description"] = "\n".join(desc)
+
+            set_lo_ping_state(sorted_hash)
+
+            webhooks = DiscordWebhook.objects.filter(lo_pings=True)\
+                .prefetch_related("alliance_filter", "corporation_filter", "region_filter")
+            logger.info(
+                f"PINGER: FUEL Webhooks {webhooks.count()}")
+
+            for hook in webhooks:
+                corporations = hook.corporation_filter.all(
+                ).values_list("corporation_id", flat=True)
+
+                corp_filter = corporation_id
+
+                if corp_filter is not None and len(corporations) > 0:
+                    if corp_filter not in corporations:
+                        logger.info(
+                            f"PINGER: FUEL  Skipped {self.structure.name} Corp {corp_filter} not in {corporations}")
+                        continue
+
+                alert = False
+                p = Ping.objects.create(notification_id=-1,
+                                        hook=hook,
+                                        body=json.dumps(embed),
+                                        time=timezone.now(),
+                                        alerting=alert
+                                        )
+                p.send_ping()
+
+                return embed
+
+
 @shared_task(bind=True, base=QueueOnce, max_retries=None)
 def corporation_notification_update(self, corporation_id):
     # get oldest token and update notifications chained with a notification check
     data = _get_cache_data_for_corp(corporation_id)
+    CUTTOFF = timezone.now() - datetime.timedelta(hours=LOOK_BACK_HOURS)
 
     if data:
         last_character = data[0]
 
         logger.info(
             f"PINGER: {corporation_id} Last Update was with {last_character}")
 
@@ -232,14 +363,18 @@
                                                               character__corporation_id=corporation_id,
                                                               active=True).values_list("character__character_id", flat=True))
 
         all_hr_chars = list(set(CharacterAudit.objects.filter(characterroles__personnel_manager=True,
                                                               character__corporation_id=corporation_id,
                                                               active=True).values_list("character__character_id", flat=True)))
 
+        all_hr_chars = list(set(CharacterAudit.objects.filter(characterroles__personnel_manager=True,
+                                                              character__corporation_id=corporation_id,
+                                                              active=True).values_list("character__character_id", flat=True)))
+
         # todo make this nicer...
         if len(all_hr_chars) > 0:
             hr_presented = False
             for i in all_hr_chars:
                 if i in all_chars_in_corp:
                     hr_presented = True
                     logger.info(
@@ -297,15 +432,15 @@
         notifs.request_config.also_return_response = True
         notifs, response = notifs.results()
 
         now = time.mktime(timezone.now().timetuple())
         next_expire = http2time(response.headers.get('Expires'))
 
         secs_till_expire = next_expire - now
-
+        print(secs_till_expire)
         if next_expire == last_expire:
             logger.info(f"PINGER: CACHE: Same Cache as last update.")
         if secs_till_expire < 30:
             logger.warning(
                 f"PINGER: CACHE: Almost expired cache {token.character_name}, retrying with this character in {secs_till_expire + 1} seconds")
             _set_cache_data_for_corp(
                 corporation_id, last_character, all_chars_in_corp, 0)
@@ -316,20 +451,21 @@
             self.retry(countdown=1)
 
         _set_last_cache_expire(character_id, next_expire)
 
         pingable_notifs = []
         pinged_already = set(
             list(Ping.objects.values_list("notification_id", flat=True)))
-        cuttoff = timezone.now() - datetime.timedelta(hours=1)
 
         for n in notifs:
-            if n.get('timestamp') > cuttoff:
+            if n.get('timestamp') > CUTTOFF:
                 if n.get('type') in types.keys():
                     if n.get('notification_id') not in pinged_already:
+                        n['time'] = datetime.datetime.timestamp(
+                            n.get('timestamp'))
                         pingable_notifs.append(n)
 
         logger.info(
             f"PINGER: {corporation_id} Pings to process: {len(pingable_notifs)}")
 
         # did we get any?
         process_notifications.apply_async(priority=TASK_PRIO, args=[
@@ -364,22 +500,23 @@
         self.timestamp = timestamp
         self.notification_type = notification_type
         self.notification_text = notification_text
 
 
 @shared_task(bind=True, base=QueueOnce)
 def process_notifications(self, cid, notifs):
-    cuttoff = timezone.now() - datetime.timedelta(hours=1)
     char = CharacterAudit.objects.get(character__character_id=cid)
     new_notifs = []
+    CUTTOFF = timezone.now() - datetime.timedelta(hours=LOOK_BACK_HOURS)
 
     for note in notifs:
-        note['timestamp'] = datetime.datetime.fromisoformat(
-            note.get('timestamp').replace("Z", "+00:00"))
-        if note.get('timestamp') > cuttoff:
+        if not isinstance(note['timestamp'], datetime.datetime):
+            note['timestamp'] = datetime.datetime.fromtimestamp(
+                note.get('time'), tz=datetime.timezone.utc)
+        if note.get('timestamp') > CUTTOFF:
             logger.info(
                 f"PINGER: {char} Got Notification {note.get('notification_id')} {note.get('type')} {note.get('timestamp')}")
 
             n = Notification(character=char,
                              notification_id=note.get(
                                  'notification_id'),
                              timestamp=note.get('timestamp'),
@@ -387,15 +524,15 @@
                              notification_text=note.get('text'))
             new_notifs.append(n)
 
     pings = {}
     # grab all notifications within scope.
     types = notifications.get_available_types()
     pinged_already = set(list(Ping.objects.filter(
-        time__gte=cuttoff).values_list("notification_id", flat=True)))
+        time__gte=(CUTTOFF-datetime.timedelta(days=1))).values_list("notification_id", flat=True)))
     # parse them into the parsers
     for n in new_notifs:
         if n.notification_id not in pinged_already:
             pinged_already.add(n.notification_id)
             try:
                 note = types[n.notification_type](n)
                 if n.notification_type not in pings:
@@ -472,14 +609,16 @@
     else:
         return 0
 
 
 @shared_task(bind=True, max_retries=None)
 def send_ping(self, ping_id):
     ping_ob = Ping.objects.get(id=ping_id)
+    CUTTOFF = timezone.now() - datetime.timedelta(hours=LOOK_BACK_HOURS)
+
     if ping_ob.notification_id > 0:
         saved = cache_client.sadd(
             "ct-pinger-ping-lock-set", f"{ping_id}{ping_ob.notification_id}")
         if saved == 0:
             logger.info(
                 f"PINGER: DUPLICATE skipping {ping_ob.notification_id}")
             ping_ob.ping_sent = True
@@ -491,16 +630,19 @@
         logger.warning(
             f"Webhook rate limited: trying again in {wh_sleep} seconds...")
         self.retry(countdown=wh_sleep)
 
     if ping_ob.ping_sent == True:
         return "Already done!"
 
+    if ping_ob.time < CUTTOFF:
+        return "TOO OLD!"
+
     alertText = ""
-    if ping_ob.alerting == True:
+    if ping_ob.alerting and not ping_ob.hook.no_at_pings:
         alertText = '"content": "@here", '
 
     payload = '{%s"embeds": [%s]}' % (
         alertText,
         ping_ob.body
     )
```

### Comparing `allianceauth-corptools-pinger-0.3.1/setup.py` & `allianceauth-corptools-pinger-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/tests/celery.py` & `allianceauth-corptools-pinger-0.3.3/tests/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-corptools-pinger-0.3.1/tests/test_settings.py` & `allianceauth-corptools-pinger-0.3.3/tests/test_settings.py`

 * *Files identical despite different names*

