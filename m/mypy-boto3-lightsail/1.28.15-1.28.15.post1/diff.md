# Comparing `tmp/mypy-boto3-lightsail-1.28.15.tar.gz` & `tmp/mypy-boto3-lightsail-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.28.15.tar", last modified: Fri Jul 28 20:43:10 2023, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
```

## Comparing `mypy-boto3-lightsail-1.28.15.tar` & `mypy-boto3-lightsail-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:10.509409 mypy-boto3-lightsail-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-07-28 20:43:10.505408 mypy-boto3-lightsail-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35193 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:10.505408 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113940 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   113754 2023-07-28 20:30:16.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-07-28 20:30:18.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   147985 2023-07-28 20:30:22.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   147886 2023-07-28 20:30:20.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:10.505408 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:10.509409 mypy-boto3-lightsail-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.685251 mypy-boto3-lightsail-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36694 2023-07-29 10:03:33.681251 mypy-boto3-lightsail-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35193 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.669251 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114230 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114044 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-07-29 09:49:55.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-29 09:49:55.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-29 09:49:54.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   148016 2023-07-29 09:49:59.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147917 2023-07-29 09:49:57.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.681251 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36694 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:33.000000 mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.685251 mypy-boto3-lightsail-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:49:51.000000 mypy-boto3-lightsail-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-lightsail-1.28.15/LICENSE` & `mypy-boto3-lightsail-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/PKG-INFO` & `mypy-boto3-lightsail-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.15
-Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lightsail-1.28.15/README.md` & `mypy-boto3-lightsail-1.28.15.post1/README.md`

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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Lightsail 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,18 @@
     AttachDiskResultTypeDef,
     AttachInstancesToLoadBalancerResultTypeDef,
     AttachLoadBalancerTlsCertificateResultTypeDef,
     AttachStaticIpResultTypeDef,
     BucketAccessLogConfigTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
+    CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsResultTypeDef,
+    ContainerOutputTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     ContainerServicesListResultTypeDef,
     ContainerTypeDef,
     CopySnapshotResultTypeDef,
     CreateBucketAccessKeyResultTypeDef,
     CreateBucketResultTypeDef,
     CreateCertificateResultTypeDef,
@@ -132,14 +134,15 @@
     DeleteRelationalDatabaseSnapshotResultTypeDef,
     DetachCertificateFromDistributionResultTypeDef,
     DetachDiskResultTypeDef,
     DetachInstancesFromLoadBalancerResultTypeDef,
     DetachStaticIpResultTypeDef,
     DisableAddOnResultTypeDef,
     DiskMapTypeDef,
+    DomainEntryOutputTypeDef,
     DomainEntryTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     EnableAddOnResultTypeDef,
     EndpointRequestTypeDef,
     ExportSnapshotResultTypeDef,
     GetActiveNamesResultTypeDef,
     GetAlarmsResultTypeDef,
@@ -473,15 +476,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service)
         """
 
     def create_container_service_deployment(
         self,
         *,
         serviceName: str,
-        containers: Mapping[str, ContainerTypeDef] = ...,
+        containers: Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]] = ...,
         publicEndpoint: EndpointRequestTypeDef = ...
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service_deployment)
@@ -553,15 +556,15 @@
     def create_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
-        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
+        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
@@ -576,15 +579,15 @@
         Creates a domain resource for the specified domain (e.g., example.com).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_domain)
         """
 
     def create_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryTypeDef
+        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
     ) -> CreateDomainEntryResultTypeDef:
         """
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
@@ -868,15 +871,15 @@
         Deletes the specified domain recordset and all of its domain records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain)
         """
 
     def delete_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryTypeDef
+        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
     ) -> DeleteDomainEntryResultTypeDef:
         """
         Deletes a specific domain entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain_entry)
         """
@@ -2035,15 +2038,15 @@
 
     def update_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
-        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
+        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
@@ -2059,15 +2062,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution_bundle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_distribution_bundle)
         """
 
     def update_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryTypeDef
+        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
     ) -> UpdateDomainEntryResultTypeDef:
         """
         Updates a domain recordset after it is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_domain_entry)
         """
```

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,18 @@
     AttachDiskResultTypeDef,
     AttachInstancesToLoadBalancerResultTypeDef,
     AttachLoadBalancerTlsCertificateResultTypeDef,
     AttachStaticIpResultTypeDef,
     BucketAccessLogConfigTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
+    CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsResultTypeDef,
+    ContainerOutputTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     ContainerServicesListResultTypeDef,
     ContainerTypeDef,
     CopySnapshotResultTypeDef,
     CreateBucketAccessKeyResultTypeDef,
     CreateBucketResultTypeDef,
     CreateCertificateResultTypeDef,
@@ -132,14 +134,15 @@
     DeleteRelationalDatabaseSnapshotResultTypeDef,
     DetachCertificateFromDistributionResultTypeDef,
     DetachDiskResultTypeDef,
     DetachInstancesFromLoadBalancerResultTypeDef,
     DetachStaticIpResultTypeDef,
     DisableAddOnResultTypeDef,
     DiskMapTypeDef,
+    DomainEntryOutputTypeDef,
     DomainEntryTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     EnableAddOnResultTypeDef,
     EndpointRequestTypeDef,
     ExportSnapshotResultTypeDef,
     GetActiveNamesResultTypeDef,
     GetAlarmsResultTypeDef,
@@ -452,15 +455,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service)
         """
     def create_container_service_deployment(
         self,
         *,
         serviceName: str,
-        containers: Mapping[str, ContainerTypeDef] = ...,
+        containers: Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]] = ...,
         publicEndpoint: EndpointRequestTypeDef = ...
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_container_service_deployment)
@@ -527,15 +530,15 @@
     def create_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
-        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
+        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
@@ -548,15 +551,15 @@
         """
         Creates a domain resource for the specified domain (e.g., example.com).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_domain)
         """
     def create_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryTypeDef
+        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
     ) -> CreateDomainEntryResultTypeDef:
         """
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
@@ -817,15 +820,15 @@
         """
         Deletes the specified domain recordset and all of its domain records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain)
         """
     def delete_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryTypeDef
+        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
     ) -> DeleteDomainEntryResultTypeDef:
         """
         Deletes a specific domain entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#delete_domain_entry)
         """
@@ -1875,15 +1878,15 @@
         """
     def update_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
-        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
+        cacheBehaviorSettings: Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef] = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
@@ -1897,15 +1900,15 @@
         Updates the bundle of your Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution_bundle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_distribution_bundle)
         """
     def update_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryTypeDef
+        self, *, domainName: str, domainEntry: Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
     ) -> UpdateDomainEntryResultTypeDef:
         """
         Updates a domain recordset after it is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#update_domain_entry)
         """
```

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -5148,15 +5148,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerServiceDeploymentRequestRequestTypeDef",
     {
-        "containers": Mapping[str, ContainerTypeDef],
+        "containers": Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
 
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
```

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -5053,15 +5053,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerServiceDeploymentRequestRequestTypeDef",
     {
-        "containers": Mapping[str, ContainerTypeDef],
+        "containers": Mapping[str, Union[ContainerTypeDef, ContainerOutputTypeDef]],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
     _RequiredCreateContainerServiceDeploymentRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.15
-Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.28.15.post1/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.15/setup.py` & `mypy-boto3-lightsail-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

