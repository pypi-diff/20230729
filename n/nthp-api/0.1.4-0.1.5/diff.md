# Comparing `tmp/nthp_api-0.1.4.tar.gz` & `tmp/nthp_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nthp_api-0.1.4.tar", max compression
+gzip compressed data, was "nthp_api-0.1.5.tar", max compression
```

## Comparing `nthp_api-0.1.4.tar` & `nthp_api-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     2020 2023-07-23 23:42:23.589970 nthp_api-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/__init__.py
--rw-r--r--   0        0        0     1737 2023-07-23 23:44:46.802802 nthp_api-0.1.4/nthp_api/cli/__init__.py
--rw-r--r--   0        0        0      386 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/cli/logs.py
--rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/__init__.py
--rw-r--r--   0        0        0     7378 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/assets.py
--rw-r--r--   0        0        0      549 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/config.py
--rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/content.py
--rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/database.py
--rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/documents.py
--rw-r--r--   0        0        0    12110 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/dumper.py
--rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/history.py
--rw-r--r--   0        0        0     7687 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/loader.py
--rw-r--r--   0        0        0     4694 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/models.py
--rw-r--r--   0        0        0     1124 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/parallel.py
--rw-r--r--   0        0        0     8105 2023-07-23 23:07:15.093248 nthp_api-0.1.4/nthp_api/nthp_build/people.py
--rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/playwrights.py
--rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/roles.py
--rw-r--r--   0        0        0     9776 2023-07-23 23:04:02.359547 nthp_api-0.1.4/nthp_api/nthp_build/schema.py
--rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/search.py
--rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/shows.py
--rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/smugmug.py
--rw-r--r--   0        0        0     9756 2023-07-23 23:32:24.722305 nthp_api-0.1.4/nthp_api/nthp_build/spec.py
--rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/trivia.py
--rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.4/nthp_api/nthp_build/venues.py
--rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/nthp_build/years.py
--rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/__init__.py
--rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/album.py
--rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/client.py
--rw-r--r--   0        0        0      358 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/config.py
--rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/database.py
--rw-r--r--   0        0        0     1134 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/schema.py
--rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.4/nthp_api/smugmugger/smugmug.py
--rw-r--r--   0        0        0     2138 2023-07-23 23:45:03.190902 nthp_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 nthp_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2020 2023-07-23 23:42:23.589970 nthp_api-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/__init__.py
+-rw-r--r--   0        0        0     1737 2023-07-23 23:44:46.802802 nthp_api-0.1.5/nthp_api/cli/__init__.py
+-rw-r--r--   0        0        0      567 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/cli/logs.py
+-rw-r--r--   0        0        0        0 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/__init__.py
+-rw-r--r--   0        0        0     7378 2023-07-29 01:38:27.147185 nthp_api-0.1.5/nthp_api/nthp_build/assets.py
+-rw-r--r--   0        0        0      558 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/nthp_build/config.py
+-rw-r--r--   0        0        0     1103 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/content.py
+-rw-r--r--   0        0        0     3996 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/database.py
+-rw-r--r--   0        0        0     1427 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/documents.py
+-rw-r--r--   0        0        0    12110 2023-07-29 01:33:59.733253 nthp_api-0.1.5/nthp_api/nthp_build/dumper.py
+-rw-r--r--   0        0        0      276 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/nthp_build/fields.py
+-rw-r--r--   0        0        0      461 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/history.py
+-rw-r--r--   0        0        0     8634 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/nthp_build/loader.py
+-rw-r--r--   0        0        0     5377 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/nthp_build/models.py
+-rw-r--r--   0        0        0     1617 2023-07-29 01:37:44.750900 nthp_api-0.1.5/nthp_api/nthp_build/parallel.py
+-rw-r--r--   0        0        0     8105 2023-07-29 01:25:49.153157 nthp_api-0.1.5/nthp_api/nthp_build/people.py
+-rw-r--r--   0        0        0     3826 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/playwrights.py
+-rw-r--r--   0        0        0     6388 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/roles.py
+-rw-r--r--   0        0        0    10192 2023-07-29 01:34:29.809507 nthp_api-0.1.5/nthp_api/nthp_build/schema.py
+-rw-r--r--   0        0        0      416 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/search.py
+-rw-r--r--   0        0        0     6446 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/shows.py
+-rw-r--r--   0        0        0     1098 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/smugmug.py
+-rw-r--r--   0        0        0    10166 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/nthp_build/spec.py
+-rw-r--r--   0        0        0     1940 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/trivia.py
+-rw-r--r--   0        0        0     2117 2023-07-23 23:03:58.959516 nthp_api-0.1.5/nthp_api/nthp_build/venues.py
+-rw-r--r--   0        0        0     1168 2023-07-23 23:03:58.963517 nthp_api-0.1.5/nthp_api/nthp_build/years.py
+-rw-r--r--   0        0        0      305 2023-07-23 23:03:58.963517 nthp_api-0.1.5/nthp_api/smugmugger/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-23 23:03:58.963517 nthp_api-0.1.5/nthp_api/smugmugger/album.py
+-rw-r--r--   0        0        0     2583 2023-07-23 23:03:58.963517 nthp_api-0.1.5/nthp_api/smugmugger/client.py
+-rw-r--r--   0        0        0      367 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/smugmugger/config.py
+-rw-r--r--   0        0        0      661 2023-07-23 23:03:58.963517 nthp_api-0.1.5/nthp_api/smugmugger/database.py
+-rw-r--r--   0        0        0     1155 2023-07-29 01:34:10.381343 nthp_api-0.1.5/nthp_api/smugmugger/schema.py
+-rw-r--r--   0        0        0     2019 2023-07-23 23:03:58.963517 nthp_api-0.1.5/nthp_api/smugmugger/smugmug.py
+-rw-r--r--   0        0        0     2166 2023-07-29 17:55:35.612574 nthp_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 nthp_api-0.1.5/PKG-INFO
```

### Comparing `nthp_api-0.1.4/README.md` & `nthp_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/cli/__init__.py` & `nthp_api-0.1.5/nthp_api/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/assets.py` & `nthp_api-0.1.5/nthp_api/nthp_build/assets.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/config.py` & `nthp_api-0.1.5/nthp_api/nthp_build/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 from pathlib import Path
 
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
     db_uri: str = "nthp.db"
     branch: str = "master"
     content_root: Path
