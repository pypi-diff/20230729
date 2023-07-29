# Comparing `tmp/mypy-protobuf-3.4.0.tar.gz` & `tmp/mypy-protobuf-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-protobuf-3.4.0.tar", last modified: Thu Oct 20 06:15:24 2022, max compression
+gzip compressed data, was "mypy-protobuf-3.5.0.tar", last modified: Sat Jul 29 00:22:30 2023, max compression
```

## Comparing `mypy-protobuf-3.4.0.tar` & `mypy-protobuf-3.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2022-10-20 06:15:24.590424 mypy-protobuf-3.4.0/
--rw-r--r--   0 nipunn     (501) staff       (20)    11348 2022-01-28 23:16:18.000000 mypy-protobuf-3.4.0/LICENSE
--rw-r--r--   0 nipunn     (501) staff       (20)      395 2022-10-20 06:15:24.590506 mypy-protobuf-3.4.0/PKG-INFO
--rw-r--r--   0 nipunn     (501) staff       (20)    10496 2022-10-20 06:14:18.000000 mypy-protobuf-3.4.0/README.md
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2022-10-20 06:15:24.588961 mypy-protobuf-3.4.0/mypy_protobuf/
--rw-r--r--   0 nipunn     (501) staff       (20)        0 2021-12-24 22:07:25.000000 mypy-protobuf-3.4.0/mypy_protobuf/__init__.py
--rw-r--r--   0 nipunn     (501) staff       (20)     2135 2022-10-18 20:27:59.000000 mypy-protobuf-3.4.0/mypy_protobuf/extensions_pb2.py
--rw-r--r--   0 nipunn     (501) staff       (20)    41207 2022-10-20 06:14:18.000000 mypy-protobuf-3.4.0/mypy_protobuf/main.py
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2022-10-20 06:15:24.590005 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/
--rw-r--r--   0 nipunn     (501) staff       (20)      395 2022-10-20 06:15:24.000000 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 nipunn     (501) staff       (20)      398 2022-10-20 06:15:24.000000 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 nipunn     (501) staff       (20)        1 2022-10-20 06:15:24.000000 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 nipunn     (501) staff       (20)      107 2022-10-20 06:15:24.000000 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/entry_points.txt
--rw-r--r--   0 nipunn     (501) staff       (20)       40 2022-10-20 06:15:24.000000 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/requires.txt
--rw-r--r--   0 nipunn     (501) staff       (20)       14 2022-10-20 06:15:24.000000 mypy-protobuf-3.4.0/mypy_protobuf.egg-info/top_level.txt
--rw-r--r--   0 nipunn     (501) staff       (20)      584 2022-09-05 16:46:27.000000 mypy-protobuf-3.4.0/pyproject.toml
--rw-r--r--   0 nipunn     (501) staff       (20)      726 2022-10-20 06:15:24.590789 mypy-protobuf-3.4.0/setup.cfg
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2022-10-20 06:15:24.590316 mypy-protobuf-3.4.0/test/
--rw-r--r--   0 nipunn     (501) staff       (20)    18098 2022-10-20 06:04:17.000000 mypy-protobuf-3.4.0/test/test_generated_mypy.py
--rw-r--r--   0 nipunn     (501) staff       (20)     2585 2022-08-23 09:57:11.000000 mypy-protobuf-3.4.0/test/test_grpc_usage.py
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.727557 mypy-protobuf-3.5.0/
+-rw-r--r--   0 nipunn     (501) staff       (20)    11348 2022-01-28 23:16:18.000000 mypy-protobuf-3.5.0/LICENSE
+-rw-r--r--   0 nipunn     (501) staff       (20)      395 2023-07-29 00:22:30.727609 mypy-protobuf-3.5.0/PKG-INFO
+-rw-r--r--   0 nipunn     (501) staff       (20)    10565 2023-07-29 00:15:31.000000 mypy-protobuf-3.5.0/README.md
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.726272 mypy-protobuf-3.5.0/mypy_protobuf/
+-rw-r--r--   0 nipunn     (501) staff       (20)        0 2021-12-24 22:07:25.000000 mypy-protobuf-3.5.0/mypy_protobuf/__init__.py
+-rw-r--r--   0 nipunn     (501) staff       (20)     2178 2023-07-28 22:09:30.000000 mypy-protobuf-3.5.0/mypy_protobuf/extensions_pb2.py
+-rw-r--r--   0 nipunn     (501) staff       (20)    44145 2023-07-29 00:22:05.000000 mypy-protobuf-3.5.0/mypy_protobuf/main.py
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.727057 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/
+-rw-r--r--   0 nipunn     (501) staff       (20)      395 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 nipunn     (501) staff       (20)      428 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)        1 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)      107 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/entry_points.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)       42 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/requires.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)       14 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)      584 2023-07-29 00:08:49.000000 mypy-protobuf-3.5.0/pyproject.toml
+-rw-r--r--   0 nipunn     (501) staff       (20)      728 2023-07-29 00:22:30.727854 mypy-protobuf-3.5.0/setup.cfg
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.727453 mypy-protobuf-3.5.0/test/
+-rw-r--r--   0 nipunn     (501) staff       (20)    18031 2023-07-28 22:09:30.000000 mypy-protobuf-3.5.0/test/test_generated_mypy.py
+-rw-r--r--   0 nipunn     (501) staff       (20)     2413 2023-07-28 20:41:01.000000 mypy-protobuf-3.5.0/test/test_grpc_async_usage.py
+-rw-r--r--   0 nipunn     (501) staff       (20)     2585 2022-08-23 09:57:11.000000 mypy-protobuf-3.5.0/test/test_grpc_usage.py
```

### Comparing `mypy-protobuf-3.4.0/LICENSE` & `mypy-protobuf-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-protobuf-3.4.0/README.md` & `mypy-protobuf-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,66 +8,81 @@
 2.10 is the last version of mypy-protobuf which supports targeting python 2.7.
 
 Built originally with love at [Dropbox](https://github.com/dropbox)
 
 See [Changelog](CHANGELOG.md) for recent changes.
 
 ## Requirements to run mypy-protobuf
+
 Earlier releases might work, but aren't tested
-- [protoc >= 4.21.8](https://github.com/protocolbuffers/protobuf/releases)
-- [python-protobuf >= 4.21.8](https://pypi.org/project/protobuf/) - matching protoc release
-- [python >= 3.7](https://www.python.org/downloads/source/) - for running mypy-protobuf plugin.
+
+- [protoc >= 23.4](https://github.com/protocolbuffers/protobuf/releases)
+- [python-protobuf >= 4.23.4](https://pypi.org/project/protobuf/) - matching protoc release
+- [python >= 3.8](https://www.python.org/downloads/source/) - for running mypy-protobuf plugin.
 
 ## Requirements to run typecheckers on stubs generated by mypy-protobuf
+
 Earlier releases might work, but aren't tested
-- [mypy >= v0.941](https://pypi.org/project/mypy) or [pyright >= 1.1.206](https://github.com/microsoft/pyright)
-- [python-protobuf >= 4.21.8](https://pypi.org/project/protobuf/) - matching protoc release
-- [types-protobuf >= 3.20.4](https://pypi.org/project/types-protobuf/) - for stubs from the google.protobuf library
+
+- [mypy >= v1.4.1](https://pypi.org/project/mypy) or [pyright >= 1.1.206](https://github.com/microsoft/pyright)
+- [python-protobuf >= 4.23.4](https://pypi.org/project/protobuf/) - matching protoc release
+- [types-protobuf >= 4.23.0.2](https://pypi.org/project/types-protobuf/) - for stubs from the google.protobuf library
 
 ### To run typecheckers on code generated with grpc plugin - you'll additionally need
+
 Earlier releases might work, but aren't tested
-- [grpcio>=1.50.0](https://pypi.org/project/grpcio/)
-- [grpcio-tools>=1.50.0](https://pypi.org/project/grpcio-tools/)
-- [grpc-stubs>=1.24.9](https://pypi.org/project/grpc-stubs/)
+
+- [grpcio>=1.56.2](https://pypi.org/project/grpcio/)
+- [grpcio-tools>=1.56.2](https://pypi.org/project/grpcio-tools/)
+- [grpc-stubs>=1.53.0.2](https://pypi.org/project/grpc-stubs/)
 
 Other configurations may work, but are not continuously tested currently.
 We would be open to expanding this list - file an issue on the issue tracker.
 
 ## Installation
 
 The plugin can be installed with
+
 ```
 pip3 install mypy-protobuf
 ```
+
 To install unreleased
+
 ```
 REV=main  # or whichever unreleased git rev you'd like
 pip3 install git+https://github.com/nipunn1313/mypy-protobuf.git@$REV
 
 # For older (1.x) versions of mypy protobuf - you may need
 pip3 install git+https://github.com/nipunn1313/mypy-protobuf.git@$REV#subdirectory=python
 ```
 
 In order to run mypy on the generated code, you'll need to install
+
 ```
 pip3 install mypy>=0.910 types-protobuf>=0.1.14
 ```
 
 # Usage
 
 On posix, protoc-gen-mypy is installed to python's executable bin. Assuming that's
 on your $PATH, you can run
+
 ```
 protoc --python_out=output/location --mypy_out=output/location
 ```
+
 Alternately, you can explicitly provide the path:
+
 ```
 protoc --plugin=protoc-gen-mypy=path/to/protoc-gen-mypy --python_out=output/location --mypy_out=output/location
 ```
+
 Check the version number with
+
 ```
 > protoc-gen-mypy --version
 ```
 
 ## Implementation
 
 The implementation of the plugin is in `mypy_protobuf/main.py`, which installs to
@@ -81,52 +96,57 @@
 
 Comments in the .proto files on messages, fields, enums, enum variants, extensions, services, and methods
 will appear as docstrings in .pyi files. Useful in IDEs for showing completions with comments.
 
 ### Types enum int values more strongly
 
 Enum int values produce stubs which wrap the int values in NewType
+
 ```proto
 enum MyEnum {
   HELLO = 0;
   WORLD = 1;
 }
 ```
+
 Will yield an [enum type wrapper](https://github.com/python/typeshed/blob/16ae4c61201cd8b96b8b22cdfb2ab9e89ba5bcf2/stubs/protobuf/google/protobuf/internal/enum_type_wrapper.pyi) whose methods type to `MyEnum.ValueType` (a `NewType(int)` rather than `int`.
 This allows mypy to catch bugs where the wrong enum value is being used.
 
 Calling code may be typed as follows.
 
 In python >= 3.7
+
 ```python
 # May need [PEP 563](https://www.python.org/dev/peps/pep-0563/) to postpone evaluation of annotations
 # from __future__ import annotations  # Not needed with python>=3.11 or protobuf>=3.20.0
 def f(x: MyEnum.ValueType):
     print(x)
 f(MyEnum.Value("HELLO"))
 ```
 
 With protobuf <= 3.20.0, for usages of cast, the type of `x` must be quoted
 After protobuf >= 3.20.0 - `ValueType` exists in the python code and quotes aren't needed
 until [upstream protobuf](https://github.com/protocolbuffers/protobuf/pull/8182) includes `ValueType`
+
 ```python
 cast('MyEnum.ValueType', x)
 ```
 
 Similarly, for type aliases with protobuf < 3.20.0, you must either quote the type or hide it behind `TYPE_CHECKING`
+
 ```python
 from typing import Tuple, TYPE_CHECKING
 HELLO = Tuple['MyEnum.ValueType', 'MyEnum.ValueType']
 if TYPE_CHECKING:
     HELLO = Tuple[MyEnum.ValueType, MyEnum.ValueType]
 ```
 
 #### Enum int impl details
 
-mypy-protobuf  autogenerates an instance of the EnumTypeWrapper as follows.
+mypy-protobuf autogenerates an instance of the EnumTypeWrapper as follows.
 
 ```python
 class _MyEnum:
     ValueType = typing.NewType('ValueType', builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 class _MyEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_MyEnum.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
@@ -137,49 +157,54 @@
 
 HELLO: MyEnum.ValueType  # 0
 WORLD: MyEnum.ValueType  # 1
 ```
 
 `_MyEnumEnumTypeWrapper` extends the EnumTypeWrapper to take/return MyEnum.ValueType rather than int
 `MyEnum` is an instance of the `EnumTypeWrapper`.
+
 - Use `_MyEnum` and of metaclass is an implementation detail to make MyEnum.ValueType a valid type w/o a circular dependency
 - `V` is supported as an alias of `ValueType` for backward compatibility
 
-
-
 ### Supports generating type wrappers for fields and maps
 
 M.proto
+
 ```proto
 message M {
   uint32 user_id = 1 [(mypy_protobuf.options).casttype="mymod.UserId"];
   map<uint32, string> email_by_uid = 2 [
     (mypy_protobuf.options).keytype="path/to/mymod.UserId",
     (mypy_protobuf.options).valuetype="path/to/mymod.Email"
   ];
 }
 ```
+
 mymod.py
+
 ```python
 UserId = NewType("UserId", int)
 Email = NewType("Email", Text)
 ```
 
 ### `py_generic_services`
+
 If `py_generic_services` is set in your proto file, then mypy-protobuf will
 generate service stubs. If you want GRPC stubs instead - use the GRPC instructions.
 
 ### `readable_stubs`
+
 If `readable_stubs` is set, mypy-protobuf will generate easier-to-read stubs. The downside
 to this approach - is that it's possible to generate stubs which do not pass mypy - particularly
 in the case of name collisions. mypy-protobuf defaults to generating stubs with fully qualified
 imports and mangled global-level identifiers to defend against name collisions between global
 identifiers and field names.
 
 If you're ok with this risk, try it out!
+
 ```
 protoc --python_out=output/location --mypy_out=readable_stubs:output/location
 ```
 
 ### `relax_strict_optional_primitives`
 
 If you are using proto3, then primitives cannot be represented as NULL on the wire -
@@ -191,46 +216,51 @@
 However, it may be helpful when migrating existing proto2 code, where the distinction is meaningful
 
 ```
 protoc --python_out=output/location --mypy_out=relax_strict_optional_primitives:output/location
 ```
 
 ### Output suppression
+
 To suppress output, you can run
+
 ```
 protoc --python_out=output/location --mypy_out=quiet:output/location
 ```
 
 ### GRPC
 
 This plugin provides stubs generation for grpcio generated code.
+
 ```
 protoc \
     --python_out=output/location \
     --mypy_out=output/location \
     --grpc_out=output/location \
     --mypy_grpc_out=output/location
 ```
 
 Note that generated code for grpc will work only together with code for python and locations should be the same.
-If you need stubs for grpc internal code we suggest using this package https://github.com/shabbyrobe/grpc-stubs 
+If you need stubs for grpc internal code we suggest using this package https://github.com/shabbyrobe/grpc-stubs
 
 ### Targeting python2 support
 
 mypy-protobuf's drops support for targeting python2 with version 3.0. If you still need python2 support -
+
 ```
 python3 -m pip install mypy_protobuf==2.10
 protoc --python_out=output/location --mypy_out=output/location
 mypy --target-version=2.7 {files}
 ```
 
-
 ## Contributing
+
 Contributions to the implementation are welcome. Please run tests using `./run_test.sh`.
 Ensure code is formatted using black.
+
 ```
 pip3 install black
 black .
 ```
 
 ## Contributors
 
@@ -267,13 +297,13 @@
 - [@alkasm](https://github.com/alkasm)
 - [@tarmath](https://github.com/tarmath)
 - [@jaredkhan](https://github.com/jaredkhan)
 - [@sodul](https://github.com/sodul)
 - [@miaachan](https://github.com/miaachan)
 - [@Alphadelta14](https://github.com/Alphadelta14)
 - [@fergyfresh](https://github.com/fergyfresh)
+- [@AlexWaygood](https://github.com/AlexWaygood)
 
-Licence etc.
-------------
+## Licence etc.
 
 1. License: Apache 2.0.
 2. Copyright attribution: Copyright (c) 2022 Nipunn Koorapati
```

### Comparing `mypy-protobuf-3.4.0/mypy_protobuf/extensions_pb2.py` & `mypy-protobuf-3.5.0/mypy_protobuf/extensions_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: mypy_protobuf/extensions.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emypy_protobuf/extensions.proto\x12\rmypy_protobuf\x1a google/protobuf/descriptor.proto\"D\n\x0c\x46ieldOptions\x12\x10\n\x08\x63\x61sttype\x18\x01 \x01(\t\x12\x0f\n\x07keytype\x18\x02 \x01(\t\x12\x11\n\tvaluetype\x18\x03 \x01(\t:L\n\x07options\x12\x1d.google.protobuf.FieldOptions\x18\x82\t \x01(\x0b\x32\x1b.mypy_protobuf.FieldOptions:4\n\x08\x63\x61sttype\x12\x1d.google.protobuf.FieldOptions\x18\xff\x08 \x01(\tB\x02\x18\x01:3\n\x07keytype\x12\x1d.google.protobuf.FieldOptions\x18\x80\t \x01(\tB\x02\x18\x01:5\n\tvaluetype\x12\x1d.google.protobuf.FieldOptions\x18\x81\t \x01(\tB\x02\x18\x01\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mypy_protobuf.extensions_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mypy_protobuf.extensions_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(options)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(casttype)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(keytype)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(valuetype)
 
   DESCRIPTOR._options = None
   casttype._options = None
   casttype._serialized_options = b'\030\001'
   keytype._options = None
   keytype._serialized_options = b'\030\001'
   valuetype._options = None
   valuetype._serialized_options = b'\030\001'
-  _FIELDOPTIONS._serialized_start=83
-  _FIELDOPTIONS._serialized_end=151
+  _globals['_FIELDOPTIONS']._serialized_start=83
+  _globals['_FIELDOPTIONS']._serialized_end=151
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mypy-protobuf-3.4.0/mypy_protobuf/main.py` & `mypy-protobuf-3.5.0/mypy_protobuf/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import google.protobuf.descriptor_pb2 as d
 from google.protobuf.compiler import plugin_pb2 as plugin_pb2
 from google.protobuf.internal.containers import RepeatedCompositeFieldContainer
 from google.protobuf.internal.well_known_types import WKTBASES
 from . import extensions_pb2
 
-__version__ = "3.4.0"
+__version__ = "3.5.0"
 
 # SourceCodeLocation is defined by `message Location` here
 # https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/descriptor.proto
 SourceCodeLocation = List[int]
 
 # So phabricator doesn't think mypy_protobuf.py is generated
 GENERATED = "@ge" + "nerated"
@@ -342,20 +342,19 @@
                     self._import("typing", "NewType"),
                     self._builtin("int"),
                 )
                 # Alias to the classic shorter definition "V"
                 wl("V: {} = ValueType", self._import("typing_extensions", "TypeAlias"))
             wl("")
             wl(
-                "class {}({}[{}], {}):{}",
+                "class {}({}[{}], {}):",
                 etw_helper_class,
                 self._import("google.protobuf.internal.enum_type_wrapper", "_EnumTypeWrapper"),
                 value_type_helper_fq,
                 self._builtin("type"),
-                "  # noqa: F821" if prefix else "",
             )
             with self._indent():
                 ed = self._import("google.protobuf.descriptor", "EnumDescriptor")
                 wl(f"DESCRIPTOR: {ed}")
                 self.write_enum_values(
                     [(i, v) for i, v in enumerate(enum.value) if v.name not in PROTO_ENUM_RESERVED],
                     value_type_helper_fq,
@@ -456,16 +455,15 @@
 
                 self.write_extensions(desc.extension, scl + [d.DescriptorProto.EXTENSION_FIELD_NUMBER])
 
                 # Constructor
                 wl("def __init__(")
                 with self._indent():
                     if any(f.name == "self" for f in desc.field):
-                        wl("# pyright: reportSelfClsParameterName=false")
-                        wl("self_,")
+                        wl("self_,  # pyright: ignore[reportSelfClsParameterName]")
                     else:
                         wl("self,")
                 with self._indent():
                     constructor_fields = [f for f in desc.field if f.name not in PYTHON_RESERVED]
                     if len(constructor_fields) > 0:
                         # Only positional args allowed
                         # See https://github.com/nipunn1313/mypy-protobuf/issues/71
@@ -573,15 +571,15 @@
         if not methods:
             wl("...")
         for i, method in methods:
             if is_abstract:
                 wl("@{}", self._import("abc", "abstractmethod"))
             wl(f"def {method.name}(")
             with self._indent():
-                wl(f"inst: {class_name},")
+                wl(f"inst: {class_name},  # pyright: ignore[reportSelfClsParameterName]")
                 wl(
                     "rpc_controller: {},",
                     self._import("google.protobuf.service", "RpcController"),
                 )
                 wl("request: {},", self._import_message(method.input_type))
                 wl(
                     "callback: {}[[{}], None] | None{},",
@@ -659,78 +657,125 @@
         if oldstyle_valuetype:
             print(f"Warning: Map Field {map_field.name}: (mypy_protobuf.valuetype) is deprecated. Prefer (mypy_protobuf.options).valuetype", file=sys.stderr)
         value_casttype = map_field.options.Extensions[extensions_pb2.options].valuetype or map_field.options.Extensions[extensions_pb2.valuetype]
         vtype = self._import_casttype(value_casttype) if value_casttype else self.python_type(value_field)
 
         return ktype, vtype
 
-    def _callable_type(self, method: d.MethodDescriptorProto) -> str:
+    def _callable_type(self, method: d.MethodDescriptorProto, is_async: bool = False) -> str:
+        module = "grpc.aio" if is_async else "grpc"
         if method.client_streaming:
             if method.server_streaming:
-                return self._import("grpc", "StreamStreamMultiCallable")
+                return self._import(module, "StreamStreamMultiCallable")
             else:
-                return self._import("grpc", "StreamUnaryMultiCallable")
+                return self._import(module, "StreamUnaryMultiCallable")
         else:
             if method.server_streaming:
-                return self._import("grpc", "UnaryStreamMultiCallable")
+                return self._import(module, "UnaryStreamMultiCallable")
             else:
-                return self._import("grpc", "UnaryUnaryMultiCallable")
+                return self._import(module, "UnaryUnaryMultiCallable")
 
-    def _input_type(self, method: d.MethodDescriptorProto, use_stream_iterator: bool = True) -> str:
+    def _input_type(self, method: d.MethodDescriptorProto) -> str:
         result = self._import_message(method.input_type)
-        if use_stream_iterator and method.client_streaming:
-            result = f"{self._import('collections.abc', 'Iterator')}[{result}]"
         return result
 
-    def _output_type(self, method: d.MethodDescriptorProto, use_stream_iterator: bool = True) -> str:
+    def _servicer_input_type(self, method: d.MethodDescriptorProto) -> str:
+        result = self._import_message(method.input_type)
+        if method.client_streaming:
+            # See write_grpc_async_hacks().
+            result = f"_MaybeAsyncIterator[{result}]"
+        return result
+
+    def _output_type(self, method: d.MethodDescriptorProto) -> str:
         result = self._import_message(method.output_type)
-        if use_stream_iterator and method.server_streaming:
-            result = f"{self._import('collections.abc', 'Iterator')}[{result}]"
         return result
 
+    def _servicer_output_type(self, method: d.MethodDescriptorProto) -> str:
+        result = self._import_message(method.output_type)
+        if method.server_streaming:
+            # Union[Iterator[Resp], AsyncIterator[Resp]] is subtyped by Iterator[Resp] and AsyncIterator[Resp].
+            # So both can be used in the covariant function return position.
+            iterator = f"{self._import('collections.abc', 'Iterator')}[{result}]"
+            aiterator = f"{self._import('collections.abc', 'AsyncIterator')}[{result}]"
+            result = f"{self._import('typing', 'Union')}[{iterator}, {aiterator}]"
+        else:
+            # Union[Resp, Awaitable[Resp]] is subtyped by Resp and Awaitable[Resp].
+            # So both can be used in the covariant function return position.
+            # Awaitable[Resp] is equivalent to async def.
+            awaitable = f"{self._import('collections.abc', 'Awaitable')}[{result}]"
+            result = f"{self._import('typing', 'Union')}[{result}, {awaitable}]"
+        return result
+
+    def write_grpc_async_hacks(self) -> None:
+        wl = self._write_line
+        # _MaybeAsyncIterator[Req] is supertyped by Iterator[Req] and AsyncIterator[Req].
+        # So both can be used in the contravariant function parameter position.
+        wl("_T = {}('_T')", self._import("typing", "TypeVar"))
+        wl("")
+        wl(
+            "class _MaybeAsyncIterator({}[_T], {}[_T], metaclass={}):",
+            self._import("collections.abc", "AsyncIterator"),
+            self._import("collections.abc", "Iterator"),
+            self._import("abc", "ABCMeta"),
+        )
+        with self._indent():
+            wl("...")
+        wl("")
+
+        # _ServicerContext is supertyped by grpc.ServicerContext and grpc.aio.ServicerContext
+        # So both can be used in the contravariant function parameter position.
+        wl(
+            "class _ServicerContext({}, {}):  # type: ignore",
+            self._import("grpc", "ServicerContext"),
+            self._import("grpc.aio", "ServicerContext"),
+        )
+        with self._indent():
+            wl("...")
+        wl("")
+
     def write_grpc_methods(self, service: d.ServiceDescriptorProto, scl_prefix: SourceCodeLocation) -> None:
         wl = self._write_line
         methods = [(i, m) for i, m in enumerate(service.method) if m.name not in PYTHON_RESERVED]
         if not methods:
             wl("...")
             wl("")
         for i, method in methods:
             scl = scl_prefix + [d.ServiceDescriptorProto.METHOD_FIELD_NUMBER, i]
 
             wl("@{}", self._import("abc", "abstractmethod"))
             wl("def {}(", method.name)
             with self._indent():
                 wl("self,")
                 input_name = "request_iterator" if method.client_streaming else "request"
-                input_type = self._input_type(method)
+                input_type = self._servicer_input_type(method)
                 wl(f"{input_name}: {input_type},")
-                wl("context: {},", self._import("grpc", "ServicerContext"))
+                wl("context: _ServicerContext,")
             wl(
                 ") -> {}:{}",
-                self._output_type(method),
+                self._servicer_output_type(method),
                 " ..." if not self._has_comments(scl) else "",
             )
             if self._has_comments(scl):
                 with self._indent():
                     if not self._write_comments(scl):
                         wl("...")
 
-    def write_grpc_stub_methods(self, service: d.ServiceDescriptorProto, scl_prefix: SourceCodeLocation) -> None:
+    def write_grpc_stub_methods(self, service: d.ServiceDescriptorProto, scl_prefix: SourceCodeLocation, is_async: bool = False) -> None:
         wl = self._write_line
         methods = [(i, m) for i, m in enumerate(service.method) if m.name not in PYTHON_RESERVED]
         if not methods:
             wl("...")
             wl("")
         for i, method in methods:
             scl = scl_prefix + [d.ServiceDescriptorProto.METHOD_FIELD_NUMBER, i]
 
-            wl("{}: {}[", method.name, self._callable_type(method))
+            wl("{}: {}[", method.name, self._callable_type(method, is_async=is_async))
             with self._indent():
-                wl("{},", self._input_type(method, False))
-                wl("{},", self._output_type(method, False))
+                wl("{},", self._input_type(method))
+                wl("{},", self._output_type(method))
             wl("]")
             self._write_comments(scl)
 
     def write_grpc_services(
         self,
         services: Iterable[d.ServiceDescriptorProto],
         scl_prefix: SourceCodeLocation,
@@ -739,41 +784,57 @@
         for i, service in enumerate(services):
             if service.name in PYTHON_RESERVED:
                 continue
 
             scl = scl_prefix + [i]
 
             # The stub client
-            wl(f"class {service.name}Stub:")
+            wl(
+                "class {}Stub:",
+                service.name,
+            )
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
-                wl(
-                    "def __init__(self, channel: {}) -> None: ...",
-                    self._import("grpc", "Channel"),
-                )
+                # To support casting into FooAsyncStub, allow both Channel and aio.Channel here.
+                channel = f"{self._import('typing', 'Union')}[{self._import('grpc', 'Channel')}, {self._import('grpc.aio', 'Channel')}]"
+                wl("def __init__(self, channel: {}) -> None: ...", channel)
                 self.write_grpc_stub_methods(service, scl)
             wl("")
 
+            # The (fake) async stub client
+            wl(
+                "class {}AsyncStub:",
+                service.name,
+            )
+            with self._indent():
+                if self._write_comments(scl):
+                    wl("")
+                # No __init__ since this isn't a real class (yet), and requires manual casting to work.
+                self.write_grpc_stub_methods(service, scl, is_async=True)
+            wl("")
+
             # The service definition interface
             wl(
                 "class {}Servicer(metaclass={}):",
                 service.name,
                 self._import("abc", "ABCMeta"),
             )
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
                 self.write_grpc_methods(service, scl)
             wl("")
+            server = self._import("grpc", "Server")
+            aserver = self._import("grpc.aio", "Server")
             wl(
                 "def add_{}Servicer_to_server(servicer: {}Servicer, server: {}) -> None: ...",
                 service.name,
                 service.name,
-                self._import("grpc", "Server"),
+                f"{self._import('typing', 'Union')}[{server}, {aserver}]",
             )
             wl("")
 
     def python_type(self, field: d.FieldDescriptorProto, generic_container: bool = False) -> str:
         """
         generic_container
           if set, type the field with generic interfaces. Eg.
@@ -888,15 +949,15 @@
             self._write_line(f"if sys.version_info >= {self.typing_extensions_min}:")
             self._write_line("    import typing as typing_extensions")
             self._write_line("else:")
             self._write_line("    import typing_extensions")
 
         for pkg, items in sorted(self.from_imports.items()):
             self._write_line(f"from {pkg} import (")
-            for (name, reexport_name) in sorted(items):
+            for name, reexport_name in sorted(items):
                 if reexport_name is None:
                     self._write_line(f"    {name},")
                 else:
                     self._write_line(f"    {name} as {reexport_name},")
             self._write_line(")")
         self._write_line("")
 
@@ -956,29 +1017,28 @@
         pkg_writer = PkgWriter(
             fd,
             descriptors,
             readable_stubs,
             relax_strict_optional_primitives,
             grpc=True,
         )
+        pkg_writer.write_grpc_async_hacks()
         pkg_writer.write_grpc_services(fd.service, [d.FileDescriptorProto.SERVICE_FIELD_NUMBER])
 
         assert name == fd.name
         assert fd.name.endswith(".proto")
         output = response.file.add()
         output.name = fd.name[:-6].replace("-", "_").replace(".", "/") + "_pb2_grpc.pyi"
         output.content = pkg_writer.write()
         if not quiet:
             print("Writing mypy to", output.name, file=sys.stderr)
 
 
 @contextmanager
-def code_generation() -> Iterator[
-    Tuple[plugin_pb2.CodeGeneratorRequest, plugin_pb2.CodeGeneratorResponse],
-]:
+def code_generation() -> Iterator[Tuple[plugin_pb2.CodeGeneratorRequest, plugin_pb2.CodeGeneratorResponse],]:
     if len(sys.argv) > 1 and sys.argv[1] in ("-V", "--version"):
         print("mypy-protobuf " + __version__)
         sys.exit(0)
 
     # Read request message from stdin
     data = sys.stdin.buffer.read()
```

### Comparing `mypy-protobuf-3.4.0/pyproject.toml` & `mypy-protobuf-3.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [tool.mypy]
 strict = true
 show_error_codes = true
 
 [tool.pyright]
 venvPath = "."
-venv = "venv_3.8.13"
+venv = "venv_3.8.17"
 # verboseOutput = true
 extraPaths = ["test/generated"]
 include = [
     "mypy_protobuf/",
     "test/"
 ]
 exclude = [
```

### Comparing `mypy-protobuf-3.4.0/setup.cfg` & `mypy-protobuf-3.5.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 [options]
 py_modules = 
 	mypy_protobuf
 	mypy_protobuf.main
 	mypy_protobuf.extensions_pb2
 install_requires = 
-	protobuf>=4.21.8
-	types-protobuf>=3.20.4
-python_requires = >=3.7
+	protobuf>=4.23.4
+	types-protobuf>=4.23.0.2
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	protoc-gen-mypy = mypy_protobuf.main:main
 	protoc-gen-mypy_grpc = mypy_protobuf.main:grpc
 
 [egg_info]
```

### Comparing `mypy-protobuf-3.4.0/test/test_generated_mypy.py` & `mypy-protobuf-3.5.0/test/test_generated_mypy.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,20 +104,20 @@
     def grab_expectations(filename: str, marker: str) -> Generator[Tuple[str, int], None, None]:
         for idx, line in enumerate(open(filename).readlines()):
             if "#" in line and marker in line:
                 yield filename, idx + 1
 
     errors_38 = set(grab_errors("test_negative/output.expected.3.8"))
 
-    expected_errors_38 = set(grab_expectations("test_negative/negative.py", "E:3.8")) | set(grab_expectations("test_negative/negative_3.8.py", "E:3.8"))
+    expected_errors_38 = set(grab_expectations("test_negative/negative.py", "E:3.8"))
 
     assert errors_38 == expected_errors_38
 
     # Some sanity checks to make sure we don't mess this up. Please update as necessary.
-    assert len(errors_38) == 74
+    assert len(errors_38) == 77
 
 
 def test_func() -> None:
     s = Simple1(a_string="hello")
 
     s = Simple1()
     s.a_string = "Hello"
```

### Comparing `mypy-protobuf-3.4.0/test/test_grpc_usage.py` & `mypy-protobuf-3.5.0/test/test_grpc_usage.py`

 * *Files identical despite different names*

