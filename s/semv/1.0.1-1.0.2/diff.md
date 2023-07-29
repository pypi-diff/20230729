# Comparing `tmp/semv-1.0.1.tar.gz` & `tmp/semv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semv-1.0.1.tar", last modified: Sat Jul 29 19:35:30 2023, max compression
+gzip compressed data, was "semv-1.0.2.tar", last modified: Sat Jul 29 20:36:27 2023, max compression
```

## Comparing `semv-1.0.1.tar` & `semv-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.599943 semv-1.0.1/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.594823 semv-1.0.1/.github/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.596322 semv-1.0.1/.github/workflows/
--rw-r--r--   0 ingo       (501) staff       (20)      856 2023-07-29 19:18:34.000000 semv-1.0.1/.github/workflows/create-version-tag.yml
--rw-r--r--   0 ingo       (501) staff       (20)      564 2023-07-29 18:58:25.000000 semv-1.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 ingo       (501) staff       (20)     3078 2023-07-28 08:00:44.000000 semv-1.0.1/.gitignore
--rw-r--r--   0 ingo       (501) staff       (20)    11357 2023-07-28 07:59:58.000000 semv-1.0.1/LICENSE
--rw-r--r--   0 ingo       (501) staff       (20)      383 2023-07-29 19:35:30.599690 semv-1.0.1/PKG-INFO
--rw-r--r--   0 ingo       (501) staff       (20)      170 2023-07-28 13:23:56.000000 semv-1.0.1/README.md
--rw-r--r--   0 ingo       (501) staff       (20)      518 2023-07-28 14:36:13.000000 semv-1.0.1/pyproject.toml
--rw-r--r--   0 ingo       (501) staff       (20)       38 2023-07-29 19:35:30.599994 semv-1.0.1/setup.cfg
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.595040 semv-1.0.1/src/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.597856 semv-1.0.1/src/semv/
--rw-r--r--   0 ingo       (501) staff       (20)        0 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/__init__.py
--rw-r--r--   0 ingo       (501) staff       (20)      859 2023-07-28 14:27:45.000000 semv-1.0.1/src/semv/commands.py
--rw-r--r--   0 ingo       (501) staff       (20)      233 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/config.py
--rw-r--r--   0 ingo       (501) staff       (20)      136 2023-07-28 13:37:16.000000 semv-1.0.1/src/semv/errors.py
--rw-r--r--   0 ingo       (501) staff       (20)     1344 2023-07-28 13:46:24.000000 semv-1.0.1/src/semv/increment.py
--rw-r--r--   0 ingo       (501) staff       (20)      669 2023-07-28 13:34:22.000000 semv-1.0.1/src/semv/interface.py
--rw-r--r--   0 ingo       (501) staff       (20)      302 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/main.py
--rw-r--r--   0 ingo       (501) staff       (20)     1249 2023-07-29 18:58:25.000000 semv-1.0.1/src/semv/parse.py
--rw-r--r--   0 ingo       (501) staff       (20)        0 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/py.typed
--rw-r--r--   0 ingo       (501) staff       (20)     1484 2023-07-28 14:28:01.000000 semv-1.0.1/src/semv/types.py
--rw-r--r--   0 ingo       (501) staff       (20)      350 2023-07-28 14:27:54.000000 semv-1.0.1/src/semv/utils.py
--rw-r--r--   0 ingo       (501) staff       (20)      964 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/version_control_system.py
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.598569 semv-1.0.1/src/semv.egg-info/
--rw-r--r--   0 ingo       (501) staff       (20)      383 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/PKG-INFO
--rw-r--r--   0 ingo       (501) staff       (20)      709 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/SOURCES.txt
--rw-r--r--   0 ingo       (501) staff       (20)        1 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/dependency_links.txt
--rw-r--r--   0 ingo       (501) staff       (20)       40 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/entry_points.txt
--rw-r--r--   0 ingo       (501) staff       (20)        5 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/top_level.txt
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.595240 semv-1.0.1/tests/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.598925 semv-1.0.1/tests/cram/
--rw-r--r--   0 ingo       (501) staff       (20)      208 2023-07-29 18:38:01.000000 semv-1.0.1/tests/cram/setup.sh
--rw-r--r--   0 ingo       (501) staff       (20)     2496 2023-07-29 18:39:01.000000 semv-1.0.1/tests/cram/test_normal_usage.t
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.599465 semv-1.0.1/tests/unit/
--rw-r--r--   0 ingo       (501) staff       (20)     1168 2023-07-29 18:58:25.000000 semv-1.0.1/tests/unit/test_commit_parsing.py
--rw-r--r--   0 ingo       (501) staff       (20)     2441 2023-07-29 18:34:00.000000 semv-1.0.1/tests/unit/test_git.py
--rw-r--r--   0 ingo       (501) staff       (20)      890 2023-07-28 13:23:56.000000 semv-1.0.1/tests/unit/test_version.py
--rw-r--r--   0 ingo       (501) staff       (20)     1814 2023-07-28 13:23:56.000000 semv-1.0.1/tests/unit/test_version_incrementer.py
--rw-r--r--   0 ingo       (501) staff       (20)      640 2023-07-28 14:39:35.000000 semv-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.503829 semv-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.487829 semv-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.491829 semv-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-29 20:35:39.000000 semv-1.0.2/.github/workflows/attempt-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-29 20:35:39.000000 semv-1.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-29 20:35:39.000000 semv-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 20:35:39.000000 semv-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 20:36:27.503829 semv-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-29 20:35:39.000000 semv-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-29 20:35:39.000000 semv-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:36:27.503829 semv-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.487829 semv-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.495829 semv-1.0.2/src/semv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 20:35:39.000000 semv-1.0.2/src/semv/version_control_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.499829 semv-1.0.2/src/semv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 20:36:27.000000 semv-1.0.2/src/semv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.487829 semv-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.499829 semv-1.0.2/tests/cram/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-29 20:35:39.000000 semv-1.0.2/tests/cram/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-29 20:35:39.000000 semv-1.0.2/tests/cram/test_normal_usage.t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:36:27.503829 semv-1.0.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_commit_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-29 20:35:39.000000 semv-1.0.2/tests/unit/test_version_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 20:35:39.000000 semv-1.0.2/tox.ini
```

### Comparing `semv-1.0.1/.github/workflows/create-version-tag.yml` & `semv-1.0.2/.github/workflows/attempt-release.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-name: Create version tag
+name: Attempt release
 on:
   push:
     branches: ["master"]
 
 jobs:
   create-version-tag:
     runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/p/semv
