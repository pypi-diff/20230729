# Comparing `tmp/poetry_polylith_plugin-1.6.2.tar.gz` & `tmp/poetry_polylith_plugin-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_polylith_plugin-1.6.2.tar", max compression
+gzip compressed data, was "poetry_polylith_plugin-1.7.0.tar", max compression
```

## Comparing `poetry_polylith_plugin-1.6.2.tar` & `poetry_polylith_plugin-1.7.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     1475 2023-04-01 08:55:53.793699 poetry_polylith_plugin-1.6.2/README.md
--rw-r--r--   0        0        0      244 2022-11-22 16:34:48.997679 poetry_polylith_plugin-1.6.2/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      555 2023-03-13 14:27:27.458090 poetry_polylith_plugin-1.6.2/polylith/bricks/base.py
--rw-r--r--   0        0        0     1045 2023-03-13 14:27:27.458215 poetry_polylith_plugin-1.6.2/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1096 2023-03-14 14:29:50.224158 poetry_polylith_plugin-1.6.2/polylith/bricks/component.py
--rw-r--r--   0        0        0       56 2023-03-13 14:27:27.458433 poetry_polylith_plugin-1.6.2/polylith/check/__init__.py
--rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 poetry_polylith_plugin-1.6.2/polylith/check/grouping.py
--rw-r--r--   0        0        0     1756 2023-04-23 13:53:29.379020 poetry_polylith_plugin-1.6.2/polylith/check/report.py
--rw-r--r--   0        0        0       98 2022-11-04 07:17:35.622947 poetry_polylith_plugin-1.6.2/polylith/development/__init__.py
--rw-r--r--   0        0        0      211 2022-11-22 16:34:48.998071 poetry_polylith_plugin-1.6.2/polylith/development/development.py
--rw-r--r--   0        0        0       75 2022-11-22 16:34:48.998183 poetry_polylith_plugin-1.6.2/polylith/diff/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-05 14:32:20.927245 poetry_polylith_plugin-1.6.2/polylith/diff/collect.py
--rw-r--r--   0        0        0     2670 2023-04-23 13:53:29.379615 poetry_polylith_plugin-1.6.2/polylith/diff/report.py
--rw-r--r--   0        0        0       68 2022-11-04 07:17:35.623197 poetry_polylith_plugin-1.6.2/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      273 2022-11-22 16:34:48.998517 poetry_polylith_plugin-1.6.2/polylith/dirs/dirs.py
--rw-r--r--   0        0        0       72 2022-11-04 07:17:35.623423 poetry_polylith_plugin-1.6.2/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 poetry_polylith_plugin-1.6.2/polylith/files/files.py
--rw-r--r--   0        0        0      151 2023-04-23 13:53:29.379732 poetry_polylith_plugin-1.6.2/polylith/imports/__init__.py
--rw-r--r--   0        0        0     1687 2023-04-23 13:53:29.379831 poetry_polylith_plugin-1.6.2/polylith/imports/parser.py
--rw-r--r--   0        0        0      426 2023-04-01 08:55:53.790585 poetry_polylith_plugin-1.6.2/polylith/info/__init__.py
--rw-r--r--   0        0        0     1692 2023-04-01 08:55:53.790905 poetry_polylith_plugin-1.6.2/polylith/info/collect.py
--rw-r--r--   0        0        0     2216 2023-04-23 13:53:29.380456 poetry_polylith_plugin-1.6.2/polylith/info/report.py
--rw-r--r--   0        0        0       91 2022-11-04 07:17:35.623663 poetry_polylith_plugin-1.6.2/polylith/interface/__init__.py
--rw-r--r--   0        0        0      876 2023-03-13 14:27:27.458927 poetry_polylith_plugin-1.6.2/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      201 2023-04-23 13:53:29.380600 poetry_polylith_plugin-1.6.2/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-23 13:53:29.380732 poetry_polylith_plugin-1.6.2/polylith/libs/grouping.py
--rw-r--r--   0        0        0     3677 2023-04-23 13:53:29.380856 poetry_polylith_plugin-1.6.2/polylith/libs/report.py
--rw-r--r--   0        0        0     4156 2023-04-23 13:53:29.381083 poetry_polylith_plugin-1.6.2/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      790 2023-04-23 13:53:29.381323 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/__init__.py
--rw-r--r--   0        0        0     2188 2023-04-01 08:55:53.792059 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/check.py
--rw-r--r--   0        0        0      552 2023-03-13 14:27:27.461635 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create.py
--rw-r--r--   0        0        0      634 2023-03-13 14:27:27.461785 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_base.py
--rw-r--r--   0        0        0      674 2023-03-13 14:27:27.461919 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_component.py
--rw-r--r--   0        0        0      680 2023-03-13 14:27:27.462039 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_project.py
--rw-r--r--   0        0        0      949 2022-11-22 16:34:48.999505 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_workspace.py
--rw-r--r--   0        0        0     1744 2023-04-05 14:32:20.927796 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/diff.py
--rw-r--r--   0        0        0      876 2022-11-22 16:34:48.999675 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/info.py
--rw-r--r--   0        0        0     2328 2023-04-01 08:55:53.792609 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/libs.py
--rw-r--r--   0        0        0     1676 2023-04-25 16:19:39.164291 poetry_polylith_plugin-1.6.2/polylith/poetry/commands/sync.py
--rw-r--r--   0        0        0       87 2022-11-04 07:17:35.621247 poetry_polylith_plugin-1.6.2/polylith/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      959 2023-04-23 13:53:29.378523 poetry_polylith_plugin-1.6.2/polylith/poetry_plugin/plugin.py
--rw-r--r--   0        0        0      331 2023-04-23 13:53:29.381659 poetry_polylith_plugin-1.6.2/polylith/project/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-05 14:32:20.927943 poetry_polylith_plugin-1.6.2/polylith/project/create.py
--rw-r--r--   0        0        0     1433 2023-04-23 13:53:29.381846 poetry_polylith_plugin-1.6.2/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 poetry_polylith_plugin-1.6.2/polylith/project/parser.py
--rw-r--r--   0        0        0      142 2023-03-13 14:27:27.462643 poetry_polylith_plugin-1.6.2/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-05 14:32:20.928603 poetry_polylith_plugin-1.6.2/polylith/readme/readme.py
--rw-r--r--   0        0        0      374 2022-11-22 16:34:49.000462 poetry_polylith_plugin-1.6.2/polylith/repo/__init__.py
--rw-r--r--   0        0        0      985 2022-11-22 16:34:49.000581 poetry_polylith_plugin-1.6.2/polylith/repo/repo.py
--rw-r--r--   0        0        0       58 2023-04-23 13:53:29.381960 poetry_polylith_plugin-1.6.2/polylith/reporting/__init__.py
--rw-r--r--   0        0        0      172 2023-04-23 13:53:29.382046 poetry_polylith_plugin-1.6.2/polylith/reporting/theme.py
--rw-r--r--   0        0        0      188 2023-04-23 13:53:29.382161 poetry_polylith_plugin-1.6.2/polylith/sync/__init__.py
--rw-r--r--   0        0        0     2968 2023-05-22 11:03:54.994596 poetry_polylith_plugin-1.6.2/polylith/sync/collect.py
--rw-r--r--   0        0        0      794 2023-04-23 13:53:29.382340 poetry_polylith_plugin-1.6.2/polylith/sync/report.py
--rw-r--r--   0        0        0     1787 2023-04-23 13:53:29.382434 poetry_polylith_plugin-1.6.2/polylith/sync/update.py
--rw-r--r--   0        0        0       71 2022-11-04 07:17:35.625873 poetry_polylith_plugin-1.6.2/polylith/test/__init__.py
--rw-r--r--   0        0        0      859 2022-11-22 16:34:49.000744 poetry_polylith_plugin-1.6.2/polylith/test/tests.py
--rw-r--r--   0        0        0       94 2023-03-13 14:27:27.463180 poetry_polylith_plugin-1.6.2/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1089 2023-03-13 14:27:27.463863 poetry_polylith_plugin-1.6.2/polylith/workspace/create.py
--rw-r--r--   0        0        0     1832 2023-05-22 11:03:54.995273 poetry_polylith_plugin-1.6.2/polylith/workspace/parser.py
--rw-r--r--   0        0        0      949 2023-03-13 14:27:27.464047 poetry_polylith_plugin-1.6.2/polylith/workspace/paths.py
--rw-r--r--   0        0        0      781 2023-07-23 11:17:37.358176 poetry_polylith_plugin-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-04-01 08:55:53.793699 poetry_polylith_plugin-1.7.0/README.md
+-rw-r--r--   0        0        0      244 2022-11-22 16:34:48.997679 poetry_polylith_plugin-1.7.0/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      555 2023-03-13 14:27:27.458090 poetry_polylith_plugin-1.7.0/polylith/bricks/base.py
+-rw-r--r--   0        0        0     1045 2023-03-13 14:27:27.458215 poetry_polylith_plugin-1.7.0/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1096 2023-03-14 14:29:50.224158 poetry_polylith_plugin-1.7.0/polylith/bricks/component.py
+-rw-r--r--   0        0        0       98 2023-07-29 11:51:13.391379 poetry_polylith_plugin-1.7.0/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-29 11:51:13.391711 poetry_polylith_plugin-1.7.0/polylith/check/collect.py
+-rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 poetry_polylith_plugin-1.7.0/polylith/check/grouping.py
+-rw-r--r--   0        0        0     2516 2023-07-29 11:51:13.391873 poetry_polylith_plugin-1.7.0/polylith/check/report.py
+-rw-r--r--   0        0        0       98 2022-11-04 07:17:35.622947 poetry_polylith_plugin-1.7.0/polylith/development/__init__.py
+-rw-r--r--   0        0        0      211 2022-11-22 16:34:48.998071 poetry_polylith_plugin-1.7.0/polylith/development/development.py
+-rw-r--r--   0        0        0       75 2022-11-22 16:34:48.998183 poetry_polylith_plugin-1.7.0/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-05 14:32:20.927245 poetry_polylith_plugin-1.7.0/polylith/diff/collect.py
+-rw-r--r--   0        0        0     2670 2023-04-23 13:53:29.379615 poetry_polylith_plugin-1.7.0/polylith/diff/report.py
+-rw-r--r--   0        0        0       68 2022-11-04 07:17:35.623197 poetry_polylith_plugin-1.7.0/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      273 2022-11-22 16:34:48.998517 poetry_polylith_plugin-1.7.0/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0       72 2022-11-04 07:17:35.623423 poetry_polylith_plugin-1.7.0/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 poetry_polylith_plugin-1.7.0/polylith/files/files.py
+-rw-r--r--   0        0        0      151 2023-04-23 13:53:29.379732 poetry_polylith_plugin-1.7.0/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-29 11:51:13.392045 poetry_polylith_plugin-1.7.0/polylith/imports/parser.py
+-rw-r--r--   0        0        0      426 2023-04-01 08:55:53.790585 poetry_polylith_plugin-1.7.0/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1692 2023-04-01 08:55:53.790905 poetry_polylith_plugin-1.7.0/polylith/info/collect.py
+-rw-r--r--   0        0        0     2216 2023-04-23 13:53:29.380456 poetry_polylith_plugin-1.7.0/polylith/info/report.py
+-rw-r--r--   0        0        0       91 2022-11-04 07:17:35.623663 poetry_polylith_plugin-1.7.0/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      876 2023-03-13 14:27:27.458927 poetry_polylith_plugin-1.7.0/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      201 2023-04-23 13:53:29.380600 poetry_polylith_plugin-1.7.0/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-23 13:53:29.380732 poetry_polylith_plugin-1.7.0/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     3677 2023-07-28 17:52:12.877081 poetry_polylith_plugin-1.7.0/polylith/libs/report.py
+-rw-r--r--   0        0        0     4156 2023-04-23 13:53:29.381083 poetry_polylith_plugin-1.7.0/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      790 2023-04-23 13:53:29.381323 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/__init__.py
+-rw-r--r--   0        0        0     2532 2023-07-29 11:51:13.392333 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/check.py
+-rw-r--r--   0        0        0      552 2023-03-13 14:27:27.461635 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create.py
+-rw-r--r--   0        0        0      634 2023-03-13 14:27:27.461785 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_base.py
+-rw-r--r--   0        0        0      674 2023-03-13 14:27:27.461919 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_component.py
+-rw-r--r--   0        0        0      680 2023-03-13 14:27:27.462039 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_project.py
+-rw-r--r--   0        0        0      949 2022-11-22 16:34:48.999505 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_workspace.py
+-rw-r--r--   0        0        0     1744 2023-04-05 14:32:20.927796 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/diff.py
+-rw-r--r--   0        0        0      876 2022-11-22 16:34:48.999675 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/info.py
+-rw-r--r--   0        0        0     2328 2023-04-01 08:55:53.792609 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/libs.py
+-rw-r--r--   0        0        0     1803 2023-07-29 11:51:13.392698 poetry_polylith_plugin-1.7.0/polylith/poetry/commands/sync.py
+-rw-r--r--   0        0        0       87 2022-11-04 07:17:35.621247 poetry_polylith_plugin-1.7.0/polylith/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-23 13:53:29.378523 poetry_polylith_plugin-1.7.0/polylith/poetry_plugin/plugin.py
+-rw-r--r--   0        0        0      331 2023-04-23 13:53:29.381659 poetry_polylith_plugin-1.7.0/polylith/project/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-05 14:32:20.927943 poetry_polylith_plugin-1.7.0/polylith/project/create.py
+-rw-r--r--   0        0        0     1433 2023-04-23 13:53:29.381846 poetry_polylith_plugin-1.7.0/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 poetry_polylith_plugin-1.7.0/polylith/project/parser.py
+-rw-r--r--   0        0        0      142 2023-03-13 14:27:27.462643 poetry_polylith_plugin-1.7.0/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1067 2023-04-05 14:32:20.928603 poetry_polylith_plugin-1.7.0/polylith/readme/readme.py
+-rw-r--r--   0        0        0      374 2022-11-22 16:34:49.000462 poetry_polylith_plugin-1.7.0/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      985 2022-11-22 16:34:49.000581 poetry_polylith_plugin-1.7.0/polylith/repo/repo.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:53:29.381960 poetry_polylith_plugin-1.7.0/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-27 12:41:39.939902 poetry_polylith_plugin-1.7.0/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      188 2023-04-23 13:53:29.382161 poetry_polylith_plugin-1.7.0/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-29 11:51:13.393013 poetry_polylith_plugin-1.7.0/polylith/sync/collect.py
+-rw-r--r--   0        0        0      971 2023-07-29 11:51:13.393395 poetry_polylith_plugin-1.7.0/polylith/sync/report.py
+-rw-r--r--   0        0        0     1787 2023-04-23 13:53:29.382434 poetry_polylith_plugin-1.7.0/polylith/sync/update.py
+-rw-r--r--   0        0        0       71 2022-11-04 07:17:35.625873 poetry_polylith_plugin-1.7.0/polylith/test/__init__.py
+-rw-r--r--   0        0        0      859 2022-11-22 16:34:49.000744 poetry_polylith_plugin-1.7.0/polylith/test/tests.py
+-rw-r--r--   0        0        0       94 2023-03-13 14:27:27.463180 poetry_polylith_plugin-1.7.0/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1089 2023-03-13 14:27:27.463863 poetry_polylith_plugin-1.7.0/polylith/workspace/create.py
+-rw-r--r--   0        0        0     1832 2023-05-22 11:03:54.995273 poetry_polylith_plugin-1.7.0/polylith/workspace/parser.py
+-rw-r--r--   0        0        0      949 2023-03-13 14:27:27.464047 poetry_polylith_plugin-1.7.0/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      781 2023-07-29 11:51:28.912495 poetry_polylith_plugin-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.7.0/PKG-INFO
```

### Comparing `poetry_polylith_plugin-1.6.2/README.md` & `poetry_polylith_plugin-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/bricks/base.py` & `poetry_polylith_plugin-1.7.0/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/bricks/brick.py` & `poetry_polylith_plugin-1.7.0/polylith/bricks/brick.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/bricks/component.py` & `poetry_polylith_plugin-1.7.0/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/check/grouping.py` & `poetry_polylith_plugin-1.7.0/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/check/report.py` & `poetry_polylith_plugin-1.7.0/polylith/sync/collect.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 from pathlib import Path
-from typing import Set
 
