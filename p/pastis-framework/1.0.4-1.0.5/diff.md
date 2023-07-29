# Comparing `tmp/pastis-framework-1.0.4.tar.gz` & `tmp/pastis-framework-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastis-framework-1.0.4.tar", last modified: Thu Jul 20 13:50:18 2023, max compression
+gzip compressed data, was "pastis-framework-1.0.5.tar", last modified: Sat Jul 29 12:43:01 2023, max compression
```

## Comparing `pastis-framework-1.0.4.tar` & `pastis-framework-1.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16319 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/bin/pastis-benchmark
--rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/bin/pastis-broker
--rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/bin/pastisd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/bin/pastis-aflpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/aflppbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/aflpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/bin/pastis-honggfuzz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/hfbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/honggfuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-triton/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/engines/pastis-triton/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/bin/pastis-triton
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.530456 pastis-framework-1.0.4/engines/pastis-triton/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/engines/pastis-triton/broker-addon/pastisttbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/engines/pastis-triton/pastisdse/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/pastisdse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40564 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/engines/pastis-triton/pastisdse/pastisdse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/libpastis/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/enginedesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/libpastis/proto/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/proto/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/sast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/libpastis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/pastis_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 13:50:18.000000 pastis-framework-1.0.4/pastis_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/pastisbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/replayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbenchmark/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/pastisbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35282 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10450 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/stat_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/pastisbroker/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:50:18.534456 pastis-framework-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-20 13:50:15.000000 pastis-framework-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16489 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/bin/pastis-benchmark
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/bin/pastis-broker
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/bin/pastisd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-aflpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-aflpp/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/bin/pastis-aflpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/aflppbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/aflpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-honggfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-honggfuzz/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/bin/pastis-honggfuzz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/hfbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/honggfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-triton/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-triton/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/bin/pastis-triton
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-triton/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-triton/broker-addon/pastisttbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-triton/pastisdse/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/pastisdse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41039 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/pastisdse/pastisdse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/libpastis/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/enginedesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/libpastis/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/proto/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/sast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/pastis_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/pastisbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/replayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/pastisbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36051 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/stat_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/setup.py
```

### Comparing `pastis-framework-1.0.4/LICENSE` & `pastis-framework-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/PKG-INFO` & `pastis-framework-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.4
+Version: 1.0.5
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.4/README.md` & `pastis-framework-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/bin/pastis-benchmark` & `pastis-framework-1.0.5/bin/pastis-benchmark`

 * *Files 2% similar despite different names*

```diff
@@ -159,35 +159,37 @@
 @click.option('--probe', type=str, help="Probe to load as a python module (should contain a ProbeInterface)", multiple=True)
 @click.option('--skip-cpufreq', is_flag=True, type=bool, default=False, help="Skip CPU frequency scaling check")
 @click.option('--mem-threshold', type=int, default=85, help="RAM consumption limit", show_default=True)
 @click.option('--start-quorum', type=int, default=0, help="Number of client connection to receive before triggering startup", show_default=True)
 @click.option('--filter-inputs', type=bool, is_flag=True, default=False, help="Filter inputs that do not generate coverage", show_default=True)
 @click.option('--stream', type=bool, is_flag=True, default=False, help="Stream input and coverage info in the given file", show_default=True)
 @click.option('--replay-threads', type=int, default=4, help="number of threads to use for input replay", show_default=True)
