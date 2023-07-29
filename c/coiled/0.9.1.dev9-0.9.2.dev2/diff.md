# Comparing `tmp/coiled-0.9.1.dev9.tar.gz` & `tmp/coiled-0.9.2.dev2.tar.gz`

## Comparing `coiled-0.9.1.dev9.tar` & `coiled-0.9.2.dev2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/auth.py
--rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/capture_environment.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/context.py
--rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/run.py
--rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/scan.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/types.py
--rw-r--r--   0        0        0    56396 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/prefect.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    48728 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0   100308 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/cluster.py
--rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/.gitignore
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coiled-0.9.1.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/analytics.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/auth.py
+-rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/capture_environment.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/context.py
+-rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/exceptions.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/run.py
+-rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/scan.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/types.py
+-rw-r--r--   0        0        0    56396 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/utils.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/core.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/utils.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    48728 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    27132 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/__init__.py
+-rw-r--r--   0        0        0   100308 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coiled-0.9.2.dev2/PKG-INFO
```

### Comparing `coiled-0.9.1.dev9/coiled/__init__.py` & `coiled-0.9.2.dev2/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/analytics.py` & `coiled-0.9.2.dev2/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/auth.py` & `coiled-0.9.2.dev2/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/capture_environment.py` & `coiled-0.9.2.dev2/coiled/capture_environment.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cluster.py` & `coiled-0.9.2.dev2/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/coiled.yaml` & `coiled-0.9.2.dev2/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/context.py` & `coiled-0.9.2.dev2/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/core.py` & `coiled-0.9.2.dev2/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/exceptions.py` & `coiled-0.9.2.dev2/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/run.py` & `coiled-0.9.2.dev2/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/scan.py` & `coiled-0.9.2.dev2/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/shutdown.py` & `coiled-0.9.2.dev2/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/software.py` & `coiled-0.9.2.dev2/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/types.py` & `coiled-0.9.2.dev2/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/utils.py` & `coiled-0.9.2.dev2/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/websockets.py` & `coiled-0.9.2.dev2/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/config.py` & `coiled-0.9.2.dev2/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/core.py` & `coiled-0.9.2.dev2/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/curl.py` & `coiled-0.9.2.dev2/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/env.py` & `coiled-0.9.2.dev2/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/login.py` & `coiled-0.9.2.dev2/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/package_sync.py` & `coiled-0.9.2.dev2/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/prefect.py` & `coiled-0.9.2.dev2/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/run.py` & `coiled-0.9.2.dev2/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/utils.py` & `coiled-0.9.2.dev2/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.9.2.dev2/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.9.2.dev2/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/cluster/logs.py` & `coiled-0.9.2.dev2/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/cluster/metrics.py` & `coiled-0.9.2.dev2/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.9.2.dev2/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/cluster/utils.py` & `coiled-0.9.2.dev2/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.9.2.dev2/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.9.2.dev2/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/setup/__init__.py` & `coiled-0.9.2.dev2/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/setup/amp.py` & `coiled-0.9.2.dev2/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/setup/aws.py` & `coiled-0.9.2.dev2/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/setup/entry.py` & `coiled-0.9.2.dev2/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/cli/setup/gcp.py` & `coiled-0.9.2.dev2/coiled/cli/setup/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,29 +362,37 @@
 @click.option(
     "-y",
     "--yes",
     default=False,
     is_flag=True,
     help="Don't prompt for confirmation, just do it!",
 )
+@click.option(
+    "--use-shim",
+    default=False,
+    is_flag=True,
+    hidden=True,
+    help="Use new setup backend",
+)
 @click.command(context_settings=CONTEXT_SETTINGS)
-def gcp_setup(region, skip_gar, manual_final_setup, quotas, quota_link, export, iam_user, yes):
-    do_setup(region, skip_gar, manual_final_setup, quotas, quota_link, export, iam_user, yes)
+def gcp_setup(region, skip_gar, manual_final_setup, quotas, quota_link, export, iam_user, yes, use_shim):
+    do_setup(region, skip_gar, manual_final_setup, quotas, quota_link, export, iam_user, yes, use_shim)
 
 
 def do_setup(
     region=None,
     skip_gar=False,
     manual_final_setup=False,
     quotas=False,
     quota_link=False,
     export=None,
     iam_user="coiled",
     yes=False,
-):
+    use_shim: bool = False,
+) -> bool:
     local_user = get_local_user()
 
     coiled.add_interaction(
         action="CliSetupGcp",
         success=True,
         local_user=local_user,
         # use keys that match the cli args
@@ -403,15 +411,15 @@
             print(f"Exported Coiled role definition to {export_path}")
 
         elif export == "data-role":
             with open(export_path, "w") as f:
                 f.write(DATA_ROLE)
             print(f"Exported Coiled 'data access' role definition to {export_path}")
 
-        return
+        return False
 
     if not has_gcloud():
         print("\n[red]Missing:[/red] The gcloud CLI tool is required for automatic setup.\n")
         if os.path.exists(os.path.join(sys.prefix, "conda-meta")):
             print(
                 "Install gcloud with conda using the following command:\n\n"
                 "\t[green]conda install -c conda-forge google-cloud-sdk\n"
@@ -442,15 +450,15 @@
             "[green]coiled setup gcp --region us-central1[/green]"
         )
         setup_failure("Region was not set", backend="gcp")
         return False
 
     if quotas or quota_link:
         show_quotas(project, region, help=not quota_link)
-        return
+        return False
 
     base_account_name = iam_user
     base_name_for_role = iam_user.replace("-", "_")  # role can't have `-`
 
     main_sa = base_account_name
     data_sa = f"{base_account_name}-data"
     main_role = base_name_for_role
@@ -606,14 +614,15 @@
             print("Setting up Coiled to use your Google Cloud account...")
             coiled.set_backend_options(
                 backend="gcp",
                 registry_type="gar" if not skip_gar else "ecr",
                 gcp_region=region,
                 gcp_service_creds_file=key_path,
                 instance_service_account=data_email,
+                use_shim=use_shim,
             )
             coiled.add_interaction(action="CoiledSetup", success=True)
 
     else:
         coiled.add_interaction(action="prompt:CoiledSetup", success=False)
         with coiled.Cloud() as cloud:
             coiled_account = cloud.default_account
```

### Comparing `coiled-0.9.1.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.9.2.dev2/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/extensions/prefect/runners.py` & `coiled-0.9.2.dev2/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/extensions/prefect/workers.py` & `coiled-0.9.2.dev2/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/__init__.py` & `coiled-0.9.2.dev2/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/cluster.py` & `coiled-0.9.2.dev2/coiled/v2/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/core.py` & `coiled-0.9.2.dev2/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/cwi_log_link.py` & `coiled-0.9.2.dev2/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/states.py` & `coiled-0.9.2.dev2/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/widgets/__init__.py` & `coiled-0.9.2.dev2/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/widgets/rich.py` & `coiled-0.9.2.dev2/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/coiled/v2/widgets/util.py` & `coiled-0.9.2.dev2/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/README.md` & `coiled-0.9.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/pyproject.toml` & `coiled-0.9.2.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.1.dev9/PKG-INFO` & `coiled-0.9.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.9.1.dev9
+Version: 0.9.2.dev2
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.9.1.dev9 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.9.2.dev2 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: gilknocker>=0.4.1 Requires-Dist: importlib-metadata Requires-
 Dist: ipywidgets Requires-Dist: jmespath Requires-Dist: jsondiff Requires-Dist:
 packaging Requires-Dist: pip Requires-Dist: pip>=19.3 Requires-Dist:
```