-from polylith import imports, libs, workspace
-from polylith.check import grouping
-from polylith.reporting import theme
-from rich.console import Console
+from polylith import check, info, workspace
 
 
-def print_missing_deps(brick_imports: dict, deps: Set[str], project_name: str) -> bool:
-    diff = libs.report.calculate_diff(brick_imports, deps)
-
-    if not diff:
-        return True
-
-    console = Console(theme=theme.poly_theme)
-
-    missing = ", ".join(sorted(diff))
-
-    console.print(f":thinking_face: Cannot locate {missing} in {project_name}")
-    return False
-
-
-def print_report(
-    root: Path, ns: str, project_data: dict, third_party_libs: Set
-) -> bool:
-    name = project_data["name"]
-
+def get_brick_imports(root: Path, ns: str, project_data: dict) -> dict:
     bases = {b for b in project_data.get("bases", [])}
     components = {c for c in project_data.get("components", [])}
 
     bases_paths = workspace.paths.collect_bases_paths(root, ns, bases)
     components_paths = workspace.paths.collect_components_paths(root, ns, components)
 
-    all_imports_in_bases = imports.fetch_all_imports(bases_paths)
-    all_imports_in_components = imports.fetch_all_imports(components_paths)
-
-    brick_imports = {
-        "bases": grouping.extract_brick_imports(all_imports_in_bases, ns),
-        "components": grouping.extract_brick_imports(all_imports_in_components, ns),
-    }
+    brick_imports_in_bases = check.collect.extract_bricks(bases_paths, ns)
+    brick_imports_in_components = check.collect.extract_bricks(components_paths, ns)
 
