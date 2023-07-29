# Comparing `tmp/sciolyid-2.0.1.tar.gz` & `tmp/sciolyid-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciolyid-2.0.1.tar", last modified: Sun Jan  1 23:34:16 2023, max compression
+gzip compressed data, was "sciolyid-2.0.2.tar", last modified: Sat Jul 29 20:45:47 2023, max compression
```

## Comparing `sciolyid-2.0.1.tar` & `sciolyid-2.0.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.101322 sciolyid-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-01 23:34:03.000000 sciolyid-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-01-01 23:34:16.101322 sciolyid-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-01-01 23:34:03.000000 sciolyid-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.089321 sciolyid-2.0.1/sciolyid/
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.093321 sciolyid-2.0.1/sciolyid/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/media.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/race.py
--rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/score.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/cogs/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/data_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    18621 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.097321 sciolyid-2.0.1/sciolyid/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/scripts/find_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/scripts/generate_file_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/scripts/generate_wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/scripts/install_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/scripts/restore_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/start_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.097321 sciolyid-2.0.1/sciolyid/web/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.101322 sciolyid-2.0.1/sciolyid/web/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/blueprints/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/blueprints/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/blueprints/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/blueprints/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.101322 sciolyid-2.0.1/sciolyid/web/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/functions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/functions/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/functions/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.101322 sciolyid-2.0.1/sciolyid/web/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-01-01 23:34:03.000000 sciolyid-2.0.1/sciolyid/web/tasks/git_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 23:34:16.089321 sciolyid-2.0.1/sciolyid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-01-01 23:34:15.000000 sciolyid-2.0.1/sciolyid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-01 23:34:15.000000 sciolyid-2.0.1/sciolyid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 23:34:15.000000 sciolyid-2.0.1/sciolyid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-01 23:34:15.000000 sciolyid-2.0.1/sciolyid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-01 23:34:15.000000 sciolyid-2.0.1/sciolyid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-01 23:34:16.101322 sciolyid-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-01-01 23:34:03.000000 sciolyid-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.126159 sciolyid-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 20:45:38.000000 sciolyid-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-29 20:45:47.126159 sciolyid-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-29 20:45:38.000000 sciolyid-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/race.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/cogs/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/data_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18621 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/scripts/find_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/scripts/generate_file_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/scripts/generate_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/scripts/install_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/scripts/restore_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/start_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid/web/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/blueprints/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/blueprints/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/blueprints/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/blueprints/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid/web/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/functions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/functions/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/functions/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.126159 sciolyid-2.0.2/sciolyid/web/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-29 20:45:38.000000 sciolyid-2.0.2/sciolyid/web/tasks/git_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:45:47.122158 sciolyid-2.0.2/sciolyid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-29 20:45:47.000000 sciolyid-2.0.2/sciolyid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-29 20:45:47.000000 sciolyid-2.0.2/sciolyid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:45:47.000000 sciolyid-2.0.2/sciolyid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-29 20:45:47.000000 sciolyid-2.0.2/sciolyid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-29 20:45:47.000000 sciolyid-2.0.2/sciolyid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:45:47.126159 sciolyid-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-29 20:45:38.000000 sciolyid-2.0.2/setup.py
```

### Comparing `sciolyid-2.0.1/LICENSE` & `sciolyid-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/PKG-INFO` & `sciolyid-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sciolyid
-Version: 2.0.1
+Version: 2.0.2
 Summary: Create ID Discord bots for SciOly studying.
 Home-page: https://github.com/tctree333/SciOly-ID
 Author: Tomi Chen
-Author-email: tomichen33@gmail.com
+Author-email: pypi@tomichen.com
 License: GPLv3+
 Keywords: science_olympiad discord_bot discord studying
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: web
 License-File: LICENSE
 
 # SciOly-ID-Discord-Bots
