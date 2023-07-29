# Comparing `tmp/nc_py_api-0.0.25.tar.gz` & `tmp/nc_py_api-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.25.tar", last modified: Mon Jul 24 19:20:45 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.26.tar", last modified: Sat Jul 29 13:19:53 2023, max compression
```

## Comparing `nc_py_api-0.0.25.tar` & `nc_py_api-0.0.26.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13624 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    24442 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/files_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-24 19:20:45.000000 nc_py_api-0.0.25/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 19:20:36.000000 nc_py_api-0.0.25/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-24 19:20:45.594195 nc_py_api-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-24 19:20:23.000000 nc_py_api-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 13:19:53.803912 nc_py_api-0.0.26/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14068 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26651 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4972 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/files_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5620 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7900 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4288 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 13:19:43.000000 nc_py_api-0.0.26/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/setup.py
```

### Comparing `nc_py_api-0.0.25/LICENSE.txt` & `nc_py_api-0.0.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/PKG-INFO` & `nc_py_api-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc_py_api
-Version: 0.0.25
+Version: 0.0.26
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
```

### Comparing `nc_py_api-0.0.25/README.md` & `nc_py_api-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/nc_py_api/__init__.py` & `nc_py_api-0.0.26/nc_py_api/__init__.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/nc_py_api/_session.py` & `nc_py_api-0.0.26/nc_py_api/_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,41 @@
 
 from . import options
 from .constants import OCSRespond
 from .exceptions import NextcloudException, NextcloudExceptionNotFound, check_error
 
 
 class ServerVersion(TypedDict):
+    """Nextcloud version information"""
+
     major: int
+    """Major version"""
     minor: int
+    """Minor version"""
     micro: int
+    """Micro version"""
     string: str
+    """Full version in string format"""
     extended_support: bool
+    """Indicates if the subscription has extended support"""
 
 
 @dataclass
 class BasicConfig:
     endpoint: str
     dav_endpoint: str
     dav_url_suffix: str
 
     def __init__(self, **kwargs):
         full_nc_url = self._get_value("nextcloud_url", **kwargs)
         self.endpoint = full_nc_url.removesuffix("/index.php").removesuffix("/")
         self.dav_url_suffix = self._get_value("dav_url_suffix", raise_not_found=False, **kwargs)
         if not self.dav_url_suffix:
-            self.dav_url_suffix = options.DAV_URL_SUFFIX
+            self.dav_url_suffix = "remote.php/dav"
+        self.dav_url_suffix = "/" + self.dav_url_suffix.strip("/")
         self.dav_endpoint = self.endpoint + self.dav_url_suffix
 
     @staticmethod
     def _get_value(value_name: str, raise_not_found=True, **kwargs):
         value = kwargs.get(value_name, None)
         if not value:
             value = environ.get(value_name.upper(), None)
@@ -62,18 +70,24 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.auth = (self._get_value("nc_auth_user", **kwargs), self._get_value("nc_auth_pass", **kwargs))
 
 
 @dataclass
 class AppConfig(BasicConfig):
+    """Application configuration"""
+
     ae_version: str
+    """AppEcosystem version"""
     app_name: str
+    """Application name"""
     app_version: str
+    """Application version"""
     app_secret: bytes
+    """Application authentication secret"""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.ae_version = self._get_value("ae_version", raise_not_found=False, **kwargs)
         if not self.ae_version:
             self.ae_version = "1.0.0"
         self.app_name = self._get_value("app_id", **kwargs)
```

### Comparing `nc_py_api-0.0.25/nc_py_api/appconfig_preferences_ex.py` & `nc_py_api-0.0.26/nc_py_api/appconfig_preferences_ex.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,15 @@
     def get_values(self, keys: list[str]) -> list[AppCfgPrefRecord]:
         if not keys:
             return []
         if not all(keys):
             raise ValueError("`key` parameter can not be empty")
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         data = {"configKeys": keys}
-        try:
-            return self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self.url_suffix}/get-values", json=data)
-        except NextcloudExceptionNotFound:
-            return []
+        return self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self.url_suffix}/get-values", json=data)
 
     def set(self, key: str, value: str) -> None:
         if not key:
             raise ValueError("`key` parameter can not be empty")
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         params = {"configKey": key, "configValue": value}
         self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self.url_suffix}", json=params)
