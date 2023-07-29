# Comparing `tmp/yascheduler-1.0.9.tar.gz` & `tmp/yascheduler-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yascheduler-1.0.9.tar", last modified: Mon Apr 24 19:43:08 2023, max compression
+gzip compressed data, was "yascheduler-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yascheduler-1.0.9.tar` & `yascheduler-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.812351 yascheduler-1.0.9/
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-24 19:43:01.000000 yascheduler-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-24 19:43:08.812351 yascheduler-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10424 2023-03-08 16:11:57.000000 yascheduler-1.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-24 19:43:08.812351 yascheduler-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1576 2022-07-30 22:43:35.000000 yascheduler-1.0.9/setup.json
--rw-r--r--   0 root         (0) root         (0)     1972 2022-08-17 12:59:28.000000 yascheduler-1.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/
--rw-r--r--   0 root         (0) root         (0)      228 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-24 19:38:14.000000 yascheduler-1.0.9/yascheduler/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4747 2022-09-26 15:10:05.000000 yascheduler-1.0.9/yascheduler/aiida_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-08-01 14:38:59.000000 yascheduler-1.0.9/yascheduler/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/clouds/
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/clouds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2981 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/adapters.py
--rw-r--r--   0 root         (0) root         (0)     8736 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/az.py
--rw-r--r--   0 root         (0) root         (0)     6867 2022-08-16 14:53:47.000000 yascheduler-1.0.9/yascheduler/clouds/cloud_api.py
--rw-r--r--   0 root         (0) root         (0)     6821 2022-08-16 14:53:47.000000 yascheduler-1.0.9/yascheduler/clouds/cloud_api_manager.py
--rw-r--r--   0 root         (0) root         (0)     3282 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/hetzner.py
--rw-r--r--   0 root         (0) root         (0)     5802 2022-08-16 14:53:47.000000 yascheduler-1.0.9/yascheduler/clouds/protocols.py
--rw-r--r--   0 root         (0) root         (0)     2831 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/upcloud.py
--rw-r--r--   0 root         (0) root         (0)      763 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/config/
--rw-r--r--   0 root         (0) root         (0)      731 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6408 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/config/cloud.py
--rw-r--r--   0 root         (0) root         (0)     2438 2022-08-17 12:59:28.000000 yascheduler-1.0.9/yascheduler/config/config.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/db.py
--rw-r--r--   0 root         (0) root         (0)     4917 2022-08-01 15:25:53.000000 yascheduler-1.0.9/yascheduler/config/engine.py
--rw-r--r--   0 root         (0) root         (0)     2635 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/engine_repository.py
--rw-r--r--   0 root         (0) root         (0)     2844 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/config/local.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/remote.py
--rw-r--r--   0 root         (0) root         (0)      484 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/utils.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-30 22:43:26.000000 yascheduler-1.0.9/yascheduler/daemon_systemd.py
--rw-r--r--   0 root         (0) root         (0)      864 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/daemon_sysv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/data/
--rw-r--r--   0 root         (0) root         (0)      360 2023-02-09 18:58:39.000000 yascheduler-1.0.9/yascheduler/data/schema.sql
--rw-r--r--   0 root         (0) root         (0)     1493 2022-07-30 22:43:26.000000 yascheduler-1.0.9/yascheduler/data/yascheduler.conf
--rw-r--r--   0 root         (0) root         (0)      664 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/data/yascheduler.service
--rwxr-xr-x   0 root         (0) root         (0)     1832 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/data/yascheduler.sh
--rw-r--r--   0 root         (0) root         (0)    12108 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/db.py
--rw-r--r--   0 root         (0) root         (0)     1651 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.812351 yascheduler-1.0.9/yascheduler/remote_machine/
--rw-r--r--   0 root         (0) root         (0)      417 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/remote_machine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3271 2022-08-17 12:59:28.000000 yascheduler-1.0.9/yascheduler/remote_machine/adapters.py
--rw-r--r--   0 root         (0) root         (0)     2338 2022-08-17 12:59:28.000000 yascheduler-1.0.9/yascheduler/remote_machine/checks.py
--rw-r--r--   0 root         (0) root         (0)     1213 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/remote_machine/common.py
--rw-r--r--   0 root         (0) root         (0)       72 2022-07-30 22:43:26.000000 yascheduler-1.0.9/yascheduler/remote_machine/exc.py
--rw-r--r--   0 root         (0) root         (0)     6980 2022-08-03 22:43:25.000000 yascheduler-1.0.9/yascheduler/remote_machine/linux_methods.py
--rw-r--r--   0 root         (0) root         (0)     8641 2022-08-16 21:24:49.000000 yascheduler-1.0.9/yascheduler/remote_machine/protocol.py
--rw-r--r--   0 root         (0) root         (0)    13207 2023-03-10 23:58:05.000000 yascheduler-1.0.9/yascheduler/remote_machine/remote_machine.py
--rw-r--r--   0 root         (0) root         (0)     2655 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/remote_machine/remote_machine_repository.py
--rw-r--r--   0 root         (0) root         (0)     7288 2022-08-03 22:43:25.000000 yascheduler-1.0.9/yascheduler/remote_machine/windows_methods.py
--rwxr-xr-x   0 root         (0) root         (0)    26345 2023-03-10 23:59:11.000000 yascheduler-1.0.9/yascheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)      435 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/time.py
--rw-r--r--   0 root         (0) root         (0)    15688 2023-03-08 16:11:57.000000 yascheduler-1.0.9/yascheduler/utils.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      235 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/top_level.txt
+-rw-r--r--   0        0        0      415 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.flake8
+-rw-r--r--   0        0        0     1254 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.github/workflows/linter.yml
+-rw-r--r--   0        0        0      728 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1940 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.github/workflows/push.yml
+-rw-r--r--   0        0        0      905 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1892 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.gitignore
+-rw-r--r--   0        0        0       55 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     2056 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      139 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.whitesource
+-rw-r--r--   0        0        0       46 2023-07-29 13:27:07.195994 yascheduler-1.2.0/.yamllint.yaml
+-rw-r--r--   0        0        0     3168 2023-07-29 13:27:07.195994 yascheduler-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      652 2023-07-29 13:27:07.195994 yascheduler-1.2.0/CITATION.cff
+-rw-r--r--   0        0        0     3000 2023-07-29 13:27:07.195994 yascheduler-1.2.0/CLOUD.md
+-rw-r--r--   0        0        0     1083 2023-07-29 13:27:07.195994 yascheduler-1.2.0/LICENSE
+-rw-r--r--   0        0        0    10479 2023-07-29 13:27:07.195994 yascheduler-1.2.0/README.md
+-rw-r--r--   0        0        0     2936 2023-07-29 13:27:07.195994 yascheduler-1.2.0/WINDOWS.md
+-rw-r--r--   0        0        0     4375 2023-07-29 13:27:07.199994 yascheduler-1.2.0/data/CRYSTAL-benchmark/INPUT
+-rw-r--r--   0        0        0      468 2023-07-29 13:27:07.199994 yascheduler-1.2.0/examples/submit_dummy_input.py
+-rw-r--r--   0        0        0      933 2023-07-29 13:27:07.199994 yascheduler-1.2.0/examples/submit_gulp_input.py
+-rwxr-xr-x   0        0        0     1229 2023-07-29 13:27:07.199994 yascheduler-1.2.0/examples/submit_pcrystal_input.py
+-rw-r--r--   0        0        0      792 2023-07-29 13:27:07.199994 yascheduler-1.2.0/examples/submit_topas_input.py
+-rw-r--r--   0        0        0     3448 2023-07-29 13:27:07.199994 yascheduler-1.2.0/initialize.ps1
+-rw-r--r--   0        0        0      406 2023-07-29 13:27:07.199994 yascheduler-1.2.0/jumper.sh
+-rw-r--r--   0        0        0     3713 2023-07-29 13:27:07.199994 yascheduler-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5961 2023-07-29 13:27:07.199994 yascheduler-1.2.0/read_ini.sh
+-rwxr-xr-x   0        0        0     1574 2023-07-29 13:27:07.199994 yascheduler-1.2.0/setup_nodes.sh
+-rwxr-xr-x   0        0        0      457 2023-07-29 13:27:07.199994 yascheduler-1.2.0/warmup_nodes.sh
+-rw-r--r--   0        0        0      213 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/__init__.py
+-rw-r--r--   0        0        0     4907 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/aiida_plugin.py
+-rw-r--r--   0        0        0     2679 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/client.py
+-rw-r--r--   0        0        0      170 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/__init__.py
+-rw-r--r--   0        0        0     2979 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/adapters.py
+-rw-r--r--   0        0        0     8736 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/az.py
+-rw-r--r--   0        0        0     6867 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/cloud_api.py
+-rw-r--r--   0        0        0     6821 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/cloud_api_manager.py
+-rw-r--r--   0        0        0     3280 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/hetzner.py
+-rw-r--r--   0        0        0     5802 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/protocols.py
+-rw-r--r--   0        0        0     2831 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/upcloud.py
+-rw-r--r--   0        0        0      763 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/clouds/utils.py
+-rw-r--r--   0        0        0      731 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/__init__.py
+-rw-r--r--   0        0        0     8543 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/cloud.py
+-rw-r--r--   0        0        0     2438 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/config.py
+-rw-r--r--   0        0        0     1106 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/db.py
+-rw-r--r--   0        0        0     5448 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/engine.py
+-rw-r--r--   0        0        0     2635 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/engine_repository.py
+-rw-r--r--   0        0        0     3123 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/local.py
+-rw-r--r--   0        0        0     1575 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/remote.py
+-rw-r--r--   0        0        0      912 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/config/utils.py
+-rw-r--r--   0        0        0      200 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/daemon_systemd.py
+-rw-r--r--   0        0        0      864 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/daemon_sysv.py
+-rw-r--r--   0        0        0      360 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/data/schema.sql
+-rw-r--r--   0        0        0     1493 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/data/yascheduler.conf
+-rw-r--r--   0        0        0      664 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/data/yascheduler.service
+-rwxr-xr-x   0        0        0     1832 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/data/yascheduler.sh
+-rw-r--r--   0        0        0    12108 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/db.py
+-rw-r--r--   0        0        0     1651 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/queue.py
+-rw-r--r--   0        0        0      417 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/__init__.py
+-rw-r--r--   0        0        0     4034 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/adapters.py
+-rw-r--r--   0        0        0     2868 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/checks.py
+-rw-r--r--   0        0        0     1213 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/common.py
+-rw-r--r--   0        0        0       72 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/exc.py
+-rw-r--r--   0        0        0     6980 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/linux_methods.py
+-rw-r--r--   0        0        0     8641 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/protocol.py
+-rw-r--r--   0        0        0    13614 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/remote_machine.py
+-rw-r--r--   0        0        0     2663 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/remote_machine_repository.py
+-rw-r--r--   0        0        0     7288 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/remote_machine/windows_methods.py
+-rwxr-xr-x   0        0        0    26437 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/scheduler.py
+-rw-r--r--   0        0        0      435 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/time.py
+-rw-r--r--   0        0        0    16072 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/utils.py
+-rw-r--r--   0        0        0      263 2023-07-29 13:27:07.199994 yascheduler-1.2.0/yascheduler/variables.py
+-rw-r--r--   0        0        0    12735 1970-01-01 00:00:00.000000 yascheduler-1.2.0/PKG-INFO
```

### Comparing `yascheduler-1.0.9/README.md` & `yascheduler-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -448,14 +448,15 @@
 
   _Default_: `10`
 
 - `input_files`
 
   A list of task input file names, separated by a space or new line,
   that will be copied to the remote directory of the task before it is started.
