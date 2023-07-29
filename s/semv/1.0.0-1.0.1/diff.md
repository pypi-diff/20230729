# Comparing `tmp/semv-1.0.0.tar.gz` & `tmp/semv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semv-1.0.0.tar", last modified: Fri Jul 28 14:19:32 2023, max compression
+gzip compressed data, was "semv-1.0.1.tar", last modified: Sat Jul 29 19:35:30 2023, max compression
```

## Comparing `semv-1.0.0.tar` & `semv-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.342517 semv-1.0.0/
--rw-r--r--   0 ingo       (501) staff       (20)     3078 2023-07-28 08:00:44.000000 semv-1.0.0/.gitignore
--rw-r--r--   0 ingo       (501) staff       (20)    11357 2023-07-28 07:59:58.000000 semv-1.0.0/LICENSE
--rw-r--r--   0 ingo       (501) staff       (20)      383 2023-07-28 14:19:32.342265 semv-1.0.0/PKG-INFO
--rw-r--r--   0 ingo       (501) staff       (20)      170 2023-07-28 13:23:56.000000 semv-1.0.0/README.md
--rw-r--r--   0 ingo       (501) staff       (20)      410 2023-07-28 14:19:14.000000 semv-1.0.0/pyproject.toml
--rw-r--r--   0 ingo       (501) staff       (20)       38 2023-07-28 14:19:32.342566 semv-1.0.0/setup.cfg
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.338071 semv-1.0.0/src/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.340672 semv-1.0.0/src/semv/
--rw-r--r--   0 ingo       (501) staff       (20)        0 2023-07-28 13:23:56.000000 semv-1.0.0/src/semv/__init__.py
--rw-r--r--   0 ingo       (501) staff       (20)      845 2023-07-28 13:34:03.000000 semv-1.0.0/src/semv/commands.py
--rw-r--r--   0 ingo       (501) staff       (20)      233 2023-07-28 13:23:56.000000 semv-1.0.0/src/semv/config.py
--rw-r--r--   0 ingo       (501) staff       (20)      136 2023-07-28 13:37:16.000000 semv-1.0.0/src/semv/errors.py
--rw-r--r--   0 ingo       (501) staff       (20)     1344 2023-07-28 13:46:24.000000 semv-1.0.0/src/semv/increment.py
--rw-r--r--   0 ingo       (501) staff       (20)      669 2023-07-28 13:34:22.000000 semv-1.0.0/src/semv/interface.py
--rw-r--r--   0 ingo       (501) staff       (20)      302 2023-07-28 13:23:56.000000 semv-1.0.0/src/semv/main.py
--rw-r--r--   0 ingo       (501) staff       (20)     1241 2023-07-28 13:51:47.000000 semv-1.0.0/src/semv/parse.py
--rw-r--r--   0 ingo       (501) staff       (20)        0 2023-07-28 13:23:56.000000 semv-1.0.0/src/semv/py.typed
--rw-r--r--   0 ingo       (501) staff       (20)     1478 2023-07-28 13:23:56.000000 semv-1.0.0/src/semv/types.py
--rw-r--r--   0 ingo       (501) staff       (20)      344 2023-07-28 13:46:43.000000 semv-1.0.0/src/semv/utils.py
--rw-r--r--   0 ingo       (501) staff       (20)      964 2023-07-28 13:23:56.000000 semv-1.0.0/src/semv/version_control_system.py
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.341395 semv-1.0.0/src/semv.egg-info/
--rw-r--r--   0 ingo       (501) staff       (20)      383 2023-07-28 14:19:32.000000 semv-1.0.0/src/semv.egg-info/PKG-INFO
--rw-r--r--   0 ingo       (501) staff       (20)      616 2023-07-28 14:19:32.000000 semv-1.0.0/src/semv.egg-info/SOURCES.txt
--rw-r--r--   0 ingo       (501) staff       (20)        1 2023-07-28 14:19:32.000000 semv-1.0.0/src/semv.egg-info/dependency_links.txt
--rw-r--r--   0 ingo       (501) staff       (20)       40 2023-07-28 14:19:32.000000 semv-1.0.0/src/semv.egg-info/entry_points.txt
--rw-r--r--   0 ingo       (501) staff       (20)        5 2023-07-28 14:19:32.000000 semv-1.0.0/src/semv.egg-info/top_level.txt
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.338293 semv-1.0.0/tests/
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.341517 semv-1.0.0/tests/cram/
--rw-r--r--   0 ingo       (501) staff       (20)     2608 2023-07-28 13:23:56.000000 semv-1.0.0/tests/cram/test_normal_usage.t
-drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-28 14:19:32.342046 semv-1.0.0/tests/unit/
--rw-r--r--   0 ingo       (501) staff       (20)      632 2023-07-28 13:23:55.000000 semv-1.0.0/tests/unit/test_commit_parsing.py
--rw-r--r--   0 ingo       (501) staff       (20)     2288 2023-07-28 13:23:55.000000 semv-1.0.0/tests/unit/test_git.py
--rw-r--r--   0 ingo       (501) staff       (20)      890 2023-07-28 13:23:56.000000 semv-1.0.0/tests/unit/test_version.py
--rw-r--r--   0 ingo       (501) staff       (20)     1814 2023-07-28 13:23:56.000000 semv-1.0.0/tests/unit/test_version_incrementer.py
--rw-r--r--   0 ingo       (501) staff       (20)      309 2023-07-28 13:58:01.000000 semv-1.0.0/tox.ini
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.599943 semv-1.0.1/
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.594823 semv-1.0.1/.github/
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.596322 semv-1.0.1/.github/workflows/
+-rw-r--r--   0 ingo       (501) staff       (20)      856 2023-07-29 19:18:34.000000 semv-1.0.1/.github/workflows/create-version-tag.yml
+-rw-r--r--   0 ingo       (501) staff       (20)      564 2023-07-29 18:58:25.000000 semv-1.0.1/.github/workflows/run-tests.yml
+-rw-r--r--   0 ingo       (501) staff       (20)     3078 2023-07-28 08:00:44.000000 semv-1.0.1/.gitignore
+-rw-r--r--   0 ingo       (501) staff       (20)    11357 2023-07-28 07:59:58.000000 semv-1.0.1/LICENSE
+-rw-r--r--   0 ingo       (501) staff       (20)      383 2023-07-29 19:35:30.599690 semv-1.0.1/PKG-INFO
+-rw-r--r--   0 ingo       (501) staff       (20)      170 2023-07-28 13:23:56.000000 semv-1.0.1/README.md
+-rw-r--r--   0 ingo       (501) staff       (20)      518 2023-07-28 14:36:13.000000 semv-1.0.1/pyproject.toml
+-rw-r--r--   0 ingo       (501) staff       (20)       38 2023-07-29 19:35:30.599994 semv-1.0.1/setup.cfg
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.595040 semv-1.0.1/src/
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.597856 semv-1.0.1/src/semv/
+-rw-r--r--   0 ingo       (501) staff       (20)        0 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/__init__.py
+-rw-r--r--   0 ingo       (501) staff       (20)      859 2023-07-28 14:27:45.000000 semv-1.0.1/src/semv/commands.py
+-rw-r--r--   0 ingo       (501) staff       (20)      233 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/config.py
+-rw-r--r--   0 ingo       (501) staff       (20)      136 2023-07-28 13:37:16.000000 semv-1.0.1/src/semv/errors.py
+-rw-r--r--   0 ingo       (501) staff       (20)     1344 2023-07-28 13:46:24.000000 semv-1.0.1/src/semv/increment.py
+-rw-r--r--   0 ingo       (501) staff       (20)      669 2023-07-28 13:34:22.000000 semv-1.0.1/src/semv/interface.py
+-rw-r--r--   0 ingo       (501) staff       (20)      302 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/main.py
+-rw-r--r--   0 ingo       (501) staff       (20)     1249 2023-07-29 18:58:25.000000 semv-1.0.1/src/semv/parse.py
+-rw-r--r--   0 ingo       (501) staff       (20)        0 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/py.typed
+-rw-r--r--   0 ingo       (501) staff       (20)     1484 2023-07-28 14:28:01.000000 semv-1.0.1/src/semv/types.py
+-rw-r--r--   0 ingo       (501) staff       (20)      350 2023-07-28 14:27:54.000000 semv-1.0.1/src/semv/utils.py
+-rw-r--r--   0 ingo       (501) staff       (20)      964 2023-07-28 13:23:56.000000 semv-1.0.1/src/semv/version_control_system.py
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.598569 semv-1.0.1/src/semv.egg-info/
+-rw-r--r--   0 ingo       (501) staff       (20)      383 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/PKG-INFO
+-rw-r--r--   0 ingo       (501) staff       (20)      709 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/SOURCES.txt
+-rw-r--r--   0 ingo       (501) staff       (20)        1 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/dependency_links.txt
+-rw-r--r--   0 ingo       (501) staff       (20)       40 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/entry_points.txt
+-rw-r--r--   0 ingo       (501) staff       (20)        5 2023-07-29 19:35:30.000000 semv-1.0.1/src/semv.egg-info/top_level.txt
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.595240 semv-1.0.1/tests/
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.598925 semv-1.0.1/tests/cram/
+-rw-r--r--   0 ingo       (501) staff       (20)      208 2023-07-29 18:38:01.000000 semv-1.0.1/tests/cram/setup.sh
+-rw-r--r--   0 ingo       (501) staff       (20)     2496 2023-07-29 18:39:01.000000 semv-1.0.1/tests/cram/test_normal_usage.t
+drwxr-xr-x   0 ingo       (501) staff       (20)        0 2023-07-29 19:35:30.599465 semv-1.0.1/tests/unit/
+-rw-r--r--   0 ingo       (501) staff       (20)     1168 2023-07-29 18:58:25.000000 semv-1.0.1/tests/unit/test_commit_parsing.py
+-rw-r--r--   0 ingo       (501) staff       (20)     2441 2023-07-29 18:34:00.000000 semv-1.0.1/tests/unit/test_git.py
+-rw-r--r--   0 ingo       (501) staff       (20)      890 2023-07-28 13:23:56.000000 semv-1.0.1/tests/unit/test_version.py
+-rw-r--r--   0 ingo       (501) staff       (20)     1814 2023-07-28 13:23:56.000000 semv-1.0.1/tests/unit/test_version_incrementer.py
+-rw-r--r--   0 ingo       (501) staff       (20)      640 2023-07-28 14:39:35.000000 semv-1.0.1/tox.ini
```

### Comparing `semv-1.0.0/.gitignore` & `semv-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `semv-1.0.0/LICENSE` & `semv-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semv-1.0.0/src/semv/commands.py` & `semv-1.0.1/src/semv/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,13 +14,15 @@
         InvalidCommitType
     """
     vcs = Git()
     cp = AngularCommitParser(config.invalid_commit_action)
     vi = DefaultIncrementer(config.invalid_commit_action)
 
     current_version = vcs.get_current_version()
-    commits_or_none = (cp.parse(c) for c in vcs.get_commits_without(current_version))
+    commits_or_none = (
+        cp.parse(c) for c in vcs.get_commits_without(current_version)
+    )
     commits = (c for c in commits_or_none if c is not None)
     inc = vi.get_version_increment(commits)
     if inc == VersionIncrement.skip:
         raise errors.NoNewVersion
     return current_version + inc
```

