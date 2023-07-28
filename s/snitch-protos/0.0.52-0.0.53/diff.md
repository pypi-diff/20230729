# Comparing `tmp/snitch-protos-0.0.52.tar.gz` & `tmp/snitch-protos-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.52.tar", last modified: Thu Jul 27 16:46:07 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.53.tar", last modified: Fri Jul 28 22:08:45 2023, max compression
```

## Comparing `snitch-protos-0.0.52.tar` & `snitch-protos-0.0.53.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 16:45:38.000000 snitch-protos-0.0.52/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-27 16:46:07.000000 snitch-protos-0.0.52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:45:38.000000 snitch-protos-0.0.52/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    32514 2023-07-27 16:45:38.000000 snitch-protos-0.0.52/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-27 16:45:38.000000 snitch-protos-0.0.52/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:07.369872 snitch-protos-0.0.52/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 16:46:07.000000 snitch-protos-0.0.52/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 16:46:07.000000 snitch-protos-0.0.52/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:46:07.000000 snitch-protos-0.0.52/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 16:46:07.000000 snitch-protos-0.0.52/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-28 22:08:44.000000 snitch-protos-0.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.399022 snitch-protos-0.0.53/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    33159 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-28 22:08:12.000000 snitch-protos-0.0.53/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:08:45.403022 snitch-protos-0.0.53/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 22:08:45.000000 snitch-protos-0.0.53/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.52/PKG-INFO` & `snitch-protos-0.0.53/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.52
+Version: 0.0.53
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.52/setup.py` & `snitch-protos-0.0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.52',
+    version='0.0.53',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.52/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.53/snitch_protos/protos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,99 +150,178 @@
     """WASM module bytes (set by snitch-server)"""
 
     wasm_function: str = betterproto.string_field(10002)
     """WASM function name to execute (set by snitch-server)"""
 
 
 @dataclass(eq=False, repr=False)
