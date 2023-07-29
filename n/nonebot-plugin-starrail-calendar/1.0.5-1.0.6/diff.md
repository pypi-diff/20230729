# Comparing `tmp/nonebot_plugin_starrail_calendar-1.0.5.tar.gz` & `tmp/nonebot_plugin_starrail_calendar-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_starrail_calendar-1.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_starrail_calendar-1.0.6.tar", max compression
```

## Comparing `nonebot_plugin_starrail_calendar-1.0.5.tar` & `nonebot_plugin_starrail_calendar-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35823 2022-05-26 22:27:12.688017 nonebot_plugin_starrail_calendar-1.0.5/LICENSE
--rw-r--r--   0        0        0     5601 2023-07-23 04:22:45.835743 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/__init__.py
--rw-r--r--   0        0        0     2387 2022-10-25 13:40:10.642123 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/browser.py
--rw-r--r--   0        0        0      253 2023-05-14 14:40:54.472627 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/config.py
--rw-r--r--   0        0        0     4786 2023-07-23 04:20:12.757136 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/data_source.py
--rw-r--r--   0        0        0     1901 2023-05-02 03:04:38.808483 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/draw_calendar.py
--rw-r--r--   0        0        0     2371 2023-05-01 13:36:07.373205 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/calendar.html
--rw-r--r--   0        0        0     6882 2022-06-26 03:57:47.000000 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/index.css
--rw-r--r--   0        0        0   315626 2022-06-26 03:57:47.000000 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/iview.css
--rw-r--r--   0        0        0     6346 2022-06-26 03:57:47.000000 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/normalize.css
--rw-r--r--   0        0        0     2255 2023-04-29 01:27:19.441019 nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/utils.py
--rw-r--r--   0        0        0      547 2023-07-23 04:26:48.376437 nonebot_plugin_starrail_calendar-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      596 2023-05-09 12:37:06.326249 nonebot_plugin_starrail_calendar-1.0.5/README.md
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 nonebot_plugin_starrail_calendar-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-05-26 22:27:12.688017 nonebot_plugin_starrail_calendar-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5601 2023-07-23 04:22:45.835743 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/__init__.py
+-rw-r--r--   0        0        0     2387 2022-10-25 13:40:10.642123 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/browser.py
+-rw-r--r--   0        0        0      253 2023-05-14 14:40:54.472627 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/config.py
+-rw-r--r--   0        0        0     4786 2023-07-23 04:20:12.757136 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/data_source.py
+-rw-r--r--   0        0        0     1901 2023-05-02 03:04:38.808483 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/draw_calendar.py
+-rw-r--r--   0        0        0     2371 2023-05-01 13:36:07.373205 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/calendar.html
+-rw-r--r--   0        0        0     6882 2022-06-26 03:57:47.000000 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/index.css
+-rw-r--r--   0        0        0   315626 2022-06-26 03:57:47.000000 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/iview.css
+-rw-r--r--   0        0        0     6346 2022-06-26 03:57:47.000000 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/normalize.css
+-rw-r--r--   0        0        0     2255 2023-04-29 01:27:19.441019 nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/utils.py
+-rw-r--r--   0        0        0      531 2023-07-29 00:28:31.389882 nonebot_plugin_starrail_calendar-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      596 2023-05-09 12:37:06.326249 nonebot_plugin_starrail_calendar-1.0.6/README.md
+-rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 nonebot_plugin_starrail_calendar-1.0.6/PKG-INFO
```

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/LICENSE` & `nonebot_plugin_starrail_calendar-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/__init__.py` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/browser.py` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/data_source.py` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/draw_calendar.py` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/draw_calendar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/calendar.html` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/calendar.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/index.css` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/index.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/iview.css` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/iview.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/template/normalize.css` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/template/normalize.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/nonebot_plugin_starrail_calendar/utils.py` & `nonebot_plugin_starrail_calendar-1.0.6/nonebot_plugin_starrail_calendar/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/pyproject.toml` & `nonebot_plugin_starrail_calendar-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-starrail-calendar"
-version = "1.0.5"
+version = "1.0.6"
 description = "查看《崩坏：星穹铁道》官方活动"
 authors = ["nicklly <1134741727@qq.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_starrail_calendar"}]
 
 [tool.poetry.dependencies]
-python = "3.10.11"
 nonebot2 = "2.0.0rc4"
 nonebot-adapter-onebot = "2.2.2"
-playwright = "1.32.1"
-httpx = "0.23.3"
-apscheduler = "3.10.1"
-jinja2 = "3.1.2"
+playwright = "^1.32.1"
+httpx = "~0.23.3"
+apscheduler = "~3.10.1"
+jinja2 = "^3.1.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_starrail_calendar-1.0.5/README.md` & `nonebot_plugin_starrail_calendar-1.0.6/README.md`

 * *Files identical despite different names*

