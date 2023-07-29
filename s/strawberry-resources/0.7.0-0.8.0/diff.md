# Comparing `tmp/strawberry_resources-0.7.0.tar.gz` & `tmp/strawberry_resources-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_resources-0.7.0.tar", max compression
+gzip compressed data, was "strawberry_resources-0.8.0.tar", max compression
```

## Comparing `strawberry_resources-0.7.0.tar` & `strawberry_resources-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/LICENSE
--rw-r--r--   0        0        0     9125 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/README.md
--rw-r--r--   0        0        0     4034 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/__init__.py
--rw-r--r--   0        0        0       59 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/__main__.py
--rw-r--r--   0        0        0      123 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/cli/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/cli/export.py
--rw-r--r--   0        0        0     2828 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/exporter.py
--rw-r--r--   0        0        0      124 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/integrations/__init__.py
--rw-r--r--   0        0        0     1660 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/integrations/base.py
--rw-r--r--   0        0        0    10066 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/integrations/django.py
--rw-r--r--   0        0        0        0 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/py.typed
--rw-r--r--   0        0        0      628 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/queries.py
--rw-r--r--   0        0        0     7741 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/resolver.py
--rw-r--r--   0        0        0     7169 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/types.py
--rw-r--r--   0        0        0        0 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/utils/__init__.py
--rw-r--r--   0        0        0     2033 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/utils/inspect.py
--rw-r--r--   0        0        0      662 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/utils/pyutils.py
--rw-r--r--   0        0        0    10700 1970-01-01 00:00:00.000000 strawberry_resources-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/LICENSE
+-rw-r--r--   0        0        0     9125 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/README.md
+-rw-r--r--   0        0        0     3851 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/__main__.py
+-rw-r--r--   0        0        0      123 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/cli/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/cli/export.py
+-rw-r--r--   0        0        0     2811 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/exporter.py
+-rw-r--r--   0        0        0      124 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/integrations/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/integrations/base.py
+-rw-r--r--   0        0        0     9607 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/integrations/django.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/py.typed
+-rw-r--r--   0        0        0      628 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/queries.py
+-rw-r--r--   0        0        0     7943 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/resolver.py
+-rw-r--r--   0        0        0     7169 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/types.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/utils/__init__.py
+-rw-r--r--   0        0        0     2021 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/utils/inspect.py
+-rw-r--r--   0        0        0      662 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/utils/pyutils.py
+-rw-r--r--   0        0        0    10547 1970-01-01 00:00:00.000000 strawberry_resources-0.8.0/PKG-INFO
```

### Comparing `strawberry_resources-0.7.0/LICENSE` & `strawberry_resources-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/README.md` & `strawberry_resources-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/pyproject.toml` & `strawberry_resources-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-resources"
-version = "0.7.0"
+version = "0.8.0"
 description = "Introspection utilities to extract data from strawberry graphql"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-resources"
 repository = "https://github.com/blb-ventures/strawberry-resources"
 documentation = "https://github.com/blb-ventures/strawberry-resources"
@@ -26,46 +26,38 @@
 include = ["strawberry_resources/py.typed"]
 
 [tool.poetry.scripts]
 strawberry_resources = "strawberry_resources.cli:run"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-strawberry-graphql = ">= 0.140.3"
-strawberry-graphql-django = { version = ">=0.8", optional = true }
-strawberry-django-plus = { version = ">=2.0", optional = true }
+strawberry-graphql = ">= 0.196.2"
+strawberry-graphql-django = { version = ">=0.14.0", optional = true }
 django = { version = ">=3.2", optional = true }
 django-choices-field = { version = ">=2.0", optional = true }
 typing-extensions = ">= 4.2.0"
 click = ">=8.1.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
-strawberry-graphql-django = "^0.9.2"
-strawberry-django-plus = "^2.0"
+strawberry-graphql-django = "^0.14.0"
 django = "^4.1.0"
 django-choices-field = "^2.0"
 django-types = "^0.17.0"
 django-phonenumber-field = "^7.0.0"
 codecov = "^2.1.12"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 ipython = "^8.4.0"
 pytest-asyncio = "^0.21.0"
-ruff = "^0.0.272"
+ruff = "^0.0.280"
 pytest-django = "^4.5.2"
 
 [tool.poetry.extras]