```

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/content.py` & `nthp_api-0.1.5/nthp_api/nthp_build/content.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/database.py` & `nthp_api-0.1.5/nthp_api/nthp_build/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/documents.py` & `nthp_api-0.1.5/nthp_api/nthp_build/documents.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/dumper.py` & `nthp_api-0.1.5/nthp_api/nthp_build/dumper.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/loader.py` & `nthp_api-0.1.5/nthp_api/nthp_build/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -192,52 +192,78 @@
         path=Path("_data/history.yaml"),
         schema_type=models.HistoryRecordCollection,
         func=load_history,
     ),
 ]
 
 
+def loc_to_path(loc: str | tuple) -> str:
+    if isinstance(loc, tuple):
+        return ".".join(map(str, loc))
+    return loc
+
+
+def print_validation_error(validation_error: ValidationError, path: Path) -> None:
+    log.error(f"Validation error in {path}")
+    for error in validation_error.errors():
+        loc = loc_to_path(error["loc"])
+        log.warning(f"{loc} : {error['msg']}")
+        log.info(f"     {error['input']}")
+
+
 def run_document_loader(loader: Loader):
     doc_paths = find_documents(loader.path)
+    docs_that_failed_validation = []
     with database.db.atomic():
         for doc_path in doc_paths:
             document = load_document(doc_path.path)
             try:
                 data = loader.schema_type(**{"id": doc_path.id, **document.metadata})  # type: ignore[call-arg]
-            except ValidationError:
-                log.exception(f"Failed validation: {doc_path.content_path}")
+            except ValidationError as error:
+                print_validation_error(error, doc_path.path)
+                docs_that_failed_validation.append(doc_path)
                 continue
             loader.func(path=doc_path, document=document, data=data)  # type: ignore[call-arg]
+    if docs_that_failed_validation:
+        log.error(
+            f"{len(docs_that_failed_validation)} documents failed validation for {loader.path}"
+        )
 
 
 def run_data_loader(loader: Loader):
+    files_that_failed_validation = []
     with database.db.atomic():
         try:
             document_data = load_yaml(loader.path)
         except yaml.YAMLError:
             log.exception(f"Failed to parse YAML: {loader.path}")
             return
         try:
             if isinstance(loader.schema_type, models.NthpModel):
                 data = loader.schema_type(**document_data)  # type: ignore[call-arg]
             else:
                 data = loader.schema_type(document_data)  # type: ignore[call-arg]
         except ValidationError:
-            log.exception(f"Failed validation: {loader.path}")
+            print_validation_error(ValidationError(), loader.path)
+            files_that_failed_validation.append(loader.path)
             return
         loader.func(
             path=DocumentPath(
                 path=loader.path,
                 id=loader.path.stem,
                 content_path=loader.path,
                 filename=loader.path.name,
                 basename=loader.path.stem,
             ),
             data=data,
         )  # type: ignore[call-arg]
+    if files_that_failed_validation:
+        log.error(
+            f"{len(files_that_failed_validation)} files failed validation for {loader.path}"
+        )
 
 
 def run_loader(loader: Loader):
     log.info(f"Running loader for {loader.schema_type.__name__}")
     tick = time.perf_counter()
     if loader.type is DocumentLoaderFunc:
         run_document_loader(loader)
```

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/models.py` & `nthp_api-0.1.5/nthp_api/nthp_build/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,190 +1,199 @@
 """The models for ingesting data"""
 
 import datetime
 