+@click.option('--replay-timeout', type=int, default=60, help="Timeout for seed replay", show_default=True)
 @click.option('--proxy', type=str, default="", help="Run the broker as a proxy to another broker: pymodule@ip:port")
 @click.argument('pargs', nargs=-1)
 def run(workspace: str, bins: str, seeds: str, mode: str, injloc: str, aflpp: bool, hfuzz: bool, triton: bool,
         debug: bool, timeout: Optional[int], port: int, hfuzz_path: str, hfuzz_threads: int, spawn: bool,
         allow_remote: bool, probe: Tuple[str], skip_cpufreq: bool,  mem_threshold: int, start_quorum: int,  proxy: str,
-        filter_inputs: bool, stream: bool, replay_threads: int, pargs: Tuple[str]):
+        filter_inputs: bool, stream: bool, replay_threads: int, replay_timeout: int, pargs: Tuple[str]):
 
     configure_logging(logging.DEBUG if debug else logging.INFO, "%(asctime)s %(name)s [%(levelname)s] %(message)s")
 
     broker = PastisBroker(workspace,
                           bins,
                           BrokingMode[mode],
                           CheckMode.CHECK_ALL,
                           SeedInjectLoc[injloc],
                           None,
                           list(pargs),
                           mem_threshold,
                           start_quorum,
                           filter_inputs,
                           stream,
-                          replay_threads)
+                          replay_threads,
+                          replay_timeout)
 
     if proxy:  # proxy format should be:  IP:port@py_module
         try:
             py_module, url = proxy.split("@")
             proxy_ip, proxy_port = url.split(":")
             broker.set_proxy(proxy_ip, int(proxy_port), py_module)
         except ValueError:
```

### Comparing `pastis-framework-1.0.4/bin/pastis-broker` & `pastis-framework-1.0.5/bin/pastis-broker`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/bin/pastisd` & `pastis-framework-1.0.5/bin/pastisd`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/bin/pastis-aflpp` & `pastis-framework-1.0.5/engines/pastis-aflpp/bin/pastis-aflpp`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py` & `pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/__init__.py` & `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/aflpp.py` & `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/aflpp.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/driver.py` & `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/driver.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/replay.py` & `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-aflpp/pastisaflpp/workspace.py` & `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/bin/pastis-honggfuzz` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/bin/pastis-honggfuzz`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/__init__.py` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/driver.py` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/driver.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/honggfuzz.py` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/replay.py` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-honggfuzz/pastishf/workspace.py` & `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-triton/bin/pastis-triton` & `pastis-framework-1.0.5/engines/pastis-triton/bin/pastis-triton`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py` & `pastis-framework-1.0.5/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/engines/pastis-triton/pastisdse/pastisdse.py` & `pastis-framework-1.0.5/engines/pastis-triton/pastisdse/pastisdse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # built-in imports
 from typing import List, Tuple
 import os
 import time
 import logging
+from hashlib import md5
 from pathlib import Path
 import threading
 import platform
 import json
 import queue
 
 # third-party imports
@@ -20,14 +21,25 @@
 from tritondse.sanitizers import FormatStringSanitizer, NullDerefSanitizer, UAFSanitizer, IntegerOverflowSanitizer, mk_new_crashing_seed
 from tritondse.types      import Addr, Edge, SymExType, Architecture, Platform
 from libpastis import ClientAgent, BinaryPackage, SASTReport
 from libpastis.types      import SeedType, FuzzingEngineInfo, ExecMode, CoverageMode, SeedInjectLoc, CheckMode, LogLevel, AlertData, FuzzMode
 from tritondse.trace      import QBDITrace, TraceException
 from tritondse.worklist import FreshSeedPrioritizerWorklist, WorklistAddressToSet
 
+def to_h(seed: Seed) -> str:
+    if seed.is_composite():
+        if PastisDSE.INPUT_FILE_NAME in seed.content.files:
+            return md5(seed.content.files[PastisDSE.INPUT_FILE_NAME]).hexdigest()
+        elif "stdin" in seed.content.files:
+            return md5(seed.content.files["stdin"]).hexdigest()
+        else:
+            raise NameError("can't find main payload in Seed")
+    else:
+        return md5(seed.content).hexdigest()
+
 
 class PastisDSE(object):
 
     INPUT_FILE_NAME = "input_file"
     STAT_FILE = "pastidse-stats.json"
 
     RAMDISK = "/mnt/ramdisk"