-    third_party_imports = {
-        "bases": libs.extract_third_party_imports(all_imports_in_bases, ns),
-        "components": libs.extract_third_party_imports(all_imports_in_components, ns),
+    return {
+        "bases": check.collect.with_unknown_components(
+            root, ns, brick_imports_in_bases
+        ),
+        "components": check.collect.with_unknown_components(
+            root, ns, brick_imports_in_components
+        ),
     }
 
-    packages = set().union(bases, components)
 
-    brick_result = print_missing_deps(brick_imports, packages, name)
-    libs_result = print_missing_deps(third_party_imports, third_party_libs, name)
-
-    return all([brick_result, libs_result])
+def calculate_diff(
+    root: Path,
+    namespace: str,
+    project_data: dict,
+    workspace_data: dict,
+) -> dict:
+    brick_imports = get_brick_imports(root, namespace, project_data)
+
+    all_bases = workspace_data["bases"]
+    all_components = workspace_data["components"]
+
+    bases = project_data["bases"]
+    components = project_data["components"]
+
+    is_project = info.is_project(project_data)
+
+    if is_project:
+        brick_diff = check.collect.imports_diff(brick_imports, bases, components)
+    else:
+        all_bricks = set().union(all_bases, all_components)
+        brick_diff = check.collect.diff(all_bricks, bases, components)
+
+    bases_diff = {b for b in brick_diff if b in all_bases}
+    components_diff = {b for b in brick_diff if b in all_components}
+
+    return {
+        "name": project_data["name"],
+        "path": project_data["path"],
+        "is_project": is_project,
+        "bases": bases_diff,
+        "components": components_diff,
+        "brick_imports": brick_imports,
+    }
```

### Comparing `poetry_polylith_plugin-1.6.2/polylith/diff/collect.py` & `poetry_polylith_plugin-1.7.0/polylith/diff/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/diff/report.py` & `poetry_polylith_plugin-1.7.0/polylith/diff/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/imports/parser.py` & `poetry_polylith_plugin-1.7.0/polylith/imports/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+from functools import lru_cache
 from pathlib import Path
 from typing import List, Set
 
 
 def parse_import(node: ast.Import) -> List[str]:
     return [name.name for name in node.names]
 
@@ -25,14 +26,15 @@
 
     if isinstance(node, ast.ImportFrom):
         return parse_import_from(node)
 
     return []
 
 
+@lru_cache
 def parse_module(path: Path) -> ast.AST:
     with open(path.as_posix(), "r", encoding="utf-8", errors="ignore") as f:
         tree = ast.parse(f.read(), path.name)
 
     return tree
```

### Comparing `poetry_polylith_plugin-1.6.2/polylith/info/collect.py` & `poetry_polylith_plugin-1.7.0/polylith/info/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/info/report.py` & `poetry_polylith_plugin-1.7.0/polylith/info/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/interface/interfaces.py` & `poetry_polylith_plugin-1.7.0/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/libs/grouping.py` & `poetry_polylith_plugin-1.7.0/polylith/libs/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/libs/report.py` & `poetry_polylith_plugin-1.7.0/polylith/libs/report.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/libs/stdlib.py` & `poetry_polylith_plugin-1.7.0/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/__init__.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/check.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/libs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 from pathlib import Path
 from typing import Set, Union
 
 from poetry.console.commands.command import Command
 from poetry.factory import Factory
-from polylith import check, info, project, repo, workspace
+from polylith import info, project, repo, workspace
+from polylith.libs import report
 
 
-class CheckCommand(Command):
-    name = "poly check"
-    description = "Validates the <comment>Polylith</> workspace."
+class LibsCommand(Command):
+    name = "poly libs"
+    description = "Show third-party libraries used in the workspace."
 
     def find_third_party_libs(self, path: Union[Path, None]) -> Set:
         project_poetry = Factory().create_poetry(path) if path else self.poetry
 
         if not project_poetry.locker.is_locked():
             raise ValueError("poetry.lock not found. Run `poetry lock` to create it.")
 
         packages = project_poetry.locker.locked_repository().packages
 
         return {p.name for p in packages}
 
-    def print_report(self, root: Path, ns: str, project_data: dict) -> bool:
-        path = project_data["path"]
-        name = project_data["name"]
+    def print_report(self, root: Path, ns: str, data: dict) -> bool:
+        name = data["name"]
+        path = data["path"]
+
+        brick_imports = report.get_third_party_imports(root, ns, data)
+
+        report.print_libs_summary(brick_imports, data)
+        report.print_libs_in_bricks(brick_imports)
 
         try:
             third_party_libs = self.find_third_party_libs(path)
-            return check.report.print_report(root, ns, project_data, third_party_libs)
+
+            return report.print_missing_installed_libs(
+                brick_imports, third_party_libs, name
+            )
         except ValueError as e:
             self.line_error(f"{name}: <error>{e}</error>")
             return False
 
     def handle(self) -> int:
         root = repo.find_workspace_root(Path.cwd())
 
         if not root:
             raise ValueError(
                 "Didn't find the workspace root. Expected to find a workspace.toml file."
             )
 
         ns = workspace.parser.get_namespace_from_config(root)
 
-        all_projects_data = info.get_projects_data(root, ns)
-        projects_data = [p for p in all_projects_data if info.is_project(p)]
+        projects_data = info.get_projects_data(root, ns)
 
         if self.option("directory"):
             project_name = project.get_project_name(self.poetry.pyproject.data)
 
             data = next((p for p in projects_data if p["name"] == project_name), None)
 
             if not data:
```

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_base.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_component.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_project.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/create_workspace.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/create_workspace.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/diff.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/diff.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/info.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/info.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/libs.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/check.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 from pathlib import Path
 from typing import Set, Union
 
 from poetry.console.commands.command import Command
 from poetry.factory import Factory
-from polylith import info, project, repo, workspace
-from polylith.libs import report
+from polylith import check, info, project, repo, workspace
 
 
-class LibsCommand(Command):
-    name = "poly libs"
-    description = "Show third-party libraries used in the workspace."
+class CheckCommand(Command):
+    name = "poly check"
+    description = "Validates the <comment>Polylith</> workspace."
 
     def find_third_party_libs(self, path: Union[Path, None]) -> Set:
         project_poetry = Factory().create_poetry(path) if path else self.poetry
 
         if not project_poetry.locker.is_locked():
             raise ValueError("poetry.lock not found. Run `poetry lock` to create it.")
 
         packages = project_poetry.locker.locked_repository().packages
 
         return {p.name for p in packages}
 
-    def print_report(self, root: Path, ns: str, data: dict) -> bool:
-        name = data["name"]
-        path = data["path"]
-
-        brick_imports = report.get_third_party_imports(root, ns, data)
-
-        report.print_libs_summary(brick_imports, data)
-        report.print_libs_in_bricks(brick_imports)
+    def print_report(self, root: Path, ns: str, project_data: dict) -> bool:
+        is_verbose = self.option("verbose")
+        path = project_data["path"]
+        name = project_data["name"]
 
         try:
             third_party_libs = self.find_third_party_libs(path)
-
-            return report.print_missing_installed_libs(
-                brick_imports, third_party_libs, name
+            res, brick_imports, third_party_imports = check.report.print_report(
+                root,
+                ns,
+                project_data,
+                third_party_libs,
             )
+
+            if is_verbose:
+                check.report.print_brick_imports(brick_imports)
+                check.report.print_brick_imports(third_party_imports)
+
+            return res
         except ValueError as e:
             self.line_error(f"{name}: <error>{e}</error>")
             return False
 
     def handle(self) -> int:
         root = repo.find_workspace_root(Path.cwd())
 
         if not root:
             raise ValueError(
                 "Didn't find the workspace root. Expected to find a workspace.toml file."
             )
 
         ns = workspace.parser.get_namespace_from_config(root)
 
-        projects_data = info.get_projects_data(root, ns)
+        all_projects_data = info.get_projects_data(root, ns)
+        projects_data = [p for p in all_projects_data if info.is_project(p)]
 
         if self.option("directory"):
             project_name = project.get_project_name(self.poetry.pyproject.data)
 
             data = next((p for p in projects_data if p["name"] == project_name), None)
 
             if not data:
```

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry/commands/sync.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry/commands/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,16 @@
                 raise ValueError(f"Didn't find project in {self.option('directory')}")
 
             return [data]
 
         return all_projects_data
 
     def handle(self) -> int:
+        is_verbose = self.option("verbose")
+
         root = repo.find_workspace_root(Path.cwd())
 
         if not root:
             raise ValueError(
                 "Didn't find the workspace root. Expected to find a workspace.toml file."
             )
 
@@ -46,8 +48,11 @@
             for data in projects_data
         ]
 
         for diff in diffs:
             sync.report.print_summary(diff)
             sync.update_project(root, ns, diff)
 