-from pydantic import BaseModel, root_validator, validator
+from nthp_build.fields import PermissiveStr
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    field_validator,
+    model_validator,
+)
 from pydantic_collections import BaseCollectionModel
 from slugify import slugify
 
 from nthp_api.nthp_build import years
 
 
 class NthpModel(BaseModel):
-    class Config:
-        frozen = True
+    model_config = ConfigDict(frozen=True)
 
 
 class Link(NthpModel):
     type: str
-    href: str | None
-    snapshot: str | None
-    username: str | None
-    title: str | None
-    date: datetime.date | None
-    publisher: str | None
-    rating: str | None
-    quote: str | None
-    note: str | None
-    comment: str | None
+    href: str | None = None
+    snapshot: str | None = None
+    username: PermissiveStr | None = None
+    title: PermissiveStr | None = None
+    date: datetime.date | None = None
+    publisher: PermissiveStr | None = None
+    rating: PermissiveStr | None = None
+    quote: PermissiveStr | None = None
+    note: PermissiveStr | None = None
+    comment: PermissiveStr | None = None
 
 
 class Location(NthpModel):
     lat: float
     lon: float
 
 
 class PersonRef(NthpModel):
-    role: str | None
-    name: str | None
-    note: str | None
+    role: PermissiveStr | None = None
+    name: str | None = None
+    note: PermissiveStr | None = None
     person: bool = True
-    comment: str | None
+    comment: PermissiveStr | None = None
 
 
 class PersonRole(NthpModel):
-    person_id: str | None
-    person_name: str | None
-    role: str | None
-    note: str | None
+    person_id: str | None = None
+    person_name: str | None = None
+    role: PermissiveStr | None = None
+    note: PermissiveStr | None = None
     is_person: bool = True
-    comment: str | None
+    comment: PermissiveStr | None = None
 
 
 class ShowCanonical(NthpModel):
-    title: str | None
-    playwright: str | None
+    title: PermissiveStr | None = None
+    playwright: str | None = None
 
 
 class Asset(NthpModel):
     type: str
-    image: str | None
-    video: str | None
-    filename: str | None
-    title: str | None
-    page: int | None
+    image: str | None = None
+    video: str | None = None
+    filename: str | None = None
+    title: PermissiveStr | None = None
+    page: int | None = None
     display_image: bool = False
 
-    @root_validator()
+    @model_validator(mode="before")
+    @classmethod
     def require_image_xor_video_xor_filename(cls, values: dict) -> dict:
         if (
             sum(
                 (
                     1 if values.get("image") else 0,
                     1 if values.get("video") else 0,
                     1 if values.get("filename") else 0,
                 )
             )
             != 1
         ):
             raise ValueError("Must have exactly one of image, video, or filename")
         return values
 
