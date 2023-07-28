# Comparing `tmp/s4-clarity-1.4.1.tar.gz` & `tmp/s4-clarity-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s4-clarity-1.4.1.tar", last modified: Wed Jan  4 22:34:53 2023, max compression
+gzip compressed data, was "s4-clarity-1.4.2.tar", last modified: Fri Jul 28 22:22:47 2023, max compression
```

## Comparing `s4-clarity-1.4.1.tar` & `s4-clarity-1.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.578852 s4-clarity-1.4.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     3284 2023-01-04 22:34:53.578852 s4-clarity-1.4.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2087 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.562852 s4-clarity-1.4.1/s4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.570852 s4-clarity-1.4.1/s4/clarity/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1439 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.570852 s4-clarity-1.4.1/s4/clarity/_internal/
--rw-rw-r--   0 travis    (2000) travis    (2000)      588 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7989 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/element.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16591 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/factory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1926 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/fakesession.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9389 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/fields.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      653 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/lazy_property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27938 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/props.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/stepfactory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1648 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/_internal/udffactory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9944 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/artifact.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.574852 s4-clarity-1.4.1/s4/clarity/configuration/
--rw-rw-r--   0 travis    (2000) travis    (2000)      735 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/configuration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1880 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/configuration/process_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4686 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/configuration/protocol.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1793 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/configuration/stage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4780 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/configuration/udf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/configuration/workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2561 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/console.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6034 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/container.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/control_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2696 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8032 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1854 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/instrument.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6186 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/iomaps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/lab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12313 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/lims.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/permission.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1779 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/queue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      729 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/reagent_kit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/reagent_lot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1439 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/reagent_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/researcher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4809 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/routing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/sample.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.574852 s4-clarity-1.4.1/s4/clarity/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      821 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3097 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/derived_sample_automation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1371 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/epp_output_formatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2298 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/file_argument_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10688 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/genericscript.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3352 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/htmllogging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1766 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/shell.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6752 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/stepepp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3393 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/triggered_step_epp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/user_message_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      480 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/scripts/workflow_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23555 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/step.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.578852 s4-clarity-1.4.1/s4/clarity/steputils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7853 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/actions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/copyudfs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1437 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/file_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3853 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/placement_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4088 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/step_average_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24069 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/steputils/step_runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2277 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.578852 s4-clarity-1.4.1/s4/clarity/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      590 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7129 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/utils/artifact_ancestry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      695 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/utils/date_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      422 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/utils/sorting_util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1429 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/utils/ssh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/s4/clarity/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-04 22:34:53.578852 s4-clarity-1.4.1/s4_clarity.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3284 2023-01-04 22:34:53.000000 s4-clarity-1.4.1/s4_clarity.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2023-01-04 22:34:53.000000 s4-clarity-1.4.1/s4_clarity.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-04 22:34:53.000000 s4-clarity-1.4.1/s4_clarity.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-01-04 22:34:53.000000 s4-clarity-1.4.1/s4_clarity.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-01-04 22:34:53.000000 s4-clarity-1.4.1/s4_clarity.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2023-01-04 22:34:53.578852 s4-clarity-1.4.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2033 2023-01-04 22:34:24.000000 s4-clarity-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.488718 s4-clarity-1.4.2/s4/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.492718 s4-clarity-1.4.2/s4/clarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.496718 s4-clarity-1.4.2/s4/clarity/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/fakesession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/lazy_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27938 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/stepfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/_internal/udffactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.496718 s4-clarity-1.4.2/s4/clarity/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/process_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/udf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/configuration/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/control_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/iomaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/reagent_kit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/reagent_lot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/reagent_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/researcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.496718 s4-clarity-1.4.2/s4/clarity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/derived_sample_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/epp_output_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/file_argument_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/genericscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/htmllogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/stepepp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/triggered_step_epp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/user_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/scripts/workflow_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/s4/clarity/steputils/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/copyudfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/placement_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/step_average_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/steputils/step_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/s4/clarity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/artifact_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/date_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/sorting_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/s4/clarity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/s4_clarity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-28 22:22:47.000000 s4-clarity-1.4.2/s4_clarity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 22:22:47.500718 s4-clarity-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-28 22:22:43.000000 s4-clarity-1.4.2/setup.py
```

### Comparing `s4-clarity-1.4.1/LICENSE` & `s4-clarity-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/PKG-INFO` & `s4-clarity-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s4-clarity
-Version: 1.4.1
+Version: 1.4.2
 Summary: A general purpose library for interacting with Clarity LIMS
 Home-page: https://github.com/SemaphoreSolutions/s4-clarity-lib
 Author: Semaphore Solutions
 Author-email: info@semaphoresolutions.ca
 Project-URL: Documentation, https://readthedocs.org/projects/s4-clarity-lib
 Project-URL: Source, https://github.com/SemaphoreSolutions/s4-clarity-lib
 Classifier: License :: OSI Approved :: MIT License