### Comparing `semv-1.0.0/src/semv/increment.py` & `semv-1.0.1/src/semv/increment.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.0/src/semv/interface.py` & `semv-1.0.1/src/semv/interface.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.0/src/semv/parse.py` & `semv-1.0.1/src/semv/parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class AngularCommitParser(CommitParser):
     def __init__(
         self,
         invalid_commit_action: InvalidCommitAction = InvalidCommitAction.skip,
     ):
         self.type_and_scope_pattern = re.compile(
-            r'(?P<type>\w+)\((?P<scope>\w+)\): .*'
+            r'(?P<type>\w+)\((?P<scope>[a-zA-Z-_]+)\): .*'
         )
         self.breaking_pattern = re.compile(
             r'BREAKING CHANGE: .*', flags=re.DOTALL
         )
         self.invalid_commit_action = invalid_commit_action
 
     def parse(self, commit: RawCommit) -> Optional[Commit]:
```

### Comparing `semv-1.0.0/src/semv/types.py` & `semv-1.0.1/src/semv/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,13 +50,13 @@
     def __str__(self):
         return f'v{self.major}.{self.minor}.{self.patch}'
 
     def __add__(self, inc: VersionIncrement) -> 'Version':
         if inc == VersionIncrement.skip:
             return self
         elif inc == VersionIncrement.major:
