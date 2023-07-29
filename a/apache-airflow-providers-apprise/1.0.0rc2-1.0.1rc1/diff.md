# Comparing `tmp/apache-airflow-providers-apprise-1.0.0rc2.tar.gz` & `tmp/apache-airflow-providers-apprise-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apprise-1.0.0rc2.tar", last modified: Thu Jul  6 04:50:24 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apprise-1.0.1rc1.tar", last modified: Sat Jul 29 12:08:06 2023, max compression
```

## Comparing `apache-airflow-providers-apprise-1.0.0rc2.tar` & `apache-airflow-providers-apprise-1.0.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.258325 apache-airflow-providers-apprise-1.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-06 04:50:24.258938 apache-airflow-providers-apprise-1.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2760 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.180173 apache-airflow-providers-apprise-1.0.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.181246 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.214239 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-07-05 18:47:43.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.220052 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5224 2023-06-29 05:49:30.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/apprise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.225678 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/apprise.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:24.255907 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:24.000000 apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 04:50:24.260830 apache-airflow-providers-apprise-1.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-07-06 04:50:23.000000 apache-airflow-providers-apprise-1.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.978369 apache-airflow-providers-apprise-1.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apprise-1.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-29 12:08:06.978922 apache-airflow-providers-apprise-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.901871 apache-airflow-providers-apprise-1.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.903227 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.939635 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-29 12:01:19.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.945822 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/apprise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.951850 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-24 10:23:12.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/apprise.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:06.976101 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:06.000000 apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apprise-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-29 12:08:06.981045 apache-airflow-providers-apprise-1.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-29 12:08:05.000000 apache-airflow-providers-apprise-1.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/LICENSE` & `apache-airflow-providers-apprise-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/MANIFEST.in` & `apache-airflow-providers-apprise-1.0.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/PKG-INFO` & `apache-airflow-providers-apprise-1.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.0.0rc2
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apprise package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.0rc2``
+Release: ``1.0.1rc1``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apprise`` provider. All classes for this provider package
 are in ``airflow.providers.apprise`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -102,8 +102,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
 ``apprise``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/README.rst` & `apache-airflow-providers-apprise-1.0.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.0rc2``
+Release: ``1.0.1rc1``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apprise`` provider. All classes for this provider package
 are in ``airflow.providers.apprise`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -68,8 +68,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
 ``apprise``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/__init__.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-apprise:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/get_provider_info.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apprise",
         "name": "Apprise",
         "description": "`Apprise <https://github.com/caronc/apprise>`__\n",
         "suspended": False,
-        "versions": ["1.0.0"],
+        "versions": ["1.0.1", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Apprise",
                 "external-doc-url": "https://github.com/caronc/apprise",
                 "tags": ["software"],
             }
         ],
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/__init__.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/hooks/apprise.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/hooks/apprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 # under the License.
 from __future__ import annotations
 
 import json
 from typing import Any, Iterable
 
 import apprise
-from airflow.hooks.base import BaseHook
 from apprise import AppriseConfig, NotifyFormat, NotifyType
 
+from airflow.hooks.base import BaseHook
+
 
 class AppriseHook(BaseHook):
     """
     Use Apprise(https://github.com/caronc/apprise) to interact with notification services.
 
     The complete list of notification services supported by Apprise can be found at:
     https://github.com/caronc/apprise/wiki#notification-services.
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/__init__.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/airflow/providers/apprise/notifications/apprise.py` & `apache-airflow-providers-apprise-1.0.1rc1/airflow/providers/apprise/notifications/apprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 try:
     from airflow.notifications.basenotifier import BaseNotifier
 except ImportError:
     raise AirflowOptionalProviderFeatureException(
         "Failed to import BaseNotifier. This feature is only available in Airflow versions >= 2.6.0"
     )
 
-from airflow.providers.apprise.hooks.apprise import AppriseHook
 from apprise import AppriseConfig, NotifyFormat, NotifyType
 
+from airflow.providers.apprise.hooks.apprise import AppriseHook
+
 
 class AppriseNotifier(BaseNotifier):
     """
     Apprise BaseNotifier.
 
     :param body: Specify the message body
     :param title: Specify the message title. This field is complete optional
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/PKG-INFO` & `apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apprise
-Version: 1.0.0rc2
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apprise package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apprise``
 
-Release: ``1.0.0rc2``
+Release: ``1.0.1rc1``
 
 
 `Apprise <https://github.com/caronc/apprise>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apprise`` provider. All classes for this provider package
 are in ``airflow.providers.apprise`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -102,8 +102,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
 ``apprise``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/apache_airflow_providers_apprise.egg-info/SOURCES.txt` & `apache-airflow-providers-apprise-1.0.1rc1/apache_airflow_providers_apprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/pyproject.toml` & `apache-airflow-providers-apprise-1.0.1rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi",
-    "airflow/migrations/versions/*.py"
+    "airflow/migrations/versions/*.py",
+    "tests/dags/test_imports.py",
 ]
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
@@ -69,14 +70,16 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+namespace-packages = ["airflow/providers"]
+
 [tool.pytest.ini_options]
 # * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
 # * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
 # * And we focus on use native pytest capabilities rather than adopt another frameworks.
 addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
 norecursedirs = [
     ".eggs",
@@ -95,54 +98,28 @@
     "ignore::DeprecationWarning:flask_appbuilder.widgets",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
-    "*.py",
+    "test_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
-# TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
-known-third-party = [
-    "asana",
-    "atlassian",
-    "celery",
-    "cloudant",
-    "databricks",
-    "datadog",
-    "docker",
-    "elasticsearch",
-    "github",
-    "google",
-    "grpc",
-    "jenkins",
-    "mysql",
-    "neo4j",
-    "papermill",
-    "redis",
-    "sendgrid",
-    "snowflake",
-    "telegram",
-    "trino",
-]
-
 [tool.ruff.per-file-ignores]
 "airflow/models/__init__.py" = ["F401"]
 "airflow/models/sqla_models.py" = ["F401"]
 
-
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
 "airflow/serialization/pydantic/*.py" = ["I002"]
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/setup.cfg` & `apache-airflow-providers-apprise-1.0.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apprise/1.0.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apprise.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apprise
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apprise-1.0.0rc2/setup.py` & `apache-airflow-providers-apprise-1.0.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apprise package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.0.0"
+version = "1.0.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apprise setup."""
     setup(
         version=version,
         extras_require={},
```

