# Comparing `tmp/ex4nicegui-0.2.5.tar.gz` & `tmp/ex4nicegui-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.2.5.tar", last modified: Sun Jul 23 07:22:38 2023, max compression
+gzip compressed data, was "ex4nicegui-0.2.6.tar", last modified: Sat Jul 29 10:19:35 2023, max compression
```

## Comparing `ex4nicegui-0.2.5.tar` & `ex4nicegui-0.2.6.tar`

### file list

```diff
@@ -1,70 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.136046 ex4nicegui-0.2.5/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-23 07:22:38.135048 ex4nicegui-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.027824 ex4nicegui-0.2.5/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-23 07:09:38.000000 ex4nicegui-0.2.5/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.042784 ex4nicegui-0.2.5/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.5/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.5/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.057744 ex4nicegui-0.2.5/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.066721 ex4nicegui-0.2.5/ex4nicegui/reactive/ECharts/
--rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/ECharts/ECharts.js
--rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/ECharts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/ECharts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.072705 ex4nicegui-0.2.5/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     4857 2023-07-23 07:06:08.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     2888 2023-07-23 06:34:34.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0      366 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/drawer.py
--rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/local_file_picker.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.118094 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/
--rw-rw-rw-   0        0        0     1330 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/aggrid.py
--rw-rw-rw-   0        0        0     4292 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/base.py
--rw-rw-rw-   0        0        0     2250 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/button.py
--rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/card.py
--rw-rw-rw-   0        0        0     1769 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/checkbox.py
--rw-rw-rw-   0        0        0     2744 2023-07-23 07:09:38.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/color_picker.py
--rw-rw-rw-   0        0        0     2700 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/date.py
--rw-rw-rw-   0        0        0     2443 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/drawer.py
--rw-rw-rw-   0        0        0     1783 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/echarts.py
--rw-rw-rw-   0        0        0     1687 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/html.py
--rw-rw-rw-   0        0        0     1600 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/icon.py
--rw-rw-rw-   0        0        0     1440 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/image.py
--rw-rw-rw-   0        0        0     3337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/input.py
--rw-rw-rw-   0        0        0     1756 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/label.py
--rw-rw-rw-   0        0        0     2080 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/radio.py
--rw-rw-rw-   0        0        0      404 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/row.py
--rw-rw-rw-   0        0        0     2482 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/select.py
--rw-rw-rw-   0        0        0     2607 2023-07-23 07:09:38.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/slider.py
--rw-rw-rw-   0        0        0     1979 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/switch.py
--rw-rw-rw-   0        0        0     3903 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/table.py
--rw-rw-rw-   0        0        0     2728 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/textarea.py
--rw-rw-rw-   0        0        0     2337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/upload.py
--rw-rw-rw-   0        0        0      205 2023-07-21 14:29:40.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/officials/utils.py
--rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/rxui.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.124076 ex4nicegui-0.2.5/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2468 2023-07-19 08:10:43.000000 ex4nicegui-0.2.5/ex4nicegui/reactive/usePagination.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.127068 ex4nicegui-0.2.5/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.5/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.5/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.133052 ex4nicegui-0.2.5/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.5/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.5/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.2.5/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-23 07:22:38.039794 ex4nicegui-0.2.5/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-23 07:22:37.000000 ex4nicegui-0.2.5/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2022 2023-07-23 07:22:37.000000 ex4nicegui-0.2.5/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 07:22:37.000000 ex4nicegui-0.2.5/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 07:22:37.000000 ex4nicegui-0.2.5/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-23 07:22:37.000000 ex4nicegui-0.2.5/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-23 07:22:37.000000 ex4nicegui-0.2.5/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 07:22:38.137043 ex4nicegui-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.162919 ex4nicegui-0.2.6/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-29 10:19:35.161945 ex4nicegui-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.028019 ex4nicegui-0.2.6/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-29 10:19:11.000000 ex4nicegui-0.2.6/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.043004 ex4nicegui-0.2.6/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.055945 ex4nicegui-0.2.6/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.091067 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.js
+-rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.096053 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     5235 2023-07-29 10:16:43.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3501 2023-07-29 10:16:43.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-07-29 10:16:25.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.097079 ex4nicegui-0.2.6/ex4nicegui/reactive/dropZone/
+-rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/dropZone/dropZone.js
+-rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/local_file_picker.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.145948 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/
+-rw-rw-rw-   0        0        0     1468 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/aggrid.py
+-rw-rw-rw-   0        0        0     4242 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/base.py
+-rw-rw-rw-   0        0        0     2250 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/button.py
+-rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/card.py
+-rw-rw-rw-   0        0        0     1769 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/checkbox.py
+-rw-rw-rw-   0        0        0     2744 2023-07-23 13:10:30.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/color_picker.py
+-rw-rw-rw-   0        0        0      413 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/column.py
+-rw-rw-rw-   0        0        0     2700 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/date.py
+-rw-rw-rw-   0        0        0     2443 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/drawer.py
+-rw-rw-rw-   0        0        0     1783 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/echarts.py
+-rw-rw-rw-   0        0        0      925 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/grid.py
+-rw-rw-rw-   0        0        0     1687 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/html.py
+-rw-rw-rw-   0        0        0     1600 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/icon.py
+-rw-rw-rw-   0        0        0     1440 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/image.py
+-rw-rw-rw-   0        0        0     3337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/input.py
+-rw-rw-rw-   0        0        0     1756 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/label.py
+-rw-rw-rw-   0        0        0     2058 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/number.py
+-rw-rw-rw-   0        0        0     2080 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/radio.py
+-rw-rw-rw-   0        0        0      404 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/row.py
+-rw-rw-rw-   0        0        0     2482 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/select.py
+-rw-rw-rw-   0        0        0     2607 2023-07-23 13:10:30.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/slider.py
+-rw-rw-rw-   0        0        0     1979 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/switch.py
+-rw-rw-rw-   0        0        0     3903 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/table.py
+-rw-rw-rw-   0        0        0     2728 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/textarea.py
+-rw-rw-rw-   0        0        0     2337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/upload.py
+-rw-rw-rw-   0        0        0      205 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/utils.py
+-rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.150937 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2468 2023-07-19 08:10:43.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.154897 ex4nicegui-0.2.6/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.6/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.6/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.159924 ex4nicegui-0.2.6/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.6/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.2.6/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.038990 ex4nicegui-0.2.6/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2181 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:19:35.162919 ex4nicegui-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.6/setup.py
```

### Comparing `ex4nicegui-0.2.5/LICENSE` & `ex4nicegui-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/README.md` & `ex4nicegui-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.2.6/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/ECharts/ECharts.js` & `ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/ECharts/ECharts.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,215 +1,241 @@
-const B = Vue.unref
-const N = Vue.isRef
-const T = Vue.toRefs
-const W = Vue.customRef
-const X = Vue.getCurrentScope
-const Y = Vue.onScopeDispose
-const D = Vue.ref
-const x = Vue.computed
+const U = Vue.unref
+const B = Vue.isRef
+const N = Vue.toRefs
+const T = Vue.customRef
+const W = Vue.getCurrentScope
+const X = Vue.onScopeDispose
+const x = Vue.ref
+const D = Vue.computed
 const h = Vue.watch