+            if is_verbose:
+                sync.report.print_brick_imports(diff)
+
         return 0
```

### Comparing `poetry_polylith_plugin-1.6.2/polylith/poetry_plugin/plugin.py` & `poetry_polylith_plugin-1.7.0/polylith/poetry_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/project/create.py` & `poetry_polylith_plugin-1.7.0/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/project/get.py` & `poetry_polylith_plugin-1.7.0/polylith/project/get.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/readme/readme.py` & `poetry_polylith_plugin-1.7.0/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/repo/repo.py` & `poetry_polylith_plugin-1.7.0/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/sync/report.py` & `poetry_polylith_plugin-1.7.0/polylith/sync/report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+from polylith import check
 from polylith.reporting import theme
 from rich.console import Console
 
 
-def print_summary(diff: dict):
+def print_brick_imports(diff: dict) -> None:
+    brick_imports = diff["brick_imports"]
+
+    check.report.print_brick_imports(brick_imports)
+
+
+def print_summary(diff: dict) -> None:
     console = Console(theme=theme.poly_theme)
 
     is_project = diff["is_project"]
     name = diff["name"] if is_project else "development"
     bases = diff["bases"]
     components = diff["components"]
```

### Comparing `poetry_polylith_plugin-1.6.2/polylith/sync/update.py` & `poetry_polylith_plugin-1.7.0/polylith/sync/update.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/test/tests.py` & `poetry_polylith_plugin-1.7.0/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/workspace/create.py` & `poetry_polylith_plugin-1.7.0/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/workspace/parser.py` & `poetry_polylith_plugin-1.7.0/polylith/workspace/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/polylith/workspace/paths.py` & `poetry_polylith_plugin-1.7.0/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.6.2/pyproject.toml` & `poetry_polylith_plugin-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-polylith-plugin"
-version = "1.6.2"
+version = "1.7.0"
 description = "A Poetry plugin that adds tooling support for the Polylith Architecture"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 readme = "README.md"
 packages = [
     {include = "polylith"},
```

### Comparing `poetry_polylith_plugin-1.6.2/PKG-INFO` & `poetry_polylith_plugin-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-polylith-plugin
-Version: 1.6.2
+Version: 1.7.0
 Summary: A Poetry plugin that adds tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

