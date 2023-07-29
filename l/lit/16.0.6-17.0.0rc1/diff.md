# Comparing `tmp/lit-16.0.6.tar.gz` & `tmp/lit-17.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lit-16.0.6.tar", last modified: Wed Jun 14 18:54:46 2023, max compression
+gzip compressed data, was "lit-17.0.0rc1.tar", last modified: Sat Jul 29 14:13:58 2023, max compression
```

## Comparing `lit-16.0.6.tar` & `lit-17.0.0rc1.tar`

### file list

```diff
@@ -1,606 +1,611 @@
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.654749 lit-16.0.6/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    15141 2022-05-20 05:53:51.000000 lit-16.0.6/LICENSE.TXT
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      242 2022-05-20 05:53:51.000000 lit-16.0.6/MANIFEST.in
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2516 2023-06-14 18:54:46.653749 lit-16.0.6/PKG-INFO
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1874 2023-05-13 06:19:19.000000 lit-16.0.6/README.rst
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.630749 lit-16.0.6/examples/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-16.0.6/examples/README.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.631749 lit-16.0.6/examples/many-tests/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      533 2022-05-20 05:53:51.000000 lit-16.0.6/examples/many-tests/ManyTests.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      382 2022-05-20 05:53:51.000000 lit-16.0.6/examples/many-tests/README.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      146 2023-06-10 22:52:12.000000 lit-16.0.6/examples/many-tests/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.631749 lit-16.0.6/lit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)    11756 2023-06-10 22:52:12.000000 lit-16.0.6/lit/BooleanExpression.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     7772 2023-06-10 22:52:12.000000 lit-16.0.6/lit/LitConfig.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2023-06-10 22:52:12.000000 lit-16.0.6/lit/LitTestCase.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    11007 2023-06-10 22:52:12.000000 lit-16.0.6/lit/ProgressBar.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     3286 2023-06-10 22:52:12.000000 lit-16.0.6/lit/ShCommands.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8896 2023-06-10 22:52:12.000000 lit-16.0.6/lit/ShUtil.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13737 2023-06-10 22:52:12.000000 lit-16.0.6/lit/Test.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    79561 2023-06-10 22:52:12.000000 lit-16.0.6/lit/TestRunner.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1638 2023-06-10 22:52:12.000000 lit-16.0.6/lit/TestTimes.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     8115 2023-06-10 22:52:12.000000 lit-16.0.6/lit/TestingConfig.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      191 2023-06-14 18:49:20.000000 lit-16.0.6/lit/__init__.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.632749 lit-16.0.6/lit/builtin_commands/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-16.0.6/lit/builtin_commands/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1867 2023-06-10 22:52:12.000000 lit-16.0.6/lit/builtin_commands/cat.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     9308 2023-06-10 22:52:12.000000 lit-16.0.6/lit/builtin_commands/diff.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    10786 2023-06-10 22:52:12.000000 lit-16.0.6/lit/cl_arguments.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    10919 2023-06-10 22:52:12.000000 lit-16.0.6/lit/discovery.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     6055 2023-06-10 22:52:12.000000 lit-16.0.6/lit/display.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.632749 lit-16.0.6/lit/formats/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      241 2023-06-10 22:52:12.000000 lit-16.0.6/lit/formats/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4341 2023-06-10 22:52:12.000000 lit-16.0.6/lit/formats/base.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13217 2023-06-10 22:52:12.000000 lit-16.0.6/lit/formats/googletest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1055 2023-06-10 22:52:12.000000 lit-16.0.6/lit/formats/shtest.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.632749 lit-16.0.6/lit/llvm/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-05-20 05:53:51.000000 lit-16.0.6/lit/llvm/__init__.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    30089 2023-06-10 22:52:12.000000 lit-16.0.6/lit/llvm/config.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5544 2023-06-10 22:52:12.000000 lit-16.0.6/lit/llvm/subst.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11435 2023-06-10 22:52:12.000000 lit-16.0.6/lit/main.py
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)    10995 2023-06-10 22:52:12.000000 lit-16.0.6/lit/reports.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4697 2023-06-10 22:52:12.000000 lit-16.0.6/lit/run.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    15705 2023-06-10 22:52:12.000000 lit-16.0.6/lit/util.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2666 2023-06-10 22:52:12.000000 lit-16.0.6/lit/worker.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.632749 lit-16.0.6/lit.egg-info/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2516 2023-06-14 18:54:46.000000 lit-16.0.6/lit.egg-info/PKG-INFO
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    21186 2023-06-14 18:54:46.000000 lit-16.0.6/lit.egg-info/SOURCES.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-06-14 18:54:46.000000 lit-16.0.6/lit.egg-info/dependency_links.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-06-14 18:54:46.000000 lit-16.0.6/lit.egg-info/entry_points.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-04-10 18:12:43.000000 lit-16.0.6/lit.egg-info/not-zip-safe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        4 2023-06-14 18:54:46.000000 lit-16.0.6/lit.egg-info/top_level.txt
--rwxr-xr-x   0 tstellar (101195) tstellar (101195)       89 2023-06-10 22:52:12.000000 lit-16.0.6/lit.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2023-04-28 22:43:05.000000 lit-16.0.6/pyproject.toml
--rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2023-06-14 18:54:46.654749 lit-16.0.6/setup.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1336 2023-06-10 22:52:12.000000 lit-16.0.6/setup.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.634749 lit-16.0.6/tests/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      152 2022-05-20 05:53:51.000000 lit-16.0.6/tests/.coveragerc
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.634749 lit-16.0.6/tests/Inputs/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/allow-retries/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/allow-retries/does-not-succeed-within-limit.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      336 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/allow-retries/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       51 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/allow-retries/more-than-one-allow-retries-lines.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       45 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/allow-retries/not-a-valid-integer.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/allow-retries/succeeds-within-limit.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/config-map-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      443 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/config-map-discovery/driver.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/config-map-discovery/invalid-test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      281 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/config-map-discovery/lit.alt.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/config-map-discovery/main-config/
--rw-r--r--   0 tstellar (101195) tstellar (101195)       32 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/config-map-discovery/main-config/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/config-map-discovery/tests/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/config-map-discovery/tests/test1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/config-map-discovery/tests/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/custom-result-category/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      467 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/custom-result-category/format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/custom-result-category/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/custom-result-category/test1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/custom-result-category/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      759 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/discovery/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/discovery/subdir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/discovery/subdir/lit.local.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/discovery/subdir/test-three.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/discovery/subsuite/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      174 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/discovery/subsuite/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/discovery/subsuite/test-one.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/discovery/subsuite/test-two.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/discovery/test-one.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/discovery/test-two.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/discovery/test.not-txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.635749 lit-16.0.6/tests/Inputs/exec-discovery/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      292 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/exec-discovery/lit.site.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/exec-discovery-in-tree/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      308 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/exec-discovery-in-tree/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/exec-discovery-in-tree/obj/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      205 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/exec-discovery-in-tree/obj/lit.site.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/exec-discovery-in-tree/test-one.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/fake-externals/
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/fake-externals/cd
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/fake-externals/diff
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/fake-externals/env
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/fake-externals/export
--rw-r--r--   0 tstellar (101195) tstellar (101195)      188 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/fake-externals/fake_external.py
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/fake-externals/mkdir
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/fake-externals/rm
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-cmd-wrapper/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-cmd-wrapper/DummySubDir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1267 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-cmd-wrapper/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-crash/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-crash/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1387 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-crash/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      119 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-crash/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-detect-duplicate/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-detect-duplicate/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1336 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      130 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-detect-duplicate/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-discovery-failed/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-discovery-failed/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-discovery-failed/subdir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       80 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/googletest-discovery-failed/subdir/OneTest.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-format/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-format/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2727 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-format/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-format/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2728 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.636749 lit-16.0.6/tests/Inputs/googletest-sanitizer-error/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.637749 lit-16.0.6/tests/Inputs/googletest-sanitizer-error/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1492 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      129 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-sanitizer-error/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.637749 lit-16.0.6/tests/Inputs/googletest-timeout/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.637749 lit-16.0.6/tests/Inputs/googletest-timeout/DummySubDir/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1671 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      396 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/googletest-timeout/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.637749 lit-16.0.6/tests/Inputs/ignore-fail/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/ignore-fail/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      176 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/ignore-fail/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/ignore-fail/unresolved.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/ignore-fail/xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/ignore-fail/xpass.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.637749 lit-16.0.6/tests/Inputs/lit-opts/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      245 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/lit-opts/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/lit-opts/test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.638749 lit-16.0.6/tests/Inputs/lld-features/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/ld.lld
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/ld.lld.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       31 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/ld.lld.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/ld64.lld
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/ld64.lld.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/ld64.lld.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      711 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/lld-features/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/lld-link
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/lld-link.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/lld-link.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/wasm-ld
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/wasm-ld.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/lld-features/wasm-ld.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.638749 lit-16.0.6/tests/Inputs/max-failures/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/max-failures/fail1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/max-failures/fail2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/max-failures/fail3.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/max-failures/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.638749 lit-16.0.6/tests/Inputs/max-time/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/max-time/fast.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      250 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/max-time/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/max-time/slow.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.638749 lit-16.0.6/tests/Inputs/parallelism-groups/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      473 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/parallelism-groups/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/parallelism-groups/test1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/parallelism-groups/test2.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.638749 lit-16.0.6/tests/Inputs/progress-bar/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/progress-bar/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/progress-bar/test-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/progress-bar/test-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/progress-bar/test-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/progress-bar/test-4.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.638749 lit-16.0.6/tests/Inputs/py-config-discovery/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      292 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/py-config-discovery/lit.site.cfg.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.639749 lit-16.0.6/tests/Inputs/reorder/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/reorder/aaa.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/reorder/bbb.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/reorder/fff.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      172 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/reorder/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       78 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/reorder/lit_test_times
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/reorder/new-test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.639749 lit-16.0.6/tests/Inputs/reorder/subdir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/reorder/subdir/ccc.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.639749 lit-16.0.6/tests/Inputs/show-result-codes/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-result-codes/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/show-result-codes/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-result-codes/pass.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       36 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-result-codes/unsupported.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-result-codes/xfail.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.639749 lit-16.0.6/tests/Inputs/show-used-features/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/show-used-features/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      267 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/show-used-features/mixed.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       35 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-used-features/requires.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       42 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-used-features/unsupported.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       30 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/show-used-features/xfail.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.640749 lit-16.0.6/tests/Inputs/shtest-define/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.640749 lit-16.0.6/tests/Inputs/shtest-define/errors/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.640749 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/before-name.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      259 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/between-name-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/braces-empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      507 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      244 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/braces-with-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/braces-with-newline.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      490 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/braces-with-ws.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      196 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/no-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/no-name.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      222 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/assignment/ws-only.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.641749 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      329 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/end-in-double-backslash.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      420 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-define-bad-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      289 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-define-continuation.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      427 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-define-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      229 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-define-run.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      254 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-bad-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-continuation.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-run.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      268 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-run-define.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/unterminated-run-redefine.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/continuation/ws-only.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.641749 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      319 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-already-by-config.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      318 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-already-by-test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      324 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-inside-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      409 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-multiple-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      436 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-multiple-once-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      333 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-prefixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      322 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/define-suffixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      399 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-inside-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      611 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      408 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-prefixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      397 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-suffixes-pattern.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/location-range.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/errors/no-run.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.642749 lit-16.0.6/tests/Inputs/shtest-define/examples/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1772 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/examples/param-subst.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1683 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/expansion-order.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1224 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/line-number-substitutions.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)     2663 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-define/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      662 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/name-chars.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      265 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/recursiveExpansionLimit.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/shared-substs-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/shared-substs-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      886 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/value-equals.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      509 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/value-escaped.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     3926 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-define/ws-and-continuations.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.642749 lit-16.0.6/tests/Inputs/shtest-env/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-args-last-is-assign.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-args-last-is-u-arg.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       14 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-args-last-is-u.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-args-nested-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-args-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-cd.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-colon.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-echo.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      875 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-env.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-export.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-mkdir.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      198 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-not-builtin.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-calls-rm.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      687 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env-u.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      465 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/env.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      309 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-env/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-env/mixed.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      185 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-env/print_environment.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.643749 lit-16.0.6/tests/Inputs/shtest-format/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.644749 lit-16.0.6/tests/Inputs/shtest-format/external_shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/fail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      107 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/fail_with_bad_encoding.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      191 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/fail_with_control_chars.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       82 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/lit.local.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/pass.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/utf8_command.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      138 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/write-bad-encoding.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      146 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/external_shell/write-control-chars.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      104 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/fail.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      413 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-format/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/no-test-line.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/pass.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/requires-missing.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      122 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/requires-present.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       49 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/requires-star.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      114 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-format/requires-triple.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      218 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/unsupported-expr-false.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      174 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-format/unsupported-expr-true.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       52 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/unsupported-star.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.644749 lit-16.0.6/tests/Inputs/shtest-format/unsupported_dir/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/unsupported_dir/lit.local.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/unsupported_dir/some-test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      147 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-format/xfail-expr-false.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      151 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-format/xfail-expr-true.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       40 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/xfail-feature.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-format/xfail-target.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format/xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-format/xpass.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.643749 lit-16.0.6/tests/Inputs/shtest-format-argv0/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      320 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-format-argv0/argv0.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      232 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-format-argv0/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.644749 lit-16.0.6/tests/Inputs/shtest-if-else/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-if-else/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       93 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-if-else/test-neg1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-if-else/test-neg2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-if-else/test-neg3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-if-else/test-neg4.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     3294 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-if-else/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.644749 lit-16.0.6/tests/Inputs/shtest-inject/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      276 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-inject/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      109 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-inject/test-empty.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      183 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-inject/test-many.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-inject/test-one.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.644749 lit-16.0.6/tests/Inputs/shtest-keyword-parse-errors/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-keyword-parse-errors/empty.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      132 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-keyword-parse-errors/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       44 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-keyword-parse-errors/multiple-allow-retries.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       29 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-keyword-parse-errors/unterminated-run.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.645749 lit-16.0.6/tests/Inputs/shtest-not/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/shtest-not/exclamation-args-nested-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/shtest-not/exclamation-args-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      211 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/shtest-not/exclamation-calls-external.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/fail.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/shtest-not/fail2.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      245 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-not/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-args-last-is-crash.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-args-nested-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-args-none.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       85 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-cd.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-colon.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      252 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-diff-with-crash.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      413 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-diff.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-echo.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-env-builtin.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       97 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-export.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1933 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-external.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      142 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-fail2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       59 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-mkdir.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       46 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/not-calls-rm.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-not/pass.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      158 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-not/print_environment.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-output-printing/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-output-printing/basic.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      149 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-output-printing/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-pushd-popd/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      144 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-pushd-popd/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-pushd-popd/popd-args.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-pushd-popd/popd-no-stack.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-pushd-popd/pushd-popd-ok.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       16 2023-03-31 08:26:53.000000 lit-16.0.6/tests/Inputs/shtest-pushd-popd/pushd-too-many-args.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.630749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      364 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      404 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/escaping/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      271 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/escaping/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       28 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/escaping/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/negative-integer/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      217 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/negative-integer/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/negative-integer/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/not-an-integer/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      229 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/not-an-integer/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/not-an-integer/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/set-to-none/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      214 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/set-to-none/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/set-to-none/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.646749 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      396 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.647749 lit-16.0.6/tests/Inputs/shtest-run-at-line/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.647749 lit-16.0.6/tests/Inputs/shtest-run-at-line/external-shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      125 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/external-shell/basic.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/external-shell/line-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       82 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/external-shell/lit.local.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.647749 lit-16.0.6/tests/Inputs/shtest-run-at-line/internal-shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/internal-shell/basic.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      221 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/internal-shell/line-continuation.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/internal-shell/lit.local.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)       62 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-run-at-line/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/shtest-shell/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       75 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/cat-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/cat-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      269 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/cat_nonprinting.bin
--rw-r--r--   0 tstellar (101195) tstellar (101195)      276 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-shell/check_args.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      623 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-shell/check_path.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/colon-error.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      373 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/shtest-shell/continuations.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      513 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/dev-null.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-b.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      622 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-encodings.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-error-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      141 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-error-4.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-error-5.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-error-6.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-in.bin
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       55 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-in.dos
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       50 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-in.unix
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-in.utf16
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-in.utf8
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      734 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-pipes.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      274 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      346 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      251 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-4.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      282 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-5.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      271 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-6.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-7.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r-error-8.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      675 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-r.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      358 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-strip-trailing-cr.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      976 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-unified.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/diff-w.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       71 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/error-2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      247 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-shell/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/mkdir-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/mkdir-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       74 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/mkdir-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1215 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/redirects.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/rm-error-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/rm-error-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/rm-error-2.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      120 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/rm-error-3.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/rm-unicode-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      738 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/sequencing-0.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/sequencing-1.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      157 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/stdout-encoding.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     7169 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/valid-shell.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/write-to-stderr.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      153 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-shell/write-to-stdout-and-stderr.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/shtest-timeout/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-timeout/infinite_loop.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1217 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/shtest-timeout/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       82 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/shtest-timeout/short.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/standalone-tests/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/standalone-tests/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/standalone-tests/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/standalone-tests-with-excludes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/standalone-tests-with-excludes/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/standalone-tests-with-excludes/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/standalone-tests-with-suffixes/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      152 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/standalone-tests-with-suffixes/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/standalone-tests-with-suffixes/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/test-data/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1203 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/test-data/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      265 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/test-data/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/test-data/metrics.ini
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/test-data-micro/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1935 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/test-data-micro/dummy_format.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      271 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/test-data-micro/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      220 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/test-data-micro/micro-tests.ini
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/test_retry_attempts/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      373 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/test_retry_attempts/lit.cfg
--rw-r--r--   0 tstellar (101195) tstellar (101195)      553 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/test_retry_attempts/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.650749 lit-16.0.6/tests/Inputs/testrunner-custom-parsers/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      374 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/testrunner-custom-parsers/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      387 2023-04-28 22:43:05.000000 lit-16.0.6/tests/Inputs/testrunner-custom-parsers/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.651749 lit-16.0.6/tests/Inputs/unittest-adaptor/
--rw-r--r--   0 tstellar (101195) tstellar (101195)      181 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/unittest-adaptor/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/unittest-adaptor/test-one.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/unittest-adaptor/test-two.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.651749 lit-16.0.6/tests/Inputs/unparsed-requirements/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/unparsed-requirements/test.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.651749 lit-16.0.6/tests/Inputs/use-llvm-tool/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.651749 lit-16.0.6/tests/Inputs/use-llvm-tool/build/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case10
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case10.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case2
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case2.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case3
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case3.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case6
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case6.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case7
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case7.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case9
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/build/case9.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/env-case1
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/env-case6
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1379 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/lit.cfg
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.652749 lit-16.0.6/tests/Inputs/use-llvm-tool/path/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case10
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case10.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case4
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case4.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case5
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case5.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case6
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case6.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case7
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/path/case7.exe
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.652749 lit-16.0.6/tests/Inputs/use-llvm-tool/search1/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/search1/empty
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.652749 lit-16.0.6/tests/Inputs/use-llvm-tool/search2/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/search2/case9
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/search2/case9.exe
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.652749 lit-16.0.6/tests/Inputs/use-llvm-tool/search3/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/search3/case9
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/search3/case9.exe
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.651749 lit-16.0.6/tests/Inputs/use-llvm-tool-required/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool-required/found
--rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool-required/found.exe
--rw-r--r--   0 tstellar (101195) tstellar (101195)      448 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/use-llvm-tool-required/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/use-llvm-tool-required/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.652749 lit-16.0.6/tests/Inputs/xfail-cl/
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.652749 lit-16.0.6/tests/Inputs/xfail-cl/a/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/a/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/xfail-cl/a/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/a/test-xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/a/test.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.653749 lit-16.0.6/tests/Inputs/xfail-cl/b/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/b/false.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      125 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/xfail-cl/b/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/b/test-xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/b/test.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/false.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/false2.txt
--rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/xfail-cl/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/true-xfail.txt
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-16.0.6/tests/Inputs/xfail-cl/true.txt
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.653749 lit-16.0.6/tests/Inputs/xunit-output/
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/xunit-output/bad&name.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)     1418 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/xunit-output/dummy_format.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       69 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/xunit-output/excluded.ini
--rw-r--r--   0 tstellar (101195) tstellar (101195)      265 2023-06-10 22:52:12.000000 lit-16.0.6/tests/Inputs/xunit-output/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/xunit-output/missing_feature.ini
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       65 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/xunit-output/pass.ini
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-16.0.6/tests/Inputs/xunit-output/unsupported.ini
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1954 2022-08-02 09:00:57.000000 lit-16.0.6/tests/allow-retries.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-16.0.6/tests/boolean-parsing.py
--rwxrwxr-x   0 tstellar (101195) tstellar (101195)      199 2022-08-02 09:00:57.000000 lit-16.0.6/tests/check-tested-lit-timeout-ability
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      484 2022-08-02 09:00:57.000000 lit-16.0.6/tests/custom-result-category.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     9427 2022-08-02 09:00:57.000000 lit-16.0.6/tests/discovery.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2023-03-31 08:26:53.000000 lit-16.0.6/tests/googletest-cmd-wrapper.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1009 2023-03-31 08:26:53.000000 lit-16.0.6/tests/googletest-crash.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      502 2023-04-28 22:43:05.000000 lit-16.0.6/tests/googletest-detect-duplicate.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      337 2022-08-02 09:00:57.000000 lit-16.0.6/tests/googletest-discovery-failed.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      800 2023-04-28 22:43:05.000000 lit-16.0.6/tests/googletest-format-respect-gtest-sharding-env-vars.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1432 2023-03-31 08:26:53.000000 lit-16.0.6/tests/googletest-format.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1234 2023-03-31 08:26:53.000000 lit-16.0.6/tests/googletest-sanitizer-error.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2561 2023-04-28 22:43:05.000000 lit-16.0.6/tests/googletest-timeout.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      640 2022-08-02 09:00:57.000000 lit-16.0.6/tests/ignore-fail.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1096 2022-08-02 09:00:57.000000 lit-16.0.6/tests/lit-opts.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)     5345 2023-06-10 22:52:12.000000 lit-16.0.6/tests/lit.cfg
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      410 2023-03-31 08:26:53.000000 lit-16.0.6/tests/lit.site.cfg.in
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-08-02 09:00:57.000000 lit-16.0.6/tests/lld-features.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      808 2022-08-02 09:00:57.000000 lit-16.0.6/tests/max-failures.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2022-05-20 05:53:51.000000 lit-16.0.6/tests/max-time.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      558 2022-05-20 05:53:51.000000 lit-16.0.6/tests/parallelism-groups.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      538 2022-08-02 09:00:57.000000 lit-16.0.6/tests/progress-bar.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      732 2023-04-28 22:43:05.000000 lit-16.0.6/tests/reorder.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     6440 2022-08-02 09:00:57.000000 lit-16.0.6/tests/selecting.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       67 2022-05-20 05:53:51.000000 lit-16.0.6/tests/shell-parsing.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      847 2022-05-20 05:53:51.000000 lit-16.0.6/tests/show-result-codes.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      512 2022-08-02 09:00:57.000000 lit-16.0.6/tests/show-used-features.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     6636 2023-04-28 22:43:05.000000 lit-16.0.6/tests/shtest-define.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-16.0.6/tests/shtest-encoding.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     4015 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-env.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      588 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-format-argv0.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     6916 2023-04-28 22:43:05.000000 lit-16.0.6/tests/shtest-format.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      699 2023-03-31 08:26:53.000000 lit-16.0.6/tests/shtest-if-else.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1228 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-inject.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      581 2023-04-28 22:43:05.000000 lit-16.0.6/tests/shtest-keyword-parse-errors.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     5363 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-not.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      979 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-output-printing.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      636 2023-03-31 08:26:53.000000 lit-16.0.6/tests/shtest-pushd-popd.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1615 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-recursive-substitution.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2221 2022-08-02 09:00:57.000000 lit-16.0.6/tests/shtest-run-at-line.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)    17367 2023-04-28 22:43:05.000000 lit-16.0.6/tests/shtest-shell.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     3498 2022-05-20 05:53:51.000000 lit-16.0.6/tests/shtest-timeout.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      679 2022-08-02 09:00:57.000000 lit-16.0.6/tests/test-data-micro.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      353 2022-08-02 09:00:57.000000 lit-16.0.6/tests/test-data.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2380 2022-08-02 09:00:57.000000 lit-16.0.6/tests/test-output-micro-resultdb.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1624 2023-04-28 22:43:05.000000 lit-16.0.6/tests/test-output-micro.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1546 2023-03-31 08:26:53.000000 lit-16.0.6/tests/test-output-resultdb.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      552 2023-04-28 22:43:05.000000 lit-16.0.6/tests/test-output.py
-drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-06-14 18:54:46.653749 lit-16.0.6/tests/unit/
--rw-r--r--   0 tstellar (101195) tstellar (101195)     4682 2023-06-10 22:52:12.000000 lit-16.0.6/tests/unit/ShUtil.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)    13750 2023-06-10 22:52:12.000000 lit-16.0.6/tests/unit/TestRunner.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      460 2022-05-20 05:53:51.000000 lit-16.0.6/tests/unittest-adaptor.py
--rw-r--r--   0 tstellar (101195) tstellar (101195)      765 2023-06-10 22:52:12.000000 lit-16.0.6/tests/unparsed-requirements.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2022-05-20 05:53:51.000000 lit-16.0.6/tests/usage.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     2077 2022-08-02 09:00:57.000000 lit-16.0.6/tests/use-llvm-tool.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1860 2022-08-02 09:00:57.000000 lit-16.0.6/tests/xfail-cl.py
--rw-rw-r--   0 tstellar (101195) tstellar (101195)     1486 2022-05-20 05:53:51.000000 lit-16.0.6/tests/xunit-output.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.786108 lit-17.0.0rc1/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    15141 2022-05-20 05:53:51.000000 lit-17.0.0rc1/LICENSE.TXT
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      242 2022-05-20 05:53:51.000000 lit-17.0.0rc1/MANIFEST.in
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2519 2023-07-29 14:13:58.786108 lit-17.0.0rc1/PKG-INFO
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1874 2023-05-13 06:19:19.000000 lit-17.0.0rc1/README.rst
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.763108 lit-17.0.0rc1/examples/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-17.0.0rc1/examples/README.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.763108 lit-17.0.0rc1/examples/many-tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      549 2023-07-06 03:21:05.000000 lit-17.0.0rc1/examples/many-tests/ManyTests.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      382 2022-05-20 05:53:51.000000 lit-17.0.0rc1/examples/many-tests/README.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      147 2023-07-06 00:01:13.000000 lit-17.0.0rc1/examples/many-tests/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.764108 lit-17.0.0rc1/lit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    12039 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/BooleanExpression.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     7871 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/LitConfig.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1593 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/LitTestCase.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    11087 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/ProgressBar.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     3242 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/ShCommands.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8811 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/ShUtil.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13734 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/Test.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    78657 2023-07-06 00:02:35.000000 lit-17.0.0rc1/lit/TestRunner.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1629 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/TestTimes.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     8659 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/TestingConfig.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      199 2023-07-29 14:11:55.000000 lit-17.0.0rc1/lit/__init__.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.764108 lit-17.0.0rc1/lit/builtin_commands/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/lit/builtin_commands/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1892 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/builtin_commands/cat.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9817 2023-07-06 00:02:35.000000 lit-17.0.0rc1/lit/builtin_commands/diff.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    10608 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/cl_arguments.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9564 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/discovery.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5987 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/display.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.765108 lit-17.0.0rc1/lit/formats/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2023-07-06 03:21:05.000000 lit-17.0.0rc1/lit/formats/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2299 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/formats/base.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13602 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/formats/googletest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      992 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/formats/shtest.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.765108 lit-17.0.0rc1/lit/llvm/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-05-20 05:53:51.000000 lit-17.0.0rc1/lit/llvm/__init__.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    31158 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/llvm/config.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5430 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/llvm/subst.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11652 2023-07-29 14:11:39.000000 lit-17.0.0rc1/lit/main.py
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)    11056 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/reports.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4692 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/run.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    15927 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/util.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2666 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit/worker.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.764108 lit-17.0.0rc1/lit.egg-info/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2519 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/PKG-INFO
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    21372 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/entry_points.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        1 2023-04-10 18:12:43.000000 lit-17.0.0rc1/lit.egg-info/not-zip-safe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        4 2023-07-29 14:13:58.000000 lit-17.0.0rc1/lit.egg-info/top_level.txt
+-rwxr-xr-x   0 tstellar (101195) tstellar (101195)       89 2023-07-06 00:01:13.000000 lit-17.0.0rc1/lit.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2023-04-28 22:43:05.000000 lit-17.0.0rc1/pyproject.toml
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       38 2023-07-29 14:13:58.786108 lit-17.0.0rc1/setup.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1295 2023-07-06 00:01:13.000000 lit-17.0.0rc1/setup.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      152 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/.coveragerc
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/Inputs/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/Inputs/allow-retries/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/does-not-succeed-within-limit.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      337 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       51 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/more-than-one-allow-retries-lines.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       45 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/not-a-valid-integer.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      573 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/allow-retries/succeeds-within-limit.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.767108 lit-17.0.0rc1/tests/Inputs/config-map-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      444 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/driver.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/invalid-test.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      281 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/lit.alt.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/config-map-discovery/main-config/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       33 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/main-config/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/config-map-discovery/tests/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/tests/test1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/config-map-discovery/tests/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/custom-result-category/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      467 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      247 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/test1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/custom-result-category/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      762 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/discovery/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery/subdir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      141 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/discovery/subdir/lit.local.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/subdir/test-three.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      175 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/test-one.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/subsuite/test-two.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/test-one.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/test-two.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/discovery/test.not-txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      538 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/custom_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      270 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)        0 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/Inputs/discovery-getTestsForPath/x.test
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/exec-discovery/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      292 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery/lit.site.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      308 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.768108 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/obj/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      205 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/obj/lit.site.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/exec-discovery-in-tree/test-one.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/fake-externals/
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/cd
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/diff
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/env
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/export
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      208 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/fake_external.py
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/mkdir
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/fake-externals/rm
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/DummySubDir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1267 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      189 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-crash/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-crash/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1424 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-crash/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      120 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-crash/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1350 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      131 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/subdir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       80 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/googletest-discovery-failed/subdir/OneTest.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2741 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2742 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.769108 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1506 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      130 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/googletest-timeout/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/googletest-timeout/DummySubDir/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1685 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      397 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/googletest-timeout/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/ignore-fail/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      177 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/unresolved.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/ignore-fail/xpass.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/lit-opts/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/lit-opts/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/lit-opts/test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.770108 lit-17.0.0rc1/tests/Inputs/lld-features/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld.lld
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld.lld.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       31 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld.lld.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld64.lld
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld64.lld.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/ld64.lld.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      714 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lld-link
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lld-link.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       33 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/lld-link.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/wasm-ld
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/wasm-ld.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/lld-features/wasm-ld.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/max-failures/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-failures/fail1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-failures/fail2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-failures/fail3.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/max-failures/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/max-time/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-time/fast.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      251 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/max-time/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/max-time/slow.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/parallelism-groups/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      474 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/parallelism-groups/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/parallelism-groups/test1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/parallelism-groups/test2.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/progress-bar/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      178 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/progress-bar/test-4.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/py-config-discovery/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      299 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/py-config-discovery/lit.site.cfg.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/reorder/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/aaa.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/bbb.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/reorder/fff.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      173 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/reorder/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       78 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/reorder/lit_test_times
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/new-test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.771108 lit-17.0.0rc1/tests/Inputs/reorder/subdir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/reorder/subdir/ccc.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/show-result-codes/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      183 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       10 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/pass.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       36 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/unsupported.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-result-codes/xfail.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/show-used-features/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      184 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      267 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/mixed.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       35 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/requires.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       42 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/unsupported.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       30 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/show-used-features/xfail.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/shtest-define/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.772108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.773108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/before-name.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      259 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/between-name-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      507 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-dot.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      244 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-newline.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      490 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-number.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/braces-with-ws.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      196 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/no-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      185 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/no-name.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      222 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/assignment/ws-only.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.774108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      329 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/end-in-double-backslash.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      420 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-bad-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      289 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-continuation.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      427 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      229 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define-run.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      254 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-bad-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-continuation.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      424 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine-run.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      268 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      216 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-run-define.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/unterminated-run-redefine.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      313 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/continuation/ws-only.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.774108 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      319 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-already-by-config.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      318 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-already-by-test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      324 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-inside-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      409 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-multiple-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      436 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-multiple-once-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      333 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-prefixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      322 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/define-suffixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      399 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-inside-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      611 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      408 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-prefixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      397 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-suffixes-pattern.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/location-range.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      186 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/errors/no-run.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.774108 lit-17.0.0rc1/tests/Inputs/shtest-define/examples/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1772 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/examples/param-subst.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1683 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/expansion-order.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1224 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/line-number-substitutions.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     2668 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      662 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/name-chars.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      265 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/recursiveExpansionLimit.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      700 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      886 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/value-equals.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      509 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/value-escaped.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     3926 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-define/ws-and-continuations.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.775108 lit-17.0.0rc1/tests/Inputs/shtest-env/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       17 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-last-is-assign.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-last-is-u-arg.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       14 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-last-is-u.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-nested-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-args-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-cd.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-colon.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-echo.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      875 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-env.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-export.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-mkdir.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      198 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-not-builtin.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       34 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-rm.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      687 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env-u.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      465 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/env.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      310 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      585 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/mixed.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      188 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-env/print_environment.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/fail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      107 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/fail_with_bad_encoding.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      191 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/fail_with_control_chars.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/lit.local.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/pass.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/utf8_command.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      138 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/write-bad-encoding.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      146 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/external_shell/write-control-chars.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      104 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/fail.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      414 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/no-test-line.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/pass.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-missing.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      122 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-present.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       49 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-star.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      114 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/requires-triple.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      218 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported-expr-false.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      174 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported-expr-true.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       52 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported-star.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported_dir/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported_dir/lit.local.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/unsupported_dir/some-test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      147 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-expr-false.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      151 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-expr-true.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       40 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-feature.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       38 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail-target.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       20 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-format/xpass.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.776108 lit-17.0.0rc1/tests/Inputs/shtest-format-argv0/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      320 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-format-argv0/argv0.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      233 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-format-argv0/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.777108 lit-17.0.0rc1/tests/Inputs/shtest-if-else/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      267 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       93 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test-neg4.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     3294 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-if-else/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.777108 lit-17.0.0rc1/tests/Inputs/shtest-inject/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      109 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/test-empty.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      183 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/test-many.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-inject/test-one.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.777108 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/empty.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      133 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       44 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/multiple-allow-retries.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       29 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-keyword-parse-errors/unterminated-run.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.778108 lit-17.0.0rc1/tests/Inputs/shtest-not/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/exclamation-args-nested-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        9 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/exclamation-args-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      211 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/exclamation-calls-external.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/fail.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      100 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/fail2.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      246 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-args-last-is-crash.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-args-nested-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-args-none.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       85 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-cd.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-colon.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      252 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-diff-with-crash.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      413 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-diff.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      103 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-echo.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      207 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-env-builtin.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       97 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-export.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1933 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-external.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      142 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-fail2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       59 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-mkdir.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       46 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-rm.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       77 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/pass.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      159 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-not/print_environment.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.778108 lit-17.0.0rc1/tests/Inputs/shtest-output-printing/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-output-printing/basic.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      150 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-output-printing/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.778108 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      145 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       19 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/popd-args.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       11 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/popd-no-stack.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      223 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/pushd-popd-ok.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       16 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/Inputs/shtest-pushd-popd/pushd-too-many-args.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.762108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      340 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-no-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/does-not-substitute-within-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/escaping/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/escaping/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       28 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/escaping/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/negative-integer/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      218 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/negative-integer/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/negative-integer/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/not-an-integer/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      230 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/not-an-integer/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/not-an-integer/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/set-to-none/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      215 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/set-to-none/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/set-to-none/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      372 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       18 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-recursive-substitution/substitutes-within-limit/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.779108 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      125 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/basic.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      253 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/line-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       83 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/external-shell/lit.local.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.780108 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       37 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/basic.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      221 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/line-continuation.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       84 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/internal-shell/lit.local.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)       62 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-run-at-line/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.782108 lit-17.0.0rc1/tests/Inputs/shtest-shell/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       75 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/cat-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       87 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/cat-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      269 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/cat_nonprinting.bin
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/check_args.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      622 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/check_path.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/colon-error.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      373 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/continuations.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      513 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/dev-null.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      274 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-I.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      181 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-b.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      622 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-encodings.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       81 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      141 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-4.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-5.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-error-6.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       26 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.bin
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       55 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.dos
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       50 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.unix
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.utf16
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-in.utf8
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      734 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-pipes.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      274 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      346 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      251 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      273 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-4.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      282 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-5.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      271 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-6.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-7.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       61 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r-error-8.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      675 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      358 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-strip-trailing-cr.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      976 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-unified.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      236 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-w.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       71 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       68 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/error-2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      248 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/mkdir-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/mkdir-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       74 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/mkdir-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1215 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/redirects.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      102 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       92 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      128 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-2.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      120 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-error-3.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      204 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/rm-unicode-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      738 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/sequencing-0.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       32 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/sequencing-1.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      157 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/stdout-encoding.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     7169 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/valid-shell.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/write-to-stderr.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      153 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-shell/write-to-stdout-and-stderr.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.782108 lit-17.0.0rc1/tests/Inputs/shtest-timeout/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       41 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-timeout/infinite_loop.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1217 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/shtest-timeout/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       82 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/shtest-timeout/short.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.782108 lit-17.0.0rc1/tests/Inputs/standalone-tests/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-excludes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      154 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-excludes/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-excludes/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-suffixes/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      153 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-suffixes/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/standalone-tests-with-suffixes/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/test-data/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1172 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       94 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/test-data/metrics.ini
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/test-data-micro/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1907 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data-micro/dummy_format.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      272 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test-data-micro/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      220 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/test-data-micro/micro-tests.ini
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/test_retry_attempts/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      374 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test_retry_attempts/lit.cfg
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      553 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/test_retry_attempts/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/testrunner-custom-parsers/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      380 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/testrunner-custom-parsers/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      387 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/Inputs/testrunner-custom-parsers/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      182 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/test-one.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/unittest-adaptor/test-two.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.783108 lit-17.0.0rc1/tests/Inputs/unparsed-requirements/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       76 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/unparsed-requirements/test.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.784108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.784108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case10
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case10.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case2
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case2.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case3
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case3.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case6
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case6.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case7
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case7.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case9
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/build/case9.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/env-case1
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/env-case6
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1403 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/lit.cfg
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case10
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case10.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case4
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case4.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case5
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case5.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case6
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case6.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case7
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/path/case7.exe
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search1/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search1/empty
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search2/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search2/case9
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search2/case9.exe
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search3/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search3/case9
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/search3/case9.exe
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.784108 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/found
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)        0 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/found.exe
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      451 2023-07-06 00:02:35.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/use-llvm-tool-required/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/xfail-cl/
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/test-xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/a/test.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.785108 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/false.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      126 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       24 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/test-xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/b/test.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/false.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       13 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/false2.txt
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      121 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       23 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/true-xfail.txt
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       12 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/Inputs/xfail-cl/true.txt
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.786108 lit-17.0.0rc1/tests/Inputs/xunit-output/
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       95 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/bad&name.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1387 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/dummy_format.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       69 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/excluded.ini
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      266 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      106 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/missing_feature.ini
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       65 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/pass.ini
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/Inputs/xunit-output/unsupported.ini
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1954 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/allow-retries.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      126 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/boolean-parsing.py
+-rwxrwxr-x   0 tstellar (101195) tstellar (101195)      199 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/check-tested-lit-timeout-ability
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      484 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/custom-result-category.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     9769 2023-07-29 14:11:39.000000 lit-17.0.0rc1/tests/discovery.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      246 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-cmd-wrapper.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1009 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-crash.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      502 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/googletest-detect-duplicate.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      337 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/googletest-discovery-failed.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      800 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/googletest-format-respect-gtest-sharding-env-vars.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1432 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-format.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1234 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/googletest-sanitizer-error.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2561 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/googletest-timeout.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      640 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/ignore-fail.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1096 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/lit-opts.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     5298 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/lit.cfg
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      410 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/lit.site.cfg.in
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      176 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/lld-features.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     1001 2023-07-06 03:21:05.000000 lit-17.0.0rc1/tests/max-failures.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      234 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/max-time.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      558 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/parallelism-groups.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      538 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/progress-bar.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      732 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/reorder.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     6440 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/selecting.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       67 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/shell-parsing.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      847 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/show-result-codes.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      512 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/show-used-features.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     6636 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-define.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)       72 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/shtest-encoding.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     4015 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-env.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      588 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-format-argv0.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     6916 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-format.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      699 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/shtest-if-else.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1228 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-inject.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      581 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-keyword-parse-errors.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     5363 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-not.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      979 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-output-printing.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      636 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/shtest-pushd-popd.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1615 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-recursive-substitution.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2221 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/shtest-run-at-line.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)    17367 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/shtest-shell.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     3498 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/shtest-timeout.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      679 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/test-data-micro.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      353 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/test-data.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2380 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/test-output-micro-resultdb.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1624 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/test-output-micro.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1546 2023-03-31 08:26:53.000000 lit-17.0.0rc1/tests/test-output-resultdb.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      552 2023-04-28 22:43:05.000000 lit-17.0.0rc1/tests/test-output.py
+drwxr-xr-x   0 tstellar (101195) tstellar (101195)        0 2023-07-29 14:13:58.786108 lit-17.0.0rc1/tests/unit/
+-rw-r--r--   0 tstellar (101195) tstellar (101195)     4360 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/unit/ShUtil.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)    13421 2023-07-29 14:11:39.000000 lit-17.0.0rc1/tests/unit/TestRunner.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      460 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/unittest-adaptor.py
+-rw-r--r--   0 tstellar (101195) tstellar (101195)      816 2023-07-06 00:01:13.000000 lit-17.0.0rc1/tests/unparsed-requirements.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)      272 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/usage.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     2077 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/use-llvm-tool.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1860 2022-08-02 09:00:57.000000 lit-17.0.0rc1/tests/xfail-cl.py
+-rw-rw-r--   0 tstellar (101195) tstellar (101195)     1486 2022-05-20 05:53:51.000000 lit-17.0.0rc1/tests/xunit-output.py
```

### Comparing `lit-16.0.6/LICENSE.TXT` & `lit-17.0.0rc1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/PKG-INFO` & `lit-17.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit
-Version: 16.0.6
+Version: 17.0.0rc1
 Summary: A Software Testing Tool
 Home-page: http://llvm.org
 Author: Daniel Dunbar
 Author-email: daniel@minormatter.com
 License: Apache-2.0 with LLVM exception
 Keywords: test C++ automatic discovery
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lit-16.0.6/README.rst` & `lit-17.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/examples/many-tests/ManyTests.py` & `lit-17.0.0rc1/examples/many-tests/ManyTests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from lit import Test
+from lit import Test, TestFormat
 
 
-class ManyTests(object):
+class ManyTests(TestFormat):
     def __init__(self, N=10000):
         self.N = N
 
     def getTestsInDirectory(self, testSuite, path_in_suite, litConfig, localConfig):
         for i in range(self.N):
             test_name = "test-%04d" % (i,)
             yield Test.Test(testSuite, path_in_suite + (test_name,), localConfig)
```

### Comparing `lit-16.0.6/lit/BooleanExpression.py` & `lit-17.0.0rc1/lit/BooleanExpression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+
 class BooleanExpression:
     # A simple evaluator of boolean expressions.
     #
     # Grammar:
     #   expr         :: or_expr
     #   or_expr      :: and_expr ('||' and_expr)*
     #   and_expr     :: not_expr ('&&' not_expr)*
@@ -26,49 +27,51 @@
     # All other identifiers are false.
     @staticmethod
     def evaluate(string, variables):
         try:
             parser = BooleanExpression(string, set(variables))
             return parser.parseAll()
         except ValueError as e:
-            raise ValueError(str(e) + ('\nin expression: %r' % string))
+            raise ValueError(str(e) + ("\nin expression: %r" % string))
 
     #####
 
     def __init__(self, string, variables):
         self.tokens = BooleanExpression.tokenize(string)
         self.variables = variables
-        self.variables.add('true')
+        self.variables.add("true")
         self.value = None
         self.token = None
 
     # Singleton end-of-expression marker.
     END = object()
 
     # Tokenization pattern.
-    Pattern = re.compile(r'\A\s*([()]|&&|\|\||!|(?:[-+=._a-zA-Z0-9]+|\{\{.+?\}\})+)\s*(.*)\Z')
+    Pattern = re.compile(
+        r"\A\s*([()]|&&|\|\||!|(?:[-+=._a-zA-Z0-9]+|\{\{.+?\}\})+)\s*(.*)\Z"
+    )
 
     @staticmethod
     def tokenize(string):
         while True:
             m = re.match(BooleanExpression.Pattern, string)
             if m is None:
                 if string == "":
-                    yield BooleanExpression.END;
+                    yield BooleanExpression.END
                     return
                 else:
                     raise ValueError("couldn't parse text: %r" % string)
 
             token = m.group(1)
             string = m.group(2)
             yield token
 
     def quote(self, token):
         if token is BooleanExpression.END:
-            return '<end of expression>'
+            return "<end of expression>"
         else:
             return repr(token)
 
     def accept(self, t):
         if self.token == t:
             self.token = next(self.tokens)
             return True
@@ -76,62 +79,71 @@
             return False
 
     def expect(self, t):
         if self.token == t:
             if self.token != BooleanExpression.END:
                 self.token = next(self.tokens)
         else:
-            raise ValueError("expected: %s\nhave: %s" %
-                             (self.quote(t), self.quote(self.token)))
+            raise ValueError(
+                "expected: %s\nhave: %s" % (self.quote(t), self.quote(self.token))
+            )
 
     @staticmethod
     def isMatchExpression(token):
-        if (token is BooleanExpression.END or token == '&&' or token == '||' or
-            token == '!' or token == '(' or token == ')'):
+        if (
+            token is BooleanExpression.END
+            or token == "&&"
+            or token == "||"
+            or token == "!"
+            or token == "("
+            or token == ")"
+        ):
             return False
         return True
 
     def parseMATCH(self):
-        regex = ''
-        for part in filter(None, re.split(r'(\{\{.+?\}\})', self.token)):
-            if part.startswith('{{'):
-                assert part.endswith('}}')
-                regex += '(?:{})'.format(part[2:-2])
+        regex = ""
+        for part in filter(None, re.split(r"(\{\{.+?\}\})", self.token)):
+            if part.startswith("{{"):
+                assert part.endswith("}}")
+                regex += "(?:{})".format(part[2:-2])
             else:
                 regex += re.escape(part)
         regex = re.compile(regex)
         self.value = any(regex.fullmatch(var) for var in self.variables)
         self.token = next(self.tokens)
 
     def parseNOT(self):
-        if self.accept('!'):
+        if self.accept("!"):
             self.parseNOT()
             self.value = not self.value
-        elif self.accept('('):
+        elif self.accept("("):
             self.parseOR()
-            self.expect(')')
+            self.expect(")")
         elif not BooleanExpression.isMatchExpression(self.token):
-            raise ValueError("expected: '!', '(', '{{', or identifier\nhave: %s" %
-                             self.quote(self.token))
+            raise ValueError(
+                "expected: '!', '(', '{{', or identifier\nhave: %s"
+                % self.quote(self.token)
+            )
         else:
             self.parseMATCH()
 
     def parseAND(self):
         self.parseNOT()
-        while self.accept('&&'):
+        while self.accept("&&"):
             left = self.value
             self.parseNOT()
             right = self.value
             # this is technically the wrong associativity, but it
             # doesn't matter for this limited expression grammar
             self.value = left and right
 
     def parseOR(self):
         self.parseAND()
-        while self.accept('||'):
+        while self.accept("||"):
             left = self.value
             self.parseAND()
             right = self.value
             # this is technically the wrong associativity, but it
             # doesn't matter for this limited expression grammar
             self.value = left or right
 
@@ -143,142 +155,196 @@
 
 
 #######
 # Tests
 
 import unittest
 
+
 class TestBooleanExpression(unittest.TestCase):
     def test_variables(self):
-        variables = {'its-true', 'false-lol-true', 'under_score',
-                     'e=quals', 'd1g1ts'}
-        self.assertTrue(BooleanExpression.evaluate('true', variables))
-        self.assertTrue(BooleanExpression.evaluate('its-true', variables))
-        self.assertTrue(BooleanExpression.evaluate('false-lol-true', variables))
-        self.assertTrue(BooleanExpression.evaluate('under_score', variables))
-        self.assertTrue(BooleanExpression.evaluate('e=quals', variables))
-        self.assertTrue(BooleanExpression.evaluate('d1g1ts', variables))
-        self.assertTrue(BooleanExpression.evaluate('{{its.+}}', variables))
-        self.assertTrue(BooleanExpression.evaluate('{{false-[lo]+-true}}', variables))
-        self.assertTrue(BooleanExpression.evaluate('{{(true|false)-lol-(true|false)}}', variables))
-        self.assertTrue(BooleanExpression.evaluate('d1g{{[0-9]}}ts', variables))
-        self.assertTrue(BooleanExpression.evaluate('d1g{{[0-9]}}t{{[a-z]}}', variables))
-        self.assertTrue(BooleanExpression.evaluate('{{d}}1g{{[0-9]}}t{{[a-z]}}', variables))
-        self.assertTrue(BooleanExpression.evaluate('d1{{(g|1)+}}ts', variables))
-
-        self.assertFalse(BooleanExpression.evaluate('false', variables))
-        self.assertFalse(BooleanExpression.evaluate('True', variables))
-        self.assertFalse(BooleanExpression.evaluate('true-ish', variables))
-        self.assertFalse(BooleanExpression.evaluate('not_true', variables))
-        self.assertFalse(BooleanExpression.evaluate('tru', variables))
-        self.assertFalse(BooleanExpression.evaluate('{{its-true.+}}', variables))
+        variables = {"its-true", "false-lol-true", "under_score", "e=quals", "d1g1ts"}
+        self.assertTrue(BooleanExpression.evaluate("true", variables))
+        self.assertTrue(BooleanExpression.evaluate("its-true", variables))
+        self.assertTrue(BooleanExpression.evaluate("false-lol-true", variables))
+        self.assertTrue(BooleanExpression.evaluate("under_score", variables))
+        self.assertTrue(BooleanExpression.evaluate("e=quals", variables))
+        self.assertTrue(BooleanExpression.evaluate("d1g1ts", variables))
+        self.assertTrue(BooleanExpression.evaluate("{{its.+}}", variables))
+        self.assertTrue(BooleanExpression.evaluate("{{false-[lo]+-true}}", variables))
+        self.assertTrue(
+            BooleanExpression.evaluate("{{(true|false)-lol-(true|false)}}", variables)
+        )
+        self.assertTrue(BooleanExpression.evaluate("d1g{{[0-9]}}ts", variables))
+        self.assertTrue(BooleanExpression.evaluate("d1g{{[0-9]}}t{{[a-z]}}", variables))
+        self.assertTrue(
+            BooleanExpression.evaluate("{{d}}1g{{[0-9]}}t{{[a-z]}}", variables)
+        )
+        self.assertTrue(BooleanExpression.evaluate("d1{{(g|1)+}}ts", variables))
+
+        self.assertFalse(BooleanExpression.evaluate("false", variables))
+        self.assertFalse(BooleanExpression.evaluate("True", variables))
+        self.assertFalse(BooleanExpression.evaluate("true-ish", variables))
+        self.assertFalse(BooleanExpression.evaluate("not_true", variables))
+        self.assertFalse(BooleanExpression.evaluate("tru", variables))
+        self.assertFalse(BooleanExpression.evaluate("{{its-true.+}}", variables))
 
     def test_matching(self):
-        expr1 = 'linux && (target={{aarch64-.+}} || target={{x86_64-.+}})'
-        self.assertTrue(BooleanExpression.evaluate(expr1, {'linux', 'target=x86_64-unknown-linux-gnu'}))
-        self.assertFalse(BooleanExpression.evaluate(expr1, {'linux', 'target=i386-unknown-linux-gnu'}))
-
-        expr2 = 'use_system_cxx_lib && target={{.+}}-apple-macosx10.{{9|10|11|12}} && !no-exceptions'
-        self.assertTrue(BooleanExpression.evaluate(expr2, {'use_system_cxx_lib', 'target=arm64-apple-macosx10.12'}))
-        self.assertFalse(BooleanExpression.evaluate(expr2, {'use_system_cxx_lib', 'target=arm64-apple-macosx10.12', 'no-exceptions'}))
-        self.assertFalse(BooleanExpression.evaluate(expr2, {'use_system_cxx_lib', 'target=arm64-apple-macosx10.15'}))
+        expr1 = "linux && (target={{aarch64-.+}} || target={{x86_64-.+}})"
+        self.assertTrue(
+            BooleanExpression.evaluate(
+                expr1, {"linux", "target=x86_64-unknown-linux-gnu"}
+            )
+        )
+        self.assertFalse(
+            BooleanExpression.evaluate(
+                expr1, {"linux", "target=i386-unknown-linux-gnu"}
+            )
+        )
+
+        expr2 = "use_system_cxx_lib && target={{.+}}-apple-macosx10.{{9|10|11|12}} && !no-exceptions"
+        self.assertTrue(
+            BooleanExpression.evaluate(
+                expr2, {"use_system_cxx_lib", "target=arm64-apple-macosx10.12"}
+            )
+        )
+        self.assertFalse(
+            BooleanExpression.evaluate(
+                expr2,
+                {
+                    "use_system_cxx_lib",
+                    "target=arm64-apple-macosx10.12",
+                    "no-exceptions",
+                },
+            )
+        )
+        self.assertFalse(
+            BooleanExpression.evaluate(
+                expr2, {"use_system_cxx_lib", "target=arm64-apple-macosx10.15"}
+            )
+        )
 
     def test_operators(self):
-        self.assertTrue(BooleanExpression.evaluate('true || true', {}))
-        self.assertTrue(BooleanExpression.evaluate('true || false', {}))
-        self.assertTrue(BooleanExpression.evaluate('false || true', {}))
-        self.assertFalse(BooleanExpression.evaluate('false || false', {}))
-
-        self.assertTrue(BooleanExpression.evaluate('true && true', {}))
-        self.assertFalse(BooleanExpression.evaluate('true && false', {}))
-        self.assertFalse(BooleanExpression.evaluate('false && true', {}))
-        self.assertFalse(BooleanExpression.evaluate('false && false', {}))
-
-        self.assertFalse(BooleanExpression.evaluate('!true', {}))
-        self.assertTrue(BooleanExpression.evaluate('!false', {}))
-
-        self.assertTrue(BooleanExpression.evaluate('   ((!((false) ))   ) ', {}))
-        self.assertTrue(BooleanExpression.evaluate('true && (true && (true))', {}))
-        self.assertTrue(BooleanExpression.evaluate('!false && !false && !! !false', {}))
-        self.assertTrue(BooleanExpression.evaluate('false && false || true', {}))
-        self.assertTrue(BooleanExpression.evaluate('(false && false) || true', {}))
-        self.assertFalse(BooleanExpression.evaluate('false && (false || true)', {}))
+        self.assertTrue(BooleanExpression.evaluate("true || true", {}))
+        self.assertTrue(BooleanExpression.evaluate("true || false", {}))
+        self.assertTrue(BooleanExpression.evaluate("false || true", {}))
+        self.assertFalse(BooleanExpression.evaluate("false || false", {}))
+
+        self.assertTrue(BooleanExpression.evaluate("true && true", {}))
+        self.assertFalse(BooleanExpression.evaluate("true && false", {}))
+        self.assertFalse(BooleanExpression.evaluate("false && true", {}))
+        self.assertFalse(BooleanExpression.evaluate("false && false", {}))
+
+        self.assertFalse(BooleanExpression.evaluate("!true", {}))
+        self.assertTrue(BooleanExpression.evaluate("!false", {}))
+
+        self.assertTrue(BooleanExpression.evaluate("   ((!((false) ))   ) ", {}))
+        self.assertTrue(BooleanExpression.evaluate("true && (true && (true))", {}))
+        self.assertTrue(BooleanExpression.evaluate("!false && !false && !! !false", {}))
+        self.assertTrue(BooleanExpression.evaluate("false && false || true", {}))
+        self.assertTrue(BooleanExpression.evaluate("(false && false) || true", {}))
+        self.assertFalse(BooleanExpression.evaluate("false && (false || true)", {}))
 
     # Evaluate boolean expression `expr`.
     # Fail if it does not throw a ValueError containing the text `error`.
     def checkException(self, expr, error):
         try:
             BooleanExpression.evaluate(expr, {})
             self.fail("expression %r didn't cause an exception" % expr)
         except ValueError as e:
             if -1 == str(e).find(error):
-                self.fail(("expression %r caused the wrong ValueError\n" +
-                           "actual error was:\n%s\n" +
-                           "expected error was:\n%s\n") % (expr, e, error))
+                self.fail(
+                    (
+                        "expression %r caused the wrong ValueError\n"
+                        + "actual error was:\n%s\n"
+                        + "expected error was:\n%s\n"
+                    )
+                    % (expr, e, error)
+                )
         except BaseException as e:
-            self.fail(("expression %r caused the wrong exception; actual " +
-                      "exception was: \n%r") % (expr, e))
+            self.fail(
+                (
+                    "expression %r caused the wrong exception; actual "
+                    + "exception was: \n%r"
+                )
+                % (expr, e)
+            )
 
     def test_errors(self):
-        self.checkException("ba#d",
-                            "couldn't parse text: '#d'\n" +
-                            "in expression: 'ba#d'")
-
-        self.checkException("true and true",
-                            "expected: <end of expression>\n" +
-                            "have: 'and'\n" +
-                            "in expression: 'true and true'")
-
-        self.checkException("|| true",
-                            "expected: '!', '(', '{{', or identifier\n" +
-                            "have: '||'\n" +
-                            "in expression: '|| true'")
-
-        self.checkException("true &&",
-                            "expected: '!', '(', '{{', or identifier\n" +
-                            "have: <end of expression>\n" +
-                            "in expression: 'true &&'")
-
-        self.checkException("",
-                            "expected: '!', '(', '{{', or identifier\n" +
-                            "have: <end of expression>\n" +
-                            "in expression: ''")
-
-        self.checkException("*",
-                            "couldn't parse text: '*'\n" +
-                            "in expression: '*'")
-
-        self.checkException("no wait stop",
-                            "expected: <end of expression>\n" +
-                            "have: 'wait'\n" +
-                            "in expression: 'no wait stop'")
-
-        self.checkException("no-$-please",
-                            "couldn't parse text: '$-please'\n" +
-                            "in expression: 'no-$-please'")
-
-        self.checkException("(((true && true) || true)",
-                            "expected: ')'\n" +
-                            "have: <end of expression>\n" +
-                            "in expression: '(((true && true) || true)'")
-
-        self.checkException("true (true)",
-                            "expected: <end of expression>\n" +
-                            "have: '('\n" +
-                            "in expression: 'true (true)'")
-
-        self.checkException("( )",
-                            "expected: '!', '(', '{{', or identifier\n" +
-                            "have: ')'\n" +
-                            "in expression: '( )'")
-
-        self.checkException("abc{{def",
-                            "couldn't parse text: '{{def'\n" +
-                            "in expression: 'abc{{def'")
-
-        self.checkException("{{}}",
-                            "couldn't parse text: '{{}}'\n" +
-                            "in expression: '{{}}'")
+        self.checkException(
+            "ba#d", "couldn't parse text: '#d'\n" + "in expression: 'ba#d'"
+        )
+
+        self.checkException(
+            "true and true",
+            "expected: <end of expression>\n"
+            + "have: 'and'\n"
+            + "in expression: 'true and true'",
+        )
+
+        self.checkException(
+            "|| true",
+            "expected: '!', '(', '{{', or identifier\n"
+            + "have: '||'\n"
+            + "in expression: '|| true'",
+        )
+
+        self.checkException(
+            "true &&",
+            "expected: '!', '(', '{{', or identifier\n"
+            + "have: <end of expression>\n"
+            + "in expression: 'true &&'",
+        )
+
+        self.checkException(
+            "",
+            "expected: '!', '(', '{{', or identifier\n"
+            + "have: <end of expression>\n"
+            + "in expression: ''",
+        )
+
+        self.checkException("*", "couldn't parse text: '*'\n" + "in expression: '*'")
+
+        self.checkException(
+            "no wait stop",
+            "expected: <end of expression>\n"
+            + "have: 'wait'\n"
+            + "in expression: 'no wait stop'",
+        )
+
+        self.checkException(
+            "no-$-please",
+            "couldn't parse text: '$-please'\n" + "in expression: 'no-$-please'",
+        )
+
+        self.checkException(
+            "(((true && true) || true)",
+            "expected: ')'\n"
+            + "have: <end of expression>\n"
+            + "in expression: '(((true && true) || true)'",
+        )
+
+        self.checkException(
+            "true (true)",
+            "expected: <end of expression>\n"
+            + "have: '('\n"
+            + "in expression: 'true (true)'",
+        )
+
+        self.checkException(
+            "( )",
+            "expected: '!', '(', '{{', or identifier\n"
+            + "have: ')'\n"
+            + "in expression: '( )'",
+        )
+
+        self.checkException(
+            "abc{{def", "couldn't parse text: '{{def'\n" + "in expression: 'abc{{def'"
+        )
+
+        self.checkException(
+            "{{}}", "couldn't parse text: '{{}}'\n" + "in expression: '{{}}'"
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `lit-16.0.6/lit/LitConfig.py` & `lit-17.0.0rc1/lit/LitConfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,21 +16,32 @@
 
     The LitConfig object is also used to communicate with client configuration
     files, it is always passed in as the global variable 'lit' so that
     configuration files can access common functionality and internal components
     easily.
     """
 
-    def __init__(self, progname, path, quiet,
-                 useValgrind, valgrindLeakCheck, valgrindArgs,
-                 noExecute, debug, isWindows, order,
-                 params, config_prefix = None,
-                 maxIndividualTestTime = 0,
-                 parallelism_groups = {},
-                 echo_all_commands = False):
+    def __init__(
+        self,
+        progname,
+        path,
+        quiet,
+        useValgrind,
+        valgrindLeakCheck,
+        valgrindArgs,
+        noExecute,
+        debug,
+        isWindows,
+        order,
+        params,
+        config_prefix=None,
+        maxIndividualTestTime=0,
+        parallelism_groups={},
+        echo_all_commands=False,
+    ):
         # The name of the test runner.
         self.progname = progname
         # The items to add to the PATH environment variable.
         self.path = [str(p) for p in path]
         self.quiet = bool(quiet)
         self.useValgrind = bool(useValgrind)
         self.valgrindLeakCheck = bool(valgrindLeakCheck)
@@ -39,165 +50,179 @@
         self.debug = debug
         self.isWindows = bool(isWindows)
         self.order = order
         self.params = dict(params)
         self.bashPath = None
 
         # Configuration files to look for when discovering test suites.
-        self.config_prefix = config_prefix or 'lit'
-        self.suffixes = ['cfg.py', 'cfg']
-        self.config_names = ['%s.%s' % (self.config_prefix,x) for x in self.suffixes]
-        self.site_config_names = ['%s.site.%s' % (self.config_prefix,x) for x in self.suffixes]
-        self.local_config_names = ['%s.local.%s' % (self.config_prefix,x) for x in self.suffixes]
+        self.config_prefix = config_prefix or "lit"
+        self.suffixes = ["cfg.py", "cfg"]
+        self.config_names = ["%s.%s" % (self.config_prefix, x) for x in self.suffixes]
+        self.site_config_names = [
+            "%s.site.%s" % (self.config_prefix, x) for x in self.suffixes
+        ]
+        self.local_config_names = [
+            "%s.local.%s" % (self.config_prefix, x) for x in self.suffixes
+        ]
 
         self.numErrors = 0
         self.numWarnings = 0
 
         self.valgrindArgs = []
         if self.useValgrind:
-            self.valgrindArgs = ['valgrind', '-q', '--run-libc-freeres=no',
-                                 '--tool=memcheck', '--trace-children=yes',
-                                 '--error-exitcode=123']
+            self.valgrindArgs = [
+                "valgrind",
+                "-q",
+                "--run-libc-freeres=no",
+                "--tool=memcheck",
+                "--trace-children=yes",
+                "--error-exitcode=123",
+            ]
             if self.valgrindLeakCheck:
-                self.valgrindArgs.append('--leak-check=full')
+                self.valgrindArgs.append("--leak-check=full")
             else:
                 # The default is 'summary'.
-                self.valgrindArgs.append('--leak-check=no')
+                self.valgrindArgs.append("--leak-check=no")
             self.valgrindArgs.extend(self.valgrindUserArgs)
 
         self.maxIndividualTestTime = maxIndividualTestTime
         self.parallelism_groups = parallelism_groups
         self.echo_all_commands = echo_all_commands
 
     @property
     def maxIndividualTestTime(self):
         """
-            Interface for getting maximum time to spend executing
-            a single test
+        Interface for getting maximum time to spend executing
+        a single test
         """
         return self._maxIndividualTestTime
 
     @property
     def maxIndividualTestTimeIsSupported(self):
         """
-            Returns a tuple (<supported> , <error message>)
-            where
-            `<supported>` is True if setting maxIndividualTestTime is supported
-                on the current host, returns False otherwise.
-            `<error message>` is an empty string if `<supported>` is True,
-                otherwise is contains a string describing why setting
-                maxIndividualTestTime is not supported.
+        Returns a tuple (<supported> , <error message>)
+        where
+        `<supported>` is True if setting maxIndividualTestTime is supported
+            on the current host, returns False otherwise.
+        `<error message>` is an empty string if `<supported>` is True,
+            otherwise is contains a string describing why setting
+            maxIndividualTestTime is not supported.
         """
         return lit.util.killProcessAndChildrenIsSupported()
 
     @maxIndividualTestTime.setter
     def maxIndividualTestTime(self, value):
         """
-            Interface for setting maximum time to spend executing
-            a single test
+        Interface for setting maximum time to spend executing
+        a single test
         """
         if not isinstance(value, int):
-            self.fatal('maxIndividualTestTime must set to a value of type int.')
+            self.fatal("maxIndividualTestTime must set to a value of type int.")
         self._maxIndividualTestTime = value
         if self.maxIndividualTestTime > 0:
             # The current implementation needs psutil on some platforms to set
             # a timeout per test. Check it's available.
             # See lit.util.killProcessAndChildren()
             supported, errormsg = self.maxIndividualTestTimeIsSupported
             if not supported:
-                self.fatal('Setting a timeout per test not supported. ' +
-                           errormsg)
+                self.fatal("Setting a timeout per test not supported. " + errormsg)
         elif self.maxIndividualTestTime < 0:
-            self.fatal('The timeout per test must be >= 0 seconds')
+            self.fatal("The timeout per test must be >= 0 seconds")
 
     def load_config(self, config, path):
         """load_config(config, path) - Load a config object from an alternate
         path."""
         if self.debug:
-            self.note('load_config from %r' % path)
+            self.note("load_config from %r" % path)
         config.load_from_path(path, self)
         return config
 
     def getBashPath(self):
         """getBashPath - Get the path to 'bash'"""
         if self.bashPath is not None:
             return self.bashPath
 
-        self.bashPath = lit.util.which('bash', os.pathsep.join(self.path))
+        self.bashPath = lit.util.which("bash", os.pathsep.join(self.path))
         if self.bashPath is None:
-            self.bashPath = lit.util.which('bash')
+            self.bashPath = lit.util.which("bash")
 
         if self.bashPath is None:
-            self.bashPath = ''
+            self.bashPath = ""
 
         # Check whether the found version of bash is able to cope with paths in
         # the host path format. If not, don't return it as it can't be used to
         # run scripts. For example, WSL's bash.exe requires '/mnt/c/foo' rather
         # than 'C:\\foo' or 'C:/foo'.
         if self.isWindows and self.bashPath:
-            command = [self.bashPath, '-c',
-                       '[[ -f "%s" ]]' % self.bashPath.replace('\\', '\\\\')]
+            command = [
+                self.bashPath,
+                "-c",
+                '[[ -f "%s" ]]' % self.bashPath.replace("\\", "\\\\"),
+            ]
             _, _, exitCode = lit.util.executeCommand(command)
             if exitCode:
-                self.note('bash command failed: %s' % (
-                    ' '.join('"%s"' % c for c in command)))
-                self.bashPath = ''
+                self.note(
+                    "bash command failed: %s" % (" ".join('"%s"' % c for c in command))
+                )
+                self.bashPath = ""
 
         if not self.bashPath:
-            self.warning('Unable to find a usable version of bash.')
+            self.warning("Unable to find a usable version of bash.")
 
         return self.bashPath
 
     def getToolsPath(self, dir, paths, tools):
         if dir is not None and os.path.isabs(dir) and os.path.isdir(dir):
             if not lit.util.checkToolsPath(dir, tools):
                 return None
         else:
             dir = lit.util.whichTools(tools, paths)
 
         # bash
-        self.bashPath = lit.util.which('bash', dir)
+        self.bashPath = lit.util.which("bash", dir)
         if self.bashPath is None:
-            self.bashPath = ''
+            self.bashPath = ""
 
         return dir
 
     def _write_message(self, kind, message):
         # Get the file/line where this message was generated.
         f = inspect.currentframe()
         # Step out of _write_message, and then out of wrapper.
         f = f.f_back.f_back
         file = os.path.abspath(inspect.getsourcefile(f))
         line = inspect.getlineno(f)
-        sys.stderr.write('%s: %s:%d: %s: %s\n' % (self.progname, file, line,
-                                                  kind, message))
+        sys.stderr.write(
+            "%s: %s:%d: %s: %s\n" % (self.progname, file, line, kind, message)
+        )
         if self.isWindows:
             # In a git bash terminal, the writes to sys.stderr aren't visible
             # on screen immediately. Flush them here to avoid broken/misoredered
             # output.
             sys.stderr.flush()
 
     def substitute(self, string):
         """substitute - Interpolate params into a string"""
         try:
-          return string % self.params
+            return string % self.params
         except KeyError as e:
-          key, = e.args
-          self.fatal("unable to find %r parameter, use '--param=%s=VALUE'" % (
-              key,key))
+            (key,) = e.args
+            self.fatal(
+                "unable to find %r parameter, use '--param=%s=VALUE'" % (key, key)
+            )
 
     def note(self, message):
         if not self.quiet:
-            self._write_message('note', message)
+            self._write_message("note", message)
 
     def warning(self, message):
         if not self.quiet:
-            self._write_message('warning', message)
+            self._write_message("warning", message)
         self.numWarnings += 1
 
     def error(self, message):
-        self._write_message('error', message)
+        self._write_message("error", message)
         self.numErrors += 1
 
     def fatal(self, message):
-        self._write_message('fatal', message)
+        self._write_message("fatal", message)
         sys.exit(2)
```

### Comparing `lit-16.0.6/lit/LitTestCase.py` & `lit-17.0.0rc1/lit/LitTestCase.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,29 +35,31 @@
             raise UnresolvedError(result.output)
         elif result.code.isFailure:
             self.fail(result.output)
 
 
 def load_test_suite(inputs):
     import platform
-    windows = platform.system() == 'Windows'
+
+    windows = platform.system() == "Windows"
 
     # Create the global config object.
     lit_config = lit.LitConfig.LitConfig(
-        progname='lit',
+        progname="lit",
         path=[],
         quiet=False,
         useValgrind=False,
         valgrindLeakCheck=False,
         valgrindArgs=[],
         noExecute=False,
         debug=False,
         isWindows=windows,
-        order='smart',
-        params={})
+        order="smart",
+        params={},
+    )
 
     # Perform test discovery.
-    tests = lit.discovery.find_tests_for_inputs(lit_config, inputs, False)
+    tests = lit.discovery.find_tests_for_inputs(lit_config, inputs)
     test_adaptors = [LitTestCase(t, lit_config) for t in tests]
 
     # Return a unittest test suite which just runs the tests in order.
     return unittest.TestSuite(test_adaptors)
```

### Comparing `lit-16.0.6/lit/ProgressBar.py` & `lit-17.0.0rc1/lit/ProgressBar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python
 
 # Source: http://code.activestate.com/recipes/475116/, with
 # modifications by Daniel Dunbar.
 
 import sys, re, time
 
+
 def to_bytes(str):
     # Encode to UTF-8 to get binary data.
-    return str.encode('utf-8')
+    return str.encode("utf-8")
+
 
 class TerminalController:
     """
     A class that can be used to portably generate formatted output to
-    a terminal.  
-    
+    a terminal.
+
     `TerminalController` defines a set of instance variables whose
     values are initialized to the control sequence necessary to
     perform a given action.  These can be simply included in normal
     output to the terminal:
 
         >>> term = TerminalController()
         >>> print('This is '+term.GREEN+'green'+term.NORMAL)
@@ -39,49 +41,50 @@
         >>> term = TerminalController()
         >>> if term.CLEAR_SCREEN:
         ...     print('This terminal supports clearning the screen.')
 
     Finally, if the width and height of the terminal are known, then
     they will be stored in the `COLS` and `LINES` attributes.
     """
+
     # Cursor movement:
-    BOL = ''             #: Move the cursor to the beginning of the line
-    UP = ''              #: Move the cursor up one line
-    DOWN = ''            #: Move the cursor down one line
-    LEFT = ''            #: Move the cursor left one char
-    RIGHT = ''           #: Move the cursor right one char
+    BOL = ""  #: Move the cursor to the beginning of the line
+    UP = ""  #: Move the cursor up one line
+    DOWN = ""  #: Move the cursor down one line
+    LEFT = ""  #: Move the cursor left one char
+    RIGHT = ""  #: Move the cursor right one char
 
     # Deletion:
-    CLEAR_SCREEN = ''    #: Clear the screen and move to home position
-    CLEAR_EOL = ''       #: Clear to the end of the line.
-    CLEAR_BOL = ''       #: Clear to the beginning of the line.
-    CLEAR_EOS = ''       #: Clear to the end of the screen
+    CLEAR_SCREEN = ""  #: Clear the screen and move to home position
+    CLEAR_EOL = ""  #: Clear to the end of the line.
+    CLEAR_BOL = ""  #: Clear to the beginning of the line.
+    CLEAR_EOS = ""  #: Clear to the end of the screen
 
     # Output modes:
-    BOLD = ''            #: Turn on bold mode
-    BLINK = ''           #: Turn on blink mode
-    DIM = ''             #: Turn on half-bright mode
-    REVERSE = ''         #: Turn on reverse-video mode
-    NORMAL = ''          #: Turn off all modes
+    BOLD = ""  #: Turn on bold mode
+    BLINK = ""  #: Turn on blink mode
+    DIM = ""  #: Turn on half-bright mode
+    REVERSE = ""  #: Turn on reverse-video mode
+    NORMAL = ""  #: Turn off all modes
 
     # Cursor display:
-    HIDE_CURSOR = ''     #: Make the cursor invisible
-    SHOW_CURSOR = ''     #: Make the cursor visible
+    HIDE_CURSOR = ""  #: Make the cursor invisible
+    SHOW_CURSOR = ""  #: Make the cursor visible
 
     # Terminal size:
-    COLS = None          #: Width of the terminal (None for unknown)
-    LINES = None         #: Height of the terminal (None for unknown)
+    COLS = None  #: Width of the terminal (None for unknown)
+    LINES = None  #: Height of the terminal (None for unknown)
 
     # Foreground colors:
-    BLACK = BLUE = GREEN = CYAN = RED = MAGENTA = YELLOW = WHITE = ''
-    
+    BLACK = BLUE = GREEN = CYAN = RED = MAGENTA = YELLOW = WHITE = ""
+
     # Background colors:
-    BG_BLACK = BG_BLUE = BG_GREEN = BG_CYAN = ''
-    BG_RED = BG_MAGENTA = BG_YELLOW = BG_WHITE = ''
-    
+    BG_BLACK = BG_BLUE = BG_GREEN = BG_CYAN = ""
+    BG_RED = BG_MAGENTA = BG_YELLOW = BG_WHITE = ""
+
     _STRING_CAPABILITIES = """
     BOL=cr UP=cuu1 DOWN=cud1 LEFT=cub1 RIGHT=cuf1
     CLEAR_SCREEN=clear CLEAR_EOL=el CLEAR_BOL=el1 CLEAR_EOS=ed BOLD=bold
     BLINK=blink DIM=dim REVERSE=rev UNDERLINE=smul NORMAL=sgr0
     HIDE_CURSOR=cinvis SHOW_CURSOR=cnorm""".split()
     _COLORS = """BLACK BLUE GREEN CYAN RED MAGENTA YELLOW WHITE""".split()
     _ANSICOLORS = "BLACK RED GREEN YELLOW BLUE MAGENTA CYAN WHITE".split()
@@ -91,86 +94,97 @@
         Create a `TerminalController` and initialize its attributes
         with appropriate values for the current terminal.
         `term_stream` is the stream that will be used for terminal
         output; if this stream is not a tty, then the terminal is
         assumed to be a dumb terminal (i.e., have no capabilities).
         """
         # Curses isn't available on all platforms
-        try: import curses
-        except: return
+        try:
+            import curses
+        except:
+            return
 
         # If the stream isn't a tty, then assume it has no capabilities.
-        if not term_stream.isatty(): return
+        if not term_stream.isatty():
+            return
 
         # Check the terminal type.  If we fail, then assume that the
         # terminal has no capabilities.
-        try: curses.setupterm()
-        except: return
+        try:
+            curses.setupterm()
+        except:
+            return
 
         # Look up numeric capabilities.
-        self.COLS = curses.tigetnum('cols')
-        self.LINES = curses.tigetnum('lines')
-        self.XN = curses.tigetflag('xenl')
-        
+        self.COLS = curses.tigetnum("cols")
+        self.LINES = curses.tigetnum("lines")
+        self.XN = curses.tigetflag("xenl")
+
         # Look up string capabilities.
         for capability in self._STRING_CAPABILITIES:
-            (attrib, cap_name) = capability.split('=')
-            setattr(self, attrib, self._tigetstr(cap_name) or '')
+            (attrib, cap_name) = capability.split("=")
+            setattr(self, attrib, self._tigetstr(cap_name) or "")
 
         # Colors
-        set_fg = self._tigetstr('setf')
+        set_fg = self._tigetstr("setf")
         if set_fg:
-            for i,color in zip(range(len(self._COLORS)), self._COLORS):
+            for i, color in zip(range(len(self._COLORS)), self._COLORS):
                 setattr(self, color, self._tparm(set_fg, i))
-        set_fg_ansi = self._tigetstr('setaf')
+        set_fg_ansi = self._tigetstr("setaf")
         if set_fg_ansi:
-            for i,color in zip(range(len(self._ANSICOLORS)), self._ANSICOLORS):
+            for i, color in zip(range(len(self._ANSICOLORS)), self._ANSICOLORS):
                 setattr(self, color, self._tparm(set_fg_ansi, i))
-        set_bg = self._tigetstr('setb')
+        set_bg = self._tigetstr("setb")
         if set_bg:
-            for i,color in zip(range(len(self._COLORS)), self._COLORS):
-                setattr(self, 'BG_'+color, self._tparm(set_bg, i))
-        set_bg_ansi = self._tigetstr('setab')
+            for i, color in zip(range(len(self._COLORS)), self._COLORS):
+                setattr(self, "BG_" + color, self._tparm(set_bg, i))
+        set_bg_ansi = self._tigetstr("setab")
         if set_bg_ansi:
-            for i,color in zip(range(len(self._ANSICOLORS)), self._ANSICOLORS):
-                setattr(self, 'BG_'+color, self._tparm(set_bg_ansi, i))
+            for i, color in zip(range(len(self._ANSICOLORS)), self._ANSICOLORS):
+                setattr(self, "BG_" + color, self._tparm(set_bg_ansi, i))
 
     def _tparm(self, arg, index):
         import curses
-        return curses.tparm(to_bytes(arg), index).decode('utf-8') or ''
+
+        return curses.tparm(to_bytes(arg), index).decode("utf-8") or ""
 
     def _tigetstr(self, cap_name):
         # String capabilities can include "delays" of the form "$<2>".
         # For any modern terminal, we should be able to just ignore
         # these, so strip them out.
         import curses
+
         cap = curses.tigetstr(cap_name)
         if cap is None:
-            cap = ''
+            cap = ""
         else:
-            cap = cap.decode('utf-8')
-        return re.sub(r'\$<\d+>[/*]?', '', cap)
+            cap = cap.decode("utf-8")
+        return re.sub(r"\$<\d+>[/*]?", "", cap)
 
     def render(self, template):
         """
         Replace each $-substitutions in the given template string with
         the corresponding terminal control string (if it's defined) or
         '' (if it's not).
         """
-        return re.sub(r'\$\$|\${\w+}', self._render_sub, template)
+        return re.sub(r"\$\$|\${\w+}", self._render_sub, template)
 
     def _render_sub(self, match):
         s = match.group()
-        if s == '$$': return s
-        else: return getattr(self, s[2:-1])
+        if s == "$$":
+            return s
+        else:
+            return getattr(self, s[2:-1])
+
 
 #######################################################################
 # Example use case: progress bar
 #######################################################################
 
+
 class SimpleProgressBar:
     """
     A simple progress bar which doesn't need any terminal support.
 
     This prints out a progress bar like:
       'Header:  0.. 10.. 20.. ...'
     """
@@ -180,118 +194,133 @@
         self.atIndex = None
 
     def update(self, percent, message):
         if self.atIndex is None:
             sys.stdout.write(self.header)
             self.atIndex = 0
 
-        next = int(percent*50)
+        next = int(percent * 50)
         if next == self.atIndex:
             return
 
         for i in range(self.atIndex, next):
             idx = i % 5
             if idx == 0:
-                sys.stdout.write('%2d' % (i*2))
+                sys.stdout.write("%2d" % (i * 2))
             elif idx == 1:
-                pass # Skip second char
+                pass  # Skip second char
             elif idx < 4:
-                sys.stdout.write('.')
+                sys.stdout.write(".")
             else:
-                sys.stdout.write(' ')
+                sys.stdout.write(" ")
         sys.stdout.flush()
         self.atIndex = next
 
     def clear(self, interrupted):
         if self.atIndex is not None and not interrupted:
-            sys.stdout.write('\n')
+            sys.stdout.write("\n")
             sys.stdout.flush()
             self.atIndex = None
 
+
 class ProgressBar:
     """
     A 3-line progress bar, which looks like::
-    
+
                                 Header
         20% [===========----------------------------------]
                            progress message
 
     The progress bar is colored, if the terminal supports color
     output; and adjusts to the width of the terminal.
     """
-    BAR = '%s${%s}[${BOLD}%s%s${NORMAL}${%s}]${NORMAL}%s'
-    HEADER = '${BOLD}${CYAN}%s${NORMAL}\n\n'
-        
+
+    BAR = "%s${%s}[${BOLD}%s%s${NORMAL}${%s}]${NORMAL}%s"
+    HEADER = "${BOLD}${CYAN}%s${NORMAL}\n\n"
+
     def __init__(self, term, header, useETA=True):
         self.term = term
         if not (self.term.CLEAR_EOL and self.term.UP and self.term.BOL):
-            raise ValueError("Terminal isn't capable enough -- you "
-                             "should use a simpler progress dispaly.")
-        self.BOL = self.term.BOL # BoL from col#79
-        self.XNL = "\n" # Newline from col#79
+            raise ValueError(
+                "Terminal isn't capable enough -- you "
+                "should use a simpler progress dispaly."
+            )
+        self.BOL = self.term.BOL  # BoL from col#79
+        self.XNL = "\n"  # Newline from col#79
         if self.term.COLS:
             self.width = self.term.COLS
             if not self.term.XN:
                 self.BOL = self.term.UP + self.term.BOL
-                self.XNL = "" # Cursor must be fed to the next line
+                self.XNL = ""  # Cursor must be fed to the next line
         else:
             self.width = 75
-        self.barColor = 'GREEN'
+        self.barColor = "GREEN"
         self.header = self.term.render(self.HEADER % header.center(self.width))
-        self.cleared = 1 #: true if we haven't drawn the bar yet.
+        self.cleared = 1  #: true if we haven't drawn the bar yet.
         self.useETA = useETA
         if self.useETA:
             self.startTime = time.time()
         # self.update(0, '')
 
     def update(self, percent, message):
         if self.cleared:
             sys.stdout.write(self.header)
             self.cleared = 0
-        prefix = '%3d%% ' % (percent*100,)
-        suffix = ''
+        prefix = "%3d%% " % (percent * 100,)
+        suffix = ""
         if self.useETA:
             elapsed = time.time() - self.startTime
-            if percent > .0001 and elapsed > 1:
+            if percent > 0.0001 and elapsed > 1:
                 total = elapsed / percent
                 eta = total - elapsed
-                h = eta//3600.
-                m = (eta//60) % 60
+                h = eta // 3600.0
+                m = (eta // 60) % 60
                 s = eta % 60
-                suffix = ' ETA: %02d:%02d:%02d'%(h,m,s)
+                suffix = " ETA: %02d:%02d:%02d" % (h, m, s)
         barWidth = self.width - len(prefix) - len(suffix) - 2
-        n = int(barWidth*percent)
+        n = int(barWidth * percent)
         if len(message) < self.width:
-            message = message + ' '*(self.width - len(message))
+            message = message + " " * (self.width - len(message))
         else:
-            message = '... ' + message[-(self.width-4):]
+            message = "... " + message[-(self.width - 4) :]
         bc = self.barColor
-        bar = self.BAR % (prefix, bc, '='*n, '-'*(barWidth-n), bc, suffix)
+        bar = self.BAR % (prefix, bc, "=" * n, "-" * (barWidth - n), bc, suffix)
         bar = self.term.render(bar)
         sys.stdout.write(
-            self.BOL + self.term.UP + self.term.CLEAR_EOL +
-            bar +
-            self.XNL +
-            self.term.CLEAR_EOL + message)
+            self.BOL
+            + self.term.UP
+            + self.term.CLEAR_EOL
+            + bar
+            + self.XNL
+            + self.term.CLEAR_EOL
+            + message
+        )
         if not self.term.XN:
             sys.stdout.flush()
 
     def clear(self, interrupted):
         if not self.cleared:
-            sys.stdout.write(self.BOL + self.term.CLEAR_EOL +
-                             self.term.UP + self.term.CLEAR_EOL +
-                             self.term.UP + self.term.CLEAR_EOL)
+            sys.stdout.write(
+                self.BOL
+                + self.term.CLEAR_EOL
+                + self.term.UP
+                + self.term.CLEAR_EOL
+                + self.term.UP
+                + self.term.CLEAR_EOL
+            )
             if interrupted:  # ^C creates extra line. Gobble it up!
                 sys.stdout.write(self.term.UP + self.term.CLEAR_EOL)
-                sys.stdout.write('^C')
+                sys.stdout.write("^C")
             sys.stdout.flush()
             self.cleared = 1
 
+
 def test():
     tc = TerminalController()
-    p = ProgressBar(tc, 'Tests')
+    p = ProgressBar(tc, "Tests")
     for i in range(101):
-        p.update(i/100., str(i))        
-        time.sleep(.3)
+        p.update(i / 100.0, str(i))
+        time.sleep(0.3)
+
 
-if __name__=='__main__':
+if __name__ == "__main__":
     test()
```

### Comparing `lit-16.0.6/lit/ShCommands.py` & `lit-17.0.0rc1/lit/ShCommands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,108 +1,113 @@
 class Command:
     def __init__(self, args, redirects):
         self.args = list(args)
         self.redirects = list(redirects)
 
     def __repr__(self):
-        return 'Command(%r, %r)' % (self.args, self.redirects)
+        return "Command(%r, %r)" % (self.args, self.redirects)
 
     def __eq__(self, other):
         if not isinstance(other, Command):
             return False
 
-        return ((self.args, self.redirects) ==
-                (other.args, other.redirects))
+        return (self.args, self.redirects) == (other.args, other.redirects)
 
     def toShell(self, file):
         for arg in self.args:
             if "'" not in arg:
                 quoted = "'%s'" % arg
-            elif '"' not in arg and '$' not in arg:
+            elif '"' not in arg and "$" not in arg:
                 quoted = '"%s"' % arg
             else:
-                raise NotImplementedError('Unable to quote %r' % arg)
+                raise NotImplementedError("Unable to quote %r" % arg)
             file.write(quoted)
 
             # For debugging / validation.
             import ShUtil
+
             dequoted = list(ShUtil.ShLexer(quoted).lex())
             if dequoted != [arg]:
-                raise NotImplementedError('Unable to quote %r' % arg)
+                raise NotImplementedError("Unable to quote %r" % arg)
 
         for r in self.redirects:
             if len(r[0]) == 1:
                 file.write("%s '%s'" % (r[0][0], r[1]))
             else:
                 file.write("%s%s '%s'" % (r[0][1], r[0][0], r[1]))
 
+
 class GlobItem:
     def __init__(self, pattern):
         self.pattern = pattern
 
     def __repr__(self):
         return self.pattern
 
     def __eq__(self, other):
         if not isinstance(other, Command):
             return False
 
-        return (self.pattern == other.pattern)
+        return self.pattern == other.pattern
 
     def resolve(self, cwd):
         import glob
         import os
+
         if os.path.isabs(self.pattern):
-           abspath = self.pattern
+            abspath = self.pattern
         else:
             abspath = os.path.join(cwd, self.pattern)
         results = glob.glob(abspath)
         return [self.pattern] if len(results) == 0 else results
 
+
 class Pipeline:
     def __init__(self, commands, negate=False, pipe_err=False):
         self.commands = commands
         self.negate = negate
         self.pipe_err = pipe_err
 
     def __repr__(self):
-        return 'Pipeline(%r, %r, %r)' % (self.commands, self.negate,
-                                         self.pipe_err)
+        return "Pipeline(%r, %r, %r)" % (self.commands, self.negate, self.pipe_err)
 
     def __eq__(self, other):
         if not isinstance(other, Pipeline):
             return False
 
-        return ((self.commands, self.negate, self.pipe_err) ==
-                (other.commands, other.negate, self.pipe_err))
+        return (self.commands, self.negate, self.pipe_err) == (
+            other.commands,
+            other.negate,
+            self.pipe_err,
+        )
 
     def toShell(self, file, pipefail=False):
         if pipefail != self.pipe_err:
             raise ValueError('Inconsistent "pipefail" attribute!')
         if self.negate:
-            file.write('! ')
+            file.write("! ")
         for cmd in self.commands:
             cmd.toShell(file)
             if cmd is not self.commands[-1]:
-                file.write('|\n  ')
+                file.write("|\n  ")
+
 
 class Seq:
     def __init__(self, lhs, op, rhs):
-        assert op in (';', '&', '||', '&&')
+        assert op in (";", "&", "||", "&&")
         self.op = op
         self.lhs = lhs
         self.rhs = rhs
 
     def __repr__(self):
-        return 'Seq(%r, %r, %r)' % (self.lhs, self.op, self.rhs)
+        return "Seq(%r, %r, %r)" % (self.lhs, self.op, self.rhs)
 
     def __eq__(self, other):
         if not isinstance(other, Seq):
             return False
 
-        return ((self.lhs, self.op, self.rhs) ==
-                (other.lhs, other.op, other.rhs))
+        return (self.lhs, self.op, self.rhs) == (other.lhs, other.op, other.rhs)
 
     def toShell(self, file, pipefail=False):
         self.lhs.toShell(file, pipefail)
-        file.write(' %s\n' % self.op)
+        file.write(" %s\n" % self.op)
         self.rhs.toShell(file, pipefail)
```

### Comparing `lit-16.0.6/lit/ShUtil.py` & `lit-17.0.0rc1/lit/ShUtil.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import absolute_import
 import itertools
 
 import lit.util
 from lit.ShCommands import Command, GlobItem, Pipeline, Seq
 
+
 class ShLexer:
-    def __init__(self, data, win32Escapes = False):
+    def __init__(self, data, win32Escapes=False):
         self.data = data
         self.pos = 0
         self.end = len(data)
         self.win32Escapes = win32Escapes
 
     def eat(self):
         c = self.data[self.pos]
@@ -18,74 +19,81 @@
 
     def look(self):
         return self.data[self.pos]
 
     def maybe_eat(self, c):
         """
         maybe_eat(c) - Consume the character c if it is the next character,
-        returning True if a character was consumed. """
+        returning True if a character was consumed."""
         if self.data[self.pos] == c:
             self.pos += 1
             return True
         return False
 
     def lex_arg_fast(self, c):
         # Get the leading whitespace free section.
-        chunk = self.data[self.pos - 1:].split(None, 1)[0]
-        
+        chunk = self.data[self.pos - 1 :].split(None, 1)[0]
+
         # If it has special characters, the fast path failed.
-        if ('|' in chunk or '&' in chunk or 
-            '<' in chunk or '>' in chunk or
-            "'" in chunk or '"' in chunk or
-            ';' in chunk or '\\' in chunk):
+        if (
+            "|" in chunk
+            or "&" in chunk
+            or "<" in chunk
+            or ">" in chunk
+            or "'" in chunk
+            or '"' in chunk
+            or ";" in chunk
+            or "\\" in chunk
+        ):
             return None
-        
+
         self.pos = self.pos - 1 + len(chunk)
-        return GlobItem(chunk) if '*' in chunk or '?' in chunk else chunk
-        
+        return GlobItem(chunk) if "*" in chunk or "?" in chunk else chunk
+
     def lex_arg_slow(self, c):
         if c in "'\"":
             str = self.lex_arg_quoted(c)
         else:
             str = c
         unquoted_glob_char = False
         quoted_glob_char = False
         while self.pos != self.end:
             c = self.look()
             if c.isspace() or c in "|&;":
                 break
-            elif c in '><':
+            elif c in "><":
                 # This is an annoying case; we treat '2>' as a single token so
                 # we don't have to track whitespace tokens.
 
                 # If the parse string isn't an integer, do the usual thing.
                 if not str.isdigit():
                     break
 
                 # Otherwise, lex the operator and convert to a redirection
                 # token.
                 num = int(str)
                 tok = self.lex_one_token()
                 assert isinstance(tok, tuple) and len(tok) == 1
-                return (tok[0], num)                    
+                return (tok[0], num)
             elif c == '"' or c == "'":
                 self.eat()
                 quoted_arg = self.lex_arg_quoted(c)
-                if '*' in quoted_arg or '?' in quoted_arg:
+                if "*" in quoted_arg or "?" in quoted_arg:
                     quoted_glob_char = True
                 str += quoted_arg
-            elif not self.win32Escapes and c == '\\':
+            elif not self.win32Escapes and c == "\\":
                 # Outside of a string, '\\' escapes everything.
                 self.eat()
                 if self.pos == self.end:
                     lit.util.warning(
-                        "escape at end of quoted argument in: %r" % self.data)
+                        "escape at end of quoted argument in: %r" % self.data
+                    )
                     return str
                 str += self.eat()
-            elif c in '*?':
+            elif c in "*?":
                 unquoted_glob_char = True
                 str += self.eat()
             else:
                 str += self.eat()
         # If a quote character is present, lex_arg_quoted will remove the quotes
         # and append the argument directly.  This causes a problem when the
         # quoted portion contains a glob character, as the character will no
@@ -98,122 +106,123 @@
         # By adding an assertion, it means some bot somewhere will catch this
         # and flag the user of a non-portable test (which could almost certainly
         # be re-written to work correctly without triggering this).
         assert not (quoted_glob_char and unquoted_glob_char)
         return GlobItem(str) if unquoted_glob_char else str
 
     def lex_arg_quoted(self, delim):
-        str = ''
+        str = ""
         while self.pos != self.end:
             c = self.eat()
             if c == delim:
                 return str
-            elif c == '\\' and delim == '"':
+            elif c == "\\" and delim == '"':
                 # Inside a '"' quoted string, '\\' only escapes the quote
                 # character and backslash, otherwise it is preserved.
                 if self.pos == self.end:
                     lit.util.warning(
-                        "escape at end of quoted argument in: %r" % self.data)
+                        "escape at end of quoted argument in: %r" % self.data
+                    )
                     return str
                 c = self.eat()
-                if c == '"': # 
+                if c == '"':  #
                     str += '"'
-                elif c == '\\':
-                    str += '\\'
+                elif c == "\\":
+                    str += "\\"
                 else:
-                    str += '\\' + c
+                    str += "\\" + c
             else:
                 str += c
         lit.util.warning("missing quote character in %r" % self.data)
         return str
-    
+
     def lex_arg_checked(self, c):
         pos = self.pos
         res = self.lex_arg_fast(c)
         end = self.pos
 
         self.pos = pos
         reference = self.lex_arg_slow(c)
         if res is not None:
             if res != reference:
-                raise ValueError("Fast path failure: %r != %r" % (
-                        res, reference))
+                raise ValueError("Fast path failure: %r != %r" % (res, reference))
             if self.pos != end:
-                raise ValueError("Fast path failure: %r != %r" % (
-                        self.pos, end))
+                raise ValueError("Fast path failure: %r != %r" % (self.pos, end))
         return reference
-        
+
     def lex_arg(self, c):
         return self.lex_arg_fast(c) or self.lex_arg_slow(c)
-        
+
     def lex_one_token(self):
         """
-        lex_one_token - Lex a single 'sh' token. """
+        lex_one_token - Lex a single 'sh' token."""
 
         c = self.eat()
-        if c == ';':
+        if c == ";":
             return (c,)
-        if c == '|':
-            if self.maybe_eat('|'):
-                return ('||',)
+        if c == "|":
+            if self.maybe_eat("|"):
+                return ("||",)
             return (c,)
-        if c == '&':
-            if self.maybe_eat('&'):
-                return ('&&',)
-            if self.maybe_eat('>'): 
-                return ('&>',)
+        if c == "&":
+            if self.maybe_eat("&"):
+                return ("&&",)
+            if self.maybe_eat(">"):
+                return ("&>",)
             return (c,)
-        if c == '>':
-            if self.maybe_eat('&'):
-                return ('>&',)
-            if self.maybe_eat('>'):
-                return ('>>',)
+        if c == ">":
+            if self.maybe_eat("&"):
+                return (">&",)
+            if self.maybe_eat(">"):
+                return (">>",)
             return (c,)
-        if c == '<':
-            if self.maybe_eat('&'):
-                return ('<&',)
-            if self.maybe_eat('>'):
-                return ('<<',)
+        if c == "<":
+            if self.maybe_eat("&"):
+                return ("<&",)
+            if self.maybe_eat(">"):
+                return ("<<",)
             return (c,)
 
         return self.lex_arg(c)
 
     def lex(self):
         while self.pos != self.end:
             if self.look().isspace():
                 self.eat()
             else:
                 yield self.lex_one_token()
 
+
 ###
- 
+
+
 class ShParser:
-    def __init__(self, data, win32Escapes = False, pipefail = False):
+    def __init__(self, data, win32Escapes=False, pipefail=False):
         self.data = data
         self.pipefail = pipefail
-        self.tokens = ShLexer(data, win32Escapes = win32Escapes).lex()
-    
+        self.tokens = ShLexer(data, win32Escapes=win32Escapes).lex()
+
     def lex(self):
         for item in self.tokens:
             return item
         return None
-    
+
     def look(self):
         token = self.lex()
         if token is not None:
             self.tokens = itertools.chain([token], self.tokens)
         return token
-    
+
     def parse_command(self):
         tok = self.lex()
         if not tok:
             raise ValueError("empty command!")
         if isinstance(tok, tuple):
             raise ValueError("syntax error near unexpected token %r" % tok[0])
-        
+
         args = [tok]
         redirects = []
         while 1:
             tok = self.look()
 
             # EOF?
             if tok is None:
@@ -222,44 +231,42 @@
             # If this is an argument, just add it to the current command.
             if isinstance(tok, (str, GlobItem)):
                 args.append(self.lex())
                 continue
 
             # Otherwise see if it is a terminator.
             assert isinstance(tok, tuple)
-            if tok[0] in ('|',';','&','||','&&'):
+            if tok[0] in ("|", ";", "&", "||", "&&"):
                 break
-            
+
             # Otherwise it must be a redirection.
             op = self.lex()
             arg = self.lex()
             if not arg:
                 raise ValueError("syntax error near token %r" % op[0])
             redirects.append((op, arg))
 
         return Command(args, redirects)
 
     def parse_pipeline(self):
         negate = False
 
         commands = [self.parse_command()]
-        while self.look() == ('|',):
+        while self.look() == ("|",):
             self.lex()
             commands.append(self.parse_command())
         return Pipeline(commands, negate, self.pipefail)
-            
+
     def parse(self):
         lhs = self.parse_pipeline()
 
         while self.look():
             operator = self.lex()
             assert isinstance(operator, tuple) and len(operator) == 1
 
             if not self.look():
-                raise ValueError(
-                    "missing argument to operator %r" % operator[0])
-            
+                raise ValueError("missing argument to operator %r" % operator[0])
+
             # FIXME: Operator precedence!!
             lhs = Seq(lhs, operator[0], self.parse_pipeline())
 
         return lhs
-
```

### Comparing `lit-16.0.6/lit/Test.py` & `lit-17.0.0rc1/lit/Test.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from json import JSONEncoder
 
 from lit.BooleanExpression import BooleanExpression
 from lit.TestTimes import read_test_times
 
 # Test result codes.
 
+
 class ResultCode(object):
     """Test result codes."""
 
     # All result codes (including user-defined ones) in declaration order
     _all_codes = []
 
     @staticmethod
@@ -33,34 +34,34 @@
     def __init__(self, name, label, isFailure):
         self.name = name
         self.label = label
         self.isFailure = isFailure
         ResultCode._all_codes.append(self)
 
     def __repr__(self):
-        return '%s%r' % (self.__class__.__name__,
-                         (self.name, self.isFailure))
+        return "%s%r" % (self.__class__.__name__, (self.name, self.isFailure))
 
 
 # Successes
-EXCLUDED    = ResultCode('EXCLUDED',    'Excluded', False)
-SKIPPED     = ResultCode('SKIPPED',     'Skipped', False)
-UNSUPPORTED = ResultCode('UNSUPPORTED', 'Unsupported', False)
-PASS        = ResultCode('PASS',        'Passed', False)
-FLAKYPASS   = ResultCode('FLAKYPASS',   'Passed With Retry', False)
-XFAIL       = ResultCode('XFAIL',       'Expectedly Failed', False)
+EXCLUDED = ResultCode("EXCLUDED", "Excluded", False)
+SKIPPED = ResultCode("SKIPPED", "Skipped", False)
+UNSUPPORTED = ResultCode("UNSUPPORTED", "Unsupported", False)
+PASS = ResultCode("PASS", "Passed", False)
+FLAKYPASS = ResultCode("FLAKYPASS", "Passed With Retry", False)
+XFAIL = ResultCode("XFAIL", "Expectedly Failed", False)
 # Failures
-UNRESOLVED  = ResultCode('UNRESOLVED',  'Unresolved', True)
-TIMEOUT     = ResultCode('TIMEOUT',     'Timed Out', True)
-FAIL        = ResultCode('FAIL',        'Failed', True)
-XPASS       = ResultCode('XPASS',       'Unexpectedly Passed', True)
+UNRESOLVED = ResultCode("UNRESOLVED", "Unresolved", True)
+TIMEOUT = ResultCode("TIMEOUT", "Timed Out", True)
+FAIL = ResultCode("FAIL", "Failed", True)
+XPASS = ResultCode("XPASS", "Unexpectedly Passed", True)
 
 
 # Test metric values.
 
+
 class MetricValue(object):
     def format(self):
         """
         format() -> str
 
         Convert this metric to a string suitable for displaying as part of the
         console output.
@@ -72,39 +73,43 @@
         todata() -> json-serializable data
 
         Convert this metric to content suitable for serializing in the JSON test
         output.
         """
         raise RuntimeError("abstract method")
 
+
 class IntMetricValue(MetricValue):
     def __init__(self, value):
         self.value = value
 
     def format(self):
         return str(self.value)
 
     def todata(self):
         return self.value
 
+
 class RealMetricValue(MetricValue):
     def __init__(self, value):
         self.value = value
 
     def format(self):
-        return '%.4f' % self.value
+        return "%.4f" % self.value
 
     def todata(self):
         return self.value
 
+
 class JSONMetricValue(MetricValue):
     """
-        JSONMetricValue is used for types that are representable in the output
-        but that are otherwise uninterpreted.
+    JSONMetricValue is used for types that are representable in the output
+    but that are otherwise uninterpreted.
     """
+
     def __init__(self, value):
         # Ensure the value is a serializable by trying to encode it.
         # WARNING: The value may change before it is encoded again, and may
         #          not be encodable after the change.
         try:
             e = JSONEncoder()
             e.encode(value)
@@ -115,14 +120,15 @@
     def format(self):
         e = JSONEncoder(indent=2, sort_keys=True)
         return e.encode(self.value)
 
     def todata(self):
         return self.value
 
+
 def toMetricValue(value):
     if isinstance(value, MetricValue):
         return value
     elif isinstance(value, int):
         return IntMetricValue(value)
     elif isinstance(value, float):
         return RealMetricValue(value)
@@ -137,18 +143,19 @@
         # Try to create a JSONMetricValue and let the constructor throw
         # if value is not a valid type.
         return JSONMetricValue(value)
 
 
 # Test results.
 
+
 class Result(object):
     """Wrapper for the results of executing an individual test."""
 
-    def __init__(self, code, output='', elapsed=None):
+    def __init__(self, code, output="", elapsed=None):
         # The result code.
         self.code = code
         # The test output.
         self.output = output
         # The wall timing to execute the test, if timing.
         self.elapsed = elapsed
         self.start = None
@@ -165,16 +172,15 @@
         Attach a test metric to the test result, with the given name and list of
         values. It is an error to attempt to attach the metrics with the same
         name multiple times.
 
         Each value must be an instance of a MetricValue subclass.
         """
         if name in self.metrics:
-            raise ValueError("result already includes metrics for %r" % (
-                    name,))
+            raise ValueError("result already includes metrics for %r" % (name,))
         if not isinstance(value, MetricValue):
             raise TypeError("unexpected metric value: %r" % (value,))
         self.metrics[name] = value
 
     def addMicroResult(self, name, microResult):
         """
         addMicroResult(microResult)
@@ -182,23 +188,23 @@
         Attach a micro-test result to the test result, with the given name and
         result.  It is an error to attempt to attach a micro-test with the
         same name multiple times.
 
         Each micro-test result must be an instance of the Result class.
         """
         if name in self.microResults:
-            raise ValueError("Result already includes microResult for %r" % (
-                   name,))
+            raise ValueError("Result already includes microResult for %r" % (name,))
         if not isinstance(microResult, Result):
             raise TypeError("unexpected MicroResult value %r" % (microResult,))
         self.microResults[name] = microResult
 
 
 # Test classes.
 
+
 class TestSuite:
     """TestSuite - Information on a group of tests.
 
     A test suite groups together a set of logically related tests.
     """
 
     def __init__(self, name, source_root, exec_root, config):
@@ -212,18 +218,21 @@
 
     def getSourcePath(self, components):
         return os.path.join(self.source_root, *components)
 
     def getExecPath(self, components):
         return os.path.join(self.exec_root, *components)
 
+
 class Test:
     """Test - Information on a single test instance."""
 
-    def __init__(self, suite, path_in_suite, config, file_path = None, gtest_json_file = None):
+    def __init__(
+        self, suite, path_in_suite, config, file_path=None, gtest_json_file=None
+    ):
         self.suite = suite
         self.path_in_suite = path_in_suite
         self.config = config
         self.file_path = file_path
         self.gtest_json_file = gtest_json_file
 
         # A list of conditions under which this test is expected to fail.
@@ -243,31 +252,30 @@
         # A list of conditions that prevent execution of the test.
         # Each condition is a boolean expression of features. All of them
         # must be False for the test to run.
         self.unsupported = []
 
         # An optional number of retries allowed before the test finally succeeds.
         # The test is run at most once plus the number of retries specified here.
-        self.allowed_retries = getattr(config, 'test_retry_attempts', 0)
+        self.allowed_retries = getattr(config, "test_retry_attempts", 0)
 
         # The test result, once complete.
         self.result = None
 
         # The previous test failure state, if applicable.
         self.previous_failure = False
 
         # The previous test elapsed time, if applicable.
         self.previous_elapsed = 0.0
 
-        if suite.test_times and '/'.join(path_in_suite) in suite.test_times:
-            time = suite.test_times['/'.join(path_in_suite)]
+        if suite.test_times and "/".join(path_in_suite) in suite.test_times:
+            time = suite.test_times["/".join(path_in_suite)]
             self.previous_elapsed = abs(time)
             self.previous_failure = time < 0
 
-
     def setResult(self, result):
         assert self.result is None, "result already set"
         assert isinstance(result, Result), "unexpected result type"
         try:
             expected_to_fail = self.isExpectedToFail()
         except ValueError as err:
             # Syntax error in an XFAIL line.
@@ -284,15 +292,15 @@
         self.result = result
 
     def isFailure(self):
         assert self.result
         return self.result.code.isFailure
 
     def getFullName(self):
-        return self.suite.config.name + ' :: ' + '/'.join(self.path_in_suite)
+        return self.suite.config.name + " :: " + "/".join(self.path_in_suite)
 
     def getFilePath(self):
         if self.file_path:
             return self.file_path
         return self.getSourcePath()
 
     def getSourcePath(self):
@@ -309,30 +317,30 @@
         configuration. This check relies on the test xfails property which by
         some test formats may not be computed until the test has first been
         executed.
         Throws ValueError if an XFAIL line has a syntax error.
         """
 
         if self.xfail_not:
-          return False
+            return False
 
         features = self.config.available_features
 
         # Check if any of the xfails match an available feature.
         for item in self.xfails:
             # If this is the wildcard, it always fails.
-            if item == '*':
+            if item == "*":
                 return True
 
             # If this is a True expression of features, it fails.
             try:
                 if BooleanExpression.evaluate(item, features):
                     return True
             except ValueError as e:
-                raise ValueError('Error in XFAIL list:\n%s' % str(e))
+                raise ValueError("Error in XFAIL list:\n%s" % str(e))
 
         return False
 
     def isWithinFeatureLimits(self):
         """
         isWithinFeatureLimits() -> bool
 
@@ -348,27 +356,33 @@
             return True  # No limits. Run it.
 
         # Check the requirements as-is (#1)
         if self.getMissingRequiredFeatures():
             return False
 
         # Check the requirements after removing the limiting features (#2)
-        featuresMinusLimits = [f for f in self.config.available_features
-                               if not f in self.config.limit_to_features]
+        featuresMinusLimits = [
+            f
+            for f in self.config.available_features
+            if not f in self.config.limit_to_features
+        ]
         if not self.getMissingRequiredFeaturesFromList(featuresMinusLimits):
             return False
 
         return True
 
     def getMissingRequiredFeaturesFromList(self, features):
         try:
-            return [item for item in self.requires
-                    if not BooleanExpression.evaluate(item, features)]
+            return [
+                item
+                for item in self.requires
+                if not BooleanExpression.evaluate(item, features)
+            ]
         except ValueError as e:
-            raise ValueError('Error in REQUIRES list:\n%s' % str(e))
+            raise ValueError("Error in REQUIRES list:\n%s" % str(e))
 
     def getMissingRequiredFeatures(self):
         """
         getMissingRequiredFeatures() -> list of strings
 
         Returns a list of features from REQUIRES that are not satisfied."
         Throws ValueError if a REQUIRES line has a syntax error.
@@ -385,31 +399,38 @@
         in the test configuration's features.
         Throws ValueError if an UNSUPPORTED line has a syntax error.
         """
 
         features = self.config.available_features
 
         try:
-            return [item for item in self.unsupported
-                    if BooleanExpression.evaluate(item, features)]
+            return [
+                item
+                for item in self.unsupported
+                if BooleanExpression.evaluate(item, features)
+            ]
         except ValueError as e:
-            raise ValueError('Error in UNSUPPORTED list:\n%s' % str(e))
+            raise ValueError("Error in UNSUPPORTED list:\n%s" % str(e))
 
     def getUsedFeatures(self):
         """
         getUsedFeatures() -> list of strings
 
         Returns a list of all features appearing in XFAIL, UNSUPPORTED and
         REQUIRES annotations for this test.
         """
         import lit.TestRunner
-        parsed = lit.TestRunner._parseKeywords(self.getSourcePath(), require_script=False)
-        feature_keywords = ('UNSUPPORTED:', 'REQUIRES:', 'XFAIL:')
+
+        parsed = lit.TestRunner._parseKeywords(
+            self.getSourcePath(), require_script=False
+        )
+        feature_keywords = ("UNSUPPORTED:", "REQUIRES:", "XFAIL:")
         boolean_expressions = itertools.chain.from_iterable(
             parsed[k] or [] for k in feature_keywords
         )
         tokens = itertools.chain.from_iterable(
-            BooleanExpression.tokenize(expr) for expr in
-                boolean_expressions if expr != '*'
+            BooleanExpression.tokenize(expr)
+            for expr in boolean_expressions
+            if expr != "*"
         )
         matchExpressions = set(filter(BooleanExpression.isMatchExpression, tokens))
         return matchExpressions
```

### Comparing `lit-16.0.6/lit/TestRunner.py` & `lit-17.0.0rc1/lit/TestRunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,32 +9,35 @@
 import pathlib
 import platform
 import shutil
 import tempfile
 import threading
 
 import io
+
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 from lit.ShCommands import GlobItem, Command
 import lit.ShUtil as ShUtil
 import lit.Test as Test
 import lit.util
 from lit.util import to_bytes, to_string, to_unicode
 from lit.BooleanExpression import BooleanExpression
 
+
 class InternalShellError(Exception):
     def __init__(self, command, message):
         self.command = command
         self.message = message
 
-kIsWindows = platform.system() == 'Windows'
+
+kIsWindows = platform.system() == "Windows"
 
 # Don't use close_fds on Windows.
 kUseCloseFDs = not kIsWindows
 
 # Use temporary files to replace /dev/null on Windows.
 kAvoidDevNull = kIsWindows
 kDevNull = "/dev/null"
@@ -47,15 +50,16 @@
 #
 # This regex captures ARG.  ARG must not contain a right parenthesis, which
 # terminates %dbg.  ARG must not contain quotes, in which ARG might be enclosed
 # during expansion.
 #
 # COMMAND that follows %dbg(ARG) is also captured. COMMAND can be
 # empty as a result of conditinal substitution.
-kPdbgRegex = '%dbg\\(([^)\'"]*)\\)(.*)'
+kPdbgRegex = "%dbg\\(([^)'\"]*)\\)(.*)"
+
 
 class ShellEnvironment(object):
 
     """Mutable shell environment containing things like CWD and env vars.
 
     Environment variables are not implemented, but cwd tracking is. In addition,
     we maintain a dir stack for pushd/popd.
@@ -68,21 +72,23 @@
 
     def change_dir(self, newdir):
         if os.path.isabs(newdir):
             self.cwd = newdir
         else:
             self.cwd = os.path.realpath(os.path.join(self.cwd, newdir))
 
+
 class TimeoutHelper(object):
     """
-        Object used to helper manage enforcing a timeout in
-        _executeShCmd(). It is passed through recursive calls
-        to collect processes that have been executed so that when
-        the timeout happens they can be killed.
+    Object used to helper manage enforcing a timeout in
+    _executeShCmd(). It is passed through recursive calls
+    to collect processes that have been executed so that when
+    the timeout happens they can be killed.
     """
+
     def __init__(self, timeout):
         self.timeout = timeout
         self._procs = []
         self._timeoutReached = False
         self._doneKillPass = False
         # This lock will be used to protect concurrent access
         # to _procs and _doneKillPass
@@ -131,68 +137,74 @@
         self._kill()
 
     def timeoutReached(self):
         return self._timeoutReached
 
     def _kill(self):
         """
-            This method may be called multiple times as we might get unlucky
-            and be in the middle of creating a new process in _executeShCmd()
-            which won't yet be in ``self._procs``. By locking here and in
-            addProcess() we should be able to kill processes launched after
-            the initial call to _kill()
+        This method may be called multiple times as we might get unlucky
+        and be in the middle of creating a new process in _executeShCmd()
+        which won't yet be in ``self._procs``. By locking here and in
+        addProcess() we should be able to kill processes launched after
+        the initial call to _kill()
         """
         with self._lock:
             for p in self._procs:
                 lit.util.killProcessAndChildren(p.pid)
             # Empty the list and note that we've done a pass over the list
-            self._procs = [] # Python2 doesn't have list.clear()
+            self._procs = []  # Python2 doesn't have list.clear()
             self._doneKillPass = True
 
+
 class ShellCommandResult(object):
     """Captures the result of an individual command."""
 
-    def __init__(self, command, stdout, stderr, exitCode, timeoutReached,
-                 outputFiles = []):
+    def __init__(
+        self, command, stdout, stderr, exitCode, timeoutReached, outputFiles=[]
+    ):
         self.command = command
         self.stdout = stdout
         self.stderr = stderr
         self.exitCode = exitCode
         self.timeoutReached = timeoutReached
         self.outputFiles = list(outputFiles)
 
+
 def executeShCmd(cmd, shenv, results, timeout=0):
     """
-        Wrapper around _executeShCmd that handles
-        timeout
+    Wrapper around _executeShCmd that handles
+    timeout
     """
     # Use the helper even when no timeout is required to make
     # other code simpler (i.e. avoid bunch of ``!= None`` checks)
     timeoutHelper = TimeoutHelper(timeout)
     if timeout > 0:
         timeoutHelper.startTimer()
     finalExitCode = _executeShCmd(cmd, shenv, results, timeoutHelper)
     timeoutHelper.cancel()
     timeoutInfo = None
     if timeoutHelper.timeoutReached():
-        timeoutInfo = 'Reached timeout of {} seconds'.format(timeout)
+        timeoutInfo = "Reached timeout of {} seconds".format(timeout)
 
     return (finalExitCode, timeoutInfo)
 
+
 def expand_glob(arg, cwd):
     if isinstance(arg, GlobItem):
         return sorted(arg.resolve(cwd))
     return [arg]
 
+
 def expand_glob_expressions(args, cwd):
     result = [args[0]]
     for arg in args[1:]:
         result.extend(expand_glob(arg, cwd))
     return result
 
+
 def quote_windows_command(seq):
     """
     Reimplement Python's private subprocess.list2cmdline for MSys compatibility
 
     Based on CPython implementation here:
       https://hg.python.org/cpython/file/849826a900d2/Lib/subprocess.py#l422
 
@@ -214,28 +226,35 @@
     result = []
     needquote = False
     for arg in seq:
         bs_buf = []
 
         # Add a space to separate this argument from the others
         if result:
-            result.append(' ')
+            result.append(" ")
 
         # This logic differs from upstream list2cmdline.
-        needquote = (" " in arg) or ("\t" in arg) or ("\"" in arg) or ("[" in arg) or (";" in arg) or not arg
+        needquote = (
+            (" " in arg)
+            or ("\t" in arg)
+            or ('"' in arg)
+            or ("[" in arg)
+            or (";" in arg)
+            or not arg
+        )
         if needquote:
             result.append('"')
 
         for c in arg:
-            if c == '\\':
+            if c == "\\":
                 # Don't know if we need to double yet.
                 bs_buf.append(c)
             elif c == '"':
                 # Double backslashes.
-                result.append('\\' * len(bs_buf)*2)
+                result.append("\\" * len(bs_buf) * 2)
                 bs_buf = []
                 result.append('\\"')
             else:
                 # Normal char
                 if bs_buf:
                     result.extend(bs_buf)
                     bs_buf = []
@@ -245,146 +264,153 @@
         if bs_buf:
             result.extend(bs_buf)
 
         if needquote:
             result.extend(bs_buf)
             result.append('"')
 
-    return ''.join(result)
+    return "".join(result)
+
 
 # args are from 'export' or 'env' command.
 # Skips the command, and parses its arguments.
 # Modifies env accordingly.
 # Returns copy of args without the command or its arguments.
 def updateEnv(env, args):
     arg_idx_next = len(args)
     unset_next_env_var = False
     for arg_idx, arg in enumerate(args[1:]):
         # Support for the -u flag (unsetting) for env command
         # e.g., env -u FOO -u BAR will remove both FOO and BAR
         # from the environment.
-        if arg == '-u':
+        if arg == "-u":
             unset_next_env_var = True
             continue
         if unset_next_env_var:
             unset_next_env_var = False
             if arg in env.env:
                 del env.env[arg]
             continue
 
         # Partition the string into KEY=VALUE.
-        key, eq, val = arg.partition('=')
+        key, eq, val = arg.partition("=")
         # Stop if there was no equals.
-        if eq == '':
+        if eq == "":
             arg_idx_next = arg_idx + 1
             break
         env.env[key] = val
     return args[arg_idx_next:]
 
+
 def executeBuiltinCd(cmd, shenv):
     """executeBuiltinCd - Change the current directory."""
     if len(cmd.args) != 2:
         raise InternalShellError(cmd, "'cd' supports only one argument")
     # Update the cwd in the parent environment.
     shenv.change_dir(cmd.args[1])
     # The cd builtin always succeeds. If the directory does not exist, the
     # following Popen calls will fail instead.
     return ShellCommandResult(cmd, "", "", 0, False)
 
+
 def executeBuiltinPushd(cmd, shenv):
     """executeBuiltinPushd - Change the current dir and save the old."""
     if len(cmd.args) != 2:
         raise InternalShellError(cmd, "'pushd' supports only one argument")
     shenv.dirStack.append(shenv.cwd)
     shenv.change_dir(cmd.args[1])
     return ShellCommandResult(cmd, "", "", 0, False)
 
+
 def executeBuiltinPopd(cmd, shenv):
     """executeBuiltinPopd - Restore a previously saved working directory."""
     if len(cmd.args) != 1:
         raise InternalShellError(cmd, "'popd' does not support arguments")
     if not shenv.dirStack:
         raise InternalShellError(cmd, "popd: directory stack empty")
     shenv.cwd = shenv.dirStack.pop()
     return ShellCommandResult(cmd, "", "", 0, False)
 
+
 def executeBuiltinExport(cmd, shenv):
     """executeBuiltinExport - Set an environment variable."""
     if len(cmd.args) != 2:
         raise InternalShellError("'export' supports only one argument")
     updateEnv(shenv, cmd.args)
     return ShellCommandResult(cmd, "", "", 0, False)
 
+
 def executeBuiltinEcho(cmd, shenv):
     """Interpret a redirected echo command"""
     opened_files = []
-    stdin, stdout, stderr = processRedirects(cmd, subprocess.PIPE, shenv,
-                                             opened_files)
+    stdin, stdout, stderr = processRedirects(cmd, subprocess.PIPE, shenv, opened_files)
     if stdin != subprocess.PIPE or stderr != subprocess.PIPE:
         raise InternalShellError(
-                cmd, "stdin and stderr redirects not supported for echo")
+            cmd, "stdin and stderr redirects not supported for echo"
+        )
 
     # Some tests have un-redirected echo commands to help debug test failures.
     # Buffer our output and return it to the caller.
     is_redirected = True
-    encode = lambda x : x
+    encode = lambda x: x
     if stdout == subprocess.PIPE:
         is_redirected = False
         stdout = StringIO()
     elif kIsWindows:
         # Reopen stdout in binary mode to avoid CRLF translation. The versions
         # of echo we are replacing on Windows all emit plain LF, and the LLVM
         # tests now depend on this.
         # When we open as binary, however, this also means that we have to write
         # 'bytes' objects to stdout instead of 'str' objects.
         encode = lit.util.to_bytes
-        stdout = open(stdout.name, stdout.mode + 'b')
+        stdout = open(stdout.name, stdout.mode + "b")
         opened_files.append((None, None, stdout, None))
 
     # Implement echo flags. We only support -e and -n, and not yet in
     # combination. We have to ignore unknown flags, because `echo "-D FOO"`
     # prints the dash.
     args = cmd.args[1:]
     interpret_escapes = False
     write_newline = True
-    while len(args) >= 1 and args[0] in ('-e', '-n'):
+    while len(args) >= 1 and args[0] in ("-e", "-n"):
         flag = args[0]
         args = args[1:]
-        if flag == '-e':
+        if flag == "-e":
             interpret_escapes = True
-        elif flag == '-n':
+        elif flag == "-n":
             write_newline = False
 
     def maybeUnescape(arg):
         if not interpret_escapes:
             return arg
 
         arg = lit.util.to_bytes(arg)
-        codec = 'string_escape' if sys.version_info < (3,0) else 'unicode_escape'
+        codec = "string_escape" if sys.version_info < (3, 0) else "unicode_escape"
         return arg.decode(codec)
 
     if args:
         for arg in args[:-1]:
             stdout.write(encode(maybeUnescape(arg)))
-            stdout.write(encode(' '))
+            stdout.write(encode(" "))
         stdout.write(encode(maybeUnescape(args[-1])))
     if write_newline:
-        stdout.write(encode('\n'))
+        stdout.write(encode("\n"))
 
     for (name, mode, f, path) in opened_files:
         f.close()
 
     output = "" if is_redirected else stdout.getvalue()
     return ShellCommandResult(cmd, output, "", 0, False)
 
+
 def executeBuiltinMkdir(cmd, cmd_shenv):
     """executeBuiltinMkdir - Create new directories."""
     args = expand_glob_expressions(cmd.args, cmd_shenv.cwd)[1:]
     try:
-        opts, args = getopt.gnu_getopt(args, 'p')
+        opts, args = getopt.gnu_getopt(args, "p")
     except getopt.GetoptError as err:
         raise InternalShellError(cmd, "Unsupported: 'mkdir':  %s" % str(err))
 
     parent = False
     for o, a in opts:
         if o == "-p":
             parent = True
@@ -408,14 +434,15 @@
             try:
                 lit.util.mkdir(dir)
             except OSError as err:
                 stderr.write("Error: 'mkdir' command failed, %s\n" % str(err))
                 exitCode = 1
     return ShellCommandResult(cmd, "", stderr.getvalue(), exitCode, False)
 
+
 def executeBuiltinRm(cmd, cmd_shenv):
     """executeBuiltinRm - Removes (deletes) files or directories."""
     args = expand_glob_expressions(cmd.args, cmd_shenv.cwd)[1:]
     try:
         opts, args = getopt.gnu_getopt(args, "frR", ["--recursive"])
     except getopt.GetoptError as err:
         raise InternalShellError(cmd, "Unsupported: 'rm':  %s" % str(err))
@@ -432,15 +459,15 @@
 
     if len(args) == 0:
         raise InternalShellError(cmd, "Error: 'rm' is missing an operand")
 
     def on_rm_error(func, path, exc_info):
         # path contains the path of the file that couldn't be removed
         # let's just assume that it's read-only and remove it.
-        os.chmod(path, stat.S_IMODE( os.stat(path).st_mode) | stat.S_IWRITE)
+        os.chmod(path, stat.S_IMODE(os.stat(path).st_mode) | stat.S_IWRITE)
         os.remove(path)
 
     stderr = StringIO()
     exitCode = 0
     for path in args:
         cwd = cmd_shenv.cwd
         path = to_unicode(path) if kIsWindows else to_bytes(path)
@@ -450,103 +477,113 @@
         if force and not os.path.exists(path):
             continue
         try:
             if os.path.isdir(path):
                 if not recursive:
                     stderr.write("Error: %s is a directory\n" % path)
                     exitCode = 1
-                if platform.system() == 'Windows':
+                if platform.system() == "Windows":
                     # NOTE: use ctypes to access `SHFileOperationsW` on Windows to
                     # use the NT style path to get access to long file paths which
                     # cannot be removed otherwise.
                     from ctypes.wintypes import BOOL, HWND, LPCWSTR, UINT, WORD
                     from ctypes import addressof, byref, c_void_p, create_unicode_buffer
                     from ctypes import Structure
                     from ctypes import windll, WinError, POINTER
 
                     class SHFILEOPSTRUCTW(Structure):
                         _fields_ = [
-                                ('hWnd', HWND),
-                                ('wFunc', UINT),
-                                ('pFrom', LPCWSTR),
-                                ('pTo', LPCWSTR),
-                                ('fFlags', WORD),
-                                ('fAnyOperationsAborted', BOOL),
-                                ('hNameMappings', c_void_p),
-                                ('lpszProgressTitle', LPCWSTR),
+                            ("hWnd", HWND),
+                            ("wFunc", UINT),
+                            ("pFrom", LPCWSTR),
+                            ("pTo", LPCWSTR),
+                            ("fFlags", WORD),
+                            ("fAnyOperationsAborted", BOOL),
+                            ("hNameMappings", c_void_p),
+                            ("lpszProgressTitle", LPCWSTR),
                         ]
 
                     FO_MOVE, FO_COPY, FO_DELETE, FO_RENAME = range(1, 5)
 
                     FOF_SILENT = 4
                     FOF_NOCONFIRMATION = 16
                     FOF_NOCONFIRMMKDIR = 512
                     FOF_NOERRORUI = 1024
 
-                    FOF_NO_UI = FOF_SILENT | FOF_NOCONFIRMATION | FOF_NOERRORUI | FOF_NOCONFIRMMKDIR
+                    FOF_NO_UI = (
+                        FOF_SILENT
+                        | FOF_NOCONFIRMATION
+                        | FOF_NOERRORUI
+                        | FOF_NOCONFIRMMKDIR
+                    )
 
                     SHFileOperationW = windll.shell32.SHFileOperationW
                     SHFileOperationW.argtypes = [POINTER(SHFILEOPSTRUCTW)]
 
                     path = os.path.abspath(path)
 
                     pFrom = create_unicode_buffer(path, len(path) + 2)
-                    pFrom[len(path)] = pFrom[len(path) + 1] = '\0'
-                    operation = SHFILEOPSTRUCTW(wFunc=UINT(FO_DELETE),
-                                                pFrom=LPCWSTR(addressof(pFrom)),
-                                                fFlags=FOF_NO_UI)
+                    pFrom[len(path)] = pFrom[len(path) + 1] = "\0"
+                    operation = SHFILEOPSTRUCTW(
+                        wFunc=UINT(FO_DELETE),
+                        pFrom=LPCWSTR(addressof(pFrom)),
+                        fFlags=FOF_NO_UI,
+                    )
                     result = SHFileOperationW(byref(operation))
                     if result:
                         raise WinError(result)
                 else:
-                    shutil.rmtree(path, onerror = on_rm_error if force else None)
+                    shutil.rmtree(path, onerror=on_rm_error if force else None)
             else:
                 if force and not os.access(path, os.W_OK):
-                    os.chmod(path,
-                             stat.S_IMODE(os.stat(path).st_mode) | stat.S_IWRITE)
+                    os.chmod(path, stat.S_IMODE(os.stat(path).st_mode) | stat.S_IWRITE)
                 os.remove(path)
         except OSError as err:
             stderr.write("Error: 'rm' command failed, %s" % str(err))
             exitCode = 1
     return ShellCommandResult(cmd, "", stderr.getvalue(), exitCode, False)
 
+
 def executeBuiltinColon(cmd, cmd_shenv):
     """executeBuiltinColon - Discard arguments and exit with status 0."""
     return ShellCommandResult(cmd, "", "", 0, False)
 
+
 def processRedirects(cmd, stdin_source, cmd_shenv, opened_files):
     """Return the standard fds for cmd after applying redirects
 
     Returns the three standard file descriptors for the new child process.  Each
     fd may be an open, writable file object or a sentinel value from the
     subprocess module.
     """
 
     # Apply the redirections, we use (N,) as a sentinel to indicate stdin,
     # stdout, stderr for N equal to 0, 1, or 2 respectively. Redirects to or
     # from a file are represented with a list [file, mode, file-object]
     # where file-object is initially None.
     redirects = [(0,), (1,), (2,)]
     for (op, filename) in cmd.redirects:
-        if op == ('>',2):
-            redirects[2] = [filename, 'w', None]
-        elif op == ('>>',2):
-            redirects[2] = [filename, 'a', None]
-        elif op == ('>&',2) and filename in '012':
+        if op == (">", 2):
+            redirects[2] = [filename, "w", None]
+        elif op == (">>", 2):
+            redirects[2] = [filename, "a", None]
+        elif op == (">&", 2) and filename in "012":
             redirects[2] = redirects[int(filename)]
-        elif op == ('>&',) or op == ('&>',):
-            redirects[1] = redirects[2] = [filename, 'w', None]
-        elif op == ('>',):
-            redirects[1] = [filename, 'w', None]
-        elif op == ('>>',):
-            redirects[1] = [filename, 'a', None]
-        elif op == ('<',):
-            redirects[0] = [filename, 'r', None]
+        elif op == (">&",) or op == ("&>",):
+            redirects[1] = redirects[2] = [filename, "w", None]
+        elif op == (">",):
+            redirects[1] = [filename, "w", None]
+        elif op == (">>",):
+            redirects[1] = [filename, "a", None]
+        elif op == ("<",):
+            redirects[0] = [filename, "r", None]
         else:
-            raise InternalShellError(cmd, "Unsupported redirect: %r" % ((op, filename),))
+            raise InternalShellError(
+                cmd, "Unsupported redirect: %r" % ((op, filename),)
+            )
 
     # Open file descriptors in a second pass.
     std_fds = [None, None, None]
     for (index, r) in enumerate(redirects):
         # Handle the sentinel values for defaults up front.
         if isinstance(r, tuple):
             if r == (0,):
@@ -574,165 +611,172 @@
         if fd is not None:
             std_fds[index] = fd
             continue
 
         redir_filename = None
         name = expand_glob(filename, cmd_shenv.cwd)
         if len(name) != 1:
-           raise InternalShellError(cmd, "Unsupported: glob in "
-                                    "redirect expanded to multiple files")
+            raise InternalShellError(
+                cmd, "Unsupported: glob in " "redirect expanded to multiple files"
+            )
         name = name[0]
         if kAvoidDevNull and name == kDevNull:
             fd = tempfile.TemporaryFile(mode=mode)
-        elif kIsWindows and name == '/dev/tty':
+        elif kIsWindows and name == "/dev/tty":
             # Simulate /dev/tty on Windows.
             # "CON" is a special filename for the console.
             fd = open("CON", mode)
         else:
             # Make sure relative paths are relative to the cwd.
             redir_filename = os.path.join(cmd_shenv.cwd, name)
-            redir_filename = to_unicode(redir_filename) \
-                    if kIsWindows else to_bytes(redir_filename)
+            redir_filename = (
+                to_unicode(redir_filename) if kIsWindows else to_bytes(redir_filename)
+            )
             fd = open(redir_filename, mode)
         # Workaround a Win32 and/or subprocess bug when appending.
         #
         # FIXME: Actually, this is probably an instance of PR6753.
-        if mode == 'a':
+        if mode == "a":
             fd.seek(0, 2)
         # Mutate the underlying redirect list so that we can redirect stdout
         # and stderr to the same place without opening the file twice.
         r[2] = fd
         opened_files.append((filename, mode, fd) + (redir_filename,))
         std_fds[index] = fd
 
     return std_fds
 
+
 def _executeShCmd(cmd, shenv, results, timeoutHelper):
     if timeoutHelper.timeoutReached():
         # Prevent further recursion if the timeout has been hit
         # as we should try avoid launching more processes.
         return None
 
     if isinstance(cmd, ShUtil.Seq):
-        if cmd.op == ';':
+        if cmd.op == ";":
             res = _executeShCmd(cmd.lhs, shenv, results, timeoutHelper)
             return _executeShCmd(cmd.rhs, shenv, results, timeoutHelper)
 
-        if cmd.op == '&':
-            raise InternalShellError(cmd,"unsupported shell operator: '&'")
+        if cmd.op == "&":
+            raise InternalShellError(cmd, "unsupported shell operator: '&'")
 
-        if cmd.op == '||':
+        if cmd.op == "||":
             res = _executeShCmd(cmd.lhs, shenv, results, timeoutHelper)
             if res != 0:
                 res = _executeShCmd(cmd.rhs, shenv, results, timeoutHelper)
             return res
 
-        if cmd.op == '&&':
+        if cmd.op == "&&":
             res = _executeShCmd(cmd.lhs, shenv, results, timeoutHelper)
             if res is None:
                 return res
 
             if res == 0:
                 res = _executeShCmd(cmd.rhs, shenv, results, timeoutHelper)
             return res
 
-        raise ValueError('Unknown shell command: %r' % cmd.op)
+        raise ValueError("Unknown shell command: %r" % cmd.op)
     assert isinstance(cmd, ShUtil.Pipeline)
 
     procs = []
     proc_not_counts = []
     default_stdin = subprocess.PIPE
     stderrTempFiles = []
     opened_files = []
     named_temp_files = []
-    builtin_commands = set(['cat', 'diff'])
-    builtin_commands_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "builtin_commands")
-    inproc_builtins = {'cd': executeBuiltinCd,
-                       'export': executeBuiltinExport,
-                       'echo': executeBuiltinEcho,
-                       'mkdir': executeBuiltinMkdir,
-                       'popd': executeBuiltinPopd,
-                       'pushd': executeBuiltinPushd,
-                       'rm': executeBuiltinRm,
-                       ':': executeBuiltinColon}
+    builtin_commands = set(["cat", "diff"])
+    builtin_commands_dir = os.path.join(
+        os.path.dirname(os.path.abspath(__file__)), "builtin_commands"
+    )
+    inproc_builtins = {
+        "cd": executeBuiltinCd,
+        "export": executeBuiltinExport,
+        "echo": executeBuiltinEcho,
+        "mkdir": executeBuiltinMkdir,
+        "popd": executeBuiltinPopd,
+        "pushd": executeBuiltinPushd,
+        "rm": executeBuiltinRm,
+        ":": executeBuiltinColon,
+    }
     # To avoid deadlock, we use a single stderr stream for piped
     # output. This is null until we have seen some output using
     # stderr.
-    for i,j in enumerate(cmd.commands):
+    for i, j in enumerate(cmd.commands):
         # Reference the global environment by default.
         cmd_shenv = shenv
         args = list(j.args)
         not_args = []
         not_count = 0
         not_crash = False
         while True:
-            if args[0] == 'env':
+            if args[0] == "env":
                 # Create a copy of the global environment and modify it for
                 # this one command. There might be multiple envs in a pipeline,
                 # and there might be multiple envs in a command (usually when
                 # one comes from a substitution):
                 #   env FOO=1 llc < %s | env BAR=2 llvm-mc | FileCheck %s
                 #   env FOO=1 %{another_env_plus_cmd} | FileCheck %s
                 if cmd_shenv is shenv:
                     cmd_shenv = ShellEnvironment(shenv.cwd, shenv.env)
                 args = updateEnv(cmd_shenv, args)
                 if not args:
-                    raise InternalShellError(j, "Error: 'env' requires a"
-                                                " subcommand")
-            elif args[0] == 'not':
+                    raise InternalShellError(j, "Error: 'env' requires a" " subcommand")
+            elif args[0] == "not":
                 not_args.append(args.pop(0))
                 not_count += 1
-                if args and args[0] == '--crash':
+                if args and args[0] == "--crash":
                     not_args.append(args.pop(0))
                     not_crash = True
                 if not args:
-                    raise InternalShellError(j, "Error: 'not' requires a"
-                                                " subcommand")
-            elif args[0] == '!':
+                    raise InternalShellError(j, "Error: 'not' requires a" " subcommand")
+            elif args[0] == "!":
                 not_args.append(args.pop(0))
                 not_count += 1
                 if not args:
-                    raise InternalShellError(j, "Error: '!' requires a"
-                                                " subcommand")
+                    raise InternalShellError(j, "Error: '!' requires a" " subcommand")
             else:
                 break
 
         # Handle in-process builtins.
         #
         # Handle "echo" as a builtin if it is not part of a pipeline. This
         # greatly speeds up tests that construct input files by repeatedly
         # echo-appending to a file.
         # FIXME: Standardize on the builtin echo implementation. We can use a
         # temporary file to sidestep blocking pipe write issues.
         inproc_builtin = inproc_builtins.get(args[0], None)
-        if inproc_builtin and (args[0] != 'echo' or len(cmd.commands) == 1):
+        if inproc_builtin and (args[0] != "echo" or len(cmd.commands) == 1):
             # env calling an in-process builtin is useless, so we take the safe
             # approach of complaining.
             if not cmd_shenv is shenv:
-                raise InternalShellError(j, "Error: 'env' cannot call '{}'"
-                                            .format(args[0]))
+                raise InternalShellError(
+                    j, "Error: 'env' cannot call '{}'".format(args[0])
+                )
             if not_crash:
-                raise InternalShellError(j, "Error: 'not --crash' cannot call"
-                                            " '{}'".format(args[0]))
+                raise InternalShellError(
+                    j, "Error: 'not --crash' cannot call" " '{}'".format(args[0])
+                )
             if len(cmd.commands) != 1:
-                raise InternalShellError(j, "Unsupported: '{}' cannot be part"
-                                            " of a pipeline".format(args[0]))
+                raise InternalShellError(
+                    j,
+                    "Unsupported: '{}' cannot be part" " of a pipeline".format(args[0]),
+                )
             result = inproc_builtin(Command(args, j.redirects), cmd_shenv)
             if not_count % 2:
                 result.exitCode = int(not result.exitCode)
-            result.command.args = j.args;
+            result.command.args = j.args
             results.append(result)
             return result.exitCode
 
         # Resolve any out-of-process builtin command before adding back 'not'
         # commands.
         if args[0] in builtin_commands:
             args.insert(0, sys.executable)
-            cmd_shenv.env['PYTHONPATH'] = \
-                os.path.dirname(os.path.abspath(__file__))
+            cmd_shenv.env["PYTHONPATH"] = os.path.dirname(os.path.abspath(__file__))
             args[1] = os.path.join(builtin_commands_dir, args[1] + ".py")
 
         # We had to search through the 'not' commands to find all the 'env'
         # commands and any other in-process builtin command.  We don't want to
         # reimplement 'not' and its '--crash' here, so just push all 'not'
         # commands back to be called as external commands.  Because this
         # approach effectively moves all 'env' commands up front, it relies on
@@ -745,54 +789,55 @@
         # invert the result code afterwards.
         if not_crash:
             args = not_args + args
             not_count = 0
         else:
             not_args = []
 
-        stdin, stdout, stderr = processRedirects(j, default_stdin, cmd_shenv,
-                                                 opened_files)
+        stdin, stdout, stderr = processRedirects(
+            j, default_stdin, cmd_shenv, opened_files
+        )
 
         # If stderr wants to come from stdout, but stdout isn't a pipe, then put
         # stderr on a pipe and treat it as stdout.
-        if (stderr == subprocess.STDOUT and stdout != subprocess.PIPE):
+        if stderr == subprocess.STDOUT and stdout != subprocess.PIPE:
             stderr = subprocess.PIPE
             stderrIsStdout = True
         else:
             stderrIsStdout = False
 
             # Don't allow stderr on a PIPE except for the last
             # process, this could deadlock.
             #
             # FIXME: This is slow, but so is deadlock.
             if stderr == subprocess.PIPE and j != cmd.commands[-1]:
-                stderr = tempfile.TemporaryFile(mode='w+b')
+                stderr = tempfile.TemporaryFile(mode="w+b")
                 stderrTempFiles.append((i, stderr))
 
         # Resolve the executable path ourselves.
         executable = None
         # For paths relative to cwd, use the cwd of the shell environment.
-        if args[0].startswith('.'):
+        if args[0].startswith("."):
             exe_in_cwd = os.path.join(cmd_shenv.cwd, args[0])
             if os.path.isfile(exe_in_cwd):
                 executable = exe_in_cwd
         if not executable:
-            executable = lit.util.which(args[0], cmd_shenv.env['PATH'])
+            executable = lit.util.which(args[0], cmd_shenv.env["PATH"])
         if not executable:
-            raise InternalShellError(j, '%r: command not found' % args[0])
+            raise InternalShellError(j, "%r: command not found" % args[0])
 
         # Replace uses of /dev/null with temporary files.
         if kAvoidDevNull:
             # In Python 2.x, basestring is the base class for all string (including unicode)
             # In Python 3.x, basestring no longer exist and str is always unicode
             try:
                 str_type = basestring
             except NameError:
                 str_type = str
-            for i,arg in enumerate(args):
+            for i, arg in enumerate(args):
                 if isinstance(arg, str_type) and kDevNull in arg:
                     f = tempfile.NamedTemporaryFile(delete=False)
                     f.close()
                     named_temp_files.append(f.name)
                     args[i] = arg.replace(kDevNull, f.name)
 
         # Expand all glob expressions
@@ -800,28 +845,35 @@
 
         # On Windows, do our own command line quoting for better compatibility
         # with some core utility distributions.
         if kIsWindows:
             args = quote_windows_command(args)
 
         try:
-            procs.append(subprocess.Popen(args, cwd=cmd_shenv.cwd,
-                                          executable = executable,
-                                          stdin = stdin,
-                                          stdout = stdout,
-                                          stderr = stderr,
-                                          env = cmd_shenv.env,
-                                          close_fds = kUseCloseFDs,
-                                          universal_newlines = True,
-                                          errors = 'replace'))
+            procs.append(
+                subprocess.Popen(
+                    args,
+                    cwd=cmd_shenv.cwd,
+                    executable=executable,
+                    stdin=stdin,
+                    stdout=stdout,
+                    stderr=stderr,
+                    env=cmd_shenv.env,
+                    close_fds=kUseCloseFDs,
+                    universal_newlines=True,
+                    errors="replace",
+                )
+            )
             proc_not_counts.append(not_count)
             # Let the helper know about this process
             timeoutHelper.addProcess(procs[-1])
         except OSError as e:
-            raise InternalShellError(j, 'Could not create process ({}) due to {}'.format(executable, e))
+            raise InternalShellError(
+                j, "Could not create process ({}) due to {}".format(executable, e)
+            )
 
         # Immediately close stdin for any process taking stdin from us.
         if stdin == subprocess.PIPE:
             procs[-1].stdin.close()
             procs[-1].stdin = None
 
         # Update the current stdin source.
@@ -843,70 +895,77 @@
     procData = [None] * len(procs)
     procData[-1] = procs[-1].communicate()
 
     for i in range(len(procs) - 1):
         if procs[i].stdout is not None:
             out = procs[i].stdout.read()
         else:
-            out = ''
+            out = ""
         if procs[i].stderr is not None:
             err = procs[i].stderr.read()
         else:
-            err = ''
-        procData[i] = (out,err)
+            err = ""
+        procData[i] = (out, err)
 
     # Read stderr out of the temp files.
-    for i,f in stderrTempFiles:
+    for i, f in stderrTempFiles:
         f.seek(0, 0)
         procData[i] = (procData[i][0], f.read())
         f.close()
 
     exitCode = None
-    for i,(out,err) in enumerate(procData):
+    for i, (out, err) in enumerate(procData):
         res = procs[i].wait()
         # Detect Ctrl-C in subprocess.
         if res == -signal.SIGINT:
             raise KeyboardInterrupt
         if proc_not_counts[i] % 2:
             res = not res
         elif proc_not_counts[i] > 1:
             res = 1 if res != 0 else 0
 
         # Ensure the resulting output is always of string type.
         try:
             if out is None:
-                out = ''
+                out = ""
             else:
-                out = to_string(out.decode('utf-8', errors='replace'))
+                out = to_string(out.decode("utf-8", errors="replace"))
         except:
             out = str(out)
         try:
             if err is None:
-                err = ''
+                err = ""
             else:
-                err = to_string(err.decode('utf-8', errors='replace'))
+                err = to_string(err.decode("utf-8", errors="replace"))
         except:
             err = str(err)
 
         # Gather the redirected output files for failed commands.
         output_files = []
         if res != 0:
             for (name, mode, f, path) in sorted(opened_files):
-                if path is not None and mode in ('w', 'a'):
+                if path is not None and mode in ("w", "a"):
                     try:
-                        with open(path, 'rb') as f:
+                        with open(path, "rb") as f:
                             data = f.read()
                     except:
                         data = None
                     if data is not None:
                         output_files.append((name, path, data))
 
-        results.append(ShellCommandResult(
-            cmd.commands[i], out, err, res, timeoutHelper.timeoutReached(),
-            output_files))
+        results.append(
+            ShellCommandResult(
+                cmd.commands[i],
+                out,
+                err,
+                res,
+                timeoutHelper.timeoutReached(),
+                output_files,
+            )
+        )
         if cmd.pipe_err:
             # Take the last failing exit code from the pipeline.
             if not exitCode or res != 0:
                 exitCode = res
         else:
             exitCode = res
 
@@ -918,158 +977,166 @@
             pass
 
     if cmd.negate:
         exitCode = not exitCode
 
     return exitCode
 
+
 def executeScriptInternal(test, litConfig, tmpBase, commands, cwd):
     cmds = []
     for i, ln in enumerate(commands):
         match = re.match(kPdbgRegex, ln)
         if match:
             command = match.group(2)
-            ln = commands[i] = \
-                match.expand(": '\\1'; \\2" if command else ": '\\1'")
+            ln = commands[i] = match.expand(": '\\1'; \\2" if command else ": '\\1'")
         try:
-            cmds.append(ShUtil.ShParser(ln, litConfig.isWindows,
-                                        test.config.pipefail).parse())
+            cmds.append(
+                ShUtil.ShParser(ln, litConfig.isWindows, test.config.pipefail).parse()
+            )
         except:
             return lit.Test.Result(Test.FAIL, "shell parser error on: %r" % ln)
 
     cmd = cmds[0]
     for c in cmds[1:]:
-        cmd = ShUtil.Seq(cmd, '&&', c)
+        cmd = ShUtil.Seq(cmd, "&&", c)
 
     results = []
     timeoutInfo = None
     try:
         shenv = ShellEnvironment(cwd, test.config.environment)
-        exitCode, timeoutInfo = executeShCmd(cmd, shenv, results, timeout=litConfig.maxIndividualTestTime)
+        exitCode, timeoutInfo = executeShCmd(
+            cmd, shenv, results, timeout=litConfig.maxIndividualTestTime
+        )
     except InternalShellError:
         e = sys.exc_info()[1]
         exitCode = 127
-        results.append(
-            ShellCommandResult(e.command, '', e.message, exitCode, False))
+        results.append(ShellCommandResult(e.command, "", e.message, exitCode, False))
 
-    out = err = ''
-    for i,result in enumerate(results):
+    out = err = ""
+    for i, result in enumerate(results):
         # Write the command line run.
-        out += '$ %s\n' % (' '.join('"%s"' % s
-                                    for s in result.command.args),)
+        out += "$ %s\n" % (" ".join('"%s"' % s for s in result.command.args),)
 
         # If nothing interesting happened, move on.
-        if litConfig.maxIndividualTestTime == 0 and \
-               result.exitCode == 0 and \
-               not result.stdout.strip() and not result.stderr.strip():
+        if (
+            litConfig.maxIndividualTestTime == 0
+            and result.exitCode == 0
+            and not result.stdout.strip()
+            and not result.stderr.strip()
+        ):
             continue
 
         # Otherwise, something failed or was printed, show it.
 
         # Add the command output, if redirected.
         for (name, path, data) in result.outputFiles:
             if data.strip():
                 out += "# redirected output from %r:\n" % (name,)
-                data = to_string(data.decode('utf-8', errors='replace'))
+                data = to_string(data.decode("utf-8", errors="replace"))
                 if len(data) > 1024:
                     out += data[:1024] + "\n...\n"
                     out += "note: data was truncated\n"
                 else:
                     out += data
                 out += "\n"
 
         if result.stdout.strip():
-            out += '# command output:\n%s\n' % (result.stdout,)
+            out += "# command output:\n%s\n" % (result.stdout,)
         if result.stderr.strip():
-            out += '# command stderr:\n%s\n' % (result.stderr,)
+            out += "# command stderr:\n%s\n" % (result.stderr,)
         if not result.stdout.strip() and not result.stderr.strip():
             out += "note: command had no output on stdout or stderr\n"
 
         # Show the error conditions:
         if result.exitCode != 0:
             # On Windows, a negative exit code indicates a signal, and those are
             # easier to recognize or look up if we print them in hex.
             if litConfig.isWindows and (result.exitCode < 0 or result.exitCode > 255):
                 codeStr = hex(int(result.exitCode & 0xFFFFFFFF)).rstrip("L")
             else:
                 codeStr = str(result.exitCode)
-            out += "error: command failed with exit status: %s\n" % (
-                codeStr,)
+            out += "error: command failed with exit status: %s\n" % (codeStr,)
         if litConfig.maxIndividualTestTime > 0 and result.timeoutReached:
-            out += 'error: command reached timeout: %s\n' % (
-                str(result.timeoutReached),)
+            out += "error: command reached timeout: %s\n" % (
+                str(result.timeoutReached),
+            )
 
     return out, err, exitCode, timeoutInfo
 
+
 def executeScript(test, litConfig, tmpBase, commands, cwd):
     bashPath = litConfig.getBashPath()
-    isWin32CMDEXE = (litConfig.isWindows and not bashPath)
-    script = tmpBase + '.script'
+    isWin32CMDEXE = litConfig.isWindows and not bashPath
+    script = tmpBase + ".script"
     if isWin32CMDEXE:
-        script += '.bat'
+        script += ".bat"
 
     # Write script file
-    mode = 'w'
+    mode = "w"
     open_kwargs = {}
     if litConfig.isWindows and not isWin32CMDEXE:
-        mode += 'b'  # Avoid CRLFs when writing bash scripts.
-    elif sys.version_info > (3,0):
-        open_kwargs['encoding'] = 'utf-8'
+        mode += "b"  # Avoid CRLFs when writing bash scripts.
+    elif sys.version_info > (3, 0):
+        open_kwargs["encoding"] = "utf-8"
     f = open(script, mode, **open_kwargs)
     if isWin32CMDEXE:
         for i, ln in enumerate(commands):
             match = re.match(kPdbgRegex, ln)
             if match:
                 command = match.group(2)
-                commands[i] = \
-                    match.expand("echo '\\1' > nul && " if command
-                                 else "echo '\\1' > nul")
+                commands[i] = match.expand(
+                    "echo '\\1' > nul && " if command else "echo '\\1' > nul"
+                )
         if litConfig.echo_all_commands:
-            f.write('@echo on\n')
+            f.write("@echo on\n")
         else:
-            f.write('@echo off\n')
-        f.write('\n@if %ERRORLEVEL% NEQ 0 EXIT\n'.join(commands))
+            f.write("@echo off\n")
+        f.write("\n@if %ERRORLEVEL% NEQ 0 EXIT\n".join(commands))
     else:
         for i, ln in enumerate(commands):
             match = re.match(kPdbgRegex, ln)
             if match:
                 command = match.group(2)
-                commands[i] = match.expand(": '\\1'; \\2" if command
-                                           else ": '\\1'")
+                commands[i] = match.expand(": '\\1'; \\2" if command else ": '\\1'")
         if test.config.pipefail:
-            f.write(b'set -o pipefail;' if mode == 'wb' else 'set -o pipefail;')
+            f.write(b"set -o pipefail;" if mode == "wb" else "set -o pipefail;")
         if litConfig.echo_all_commands:
-            f.write(b'set -x;' if mode == 'wb' else 'set -x;')
-        if sys.version_info > (3,0) and mode == 'wb':
-            f.write(bytes('{ ' + '; } &&\n{ '.join(commands) + '; }', 'utf-8'))
+            f.write(b"set -x;" if mode == "wb" else "set -x;")
+        if sys.version_info > (3, 0) and mode == "wb":
+            f.write(bytes("{ " + "; } &&\n{ ".join(commands) + "; }", "utf-8"))
         else:
-            f.write('{ ' + '; } &&\n{ '.join(commands) + '; }')
-    f.write(b'\n' if mode == 'wb' else '\n')
+            f.write("{ " + "; } &&\n{ ".join(commands) + "; }")
+    f.write(b"\n" if mode == "wb" else "\n")
     f.close()
 
     if isWin32CMDEXE:
-        command = ['cmd','/c', script]
+        command = ["cmd", "/c", script]
     else:
         if bashPath:
             command = [bashPath, script]
         else:
-            command = ['/bin/sh', script]
+            command = ["/bin/sh", script]
         if litConfig.useValgrind:
             # FIXME: Running valgrind on sh is overkill. We probably could just
             # run on clang with no real loss.
             command = litConfig.valgrindArgs + command
 
     try:
-        out, err, exitCode = lit.util.executeCommand(command, cwd=cwd,
-                                       env=test.config.environment,
-                                       timeout=litConfig.maxIndividualTestTime)
+        out, err, exitCode = lit.util.executeCommand(
+            command,
+            cwd=cwd,
+            env=test.config.environment,
+            timeout=litConfig.maxIndividualTestTime,
+        )
         return (out, err, exitCode, None)
     except lit.util.ExecuteCommandTimeoutException as e:
         return (e.out, e.err, e.exitCode, e.msg)
 
+
 def parseIntegratedTestScriptCommands(source_path, keywords):
     """
     parseIntegratedTestScriptCommands(source_path) -> commands
 
     Parse the commands in an integrated test script file into a list of
     (line_number, command_type, line).
     """
@@ -1082,147 +1149,171 @@
     #
     # Once we find a match, we do require each script line to be decodable to
     # UTF-8, so we convert the outputs to UTF-8 before returning. This way the
     # remaining code can work with "strings" agnostic of the executing Python
     # version.
 
     keywords_re = re.compile(
-        to_bytes("(%s)(.*)\n" % ("|".join(re.escape(k) for k in keywords),)))
+        to_bytes("(%s)(.*)\n" % ("|".join(re.escape(k) for k in keywords),))
+    )
 
-    f = open(source_path, 'rb')
+    f = open(source_path, "rb")
     try:
         # Read the entire file contents.
         data = f.read()
 
         # Ensure the data ends with a newline.
-        if not data.endswith(to_bytes('\n')):
-            data = data + to_bytes('\n')
+        if not data.endswith(to_bytes("\n")):
+            data = data + to_bytes("\n")
 
         # Iterate over the matches.
         line_number = 1
         last_match_position = 0
         for match in keywords_re.finditer(data):
             # Compute the updated line number by counting the intervening
             # newlines.
             match_position = match.start()
-            line_number += data.count(to_bytes('\n'), last_match_position,
-                                      match_position)
+            line_number += data.count(
+                to_bytes("\n"), last_match_position, match_position
+            )
             last_match_position = match_position
 
             # Convert the keyword and line to UTF-8 strings and yield the
             # command. Note that we take care to return regular strings in
             # Python 2, to avoid other code having to differentiate between the
             # str and unicode types.
             #
             # Opening the file in binary mode prevented Windows \r newline
             # characters from being converted to Unix \n newlines, so manually
             # strip those from the yielded lines.
-            keyword,ln = match.groups()
-            yield (line_number, to_string(keyword.decode('utf-8')),
-                   to_string(ln.decode('utf-8').rstrip('\r')))
+            keyword, ln = match.groups()
+            yield (
+                line_number,
+                to_string(keyword.decode("utf-8")),
+                to_string(ln.decode("utf-8").rstrip("\r")),
+            )
     finally:
         f.close()
 
+
 def getTempPaths(test):
     """Get the temporary location, this is always relative to the test suite
     root, not test source root."""
     execpath = test.getExecPath()
-    execdir,execbase = os.path.split(execpath)
-    tmpDir = os.path.join(execdir, 'Output')
+    execdir, execbase = os.path.split(execpath)
+    tmpDir = os.path.join(execdir, "Output")
     tmpBase = os.path.join(tmpDir, execbase)
     return tmpDir, tmpBase
 
+
 def colonNormalizePath(path):
     if kIsWindows:
-        return re.sub(r'^(.):', r'\1', path.replace('\\', '/'))
+        return re.sub(r"^(.):", r"\1", path.replace("\\", "/"))
     else:
-        assert path[0] == '/'
+        assert path[0] == "/"
         return path[1:]
 
+
 def getDefaultSubstitutions(test, tmpDir, tmpBase, normalize_slashes=False):
     sourcepath = test.getSourcePath()
     sourcedir = os.path.dirname(sourcepath)
 
     # Normalize slashes, if requested.
     if normalize_slashes:
-        sourcepath = sourcepath.replace('\\', '/')
-        sourcedir = sourcedir.replace('\\', '/')
-        tmpDir = tmpDir.replace('\\', '/')
-        tmpBase = tmpBase.replace('\\', '/')
+        sourcepath = sourcepath.replace("\\", "/")
+        sourcedir = sourcedir.replace("\\", "/")
+        tmpDir = tmpDir.replace("\\", "/")
+        tmpBase = tmpBase.replace("\\", "/")
 
     substitutions = []
     substitutions.extend(test.config.substitutions)
-    tmpName = tmpBase + '.tmp'
+    tmpName = tmpBase + ".tmp"
     baseName = os.path.basename(tmpBase)
-    substitutions.extend([('%s', sourcepath),
-                          ('%S', sourcedir),
-                          ('%p', sourcedir),
-                          ('%{pathsep}', os.pathsep),
-                          ('%t', tmpName),
-                          ('%basename_t', baseName),
-                          ('%T', tmpDir)])
-
-    substitutions.extend([
-        ('%{fs-src-root}', pathlib.Path(sourcedir).anchor),
-        ('%{fs-tmp-root}', pathlib.Path(tmpBase).anchor),
-        ('%{fs-sep}', os.path.sep),
-    ])
+    substitutions.extend(
+        [
+            ("%s", sourcepath),
+            ("%S", sourcedir),
+            ("%p", sourcedir),
+            ("%{pathsep}", os.pathsep),
+            ("%t", tmpName),
+            ("%basename_t", baseName),
+            ("%T", tmpDir),
+        ]
+    )
+
+    substitutions.extend(
+        [
+            ("%{fs-src-root}", pathlib.Path(sourcedir).anchor),
+            ("%{fs-tmp-root}", pathlib.Path(tmpBase).anchor),
+            ("%{fs-sep}", os.path.sep),
+        ]
+    )
 
     # "%/[STpst]" should be normalized.
-    substitutions.extend([
-            ('%/s', sourcepath.replace('\\', '/')),
-            ('%/S', sourcedir.replace('\\', '/')),
-            ('%/p', sourcedir.replace('\\', '/')),
-            ('%/t', tmpBase.replace('\\', '/') + '.tmp'),
-            ('%/T', tmpDir.replace('\\', '/')),
-            ('%/et',tmpName.replace('\\', '\\\\\\\\\\\\\\\\')),
-            ])
+    substitutions.extend(
+        [
+            ("%/s", sourcepath.replace("\\", "/")),
+            ("%/S", sourcedir.replace("\\", "/")),
+            ("%/p", sourcedir.replace("\\", "/")),
+            ("%/t", tmpBase.replace("\\", "/") + ".tmp"),
+            ("%/T", tmpDir.replace("\\", "/")),
+            ("%/et", tmpName.replace("\\", "\\\\\\\\\\\\\\\\")),
+        ]
+    )
 
     # "%{/[STpst]:regex_replacement}" should be normalized like "%/[STpst]" but we're
     # also in a regex replacement context of a s@@@ regex.
     def regex_escape(s):
-        s = s.replace('@', r'\@')
-        s = s.replace('&', r'\&')
+        s = s.replace("@", r"\@")
+        s = s.replace("&", r"\&")
         return s
-    substitutions.extend([
-            ('%{/s:regex_replacement}',
-             regex_escape(sourcepath.replace('\\', '/'))),
-            ('%{/S:regex_replacement}',
-             regex_escape(sourcedir.replace('\\', '/'))),
-            ('%{/p:regex_replacement}',
-             regex_escape(sourcedir.replace('\\', '/'))),
-            ('%{/t:regex_replacement}',
-             regex_escape(tmpBase.replace('\\', '/')) + '.tmp'),
-            ('%{/T:regex_replacement}',
-             regex_escape(tmpDir.replace('\\', '/'))),
-            ])
+
+    substitutions.extend(
+        [
+            ("%{/s:regex_replacement}", regex_escape(sourcepath.replace("\\", "/"))),
+            ("%{/S:regex_replacement}", regex_escape(sourcedir.replace("\\", "/"))),
+            ("%{/p:regex_replacement}", regex_escape(sourcedir.replace("\\", "/"))),
+            (
+                "%{/t:regex_replacement}",
+                regex_escape(tmpBase.replace("\\", "/")) + ".tmp",
+            ),
+            ("%{/T:regex_replacement}", regex_escape(tmpDir.replace("\\", "/"))),
+        ]
+    )
 
     # "%:[STpst]" are normalized paths without colons and without a leading
     # slash.
-    substitutions.extend([
-            ('%:s', colonNormalizePath(sourcepath)),
-            ('%:S', colonNormalizePath(sourcedir)),
-            ('%:p', colonNormalizePath(sourcedir)),
-            ('%:t', colonNormalizePath(tmpBase + '.tmp')),
-            ('%:T', colonNormalizePath(tmpDir)),
-            ])
+    substitutions.extend(
+        [
+            ("%:s", colonNormalizePath(sourcepath)),
+            ("%:S", colonNormalizePath(sourcedir)),
+            ("%:p", colonNormalizePath(sourcedir)),
+            ("%:t", colonNormalizePath(tmpBase + ".tmp")),
+            ("%:T", colonNormalizePath(tmpDir)),
+        ]
+    )
     return substitutions
 
+
 def _memoize(f):
     cache = {}  # Intentionally unbounded, see applySubstitutions()
+
     def memoized(x):
         if x not in cache:
             cache[x] = f(x)
         return cache[x]
+
     return memoized
 
+
 @_memoize
 def _caching_re_compile(r):
     return re.compile(r)
 
+
 class ExpandableScriptDirective(object):
     """
     Common interface for lit directives for which any lit substitutions must be
     expanded to produce the shell script.  It includes directives (e.g., 'RUN:')
     specifying shell commands that might have lit substitutions to be expanded.
     It also includes lit directives (e.g., 'DEFINE:') that adjust substitutions.
 
@@ -1266,16 +1357,17 @@
 
     def get_location(self):
         """
         Get a phrase describing the line or range of lines so far included by
         this directive and any line continuations.
         """
         if self.start_line_number == self.end_line_number:
-            return f'at line {self.start_line_number}'
-        return f'from line {self.start_line_number} to {self.end_line_number}'
+            return f"at line {self.start_line_number}"
+        return f"from line {self.start_line_number} to {self.end_line_number}"
+
 
 class CommandDirective(ExpandableScriptDirective):
     """
     A lit directive taking a shell command line.  For example,
     'RUN: echo hello world'.
 
     command: The content accumulated so far from the directive and its
@@ -1292,15 +1384,16 @@
         self.command = self.command[:-1] + line.rstrip()
         self.end_line_number = line_number
         return True
 
     def needs_continuation(self):
         # Trailing whitespace is stripped immediately when each line is added,
         # so '\' is never hidden here.
-        return self.command[-1] == '\\'
+        return self.command[-1] == "\\"
+
 
 class SubstDirective(ExpandableScriptDirective):
     """
     A lit directive taking a substitution definition or redefinition.  For
     example, 'DEFINE: %{name} = value'.
 
     new_subst: True if this directive defines a new substitution.  False if it
@@ -1309,50 +1402,49 @@
         continuation lines.
     name: The substitution's name, or None if more continuation lines are still
         required.
     value: The substitution's value, or None if more continuation lines are
         still required.
     """
 
-    def __init__(self, start_line_number, end_line_number, keyword, new_subst,
-                 line):
+    def __init__(self, start_line_number, end_line_number, keyword, new_subst, line):
         super().__init__(start_line_number, end_line_number, keyword)
         self.new_subst = new_subst
         self.body = line
         self.name = None
         self.value = None
         self._parse_body()
 
     def add_continuation(self, line_number, keyword, line):
         if keyword != self.keyword or not self.needs_continuation():
             return False
         if not line.strip():
             raise ValueError("Substitution's continuation is empty")
         # Append line.  Replace the '\' and any adjacent whitespace with a
         # single space.
-        self.body = self.body.rstrip()[:-1].rstrip() + ' ' + line.lstrip()
+        self.body = self.body.rstrip()[:-1].rstrip() + " " + line.lstrip()
         self.end_line_number = line_number
         self._parse_body()
         return True
 
     def needs_continuation(self):
-        return self.body.rstrip()[-1:] == '\\'
+        return self.body.rstrip()[-1:] == "\\"
 
     def _parse_body(self):
         """
         If no more line continuations are required, parse all the directive's
         accumulated lines in order to identify the substitution's name and full
         value, and raise an exception if invalid.
         """
         if self.needs_continuation():
             return
 
         # Extract the left-hand side and value, and discard any whitespace
         # enclosing each.
-        parts = self.body.split('=', 1)
+        parts = self.body.split("=", 1)
         if len(parts) == 1:
             raise ValueError("Substitution's definition does not contain '='")
         self.name = parts[0].strip()
         self.value = parts[1].strip()
 
         # Check the substitution's name.
         #
@@ -1365,147 +1457,153 @@
         # (e.g., '\.' vs. '[.]') in order for REDEFINE to successfully redefine
         # a substitution previously defined by a lit configuration file.  All
         # this seems too error prone and confusing to be worthwhile.  If you
         # want your name to express structure, use ':' instead of '.'.
         #
         # Actually, '{' and '}' are special if they contain only digits possibly
         # separated by a comma.  Requiring a leading letter avoids that.
-        if not re.fullmatch(r'%{[_a-zA-Z][-_:0-9a-zA-Z]*}', self.name):
+        if not re.fullmatch(r"%{[_a-zA-Z][-_:0-9a-zA-Z]*}", self.name):
             raise ValueError(
                 f"Substitution name '{self.name}' is malformed as it must "
                 f"start with '%{{', it must end with '}}', and the rest must "
                 f"start with a letter or underscore and contain only "
-                f"alphanumeric characters, hyphens, underscores, and colons")
+                f"alphanumeric characters, hyphens, underscores, and colons"
+            )
 
     def adjust_substitutions(self, substitutions):
         """
         Modify the specified substitution list as specified by this directive.
         """
-        assert not self.needs_continuation(), \
-               "expected directive continuations to be parsed before applying"
-        value_repl = self.value.replace('\\', '\\\\')
-        existing = [i for i, subst in enumerate(substitutions)
-                    if self.name in subst[0]]
-        existing_res = ''.join("\nExisting pattern: " + substitutions[i][0]
-                               for i in existing)
+        assert (
+            not self.needs_continuation()
+        ), "expected directive continuations to be parsed before applying"
+        value_repl = self.value.replace("\\", "\\\\")
+        existing = [i for i, subst in enumerate(substitutions) if self.name in subst[0]]
+        existing_res = "".join(
+            "\nExisting pattern: " + substitutions[i][0] for i in existing
+        )
         if self.new_subst:
             if existing:
                 raise ValueError(
                     f"Substitution whose pattern contains '{self.name}' is "
                     f"already defined before '{self.keyword}' directive "
                     f"{self.get_location()}"
-                    f"{existing_res}")
+                    f"{existing_res}"
+                )
             substitutions.insert(0, (self.name, value_repl))
             return
         if len(existing) > 1:
             raise ValueError(
                 f"Multiple substitutions whose patterns contain '{self.name}' "
                 f"are defined before '{self.keyword}' directive "
                 f"{self.get_location()}"
-                f"{existing_res}")
+                f"{existing_res}"
+            )
         if not existing:
             raise ValueError(
                 f"No substitution for '{self.name}' is defined before "
-                f"'{self.keyword}' directive {self.get_location()}")
+                f"'{self.keyword}' directive {self.get_location()}"
+            )
         if substitutions[existing[0]][0] != self.name:
             raise ValueError(
                 f"Existing substitution whose pattern contains '{self.name}' "
                 f"does not have the pattern specified by '{self.keyword}' "
                 f"directive {self.get_location()}\n"
                 f"Expected pattern: {self.name}"
-                f"{existing_res}")
+                f"{existing_res}"
+            )
         substitutions[existing[0]] = (self.name, value_repl)
 
 
-def applySubstitutions(script, substitutions, conditions={},
-                       recursion_limit=None):
+def applySubstitutions(script, substitutions, conditions={}, recursion_limit=None):
     """
     Apply substitutions to the script.  Allow full regular expression syntax.
     Replace each matching occurrence of regular expression pattern a with
     substitution b in line ln.
 
     If a substitution expands into another substitution, it is expanded
     recursively until the line has no more expandable substitutions. If
     the line can still can be substituted after being substituted
     `recursion_limit` times, it is an error. If the `recursion_limit` is
     `None` (the default), no recursive substitution is performed at all.
     """
 
     # We use #_MARKER_# to hide %% while we do the other substitutions.
     def escapePercents(ln):
-        return _caching_re_compile('%%').sub('#_MARKER_#', ln)
+        return _caching_re_compile("%%").sub("#_MARKER_#", ln)
 
     def unescapePercents(ln):
-        return _caching_re_compile('#_MARKER_#').sub('%', ln)
+        return _caching_re_compile("#_MARKER_#").sub("%", ln)
 
     def substituteIfElse(ln):
         # early exit to avoid wasting time on lines without
         # conditional substitutions
-        if ln.find('%if ') == -1:
+        if ln.find("%if ") == -1:
             return ln
 
         def tryParseIfCond(ln):
             # space is important to not conflict with other (possible)
             # substitutions
-            if not ln.startswith('%if '):
+            if not ln.startswith("%if "):
                 return None, ln
             ln = ln[4:]
 
             # stop at '%{'
-            match = _caching_re_compile('%{').search(ln)
+            match = _caching_re_compile("%{").search(ln)
             if not match:
                 raise ValueError("'%{' is missing for %if substitution")
-            cond = ln[:match.start()]
+            cond = ln[: match.start()]
 
             # eat '%{' as well
-            ln = ln[match.end():]
+            ln = ln[match.end() :]
             return cond, ln
 
         def tryParseElse(ln):
-            match = _caching_re_compile('^\s*%else\s*(%{)?').search(ln)
+            match = _caching_re_compile("^\s*%else\s*(%{)?").search(ln)
             if not match:
                 return False, ln
             if not match.group(1):
                 raise ValueError("'%{' is missing for %else substitution")
-            return True, ln[match.end():]
+            return True, ln[match.end() :]
 
         def tryParseEnd(ln):
-            if ln.startswith('%}'):
+            if ln.startswith("%}"):
                 return True, ln[2:]
             return False, ln
 
         def parseText(ln, isNested):
             # parse everything until %if, or %} if we're parsing a
             # nested expression.
             match = _caching_re_compile(
-                '(.*?)(?:%if|%})' if isNested else '(.*?)(?:%if)').search(ln)
+                "(.*?)(?:%if|%})" if isNested else "(.*?)(?:%if)"
+            ).search(ln)
             if not match:
                 # there is no terminating pattern, so treat the whole
                 # line as text
-                return ln, ''
+                return ln, ""
             text_end = match.end(1)
             return ln[:text_end], ln[text_end:]
 
         def parseRecursive(ln, isNested):
-            result = ''
+            result = ""
             while len(ln):
                 if isNested:
                     found_end, _ = tryParseEnd(ln)
                     if found_end:
                         break
 
                 # %if cond %{ branch_if %} %else %{ branch_else %}
                 cond, ln = tryParseIfCond(ln)
                 if cond:
                     branch_if, ln = parseRecursive(ln, isNested=True)
                     found_end, ln = tryParseEnd(ln)
                     if not found_end:
                         raise ValueError("'%}' is missing for %if substitution")
 
-                    branch_else = ''
+                    branch_else = ""
                     found_else, ln = tryParseElse(ln)
                     if found_else:
                         branch_else, ln = parseRecursive(ln, isNested=True)
                         found_end, ln = tryParseEnd(ln)
                         if not found_end:
                             raise ValueError("'%}' is missing for %else substitution")
 
@@ -1524,17 +1622,17 @@
         result, ln = parseRecursive(ln, isNested=False)
         assert len(ln) == 0
         return result
 
     def processLine(ln):
         # Apply substitutions
         ln = substituteIfElse(escapePercents(ln))
-        for a,b in substitutions:
+        for a, b in substitutions:
             if kIsWindows:
-                b = b.replace("\\","\\\\")
+                b = b.replace("\\", "\\\\")
             # re.compile() has a built-in LRU cache with 512 entries. In some
             # test suites lit ends up thrashing that cache, which made e.g.
             # check-llvm run 50% slower.  Use an explicit, unbounded cache
             # to prevent that from happening.  Since lit is fairly
             # short-lived, since the set of substitutions is fairly small, and
             # since thrashing has such bad consequences, not bounding the cache
             # seems reasonable.
@@ -1550,17 +1648,18 @@
         processed = processLine(ln)
         while processed != ln and steps < recursion_limit:
             ln = processed
             processed = processLine(ln)
             steps += 1
 
         if processed != ln:
-            raise ValueError("Recursive substitution of '%s' did not complete "
-                             "in the provided recursion limit (%s)" % \
-                             (origLine, recursion_limit))
+            raise ValueError(
+                "Recursive substitution of '%s' did not complete "
+                "in the provided recursion limit (%s)" % (origLine, recursion_limit)
+            )
 
         return processed
 
     process = processLine if recursion_limit is None else processLineToFixedPoint
     output = []
     for directive in script:
         if isinstance(directive, SubstDirective):
@@ -1590,416 +1689,439 @@
     INTEGER: A keyword taking a single integer. Ex 'ALLOW_RETRIES:'
     CUSTOM: A keyword with custom parsing semantics.
     DEFINE: A keyword taking a new lit substitution definition. Ex
         'DEFINE: %{name}=value'
     REDEFINE: A keyword taking a lit substitution redefinition. Ex
         'REDEFINE: %{name}=value'
     """
+
     TAG = 0
     COMMAND = 1
     LIST = 2
     BOOLEAN_EXPR = 3
     INTEGER = 4
     CUSTOM = 5
     DEFINE = 6
     REDEFINE = 7
 
     @staticmethod
     def allowedKeywordSuffixes(value):
-        return { ParserKind.TAG:          ['.'],
-                 ParserKind.COMMAND:      [':'],
-                 ParserKind.LIST:         [':'],
-                 ParserKind.BOOLEAN_EXPR: [':'],
-                 ParserKind.INTEGER:      [':'],
-                 ParserKind.CUSTOM:       [':', '.'],
-                 ParserKind.DEFINE:       [':'],
-                 ParserKind.REDEFINE:     [':']
-               } [value]
+        return {
+            ParserKind.TAG: ["."],
+            ParserKind.COMMAND: [":"],
+            ParserKind.LIST: [":"],
+            ParserKind.BOOLEAN_EXPR: [":"],
+            ParserKind.INTEGER: [":"],
+            ParserKind.CUSTOM: [":", "."],
+            ParserKind.DEFINE: [":"],
+            ParserKind.REDEFINE: [":"],
+        }[value]
 
     @staticmethod
     def str(value):
-        return { ParserKind.TAG:          'TAG',
-                 ParserKind.COMMAND:      'COMMAND',
-                 ParserKind.LIST:         'LIST',
-                 ParserKind.BOOLEAN_EXPR: 'BOOLEAN_EXPR',
-                 ParserKind.INTEGER:      'INTEGER',
-                 ParserKind.CUSTOM:       'CUSTOM',
-                 ParserKind.DEFINE:       'DEFINE',
-                 ParserKind.REDEFINE:     'REDEFINE'
-               } [value]
+        return {
+            ParserKind.TAG: "TAG",
+            ParserKind.COMMAND: "COMMAND",
+            ParserKind.LIST: "LIST",
+            ParserKind.BOOLEAN_EXPR: "BOOLEAN_EXPR",
+            ParserKind.INTEGER: "INTEGER",
+            ParserKind.CUSTOM: "CUSTOM",
+            ParserKind.DEFINE: "DEFINE",
+            ParserKind.REDEFINE: "REDEFINE",
+        }[value]
 
 
 class IntegratedTestKeywordParser(object):
     """A parser for LLVM/Clang style integrated test scripts.
 
     keyword: The keyword to parse for. It must end in either '.' or ':'.
     kind: An value of ParserKind.
     parser: A custom parser. This value may only be specified with
             ParserKind.CUSTOM.
     """
+
     def __init__(self, keyword, kind, parser=None, initial_value=None):
         allowedSuffixes = ParserKind.allowedKeywordSuffixes(kind)
         if len(keyword) == 0 or keyword[-1] not in allowedSuffixes:
             if len(allowedSuffixes) == 1:
-                raise ValueError("Keyword '%s' of kind '%s' must end in '%s'"
-                                 % (keyword, ParserKind.str(kind),
-                                    allowedSuffixes[0]))
+                raise ValueError(
+                    "Keyword '%s' of kind '%s' must end in '%s'"
+                    % (keyword, ParserKind.str(kind), allowedSuffixes[0])
+                )
             else:
-                raise ValueError("Keyword '%s' of kind '%s' must end in "
-                                 " one of '%s'"
-                                 % (keyword, ParserKind.str(kind),
-                                    ' '.join(allowedSuffixes)))
+                raise ValueError(
+                    "Keyword '%s' of kind '%s' must end in "
+                    " one of '%s'"
+                    % (keyword, ParserKind.str(kind), " ".join(allowedSuffixes))
+                )
 
         if parser is not None and kind != ParserKind.CUSTOM:
-            raise ValueError("custom parsers can only be specified with "
-                             "ParserKind.CUSTOM")
+            raise ValueError(
+                "custom parsers can only be specified with " "ParserKind.CUSTOM"
+            )
         self.keyword = keyword
         self.kind = kind
         self.parsed_lines = []
         self.value = initial_value
         self.parser = parser
 
         if kind == ParserKind.COMMAND:
-            self.parser = lambda line_number, line, output: \
-                                 self._handleCommand(line_number, line, output,
-                                                     self.keyword)
+            self.parser = lambda line_number, line, output: self._handleCommand(
+                line_number, line, output, self.keyword
+            )
         elif kind == ParserKind.LIST:
             self.parser = self._handleList
         elif kind == ParserKind.BOOLEAN_EXPR:
             self.parser = self._handleBooleanExpr
         elif kind == ParserKind.INTEGER:
             self.parser = self._handleSingleInteger
         elif kind == ParserKind.TAG:
             self.parser = self._handleTag
         elif kind == ParserKind.CUSTOM:
             if parser is None:
                 raise ValueError("ParserKind.CUSTOM requires a custom parser")
             self.parser = parser
         elif kind == ParserKind.DEFINE:
-            self.parser = lambda line_number, line, output: \
-                                 self._handleSubst(line_number, line, output,
-                                                   self.keyword, new_subst=True)
+            self.parser = lambda line_number, line, output: self._handleSubst(
+                line_number, line, output, self.keyword, new_subst=True
+            )
         elif kind == ParserKind.REDEFINE:
-            self.parser = lambda line_number, line, output: \
-                                 self._handleSubst(line_number, line, output,
-                                                   self.keyword,
-                                                   new_subst=False)
+            self.parser = lambda line_number, line, output: self._handleSubst(
+                line_number, line, output, self.keyword, new_subst=False
+            )
         else:
             raise ValueError("Unknown kind '%s'" % kind)
 
     def parseLine(self, line_number, line):
         try:
             self.parsed_lines += [(line_number, line)]
             self.value = self.parser(line_number, line, self.value)
         except ValueError as e:
-            raise ValueError(str(e) + ("\nin %s directive on test line %d" %
-                                       (self.keyword, line_number)))
+            raise ValueError(
+                str(e)
+                + ("\nin %s directive on test line %d" % (self.keyword, line_number))
+            )
 
     def getValue(self):
         return self.value
 
     @staticmethod
     def _handleTag(line_number, line, output):
         """A helper for parsing TAG type keywords"""
-        return (not line.strip() or output)
+        return not line.strip() or output
 
     @staticmethod
     def _substituteLineNumbers(line_number, line):
-        line = re.sub(r'%\(line\)', str(line_number), line)
+        line = re.sub(r"%\(line\)", str(line_number), line)
+
         def replace_line_number(match):
-            if match.group(1) == '+':
+            if match.group(1) == "+":
                 return str(line_number + int(match.group(2)))
-            if match.group(1) == '-':
+            if match.group(1) == "-":
                 return str(line_number - int(match.group(2)))
-        return re.sub(r'%\(line *([\+-]) *(\d+)\)', replace_line_number, line)
+
+        return re.sub(r"%\(line *([\+-]) *(\d+)\)", replace_line_number, line)
 
     @classmethod
     def _handleCommand(cls, line_number, line, output, keyword):
         """A helper for parsing COMMAND type keywords"""
         # Substitute line number expressions.
         line = cls._substituteLineNumbers(line_number, line)
 
         # Collapse lines with trailing '\\', or add line with line number to
         # start a new pipeline.
-        if not output or not output[-1].add_continuation(line_number, keyword,
-                                                         line):
+        if not output or not output[-1].add_continuation(line_number, keyword, line):
             if output is None:
                 output = []
             pdbg = "%dbg({keyword} at line {line_number})".format(
-                keyword=keyword,
-                line_number=line_number)
-            assert re.match(kPdbgRegex + "$", pdbg), \
-                   "kPdbgRegex expected to match actual %dbg usage"
-            line = "{pdbg} {real_command}".format(
-                pdbg=pdbg,
-                real_command=line)
-            output.append(CommandDirective(line_number, line_number, keyword,
-                                           line))
+                keyword=keyword, line_number=line_number
+            )
+            assert re.match(
+                kPdbgRegex + "$", pdbg
+            ), "kPdbgRegex expected to match actual %dbg usage"
+            line = "{pdbg} {real_command}".format(pdbg=pdbg, real_command=line)
+            output.append(CommandDirective(line_number, line_number, keyword, line))
         return output
 
     @staticmethod
     def _handleList(line_number, line, output):
         """A parser for LIST type keywords"""
         if output is None:
             output = []
-        output.extend([s.strip() for s in line.split(',')])
+        output.extend([s.strip() for s in line.split(",")])
         return output
 
     @staticmethod
     def _handleSingleInteger(line_number, line, output):
         """A parser for INTEGER type keywords"""
         if output is None:
             output = []
         try:
             n = int(line)
         except ValueError:
-            raise ValueError("INTEGER parser requires the input to be an integer (got {})".format(line))
+            raise ValueError(
+                "INTEGER parser requires the input to be an integer (got {})".format(
+                    line
+                )
+            )
         output.append(n)
         return output
 
     @staticmethod
     def _handleBooleanExpr(line_number, line, output):
         """A parser for BOOLEAN_EXPR type keywords"""
-        parts = [s.strip() for s in line.split(',') if s.strip() != '']
-        if output and output[-1][-1] == '\\':
+        parts = [s.strip() for s in line.split(",") if s.strip() != ""]
+        if output and output[-1][-1] == "\\":
             output[-1] = output[-1][:-1] + parts[0]
             del parts[0]
         if output is None:
             output = []
         output.extend(parts)
         # Evaluate each expression to verify syntax.
         # We don't want any results, just the raised ValueError.
         for s in output:
-            if s != '*' and not s.endswith('\\'):
+            if s != "*" and not s.endswith("\\"):
                 BooleanExpression.evaluate(s, [])
         return output
 
     @classmethod
     def _handleSubst(cls, line_number, line, output, keyword, new_subst):
         """A parser for DEFINE and REDEFINE type keywords"""
         line = cls._substituteLineNumbers(line_number, line)
         if output and output[-1].add_continuation(line_number, keyword, line):
             return output
         if output is None:
             output = []
-        output.append(SubstDirective(line_number, line_number, keyword,
-                                     new_subst, line))
+        output.append(
+            SubstDirective(line_number, line_number, keyword, new_subst, line)
+        )
         return output
 
 
-def _parseKeywords(sourcepath, additional_parsers=[],
-                   require_script=True):
+def _parseKeywords(sourcepath, additional_parsers=[], require_script=True):
     """_parseKeywords
 
     Scan an LLVM/Clang style integrated test script and extract all the lines
     pertaining to a special parser. This includes 'RUN', 'XFAIL', 'REQUIRES',
     'UNSUPPORTED', 'ALLOW_RETRIES', 'END', 'DEFINE', 'REDEFINE', as well as
     other specified custom parsers.
 
     Returns a dictionary mapping each custom parser to its value after
     parsing the test.
     """
     # Install the built-in keyword parsers.
     script = []
     builtin_parsers = [
-        IntegratedTestKeywordParser('RUN:', ParserKind.COMMAND, initial_value=script),
-        IntegratedTestKeywordParser('XFAIL:', ParserKind.BOOLEAN_EXPR),
-        IntegratedTestKeywordParser('REQUIRES:', ParserKind.BOOLEAN_EXPR),
-        IntegratedTestKeywordParser('UNSUPPORTED:', ParserKind.BOOLEAN_EXPR),
-        IntegratedTestKeywordParser('ALLOW_RETRIES:', ParserKind.INTEGER),
-        IntegratedTestKeywordParser('END.', ParserKind.TAG),
-        IntegratedTestKeywordParser('DEFINE:', ParserKind.DEFINE,
-                                    initial_value=script),
-        IntegratedTestKeywordParser('REDEFINE:', ParserKind.REDEFINE,
-                                    initial_value=script)
+        IntegratedTestKeywordParser("RUN:", ParserKind.COMMAND, initial_value=script),
+        IntegratedTestKeywordParser("XFAIL:", ParserKind.BOOLEAN_EXPR),
+        IntegratedTestKeywordParser("REQUIRES:", ParserKind.BOOLEAN_EXPR),
+        IntegratedTestKeywordParser("UNSUPPORTED:", ParserKind.BOOLEAN_EXPR),
+        IntegratedTestKeywordParser("ALLOW_RETRIES:", ParserKind.INTEGER),
+        IntegratedTestKeywordParser("END.", ParserKind.TAG),
+        IntegratedTestKeywordParser("DEFINE:", ParserKind.DEFINE, initial_value=script),
+        IntegratedTestKeywordParser(
+            "REDEFINE:", ParserKind.REDEFINE, initial_value=script
+        ),
     ]
     keyword_parsers = {p.keyword: p for p in builtin_parsers}
 
     # Install user-defined additional parsers.
     for parser in additional_parsers:
         if not isinstance(parser, IntegratedTestKeywordParser):
-            raise ValueError('Additional parser must be an instance of '
-                             'IntegratedTestKeywordParser')
+            raise ValueError(
+                "Additional parser must be an instance of "
+                "IntegratedTestKeywordParser"
+            )
         if parser.keyword in keyword_parsers:
-            raise ValueError("Parser for keyword '%s' already exists"
-                             % parser.keyword)
+            raise ValueError("Parser for keyword '%s' already exists" % parser.keyword)
         keyword_parsers[parser.keyword] = parser
 
     # Collect the test lines from the script.
-    for line_number, command_type, ln in \
-            parseIntegratedTestScriptCommands(sourcepath,
-                                              keyword_parsers.keys()):
+    for line_number, command_type, ln in parseIntegratedTestScriptCommands(
+        sourcepath, keyword_parsers.keys()
+    ):
         parser = keyword_parsers[command_type]
         parser.parseLine(line_number, ln)
-        if command_type == 'END.' and parser.getValue() is True:
+        if command_type == "END." and parser.getValue() is True:
             break
 
     # Verify the script contains a run line.
-    if require_script and not any(isinstance(directive, CommandDirective)
-                                  for directive in script):
+    if require_script and not any(
+        isinstance(directive, CommandDirective) for directive in script
+    ):
         raise ValueError("Test has no 'RUN:' line")
 
     # Check for unterminated run or subst lines.
     #
     # If, after a line continuation for one kind of directive (e.g., 'RUN:',
     # 'DEFINE:', 'REDEFINE:') in script, the next directive in script is a
     # different kind, then the '\\' remains on the former, and we report it
     # here.
     for directive in script:
         if directive.needs_continuation():
-            raise ValueError(f"Test has unterminated '{directive.keyword}' "
-                             f"directive (with '\\') "
-                             f"{directive.get_location()}")
+            raise ValueError(
+                f"Test has unterminated '{directive.keyword}' "
+                f"directive (with '\\') "
+                f"{directive.get_location()}"
+            )
 
     # Check boolean expressions for unterminated lines.
     for key in keyword_parsers:
         kp = keyword_parsers[key]
         if kp.kind != ParserKind.BOOLEAN_EXPR:
             continue
         value = kp.getValue()
-        if value and value[-1][-1] == '\\':
-            raise ValueError("Test has unterminated '{key}' lines (with '\\')"
-                             .format(key=key))
+        if value and value[-1][-1] == "\\":
+            raise ValueError(
+                "Test has unterminated '{key}' lines (with '\\')".format(key=key)
+            )
 
     # Make sure there's at most one ALLOW_RETRIES: line
-    allowed_retries = keyword_parsers['ALLOW_RETRIES:'].getValue()
+    allowed_retries = keyword_parsers["ALLOW_RETRIES:"].getValue()
     if allowed_retries and len(allowed_retries) > 1:
         raise ValueError("Test has more than one ALLOW_RETRIES lines")
 
     return {p.keyword: p.getValue() for p in keyword_parsers.values()}
 
 
-def parseIntegratedTestScript(test, additional_parsers=[],
-                              require_script=True):
+def parseIntegratedTestScript(test, additional_parsers=[], require_script=True):
     """parseIntegratedTestScript - Scan an LLVM/Clang style integrated test
     script and extract the lines to 'RUN' as well as 'XFAIL', 'REQUIRES',
     'UNSUPPORTED' and 'ALLOW_RETRIES' information into the given test.
 
     If additional parsers are specified then the test is also scanned for the
     keywords they specify and all matches are passed to the custom parser.
 
     If 'require_script' is False an empty script
     may be returned. This can be used for test formats where the actual script
     is optional or ignored.
     """
     # Parse the test sources and extract test properties
     try:
-        parsed = _parseKeywords(test.getSourcePath(), additional_parsers,
-                                require_script)
+        parsed = _parseKeywords(
+            test.getSourcePath(), additional_parsers, require_script
+        )
     except ValueError as e:
         return lit.Test.Result(Test.UNRESOLVED, str(e))
-    script = parsed['RUN:'] or []
-    assert parsed['DEFINE:'] == script
-    assert parsed['REDEFINE:'] == script
-    test.xfails += parsed['XFAIL:'] or []
-    test.requires += parsed['REQUIRES:'] or []
-    test.unsupported += parsed['UNSUPPORTED:'] or []
-    if parsed['ALLOW_RETRIES:']:
-        test.allowed_retries = parsed['ALLOW_RETRIES:'][0]
+    script = parsed["RUN:"] or []
+    assert parsed["DEFINE:"] == script
+    assert parsed["REDEFINE:"] == script
+    test.xfails += parsed["XFAIL:"] or []
+    test.requires += parsed["REQUIRES:"] or []
+    test.unsupported += parsed["UNSUPPORTED:"] or []
+    if parsed["ALLOW_RETRIES:"]:
+        test.allowed_retries = parsed["ALLOW_RETRIES:"][0]
 
     # Enforce REQUIRES:
     missing_required_features = test.getMissingRequiredFeatures()
     if missing_required_features:
-        msg = ', '.join(missing_required_features)
-        return lit.Test.Result(Test.UNSUPPORTED,
-                               "Test requires the following unavailable "
-                               "features: %s" % msg)
+        msg = ", ".join(missing_required_features)
+        return lit.Test.Result(
+            Test.UNSUPPORTED,
+            "Test requires the following unavailable " "features: %s" % msg,
+        )
 
     # Enforce UNSUPPORTED:
     unsupported_features = test.getUnsupportedFeatures()
     if unsupported_features:
-        msg = ', '.join(unsupported_features)
+        msg = ", ".join(unsupported_features)
         return lit.Test.Result(
             Test.UNSUPPORTED,
-            "Test does not support the following features "
-            "and/or targets: %s" % msg)
+            "Test does not support the following features " "and/or targets: %s" % msg,
+        )
 
     # Enforce limit_to_features.
     if not test.isWithinFeatureLimits():
-        msg = ', '.join(test.config.limit_to_features)
-        return lit.Test.Result(Test.UNSUPPORTED,
-                               "Test does not require any of the features "
-                               "specified in limit_to_features: %s" % msg)
+        msg = ", ".join(test.config.limit_to_features)
+        return lit.Test.Result(
+            Test.UNSUPPORTED,
+            "Test does not require any of the features "
+            "specified in limit_to_features: %s" % msg,
+        )
 
     return script
 
 
 def _runShTest(test, litConfig, useExternalSh, script, tmpBase):
     def runOnce(execdir):
         if useExternalSh:
             res = executeScript(test, litConfig, tmpBase, script, execdir)
         else:
             res = executeScriptInternal(test, litConfig, tmpBase, script, execdir)
         if isinstance(res, lit.Test.Result):
             return res
 
-        out,err,exitCode,timeoutInfo = res
+        out, err, exitCode, timeoutInfo = res
         if exitCode == 0:
             status = Test.PASS
         else:
             if timeoutInfo is None:
                 status = Test.FAIL
             else:
                 status = Test.TIMEOUT
-        return out,err,exitCode,timeoutInfo,status
+        return out, err, exitCode, timeoutInfo, status
 
     # Create the output directory if it does not already exist.
     lit.util.mkdir_p(os.path.dirname(tmpBase))
 
     # Re-run failed tests up to test.allowed_retries times.
     execdir = os.path.dirname(test.getExecPath())
     attempts = test.allowed_retries + 1
     for i in range(attempts):
         res = runOnce(execdir)
         if isinstance(res, lit.Test.Result):
             return res
 
-        out,err,exitCode,timeoutInfo,status = res
+        out, err, exitCode, timeoutInfo, status = res
         if status != Test.FAIL:
             break
 
     # If we had to run the test more than once, count it as a flaky pass. These
     # will be printed separately in the test summary.
     if i > 0 and status == Test.PASS:
         status = Test.FLAKYPASS
 
     # Form the output log.
-    output = """Script:\n--\n%s\n--\nExit Code: %d\n""" % (
-        '\n'.join(script), exitCode)
+    output = """Script:\n--\n%s\n--\nExit Code: %d\n""" % ("\n".join(script), exitCode)
 
     if timeoutInfo is not None:
         output += """Timeout: %s\n""" % (timeoutInfo,)
     output += "\n"
 
     # Append the outputs, if present.
     if out:
         output += """Command Output (stdout):\n--\n%s\n--\n""" % (out,)
     if err:
         output += """Command Output (stderr):\n--\n%s\n--\n""" % (err,)
 
     return lit.Test.Result(status, output)
 
 
-def executeShTest(test, litConfig, useExternalSh,
-                  extra_substitutions=[],
-                  preamble_commands=[]):
+def executeShTest(
+    test, litConfig, useExternalSh, extra_substitutions=[], preamble_commands=[]
+):
     if test.config.unsupported:
-        return lit.Test.Result(Test.UNSUPPORTED, 'Test is unsupported')
+        return lit.Test.Result(Test.UNSUPPORTED, "Test is unsupported")
 
     script = list(preamble_commands)
     parsed = parseIntegratedTestScript(test, require_script=not script)
     if isinstance(parsed, lit.Test.Result):
         return parsed
     script += parsed
 
     if litConfig.noExecute:
         return lit.Test.Result(Test.PASS)
 
     tmpDir, tmpBase = getTempPaths(test)
     substitutions = list(extra_substitutions)
-    substitutions += getDefaultSubstitutions(test, tmpDir, tmpBase,
-                                             normalize_slashes=useExternalSh)
-    conditions = { feature: True for feature in test.config.available_features }
-    script = applySubstitutions(script, substitutions, conditions,
-                                recursion_limit=test.config.recursiveExpansionLimit)
+    substitutions += getDefaultSubstitutions(
+        test, tmpDir, tmpBase, normalize_slashes=useExternalSh
+    )
+    conditions = {feature: True for feature in test.config.available_features}
+    script = applySubstitutions(
+        script,
+        substitutions,
+        conditions,
+        recursion_limit=test.config.recursiveExpansionLimit,
+    )
 
     return _runShTest(test, litConfig, useExternalSh, script, tmpBase)
```

### Comparing `lit-16.0.6/lit/TestTimes.py` & `lit-17.0.0rc1/lit/TestTimes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import os
 
 
 def read_test_times(suite):
     test_times = {}
-    test_times_file = os.path.join(suite.exec_root, '.lit_test_times.txt')
+    test_times_file = os.path.join(suite.exec_root, ".lit_test_times.txt")
     if not os.path.exists(test_times_file):
-        test_times_file = os.path.join(
-            suite.source_root, '.lit_test_times.txt')
+        test_times_file = os.path.join(suite.source_root, ".lit_test_times.txt")
     if os.path.exists(test_times_file):
-        with open(test_times_file, 'r') as time_file:
+        with open(test_times_file, "r") as time_file:
             for line in time_file:
                 time, path = line.split(maxsplit=1)
-                test_times[path.strip('\n')] = float(time)
+                test_times[path.strip("\n")] = float(time)
     return test_times
 
 
 def record_test_times(tests, lit_config):
     times_by_suite = {}
     for t in tests:
         assert t.suite.test_times is None
-        if not t.result.elapsed:
+        if t.result.elapsed is None:
             continue
         if not t.suite.exec_root in times_by_suite:
             times_by_suite[t.suite.exec_root] = read_test_times(t.suite)
         time = -t.result.elapsed if t.isFailure() else t.result.elapsed
         # The "path" here is only used as a key into a dictionary. It is never
         # used as an actual path to a filesystem API, therefore we use '/' as
         # the canonical separator so that Unix and Windows machines can share
         # timing data.
-        times_by_suite[t.suite.exec_root]['/'.join(t.path_in_suite)] = time
+        times_by_suite[t.suite.exec_root]["/".join(t.path_in_suite)] = time
 
     for s, value in times_by_suite.items():
         try:
-            path = os.path.join(s, '.lit_test_times.txt')
-            with open(path, 'w') as time_file:
+            path = os.path.join(s, ".lit_test_times.txt")
+            with open(path, "w") as time_file:
                 for name, time in value.items():
-                    time_file.write(("%e" % time) + ' ' + name + '\n')
+                    time_file.write(("%e" % time) + " " + name + "\n")
         except:
-            lit_config.warning('Could not save test time: ' + path)
+            lit_config.warning("Could not save test time: " + path)
             continue
```

### Comparing `lit-16.0.6/lit/TestingConfig.py` & `lit-17.0.0rc1/lit/TestingConfig.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,111 +1,121 @@
 import os
 import sys
 
 
 class TestingConfig(object):
-    """"
+    """ "
     TestingConfig - Information on the tests inside a suite.
     """
 
     @staticmethod
     def fromdefaults(litConfig):
         """
         fromdefaults(litConfig) -> TestingConfig
 
         Create a TestingConfig object with default values.
         """
         # Set the environment based on the command line arguments.
         environment = {
-            'PATH' : os.pathsep.join(litConfig.path +
-                                     [os.environ.get('PATH','')]),
-            'LLVM_DISABLE_CRASH_REPORT' : '1',
-            }
+            "PATH": os.pathsep.join(litConfig.path + [os.environ.get("PATH", "")]),
+            "LLVM_DISABLE_CRASH_REPORT": "1",
+        }
 
         pass_vars = [
-            'LIBRARY_PATH',
-            'LD_LIBRARY_PATH',
-            'SYSTEMROOT',
-            'TERM',
-            'CLANG',
-            'LLDB',
-            'LD_PRELOAD',
-            'LLVM_SYMBOLIZER_PATH',
-            'ASAN_SYMBOLIZER_PATH',
-            'HWASAN_SYMBOLIZER_PATH',
-            'LSAN_SYMBOLIZER_PATH',
-            'MSAN_SYMBOLIZER_PATH',
-            'TSAN_SYMBOLIZER_PATH',
-            'UBSAN_SYMBOLIZER_PATH',
-            'ASAN_OPTIONS',
-            'LSAN_OPTIONS',
-            'HWASAN_OPTIONS',
-            'MSAN_OPTIONS',
-            'TSAN_OPTIONS',
-            'UBSAN_OPTIONS',
-            'ADB',
-            'ANDROID_SERIAL',
-            'SSH_AUTH_SOCK',
-            'SANITIZER_IGNORE_CVE_2016_2143',
-            'TMPDIR',
-            'TMP',
-            'TEMP',
-            'TEMPDIR',
-            'AVRLIT_BOARD',
-            'AVRLIT_PORT',
-            'FILECHECK_OPTS',
-            'VCINSTALLDIR',
-            'VCToolsinstallDir',
-            'VSINSTALLDIR',
-            'WindowsSdkDir',
-            'WindowsSDKLibVersion',
-            'SOURCE_DATE_EPOCH',
-            'GTEST_FILTER',
-            'DFLTCC',
+            "LIBRARY_PATH",
+            "LD_LIBRARY_PATH",
+            "SYSTEMROOT",
+            "TERM",
+            "CLANG",
+            "LLDB",
+            "LD_PRELOAD",
+            "LLVM_SYMBOLIZER_PATH",
+            "LLVM_PROFILE_FILE",
+            "ASAN_SYMBOLIZER_PATH",
+            "HWASAN_SYMBOLIZER_PATH",
+            "LSAN_SYMBOLIZER_PATH",
+            "MSAN_SYMBOLIZER_PATH",
+            "TSAN_SYMBOLIZER_PATH",
+            "UBSAN_SYMBOLIZER_PATH",
+            "ASAN_OPTIONS",
+            "LSAN_OPTIONS",
+            "HWASAN_OPTIONS",
+            "MSAN_OPTIONS",
+            "TSAN_OPTIONS",
+            "UBSAN_OPTIONS",
+            "ADB",
+            "ANDROID_SERIAL",
+            "SSH_AUTH_SOCK",
+            "SANITIZER_IGNORE_CVE_2016_2143",
+            "TMPDIR",
+            "TMP",
+            "TEMP",
+            "TEMPDIR",
+            "AVRLIT_BOARD",
+            "AVRLIT_PORT",
+            "FILECHECK_OPTS",
+            "VCINSTALLDIR",
+            "VCToolsinstallDir",
+            "VSINSTALLDIR",
+            "WindowsSdkDir",
+            "WindowsSDKLibVersion",
+            "SOURCE_DATE_EPOCH",
+            "GTEST_FILTER",
+            "DFLTCC",
         ]
 
-        if sys.platform.startswith('aix'):
-            pass_vars += ['LIBPATH']
-        elif sys.platform == 'win32':
+        if sys.platform.startswith("aix"):
+            pass_vars += ["LIBPATH"]
+        elif sys.platform == "win32":
             pass_vars += [
-                'COMSPEC',
-                'INCLUDE',
-                'LIB',
-                'PATHEXT',
-                'USERPROFILE',
+                "COMSPEC",
+                "INCLUDE",
+                "LIB",
+                "PATHEXT",
+                "USERPROFILE",
             ]
-            environment['PYTHONBUFFERED'] = '1'
+            environment["PYTHONBUFFERED"] = "1"
+            # Avoid Windows heuristics which try to detect potential installer
+            # programs (which may need to run with elevated privileges) and ask
+            # if the user wants to run them in that way. This heuristic may
+            # match for executables containing the substrings "patch" (which is
+            # a substring of "dispatch"), "update", "setup", etc. Set this
+            # environment variable indicating that we want to execute them with
+            # the current user.
+            environment["__COMPAT_LAYER"] = "RunAsInvoker"
 
         for var in pass_vars:
-            val = os.environ.get(var, '')
+            val = os.environ.get(var, "")
             # Check for empty string as some variables such as LD_PRELOAD cannot be empty
             # ('') for OS's such as OpenBSD.
             if val:
                 environment[var] = val
 
         # Set the default available features based on the LitConfig.
         available_features = []
         if litConfig.useValgrind:
-            available_features.append('valgrind')
+            available_features.append("valgrind")
             if litConfig.valgrindLeakCheck:
-                available_features.append('vg_leak')
+                available_features.append("vg_leak")
 
-        return TestingConfig(None,
-                             name = '<unnamed>',
-                             suffixes = set(),
-                             test_format = None,
-                             environment = environment,
-                             substitutions = [],
-                             unsupported = False,
-                             test_exec_root = None,
-                             test_source_root = None,
-                             excludes = [],
-                             available_features = available_features,
-                             pipefail = True,
-                             standalone_tests = False)
+        return TestingConfig(
+            None,
+            name="<unnamed>",
+            suffixes=set(),
+            test_format=None,
+            environment=environment,
+            substitutions=[],
+            unsupported=False,
+            test_exec_root=None,
+            test_source_root=None,
+            excludes=[],
+            available_features=available_features,
+            pipefail=True,
+            standalone_tests=False,
+        )
 
     def load_from_path(self, path, litConfig):
         """
         load_from_path(path, litConfig)
 
         Load the configuration module at the provided path into the given config
         object.
@@ -113,45 +123,60 @@
 
         # Load the config script data.
         data = None
         f = open(path)
         try:
             data = f.read()
         except:
-            litConfig.fatal('unable to load config file: %r' % (path,))
+            litConfig.fatal("unable to load config file: %r" % (path,))
         f.close()
 
         # Execute the config script to initialize the object.
         cfg_globals = dict(globals())
-        cfg_globals['config'] = self
-        cfg_globals['lit_config'] = litConfig
-        cfg_globals['__file__'] = path
+        cfg_globals["config"] = self
+        cfg_globals["lit_config"] = litConfig
+        cfg_globals["__file__"] = path
         try:
-            exec(compile(data, path, 'exec'), cfg_globals, None)
+            exec(compile(data, path, "exec"), cfg_globals, None)
             if litConfig.debug:
-                litConfig.note('... loaded config %r' % path)
+                litConfig.note("... loaded config %r" % path)
         except SystemExit:
             e = sys.exc_info()[1]
             # We allow normal system exit inside a config file to just
             # return control without error.
             if e.args:
                 raise
         except:
             import traceback
+
             litConfig.fatal(
-                'unable to parse config file %r, traceback: %s' % (
-                    path, traceback.format_exc()))
+                "unable to parse config file %r, traceback: %s"
+                % (path, traceback.format_exc())
+            )
         self.finish(litConfig)
 
-    def __init__(self, parent, name, suffixes, test_format,
-                 environment, substitutions, unsupported,
-                 test_exec_root, test_source_root, excludes,
-                 available_features, pipefail, limit_to_features = [],
-                 is_early = False, parallelism_group = None,
-                 standalone_tests = False):
+    def __init__(
+        self,
+        parent,
+        name,
+        suffixes,
+        test_format,
+        environment,
+        substitutions,
+        unsupported,
+        test_exec_root,
+        test_source_root,
+        excludes,
+        available_features,
+        pipefail,
+        limit_to_features=[],
+        is_early=False,
+        parallelism_group=None,
+        standalone_tests=False,
+    ):
         self.parent = parent
         self.name = str(name)
         self.suffixes = set(suffixes)
         self.test_format = test_format
         self.environment = dict(environment)
         self.substitutions = list(substitutions)
         self.unsupported = unsupported
@@ -171,17 +196,25 @@
     @property
     def recursiveExpansionLimit(self):
         return self._recursiveExpansionLimit
 
     @recursiveExpansionLimit.setter
     def recursiveExpansionLimit(self, value):
         if value is not None and not isinstance(value, int):
-            raise ValueError('recursiveExpansionLimit must be either None or an integer (got <{}>)'.format(value))
+            raise ValueError(
+                "recursiveExpansionLimit must be either None or an integer (got <{}>)".format(
+                    value
+                )
+            )
         if isinstance(value, int) and value < 0:
-            raise ValueError('recursiveExpansionLimit must be a non-negative integer (got <{}>)'.format(value))
+            raise ValueError(
+                "recursiveExpansionLimit must be a non-negative integer (got <{}>)".format(
+                    value
+                )
+            )
         self._recursiveExpansionLimit = value
 
     def finish(self, litConfig):
         """finish() - Finish this config object, after loading is complete."""
 
         self.name = str(self.name)
         self.suffixes = set(self.suffixes)
@@ -201,32 +234,33 @@
     def root(self):
         """root attribute - The root configuration for the test suite."""
         if self.parent is None:
             return self
         else:
             return self.parent.root
 
+
 class SubstituteCaptures:
     """
     Helper class to indicate that the substitutions contains backreferences.
 
     This can be used as the following in lit.cfg to mark subsitutions as having
     back-references::
 
         config.substutions.append(('\b[^ ]*.cpp', SubstituteCaptures('\0.txt')))
 
     """
+
     def __init__(self, substitution):
         self.substitution = substitution
 
     def replace(self, pattern, replacement):
         return self.substitution
 
     def __str__(self):
         return self.substitution
 
     def __len__(self):
         return len(self.substitution)
 
     def __getitem__(self, item):
         return self.substitution.__getitem__(item)
-
```

### Comparing `lit-16.0.6/lit/builtin_commands/cat.py` & `lit-17.0.0rc1/lit/builtin_commands/cat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 import getopt
 import sys
+
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
+
 def convertToCaretAndMNotation(data):
-   newdata = StringIO()
-   if isinstance(data, str):
-       data = bytearray(data)
-
-   for intval in data:
-       if intval == 9 or intval == 10:
-           newdata.write(chr(intval))
-           continue
-       if intval > 127:
-           intval = intval -128
-           newdata.write("M-")
-       if intval < 32:
-           newdata.write("^")
-           newdata.write(chr(intval+64))
-       elif intval == 127:
-           newdata.write("^?")
-       else:
-           newdata.write(chr(intval))
+    newdata = StringIO()
+    if isinstance(data, str):
+        data = bytearray(data)
+
+    for intval in data:
+        if intval == 9 or intval == 10:
+            newdata.write(chr(intval))
+            continue
+        if intval > 127:
+            intval = intval - 128
+            newdata.write("M-")
+        if intval < 32:
+            newdata.write("^")
+            newdata.write(chr(intval + 64))
+        elif intval == 127:
+            newdata.write("^?")
+        else:
+            newdata.write(chr(intval))
 
-   return newdata.getvalue().encode()
+    return newdata.getvalue().encode()
 
 
 def main(argv):
     arguments = argv[1:]
     short_options = "v"
     long_options = ["show-nonprinting"]
-    show_nonprinting = False;
+    show_nonprinting = False
 
     try:
         options, filenames = getopt.gnu_getopt(arguments, short_options, long_options)
     except getopt.GetoptError as err:
         sys.stderr.write("Unsupported: 'cat':  %s\n" % str(err))
         sys.exit(1)
 
     for option, value in options:
         if option == "-v" or option == "--show-nonprinting":
-            show_nonprinting = True;
+            show_nonprinting = True
 
-    writer = getattr(sys.stdout, 'buffer', None)
+    writer = getattr(sys.stdout, "buffer", None)
     if writer is None:
         writer = sys.stdout
         if sys.platform == "win32":
             import os, msvcrt
-            msvcrt.setmode(sys.stdout.fileno(),os.O_BINARY)
+
+            msvcrt.setmode(sys.stdout.fileno(), os.O_BINARY)
     for filename in filenames:
         try:
-            fileToCat = open(filename,"rb")
+            fileToCat = open(filename, "rb")
             contents = fileToCat.read()
             if show_nonprinting:
                 contents = convertToCaretAndMNotation(contents)
             writer.write(contents)
             sys.stdout.flush()
             fileToCat.close()
         except IOError as error:
             sys.stderr.write(str(error))
             sys.exit(1)
 
+
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `lit-16.0.6/lit/builtin_commands/diff.py` & `lit-17.0.0rc1/lit/builtin_commands/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,152 +1,196 @@
 import difflib
 import functools
 import getopt
 import io
 import locale
 import os
+import re
 import sys
 
 import util
 from util import to_string
 
-class DiffFlags():
+
+class DiffFlags:
     def __init__(self):
         self.ignore_all_space = False
         self.ignore_space_change = False
+        self.ignore_matching_lines = False
+        self.ignore_matching_lines_regex = ""
         self.unified_diff = False
         self.num_context_lines = 3
         self.recursive_diff = False
         self.strip_trailing_cr = False
 
+
 def getDirTree(path, basedir=""):
     # Tree is a tuple of form (dirname, child_trees).
     # An empty dir has child_trees = [], a file has child_trees = None.
     child_trees = []
     for dirname, child_dirs, files in os.walk(os.path.join(basedir, path)):
         for child_dir in child_dirs:
             child_trees.append(getDirTree(child_dir, dirname))
         for filename in files:
             child_trees.append((filename, None))
         return path, sorted(child_trees)
 
+
 def compareTwoFiles(flags, filepaths):
     filelines = []
     for file in filepaths:
         if file == "-":
             stdin_fileno = sys.stdin.fileno()
-            with os.fdopen(os.dup(stdin_fileno), 'rb') as stdin_bin:
+            with os.fdopen(os.dup(stdin_fileno), "rb") as stdin_bin:
                 filelines.append(stdin_bin.readlines())
         else:
-            with open(file, 'rb') as file_bin:
+            with open(file, "rb") as file_bin:
                 filelines.append(file_bin.readlines())
 
     try:
-        return compareTwoTextFiles(flags, filepaths, filelines,
-                                   locale.getpreferredencoding(False))
+        return compareTwoTextFiles(
+            flags, filepaths, filelines, locale.getpreferredencoding(False)
+        )
     except UnicodeDecodeError:
         try:
             return compareTwoTextFiles(flags, filepaths, filelines, "utf-8")
         except:
             return compareTwoBinaryFiles(flags, filepaths, filelines)
 
+
 def compareTwoBinaryFiles(flags, filepaths, filelines):
     exitCode = 0
-    if hasattr(difflib, 'diff_bytes'):
+    if hasattr(difflib, "diff_bytes"):
         # python 3.5 or newer
-        diffs = difflib.diff_bytes(difflib.unified_diff, filelines[0],
-                                   filelines[1], filepaths[0].encode(),
-                                   filepaths[1].encode(),
-                                   n = flags.num_context_lines)
+        diffs = difflib.diff_bytes(
+            difflib.unified_diff,
+            filelines[0],
+            filelines[1],
+            filepaths[0].encode(),
+            filepaths[1].encode(),
+            n=flags.num_context_lines,
+        )
         diffs = [diff.decode(errors="backslashreplace") for diff in diffs]
     else:
         # python 2.7
         if flags.unified_diff:
             func = difflib.unified_diff
         else:
             func = difflib.context_diff
-        diffs = func(filelines[0], filelines[1], filepaths[0], filepaths[1],
-                     n = flags.num_context_lines)
+        diffs = func(
+            filelines[0],
+            filelines[1],
+            filepaths[0],
+            filepaths[1],
+            n=flags.num_context_lines,
+        )
 
     for diff in diffs:
         sys.stdout.write(to_string(diff))
         exitCode = 1
     return exitCode
 
+
 def compareTwoTextFiles(flags, filepaths, filelines_bin, encoding):
     filelines = []
     for lines_bin in filelines_bin:
         lines = []
         for line_bin in lines_bin:
             line = line_bin.decode(encoding=encoding)
             lines.append(line)
         filelines.append(lines)
 
     exitCode = 0
+
     def compose2(f, g):
         return lambda x: f(g(x))
 
     f = lambda x: x
     if flags.strip_trailing_cr:
-        f = compose2(lambda line: line.replace('\r\n', '\n'), f)
+        f = compose2(lambda line: line.replace("\r\n", "\n"), f)
     if flags.ignore_all_space or flags.ignore_space_change:
-        ignoreSpace = lambda line, separator: \
-                          separator.join(line.split()) + "\n"
-        ignoreAllSpaceOrSpaceChange = functools.partial(ignoreSpace, separator='' if flags.ignore_all_space else ' ')
+        ignoreSpace = lambda line, separator: separator.join(line.split()) + "\n"
+        ignoreAllSpaceOrSpaceChange = functools.partial(
+            ignoreSpace, separator="" if flags.ignore_all_space else " "
+        )
         f = compose2(ignoreAllSpaceOrSpaceChange, f)
 
     for idx, lines in enumerate(filelines):
-        filelines[idx]= [f(line) for line in lines]
+        if flags.ignore_matching_lines:
+            lines = filter(
+                lambda x: not re.match(
+                    r"{}".format(flags.ignore_matching_lines_regex), x
+                ),
+                lines,
+            )
+        filelines[idx] = [f(line) for line in lines]
 
     func = difflib.unified_diff if flags.unified_diff else difflib.context_diff
-    for diff in func(filelines[0], filelines[1], filepaths[0], filepaths[1],
-                     n = flags.num_context_lines):
+    for diff in func(
+        filelines[0],
+        filelines[1],
+        filepaths[0],
+        filepaths[1],
+        n=flags.num_context_lines,
+    ):
         sys.stdout.write(to_string(diff))
         exitCode = 1
     return exitCode
 
+
 def printDirVsFile(dir_path, file_path):
     if os.path.getsize(file_path):
         msg = "File %s is a directory while file %s is a regular file"
     else:
         msg = "File %s is a directory while file %s is a regular empty file"
     sys.stdout.write(msg % (dir_path, file_path) + "\n")
 
+
 def printFileVsDir(file_path, dir_path):
     if os.path.getsize(file_path):
         msg = "File %s is a regular file while file %s is a directory"
     else:
         msg = "File %s is a regular empty file while file %s is a directory"
     sys.stdout.write(msg % (file_path, dir_path) + "\n")
 
+
 def printOnlyIn(basedir, path, name):
     sys.stdout.write("Only in %s: %s\n" % (os.path.join(basedir, path), name))
 
+
 def compareDirTrees(flags, dir_trees, base_paths=["", ""]):
     # Dirnames of the trees are not checked, it's caller's responsibility,
     # as top-level dirnames are always different. Base paths are important
     # for doing os.walk, but we don't put it into tree's dirname in order
     # to speed up string comparison below and while sorting in getDirTree.
     left_tree, right_tree = dir_trees[0], dir_trees[1]
     left_base, right_base = base_paths[0], base_paths[1]
 
     # Compare two files or report file vs. directory mismatch.
     if left_tree[1] is None and right_tree[1] is None:
-        return compareTwoFiles(flags,
-                               [os.path.join(left_base, left_tree[0]),
-                                os.path.join(right_base, right_tree[0])])
+        return compareTwoFiles(
+            flags,
+            [
+                os.path.join(left_base, left_tree[0]),
+                os.path.join(right_base, right_tree[0]),
+            ],
+        )
 
     if left_tree[1] is None and right_tree[1] is not None:
-        printFileVsDir(os.path.join(left_base, left_tree[0]),
-                       os.path.join(right_base, right_tree[0]))
+        printFileVsDir(
+            os.path.join(left_base, left_tree[0]),
+            os.path.join(right_base, right_tree[0]),
+        )
         return 1
 
     if left_tree[1] is not None and right_tree[1] is None:
-        printDirVsFile(os.path.join(left_base, left_tree[0]),
-                       os.path.join(right_base, right_tree[0]))
+        printDirVsFile(
+            os.path.join(left_base, left_tree[0]),
+            os.path.join(right_base, right_tree[0]),
+        )
         return 1
 
     # Compare two directories via recursive use of compareDirTrees.
     exitCode = 0
     left_names = [node[0] for node in left_tree[1]]
     right_names = [node[0] for node in right_tree[1]]
     l, r = 0, 0
@@ -157,44 +201,50 @@
             printOnlyIn(left_base, left_tree[0], left_names[l])
             l += 1
         elif left_names[l] > right_names[r]:
             exitCode = 1
             printOnlyIn(right_base, right_tree[0], right_names[r])
             r += 1
         else:
-            exitCode |= compareDirTrees(flags,
-                                        [left_tree[1][l], right_tree[1][r]],
-                                        [os.path.join(left_base, left_tree[0]),
-                                        os.path.join(right_base, right_tree[0])])
+            exitCode |= compareDirTrees(
+                flags,
+                [left_tree[1][l], right_tree[1][r]],
+                [
+                    os.path.join(left_base, left_tree[0]),
+                    os.path.join(right_base, right_tree[0]),
+                ],
+            )
             l += 1
             r += 1
 
     # At least one of the trees has ended. Report names from the other tree.
     while l < len(left_names):
         exitCode = 1
         printOnlyIn(left_base, left_tree[0], left_names[l])
         l += 1
     while r < len(right_names):
         exitCode = 1
         printOnlyIn(right_base, right_tree[0], right_names[r])
         r += 1
     return exitCode
 
+
 def main(argv):
     if sys.platform == "win32":
-        if hasattr(sys.stdout, 'buffer'):
+        if hasattr(sys.stdout, "buffer"):
             # python 3
-            sys.stdout = io.TextIOWrapper(sys.stdout.buffer, newline='\n')
+            sys.stdout = io.TextIOWrapper(sys.stdout.buffer, newline="\n")
         else:
             # python 2.7
             import msvcrt
+
             msvcrt.setmode(sys.stdout.fileno(), os.O_BINARY)
     args = argv[1:]
     try:
-        opts, args = getopt.gnu_getopt(args, "wbuU:r", ["strip-trailing-cr"])
+        opts, args = getopt.gnu_getopt(args, "wbuI:U:r", ["strip-trailing-cr"])
     except getopt.GetoptError as err:
         sys.stderr.write("Unsupported: 'diff': %s\n" % str(err))
         sys.exit(1)
 
     flags = DiffFlags()
     filelines, filepaths, dir_trees = ([] for i in range(3))
     for o, a in opts:
@@ -207,17 +257,19 @@
         elif o.startswith("-U"):
             flags.unified_diff = True
             try:
                 flags.num_context_lines = int(a)
                 if flags.num_context_lines < 0:
                     raise ValueException
             except:
-                sys.stderr.write("Error: invalid '-U' argument: {}\n"
-                                 .format(a))
+                sys.stderr.write("Error: invalid '-U' argument: {}\n".format(a))
                 sys.exit(1)
+        elif o == "-I":
+            flags.ignore_matching_lines = True
+            flags.ignore_matching_lines_regex = a
         elif o == "-r":
             flags.recursive_diff = True
         elif o == "--strip-trailing-cr":
             flags.strip_trailing_cr = True
         else:
             assert False, "unhandled option"
 
@@ -246,9 +298,10 @@
 
     except IOError as err:
         sys.stderr.write("Error: 'diff' command failed, %s\n" % str(err))
         exitCode = 1
 
     sys.exit(exitCode)
 
+
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `lit-16.0.6/lit/cl_arguments.py` & `lit-17.0.0rc1/lit/cl_arguments.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,251 +6,333 @@
 
 import lit.reports
 import lit.util
 
 
 @enum.unique
 class TestOrder(enum.Enum):
-    LEXICAL = 'lexical'
-    RANDOM = 'random'
-    SMART = 'smart'
+    LEXICAL = "lexical"
+    RANDOM = "random"
+    SMART = "smart"
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(prog='lit', fromfile_prefix_chars='@')
-    parser.add_argument('test_paths',
-            nargs='+',
-            metavar="TEST_PATH",
-            help='File or path to include in the test suite')
-
-    parser.add_argument('--version',
-            action='version',
-            version='%(prog)s ' + lit.__version__)
-
-    parser.add_argument("-j", "--threads", "--workers",
-            dest="workers",
-            metavar="N",
-            help="Number of workers used for testing",
-            type=_positive_int,
-            default=lit.util.usable_core_count())
-    parser.add_argument("--config-prefix",
-            dest="configPrefix",
-            metavar="NAME",
-            help="Prefix for 'lit' config files")
-    parser.add_argument("-D", "--param",
-            dest="user_params",
-            metavar="NAME=VAL",
-            help="Add 'NAME' = 'VAL' to the user defined parameters",
-            action="append",
-            default=[])
+    parser = argparse.ArgumentParser(prog="lit", fromfile_prefix_chars="@")
+    parser.add_argument(
+        "test_paths",
+        nargs="+",
+        metavar="TEST_PATH",
+        help="File or path to include in the test suite",
+    )
+
+    parser.add_argument(
+        "--version", action="version", version="%(prog)s " + lit.__version__
+    )
+
+    parser.add_argument(
+        "-j",
+        "--threads",
+        "--workers",
+        dest="workers",
+        metavar="N",
+        help="Number of workers used for testing",
+        type=_positive_int,
+        default=lit.util.usable_core_count(),
+    )
+    parser.add_argument(
+        "--config-prefix",
+        dest="configPrefix",
+        metavar="NAME",
+        help="Prefix for 'lit' config files",
+    )
+    parser.add_argument(
+        "-D",
+        "--param",
+        dest="user_params",
+        metavar="NAME=VAL",
+        help="Add 'NAME' = 'VAL' to the user defined parameters",
+        action="append",
+        default=[],
+    )
 
     format_group = parser.add_argument_group("Output Format")
     # FIXME: I find these names very confusing, although I like the
     # functionality.
-    format_group.add_argument("-q", "--quiet",
-            help="Suppress no error output",
-            action="store_true")
-    format_group.add_argument("-s", "--succinct",
-            help="Reduce amount of output."
-                 " Additionally, show a progress bar,"
-                 " unless --no-progress-bar is specified.",
-            action="store_true")
-    format_group.add_argument("-v", "--verbose",
-            dest="showOutput",
-            help="Show test output for failures",
-            action="store_true")
-    format_group.add_argument("-vv", "--echo-all-commands",
-            dest="echoAllCommands",
-            action="store_true",
-            help="Echo all commands as they are executed to stdout. In case of "
-                 "failure, last command shown will be the failing one.")
-    format_group.add_argument("-a", "--show-all",
-            dest="showAllOutput",
-            help="Display all commandlines and output",
-            action="store_true")
-    format_group.add_argument("-o", "--output",
-            type=lit.reports.JsonReport,
-            help="Write test results to the provided path",
-            metavar="PATH")
-    format_group.add_argument("--no-progress-bar",
-            dest="useProgressBar",
-            help="Do not use curses based progress bar",
-            action="store_false")
+    format_group.add_argument(
+        "-q", "--quiet", help="Suppress no error output", action="store_true"
+    )
+    format_group.add_argument(
+        "-s",
+        "--succinct",
+        help="Reduce amount of output."
+        " Additionally, show a progress bar,"
+        " unless --no-progress-bar is specified.",
+        action="store_true",
+    )
+    format_group.add_argument(
+        "-v",
+        "--verbose",
+        dest="showOutput",
+        help="Show test output for failures",
+        action="store_true",
+    )
+    format_group.add_argument(
+        "-vv",
+        "--echo-all-commands",
+        dest="echoAllCommands",
+        action="store_true",
+        help="Echo all commands as they are executed to stdout. In case of "
+        "failure, last command shown will be the failing one.",
+    )
+    format_group.add_argument(
+        "-a",
+        "--show-all",
+        dest="showAllOutput",
+        help="Display all commandlines and output",
+        action="store_true",
+    )
+    format_group.add_argument(
+        "-o",
+        "--output",
+        type=lit.reports.JsonReport,
+        help="Write test results to the provided path",
+        metavar="PATH",
+    )
+    format_group.add_argument(
+        "--no-progress-bar",
+        dest="useProgressBar",
+        help="Do not use curses based progress bar",
+        action="store_false",
+    )
 
     # Note: this does not generate flags for user-defined result codes.
-    success_codes = [c for c in lit.Test.ResultCode.all_codes()
-                     if not c.isFailure]
+    success_codes = [c for c in lit.Test.ResultCode.all_codes() if not c.isFailure]
     for code in success_codes:
         format_group.add_argument(
             "--show-{}".format(code.name.lower()),
             dest="shown_codes",
             help="Show {} tests ({})".format(code.label.lower(), code.name),
             action="append_const",
             const=code,
-            default=[])
+            default=[],
+        )
 
     execution_group = parser.add_argument_group("Test Execution")
-    execution_group.add_argument("--path",
-            help="Additional paths to add to testing environment",
-            action="append",
-            default=[],
-            type=os.path.abspath)
-    execution_group.add_argument("--vg",
-            dest="useValgrind",
-            help="Run tests under valgrind",
-            action="store_true")
-    execution_group.add_argument("--vg-leak",
-            dest="valgrindLeakCheck",
-            help="Check for memory leaks under valgrind",
-            action="store_true")
-    execution_group.add_argument("--vg-arg",
-            dest="valgrindArgs",
-            metavar="ARG",
-            help="Specify an extra argument for valgrind",
-            action="append",
-            default=[])
-    execution_group.add_argument("--time-tests",
-            help="Track elapsed wall time for each test",
-            action="store_true")
-    execution_group.add_argument("--no-execute",
-            dest="noExecute",
-            help="Don't execute any tests (assume PASS)",
-            action="store_true")
-    execution_group.add_argument("--xunit-xml-output",
-            type=lit.reports.XunitReport,
-            help="Write XUnit-compatible XML test reports to the specified file")
-    execution_group.add_argument("--resultdb-output",
-            type=lit.reports.ResultDBReport,
-            help="Write LuCI ResuldDB compatible JSON to the specified file")
-    execution_group.add_argument("--time-trace-output",
-            type=lit.reports.TimeTraceReport,
-            help="Write Chrome tracing compatible JSON to the specified file")
-    execution_group.add_argument("--timeout",
-            dest="maxIndividualTestTime",
-            help="Maximum time to spend running a single test (in seconds). "
-                 "0 means no time limit. [Default: 0]",
-            type=_non_negative_int)
-    execution_group.add_argument("--max-failures",
-            help="Stop execution after the given number of failures.",
-            type=_positive_int)
-    execution_group.add_argument("--allow-empty-runs",
-            help="Do not fail the run if all tests are filtered out",
-            action="store_true")
-    execution_group.add_argument("--ignore-fail",
-            dest="ignoreFail",
-            action="store_true",
-            help="Exit with status zero even if some tests fail")
-    execution_group.add_argument("--no-indirectly-run-check",
-            dest="indirectlyRunCheck",
-            help="Do not error if a test would not be run if the user had "
-                 "specified the containing directory instead of naming the "
-                 "test directly.",
-            action="store_false")
+    execution_group.add_argument(
+        "--path",
+        help="Additional paths to add to testing environment",
+        action="append",
+        default=[],
+        type=os.path.abspath,
+    )
+    execution_group.add_argument(
+        "--vg", dest="useValgrind", help="Run tests under valgrind", action="store_true"
+    )
+    execution_group.add_argument(
+        "--vg-leak",
+        dest="valgrindLeakCheck",
+        help="Check for memory leaks under valgrind",
+        action="store_true",
+    )
+    execution_group.add_argument(
+        "--vg-arg",
+        dest="valgrindArgs",
+        metavar="ARG",
+        help="Specify an extra argument for valgrind",
+        action="append",
+        default=[],
+    )
+    execution_group.add_argument(
+        "--time-tests",
+        help="Track elapsed wall time for each test",
+        action="store_true",
+    )
+    execution_group.add_argument(
+        "--no-execute",
+        dest="noExecute",
+        help="Don't execute any tests (assume PASS)",
+        action="store_true",
+    )
+    execution_group.add_argument(
+        "--xunit-xml-output",
+        type=lit.reports.XunitReport,
+        help="Write XUnit-compatible XML test reports to the specified file",
+    )
+    execution_group.add_argument(
+        "--resultdb-output",
+        type=lit.reports.ResultDBReport,
+        help="Write LuCI ResuldDB compatible JSON to the specified file",
+    )
+    execution_group.add_argument(
+        "--time-trace-output",
+        type=lit.reports.TimeTraceReport,
+        help="Write Chrome tracing compatible JSON to the specified file",
+    )
+    execution_group.add_argument(
+        "--timeout",
+        dest="maxIndividualTestTime",
+        help="Maximum time to spend running a single test (in seconds). "
+        "0 means no time limit. [Default: 0]",
+        type=_non_negative_int,
+    )
+    execution_group.add_argument(
+        "--max-failures",
+        help="Stop execution after the given number of failures.",
+        type=_positive_int,
+    )
+    execution_group.add_argument(
+        "--allow-empty-runs",
+        help="Do not fail the run if all tests are filtered out",
+        action="store_true",
+    )
+    execution_group.add_argument(
+        "--ignore-fail",
+        dest="ignoreFail",
+        action="store_true",
+        help="Exit with status zero even if some tests fail",
+    )
 
     selection_group = parser.add_argument_group("Test Selection")
-    selection_group.add_argument("--max-tests",
-            metavar="N",
-            help="Maximum number of tests to run",
-            type=_positive_int)
-    selection_group.add_argument("--max-time",
-            dest="timeout",
-            metavar="N",
-            help="Maximum time to spend testing (in seconds)",
-            type=_positive_int)
-    selection_group.add_argument("--order",
-            choices=[x.value for x in TestOrder],
-            default=TestOrder.SMART,
-            help="Test order to use (default: smart)")
-    selection_group.add_argument("--shuffle",
-            dest="order",
-            help="Run tests in random order (DEPRECATED: use --order=random)",
-            action="store_const",
-            const=TestOrder.RANDOM)
-    selection_group.add_argument("-i", "--incremental",
-            help="Run failed tests first (DEPRECATED: use --order=smart)",
-            action="store_true")
-    selection_group.add_argument("--filter",
-            metavar="REGEX",
-            type=_case_insensitive_regex,
-            help="Only run tests with paths matching the given regular expression",
-            default=os.environ.get("LIT_FILTER", ".*"))
-    selection_group.add_argument("--filter-out",
-            metavar="REGEX",
-            type=_case_insensitive_regex,
-            help="Filter out tests with paths matching the given regular expression",
-            default=os.environ.get("LIT_FILTER_OUT", "^$"))
-    selection_group.add_argument("--xfail",
-            metavar="LIST",
-            type=_semicolon_list,
-            help="XFAIL tests with paths in the semicolon separated list",
-            default=os.environ.get("LIT_XFAIL", ""))
-    selection_group.add_argument("--xfail-not",
-            metavar="LIST",
-            type=_semicolon_list,
-            help="do not XFAIL tests with paths in the semicolon separated list",
-            default=os.environ.get("LIT_XFAIL_NOT", ""))
-    selection_group.add_argument("--num-shards",
-            dest="numShards",
-            metavar="M",
-            help="Split testsuite into M pieces and only run one",
-            type=_positive_int,
-            default=os.environ.get("LIT_NUM_SHARDS"))
-    selection_group.add_argument("--run-shard",
-            dest="runShard",
-            metavar="N",
-            help="Run shard #N of the testsuite",
-            type=_positive_int,
-            default=os.environ.get("LIT_RUN_SHARD"))
+    selection_group.add_argument(
+        "--max-tests",
+        metavar="N",
+        help="Maximum number of tests to run",
+        type=_positive_int,
+    )
+    selection_group.add_argument(
+        "--max-time",
+        dest="timeout",
+        metavar="N",
+        help="Maximum time to spend testing (in seconds)",
+        type=_positive_int,
+    )
+    selection_group.add_argument(
+        "--order",
+        choices=[x.value for x in TestOrder],
+        default=TestOrder.SMART,
+        help="Test order to use (default: smart)",
+    )
+    selection_group.add_argument(
+        "--shuffle",
+        dest="order",
+        help="Run tests in random order (DEPRECATED: use --order=random)",
+        action="store_const",
+        const=TestOrder.RANDOM,
+    )
+    selection_group.add_argument(
+        "-i",
+        "--incremental",
+        help="Run failed tests first (DEPRECATED: use --order=smart)",
+        action="store_true",
+    )
+    selection_group.add_argument(
+        "--filter",
+        metavar="REGEX",
+        type=_case_insensitive_regex,
+        help="Only run tests with paths matching the given regular expression",
+        default=os.environ.get("LIT_FILTER", ".*"),
+    )
+    selection_group.add_argument(
+        "--filter-out",
+        metavar="REGEX",
+        type=_case_insensitive_regex,
+        help="Filter out tests with paths matching the given regular expression",
+        default=os.environ.get("LIT_FILTER_OUT", "^$"),
+    )
+    selection_group.add_argument(
+        "--xfail",
+        metavar="LIST",
+        type=_semicolon_list,
+        help="XFAIL tests with paths in the semicolon separated list",
+        default=os.environ.get("LIT_XFAIL", ""),
+    )
+    selection_group.add_argument(
+        "--xfail-not",
+        metavar="LIST",
+        type=_semicolon_list,
+        help="do not XFAIL tests with paths in the semicolon separated list",
+        default=os.environ.get("LIT_XFAIL_NOT", ""),
+    )
+    selection_group.add_argument(
+        "--num-shards",
+        dest="numShards",
+        metavar="M",
+        help="Split testsuite into M pieces and only run one",
+        type=_positive_int,
+        default=os.environ.get("LIT_NUM_SHARDS"),
+    )
+    selection_group.add_argument(
+        "--run-shard",
+        dest="runShard",
+        metavar="N",
+        help="Run shard #N of the testsuite",
+        type=_positive_int,
+        default=os.environ.get("LIT_RUN_SHARD"),
+    )
 
     debug_group = parser.add_argument_group("Debug and Experimental Options")
-    debug_group.add_argument("--debug",
-            help="Enable debugging (for 'lit' development)",
-            action="store_true")
-    debug_group.add_argument("--show-suites",
-            help="Show discovered test suites and exit",
-            action="store_true")
-    debug_group.add_argument("--show-tests",
-            help="Show all discovered tests and exit",
-            action="store_true")
-    debug_group.add_argument("--show-used-features",
-            help="Show all features used in the test suite (in XFAIL, UNSUPPORTED and REQUIRES) and exit",
-            action="store_true")
+    debug_group.add_argument(
+        "--debug", help="Enable debugging (for 'lit' development)", action="store_true"
+    )
+    debug_group.add_argument(
+        "--show-suites",
+        help="Show discovered test suites and exit",
+        action="store_true",
+    )
+    debug_group.add_argument(
+        "--show-tests", help="Show all discovered tests and exit", action="store_true"
+    )
+    debug_group.add_argument(
+        "--show-used-features",
+        help="Show all features used in the test suite (in XFAIL, UNSUPPORTED and REQUIRES) and exit",
+        action="store_true",
+    )
 
     # LIT is special: environment variables override command line arguments.
     env_args = shlex.split(os.environ.get("LIT_OPTS", ""))
     args = sys.argv[1:] + env_args
     opts = parser.parse_args(args)
 
     # Validate command line options
     if opts.echoAllCommands:
         opts.showOutput = True
 
     if opts.incremental:
-        print('WARNING: --incremental is deprecated. Failing tests now always run first.')
+        print(
+            "WARNING: --incremental is deprecated. Failing tests now always run first."
+        )
 
     if opts.numShards or opts.runShard:
         if not opts.numShards or not opts.runShard:
             parser.error("--num-shards and --run-shard must be used together")
         if opts.runShard > opts.numShards:
             parser.error("--run-shard must be between 1 and --num-shards (inclusive)")
         opts.shard = (opts.runShard, opts.numShards)
     else:
         opts.shard = None
 
-    opts.reports = filter(None, [opts.output, opts.xunit_xml_output, opts.resultdb_output, opts.time_trace_output])
+    opts.reports = filter(
+        None,
+        [
+            opts.output,
+            opts.xunit_xml_output,
+            opts.resultdb_output,
+            opts.time_trace_output,
+        ],
+    )
 
     return opts
 
 
 def _positive_int(arg):
-    return _int(arg, 'positive', lambda i: i > 0)
+    return _int(arg, "positive", lambda i: i > 0)
 
 
 def _non_negative_int(arg):
-    return _int(arg, 'non-negative', lambda i: i >= 0)
+    return _int(arg, "non-negative", lambda i: i >= 0)
 
 
 def _int(arg, kind, pred):
     desc = "requires {} integer, but found '{}'"
     try:
         i = int(arg)
     except ValueError:
@@ -258,20 +340,21 @@
     if not pred(i):
         raise _error(desc, kind, arg)
     return i
 
 
 def _case_insensitive_regex(arg):
     import re
+
     try:
         return re.compile(arg, re.IGNORECASE)
     except re.error as reason:
         raise _error("invalid regular expression: '{}', {}", arg, reason)
 
 
 def _semicolon_list(arg):
-    return arg.split(';')
+    return arg.split(";")
 
 
 def _error(desc, *args):
     msg = desc.format(*args)
     return argparse.ArgumentTypeError(msg)
```

### Comparing `lit-16.0.6/lit/display.py` & `lit-17.0.0rc1/lit/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 
 def create_display(opts, tests, total_tests, workers):
     if opts.quiet:
         return NopDisplay()
 
     num_tests = len(tests)
-    of_total = (' of %d' % total_tests) if (num_tests != total_tests) else ''
-    header = '-- Testing: %d%s tests, %d workers --' % (
-        num_tests, of_total, workers)
+    of_total = (" of %d" % total_tests) if (num_tests != total_tests) else ""
+    header = "-- Testing: %d%s tests, %d workers --" % (num_tests, of_total, workers)
 
     progress_bar = None
     if opts.succinct and opts.useProgressBar:
         import lit.ProgressBar
+
         try:
             tc = lit.ProgressBar.TerminalController()
             progress_bar = lit.ProgressBar.ProgressBar(tc, header)
             header = None
         except ValueError:
-            progress_bar = lit.ProgressBar.SimpleProgressBar('Testing: ')
+            progress_bar = lit.ProgressBar.SimpleProgressBar("Testing: ")
 
     return Display(opts, tests, header, progress_bar)
 
 
 class ProgressPredictor(object):
     def __init__(self, tests):
         self.completed = 0
@@ -45,116 +45,125 @@
         if test.previous_elapsed:
             self.predictable_tests_remaining -= 1
             self.predictable_time_remaining -= test.previous_elapsed
         else:
             self.unpredictable_tests_remaining -= 1
 
         # NOTE: median would be more precise, but might be too slow.
-        average_test_time = (self.time_elapsed + self.predictable_time_remaining) / \
-            (self.completed + self.predictable_tests_remaining)
-        unpredictable_time_remaining = average_test_time * \
-            self.unpredictable_tests_remaining
-        total_time_remaining = self.predictable_time_remaining + unpredictable_time_remaining
+        average_test_time = (self.time_elapsed + self.predictable_time_remaining) / (
+            self.completed + self.predictable_tests_remaining
+        )
+        unpredictable_time_remaining = (
+            average_test_time * self.unpredictable_tests_remaining
+        )
+        total_time_remaining = (
+            self.predictable_time_remaining + unpredictable_time_remaining
+        )
         total_time = self.time_elapsed + total_time_remaining
 
         if total_time > 0:
             return self.time_elapsed / total_time
         return 0
 
 
 class NopDisplay(object):
-    def print_header(self): pass
-    def update(self, test): pass
-    def clear(self, interrupted): pass
+    def print_header(self):
+        pass
+
+    def update(self, test):
+        pass
+
+    def clear(self, interrupted):
+        pass
 
 
 class Display(object):
     def __init__(self, opts, tests, header, progress_bar):
         self.opts = opts
         self.num_tests = len(tests)
         self.header = header
-        self.progress_predictor = ProgressPredictor(
-            tests) if progress_bar else None
+        self.progress_predictor = ProgressPredictor(tests) if progress_bar else None
         self.progress_bar = progress_bar
         self.completed = 0
 
     def print_header(self):
         if self.header:
             print(self.header)
         if self.progress_bar:
-            self.progress_bar.update(0.0, '')
+            self.progress_bar.update(0.0, "")
 
     def update(self, test):
         self.completed += 1
 
-        show_result = test.isFailure() or \
-                self.opts.showAllOutput or \
-                (not self.opts.quiet and not self.opts.succinct)
+        show_result = (
+            test.isFailure()
+            or self.opts.showAllOutput
+            or (not self.opts.quiet and not self.opts.succinct)
+        )
         if show_result:
             if self.progress_bar:
                 self.progress_bar.clear(interrupted=False)
             self.print_result(test)
 
         if self.progress_bar:
             if test.isFailure():
-                self.progress_bar.barColor = 'RED'
+                self.progress_bar.barColor = "RED"
             percent = self.progress_predictor.update(test)
             self.progress_bar.update(percent, test.getFullName())
 
     def clear(self, interrupted):
         if self.progress_bar:
             self.progress_bar.clear(interrupted)
 
     def print_result(self, test):
         # Show the test result line.
         test_name = test.getFullName()
-        print('%s: %s (%d of %d)' % (test.result.code.name, test_name,
-                                     self.completed, self.num_tests))
+        print(
+            "%s: %s (%d of %d)"
+            % (test.result.code.name, test_name, self.completed, self.num_tests)
+        )
 
         # Show the test failure output, if requested.
-        if (test.isFailure() and self.opts.showOutput) or \
-           self.opts.showAllOutput:
+        if (test.isFailure() and self.opts.showOutput) or self.opts.showAllOutput:
             if test.isFailure():
-                print("%s TEST '%s' FAILED %s" % ('*'*20, test.getFullName(),
-                                                  '*'*20))
+                print(
+                    "%s TEST '%s' FAILED %s" % ("*" * 20, test.getFullName(), "*" * 20)
+                )
             out = test.result.output
             # Encode/decode so that, when using Python 3.6.5 in Windows 10,
             # print(out) doesn't raise UnicodeEncodeError if out contains
             # special characters.  However, Python 2 might try to decode
             # as part of the encode call if out is already encoded, so skip
             # encoding if it raises UnicodeDecodeError.
             if sys.stdout.encoding:
                 try:
-                    out = out.encode(encoding=sys.stdout.encoding,
-                                     errors="replace")
+                    out = out.encode(encoding=sys.stdout.encoding, errors="replace")
                 except UnicodeDecodeError:
                     pass
                 # Python 2 can raise UnicodeDecodeError here too in cases
                 # where the stdout encoding is ASCII. Ignore decode errors
                 # in this case.
                 out = out.decode(encoding=sys.stdout.encoding, errors="ignore")
             print(out)
             print("*" * 20)
 
         # Report test metrics, if present.
         if test.result.metrics:
-            print("%s TEST '%s' RESULTS %s" % ('*'*10, test.getFullName(),
-                                               '*'*10))
+            print("%s TEST '%s' RESULTS %s" % ("*" * 10, test.getFullName(), "*" * 10))
             items = sorted(test.result.metrics.items())
             for metric_name, value in items:
-                print('%s: %s ' % (metric_name, value.format()))
+                print("%s: %s " % (metric_name, value.format()))
             print("*" * 10)
 
         # Report micro-tests, if present
         if test.result.microResults:
             items = sorted(test.result.microResults.items())
             for micro_test_name, micro_test in items:
-                print("%s MICRO-TEST: %s" %
-                         ('*'*3, micro_test_name))
+                print("%s MICRO-TEST: %s" % ("*" * 3, micro_test_name))
 
                 if micro_test.metrics:
                     sorted_metrics = sorted(micro_test.metrics.items())
                     for metric_name, value in sorted_metrics:
-                        print('    %s:  %s ' % (metric_name, value.format()))
+                        print("    %s:  %s " % (metric_name, value.format()))
 
         # Ensure the output is flushed.
         sys.stdout.flush()
```

### Comparing `lit-16.0.6/lit/formats/googletest.py` & `lit-17.0.0rc1/lit/formats/googletest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,202 +7,223 @@
 import sys
 
 import lit.Test
 import lit.TestRunner
 import lit.util
 from .base import TestFormat
 
-kIsWindows = sys.platform in ['win32', 'cygwin']
+kIsWindows = sys.platform in ["win32", "cygwin"]
+
 
 class GoogleTest(TestFormat):
-    def __init__(self, test_sub_dirs, test_suffix, run_under = []):
+    def __init__(self, test_sub_dirs, test_suffix, run_under=[]):
         self.seen_executables = set()
-        self.test_sub_dirs = str(test_sub_dirs).split(';')
+        self.test_sub_dirs = str(test_sub_dirs).split(";")
 
         # On Windows, assume tests will also end in '.exe'.
         exe_suffix = str(test_suffix)
         if kIsWindows:
-            exe_suffix += '.exe'
+            exe_suffix += ".exe"
 
         # Also check for .py files for testing purposes.
-        self.test_suffixes = {exe_suffix, test_suffix + '.py'}
+        self.test_suffixes = {exe_suffix, test_suffix + ".py"}
         self.run_under = run_under
 
     def get_num_tests(self, path, litConfig, localConfig):
         list_test_cmd = self.prepareCmd(
-            [path, '--gtest_list_tests', '--gtest_filter=-*DISABLED_*'])
+            [path, "--gtest_list_tests", "--gtest_filter=-*DISABLED_*"]
+        )
         try:
-            out = subprocess.check_output(list_test_cmd,
-                                          env=localConfig.environment)
+            out = subprocess.check_output(list_test_cmd, env=localConfig.environment)
         except subprocess.CalledProcessError as exc:
             litConfig.warning(
                 "unable to discover google-tests in %r: %s. Process output: %s"
-                % (path, sys.exc_info()[1], exc.output))
+                % (path, sys.exc_info()[1], exc.output)
+            )
             return None
         return sum(
-            map(lambda line: lit.util.to_string(line).startswith('  '),
-                out.splitlines(False)))
+            map(
+                lambda line: lit.util.to_string(line).startswith("  "),
+                out.splitlines(False),
+            )
+        )
 
-    def getTestsInDirectory(self, testSuite, path_in_suite, litConfig,
-                            localConfig):
+    def getTestsInDirectory(self, testSuite, path_in_suite, litConfig, localConfig):
         init_shard_size = 512  # number of tests in a shard
         core_count = lit.util.usable_core_count()
         source_path = testSuite.getSourcePath(path_in_suite)
         for subdir in self.test_sub_dirs:
             dir_path = os.path.join(source_path, subdir)
             if not os.path.isdir(dir_path):
                 continue
-            for fn in lit.util.listdir_files(dir_path,
-                                             suffixes=self.test_suffixes):
+            for fn in lit.util.listdir_files(dir_path, suffixes=self.test_suffixes):
                 # Discover the tests in this executable.
                 execpath = os.path.join(source_path, subdir, fn)
                 if execpath in self.seen_executables:
                     litConfig.warning(
-                        "Skip adding %r since it has been added to the test pool" % execpath)
+                        "Skip adding %r since it has been added to the test pool"
+                        % execpath
+                    )
                     continue
                 else:
                     self.seen_executables.add(execpath)
-                num_tests = self.get_num_tests(execpath, litConfig,
-                                               localConfig)
+                num_tests = self.get_num_tests(execpath, litConfig, localConfig)
                 if num_tests is not None:
                     # Compute the number of shards.
                     shard_size = init_shard_size
                     nshard = int(math.ceil(num_tests / shard_size))
                     while nshard < core_count and shard_size > 1:
                         shard_size = shard_size // 2
                         nshard = int(math.ceil(num_tests / shard_size))
 
                     # Create one lit test for each shard.
                     for idx in range(nshard):
-                        testPath = path_in_suite + (subdir, fn, str(idx),
-                                                    str(nshard))
-                        json_file = '-'.join([
-                            execpath, testSuite.config.name,
-                            str(os.getpid()),
-                            str(idx),
-                            str(nshard)
-                        ]) + '.json'
-                        yield lit.Test.Test(testSuite,
-                                            testPath,
-                                            localConfig,
-                                            file_path=execpath,
-                                            gtest_json_file=json_file)
+                        testPath = path_in_suite + (subdir, fn, str(idx), str(nshard))
+                        json_file = (
+                            "-".join(
+                                [
+                                    execpath,
+                                    testSuite.config.name,
+                                    str(os.getpid()),
+                                    str(idx),
+                                    str(nshard),
+                                ]
+                            )
+                            + ".json"
+                        )
+                        yield lit.Test.Test(
+                            testSuite,
+                            testPath,
+                            localConfig,
+                            file_path=execpath,
+                            gtest_json_file=json_file,
+                        )
                 else:
                     # This doesn't look like a valid gtest file.  This can
                     # have a number of causes, none of them good.  For
                     # instance, we could have created a broken executable.
                     # Alternatively, someone has cruft in their test
                     # directory.  If we don't return a test here, then no
                     # failures will get reported, so return a dummy test name
                     # so that the failure is reported later.
                     testPath = path_in_suite + (
-                        subdir, fn, 'failed_to_discover_tests_from_gtest')
-                    yield lit.Test.Test(testSuite,
-                                        testPath,
-                                        localConfig,
-                                        file_path=execpath)
+                        subdir,
+                        fn,
+                        "failed_to_discover_tests_from_gtest",
+                    )
+                    yield lit.Test.Test(
+                        testSuite, testPath, localConfig, file_path=execpath
+                    )
 
     def execute(self, test, litConfig):
         if test.gtest_json_file is None:
-            return lit.Test.FAIL, ''
+            return lit.Test.FAIL, ""
 
-        testPath,testName = os.path.split(test.getSourcePath())
+        testPath, testName = os.path.split(test.getSourcePath())
         while not os.path.exists(testPath):
             # Handle GTest parametrized and typed tests, whose name includes
             # some '/'s.
             testPath, namePrefix = os.path.split(testPath)
-            testName = namePrefix + '/' + testName
+            testName = namePrefix + "/" + testName
 
-        testName,total_shards = os.path.split(testName)
-        testName,shard_idx = os.path.split(testName)
+        testName, total_shards = os.path.split(testName)
+        testName, shard_idx = os.path.split(testName)
         from lit.cl_arguments import TestOrder
+
         use_shuffle = TestOrder(litConfig.order) == TestOrder.RANDOM
         shard_env = {
-            'GTEST_OUTPUT': 'json:' + test.gtest_json_file,
-            'GTEST_SHUFFLE': '1' if use_shuffle else '0',
-            'GTEST_TOTAL_SHARDS': os.environ.get("GTEST_TOTAL_SHARDS", total_shards),
-            'GTEST_SHARD_INDEX': os.environ.get("GTEST_SHARD_INDEX", shard_idx)
+            "GTEST_OUTPUT": "json:" + test.gtest_json_file,
+            "GTEST_SHUFFLE": "1" if use_shuffle else "0",
+            "GTEST_TOTAL_SHARDS": os.environ.get("GTEST_TOTAL_SHARDS", total_shards),
+            "GTEST_SHARD_INDEX": os.environ.get("GTEST_SHARD_INDEX", shard_idx),
         }
         test.config.environment.update(shard_env)
 
         cmd = [testPath]
         cmd = self.prepareCmd(cmd)
         if litConfig.useValgrind:
             cmd = litConfig.valgrindArgs + cmd
 
         if litConfig.noExecute:
-            return lit.Test.PASS, ''
+            return lit.Test.PASS, ""
 
         def get_shard_header(shard_env):
-            shard_envs = ' '.join([k + '=' + v for k, v in shard_env.items()])
-            return f"Script(shard):\n--\n%s %s\n--\n" % (shard_envs, ' '.join(cmd))
+            shard_envs = " ".join([k + "=" + v for k, v in shard_env.items()])
+            return f"Script(shard):\n--\n%s %s\n--\n" % (shard_envs, " ".join(cmd))
 
         shard_header = get_shard_header(shard_env)
 
         try:
             out, _, exitCode = lit.util.executeCommand(
-                cmd, env=test.config.environment,
-                timeout=litConfig.maxIndividualTestTime, redirect_stderr=True)
+                cmd,
+                env=test.config.environment,
+                timeout=litConfig.maxIndividualTestTime,
+                redirect_stderr=True,
+            )
         except lit.util.ExecuteCommandTimeoutException as e:
             stream_msg = f"\n{e.out}\n--\nexit: {e.exitCode}\n--\n"
-            return (lit.Test.TIMEOUT, f'{shard_header}{stream_msg}Reached '
-                    f'timeout of {litConfig.maxIndividualTestTime} seconds')
+            return (
+                lit.Test.TIMEOUT,
+                f"{shard_header}{stream_msg}Reached "
+                f"timeout of {litConfig.maxIndividualTestTime} seconds",
+            )
 
         if not os.path.exists(test.gtest_json_file):
-            errmsg = f"shard JSON output does not exist: %s" % (
-                test.gtest_json_file)
+            errmsg = f"shard JSON output does not exist: %s" % (test.gtest_json_file)
             stream_msg = f"\n{out}\n--\nexit: {exitCode}\n--\n"
             return lit.Test.FAIL, shard_header + stream_msg + errmsg
 
         if exitCode == 0:
-            return lit.Test.PASS, ''
+            return lit.Test.PASS, ""
 
         def get_test_stdout(test_name):
             res = []
-            header = f'[ RUN      ] ' + test_name
-            footer = f'[  FAILED  ] ' + test_name
+            header = f"[ RUN      ] " + test_name
+            footer = f"[  FAILED  ] " + test_name
             in_range = False
             for l in out.splitlines():
                 if l.startswith(header):
                     in_range = True
                 elif l.startswith(footer):
-                    return f'' if len(res) == 0 else '\n'.join(res)
+                    return f"" if len(res) == 0 else "\n".join(res)
                 elif in_range:
                     res.append(l)
-            assert False, f'gtest did not report the result for ' + test_name
+            assert False, f"gtest did not report the result for " + test_name
 
         found_failed_test = False
 
-        with open(test.gtest_json_file, encoding='utf-8') as f:
+        with open(test.gtest_json_file, encoding="utf-8") as f:
             jf = json.load(f)
 
             if use_shuffle:
-                shard_env['GTEST_RANDOM_SEED'] = str(jf['random_seed'])
-            output = get_shard_header(shard_env) + '\n'
+                shard_env["GTEST_RANDOM_SEED"] = str(jf["random_seed"])
+            output = get_shard_header(shard_env) + "\n"
 
-            for testcase in jf['testsuites']:
-                for testinfo in testcase['testsuite']:
-                    result = testinfo['result']
-                    if result == 'SUPPRESSED' or result == 'SKIPPED':
+            for testcase in jf["testsuites"]:
+                for testinfo in testcase["testsuite"]:
+                    result = testinfo["result"]
+                    if result == "SUPPRESSED" or result == "SKIPPED":
                         continue
-                    testname = testcase['name'] + '.' + testinfo['name']
+                    testname = testcase["name"] + "." + testinfo["name"]
                     header = f"Script:\n--\n%s --gtest_filter=%s\n--\n" % (
-                        ' '.join(cmd), testname)
-                    if 'failures' in testinfo:
+                        " ".join(cmd),
+                        testname,
+                    )
+                    if "failures" in testinfo:
                         found_failed_test = True
                         output += header
                         test_out = get_test_stdout(testname)
                         if test_out:
-                            output += test_out + '\n\n'
-                        for fail in testinfo['failures']:
-                            output += fail['failure'] + '\n'
-                        output += '\n'
-                    elif result != 'COMPLETED':
+                            output += test_out + "\n\n"
+                        for fail in testinfo["failures"]:
+                            output += fail["failure"] + "\n"
+                        output += "\n"
+                    elif result != "COMPLETED":
                         output += header
-                        output += 'unresolved test result\n'
+                        output += "unresolved test result\n"
 
         # In some situations, like running tests with sanitizers, all test passes but
         # the shard could still fail due to memory issues.
         if not found_failed_test:
             output += f"\n{out}\n--\nexit: {exitCode}\n--\n"
 
         return lit.Test.FAIL, output
@@ -212,15 +233,15 @@
 
         It inserts the python exe into the command if cmd[0] ends in .py or caller
         specified run_under.
         We cannot rely on the system to interpret shebang lines for us on
         Windows, so add the python executable to the command if this is a .py
         script.
         """
-        if cmd[0].endswith('.py'):
+        if cmd[0].endswith(".py"):
             cmd = [sys.executable] + cmd
         if self.run_under:
             if isinstance(self.run_under, list):
                 cmd = self.run_under + cmd
             else:
                 cmd = shlex.split(self.run_under) + cmd
         return cmd
@@ -241,51 +262,60 @@
                 continue
 
             start_time = test.result.start or 0.0
 
             has_failure_in_shard = False
 
             # Load json file to retrieve results.
-            with open(test.gtest_json_file, encoding='utf-8') as f:
+            with open(test.gtest_json_file, encoding="utf-8") as f:
                 try:
-                    testsuites = json.load(f)['testsuites']
+                    testsuites = json.load(f)["testsuites"]
                 except json.JSONDecodeError as e:
-                    raise RuntimeError("Failed to parse json file: " +
-                                       test.gtest_json_file + "\n" + e.doc)
+                    raise RuntimeError(
+                        "Failed to parse json file: "
+                        + test.gtest_json_file
+                        + "\n"
+                        + e.doc
+                    )
                 for testcase in testsuites:
-                    for testinfo in testcase['testsuite']:
+                    for testinfo in testcase["testsuite"]:
                         # Ignore disabled tests.
-                        if testinfo['result'] == 'SUPPRESSED':
+                        if testinfo["result"] == "SUPPRESSED":
                             continue
 
-                        testPath = test.path_in_suite[:-2] + (testcase['name'],
-                                                              testinfo['name'])
-                        subtest = lit.Test.Test(test.suite, testPath,
-                                                test.config, test.file_path)
+                        testPath = test.path_in_suite[:-2] + (
+                            testcase["name"],
+                            testinfo["name"],
+                        )
+                        subtest = lit.Test.Test(
+                            test.suite, testPath, test.config, test.file_path
+                        )
 
-                        testname = testcase['name'] + '.' + testinfo['name']
+                        testname = testcase["name"] + "." + testinfo["name"]
                         header = f"Script:\n--\n%s --gtest_filter=%s\n--\n" % (
-                            test.file_path, testname)
+                            test.file_path,
+                            testname,
+                        )
 
-                        output = ''
-                        if testinfo['result'] == 'SKIPPED':
+                        output = ""
+                        if testinfo["result"] == "SKIPPED":
                             returnCode = lit.Test.SKIPPED
-                        elif 'failures' in testinfo:
+                        elif "failures" in testinfo:
                             has_failure_in_shard = True
                             returnCode = lit.Test.FAIL
                             output = header
-                            for fail in testinfo['failures']:
-                                output += fail['failure'] + '\n'
-                        elif testinfo['result'] == 'COMPLETED':
+                            for fail in testinfo["failures"]:
+                                output += fail["failure"] + "\n"
+                        elif testinfo["result"] == "COMPLETED":
                             returnCode = lit.Test.PASS
                         else:
                             returnCode = lit.Test.UNRESOLVED
-                            output = header + 'unresolved test result\n'
+                            output = header + "unresolved test result\n"
 
-                        elapsed_time = float(testinfo['time'][:-1])
+                        elapsed_time = float(testinfo["time"][:-1])
                         res = lit.Test.Result(returnCode, output, elapsed_time)
                         res.pid = test.result.pid or 0
                         res.start = start_time
                         start_time = start_time + elapsed_time
                         subtest.setResult(res)
 
                         selected_tests.append(subtest)
```

### Comparing `lit-16.0.6/lit/formats/shtest.py` & `lit-17.0.0rc1/lit/formats/shtest.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,18 +13,23 @@
     testing guide:
 
         http://llvm.org/docs/TestingGuide.html
 
     The ShTest files contain some number of shell-like command pipelines, along
     with assertions about what should be in the output.
     """
-    def __init__(self, execute_external=False, extra_substitutions=[],
-                 preamble_commands=[]):
+
+    def __init__(
+        self, execute_external=False, extra_substitutions=[], preamble_commands=[]
+    ):
         self.execute_external = execute_external
         self.extra_substitutions = extra_substitutions
         self.preamble_commands = preamble_commands
 
     def execute(self, test, litConfig):
-        return lit.TestRunner.executeShTest(test, litConfig,
-                                            self.execute_external,
-                                            self.extra_substitutions,
-                                            self.preamble_commands)
+        return lit.TestRunner.executeShTest(
+            test,
+            litConfig,
+            self.execute_external,
+            self.extra_substitutions,
+            self.preamble_commands,
+        )
```

### Comparing `lit-16.0.6/lit/llvm/subst.py` & `lit-17.0.0rc1/lit/llvm/subst.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,102 +8,106 @@
 
 
 class FindTool(object):
     def __init__(self, name):
         self.name = name
 
     def resolve(self, config, dirs):
-        # Check for a user explicitely overriding a tool.  This allows:
+        # Check for a user explicitly overriding a tool. This allows:
         #     llvm-lit -D llc="llc -enable-misched -verify-machineinstrs"
         command = config.lit_config.params.get(self.name)
         if command is None:
             # Then check out search paths.
             command = lit.util.which(self.name, dirs)
             if not command:
                 return None
 
-        if self.name == 'llc' and os.environ.get('LLVM_ENABLE_MACHINE_VERIFIER') == '1':
-            command += ' -verify-machineinstrs'
+        if self.name == "llc" and os.environ.get("LLVM_ENABLE_MACHINE_VERIFIER") == "1":
+            command += " -verify-machineinstrs"
         return command
 
 
 class ToolSubst(object):
     """String-like class used to build regex substitution patterns for llvm
     tools.
 
     Handles things like adding word-boundary patterns, and filtering
     characters from the beginning an end of a tool name
 
     """
 
-    def __init__(self, key, command=None, pre=r'.-^/\<', post='-.', verbatim=False,
-                 unresolved='warn', extra_args=None):
+    def __init__(
+        self,
+        key,
+        command=None,
+        pre=r".-^/\<",
+        post="-.",
+        verbatim=False,
+        unresolved="warn",
+        extra_args=None,
+    ):
         """Construct a ToolSubst.
 
         key: The text which is to be substituted.
 
-        command: The command to substitute when the key is matched.  By default,
-        this will treat `key` as a tool name and search for it.  If it is
-        a string, it is intereprted as an exact path.  If it is an instance of
+        command: The command to substitute when the key is matched. By default,
+        this will treat `key` as a tool name and search for it. If it is a
+        string, it is interpreted as an exact path. If it is an instance of
         FindTool, the specified tool name is searched for on disk.
 
         pre: If specified, the substitution will not find matches where
         the character immediately preceding the word-boundary that begins
         `key` is any of the characters in the string `pre`.
 
         post: If specified, the substitution will not find matches where
         the character immediately after the word-boundary that ends `key`
         is any of the characters specified in the string `post`.
 
         verbatim: If True, `key` is an exact regex that is passed to the
         underlying substitution
 
         unresolved: Action to take if the tool substitution cannot be
-        resolved.  Valid values:
+        resolved. Valid values:
             'warn' - log a warning but add the substitution anyway.
             'fatal' - Exit the test suite and log a fatal error.
             'break' - Don't add any of the substitutions from the current
                       group, and return a value indicating a failure.
             'ignore' - Don't add the substitution, and don't log an error
 
         extra_args: If specified, represents a list of arguments that will be
         appended to the tool's substitution.
 
-        explicit_path: If specified, the exact path will be used as a substitution.
-        Otherwise, the tool will be searched for as if by calling which(tool)
-
         """
         self.unresolved = unresolved
         self.extra_args = extra_args
         self.key = key
         self.command = command if command is not None else FindTool(key)
         self.was_resolved = False
         if verbatim:
             self.regex = key
             return
 
-        def not_in(chars, where=''):
+        def not_in(chars, where=""):
             if not chars:
-                return ''
-            pattern_str = '|'.join(re.escape(x) for x in chars)
-            return r'(?{}!({}))'.format(where, pattern_str)
+                return ""
+            pattern_str = "|".join(re.escape(x) for x in chars)
+            return r"(?{}!({}))".format(where, pattern_str)
 
         def wordify(word):
             match = wordifier.match(word)
             introducer = match.group(1)
             word = match.group(2)
-            return introducer + r'\b' + word + r'\b'
+            return introducer + r"\b" + word + r"\b"
 
-        self.regex = not_in(pre, '<') + wordify(key) + not_in(post)
+        self.regex = not_in(pre, "<") + wordify(key) + not_in(post)
 
     def resolve(self, config, search_dirs):
-        # Extract the tool name from the pattern.  This relies on the tool
-        # name being surrounded by \b word match operators.  If the
-        # pattern starts with "| ", include it in the string to be
-        # substituted.
+        # Extract the tool name from the pattern. This relies on the tool name
+        # being surrounded by \b word match operators. If the pattern starts
+        # with "| ", include it in the string to be substituted.
 
         tool_match = expr.match(self.regex)
         if not tool_match:
             return None
 
         tool_pipe = tool_match.group(2)
         tool_name = tool_match.group(4)
@@ -111,33 +115,34 @@
         if isinstance(self.command, FindTool):
             command_str = self.command.resolve(config, search_dirs)
         else:
             command_str = str(self.command)
 
         if command_str:
             if self.extra_args:
-                command_str = ' '.join([command_str] + self.extra_args)
+                command_str = " ".join([command_str] + self.extra_args)
         else:
-            if self.unresolved == 'warn':
+            if self.unresolved == "warn":
                 # Warn, but still provide a substitution.
                 config.lit_config.note(
-                    'Did not find ' + tool_name + ' in %s' % search_dirs)
-                command_str = os.path.join(
-                    config.config.llvm_tools_dir, tool_name)
-            elif self.unresolved == 'fatal':
+                    "Did not find " + tool_name + " in %s" % search_dirs
+                )
+                command_str = os.path.join(config.config.llvm_tools_dir, tool_name)
+            elif self.unresolved == "fatal":
                 # The function won't even return in this case, this leads to
                 # sys.exit
                 config.lit_config.fatal(
-                    'Did not find ' + tool_name + ' in %s' % search_dirs)
-            elif self.unresolved == 'break':
+                    "Did not find " + tool_name + " in %s" % search_dirs
+                )
+            elif self.unresolved == "break":
                 # By returning a valid result with an empty command, the
                 # caller treats this as a failure.
                 pass
-            elif self.unresolved == 'ignore':
+            elif self.unresolved == "ignore":
                 # By returning None, the caller just assumes there was no
                 # match in the first place.
                 return None
             else:
-                raise 'Unexpected value for ToolSubst.unresolved'
+                raise "Unexpected value for ToolSubst.unresolved"
         if command_str:
             self.was_resolved = True
         return (self.regex, tool_pipe, command_str)
```

### Comparing `lit-16.0.6/lit/main.py` & `lit-17.0.0rc1/lit/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,296 +21,334 @@
 from lit.formats.googletest import GoogleTest
 from lit.TestTimes import record_test_times
 
 
 def main(builtin_params={}):
     opts = lit.cl_arguments.parse_args()
     params = create_params(builtin_params, opts.user_params)
-    is_windows = platform.system() == 'Windows'
+    is_windows = platform.system() == "Windows"
 
     lit_config = lit.LitConfig.LitConfig(
         progname=os.path.basename(sys.argv[0]),
         path=opts.path,
         quiet=opts.quiet,
         useValgrind=opts.useValgrind,
         valgrindLeakCheck=opts.valgrindLeakCheck,
         valgrindArgs=opts.valgrindArgs,
         noExecute=opts.noExecute,
         debug=opts.debug,
         isWindows=is_windows,
         order=opts.order,
         params=params,
         config_prefix=opts.configPrefix,
-        echo_all_commands=opts.echoAllCommands)
+        echo_all_commands=opts.echoAllCommands,
+    )
 
-    discovered_tests = lit.discovery.find_tests_for_inputs(lit_config, opts.test_paths,
-                                                           opts.indirectlyRunCheck)
+    discovered_tests = lit.discovery.find_tests_for_inputs(
+        lit_config, opts.test_paths
+    )
     if not discovered_tests:
-        sys.stderr.write('error: did not discover any tests for provided path(s)\n')
+        sys.stderr.write("error: did not discover any tests for provided path(s)\n")
         sys.exit(2)
 
     if opts.show_suites or opts.show_tests:
         print_discovered(discovered_tests, opts.show_suites, opts.show_tests)
         sys.exit(0)
 
     if opts.show_used_features:
-        features = set(itertools.chain.from_iterable(t.getUsedFeatures() for t in discovered_tests if t.gtest_json_file is None))
-        print(' '.join(sorted(features)))
+        features = set(
+            itertools.chain.from_iterable(
+                t.getUsedFeatures()
+                for t in discovered_tests
+                if t.gtest_json_file is None
+            )
+        )
+        print(" ".join(sorted(features)))
         sys.exit(0)
 
     # Command line overrides configuration for maxIndividualTestTime.
     if opts.maxIndividualTestTime is not None:  # `not None` is important (default: 0)
         if opts.maxIndividualTestTime != lit_config.maxIndividualTestTime:
-            lit_config.note(('The test suite configuration requested an individual'
-                ' test timeout of {0} seconds but a timeout of {1} seconds was'
-                ' requested on the command line. Forcing timeout to be {1}'
-                ' seconds')
-                .format(lit_config.maxIndividualTestTime,
-                        opts.maxIndividualTestTime))
+            lit_config.note(
+                (
+                    "The test suite configuration requested an individual"
+                    " test timeout of {0} seconds but a timeout of {1} seconds was"
+                    " requested on the command line. Forcing timeout to be {1}"
+                    " seconds"
+                ).format(lit_config.maxIndividualTestTime, opts.maxIndividualTestTime)
+            )
             lit_config.maxIndividualTestTime = opts.maxIndividualTestTime
 
     determine_order(discovered_tests, opts.order)
 
-    selected_tests = [t for t in discovered_tests if
-        opts.filter.search(t.getFullName()) and not
-        opts.filter_out.search(t.getFullName())]
+    selected_tests = [
+        t
+        for t in discovered_tests
+        if opts.filter.search(t.getFullName())
+        and not opts.filter_out.search(t.getFullName())
+    ]
 
     if not selected_tests:
-        sys.stderr.write('error: filter did not match any tests '
-                         '(of %d discovered).  ' % len(discovered_tests))
+        sys.stderr.write(
+            "error: filter did not match any tests "
+            "(of %d discovered).  " % len(discovered_tests)
+        )
         if opts.allow_empty_runs:
-            sys.stderr.write("Suppressing error because '--allow-empty-runs' "
-                             'was specified.\n')
+            sys.stderr.write(
+                "Suppressing error because '--allow-empty-runs' " "was specified.\n"
+            )
             sys.exit(0)
         else:
-            sys.stderr.write("Use '--allow-empty-runs' to suppress this "
-                             'error.\n')
+            sys.stderr.write("Use '--allow-empty-runs' to suppress this " "error.\n")
             sys.exit(2)
 
     # When running multiple shards, don't include skipped tests in the xunit
     # output since merging the files will result in duplicates.
     if opts.shard:
         (run, shards) = opts.shard
         selected_tests = filter_by_shard(selected_tests, run, shards, lit_config)
         if not selected_tests:
-            sys.stderr.write('warning: shard does not contain any tests.  '
-                             'Consider decreasing the number of shards.\n')
+            sys.stderr.write(
+                "warning: shard does not contain any tests.  "
+                "Consider decreasing the number of shards.\n"
+            )
             sys.exit(0)
 
-    selected_tests = selected_tests[:opts.max_tests]
+    selected_tests = selected_tests[: opts.max_tests]
 
     mark_xfail(discovered_tests, opts)
 
     mark_excluded(discovered_tests, selected_tests)
 
     start = time.time()
     run_tests(selected_tests, lit_config, opts, len(discovered_tests))
     elapsed = time.time() - start
 
     record_test_times(selected_tests, lit_config)
 
     selected_tests, discovered_tests = GoogleTest.post_process_shard_results(
-        selected_tests, discovered_tests)
+        selected_tests, discovered_tests
+    )
 
     if opts.time_tests:
         print_histogram(discovered_tests)
 
     print_results(discovered_tests, elapsed, opts)
 
     tests_for_report = selected_tests if opts.shard else discovered_tests
     for report in opts.reports:
         report.write_results(tests_for_report, elapsed)
 
     if lit_config.numErrors:
-        sys.stderr.write('\n%d error(s) in tests\n' % lit_config.numErrors)
+        sys.stderr.write("\n%d error(s) in tests\n" % lit_config.numErrors)
         sys.exit(2)
 
     if lit_config.numWarnings:
-        sys.stderr.write('\n%d warning(s) in tests\n' % lit_config.numWarnings)
+        sys.stderr.write("\n%d warning(s) in tests\n" % lit_config.numWarnings)
 
     has_failure = any(t.isFailure() for t in discovered_tests)
     if has_failure:
         if opts.ignoreFail:
-            sys.stderr.write("\nExiting with status 0 instead of 1 because "
-                             "'--ignore-fail' was specified.\n")
+            sys.stderr.write(
+                "\nExiting with status 0 instead of 1 because "
+                "'--ignore-fail' was specified.\n"
+            )
         else:
             sys.exit(1)
 
+
 def create_params(builtin_params, user_params):
     def parse(p):
-        return p.split('=', 1) if '=' in p else (p, '')
+        return p.split("=", 1) if "=" in p else (p, "")
 
     params = dict(builtin_params)
     params.update([parse(p) for p in user_params])
     return params
 
 
 def print_discovered(tests, show_suites, show_tests):
     tests.sort(key=lit.reports.by_suite_and_test_path)
 
     if show_suites:
         tests_by_suite = itertools.groupby(tests, lambda t: t.suite)
-        print('-- Test Suites --')
+        print("-- Test Suites --")
         for suite, test_iter in tests_by_suite:
             test_count = sum(1 for _ in test_iter)
-            print('  %s - %d tests' % (suite.name, test_count))
-            print('    Source Root: %s' % suite.source_root)
-            print('    Exec Root  : %s' % suite.exec_root)
-            features = ' '.join(sorted(suite.config.available_features))
-            print('    Available Features: %s' % features)
+            print("  %s - %d tests" % (suite.name, test_count))
+            print("    Source Root: %s" % suite.source_root)
+            print("    Exec Root  : %s" % suite.exec_root)
+            features = " ".join(sorted(suite.config.available_features))
+            print("    Available Features: %s" % features)
             substitutions = sorted(suite.config.substitutions)
-            substitutions = ('%s => %s' % (x, y) for (x, y) in substitutions)
-            substitutions = '\n'.ljust(30).join(substitutions)
-            print('    Available Substitutions: %s' % substitutions)
+            substitutions = ("%s => %s" % (x, y) for (x, y) in substitutions)
+            substitutions = "\n".ljust(30).join(substitutions)
+            print("    Available Substitutions: %s" % substitutions)
 
     if show_tests:
-        print('-- Available Tests --')
+        print("-- Available Tests --")
         for t in tests:
-            print('  %s' % t.getFullName())
+            print("  %s" % t.getFullName())
 
 
 def determine_order(tests, order):
     from lit.cl_arguments import TestOrder
+
     enum_order = TestOrder(order)
     if enum_order == TestOrder.RANDOM:
         import random
+
         random.shuffle(tests)
     elif enum_order == TestOrder.LEXICAL:
         tests.sort(key=lambda t: t.getFullName())
     else:
-        assert enum_order == TestOrder.SMART, 'Unknown TestOrder value'
-        tests.sort(key=lambda t: (not t.previous_failure, -t.previous_elapsed, t.getFullName()))
+        assert enum_order == TestOrder.SMART, "Unknown TestOrder value"
+        tests.sort(
+            key=lambda t: (not t.previous_failure, -t.previous_elapsed, t.getFullName())
+        )
 
 
 def filter_by_shard(tests, run, shards, lit_config):
     test_ixs = range(run - 1, len(tests), shards)
     selected_tests = [tests[i] for i in test_ixs]
 
     # For clarity, generate a preview of the first few test indices in the shard
     # to accompany the arithmetic expression.
     preview_len = 3
-    preview = ', '.join([str(i + 1) for i in test_ixs[:preview_len]])
+    preview = ", ".join([str(i + 1) for i in test_ixs[:preview_len]])
     if len(test_ixs) > preview_len:
-        preview += ', ...'
-    msg = f'Selecting shard {run}/{shards} = ' \
-          f'size {len(selected_tests)}/{len(tests)} = ' \
-          f'tests #({shards}*k)+{run} = [{preview}]'
+        preview += ", ..."
+    msg = (
+        f"Selecting shard {run}/{shards} = "
+        f"size {len(selected_tests)}/{len(tests)} = "
+        f"tests #({shards}*k)+{run} = [{preview}]"
+    )
     lit_config.note(msg)
     return selected_tests
 
 
 def mark_xfail(selected_tests, opts):
     for t in selected_tests:
         test_file = os.sep.join(t.path_in_suite)
         test_full_name = t.getFullName()
         if test_file in opts.xfail or test_full_name in opts.xfail:
-            t.xfails += '*'
+            t.xfails += "*"
         if test_file in opts.xfail_not or test_full_name in opts.xfail_not:
             t.xfail_not = True
 
+
 def mark_excluded(discovered_tests, selected_tests):
     excluded_tests = set(discovered_tests) - set(selected_tests)
     result = lit.Test.Result(lit.Test.EXCLUDED)
     for t in excluded_tests:
         t.setResult(result)
 
 
 def run_tests(tests, lit_config, opts, discovered_tests):
     workers = min(len(tests), opts.workers)
     display = lit.display.create_display(opts, tests, discovered_tests, workers)
 
-    run = lit.run.Run(tests, lit_config, workers, display.update,
-                      opts.max_failures, opts.timeout)
+    run = lit.run.Run(
+        tests, lit_config, workers, display.update, opts.max_failures, opts.timeout
+    )
 
     display.print_header()
 
     interrupted = False
     error = None
     try:
         execute_in_tmp_dir(run, lit_config)
     except KeyboardInterrupt:
         interrupted = True
-        error = '  interrupted by user'
+        error = "  interrupted by user"
     except lit.run.MaxFailuresError:
-        error = 'warning: reached maximum number of test failures'
+        error = "warning: reached maximum number of test failures"
     except lit.run.TimeoutError:
-        error = 'warning: reached timeout'
+        error = "warning: reached timeout"
 
     display.clear(interrupted)
     if error:
-        sys.stderr.write('%s, skipping remaining tests\n' % error)
+        sys.stderr.write("%s, skipping remaining tests\n" % error)
 
 
 def execute_in_tmp_dir(run, lit_config):
     # Create a temp directory inside the normal temp directory so that we can
     # try to avoid temporary test file leaks. The user can avoid this behavior
     # by setting LIT_PRESERVES_TMP in the environment, so they can easily use
     # their own temp directory to monitor temporary file leaks or handle them at
     # the buildbot level.
     tmp_dir = None
-    if 'LIT_PRESERVES_TMP' not in os.environ:
+    if "LIT_PRESERVES_TMP" not in os.environ:
         import tempfile
+
         # z/OS linker does not support '_' in paths, so use '-'.
-        tmp_dir = tempfile.mkdtemp(prefix='lit-tmp-')
-        tmp_dir_envs = {k: tmp_dir for k in ['TMP', 'TMPDIR', 'TEMP', 'TEMPDIR']}
+        tmp_dir = tempfile.mkdtemp(prefix="lit-tmp-")
+        tmp_dir_envs = {k: tmp_dir for k in ["TMP", "TMPDIR", "TEMP", "TEMPDIR"]}
         os.environ.update(tmp_dir_envs)
         for cfg in {t.config for t in run.tests}:
             cfg.environment.update(tmp_dir_envs)
     try:
         run.execute()
     finally:
         if tmp_dir:
             try:
                 import shutil
+
                 shutil.rmtree(tmp_dir)
-            except Exception as e: 
-                lit_config.warning("Failed to delete temp directory '%s', try upgrading your version of Python to fix this" % tmp_dir)
+            except Exception as e:
+                lit_config.warning(
+                    "Failed to delete temp directory '%s', try upgrading your version of Python to fix this"
+                    % tmp_dir
+                )
 
 
 def print_histogram(tests):
-    test_times = [(t.getFullName(), t.result.elapsed)
-                  for t in tests if t.result.elapsed]
+    test_times = [
+        (t.getFullName(), t.result.elapsed) for t in tests if t.result.elapsed
+    ]
     if test_times:
-        lit.util.printHistogram(test_times, title='Tests')
+        lit.util.printHistogram(test_times, title="Tests")
 
 
 def print_results(tests, elapsed, opts):
     tests_by_code = {code: [] for code in lit.Test.ResultCode.all_codes()}
     for test in tests:
         tests_by_code[test.result.code].append(test)
 
     for code in lit.Test.ResultCode.all_codes():
-        print_group(sorted(tests_by_code[code], key=lambda t: t.getFullName()), code, opts.shown_codes)
+        print_group(
+            sorted(tests_by_code[code], key=lambda t: t.getFullName()),
+            code,
+            opts.shown_codes,
+        )
 
     print_summary(tests_by_code, opts.quiet, elapsed)
 
 
 def print_group(tests, code, shown_codes):
     if not tests:
         return
     if not code.isFailure and code not in shown_codes:
         return
-    print('*' * 20)
-    print('{} Tests ({}):'.format(code.label, len(tests)))
+    print("*" * 20)
+    print("{} Tests ({}):".format(code.label, len(tests)))
     for test in tests:
-        print('  %s' % test.getFullName())
-    sys.stdout.write('\n')
+        print("  %s" % test.getFullName())
+    sys.stdout.write("\n")
 
 
 def print_summary(tests_by_code, quiet, elapsed):
     if not quiet:
-        print('\nTesting Time: %.2fs' % elapsed)
+        print("\nTesting Time: %.2fs" % elapsed)
 
-    codes = [c for c in lit.Test.ResultCode.all_codes()
-             if not quiet or c.isFailure]
+    codes = [c for c in lit.Test.ResultCode.all_codes() if not quiet or c.isFailure]
     groups = [(c.label, len(tests_by_code[c])) for c in codes]
     groups = [(label, count) for label, count in groups if count]
     if not groups:
         return
 
     max_label_len = max(len(label) for label, _ in groups)
     max_count_len = max(len(str(count)) for _, count in groups)
 
     for (label, count) in groups:
         label = label.ljust(max_label_len)
         count = str(count).rjust(max_count_len)
-        print('  %s: %s' % (label, count))
+        print("  %s: %s" % (label, count))
```

### Comparing `lit-16.0.6/lit/reports.py` & `lit-17.0.0rc1/lit/reports.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,61 +20,65 @@
 
     def write_results(self, tests, elapsed):
         unexecuted_codes = {lit.Test.EXCLUDED, lit.Test.SKIPPED}
         tests = [t for t in tests if t.result.code not in unexecuted_codes]
         # Construct the data we will write.
         data = {}
         # Encode the current lit version as a schema version.
-        data['__version__'] = lit.__versioninfo__
-        data['elapsed'] = elapsed
+        data["__version__"] = lit.__versioninfo__
+        data["elapsed"] = elapsed
         # FIXME: Record some information on the lit configuration used?
         # FIXME: Record information from the individual test suites?
 
         # Encode the tests.
-        data['tests'] = tests_data = []
+        data["tests"] = tests_data = []
         for test in tests:
             test_data = {
-                'name': test.getFullName(),
-                'code': test.result.code.name,
-                'output': test.result.output,
-                'elapsed': test.result.elapsed}
+                "name": test.getFullName(),
+                "code": test.result.code.name,
+                "output": test.result.output,
+                "elapsed": test.result.elapsed,
+            }
 
             # Add test metrics, if present.
             if test.result.metrics:
-                test_data['metrics'] = metrics_data = {}
+                test_data["metrics"] = metrics_data = {}
                 for key, value in test.result.metrics.items():
                     metrics_data[key] = value.todata()
 
             # Report micro-tests separately, if present
             if test.result.microResults:
                 for key, micro_test in test.result.microResults.items():
                     # Expand parent test name with micro test name
                     parent_name = test.getFullName()
-                    micro_full_name = parent_name + ':' + key
+                    micro_full_name = parent_name + ":" + key
 
                     micro_test_data = {
-                        'name': micro_full_name,
-                        'code': micro_test.code.name,
-                        'output': micro_test.output,
-                        'elapsed': micro_test.elapsed}
+                        "name": micro_full_name,
+                        "code": micro_test.code.name,
+                        "output": micro_test.output,
+                        "elapsed": micro_test.elapsed,
+                    }
                     if micro_test.metrics:
-                        micro_test_data['metrics'] = micro_metrics_data = {}
+                        micro_test_data["metrics"] = micro_metrics_data = {}
                         for key, value in micro_test.metrics.items():
                             micro_metrics_data[key] = value.todata()
 
                     tests_data.append(micro_test_data)
 
             tests_data.append(test_data)
 
-        with open(self.output_file, 'w') as file:
+        with open(self.output_file, "w") as file:
             json.dump(data, file, indent=2, sort_keys=True)
-            file.write('\n')
+            file.write("\n")
 
 
-_invalid_xml_chars_dict = {c: None for c in range(32) if chr(c) not in ('\t', '\n', '\r')}
+_invalid_xml_chars_dict = {
+    c: None for c in range(32) if chr(c) not in ("\t", "\n", "\r")
+}
 
 
 def remove_invalid_xml_chars(s):
     # According to the XML 1.0 spec, control characters other than
     # \t,\r, and \n are not permitted anywhere in the document
     # (https://www.w3.org/TR/xml/#charsets) and therefore this function
     # removes them to produce a valid XML document.
@@ -83,130 +87,133 @@
     # but lit currently produces XML 1.0 output.
     return s.translate(_invalid_xml_chars_dict)
 
 
 class XunitReport(object):
     def __init__(self, output_file):
         self.output_file = output_file
-        self.skipped_codes = {lit.Test.EXCLUDED,
-                              lit.Test.SKIPPED, lit.Test.UNSUPPORTED}
+        self.skipped_codes = {lit.Test.EXCLUDED, lit.Test.SKIPPED, lit.Test.UNSUPPORTED}
 
     def write_results(self, tests, elapsed):
         tests.sort(key=by_suite_and_test_path)
         tests_by_suite = itertools.groupby(tests, lambda t: t.suite)
 
-        with open(self.output_file, 'w') as file:
+        with open(self.output_file, "w") as file:
             file.write('<?xml version="1.0" encoding="UTF-8"?>\n')
             file.write('<testsuites time="{time:.2f}">\n'.format(time=elapsed))
             for suite, test_iter in tests_by_suite:
                 self._write_testsuite(file, suite, list(test_iter))
-            file.write('</testsuites>\n')
+            file.write("</testsuites>\n")
 
     def _write_testsuite(self, file, suite, tests):
         skipped = sum(1 for t in tests if t.result.code in self.skipped_codes)
         failures = sum(1 for t in tests if t.isFailure())
 
-        name = suite.config.name.replace('.', '-')
-        file.write(f'<testsuite name={quo(name)} tests="{len(tests)}" failures="{failures}" skipped="{skipped}">\n')
+        name = suite.config.name.replace(".", "-")
+        file.write(
+            f'<testsuite name={quo(name)} tests="{len(tests)}" failures="{failures}" skipped="{skipped}">\n'
+        )
         for test in tests:
             self._write_test(file, test, name)
-        file.write('</testsuite>\n')
+        file.write("</testsuite>\n")
 
     def _write_test(self, file, test, suite_name):
-        path = '/'.join(test.path_in_suite[:-1]).replace('.', '_')
-        class_name = f'{suite_name}.{path or suite_name}'
+        path = "/".join(test.path_in_suite[:-1]).replace(".", "_")
+        class_name = f"{suite_name}.{path or suite_name}"
         name = test.path_in_suite[-1]
         time = test.result.elapsed or 0.0
-        file.write(f'<testcase classname={quo(class_name)} name={quo(name)} time="{time:.2f}"')
+        file.write(
+            f'<testcase classname={quo(class_name)} name={quo(name)} time="{time:.2f}"'
+        )
 
         if test.isFailure():
-            file.write('>\n  <failure><![CDATA[')
+            file.write(">\n  <failure><![CDATA[")
             # In the unlikely case that the output contains the CDATA
             # terminator we wrap it by creating a new CDATA block.
-            output = test.result.output.replace(']]>', ']]]]><![CDATA[>')
+            output = test.result.output.replace("]]>", "]]]]><![CDATA[>")
             if isinstance(output, bytes):
-                output = output.decode("utf-8", 'ignore')
+                output = output.decode("utf-8", "ignore")
 
             # Failing test  output sometimes contains control characters like
             # \x1b (e.g. if there was some -fcolor-diagnostics output) which are
             # not allowed inside XML files.
             # This causes problems with CI systems: for example, the Jenkins
             # JUnit XML will throw an exception when ecountering those
             # characters and similar problems also occur with GitLab CI.
             output = remove_invalid_xml_chars(output)
             file.write(output)
-            file.write(']]></failure>\n</testcase>\n')
+            file.write("]]></failure>\n</testcase>\n")
         elif test.result.code in self.skipped_codes:
             reason = self._get_skip_reason(test)
-            file.write(f'>\n  <skipped message={quo(reason)}/>\n</testcase>\n')
+            file.write(f">\n  <skipped message={quo(reason)}/>\n</testcase>\n")
         else:
-            file.write('/>\n')
+            file.write("/>\n")
 
     def _get_skip_reason(self, test):
         code = test.result.code
         if code == lit.Test.EXCLUDED:
-            return 'Test not selected (--filter, --max-tests)'
+            return "Test not selected (--filter, --max-tests)"
         if code == lit.Test.SKIPPED:
-            return 'User interrupt'
+            return "User interrupt"
 
         assert code == lit.Test.UNSUPPORTED
         features = test.getMissingRequiredFeatures()
         if features:
-            return 'Missing required feature(s): ' + ', '.join(features)
-        return 'Unsupported configuration'
+            return "Missing required feature(s): " + ", ".join(features)
+        return "Unsupported configuration"
 
 
 def gen_resultdb_test_entry(
     test_name, start_time, elapsed_time, test_output, result_code, is_expected
 ):
     test_data = {
-        'testId': test_name,
-        'start_time': datetime.datetime.fromtimestamp(start_time).isoformat() + 'Z',
-        'duration': '%.9fs' % elapsed_time,
-        'summary_html': '<p><text-artifact artifact-id="artifact-content-in-request"></p>',
-        'artifacts': {
-            'artifact-content-in-request': {
-                'contents': base64.b64encode(test_output.encode('utf-8')).decode(
-                    'utf-8'
+        "testId": test_name,
+        "start_time": datetime.datetime.fromtimestamp(start_time).isoformat() + "Z",
+        "duration": "%.9fs" % elapsed_time,
+        "summary_html": '<p><text-artifact artifact-id="artifact-content-in-request"></p>',
+        "artifacts": {
+            "artifact-content-in-request": {
+                "contents": base64.b64encode(test_output.encode("utf-8")).decode(
+                    "utf-8"
                 ),
             },
         },
-        'expected': is_expected,
+        "expected": is_expected,
     }
     if (
         result_code == lit.Test.PASS
         or result_code == lit.Test.XPASS
         or result_code == lit.Test.FLAKYPASS
     ):
-        test_data['status'] = 'PASS'
+        test_data["status"] = "PASS"
     elif result_code == lit.Test.FAIL or result_code == lit.Test.XFAIL:
-        test_data['status'] = 'FAIL'
+        test_data["status"] = "FAIL"
     elif (
         result_code == lit.Test.UNSUPPORTED
         or result_code == lit.Test.SKIPPED
         or result_code == lit.Test.EXCLUDED
     ):
-        test_data['status'] = 'SKIP'
+        test_data["status"] = "SKIP"
     elif result_code == lit.Test.UNRESOLVED or result_code == lit.Test.TIMEOUT:
-        test_data['status'] = 'ABORT'
+        test_data["status"] = "ABORT"
     return test_data
 
 
 class ResultDBReport(object):
     def __init__(self, output_file):
         self.output_file = output_file
 
     def write_results(self, tests, elapsed):
         unexecuted_codes = {lit.Test.EXCLUDED, lit.Test.SKIPPED}
         tests = [t for t in tests if t.result.code not in unexecuted_codes]
         data = {}
-        data['__version__'] = lit.__versioninfo__
-        data['elapsed'] = elapsed
+        data["__version__"] = lit.__versioninfo__
+        data["elapsed"] = elapsed
         # Encode the tests.
-        data['tests'] = tests_data = []
+        data["tests"] = tests_data = []
         for test in tests:
             tests_data.append(
                 gen_resultdb_test_entry(
                     test_name=test.getFullName(),
                     start_time=test.result.start,
                     elapsed_time=test.result.elapsed,
                     test_output=test.result.output,
@@ -214,15 +221,15 @@
                     is_expected=not test.result.code.isFailure,
                 )
             )
             if test.result.microResults:
                 for key, micro_test in test.result.microResults.items():
                     # Expand parent test name with micro test name
                     parent_name = test.getFullName()
-                    micro_full_name = parent_name + ':' + key + 'microres'
+                    micro_full_name = parent_name + ":" + key + "microres"
                     tests_data.append(
                         gen_resultdb_test_entry(
                             test_name=micro_full_name,
                             start_time=micro_test.start
                             if micro_test.start
                             else test.result.start,
                             elapsed_time=micro_test.elapsed
@@ -230,42 +237,44 @@
                             else test.result.elapsed,
                             test_output=micro_test.output,
                             result_code=micro_test.code,
                             is_expected=not micro_test.code.isFailure,
                         )
                     )
 
-        with open(self.output_file, 'w') as file:
+        with open(self.output_file, "w") as file:
             json.dump(data, file, indent=2, sort_keys=True)
-            file.write('\n')
+            file.write("\n")
 
 
 class TimeTraceReport(object):
     def __init__(self, output_file):
         self.output_file = output_file
-        self.skipped_codes = {lit.Test.EXCLUDED,
-                              lit.Test.SKIPPED, lit.Test.UNSUPPORTED}
+        self.skipped_codes = {lit.Test.EXCLUDED, lit.Test.SKIPPED, lit.Test.UNSUPPORTED}
 
     def write_results(self, tests, elapsed):
         # Find when first test started so we can make start times relative.
         first_start_time = min([t.result.start for t in tests])
-        events = [self._get_test_event(
-            x, first_start_time) for x in tests if x.result.code not in self.skipped_codes]
+        events = [
+            self._get_test_event(x, first_start_time)
+            for x in tests
+            if x.result.code not in self.skipped_codes
+        ]
 
-        json_data = {'traceEvents': events}
+        json_data = {"traceEvents": events}
 
         with open(self.output_file, "w") as time_trace_file:
             json.dump(json_data, time_trace_file, indent=2, sort_keys=True)
 
     def _get_test_event(self, test, first_start_time):
         test_name = test.getFullName()
         elapsed_time = test.result.elapsed or 0.0
         start_time = test.result.start - first_start_time if test.result.start else 0.0
         pid = test.result.pid or 0
         return {
-            'pid': pid,
-            'tid': 1,
-            'ph': 'X',
-            'ts': int(start_time * 1000000.),
-            'dur': int(elapsed_time * 1000000.),
-            'name': test_name,
+            "pid": pid,
+            "tid": 1,
+            "ph": "X",
+            "ts": int(start_time * 1000000.0),
+            "dur": int(elapsed_time * 1000000.0),
+            "name": test_name,
         }
```

### Comparing `lit-16.0.6/lit/run.py` & `lit-17.0.0rc1/lit/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 import lit.Test
 import lit.util
 import lit.worker
 
 
 class MaxFailuresError(Exception):
     pass
+
+
 class TimeoutError(Exception):
     pass
 
 
 class Run(object):
     """A concrete, configured testing run."""
 
-    def __init__(self, tests, lit_config, workers, progress_callback,
-                 max_failures, timeout):
+    def __init__(
+        self, tests, lit_config, workers, progress_callback, max_failures, timeout
+    ):
         self.tests = tests
         self.lit_config = lit_config
         self.workers = workers
         self.progress_callback = progress_callback
         self.max_failures = max_failures
         self.timeout = timeout
         assert workers > 0
@@ -58,25 +61,30 @@
             for test in self.tests:
                 if test.result is None:
                     test.setResult(skipped)
 
     def _execute(self, deadline):
         self._increase_process_limit()
 
-        semaphores = {k: multiprocessing.BoundedSemaphore(v)
-                      for k, v in self.lit_config.parallelism_groups.items()
-                      if v is not None}
-
-        pool = multiprocessing.Pool(self.workers, lit.worker.initialize,
-                                    (self.lit_config, semaphores))
+        semaphores = {
+            k: multiprocessing.BoundedSemaphore(v)
+            for k, v in self.lit_config.parallelism_groups.items()
+            if v is not None
+        }
+
+        pool = multiprocessing.Pool(
+            self.workers, lit.worker.initialize, (self.lit_config, semaphores)
+        )
 
         async_results = [
-            pool.apply_async(lit.worker.execute, args=[test],
-                             callback=self.progress_callback)
-            for test in self.tests]
+            pool.apply_async(
+                lit.worker.execute, args=[test], callback=self.progress_callback
+            )
+            for test in self.tests
+        ]
         pool.close()
 
         try:
             self._wait_for(async_results, deadline)
         except:
             pool.terminate()
             raise
@@ -107,25 +115,27 @@
 
     # TODO(yln): interferes with progress bar
     # Some tests use threads internally, and at least on Linux each of these
     # threads counts toward the current process limit. Try to raise the (soft)
     # process limit so that tests don't fail due to resource exhaustion.
     def _increase_process_limit(self):
         ncpus = lit.util.usable_core_count()
-        desired_limit = self.workers * ncpus * 2 # the 2 is a safety factor
+        desired_limit = self.workers * ncpus * 2  # the 2 is a safety factor
 
         # Importing the resource module will likely fail on Windows.
         try:
             import resource
+
             NPROC = resource.RLIMIT_NPROC
 
             soft_limit, hard_limit = resource.getrlimit(NPROC)
             desired_limit = min(desired_limit, hard_limit)
 
             if soft_limit < desired_limit:
                 resource.setrlimit(NPROC, (desired_limit, hard_limit))
-                self.lit_config.note('Raised process limit from %d to %d' % \
-                                        (soft_limit, desired_limit))
+                self.lit_config.note(
+                    "Raised process limit from %d to %d" % (soft_limit, desired_limit)
+                )
         except Exception as ex:
             # Warn, unless this is Windows, in which case this is expected.
-            if os.name != 'nt':
-                self.lit_config.warning('Failed to raise process limit: %s' % ex)
+            if os.name != "nt":
+                self.lit_config.warning("Failed to raise process limit: %s" % ex)
```

### Comparing `lit-16.0.6/lit/util.py` & `lit-17.0.0rc1/lit/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     if value is None:
         return False
     if type(value) is bool:
         return value
     if isinstance(value, numbers.Number):
         return value != 0
     if is_string(value):
-        if value.lower() in ('1', 'true', 'on', 'yes'):
+        if value.lower() in ("1", "true", "on", "yes"):
             return True
-        if value.lower() in ('', '0', 'false', 'off', 'no'):
+        if value.lower() in ("", "0", "false", "off", "no"):
             return False
     raise ValueError('"{}" is not a valid boolean'.format(value))
 
 
 def make_word_regex(word):
-    return r'\b' + word + r'\b'
+    return r"\b" + word + r"\b"
 
 
 def to_bytes(s):
     """Return the parameter as type 'bytes', possibly encoding it.
 
     In Python2, the 'bytes' type is the same as 'str'. In Python3, they
     are distinct.
@@ -49,15 +49,15 @@
     if isinstance(s, bytes):
         # In Python2, this branch is taken for both 'str' and 'bytes'.
         # In Python3, this branch is taken only for 'bytes'.
         return s
     # In Python2, 's' is a 'unicode' object.
     # In Python3, 's' is a 'str' object.
     # Encode to UTF-8 to get 'bytes' data.
-    return s.encode('utf-8')
+    return s.encode("utf-8")
 
 
 def to_string(b):
     """Return the parameter as type 'str', possibly encoding it.
 
     In Python2, the 'str' type is the same as 'bytes'. In Python3, the
     'str' type is (essentially) Python2's 'unicode' type, and 'bytes' is
@@ -68,15 +68,15 @@
         # In Python2, this branch is taken for types 'str' and 'bytes'.
         # In Python3, this branch is taken only for 'str'.
         return b
     if isinstance(b, bytes):
         # In Python2, this branch is never taken ('bytes' is handled as 'str').
         # In Python3, this is true only for 'bytes'.
         try:
-            return b.decode('utf-8')
+            return b.decode("utf-8")
         except UnicodeDecodeError:
             # If the value is not valid Unicode, return the default
             # repr-line encoding.
             return str(b)
 
     # By this point, here's what we *don't* have:
     #
@@ -86,30 +86,30 @@
     #    - 'str' (1st branch above)
     #    - 'bytes' (2nd branch above)
     #
     # The last type we might expect is the Python2 'unicode' type. There is no
     # 'unicode' type in Python3 (all the Python3 cases were already handled). In
     # order to get a 'str' object, we need to encode the 'unicode' object.
     try:
-        return b.encode('utf-8')
+        return b.encode("utf-8")
     except AttributeError:
-        raise TypeError('not sure how to convert %s to %s' % (type(b), str))
+        raise TypeError("not sure how to convert %s to %s" % (type(b), str))
 
 
 def to_unicode(s):
     """Return the parameter as type which supports unicode, possibly decoding
     it.
 
     In Python2, this is the unicode type. In Python3 it's the str type.
 
     """
     if isinstance(s, bytes):
         # In Python2, this branch is taken for both 'str' and 'bytes'.
         # In Python3, this branch is taken only for 'bytes'.
-        return s.decode('utf-8')
+        return s.decode("utf-8")
     return s
 
 
 def usable_core_count():
     """Return the number of cores the current process can use, if supported.
     Otherwise, return the total number of cores (like `os.cpu_count()`).
     Default to 1 if undetermined.
@@ -118,32 +118,32 @@
     try:
         n = len(os.sched_getaffinity(0))
     except AttributeError:
         n = os.cpu_count() or 1
 
     # On Windows with more than 60 processes, multiprocessing's call to
     # _winapi.WaitForMultipleObjects() prints an error and lit hangs.
-    if platform.system() == 'Windows':
+    if platform.system() == "Windows":
         return min(n, 60)
 
     return n
 
 
 def mkdir(path):
     try:
-        if platform.system() == 'Windows':
+        if platform.system() == "Windows":
             from ctypes import windll
             from ctypes import GetLastError, WinError
 
             path = os.path.abspath(path)
             # Make sure that the path uses backslashes here, in case
             # python would have happened to use forward slashes, as the
             # NT path format only supports backslashes.
-            path = path.replace('/', '\\')
-            NTPath = to_unicode(r'\\?\%s' % path)
+            path = path.replace("/", "\\")
+            NTPath = to_unicode(r"\\?\%s" % path)
             if not windll.kernel32.CreateDirectoryW(NTPath, None):
                 raise WinError(GetLastError())
         else:
             os.mkdir(path)
     except OSError:
         e = sys.exc_info()[1]
         # ignore EEXIST, which may occur during a race condition
@@ -191,45 +191,47 @@
     Yields:
         Filenames as returned by os.listdir (generally, str).
 
     """
     if exclude_filenames is None:
         exclude_filenames = set()
     if suffixes is None:
-        suffixes = {''}
+        suffixes = {""}
     for filename in os.listdir(dirname):
-        if (os.path.isdir(os.path.join(dirname, filename)) or
-            filename.startswith('.') or
-            filename in exclude_filenames or
-                not any(filename.endswith(sfx) for sfx in suffixes)):
+        if (
+            os.path.isdir(os.path.join(dirname, filename))
+            or filename.startswith(".")
+            or filename in exclude_filenames
+            or not any(filename.endswith(sfx) for sfx in suffixes)
+        ):
             continue
         yield filename
 
 
 def which(command, paths=None):
     """which(command, [paths]) - Look up the given command in the paths string
     (or the PATH environment variable, if unspecified)."""
 
     if paths is None:
-        paths = os.environ.get('PATH', '')
+        paths = os.environ.get("PATH", "")
 
     # Check for absolute match first.
     if os.path.isabs(command) and os.path.isfile(command):
         return os.path.normcase(os.path.normpath(command))
 
     # Would be nice if Python had a lib function for this.
     if not paths:
         paths = os.defpath
 
     # Get suffixes to search.
     # On Cygwin, 'PATHEXT' may exist but it should not be used.
-    if os.pathsep == ';':
-        pathext = os.environ.get('PATHEXT', '').split(';')
+    if os.pathsep == ";":
+        pathext = os.environ.get("PATHEXT", "").split(";")
     else:
-        pathext = ['']
+        pathext = [""]
 
     # Search the paths...
     for path in paths.split(os.pathsep):
         for ext in pathext:
             p = os.path.join(path, command + ext)
             if os.path.exists(p) and not os.path.isdir(p):
                 return os.path.normcase(os.path.abspath(p))
@@ -247,15 +249,15 @@
 def whichTools(tools, paths):
     for path in paths.split(os.pathsep):
         if checkToolsPath(path, tools):
             return path
     return None
 
 
-def printHistogram(items, title='Items'):
+def printHistogram(items, title="Items"):
     items.sort(key=lambda item: item[1])
 
     maxValue = max([v for _, v in items])
 
     # Select first "nice" bar height that produces more than 10 bars.
     power = int(math.ceil(math.log(maxValue, 10)))
     for inc in itertools.cycle((5, 2, 2.5, 1)):
@@ -268,36 +270,55 @@
 
     histo = [set() for i in range(N)]
     for name, v in items:
         bin = min(int(N * v / maxValue), N - 1)
         histo[bin].add(name)
 
     barW = 40
-    hr = '-' * (barW + 34)
-    print('Slowest %s:' % title)
+    hr = "-" * (barW + 34)
+    print("Slowest %s:" % title)
     print(hr)
     for name, value in reversed(items[-20:]):
-        print('%.2fs: %s' % (value, name))
-    print('\n%s Times:' % title)
+        print("%.2fs: %s" % (value, name))
+    print("\n%s Times:" % title)
     print(hr)
     pDigits = int(math.ceil(math.log(maxValue, 10)))
     pfDigits = max(0, 3 - pDigits)
     if pfDigits:
         pDigits += pfDigits + 1
     cDigits = int(math.ceil(math.log(len(items), 10)))
-    print('[%s] :: [%s] :: [%s]' % ('Range'.center((pDigits + 1) * 2 + 3),
-                                    'Percentage'.center(barW),
-                                    'Count'.center(cDigits * 2 + 1)))
+    print(
+        "[%s] :: [%s] :: [%s]"
+        % (
+            "Range".center((pDigits + 1) * 2 + 3),
+            "Percentage".center(barW),
+            "Count".center(cDigits * 2 + 1),
+        )
+    )
     print(hr)
     for i, row in reversed(list(enumerate(histo))):
         pct = float(len(row)) / len(items)
         w = int(barW * pct)
-        print('[%*.*fs,%*.*fs) :: [%s%s] :: [%*d/%*d]' % (
-            pDigits, pfDigits, i * barH, pDigits, pfDigits, (i + 1) * barH,
-            '*' * w, ' ' * (barW - w), cDigits, len(row), cDigits, len(items)))
+        print(
+            "[%*.*fs,%*.*fs) :: [%s%s] :: [%*d/%*d]"
+            % (
+                pDigits,
+                pfDigits,
+                i * barH,
+                pDigits,
+                pfDigits,
+                (i + 1) * barH,
+                "*" * w,
+                " " * (barW - w),
+                cDigits,
+                len(row),
+                cDigits,
+                len(items),
+            )
+        )
     print(hr)
 
 
 class ExecuteCommandTimeoutException(Exception):
     def __init__(self, msg, out, err, exitCode):
         assert isinstance(msg, str)
         assert isinstance(out, str)
@@ -307,19 +328,20 @@
         self.out = out
         self.err = err
         self.exitCode = exitCode
 
 
 # Close extra file handles on UNIX (on Windows this cannot be done while
 # also redirecting input).
-kUseCloseFDs = not (platform.system() == 'Windows')
+kUseCloseFDs = not (platform.system() == "Windows")
 
 
-def executeCommand(command, cwd=None, env=None, input=None, timeout=0,
-                   redirect_stderr=False):
+def executeCommand(
+    command, cwd=None, env=None, input=None, timeout=0, redirect_stderr=False
+):
     """Execute command ``command`` (list of arguments or string) with.
 
     * working directory ``cwd`` (str), use None to use the current
       working directory
     * environment ``env`` (dict), use None for none
     * Input to the command ``input`` (str), use string to pass
       no input.
@@ -334,27 +356,32 @@
     If the timeout is hit an ``ExecuteCommandTimeoutException``
     is raised.
 
     """
     if input is not None:
         input = to_bytes(input)
     err_out = subprocess.STDOUT if redirect_stderr else subprocess.PIPE
-    p = subprocess.Popen(command, cwd=cwd,
-                         stdin=subprocess.PIPE,
-                         stdout=subprocess.PIPE,
-                         stderr=err_out,
-                         env=env, close_fds=kUseCloseFDs)
+    p = subprocess.Popen(
+        command,
+        cwd=cwd,
+        stdin=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        stderr=err_out,
+        env=env,
+        close_fds=kUseCloseFDs,
+    )
     timerObject = None
     # FIXME: Because of the way nested function scopes work in Python 2.x we
     # need to use a reference to a mutable object rather than a plain
     # bool. In Python 3 we could use the "nonlocal" keyword but we need
     # to support Python 2 as well.
     hitTimeOut = [False]
     try:
         if timeout > 0:
+
             def killProcess():
                 # We may be invoking a shell so we need to kill the
                 # process and all its children.
                 hitTimeOut[0] = True
                 killProcessAndChildren(p.pid)
 
             timerObject = threading.Timer(timeout, killProcess)
@@ -364,103 +391,116 @@
         exitCode = p.wait()
     finally:
         if timerObject != None:
             timerObject.cancel()
 
     # Ensure the resulting output is always of string type.
     out = to_string(out)
-    err = '' if redirect_stderr else to_string(err)
+    err = "" if redirect_stderr else to_string(err)
 
     if hitTimeOut[0]:
         raise ExecuteCommandTimeoutException(
-            msg='Reached timeout of {} seconds'.format(timeout),
+            msg="Reached timeout of {} seconds".format(timeout),
             out=out,
             err=err,
-            exitCode=exitCode
+            exitCode=exitCode,
         )
 
     # Detect Ctrl-C in subprocess.
     if exitCode == -signal.SIGINT:
         raise KeyboardInterrupt
 
     return out, err, exitCode
 
 
 def isMacOSTriple(target_triple):
     """Whether the given target triple is for macOS,
-       e.g. x86_64-apple-darwin, arm64-apple-macos
+    e.g. x86_64-apple-darwin, arm64-apple-macos
     """
-    return 'darwin' in target_triple or 'macos' in target_triple
+    return "darwin" in target_triple or "macos" in target_triple
 
 
 def usePlatformSdkOnDarwin(config, lit_config):
     # On Darwin, support relocatable SDKs by providing Clang with a
     # default system root path.
     if isMacOSTriple(config.target_triple):
         try:
-            cmd = subprocess.Popen(['xcrun', '--show-sdk-path', '--sdk', 'macosx'],
-                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            cmd = subprocess.Popen(
+                ["xcrun", "--show-sdk-path", "--sdk", "macosx"],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
             out, err = cmd.communicate()
             out = out.strip()
             res = cmd.wait()
         except OSError:
             res = -1
         if res == 0 and out:
             sdk_path = out.decode()
-            lit_config.note('using SDKROOT: %r' % sdk_path)
-            config.environment['SDKROOT'] = sdk_path
+            lit_config.note("using SDKROOT: %r" % sdk_path)
+            config.environment["SDKROOT"] = sdk_path
 
 
 def findPlatformSdkVersionOnMacOS(config, lit_config):
     if isMacOSTriple(config.target_triple):
         try:
-            cmd = subprocess.Popen(['xcrun', '--show-sdk-version', '--sdk', 'macosx'],
-                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            cmd = subprocess.Popen(
+                ["xcrun", "--show-sdk-version", "--sdk", "macosx"],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
             out, err = cmd.communicate()
             out = out.strip()
             res = cmd.wait()
         except OSError:
             res = -1
         if res == 0 and out:
             return out.decode()
     return None
 
+
 def killProcessAndChildrenIsSupported():
     """
-        Returns a tuple (<supported> , <error message>)
-        where
-        `<supported>` is True if `killProcessAndChildren()` is supported on
-            the current host, returns False otherwise.
-        `<error message>` is an empty string if `<supported>` is True,
-            otherwise is contains a string describing why the function is
-            not supported.
+    Returns a tuple (<supported> , <error message>)
+    where
+    `<supported>` is True if `killProcessAndChildren()` is supported on
+        the current host, returns False otherwise.
+    `<error message>` is an empty string if `<supported>` is True,
+        otherwise is contains a string describing why the function is
+        not supported.
     """
-    if platform.system() == 'AIX':
+    if platform.system() == "AIX":
         return (True, "")
     try:
         import psutil  # noqa: F401
+
         return (True, "")
     except ImportError:
-        return (False,  "Requires the Python psutil module but it could"
-                        " not be found. Try installing it via pip or via"
-                        " your operating system's package manager.")
+        return (
+            False,
+            "Requires the Python psutil module but it could"
+            " not be found. Try installing it via pip or via"
+            " your operating system's package manager.",
+        )
+
 
 def killProcessAndChildren(pid):
     """This function kills a process with ``pid`` and all its running children
     (recursively). It is currently implemented using the psutil module on some
     platforms which provides a simple platform neutral implementation.
 
     TODO: Reimplement this without using psutil on all platforms so we can
     remove our dependency on it.
 
     """
-    if platform.system() == 'AIX':
-        subprocess.call('kill -kill $(ps -o pid= -L{})'.format(pid), shell=True)
+    if platform.system() == "AIX":
+        subprocess.call("kill -kill $(ps -o pid= -L{})".format(pid), shell=True)
     else:
         import psutil
+
         try:
             psutilProc = psutil.Process(pid)
             # Handle the different psutil API versions
             try:
                 # psutil >= 2.x
                 children_iterator = psutilProc.children(recursive=True)
             except AttributeError:
```

### Comparing `lit-16.0.6/lit/worker.py` & `lit-17.0.0rc1/lit/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 def _execute_test_handle_errors(test, lit_config):
     try:
         result = test.config.test_format.execute(test, lit_config)
         return _adapt_result(result)
     except:
         if lit_config.debug:
             raise
-        output = 'Exception during script execution:\n'
+        output = "Exception during script execution:\n"
         output += traceback.format_exc()
-        output += '\n'
+        output += "\n"
         return lit.Test.Result(lit.Test.UNRESOLVED, output)
 
 
 # Support deprecated result from execute() which returned the result
 # code and additional output as a tuple.
 def _adapt_result(result):
     if isinstance(result, lit.Test.Result):
```

### Comparing `lit-16.0.6/lit.egg-info/PKG-INFO` & `lit-17.0.0rc1/lit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lit
-Version: 16.0.6
+Version: 17.0.0rc1
 Summary: A Software Testing Tool
 Home-page: http://llvm.org
 Author: Daniel Dunbar
 Author-email: daniel@minormatter.com
 License: Apache-2.0 with LLVM exception
 Keywords: test C++ automatic discovery
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lit-16.0.6/lit.egg-info/SOURCES.txt` & `lit-17.0.0rc1/lit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,17 @@
 tests/Inputs/custom-result-category/lit.cfg
 tests/Inputs/custom-result-category/test1.txt
 tests/Inputs/custom-result-category/test2.txt
 tests/Inputs/discovery/lit.cfg
 tests/Inputs/discovery/test-one.txt
 tests/Inputs/discovery/test-two.txt
 tests/Inputs/discovery/test.not-txt
+tests/Inputs/discovery-getTestsForPath/custom_format.py
+tests/Inputs/discovery-getTestsForPath/lit.cfg
+tests/Inputs/discovery-getTestsForPath/x.test
 tests/Inputs/discovery/subdir/lit.local.cfg
 tests/Inputs/discovery/subdir/test-three.py
 tests/Inputs/discovery/subsuite/lit.cfg
 tests/Inputs/discovery/subsuite/test-one.txt
 tests/Inputs/discovery/subsuite/test-two.txt
 tests/Inputs/exec-discovery/lit.site.cfg
 tests/Inputs/exec-discovery-in-tree/lit.cfg
@@ -371,14 +374,15 @@
 tests/Inputs/shtest-shell/cat-error-1.txt
 tests/Inputs/shtest-shell/cat_nonprinting.bin
 tests/Inputs/shtest-shell/check_args.py
 tests/Inputs/shtest-shell/check_path.py
 tests/Inputs/shtest-shell/colon-error.txt
 tests/Inputs/shtest-shell/continuations.txt
 tests/Inputs/shtest-shell/dev-null.txt
+tests/Inputs/shtest-shell/diff-I.txt
 tests/Inputs/shtest-shell/diff-b.txt
 tests/Inputs/shtest-shell/diff-encodings.txt
 tests/Inputs/shtest-shell/diff-error-1.txt
 tests/Inputs/shtest-shell/diff-error-2.txt
 tests/Inputs/shtest-shell/diff-error-3.txt
 tests/Inputs/shtest-shell/diff-error-4.txt
 tests/Inputs/shtest-shell/diff-error-5.txt
```

### Comparing `lit-16.0.6/setup.py` & `lit-17.0.0rc1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,39 +12,35 @@
 
 import lit
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name = "lit",
-    version = lit.__version__,
-
-    author = lit.__author__,
-    author_email = lit.__email__,
-    url = 'http://llvm.org',
-    license = 'Apache-2.0 with LLVM exception',
-    license_files = ['LICENSE.TXT'],
-
-    description = "A Software Testing Tool",
-    keywords = 'test C++ automatic discovery',
-    long_description = long_description,
-
+    name="lit",
+    version=lit.__version__,
+    author=lit.__author__,
+    author_email=lit.__email__,
+    url="http://llvm.org",
+    license="Apache-2.0 with LLVM exception",
+    license_files=["LICENSE.TXT"],
+    description="A Software Testing Tool",
+    keywords="test C++ automatic discovery",
+    long_description=long_description,
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Topic :: Software Development :: Testing',
+        "Development Status :: 3 - Alpha",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Testing",
+    ],
+    zip_safe=False,
+    packages=find_packages(),
+    entry_points={
+        "console_scripts": [
+            "lit = lit.main:main",
         ],
-
-    zip_safe = False,
-    packages = find_packages(),
-    entry_points = {
-        'console_scripts': [
-            'lit = lit.main:main',
-            ],
-        }
+    },
 )
```

### Comparing `lit-16.0.6/tests/Inputs/allow-retries/succeeds-within-limit.py` & `lit-17.0.0rc1/tests/Inputs/allow-retries/succeeds-within-limit.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import sys
 import os
 
 counter_file = sys.argv[1]
 
 # The first time the test is run, initialize the counter to 1.
 if not os.path.exists(counter_file):
-    with open(counter_file, 'w') as counter:
+    with open(counter_file, "w") as counter:
         counter.write("1")
 
 # Succeed if this is the fourth time we're being run.
-with open(counter_file, 'r') as counter:
+with open(counter_file, "r") as counter:
     num = int(counter.read())
     if num == 4:
         sys.exit(0)
 
 # Otherwise, increment the counter and fail
-with open(counter_file, 'w') as counter:
+with open(counter_file, "w") as counter:
     counter.write(str(num + 1))
     sys.exit(1)
```

### Comparing `lit-16.0.6/tests/Inputs/discovery/lit.cfg` & `lit-17.0.0rc1/tests/Inputs/discovery/lit.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import lit.formats
-config.name = 'top-level-suite'
-config.suffixes = ['.txt']
+
+config.name = "top-level-suite"
+config.suffixes = [".txt"]
 config.test_format = lit.formats.ShTest()
 
 # We intentionally don't set the source root or exec root directories here,
 # because this suite gets reused for testing the exec root behavior (in
 # ../exec-discovery).
 #
-#config.test_source_root = None
-#config.test_exec_root = None
+# config.test_source_root = None
+# config.test_exec_root = None
 
 # Check that arbitrary config values are copied (tested by subdir/lit.local.cfg).
 config.an_extra_variable = False
 
 # Check that available_features are printed by --show-suites (and in the right order)
-config.available_features = ['feature2', 'feature1']
+config.available_features = ["feature2", "feature1"]
 
 # Check that substitutions are printed by --show-suites (and in the right order)
-config.substitutions = [('%key2', 'value2'), ('%key1', 'value1')]
+config.substitutions = [("%key2", "value2"), ("%key1", "value1")]
```

### Comparing `lit-16.0.6/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe` & `lit-17.0.0rc1/tests/Inputs/googletest-cmd-wrapper/DummySubDir/OneTest.exe`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/googletest-crash/DummySubDir/OneTest.py` & `lit-17.0.0rc1/tests/Inputs/googletest-crash/DummySubDir/OneTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 if len(sys.argv) == 3 and sys.argv[1] == "--gtest_list_tests":
-    if sys.argv[2] != '--gtest_filter=-*DISABLED_*':
+    if sys.argv[2] != "--gtest_filter=-*DISABLED_*":
         raise ValueError("unexpected argument: %s" % (sys.argv[2]))
-    print("""\
+    print(
+        """\
 FirstTest.
   subTestA
   subTestB
   subTestC
   subTestD
 ParameterizedTest/0.
   subTest
 ParameterizedTest/1.
-  subTest""")
+  subTest"""
+    )
     sys.exit(0)
 elif len(sys.argv) != 1:
     # sharding and json output are specified using environment variables
-    raise ValueError("unexpected argument: %r" % (' '.join(sys.argv[1:])))
+    raise ValueError("unexpected argument: %r" % (" ".join(sys.argv[1:])))
 
-for e in ['GTEST_TOTAL_SHARDS', 'GTEST_SHARD_INDEX', 'GTEST_OUTPUT']:
+for e in ["GTEST_TOTAL_SHARDS", "GTEST_SHARD_INDEX", "GTEST_OUTPUT"]:
     if e not in os.environ:
         raise ValueError("missing environment variables: " + e)
 
-if not os.environ['GTEST_OUTPUT'].startswith('json:'):
-    raise ValueError("must emit json output: " + os.environ['GTEST_OUTPUT'])
+if not os.environ["GTEST_OUTPUT"].startswith("json:"):
+    raise ValueError("must emit json output: " + os.environ["GTEST_OUTPUT"])
 
 dummy_output = """\
 {
 "testsuites": [
 ]
 }"""
 
-if os.environ['GTEST_SHARD_INDEX'] == '0':
-    print("""\
+if os.environ["GTEST_SHARD_INDEX"] == "0":
+    print(
+        """\
 [----------] 4 test from FirstTest
 [ RUN      ] FirstTest.subTestA
 [       OK ] FirstTest.subTestA (18 ms)
-[ RUN      ] FirstTest.subTestB""", flush=True)
-    print('I am about to crash', file=sys.stderr, flush=True)
+[ RUN      ] FirstTest.subTestB""",
+        flush=True,
+    )
+    print("I am about to crash", file=sys.stderr, flush=True)
     exit_code = 1
 else:
-    json_filename = os.environ['GTEST_OUTPUT'].split(':', 1)[1]
-    with open(json_filename, 'w', encoding='utf-8') as f:
+    json_filename = os.environ["GTEST_OUTPUT"].split(":", 1)[1]
+    with open(json_filename, "w", encoding="utf-8") as f:
         f.write(dummy_output)
     exit_code = 0
 
 sys.exit(exit_code)
```

### Comparing `lit-16.0.6/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py` & `lit-17.0.0rc1/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 if len(sys.argv) == 3 and sys.argv[1] == "--gtest_list_tests":
-    if sys.argv[2] != '--gtest_filter=-*DISABLED_*':
+    if sys.argv[2] != "--gtest_filter=-*DISABLED_*":
         raise ValueError("unexpected argument: %s" % (sys.argv[2]))
-    print("""\
-FirstTest.
-  subTestA""")
+    print(
+        """\
+T.
+  QuickSubTest
+  InfiniteLoopSubTest
+"""
+    )
     sys.exit(0)
 elif len(sys.argv) != 1:
     # sharding and json output are specified using environment variables
-    raise ValueError("unexpected argument: %r" % (' '.join(sys.argv[1:])))
+    raise ValueError("unexpected argument: %r" % (" ".join(sys.argv[1:])))
 
-for e in ['GTEST_TOTAL_SHARDS', 'GTEST_SHARD_INDEX', 'GTEST_OUTPUT']:
+for e in ["GTEST_TOTAL_SHARDS", "GTEST_SHARD_INDEX", "GTEST_OUTPUT", "GTEST_FILTER"]:
     if e not in os.environ:
         raise ValueError("missing environment variables: " + e)
 
-if not os.environ['GTEST_OUTPUT'].startswith('json:'):
-    raise ValueError("must emit json output: " + os.environ['GTEST_OUTPUT'])
+if not os.environ["GTEST_OUTPUT"].startswith("json:"):
+    raise ValueError("must emit json output: " + os.environ["GTEST_OUTPUT"])
 
 output = """\
 {
-"random_seed": 123,
 "testsuites": [
     {
-        "name": "FirstTest",
+        "name": "T",
         "testsuite": [
             {
-                "name": "subTestA",
+                "name": "QuickSubTest",
                 "result": "COMPLETED",
-                "time": "0.001s"
+                "time": "2s"
             }
         ]
     }
 ]
 }"""
 
 dummy_output = """\
 {
 "testsuites": [
 ]
 }"""
 
-json_filename = os.environ['GTEST_OUTPUT'].split(':', 1)[1]
-with open(json_filename, 'w', encoding='utf-8') as f:
-    if os.environ['GTEST_SHARD_INDEX'] == '0':
-        f.write(output)
+json_filename = os.environ["GTEST_OUTPUT"].split(":", 1)[1]
+
+if os.environ["GTEST_SHARD_INDEX"] == "0":
+    test_name = os.environ["GTEST_FILTER"]
+    if test_name == "QuickSubTest":
+        with open(json_filename, "w", encoding="utf-8") as f:
+            f.write(output)
+        exit_code = 0
+    elif test_name == "InfiniteLoopSubTest":
+        while True:
+            pass
     else:
+        raise SystemExit("error: invalid test name: %r" % (test_name,))
+else:
+    with open(json_filename, "w", encoding="utf-8") as f:
         f.write(dummy_output)
     exit_code = 0
 
 sys.exit(exit_code)
```

### Comparing `lit-16.0.6/tests/Inputs/googletest-format/DummySubDir/OneTest.py` & `lit-17.0.0rc1/tests/Inputs/googletest-format/DummySubDir/OneTest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 if len(sys.argv) == 3 and sys.argv[1] == "--gtest_list_tests":
-    if sys.argv[2] != '--gtest_filter=-*DISABLED_*':
+    if sys.argv[2] != "--gtest_filter=-*DISABLED_*":
         raise ValueError("unexpected argument: %s" % (sys.argv[2]))
-    print("""\
+    print(
+        """\
 FirstTest.
   subTestA
   subTestB
   subTestC
   subTestD
 ParameterizedTest/0.
   subTest
 ParameterizedTest/1.
-  subTest""")
+  subTest"""
+    )
     sys.exit(0)
 elif len(sys.argv) != 1:
     # sharding and json output are specified using environment variables
-    raise ValueError("unexpected argument: %r" % (' '.join(sys.argv[1:])))
+    raise ValueError("unexpected argument: %r" % (" ".join(sys.argv[1:])))
 
-for e in ['GTEST_TOTAL_SHARDS', 'GTEST_SHARD_INDEX', 'GTEST_OUTPUT']:
+for e in ["GTEST_TOTAL_SHARDS", "GTEST_SHARD_INDEX", "GTEST_OUTPUT"]:
     if e not in os.environ:
         raise ValueError("missing environment variables: " + e)
 
-if not os.environ['GTEST_OUTPUT'].startswith('json:'):
-    raise ValueError("must emit json output: " + os.environ['GTEST_OUTPUT'])
+if not os.environ["GTEST_OUTPUT"].startswith("json:"):
+    raise ValueError("must emit json output: " + os.environ["GTEST_OUTPUT"])
 
 output = """\
 {
 "random_seed": 123,
 "testsuites": [
     {
         "name": "FirstTest",
@@ -88,20 +90,20 @@
 
 dummy_output = """\
 {
 "testsuites": [
 ]
 }"""
 
-json_filename = os.environ['GTEST_OUTPUT'].split(':', 1)[1]
-with open(json_filename, 'w', encoding='utf-8') as f:
-    if os.environ['GTEST_SHARD_INDEX'] == '0':
-        print('[ RUN      ] FirstTest.subTestB', flush=True)
-        print('I am subTest B output', file=sys.stderr, flush=True)
-        print('[  FAILED  ] FirstTest.subTestB (8 ms)', flush=True)
+json_filename = os.environ["GTEST_OUTPUT"].split(":", 1)[1]
+with open(json_filename, "w", encoding="utf-8") as f:
+    if os.environ["GTEST_SHARD_INDEX"] == "0":
+        print("[ RUN      ] FirstTest.subTestB", flush=True)
+        print("I am subTest B output", file=sys.stderr, flush=True)
+        print("[  FAILED  ] FirstTest.subTestB (8 ms)", flush=True)
 
         f.write(output)
         exit_code = 1
     else:
         f.write(dummy_output)
         exit_code = 0
```

### Comparing `lit-16.0.6/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py` & `lit-17.0.0rc1/tests/Inputs/googletest-format-respect-gtest-sharding-env-vars/DummySubDir/OneTest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 if len(sys.argv) == 3 and sys.argv[1] == "--gtest_list_tests":
-    if sys.argv[2] != '--gtest_filter=-*DISABLED_*':
+    if sys.argv[2] != "--gtest_filter=-*DISABLED_*":
         raise ValueError("unexpected argument: %s" % (sys.argv[2]))
-    print("""\
+    print(
+        """\
 FirstTest.
   subTestA
   subTestB
   subTestC
   subTestD
 ParameterizedTest/0.
   subTest
 ParameterizedTest/1.
-  subTest""")
+  subTest"""
+    )
     sys.exit(0)
 elif len(sys.argv) != 1:
     # sharding and json output are specified using environment variables
-    raise ValueError("unexpected argument: %r" % (' '.join(sys.argv[1:])))
+    raise ValueError("unexpected argument: %r" % (" ".join(sys.argv[1:])))
 
-for e in ['GTEST_TOTAL_SHARDS', 'GTEST_SHARD_INDEX', 'GTEST_OUTPUT']:
+for e in ["GTEST_TOTAL_SHARDS", "GTEST_SHARD_INDEX", "GTEST_OUTPUT"]:
     if e not in os.environ:
         raise ValueError("missing environment variables: " + e)
 
-if not os.environ['GTEST_OUTPUT'].startswith('json:'):
-    raise ValueError("must emit json output: " + os.environ['GTEST_OUTPUT'])
+if not os.environ["GTEST_OUTPUT"].startswith("json:"):
+    raise ValueError("must emit json output: " + os.environ["GTEST_OUTPUT"])
 
 output = """\
 {
 "random_seed": 123,
 "testsuites": [
     {
         "name": "FirstTest",
@@ -88,20 +90,20 @@
 
 dummy_output = """\
 {
 "testsuites": [
 ]
 }"""
 
-json_filename = os.environ['GTEST_OUTPUT'].split(':', 1)[1]
-with open(json_filename, 'w', encoding='utf-8') as f:
-    if os.environ['GTEST_TOTAL_SHARDS'] == '1':
-        print('[ RUN      ] FirstTest.subTestB', flush=True)
-        print('I am subTest B output', file=sys.stderr, flush=True)
-        print('[  FAILED  ] FirstTest.subTestB (8 ms)', flush=True)
+json_filename = os.environ["GTEST_OUTPUT"].split(":", 1)[1]
+with open(json_filename, "w", encoding="utf-8") as f:
+    if os.environ["GTEST_TOTAL_SHARDS"] == "1":
+        print("[ RUN      ] FirstTest.subTestB", flush=True)
+        print("I am subTest B output", file=sys.stderr, flush=True)
+        print("[  FAILED  ] FirstTest.subTestB (8 ms)", flush=True)
 
         f.write(output)
         exit_code = 1
     else:
         f.write(dummy_output)
         exit_code = 0
```

### Comparing `lit-16.0.6/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py` & `lit-17.0.0rc1/tests/Inputs/googletest-sanitizer-error/DummySubDir/OneTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 if len(sys.argv) == 3 and sys.argv[1] == "--gtest_list_tests":
-    if sys.argv[2] != '--gtest_filter=-*DISABLED_*':
+    if sys.argv[2] != "--gtest_filter=-*DISABLED_*":
         raise ValueError("unexpected argument: %s" % (sys.argv[2]))
-    print("""\
+    print(
+        """\
 FirstTest.
-  subTestA""")
+  subTestA"""
+    )
     sys.exit(0)
 elif len(sys.argv) != 1:
     # sharding and json output are specified using environment variables
-    raise ValueError("unexpected argument: %r" % (' '.join(sys.argv[1:])))
+    raise ValueError("unexpected argument: %r" % (" ".join(sys.argv[1:])))
 
-for e in ['GTEST_TOTAL_SHARDS', 'GTEST_SHARD_INDEX', 'GTEST_OUTPUT']:
+for e in ["GTEST_TOTAL_SHARDS", "GTEST_SHARD_INDEX", "GTEST_OUTPUT"]:
     if e not in os.environ:
         raise ValueError("missing environment variables: " + e)
 
-if not os.environ['GTEST_OUTPUT'].startswith('json:'):
-    raise ValueError("must emit json output: " + os.environ['GTEST_OUTPUT'])
+if not os.environ["GTEST_OUTPUT"].startswith("json:"):
+    raise ValueError("must emit json output: " + os.environ["GTEST_OUTPUT"])
 
 output = """\
 {
 "random_seed": 123,
 "testsuites": [
     {
         "name": "FirstTest",
@@ -40,19 +42,19 @@
 
 dummy_output = """\
 {
 "testsuites": [
 ]
 }"""
 
-json_filename = os.environ['GTEST_OUTPUT'].split(':', 1)[1]
-with open(json_filename, 'w', encoding='utf-8') as f:
-    if os.environ['GTEST_SHARD_INDEX'] == '0':
-        print('[ RUN      ] FirstTest.subTestA', flush=True)
-        print('[       OK ] FirstTest.subTestA (8 ms)', flush=True)
+json_filename = os.environ["GTEST_OUTPUT"].split(":", 1)[1]
+with open(json_filename, "w", encoding="utf-8") as f:
+    if os.environ["GTEST_SHARD_INDEX"] == "0":
+        print("[ RUN      ] FirstTest.subTestA", flush=True)
+        print("[       OK ] FirstTest.subTestA (8 ms)", flush=True)
 
         f.write(output)
         exit_code = 1
     else:
         f.write(dummy_output)
         exit_code = 0
```

### Comparing `lit-16.0.6/tests/Inputs/googletest-timeout/DummySubDir/OneTest.py` & `lit-17.0.0rc1/tests/Inputs/googletest-detect-duplicate/DummySubDir/OneTest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 #!/usr/bin/env python
 
 import os
 import sys
 
 if len(sys.argv) == 3 and sys.argv[1] == "--gtest_list_tests":
-    if sys.argv[2] != '--gtest_filter=-*DISABLED_*':
+    if sys.argv[2] != "--gtest_filter=-*DISABLED_*":
         raise ValueError("unexpected argument: %s" % (sys.argv[2]))
-    print("""\
-T.
-  QuickSubTest
-  InfiniteLoopSubTest
-""")
+    print(
+        """\
+FirstTest.
+  subTestA"""
+    )
     sys.exit(0)
 elif len(sys.argv) != 1:
     # sharding and json output are specified using environment variables
-    raise ValueError("unexpected argument: %r" % (' '.join(sys.argv[1:])))
+    raise ValueError("unexpected argument: %r" % (" ".join(sys.argv[1:])))
 
-for e in ['GTEST_TOTAL_SHARDS', 'GTEST_SHARD_INDEX', 'GTEST_OUTPUT', 'GTEST_FILTER']:
+for e in ["GTEST_TOTAL_SHARDS", "GTEST_SHARD_INDEX", "GTEST_OUTPUT"]:
     if e not in os.environ:
         raise ValueError("missing environment variables: " + e)
 
-if not os.environ['GTEST_OUTPUT'].startswith('json:'):
-    raise ValueError("must emit json output: " + os.environ['GTEST_OUTPUT'])
+if not os.environ["GTEST_OUTPUT"].startswith("json:"):
+    raise ValueError("must emit json output: " + os.environ["GTEST_OUTPUT"])
 
 output = """\
 {
+"random_seed": 123,
 "testsuites": [
     {
-        "name": "T",
+        "name": "FirstTest",
         "testsuite": [
             {
-                "name": "QuickSubTest",
+                "name": "subTestA",
                 "result": "COMPLETED",
-                "time": "2s"
+                "time": "0.001s"
             }
         ]
     }
 ]
 }"""
 
 dummy_output = """\
 {
 "testsuites": [
 ]
 }"""
 
-json_filename = os.environ['GTEST_OUTPUT'].split(':', 1)[1]
-
-if os.environ['GTEST_SHARD_INDEX'] == '0':
-    test_name = os.environ['GTEST_FILTER']
-    if test_name == 'QuickSubTest':
-        with open(json_filename, 'w', encoding='utf-8') as f:
-            f.write(output)
-        exit_code = 0
-    elif test_name == 'InfiniteLoopSubTest':
-        while True:
-            pass
+json_filename = os.environ["GTEST_OUTPUT"].split(":", 1)[1]
+with open(json_filename, "w", encoding="utf-8") as f:
+    if os.environ["GTEST_SHARD_INDEX"] == "0":
+        f.write(output)
     else:
-        raise SystemExit("error: invalid test name: %r" % (test_name,))
-else:
-    with open(json_filename, 'w', encoding='utf-8') as f:
         f.write(dummy_output)
     exit_code = 0
 
 sys.exit(exit_code)
```

### Comparing `lit-16.0.6/tests/Inputs/lld-features/lit.cfg` & `lit-17.0.0rc1/tests/Inputs/lld-features/lit.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import lit.formats
-config.name = 'search-env'
-config.suffixes = ['.txt']
+
+config.name = "search-env"
+config.suffixes = [".txt"]
 config.test_format = lit.formats.ShTest()
 config.test_source_root = None
 config.test_exec_root = None
-config.llvm_tools_dir = ''
+config.llvm_tools_dir = ""
 import lit.llvm
+
 lit.llvm.initialize(lit_config, config)
 import os.path
+
 curdir = os.path.dirname(__file__)
 # The current directory contains files for each version of LLD, both with and
 # without a .exe extension. The .exe versions will be found on Windows and the
 # ones without will be found on Linux. Note that all files are just empty files,
 # since the test doesn't actually use them.
-lit.llvm.llvm_config.with_environment('PATH', curdir, append_path=True)
+lit.llvm.llvm_config.with_environment("PATH", curdir, append_path=True)
 lit.llvm.llvm_config.use_lld(use_installed=True)
```

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-exact.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/errors/defined-check/redefine-multiple-once-exact.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/examples/param-subst.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/examples/param-subst.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/expansion-order.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/expansion-order.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/line-number-substitutions.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/line-number-substitutions.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/lit.cfg` & `lit-17.0.0rc1/tests/Inputs/shtest-define/lit.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import lit.formats
-config.name = 'shtest-define'
-config.suffixes = ['.txt']
+
+config.name = "shtest-define"
+config.suffixes = [".txt"]
 # Use lit's internal shell to avoid shell portability issues within RUN lines
 # (e.g., for 'echo' commands in Windows).  Those issues should be orthogonal to
 # the substitution behavior we are trying to test.
 config.test_format = lit.formats.ShTest(execute_external=False)
 config.test_source_root = None
 config.test_exec_root = None
 
@@ -12,39 +13,40 @@
 # prepend substitutions before substitutions they might now or later (upon a
 # redefinition) depend upon.  For example, %{global:greeting} and %{global:what}
 # act as parameters for %{global:echo}, so we make sure the latter expands
 # before the former.  Moreover, some tests redefine %{global:greeting} in terms
 # of %{global:what}, so we make sure the former expands before the latter.
 # If we always insert at the beginning of the substitution list (as DEFINE
 # does), then the rule is simple: define a substitution before you refer to it.
-config.substitutions.insert(0, ('%{global:what}', 'World'))
-config.substitutions.insert(0, ('%{global:greeting}', ''))
-config.substitutions.insert(0,
-    ('%{global:echo}', "echo GLOBAL: %{global:greeting} %{global:what}"))
+config.substitutions.insert(0, ("%{global:what}", "World"))
+config.substitutions.insert(0, ("%{global:greeting}", ""))
+config.substitutions.insert(
+    0, ("%{global:echo}", "echo GLOBAL: %{global:greeting} %{global:what}")
+)
 
 # The following substitution definitions are confusing and should be avoided.
 # We define them here so we can test that 'DEFINE:' and 'REDEFINE:' directives
 # guard against the confusion they cause.
 
 # Even though each of '%{global:inside}', '%{global:prefix}', and
 # '%{global:suffix}' is not already the exact pattern of a substitution,
 # 'DEFINE:' and 'REDEFINE:' will refuse to (re)define a substitution with that
 # pattern because it is a substring of one of the following substitution's
 # patterns.
-config.substitutions.insert(0, ('<%{global:inside}>', '<@>'))
-config.substitutions.insert(0, (r'%{global:prefix}\((.*)\)', r'@(\g<1>)'))
-config.substitutions.insert(0, ('@%{global:suffix}', '@@'))
+config.substitutions.insert(0, ("<%{global:inside}>", "<@>"))
+config.substitutions.insert(0, (r"%{global:prefix}\((.*)\)", r"@(\g<1>)"))
+config.substitutions.insert(0, ("@%{global:suffix}", "@@"))
 
 # These cannot be redefined by 'REDEFINE:', which doesn't know which one to
 # redefine.
-config.substitutions.insert(0, ('%{global:multiple-exact}', 'first'))
-config.substitutions.insert(0, ('%{global:multiple-exact}', 'second'))
+config.substitutions.insert(0, ("%{global:multiple-exact}", "first"))
+config.substitutions.insert(0, ("%{global:multiple-exact}", "second"))
 
 # Even though '%{global:multiple-once-exact}' is the exact pattern of only one
 # existing substitution, 'REDEFINE:' will refuse to redefine that substitution
 # because that string is a substring of another substitution's pattern.
-config.substitutions.insert(0, ('%{global:multiple-once-exact}', '@'))
-config.substitutions.insert(0, ('<%{global:multiple-once-exact}>', '<@>'))
+config.substitutions.insert(0, ("%{global:multiple-once-exact}", "@"))
+config.substitutions.insert(0, ("<%{global:multiple-once-exact}>", "<@>"))
 
-recur = lit_config.params.get('recur', None)
+recur = lit_config.params.get("recur", None)
 if recur:
-  config.recursiveExpansionLimit = int(recur)
+    config.recursiveExpansionLimit = int(recur)
```

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/name-chars.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/name-chars.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/shared-substs-0.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-0.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/shared-substs-1.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/shared-substs-1.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/value-equals.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/value-equals.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-define/ws-and-continuations.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-define/ws-and-continuations.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-env/env-calls-env.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-env/env-calls-env.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-env/env-u.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-env/env-u.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-env/mixed.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-env/mixed.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-if-else/test.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-if-else/test.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-not/not-calls-external.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-not/not-calls-external.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/check_path.py` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/check_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,21 @@
         print("Wrong number of args")
         return 1
 
     type = argv[1]
     paths = argv[2:]
     exit_code = 0
 
-    if type == 'dir':
+    if type == "dir":
         for idx, dir in enumerate(paths):
             print(os.path.isdir(dir))
-    elif type == 'file':
+    elif type == "file":
         for idx, file in enumerate(paths):
             print(os.path.isfile(file))
     else:
         print("Unrecognised type {}".format(type))
         exit_code = 1
     return exit_code
 
-if __name__ == '__main__':
-    sys.exit (check_path (sys.argv))
+
+if __name__ == "__main__":
+    sys.exit(check_path(sys.argv))
```

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/dev-null.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/dev-null.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/diff-encodings.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-encodings.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/diff-pipes.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-pipes.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/diff-r.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-r.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/diff-unified.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/diff-unified.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/redirects.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/redirects.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/sequencing-0.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/sequencing-0.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-shell/valid-shell.txt` & `lit-17.0.0rc1/tests/Inputs/shtest-shell/valid-shell.txt`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/Inputs/shtest-timeout/lit.cfg` & `lit-17.0.0rc1/tests/Inputs/shtest-timeout/lit.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # -*- Python -*-
 import os
 import sys
 
 import lit.formats
 
-config.name = 'per_test_timeout'
+config.name = "per_test_timeout"
 
-shellType = lit_config.params.get('external', '1')
+shellType = lit_config.params.get("external", "1")
 
-if shellType == '0':
-    lit_config.note('Using internal shell')
+if shellType == "0":
+    lit_config.note("Using internal shell")
     externalShell = False
 else:
-    lit_config.note('Using external shell')
+    lit_config.note("Using external shell")
     externalShell = True
 
-configSetTimeout = lit_config.params.get('set_timeout', '0')
+configSetTimeout = lit_config.params.get("set_timeout", "0")
 
-if configSetTimeout != '0':
+if configSetTimeout != "0":
     # Try setting the max individual test time in the configuration
     lit_config.maxIndividualTestTime = int(configSetTimeout)
 
 config.test_format = lit.formats.ShTest(execute_external=externalShell)
-config.suffixes = ['.py']
+config.suffixes = [".py"]
 
 config.test_source_root = os.path.dirname(__file__)
 config.test_exec_root = config.test_source_root
-config.target_triple = '(unused)'
-src_root = os.path.join(config.test_source_root, '..')
+config.target_triple = "(unused)"
+src_root = os.path.join(config.test_source_root, "..")
 
 pythonpath_list = [src_root]
 # Ensure the user's PYTHONPATH is included.
-if 'PYTHONPATH' in os.environ:
-    pythonpath_list.append(os.environ['PYTHONPATH'])
-if 'PYTHONPATH' in config.environment:
-    pythonpath_list.append(config.environment['PYTHONPATH'])
-config.environment['PYTHONPATH'] = os.pathsep.join(pythonpath_list)
+if "PYTHONPATH" in os.environ:
+    pythonpath_list.append(os.environ["PYTHONPATH"])
+if "PYTHONPATH" in config.environment:
+    pythonpath_list.append(config.environment["PYTHONPATH"])
+config.environment["PYTHONPATH"] = os.pathsep.join(pythonpath_list)
 
-config.substitutions.append(('%{python}', '"%s"' % (sys.executable)))
+config.substitutions.append(("%{python}", '"%s"' % (sys.executable)))
```

### Comparing `lit-16.0.6/tests/Inputs/test-data/dummy_format.py` & `lit-17.0.0rc1/tests/Inputs/test-data/dummy_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
+
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 import lit.formats
 import lit.Test
 
+
 class DummyFormat(lit.formats.FileBasedTest):
     def execute(self, test, lit_config):
         # In this dummy format, expect that each test file is actually just a
         # .ini format dump of the results to report.
 
         source_path = test.getSourcePath()
 
         cfg = ConfigParser.ConfigParser()
         cfg.read(source_path)
 
         # Create the basic test result.
-        result_code = cfg.get('global', 'result_code')
-        result_output = cfg.get('global', 'result_output')
-        result = lit.Test.Result(getattr(lit.Test, result_code),
-                                 result_output)
+        result_code = cfg.get("global", "result_code")
+        result_output = cfg.get("global", "result_output")
+        result = lit.Test.Result(getattr(lit.Test, result_code), result_output)
 
         # Load additional metrics.
-        for key,value_str in cfg.items('results'):
+        for key, value_str in cfg.items("results"):
             value = eval(value_str)
             if isinstance(value, int):
                 metric = lit.Test.IntMetricValue(value)
             elif isinstance(value, float):
                 metric = lit.Test.RealMetricValue(value)
             else:
                 raise RuntimeError("unsupported result type")
             result.addMetric(key, metric)
 
         return result
-
```

### Comparing `lit-16.0.6/tests/Inputs/test-data-micro/dummy_format.py` & `lit-17.0.0rc1/tests/Inputs/test-data-micro/dummy_format.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import os
+
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 import lit.formats
 import lit.Test
 
+
 class DummyFormat(lit.formats.FileBasedTest):
     def execute(self, test, lit_config):
         # In this dummy format, expect that each test file is actually just a
         # .ini format dump of the results to report.
 
         source_path = test.getSourcePath()
 
         cfg = ConfigParser.ConfigParser()
         cfg.read(source_path)
 
         # Create the basic test result.
-        result_code = cfg.get('global', 'result_code')
-        result_output = cfg.get('global', 'result_output')
-        result = lit.Test.Result(getattr(lit.Test, result_code),
-                                 result_output)
+        result_code = cfg.get("global", "result_code")
+        result_output = cfg.get("global", "result_output")
+        result = lit.Test.Result(getattr(lit.Test, result_code), result_output)
 
         # Load additional metrics.
-        for key,value_str in cfg.items('results'):
+        for key, value_str in cfg.items("results"):
             value = eval(value_str)
             if isinstance(value, int):
                 metric = lit.Test.IntMetricValue(value)
             elif isinstance(value, float):
                 metric = lit.Test.RealMetricValue(value)
             else:
                 raise RuntimeError("unsupported result type")
             result.addMetric(key, metric)
 
         # Create micro test results
-        for key,micro_name in cfg.items('micro-tests'):
-            micro_result = lit.Test.Result(getattr(lit.Test, result_code, ''))
+        for key, micro_name in cfg.items("micro-tests"):
+            micro_result = lit.Test.Result(getattr(lit.Test, result_code, ""))
             # Load micro test additional metrics
-            for key,value_str in cfg.items('micro-results'):
+            for key, value_str in cfg.items("micro-results"):
                 value = eval(value_str)
                 if isinstance(value, int):
                     metric = lit.Test.IntMetricValue(value)
                 elif isinstance(value, float):
                     metric = lit.Test.RealMetricValue(value)
                 else:
                     raise RuntimeError("unsupported result type")
```

### Comparing `lit-16.0.6/tests/Inputs/test_retry_attempts/test.py` & `lit-17.0.0rc1/tests/Inputs/test_retry_attempts/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import sys
 import os
 
 counter_file = sys.argv[1]
 
 # The first time the test is run, initialize the counter to 1.
 if not os.path.exists(counter_file):
-    with open(counter_file, 'w') as counter:
+    with open(counter_file, "w") as counter:
         counter.write("1")
 
 # Succeed if this is the fourth time we're being run.
-with open(counter_file, 'r') as counter:
+with open(counter_file, "r") as counter:
     num = int(counter.read())
     if num == 4:
         sys.exit(0)
 
 # Otherwise, increment the counter and fail
-with open(counter_file, 'w') as counter:
+with open(counter_file, "w") as counter:
     counter.write(str(num + 1))
     sys.exit(1)
```

### Comparing `lit-16.0.6/tests/Inputs/use-llvm-tool/lit.cfg` & `lit-17.0.0rc1/tests/Inputs/use-llvm-tool/lit.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import lit.formats
-config.name = 'use-llvm-tool'
-config.suffixes = ['.txt']
+
+config.name = "use-llvm-tool"
+config.suffixes = [".txt"]
 config.test_format = lit.formats.ShTest()
 config.test_source_root = None
 config.test_exec_root = None
 import os.path
+
 this_dir = os.path.realpath(os.path.dirname(__file__))
-config.llvm_tools_dir = os.path.join(this_dir, 'build')
+config.llvm_tools_dir = os.path.join(this_dir, "build")
 import lit.llvm
+
 lit.llvm.initialize(lit_config, config)
-lit.llvm.llvm_config.with_environment('CASE1', os.path.join(this_dir, 'env-case1'))
-lit.llvm.llvm_config.with_environment('CASE6', os.path.join(this_dir, 'env-case6'))
-lit.llvm.llvm_config.with_environment('PATH', os.path.join(this_dir, 'path'), append_path=True)
-lit.llvm.llvm_config.use_llvm_tool('case1', search_env='CASE1')
-lit.llvm.llvm_config.use_llvm_tool('case2', search_env='CASE2')
-lit.llvm.llvm_config.use_llvm_tool('case3')
-lit.llvm.llvm_config.use_llvm_tool('case4', use_installed=True)
-lit.llvm.llvm_config.use_llvm_tool('case5')
-lit.llvm.llvm_config.use_llvm_tool('case6', search_env='CASE6', use_installed=True)
-lit.llvm.llvm_config.use_llvm_tool('case7', use_installed=True)
-lit.llvm.llvm_config.use_llvm_tool('case8', use_installed=True)
-paths = [os.path.join(this_dir, 'search1'), os.path.join(this_dir, 'search2'), os.path.join(this_dir, 'search3')]
-lit.llvm.llvm_config.use_llvm_tool('case9', search_paths=paths)
-lit.llvm.llvm_config.use_llvm_tool('case10', search_paths=paths, use_installed=True)
+lit.llvm.llvm_config.with_environment("CASE1", os.path.join(this_dir, "env-case1"))
+lit.llvm.llvm_config.with_environment("CASE6", os.path.join(this_dir, "env-case6"))
+lit.llvm.llvm_config.with_environment(
+    "PATH", os.path.join(this_dir, "path"), append_path=True
+)
+lit.llvm.llvm_config.use_llvm_tool("case1", search_env="CASE1")
+lit.llvm.llvm_config.use_llvm_tool("case2", search_env="CASE2")
+lit.llvm.llvm_config.use_llvm_tool("case3")
+lit.llvm.llvm_config.use_llvm_tool("case4", use_installed=True)
+lit.llvm.llvm_config.use_llvm_tool("case5")
+lit.llvm.llvm_config.use_llvm_tool("case6", search_env="CASE6", use_installed=True)
+lit.llvm.llvm_config.use_llvm_tool("case7", use_installed=True)
+lit.llvm.llvm_config.use_llvm_tool("case8", use_installed=True)
+paths = [
+    os.path.join(this_dir, "search1"),
+    os.path.join(this_dir, "search2"),
+    os.path.join(this_dir, "search3"),
+]
+lit.llvm.llvm_config.use_llvm_tool("case9", search_paths=paths)
+lit.llvm.llvm_config.use_llvm_tool("case10", search_paths=paths, use_installed=True)
```

### Comparing `lit-16.0.6/tests/Inputs/xunit-output/dummy_format.py` & `lit-17.0.0rc1/tests/Inputs/xunit-output/dummy_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import os
+
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 import lit.formats
 import lit.Test
 
+
 class DummyFormat(lit.formats.FileBasedTest):
     def execute(self, test, lit_config):
         # In this dummy format, expect that each test file is actually just a
         # .ini format dump of the results to report.
 
         source_path = test.getSourcePath()
 
         cfg = ConfigParser.ConfigParser()
         cfg.read(source_path)
 
         # Create the basic test result.
-        result_code = cfg.get('global', 'result_code')
-        result_output = cfg.get('global', 'result_output')
-        result = lit.Test.Result(getattr(lit.Test, result_code),
-                                 result_output)
+        result_code = cfg.get("global", "result_code")
+        result_output = cfg.get("global", "result_output")
+        result = lit.Test.Result(getattr(lit.Test, result_code), result_output)
 
-        if cfg.has_option('global', 'required_feature'):
-            required_feature = cfg.get('global', 'required_feature')
+        if cfg.has_option("global", "required_feature"):
+            required_feature = cfg.get("global", "required_feature")
             if required_feature:
                 test.requires.append(required_feature)
 
         # Load additional metrics.
-        for key,value_str in cfg.items('results'):
+        for key, value_str in cfg.items("results"):
             value = eval(value_str)
             if isinstance(value, int):
                 metric = lit.Test.IntMetricValue(value)
             elif isinstance(value, float):
                 metric = lit.Test.RealMetricValue(value)
             else:
                 raise RuntimeError("unsupported result type")
             result.addMetric(key, metric)
 
         return result
-
```

### Comparing `lit-16.0.6/tests/allow-retries.py` & `lit-17.0.0rc1/tests/allow-retries.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/discovery.py` & `lit-17.0.0rc1/tests/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,27 +130,23 @@
 # RUN:     %{inputs}/exec-discovery/subdir/test-three.py \
 # RUN:   --show-tests --show-suites -v > %t.out
 # RUN: FileCheck --check-prefix=CHECK-ASEXEC-DIRECT-TEST < %t.out %s
 #
 # CHECK-ASEXEC-DIRECT-TEST: -- Available Tests --
 # CHECK-ASEXEC-DIRECT-TEST: top-level-suite :: subdir/test-three
 
-# Check an error is emitted when the directly named test would not be run
-# indirectly (e.g. when the directory containing the test is specified).
+# Check that an error is emitted when the directly named test does not satisfy
+# the test config's requirements.
 #
 # RUN: not %{lit} \
 # RUN:     %{inputs}/discovery/test.not-txt 2>%t.err
-# RUN: FileCheck --check-prefix=CHECK-ERROR-INDIRECT-RUN-CHECK < %t.err %s
+# RUN: FileCheck --check-prefix=CHECK-ERROR-INPUT-CONTAINED-NO-TESTS < %t.err %s
 #
-# CHECK-ERROR-INDIRECT-RUN-CHECK: error: 'top-level-suite :: test.not-txt' would not be run indirectly
-
-# Check that no error is emitted with --no-indirectly-run-check.
-#
-# RUN: %{lit} \
-# RUN:     %{inputs}/discovery/test.not-txt --no-indirectly-run-check
+# CHECK-ERROR-INPUT-CONTAINED-NO-TESTS: warning: input 'Inputs/discovery/test.not-txt' contained no tests
+# CHECK-ERROR-INPUT-CONTAINED-NO-TESTS: error: did not discover any tests for provided path(s)
 
 # Check that a standalone test with no suffixes set is run without any errors.
 #
 # RUN: %{lit} %{inputs}/standalone-tests/true.txt > %t.out
 # RUN: FileCheck --check-prefix=CHECK-STANDALONE < %t.out %s
 #
 # CHECK-STANDALONE: PASS: Standalone tests :: true.txt
@@ -174,14 +170,23 @@
 # Check that no discovery is done for testsuite with standalone tests.
 #
 # RUN: not %{lit} %{inputs}/standalone-tests 2>%t.err
 # RUN: FileCheck --check-prefix=CHECK-STANDALONE-DISCOVERY < %t.err %s
 #
 # CHECK-STANDALONE-DISCOVERY: error: did not discover any tests for provided path(s)
 
+# Check that a single file path can result in multiple tests being discovered if
+# the test format implements those semantics.
+#
+# RUN: %{lit} %{inputs}/discovery-getTestsForPath/x.test > %t.out
+# RUN: FileCheck --check-prefix=CHECK-getTestsForPath < %t.out %s
+#
+# CHECK-getTestsForPath: PASS: discovery-getTestsForPath-suite :: {{.+}}one.test
+# CHECK-getTestsForPath: PASS: discovery-getTestsForPath-suite :: {{.+}}two.test
+
 # Check that we don't recurse infinitely when loading an site specific test
 # suite located inside the test source root.
 #
 # RUN: %{lit} \
 # RUN:     %{inputs}/exec-discovery-in-tree/obj/ \
 # RUN:   --show-tests --show-suites -v > %t.out
 # RUN: FileCheck --check-prefix=CHECK-ASEXEC-INTREE < %t.out %s
```

### Comparing `lit-16.0.6/tests/googletest-crash.py` & `lit-17.0.0rc1/tests/googletest-crash.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/googletest-format-respect-gtest-sharding-env-vars.py` & `lit-17.0.0rc1/tests/googletest-format-respect-gtest-sharding-env-vars.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/googletest-format.py` & `lit-17.0.0rc1/tests/googletest-format.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/googletest-sanitizer-error.py` & `lit-17.0.0rc1/tests/googletest-sanitizer-error.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/googletest-timeout.py` & `lit-17.0.0rc1/tests/googletest-timeout.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/ignore-fail.py` & `lit-17.0.0rc1/tests/ignore-fail.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/lit-opts.py` & `lit-17.0.0rc1/tests/lit-opts.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/lit.cfg` & `lit-17.0.0rc1/tests/lit.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -7,109 +7,122 @@
 
 import lit.formats
 from lit.llvm import llvm_config
 
 # Configuration file for the 'lit' test runner.
 
 # name: The name of this test suite.
-config.name = 'lit'
+config.name = "lit"
 
 # testFormat: The test format to use to interpret tests.
 config.test_format = lit.formats.ShTest(execute_external=False)
 
 # suffixes: A list of file extensions to treat as test files.
-config.suffixes = ['.py']
+config.suffixes = [".py"]
 
 # excludes: A list of individual files to exclude.
-config.excludes = ['Inputs']
+config.excludes = ["Inputs"]
 
 # test_source_root: The root path where tests are located.
 config.test_source_root = os.path.dirname(__file__)
 config.test_exec_root = config.test_source_root
 
-config.target_triple = '(unused)'
+config.target_triple = "(unused)"
 
-llvm_src_root = getattr(config, 'llvm_src_root', None)
+llvm_src_root = getattr(config, "llvm_src_root", None)
 if llvm_src_root:
-  # ``test_source_root`` may be in LLVM's binary build directory which does not contain
-  # ``lit.py``, so use `llvm_src_root` instead.
-  lit_path = os.path.join(llvm_src_root, 'utils', 'lit')
+    # ``test_source_root`` may be in LLVM's binary build directory which does not contain
+    # ``lit.py``, so use `llvm_src_root` instead.
+    lit_path = os.path.join(llvm_src_root, "utils", "lit")
 else:
-  lit_path = os.path.join(config.test_source_root, '..')
+    lit_path = os.path.join(config.test_source_root, "..")
 lit_path = os.path.abspath(lit_path)
 
 # Required because some tests import the lit module
 if llvm_config:
-  llvm_config.with_environment('PYTHONPATH', lit_path, append_path=True)
+    llvm_config.with_environment("PYTHONPATH", lit_path, append_path=True)
 else:
-  config.environment['PYTHONPATH'] = lit_path
+    config.environment["PYTHONPATH"] = lit_path
 # Do not add user-site packages directory to the python search path. This avoids test failures if there's an
 # incompatible lit module installed inside the user-site packages directory, as it gets prioritized over the lit
 # from the PYTHONPATH.
-config.environment['PYTHONNOUSERSITE'] = '1'
+config.environment["PYTHONNOUSERSITE"] = "1"
 
 # Add llvm and lit tools directories if this config is being loaded indirectly.
 # In this case, we can also expect llvm_config to have been imported correctly.
-for attribute in ('llvm_tools_dir', 'lit_tools_dir'):
+for attribute in ("llvm_tools_dir", "lit_tools_dir"):
     directory = getattr(config, attribute, None)
     if directory:
-        llvm_config.with_environment('PATH', directory, append_path=True)
+        llvm_config.with_environment("PATH", directory, append_path=True)
 
 # This test suite calls %{lit} to test lit's behavior for the sample test
 # suites in %{inputs}.  This test suite's results are then determined in part
 # by %{lit}'s textual output, which includes the output of FileCheck calls
 # within %{inputs}'s test suites.  Thus, %{lit} clears environment variables
 # that can affect FileCheck's output.  It also includes "--order=lexical -j1"
 # to ensure predictable test order, as it is often required for FileCheck
 # matches.
-config.substitutions.append(('%{inputs}', 'Inputs'))
-config.substitutions.append(('%{lit}', '%{lit-no-order-opt} --order=lexical'))
-config.substitutions.append(('%{lit-no-order-opt}',
-    "{env} %{{python}} {lit} -j1".format(
-        env="env -u FILECHECK_OPTS",
-        lit=os.path.join(lit_path, 'lit.py'))))
-config.substitutions.append(('%{python}', '"%s"' % (sys.executable)))
+config.substitutions.append(("%{inputs}", "Inputs"))
+config.substitutions.append(("%{lit}", "%{lit-no-order-opt} --order=lexical"))
+config.substitutions.append(
+    (
+        "%{lit-no-order-opt}",
+        "{env} %{{python}} {lit} -j1".format(
+            env="env -u FILECHECK_OPTS", lit=os.path.join(lit_path, "lit.py")
+        ),
+    )
+)
+config.substitutions.append(("%{python}", '"%s"' % (sys.executable)))
 
 # Enable coverage.py reporting, assuming the coverage module has been installed
 # and sitecustomize.py in the virtualenv has been modified appropriately.
-if lit_config.params.get('check-coverage', None):
-    config.environment['COVERAGE_PROCESS_START'] = os.path.join(
-        os.path.dirname(__file__), ".coveragerc")
+if lit_config.params.get("check-coverage", None):
+    config.environment["COVERAGE_PROCESS_START"] = os.path.join(
+        os.path.dirname(__file__), ".coveragerc"
+    )
 
 # Add a feature to detect if test cancellation is available. Check the ability
 # to do cancellation in the same environment as where RUN commands are run.
 # The reason is that on most systems cancellation depends on psutil being
 # available and RUN commands are run with a cleared PYTHONPATH and user site
 # packages disabled.
-testing_script_path = "/".join((os.path.dirname(__file__),
-                                "check-tested-lit-timeout-ability"))
-proc = subprocess.run([sys.executable, testing_script_path],
-                      stderr=subprocess.PIPE, env=config.environment,
-                      universal_newlines=True)
+testing_script_path = "/".join(
+    (os.path.dirname(__file__), "check-tested-lit-timeout-ability")
+)
+proc = subprocess.run(
+    [sys.executable, testing_script_path],
+    stderr=subprocess.PIPE,
+    env=config.environment,
+    universal_newlines=True,
+)
 if proc.returncode == 0:
     config.available_features.add("lit-max-individual-test-time")
 else:
     errormsg = proc.stderr
-    lit_config.warning('Setting a timeout per test not supported. ' + errormsg
-                       + ' Some tests will be skipped and the --timeout'
-                         ' command line argument will not work.')
+    lit_config.warning(
+        "Setting a timeout per test not supported. "
+        + errormsg
+        + " Some tests will be skipped and the --timeout"
+        " command line argument will not work."
+    )
 
 # When running the lit tests standalone, we want to define the same features
 # that the llvm_config defines. This means that the 'system-windows' feature
 # (and any others) need to match the names in llvm_config for consistency
 if not llvm_config:
-  if sys.platform.startswith('win') or sys.platform.startswith('cygwin'):
-    config.available_features.add('system-windows')
-  if platform.system() == 'AIX':
-    config.available_features.add('system-aix')
+    if sys.platform.startswith("win") or sys.platform.startswith("cygwin"):
+        config.available_features.add("system-windows")
+    if platform.system() == "AIX":
+        config.available_features.add("system-aix")
 
 # For each of lit's internal shell commands ('env', 'cd', 'diff', etc.), put
 # a fake command that always fails at the start of PATH.  This helps us check
 # that we always use lit's internal version rather than some external version
 # that might not be present or behave correctly on all platforms.  Don't do
 # this for 'echo' because an external version is used when it appears in a
 # pipeline.  Don't do this for ':' because it doesn't appear to be a valid file
 # name under Windows. Don't do this for 'not' because lit uses the external
 # 'not' throughout a RUN line that calls 'not --crash'.
-test_bin = os.path.join(os.path.dirname(__file__), 'Inputs', 'fake-externals')
-config.environment['PATH'] = os.path.pathsep.join((test_bin,
-                                                   config.environment['PATH']))
+test_bin = os.path.join(os.path.dirname(__file__), "Inputs", "fake-externals")
+config.environment["PATH"] = os.path.pathsep.join(
+    (test_bin, config.environment["PATH"])
+)
```

### Comparing `lit-16.0.6/tests/max-failures.py` & `lit-17.0.0rc1/tests/max-failures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # UNSUPPORTED: system-windows
+# FIXME: This test is flaky and hangs randomly on multi-core systems.
+# See https://github.com/llvm/llvm-project/issues/56336 for more
+# details.
+# REQUIRES:  less-than-4-cpu-cores-in-parallel
 
 # Check the behavior of --max-failures option.
 #
 # RUN: not %{lit}                  %{inputs}/max-failures >  %t.out 2>&1
 # RUN: not %{lit} --max-failures=1 %{inputs}/max-failures >> %t.out 2>&1
 # RUN: not %{lit} --max-failures=2 %{inputs}/max-failures >> %t.out 2>&1
 # RUN: not %{lit} --max-failures=0 %{inputs}/max-failures 2>> %t.out
```

### Comparing `lit-16.0.6/tests/parallelism-groups.py` & `lit-17.0.0rc1/tests/parallelism-groups.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/progress-bar.py` & `lit-17.0.0rc1/tests/progress-bar.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/reorder.py` & `lit-17.0.0rc1/tests/reorder.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/selecting.py` & `lit-17.0.0rc1/tests/selecting.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/show-result-codes.py` & `lit-17.0.0rc1/tests/show-result-codes.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/show-used-features.py` & `lit-17.0.0rc1/tests/show-used-features.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-define.py` & `lit-17.0.0rc1/tests/shtest-define.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-env.py` & `lit-17.0.0rc1/tests/shtest-env.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-format-argv0.py` & `lit-17.0.0rc1/tests/shtest-format-argv0.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-format.py` & `lit-17.0.0rc1/tests/shtest-format.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-if-else.py` & `lit-17.0.0rc1/tests/shtest-if-else.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-inject.py` & `lit-17.0.0rc1/tests/shtest-inject.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-keyword-parse-errors.py` & `lit-17.0.0rc1/tests/shtest-keyword-parse-errors.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-not.py` & `lit-17.0.0rc1/tests/shtest-not.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-output-printing.py` & `lit-17.0.0rc1/tests/shtest-output-printing.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-pushd-popd.py` & `lit-17.0.0rc1/tests/shtest-pushd-popd.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-recursive-substitution.py` & `lit-17.0.0rc1/tests/shtest-recursive-substitution.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-run-at-line.py` & `lit-17.0.0rc1/tests/shtest-run-at-line.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-shell.py` & `lit-17.0.0rc1/tests/shtest-shell.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/shtest-timeout.py` & `lit-17.0.0rc1/tests/shtest-timeout.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/test-data-micro.py` & `lit-17.0.0rc1/tests/test-data-micro.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/test-output-micro-resultdb.py` & `lit-17.0.0rc1/tests/test-output-micro-resultdb.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/test-output-micro.py` & `lit-17.0.0rc1/tests/test-output-micro.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/test-output-resultdb.py` & `lit-17.0.0rc1/tests/test-output-resultdb.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/test-output.py` & `lit-17.0.0rc1/tests/test-output.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/unit/TestRunner.py` & `lit-17.0.0rc1/tests/unit/TestRunner.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,66 +6,69 @@
 import os.path
 import platform
 import unittest
 
 import lit.discovery
 import lit.LitConfig
 import lit.Test as Test
-from lit.TestRunner import ParserKind, IntegratedTestKeywordParser, \
-                           parseIntegratedTestScript
+from lit.TestRunner import (
+    ParserKind,
+    IntegratedTestKeywordParser,
+    parseIntegratedTestScript,
+)
 
 
 class TestIntegratedTestKeywordParser(unittest.TestCase):
     inputTestCase = None
 
     @staticmethod
     def load_keyword_parser_lit_tests():
         """
         Create and load the LIT test suite and test objects used by
         TestIntegratedTestKeywordParser
         """
         # Create the global config object.
-        lit_config = lit.LitConfig.LitConfig(progname='lit',
-                                             path=[],
-                                             quiet=False,
-                                             useValgrind=False,
-                                             valgrindLeakCheck=False,
-                                             valgrindArgs=[],
-                                             noExecute=False,
-                                             debug=False,
-                                             isWindows=(
-                                               platform.system() == 'Windows'),
-                                             order='smart',
-                                             params={})
+        lit_config = lit.LitConfig.LitConfig(
+            progname="lit",
+            path=[],
+            quiet=False,
+            useValgrind=False,
+            valgrindLeakCheck=False,
+            valgrindArgs=[],
+            noExecute=False,
+            debug=False,
+            isWindows=(platform.system() == "Windows"),
+            order="smart",
+            params={},
+        )
         TestIntegratedTestKeywordParser.litConfig = lit_config
         # Perform test discovery.
         test_path = os.path.dirname(os.path.dirname(__file__))
-        inputs = [os.path.join(test_path, 'Inputs/testrunner-custom-parsers/')]
+        inputs = [os.path.join(test_path, "Inputs/testrunner-custom-parsers/")]
         assert os.path.isdir(inputs[0])
-        tests = lit.discovery.find_tests_for_inputs(lit_config, inputs, False)
+        tests = lit.discovery.find_tests_for_inputs(lit_config, inputs)
         assert len(tests) == 1 and "there should only be one test"
         TestIntegratedTestKeywordParser.inputTestCase = tests[0]
 
     @staticmethod
     def make_parsers():
         def custom_parse(line_number, line, output):
             if output is None:
                 output = []
-            output += [part for part in line.split(' ') if part.strip()]
+            output += [part for part in line.split(" ") if part.strip()]
             return output
 
         return [
             IntegratedTestKeywordParser("MY_TAG.", ParserKind.TAG),
             IntegratedTestKeywordParser("MY_DNE_TAG.", ParserKind.TAG),
             IntegratedTestKeywordParser("MY_LIST:", ParserKind.LIST),
             IntegratedTestKeywordParser("MY_BOOL:", ParserKind.BOOLEAN_EXPR),
             IntegratedTestKeywordParser("MY_INT:", ParserKind.INTEGER),
             IntegratedTestKeywordParser("MY_RUN:", ParserKind.COMMAND),
-            IntegratedTestKeywordParser("MY_CUSTOM:", ParserKind.CUSTOM,
-                                        custom_parse),
+            IntegratedTestKeywordParser("MY_CUSTOM:", ParserKind.CUSTOM, custom_parse),
             IntegratedTestKeywordParser("MY_DEFINE:", ParserKind.DEFINE),
             IntegratedTestKeywordParser("MY_REDEFINE:", ParserKind.REDEFINE),
         ]
 
     @staticmethod
     def get_parser(parser_list, keyword):
         for p in parser_list:
@@ -73,128 +76,132 @@
                 return p
         assert False and "parser not found"
 
     @staticmethod
     def parse_test(parser_list, allow_result=False):
         script = parseIntegratedTestScript(
             TestIntegratedTestKeywordParser.inputTestCase,
-            additional_parsers=parser_list, require_script=False)
+            additional_parsers=parser_list,
+            require_script=False,
+        )
         if isinstance(script, lit.Test.Result):
             assert allow_result
         else:
             assert isinstance(script, list)
             assert len(script) == 0
         return script
 
     def test_tags(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        tag_parser = self.get_parser(parsers, 'MY_TAG.')
-        dne_tag_parser = self.get_parser(parsers, 'MY_DNE_TAG.')
+        tag_parser = self.get_parser(parsers, "MY_TAG.")
+        dne_tag_parser = self.get_parser(parsers, "MY_DNE_TAG.")
         self.assertTrue(tag_parser.getValue())
         self.assertFalse(dne_tag_parser.getValue())
 
     def test_lists(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        list_parser = self.get_parser(parsers, 'MY_LIST:')
-        self.assertEqual(list_parser.getValue(),
-                              ['one', 'two', 'three', 'four'])
+        list_parser = self.get_parser(parsers, "MY_LIST:")
+        self.assertEqual(list_parser.getValue(), ["one", "two", "three", "four"])
 
     def test_commands(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        cmd_parser = self.get_parser(parsers, 'MY_RUN:')
+        cmd_parser = self.get_parser(parsers, "MY_RUN:")
         value = cmd_parser.getValue()
         self.assertEqual(len(value), 2)  # there are only two run lines
-        self.assertEqual(value[0].command.strip(),
-                         "%dbg(MY_RUN: at line 4)  baz")
-        self.assertEqual(value[1].command.strip(),
-                         "%dbg(MY_RUN: at line 7)  foo  bar")
+        self.assertEqual(value[0].command.strip(), "%dbg(MY_RUN: at line 4)  baz")
+        self.assertEqual(value[1].command.strip(), "%dbg(MY_RUN: at line 7)  foo  bar")
 
     def test_boolean(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        bool_parser = self.get_parser(parsers, 'MY_BOOL:')
+        bool_parser = self.get_parser(parsers, "MY_BOOL:")
         value = bool_parser.getValue()
         self.assertEqual(len(value), 2)  # there are only two run lines
         self.assertEqual(value[0].strip(), "a && (b)")
         self.assertEqual(value[1].strip(), "d")
 
     def test_integer(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        int_parser = self.get_parser(parsers, 'MY_INT:')
+        int_parser = self.get_parser(parsers, "MY_INT:")
         value = int_parser.getValue()
         self.assertEqual(len(value), 2)  # there are only two MY_INT: lines
         self.assertEqual(type(value[0]), int)
         self.assertEqual(value[0], 4)
         self.assertEqual(type(value[1]), int)
         self.assertEqual(value[1], 6)
 
     def test_bad_parser_type(self):
         parsers = self.make_parsers() + ["BAD_PARSER_TYPE"]
         script = self.parse_test(parsers, allow_result=True)
         self.assertTrue(isinstance(script, lit.Test.Result))
         self.assertEqual(script.code, lit.Test.UNRESOLVED)
-        self.assertEqual('Additional parser must be an instance of '
-                         'IntegratedTestKeywordParser',
-                         script.output)
+        self.assertEqual(
+            "Additional parser must be an instance of " "IntegratedTestKeywordParser",
+            script.output,
+        )
 
     def test_duplicate_keyword(self):
-        parsers = self.make_parsers() + \
-            [IntegratedTestKeywordParser("KEY:", ParserKind.BOOLEAN_EXPR),
-             IntegratedTestKeywordParser("KEY:", ParserKind.BOOLEAN_EXPR)]
+        parsers = self.make_parsers() + [
+            IntegratedTestKeywordParser("KEY:", ParserKind.BOOLEAN_EXPR),
+            IntegratedTestKeywordParser("KEY:", ParserKind.BOOLEAN_EXPR),
+        ]
         script = self.parse_test(parsers, allow_result=True)
         self.assertTrue(isinstance(script, lit.Test.Result))
         self.assertEqual(script.code, lit.Test.UNRESOLVED)
-        self.assertEqual("Parser for keyword 'KEY:' already exists",
-                         script.output)
+        self.assertEqual("Parser for keyword 'KEY:' already exists", script.output)
 
     def test_boolean_unterminated(self):
-        parsers = self.make_parsers() + \
-            [IntegratedTestKeywordParser("MY_BOOL_UNTERMINATED:", ParserKind.BOOLEAN_EXPR)]
+        parsers = self.make_parsers() + [
+            IntegratedTestKeywordParser(
+                "MY_BOOL_UNTERMINATED:", ParserKind.BOOLEAN_EXPR
+            )
+        ]
         script = self.parse_test(parsers, allow_result=True)
         self.assertTrue(isinstance(script, lit.Test.Result))
         self.assertEqual(script.code, lit.Test.UNRESOLVED)
-        self.assertEqual("Test has unterminated 'MY_BOOL_UNTERMINATED:' lines "
-                         "(with '\\')",
-                         script.output)
+        self.assertEqual(
+            "Test has unterminated 'MY_BOOL_UNTERMINATED:' lines " "(with '\\')",
+            script.output,
+        )
 
     def test_custom(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        custom_parser = self.get_parser(parsers, 'MY_CUSTOM:')
+        custom_parser = self.get_parser(parsers, "MY_CUSTOM:")
         value = custom_parser.getValue()
-        self.assertEqual(value, ['a', 'b', 'c'])
+        self.assertEqual(value, ["a", "b", "c"])
 
     def test_defines(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        cmd_parser = self.get_parser(parsers, 'MY_DEFINE:')
+        cmd_parser = self.get_parser(parsers, "MY_DEFINE:")
         value = cmd_parser.getValue()
-        self.assertEqual(len(value), 1) # there's only one MY_DEFINE directive
+        self.assertEqual(len(value), 1)  # there's only one MY_DEFINE directive
         self.assertEqual(value[0].new_subst, True)
-        self.assertEqual(value[0].name, '%{name}')
-        self.assertEqual(value[0].value, 'value one')
+        self.assertEqual(value[0].name, "%{name}")
+        self.assertEqual(value[0].value, "value one")
 
     def test_redefines(self):
         parsers = self.make_parsers()
         self.parse_test(parsers)
-        cmd_parser = self.get_parser(parsers, 'MY_REDEFINE:')
+        cmd_parser = self.get_parser(parsers, "MY_REDEFINE:")
         value = cmd_parser.getValue()
-        self.assertEqual(len(value), 1) # there's only one MY_REDEFINE directive
+        self.assertEqual(len(value), 1)  # there's only one MY_REDEFINE directive
         self.assertEqual(value[0].new_subst, False)
-        self.assertEqual(value[0].name, '%{name}')
-        self.assertEqual(value[0].value, 'value two')
+        self.assertEqual(value[0].name, "%{name}")
+        self.assertEqual(value[0].value, "value two")
 
     def test_bad_keywords(self):
         def custom_parse(line_number, line, output):
             return output
-        
+
         try:
             IntegratedTestKeywordParser("TAG_NO_SUFFIX", ParserKind.TAG),
             self.fail("TAG_NO_SUFFIX failed to raise an exception")
         except ValueError as e:
             pass
         except BaseException as e:
             self.fail("TAG_NO_SUFFIX raised the wrong exception: %r" % e)
@@ -212,107 +219,140 @@
             self.fail("LIST_WITH_DOT. failed to raise an exception")
         except ValueError as e:
             pass
         except BaseException as e:
             self.fail("LIST_WITH_DOT. raised the wrong exception: %r" % e)
 
         try:
-            IntegratedTestKeywordParser("CUSTOM_NO_SUFFIX",
-                                        ParserKind.CUSTOM, custom_parse),
+            IntegratedTestKeywordParser(
+                "CUSTOM_NO_SUFFIX", ParserKind.CUSTOM, custom_parse
+            ),
             self.fail("CUSTOM_NO_SUFFIX failed to raise an exception")
         except ValueError as e:
             pass
         except BaseException as e:
             self.fail("CUSTOM_NO_SUFFIX raised the wrong exception: %r" % e)
 
         # Both '.' and ':' are allowed for CUSTOM keywords.
         try:
-            IntegratedTestKeywordParser("CUSTOM_WITH_DOT.",
-                                        ParserKind.CUSTOM, custom_parse),
+            IntegratedTestKeywordParser(
+                "CUSTOM_WITH_DOT.", ParserKind.CUSTOM, custom_parse
+            ),
         except BaseException as e:
             self.fail("CUSTOM_WITH_DOT. raised an exception: %r" % e)
         try:
-            IntegratedTestKeywordParser("CUSTOM_WITH_COLON:",
-                                        ParserKind.CUSTOM, custom_parse),
+            IntegratedTestKeywordParser(
+                "CUSTOM_WITH_COLON:", ParserKind.CUSTOM, custom_parse
+            ),
         except BaseException as e:
             self.fail("CUSTOM_WITH_COLON: raised an exception: %r" % e)
 
         try:
-            IntegratedTestKeywordParser("CUSTOM_NO_PARSER:",
-                                        ParserKind.CUSTOM),
+            IntegratedTestKeywordParser("CUSTOM_NO_PARSER:", ParserKind.CUSTOM),
             self.fail("CUSTOM_NO_PARSER: failed to raise an exception")
         except ValueError as e:
             pass
         except BaseException as e:
             self.fail("CUSTOM_NO_PARSER: raised the wrong exception: %r" % e)
 
+
 class TestApplySubtitutions(unittest.TestCase):
     def test_simple(self):
         script = ["echo %bar"]
         substitutions = [("%bar", "hello")]
         result = lit.TestRunner.applySubstitutions(script, substitutions)
         self.assertEqual(result, ["echo hello"])
 
     def test_multiple_substitutions(self):
         script = ["echo %bar %baz"]
-        substitutions = [("%bar", "hello"),
-                         ("%baz", "world"),
-                         ("%useless", "shouldnt expand")]
+        substitutions = [
+            ("%bar", "hello"),
+            ("%baz", "world"),
+            ("%useless", "shouldnt expand"),
+        ]
         result = lit.TestRunner.applySubstitutions(script, substitutions)
         self.assertEqual(result, ["echo hello world"])
 
     def test_multiple_script_lines(self):
-        script = ["%cxx %compile_flags -c -o %t.o",
-                  "%cxx %link_flags %t.o -o %t.exe"]
-        substitutions = [("%cxx", "clang++"),
-                         ("%compile_flags", "-std=c++11 -O3"),
-                         ("%link_flags", "-lc++")]
+        script = ["%cxx %compile_flags -c -o %t.o", "%cxx %link_flags %t.o -o %t.exe"]
+        substitutions = [
+            ("%cxx", "clang++"),
+            ("%compile_flags", "-std=c++11 -O3"),
+            ("%link_flags", "-lc++"),
+        ]
         result = lit.TestRunner.applySubstitutions(script, substitutions)
-        self.assertEqual(result, ["clang++ -std=c++11 -O3 -c -o %t.o",
-                                  "clang++ -lc++ %t.o -o %t.exe"])
+        self.assertEqual(
+            result,
+            ["clang++ -std=c++11 -O3 -c -o %t.o", "clang++ -lc++ %t.o -o %t.exe"],
+        )
 
     def test_recursive_substitution_real(self):
         script = ["%build %s"]
-        substitutions = [("%cxx", "clang++"),
-                         ("%compile_flags", "-std=c++11 -O3"),
-                         ("%link_flags", "-lc++"),
-                         ("%build", "%cxx %compile_flags %link_flags %s -o %t.exe")]
-        result = lit.TestRunner.applySubstitutions(script, substitutions, recursion_limit=3)
+        substitutions = [
+            ("%cxx", "clang++"),
+            ("%compile_flags", "-std=c++11 -O3"),
+            ("%link_flags", "-lc++"),
+            ("%build", "%cxx %compile_flags %link_flags %s -o %t.exe"),
+        ]
+        result = lit.TestRunner.applySubstitutions(
+            script, substitutions, recursion_limit=3
+        )
         self.assertEqual(result, ["clang++ -std=c++11 -O3 -lc++ %s -o %t.exe %s"])
 
     def test_recursive_substitution_limit(self):
         script = ["%rec5"]
         # Make sure the substitutions are not in an order where the global
         # substitution would appear to be recursive just because they are
         # processed in the right order.
-        substitutions = [("%rec1", "STOP"), ("%rec2", "%rec1"),
-                         ("%rec3", "%rec2"), ("%rec4", "%rec3"), ("%rec5", "%rec4")]
+        substitutions = [
+            ("%rec1", "STOP"),
+            ("%rec2", "%rec1"),
+            ("%rec3", "%rec2"),
+            ("%rec4", "%rec3"),
+            ("%rec5", "%rec4"),
+        ]
         for limit in [5, 6, 7]:
-            result = lit.TestRunner.applySubstitutions(script, substitutions, recursion_limit=limit)
+            result = lit.TestRunner.applySubstitutions(
+                script, substitutions, recursion_limit=limit
+            )
             self.assertEqual(result, ["STOP"])
 
     def test_recursive_substitution_limit_exceeded(self):
         script = ["%rec5"]
-        substitutions = [("%rec1", "STOP"), ("%rec2", "%rec1"),
-                         ("%rec3", "%rec2"), ("%rec4", "%rec3"), ("%rec5", "%rec4")]
+        substitutions = [
+            ("%rec1", "STOP"),
+            ("%rec2", "%rec1"),
+            ("%rec3", "%rec2"),
+            ("%rec4", "%rec3"),
+            ("%rec5", "%rec4"),
+        ]
         for limit in [0, 1, 2, 3, 4]:
             try:
-                lit.TestRunner.applySubstitutions(script, substitutions, recursion_limit=limit)
+                lit.TestRunner.applySubstitutions(
+                    script, substitutions, recursion_limit=limit
+                )
                 self.fail("applySubstitutions should have raised an exception")
             except ValueError:
                 pass
 
     def test_recursive_substitution_invalid_value(self):
         script = ["%rec5"]
-        substitutions = [("%rec1", "STOP"), ("%rec2", "%rec1"),
-                         ("%rec3", "%rec2"), ("%rec4", "%rec3"), ("%rec5", "%rec4")]
+        substitutions = [
+            ("%rec1", "STOP"),
+            ("%rec2", "%rec1"),
+            ("%rec3", "%rec2"),
+            ("%rec4", "%rec3"),
+            ("%rec5", "%rec4"),
+        ]
         for limit in [-1, -2, -3, "foo"]:
             try:
-                lit.TestRunner.applySubstitutions(script, substitutions, recursion_limit=limit)
+                lit.TestRunner.applySubstitutions(
+                    script, substitutions, recursion_limit=limit
+                )
                 self.fail("applySubstitutions should have raised an exception")
             except AssertionError:
                 pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     TestIntegratedTestKeywordParser.load_keyword_parser_lit_tests()
     unittest.main(verbosity=2)
```

### Comparing `lit-16.0.6/tests/unparsed-requirements.py` & `lit-17.0.0rc1/tests/unparsed-requirements.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 # RUN: %{python} %s %{inputs}/unparsed-requirements
 
 import sys
 from lit.Test import Result, Test, TestSuite
 from lit.TestRunner import parseIntegratedTestScript
 from lit.TestingConfig import TestingConfig
 
-config = TestingConfig(None, "config", [".txt"], None, [], [], False, sys.argv[1], sys.argv[1], [], [], True)
+config = TestingConfig(
+    None,
+    "config",
+    [".txt"],
+    None,
+    [],
+    [],
+    False,
+    sys.argv[1],
+    sys.argv[1],
+    [],
+    [],
+    True,
+)
 suite = TestSuite("suite", sys.argv[1], sys.argv[1], config)
 
 test = Test(suite, ["test.py"], config)
 test.requires = ["meow"]
 test.unsupported = ["alpha"]
 test.xfails = ["foo"]
```

### Comparing `lit-16.0.6/tests/use-llvm-tool.py` & `lit-17.0.0rc1/tests/use-llvm-tool.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/xfail-cl.py` & `lit-17.0.0rc1/tests/xfail-cl.py`

 * *Files identical despite different names*

### Comparing `lit-16.0.6/tests/xunit-output.py` & `lit-17.0.0rc1/tests/xunit-output.py`

 * *Files identical despite different names*

