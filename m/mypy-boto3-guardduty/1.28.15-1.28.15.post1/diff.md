# Comparing `tmp/mypy-boto3-guardduty-1.28.15.tar.gz` & `tmp/mypy-boto3-guardduty-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
+gzip compressed data, was "mypy-boto3-guardduty-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:14 2023, max compression
```

## Comparing `mypy-boto3-guardduty-1.28.15.tar` & `mypy-boto3-guardduty-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25967 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.245171 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49732 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-28 20:27:14.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-07-28 20:27:14.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94150 2023-07-28 20:27:16.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94063 2023-07-28 20:27:15.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25967 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50024 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49939 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-29 09:46:46.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94150 2023-07-29 09:46:49.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94063 2023-07-29 09:46:47.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:14.000000 mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:14.265172 mypy-boto3-guardduty-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:46:45.000000 mypy-boto3-guardduty-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-guardduty-1.28.15/LICENSE` & `mypy-boto3-guardduty-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/PKG-INFO` & `mypy-boto3-guardduty-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.15
-Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-guardduty-1.28.15/README.md` & `mypy-boto3-guardduty-1.28.15.post1/README.md`

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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.py` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.pyi` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__main__.py` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.GuardDuty 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.py` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_guardduty.client import GuardDutyClient
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableMembersType,
     CoverageStatisticsTypeType,
     EbsSnapshotPreservationType,
@@ -58,14 +58,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
@@ -89,14 +90,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
@@ -208,15 +210,15 @@
         """
 
     def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: FindingCriteriaTypeDef,
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef],
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -523,15 +525,15 @@
         """
 
     def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_findings_statistics)
         """
@@ -684,15 +686,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_filters)
         """
 
     def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -848,15 +850,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_filter)
         """
@@ -892,15 +894,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_ip_set)
         """
 
     def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
+        ScanResourceCriteria: Union[
+            ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
+        ] = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_malware_scan_settings)
```

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.pyi` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_guardduty.client import GuardDutyClient
 
     session = Session()
     client: GuardDutyClient = session.client("guardduty")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableMembersType,
     CoverageStatisticsTypeType,
     EbsSnapshotPreservationType,
@@ -58,14 +58,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
@@ -89,14 +90,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
@@ -197,15 +199,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#create_detector)
         """
     def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: FindingCriteriaTypeDef,
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef],
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -484,15 +486,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_findings)
         """
     def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#get_findings_statistics)
         """
@@ -631,15 +633,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_filters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#list_filters)
         """
     def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -780,15 +782,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_filter)
         """
@@ -821,15 +823,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_ip_set)
         """
     def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
+        ScanResourceCriteria: Union[
+            ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
+        ] = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/client/#update_malware_scan_settings)
```

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.py` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.pyi` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.py` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,24 @@
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_threat_intel_sets_paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
     ```
 """
-from typing import Generic, Iterator, TypeVar
+from typing import Generic, Iterator, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
@@ -160,15 +161,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.pyi` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,23 +33,24 @@
     list_ip_sets_paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
     list_threat_intel_sets_paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
     ```
 """
-from typing import Generic, Iterator, TypeVar
+from typing import Generic, Iterator, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
@@ -153,15 +154,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef] = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.py` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.pyi` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.15
-Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy-boto3-guardduty-1.28.15.post1/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.15/setup.py` & `mypy-boto3-guardduty-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder"
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

