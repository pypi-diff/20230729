# Comparing `tmp/unifi_protect_backup-0.9.3.tar.gz` & `tmp/unifi_protect_backup-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_protect_backup-0.9.3.tar", max compression
+gzip compressed data, was "unifi_protect_backup-0.9.4.tar", max compression
```

## Comparing `unifi_protect_backup-0.9.3.tar` & `unifi_protect_backup-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/LICENSE
--rw-r--r--   0        0        0    17222 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/README.md
--rw-r--r--   0        0        0     2131 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       50 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/tests/test_unifi_protect_backup.py
--rw-r--r--   0        0        0      359 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/__init__.py
--rw-r--r--   0        0        0     6416 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/cli.py
--rw-r--r--   0        0        0     9087 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/downloader.py
--rw-r--r--   0        0        0     5371 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/event_listener.py
--rw-r--r--   0        0        0     6704 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/missing_event_checker.py
--rw-r--r--   0        0        0      540 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/notifications.py
--rw-r--r--   0        0        0     3682 2023-07-08 16:39:29.001762 unifi_protect_backup-0.9.3/unifi_protect_backup/purge.py
--rw-r--r--   0        0        0    12747 2023-07-08 16:39:29.005762 unifi_protect_backup-0.9.3/unifi_protect_backup/unifi_protect_backup_core.py
--rw-r--r--   0        0        0     6365 2023-07-08 16:39:29.005762 unifi_protect_backup-0.9.3/unifi_protect_backup/uploader.py
--rw-r--r--   0        0        0    16858 2023-07-08 16:39:29.005762 unifi_protect_backup-0.9.3/unifi_protect_backup/utils.py
--rw-r--r--   0        0        0    18300 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-29 10:35:01.999399 unifi_protect_backup-0.9.4/LICENSE
+-rw-r--r--   0        0        0    17222 2023-07-29 10:35:01.999399 unifi_protect_backup-0.9.4/README.md
+-rw-r--r--   0        0        0     2131 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/tests/test_unifi_protect_backup.py
+-rw-r--r--   0        0        0      359 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/__init__.py
+-rw-r--r--   0        0        0     6370 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/cli.py
+-rw-r--r--   0        0        0     9087 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/downloader.py
+-rw-r--r--   0        0        0     5371 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/event_listener.py
+-rw-r--r--   0        0        0     6704 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/missing_event_checker.py
+-rw-r--r--   0        0        0      540 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/notifications.py
+-rw-r--r--   0        0        0     3682 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/purge.py
+-rw-r--r--   0        0        0    12747 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/unifi_protect_backup_core.py
+-rw-r--r--   0        0        0     6365 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/uploader.py
+-rw-r--r--   0        0        0    16858 2023-07-29 10:35:02.003399 unifi_protect_backup-0.9.4/unifi_protect_backup/utils.py
+-rw-r--r--   0        0        0    18300 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.4/PKG-INFO
```

### Comparing `unifi_protect_backup-0.9.3/LICENSE` & `unifi_protect_backup-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/README.md` & `unifi_protect_backup-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/pyproject.toml` & `unifi_protect_backup-0.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "unifi_protect_backup"
-version = "0.9.3"
+version = "0.9.4"
 homepage = "https://github.com/ep1cman/unifi-protect-backup"
 description = "Python tool to backup unifi event clips in realtime."
 authors = ["sebastian.goscik <sebastian@goscik.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
```

### Comparing `unifi_protect_backup-0.9.3/tests/test_unifi_protect_backup.py` & `unifi_protect_backup-0.9.4/tests/test_unifi_protect_backup.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/cli.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     " E.g. `gdrive:/backups/unifi_protect`",
 )
 @click.option(
     '--retention',
     default='7d',
     show_default=True,
     envvar='RCLONE_RETENTION',
-    help="How long should event clips be backed up for. Format as per the `--max-age` argument of "
-    "`rclone` (https://rclone.org/filtering/#max-age-don-t-transfer-any-file-older-than-this)",
+    help="How long should event clips be backed up for. Format as per the `rclone1 time option format "
+    "(https://rclone.org/docs/#time-option)",
 )
 @click.option(
     '--rclone-args',
     default='',
     envvar='RCLONE_ARGS',
     help="Optional extra arguments to pass to `rclone rcat` directly. Common usage for this would "
     "be to set a bandwidth limit, for example.",
```

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/downloader.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/downloader.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/event_listener.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/event_listener.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/missing_event_checker.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/missing_event_checker.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/notifications.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/notifications.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/purge.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/purge.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/unifi_protect_backup_core.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/unifi_protect_backup_core.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/uploader.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/uploader.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.3/unifi_protect_backup/utils.py` & `unifi_protect_backup-0.9.4/unifi_protect_backup/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         microseconds=matches.get("ms", 0) * 1000,
         seconds=matches.get("s", 0),
         minutes=matches.get("m", 0),
         hours=matches.get("h", 0),
         days=matches.get("d", 0),
         weeks=matches.get("w", 0),
         months=matches.get("M", 0),
-        years=matches.get("Y", 0),
+        years=matches.get("y", 0),
     )
 
 
 async def run_command(cmd: str, data=None):
     """Runs the given command returning the exit code, stdout and stderr."""
     proc = await asyncio.create_subprocess_shell(
         cmd,
```

### Comparing `unifi_protect_backup-0.9.3/PKG-INFO` & `unifi_protect_backup-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi-protect-backup
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python tool to backup unifi event clips in realtime.
 Home-page: https://github.com/ep1cman/unifi-protect-backup
 License: MIT
 Author: sebastian.goscik
 Author-email: sebastian@goscik.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