@@ -488,19 +500,19 @@
         :param typ: The type of the seed
         :param seed: The seed
         :return: None
         """
         seed = self._get_seed(seed)
 
         if seed in self._seed_received:
-            logging.warning(f"receiving seed already known: {seed.hash} (dropped)")
+            logging.warning(f"receiving seed already known: {to_h(seed)} (dropped)")
             return
         else:
             self._seed_queue.put((seed, typ))
-            logging.info(f"seed received {seed.hash} (pool: {self._seed_queue.qsize()})")
+            logging.info(f"seed received {to_h(seed)} (pool: {self._seed_queue.qsize()})")
 
 
     def _process_seed_received(self, typ: SeedType, seed: Seed):
         """
         This function is called when we receive a seed from the broker.
 
         :param typ: The type of the seed
@@ -511,15 +523,15 @@
             if not self._tracing_enabled:
                 # Accept all seeds
                 self.dse.add_input_seed(seed)
 
             else:  # Try running the seed to know whether to keep it
                 # NOTE: re-run the seed regardless of its status
                 coverage = None
-                logging.info(f"process seed received {seed.hash} (pool: {self._seed_queue.qsize()})")
+                logging.info(f"process seed received {to_h(seed)} (pool: {self._seed_queue.qsize()})")
 
                 data = seed.content.files[self.INPUT_FILE_NAME] if seed.is_composite() else seed.bytes()
                 self.replay_seed_file.write_bytes(data)
                 # Adjust injection location before calling QBDITrace
                 if self._seedloc == SeedInjectLoc.STDIN:
                     stdin_file = str(self.replay_seed_file)
                     argv = self.config.program_argv
@@ -551,32 +563,32 @@
                     self._replay_acc += time.time() - t0  # Save time spent replaying inputs
                 except FileNotFoundError:
                     logging.warning("Cannot load the coverage file generated (maybe had crashed?)")
                 except TraceException:
                     logging.warning('There was an error while trying to re-run the seed')
 
                 if not coverage:
-                    logging.warning(f"coverage not found after replaying: {seed.hash} [{typ.name}] (add it anyway)")
+                    logging.warning(f"coverage not found after replaying: {to_h(seed)} [{typ.name}] (add it anyway)")
                     # Add the seed anyway, if it was not possible to re-run the seed.
                     # TODO Set seed.coverage_objectives as "empty" (use ellipsis
                     # object). Modify WorklistAddressToSet to support it.
                     self.seeds_merged += 1
                     self.dse.add_input_seed(seed)
                 else:
                     # Check whether the seed improves the current coverage.
                     if self.dse.coverage.improve_coverage(coverage):
-                        logging.info(f"seed added {seed.hash} [{typ.name}] (coverage merged)")
+                        logging.info(f"seed added {to_h(seed)} [{typ.name}] (coverage merged)")
                         self.seeds_merged += 1
                         self.dse.coverage.merge(coverage)
                         self.dse.seeds_manager.worklist.update_worklist(coverage)
 
                         seed.coverage_objectives = self.dse.coverage.new_items_to_cover(coverage)
                         self.dse.add_input_seed(seed)
                     else:
-                        logging.info(f"seed archived {seed.hash} [{typ.name}] (NOT merging coverage)")
+                        logging.info(f"seed archived {to_h(seed)} [{typ.name}] (NOT merging coverage)")
                         self.seeds_rejected += 1
                         #self.dse.seeds_manager.archive_seed(seed)
                         # logging.info(f"seed archived {seed.hash} [{typ.name}]")
 
             self._seed_received.add(seed)  # Remember seed received not to send them back
         except FileNotFoundError as e:
             # NOTE If reset() is call during the execution of this function,
