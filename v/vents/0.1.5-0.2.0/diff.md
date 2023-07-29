# Comparing `tmp/vents-0.1.5.tar.gz` & `tmp/vents-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.1.5.tar", last modified: Fri Jun 30 18:50:06 2023, max compression
+gzip compressed data, was "vents-0.2.0.tar", last modified: Sat Jul 29 14:34:52 2023, max compression
```

## Comparing `vents-0.1.5.tar` & `vents-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.660574 vents-0.1.5/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-06-30 18:47:37.000000 vents-0.1.5/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-30 18:50:06.660687 vents-0.1.5/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-06-30 18:50:06.661143 vents-0.1.5/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-06-30 18:47:37.000000 vents-0.1.5/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.654784 vents-0.1.5/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     5003 2023-06-30 18:47:37.000000 vents-0.1.5/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.656684 vents-0.1.5/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      335 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     3842 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)      513 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/connection_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-06-30 18:47:37.000000 vents-0.1.5/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-06-30 18:47:37.000000 vents-0.1.5/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.657980 vents-0.1.5/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-06-30 18:47:37.000000 vents-0.1.5/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-06-30 18:47:37.000000 vents-0.1.5/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.658638 vents-0.1.5/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.659324 vents-0.1.5/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1650 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.659907 vents-0.1.5/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.660442 vents-0.1.5/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-06-30 18:47:37.000000 vents-0.1.5/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-30 18:47:37.000000 vents-0.1.5/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-06-30 18:47:37.000000 vents-0.1.5/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-30 18:50:06.655891 vents-0.1.5/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       73 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-06-30 18:50:06.000000 vents-0.1.5/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.004098 vents-0.2.0/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-07-29 14:25:20.000000 vents-0.2.0/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-07-29 14:34:52.004183 vents-0.2.0/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-07-29 14:34:52.004622 vents-0.2.0/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-07-29 14:25:20.000000 vents-0.2.0/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:51.999293 vents-0.2.0/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 vents-0.2.0/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5003 2023-07-29 14:25:20.000000 vents-0.2.0/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.000660 vents-0.2.0/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      335 2023-07-29 14:25:20.000000 vents-0.2.0/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2501 2023-07-29 14:25:20.000000 vents-0.2.0/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3858 2023-07-29 14:25:20.000000 vents-0.2.0/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)      529 2023-07-29 14:25:20.000000 vents-0.2.0/vents/connections/connection_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3317 2023-07-29 14:25:20.000000 vents-0.2.0/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-07-29 14:25:20.000000 vents-0.2.0/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.001807 vents-0.2.0/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-07-29 14:25:20.000000 vents-0.2.0/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-07-29 14:25:20.000000 vents-0.2.0/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.002158 vents-0.2.0/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.002810 vents-0.2.0/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1650 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.003403 vents-0.2.0/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1636 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:52.003979 vents-0.2.0/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-07-29 14:25:20.000000 vents-0.2.0/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-07-29 14:25:20.000000 vents-0.2.0/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-07-29 14:25:20.000000 vents-0.2.0/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-07-29 14:34:51.999997 vents-0.2.0/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-07-29 14:34:51.000000 vents-0.2.0/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-07-29 14:34:51.000000 vents-0.2.0/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-07-29 14:34:51.000000 vents-0.2.0/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       69 2023-07-29 14:34:51.000000 vents-0.2.0/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-07-29 14:34:51.000000 vents-0.2.0/vents.egg-info/top_level.txt
```

### Comparing `vents-0.1.5/PKG-INFO` & `vents-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.5
+Version: 0.2.0
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.5/setup.cfg` & `vents-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/setup.py` & `vents-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/config.py` & `vents-0.2.0/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/connections/catalog.py` & `vents-0.2.0/vents/connections/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Optional
 
+from clipped.compact.pydantic import PrivateAttr
 from clipped.config.schema import BaseSchemaModel
-from pydantic import PrivateAttr
 
 from vents.connections.connection import Connection
 from vents.connections.connection_resource import ConnectionResource
 
 
 class ConnectionCatalog(BaseSchemaModel):
     connections: Optional[List[Connection]]
```

### Comparing `vents-0.1.5/vents/connections/connection.py` & `vents-0.2.0/vents/connections/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Optional, Union
 from typing_extensions import Literal
 
+from clipped.compact.pydantic import Field, StrictStr
 from clipped.config.schema import BaseSchemaModel
 from clipped.types.ref_or_obj import RefField
-from pydantic import Field, StrictStr
 
 from vents.connections.connection_resource import ConnectionResource
 from vents.connections.connection_schema import ConnectionSchema
 from vents.providers.kinds import ProviderKind
 
 
 class Connection(BaseSchemaModel):
```

### Comparing `vents-0.1.5/vents/connections/connection_resource.py` & `vents-0.2.0/vents/connections/connection_resource.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional
 
+from clipped.compact.pydantic import Field, StrictStr
 from clipped.config.schema import BaseSchemaModel
-from pydantic import Field, StrictStr
 
 
 class ConnectionResource(BaseSchemaModel):
     _IDENTIFIER = "connection_resource"
 
     name: StrictStr
     mount_path: Optional[StrictStr] = Field(alias="mountPath")
```

### Comparing `vents-0.1.5/vents/connections/connection_schema.py` & `vents-0.2.0/vents/connections/connection_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Union
 
+from clipped.compact.pydantic import Field, StrictStr
 from clipped.config.schema import BaseSchemaModel
 from clipped.types.ref_or_obj import RefField
-from pydantic import Field, StrictStr
 
 
 class BucketConnection(BaseSchemaModel):
     _IDENTIFIER = "bucket"
 
     kind: Optional[
         StrictStr
```

### Comparing `vents-0.1.5/vents/notifiers/__init__.py` & `vents-0.2.0/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/base.py` & `vents-0.2.0/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/discord_webhook.py` & `vents-0.2.0/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/hipchat_webhook.py` & `vents-0.2.0/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/mattermost_webhook.py` & `vents-0.2.0/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/pagerduty_webhook.py` & `vents-0.2.0/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/slack_webhook.py` & `vents-0.2.0/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/notifiers/webhook.py` & `vents-0.2.0/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/aws/base.py` & `vents-0.2.0/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/aws/s3.py` & `vents-0.2.0/vents/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/aws/service.py` & `vents-0.2.0/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/azure/base.py` & `vents-0.2.0/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/azure/blob_storage.py` & `vents-0.2.0/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/azure/service.py` & `vents-0.2.0/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/base.py` & `vents-0.2.0/vents/providers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 
 from typing import TYPE_CHECKING, Any, Optional
 
+from clipped.compact.pydantic import Extra, PrivateAttr
 from clipped.config.schema import BaseSchemaModel
-from pydantic import Extra, PrivateAttr
 
 if TYPE_CHECKING:
     from vents.connections.catalog import ConnectionCatalog
     from vents.connections.connection import Connection
 
 
 class BaseService(BaseSchemaModel):
```

### Comparing `vents-0.1.5/vents/providers/gcp/base.py` & `vents-0.2.0/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/gcp/gcs.py` & `vents-0.2.0/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/gcp/service.py` & `vents-0.2.0/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents/providers/kinds.py` & `vents-0.2.0/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.5/vents.egg-info/PKG-INFO` & `vents-0.2.0/vents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.5
+Version: 0.2.0
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.5/vents.egg-info/SOURCES.txt` & `vents-0.2.0/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