-            return replace(self, major=self.major+1, minor=0, patch=0)
+            return replace(self, major=self.major + 1, minor=0, patch=0)
         elif inc == VersionIncrement.minor:
-            return replace(self, minor=self.minor+1, patch=0)
+            return replace(self, minor=self.minor + 1, patch=0)
         elif inc == VersionIncrement.patch:
-            return replace(self, patch=self.patch+1)
+            return replace(self, patch=self.patch + 1)
         raise RuntimeError('This should never happen')
```

### Comparing `semv-1.0.0/src/semv/version_control_system.py` & `semv-1.0.1/src/semv/version_control_system.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.0/src/semv.egg-info/SOURCES.txt` & `semv-1.0.1/src/semv.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 tox.ini
+.github/workflows/create-version-tag.yml
+.github/workflows/run-tests.yml
 src/semv/__init__.py
 src/semv/commands.py
 src/semv/config.py
 src/semv/errors.py
 src/semv/increment.py
 src/semv/interface.py
 src/semv/main.py
@@ -16,12 +18,13 @@
 src/semv/utils.py
 src/semv/version_control_system.py
 src/semv.egg-info/PKG-INFO
 src/semv.egg-info/SOURCES.txt
 src/semv.egg-info/dependency_links.txt
 src/semv.egg-info/entry_points.txt
 src/semv.egg-info/top_level.txt