```

### Comparing `nc_py_api-0.0.25/nc_py_api/exceptions.py` & `nc_py_api-0.0.26/nc_py_api/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Exceptions for the Nextcloud API.
 """
 from httpx import codes
 
 
 class NextcloudException(Exception):
+    """The base exception for all Nextcloud operation errors."""
+
     status_code: int
     reason: str
 
     def __init__(self, status_code: int = 0, reason: str = "", info: str = ""):
         super(BaseException, self).__init__()
         self.status_code = status_code
         self.reason = reason
@@ -17,14 +19,16 @@
     def __str__(self):
         reason = f" {self.reason}" if self.reason else ""
         info = f" <{self.info}>" if self.info else ""
         return f"[{self.status_code}]{reason}{info}"
 
 
 class NextcloudExceptionNotFound(NextcloudException):
+    """The exception that is thrown during operations when the object is not found."""
+
     def __init__(self, reason="Not found", info: str = ""):
         super().__init__(404, reason=reason, info=info)
 
 
 def check_error(code: int, info: str = ""):
     if 996 <= code <= 999:
         if code == 996:
```

### Comparing `nc_py_api-0.0.25/nc_py_api/files.py` & `nc_py_api-0.0.26/nc_py_api/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,133 +8,179 @@
 from datetime import datetime
 from email.utils import parsedate_to_datetime
 from io import BytesIO
 from json import dumps, loads
 from pathlib import Path
 from random import choice
 from string import ascii_lowercase, digits
-from typing import Optional, TypedDict, Union
+from typing import Optional, Union
 from urllib.parse import unquote
 from xml.etree import ElementTree
 
 import xmltodict
 from httpx import Response
 
 from ._session import NcSessionBasic
 from .exceptions import NextcloudException, check_error
 
 
-class FsNodeInfo(TypedDict):
+@dataclass
+class FsNodeInfo:
     """Extra FS object attributes from Nextcloud"""
 
-    nc_id: str
-    """Nextcloud instance ID."""
-    fileid: int
-    """Object file ID."""
-    etag: str
     size: int
+    """Length of file in bytes, zero for directories.."""
     content_length: int
-    last_modified: datetime
+    """For directories it is size of all content in it, for files it is equal to ``size``."""
     permissions: str
     """Permissions for the object."""
     favorite: bool
+    """Flag indicating if the object is marked as favorite."""
+    fileid: int
+    """Clear file ID without Nextcloud instance ID."""
+    _last_modified: datetime
+
+    def __init__(self, **kwargs):
+        self.size = kwargs.get("size", 0)
+        self.content_length = kwargs.get("content_length", 0)
+        self.permissions = kwargs.get("permissions", "")
+        self.favorite = kwargs.get("favorite", False)
+        self.fileid = kwargs.get("fileid", 0)
+        try:
+            self.last_modified = kwargs.get("last_modified", datetime(1970, 1, 1))
+        except (ValueError, TypeError):
+            self.last_modified = datetime(1970, 1, 1)
+
+    @property
+    def last_modified(self) -> datetime:
+        """Time when the object was last modified.
+
+        .. note:: ETag if more preferable way to check if the object was changed."""
+
+        return self._last_modified
+
+    @last_modified.setter
+    def last_modified(self, value: Union[str, datetime]):
+        if isinstance(value, str):
+            self._last_modified = parsedate_to_datetime(value)
+        else:
+            self._last_modified = value
 
 
 @dataclass
 class FsNode:
     """A class that represents a Nextcloud file object.
 
     Acceptable itself as a ``path`` parameter for the most file APIs."""
 
-    user: str
-    """The username of the object. May be different from the owner of the object if it is shared."""
+    full_path: str
+    """Path to the object, including the username. Does not include `dav` prefix"""
 
-    path: str
-    """Path to the object. Does not include the username, but includes the object name."""
+    file_id: str
+    """File ID + NC instance ID"""
 
-    name: str
-    """last ``pathname`` component."""
+    etag: str
+    """An entity tag (ETag) of the object"""
 
-    def __init__(self, user: str, path: str, name: str, **kwargs):
-        self.user = user
-        self.path = path
-        self.name = name
-        self.info: FsNodeInfo = {
-            "nc_id": kwargs.get("nc_id", ""),
-            "fileid": kwargs.get("fileid", 0),
-            "etag": kwargs.get("etag", ""),
-            "size": kwargs.get("size", 0),
-            "content_length": kwargs.get("content_length", 0),
-            "last_modified": datetime(1970, 1, 1),
-            "permissions": kwargs.get("permissions", ""),
-            "favorite": kwargs.get("favorite", False),
-        }
-        if "last_modified" in kwargs:
-            self.last_modified = kwargs["last_modified"]
+    info: FsNodeInfo
+    """Additional extra information for the object"""
 
-    @property
-    def last_modified(self) -> datetime:
-        return self.info["last_modified"]
-
-    @last_modified.setter
-    def last_modified(self, value: Union[str, datetime]):
-        if isinstance(value, str):
-            self.info["last_modified"] = parsedate_to_datetime(value)
-        else:
-            self.info["last_modified"] = value
+    def __init__(self, full_path: str, **kwargs):
+        self.full_path = full_path
+        self.file_id = kwargs.get("file_id", "")
+        self.etag = kwargs.get("etag", "")
+        self.info = FsNodeInfo(**kwargs)
 
     @property
     def is_dir(self) -> bool:
         """Returns ``True`` for the directories, ``False`` otherwise."""
 
-        return self.path.endswith("/")
-
-    @property
-    def full_path(self) -> str:
-        """Full path including username."""
-
-        return f"{self.user}/{self.path.lstrip('/')}" if self.user else self.path
+        return self.full_path.endswith("/")
 
     def __str__(self):
         return (
-            f"{'Dir' if self.is_dir else 'File'}: `{self.name}` with id={self.info['fileid']}"
-            f" last modified at {str(self.last_modified)} and {self.info['permissions']} permissions."
+            f"{'Dir' if self.is_dir else 'File'}: `{self.name}` with id={self.file_id}"
+            f" last modified at {str(self.info.last_modified)} and {self.info.permissions} permissions."
         )
 
+    def __eq__(self, other):
+        if self.file_id and self.file_id == other.file_id:
+            return True
+        return False
+
+    @property
+    def has_extra(self) -> bool:
+        """Flag indicating whether this ``FsNode`` was obtained by the `mkdir` or `upload`
+        methods and does not contain extended information."""
+
+        return bool(self.info.permissions)
+
+    @property
+    def name(self) -> str:
+        """Returns last ``pathname`` component."""
+
+        return self.full_path.rstrip("/").rsplit("/", maxsplit=1)[-1]
+
+    @property
+    def user(self) -> str:
+        """Returns user ID extracted from the `full_path`."""
+
+        return self.full_path.lstrip("/").split("/", maxsplit=2)[1]
+
+    @property
+    def user_path(self) -> str:
+        """Returns path relative to the user's root directory."""
+
+        return self.full_path.lstrip("/").split("/", maxsplit=2)[-1]
+
     @property
     def is_shared(self) -> bool:
-        return self.info["permissions"].find("S") != -1
+        """Check if a file or folder is shared"""
+
+        return self.info.permissions.find("S") != -1
 
     @property
     def is_shareable(self) -> bool:
-        return self.info["permissions"].find("R") != -1
+        """Check if a file or folder can be shared"""
+
+        return self.info.permissions.find("R") != -1
 
     @property
     def is_mounted(self) -> bool:
-        return self.info["permissions"].find("M") != -1
+        """Check if a file or folder is mounted"""
+
+        return self.info.permissions.find("M") != -1
 
     @property
     def is_readable(self) -> bool:
-        return self.info["permissions"].find("G") != -1
+        """Check if the file or folder is readable"""
+
+        return self.info.permissions.find("G") != -1
 
     @property
     def is_deletable(self) -> bool:
-        return self.info["permissions"].find("D") != -1
+        """Check if a file or folder can be deleted"""
+
+        return self.info.permissions.find("D") != -1
 
     @property
     def is_updatable(self) -> bool:
+        """Check if file/directory is writable"""
+
         if self.is_dir:
-            return self.info["permissions"].find("NV") != -1
-        return self.info["permissions"].find("W") != -1
+            return self.info.permissions.find("NV") != -1
+        return self.info.permissions.find("W") != -1
 
     @property
     def is_creatable(self) -> bool:
+        """Check whether new files or folders can be created inside this folder"""
+
         if not self.is_dir:
             return False
