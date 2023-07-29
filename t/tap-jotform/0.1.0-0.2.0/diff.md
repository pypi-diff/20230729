# Comparing `tmp/tap_jotform-0.1.0.tar.gz` & `tmp/tap_jotform-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_jotform-0.1.0.tar", max compression
+gzip compressed data, was "tap_jotform-0.2.0.tar", max compression
```

## Comparing `tap_jotform-0.1.0.tar` & `tap_jotform-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-07-07 16:27:18.414427 tap_jotform-0.1.0/LICENSE
--rw-r--r--   0        0        0     3508 2023-07-07 16:27:18.414427 tap_jotform-0.1.0/README.md
--rw-r--r--   0        0        0     1845 2023-07-07 16:27:43.370377 tap_jotform-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/__init__.py
--rw-r--r--   0        0        0      116 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/__main__.py
--rw-r--r--   0        0        0     5296 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/client.py
--rw-r--r--   0        0        0     8428 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/streams.py
--rw-r--r--   0        0        0     2738 2023-07-07 16:27:18.418427 tap_jotform-0.1.0/tap_jotform/tap.py
--rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 tap_jotform-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-29 00:55:13.786449 tap_jotform-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5067 2023-07-29 00:55:13.786449 tap_jotform-0.2.0/README.md
+-rw-r--r--   0        0        0     1845 2023-07-29 00:55:31.034561 tap_jotform-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/__main__.py
+-rw-r--r--   0        0        0     5285 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/client.py
+-rw-r--r--   0        0        0     8428 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/streams.py
+-rw-r--r--   0        0        0     2738 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/tap.py
+-rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 tap_jotform-0.2.0/PKG-INFO
```

### Comparing `tap_jotform-0.1.0/LICENSE` & `tap_jotform-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.1.0/README.md` & `tap_jotform-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -36,14 +36,47 @@
 | stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
 | flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth| False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `tap-jotform --about`
 