@@ -592,15 +604,15 @@
         This function is called when the broker says stop. (Called from the agent thread)
         """
         logging.info(f"[BROKER] [STOP]")
 
         if self.dse:
             self.dse.stop_exploration()
 
-        self.save_stats()  # Save stats
+            self.save_stats()  # Save stats
 
         self._stop = True
         # self.agent.stop()  # Can't call it here as this function executed from within agent thread
 
     def save_stats(self):
         stat_file = self.dse.workspace.get_metadata_file_path(self.STAT_FILE)
         data = {
@@ -631,15 +643,15 @@
         log_f = getattr(logging, mapper[level])
         log_f(message)
         self.agent.send_log(level, message)
 
     def send_seed_to_broker(self, se: SymbolicExecutor, state: ProcessState, seed: Seed):
         if seed not in self._seed_received:  # Do not send back a seed that already came from broker
             self._sending_count += 1
-            logging.info(f"Sending new: {seed.hash} [{self._sending_count}]")
+            logging.info(f"Sending new: {to_h(seed)} [{self._sending_count}]")
             bytes = seed.content.files[self.INPUT_FILE_NAME] if seed.is_composite() else seed.content
             self.agent.send_seed(SeedType.INPUT, bytes)
 
     def intrinsic_callback(self, se: SymbolicExecutor, state: ProcessState, addr: Addr):
         """
         This function is called when an intrinsic call occurs in order to verify
         defaults and vulnerabilities.
```

### Comparing `pastis-framework-1.0.4/libpastis/agent.py` & `pastis-framework-1.0.5/libpastis/agent.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/libpastis/enginedesc.py` & `pastis-framework-1.0.5/libpastis/enginedesc.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/libpastis/package.py` & `pastis-framework-1.0.5/libpastis/package.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/libpastis/proto/message_pb2.py` & `pastis-framework-1.0.5/libpastis/proto/message_pb2.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/libpastis/sast.py` & `pastis-framework-1.0.5/libpastis/sast.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/libpastis/types.py` & `pastis-framework-1.0.5/libpastis/types.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/libpastis/utils.py` & `pastis-framework-1.0.5/libpastis/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastis_framework.egg-info/PKG-INFO` & `pastis-framework-1.0.5/pastis_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.4
+Version: 1.0.5
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.4/pastis_framework.egg-info/SOURCES.txt` & `pastis-framework-1.0.5/pastis_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbenchmark/models.py` & `pastis-framework-1.0.5/pastisbenchmark/models.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbenchmark/plotter.py` & `pastis-framework-1.0.5/pastisbenchmark/plotter.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbenchmark/replayer.py` & `pastis-framework-1.0.5/pastisbenchmark/replayer.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbenchmark/results.py` & `pastis-framework-1.0.5/pastisbenchmark/results.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbroker/broker.py` & `pastis-framework-1.0.5/pastisbroker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
                  inject_loc: SeedInjectLoc = SeedInjectLoc.STDIN,
                  sast_report: PathLike = None,
                  p_argv: List[str] = None,
                  memory_threshold: int = 85,
                  start_quorum: int = 0,
                  filter_inputs: bool = False,
                  stream: bool = False,