+    permissions:
+      contents: write
+      id-token: write
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup python 3.8
         uses: actions/setup-python@v4
         with:
@@ -28,7 +34,16 @@
         run: tox
       - name: Print version
         id: print-version
         run: echo "semv-out=$(semv)" >> $GITHUB_OUTPUT
       - uses: thejeff77/action-push-tag@v1.0.0
         with:
           tag: ${{ steps.print-version.outputs.semv-out }}
+      - name: Create github release
+        uses: softprops/action-gh-release@v1
+        with:
+          tag_name: ${{ steps.print-version.outputs.semv-out }}
+          generate_release_notes: true
+      - name: Build package
+        run: tox -e build
+      - name: Publish to pypi
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `semv-1.0.1/.github/workflows/run-tests.yml` & `semv-1.0.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/.gitignore` & `semv-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/LICENSE` & `semv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/pyproject.toml` & `semv-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/src/semv/commands.py` & `semv-1.0.2/src/semv/commands.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/src/semv/increment.py` & `semv-1.0.2/src/semv/increment.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/src/semv/interface.py` & `semv-1.0.2/src/semv/interface.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/src/semv/parse.py` & `semv-1.0.2/src/semv/parse.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/src/semv/types.py` & `semv-1.0.2/src/semv/types.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/src/semv/version_control_system.py` & `semv-1.0.2/src/semv/version_control_system.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 
 
 class Git(VersionControlSystem):
     def get_current_version(self) -> Version:
         v = (
             subprocess.check_output('git tag', shell=True)
             .decode('utf-8')
-            .splitlines()[-1]
+            .splitlines()
         )
 
-        return Version.from_string(v)
+        if v:
+            return Version.from_string(v[-1])
+        else:
+            return Version(major=0)
 
     def get_commits_without(
         self, current_version: Version
     ) -> Iterator[RawCommit]:
         fmt = {
             'sha': '%h',
             'title': '%s',
```

### Comparing `semv-1.0.1/src/semv.egg-info/SOURCES.txt` & `semv-1.0.2/src/semv.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 tox.ini
-.github/workflows/create-version-tag.yml
+.github/workflows/attempt-release.yml
 .github/workflows/run-tests.yml
 src/semv/__init__.py
 src/semv/commands.py
 src/semv/config.py
 src/semv/errors.py
 src/semv/increment.py
 src/semv/interface.py
```

### Comparing `semv-1.0.1/tests/cram/test_normal_usage.t` & `semv-1.0.2/tests/cram/test_normal_usage.t`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/tests/unit/test_commit_parsing.py` & `semv-1.0.2/tests/unit/test_commit_parsing.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/tests/unit/test_git.py` & `semv-1.0.2/tests/unit/test_git.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,23 @@
         git_repo.git('add test.txt')
         git_repo.git('commit -m "Second commit"')
 
         with git_repo.as_working_dir():
             g = Git()
             assert str(g.get_current_version()) == 'v1.0.0'
 
+    def test_default_version_if_no_tags(self, git_repo):
+        git_repo: Repo
+        git_repo.add_to_file('test.txt', 'First line')
+        git_repo.git('add test.txt')
+        git_repo.git('commit -m "First commit"')
+        with git_repo.as_working_dir():
+            g = Git()
+            assert str(g.get_current_version()) == 'v0.0.0'
+
 
 class TestCommitsWithout:
     def test_commits_without(self, git_repo):
         git_repo: Repo
         git_repo.commit_change('test.txt', 'First line', 'First commit')
         git_repo.commit_change('test.txt', 'Second line', 'Second commit')
         git_repo.git('tag v1.0.0')
```

### Comparing `semv-1.0.1/tests/unit/test_version.py` & `semv-1.0.2/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/tests/unit/test_version_incrementer.py` & `semv-1.0.2/tests/unit/test_version_incrementer.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.1/tox.ini` & `semv-1.0.2/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -26,10 +26,13 @@
 deps =
   build
 commands = python -m build
 
 [testenv:publish]
 skip_dist = true
 skip_install = true
+allowlist_externals =
+  bash
 deps =
   twine
-commands = twine upload dist/semv-$(python -m setuptools_scm).tar.gz dist/semv-$(python -m setuptools_scm)-py3-none-any.whl
+  setuptools-scm
+commands = bash -c 'twine upload "dist/semv-$(python -m setuptools_scm).tar.gz" "dist/semv-$(python -m setuptools_scm)-py3-none-any.whl"'
```