-        return self.info["permissions"].find("CK") != -1
+        return self.info.permissions.find("CK") != -1
 
 
 PROPFIND_PROPERTIES = [
     "d:resourcetype",
     "d:getlastmodified",
     "d:getcontentlength",
     "d:getetag",
@@ -169,215 +215,229 @@
 
 class FilesAPI:
     """This class provides all WebDAV functionality related to the files."""
 
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
-    def listdir(self, path: Union[str, FsNode] = "", exclude_self=True) -> list[FsNode]:
+    def listdir(self, path: Union[str, FsNode] = "", depth: int = 1, exclude_self=True) -> list[FsNode]:
         """Returns a list of all entries in the specified directory.
 
-        :param path: Path to the directory to get the list.
-        :param exclude_self: Boolean value indicating whether the `path` itself should be excluded from the list or not.
+        :param path: path to the directory to get the list.
+        :param depth: how many directory levels should be included in output. Default = **1** (only specified directory)
+        :param exclude_self: boolean value indicating whether the `path` itself should be excluded from the list or not.
             Default = **True**.
         """
 
+        if exclude_self and not depth:
+            raise ValueError("Wrong input parameters, query will return nothing.")
         properties = PROPFIND_PROPERTIES
-        path = path.path if isinstance(path, FsNode) else path
-        return self._listdir(self._session.user, path, properties=properties, exclude_self=exclude_self)
+        path = path.user_path if isinstance(path, FsNode) else path
+        return self._listdir(self._session.user, path, properties=properties, depth=depth, exclude_self=exclude_self)
 
-    def by_id(self, fileid: int) -> Optional[FsNode]:
-        """Returns :py:class:`FsNode` by fileid if any."""
+    def by_id(self, file_id: Union[int, str, FsNode]) -> Optional[FsNode]:
+        """Returns :py:class:`FsNode` by file_id if any.
+
+        :param file_id: can be full file ID with Nextcloud instance ID or only clear file ID.
+        """
 
-        result = self.find(req=["eq", "fileid", fileid])
+        file_id = file_id.file_id if isinstance(file_id, FsNode) else file_id
+        result = self.find(req=["eq", "fileid", file_id])
         return result[0] if result else None
 
-    def by_path(self, path: str) -> Optional[FsNode]:
+    def by_path(self, path: Union[str, FsNode]) -> Optional[FsNode]:
         """Returns :py:class:`FsNode` by exact path if any."""
 
-        result = self.listdir(path, exclude_self=False)
+        path = path.user_path if isinstance(path, FsNode) else path
+        result = self.listdir(path, depth=0, exclude_self=False)
         return result[0] if result else None
 
-    def find(self, req: list, path: Union[str, FsNode] = "", depth=-1) -> list[FsNode]:
+    def find(self, req: list, path: Union[str, FsNode] = "") -> list[FsNode]:
         """Searches a directory for a file or subdirectory with a name.
 
         :param req: list of conditions to search for. Detailed description here...
-        :param path: Path where to search from. Default = **""**.
-        :param depth: In how many levels of subdirectories to search. Default = **-1**.
+        :param path: path where to search from. Default = **""**.
         """
 
         # `req` possible keys: "name", "mime", "last_modified", "size", "favorite", "fileid"
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         root = ElementTree.Element(
             "d:searchrequest",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns", "xmlns:nc": "http://nextcloud.org/ns"},
         )
         xml_search = ElementTree.SubElement(root, "d:basicsearch")
         xml_select_prop = ElementTree.SubElement(ElementTree.SubElement(xml_search, "d:select"), "d:prop")
         for i in PROPFIND_PROPERTIES:
             ElementTree.SubElement(xml_select_prop, i)
         xml_from_scope = ElementTree.SubElement(ElementTree.SubElement(xml_search, "d:from"), "d:scope")
-        if path.startswith("/"):
-            href = f"/files/{self._session.user}{path}"
-        else:
-            href = f"/files/{self._session.user}/{path}"
+        href = f"/files/{self._session.user}/{path.removeprefix('/')}"
         ElementTree.SubElement(xml_from_scope, "d:href").text = href
-        xml_from_scope_depth = ElementTree.SubElement(xml_from_scope, "d:depth")
-        if depth == -1:
-            xml_from_scope_depth.text = "infinity"
-        else:
-            xml_from_scope_depth.text = str(depth)
+        ElementTree.SubElement(xml_from_scope, "d:depth").text = "infinity"
         xml_where = ElementTree.SubElement(xml_search, "d:where")
         self._build_search_req(xml_where, req)
 
         headers = {"Content-Type": "text/xml"}
         webdav_response = self._session.dav("SEARCH", "", data=self._element_tree_as_str(root), headers=headers)
-        request_info = f"find: {self._session.user}, {req}, {path}, {depth}"
-        return self._lf_parse_webdav_records(webdav_response, self._session.user, request_info)
+        request_info = f"find: {self._session.user}, {req}, {path}"
+        return self._lf_parse_webdav_records(webdav_response, request_info)
 
     def download(self, path: Union[str, FsNode]) -> bytes:
         """Downloads and returns the content of a file.
 
-        :param path: Path to download file.
+        :param path: path to download file.
         """
 
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         response = self._session.dav("GET", self._dav_get_obj_path(self._session.user, path))
         check_error(response.status_code, f"download: user={self._session.user}, path={path}")
         return response.content
 
     def download2stream(self, path: Union[str, FsNode], fp, **kwargs) -> None:
         """Downloads file to the given `fp` object.
 
-        :param path: Path to download file.
-        :param fp: A filename (string), pathlib.Path object or a file object.
+        :param path: path to download file.
+        :param fp: filename (string), pathlib.Path object or a file object.
             The object must implement the ``file.write`` method and be able to write binary data.
         :param kwargs: **chunk_size** an int value specifying chunk size to write. Default = **4Mb**
         """
 
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         if isinstance(fp, (str, Path)):
             with builtins.open(fp, "wb") as f:
                 self.__download2stream(path, f, **kwargs)
         elif hasattr(fp, "write"):
             self.__download2stream(path, fp, **kwargs)
         else:
             raise TypeError("`fp` must be a path to file or an object with `write` method.")
 
-    def upload(self, path: Union[str, FsNode], content: Union[bytes, str]) -> None:
+    def upload(self, path: Union[str, FsNode], content: Union[bytes, str]) -> FsNode:
         """Creates a file with the specified content at the specified path.
 
-        :param path: File upload path.
+        :param path: file's upload path.
         :param content: content to create the file. If it is a string, it will be encoded into bytes using UTF-8.
         """
 
-        path = path.path if isinstance(path, FsNode) else path
-        response = self._session.dav("PUT", self._dav_get_obj_path(self._session.user, path), data=content)
+        path = path.user_path if isinstance(path, FsNode) else path
+        full_path = self._dav_get_obj_path(self._session.user, path)
+        response = self._session.dav("PUT", full_path, data=content)
         check_error(response.status_code, f"upload: user={self._session.user}, path={path}, size={len(content)}")
+        return FsNode(full_path.strip("/"), **self.__get_etag_fileid_from_response(response))
 
-    def upload_stream(self, path: Union[str, FsNode], fp, **kwargs) -> None:
+    def upload_stream(self, path: Union[str, FsNode], fp, **kwargs) -> FsNode:
         """Creates a file with content provided by `fp` object at the specified path.
 
-        :param path: File upload path.
-        :param fp: A filename (string), pathlib.Path object or a file object.
+        :param path: file's upload path.
+        :param fp: filename (string), pathlib.Path object or a file object.
             The object must implement the ``file.read`` method providing data with str or bytes type.
         :param kwargs: **chunk_size** an int value specifying chunk size to read. Default = **4Mb**
         """
 
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         if isinstance(fp, (str, Path)):
             with builtins.open(fp, "rb") as f:
-                self.__upload_stream(path, f, **kwargs)
+                return self.__upload_stream(path, f, **kwargs)
         elif hasattr(fp, "read"):
-            self.__upload_stream(path, fp, **kwargs)
+            return self.__upload_stream(path, fp, **kwargs)
         else:
             raise TypeError("`fp` must be a path to file or an object with `read` method.")
 
-    def mkdir(self, path: Union[str, FsNode]) -> None:
+    def mkdir(self, path: Union[str, FsNode]) -> FsNode:
         """Creates a new directory.
 
-        :param path: The path of the directory to be created.
+        :param path: path of the directory to be created.
         """
 
-        path = path.path if isinstance(path, FsNode) else path
-        response = self._session.dav("MKCOL", self._dav_get_obj_path(self._session.user, path))
+        path = path.user_path if isinstance(path, FsNode) else path
+        full_path = self._dav_get_obj_path(self._session.user, path)
+        response = self._session.dav("MKCOL", full_path)
         check_error(response.status_code, f"mkdir: user={self._session.user}, path={path}")
+        full_path += "/" if not full_path.endswith("/") else ""
+        return FsNode(full_path.lstrip("/"), **self.__get_etag_fileid_from_response(response))
 
-    def makedirs(self, path: Union[str, FsNode], exist_ok=False) -> None:
+    def makedirs(self, path: Union[str, FsNode], exist_ok=False) -> Optional[FsNode]:
         """Creates a new directory and subdirectories.
 
-        :param path: The path of the directories to be created.
-        :param exist_ok: Ignore error if any of pathname components already exists.
+        :param path: path of the directories to be created.
+        :param exist_ok: ignore error if any of pathname components already exists.
+        :returns: `FsNode` if directory was created or ``None`` if it was already created.
         """
 
         _path = ""
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
+        result = None
         for i in Path(path).parts:
             _path = os.path.join(_path, i)
             if not exist_ok:
-                self.mkdir(_path)
+                result = self.mkdir(_path)
             else:
                 try:
-                    self.mkdir(_path)
+                    result = self.mkdir(_path)
                 except NextcloudException as e:
                     if e.status_code != 405:
                         raise e from None
+        return result
 
     def delete(self, path: Union[str, FsNode], not_fail=False) -> None:
         """Deletes a file/directory (moves to trash if trash is enabled).
 
-        :param path: Path to delete.
-        :param not_fail: if set to ``True`` and object is not found, does not raise an exception.
+        :param path: path to delete.
+        :param not_fail: if set to ``True`` and the object is not found, it does not raise an exception.
         """
 
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         response = self._session.dav("DELETE", self._dav_get_obj_path(self._session.user, path))
         if response.status_code == 404 and not_fail:
             return
         check_error(response.status_code, f"delete: user={self._session.user}, path={path}")
 
-    def move(self, path_src: Union[str, FsNode], path_dest: Union[str, FsNode], overwrite=False) -> None:
+    def move(self, path_src: Union[str, FsNode], path_dest: Union[str, FsNode], overwrite=False) -> FsNode:
         """Moves an existing file or a directory.
 
-        :param path_src: The path of an existing file/directory.
-        :param path_dest: The name of the new one.
-        :param overwrite: If ``True`` and destination object already exists it gets overwritten.
+        :param path_src: path of an existing file/directory.
+        :param path_dest: name of the new one.
+        :param overwrite: if ``True`` and the destination object already exists, it gets overwritten.
             Default = **False**.
         """
 
-        path_src = path_src.path if isinstance(path_src, FsNode) else path_src
-        path_dest = path_dest.path if isinstance(path_dest, FsNode) else path_dest
-        dest = self._session.cfg.dav_endpoint + self._dav_get_obj_path(self._session.user, path_dest)
+        path_src = path_src.user_path if isinstance(path_src, FsNode) else path_src
+        full_dest_path = self._dav_get_obj_path(
+            self._session.user, path_dest.user_path if isinstance(path_dest, FsNode) else path_dest
+        )
+        dest = self._session.cfg.dav_endpoint + full_dest_path
         headers = {"Destination": dest, "Overwrite": "T" if overwrite else "F"}
         response = self._session.dav(
             "MOVE",
             self._dav_get_obj_path(self._session.user, path_src),
             headers=headers,
         )
         check_error(response.status_code, f"move: user={self._session.user}, src={path_src}, dest={dest}, {overwrite}")
+        return self.find(req=["eq", "fileid", response.headers["OC-FileId"]])[0]
 
-    def copy(self, path_src: Union[str, FsNode], path_dest: Union[str, FsNode], overwrite=False) -> None:
+    def copy(self, path_src: Union[str, FsNode], path_dest: Union[str, FsNode], overwrite=False) -> FsNode:
         """Copies an existing file/directory.
 
-        :param path_src: The path of an existing file/directory.
-        :param path_dest: The name of the new one.
-        :param overwrite: If ``True`` and destination object already exists it gets overwritten.
+        :param path_src: path of an existing file/directory.
+        :param path_dest: name of the new one.
+        :param overwrite: if ``True`` and the destination object already exists, it gets overwritten.
             Default = **False**.
         """
 
-        path_src = path_src.path if isinstance(path_src, FsNode) else path_src
-        path_dest = path_dest.path if isinstance(path_dest, FsNode) else path_dest
-        dest = self._session.cfg.dav_endpoint + self._dav_get_obj_path(self._session.user, path_dest)
+        path_src = path_src.user_path if isinstance(path_src, FsNode) else path_src
+        full_dest_path = self._dav_get_obj_path(
+            self._session.user, path_dest.user_path if isinstance(path_dest, FsNode) else path_dest
+        )
+        dest = self._session.cfg.dav_endpoint + full_dest_path
         headers = {"Destination": dest, "Overwrite": "T" if overwrite else "F"}
         response = self._session.dav(
             "COPY",
             self._dav_get_obj_path(self._session.user, path_src),
             headers=headers,
         )
         check_error(response.status_code, f"copy: user={self._session.user}, src={path_src}, dest={dest}, {overwrite}")
+        return self.find(req=["eq", "fileid", response.headers["OC-FileId"]])[0]
 
     def listfav(self) -> list[FsNode]:
         """Returns a list of the current user's favorite files."""
 
         root = ElementTree.Element(
             "oc:filter-files",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns", "xmlns:nc": "http://nextcloud.org/ns"},
@@ -385,121 +445,110 @@
         xml_filter_rules = ElementTree.SubElement(root, "oc:filter-rules")
         ElementTree.SubElement(xml_filter_rules, "oc:favorite").text = "1"
         webdav_response = self._session.dav(
             "REPORT", self._dav_get_obj_path(self._session.user), data=self._element_tree_as_str(root)
         )
         request_info = f"listfav: {self._session.user}"
         check_error(webdav_response.status_code, request_info)
-        return self._lf_parse_webdav_records(webdav_response, self._session.user, request_info, favorite=True)
+        return self._lf_parse_webdav_records(webdav_response, request_info, favorite=True)
 
     def setfav(self, path: Union[str, FsNode], value: Union[int, bool]) -> None:
         """Sets or unsets favourite flag for specific file.
 
-        :param path: Path to the object to set the state.
-        :param value: The value to set for the ``favourite`` state.
+        :param path: path to the object to set the state.
+        :param value: value to set for the ``favourite`` state.
         """
 
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         root = ElementTree.Element(
             "d:propertyupdate",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns"},
         )
         xml_set = ElementTree.SubElement(root, "d:set")
         xml_set_prop = ElementTree.SubElement(xml_set, "d:prop")
         ElementTree.SubElement(xml_set_prop, "oc:favorite").text = str(int(bool(value)))
         webdav_response = self._session.dav(
             "PROPPATCH", self._dav_get_obj_path(self._session.user, path), data=self._element_tree_as_str(root)
         )
         check_error(webdav_response.status_code, f"setfav: path={path}, value={value}")
 
-    def _listdir(self, user: str, path: str, properties: list[str], exclude_self: bool) -> list[FsNode]:
+    def _listdir(self, user: str, path: str, properties: list[str], depth: int, exclude_self: bool) -> list[FsNode]:
         root = ElementTree.Element(
             "d:propfind",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns", "xmlns:nc": "http://nextcloud.org/ns"},
         )
         prop = ElementTree.SubElement(root, "d:prop")
         for i in properties:
             ElementTree.SubElement(prop, i)
+        headers = {"Depth": "infinity" if depth == -1 else str(depth)}
         webdav_response = self._session.dav(
-            "PROPFIND", self._dav_get_obj_path(user, path), data=self._element_tree_as_str(root)
+            "PROPFIND", self._dav_get_obj_path(user, path), data=self._element_tree_as_str(root), headers=headers
         )
         request_info = f"list: {user}, {path}, {properties}"
-        result = self._lf_parse_webdav_records(webdav_response, user, request_info)
+        result = self._lf_parse_webdav_records(webdav_response, request_info)
         if exclude_self:
-            full_path = f"{user}/{path}".rstrip("/") if user else path.rstrip("/")
             for index, v in enumerate(result):
-                if v.full_path.rstrip("/") == full_path:
+                if v.user_path.rstrip("/") == path.rstrip("/"):
                     del result[index]
                     break
         return result
 
-    def _parse_records(self, fs_records: list[dict], user: str, favorite: bool):
+    def _parse_records(self, fs_records: list[dict], favorite: bool):
         result: list[FsNode] = []
         for record in fs_records:
             obj_full_path = unquote(record.get("d:href", ""))
-            obj_name = obj_full_path.rstrip("/").rsplit("/", maxsplit=1)[-1]
-            if not obj_name:
-                continue
-            dav_full_path = self._session.cfg.dav_url_suffix + self._dav_get_obj_path(user)
-            obg_rel_path = obj_full_path.replace(dav_full_path, "").lstrip("/")
+            obj_full_path = obj_full_path.replace(self._session.cfg.dav_url_suffix, "").lstrip("/")
             propstat = record["d:propstat"]
-            fs_node = self._parse_record(
-                propstat if isinstance(propstat, list) else [propstat], user, obg_rel_path, obj_name
-            )
-            if favorite and not fs_node.info["fileid"]:
-                _fs_node = self.by_path(fs_node.path)
+            fs_node = self._parse_record(obj_full_path, propstat if isinstance(propstat, list) else [propstat])
+            if favorite and not fs_node.file_id:
+                _fs_node = self.by_path(fs_node.user_path)
                 if _fs_node:
-                    _fs_node.info["favorite"] = True
+                    _fs_node.info.favorite = True
                     result.append(_fs_node)
-            elif fs_node.info["fileid"]:
+            elif fs_node.file_id:
                 result.append(fs_node)
         return result
 
     @staticmethod
-    def _parse_record(prop_stats: list[dict], user: str, obj_rel_path: str, obj_name: str) -> FsNode:
-        fs_node = FsNode(user=user, path=obj_rel_path, name=obj_name)
+    def _parse_record(full_path: str, prop_stats: list[dict]) -> FsNode:
+        fs_node_args = {}
         for prop_stat in prop_stats:
             if str(prop_stat.get("d:status", "")).find("200 OK") == -1:
                 continue
             prop: dict = prop_stat["d:prop"]
             prop_keys = prop.keys()
             if "oc:id" in prop_keys:
-                fs_node.info["nc_id"] = prop["oc:id"]
+                fs_node_args["file_id"] = prop["oc:id"]
             if "oc:fileid" in prop_keys:
-                fs_node.info["fileid"] = int(prop["oc:fileid"])
+                fs_node_args["fileid"] = int(prop["oc:fileid"])
             if "oc:size" in prop_keys:
-                fs_node.info["size"] = int(prop["oc:size"])
+                fs_node_args["size"] = int(prop["oc:size"])
             if "d:getcontentlength" in prop_keys:
-                fs_node.info["content_length"] = int(prop["d:getcontentlength"])
+                fs_node_args["content_length"] = int(prop["d:getcontentlength"])
             if "d:getetag" in prop_keys:
-                fs_node.info["etag"] = prop["d:getetag"]
+                fs_node_args["etag"] = prop["d:getetag"]
             if "d:getlastmodified" in prop_keys:
-                try:
-                    fs_node.last_modified = prop["d:getlastmodified"]
-                except ValueError:
-                    pass
+                fs_node_args["last_modified"] = prop["d:getlastmodified"]
             if "oc:permissions" in prop_keys:
-                fs_node.info["permissions"] = prop["oc:permissions"]
+                fs_node_args["permissions"] = prop["oc:permissions"]
             if "oc:favorite" in prop_keys:
-                fs_node.info["favorite"] = bool(int(prop["oc:favorite"]))
+                fs_node_args["favorite"] = bool(int(prop["oc:favorite"]))
             # xz = prop.get("oc:dDC", "")
-        return fs_node
+        return FsNode(full_path, **fs_node_args)
 
-    def _lf_parse_webdav_records(self, webdav_res: Response, user: str, info: str, favorite=False) -> list[FsNode]:
+    def _lf_parse_webdav_records(self, webdav_res: Response, info: str, favorite=False) -> list[FsNode]:
         check_error(webdav_res.status_code, info=info)
         if webdav_res.status_code != 207:  # multistatus
             raise NextcloudException(webdav_res.status_code, "Response is not a multistatus.", info=info)
-        if not webdav_res.text:
-            raise NextcloudException(webdav_res.status_code, "Response is empty.", info=info)
         response_data = loads(dumps(xmltodict.parse(webdav_res.text)))
         if "d:error" in response_data:
             err = response_data["d:error"]
             raise NextcloudException(reason=f'{err["s:exception"]}: {err["s:message"]}'.replace("\n", ""), info=info)
         response = response_data["d:multistatus"].get("d:response", [])
-        return self._parse_records([response] if isinstance(response, dict) else response, user, favorite)
+        return self._parse_records([response] if isinstance(response, dict) else response, favorite)
 
     @staticmethod
     def _dav_get_obj_path(user: str, path: str = "", root_path="/files") -> str:
         obj_dav_path = root_path
         if user:
             obj_dav_path += "/" + user
         if path:
@@ -543,16 +592,16 @@
         with self._session.dav_stream(
             "GET", self._dav_get_obj_path(self._session.user, path)
         ) as response:  # type: ignore
             check_error(response.status_code, f"download_stream: user={self._session.user}, path={path}")
             for data_chunk in response.iter_raw(chunk_size=kwargs.get("chunk_size", 4 * 1024 * 1024)):
                 fp.write(data_chunk)
 
-    def __upload_stream(self, path: str, fp, **kwargs) -> None:
-        _rnd_folder = "".join(choice(digits + ascii_lowercase) for i in range(64))
+    def __upload_stream(self, path: str, fp, **kwargs) -> FsNode:
+        _rnd_folder = "".join(choice(digits + ascii_lowercase) for _ in range(64))
         _dav_path = self._dav_get_obj_path(self._session.user, _rnd_folder, root_path="/uploads")
         response = self._session.dav("MKCOL", _dav_path)
         check_error(response.status_code)
         try:
             chunk_size = kwargs.get("chunk_size", 4 * 1024 * 1024)
             start_bytes = end_bytes = 0
             while True:
@@ -562,18 +611,24 @@
                 end_bytes = start_bytes + len(piece)
                 _filename = str(start_bytes).rjust(15, "0") + "-" + str(end_bytes).rjust(15, "0")
                 response = self._session.dav("PUT", _dav_path + "/" + _filename, data=piece)
                 check_error(
                     response.status_code, f"upload_stream: user={self._session.user}, path={path}, cur_size={end_bytes}"
                 )
                 start_bytes = end_bytes
-            headers = {"Destination": self._session.cfg.dav_endpoint + self._dav_get_obj_path(self._session.user, path)}
+            full_path = self._dav_get_obj_path(self._session.user, path)
+            headers = {"Destination": self._session.cfg.dav_endpoint + full_path}
             response = self._session.dav(
                 "MOVE",
                 _dav_path + "/.file",
                 headers=headers,
             )
             check_error(
                 response.status_code, f"upload_stream: user={self._session.user}, path={path}, total_size={end_bytes}"
             )
+            return FsNode(full_path.strip("/"), **self.__get_etag_fileid_from_response(response))
         finally:
             self._session.dav("DELETE", _dav_path)
+
+    @staticmethod
+    def __get_etag_fileid_from_response(response: Response) -> dict:
+        return {"etag": response.headers.get("OC-Etag", ""), "file_id": response.headers["OC-FileId"]}
```

### Comparing `nc_py_api-0.0.25/nc_py_api/files_sharing.py` & `nc_py_api-0.0.26/nc_py_api/files_sharing.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     def get_list(
         self, shared_with_me=False, reshares=False, subfiles=False, path: Union[str, FsNode] = ""
     ) -> list[Share]:
         """Returns lists of shares."""
 
         require_capabilities("files_sharing", self._session.capabilities)
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         params = {
             "shared_with_me": "true" if shared_with_me else "false",
             "reshares": "true" if reshares else "false",
             "subfiles": "true" if subfiles else "false",
         }
         if path:
             params["path"] = path
@@ -92,33 +92,30 @@
     ) -> Share:
         """Creates a new share.
 
         :param path: The path of an existing file/directory.
         :param permissions: combination of the :py:class:`~nc_py_api.SharePermissions` object values.
         :param share_type: :py:class:`~nc_py_api.ShareType` value.
         :param share_with: the recipient of the shared object.
-        :param kwargs: *Additionally supported arguments*
+        :param kwargs: See below.
 
         Additionally supported arguments:
-            ``public`` - boolean indicating should share be available for non-registered users.
-                default = ``False``
-            ``password`` - string with password to protect share.
-                default = ``""``
-            ``send_password_by_talk`` - boolean indicating should password be automatically delivered using Talk.
-                default = ``False``
-            ``expire_date`` - py:class:`datetime` time when share should expire. `hours, minutes, seconds` are ignored.
-                default = None
-            ``note`` - string with note, if any.
-                default = ``""``
-            ``label`` - string with label, if any.
-                default = ``""``
+
+            * ``public`` - boolean indicating should share be available for non-registered users. default = ``False``
+            * ``password`` - string with password to protect share. default = ``""``
+            * ``send_password_by_talk`` - boolean indicating should password be automatically delivered using Talk.
+              default = ``False``
+            * ``expire_date`` - :py:class:`~datetime.datetime` time when share should expire.
+              `hours, minutes, seconds` are ignored. default = ``None``
+            * ``note`` - string with note, if any. default = ``""``
+            * ``label`` - string with label, if any. default = ``""``
         """
 
         require_capabilities("files_sharing", self._session.capabilities)
-        path = path.path if isinstance(path, FsNode) else path
+        path = path.user_path if isinstance(path, FsNode) else path
         params = {
             "path": path,
             "permissions": int(permissions),
             "shareType": int(share_type),
         }
         if share_with:
             kwargs["shareWith"] = share_with
```

### Comparing `nc_py_api-0.0.25/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.26/nc_py_api/integration_fastapi.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/nc_py_api/misc.py` & `nc_py_api-0.0.26/nc_py_api/misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/nc_py_api/preferences.py` & `nc_py_api-0.0.26/nc_py_api/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Nextcloud API for working with classics app's storage with user context(table oc_preferences).
+Nextcloud API for working with classics app's storage with user's context (table oc_preferences).
 """
 
 from ._session import NcSessionBasic
 from .misc import check_capabilities, require_capabilities
 
 ENDPOINT = "/ocs/v1.php/apps/provisioning_api/api/v1/config/users"
```

### Comparing `nc_py_api-0.0.25/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.26/nc_py_api/ui_files_actions_menu.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.26/nc_py_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc-py-api
-Version: 0.0.25
+Version: 0.0.26
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
```

### Comparing `nc_py_api-0.0.25/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.26/nc_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/pyproject.toml` & `nc_py_api-0.0.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.25/setup.cfg` & `nc_py_api-0.0.26/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 python_requires = >=3.9
 zip_safe = True
 packages = find:
 install_requires = 
 	requests==2.31.0
 	httpx==0.24.1
 	xmltodict==0.13.0
-	pydantic==2.0.3
+	pydantic==2.1.1
 	xxhash==3.2.0
-	fastapi==0.100.0
+	fastapi==0.100.1
 	uvicorn[standard]==0.23.1
 
 [options.extras_require]
 docs = 
-	sphinx>=4.4
+	sphinx>=6.2
 	sphinx-issues>=3.0.1
 	sphinx-rtd-theme>=1.0
 	sphinx-copybutton
 	sphinx-inline-tabs
 bench = 
 	matplotlib
 	py-cpuinfo
```