+tests/cram/setup.sh
 tests/cram/test_normal_usage.t
 tests/unit/test_commit_parsing.py
 tests/unit/test_git.py
 tests/unit/test_version.py
 tests/unit/test_version_incrementer.py
```

### Comparing `semv-1.0.0/tests/cram/test_normal_usage.t` & `semv-1.0.1/tests/cram/test_normal_usage.t`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 This example will run through a typical scenario of using semv. As this is a
 script, we will need to perform all code changes using echo commands, which is
 kind of awkward, but it should be sufficient for testing.
 
 We need to run semv in a git repository.
-  $ git init
+  $ bash "$TESTDIR"/setup.sh
   Initialized empty Git repository in */.git/ (glob)
-  $ echo "This is the readme" > README.md
-  $ git add README.md
-  $ git commit -m 'docs(readme): Add readme'
   [master (root-commit) *] docs(readme): Add readme (glob)
    1 file changed, 1 insertion(+)
    create mode 100644 README.md
-  $ git tag v0.0.0
 
 We now have a (non working) initial version v0.0.0 (note however, that this is
 not standard and you might rather want to pick v1.0.0). We will now add a few
 commits and then get a new version.
   $ echo "print('Hello')" > myscript.py
   $ git add myscript.py
   $ git commit -m 'feat(myscript): Print a message'
```

### Comparing `semv-1.0.0/tests/unit/test_commit_parsing.py` & `semv-1.0.1/tests/unit/test_commit_parsing.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,7 +9,19 @@
             RawCommit(sha='any sha', title='feat(scope): Message', body='')
         ) == Commit(sha='any sha', type='feat', scope='scope', breaking=False)
     def test_breaking(self):
         p = AngularCommitParser()
         assert p.parse(
             RawCommit(sha='any sha', title='feat(scope): Message', body='BREAKING CHANGE: bla bla')
         ) == Commit(sha='any sha', type='feat', scope='scope', breaking=True)
+
+    def test_scope_may_include_underscore(self):
+        p = AngularCommitParser()
+        assert p.parse(
+            RawCommit(sha='any sha', title='feat(any_scope): Message', body='')
+        ) == Commit(sha='any sha', type='feat', scope='any_scope', breaking=False)
+
+    def test_scope_may_include_dash(self):
+        p = AngularCommitParser()
+        assert p.parse(
+            RawCommit(sha='any sha', title='feat(any-scope): Message', body='')
+        ) == Commit(sha='any sha', type='feat', scope='any-scope', breaking=False)
```

### Comparing `semv-1.0.0/tests/unit/test_git.py` & `semv-1.0.1/tests/unit/test_git.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 def git_repo():
     with TemporaryDirectory() as td:
         subprocess.run(
             'git init',
             shell=True,
             cwd=td,
         )
+        subprocess.run('git config user.name "tester"', shell=True, cwd=td)
+        subprocess.run('git config user.email "tester"', shell=True, cwd=td)
         yield Repo(td)
 
 
 class TestCurrentVersion:
     def test_tagged_version(self, git_repo):
         git_repo: Repo
         git_repo.add_to_file('test.txt', 'First line')
```

### Comparing `semv-1.0.0/tests/unit/test_version.py` & `semv-1.0.1/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `semv-1.0.0/tests/unit/test_version_incrementer.py` & `semv-1.0.1/tests/unit/test_version_incrementer.py`

 * *Files identical despite different names*

