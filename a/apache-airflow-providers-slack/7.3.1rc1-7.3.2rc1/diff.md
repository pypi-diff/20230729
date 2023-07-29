# Comparing `tmp/apache-airflow-providers-slack-7.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-slack-7.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-slack-7.3.1rc1.tar", last modified: Tue Jun 20 11:43:12 2023, max compression
+gzip compressed data, was "apache-airflow-providers-slack-7.3.2rc1.tar", last modified: Sat Jul 29 12:09:06 2023, max compression
```

## Comparing `apache-airflow-providers-slack-7.3.1rc1.tar` & `apache-airflow-providers-slack-7.3.2rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.173391 apache-airflow-providers-slack-7.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15946 2023-06-20 11:43:12.174477 apache-airflow-providers-slack-7.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14394 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.072082 apache-airflow-providers-slack-7.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.073303 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.111497 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.120174 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14482 2023-06-01 07:44:14.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack.py
--rw-r--r--   0 root         (0) root         (0)    21221 2023-06-01 07:44:14.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.128994 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack_notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.137516 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-06-05 12:50:36.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack.py
--rw-r--r--   0 root         (0) root         (0)     7402 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.143280 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12879 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/sql_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.146227 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/utils/
--rw-r--r--   0 root         (0) root         (0)     5132 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.170761 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15946 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1090 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-slack-7.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1890 2023-06-20 11:43:12.176409 apache-airflow-providers-slack-7.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.359030 apache-airflow-providers-slack-7.3.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-07-29 12:09:06.359646 apache-airflow-providers-slack-7.3.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.256000 apache-airflow-providers-slack-7.3.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.257146 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.294291 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.303304 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14482 2023-07-06 04:42:33.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack.py
+-rw-r--r--   0 root         (0) root         (0)    21222 2023-07-06 04:42:33.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.312758 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack_notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.321545 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-05 12:50:36.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.327221 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12923 2023-07-26 06:59:50.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/sql_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.330505 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/utils/
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:06.356268 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:06.000000 apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-slack-7.3.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-29 12:09:06.361593 apache-airflow-providers-slack-7.3.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-29 12:09:05.000000 apache-airflow-providers-slack-7.3.2rc1/setup.py
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/LICENSE` & `apache-airflow-providers-slack-7.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/MANIFEST.in` & `apache-airflow-providers-slack-7.3.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.3.1"
+__version__ = "7.3.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-slack:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/get_provider_info.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-slack",
         "name": "Slack",
         "description": "`Slack <https://slack.com/>`__\n",
         "suspended": False,
         "versions": [
+            "7.3.2",
             "7.3.1",
             "7.3.0",
             "7.2.0",
             "7.1.1",
             "7.1.0",
             "7.0.0",
             "6.0.0",
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,16 @@
 
 if TYPE_CHECKING:
     from slack_sdk.http_retry import RetryHandler
     from slack_sdk.web.slack_response import SlackResponse
 
 
 def _ensure_prefixes(conn_type):
-    """
-    Remove when provider min airflow version >= 2.5.0 since this is handled by
-    provider manager from that version.
-    """
+    # TODO: Remove when provider min airflow version >= 2.5.0 since
+    #       this is handled by provider manager from that version.
 
     def dec(func):
         @wraps(func)
         def inner(cls):
             field_behaviors = func(cls)
             conn_attrs = {"host", "schema", "login", "password", "port", "extra"}
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack_webhook.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/hooks/slack_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,16 @@
             )
         return resp
 
     return wrapper
 
 
 def _ensure_prefixes(conn_type):
-    """
-    Remove when provider min airflow version >= 2.5.0 since this is handled by
-    provider manager from that version.
-    """
+    # TODO: Remove when provider min airflow version >= 2.5.0 since
+    #       this is handled by provider manager from that version.
 
     def dec(func):
         @wraps(func)
         def inner(cls):
             field_behaviors = func(cls)
             conn_attrs = {"host", "schema", "login", "password", "port", "extra"}
 