+  The first input is considered as the **main** input.
 
   _Example_: `INPUT sibling.file`
 
 - `output_files`
 
   A list of task output file names, separated by a space or new line,
   that will be copied from the remote directory of the task after it is finished.
```

### Comparing `yascheduler-1.0.9/yascheduler/aiida_plugin.py` & `yascheduler-1.2.0/yascheduler/aiida_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Aiida plugin for yascheduler,
 with respect to the supported yascheduler engines
 """
 
-import aiida.schedulers
-from aiida.orm import load_node
+import aiida.schedulers  # pylint: disable=import-error
+from aiida.orm import load_node  # pylint: disable=import-error
+
+# pylint: disable=import-error
 from aiida.schedulers.datastructures import JobInfo, JobState, NodeNumberJobResource
 
 _MAP_STATUS_YASCHEDULER = {
     "TO_DO": JobState.QUEUED,
     "RUNNING": JobState.RUNNING,
     "DONE": JobState.DONE,
 }
@@ -35,14 +37,16 @@
     # The class to be used for the job resource.
     _job_resource_class = YaschedJobResource
 
     def _get_joblist_command(self, jobs=None, user=None):
         """
         The command to report full information on existing jobs.
         """
+
+        # pylint: disable=import-error
         from aiida.common.exceptions import FeatureNotAvailable
 
         if user:
             raise FeatureNotAvailable("Cannot query by user in Yascheduler")
         command = [f"{_CMD_PREFIX}yastatus"]
         # make list from job ids (taken from slurm scheduler)
         if jobs:
@@ -75,16 +79,18 @@
         pk = int(job_tmpl.job_name.split("-")[1])
         aiida_node = load_node(pk)
 
         # We map the lowercase code labels onto yascheduler engines,
         # so that the required input file(s) can be deduced
         lines = [f"ENGINE={aiida_node.inputs.code.label.lower()}"]
 
-        try: lines.append(f"PARENT={aiida_node.caller.uuid}")
-        except AttributeError: pass
+        try:
+            lines.append(f"PARENT={aiida_node.caller.uuid}")
+        except AttributeError:
+            pass
 
         lines.append(f"LABEL={job_tmpl.job_name}")
         return "\n".join(lines)
 
     def _get_submit_command(self, submit_script):
         """
         Return the string to execute to submit a given script.