-                 replay_threads: int = 4):
+                 replay_threads: int = 4,
+                 replay_timeout: int = 60):
         super(PastisBroker, self).__init__()
 
         # Initialize workspace
         self.workspace = Workspace(Path(workspace))
         params = {"binaries_dir": str(Path(binaries_dir).absolute()),
                   "broker_mode": broker_mode.name,
                   "check_mode": check_mode.name,
@@ -122,15 +123,15 @@
         # Coverage + filtering feature
         self._coverage_manager = None
         self.filter_inputs: bool = filter_inputs
         if filter_inputs or stream:
             if (path := self.find_vanilla_binary()) is not None:  # Find an executable suitable for coverage
                 logging.info(f"Coverage binary: {path}")
                 stream_file = self.workspace.coverage_history if stream else ""
-                self._coverage_manager = CoverageManager(replay_threads, filter_inputs, path, self.argv, self.inject, stream_file)
+                self._coverage_manager = CoverageManager(replay_threads, replay_timeout, filter_inputs, path, self.argv, self.inject, stream_file)
             else:
                 logging.warning("filtering or stream enabled but cannot find vanilla binary")
 
 
     def find_vanilla_binary(self) -> Optional[str]:
         """
         Find a binary without instrumentation to be used for coverage
@@ -581,15 +582,29 @@
         logging.info("start broking")
 
         if self._coverage_manager:  # if it has been instanciated start it
             self._coverage_manager.start()
             for seed in self._init_seed_pool.keys():  # Push initial corpus to set baseline coverage
                 fname = self.mk_input_name("INITIAL", seed)
                 sp = fname.split("_")
-                covi = ClientInput(seed, "", f"{sp[0]}_{sp[1]}", sp[2], sp[4], fname, SeedType.INPUT, b"INITIAL", "INITIAL", "GRANTED", "", -1, [])
+                hash = sp[4].split(".")[0]
+                covi = ClientInput(
+                    content=seed,
+                    log_time="",
+                    recv_time=f"{sp[0]}_{sp[1]}",
+                    elapsed=sp[2],
+                    hash=hash,
+                    path=fname,
+                    seed_status=SeedType.INPUT,
+                    fuzzer_id=b"INITIAL",
+                    fuzzer_name="INITIAL",
+                    broker_status="GRANTED",  # Unless rejected (later)
+                    replay_status="",
+                    replay_time=-1,
+                    new_coverage=[])
                 self._coverage_manager.push_input(covi)
 
         if self.is_proxied and self._proxy_cli:
             self._running = False  # disable running wait start broker
             self._proxy.send_hello([self._proxy_cli])
         else:
             # Send the start message to all clients (already connected)
@@ -617,32 +632,34 @@
                     if not self._check_memory_usage():
                         # The machine starts being overloaded
                         # For security kill triton instance
                         for cli in list(self.clients.values()):
                             if cli.engine.SHORT_NAME == "TT":  # is triton
                                 self.kick_client(cli.netid)
 
-                # if inputs are filtered. Get granted inputs and forward them to appropriate clients
-                if self.filter_inputs:
-                    for item in self._coverage_manager.iter_granted_inputs():
-                        self.seed_granted(item.fuzzer_id, item.seed_status, item.content)
-
                 # Check if we received the start signal from the proxy-master
                 if self._proxy_start_signal:
+                    logging.info("signal received start clients !")
                     self._proxy_start_signal = False
                     self.start_pending_clients()
 
-                # Check if there are seed coming from the proxy-master to forward to clients
-                if not self._proxy_seed_queue.empty():
-                    try:
-                        while True:
-                            origin, typ, seed = self._proxy_seed_queue.get_nowait()
-                            self.send_seed_to_all_others(origin, typ, seed)
-                    except queue.Empty:
-                        pass
+                if self._running: # Perform following checks only if running
+                    # if inputs are filtered. Get granted inputs and forward them to appropriate clients
+                    if self.filter_inputs:
+                        for item in self._coverage_manager.iter_granted_inputs():
+                            self.seed_granted(item.fuzzer_id, item.seed_status, item.content)
+
+                    # Check if there are seed coming from the proxy-master to forward to clients
+                    if not self._proxy_seed_queue.empty():
+                        try:
+                            while True:
+                                origin, typ, seed = self._proxy_seed_queue.get_nowait()
+                                self.send_seed_to_all_others(origin, typ, seed)
+                        except queue.Empty:
+                            pass
 
                 if self._stop:
                     logging.info("broker terminate")
                     break
         except KeyboardInterrupt:
             logging.info("stop required (Ctrl+C)")
         self.workspace.status = WorkspaceStatus.FINISHED
@@ -772,20 +789,21 @@
 
     def _proxy_start_received(self, fname: str, binary: bytes, engine: FuzzingEngineInfo, exmode: ExecMode,
                               fuzzmode: FuzzMode, chkmode: CheckMode, covmode: CoverageMode, seed_inj: SeedInjectLoc,
                               engine_args: str, argv: List[str], sast_report: str = None):
         # FIXME: Use parameters received
         logging.info("[PROXY] start received !")
         self._running = True
+        self._proxy_start_signal = True
         # if self._running:
         #     self.start_pending_clients()
 
     def _proxy_seed_received(self, typ: SeedType, seed: bytes):
         # Forward the seed to underlying clients
-        logging.info(f"[PROXY] seed {typ.name} received forward to agents")
+        logging.info(f"[PROXY] receive {md5(seed).hexdigest()} [{typ.name}] (forward it)")
 
         # Save the seed locally
         self.write_seed(typ, "PROXY", seed)
         self._seed_pool[seed] = typ  # add it to the pool
         self._init_seed_pool[seed] = typ  # also consider it as initial corpus
 
         # Forward it to all clients
```

### Comparing `pastis-framework-1.0.4/pastisbroker/client.py` & `pastis-framework-1.0.5/pastisbroker/client.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbroker/coverage.py` & `pastis-framework-1.0.5/pastisbroker/coverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import json
 import time
 import logging
 import tempfile
 import os
 import subprocess
 from typing import Generator
 from pathlib import Path
@@ -40,17 +41,18 @@
 
 
 class CoverageManager(object):
 
     ARGV_PLACEHOLDER = "@@"
     STRATEGY = CoverageStrategy.EDGE
 
-    def __init__(self, pool_size: int, filter: bool, program: str, args: list[str], inj_loc: SeedInjectLoc, stream_file: str = ""):
+    def __init__(self, pool_size: int, replay_timeout: int, filter: bool, program: str, args: list[str], inj_loc: SeedInjectLoc, stream_file: str = ""):
         # Base info for replay
         self.pool_size = pool_size
+        self.replay_timeout = replay_timeout
         self.filter_enabled = filter
         self.program = str(program)
         self.args = args
         self.inj_loc = inj_loc
 
         # Coverage and messaging attributes
         self._coverage = GlobalCoverage(self.STRATEGY, BranchSolvingStrategy.ALL_NOT_COVERED)
@@ -82,15 +84,15 @@
         """
         # First start the coverage worker
         self._running = True
         self.cov_worker.start()
         logging.info("Starting coverage manager")
 
         for work_id in range(self.pool_size):
-            self.pool.apply_async(self.worker, (self.input_queue, self.cov_queue, self.program, self.args, self.inj_loc))
+            self.pool.apply_async(self.worker, (self.input_queue, self.cov_queue, self.program, self.args, self.inj_loc, self.replay_timeout))
 
     def stop(self) -> None:
         self._running = False
         self.cov_worker.join()
         self.pool.terminate()
 
     def push_input(self, cli_input: ClientInput) -> None:
@@ -168,24 +170,29 @@
 
                     else:
                         item.broker_status = "DROPPED" if self.filter_enabled else "GRANTED"
                         # logging.info(f"seed {item.hash} ({item.seed_status.name}) of {item.fuzzer_name} rejected (do not improve coverage)")
 
                     # Remove the coverage file
                     os.unlink(cov_file)
+
+                except json.JSONDecodeError:
+                    item.replay_status = "FAIL_PARSE_COV"
+                    os.unlink(cov_file)
+                    self.seeds_accepted += 1
+                    if item.fuzzer_name != "INITIAL":  # if not initial corpus add it
+                        self.granted_queue.put(item)
+
                 except FileNotFoundError:
-                    if item.seed_status == SeedType.INPUT:
-                        logging.warning(f"seed {item.hash}({item.seed_status}) can't load coverage file (maybe had crashed?)")
-                    else:
-                        logging.info(f"seed {item.hash}({item.seed_status}) cannot get coverage (normal..)")
                     # Grant input
                     self.seeds_accepted += 1
-                    self.granted_queue.put(item)
+                    if item.fuzzer_name != "INITIAL":  # if not initial corpus add it
+                        self.granted_queue.put(item)
 
-                logging.info(f"seed {item.hash} ({item.fuzzer_name}) [replay:{self.mk_rpl_status(item.replay_status)}][status:{self.mk_broker_status(item.broker_status, bool(new_items))}] ({len(new_items)} new edges)")
+                logging.info(f"seed {item.hash} ({item.fuzzer_name}) [replay:{self.mk_rpl_status(item.replay_status)}][{self.mk_broker_status(item.broker_status, bool(new_items))}][{int(item.replay_time):}s] ({len(new_items)} new edges) (pool:{self.input_queue.qsize()})")
                 # Regardless if it was a success or not log it
                 self.add_item_coverage_stream(item)
             except queue.Empty:
                 pass
             except KeyboardInterrupt:
                 self._running = False
                 logging.info("coverage worker stop")
@@ -205,15 +212,15 @@
             return mk_color(status, Bcolors.OKGREEN if new_items else Bcolors.WARNING)
         elif status == "DROPPED":
             return mk_color(status, Bcolors.WARNING)
         else:
             return mk_color(status, Bcolors.FAIL)
 
     @staticmethod
-    def worker(input_queue: Queue, cov_queue: Queue, program: str, argv: list[str], seed_inj: SeedInjectLoc) -> None:
+    def worker(input_queue: Queue, cov_queue: Queue, program: str, argv: list[str], seed_inj: SeedInjectLoc, timeout) -> None:
         """
         worker thread that unstack inputs and replay them.
         """
         tmpfile = Path(tempfile.mktemp(suffix=f"{os.getpid()}.input"))
         pid = os.getpid()
         try:
             while True:
@@ -232,32 +239,31 @@
                         # Replace 'input_file' in argv with the temporary file name created
                         idx = cur_argv.index(CoverageManager.ARGV_PLACEHOLDER)
                         cur_argv[idx] = str(tmpfile)
                     except ValueError as e:
                         logging.error(f"seed injection {seed_inj.name} but can't find '@@' on program argv: {argv}: {e}")
                         continue
 
+                t0 = time.time()
                 try:
                     # Run the seed
-                    t0 = time.time()
                     if QBDITrace.run(CoverageManager.STRATEGY,
                                      program,
                                      cur_argv,  # argv[1:] if len(argv) > 1 else [],
                                      output_path=str(cov_file),
                                      stdin_file=str(tmpfile) if seed_inj == SeedInjectLoc.STDIN else None,
                                      cwd=Path(program).parent,
-                                     timeout=60):
-                        item.replay_time = time.time() - t0
+                                     timeout=timeout):
                         item.replay_status = "SUCCESS"
                         # logging.info(f"[worker-{pid}] replaying {item.hash} sucessful")
                     else:
                         item.replay_status = "FAIL_NO_COV"