@@ -81,14 +79,15 @@
 
     return dec
 
 
 class SlackWebhookHook(BaseHook):
     """
     This class provide a thin wrapper around the ``slack_sdk.WebhookClient``.
+
     This hook allows you to post messages to Slack by using Incoming Webhooks.
 
     .. seealso::
         - :ref:`Slack Incoming Webhook connection <howto/connection:slack-incoming-webhook>`
         - https://api.slack.com/messaging/webhooks
         - https://slack.dev/python-slack-sdk/webhook/index.html
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack_notifier.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/notifications/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack_webhook.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/operators/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/sql_to_slack.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from tempfile import NamedTemporaryFile
-from typing import TYPE_CHECKING, Iterable, Mapping, Sequence
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, Sequence
 
 from pandas import DataFrame
 from tabulate import tabulate
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator
@@ -47,15 +47,15 @@
 
     def __init__(
         self,
         *,
         sql: str,
         sql_conn_id: str,
         sql_hook_params: dict | None = None,
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.sql_conn_id = sql_conn_id
         self.sql_hook_params = sql_hook_params
         self.sql = sql
         self.parameters = parameters
@@ -76,20 +76,23 @@
         self.log.info("Running SQL query: %s", self.sql)
         df = sql_hook.get_pandas_df(self.sql, parameters=self.parameters)
         return df
 
 
 class SqlToSlackOperator(BaseSqlToSlackOperator):
     """
-    Executes an SQL statement in a given SQL connection and sends the results to Slack. The results of the
-    query are rendered into the 'slack_message' parameter as a Pandas dataframe using a JINJA variable called
-    '{{ results_df }}'. The 'results_df' variable name can be changed by specifying a different
-    'results_df_name' parameter. The Tabulate library is added to the JINJA environment as a filter to
-    allow the dataframe to be rendered nicely. For example, set 'slack_message' to {{ results_df |
-    tabulate(tablefmt="pretty", headers="keys") }} to send the results to Slack as an ascii rendered table.
+    Executes an SQL statement in a given SQL connection and sends the results to Slack.
+
+    The results of the query are rendered into the 'slack_message' parameter as a Pandas
+    dataframe using a JINJA variable called '{{ results_df }}'. The 'results_df' variable
+    name can be changed by specifying a different 'results_df_name' parameter. The Tabulate
+    library is added to the JINJA environment as a filter to allow the dataframe to be
+    rendered nicely. For example, set 'slack_message' to {{ results_df |
+    tabulate(tablefmt="pretty", headers="keys") }} to send the results to Slack as an ascii
+    rendered table.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SqlToSlackOperator`
 
     :param sql: The SQL query to be executed (templated)
     :param slack_message: The templated Slack message to send with the data returned from the SQL connection.
@@ -118,15 +121,15 @@
         sql_conn_id: str,
         sql_hook_params: dict | None = None,
         slack_conn_id: str | None = None,
         slack_webhook_token: str | None = None,
         slack_channel: str | None = None,
         slack_message: str,
         results_df_name: str = "results_df",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         **kwargs,
     ) -> None:
 
         super().__init__(
             sql=sql, sql_conn_id=sql_conn_id, sql_hook_params=sql_hook_params, parameters=parameters, **kwargs
         )
 
@@ -239,15 +242,15 @@
 
     def __init__(
         self,
         *,
         sql: str,
         sql_conn_id: str,
         sql_hook_params: dict | None = None,
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         slack_conn_id: str,
         slack_filename: str,
         slack_channels: str | Sequence[str] | None = None,
         slack_initial_comment: str | None = None,
         slack_title: str | None = None,
         df_kwargs: dict | None = None,
         **kwargs,
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/utils/__init__.py` & `apache-airflow-providers-slack-7.3.2rc1/airflow/providers/slack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt` & `apache-airflow-providers-slack-7.3.2rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.1rc1/pyproject.toml` & `apache-airflow-providers-slack-7.3.2rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
 
@@ -35,15 +37,16 @@
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
 
@@ -67,14 +70,16 @@
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
@@ -93,54 +98,28 @@
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

### Comparing `apache-airflow-providers-slack-7.3.1rc1/setup.cfg` & `apache-airflow-providers-slack-7.3.2rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-slack-7.3.1rc1/setup.py` & `apache-airflow-providers-slack-7.3.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-slack package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.3.1"
+version = "7.3.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-slack setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

