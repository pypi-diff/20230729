# Comparing `tmp/svgdiagram-1.4.4.tar.gz` & `tmp/svgdiagram-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgdiagram-1.4.4.tar", last modified: Mon Mar  6 15:12:24 2023, max compression
+gzip compressed data, was "svgdiagram-1.5.0.tar", last modified: Sat Jul 29 14:46:08 2023, max compression
```

## Comparing `svgdiagram-1.4.4.tar` & `svgdiagram-1.5.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.590009 svgdiagram-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-06 15:12:24.590009 svgdiagram-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 15:12:24.590009 svgdiagram-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.582008 svgdiagram-1.4.4/svgdiagram/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.582008 svgdiagram-1.4.4/svgdiagram/derived_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/derived_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/derived_elements/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/derived_elements/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.582008 svgdiagram-1.4.4/svgdiagram/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.586008 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/gantt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/gantt_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/gantt_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/milestone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.586008 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/renderer/swimlane.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/swimlane.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/gantt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.586008 svgdiagram-1.4.4/svgdiagram/diagrams/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/network/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/network/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/diagrams/network/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.586008 svgdiagram-1.4.4/svgdiagram/elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/svg_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/elements/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.590009 svgdiagram-1.4.4/svgdiagram/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/circular_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/diamond_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/shapes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.590009 svgdiagram-1.4.4/svgdiagram/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/wrappers/wrap_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/svgdiagram/wrappers/wrap_rect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.582008 svgdiagram-1.4.4/svgdiagram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-06 15:12:24.000000 svgdiagram-1.4.4/svgdiagram.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:12:24.590009 svgdiagram-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/tests/test_custom_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-06 15:12:13.000000 svgdiagram-1.4.4/tests/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram/derived_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/derived_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/derived_elements/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/derived_elements/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/gantt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/gantt_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/gantt_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/milestone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/renderer/swimlane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/swimlane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/gantt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram/diagrams/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/network/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/diagrams/network/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/svgdiagram/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/svg_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/elements/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/svgdiagram/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/circular_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/diamond_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/shapes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/svgdiagram/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/wrappers/wrap_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/svgdiagram/wrappers/wrap_rect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.263730 svgdiagram-1.5.0/svgdiagram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 14:46:08.000000 svgdiagram-1.5.0/svgdiagram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:46:08.267731 svgdiagram-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/tests/test_custom_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-29 14:45:58.000000 svgdiagram-1.5.0/tests/test_readme.py
```

### Comparing `svgdiagram-1.4.4/LICENSE` & `svgdiagram-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/PKG-INFO` & `svgdiagram-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgdiagram
-Version: 1.4.4
+Version: 1.5.0
 Summary: Create SVG diagrams with python
 Home-page: https://github.com/MatthiasRieck/svgdiagram
 Author: Matthias Rieck
 Author-email: Matthias.Rieck@tum.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `svgdiagram-1.4.4/README.md` & `svgdiagram-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/setup.py` & `svgdiagram-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/derived_elements/task.py` & `svgdiagram-1.5.0/svgdiagram/derived_elements/task.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/gantt/gantt.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/gantt/gantt.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/gantt/gantt_content.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/gantt/gantt_content.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import List, Optional, Union
 from datetime import date
 from .swimlane import Swimlane, CalendarSwimlane
 from .dependency import Dependency
 
 
 class GanttContent(BaseModel):
-    start_date: Optional[date]
-    end_date: Optional[date]
+    start_date: Optional[date] = None
+    end_date: Optional[date] = None
     swimlanes: List[Union[
         CalendarSwimlane, Swimlane,
     ]] = Field(default_factory=list)
     dependencies: List[Dependency] = Field(default_factory=list)
 
     def iter_all_swimlane_dates(self):
         for swimlane in self.swimlanes:
@@ -22,11 +22,11 @@
                 yield milestone.due_date
             for task in swimlane.tasks:
                 yield task.start_date
                 yield task.end_date
 
 
 class GanttGroup(BaseModel):
-    group_id: Optional[str]
-    swimlane_order: Optional[List[str]]
+    group_id: Optional[str] = None
+    swimlane_order: List[str] = Field(default_factory=list)
     swimlanes: List[Swimlane] = Field(default_factory=list)
     dependencies: List[Dependency] = Field(default_factory=list)
```

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/gantt/loader.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/gantt/loader.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/gantt/renderer/swimlane.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/gantt/renderer/swimlane.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/gantt/swimlane.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/gantt/swimlane.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/gantt/task.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/gantt/task.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/network/link.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/network/link.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/network/network.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/network/network.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/diagrams/network/node.py` & `svgdiagram-1.5.0/svgdiagram/diagrams/network/node.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/circle.py` & `svgdiagram-1.5.0/svgdiagram/elements/circle.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/group.py` & `svgdiagram-1.5.0/svgdiagram/elements/group.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/marker.py` & `svgdiagram-1.5.0/svgdiagram/elements/marker.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/multi_line_text.py` & `svgdiagram-1.5.0/svgdiagram/elements/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/path.py` & `svgdiagram-1.5.0/svgdiagram/elements/path.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/rect.py` & `svgdiagram-1.5.0/svgdiagram/elements/rect.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/svg.py` & `svgdiagram-1.5.0/svgdiagram/elements/svg.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/svg_element.py` & `svgdiagram-1.5.0/svgdiagram/elements/svg_element.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/elements/text.py` & `svgdiagram-1.5.0/svgdiagram/elements/text.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/shapes/circular_shape.py` & `svgdiagram-1.5.0/svgdiagram/shapes/circular_shape.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/shapes/connection.py` & `svgdiagram-1.5.0/svgdiagram/shapes/connection.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/shapes/diamond_shape.py` & `svgdiagram-1.5.0/svgdiagram/shapes/diamond_shape.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/shapes/shape.py` & `svgdiagram-1.5.0/svgdiagram/shapes/shape.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/wrappers/wrap_circle.py` & `svgdiagram-1.5.0/svgdiagram/wrappers/wrap_circle.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram/wrappers/wrap_rect.py` & `svgdiagram-1.5.0/svgdiagram/wrappers/wrap_rect.py`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/svgdiagram.egg-info/PKG-INFO` & `svgdiagram-1.5.0/svgdiagram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgdiagram
-Version: 1.4.4
+Version: 1.5.0
 Summary: Create SVG diagrams with python
 Home-page: https://github.com/MatthiasRieck/svgdiagram
 Author: Matthias Rieck
 Author-email: Matthias.Rieck@tum.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `svgdiagram-1.4.4/svgdiagram.egg-info/SOURCES.txt` & `svgdiagram-1.5.0/svgdiagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svgdiagram-1.4.4/tests/test_readme.py` & `svgdiagram-1.5.0/tests/test_readme.py`

 * *Files identical despite different names*