-    @validator("type")
+    @field_validator("type")
+    @classmethod
     def slugify_type(cls, value: str) -> str:
         return slugify(value)
 
-    @validator("title", always=True)
-    def require_title_with_filename(cls, value: str | None, values: dict) -> str | None:
-        if values.get("filename") is not None and value is None:
+    @model_validator(mode="after")
+    def require_title_with_filename(self) -> "Asset":
+        if self.filename is not None and self.title is None:
             raise ValueError("title is required if filename is provided")
-        return value
+        return self
 
-    @validator("display_image")
-    def display_image_only_for_images(cls, value: bool, values: dict) -> bool:
-        if value and not values.get("image"):
+    @model_validator(mode="after")
+    def display_image_only_for_images(self) -> "Asset":
+        if self.display_image and not self.image:
             raise ValueError("Can only set display_image for images")
-        return value
+        return self
 
 
 class Trivia(NthpModel):
     quote: str
-    name: str | None
-    submitted: datetime.date | None
+    name: str | None = None
+    submitted: datetime.date | None = None
 
 
 class Show(NthpModel):
     id: str
     title: str
-    playwright: str | None
+    playwright: str | None = None
 
     devised: str | bool = False
 
-    @validator("devised")
+    @field_validator("devised")
+    @classmethod
     def handle_devised_strings(cls, value: str | bool) -> str | bool:
         if isinstance(value, str):
             if value.lower() == "true":
                 return True
             if value.lower() == "false":
                 return False
         return value
 
     improvised: bool = False
-    adaptor: str | None
-    translator: str | None
+    adaptor: str | None = None
+    translator: str | None = None
     canonical: list[ShowCanonical] = []
     student_written: bool = False
-    company: str | None
-    company_sort: str | None
-    period: str | None
+    company: PermissiveStr | None = None
+    company_sort: PermissiveStr | None = None
+    period: str | None = None
     season: str
-    season_sort: int | None
-    venue: str | None
-    date_start: datetime.date | None
-    date_end: datetime.date | None
+    season_sort: int | None = None
+    venue: PermissiveStr | None = None
+    date_start: datetime.date | None = None
+    date_end: datetime.date | None = None
     # tour TODO
     trivia: list[Trivia] = []
     cast: list[PersonRef] = []
     crew: list[PersonRef] = []
     cast_incomplete: bool = False
-    cast_note: str | None
+    cast_note: PermissiveStr | None = None
     crew_incomplete: bool = False
-    crew_note: str | None
-    prod_shots: str | None
+    crew_note: PermissiveStr | None = None
+    prod_shots: str | None = None
     assets: list[Asset] = []
     links: list[Link] = []
-    comment: str | None
+    comment: PermissiveStr | None = None
 
 
 class Committee(NthpModel):
     committee: list[PersonRef]
 
 
 class Venue(NthpModel):
     title: str
     links: list[Link] = []
-    built: int | None
+    built: int | None = None
     images: list[str] = []
-    location: Location | None
+    location: Location | None = None
     city: str | None = None
     sort: int | None = None
-    comment: str | None = None
+    comment: PermissiveStr | None = None
 
 
 class Person(NthpModel):
     id: str | None = None
     title: str
-    submitted: datetime.date | None = None
+    submitted: datetime.date | bool | None = None
     headshot: str | None = None
     # course: List[str] = [] TODO: both lists and strings
     graduated: int | None = None
     award: str | None = None
     # career: Optional[str] TODO: both lists and strings
     links: list[Link] = []
     news: list[Link] = []
-    comment: str | None = None
+    comment: PermissiveStr | None = None
 
 
 class HistoryRecord(NthpModel):
-    year: str
+    year: PermissiveStr
     academic_year: str | None = None
     title: str
     description: str
 