@@ -27,16 +27,16 @@
 
 
 ==================
 S4-Clarity Library
 ==================
 
 
-.. image:: https://travis-ci.com/SemaphoreSolutions/s4-clarity-lib.svg?branch=master
-    :target: https://travis-ci.com/SemaphoreSolutions/s4-clarity-lib
+.. image:: https://github.com/SemaphoreSolutions/s4-clarity-lib/actions/workflows/ci.yml/badge.svg?branch=master
+    :target: https://github.com/SemaphoreSolutions/s4-clarity-lib/actions
 
 
 Used in numerous labs around the world, the S4-Clarity library provides an easy-to-use integration with the BaseSpace Clarity LIMS API. The package includes:
    - Classes representing familiar Clarity API entities that provide read-write access to most properties.
    - Helper methods that simplify common operations.
    - Base classes for scripts that integrate with Clarity: EPPs, DSAs, and shell scripts.
    - Utilities that help with Clarity-related tasks, such as managing config slices, or automating the completion of a Step.
```

### Comparing `s4-clarity-1.4.1/README.rst` & `s4-clarity-1.4.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 ==================
 S4-Clarity Library
 ==================
 
 
-.. image:: https://travis-ci.com/SemaphoreSolutions/s4-clarity-lib.svg?branch=master
-    :target: https://travis-ci.com/SemaphoreSolutions/s4-clarity-lib
+.. image:: https://github.com/SemaphoreSolutions/s4-clarity-lib/actions/workflows/ci.yml/badge.svg?branch=master
+    :target: https://github.com/SemaphoreSolutions/s4-clarity-lib/actions
 
 
 Used in numerous labs around the world, the S4-Clarity library provides an easy-to-use integration with the BaseSpace Clarity LIMS API. The package includes:
    - Classes representing familiar Clarity API entities that provide read-write access to most properties.
    - Helper methods that simplify common operations.
    - Base classes for scripts that integrate with Clarity: EPPs, DSAs, and shell scripts.
    - Utilities that help with Clarity-related tasks, such as managing config slices, or automating the completion of a Step.