-                        logging.warning("Cannot load the coverage file generated (maybe had crashed?)")
+                        # logging.warning("Cannot load the coverage file generated (maybe had crashed?)")
                 except TraceException:
                     item.replay_status = "FAIL_TIMEOUT"
-                    logging.warning('Timeout hit, while trying to re-run the seed')
-
+                    # logging.warning('Timeout hit, while trying to re-run the seed')
+                item.replay_time = time.time() - t0
                 # Add it to the coverage queue (even if it failed
                 cov_queue.put((item, cov_file))
         except KeyboardInterrupt:
             pass
             # logging.info(f"replay worker {os.getpid()}, stops (keyboard interrupt)")
```

### Comparing `pastis-framework-1.0.4/pastisbroker/stat_manager.py` & `pastis-framework-1.0.5/pastisbroker/stat_manager.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbroker/utils.py` & `pastis-framework-1.0.5/pastisbroker/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/pastisbroker/workspace.py` & `pastis-framework-1.0.5/pastisbroker/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.4/setup.py` & `pastis-framework-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md") as f:
     lines = f.readlines()
     README = "\n".join(lines[4:7]+lines[51:])
 
 
 setup(
     name="pastis-framework",
-    version="1.0.4",
+    version="1.0.5",
     description="PASTIS framework for collaborative fuzzing",
     long_description=README,
     long_description_content_type='text/markdown',
     packages=[
         "libpastis",
         "libpastis.proto",
         "pastisbroker",
```