-    @validator("academic_year")
+    @field_validator("academic_year")
+    @classmethod
     def require_valid_academic_year(cls, value: str | None) -> str | None:
         if value is not None and not years.check_year_id_is_valid(value):
             raise ValueError("Invalid academic year")
         return value
 
 
 class HistoryRecordCollection(BaseCollectionModel[HistoryRecord]):
```

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/parallel.py` & `nthp_api-0.1.5/nthp_api/nthp_build/parallel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 import logging
+from collections.abc import Callable
 from concurrent.futures import ThreadPoolExecutor
-from multiprocessing import Process
+from multiprocessing import Process, Queue
 from multiprocessing.managers import SyncManager
 from typing import Any, NamedTuple
 
 log = logging.getLogger(__name__)
 
 
+class MultiProcessError(Exception):
+    pass
+
+
 def run_tasks_in_series(tasks):
     log.info("Running %d tasks in series", len(tasks))
     for task in tasks:
         task()
 
 
-def run_cpu_tasks_in_parallel(tasks):
+def run_cpu_task(task: Callable, error_queue: Queue):
+    try:
+        task()
+    except Exception as e:
+        log.exception(f"Error occurred while running task {task}")
+        error_queue.put(e)
+
+
+def run_cpu_tasks_in_parallel(tasks: list[Callable]):
     log.info("Running %d CPU tasks in parallel", len(tasks))
-    running_tasks = [Process(target=task) for task in tasks]
+    error_queue: Queue = Queue()
+    running_tasks = [
+        Process(target=run_cpu_task, args=(task, error_queue)) for task in tasks
+    ]
     for running_task in running_tasks:
         running_task.start()
     for running_task in running_tasks:
         running_task.join()
 
+    if not error_queue.empty():
+        raise MultiProcessError("Errors occurred while running tasks")
+
 
 def run_io_tasks_in_parallel(tasks):
     log.info("Running %d IO tasks in parallel", len(tasks))
     with ThreadPoolExecutor() as executor:
         running_tasks = [executor.submit(task) for task in tasks]
         for running_task in running_tasks:
             running_task.result()
```

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/people.py` & `nthp_api-0.1.5/nthp_api/nthp_build/people.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/playwrights.py` & `nthp_api-0.1.5/nthp_api/nthp_build/playwrights.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/roles.py` & `nthp_api-0.1.5/nthp_api/nthp_build/roles.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/schema.py` & `nthp_api-0.1.5/nthp_api/nthp_build/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 """The schema for outputting data"""
 
 import datetime
 from enum import Enum
 
 import humps
-from pydantic import BaseModel, Field
+from nthp_build.fields import PermissiveStr
+from pydantic import BaseModel, ConfigDict, Field
 from pydantic_collections import BaseCollectionModel
 
 from nthp_api.nthp_build import models, years
 
 
 class ResponseConfig:
     allow_population_by_field_name = True
     alias_generator = humps.camelize
     frozen = True
 
 
+RESPONSE_CONFIG = ConfigDict(
+    populate_by_name=True,
+    alias_generator=humps.camelize,
+    frozen=True,
+)
+
+
 class NthpSchema(BaseModel):
-    class Config(ResponseConfig):
-        pass
+    model_config = RESPONSE_CONFIG
 
 
 class Location(NthpSchema):
     lat: float
     lon: float
 
     @classmethod
     def from_model(cls, model: models.Location):
         return cls(lat=model.lat, lon=model.lon)
 
 
 class PersonRoleList(models.PersonRole):
-    class Config(ResponseConfig):
-        pass
+    model_config = RESPONSE_CONFIG
 
 
 class PersonList(NthpSchema):
     id: str
-    name: str | None
+    name: str | None = None
     is_person: bool
-    headshot: str | None
+    headshot: str | None = None
     has_bio: bool
 
 
 class PlayShow(NthpSchema):
     id: str
     title: str
 
@@ -66,15 +72,15 @@
     type: PlaywrightType
     descriptor: str | None = None
     student_written: bool
 
 
 class ShowRole(NthpSchema):
     role: str | None = None
-    person: PersonList | None
+    person: PersonList | None = None
     note: str | None = None
 
 
 class Asset(NthpSchema):
     type: str
     source: str
     id: str
