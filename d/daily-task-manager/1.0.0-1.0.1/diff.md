# Comparing `tmp/daily-task-manager-1.0.0.tar.gz` & `tmp/daily-task-manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daily-task-manager-1.0.0.tar", last modified: Sat Jul 29 15:47:53 2023, max compression
+gzip compressed data, was "daily-task-manager-1.0.1.tar", last modified: Sat Jul 29 16:55:01 2023, max compression
```

## Comparing `daily-task-manager-1.0.0.tar` & `daily-task-manager-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 15:47:53.899670 daily-task-manager-1.0.0/
--rw-rw-rw-   0        0        0      153 2023-07-29 15:47:53.898675 daily-task-manager-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2790 2023-07-29 15:42:28.000000 daily-task-manager-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 15:47:53.873673 daily-task-manager-1.0.0/daily_task_manager/
--rw-rw-rw-   0        0        0        0 2023-07-29 15:22:38.000000 daily-task-manager-1.0.0/daily_task_manager/__init__.py
--rw-rw-rw-   0        0        0     9829 2023-07-29 15:36:16.000000 daily-task-manager-1.0.0/daily_task_manager/script.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:47:53.895680 daily-task-manager-1.0.0/daily_task_manager.egg-info/
--rw-rw-rw-   0        0        0      153 2023-07-29 15:47:53.000000 daily-task-manager-1.0.0/daily_task_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-07-29 15:47:53.000000 daily-task-manager-1.0.0/daily_task_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 15:47:53.000000 daily-task-manager-1.0.0/daily_task_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-29 15:47:53.000000 daily-task-manager-1.0.0/daily_task_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 15:47:53.000000 daily-task-manager-1.0.0/daily_task_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-29 15:47:53.000000 daily-task-manager-1.0.0/daily_task_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 15:47:53.900673 daily-task-manager-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-07-29 15:24:32.000000 daily-task-manager-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:55:01.104043 daily-task-manager-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-07-29 16:49:59.000000 daily-task-manager-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      176 2023-07-29 16:55:01.104043 daily-task-manager-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2790 2023-07-29 15:42:28.000000 daily-task-manager-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 16:55:01.072044 daily-task-manager-1.0.1/daily_task_manager/
+-rw-rw-rw-   0        0        0        0 2023-07-29 15:22:38.000000 daily-task-manager-1.0.1/daily_task_manager/__init__.py
+-rw-rw-rw-   0        0        0     9829 2023-07-29 15:36:16.000000 daily-task-manager-1.0.1/daily_task_manager/script.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:55:01.104043 daily-task-manager-1.0.1/daily_task_manager.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-29 16:55:00.000000 daily-task-manager-1.0.1/daily_task_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-29 16:55:00.000000 daily-task-manager-1.0.1/daily_task_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:55:00.000000 daily-task-manager-1.0.1/daily_task_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-29 16:55:00.000000 daily-task-manager-1.0.1/daily_task_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 16:55:00.000000 daily-task-manager-1.0.1/daily_task_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-29 16:55:00.000000 daily-task-manager-1.0.1/daily_task_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      502 2023-07-29 16:54:41.000000 daily-task-manager-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:55:01.104043 daily-task-manager-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-07-29 16:54:34.000000 daily-task-manager-1.0.1/setup.py
```

### Comparing `daily-task-manager-1.0.0/README.md` & `daily-task-manager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `daily-task-manager-1.0.0/daily_task_manager/script.py` & `daily-task-manager-1.0.1/daily_task_manager/script.py`

 * *Files identical despite different names*