-class Command(betterproto.Message):
-    """Command is used by snitch-server for sending commands to SDKs"""
+class ServiceInfo(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    description: str = betterproto.string_field(2)
+    pipelines: List["PipelineInfo"] = betterproto.message_field(100)
+    consumers: List["ConsumerInfo"] = betterproto.message_field(101)
+    producers: List["ProducerInfo"] = betterproto.message_field(102)
+    clients: List["ClientInfo"] = betterproto.message_field(103)
 
+
+@dataclass(eq=False, repr=False)
+class PipelineInfo(betterproto.Message):
     audience: "Audience" = betterproto.message_field(1)
-    """Who is this command intended for?"""
+    pipeline: "Pipeline" = betterproto.message_field(2)
 
-    set_pipeline: "SetPipelineCommand" = betterproto.message_field(100, group="command")
-    delete_pipeline: "DeletePipelineCommand" = betterproto.message_field(
-        101, group="command"
-    )
-    pause_pipeline: "PausePipelineCommand" = betterproto.message_field(
-        102, group="command"
-    )
-    unpause_pipeline: "UnpausePipelineCommand" = betterproto.message_field(
-        103, group="command"
+
+@dataclass(eq=False, repr=False)
+class ConsumerInfo(betterproto.Message):
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class ProducerInfo(betterproto.Message):
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class ClientInfo(betterproto.Message):
+    """This should come from the register call"""
+
+    client_type: "ClientType" = betterproto.enum_field(1)
+    library_name: str = betterproto.string_field(2)
+    library_version: str = betterproto.string_field(3)
+    language: str = betterproto.string_field(4)
+    arch: str = betterproto.string_field(5)
+    os: str = betterproto.string_field(6)
+
+
+@dataclass(eq=False, repr=False)
+class GetServiceMapRequest(betterproto.Message):
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class GetServiceMapResponse(betterproto.Message):
+    service_map: Dict[str, "ServiceInfo"] = betterproto.map_field(
+        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    keep_alive: "KeepAliveCommand" = betterproto.message_field(104, group="command")
+    """Key == service name"""
+
+
+@dataclass(eq=False, repr=False)
+class GetPipelinesRequest(betterproto.Message):
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class GetPipelinesResponse(betterproto.Message):
+    pipelines: List["Pipeline"] = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class SetPipelineCommand(betterproto.Message):
-    """Used for both Add and Update"""
+class GetPipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
 
+
+@dataclass(eq=False, repr=False)
+class GetPipelineResponse(betterproto.Message):
     pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class DeletePipelineCommand(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
+class CreatePipelineRequest(betterproto.Message):
+    pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class PausePipelineCommand(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
+class UpdatePipelineRequest(betterproto.Message):
+    pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class UnpausePipelineCommand(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    """Unique ID for the pipeline"""
+class DeletePipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class KeepAliveCommand(betterproto.Message):
-    pass
+class AttachPipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
-class ServiceInfo(betterproto.Message):
-    name: str = betterproto.string_field(1)
-    description: str = betterproto.string_field(2)
-    pipelines: List["PipelineInfo"] = betterproto.message_field(100)
-    consumers: List["ConsumerInfo"] = betterproto.message_field(101)
-    producers: List["ProducerInfo"] = betterproto.message_field(102)
-    clients: List["ClientInfo"] = betterproto.message_field(103)
+class DetachPipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
-class PipelineInfo(betterproto.Message):
+class PausePipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class ResumePipelineRequest(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class TestRequest(betterproto.Message):
+    input: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class TestResponse(betterproto.Message):
+    output: str = betterproto.string_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class Command(betterproto.Message):
+    """Command is used by snitch-server for sending commands to SDKs"""
+
     audience: "Audience" = betterproto.message_field(1)
-    pipeline: "Pipeline" = betterproto.message_field(2)
+    """Who is this command intended for?"""
+
+    attach_pipeline: "AttachPipelineCommand" = betterproto.message_field(
+        100, group="command"
+    )
+    detach_pipeline: "DetachPipelineCommand" = betterproto.message_field(
+        101, group="command"
+    )
+    pause_pipeline: "PausePipelineCommand" = betterproto.message_field(
+        102, group="command"
+    )
+    resume_pipeline: "ResumePipelineCommand" = betterproto.message_field(
+        103, group="command"
+    )
+    keep_alive: "KeepAliveCommand" = betterproto.message_field(104, group="command")
 
 
 @dataclass(eq=False, repr=False)
-class ConsumerInfo(betterproto.Message):
-    pass
+class AttachPipelineCommand(betterproto.Message):
+    pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class ProducerInfo(betterproto.Message):
-    pass
+class DetachPipelineCommand(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class ClientInfo(betterproto.Message):
-    """This should come from the register call"""
+class PausePipelineCommand(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
 
-    client_type: "ClientType" = betterproto.enum_field(1)
-    library_name: str = betterproto.string_field(2)
-    library_version: str = betterproto.string_field(3)
-    language: str = betterproto.string_field(4)
-    arch: str = betterproto.string_field(5)
-    os: str = betterproto.string_field(6)
+
+@dataclass(eq=False, repr=False)
+class ResumePipelineCommand(betterproto.Message):
+    pipeline_id: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class KeepAliveCommand(betterproto.Message):
+    pass
 
 
 @dataclass(eq=False, repr=False)
 class HeartbeatRequest(betterproto.Message):
     """
     Each consumer and producer should send periodic heartbeats to the server to
     let the server know that they are still active.
@@ -301,25 +380,47 @@
     """
 
     service_name: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class BusEvent(betterproto.Message):
-    """Type used by `snitch-server` for sending messages on its local bus."""
+    """
+    Type used by `snitch-server` for broadcasting events to other snitch nodes
+    """
 
     source: str = betterproto.string_field(1)
-    command: "Command" = betterproto.message_field(100, group="event")
-    register_request: "RegisterRequest" = betterproto.message_field(101, group="event")
+    register_request: "RegisterRequest" = betterproto.message_field(100, group="event")
     deregister_request: "DeregisterRequest" = betterproto.message_field(
-        102, group="event"
+        101, group="event"
     )
     heartbeat_request: "HeartbeatRequest" = betterproto.message_field(
+        102, group="event"
+    )
+    create_pipeline_request: "CreatePipelineRequest" = betterproto.message_field(
         103, group="event"
     )
+    delete_pipeline_request: "DeletePipelineRequest" = betterproto.message_field(
+        104, group="event"
+    )
+    update_pipeline_request: "UpdatePipelineRequest" = betterproto.message_field(
+        105, group="event"
+    )
+    attach_pipeline_request: "AttachPipelineRequest" = betterproto.message_field(
+        106, group="event"
+    )
+    detach_pipeline_request: "DetachPipelineRequest" = betterproto.message_field(
+        107, group="event"
+    )
+    pause_pipeline_request: "PausePipelineRequest" = betterproto.message_field(
+        108, group="event"
+    )
+    resume_pipeline_request: "ResumePipelineRequest" = betterproto.message_field(
+        109, group="event"
+    )
     metadata: Dict[str, str] = betterproto.map_field(
         1000, betterproto.TYPE_STRING, betterproto.TYPE_STRING
     )
     """
     All gRPC metadata is stored in ctx; when request goes outside of gRPC
     bounds, we will translate ctx metadata into this field. Example: 1. Request
     comes into snitch-server via external gRPC to set new pipeline 2. snitch-
@@ -328,96 +429,14 @@
     cmd to other services via bus 4. Since this is not a gRPC call, snitch-
     server translates ctx metadata to    this field and includes it in the bus
     event.
     """
 
 
 @dataclass(eq=False, repr=False)
-class GetServiceMapRequest(betterproto.Message):
-    pass
-
-
-@dataclass(eq=False, repr=False)
-class GetServiceMapResponse(betterproto.Message):
-    service_map: Dict[str, "ServiceInfo"] = betterproto.map_field(
-        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
-    )
-    """Key == service name"""
-
-
-@dataclass(eq=False, repr=False)
-class GetPipelinesRequest(betterproto.Message):
-    pass
-
-
-@dataclass(eq=False, repr=False)
-class GetPipelinesResponse(betterproto.Message):
-    pipelines: List["Pipeline"] = betterproto.message_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class GetPipelineRequest(betterproto.Message):
-    pipeline_id: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class GetPipelineResponse(betterproto.Message):
-    pipeline: "Pipeline" = betterproto.message_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class CreatePipelineRequest(betterproto.Message):
-    pipeline: "Pipeline" = betterproto.message_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class UpdatePipelineRequest(betterproto.Message):
-    pipeline: "Pipeline" = betterproto.message_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class DeletePipelineRequest(betterproto.Message):
-    pipeline_id: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class AttachPipelineRequest(betterproto.Message):
-    pipeline_id: str = betterproto.string_field(1)
-    audience: "Audience" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class DetachPipelineRequest(betterproto.Message):
-    pipeline_id: str = betterproto.string_field(1)
-    audience: "Audience" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class PausePipelineRequest(betterproto.Message):
-    pipeline_id: str = betterproto.string_field(1)
-    audience: "Audience" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class ResumePipelineRequest(betterproto.Message):
-    pipeline_id: str = betterproto.string_field(1)
-    audience: "Audience" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class TestRequest(betterproto.Message):
-    input: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class TestResponse(betterproto.Message):
-    output: str = betterproto.string_field(2)
-
-
-@dataclass(eq=False, repr=False)
 class WasmRequest(betterproto.Message):
     """SDK generates a WASM request and passes this to the WASM func"""
 
     step: "PipelineStep" = betterproto.message_field(1)
     input: bytes = betterproto.bytes_field(2)
 
 
@@ -426,85 +445,14 @@
     """Returned by all WASM functions"""
 
     output: bytes = betterproto.bytes_field(1)
     exit_code: "WasmExitCode" = betterproto.enum_field(2)
     exit_msg: str = betterproto.string_field(3)
 
 
-class InternalStub(betterproto.ServiceStub):
-    async def register(
-        self,
-        register_request: "RegisterRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["Command"]:
-        async for response in self._unary_stream(
-            "/protos.Internal/Register",
-            register_request,
-            Command,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    async def heartbeat(
-        self,
-        heartbeat_request: "HeartbeatRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "StandardResponse":
-        return await self._unary_unary(
-            "/protos.Internal/Heartbeat",
-            heartbeat_request,
-            StandardResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    async def notify(
-        self,
-        notify_request: "NotifyRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "StandardResponse":
-        return await self._unary_unary(
-            "/protos.Internal/Notify",
-            notify_request,
-            StandardResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    async def metrics(
-        self,
-        metrics_request: "MetricsRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "StandardResponse":
-        return await self._unary_unary(
-            "/protos.Internal/Metrics",
-            metrics_request,
-            StandardResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-
 class ExternalStub(betterproto.ServiceStub):
     async def get_service_map(
         self,
         get_service_map_request: "GetServiceMapRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
@@ -686,90 +634,83 @@
             TestResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
 
-class InternalBase(ServiceBase):
+class InternalStub(betterproto.ServiceStub):
     async def register(
-        self, register_request: "RegisterRequest"
+        self,
+        register_request: "RegisterRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
     ) -> AsyncIterator["Command"]:
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-        yield Command()
+        async for response in self._unary_stream(
+            "/protos.Internal/Register",
+            register_request,
+            Command,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
 
     async def heartbeat(
-        self, heartbeat_request: "HeartbeatRequest"
+        self,
+        heartbeat_request: "HeartbeatRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
     ) -> "StandardResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
-    async def notify(self, notify_request: "NotifyRequest") -> "StandardResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
-    async def metrics(self, metrics_request: "MetricsRequest") -> "StandardResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-
-    async def __rpc_register(
-        self, stream: "grpclib.server.Stream[RegisterRequest, Command]"
-    ) -> None:
-        request = await stream.recv_message()
-        await self._call_rpc_handler_server_stream(
-            self.register,
-            stream,
-            request,
+        return await self._unary_unary(
+            "/protos.Internal/Heartbeat",
+            heartbeat_request,
+            StandardResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
         )
 
-    async def __rpc_heartbeat(
-        self, stream: "grpclib.server.Stream[HeartbeatRequest, StandardResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.heartbeat(request)
-        await stream.send_message(response)
-
-    async def __rpc_notify(
-        self, stream: "grpclib.server.Stream[NotifyRequest, StandardResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.notify(request)
-        await stream.send_message(response)
-
-    async def __rpc_metrics(
-        self, stream: "grpclib.server.Stream[MetricsRequest, StandardResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.metrics(request)
-        await stream.send_message(response)
+    async def notify(
+        self,
+        notify_request: "NotifyRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "StandardResponse":
+        return await self._unary_unary(
+            "/protos.Internal/Notify",
+            notify_request,
+            StandardResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
-    def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
-        return {
-            "/protos.Internal/Register": grpclib.const.Handler(
-                self.__rpc_register,
-                grpclib.const.Cardinality.UNARY_STREAM,
-                RegisterRequest,
-                Command,
-            ),
-            "/protos.Internal/Heartbeat": grpclib.const.Handler(
-                self.__rpc_heartbeat,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                HeartbeatRequest,
-                StandardResponse,
-            ),
-            "/protos.Internal/Notify": grpclib.const.Handler(
-                self.__rpc_notify,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                NotifyRequest,
-                StandardResponse,
-            ),
-            "/protos.Internal/Metrics": grpclib.const.Handler(
-                self.__rpc_metrics,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                MetricsRequest,
-                StandardResponse,
-            ),
-        }
+    async def metrics(
+        self,
+        metrics_request: "MetricsRequest",
+        *,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "StandardResponse":
+        return await self._unary_unary(
+            "/protos.Internal/Metrics",
+            metrics_request,
+            StandardResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
 
 class ExternalBase(ServiceBase):
     async def get_service_map(
         self, get_service_map_request: "GetServiceMapRequest"
     ) -> "GetServiceMapResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
@@ -965,7 +906,85 @@
             "/protos.External/Test": grpclib.const.Handler(
                 self.__rpc_test,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 TestRequest,
                 TestResponse,
             ),
         }
+
+
+class InternalBase(ServiceBase):
+    async def register(
+        self, register_request: "RegisterRequest"
+    ) -> AsyncIterator["Command"]:
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+        yield Command()
+
+    async def heartbeat(
+        self, heartbeat_request: "HeartbeatRequest"
+    ) -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def notify(self, notify_request: "NotifyRequest") -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def metrics(self, metrics_request: "MetricsRequest") -> "StandardResponse":
+        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+
+    async def __rpc_register(
+        self, stream: "grpclib.server.Stream[RegisterRequest, Command]"
+    ) -> None:
+        request = await stream.recv_message()
+        await self._call_rpc_handler_server_stream(
+            self.register,
+            stream,
+            request,
+        )
+
+    async def __rpc_heartbeat(
+        self, stream: "grpclib.server.Stream[HeartbeatRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.heartbeat(request)
+        await stream.send_message(response)
+
+    async def __rpc_notify(
+        self, stream: "grpclib.server.Stream[NotifyRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.notify(request)
+        await stream.send_message(response)
+
+    async def __rpc_metrics(
+        self, stream: "grpclib.server.Stream[MetricsRequest, StandardResponse]"
+    ) -> None:
+        request = await stream.recv_message()
+        response = await self.metrics(request)
+        await stream.send_message(response)
+
+    def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
+        return {
+            "/protos.Internal/Register": grpclib.const.Handler(
+                self.__rpc_register,
+                grpclib.const.Cardinality.UNARY_STREAM,
+                RegisterRequest,
+                Command,
+            ),
+            "/protos.Internal/Heartbeat": grpclib.const.Handler(
+                self.__rpc_heartbeat,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                HeartbeatRequest,
+                StandardResponse,
+            ),
+            "/protos.Internal/Notify": grpclib.const.Handler(
+                self.__rpc_notify,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                NotifyRequest,
+                StandardResponse,
+            ),
+            "/protos.Internal/Metrics": grpclib.const.Handler(
+                self.__rpc_metrics,
+                grpclib.const.Cardinality.UNARY_UNARY,
+                MetricsRequest,
+                StandardResponse,
+            ),
+        }
```

### Comparing `snitch-protos-0.0.52/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.53/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.52/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.53/snitch_protos.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.52
+Version: 0.0.53
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

