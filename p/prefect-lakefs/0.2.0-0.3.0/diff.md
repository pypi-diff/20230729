# Comparing `tmp/prefect-lakefs-0.2.0.tar.gz` & `tmp/prefect-lakefs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-lakefs-0.2.0.tar", last modified: Mon Jul 24 22:29:30 2023, max compression
+gzip compressed data, was "prefect-lakefs-0.3.0.tar", last modified: Sat Jul 29 01:04:40 2023, max compression
```

## Comparing `prefect-lakefs-0.2.0.tar` & `prefect-lakefs-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.601976 prefect-lakefs-0.2.0/prefect_lakefs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 22:29:30.601976 prefect-lakefs-0.2.0/prefect_lakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/commits.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 22:29:30.601976 prefect-lakefs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_commits.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:04:40.680229 prefect-lakefs-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-29 01:04:40.680229 prefect-lakefs-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:04:40.680229 prefect-lakefs-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:04:40.680229 prefect-lakefs-0.3.0/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/examples/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/examples/storage/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:04:40.684229 prefect-lakefs-0.3.0/prefect_lakefs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-29 01:04:40.684229 prefect-lakefs-0.3.0/prefect_lakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/prefect_lakefs/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:04:40.680229 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-29 01:04:40.000000 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-29 01:04:40.000000 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 01:04:40.000000 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-29 01:04:40.000000 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-29 01:04:40.000000 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 01:04:40.000000 prefect-lakefs-0.3.0/prefect_lakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-29 01:04:40.684229 prefect-lakefs-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 01:04:40.680229 prefect-lakefs-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-29 01:03:51.000000 prefect-lakefs-0.3.0/versioneer.py
```

### Comparing `prefect-lakefs-0.2.0/LICENSE` & `prefect-lakefs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/PKG-INFO` & `prefect-lakefs-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-lakefs
-Version: 0.2.0
+Version: 0.3.0
 Summary: Prefect integrations for interacting with LakeFS services.
 Home-page: https://github.com/limx0/prefect-lakefs
 Author: limx0
 Author-email: limx0@example.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-lakefs-0.2.0/README.md` & `prefect-lakefs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs/branches.py` & `prefect-lakefs-0.3.0/prefect_lakefs/branches.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs/commits.py` & `prefect-lakefs-0.3.0/prefect_lakefs/commits.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs/credentials.py` & `prefect-lakefs-0.3.0/prefect_lakefs/credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from contextlib import contextmanager
 from typing import Generator, Optional, Union
 
 from lakefs_client import ApiClient
-from lakefs_client.apis import BranchesApi, CommitsApi, ObjectsApi
+from lakefs_client.apis import BranchesApi, CommitsApi, ObjectsApi, RefsApi
 from lakefs_client.client import LakeFSClient
 from lakefs_client.configuration import Configuration
 from prefect.blocks.core import Block
 from prefect.utilities.collections import listrepr
 from pydantic import Field, SecretStr
 from typing_extensions import Literal
 
 LAKEFS_CLIENT_TYPES = {
     "branches": BranchesApi,
     "commits": CommitsApi,
     "objects": ObjectsApi,
+    "refs": RefsApi,
 }
 
 
 class LakeFSCredentials(Block):
 
     """Credentials block for generating configured LakeFS API clients.
 
@@ -54,26 +55,30 @@
         description="Default LakeFS repository to use.",
         title="Default LakeFS repository",
     )
     branch: Optional[str] = Field(
         description="Default LakeFS branch to use.",
         title="Default LakeFS branch",
     )
+    commit_on_task: Optional[bool] = Field(
+        description="Commit on each task run.",
+        title="Commit on task",
+    )
     _block_type_name = "LakeFS Credentials"
     _block_type_slug = "lakefs-credentials"
     # TODO: add lakefs logo_url
     _logo_url = "https://styles.redditmedia.com/t5_57y5vj/styles/communityIcon_oapa1t4myyu71.png?width=256&v=enabled&s=d3319b91ef0a5eea78e46242e07f2034834f31f7"  # noqa
     # TODO: add LakeFSCredentials doc slug
     _documentation_url = "https://prefecthq.github.io"  # noqa
     _documentation_url = "https://limx0.github.io/prefect-lakefs/credentials/#prefect_lakefs.credentials.LakeFSCredentials"  # noqa
 
     @contextmanager
     def get_client(
         self,
-        client_type: Literal["branches", "commits", "objects", "repository"],
+        client_type: Literal["branches", "commits", "objects", "repository", "refs"],
     ) -> Generator[LakeFSClient, None, None]:
         """Convenience method for retrieving a LakeFS API client for deployment resources.
 
         Args:
             client_type: The resource-specific type of LakeFS client to retrieve.
 
         Yields:
```

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs/objects.py` & `prefect-lakefs-0.3.0/prefect_lakefs/objects.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs/storage.py` & `prefect-lakefs-0.3.0/prefect_lakefs/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 import io
 
+from lakefs_client.exceptions import NotFoundException
 from lakefs_client.model.commit_creation import CommitCreation
 from prefect.context import FlowRunContext
 from prefect_aws import S3Bucket
 from pydantic import Field
 
 from prefect_lakefs.credentials import LakeFSCredentials
 
 
 class LakeFS(S3Bucket):
     _block_type_name = "LakeFS"
 
     credentials: LakeFSCredentials = Field(
-        description="A block containing your credentials to AWS or MinIO.",
+        description="A block containing your LakeFS credentials."
     )
 
     def _get_s3_client(self):
-        # return self.credentials.get_client()
         raise NotImplementedError(
             "Should be using LakeFS client via `self.credentials.get_client()`"
         )
 
+    def _check_branch(self):
+        with self.credentials.get_client("branches") as branches:
+            try:
+                branches.get_branch(
+                    repository=self.credentials.repository,
+                    branch=self.credentials.branch,
+                )
+                return
+            except NotFoundException:
+                branches.create_branch(
+                    repository=self.credentials.repository,
+                    branch_creation={
+                        "name": self.credentials.branch,
+                        "source": "main",
+                    },
+                )
+
     def _write_sync(self, key: str, data: bytes) -> None:
+        self._check_branch()
         with self.credentials.get_client("objects") as client:
             with io.BytesIO(data) as stream:
                 stream.name = key
                 client.upload_object(
                     repository=self.credentials.repository,
                     branch=self.credentials.branch,
                     path=key,
                     content=stream,
                 )
-        # if self.credentials.commit_on_task:
-        #     self.commit_changes()
+            if self.credentials.commit_on_task:
+                self.commit_changes()
 
     def _read_sync(self, key: str) -> None:
-        client = self.credentials.objects_api
-        data = client.get_object(
-            repository=self.credentials.repository,
-            ref=self._get_branch(),
-            path=key,
-        )
-        return data
+        with self.credentials.get_client("objects") as client:
+            data = client.get_object(
+                repository=self.credentials.repository,
+                ref=self.credentials.branch,
+                path=key,
+            )
+            return data
 
     def commit_changes(self):
         repository = self.credentials.repository
         branch: str = self.credentials.branch
         assert branch, "If committing, `branch` must be set in `LakeFsCredentials`"
-        commits_api = self.credentials.commits_api
-        run_context: FlowRunContext = FlowRunContext.get()
-        metadata = {
-            "flow_run_id": run_context.flow.id,
-        }
-        commit = CommitCreation("prefect-lakefs commit", metadata=metadata)
-        commits_api.commit(repository=repository, branch=branch, commit_creation=commit)
+
+        with self.credentials.get_client("commits") as client:
+            run_context: FlowRunContext = FlowRunContext.get()
+            if run_context:
+                metadata = {"flow_run_id": run_context.flow_run.id.hex}
+            else:
+                metadata = {}
+            commit = CommitCreation("prefect-lakefs commit", metadata=metadata)
+            client.commit(repository=repository, branch=branch, commit_creation=commit)
```

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs/tasks.py` & `prefect-lakefs-0.3.0/prefect_lakefs/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs.egg-info/PKG-INFO` & `prefect-lakefs-0.3.0/prefect_lakefs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-lakefs
-Version: 0.2.0
+Version: 0.3.0
 Summary: Prefect integrations for interacting with LakeFS services.
 Home-page: https://github.com/limx0/prefect-lakefs
 Author: limx0
 Author-email: limx0@example.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-lakefs-0.2.0/prefect_lakefs.egg-info/SOURCES.txt` & `prefect-lakefs-0.3.0/prefect_lakefs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
+examples/__init__.py
+examples/storage/__init__.py
+examples/storage/example.py
 prefect_lakefs/__init__.py
 prefect_lakefs/_version.py
 prefect_lakefs/branches.py
 prefect_lakefs/commits.py
 prefect_lakefs/credentials.py
 prefect_lakefs/objects.py
+prefect_lakefs/refs.py
 prefect_lakefs/storage.py
 prefect_lakefs/tasks.py
 prefect_lakefs.egg-info/PKG-INFO
 prefect_lakefs.egg-info/SOURCES.txt
 prefect_lakefs.egg-info/dependency_links.txt
 prefect_lakefs.egg-info/entry_points.txt
 prefect_lakefs.egg-info/requires.txt
 prefect_lakefs.egg-info/top_level.txt
 tests/test_block_standards.py
 tests/test_branches.py
 tests/test_commits.py
 tests/test_credentials.py
 tests/test_objects.py
+tests/test_refs.py
 tests/test_storage.py
```

### Comparing `prefect-lakefs-0.2.0/setup.cfg` & `prefect-lakefs-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/setup.py` & `prefect-lakefs-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/tests/test_block_standards.py` & `prefect-lakefs-0.3.0/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/tests/test_branches.py` & `prefect-lakefs-0.3.0/tests/test_branches.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/tests/test_commits.py` & `prefect-lakefs-0.3.0/tests/test_commits.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/tests/test_credentials.py` & `prefect-lakefs-0.3.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/tests/test_objects.py` & `prefect-lakefs-0.3.0/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.2.0/versioneer.py` & `prefect-lakefs-0.3.0/versioneer.py`

 * *Files identical despite different names*