```

### Comparing `yascheduler-1.0.9/yascheduler/client.py` & `yascheduler-1.2.0/yascheduler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Yascheduler client"""
 
 import asyncio
 import logging
 from pathlib import PurePath
-from typing import Any, Mapping, MutableMapping, Optional, Sequence, Union
+from typing import Any, Mapping, Optional, Sequence, Union
 
 from attrs import asdict
 
 from .config import Config
 from .db import DB, TaskModel, TaskStatus
 from .scheduler import Scheduler
 from .variables import CONFIG_FILE
```

### Comparing `yascheduler-1.0.9/yascheduler/clouds/adapters.py` & `yascheduler-1.2.0/yascheduler/clouds/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             create_node=create_node,
             create_node_conn_timeout=create_node_conn_timeout,
             create_node_timeout=create_node_timeout,
             delete_node=delete_node,
             op_limit=op_limit,
         )
 
-    @lru_cache()  # noqa: B019
+    @lru_cache  # noqa: B019
     def get_op_semaphore(self) -> asyncio.Semaphore:
         return asyncio.Semaphore(self.op_limit)
 
 
 azure_adapter = CloudAdapter.create(
     name="az",
     supported_platform_checks=[can_debian_bullseye, can_win11],
```

### Comparing `yascheduler-1.0.9/yascheduler/clouds/az.py` & `yascheduler-1.2.0/yascheduler/clouds/az.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/clouds/cloud_api.py` & `yascheduler-1.2.0/yascheduler/clouds/cloud_api.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/clouds/cloud_api_manager.py` & `yascheduler-1.2.0/yascheduler/clouds/cloud_api_manager.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/clouds/hetzner.py` & `yascheduler-1.2.0/yascheduler/clouds/hetzner.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 @lru_cache(maxsize=None)
 def get_client(cfg: ConfigCloudHetzner) -> HClient:
     "Get Hetzner client"
     return HClient(cfg.token)
 
 
-@lru_cache()
+@lru_cache
 def get_ssh_key_id(client: HClient, key: ASSHKey) -> int:
     "Get Hetzner ssh id"
     key_name = get_key_name(key)
     pub_key = key.export_public_key("openssh").decode("utf-8")
 
     try:
         return client.ssh_keys.create(name=key_name, public_key=pub_key).id
```

### Comparing `yascheduler-1.0.9/yascheduler/clouds/protocols.py` & `yascheduler-1.2.0/yascheduler/clouds/protocols.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/clouds/upcloud.py` & `yascheduler-1.2.0/yascheduler/clouds/upcloud.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/clouds/utils.py` & `yascheduler-1.2.0/yascheduler/clouds/utils.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/config/__init__.py` & `yascheduler-1.2.0/yascheduler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/config/cloud.py` & `yascheduler-1.2.0/yascheduler/config/cloud.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 """Cloud configurations"""
 
 from configparser import SectionProxy
 from functools import partial
-from typing import Optional, Union
+from typing import Optional, Sequence, Union
 
-from attrs import define, field, validators
+from attrs import define, field, fields, validators
 from typing_extensions import Self
 
-from .utils import _make_default_field, opt_str_val
+from .utils import _make_default_field, opt_str_val, warn_unknown_fields
 
 
 def _check_az_user(_: "ConfigCloudAzure", __, value: str):
     if value == "root":
         raise ValueError("Root user is forbidden on Azure")
 
 
@@ -63,19 +63,39 @@
     )
     priority: int = _make_default_field(0)
     idle_tolerance: int = _make_default_field(300, extra_validators=[validators.ge(1)])
     jump_username: Optional[str] = field(default=None, validator=opt_str_val)
     jump_host: Optional[str] = field(default=None, validator=opt_str_val)
 
     @classmethod
+    def get_valid_config_parser_fields(cls) -> Sequence[str]:
+        "Returns a list of valid config keys"
+        exclude_names = ["prefix", "username", "jump_username", "vm_image", "vm_size"]
+        include_names = ["user", "jump_user", "image", "size"]
+        return [
+            f"{cls.prefix}_{x}"
+            for x in [f.name for f in fields(cls) if f.name not in exclude_names]
+            + include_names
+        ]
+
+    @classmethod
     def from_config_parser_section(cls, sec: SectionProxy) -> "ConfigCloudAzure":
         "Create config from config parser's section"
 
         fmt = partial(_fmt_key, cls.prefix)
 
+        warn_unknown_fields(
+            [
+                *cls.get_valid_config_parser_fields(),
+                *ConfigCloudHetzner.get_valid_config_parser_fields(),
+                *ConfigCloudUpcloud.get_valid_config_parser_fields(),
+            ],
+            sec,
+        )
+
         vm_image = sec.get(fmt("image"))
         image_ref = None
         if vm_image:
             image_ref = AzureImageReference.from_urn(vm_image)
 
         return cls(
             tenant_id=sec.get(fmt("tenant_id")),
@@ -110,17 +130,38 @@
     server_type: str = _make_default_field("cx51")
     image_name: str = _make_default_field("debian-10")
     idle_tolerance: int = _make_default_field(120, extra_validators=[validators.ge(1)])
     jump_username: Optional[str] = field(default=None, validator=opt_str_val)
     jump_host: Optional[str] = field(default=None, validator=opt_str_val)
 
     @classmethod
+    def get_valid_config_parser_fields(cls) -> Sequence[str]:
+        "Returns a list of valid config keys"
+        exclude_names = ["prefix", "username", "jump_username"]
+        include_names = ["user", "jump_user"]
+        return [
+            f"{cls.prefix}_{x}"
+            for x in [f.name for f in fields(cls) if f.name not in exclude_names]
+            + include_names
+        ]
+
+    @classmethod
     def from_config_parser_section(cls, sec: SectionProxy) -> "ConfigCloudHetzner":
         "Create config from config parser's section"
         fmt = partial(_fmt_key, cls.prefix)
+
+        warn_unknown_fields(
+            [
+                *ConfigCloudAzure.get_valid_config_parser_fields(),
+                *cls.get_valid_config_parser_fields(),
+                *ConfigCloudUpcloud.get_valid_config_parser_fields(),
+            ],
+            sec,
+        )
+
         return cls(
             token=sec.get(fmt("token")),
             max_nodes=sec.getint(fmt("max_nodes")),
             username=sec.get(fmt("user")),
             server_type=sec.get(fmt("server_type")),
             image_name=sec.get(fmt("image_name")),
             priority=sec.getint(fmt("priority")),
@@ -141,17 +182,38 @@
     username: str = _make_default_field("root")
     priority: int = _make_default_field(0)
     idle_tolerance: int = _make_default_field(120, extra_validators=[validators.ge(1)])
     jump_username: Optional[str] = field(default=None, validator=opt_str_val)
     jump_host: Optional[str] = field(default=None, validator=opt_str_val)
 
     @classmethod
+    def get_valid_config_parser_fields(cls) -> Sequence[str]:
+        "Returns a list of valid config keys"
+        exclude_names = ["prefix", "username", "jump_username"]
+        include_names = ["user", "jump_user"]
+        return [
+            f"{cls.prefix}_{x}"
+            for x in [f.name for f in fields(cls) if f.name not in exclude_names]
+            + include_names
+        ]
+
+    @classmethod
     def from_config_parser_section(cls, sec: SectionProxy) -> "ConfigCloudUpcloud":
         "Create config from config parser's section"
         fmt = partial(_fmt_key, cls.prefix)
+
+        warn_unknown_fields(
+            [
+                *ConfigCloudAzure.get_valid_config_parser_fields(),
+                *ConfigCloudHetzner.get_valid_config_parser_fields(),
+                *cls.get_valid_config_parser_fields(),
+            ],
+            sec,
+        )
+
         return cls(
             login=sec.get(fmt("login")),
             password=sec.get(fmt("password")),
             max_nodes=sec.getint(fmt("max_nodes")),
             username=sec.get(fmt("user")),
             priority=sec.getint(fmt("priority")),
             idle_tolerance=sec.getint(fmt("idle_tolerance")),
```

### Comparing `yascheduler-1.0.9/yascheduler/config/config.py` & `yascheduler-1.2.0/yascheduler/config/config.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/config/engine.py` & `yascheduler-1.2.0/yascheduler/config/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 """Engine configuration"""
 
 from configparser import SectionProxy
 from pathlib import PurePath
 from typing import Optional, Sequence, Tuple, Union
 
-from attrs import Attribute, define, field, validators
+from attrs import Attribute, define, field, fields, validators
 
-from .utils import _make_default_field
+from .utils import _make_default_field, warn_unknown_fields
 
 
 def _check_spawn(instance: "Engine", _, value: str):
     try:
         value.format(task_path="", engine_path="", ncpus="")
     except KeyError as err:
         msg = (
@@ -105,19 +105,34 @@
             validators.deep_iterable(member_validator=validators.instance_of(str))
         ],
     )
     check_cmd_code: int = _make_default_field(0)
     sleep_interval: int = _make_default_field(10)
 
     @classmethod
+    def get_valid_config_parser_fields(cls) -> Sequence[str]:
+        "Returns a list of valid config keys"
+        exclude_names = ["name", "deployable"]
+        include_names = [
+            "deploy_local_files",
+            "deploy_local_archive",
+            "deploy_remote_archive",
+        ]
+        return [
+            f.name for f in fields(cls) if f.name not in exclude_names
+        ] + include_names
+
+    @classmethod
     def from_config_parser_section(
         cls, sec: SectionProxy, engines_dir: PurePath
     ) -> "Engine":
         "Create config from config parser's section"
 
+        warn_unknown_fields(cls.get_valid_config_parser_fields(), sec)
+
         def gettuple(key: str) -> Tuple[str]:
             return tuple(
                 x.strip() for x in filter(None, sec.get(key, fallback="").split())
             )
 
         name = sec.name[7:]
         engine_dir = engines_dir / name
```

### Comparing `yascheduler-1.0.9/yascheduler/config/engine_repository.py` & `yascheduler-1.2.0/yascheduler/config/engine_repository.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/config/local.py` & `yascheduler-1.2.0/yascheduler/config/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 """Local configuration"""
 
 from configparser import SectionProxy
 from pathlib import Path, PurePath
 from typing import Optional, Sequence
 
-from attrs import define, field, validators
+from attrs import define, field, fields, validators
 
-from .utils import _make_default_field
+from .utils import _make_default_field, warn_unknown_fields
 
 
 @define(frozen=True)
 class ConfigLocal:
     """Local configuration"""
 
     data_dir: Path = _make_default_field(Path("./data"))
@@ -35,20 +35,28 @@
     deallocate_limit: int = _make_default_field(5, extra_validators=[validators.ge(1)])
     deallocate_pending: int = _make_default_field(
         1, extra_validators=[validators.ge(1)]
     )
 
     def get_private_keys(self) -> Sequence[PurePath]:
         "List private key file paths"
-        filepaths = filter(lambda x: x.is_file(), self.keys_dir.iterdir())
+        filepaths = filter(lambda x: x.is_file(), Path(self.keys_dir).iterdir())
         return list(filepaths)
 
     @classmethod
+    def get_valid_config_parser_fields(cls) -> Sequence[str]:
+        "Returns a list of valid config keys"
+        return [f.name for f in fields(cls)]
+
+    @classmethod
     def from_config_parser_section(cls, sec: SectionProxy) -> "ConfigLocal":
         "Create config from config parser's section"
+
+        warn_unknown_fields(cls.get_valid_config_parser_fields(), sec)
+
         data_dir = Path(sec.get("data_dir", "./data")).resolve()
         return ConfigLocal(
             data_dir,
             tasks_dir=Path(sec.get("tasks_dir", str(data_dir / "tasks"))).resolve(),
             engines_dir=Path(
                 sec.get("engines_dir", str(data_dir / "engines"))
             ).resolve(),
```

### Comparing `yascheduler-1.0.9/yascheduler/daemon_sysv.py` & `yascheduler-1.2.0/yascheduler/daemon_sysv.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/data/yascheduler.conf` & `yascheduler-1.2.0/yascheduler/data/yascheduler.conf`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/data/yascheduler.service` & `yascheduler-1.2.0/yascheduler/data/yascheduler.service`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/data/yascheduler.sh` & `yascheduler-1.2.0/yascheduler/data/yascheduler.sh`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/db.py` & `yascheduler-1.2.0/yascheduler/db.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/queue.py` & `yascheduler-1.2.0/yascheduler/queue.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/adapters.py` & `yascheduler-1.2.0/yascheduler/remote_machine/adapters.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,23 +4,28 @@
 from pathlib import PurePath, PurePosixPath
 from typing import Sequence, Type
 
 from attrs import define, evolve, field
 
 from .checks import (
     check_is_debian,
-    check_is_debian_bullseye,
-    check_is_debian_buster,
+    check_is_debian_10,
+    check_is_debian_11,
+    check_is_debian_12,
+    check_is_debian_13,
+    check_is_debian_14,
+    check_is_debian_15,
     check_is_debian_like,
     check_is_linux,
     check_is_windows,
     check_is_windows7,
     check_is_windows8,
     check_is_windows10,
     check_is_windows11,
+    check_is_windows12,
 )
 from .common import run, run_bg
 from .linux_methods import (
     linux_get_cpu_cores,
     linux_list_processes,
     linux_pgrep,
     linux_setup_deb_node,
@@ -86,24 +91,48 @@
 
 debian_adapter = evolve(
     debian_like_adapter,
     platform="debian",
     checks=(*debian_like_adapter.checks, check_is_debian),
 )
 
-debian_buster_adapter = evolve(
+debian_10_adapter = evolve(
     debian_adapter,
     platform="debian-10",
-    checks=(*debian_adapter.checks, check_is_debian_buster),
+    checks=(*debian_adapter.checks, check_is_debian_10),
 )
 
-debian_bullseye_adapter = evolve(
+debian_11_adapter = evolve(
     debian_adapter,
     platform="debian-11",
-    checks=(*debian_adapter.checks, check_is_debian_bullseye),
+    checks=(*debian_adapter.checks, check_is_debian_11),
+)
+
+debian_12_adapter = evolve(
+    debian_adapter,
+    platform="debian-12",
+    checks=(*debian_adapter.checks, check_is_debian_12),
+)
+
+debian_13_adapter = evolve(
+    debian_adapter,
+    platform="debian-13",
+    checks=(*debian_adapter.checks, check_is_debian_13),
+)
+
+debian_14_adapter = evolve(
+    debian_adapter,
+    platform="debian-14",
+    checks=(*debian_adapter.checks, check_is_debian_14),
+)
+
+debian_15_adapter = evolve(
+    debian_adapter,
+    platform="debian-15",
+    checks=(*debian_adapter.checks, check_is_debian_15),
 )
 
 windows_adapter = RemoteMachineAdapter(
     platform="windows",
     path=MyPureWindowsPath,
     quote=windows_quote,
     run=run,
@@ -134,7 +163,13 @@
 )
 
 windows11_adapter = evolve(
     windows_adapter,
     platform="windows-11",
     checks=(*windows_adapter.checks, check_is_windows11),
 )
+
+windows12_adapter = evolve(
+    windows_adapter,
+    platform="windows-12",
+    checks=(*windows_adapter.checks, check_is_windows12),
+)
```

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/checks.py` & `yascheduler-1.2.0/yascheduler/remote_machine/checks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,83 @@
-#!/usr/bin/env python3
+"OS checks"
 
+from functools import partial
 from typing import Optional, Tuple
 
 from asyncssh.connection import SSHClientConnection
 from asyncstdlib import lru_cache
 
 
 @lru_cache
 async def check_is_linux(conn: SSHClientConnection) -> bool:
-    r = await conn.run("uname")
-    return r.returncode == 0 and r.stdout is not None and r.stdout.strip() == "Linux"
+    "Check for generic Linux"
+    proc = await conn.run("uname")
+    return (
+        proc.returncode == 0
+        and proc.stdout is not None
+        and proc.stdout.strip() == "Linux"
+    )
 
 
 @lru_cache
 async def _get_os_release(conn: SSHClientConnection) -> Optional[Tuple[str, str, str]]:
-    r = await conn.run("source /etc/os-release; echo $ID@@@$ID_LIKE@@@$VERSION_ID")
-    if r.returncode != 0 or not r.stdout:
+    "Get os release string on linuxes"
+    proc = await conn.run("source /etc/os-release; echo $ID@@@$ID_LIKE@@@$VERSION_ID")
+    if proc.returncode != 0 or not proc.stdout:
         return None
-    return tuple(map(lambda x: x.strip(), str(r.stdout).split("@@@", maxsplit=3)))
+    return tuple(map(lambda x: x.strip(), str(proc.stdout).split("@@@", maxsplit=3)))
 
 
 async def check_is_debian_like(conn: SSHClientConnection) -> bool:
+    "Check for any Debian-like"
     os_release = await _get_os_release(conn)
     return "debian" in [os_release[0], os_release[1]] if os_release else False
 
 
 async def check_is_debian(conn: SSHClientConnection) -> bool:
+    "Check for any Debian"
     os_release = await _get_os_release(conn)
     return os_release[0] == "debian" if os_release else False
 
 
-async def check_is_debian_buster(conn: SSHClientConnection) -> bool:
+async def _check_debian_version(version: str, conn: SSHClientConnection) -> bool:
+    "Check for Debian version"
     os_release = await _get_os_release(conn)
-    return os_release[2] == "10" if os_release else False
+    return os_release[2] == version if os_release else False
 
 
-async def check_is_debian_bullseye(conn: SSHClientConnection) -> bool:
-    os_release = await _get_os_release(conn)
-    return os_release[2] == "11" if os_release else False
+check_is_debian_10 = partial(_check_debian_version, "10")
+check_is_debian_11 = partial(_check_debian_version, "11")
+check_is_debian_12 = partial(_check_debian_version, "12")
+check_is_debian_13 = partial(_check_debian_version, "13")
+check_is_debian_14 = partial(_check_debian_version, "14")
+check_is_debian_15 = partial(_check_debian_version, "15")
 
 
 @lru_cache
 async def check_is_windows(conn: SSHClientConnection) -> bool:
-    r = await conn.run("[environment]::OSVersion")
-    return r.returncode == 0
+    "Check for any Windows with Powershell"
+    proc = await conn.run("[environment]::OSVersion")
+    return proc.returncode == 0
 
 
 @lru_cache
 async def get_wmi_w32_os_caption(conn: SSHClientConnection) -> Optional[str]:
-    r = await conn.run("(Get-WmiObject -class Win32_OperatingSystem).Caption")
-    if r.stdout:
-        return str(r.stdout)
-
-
-async def check_is_windows7(conn: SSHClientConnection) -> bool:
-    c = await get_wmi_w32_os_caption(conn)
-    return "7" in c if c else False
-
-
-async def check_is_windows8(conn: SSHClientConnection) -> bool:
-    c = await get_wmi_w32_os_caption(conn)
-    return "8" in c if c else False
-
-
-async def check_is_windows10(conn: SSHClientConnection) -> bool:
-    c = await get_wmi_w32_os_caption(conn)
-    return "10" in c if c else False
-
-
-async def check_is_windows11(conn: SSHClientConnection) -> bool:
-    c = await get_wmi_w32_os_caption(conn)
-    return "11" in c if c else False
+    "Get OS caption from WMI object"
+    proc = await conn.run("(Get-WmiObject -class Win32_OperatingSystem).Caption")
+    if proc.stdout:
+        return str(proc.stdout)
+
+
+async def _check_is_windows_caption_version(
+    version: str, conn: SSHClientConnection
+) -> bool:
+    "Check for Windows version in caption"
+    caption = await get_wmi_w32_os_caption(conn)
+    return version in caption if caption else False
+
+
+check_is_windows7 = partial(_check_is_windows_caption_version, "7")
+check_is_windows8 = partial(_check_is_windows_caption_version, "8")
+check_is_windows10 = partial(_check_is_windows_caption_version, "10")
+check_is_windows11 = partial(_check_is_windows_caption_version, "11")
+check_is_windows12 = partial(_check_is_windows_caption_version, "12")
```

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/common.py` & `yascheduler-1.2.0/yascheduler/remote_machine/common.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/linux_methods.py` & `yascheduler-1.2.0/yascheduler/remote_machine/linux_methods.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/protocol.py` & `yascheduler-1.2.0/yascheduler/remote_machine/protocol.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/remote_machine.py` & `yascheduler-1.2.0/yascheduler/remote_machine/remote_machine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+"Remote machine"
 
 import asyncio
 import logging
 from asyncio.locks import Event, Semaphore
 from contextlib import asynccontextmanager
 from datetime import datetime, timedelta
 from functools import partial
@@ -18,23 +18,28 @@
 from asyncssh.sftp import SFTPClient
 from asyncstdlib import all as aall
 from asyncstdlib import map as amap
 from attrs import define, field, validators
 from typing_extensions import Self
 
 from .adapters import (
+    debian_10_adapter,
+    debian_11_adapter,
+    debian_12_adapter,
+    debian_13_adapter,
+    debian_14_adapter,
+    debian_15_adapter,
     debian_adapter,
-    debian_bullseye_adapter,
-    debian_buster_adapter,
     debian_like_adapter,
     linux_adapter,
     windows7_adapter,
     windows8_adapter,
     windows10_adapter,
     windows11_adapter,
+    windows12_adapter,
     windows_adapter,
 )
 from .exc import PlatformGuessFailed
 from .protocol import (
     AllSSHRetryExc,
     PEngine,
     PEngineRepository,
@@ -43,23 +48,28 @@
     PRemoteMachineAdapter,
     PRemoteMachineMetadata,
     SSHCheck,
     SSHRetryExc,
 )
 
 ADAPTERS: Sequence[PRemoteMachineAdapter] = [
-    debian_bullseye_adapter,
-    debian_buster_adapter,
+    debian_10_adapter,
+    debian_11_adapter,
+    debian_12_adapter,
+    debian_13_adapter,
+    debian_14_adapter,
+    debian_15_adapter,
     debian_adapter,
     debian_like_adapter,
     linux_adapter,
-    windows11_adapter,
     windows10_adapter,
-    windows8_adapter,
+    windows11_adapter,
+    windows12_adapter,
     windows7_adapter,
+    windows8_adapter,
     windows_adapter,
 ]
 
 # default value of MaxSessions on OpenSSH server is 10
 MAX_SESSIONS = 10
 
 my_backoff_exc = partial(
@@ -204,15 +214,15 @@
 
         adapter = None
         platforms: Sequence[str] = []
         checks: Sequence[bool] = [
             await aall(amap(lambda y: with_limit(conn, y), x.checks)) for x in ADAPTERS
         ]
 
-        for candidate, check in zip(ADAPTERS, checks):
+        for candidate, check in zip(ADAPTERS, checks, strict=True):
             if check:
                 platforms.append(candidate.platform)
             if check and not adapter:
                 adapter = candidate
 
         if not adapter:
             raise PlatformGuessFailed()
@@ -304,19 +314,20 @@
             if self.conn._transport and not self.conn._transport.is_closing():
                 return self.conn
             self.log.debug("Connection is closed - reopening")
             return await self.renew_conn()
 
     @property
     def path(self) -> Type[PurePath]:
+        "Return path of the adapter"
         return self.adapter.path
 
-    def quote(self, s: str) -> str:
+    def quote(self, string: str) -> str:
         "Platform-specific shell quoting"
-        return self.adapter.quote(s)
+        return self.adapter.quote(string)
 
     @my_backoff_exc()
     async def run(
         self, *args, cwd: Optional[str] = None, **kwargs
     ) -> SSHCompletedProcess:
         "Run process and wait for exit"
         conn = await self.get_conn()
@@ -358,42 +369,43 @@
     async def setup_node(self, engines: PEngineRepository):
         """
         Setup node for target engines.
         :raises NotImplemented: Not supported on platform.
         """
         self.log.info(f"CPUs count: {await self.get_cpu_cores()}")
         conn = await self.get_conn()
+        # pylint: disable=redundant-keyword-arg
         retry = my_backoff_exc(exception=AllSSHRetryExc)
         await retry(self.adapter.setup_node)(
             conn=conn,
             run=self.run,
             quote=self.quote,
-            engines=engines,
+            engines=engines.filter_platforms(self.platforms),
             engines_dir=self.engines_dir,
             log=self.log,
         )
 
     async def occupancy_check(self, engine: PEngine) -> bool:
         """
         Check node occupancy by task for target engine
         """
         if engine.check_pname:
             try:
                 if [x async for x in self.pgrep(engine.check_pname)]:
                     return True
-            except SSHRetryExc as e:
-                self.log.info(f"Node {self.hostname} failed pgrep: {e}")
+            except SSHRetryExc as exc:
+                self.log.info(f"Node {self.hostname} failed pgrep: {exc}")
                 await self.renew_conn()
         if engine.check_cmd:
             try:
-                r = await self.run(engine.check_cmd)
-                if r.returncode == engine.check_cmd_code:
+                proc = await self.run(engine.check_cmd)
+                if proc.returncode == engine.check_cmd_code:
                     return True
-            except SSHRetryExc as e:
-                self.log.info(f"Node {self.hostname} failed command: {e}")
+            except SSHRetryExc as exc:
+                self.log.info(f"Node {self.hostname} failed command: {exc}")
                 await self.renew_conn()
         return False
 
     async def start_occupancy_check(self, engine: PEngine) -> None:
         """
         Start occupancy checker for engine.
         """
@@ -403,14 +415,14 @@
         async def occupancy_checker():
             while not self.cancellation_event.is_set() and self.meta.busy is not False:
                 try:
                     self.meta.busy = await asyncio.wait_for(
                         self.occupancy_check(engine), timeout=engine.sleep_interval
                     )
                 except asyncio.TimeoutError:
-                    t = "Engine {} busy check timeouted on {}"
-                    self.log.warning(t.format(engine.name, self.hostname))
-                except Exception as err:
+                    tmpl = "Engine {} busy check timeouted on {}"
+                    self.log.warning(tmpl.format(engine.name, self.hostname))
+                except Exception as err:  # pylint: disable=broad-exception-caught
                     self.log.warning(err)
                 await asyncio.sleep(engine.sleep_interval)
 
         self.jobs.add(asyncio.create_task(occupancy_checker()))
```

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/remote_machine_repository.py` & `yascheduler-1.2.0/yascheduler/remote_machine/remote_machine_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         free_since_gt: Optional[timedelta] = None,
         reverse_sort: bool = False,
     ) -> Self:
         "Return machines filtered and sorted by `free_since`"
 
         checks: Sequence[Callable[[PRemoteMachine], bool]] = []
         if busy is True:
-            checks.append(lambda x: x.meta.busy)
+            checks.append(lambda x: x.meta.busy is True)
         if busy is False:
             checks.append(lambda x: not x.meta.busy)
         if platforms:
             checks.append(lambda x: bool(set(platforms) & set(x.platforms)))
         if free_since_gt:
             checks.append(lambda x: x.meta.is_free_longer_than(free_since_gt))
```

### Comparing `yascheduler-1.0.9/yascheduler/remote_machine/windows_methods.py` & `yascheduler-1.2.0/yascheduler/remote_machine/windows_methods.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.9/yascheduler/scheduler.py` & `yascheduler-1.2.0/yascheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .time import asleep_until
 from .variables import CONFIG_FILE
 
 logging.basicConfig(level=logging.INFO)
 
 
 def get_logger(log_file, level: int = logging.INFO):
+    logging.captureWarnings(True)
     logger = logging.getLogger("yascheduler")
     logger.setLevel(level)
 
     backoff_logger = logging.getLogger("backoff")
     backoff_logger.setLevel(logging.ERROR if level >= logging.INFO else logging.DEBUG)
 
     if log_file:
@@ -285,24 +286,26 @@
 
         return True
 
     async def allocate_task(self, task: TaskModel) -> bool:
         "Allocate task to a free remote machine or ask allocation of new cloud machine"
         self.log.debug(f"Allocating task {task.task_id}")
         engine_name: Optional[str] = task.metadata.get("engine", None)
-        if not engine_name or engine_name not in self.config.engines:
+        engine: Optional[Engine] = self.config.engines.get(engine_name)
+        if engine is None:
             self.log.warning(
-                "Unsupported engine '%s' for task_id=%s" % (engine_name, task.task_id)
+                "Unsupported engine '{}' for task_id={}".format(
+                    engine_name, task.task_id
+                )
             )
             await self.db.set_task_error(
                 task.task_id, metadata=task.metadata, error="unsupported engine"
             )
             await self.do_task_webhook(task.task_id, task.metadata, TaskStatus.DONE)
             return False
-        engine: Engine = self.config.engines[engine_name]
 
         busy_node_ips = [
             t.ip for t in await self.db.get_tasks_by_status((TaskStatus.RUNNING,))
         ]
         free_machines = {
             ip: m
             for ip, m in self.remote_machines.filter(
@@ -382,15 +385,15 @@
                 await sftp.rmtree(
                     machine.path(remote_folder)
                 )  # uncomment to keep raw files
 
         try:
             await sftp_get_retry(job)()
         except Exception as err:
-            self.log.warning("Cannot scp from %s: %s" % (remote_folder, err))
+            self.log.warning(f"Cannot scp from {remote_folder}: {err}")
             sftp_errors.append((remote_folder, err))
 
         if sftp_errors:
             meta_add.append(("error", {p: str(e) for p, e in sftp_errors}))
 
         new_meta = dict(list(task.metadata.items()) + meta_add)
         if "error" in new_meta:
@@ -514,15 +517,15 @@
     async def task_consumer_consumer(
         self, msg: UMessage[int, TaskModel], machine_not_found: Counter
     ):
         """Consume running task if done, mark failed if machine is gone"""
         broken_tasks_passes = 20
         task_id, task = msg.id, msg.payload
         machine = self.remote_machines.get(task.ip)
-        if not machine:
+        if machine is None:
             self.log.warning(f"Task {task_id} - machine {task.ip} is gone")
             machine_not_found.update([task_id])
             if machine_not_found[task_id] > broken_tasks_passes:
                 await self.db.set_task_error(
                     task_id, metadata=task.metadata, error="node is gone"
                 )
                 await self.do_task_webhook(task_id, task.metadata, TaskStatus.DONE)
@@ -637,15 +640,16 @@
 
         # wait some connected machines before allocation
         async def wait_some_machines():
             while not len(self.remote_machines):
                 await asyncio.sleep(1)
 
         await asyncio.wait(
-            [wait_some_machines(), asyncio.sleep(30)], return_when="FIRST_COMPLETED"
+            [asyncio.create_task(x) for x in [wait_some_machines(), asyncio.sleep(30)]],
+            return_when="FIRST_COMPLETED",
         )
 
         allocate_co = self.create_producer_consumers(
             queue=self.allocate_q,
             producer=self.allocator_producer,
             consumer=self.allocator_consumer,
             workers_num=self.config.local.allocate_limit,
```

### Comparing `yascheduler-1.0.9/yascheduler/utils.py` & `yascheduler-1.2.0/yascheduler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,29 +26,32 @@
     parser.add_argument("script")
 
     args = parser.parse_args()
     script_file = Path(args.script)
     if not script_file.exists():
         raise ValueError("Script parameter is not a file name")
 
+    logging.captureWarnings(True)
     log = logging.getLogger()
-    log.setLevel(logging.ERROR)
+    log.setLevel(logging.WARN)
     yac = Yascheduler(logger=log)
 
     script_params = {}
     with script_file.open("r") as f:
         for line in f.readlines():
             try:
                 k, v = line.split("=")
                 script_params[k.strip()] = v.strip()
             except ValueError:
                 pass
 
     label = script_params.get("LABEL", "AiiDA job")
-    metadata: Mapping[str, Any] = {"local_folder": os.getcwd()} # NB AiiDA chdirs to repo, but if not?
+    metadata: Mapping[str, Any] = {
+        "local_folder": os.getcwd()
+    }  # NB AiiDA chdirs to repo, but if not?
     if not script_params.get("ENGINE"):
         raise ValueError("Script has not defined an engine")
 
     engine = yac.config.engines.get(script_params["ENGINE"])
     if not engine:
         raise ValueError("Engine %s is not supported" % script_params["ENGINE"])
 
@@ -114,15 +117,18 @@
     else:
         tasks = await db.get_tasks_by_status(
             statuses=(TaskStatus.RUNNING, TaskStatus.TO_DO)
         )
 
     if args.convergence:
         try:
+            # pylint: disable=import-error
             from numpy import nan
+
+            # pylint: disable=import-error
             from pycrystal import CRYSTOUT, CRYSTOUT_Error
 
             local_parsing_ready = True
         except Exception:
             pass
 
     if args.view:
@@ -266,15 +272,14 @@
         systemd_script = src_unit_file.read_text("utf-8").replace(
             "%YASCHEDULER_DAEMON_FILE%", str(daemon_file)
         )
         unit_file.write_text(systemd_script, "utf-8")
 
 
 def _init_sysv(install_path: Path):
-
     print("Installing SysV service")
 
     # create sysv script in /etc/init.d
     src_startup_file = install_path / "data/yascheduler.sh"
     startup_file = Path("/etc/init.d/yascheduler")
     if not startup_file.is_file():
         if not os.access(startup_file, os.W_OK):
@@ -308,24 +313,33 @@
 async def _show_nodes():
     config = Config.from_config_parser(CONFIG_FILE)
     db = await DB.create(config.db)
 
     tasks = await db.get_tasks_by_status(statuses=[TaskStatus.RUNNING])
     nodes = await db.get_all_nodes()
     for node in nodes:
+        tmpl = (
+            "ip={ip} ncpus={ncpus} enabled={enabled} "
+            "occupied_by={occ} (task_id={tid}) {cloud}"
+        )
         node_tasks = list(filter(lambda x: x.ip == node.ip, tasks))
-        node_task = ["-", "-"]
+        node_label = "-"
+        task_id = "-"
         for x in node_tasks:
-            node_task = [x.label, x.task_id]
-        data = tuple(
-            [node.ip, node.ncpus or "MAX", node.enabled]
-            + node_task
-            + [node.cloud or ""]
+            node_label = x.label
+            task_id = x.task_id
+        msg = tmpl.format(
+            ip=node.ip,
+            ncpus=node.ncpus or "MAX",
+            enabled=node.enabled,
+            occ=node_label,
+            tid=task_id,
+            cloud=node.cloud or "",
         )
-        print("ip=%s ncpus=%s enabled=%s occupied_by=%s (task_id=%s) %s" % data)
+        print(msg)
 
 
 def show_nodes():
     asyncio.run(_show_nodes())
 
 
 async def _manage_node():
@@ -381,15 +395,17 @@
         return False
 
     if args.remove_hard:
         task_ids = await db.get_task_ids_by_ip_and_status(args.host, TaskStatus.RUNNING)
         for task_id in task_ids:
             await db.update_task_status(task_id, TaskStatus.DONE)
             print(
-                "An associated task %s at %s is now marked done!" % (task_id, args.host)
+                "An associated task {} at {} is now marked done!".format(
+                    task_id, args.host
+                )
             )
 
         await db.remove_node(args.host)
         await db.commit()
         await db.close()
         print(f"Removed host from yascheduler: {args.host}")
         return True
@@ -440,18 +456,19 @@
         choices=logging._levelToName.values(),
     )
     args = parser.parse_args()
 
     logger = get_logger(log_file, level=logging._nameToLevel[args.log_level])
 
     async def on_signal(
-        y: Scheduler, shield: Sequence[asyncio.Task], signame: str, signum: int
+        y: Scheduler, shield: Sequence[asyncio.Task], sig: signal.Signals
     ):
+        signame = signal.strsignal(sig)
         logger.info(f"Received signal {signame}")
-        if signum in [signal.SIGTERM, signal.SIGINT]:
+        if sig in [signal.SIGTERM, signal.SIGINT]:
             await y.stop()
             shielded = [*shield, asyncio.current_task()]
             tasks = [t for t in asyncio.all_tasks() if t not in shielded]
             logger.info(f"Cancelling {len(tasks)} outstanding tasks")
             [task.cancel() for task in tasks]
             await asyncio.gather(*tasks, return_exceptions=True)
             # Wait 250 ms for the underlying SSL connections to close
@@ -464,16 +481,15 @@
         loop = asyncio.get_running_loop()
         current_task = asyncio.current_task()
 
         shielded = [current_task] if current_task else []
         for sig in [signal.SIGTERM, signal.SIGINT]:
 
             def handler():
-                return asyncio.create_task(
-                    on_signal(yac, shielded, sig.name, sig.value)
-                )
+                task = on_signal(yac, shielded, sig)  # noqa: B023
+                return asyncio.create_task(task)
 
             loop.add_signal_handler(sig, handler)
 
         await yac.start()
 
     asyncio.run(run())
```

