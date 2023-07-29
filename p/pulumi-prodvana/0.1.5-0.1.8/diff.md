# Comparing `tmp/pulumi_prodvana-0.1.5.tar.gz` & `tmp/pulumi_prodvana-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_prodvana-0.1.5.tar", last modified: Fri Jul 28 22:50:50 2023, max compression
+gzip compressed data, was "pulumi_prodvana-0.1.8.tar", last modified: Sat Jul 29 00:20:32 2023, max compression
```

## Comparing `pulumi_prodvana-0.1.5.tar` & `pulumi_prodvana-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:50.737419 pulumi_prodvana-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-28 22:50:50.737419 pulumi_prodvana-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:50.733418 pulumi_prodvana-0.1.5/pulumi_prodvana/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:50.737419 pulumi_prodvana-0.1.5/pulumi_prodvana/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/get_k8s_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/get_release_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/k8s_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    47464 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/managed_k8s_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/release_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana/runtime_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:50.733418 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:50:50.737419 pulumi_prodvana-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-28 22:50:50.000000 pulumi_prodvana-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.886030 pulumi_prodvana-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/pulumi_prodvana/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93070 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/pulumi_prodvana/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/get_k8s_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/get_release_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/k8s_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47464 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/managed_k8s_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82295 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33965 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/release_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana/runtime_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:20:32.882030 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:20:32.886030 pulumi_prodvana-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-29 00:20:32.000000 pulumi_prodvana-0.1.8/setup.py
```

### Comparing `pulumi_prodvana-0.1.5/PKG-INFO` & `pulumi_prodvana-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_prodvana
-Version: 0.1.5
+Version: 0.1.8
 Summary: A Pulumi package for creating and managing Prodvana cloud resources.
 Home-page: https://prodvana.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/prodvana/pulumi-prodvana
 Keywords: pulumi prodvana category/cloud category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -19,21 +19,21 @@
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumi/prodvana
+npm install @prodvana/pulumi-prodvana
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumi/prodvana
+yarn add @prodvana/pulumi-prodvana
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
```

### Comparing `pulumi_prodvana-0.1.5/README.md` & `pulumi_prodvana-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumi/prodvana
+npm install @prodvana/pulumi-prodvana
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumi/prodvana
+yarn add @prodvana/pulumi-prodvana
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
```

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/__init__.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/_inputs.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/get_release_channel.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,348 +4,275 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = [
-    'ManagedK8sRuntimeExecArgs',
-    'ReleaseChannelPolicyArgs',
-    'ReleaseChannelPolicyDefaultEnvArgs',
-    'ReleaseChannelPolicyDefaultEnvSecretArgs',
-    'ReleaseChannelRuntimeArgs',
-    'GetReleaseChannelPolicyArgs',
-    'GetReleaseChannelPolicyDefaultEnvArgs',
-    'GetReleaseChannelPolicyDefaultEnvSecretArgs',
+    'GetReleaseChannelResult',
+    'AwaitableGetReleaseChannelResult',
+    'get_release_channel',
+    'get_release_channel_output',
 ]
 
-@pulumi.input_type
-class ManagedK8sRuntimeExecArgs:
-    def __init__(__self__, *,
-                 api_version: pulumi.Input[str],
-                 command: pulumi.Input[str],
-                 args: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 env: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[str] api_version: API version of the exec credential plugin
-        :param pulumi.Input[str] command: Command to execute
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] args: Arguments to pass when executing the command
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] env: Environment variables to set when executing the command
-        """
-        pulumi.set(__self__, "api_version", api_version)
-        pulumi.set(__self__, "command", command)
-        if args is not None:
-            pulumi.set(__self__, "args", args)
-        if env is not None:
-            pulumi.set(__self__, "env", env)
-
-    @property
-    @pulumi.getter(name="apiVersion")
-    def api_version(self) -> pulumi.Input[str]:
-        """
-        API version of the exec credential plugin
-        """
-        return pulumi.get(self, "api_version")
-
-    @api_version.setter
-    def api_version(self, value: pulumi.Input[str]):
-        pulumi.set(self, "api_version", value)
+@pulumi.output_type
+class GetReleaseChannelResult:
+    """
+    A collection of values returned by getReleaseChannel.
+    """
+    def __init__(__self__, application=None, constants=None, convergence_protections=None, id=None, manual_approval_preconditions=None, name=None, policy=None, protections=None, release_channel_stable_preconditions=None, runtimes=None, service_instance_protections=None, version=None):
+        if application and not isinstance(application, str):
+            raise TypeError("Expected argument 'application' to be a str")
+        pulumi.set(__self__, "application", application)
+        if constants and not isinstance(constants, list):
+            raise TypeError("Expected argument 'constants' to be a list")
+        pulumi.set(__self__, "constants", constants)
+        if convergence_protections and not isinstance(convergence_protections, list):
+            raise TypeError("Expected argument 'convergence_protections' to be a list")
+        pulumi.set(__self__, "convergence_protections", convergence_protections)
+        if id and not isinstance(id, str):
+            raise TypeError("Expected argument 'id' to be a str")
+        pulumi.set(__self__, "id", id)
+        if manual_approval_preconditions and not isinstance(manual_approval_preconditions, list):
+            raise TypeError("Expected argument 'manual_approval_preconditions' to be a list")
+        pulumi.set(__self__, "manual_approval_preconditions", manual_approval_preconditions)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if policy and not isinstance(policy, dict):
+            raise TypeError("Expected argument 'policy' to be a dict")
+        pulumi.set(__self__, "policy", policy)
+        if protections and not isinstance(protections, list):
+            raise TypeError("Expected argument 'protections' to be a list")
+        pulumi.set(__self__, "protections", protections)
+        if release_channel_stable_preconditions and not isinstance(release_channel_stable_preconditions, list):
+            raise TypeError("Expected argument 'release_channel_stable_preconditions' to be a list")
+        pulumi.set(__self__, "release_channel_stable_preconditions", release_channel_stable_preconditions)
+        if runtimes and not isinstance(runtimes, list):
+            raise TypeError("Expected argument 'runtimes' to be a list")
+        pulumi.set(__self__, "runtimes", runtimes)
+        if service_instance_protections and not isinstance(service_instance_protections, list):
+            raise TypeError("Expected argument 'service_instance_protections' to be a list")
+        pulumi.set(__self__, "service_instance_protections", service_instance_protections)
+        if version and not isinstance(version, str):
+            raise TypeError("Expected argument 'version' to be a str")
+        pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
-    def command(self) -> pulumi.Input[str]:
+    def application(self) -> str:
         """
-        Command to execute
+        Name of the Application this Release Channel belongs to
         """
-        return pulumi.get(self, "command")
-
-    @command.setter
-    def command(self, value: pulumi.Input[str]):
-        pulumi.set(self, "command", value)
-
-    @property
-    @pulumi.getter
-    def args(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Arguments to pass when executing the command
-        """
-        return pulumi.get(self, "args")
-
-    @args.setter
-    def args(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "args", value)
+        return pulumi.get(self, "application")
 
     @property
     @pulumi.getter
-    def env(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Environment variables to set when executing the command
+    def constants(self) -> Optional[Sequence['outputs.GetReleaseChannelConstantResult']]:
         """
-        return pulumi.get(self, "env")
-
-    @env.setter
-    def env(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "env", value)
-
-
-@pulumi.input_type
-class ReleaseChannelPolicyArgs:
-    def __init__(__self__, *,
-                 default_env: Optional[pulumi.Input[Mapping[str, pulumi.Input['ReleaseChannelPolicyDefaultEnvArgs']]]] = None):
-        """
-        :param pulumi.Input[Mapping[str, pulumi.Input['ReleaseChannelPolicyDefaultEnvArgs']]] default_env: default environment variables for services in this Release Channel
+        Constant values for this release channel
         """
-        if default_env is not None:
-            pulumi.set(__self__, "default_env", default_env)
+        return pulumi.get(self, "constants")
 
     @property
-    @pulumi.getter(name="defaultEnv")
-    def default_env(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['ReleaseChannelPolicyDefaultEnvArgs']]]]:
+    @pulumi.getter(name="convergenceProtections")
+    def convergence_protections(self) -> Optional[Sequence['outputs.GetReleaseChannelConvergenceProtectionResult']]:
         """
-        default environment variables for services in this Release Channel
+        Feature Coming Soon
         """
-        return pulumi.get(self, "default_env")
-
-    @default_env.setter
-    def default_env(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['ReleaseChannelPolicyDefaultEnvArgs']]]]):
-        pulumi.set(self, "default_env", value)
-
-
-@pulumi.input_type
-class ReleaseChannelPolicyDefaultEnvArgs:
-    def __init__(__self__, *,
-                 secret: Optional[pulumi.Input['ReleaseChannelPolicyDefaultEnvSecretArgs']] = None,
-                 value: Optional[pulumi.Input[str]] = None):
-        if secret is not None:
-            pulumi.set(__self__, "secret", secret)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
+        return pulumi.get(self, "convergence_protections")
 
     @property
     @pulumi.getter
-    def secret(self) -> Optional[pulumi.Input['ReleaseChannelPolicyDefaultEnvSecretArgs']]:
-        return pulumi.get(self, "secret")
-
-    @secret.setter
-    def secret(self, value: Optional[pulumi.Input['ReleaseChannelPolicyDefaultEnvSecretArgs']]):
-        pulumi.set(self, "secret", value)
-
-    @property
-    @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "value", value)
-
-
-@pulumi.input_type
-class ReleaseChannelPolicyDefaultEnvSecretArgs:
-    def __init__(__self__, *,
-                 key: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] version: Current application version
-        """
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
-
-    @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
-        """
-        Current application version
-        """
-        return pulumi.get(self, "version")
-
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
-
-
-@pulumi.input_type
-class ReleaseChannelRuntimeArgs:
-    def __init__(__self__, *,
-                 ecs_prefix: Optional[pulumi.Input[str]] = None,
-                 k8s_namespace: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 runtime: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] ecs_prefix: Prefix used when naming ECS resources. Can only be set on an ECS Runtime.
-        :param pulumi.Input[str] k8s_namespace: Optionally set a custom namespace. If not set, Prodvana will create and manage the namespace. If set, the namespace *must* already exist and Prodvana will not try to create or delete it. Can only be set on a Kubernetes Runtime.
-        :param pulumi.Input[str] name: optional identifier for this runtime connection within this release channel
-        :param pulumi.Input[str] runtime: name of the a runtime
-        :param pulumi.Input[str] type: type of the runtime connection, one of (EXTENSION, LONG*LIVED*COMPUTE, UNKNOWN_CONNECTION)
+    def id(self) -> str:
         """
-        if ecs_prefix is not None:
-            pulumi.set(__self__, "ecs_prefix", ecs_prefix)
-        if k8s_namespace is not None:
-            pulumi.set(__self__, "k8s_namespace", k8s_namespace)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if runtime is not None:
-            pulumi.set(__self__, "runtime", runtime)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="ecsPrefix")
-    def ecs_prefix(self) -> Optional[pulumi.Input[str]]:
+        Release channel identifier
         """
-        Prefix used when naming ECS resources. Can only be set on an ECS Runtime.
-        """
-        return pulumi.get(self, "ecs_prefix")
-
-    @ecs_prefix.setter
-    def ecs_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ecs_prefix", value)
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="k8sNamespace")
-    def k8s_namespace(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="manualApprovalPreconditions")
+    def manual_approval_preconditions(self) -> Optional[Sequence['outputs.GetReleaseChannelManualApprovalPreconditionResult']]:
         """
-        Optionally set a custom namespace. If not set, Prodvana will create and manage the namespace. If set, the namespace *must* already exist and Prodvana will not try to create or delete it. Can only be set on a Kubernetes Runtime.
+        Preconditions requiring manual approval before this release channel can be deployed
         """
-        return pulumi.get(self, "k8s_namespace")
-
-    @k8s_namespace.setter
-    def k8s_namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "k8s_namespace", value)
+        return pulumi.get(self, "manual_approval_preconditions")
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> str:
         """
-        optional identifier for this runtime connection within this release channel
+        Release Channel name
         """
         return pulumi.get(self, "name")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
     @property
     @pulumi.getter
-    def runtime(self) -> Optional[pulumi.Input[str]]:
+    def policy(self) -> 'outputs.GetReleaseChannelPolicyResult':
         """
-        name of the a runtime
+        Release Channel policy applied to all services
         """
-        return pulumi.get(self, "runtime")
-
-    @runtime.setter
-    def runtime(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "runtime", value)
+        return pulumi.get(self, "policy")
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        type of the runtime connection, one of (EXTENSION, LONG*LIVED*COMPUTE, UNKNOWN_CONNECTION)
-        """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
-
-@pulumi.input_type
-class GetReleaseChannelPolicyArgs:
-    def __init__(__self__, *,
-                 default_env: Mapping[str, 'GetReleaseChannelPolicyDefaultEnvArgs']):
+    def protections(self) -> Optional[Sequence['outputs.GetReleaseChannelProtectionResult']]:
         """
-        :param Mapping[str, 'GetReleaseChannelPolicyDefaultEnvArgs'] default_env: default environment variables for services in this Release Channel
+        Protections applied this release channel
         """
-        pulumi.set(__self__, "default_env", default_env)
+        return pulumi.get(self, "protections")
 
     @property
-    @pulumi.getter(name="defaultEnv")
-    def default_env(self) -> Mapping[str, 'GetReleaseChannelPolicyDefaultEnvArgs']:
+    @pulumi.getter(name="releaseChannelStablePreconditions")
+    def release_channel_stable_preconditions(self) -> Optional[Sequence['outputs.GetReleaseChannelReleaseChannelStablePreconditionResult']]:
         """
-        default environment variables for services in this Release Channel
+        Preconditions requiring other release channels to be stable before this release channel can be deployed
         """
-        return pulumi.get(self, "default_env")
-
-    @default_env.setter
-    def default_env(self, value: Mapping[str, 'GetReleaseChannelPolicyDefaultEnvArgs']):
-        pulumi.set(self, "default_env", value)
-
-
-@pulumi.input_type
-class GetReleaseChannelPolicyDefaultEnvArgs:
-    def __init__(__self__, *,
-                 secret: Optional['GetReleaseChannelPolicyDefaultEnvSecretArgs'] = None,
-                 value: Optional[str] = None):
-        if secret is not None:
-            pulumi.set(__self__, "secret", secret)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
-
-    @property
-    @pulumi.getter
-    def secret(self) -> Optional['GetReleaseChannelPolicyDefaultEnvSecretArgs']:
-        return pulumi.get(self, "secret")
-
-    @secret.setter
-    def secret(self, value: Optional['GetReleaseChannelPolicyDefaultEnvSecretArgs']):
-        pulumi.set(self, "secret", value)
+        return pulumi.get(self, "release_channel_stable_preconditions")
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[str]:
-        return pulumi.get(self, "value")
-
-    @value.setter
-    def value(self, value: Optional[str]):
-        pulumi.set(self, "value", value)
-
-
-@pulumi.input_type
-class GetReleaseChannelPolicyDefaultEnvSecretArgs:
-    def __init__(__self__, *,
-                 key: Optional[str] = None,
-                 version: Optional[str] = None):
-        """
-        :param str version: Current application version
-        """
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
+    def runtimes(self) -> Sequence['outputs.GetReleaseChannelRuntimeResult']:
+        """
+        Release Channel policy applied to all services
+        """
+        return pulumi.get(self, "runtimes")
 
     @property
-    @pulumi.getter
-    def key(self) -> Optional[str]:
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: Optional[str]):
-        pulumi.set(self, "key", value)
+    @pulumi.getter(name="serviceInstanceProtections")
+    def service_instance_protections(self) -> Optional[Sequence['outputs.GetReleaseChannelServiceInstanceProtectionResult']]:
+        """
+        Protections applied to service instances in this release channel
+        """
+        return pulumi.get(self, "service_instance_protections")
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[str]:
+    def version(self) -> str:
         """
         Current application version
         """
         return pulumi.get(self, "version")
 
-    @version.setter
-    def version(self, value: Optional[str]):
-        pulumi.set(self, "version", value)
-
 
+class AwaitableGetReleaseChannelResult(GetReleaseChannelResult):
+    # pylint: disable=using-constant-test
+    def __await__(self):
+        if False:
+            yield self
+        return GetReleaseChannelResult(
+            application=self.application,
+            constants=self.constants,
+            convergence_protections=self.convergence_protections,
+            id=self.id,
+            manual_approval_preconditions=self.manual_approval_preconditions,
+            name=self.name,
+            policy=self.policy,
+            protections=self.protections,
+            release_channel_stable_preconditions=self.release_channel_stable_preconditions,
+            runtimes=self.runtimes,
+            service_instance_protections=self.service_instance_protections,
+            version=self.version)
+
+
+def get_release_channel(application: Optional[str] = None,
+                        constants: Optional[Sequence[pulumi.InputType['GetReleaseChannelConstantArgs']]] = None,
+                        convergence_protections: Optional[Sequence[pulumi.InputType['GetReleaseChannelConvergenceProtectionArgs']]] = None,
+                        manual_approval_preconditions: Optional[Sequence[pulumi.InputType['GetReleaseChannelManualApprovalPreconditionArgs']]] = None,
+                        name: Optional[str] = None,
+                        policy: Optional[pulumi.InputType['GetReleaseChannelPolicyArgs']] = None,
+                        protections: Optional[Sequence[pulumi.InputType['GetReleaseChannelProtectionArgs']]] = None,
+                        release_channel_stable_preconditions: Optional[Sequence[pulumi.InputType['GetReleaseChannelReleaseChannelStablePreconditionArgs']]] = None,
+                        service_instance_protections: Optional[Sequence[pulumi.InputType['GetReleaseChannelServiceInstanceProtectionArgs']]] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetReleaseChannelResult:
+    """
+    Prodvana Release Channel
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_prodvana as prodvana
+
+    example = prodvana.get_release_channel(application="my-app",
+        name="my-rc")
+    ```
+
+
+    :param str application: Name of the Application this Release Channel belongs to
+    :param Sequence[pulumi.InputType['GetReleaseChannelConstantArgs']] constants: Constant values for this release channel
+    :param Sequence[pulumi.InputType['GetReleaseChannelConvergenceProtectionArgs']] convergence_protections: Feature Coming Soon
+    :param Sequence[pulumi.InputType['GetReleaseChannelManualApprovalPreconditionArgs']] manual_approval_preconditions: Preconditions requiring manual approval before this release channel can be deployed
+    :param str name: Release Channel name
+    :param pulumi.InputType['GetReleaseChannelPolicyArgs'] policy: Release Channel policy applied to all services
+    :param Sequence[pulumi.InputType['GetReleaseChannelProtectionArgs']] protections: Protections applied this release channel
+    :param Sequence[pulumi.InputType['GetReleaseChannelReleaseChannelStablePreconditionArgs']] release_channel_stable_preconditions: Preconditions requiring other release channels to be stable before this release channel can be deployed
+    :param Sequence[pulumi.InputType['GetReleaseChannelServiceInstanceProtectionArgs']] service_instance_protections: Protections applied to service instances in this release channel
+    """
+    __args__ = dict()
+    __args__['application'] = application
+    __args__['constants'] = constants
+    __args__['convergenceProtections'] = convergence_protections
+    __args__['manualApprovalPreconditions'] = manual_approval_preconditions
+    __args__['name'] = name
+    __args__['policy'] = policy
+    __args__['protections'] = protections
+    __args__['releaseChannelStablePreconditions'] = release_channel_stable_preconditions
+    __args__['serviceInstanceProtections'] = service_instance_protections
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
+    __ret__ = pulumi.runtime.invoke('prodvana:index/getReleaseChannel:getReleaseChannel', __args__, opts=opts, typ=GetReleaseChannelResult).value
+
+    return AwaitableGetReleaseChannelResult(
+        application=pulumi.get(__ret__, 'application'),
+        constants=pulumi.get(__ret__, 'constants'),
+        convergence_protections=pulumi.get(__ret__, 'convergence_protections'),
+        id=pulumi.get(__ret__, 'id'),
+        manual_approval_preconditions=pulumi.get(__ret__, 'manual_approval_preconditions'),
+        name=pulumi.get(__ret__, 'name'),
+        policy=pulumi.get(__ret__, 'policy'),
+        protections=pulumi.get(__ret__, 'protections'),
+        release_channel_stable_preconditions=pulumi.get(__ret__, 'release_channel_stable_preconditions'),
+        runtimes=pulumi.get(__ret__, 'runtimes'),
+        service_instance_protections=pulumi.get(__ret__, 'service_instance_protections'),
+        version=pulumi.get(__ret__, 'version'))
+
+
+@_utilities.lift_output_func(get_release_channel)
+def get_release_channel_output(application: Optional[pulumi.Input[str]] = None,
+                               constants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetReleaseChannelConstantArgs']]]]] = None,
+                               convergence_protections: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetReleaseChannelConvergenceProtectionArgs']]]]] = None,
+                               manual_approval_preconditions: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetReleaseChannelManualApprovalPreconditionArgs']]]]] = None,
+                               name: Optional[pulumi.Input[str]] = None,
+                               policy: Optional[pulumi.Input[Optional[pulumi.InputType['GetReleaseChannelPolicyArgs']]]] = None,
+                               protections: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetReleaseChannelProtectionArgs']]]]] = None,
+                               release_channel_stable_preconditions: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetReleaseChannelReleaseChannelStablePreconditionArgs']]]]] = None,
+                               service_instance_protections: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetReleaseChannelServiceInstanceProtectionArgs']]]]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetReleaseChannelResult]:
+    """
+    Prodvana Release Channel
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_prodvana as prodvana
+
+    example = prodvana.get_release_channel(application="my-app",
+        name="my-rc")
+    ```
+
+
+    :param str application: Name of the Application this Release Channel belongs to
+    :param Sequence[pulumi.InputType['GetReleaseChannelConstantArgs']] constants: Constant values for this release channel
+    :param Sequence[pulumi.InputType['GetReleaseChannelConvergenceProtectionArgs']] convergence_protections: Feature Coming Soon
+    :param Sequence[pulumi.InputType['GetReleaseChannelManualApprovalPreconditionArgs']] manual_approval_preconditions: Preconditions requiring manual approval before this release channel can be deployed
+    :param str name: Release Channel name
+    :param pulumi.InputType['GetReleaseChannelPolicyArgs'] policy: Release Channel policy applied to all services
+    :param Sequence[pulumi.InputType['GetReleaseChannelProtectionArgs']] protections: Protections applied this release channel
+    :param Sequence[pulumi.InputType['GetReleaseChannelReleaseChannelStablePreconditionArgs']] release_channel_stable_preconditions: Preconditions requiring other release channels to be stable before this release channel can be deployed
+    :param Sequence[pulumi.InputType['GetReleaseChannelServiceInstanceProtectionArgs']] service_instance_protections: Protections applied to service instances in this release channel
+    """
+    ...
```

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/_utilities.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return None
+	return "https://github.com/prodvana/pulumi-prodvana/releases"
```

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/application.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/config/vars.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/get_application.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/get_k8s_runtime.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/get_k8s_runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/k8s_runtime.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/k8s_runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/managed_k8s_runtime.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/managed_k8s_runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/provider.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana/runtime_link.py` & `pulumi_prodvana-0.1.8/pulumi_prodvana/runtime_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/PKG-INFO` & `pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-prodvana
-Version: 0.1.5
+Version: 0.1.8
 Summary: A Pulumi package for creating and managing Prodvana cloud resources.
 Home-page: https://prodvana.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/prodvana/pulumi-prodvana
 Keywords: pulumi prodvana category/cloud category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -19,21 +19,21 @@
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumi/prodvana
+npm install @prodvana/pulumi-prodvana
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumi/prodvana
+yarn add @prodvana/pulumi-prodvana
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
```

### Comparing `pulumi_prodvana-0.1.5/pulumi_prodvana.egg-info/SOURCES.txt` & `pulumi_prodvana-0.1.8/pulumi_prodvana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_prodvana-0.1.5/setup.py` & `pulumi_prodvana-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.5"
-PLUGIN_VERSION = "0.1.5"
+VERSION = "0.1.8"
+PLUGIN_VERSION = "0.1.8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'prodvana', PLUGIN_VERSION])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'prodvana', PLUGIN_VERSION, '--server', 'https://github.com/prodvana/pulumi-prodvana/releases'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the prodvana resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