```

### Comparing `s4-clarity-1.4.1/s4/clarity/__init__.py` & `s4-clarity-1.4.2/s4/clarity/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/__init__.py` & `s4-clarity-1.4.2/s4/clarity/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/element.py` & `s4-clarity-1.4.2/s4/clarity/_internal/element.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/factory.py` & `s4-clarity-1.4.2/s4/clarity/_internal/factory.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/fakesession.py` & `s4-clarity-1.4.2/s4/clarity/_internal/fakesession.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/fields.py` & `s4-clarity-1.4.2/s4/clarity/_internal/fields.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/lazy_property.py` & `s4-clarity-1.4.2/s4/clarity/_internal/lazy_property.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/props.py` & `s4-clarity-1.4.2/s4/clarity/_internal/props.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/stepfactory.py` & `s4-clarity-1.4.2/s4/clarity/_internal/stepfactory.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/_internal/udffactory.py` & `s4-clarity-1.4.2/s4/clarity/_internal/udffactory.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/artifact.py` & `s4-clarity-1.4.2/s4/clarity/artifact.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/configuration/__init__.py` & `s4-clarity-1.4.2/s4/clarity/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/configuration/process_type.py` & `s4-clarity-1.4.2/s4/clarity/configuration/process_type.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/configuration/protocol.py` & `s4-clarity-1.4.2/s4/clarity/configuration/protocol.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/configuration/stage.py` & `s4-clarity-1.4.2/s4/clarity/configuration/stage.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/configuration/udf.py` & `s4-clarity-1.4.2/s4/clarity/configuration/udf.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/configuration/workflow.py` & `s4-clarity-1.4.2/s4/clarity/configuration/workflow.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/console.py` & `s4-clarity-1.4.2/s4/clarity/console.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/container.py` & `s4-clarity-1.4.2/s4/clarity/container.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/control_type.py` & `s4-clarity-1.4.2/s4/clarity/control_type.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/exception.py` & `s4-clarity-1.4.2/s4/clarity/exception.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/file.py` & `s4-clarity-1.4.2/s4/clarity/file.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/instrument.py` & `s4-clarity-1.4.2/s4/clarity/instrument.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/iomaps.py` & `s4-clarity-1.4.2/s4/clarity/iomaps.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/lims.py` & `s4-clarity-1.4.2/s4/clarity/lims.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/process.py` & `s4-clarity-1.4.2/s4/clarity/process.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/project.py` & `s4-clarity-1.4.2/s4/clarity/project.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/queue.py` & `s4-clarity-1.4.2/s4/clarity/queue.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/reagent_kit.py` & `s4-clarity-1.4.2/s4/clarity/reagent_kit.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/reagent_lot.py` & `s4-clarity-1.4.2/s4/clarity/reagent_lot.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/reagent_type.py` & `s4-clarity-1.4.2/s4/clarity/reagent_type.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/researcher.py` & `s4-clarity-1.4.2/s4/clarity/researcher.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/role.py` & `s4-clarity-1.4.2/s4/clarity/role.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/routing.py` & `s4-clarity-1.4.2/s4/clarity/routing.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/sample.py` & `s4-clarity-1.4.2/s4/clarity/sample.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/__init__.py` & `s4-clarity-1.4.2/s4/clarity/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/derived_sample_automation.py` & `s4-clarity-1.4.2/s4/clarity/scripts/derived_sample_automation.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/epp_output_formatter.py` & `s4-clarity-1.4.2/s4/clarity/scripts/epp_output_formatter.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/file_argument_script.py` & `s4-clarity-1.4.2/s4/clarity/scripts/file_argument_script.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/genericscript.py` & `s4-clarity-1.4.2/s4/clarity/scripts/genericscript.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/htmllogging.py` & `s4-clarity-1.4.2/s4/clarity/scripts/htmllogging.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/shell.py` & `s4-clarity-1.4.2/s4/clarity/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/stepepp.py` & `s4-clarity-1.4.2/s4/clarity/scripts/stepepp.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/scripts/triggered_step_epp.py` & `s4-clarity-1.4.2/s4/clarity/scripts/triggered_step_epp.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/step.py` & `s4-clarity-1.4.2/s4/clarity/step.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/steputils/actions.py` & `s4-clarity-1.4.2/s4/clarity/steputils/actions.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/steputils/copyudfs.py` & `s4-clarity-1.4.2/s4/clarity/steputils/copyudfs.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/steputils/file_utils.py` & `s4-clarity-1.4.2/s4/clarity/steputils/file_utils.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/steputils/placement_utils.py` & `s4-clarity-1.4.2/s4/clarity/steputils/placement_utils.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/steputils/step_average_utils.py` & `s4-clarity-1.4.2/s4/clarity/steputils/step_average_utils.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/steputils/step_runner.py` & `s4-clarity-1.4.2/s4/clarity/steputils/step_runner.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/types.py` & `s4-clarity-1.4.2/s4/clarity/types.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/utils/__init__.py` & `s4-clarity-1.4.2/s4/clarity/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/utils/artifact_ancestry.py` & `s4-clarity-1.4.2/s4/clarity/utils/artifact_ancestry.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/utils/date_util.py` & `s4-clarity-1.4.2/s4/clarity/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4/clarity/utils/ssh.py` & `s4-clarity-1.4.2/s4/clarity/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/s4_clarity.egg-info/PKG-INFO` & `s4-clarity-1.4.2/s4_clarity.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s4-clarity
-Version: 1.4.1
+Version: 1.4.2
 Summary: A general purpose library for interacting with Clarity LIMS
 Home-page: https://github.com/SemaphoreSolutions/s4-clarity-lib
 Author: Semaphore Solutions
 Author-email: info@semaphoresolutions.ca
 Project-URL: Documentation, https://readthedocs.org/projects/s4-clarity-lib
 Project-URL: Source, https://github.com/SemaphoreSolutions/s4-clarity-lib
 Classifier: License :: OSI Approved :: MIT License
@@ -27,16 +27,16 @@
 
 
 ==================
 S4-Clarity Library
 ==================
 
 
-.. image:: https://travis-ci.com/SemaphoreSolutions/s4-clarity-lib.svg?branch=master
-    :target: https://travis-ci.com/SemaphoreSolutions/s4-clarity-lib
+.. image:: https://github.com/SemaphoreSolutions/s4-clarity-lib/actions/workflows/ci.yml/badge.svg?branch=master
+    :target: https://github.com/SemaphoreSolutions/s4-clarity-lib/actions
 
 
 Used in numerous labs around the world, the S4-Clarity library provides an easy-to-use integration with the BaseSpace Clarity LIMS API. The package includes:
    - Classes representing familiar Clarity API entities that provide read-write access to most properties.
    - Helper methods that simplify common operations.
    - Base classes for scripts that integrate with Clarity: EPPs, DSAs, and shell scripts.
    - Utilities that help with Clarity-related tasks, such as managing config slices, or automating the completion of a Step.
```

### Comparing `s4-clarity-1.4.1/s4_clarity.egg-info/SOURCES.txt` & `s4-clarity-1.4.2/s4_clarity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s4-clarity-1.4.1/setup.py` & `s4-clarity-1.4.2/setup.py`

 * *Files identical despite different names*