-django = ["django", "strawberry-graphql-django"]
-django-plus = [
-  "django",
-  "strawberry-graphql-django",
-  "strawberry-django-plus",
-  "django-choices-field",
-]
+django = ["django", "strawberry-graphql-django", "django-choices-field"]
 
 [tool.ruff]
 line-length = 100
 select = [
   "E",
   "F",
   "W",
```

### Comparing `strawberry_resources-0.7.0/strawberry_resources/__init__.py` & `strawberry_resources-0.8.0/strawberry_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/strawberry_resources/cli/export.py` & `strawberry_resources-0.8.0/strawberry_resources/cli/export.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/strawberry_resources/exporter.py` & `strawberry_resources-0.8.0/strawberry_resources/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,21 +82,19 @@
     *,
     remove_nulls: bool = False,
     remove_nested_types_fields: bool = False,
 ):
     resource_map = get_resource_map(schema)
     data = {name: dataclasses.asdict(r) for name, r in resource_map.items()}
     remove_types = list(data) if remove_nested_types_fields else []
-    data = {
+    return {
         k: _fix_data(v, remove_nulls=remove_nulls, remove_fields_from_types=remove_types)
         for k, v in data.items()
     }
 
-    return data
-
 
 def to_json(
     schema: strawberry.Schema,
     *,
     remove_nulls: bool = False,
     remove_nested_types_fields: bool = False,
     **kwargs,
```

### Comparing `strawberry_resources-0.7.0/strawberry_resources/integrations/base.py` & `strawberry_resources-0.8.0/strawberry_resources/integrations/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import contextlib
 import dataclasses
 import pathlib
-from typing import TYPE_CHECKING, Callable, Dict, List, NoReturn, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, NoReturn, Type, Union
 
 from strawberry.field import StrawberryField
+from strawberry.type import WithStrawberryObjectDefinition
 
 if TYPE_CHECKING:
     from strawberry_resources.types import FieldKind, FieldOrFieldObjectOptions
 
 _integrations_imported: bool = False
 integrations: Dict[str, "StrawberryResourceIntegration"] = {}
 
 
 @dataclasses.dataclass
 class StrawberryResourceIntegration:
     name: str
     get_extra_mappings: Callable[[], Dict[type, "FieldKind"]]
     get_field_options: Callable[
-        [type, StrawberryField, type, bool],
+        [Type[WithStrawberryObjectDefinition], StrawberryField, type, bool],
         Union["FieldOrFieldObjectOptions", NoReturn],
     ]
     ordering: int = 0
 
     def __post_init__(self):
         integrations[self.name] = self
```

### Comparing `strawberry_resources-0.7.0/strawberry_resources/integrations/django.py` & `strawberry_resources-0.8.0/strawberry_resources/integrations/django.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.db.models.fields import NOT_PROVIDED
 from strawberry import UNSET
 from strawberry.field import StrawberryField
 from strawberry.scalars import JSON
-from strawberry.type import StrawberryOptional
+from strawberry.type import (
+    StrawberryOptional,
+    WithStrawberryObjectDefinition,
+    has_object_definition,
+)
 from strawberry_django.fields.types import (
     DjangoFileType,
     DjangoImageType,
     resolve_model_field_name,
 )
-from strawberry_django.type import StrawberryDjangoType
+from strawberry_django.utils.typing import get_django_definition
 from typing_extensions import Annotated, get_args, get_origin
 
 from strawberry_resources.types import (
     FieldObjectKind,
     FieldObjectOptions,
     FieldOrFieldObjectOptions,
 )
@@ -47,37 +51,31 @@
 try:
     from phonenumber_field.modelfields import PhoneNumberField
 except ImportError:
     PhoneNumberField = None
 
 # strawberry-django-plus might not be installed
 try:
-    from strawberry_django_plus import relay
-    from strawberry_django_plus.descriptors import ModelProperty
-    from strawberry_django_plus.types import K, ListInput
+    from strawberry_django.descriptors import ModelProperty
+    from strawberry_django.fields.types import K, ListInput
 except ImportError:
     ModelProperty = None
     ListInput = None
-    relay = None
     K = None
 
 if TYPE_CHECKING:
     from strawberry_resources.types import FieldKind
 
 # Try to use the smaller/faster cache decorator if available
 try:
     _cache = functools.cache  # type:ignore
 except AttributeError:  # pragma:nocover
     _cache = functools.lru_cache
 
 
-def _get_django_type(type_: type) -> Optional[StrawberryDjangoType]:
-    return getattr(type_, "_django_type", None)
-
-
 @_cache
 def _get_model_field(
     model: Type[models.Model],
     field: str,
 ) -> Optional[Union[models.Field, models.ForeignObjectRel]]:
     meta = model._meta
     for f in meta.get_fields():
@@ -87,26 +85,22 @@
 
     return None
 
 
 def get_extra_mappings() -> Dict[type, "FieldKind"]:
     from strawberry_resources.types import FieldKind
 
-    mappings: Dict[type, "FieldKind"] = {
+    return {
         DjangoImageType: FieldKind.IMAGE,
         DjangoFileType: FieldKind.FILE,
     }
-    if relay is not None:
-        mappings[relay.GlobalID] = FieldKind.ID
-
-    return mappings
 
 
 def get_field_options(
-    origin: type,
+    origin: Type[WithStrawberryObjectDefinition],
     field: "StrawberryField",
     resolved_type: type,
     is_list: bool,
 ) -> Union[FieldOrFieldObjectOptions, NoReturn]:
     from strawberry_resources.types import (
         DecimalFieldValidation,
         FieldChoice,
@@ -115,22 +109,16 @@
         FieldOptionsConfig,
         HiddenField,
         HiddenFieldError,
         StringFieldValidation,
     )
 
     options: FieldOptions = {}
-    if (
-        relay is not None
-        and isinstance(resolved_type, type)
-        and issubclass(resolved_type, relay.GlobalID)
-    ):
-        options["kind"] = FieldKind.ID
 
-    if (dj_type := _get_django_type(origin)) is not None:
+    if (dj_type := get_django_definition(origin)) is not None:
         model = dj_type.model
         model_attr = getattr(model, field.name, None)
     else:
         model = None
         model_attr = None
 
     # Try to populate options from the model property
@@ -147,15 +135,15 @@
             if not isinstance(opt, FieldOptionsConfig):
                 continue
 
             options.update(opt.options)
 
     dj_field = _get_model_field(model, field.name) if model is not None else None
 
-    if hasattr(resolved_type, "_type_definition"):
+    if has_object_definition(resolved_type):
         field_obj_options: FieldObjectOptions = {}
 
         assert isinstance(resolved_type, type)
         if ListInput is not None and issubclass(resolved_type, ListInput):
             assert isinstance(K, TypeVar)
             field_obj_options["obj_kind"] = FieldObjectKind.LIST_INPUT
 
@@ -198,21 +186,17 @@
 
     options["default_value"] = cast(Any, default_value)
     if choices is not None:
         options["choices"] = choices
 
     if dj_type:
         if (order := dj_type.order) and order is not UNSET:
-            options["orderable"] = field.name in {
-                f.name for f in dataclasses.fields(cast(type, order))
-            }
+            options["orderable"] = field.name in {f.name for f in dataclasses.fields(order)}
         if (filters := dj_type.filters) and filters is not UNSET:
-            options["filterable"] = field.name in {
-                f.name for f in dataclasses.fields(cast(type, filters))
-            }
+            options["filterable"] = field.name in {f.name for f in dataclasses.fields(filters)}
 
     if dj_field:
         if (label := getattr(dj_field, "verbose_name", None) or None) is not None:
             options["label"] = label
 
         if (help_text := getattr(dj_field, "help_Text", None) or None) is not None:
             options["help_text"] = help_text
```

### Comparing `strawberry_resources-0.7.0/strawberry_resources/queries.py` & `strawberry_resources-0.8.0/strawberry_resources/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/strawberry_resources/resolver.py` & `strawberry_resources-0.8.0/strawberry_resources/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import datetime
 import decimal
 import uuid
 from typing import (
     Dict,
     Optional,
     Tuple,
+    Type,
     TypeVar,
     cast,
 )
 
 import strawberry
 from django.db import models
-from strawberry import Schema
+from strawberry import Schema, relay
 from strawberry.custom_scalar import ScalarWrapper
 from strawberry.enum import EnumDefinition
 from strawberry.file_uploads import Upload
 from strawberry.lazy_type import LazyType
 from strawberry.scalars import JSON
-from strawberry.type import StrawberryContainer, StrawberryList, StrawberryOptional
+from strawberry.type import (
+    StrawberryContainer,
+    StrawberryList,
+    StrawberryOptional,
+    WithStrawberryObjectDefinition,
+    get_object_definition,
+)
 from strawberry.types.types import TypeDefinition
 from strawberry.utils.str_converters import to_camel_case
 from typing_extensions import Annotated, TypeAlias, get_args, get_origin
 
-from strawberry_resources.integrations.base import get_all
-from strawberry_resources.utils.inspect import get_possible_type_definitions
-from strawberry_resources.utils.pyutils import dict_merge
-
+from .integrations.base import get_all
 from .types import (
     BaseFieldValidation,
     Field,
     FieldChoice,
     FieldKind,
     FieldObject,
     FieldObjectKind,
     FieldOptions,
     FieldOptionsConfig,
     FieldOrFieldObjectOptions,
     HiddenField,
     HiddenFieldError,
     Resource,
 )
+from .utils.inspect import get_possible_type_definitions
+from .utils.pyutils import dict_merge
 
 _R = TypeVar("_R")
 _T = TypeVar("_T", bound=type)
 _M = TypeVar("_M", bound=models.Model)
 _TypeMap: TypeAlias = Dict[str, Resource]
 
 MAX_DEPTH = 5
@@ -56,14 +62,15 @@
     datetime.date: FieldKind.DATE,
     datetime.time: FieldKind.TIME,
     datetime.datetime: FieldKind.DATETIME,
     datetime.timedelta: FieldKind.TIMEDELTA,
     decimal.Decimal: FieldKind.DECIMAL,
     uuid.UUID: FieldKind.UUID,
     strawberry.ID: FieldKind.ID,
+    relay.GlobalID: FieldKind.ID,
     Upload.wrap: FieldKind.FILE,  # type: ignore
 }
 
 
 def get_resource_map(schema: "Schema") -> _TypeMap:
     if (type_map := type_name_map.get(schema)) is None:
         type_map = {}
@@ -86,23 +93,32 @@
     for _name, type_ in schema.schema_converter.type_map.items():
         for type_def in get_possible_type_definitions(type_.definition):
             if type_def.name in seen:
                 continue
 
             yield Resource(
                 name=type_def.name,
-                fields=list(resolve_fields_for_type(type_def.origin)),
+                fields=list(
+                    resolve_fields_for_type(
+                        cast(Type[WithStrawberryObjectDefinition], type_def.origin),
+                    ),
+                ),
             )
             seen.add(type_def.name)
 
 
-def resolve_fields_for_type(type_: type, *, depth: int = 0):
-    type_def = cast(TypeDefinition, type_._type_definition)  # type: ignore
+def resolve_fields_for_type(type_: Type[WithStrawberryObjectDefinition], *, depth: int = 0):
     integrations = get_all()
 
+    type_def = get_object_definition(type_, strict=True)
+
+    annotations = {}
+    for o in reversed(type_def.origin.__mro__):
+        annotations.update(getattr(o, "__annotations__", {}))
+
     for field in type_def.fields:
         cname = field.graphql_name or to_camel_case(field.name)
         hidden = False
         options: FieldOrFieldObjectOptions = {
             "label": field.name,
             "validation": BaseFieldValidation(
                 required=not isinstance(field.type, StrawberryOptional),
@@ -164,18 +180,14 @@
             except HiddenFieldError:
                 hidden = True
                 break
 
         if (f_kind := field_type_map.get(cast(type, f_type))) is not None:
             options["kind"] = f_kind  # type: ignore
 
-        annotations = {}
-        for o in reversed(type_def.origin.__mro__):
-            annotations.update(getattr(o, "__annotations__", {}))
-
         # Override those options with the field options
         if (
             (annotation := annotations.get(field.name)) and get_origin(annotation) is Annotated
         ) or (
             (resolver := getattr(type_def.origin, field.name, None))
             and hasattr(resolver, "__annotations__")
             and get_origin(annotation := resolver.__annotations__.get("return")) is Annotated
```

### Comparing `strawberry_resources-0.7.0/strawberry_resources/types.py` & `strawberry_resources-0.8.0/strawberry_resources/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/strawberry_resources/utils/inspect.py` & `strawberry_resources-0.8.0/strawberry_resources/utils/inspect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import itertools
 from typing import Generator, Optional, Union
 
 from strawberry.lazy_type import LazyType
-from strawberry.type import StrawberryContainer, StrawberryType, StrawberryTypeVar
-from strawberry.types.types import TypeDefinition
+from strawberry.type import (
+    StrawberryContainer,
+    StrawberryType,
+    StrawberryTypeVar,
+    get_object_definition,
+)
+from strawberry.types.types import StrawberryObjectDefinition
 from strawberry.union import StrawberryUnion
 from typing_extensions import assert_never
 
 
 def get_possible_types(
-    gql_type: Union[TypeDefinition, StrawberryType, type],
-    type_def: Optional[TypeDefinition] = None,
+    gql_type: Union[StrawberryObjectDefinition, StrawberryType, type],
+    *,
+    object_definition: Optional[StrawberryObjectDefinition] = None,
 ) -> Generator[type, None, None]:
-    if isinstance(gql_type, TypeDefinition):
-        yield from get_possible_types(gql_type.origin, type_def=gql_type)
+    if isinstance(gql_type, StrawberryObjectDefinition):
+        yield from get_possible_types(gql_type.origin, object_definition=gql_type)
     elif isinstance(gql_type, LazyType):
         yield from get_possible_types(gql_type.resolve_type())
-    elif isinstance(gql_type, StrawberryTypeVar) and type_def is not None:
-        # Try to resolve TypeVar
-        for f in type_def.fields:
-            f_type = f.type
-            if not isinstance(f_type, StrawberryTypeVar):
-                continue
-
-            resolved = type_def.type_var_map.get(f_type.type_var, None)
-            if resolved is not None:
-                yield from get_possible_types(resolved)
+    elif isinstance(gql_type, StrawberryTypeVar) and object_definition is not None:
+        resolved = object_definition.type_var_map.get(gql_type.type_var, None)
+        if resolved is not None:
+            yield from get_possible_types(resolved)
     elif isinstance(gql_type, StrawberryContainer):
         yield from get_possible_types(gql_type.of_type)
     elif isinstance(gql_type, StrawberryUnion):
         yield from itertools.chain.from_iterable(
             (get_possible_types(t) for t in gql_type.types),
         )
     elif isinstance(gql_type, StrawberryType):
@@ -38,18 +38,18 @@
     elif isinstance(gql_type, type):
         yield gql_type
     else:
         assert_never(gql_type)
 
 
 def get_possible_type_definitions(
-    gql_type: Union[TypeDefinition, StrawberryType, type],
-) -> Generator[TypeDefinition, None, None]:
-    if isinstance(gql_type, TypeDefinition):
+    gql_type: Union[StrawberryObjectDefinition, StrawberryType, type],
+) -> Generator[StrawberryObjectDefinition, None, None]:
+    if isinstance(gql_type, StrawberryObjectDefinition):
         yield gql_type
         return
 
     for t in get_possible_types(gql_type):
-        if isinstance(t, TypeDefinition):
+        if isinstance(t, StrawberryObjectDefinition):
             yield t
-        elif hasattr(t, "_type_definition"):
-            yield t._type_definition  # type: ignore
+        elif (type_def := get_object_definition(t)) is not None:
+            yield type_def
```

### Comparing `strawberry_resources-0.7.0/strawberry_resources/utils/pyutils.py` & `strawberry_resources-0.8.0/strawberry_resources/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.7.0/PKG-INFO` & `strawberry_resources-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-resources
-Version: 0.7.0
+Version: 0.8.0
 Summary: Introspection utilities to extract data from strawberry graphql
 Home-page: https://github.com/blb-ventures/strawberry-resources
 License: MIT
 Keywords: strawberry,django,graphql,resources,forms
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -16,21 +16,19 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: django
-Provides-Extra: django-plus
 Requires-Dist: click (>=8.1.3)
-Requires-Dist: django (>=3.2) ; extra == "django" or extra == "django-plus"
-Requires-Dist: django-choices-field (>=2.0) ; extra == "django-plus"
-Requires-Dist: strawberry-django-plus (>=2.0) ; extra == "django-plus"
-Requires-Dist: strawberry-graphql (>=0.140.3)
-Requires-Dist: strawberry-graphql-django (>=0.8) ; extra == "django" or extra == "django-plus"
+Requires-Dist: django (>=3.2) ; extra == "django"
+Requires-Dist: django-choices-field (>=2.0) ; extra == "django"
+Requires-Dist: strawberry-graphql (>=0.196.2)
+Requires-Dist: strawberry-graphql-django (>=0.14.0) ; extra == "django"
 Requires-Dist: typing-extensions (>=4.2.0)
 Project-URL: Documentation, https://github.com/blb-ventures/strawberry-resources
 Project-URL: Repository, https://github.com/blb-ventures/strawberry-resources
 Description-Content-Type: text/markdown
 
 # strawberry-resources
```