@@ -92,71 +98,71 @@
     id: str
     name: str
 
 
 class ShowDetail(NthpSchema):
     id: str
     title: str
-    play: PlayShow | None
-    playwright: PlaywrightShow | None
-    adaptor: str | None
-    translator: str | None
-    company: str | None
-    period: str | None
+    play: PlayShow | None = None
+    playwright: PlaywrightShow | None = None
+    adaptor: str | None = None
+    translator: str | None = None
+    company: str | None = None
+    period: str | None = None
     season: str
-    venue: VenueShow | None
-    date_start: datetime.date | None
-    date_end: datetime.date | None
+    venue: VenueShow | None = None
+    date_start: datetime.date | None = None
+    date_end: datetime.date | None = None
     # tour TODO
     cast: list[ShowRole]
     crew: list[ShowRole]
     cast_incomplete: bool
-    cast_note: str | None
+    cast_note: str | None = None
     crew_incomplete: bool
-    crew_note: str | None
+    crew_note: str | None = None
     assets: list[Asset]
-    primary_image: str | None
+    primary_image: str | None = None
 
-    content: str | None
+    content: str | None = None
 
 
 class ShowList(NthpSchema):
     id: str
     title: str
-    playwright: PlaywrightShow | None
-    adaptor: str | None
+    playwright: PlaywrightShow | None = None
+    adaptor: str | None = None
     devised: str | bool
-    season: str | None
-    venue: VenueShow | None
-    date_start: datetime.date | None
-    date_end: datetime.date | None
-    primary_image: str | None
+    season: str | None = None
+    venue: VenueShow | None = None
+    date_start: datetime.date | None = None
+    date_end: datetime.date | None = None
+    primary_image: str | None = None
 
 
 class PlaywrightShowListItem(NthpSchema):
     id: str
     title: str
-    date_start: datetime.date | None
-    date_end: datetime.date | None
-    primary_image: str | None
+    date_start: datetime.date | None = None
+    date_end: datetime.date | None = None
+    primary_image: str | None = None
 
 
 class VenueList(NthpSchema):
     id: str
     name: str
     show_count: int
-    built: int | None
-    location: Location | None
-    city: str | None
+    built: int | None = None
+    location: Location | None = None
+    city: str | None = None
 
 
 class VenueDetail(VenueList):
     assets: list[Asset] = []
     shows: list[ShowList] = []
-    content: str | None
+    content: str | None = None
 
 
 class VenueCollection(BaseCollectionModel[VenueList]):
     pass
 
 
 class PlaywrightListItem(Playwright):
@@ -193,52 +199,52 @@
 
 class YearDetail(YearList):
     shows: list[ShowList]
     committee: list[PersonRoleList]
 
 
 class PersonShowRoleItem(NthpSchema):
-    role: str | None
+    role: str | None = None
     role_type: str
 
 
 class PersonShowRoles(NthpSchema):
     show_id: str
     show_title: str
     show_year_id: str
     show_year: int
-    show_primary_image: str | None
+    show_primary_image: str | None = None
     roles: list[PersonShowRoleItem]
 
 
 class PersonCommitteeRole(NthpSchema):
     year_title: str
     year_decade: int
     year_id: str
     role: str
 
 
 class PersonCommitteeRoleList(NthpSchema):
     id: str
     title: str
-    headshot: str | None
+    headshot: str | None = None
     year_title: str
     year_decade: int
     year_id: str
     role: str
 
 
 class PersonCommitteeRoleListCollection(BaseCollectionModel[PersonCommitteeRoleList]):
     pass
 
 
 class PersonShowRoleList(NthpSchema):
     id: str
     title: str
-    headshot: str | None
+    headshot: str | None = None
     role: str
     show_count: int
 
 
 class PersonShowRoleListCollection(BaseCollectionModel[PersonShowRoleList]):
     pass
 
@@ -267,29 +273,28 @@
             estimated=estimated,
         )
 
 
 class PersonDetail(NthpSchema):
     id: str
     title: str
-    submitted: datetime.date | None
-    headshot: str | None
-    graduated: PersonGraduated | None
+    submitted: datetime.date | bool | None = None
+    headshot: str | None = None
+    graduated: PersonGraduated | None = None
     show_roles: list[PersonShowRoles]
     committee_roles: list[PersonCommitteeRole]
