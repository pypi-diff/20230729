# Comparing `tmp/commitizen-3.5.3.tar.gz` & `tmp/commitizen-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.5.3.tar", max compression
+gzip compressed data, was "commitizen-3.5.4.tar", max compression
```

## Comparing `commitizen-3.5.3.tar` & `commitizen-3.5.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-07-15 15:41:12.908831 commitizen-3.5.3/LICENSE
--rw-r--r--   0        0        0      609 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/__version__.py
--rw-r--r--   0        0        0     4543 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/bump.py
--rw-r--r--   0        0        0    12112 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    18106 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    14245 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7148 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5208 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-07-15 15:41:12.908831 commitizen-3.5.3/commitizen/commands/info.py
--rw-r--r--   0        0        0    13053 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3336 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/factory.py
--rw-r--r--   0        0        0     7295 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/out.py
--rw-r--r--   0        0        0     7134 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9732 2023-07-15 15:41:12.912832 commitizen-3.5.3/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-07-15 15:41:12.912832 commitizen-3.5.3/docs/README.md
--rw-r--r--   0        0        0     4300 2023-07-15 15:41:12.924832 commitizen-3.5.3/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-29 11:26:12.675897 commitizen-3.5.4/LICENSE
+-rw-r--r--   0        0        0      609 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/__version__.py
+-rw-r--r--   0        0        0     4556 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/bump.py
+-rw-r--r--   0        0        0    12112 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    18106 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14245 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7148 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5208 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/info.py
+-rw-r--r--   0        0        0    13053 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3336 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/factory.py
+-rw-r--r--   0        0        0     7295 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/out.py
+-rw-r--r--   0        0        0     7134 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9726 2023-07-29 11:26:12.675897 commitizen-3.5.4/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-07-29 11:26:12.675897 commitizen-3.5.4/docs/README.md
+-rw-r--r--   0        0        0     4308 2023-07-29 11:26:12.687897 commitizen-3.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.4/PKG-INFO
```

### Comparing `commitizen-3.5.3/LICENSE` & `commitizen-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/__init__.py` & `commitizen-3.5.4/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/bump.py` & `commitizen-3.5.4/commitizen/bump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import os
 import re
 from collections import OrderedDict
 from string import Template
 
-from commitizen.defaults import bump_message
+from commitizen.defaults import MAJOR, MINOR, PATCH, bump_message
 from commitizen.exceptions import CurrentVersionNotFoundError
 from commitizen.git import GitCommit, smart_open
 from commitizen.version_schemes import DEFAULT_SCHEME, VersionScheme, Version
 
 
 def find_increment(
     commits: list[GitCommit], regex: str, increments_map: dict | OrderedDict
@@ -30,19 +30,19 @@
                 found_keyword = result.group(1)
                 new_increment = None
                 for match_pattern in increments_map.keys():
                     if re.match(match_pattern, found_keyword):
                         new_increment = increments_map[match_pattern]
                         break
 
-                if increment == "MAJOR":
+                if increment == MAJOR:
                     break
-                elif increment == "MINOR" and new_increment == "MAJOR":
+                elif increment == MINOR and new_increment == MAJOR:
                     increment = new_increment
-                elif increment == "PATCH" or increment is None:
+                elif increment == PATCH or increment is None:
                     increment = new_increment
 
     return increment
 
 
 def update_version_in_files(
     current_version: str, new_version: str, files: list[str], *, check_consistency=False
```

### Comparing `commitizen-3.5.3/commitizen/changelog.py` & `commitizen-3.5.4/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/changelog_parser.py` & `commitizen-3.5.4/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cli.py` & `commitizen-3.5.4/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cmd.py` & `commitizen-3.5.4/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/commands/bump.py` & `commitizen-3.5.4/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/commands/changelog.py` & `commitizen-3.5.4/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/commands/check.py` & `commitizen-3.5.4/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/commands/commit.py` & `commitizen-3.5.4/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/commands/init.py` & `commitizen-3.5.4/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/commands/version.py` & `commitizen-3.5.4/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/config/__init__.py` & `commitizen-3.5.4/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/config/base_config.py` & `commitizen-3.5.4/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/config/json_config.py` & `commitizen-3.5.4/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/config/toml_config.py` & `commitizen-3.5.4/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/config/yaml_config.py` & `commitizen-3.5.4/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/__init__.py` & `commitizen-3.5.4/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/base.py` & `commitizen-3.5.4/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.5.4/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/customize/customize.py` & `commitizen-3.5.4/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/jira/jira.py` & `commitizen-3.5.4/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/cz/jira/jira_info.txt` & `commitizen-3.5.4/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/defaults.py` & `commitizen-3.5.4/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/exceptions.py` & `commitizen-3.5.4/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/factory.py` & `commitizen-3.5.4/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/git.py` & `commitizen-3.5.4/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/hooks.py` & `commitizen-3.5.4/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/out.py` & `commitizen-3.5.4/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/providers.py` & `commitizen-3.5.4/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/commitizen/version_schemes.py` & `commitizen-3.5.4/commitizen/version_schemes.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                 base[PATCH] = 0
             elif increment == MINOR:
                 base[MINOR] += 1
                 base[PATCH] = 0
             elif increment == PATCH:
                 base[PATCH] += 1
 
-        return f"{base['MAJOR']}.{base['MINOR']}.{base['PATCH']}"
+        return f"{base[MAJOR]}.{base[MINOR]}.{base[PATCH]}"
 
     def bump(
         self,
         increment: str,
         prerelease: str | None = None,
         prerelease_offset: int = 0,
         devrelease: int | None = None,
```

### Comparing `commitizen-3.5.3/docs/README.md` & `commitizen-3.5.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.3/pyproject.toml` & `commitizen-3.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.5.3"
+version = "3.5.4"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.5.3"
+version = "3.5.4"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -57,18 +57,18 @@
 pytest-mock = "^3.10"
 pytest-regressions = "^2.4.0"
 pytest-freezer = "^0.4.6"
 pytest-xdist = "^3.1.0"
 # code formatter
 black = "^22.10"
 # linter
-ruff = ">=0.0.275,<0.0.279"
+ruff = ">=0.0.275,<0.0.281"
 pre-commit = "^2.18.0"
 mypy = "^1.4"
-types-PyYAML = "^5.4.3"
+types-PyYAML = ">=5.4.3,<7.0.0"
 types-termcolor = "^0.1.1"
 # documentation
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
 deprecated = "^1.2.13"
 types-deprecated = "^1.2.9.2"
 types-python-dateutil = "^2.8.19.13"
```

### Comparing `commitizen-3.5.3/PKG-INFO` & `commitizen-3.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.5.3
+Version: 3.5.4
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