-const H = Vue.defineComponent
-const q = Vue.onMounted
+const Y = Vue.defineComponent
+const H = Vue.onMounted
 
-function z(e) {
-    return X() ? (Y(e), !0) : !1;
+function q(e) {
+    return W() ? (X(e), !0) : !1;
 }
 
-function p(e) {
-    return typeof e == "function" ? e() : B(e);
+function f(e) {
+    return typeof e == "function" ? e() : U(e);
 }
 const I = typeof window < "u",
-    F = () => {};
+    z = () => {};
 var G = Object.defineProperty,
     J = Object.defineProperties,
     K = Object.getOwnPropertyDescriptors,
     E = Object.getOwnPropertySymbols,
     Q = Object.prototype.hasOwnProperty,
     Z = Object.prototype.propertyIsEnumerable,
-    A = (e, r, t) => r in e ? G(e, r, {
+    A = (e, t, r) => t in e ? G(e, t, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
-        value: t
-    }) : e[r] = t,
-    j = (e, r) => {
-        for (var t in r || (r = {}))
-            Q.call(r, t) && A(e, t, r[t]);
+        value: r
+    }) : e[t] = r,
+    j = (e, t) => {
+        for (var r in t || (t = {}))
+            Q.call(t, r) && A(e, r, t[r]);
         if (E)
-            for (var t of E(r))
-                Z.call(r, t) && A(e, t, r[t]);
+            for (var r of E(t))
+                Z.call(t, r) && A(e, r, t[r]);
         return e;
     },
-    k = (e, r) => J(e, K(r));
+    k = (e, t) => J(e, K(t));
 
 function R(e) {
-    if (!N(e))
-        return T(e);
-    const r = Array.isArray(e.value) ? new Array(e.value.length) : {};
-    for (const t in e.value)
-        r[t] = W(() => ({
+    if (!B(e))
+        return N(e);
+    const t = Array.isArray(e.value) ? new Array(e.value.length) : {};
+    for (const r in e.value)
+        t[r] = T(() => ({
             get() {
-                return e.value[t];
+                return e.value[r];
             },
             set(o) {
                 if (Array.isArray(e.value)) {
                     const a = [...e.value];
-                    a[t] = o, e.value = a;
+                    a[r] = o, e.value = a;
                 } else {
                     const a = k(j({}, e.value), {
-                        [t]: o
+                        [r]: o
                     });
                     Object.setPrototypeOf(a, e.value), e.value = a;
                 }
             }
         }));
-    return r;
+    return t;
 }
 
 function ee(e) {
-    var r;
-    const t = p(e);
-    return (r = t == null ? void 0 : t.$el) != null ? r : t;
+    var t;
+    const r = f(e);
+    return (t = r == null ? void 0 : r.$el) != null ? t : r;
 }
-const C = I ? window : void 0;
+const F = I ? window : void 0;
 
 function $(...e) {
-    let r, t, o, a;
-    if (typeof e[0] == "string" || Array.isArray(e[0]) ? ([t, o, a] = e, r = C) : [r, t, o, a] = e, !r)
-        return F;
-    Array.isArray(t) || (t = [t]), Array.isArray(o) || (o = [o]);
-    const c = [],
-        g = () => {
-            c.forEach((i) => i()), c.length = 0;
+    let t, r, o, a;
+    if (typeof e[0] == "string" || Array.isArray(e[0]) ? ([r, o, a] = e, t = F) : [t, r, o, a] = e, !t)
+        return z;
+    Array.isArray(r) || (r = [r]), Array.isArray(o) || (o = [o]);
+    const v = [],
+        l = () => {
+            v.forEach((i) => i()), v.length = 0;
         },
-        _ = (i, y, s, v) => (i.addEventListener(y, s, v), () => i.removeEventListener(y, s, v)),
-        l = h(
-            () => [ee(r), p(a)],
-            ([i, y]) => {
-                g(), i && c.push(
-                    ...t.flatMap((s) => o.map((v) => _(i, s, v, y)))
+        d = (i, p, s, g) => (i.addEventListener(p, s, g), () => i.removeEventListener(p, s, g)),
+        u = h(
+            () => [ee(t), f(a)],
+            ([i, p]) => {
+                l(), i && v.push(
+                    ...r.flatMap((s) => o.map((g) => d(i, s, g, p)))
                 );
             }, {
                 immediate: !0,
                 flush: "post"
             }
         ),
-        f = () => {
-            l(), g();
+        y = () => {
+            u(), l();
         };
-    return z(f), f;
+    return q(y), y;
 }
-var re = Object.defineProperty,
-    te = Object.defineProperties,
+var te = Object.defineProperty,
+    re = Object.defineProperties,
     ne = Object.getOwnPropertyDescriptors,
-    b = Object.getOwnPropertySymbols,
+    S = Object.getOwnPropertySymbols,
     oe = Object.prototype.hasOwnProperty,
     ae = Object.prototype.propertyIsEnumerable,
-    S = (e, r, t) => r in e ? re(e, r, {
+    b = (e, t, r) => t in e ? te(e, t, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
-        value: t
-    }) : e[r] = t,
-    ie = (e, r) => {
-        for (var t in r || (r = {}))
-            oe.call(r, t) && S(e, t, r[t]);
-        if (b)
-            for (var t of b(r))
-                ae.call(r, t) && S(e, t, r[t]);
+        value: r
+    }) : e[t] = r,
+    ie = (e, t) => {
+        for (var r in t || (t = {}))
+            oe.call(t, r) && b(e, r, t[r]);
+        if (S)
+            for (var r of S(t))
+                ae.call(t, r) && b(e, r, t[r]);
         return e;
     },
-    se = (e, r) => te(e, ne(r));
+    se = (e, t) => re(e, ne(t));
 
-function le(e, r = {}) {
-    var t, o;
+function le(e, t = {}) {
+    var r, o;
     const {
         pointerTypes: a,
-        preventDefault: c,
-        stopPropagation: g,
-        exact: _,
-        onMove: l,
-        onEnd: f,
+        preventDefault: v,
+        stopPropagation: l,
+        exact: d,
+        onMove: u,
+        onEnd: y,
         onStart: i,
-        initialValue: y,
+        initialValue: p,
         axis: s = "both",
-        draggingElement: v = C,
-        handle: V = e
-    } = r, u = D(
-        (t = p(y)) != null ? t : {
+        draggingElement: g = F,
+        handle: C = e
+    } = t, c = x(
+        (r = f(p)) != null ? r : {
             x: 0,
             y: 0
         }
-    ), d = D(), P = (n) => a ? a.includes(n.pointerType) : !0, w = (n) => {
-        p(c) && n.preventDefault(), p(g) && n.stopPropagation();
-    }, L = (n) => {
-        if (!P(n) || p(_) && n.target !== p(e))
+    ), _ = x(), P = (n) => a ? a.includes(n.pointerType) : !0, w = (n) => {
+        f(v) && n.preventDefault(), f(l) && n.stopPropagation();
+    }, V = (n) => {
+        if (!P(n) || f(d) && n.target !== f(e))
             return;
-        const m = p(e).getBoundingClientRect(),
+        const m = f(e).getBoundingClientRect(),
             O = {
                 x: n.clientX - m.left,
                 y: n.clientY - m.top
             };
-        (i == null ? void 0 : i(O, n)) !== !1 && (d.value = O, w(n));
-    }, M = (n) => {
-        if (!P(n) || !d.value)
+        (i == null ? void 0 : i(O, n)) !== !1 && (_.value = O, w(n));
+    }, L = (n) => {
+        if (!P(n) || !_.value)
             return;
         let {
             x: m,
             y: O
-        } = u.value;
-        (s === "x" || s === "both") && (m = n.clientX - d.value.x), (s === "y" || s === "both") && (O = n.clientY - d.value.y), u.value = {
+        } = c.value;
+        (s === "x" || s === "both") && (m = n.clientX - _.value.x), (s === "y" || s === "both") && (O = n.clientY - _.value.y), c.value = {
             x: m,
             y: O
-        }, l == null || l(u.value, n), w(n);
-    }, U = (n) => {
-        P(n) && d.value && (d.value = void 0, f == null || f(u.value, n), w(n));
+        }, u == null || u(c.value, n), w(n);
+    }, M = (n) => {
+        P(n) && _.value && (_.value = void 0, y == null || y(c.value, n), w(n));
     };
     if (I) {
         const n = {
-            capture: (o = r.capture) != null ? o : !0
+            capture: (o = t.capture) != null ? o : !0
         };
-        $(V, "pointerdown", L, n), $(v, "pointermove", M, n), $(v, "pointerup", U, n);
+        $(C, "pointerdown", V, n), $(g, "pointermove", L, n), $(g, "pointerup", M, n);
     }
-    return se(ie({}, R(u)), {
-        position: u,
-        isDragging: x(() => !!d.value),
-        style: x(
-            () => `left:${u.value.x}px;top:${u.value.y}px;`
+    return se(ie({}, R(c)), {
+        position: c,
+        isDragging: D(() => !!_.value),
+        style: D(
+            () => `left:${c.value.x}px;top:${c.value.y}px;`
         )
     });
 }
-const pe = /* @__PURE__ */ H({
+const pe = /* @__PURE__ */ Y({
     __name: "UseDraggable",
     props: {
         elementId: null,
         options: null
     },
     emits: ["update", "isDraggingUpdate"],
     setup(e, {
-        emit: r
+        emit: t
     }) {
-        const t = e;
-        return q(() => {
-            const o = document.getElementById(`c${t.elementId}`),
-                {
-                    x: a,
-                    y: c,
-                    style: g,
-                    isDragging: _
-                } = le(o, t.options);
-            h([a, c, g], ([l, f, i]) => {
-                r("update", {
-                    x: l,
-                    y: f,
-                    style: i
+        const r = e;
+        return H(() => {
+            const o = document.getElementById(`c${r.elementId}`);
+
+            function a() {
+                t("update", {
+                    x: l.value,
+                    y: d.value,
+                    style: u.value,
+                    isFirst: !0,
+                    isFinal: !1
+                });
+            }
+
+            function v() {
+                t("update", {
+                    x: l.value,
+                    y: d.value,
+                    style: u.value,
+                    isFirst: !1,
+                    isFinal: !0
+                });
+            }
+            const {
+                x: l,
+                y: d,
+                style: u,
+                isDragging: y
+            } = le(o, {
+                onStart: a,
+                onEnd: v,
+                ...r.options
+            });
+            h([l, d, u], ([i, p, s]) => {
+                t("update", {
+                    x: i,
+                    y: p,
+                    style: s,
+                    isFirst: !1,
+                    isFinal: !1
                 });
-            }), h(_, (l) => {
-                r("isDraggingUpdate", {
-                    isDragging: l
+            }), h(y, (i) => {
+                t("isDraggingUpdate", {
+                    isDragging: i
                 });
             });
         }), (o, a) => null;
     }
 });
 export {
     pe as
```

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 from signe import createSignal, effect, batch
 from ex4nicegui.utils.signals import ref_from_signal
 
 _Update_Args = [
     "x",
     "y",
     "style",
+    "isFirst",
+    "isFinal",
 ]
 
 
 @dataclass(**KWONLY_SLOTS)
 class UseDraggableUpdateEventArguments(EventArguments):
     x: float
     y: float
     style: str
+    isFirst: bool
+    isFinal: bool
 
 
 def use_draggable(element: Element, init_x=0.0, init_y=0.0, auto_bind_style=True):
     ud = UseDraggable(element, init_x, init_y)
     if auto_bind_style:
         element.style(add=f"position:fixed;left:{init_x}px;top:{init_y}px")
         ud.bind_style(element)
@@ -36,20 +40,25 @@
         self._props["options"] = {"initialValue": {"x": init_x, "y": init_y}}
 
         self.__style_getter, self.__style_setter = createSignal("")
         self.__x_getter, self.__x_setter = createSignal(init_x)
         self.__y_getter, self.__y_setter = createSignal(init_y)
         self.__isDragging_getter, self.__isDragging_setter = createSignal(False)
 
+        self.__isFirst_getter, self.__isFirst_setter = createSignal(True)
+        self.__isFinal_getter, self.__isFinal_setter = createSignal(False)
+
         def update(args: UseDraggableUpdateEventArguments):
             @batch
             def _():
                 self.__style_setter(args.style)
                 self.__x_setter(args.x)
                 self.__y_setter(args.y)
+                self.__isFirst_setter(args.isFirst)
+                self.__isFinal_setter(args.isFinal)
 
         self.on_update(update)
 
         def on_isDraggingUpdate(e):
             self.__isDragging_setter(e.args["isDragging"])
             # print(args['args']['isDragging'])
 
@@ -67,14 +76,22 @@
     def style(self):
         return ref_from_signal(self.__style_getter)
 
     @property
     def is_dragging(self):
         return ref_from_signal(self.__isDragging_getter)
 
+    @property
+    def isFirst(self):
+        return ref_from_signal(self.__isFirst_getter)
+
+    @property
+    def isFinal(self):
+        return ref_from_signal(self.__isFinal_getter)
+
     def bind_style(self, element: Element):
         @effect
         def _():
             element.style(self.__style_getter())
             element.update()
 
     def on_update(self, handler: Optional[Callable[..., Any]]):
@@ -84,11 +101,13 @@
                 handler,
                 UseDraggableUpdateEventArguments(
                     sender=self,
                     client=self.client,
                     x=args["x"],
                     y=args["y"],
                     style=args["style"],
+                    isFirst=args["isFirst"],
+                    isFinal=args["isFinal"],
                 ),
             )
 
         self.on("update", inner_handler, args=_Update_Args)
```

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/__init__.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,7 +31,10 @@
     TextareaBindableUi as textarea,
     LazyTextareaBindableUi as lazy_textarea,
 )
 from .upload import (
     UploadBindableUi as upload,
     UploadResult,
 )
+from .column import ColumnBindableUi as column
+from .number import NumberBindableUi as number
+from .grid import GridBindableUi as grid
```

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/aggrid.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/base.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from typing_extensions import Self
 from signe import effect
 from ex4nicegui.utils.signals import (
     ReadonlyRef,
     Ref,
     to_ref,
+    ref_computed,
     _TMaybeRef as TMaybeRef,
 )
 from nicegui import Tailwind, ui
 from nicegui.elements.mixins.color_elements import (
     TextColorElement,
     QUASAR_COLORS,
     TAILWIND_COLORS,
@@ -29,14 +30,15 @@
 
 TWidget = TypeVar("TWidget")
 
 
 class BindableUi(Generic[TWidget]):
     def __init__(self, element: TWidget) -> None:
         self.__element = element
+        self.tailwind = Tailwind(cast(ui.element, self.__element))
 
     def props(self, add: Optional[str] = None, *, remove: Optional[str] = None):
         cast(ui.element, self.element).props(add, remove=remove)
         return self
 
     def classes(
         self,
@@ -54,26 +56,14 @@
         *,
         remove: Optional[str] = None,
         replace: Optional[str] = None,
     ):
         cast(ui.element, self.element).style(add, remove=remove, replace=replace)
         return self
 
-    @overload
-    def tailwind(self, *tailwind: Tailwind) -> Self:
-        ...
-
-    @overload
-    def tailwind(self, *classes: str) -> Self:
-        ...
-
-    def tailwind(self, *args):
-        cast(ui.element, self.element).tailwind(*args)
-        return self
-
     def tooltip(self, text: str) -> Self:
         cast(ui.element, self.element).tooltip(text)
         return self
 
     def add_slot(self, name: str, template: Optional[str] = None):
         """Add a slot to the element.
 
@@ -103,14 +93,17 @@
         @effect
         def _():
             element = cast(ui.element, self.element)
             element.set_visibility(ref_ui.value)
 
         return self
 
+    def bind_not_visible(self, ref_ui: ReadonlyRef[bool]):
+        return self.bind_visible(ref_computed(lambda: not ref_ui.value))
+
     def on(
         self,
         type: str,
         handler: Optional[Callable[..., Any]] = None,
         args: Optional[List[str]] = None,
         *,
         throttle: float = 0.0,
```

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/button.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/button.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/card.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/card.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/checkbox.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/checkbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/color_picker.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/color_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/date.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/date.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/drawer.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/echarts.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/echarts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/html.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/html.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/icon.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/icon.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/image.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/image.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/input.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/input.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/label.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/label.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/radio.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/select.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/select.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/slider.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/switch.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/switch.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/table.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/textarea.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/textarea.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/officials/upload.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/upload.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.2.6/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/tools/debug.py` & `ex4nicegui-0.2.6/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui/utils/signals.py` & `ex4nicegui-0.2.6/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.5/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.2.6/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,33 @@
 ex4nicegui/reactive/usePagination.py
 ex4nicegui/reactive/ECharts/ECharts.js
 ex4nicegui/reactive/ECharts/ECharts.py
 ex4nicegui/reactive/ECharts/__init__.py
 ex4nicegui/reactive/UseDraggable/UseDraggable.js
 ex4nicegui/reactive/UseDraggable/UseDraggable.py
 ex4nicegui/reactive/UseDraggable/__init__.py
+ex4nicegui/reactive/dropZone/dropZone.js
 ex4nicegui/reactive/officials/__init__.py
 ex4nicegui/reactive/officials/aggrid.py
 ex4nicegui/reactive/officials/base.py
 ex4nicegui/reactive/officials/button.py
 ex4nicegui/reactive/officials/card.py
 ex4nicegui/reactive/officials/checkbox.py
 ex4nicegui/reactive/officials/color_picker.py
+ex4nicegui/reactive/officials/column.py
 ex4nicegui/reactive/officials/date.py
 ex4nicegui/reactive/officials/drawer.py
 ex4nicegui/reactive/officials/echarts.py
+ex4nicegui/reactive/officials/grid.py
 ex4nicegui/reactive/officials/html.py
 ex4nicegui/reactive/officials/icon.py
 ex4nicegui/reactive/officials/image.py
 ex4nicegui/reactive/officials/input.py
 ex4nicegui/reactive/officials/label.py
+ex4nicegui/reactive/officials/number.py
 ex4nicegui/reactive/officials/radio.py
 ex4nicegui/reactive/officials/row.py
 ex4nicegui/reactive/officials/select.py
 ex4nicegui/reactive/officials/slider.py
 ex4nicegui/reactive/officials/switch.py
 ex4nicegui/reactive/officials/table.py
 ex4nicegui/reactive/officials/textarea.py
```

### Comparing `ex4nicegui-0.2.5/setup.py` & `ex4nicegui-0.2.6/setup.py`

 * *Files identical despite different names*

