# Comparing `tmp/onefuzz-8.6.0.tar.gz` & `tmp/onefuzz-8.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-8.6.0.tar", last modified: Wed Jul 26 23:07:44 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.6.1.tar", last modified: Fri Jul 28 22:46:34 2023, max compression
```

## Comparing `onefuzz-8.6.0.tar` & `onefuzz-8.6.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/
--rw-rw-rw-   0        0        0     1162 2023-07-26 23:07:11.000000 onefuzz-8.6.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-07-26 23:07:11.000000 onefuzz-8.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-07-26 23:07:44.000000 onefuzz-8.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-07-26 23:07:11.000000 onefuzz-8.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      391 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       57 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/extra/
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-07-26 23:07:11.000000 onefuzz-8.6.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      902 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    70921 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1521 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22928 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1232 2023-07-26 23:07:43.000000 onefuzz-8.6.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    31472 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0      768 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/opentelemetry_exporter.py
--rw-rw-rw-   0        0        0     1682 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10701 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     7003 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    43098 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8812 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9630 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10709 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2015 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      443 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-07-26 23:07:11.000000 onefuzz-8.6.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-07-26 23:07:11.000000 onefuzz-8.6.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      607 2023-07-26 23:07:11.000000 onefuzz-8.6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 23:07:44.000000 onefuzz-8.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-07-26 23:07:11.000000 onefuzz-8.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-26 23:07:11.000000 onefuzz-8.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-07-26 23:07:11.000000 onefuzz-8.6.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/
+-rw-rw-rw-   0        0        0     1162 2023-07-28 22:46:02.000000 onefuzz-8.6.1/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-07-28 22:46:02.000000 onefuzz-8.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-07-28 22:46:34.000000 onefuzz-8.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-07-28 22:46:02.000000 onefuzz-8.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-07-28 22:46:02.000000 onefuzz-8.6.1/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/extra/
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-07-28 22:46:02.000000 onefuzz-8.6.1/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      902 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    70921 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1521 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22928 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz/data/
+-rw-rw-rw-   0        0        0     1232 2023-07-28 22:46:33.000000 onefuzz-8.6.1/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    31472 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0      768 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/opentelemetry_exporter.py
+-rw-rw-rw-   0        0        0     1682 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10701 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     7003 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    43098 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8812 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9630 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10709 2023-07-28 22:46:02.000000 onefuzz-8.6.1/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2015 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      443 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 22:46:34.000000 onefuzz-8.6.1/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-07-28 22:46:02.000000 onefuzz-8.6.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-07-28 22:46:02.000000 onefuzz-8.6.1/requirements-lint.txt
+-rw-rw-rw-   0        0        0      607 2023-07-28 22:46:02.000000 onefuzz-8.6.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 22:46:34.000000 onefuzz-8.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-07-28 22:46:02.000000 onefuzz-8.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 22:46:34.000000 onefuzz-8.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-28 22:46:02.000000 onefuzz-8.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-07-28 22:46:02.000000 onefuzz-8.6.1/tests/test_template_helper.py
```

### Comparing `onefuzz-8.6.0/LICENSE` & `onefuzz-8.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/PKG-INFO` & `onefuzz-8.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.6.0
+Version: 8.6.1
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.6.0/README.md` & `onefuzz-8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/domato.py` & `onefuzz-8.6.1/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/get-running.py` & `onefuzz-8.6.1/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/honggfuzz.py` & `onefuzz-8.6.1/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.6.1/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.6.1/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.6.1/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.6.1/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.6.1/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/examples/oss-fuzz-target.py` & `onefuzz-8.6.1/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/__main__.py` & `onefuzz-8.6.1/onefuzz/__main__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/api.py` & `onefuzz-8.6.1/onefuzz/api.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/azcopy.py` & `onefuzz-8.6.1/onefuzz/azcopy.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.6.1/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/backend.py` & `onefuzz-8.6.1/onefuzz/backend.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/cli.py` & `onefuzz-8.6.1/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/data/licenses.json` & `onefuzz-8.6.1/onefuzz/data/licenses.json`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/data/privacy.txt` & `onefuzz-8.6.1/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/debug.py` & `onefuzz-8.6.1/onefuzz/debug.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/job_templates/builder.py` & `onefuzz-8.6.1/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/job_templates/cache.py` & `onefuzz-8.6.1/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.6.1/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.6.1/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/job_templates/main.py` & `onefuzz-8.6.1/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/job_templates/manage.py` & `onefuzz-8.6.1/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/opentelemetry_exporter.py` & `onefuzz-8.6.1/onefuzz/opentelemetry_exporter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/rdp.py` & `onefuzz-8.6.1/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/ssh.py` & `onefuzz-8.6.1/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/status/cache.py` & `onefuzz-8.6.1/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/status/cmd.py` & `onefuzz-8.6.1/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/status/raw.py` & `onefuzz-8.6.1/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/status/signalr.py` & `onefuzz-8.6.1/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/status/top.py` & `onefuzz-8.6.1/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/status/top_view.py` & `onefuzz-8.6.1/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/template.py` & `onefuzz-8.6.1/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/templates/__init__.py` & `onefuzz-8.6.1/onefuzz/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/templates/afl.py` & `onefuzz-8.6.1/onefuzz/templates/afl.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.6.1/onefuzz/templates/libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.6.1/onefuzz/templates/ossfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/templates/radamsa.py` & `onefuzz-8.6.1/onefuzz/templates/radamsa.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz/templates/regression.py` & `onefuzz-8.6.1/onefuzz/templates/regression.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.6.1/onefuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.6.0
+Version: 8.6.1
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.6.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.6.1/onefuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/requirements.txt` & `onefuzz-8.6.1/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 PyJWT>=2.4.0
 opentelemetry-api==1.16.0
 opentelemetry-sdk==1.16.0
 opentelemetry-instrumentation-requests==0.37b0
 # install rsa version >=4.7 to fix CVE-2020-25658
 rsa>=4.7
 # onefuzztypes version is set during build
-onefuzztypes==8.6.0
+onefuzztypes==8.6.1
```

### Comparing `onefuzz-8.6.0/setup.py` & `onefuzz-8.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.6.0/tests/test_template_helper.py` & `onefuzz-8.6.1/tests/test_template_helper.py`

 * *Files identical despite different names*