+## Streams
+
+| Stream name | API endpoint      | API docs                                       | Notes |
+| :---------- | :---------------- | :--------------------------------------------- | :---- |
+| forms       | /user/forms       | https://api.jotform.com/docs/#user-forms       | Replication for this stream is opt-in. See instructions [below](#configuring-incremental-replication). |
+| questions   | /form/{form_id}/questions | https://api.jotform.com/docs/#form-id-questions | |
+| submissions | /user/submissions | https://api.jotform.com/docs/#user-submissions | Replication for this stream is opt-in. See instructions [below](#configuring-incremental-replication).  |
+| reports     | /user/reports     | https://api.jotform.com/docs/#user-reports | |
+| user_history | /user/history    | https://api.jotform.com/docs/#user-history | |
+
+
+### Configuring incremental replication
+
+By default, the `forms` and `submissions` stream are synced with `FULL_TABLE` replication. Incremental replication can be enabled by setting the replication metadata in the stream's entry in the catalog file:
+
+* `replication_method`: set to`INCREMENTAL`
+* `replication_key` set to `created_at` or `updated_at`. The former will omit updated submissions, while the latter will omit new submissions.
+
+For example, to enable incremental replication for the `submissions` stream:
+
+```json
+{
+  "streams": [
+    {
+      "tap_stream_id": "submissions",
+      "stream": "submissions",
+      "replication_method": "INCREMENTAL",
+      "replication_key": "updated_at",
+    }
+  ]
+}
+```
+
 ### Source Authentication and Authorization
 
 To generate an API key, follow the instructions in https://api.jotform.com/docs/#gettingstarted.
 
 ## Usage
 
 You can easily run `tap-jotform` by itself or in a pipeline using [Meltano](https://meltano.com/).
```

#### html2text {}

```diff
@@ -12,16 +12,35 @@
 configuration for HTTP requests | | stream_maps | False | None | Config object
 for stream maps capability. For more information check out [Stream Maps](https:
 //sdk.meltano.com/en/latest/stream_maps.html). | | stream_map_config | False |
 None | User-defined config values to be used within map expressions. | |
 flattening_enabled | False | None | 'True' to enable schema flattening and
 automatically expand nested properties. | | flattening_max_depth| False | None
 | The max depth to flatten schemas. | A full list of supported settings and
-capabilities is available by running: `tap-jotform --about` ### Source
-Authentication and Authorization To generate an API key, follow the
+capabilities is available by running: `tap-jotform --about` ## Streams | Stream
+name | API endpoint | API docs | Notes | | :---------- | :---------------- | :-
+-------------------------------------------- | :---- | | forms | /user/forms |
+https://api.jotform.com/docs/#user-forms | Replication for this stream is opt-
+in. See instructions [below](#configuring-incremental-replication). | |
+questions | /form/{form_id}/questions | https://api.jotform.com/docs/#form-id-
+questions | | | submissions | /user/submissions | https://api.jotform.com/docs/
+#user-submissions | Replication for this stream is opt-in. See instructions
+[below](#configuring-incremental-replication). | | reports | /user/reports |
+https://api.jotform.com/docs/#user-reports | | | user_history | /user/history |
+https://api.jotform.com/docs/#user-history | | ### Configuring incremental
+replication By default, the `forms` and `submissions` stream are synced with
+`FULL_TABLE` replication. Incremental replication can be enabled by setting the
+replication metadata in the stream's entry in the catalog file: *
+`replication_method`: set to`INCREMENTAL` * `replication_key` set to
+`created_at` or `updated_at`. The former will omit updated submissions, while
+the latter will omit new submissions. For example, to enable incremental
+replication for the `submissions` stream: ```json { "streams": [
+{ "tap_stream_id": "submissions", "stream": "submissions",
+"replication_method": "INCREMENTAL", "replication_key": "updated_at", } ] } ```
+### Source Authentication and Authorization To generate an API key, follow the
 instructions in https://api.jotform.com/docs/#gettingstarted. ## Usage You can
 easily run `tap-jotform` by itself or in a pipeline using [Meltano](https://
 meltano.com/). ### Executing the Tap Directly ```bash tap-jotform --version
 tap-jotform --help tap-jotform --config CONFIG --discover > ./catalog.json ```
 ## Developer Resources ### Initialize your Development Environment ```bash pipx
 install poetry poetry install ``` ### Create and Run Tests Create tests within
 the `tap_jotform/tests` subfolder and then run: ```bash poetry run pytest ```
```

### Comparing `tap_jotform-0.1.0/pyproject.toml` & `tap_jotform-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core>=1.1",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-jotform"
-version = "0.1.0"
+version = "0.2.0"
 description = "Singer tap for Jotform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-jotform"
 repository = "https://github.com/edgarrmondragon/tap-jotform"
@@ -19,15 +19,15 @@
 keywords = ["ELT", "Jotform"]
 
 [tool.poetry.dependencies]
 colorama = "==0.4.*"
 importlib-metadata = {version = "<5.0.0", python = "<3.8"}
 python = "<3.12,>=3.7.1"
 requests-cache = "==1.1.*"
-singer-sdk = ">=0.28,<0.30"
+singer-sdk = ">=0.28,<0.31"
 structlog = "==23.1.*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.poetry.scripts]
 # CLI declaration
```

### Comparing `tap_jotform-0.1.0/tap_jotform/client.py` & `tap_jotform-0.2.0/tap_jotform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,14 @@
                 self._requests_session = requests.Session()
         return self._requests_session
 
 
 class JotformPaginatedStream(JotformStream):
     """A Jotform stream with pagination."""
 
-    replication_key = "updated_at"
-
     def get_new_paginator(self) -> JotformPaginator:
         """Return a new instance of a paginator.
 
         Returns:
             A new instance of a paginator.
         """
         return JotformPaginator(0, self.page_size)
@@ -156,15 +154,15 @@
 
         Returns:
             A dictionary of values to be used in URL parameterization.
         """
         params: dict[str, t.Any] = {"limit": self.page_size}
 
         starting_value = self.get_starting_timestamp(context)
-        if starting_value:
+        if starting_value and self.replication_key:
             self.logger.info(
                 "Bookmark found %(bookmark)s",
                 extra={"bookmark": starting_value},
             )
             params["filter"] = f'{{"{self.replication_key}:gt": "{starting_value}"}}'
 
         if next_page_token:
```

### Comparing `tap_jotform-0.1.0/tap_jotform/streams.py` & `tap_jotform-0.2.0/tap_jotform/streams.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.1.0/tap_jotform/tap.py` & `tap_jotform-0.2.0/tap_jotform/tap.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.1.0/PKG-INFO` & `tap_jotform-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-jotform
-Version: 0.1.0
+Version: 0.2.0
 Summary: Singer tap for Jotform, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-jotform
 License: Apache-2.0
 Keywords: ELT,Jotform
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (==0.4.*)
 Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
 Requires-Dist: requests-cache (==1.1.*)
-Requires-Dist: singer-sdk (>=0.28,<0.30)
+Requires-Dist: singer-sdk (>=0.28,<0.31)
 Requires-Dist: structlog (==23.1.*)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-jotform/#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-jotform
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -63,14 +63,47 @@
 | stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |
 | flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth| False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `tap-jotform --about`
 
+## Streams
+
+| Stream name | API endpoint      | API docs                                       | Notes |
+| :---------- | :---------------- | :--------------------------------------------- | :---- |
+| forms       | /user/forms       | https://api.jotform.com/docs/#user-forms       | Replication for this stream is opt-in. See instructions [below](#configuring-incremental-replication). |
+| questions   | /form/{form_id}/questions | https://api.jotform.com/docs/#form-id-questions | |
+| submissions | /user/submissions | https://api.jotform.com/docs/#user-submissions | Replication for this stream is opt-in. See instructions [below](#configuring-incremental-replication).  |
+| reports     | /user/reports     | https://api.jotform.com/docs/#user-reports | |
+| user_history | /user/history    | https://api.jotform.com/docs/#user-history | |
+
+
+### Configuring incremental replication
+
+By default, the `forms` and `submissions` stream are synced with `FULL_TABLE` replication. Incremental replication can be enabled by setting the replication metadata in the stream's entry in the catalog file:
+
+* `replication_method`: set to`INCREMENTAL`
+* `replication_key` set to `created_at` or `updated_at`. The former will omit updated submissions, while the latter will omit new submissions.
+
+For example, to enable incremental replication for the `submissions` stream:
+
+```json
+{
+  "streams": [
+    {
+      "tap_stream_id": "submissions",
+      "stream": "submissions",
+      "replication_method": "INCREMENTAL",
+      "replication_key": "updated_at",
+    }
+  ]
+}
+```
+
 ### Source Authentication and Authorization
 
 To generate an API key, follow the instructions in https://api.jotform.com/docs/#gettingstarted.
 
 ## Usage
 
 You can easily run `tap-jotform` by itself or in a pipeline using [Meltano](https://meltano.com/).
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: tap-jotform Version: 0.1.0 Summary: Singer tap for
+Metadata-Version: 2.1 Name: tap-jotform Version: 0.2.0 Summary: Singer tap for
 Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-jotform License: Apache-2.0 Keywords:
 ELT,Jotform Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: colorama
 (==0.4.*) Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
 Requires-Dist: requests-cache (==1.1.*) Requires-Dist: singer-sdk
-(>=0.28,<0.30) Requires-Dist: structlog (==23.1.*) Project-URL: Documentation,
+(>=0.28,<0.31) Requires-Dist: structlog (==23.1.*) Project-URL: Documentation,
 https://github.com/edgarrmondragon/tap-jotform/#readme Project-URL: Repository,
 https://github.com/edgarrmondragon/tap-jotform Description-Content-Type: text/
 markdown
                                  # tap-jotform
                        [pre-commit.ci_status] [License]
      Singer Tap for Jotform. Built with the [Meltano Singer SDK](https://
                                sdk.meltano.com).
@@ -28,16 +28,35 @@
 configuration for HTTP requests | | stream_maps | False | None | Config object
 for stream maps capability. For more information check out [Stream Maps](https:
 //sdk.meltano.com/en/latest/stream_maps.html). | | stream_map_config | False |
 None | User-defined config values to be used within map expressions. | |
 flattening_enabled | False | None | 'True' to enable schema flattening and
 automatically expand nested properties. | | flattening_max_depth| False | None
 | The max depth to flatten schemas. | A full list of supported settings and
-capabilities is available by running: `tap-jotform --about` ### Source
-Authentication and Authorization To generate an API key, follow the
+capabilities is available by running: `tap-jotform --about` ## Streams | Stream
+name | API endpoint | API docs | Notes | | :---------- | :---------------- | :-
+-------------------------------------------- | :---- | | forms | /user/forms |
+https://api.jotform.com/docs/#user-forms | Replication for this stream is opt-
+in. See instructions [below](#configuring-incremental-replication). | |
+questions | /form/{form_id}/questions | https://api.jotform.com/docs/#form-id-
+questions | | | submissions | /user/submissions | https://api.jotform.com/docs/
+#user-submissions | Replication for this stream is opt-in. See instructions
+[below](#configuring-incremental-replication). | | reports | /user/reports |
+https://api.jotform.com/docs/#user-reports | | | user_history | /user/history |
+https://api.jotform.com/docs/#user-history | | ### Configuring incremental
+replication By default, the `forms` and `submissions` stream are synced with
+`FULL_TABLE` replication. Incremental replication can be enabled by setting the
+replication metadata in the stream's entry in the catalog file: *
+`replication_method`: set to`INCREMENTAL` * `replication_key` set to
+`created_at` or `updated_at`. The former will omit updated submissions, while
+the latter will omit new submissions. For example, to enable incremental
+replication for the `submissions` stream: ```json { "streams": [
+{ "tap_stream_id": "submissions", "stream": "submissions",
+"replication_method": "INCREMENTAL", "replication_key": "updated_at", } ] } ```
+### Source Authentication and Authorization To generate an API key, follow the
 instructions in https://api.jotform.com/docs/#gettingstarted. ## Usage You can
 easily run `tap-jotform` by itself or in a pipeline using [Meltano](https://
 meltano.com/). ### Executing the Tap Directly ```bash tap-jotform --version
 tap-jotform --help tap-jotform --config CONFIG --discover > ./catalog.json ```
 ## Developer Resources ### Initialize your Development Environment ```bash pipx
 install poetry poetry install ``` ### Create and Run Tests Create tests within
 the `tap_jotform/tests` subfolder and then run: ```bash poetry run pytest ```
```

