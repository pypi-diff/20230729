# Comparing `tmp/mypy-boto3-kafka-1.28.15.tar.gz` & `tmp/mypy-boto3-kafka-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kafka-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:24 2023, max compression
```

## Comparing `mypy-boto3-kafka-1.28.15.tar` & `mypy-boto3-kafka-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.668180 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36588 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36523 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-28 19:47:13.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60576 2023-07-28 19:47:12.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 19:47:31.000000 mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.672180 mypy-boto3-kafka-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 19:47:11.000000 mypy-boto3-kafka-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:24.877205 mypy-boto3-kafka-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-29 10:03:24.873205 mypy-boto3-kafka-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:24.865205 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36769 2023-07-29 09:48:29.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-29 09:48:31.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-29 09:48:33.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60576 2023-07-29 09:48:32.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:24.873205 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:24.000000 mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:24.877205 mypy-boto3-kafka-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:48:28.000000 mypy-boto3-kafka-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-kafka-1.28.15/LICENSE` & `mypy-boto3-kafka-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/PKG-INFO` & `mypy-boto3-kafka-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.28.15
-Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kafka-1.28.15/README.md` & `mypy-boto3-kafka-1.28.15.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Kafka 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.15.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
+    BrokerNodeGroupInfoOutputTypeDef,
     BrokerNodeGroupInfoTypeDef,
+    ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
@@ -172,19 +174,21 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#close)
         """
 
     def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,
+        BrokerNodeGroupInfo: Union[BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef],
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: ClientAuthenticationTypeDef = ...,
+        ClientAuthentication: Union[
+            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
+        ] = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...
@@ -661,15 +665,17 @@
         """
 
     def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: ClientAuthenticationTypeDef = ...,
+        ClientAuthentication: Union[
+            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
+        ] = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_security)
```

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     ListScramSecretsPaginator,
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BrokerEBSVolumeInfoTypeDef,
+    BrokerNodeGroupInfoOutputTypeDef,
     BrokerNodeGroupInfoTypeDef,
+    ClientAuthenticationOutputTypeDef,
     ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateVpcConnectionResponseTypeDef,
@@ -163,19 +165,21 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#close)
         """
     def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,
+        BrokerNodeGroupInfo: Union[BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoOutputTypeDef],
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: ClientAuthenticationTypeDef = ...,
+        ClientAuthentication: Union[
+            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
+        ] = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...
@@ -608,15 +612,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_monitoring)
         """
     def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: ClientAuthenticationTypeDef = ...,
+        ClientAuthentication: Union[
+            ClientAuthenticationTypeDef, ClientAuthenticationOutputTypeDef
+        ] = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_security)
```

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.28.15
-Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kafka-1.28.15/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.28.15.post1/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kafka-1.28.15/setup.py` & `mypy-boto3-kafka-1.28.15.post1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Kafka 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