-    content: str | None
+    content: str | None = None
 
 
 class PersonCollaborator(NthpSchema):
     person_id: str
     person_name: str
     target_ids: list[str]
 
-    class Config(ResponseConfig):
-        frozen = False  # Cannot be frozen as we need an ordered list
+    model_config = RESPONSE_CONFIG  # TODO frozen=False
 
 
 class PersonCollaboratorCollection(BaseCollectionModel[PersonCollaborator]):
     pass
 
 
 class BaseTrivia(NthpSchema):
@@ -346,15 +351,15 @@
     )
     target_image_id: str | None = Field(
         title="Target Image ID",
         description="The image ID of the target of the quote",
         example="qABC123",
     )
     # Uses YYYY, not YY_YY, 2000 means 2000-2001
-    target_year: str | None = Field(
+    target_year: PermissiveStr | None = Field(
         title="Target Year",
         description="The year of the target of the quote",
         example="2000",
     )
 
 
 class PersonTriviaCollection(BaseCollectionModel[PersonTrivia]):
@@ -388,19 +393,19 @@
     VENUE = "venue"
 
 
 class SearchDocument(NthpSchema):
     type: SearchDocumentType
     title: str
     id: str
-    image_id: str | None
-    playwright: PlaywrightShow | None
-    company: str | None
-    people: list[str] | None
-    plaintext: str | None
+    image_id: str | None = None
+    playwright: PlaywrightShow | None = None
+    company: str | None = None
+    people: list[str] | None = None
+    plaintext: str | None = None
 
 
 class SearchDocumentCollection(BaseCollectionModel[SearchDocument]):
     pass
 
 
 class SiteStats(NthpSchema):
```

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/shows.py` & `nthp_api-0.1.5/nthp_api/nthp_build/shows.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/smugmug.py` & `nthp_api-0.1.5/nthp_api/nthp_build/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/spec.py` & `nthp_api-0.1.5/nthp_api/nthp_build/spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import json
+from collections.abc import Sequence
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
-import pydantic.schema
+from pydantic import BaseModel
+from pydantic.json_schema import JsonSchemaMode, models_json_schema
 from pydantic_collections import BaseCollectionModel
 
 from nthp_api.nthp_build import schema
 
-JSON_SCHEMA = pydantic.schema.schema(
-    (
+
+def make_models_json_schema_models(
+    *models: type[BaseModel],
+) -> Sequence[tuple[type[BaseModel], JsonSchemaMode]]:
+    json_schema_mode: JsonSchemaMode = "validation"
+    return [(model, json_schema_mode) for model in models]
+
+
+PYDANTIC_JSON_SCHEMA = models_json_schema(
+    make_models_json_schema_models(
         schema.AssetCollection,
         schema.HistoryRecordCollection,
         schema.PersonCollaboratorCollection,
         schema.PersonCommitteeRoleListCollection,
         schema.PersonDetail,
         schema.PersonShowRoleListCollection,
         schema.PersonTriviaCollection,
@@ -26,22 +36,24 @@
         schema.VenueCollection,
         schema.VenueDetail,
         schema.YearDetail,
         schema.YearList,
         schema.YearListCollection,
     ),
     title="My Schema",
-    ref_prefix="#/components/schemas/",
+    ref_template="#/components/schemas/{model}",
 )
 
+JSON_SCHEMA = PYDANTIC_JSON_SCHEMA[1]["$defs"]
+
 Model = type[schema.NthpSchema] | type[BaseCollectionModel]
 
 
 def check_model_present(model: Model):
-    if model.__name__ not in JSON_SCHEMA["definitions"]:
+    if model.__name__ not in JSON_SCHEMA:
         raise ValueError(f"Model {model} not found in JSON_SCHEMA")
 
 
 def make_basic_get_operation(
     operation_id: str,
     tags: list[str],
     summary: str,
@@ -275,15 +287,15 @@
         "/search/documents.json": make_basic_get_operation(
             operation_id="getSearchDocuments",
             tags=["search"],
             summary="Get search documents",
             model=schema.SearchDocumentCollection,
         ),
     },
-    "components": {"schemas": JSON_SCHEMA["definitions"]},
+    "components": {"schemas": JSON_SCHEMA},
 }
 
 
 def write_spec(path: str | Path):
     if isinstance(path, str):
         path = Path(path)
     with path.open("w") as f:
```

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/trivia.py` & `nthp_api-0.1.5/nthp_api/nthp_build/trivia.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/venues.py` & `nthp_api-0.1.5/nthp_api/nthp_build/venues.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/nthp_build/years.py` & `nthp_api-0.1.5/nthp_api/nthp_build/years.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/smugmugger/album.py` & `nthp_api-0.1.5/nthp_api/smugmugger/album.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/smugmugger/client.py` & `nthp_api-0.1.5/nthp_api/smugmugger/client.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/smugmugger/database.py` & `nthp_api-0.1.5/nthp_api/smugmugger/database.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/nthp_api/smugmugger/schema.py` & `nthp_api-0.1.5/nthp_api/smugmugger/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 class SmugMugPages(BaseModel):
     Total: int
     Start: int
     Count: int
     RequestedCount: int
     FirstPage: str
     LastPage: str
-    NextPage: str | None
+    NextPage: str | None = None
 
 
 class SmugMugResponseInner(BaseModel):
     Uri: str
-    Pages: SmugMugPages | None
+    Pages: SmugMugPages | None = None
 
 
 class SmugMugResponse(BaseModel):
     Code: int
     Message: str
     Response: SmugMugResponseInner
 
@@ -43,15 +43,15 @@
     Date: datetime.datetime
     FileName: str
     Format: str
     ImageKey: str
     IsVideo: bool
     OriginalHeight: int
     OriginalWidth: int
-    OriginalSize: int | None
+    OriginalSize: int | None = None
     Processing: bool
     ThumbnailUrl: str
     Title: str
     WebUri: str
 
 
 class SmugMugImageCollection(BaseCollectionModel[SmugMugImage]):
```

### Comparing `nthp_api-0.1.4/nthp_api/smugmugger/smugmug.py` & `nthp_api-0.1.5/nthp_api/smugmugger/smugmug.py`

 * *Files identical despite different names*

### Comparing `nthp_api-0.1.4/pyproject.toml` & `nthp_api-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "nthp_api"
-version = "0.1.4"
+version = "0.1.5"
 description = "This is a CLI tool for building the Nottingham New Theatre's History Project content database."
 authors = ["Will Pimblett <will@wjdp.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/newtheatre/nthp-api"
 repository = "https://github.com/newtheatre/nthp-api"
 
 [tool.poetry.scripts]
 nthp = "nthp_api.cli:cli"
 nthp_api = "nthp_api.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "^1.10.7"
+pydantic = "^2.1.1"
 python-frontmatter = "^1.0.0"
 peewee = "^3.16.2"
 python-slugify = "^8.0.1"
 pyhumps = "^3.8.0"
 click = "^8.1.3"
 coloredlogs = "^15.0.1"
-pydantic-collections = "^0.4.0"
+pydantic-collections = "^0.5.0"
 Markdown = "^3.4.3"
 PyYAML = "^6.0"
 httpx = "^0.24.1"
+pydantic-settings = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-vcr = "^1.0.2"
 mypy = "^1.3.0"
 pytest-depends = "^1.0.1"
 types-python-slugify = "^8"
```

### Comparing `nthp_api-0.1.4/PKG-INFO` & `nthp_api-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nthp-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is a CLI tool for building the Nottingham New Theatre's History Project content database.
 Home-page: https://github.com/newtheatre/nthp-api
 License: MIT
 Author: Will Pimblett
 Author-email: will@wjdp.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,16 +13,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Markdown (>=3.4.3,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: peewee (>=3.16.2,<4.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pydantic-collections (>=0.4.0,<0.5.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Requires-Dist: pydantic-collections (>=0.5.0,<0.6.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: python-frontmatter (>=1.0.0,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/newtheatre/nthp-api
 Description-Content-Type: text/markdown
 
 # History Project API Generator
```