```

### Comparing `sciolyid-2.0.1/README.md` & `sciolyid-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/__init__.py` & `sciolyid-2.0.2/sciolyid/__init__.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/check.py` & `sciolyid-2.0.2/sciolyid/cogs/check.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/hint.py` & `sciolyid-2.0.2/sciolyid/cogs/hint.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/media.py` & `sciolyid-2.0.2/sciolyid/cogs/media.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/meta.py` & `sciolyid-2.0.2/sciolyid/cogs/meta.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/other.py` & `sciolyid-2.0.2/sciolyid/cogs/other.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/race.py` & `sciolyid-2.0.2/sciolyid/cogs/race.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/score.py` & `sciolyid-2.0.2/sciolyid/cogs/score.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/sessions.py` & `sciolyid-2.0.2/sciolyid/cogs/sessions.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/skip.py` & `sciolyid-2.0.2/sciolyid/cogs/skip.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/state.py` & `sciolyid-2.0.2/sciolyid/cogs/state.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/cogs/stats.py` & `sciolyid-2.0.2/sciolyid/cogs/stats.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/config.py` & `sciolyid-2.0.2/sciolyid/config.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/core.py` & `sciolyid-2.0.2/sciolyid/core.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/data.py` & `sciolyid-2.0.2/sciolyid/data.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/data_functions.py` & `sciolyid-2.0.2/sciolyid/data_functions.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/downloads.py` & `sciolyid-2.0.2/sciolyid/downloads.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/functions.py` & `sciolyid-2.0.2/sciolyid/functions.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/scripts/find_duplicates.py` & `sciolyid-2.0.2/sciolyid/scripts/find_duplicates.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/scripts/generate_file_structure.py` & `sciolyid-2.0.2/sciolyid/scripts/generate_file_structure.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/scripts/generate_wiki.py` & `sciolyid-2.0.2/sciolyid/scripts/generate_wiki.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/scripts/restore_backup.py` & `sciolyid-2.0.2/sciolyid/scripts/restore_backup.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/start_bot.py` & `sciolyid-2.0.2/sciolyid/start_bot.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/util.py` & `sciolyid-2.0.2/sciolyid/util.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/__init__.py` & `sciolyid-2.0.2/sciolyid/web/__init__.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/blueprints/about.py` & `sciolyid-2.0.2/sciolyid/web/blueprints/about.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/blueprints/upload.py` & `sciolyid-2.0.2/sciolyid/web/blueprints/upload.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/blueprints/user.py` & `sciolyid-2.0.2/sciolyid/web/blueprints/user.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/blueprints/verify.py` & `sciolyid-2.0.2/sciolyid/web/blueprints/verify.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/config.py` & `sciolyid-2.0.2/sciolyid/web/config.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/functions/images.py` & `sciolyid-2.0.2/sciolyid/web/functions/images.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/functions/user.py` & `sciolyid-2.0.2/sciolyid/web/functions/user.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/functions/webhooks.py` & `sciolyid-2.0.2/sciolyid/web/functions/webhooks.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/git.py` & `sciolyid-2.0.2/sciolyid/web/git.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/main.py` & `sciolyid-2.0.2/sciolyid/web/main.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/tasks/__init__.py` & `sciolyid-2.0.2/sciolyid/web/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid/web/tasks/git_tasks.py` & `sciolyid-2.0.2/sciolyid/web/tasks/git_tasks.py`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/sciolyid.egg-info/PKG-INFO` & `sciolyid-2.0.2/sciolyid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sciolyid
-Version: 2.0.1
+Version: 2.0.2
 Summary: Create ID Discord bots for SciOly studying.
 Home-page: https://github.com/tctree333/SciOly-ID
 Author: Tomi Chen
-Author-email: tomichen33@gmail.com
+Author-email: pypi@tomichen.com
 License: GPLv3+
 Keywords: science_olympiad discord_bot discord studying
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: web
 License-File: LICENSE
 
 # SciOly-ID-Discord-Bots
```

### Comparing `sciolyid-2.0.1/sciolyid.egg-info/SOURCES.txt` & `sciolyid-2.0.2/sciolyid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciolyid-2.0.1/setup.py` & `sciolyid-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setuptools.setup(
     name="sciolyid",
-    version="2.0.1",
+    version="2.0.2",
     description="Create ID Discord bots for SciOly studying.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords="science_olympiad discord_bot discord studying",
     license="GPLv3+",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     url="https://github.com/tctree333/SciOly-ID",
     author="Tomi Chen",
-    author_email="tomichen33@gmail.com",
+    author_email="pypi@tomichen.com",
     packages=setuptools.find_packages(),
     install_requires=[
-        "discord.py>=2.1.0, <3.0.0",
+        "discord.py>=2.3.1, <3.0.0",
         "redis>=3.3.5, <5.0.0",
         "sentry-sdk>=1.1.0, <2.0.0",
-        "Pillow>=9.0.1, <10.0.0",
+        "Pillow>=9.0.1, <11.0.0",
         "wikipedia>=1.4.0, <2.0.0",
         "gitpython>=3.0.6, <4.0.0",
         "hiredis>=1.0.1, <3.0.0",
-        "pandas>=1.3.0, <1.5.0",
+        "pandas>=1.3.0, <3.0.0",
         "filelock>=3.4.2, <3.7.0",
     ],
     extras_require={
         "web": [
             "Flask>=1.1.2, <2.1.0",
             "Authlib>=0.15.5, <1.0.0",
             "gunicorn>=20.0.4, <21.0.0",
```

