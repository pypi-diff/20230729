# Comparing `tmp/mypy-boto3-macie2-1.28.12.tar.gz` & `tmp/mypy-boto3-macie2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-macie2-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
+gzip compressed data, was "mypy-boto3-macie2-1.28.15.tar", last modified: Fri Jul 28 20:43:12 2023, max compression
```

## Comparing `mypy-boto3-macie2-1.28.12.tar` & `mypy-boto3-macie2-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.576450 mypy-boto3-macie2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-27 05:34:58.572450 mypy-boto3-macie2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.564450 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59831 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59728 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19545 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    96345 2023-07-27 05:25:50.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    96286 2023-07-27 05:25:47.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-27 05:25:46.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.572450 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:58.000000 mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.576450 mypy-boto3-macie2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:25:45.000000 mypy-boto3-macie2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.081430 mypy-boto3-macie2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29253 2023-07-28 20:43:12.081430 mypy-boto3-macie2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27770 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.069430 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59831 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59728 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-07-28 20:30:47.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-28 20:30:47.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19513 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93322 2023-07-28 20:30:51.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93267 2023-07-28 20:30:50.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-28 20:30:46.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:12.081430 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29253 2023-07-28 20:43:11.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:11.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:11.000000 mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:12.081430 mypy-boto3-macie2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:30:45.000000 mypy-boto3-macie2-1.28.15/setup.py
```

### Comparing `mypy-boto3-macie2-1.28.12/LICENSE` & `mypy-boto3-macie2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/PKG-INFO` & `mypy-boto3-macie2-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.28.12
-Summary: Type annotations for boto3.Macie2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Macie2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -467,23 +467,23 @@
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
     AdminAccountTypeDef,
-    S3WordsListOutputTypeDef,
     S3WordsListTypeDef,
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
     BatchGetCustomDataIdentifiersRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BucketCountByEffectivePermissionTypeDef,
     BucketCountByEncryptionTypeTypeDef,
     BucketCountBySharedAccessTypeTypeDef,
     BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef,
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketPolicyTypeDef,
     BucketServerSideEncryptionTypeDef,
@@ -491,197 +491,188 @@
     KeyValuePairTypeDef,
     ObjectCountByEncryptionTypeTypeDef,
     ObjectLevelStatisticsTypeDef,
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
-    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
-    CreateAllowListResponseTypeDef,
-    CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
-    CreateCustomDataIdentifierResponseTypeDef,
-    CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
-    CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
     CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMemberRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClassificationJobRequestRequestTypeDef,
     LastRunErrorStatusTypeDef,
     StatisticsTypeDef,
     UserPausedDetailsTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DetectedDataDetailsTypeDef,
     DetectionTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DomainDetailsTypeDef,
     EnableMacieRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     SeverityTypeDef,
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
-    GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
-    SeverityLevelOutputTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
-    SecurityHubConfigurationOutputTypeDef,
+    SecurityHubConfigurationTypeDef,
     SortCriteriaTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
-    GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
-    RevealConfigurationOutputTypeDef,
+    RevealConfigurationTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
-    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
     SensitivityInspectionTemplateExcludesOutputTypeDef,
     SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
-    MonthlyScheduleOutputTypeDef,
-    WeeklyScheduleOutputTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
     SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
     S3BucketDefinitionForJobOutputTypeDef,
-    ListAllowListsRequestListAllowListsPaginateTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
-    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
-    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
-    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
     ListFindingsFiltersRequestRequestTypeDef,
-    ListFindingsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListJobsFilterTermTypeDef,
-    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
     ListManagedDataIdentifiersRequestRequestTypeDef,
     ManagedDataIdentifierSummaryTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
     ListResourceProfileArtifactsRequestRequestTypeDef,
     ResourceProfileArtifactTypeDef,
-    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
     ListResourceProfileDetectionsRequestRequestTypeDef,
-    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
-    SecurityHubConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    RevealConfigurationTypeDef,
     S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
     SensitivityInspectionTemplateExcludesTypeDef,
     SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
-    TagCriterionPairForJobOutputTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagValuePairOutputTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
-    TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
-    UpdateFindingsFilterResponseTypeDef,
     UpdateMacieSessionRequestRequestTypeDef,
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    AllowListCriteriaOutputTypeDef,
     AllowListCriteriaTypeDef,
-    ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
+    CreateAllowListResponseTypeDef,
+    CreateClassificationJobResponseTypeDef,
+    CreateCustomDataIdentifierResponseTypeDef,
+    CreateFindingsFilterResponseTypeDef,
+    CreateMemberResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    GetAutomatedDiscoveryConfigurationResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetMacieSessionResponseTypeDef,
+    GetMemberResponseTypeDef,
+    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
+    ListAllowListsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TestCustomDataIdentifierResponseTypeDef,
+    UpdateAllowListResponseTypeDef,
+    UpdateFindingsFilterResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
-    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
-    ClassificationExportConfigurationOutputTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
+    GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
+    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
+    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
+    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
+    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
-    GetCustomDataIdentifierResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
     GetFindingsPublicationConfigurationResponseTypeDef,
+    PutFindingsPublicationConfigurationRequestRequestTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
+    UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
@@ -689,37 +680,35 @@
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
-    PutFindingsPublicationConfigurationRequestRequestTypeDef,
-    UpdateRevealConfigurationRequestRequestTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
     UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
     TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
     TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
-    GetAllowListResponseTypeDef,
     CreateAllowListRequestRequestTypeDef,
+    GetAllowListResponseTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
-    PutClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
+    PutClassificationExportConfigurationResponseTypeDef,
     GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.12/README.md` & `mypy-boto3-macie2-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -435,23 +435,23 @@
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
     AdminAccountTypeDef,
-    S3WordsListOutputTypeDef,
     S3WordsListTypeDef,
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
     BatchGetCustomDataIdentifiersRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BucketCountByEffectivePermissionTypeDef,
     BucketCountByEncryptionTypeTypeDef,
     BucketCountBySharedAccessTypeTypeDef,
     BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef,
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketPolicyTypeDef,
     BucketServerSideEncryptionTypeDef,
@@ -459,197 +459,188 @@
     KeyValuePairTypeDef,
     ObjectCountByEncryptionTypeTypeDef,
     ObjectLevelStatisticsTypeDef,
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
-    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
-    CreateAllowListResponseTypeDef,
-    CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
-    CreateCustomDataIdentifierResponseTypeDef,
-    CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
-    CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
     CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMemberRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClassificationJobRequestRequestTypeDef,
     LastRunErrorStatusTypeDef,
     StatisticsTypeDef,
     UserPausedDetailsTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DetectedDataDetailsTypeDef,
     DetectionTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DomainDetailsTypeDef,
     EnableMacieRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     SeverityTypeDef,
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
-    GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
-    SeverityLevelOutputTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
-    SecurityHubConfigurationOutputTypeDef,
+    SecurityHubConfigurationTypeDef,
     SortCriteriaTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
-    GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
-    RevealConfigurationOutputTypeDef,
+    RevealConfigurationTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
-    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
     SensitivityInspectionTemplateExcludesOutputTypeDef,
     SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
-    MonthlyScheduleOutputTypeDef,
-    WeeklyScheduleOutputTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
     SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
     S3BucketDefinitionForJobOutputTypeDef,
-    ListAllowListsRequestListAllowListsPaginateTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
-    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
-    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
-    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
     ListFindingsFiltersRequestRequestTypeDef,
-    ListFindingsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListJobsFilterTermTypeDef,
-    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
     ListManagedDataIdentifiersRequestRequestTypeDef,
     ManagedDataIdentifierSummaryTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
     ListResourceProfileArtifactsRequestRequestTypeDef,
     ResourceProfileArtifactTypeDef,
-    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
     ListResourceProfileDetectionsRequestRequestTypeDef,
-    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
-    SecurityHubConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    RevealConfigurationTypeDef,
     S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
     SensitivityInspectionTemplateExcludesTypeDef,
     SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
-    TagCriterionPairForJobOutputTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagValuePairOutputTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
-    TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
-    UpdateFindingsFilterResponseTypeDef,
     UpdateMacieSessionRequestRequestTypeDef,
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    AllowListCriteriaOutputTypeDef,
     AllowListCriteriaTypeDef,
-    ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
+    CreateAllowListResponseTypeDef,
+    CreateClassificationJobResponseTypeDef,
+    CreateCustomDataIdentifierResponseTypeDef,
+    CreateFindingsFilterResponseTypeDef,
+    CreateMemberResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    GetAutomatedDiscoveryConfigurationResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetMacieSessionResponseTypeDef,
+    GetMemberResponseTypeDef,
+    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
+    ListAllowListsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TestCustomDataIdentifierResponseTypeDef,
+    UpdateAllowListResponseTypeDef,
+    UpdateFindingsFilterResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
-    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
-    ClassificationExportConfigurationOutputTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
+    GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
+    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
+    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
+    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
+    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
-    GetCustomDataIdentifierResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
     GetFindingsPublicationConfigurationResponseTypeDef,
+    PutFindingsPublicationConfigurationRequestRequestTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
+    UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
@@ -657,37 +648,35 @@
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
-    PutFindingsPublicationConfigurationRequestRequestTypeDef,
-    UpdateRevealConfigurationRequestRequestTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
     UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
     TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
     TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
-    GetAllowListResponseTypeDef,
     CreateAllowListRequestRequestTypeDef,
+    GetAllowListResponseTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
-    PutClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
+    PutClassificationExportConfigurationResponseTypeDef,
     GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__init__.pyi` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/__main__.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Macie2 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Macie2 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/client.pyi` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/literals.pyi` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     """
 
     def paginate(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         sortCriteria: BucketSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBucketsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#describebucketspaginator)
         """
 
 
@@ -141,30 +141,30 @@
 
     def paginate(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
         timeRange: TimeRangeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetUsageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#getusagestatisticspaginator)
         """
 
 
 class ListAllowListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listallowlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAllowListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listallowlistspaginator)
         """
 
 
@@ -175,45 +175,45 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         sortCriteria: ListJobsSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listclassificationjobspaginator)
         """
 
 
 class ListClassificationScopesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listclassificationscopespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClassificationScopesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listclassificationscopespaginator)
         """
 
 
 class ListCustomDataIdentifiersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listcustomdataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listcustomdataidentifierspaginator)
         """
 
 
@@ -224,135 +224,135 @@
     """
 
     def paginate(
         self,
         *,
         findingCriteria: FindingCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingspaginator)
         """
 
 
 class ListFindingsFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingsfilterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingsfilterspaginator)
         """
 
 
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listinvitationspaginator)
         """
 
 
 class ListManagedDataIdentifiersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmanageddataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmanageddataidentifierspaginator)
         """
 
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmemberspaginator)
         """
 
 
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listorganizationadminaccountspaginator)
         """
 
 
 class ListResourceProfileArtifactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofileartifactspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceProfileArtifactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofileartifactspaginator)
         """
 
 
 class ListResourceProfileDetectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofiledetectionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceProfileDetectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofiledetectionspaginator)
         """
 
 
 class ListSensitivityInspectionTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSensitivityInspectionTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
         """
 
 
@@ -363,13 +363,13 @@
     """
 
     def paginate(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/paginator.pyi` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         sortCriteria: BucketSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBucketsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#describebucketspaginator)
         """
 
 class GetUsageStatisticsPaginator(Paginator):
@@ -137,29 +137,29 @@
 
     def paginate(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
         timeRange: TimeRangeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetUsageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#getusagestatisticspaginator)
         """
 
 class ListAllowListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listallowlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAllowListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listallowlistspaginator)
         """
 
 class ListClassificationJobsPaginator(Paginator):
@@ -169,43 +169,43 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         sortCriteria: ListJobsSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listclassificationjobspaginator)
         """
 
 class ListClassificationScopesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listclassificationscopespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClassificationScopesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listclassificationscopespaginator)
         """
 
 class ListCustomDataIdentifiersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listcustomdataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listcustomdataidentifierspaginator)
         """
 
 class ListFindingsPaginator(Paginator):
@@ -215,127 +215,127 @@
     """
 
     def paginate(
         self,
         *,
         findingCriteria: FindingCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingspaginator)
         """
 
 class ListFindingsFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingsfilterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listfindingsfilterspaginator)
         """
 
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listinvitationspaginator)
         """
 
 class ListManagedDataIdentifiersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmanageddataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmanageddataidentifierspaginator)
         """
 
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listorganizationadminaccountspaginator)
         """
 
 class ListResourceProfileArtifactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofileartifactspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceProfileArtifactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofileartifactspaginator)
         """
 
 class ListResourceProfileDetectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofiledetectionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceProfileDetectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listresourceprofiledetectionspaginator)
         """
 
 class ListSensitivityInspectionTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSensitivityInspectionTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
         """
 
 class SearchResourcesPaginator(Paginator):
@@ -345,13 +345,13 @@
     """
 
     def paginate(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,23 +80,23 @@
 
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccountDetailTypeDef",
     "BlockPublicAccessTypeDef",
     "AdminAccountTypeDef",
-    "S3WordsListOutputTypeDef",
     "S3WordsListTypeDef",
     "AllowListStatusTypeDef",
     "AllowListSummaryTypeDef",
     "ApiCallDetailsTypeDef",
     "AwsAccountTypeDef",
     "AwsServiceTypeDef",
     "BatchGetCustomDataIdentifierSummaryTypeDef",
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BucketCountByEffectivePermissionTypeDef",
     "BucketCountByEncryptionTypeTypeDef",
     "BucketCountBySharedAccessTypeTypeDef",
     "BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef",
     "BucketCriteriaAdditionalPropertiesTypeDef",
     "BucketPolicyTypeDef",
     "BucketServerSideEncryptionTypeDef",
@@ -104,197 +104,188 @@
     "KeyValuePairTypeDef",
     "ObjectCountByEncryptionTypeTypeDef",
     "ObjectLevelStatisticsTypeDef",
     "ReplicationDetailsTypeDef",
     "BucketSortCriteriaTypeDef",
     "SensitivityAggregationsTypeDef",
     "CellTypeDef",
-    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
-    "CreateAllowListResponseTypeDef",
-    "CreateClassificationJobResponseTypeDef",
     "SeverityLevelTypeDef",
-    "CreateCustomDataIdentifierResponseTypeDef",
-    "CreateFindingsFilterResponseTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
-    "CreateMemberResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
     "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMemberRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClassificationJobRequestRequestTypeDef",
     "LastRunErrorStatusTypeDef",
     "StatisticsTypeDef",
     "UserPausedDetailsTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
     "DetectedDataDetailsTypeDef",
     "DetectionTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "EnableMacieRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "FindingStatisticsSortCriteriaTypeDef",
     "SeverityTypeDef",
     "FindingsFilterListItemTypeDef",
     "InvitationTypeDef",
     "GetAllowListRequestRequestTypeDef",
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
     "GetBucketStatisticsRequestRequestTypeDef",
     "GetClassificationScopeRequestRequestTypeDef",
     "GetCustomDataIdentifierRequestRequestTypeDef",
-    "SeverityLevelOutputTypeDef",
     "GroupCountTypeDef",
     "GetFindingsFilterRequestRequestTypeDef",
-    "SecurityHubConfigurationOutputTypeDef",
+    "SecurityHubConfigurationTypeDef",
     "SortCriteriaTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "GetMacieSessionResponseTypeDef",
     "GetMemberRequestRequestTypeDef",
-    "GetMemberResponseTypeDef",
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
-    "RevealConfigurationOutputTypeDef",
+    "RevealConfigurationTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     "SensitivityInspectionTemplateExcludesOutputTypeDef",
     "SensitivityInspectionTemplateIncludesOutputTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
-    "MonthlyScheduleOutputTypeDef",
-    "WeeklyScheduleOutputTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
     "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
     "S3BucketDefinitionForJobOutputTypeDef",
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
     "ListFindingsFiltersRequestRequestTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListJobsFilterTermTypeDef",
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     "ManagedDataIdentifierSummaryTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "MemberTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
     "ListResourceProfileArtifactsRequestRequestTypeDef",
     "ResourceProfileArtifactTypeDef",
-    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
     "ListResourceProfileDetectionsRequestRequestTypeDef",
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "PaginatorConfigTypeDef",
-    "SecurityHubConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "RevealConfigurationTypeDef",
     "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
     "SensitivityInspectionTemplateExcludesTypeDef",
     "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
-    "TagCriterionPairForJobOutputTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagValuePairOutputTypeDef",
     "TagValuePairTypeDef",
     "TestCustomDataIdentifierRequestRequestTypeDef",
-    "TestCustomDataIdentifierResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAllowListResponseTypeDef",
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     "UpdateClassificationJobRequestRequestTypeDef",
-    "UpdateFindingsFilterResponseTypeDef",
     "UpdateMacieSessionRequestRequestTypeDef",
     "UpdateMemberSessionRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateResourceProfileRequestRequestTypeDef",
     "UserIdentityRootTypeDef",
     "CreateMemberRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "AllowListCriteriaOutputTypeDef",
     "AllowListCriteriaTypeDef",
-    "ListAllowListsResponseTypeDef",
     "FindingActionTypeDef",
     "BatchGetCustomDataIdentifiersResponseTypeDef",
+    "CreateAllowListResponseTypeDef",
+    "CreateClassificationJobResponseTypeDef",
+    "CreateCustomDataIdentifierResponseTypeDef",
+    "CreateFindingsFilterResponseTypeDef",
+    "CreateMemberResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetMacieSessionResponseTypeDef",
+    "GetMemberResponseTypeDef",
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    "ListAllowListsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TestCustomDataIdentifierResponseTypeDef",
+    "UpdateAllowListResponseTypeDef",
+    "UpdateFindingsFilterResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "MatchingBucketTypeDef",
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "DescribeBucketsRequestRequestTypeDef",
     "BucketStatisticsBySensitivityTypeDef",
-    "ClassificationExportConfigurationOutputTypeDef",
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
+    "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "GetSensitiveDataOccurrencesResponseTypeDef",
     "ListResourceProfileDetectionsResponseTypeDef",
     "ListFindingsFiltersResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
-    "GetCustomDataIdentifierResponseTypeDef",
     "GetFindingStatisticsResponseTypeDef",
     "GetFindingsPublicationConfigurationResponseTypeDef",
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
+    "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
@@ -302,37 +293,35 @@
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
-    "UpdateRevealConfigurationRequestRequestTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
     "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
     "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
     "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
-    "GetAllowListResponseTypeDef",
     "CreateAllowListRequestRequestTypeDef",
+    "GetAllowListResponseTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
-    "PutClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
+    "PutClassificationExportConfigurationResponseTypeDef",
     "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
@@ -441,22 +430,14 @@
     {
         "accountId": str,
         "status": AdminStatusType,
     },
     total=False,
 )
 
-S3WordsListOutputTypeDef = TypedDict(
-    "S3WordsListOutputTypeDef",
-    {
-        "bucketName": str,
-        "objectKey": str,
-    },
-)
-
 S3WordsListTypeDef = TypedDict(
     "S3WordsListTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -538,14 +519,25 @@
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
     {
         "ids": Sequence[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 BucketCountByEffectivePermissionTypeDef = TypedDict(
     "BucketCountByEffectivePermissionTypeDef",
     {
         "publiclyAccessible": int,
         "publiclyReadable": int,
         "publiclyWritable": int,
         "unknown": int,
@@ -696,36 +688,14 @@
         "column": int,
         "columnName": str,
         "row": int,
     },
     total=False,
 )
 
-_RequiredS3DestinationOutputTypeDef = TypedDict(
-    "_RequiredS3DestinationOutputTypeDef",
-    {
-        "bucketName": str,
-        "kmsKeyArn": str,
-    },
-)
-_OptionalS3DestinationOutputTypeDef = TypedDict(
-    "_OptionalS3DestinationOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-
-class S3DestinationOutputTypeDef(
-    _RequiredS3DestinationOutputTypeDef, _OptionalS3DestinationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3DestinationTypeDef = TypedDict(
     "_RequiredS3DestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -756,57 +726,22 @@
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
-CreateAllowListResponseTypeDef = TypedDict(
-    "CreateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateClassificationJobResponseTypeDef = TypedDict(
-    "CreateClassificationJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SeverityLevelTypeDef = TypedDict(
     "SeverityLevelTypeDef",
     {
         "occurrencesThreshold": int,
         "severity": DataIdentifierSeverityType,
     },
 )
 
-CreateCustomDataIdentifierResponseTypeDef = TypedDict(
-    "CreateCustomDataIdentifierResponseTypeDef",
-    {
-        "customDataIdentifierId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFindingsFilterResponseTypeDef = TypedDict(
-    "CreateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateInvitationsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInvitationsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 _OptionalCreateInvitationsRequestRequestTypeDef = TypedDict(
@@ -831,22 +766,14 @@
         "accountId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
     total=False,
 )
 
-CreateMemberResponseTypeDef = TypedDict(
-    "CreateMemberResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "CreateSampleFindingsRequestRequestTypeDef",
     {
         "findingTypes": Sequence[FindingTypeType],
     },
     total=False,
 )
@@ -963,14 +890,24 @@
 DeleteMemberRequestRequestTypeDef = TypedDict(
     "DeleteMemberRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeClassificationJobRequestRequestTypeDef = TypedDict(
     "DescribeClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -997,23 +934,14 @@
         "jobExpiresAt": datetime,
         "jobImminentExpirationHealthEventArn": str,
         "jobPausedAt": datetime,
     },
     total=False,
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "autoEnable": bool,
-        "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectedDataDetailsTypeDef = TypedDict(
     "DetectedDataDetailsTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1128,27 +1056,14 @@
 GetAllowListRequestRequestTypeDef = TypedDict(
     "GetAllowListRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
-    {
-        "classificationScopeId": str,
-        "disabledAt": datetime,
-        "firstEnabledAt": datetime,
-        "lastUpdatedAt": datetime,
-        "sensitivityInspectionTemplateId": str,
-        "status": AutomatedDiscoveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBucketStatisticsRequestRequestTypeDef = TypedDict(
     "GetBucketStatisticsRequestRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
@@ -1163,22 +1078,14 @@
 GetCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "GetCustomDataIdentifierRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SeverityLevelOutputTypeDef = TypedDict(
-    "SeverityLevelOutputTypeDef",
-    {
-        "occurrencesThreshold": int,
-        "severity": DataIdentifierSeverityType,
-    },
-)
-
 GroupCountTypeDef = TypedDict(
     "GroupCountTypeDef",
     {
         "count": int,
         "groupKey": str,
     },
     total=False,
@@ -1187,16 +1094,16 @@
 GetFindingsFilterRequestRequestTypeDef = TypedDict(
     "GetFindingsFilterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SecurityHubConfigurationOutputTypeDef = TypedDict(
-    "SecurityHubConfigurationOutputTypeDef",
+SecurityHubConfigurationTypeDef = TypedDict(
+    "SecurityHubConfigurationTypeDef",
     {
         "publishClassificationFindings": bool,
         "publishPolicyFindings": bool,
     },
 )
 
 SortCriteriaTypeDef = TypedDict(
@@ -1204,57 +1111,21 @@
     {
         "attributeName": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "invitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMacieSessionResponseTypeDef = TypedDict(
-    "GetMacieSessionResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "findingPublishingFrequency": FindingPublishingFrequencyType,
-        "serviceRole": str,
-        "status": MacieStatusType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMemberRequestRequestTypeDef = TypedDict(
     "GetMemberRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetMemberResponseTypeDef = TypedDict(
-    "GetMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "administratorAccountId": str,
-        "arn": str,
-        "email": str,
-        "invitedAt": datetime,
-        "masterAccountId": str,
-        "relationshipStatus": RelationshipStatusType,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceProfileRequestRequestTypeDef = TypedDict(
     "GetResourceProfileRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1270,51 +1141,42 @@
         "totalItemsSkippedInvalidEncryption": int,
         "totalItemsSkippedInvalidKms": int,
         "totalItemsSkippedPermissionDenied": int,
     },
     total=False,
 )
 
-_RequiredRevealConfigurationOutputTypeDef = TypedDict(
-    "_RequiredRevealConfigurationOutputTypeDef",
+_RequiredRevealConfigurationTypeDef = TypedDict(
+    "_RequiredRevealConfigurationTypeDef",
     {
         "status": RevealStatusType,
     },
 )
-_OptionalRevealConfigurationOutputTypeDef = TypedDict(
-    "_OptionalRevealConfigurationOutputTypeDef",
+_OptionalRevealConfigurationTypeDef = TypedDict(
+    "_OptionalRevealConfigurationTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
 
-class RevealConfigurationOutputTypeDef(
-    _RequiredRevealConfigurationOutputTypeDef, _OptionalRevealConfigurationOutputTypeDef
+class RevealConfigurationTypeDef(
+    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
 ):
     pass
 
 
 GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 
-GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
-    {
-        "code": AvailabilityCodeType,
-        "reasons": List[UnavailabilityReasonCodeType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1433,30 +1295,14 @@
         "asnOrg": str,
         "isp": str,
         "org": str,
     },
     total=False,
 )
 
-MonthlyScheduleOutputTypeDef = TypedDict(
-    "MonthlyScheduleOutputTypeDef",
-    {
-        "dayOfMonth": int,
-    },
-    total=False,
-)
-
-WeeklyScheduleOutputTypeDef = TypedDict(
-    "WeeklyScheduleOutputTypeDef",
-    {
-        "dayOfWeek": DayOfWeekType,
-    },
-    total=False,
-)
-
 MonthlyScheduleTypeDef = TypedDict(
     "MonthlyScheduleTypeDef",
     {
         "dayOfMonth": int,
     },
     total=False,
 )
@@ -1493,22 +1339,14 @@
     "S3BucketDefinitionForJobOutputTypeDef",
     {
         "accountId": str,
         "buckets": List[str],
     },
 )
 
-ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAllowListsRequestRequestTypeDef = TypedDict(
     "ListAllowListsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1519,83 +1357,41 @@
     {
         "attributeName": ListJobsSortAttributeNameType,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClassificationScopesRequestRequestTypeDef = TypedDict(
     "ListClassificationScopesRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListCustomDataIdentifiersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFindingsFiltersRequestRequestTypeDef = TypedDict(
     "ListFindingsFiltersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1607,22 +1403,14 @@
         "comparator": JobComparatorType,
         "key": ListJobsFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1632,23 +1420,14 @@
     {
         "category": SensitiveDataItemCategoryType,
         "id": str,
     },
     total=False,
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": str,
     },
@@ -1667,53 +1446,23 @@
         "relationshipStatus": RelationshipStatusType,
         "tags": Dict[str, str],
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
-    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileArtifactsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
@@ -1750,40 +1499,14 @@
 
 class ResourceProfileArtifactTypeDef(
     _RequiredResourceProfileArtifactTypeDef, _OptionalResourceProfileArtifactTypeDef
 ):
     pass
 
 
-_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "resourceArn": str,
-        },
-    )
-)
-_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
-    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileDetectionsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
@@ -1799,22 +1522,14 @@
 class ListResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredListResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalListResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSensitivityInspectionTemplatesRequestRequestTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1832,22 +1547,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "end": int,
         "start": int,
         "startColumn": int,
     },
@@ -1859,64 +1566,14 @@
     {
         "jsonPath": str,
         "recordIndex": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-SecurityHubConfigurationTypeDef = TypedDict(
-    "SecurityHubConfigurationTypeDef",
-    {
-        "publishClassificationFindings": bool,
-        "publishPolicyFindings": bool,
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-_RequiredRevealConfigurationTypeDef = TypedDict(
-    "_RequiredRevealConfigurationTypeDef",
-    {
-        "status": RevealStatusType,
-    },
-)
-_OptionalRevealConfigurationTypeDef = TypedDict(
-    "_OptionalRevealConfigurationTypeDef",
-    {
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class RevealConfigurationTypeDef(
-    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
-):
-    pass
-
-
 S3BucketDefinitionForJobTypeDef = TypedDict(
     "S3BucketDefinitionForJobTypeDef",
     {
         "accountId": str,
         "buckets": Sequence[str],
     },
 )
@@ -2036,23 +1693,14 @@
     {
         "id": str,
         "type": DataIdentifierTypeType,
     },
     total=False,
 )
 
-TagCriterionPairForJobOutputTypeDef = TypedDict(
-    "TagCriterionPairForJobOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 TagCriterionPairForJobTypeDef = TypedDict(
     "TagCriterionPairForJobTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -2062,23 +1710,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
-TagValuePairOutputTypeDef = TypedDict(
-    "TagValuePairOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 TagValuePairTypeDef = TypedDict(
     "TagValuePairTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -2105,39 +1744,22 @@
 class TestCustomDataIdentifierRequestRequestTypeDef(
     _RequiredTestCustomDataIdentifierRequestRequestTypeDef,
     _OptionalTestCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
 
-TestCustomDataIdentifierResponseTypeDef = TypedDict(
-    "TestCustomDataIdentifierResponseTypeDef",
-    {
-        "matchCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAllowListResponseTypeDef = TypedDict(
-    "UpdateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     {
         "status": AutomatedDiscoveryStatusType,
     },
 )
 
@@ -2145,23 +1767,14 @@
     "UpdateClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
         "jobStatus": JobStatusType,
     },
 )
 
-UpdateFindingsFilterResponseTypeDef = TypedDict(
-    "UpdateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateMacieSessionRequestRequestTypeDef = TypedDict(
     "UpdateMacieSessionRequestRequestTypeDef",
     {
         "findingPublishingFrequency": FindingPublishingFrequencyType,
         "status": MacieStatusType,
     },
     total=False,
@@ -2239,65 +1852,209 @@
     "AccountLevelPermissionsTypeDef",
     {
         "blockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
+AllowListCriteriaTypeDef = TypedDict(
+    "AllowListCriteriaTypeDef",
     {
-        "adminAccounts": List[AdminAccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "regex": str,
+        "s3WordsList": S3WordsListTypeDef,
     },
+    total=False,
 )
 
-AllowListCriteriaOutputTypeDef = TypedDict(
-    "AllowListCriteriaOutputTypeDef",
+FindingActionTypeDef = TypedDict(
+    "FindingActionTypeDef",
     {
-        "regex": str,
-        "s3WordsList": S3WordsListOutputTypeDef,
+        "actionType": Literal["AWS_API_CALL"],
+        "apiCallDetails": ApiCallDetailsTypeDef,
     },
     total=False,
 )
 
-AllowListCriteriaTypeDef = TypedDict(
-    "AllowListCriteriaTypeDef",
+BatchGetCustomDataIdentifiersResponseTypeDef = TypedDict(
+    "BatchGetCustomDataIdentifiersResponseTypeDef",
     {
-        "regex": str,
-        "s3WordsList": S3WordsListTypeDef,
+        "customDataIdentifiers": List[BatchGetCustomDataIdentifierSummaryTypeDef],
+        "notFoundIdentifierIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAllowListResponseTypeDef = TypedDict(
+    "CreateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateClassificationJobResponseTypeDef = TypedDict(
+    "CreateClassificationJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDataIdentifierResponseTypeDef = TypedDict(
+    "CreateCustomDataIdentifierResponseTypeDef",
+    {
+        "customDataIdentifierId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsFilterResponseTypeDef = TypedDict(
+    "CreateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberResponseTypeDef = TypedDict(
+    "CreateMemberResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "autoEnable": bool,
+        "maxAccountLimitReached": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    {
+        "classificationScopeId": str,
+        "disabledAt": datetime,
+        "firstEnabledAt": datetime,
+        "lastUpdatedAt": datetime,
+        "sensitivityInspectionTemplateId": str,
+        "status": AutomatedDiscoveryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "invitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMacieSessionResponseTypeDef = TypedDict(
+    "GetMacieSessionResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "findingPublishingFrequency": FindingPublishingFrequencyType,
+        "serviceRole": str,
+        "status": MacieStatusType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMemberResponseTypeDef = TypedDict(
+    "GetMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "administratorAccountId": str,
+        "arn": str,
+        "email": str,
+        "invitedAt": datetime,
+        "masterAccountId": str,
+        "relationshipStatus": RelationshipStatusType,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    {
+        "code": AvailabilityCodeType,
+        "reasons": List[UnavailabilityReasonCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListAllowListsResponseTypeDef = TypedDict(
     "ListAllowListsResponseTypeDef",
     {
         "allowLists": List[AllowListSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FindingActionTypeDef = TypedDict(
-    "FindingActionTypeDef",
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
     {
-        "actionType": Literal["AWS_API_CALL"],
-        "apiCallDetails": ApiCallDetailsTypeDef,
+        "findingIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchGetCustomDataIdentifiersResponseTypeDef = TypedDict(
-    "BatchGetCustomDataIdentifiersResponseTypeDef",
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
     {
-        "customDataIdentifiers": List[BatchGetCustomDataIdentifierSummaryTypeDef],
-        "notFoundIdentifierIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "adminAccounts": List[AdminAccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestCustomDataIdentifierResponseTypeDef = TypedDict(
+    "TestCustomDataIdentifierResponseTypeDef",
+    {
+        "matchCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAllowListResponseTypeDef = TypedDict(
+    "UpdateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFindingsFilterResponseTypeDef = TypedDict(
+    "UpdateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "accessControlList": AccessControlListTypeDef,
@@ -2325,24 +2082,14 @@
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
     },
     total=False,
 )
 
-DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
-    {
-        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
-        "sortCriteria": BucketSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeBucketsRequestRequestTypeDef = TypedDict(
     "DescribeBucketsRequestRequestTypeDef",
     {
         "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
         "maxResults": int,
         "nextToken": str,
         "sortCriteria": BucketSortCriteriaTypeDef,
@@ -2357,36 +2104,28 @@
         "notClassified": SensitivityAggregationsTypeDef,
         "notSensitive": SensitivityAggregationsTypeDef,
         "sensitive": SensitivityAggregationsTypeDef,
     },
     total=False,
 )
 
-ClassificationExportConfigurationOutputTypeDef = TypedDict(
-    "ClassificationExportConfigurationOutputTypeDef",
-    {
-        "s3Destination": S3DestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 ClassificationExportConfigurationTypeDef = TypedDict(
     "ClassificationExportConfigurationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
 
 ListClassificationScopesResponseTypeDef = TypedDict(
     "ListClassificationScopesResponseTypeDef",
     {
         "classificationScopes": List[ClassificationScopeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDataIdentifierRequestRequestTypeDef",
     {
         "name": str,
@@ -2411,35 +2150,54 @@
 class CreateCustomDataIdentifierRequestRequestTypeDef(
     _RequiredCreateCustomDataIdentifierRequestRequestTypeDef,
     _OptionalCreateCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
 
+GetCustomDataIdentifierResponseTypeDef = TypedDict(
+    "GetCustomDataIdentifierResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deleted": bool,
+        "description": str,
+        "id": str,
+        "ignoreWords": List[str],
+        "keywords": List[str],
+        "maximumMatchDistance": int,
+        "name": str,
+        "regex": str,
+        "severityLevels": List[SeverityLevelTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateInvitationsResponseTypeDef = TypedDict(
     "CreateInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingCriteriaOutputTypeDef = TypedDict(
     "FindingCriteriaOutputTypeDef",
     {
         "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
@@ -2456,106 +2214,228 @@
 )
 
 ListCustomDataIdentifiersResponseTypeDef = TypedDict(
     "ListCustomDataIdentifiersResponseTypeDef",
     {
         "items": List[CustomDataIdentifierSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    {
+        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
+        "sortCriteria": BucketSortCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    {
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
+    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "resourceArn": str,
+        },
+    )
+)
+_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
+    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+):
+    pass
+
+
+ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 GetSensitiveDataOccurrencesResponseTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesResponseTypeDef",
     {
         "error": str,
         "sensitiveDataOccurrences": Dict[str, List[DetectedDataDetailsTypeDef]],
         "status": RevealRequestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceProfileDetectionsResponseTypeDef = TypedDict(
     "ListResourceProfileDetectionsResponseTypeDef",
     {
         "detections": List[DetectionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsFiltersResponseTypeDef = TypedDict(
     "ListFindingsFiltersResponseTypeDef",
     {
         "findingsFilterListItems": List[FindingsFilterListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "administrator": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "master": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "invitations": List[InvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCustomDataIdentifierResponseTypeDef = TypedDict(
-    "GetCustomDataIdentifierResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "deleted": bool,
-        "description": str,
-        "id": str,
-        "ignoreWords": List[str],
-        "keywords": List[str],
-        "maximumMatchDistance": int,
-        "name": str,
-        "regex": str,
-        "severityLevels": List[SeverityLevelOutputTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingStatisticsResponseTypeDef = TypedDict(
     "GetFindingStatisticsResponseTypeDef",
     {
         "countsByGroup": List[GroupCountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsPublicationConfigurationResponseTypeDef = TypedDict(
     "GetFindingsPublicationConfigurationResponseTypeDef",
     {
-        "securityHubConfiguration": SecurityHubConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "findingIds": Sequence[str],
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -2576,31 +2456,38 @@
 GetResourceProfileResponseTypeDef = TypedDict(
     "GetResourceProfileResponseTypeDef",
     {
         "profileUpdatedAt": datetime,
         "sensitivityScore": int,
         "sensitivityScoreOverridden": bool,
         "statistics": ResourceStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRevealConfigurationResponseTypeDef = TypedDict(
     "GetRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": RevealConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateRevealConfigurationRequestRequestTypeDef",
+    {
+        "configuration": RevealConfigurationTypeDef,
     },
 )
 
 UpdateRevealConfigurationResponseTypeDef = TypedDict(
     "UpdateRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": RevealConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef = TypedDict(
     "_RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     {
         "findingId": str,
@@ -2626,25 +2513,25 @@
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
         "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
         "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "GetUsageStatisticsRequestRequestTypeDef",
     {
@@ -2658,15 +2545,15 @@
 )
 
 GetUsageTotalsResponseTypeDef = TypedDict(
     "GetUsageTotalsResponseTypeDef",
     {
         "timeRange": TimeRangeType,
         "usageTotals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IpAddressDetailsTypeDef = TypedDict(
     "IpAddressDetailsTypeDef",
     {
         "ipAddressV4": str,
@@ -2678,16 +2565,16 @@
     total=False,
 )
 
 JobScheduleFrequencyOutputTypeDef = TypedDict(
     "JobScheduleFrequencyOutputTypeDef",
     {
         "dailySchedule": Dict[str, Any],
-        "monthlySchedule": MonthlyScheduleOutputTypeDef,
-        "weeklySchedule": WeeklyScheduleOutputTypeDef,
+        "monthlySchedule": MonthlyScheduleTypeDef,
+        "weeklySchedule": WeeklyScheduleTypeDef,
     },
     total=False,
 )
 
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
@@ -2708,71 +2595,55 @@
 )
 
 ListManagedDataIdentifiersResponseTypeDef = TypedDict(
     "ListManagedDataIdentifiersResponseTypeDef",
     {
         "items": List[ManagedDataIdentifierSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceProfileArtifactsResponseTypeDef = TypedDict(
     "ListResourceProfileArtifactsResponseTypeDef",
     {
         "artifacts": List[ResourceProfileArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSensitivityInspectionTemplatesResponseTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "sensitivityInspectionTemplates": List[SensitivityInspectionTemplatesEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "lineRange": RangeTypeDef,
         "offsetRange": RangeTypeDef,
         "pageNumber": int,
     },
     total=False,
 )
 
-PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
-    },
-    total=False,
-)
-
-UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateRevealConfigurationRequestRequestTypeDef",
-    {
-        "configuration": RevealConfigurationTypeDef,
-    },
-)
-
 S3ObjectTypeDef = TypedDict(
     "S3ObjectTypeDef",
     {
         "bucketArn": str,
         "eTag": str,
         "extension": str,
         "key": str,
@@ -2877,15 +2748,15 @@
     pass
 
 
 TagCriterionForJobOutputTypeDef = TypedDict(
     "TagCriterionForJobOutputTypeDef",
     {
         "comparator": JobComparatorType,
-        "tagValues": List[TagCriterionPairForJobOutputTypeDef],
+        "tagValues": List[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
@@ -2896,15 +2767,15 @@
 )
 
 TagScopeTermOutputTypeDef = TypedDict(
     "TagScopeTermOutputTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
-        "tagValues": List[TagValuePairOutputTypeDef],
+        "tagValues": List[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
     },
     total=False,
 )
 
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
@@ -2913,30 +2784,14 @@
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
     },
     total=False,
 )
 
-GetAllowListResponseTypeDef = TypedDict(
-    "GetAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": AllowListCriteriaOutputTypeDef,
-        "description": str,
-        "id": str,
-        "name": str,
-        "status": AllowListStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAllowListRequestRequestTypeDef",
     {
         "clientToken": str,
         "criteria": AllowListCriteriaTypeDef,
         "name": str,
     },
@@ -2953,14 +2808,30 @@
 
 class CreateAllowListRequestRequestTypeDef(
     _RequiredCreateAllowListRequestRequestTypeDef, _OptionalCreateAllowListRequestRequestTypeDef
 ):
     pass
 
 
+GetAllowListResponseTypeDef = TypedDict(
+    "GetAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": AllowListCriteriaTypeDef,
+        "description": str,
+        "id": str,
+        "name": str,
+        "status": AllowListStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAllowListRequestRequestTypeDef",
     {
         "criteria": AllowListCriteriaTypeDef,
         "id": str,
         "name": str,
     },
@@ -3012,53 +2883,53 @@
         "classifiableSizeInBytes": int,
         "lastUpdated": datetime,
         "objectCount": int,
         "sizeInBytes": int,
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClassificationExportConfigurationResponseTypeDef = TypedDict(
     "GetClassificationExportConfigurationResponseTypeDef",
     {
-        "configuration": ClassificationExportConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": ClassificationExportConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutClassificationExportConfigurationResponseTypeDef = TypedDict(
-    "PutClassificationExportConfigurationResponseTypeDef",
+PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
+    "PutClassificationExportConfigurationRequestRequestTypeDef",
     {
-        "configuration": ClassificationExportConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": ClassificationExportConfigurationTypeDef,
     },
 )
 
-PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
-    "PutClassificationExportConfigurationRequestRequestTypeDef",
+PutClassificationExportConfigurationResponseTypeDef = TypedDict(
+    "PutClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsFilterResponseTypeDef = TypedDict(
     "GetFindingsFilterResponseTypeDef",
     {
         "action": FindingsFilterActionType,
         "arn": str,
         "description": str,
         "findingCriteria": FindingCriteriaOutputTypeDef,
         "id": str,
         "name": str,
         "position": int,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
         "action": FindingsFilterActionType,
@@ -3110,15 +2981,15 @@
 
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -3158,15 +3029,15 @@
 
 
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListClassificationJobsRequestRequestTypeDef",
     {
@@ -3192,15 +3063,15 @@
 
 GetClassificationScopeResponseTypeDef = TypedDict(
     "GetClassificationScopeResponseTypeDef",
     {
         "id": str,
         "name": str,
         "s3": S3ClassificationScopeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateClassificationScopeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClassificationScopeRequestRequestTypeDef",
     {
         "id": str,
@@ -3312,15 +3183,15 @@
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "matchingResources": List[MatchingResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDetectionTypeDef = TypedDict(
     "CustomDetectionTypeDef",
     {
         "arn": str,
@@ -3351,15 +3222,15 @@
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "nextToken": str,
         "records": List[UsageRecordTypeDef],
         "timeRange": TimeRangeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "assumedRole": AssumedRoleTypeDef,
@@ -3528,15 +3399,15 @@
 )
 
 DescribeBucketsResponseTypeDef = TypedDict(
     "DescribeBucketsResponseTypeDef",
     {
         "buckets": List[BucketMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourcesAffectedTypeDef = TypedDict(
     "ResourcesAffectedTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
@@ -3570,15 +3441,15 @@
 )
 
 SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     {
         "bucketCriteria": SearchResourcesBucketCriteriaTypeDef,
         "sortCriteria": SearchResourcesSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 PolicyDetailsTypeDef = TypedDict(
     "PolicyDetailsTypeDef",
     {
@@ -3637,15 +3508,15 @@
 )
 
 ListClassificationJobsResponseTypeDef = TypedDict(
     "ListClassificationJobsResponseTypeDef",
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClassificationJobResponseTypeDef = TypedDict(
     "DescribeClassificationJobResponseTypeDef",
     {
         "allowListIds": List[str],
@@ -3665,15 +3536,15 @@
         "name": str,
         "s3JobDefinition": S3JobDefinitionOutputTypeDef,
         "samplingPercentage": int,
         "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
         "statistics": StatisticsTypeDef,
         "tags": Dict[str, str],
         "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -3731,10 +3602,10 @@
     total=False,
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/type_defs.pyi` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,23 +79,23 @@
 
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccountDetailTypeDef",
     "BlockPublicAccessTypeDef",
     "AdminAccountTypeDef",
-    "S3WordsListOutputTypeDef",
     "S3WordsListTypeDef",
     "AllowListStatusTypeDef",
     "AllowListSummaryTypeDef",
     "ApiCallDetailsTypeDef",
     "AwsAccountTypeDef",
     "AwsServiceTypeDef",
     "BatchGetCustomDataIdentifierSummaryTypeDef",
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BucketCountByEffectivePermissionTypeDef",
     "BucketCountByEncryptionTypeTypeDef",
     "BucketCountBySharedAccessTypeTypeDef",
     "BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef",
     "BucketCriteriaAdditionalPropertiesTypeDef",
     "BucketPolicyTypeDef",
     "BucketServerSideEncryptionTypeDef",
@@ -103,197 +103,188 @@
     "KeyValuePairTypeDef",
     "ObjectCountByEncryptionTypeTypeDef",
     "ObjectLevelStatisticsTypeDef",
     "ReplicationDetailsTypeDef",
     "BucketSortCriteriaTypeDef",
     "SensitivityAggregationsTypeDef",
     "CellTypeDef",
-    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
-    "CreateAllowListResponseTypeDef",
-    "CreateClassificationJobResponseTypeDef",
     "SeverityLevelTypeDef",
-    "CreateCustomDataIdentifierResponseTypeDef",
-    "CreateFindingsFilterResponseTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
-    "CreateMemberResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
     "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMemberRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClassificationJobRequestRequestTypeDef",
     "LastRunErrorStatusTypeDef",
     "StatisticsTypeDef",
     "UserPausedDetailsTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
     "DetectedDataDetailsTypeDef",
     "DetectionTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "EnableMacieRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "FindingStatisticsSortCriteriaTypeDef",
     "SeverityTypeDef",
     "FindingsFilterListItemTypeDef",
     "InvitationTypeDef",
     "GetAllowListRequestRequestTypeDef",
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
     "GetBucketStatisticsRequestRequestTypeDef",
     "GetClassificationScopeRequestRequestTypeDef",
     "GetCustomDataIdentifierRequestRequestTypeDef",
-    "SeverityLevelOutputTypeDef",
     "GroupCountTypeDef",
     "GetFindingsFilterRequestRequestTypeDef",
-    "SecurityHubConfigurationOutputTypeDef",
+    "SecurityHubConfigurationTypeDef",
     "SortCriteriaTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "GetMacieSessionResponseTypeDef",
     "GetMemberRequestRequestTypeDef",
-    "GetMemberResponseTypeDef",
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
-    "RevealConfigurationOutputTypeDef",
+    "RevealConfigurationTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     "SensitivityInspectionTemplateExcludesOutputTypeDef",
     "SensitivityInspectionTemplateIncludesOutputTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
-    "MonthlyScheduleOutputTypeDef",
-    "WeeklyScheduleOutputTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
     "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
     "S3BucketDefinitionForJobOutputTypeDef",
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
     "ListFindingsFiltersRequestRequestTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListJobsFilterTermTypeDef",
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     "ManagedDataIdentifierSummaryTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "MemberTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
     "ListResourceProfileArtifactsRequestRequestTypeDef",
     "ResourceProfileArtifactTypeDef",
-    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
     "ListResourceProfileDetectionsRequestRequestTypeDef",
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "PaginatorConfigTypeDef",
-    "SecurityHubConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "RevealConfigurationTypeDef",
     "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
     "SensitivityInspectionTemplateExcludesTypeDef",
     "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
-    "TagCriterionPairForJobOutputTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagValuePairOutputTypeDef",
     "TagValuePairTypeDef",
     "TestCustomDataIdentifierRequestRequestTypeDef",
-    "TestCustomDataIdentifierResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAllowListResponseTypeDef",
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     "UpdateClassificationJobRequestRequestTypeDef",
-    "UpdateFindingsFilterResponseTypeDef",
     "UpdateMacieSessionRequestRequestTypeDef",
     "UpdateMemberSessionRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateResourceProfileRequestRequestTypeDef",
     "UserIdentityRootTypeDef",
     "CreateMemberRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "AllowListCriteriaOutputTypeDef",
     "AllowListCriteriaTypeDef",
-    "ListAllowListsResponseTypeDef",
     "FindingActionTypeDef",
     "BatchGetCustomDataIdentifiersResponseTypeDef",
+    "CreateAllowListResponseTypeDef",
+    "CreateClassificationJobResponseTypeDef",
+    "CreateCustomDataIdentifierResponseTypeDef",
+    "CreateFindingsFilterResponseTypeDef",
+    "CreateMemberResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetMacieSessionResponseTypeDef",
+    "GetMemberResponseTypeDef",
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    "ListAllowListsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TestCustomDataIdentifierResponseTypeDef",
+    "UpdateAllowListResponseTypeDef",
+    "UpdateFindingsFilterResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "MatchingBucketTypeDef",
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "DescribeBucketsRequestRequestTypeDef",
     "BucketStatisticsBySensitivityTypeDef",
-    "ClassificationExportConfigurationOutputTypeDef",
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
+    "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "GetSensitiveDataOccurrencesResponseTypeDef",
     "ListResourceProfileDetectionsResponseTypeDef",
     "ListFindingsFiltersResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
-    "GetCustomDataIdentifierResponseTypeDef",
     "GetFindingStatisticsResponseTypeDef",
     "GetFindingsPublicationConfigurationResponseTypeDef",
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
+    "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
@@ -301,37 +292,35 @@
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
-    "UpdateRevealConfigurationRequestRequestTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
     "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
     "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
     "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
-    "GetAllowListResponseTypeDef",
     "CreateAllowListRequestRequestTypeDef",
+    "GetAllowListResponseTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
-    "PutClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
+    "PutClassificationExportConfigurationResponseTypeDef",
     "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
@@ -438,22 +427,14 @@
     {
         "accountId": str,
         "status": AdminStatusType,
     },
     total=False,
 )
 
-S3WordsListOutputTypeDef = TypedDict(
-    "S3WordsListOutputTypeDef",
-    {
-        "bucketName": str,
-        "objectKey": str,
-    },
-)
-
 S3WordsListTypeDef = TypedDict(
     "S3WordsListTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -533,14 +514,25 @@
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
     {
         "ids": Sequence[str],
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 BucketCountByEffectivePermissionTypeDef = TypedDict(
     "BucketCountByEffectivePermissionTypeDef",
     {
         "publiclyAccessible": int,
         "publiclyReadable": int,
         "publiclyWritable": int,
         "unknown": int,
@@ -691,34 +683,14 @@
         "column": int,
         "columnName": str,
         "row": int,
     },
     total=False,
 )
 
-_RequiredS3DestinationOutputTypeDef = TypedDict(
-    "_RequiredS3DestinationOutputTypeDef",
-    {
-        "bucketName": str,
-        "kmsKeyArn": str,
-    },
-)
-_OptionalS3DestinationOutputTypeDef = TypedDict(
-    "_OptionalS3DestinationOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-class S3DestinationOutputTypeDef(
-    _RequiredS3DestinationOutputTypeDef, _OptionalS3DestinationOutputTypeDef
-):
-    pass
-
 _RequiredS3DestinationTypeDef = TypedDict(
     "_RequiredS3DestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -747,57 +719,22 @@
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
-CreateAllowListResponseTypeDef = TypedDict(
-    "CreateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateClassificationJobResponseTypeDef = TypedDict(
-    "CreateClassificationJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SeverityLevelTypeDef = TypedDict(
     "SeverityLevelTypeDef",
     {
         "occurrencesThreshold": int,
         "severity": DataIdentifierSeverityType,
     },
 )
 
-CreateCustomDataIdentifierResponseTypeDef = TypedDict(
-    "CreateCustomDataIdentifierResponseTypeDef",
-    {
-        "customDataIdentifierId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFindingsFilterResponseTypeDef = TypedDict(
-    "CreateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateInvitationsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInvitationsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 _OptionalCreateInvitationsRequestRequestTypeDef = TypedDict(
@@ -820,22 +757,14 @@
         "accountId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
     total=False,
 )
 
-CreateMemberResponseTypeDef = TypedDict(
-    "CreateMemberResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "CreateSampleFindingsRequestRequestTypeDef",
     {
         "findingTypes": Sequence[FindingTypeType],
     },
     total=False,
 )
@@ -950,14 +879,24 @@
 DeleteMemberRequestRequestTypeDef = TypedDict(
     "DeleteMemberRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeClassificationJobRequestRequestTypeDef = TypedDict(
     "DescribeClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -984,23 +923,14 @@
         "jobExpiresAt": datetime,
         "jobImminentExpirationHealthEventArn": str,
         "jobPausedAt": datetime,
     },
     total=False,
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "autoEnable": bool,
-        "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectedDataDetailsTypeDef = TypedDict(
     "DetectedDataDetailsTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1113,27 +1043,14 @@
 GetAllowListRequestRequestTypeDef = TypedDict(
     "GetAllowListRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
-    {
-        "classificationScopeId": str,
-        "disabledAt": datetime,
-        "firstEnabledAt": datetime,
-        "lastUpdatedAt": datetime,
-        "sensitivityInspectionTemplateId": str,
-        "status": AutomatedDiscoveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBucketStatisticsRequestRequestTypeDef = TypedDict(
     "GetBucketStatisticsRequestRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
@@ -1148,22 +1065,14 @@
 GetCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "GetCustomDataIdentifierRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SeverityLevelOutputTypeDef = TypedDict(
-    "SeverityLevelOutputTypeDef",
-    {
-        "occurrencesThreshold": int,
-        "severity": DataIdentifierSeverityType,
-    },
-)
-
 GroupCountTypeDef = TypedDict(
     "GroupCountTypeDef",
     {
         "count": int,
         "groupKey": str,
     },
     total=False,
@@ -1172,16 +1081,16 @@
 GetFindingsFilterRequestRequestTypeDef = TypedDict(
     "GetFindingsFilterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SecurityHubConfigurationOutputTypeDef = TypedDict(
-    "SecurityHubConfigurationOutputTypeDef",
+SecurityHubConfigurationTypeDef = TypedDict(
+    "SecurityHubConfigurationTypeDef",
     {
         "publishClassificationFindings": bool,
         "publishPolicyFindings": bool,
     },
 )
 
 SortCriteriaTypeDef = TypedDict(
@@ -1189,57 +1098,21 @@
     {
         "attributeName": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "invitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMacieSessionResponseTypeDef = TypedDict(
-    "GetMacieSessionResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "findingPublishingFrequency": FindingPublishingFrequencyType,
-        "serviceRole": str,
-        "status": MacieStatusType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMemberRequestRequestTypeDef = TypedDict(
     "GetMemberRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetMemberResponseTypeDef = TypedDict(
-    "GetMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "administratorAccountId": str,
-        "arn": str,
-        "email": str,
-        "invitedAt": datetime,
-        "masterAccountId": str,
-        "relationshipStatus": RelationshipStatusType,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceProfileRequestRequestTypeDef = TypedDict(
     "GetResourceProfileRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1255,49 +1128,40 @@
         "totalItemsSkippedInvalidEncryption": int,
         "totalItemsSkippedInvalidKms": int,
         "totalItemsSkippedPermissionDenied": int,
     },
     total=False,
 )
 
-_RequiredRevealConfigurationOutputTypeDef = TypedDict(
-    "_RequiredRevealConfigurationOutputTypeDef",
+_RequiredRevealConfigurationTypeDef = TypedDict(
+    "_RequiredRevealConfigurationTypeDef",
     {
         "status": RevealStatusType,
     },
 )
-_OptionalRevealConfigurationOutputTypeDef = TypedDict(
-    "_OptionalRevealConfigurationOutputTypeDef",
+_OptionalRevealConfigurationTypeDef = TypedDict(
+    "_OptionalRevealConfigurationTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
-class RevealConfigurationOutputTypeDef(
-    _RequiredRevealConfigurationOutputTypeDef, _OptionalRevealConfigurationOutputTypeDef
+class RevealConfigurationTypeDef(
+    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
 ):
     pass
 
 GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 
-GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
-    {
-        "code": AvailabilityCodeType,
-        "reasons": List[UnavailabilityReasonCodeType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1416,30 +1280,14 @@
         "asnOrg": str,
         "isp": str,
         "org": str,
     },
     total=False,
 )
 
-MonthlyScheduleOutputTypeDef = TypedDict(
-    "MonthlyScheduleOutputTypeDef",
-    {
-        "dayOfMonth": int,
-    },
-    total=False,
-)
-
-WeeklyScheduleOutputTypeDef = TypedDict(
-    "WeeklyScheduleOutputTypeDef",
-    {
-        "dayOfWeek": DayOfWeekType,
-    },
-    total=False,
-)
-
 MonthlyScheduleTypeDef = TypedDict(
     "MonthlyScheduleTypeDef",
     {
         "dayOfMonth": int,
     },
     total=False,
 )
@@ -1476,22 +1324,14 @@
     "S3BucketDefinitionForJobOutputTypeDef",
     {
         "accountId": str,
         "buckets": List[str],
     },
 )
 
-ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAllowListsRequestRequestTypeDef = TypedDict(
     "ListAllowListsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1502,83 +1342,41 @@
     {
         "attributeName": ListJobsSortAttributeNameType,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClassificationScopesRequestRequestTypeDef = TypedDict(
     "ListClassificationScopesRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListCustomDataIdentifiersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFindingsFiltersRequestRequestTypeDef = TypedDict(
     "ListFindingsFiltersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1590,22 +1388,14 @@
         "comparator": JobComparatorType,
         "key": ListJobsFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1615,23 +1405,14 @@
     {
         "category": SensitiveDataItemCategoryType,
         "id": str,
     },
     total=False,
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": str,
     },
@@ -1650,51 +1431,23 @@
         "relationshipStatus": RelationshipStatusType,
         "tags": Dict[str, str],
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
-    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileArtifactsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
@@ -1727,38 +1480,14 @@
 )
 
 class ResourceProfileArtifactTypeDef(
     _RequiredResourceProfileArtifactTypeDef, _OptionalResourceProfileArtifactTypeDef
 ):
     pass
 
-_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "resourceArn": str,
-        },
-    )
-)
-_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
-    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileDetectionsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
@@ -1772,22 +1501,14 @@
 
 class ListResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredListResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalListResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
-ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSensitivityInspectionTemplatesRequestRequestTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1805,22 +1526,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "end": int,
         "start": int,
         "startColumn": int,
     },
@@ -1832,62 +1545,14 @@
     {
         "jsonPath": str,
         "recordIndex": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-SecurityHubConfigurationTypeDef = TypedDict(
-    "SecurityHubConfigurationTypeDef",
-    {
-        "publishClassificationFindings": bool,
-        "publishPolicyFindings": bool,
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-_RequiredRevealConfigurationTypeDef = TypedDict(
-    "_RequiredRevealConfigurationTypeDef",
-    {
-        "status": RevealStatusType,
-    },
-)
-_OptionalRevealConfigurationTypeDef = TypedDict(
-    "_OptionalRevealConfigurationTypeDef",
-    {
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-class RevealConfigurationTypeDef(
-    _RequiredRevealConfigurationTypeDef, _OptionalRevealConfigurationTypeDef
-):
-    pass
-
 S3BucketDefinitionForJobTypeDef = TypedDict(
     "S3BucketDefinitionForJobTypeDef",
     {
         "accountId": str,
         "buckets": Sequence[str],
     },
 )
@@ -2007,23 +1672,14 @@
     {
         "id": str,
         "type": DataIdentifierTypeType,
     },
     total=False,
 )
 
-TagCriterionPairForJobOutputTypeDef = TypedDict(
-    "TagCriterionPairForJobOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 TagCriterionPairForJobTypeDef = TypedDict(
     "TagCriterionPairForJobTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -2033,23 +1689,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
-TagValuePairOutputTypeDef = TypedDict(
-    "TagValuePairOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 TagValuePairTypeDef = TypedDict(
     "TagValuePairTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -2074,39 +1721,22 @@
 
 class TestCustomDataIdentifierRequestRequestTypeDef(
     _RequiredTestCustomDataIdentifierRequestRequestTypeDef,
     _OptionalTestCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
-TestCustomDataIdentifierResponseTypeDef = TypedDict(
-    "TestCustomDataIdentifierResponseTypeDef",
-    {
-        "matchCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAllowListResponseTypeDef = TypedDict(
-    "UpdateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     {
         "status": AutomatedDiscoveryStatusType,
     },
 )
 
@@ -2114,23 +1744,14 @@
     "UpdateClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
         "jobStatus": JobStatusType,
     },
 )
 
-UpdateFindingsFilterResponseTypeDef = TypedDict(
-    "UpdateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateMacieSessionRequestRequestTypeDef = TypedDict(
     "UpdateMacieSessionRequestRequestTypeDef",
     {
         "findingPublishingFrequency": FindingPublishingFrequencyType,
         "status": MacieStatusType,
     },
     total=False,
@@ -2204,65 +1825,209 @@
     "AccountLevelPermissionsTypeDef",
     {
         "blockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
+AllowListCriteriaTypeDef = TypedDict(
+    "AllowListCriteriaTypeDef",
     {
-        "adminAccounts": List[AdminAccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "regex": str,
+        "s3WordsList": S3WordsListTypeDef,
     },
+    total=False,
 )
 
-AllowListCriteriaOutputTypeDef = TypedDict(
-    "AllowListCriteriaOutputTypeDef",
+FindingActionTypeDef = TypedDict(
+    "FindingActionTypeDef",
     {
-        "regex": str,
-        "s3WordsList": S3WordsListOutputTypeDef,
+        "actionType": Literal["AWS_API_CALL"],
+        "apiCallDetails": ApiCallDetailsTypeDef,
     },
     total=False,
 )
 
-AllowListCriteriaTypeDef = TypedDict(
-    "AllowListCriteriaTypeDef",
+BatchGetCustomDataIdentifiersResponseTypeDef = TypedDict(
+    "BatchGetCustomDataIdentifiersResponseTypeDef",
     {
-        "regex": str,
-        "s3WordsList": S3WordsListTypeDef,
+        "customDataIdentifiers": List[BatchGetCustomDataIdentifierSummaryTypeDef],
+        "notFoundIdentifierIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAllowListResponseTypeDef = TypedDict(
+    "CreateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateClassificationJobResponseTypeDef = TypedDict(
+    "CreateClassificationJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDataIdentifierResponseTypeDef = TypedDict(
+    "CreateCustomDataIdentifierResponseTypeDef",
+    {
+        "customDataIdentifierId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsFilterResponseTypeDef = TypedDict(
+    "CreateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberResponseTypeDef = TypedDict(
+    "CreateMemberResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "autoEnable": bool,
+        "maxAccountLimitReached": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    {
+        "classificationScopeId": str,
+        "disabledAt": datetime,
+        "firstEnabledAt": datetime,
+        "lastUpdatedAt": datetime,
+        "sensitivityInspectionTemplateId": str,
+        "status": AutomatedDiscoveryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "invitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMacieSessionResponseTypeDef = TypedDict(
+    "GetMacieSessionResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "findingPublishingFrequency": FindingPublishingFrequencyType,
+        "serviceRole": str,
+        "status": MacieStatusType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMemberResponseTypeDef = TypedDict(
+    "GetMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "administratorAccountId": str,
+        "arn": str,
+        "email": str,
+        "invitedAt": datetime,
+        "masterAccountId": str,
+        "relationshipStatus": RelationshipStatusType,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    {
+        "code": AvailabilityCodeType,
+        "reasons": List[UnavailabilityReasonCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListAllowListsResponseTypeDef = TypedDict(
     "ListAllowListsResponseTypeDef",
     {
         "allowLists": List[AllowListSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FindingActionTypeDef = TypedDict(
-    "FindingActionTypeDef",
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
     {
-        "actionType": Literal["AWS_API_CALL"],
-        "apiCallDetails": ApiCallDetailsTypeDef,
+        "findingIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchGetCustomDataIdentifiersResponseTypeDef = TypedDict(
-    "BatchGetCustomDataIdentifiersResponseTypeDef",
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
     {
-        "customDataIdentifiers": List[BatchGetCustomDataIdentifierSummaryTypeDef],
-        "notFoundIdentifierIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "adminAccounts": List[AdminAccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestCustomDataIdentifierResponseTypeDef = TypedDict(
+    "TestCustomDataIdentifierResponseTypeDef",
+    {
+        "matchCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAllowListResponseTypeDef = TypedDict(
+    "UpdateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFindingsFilterResponseTypeDef = TypedDict(
+    "UpdateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "accessControlList": AccessControlListTypeDef,
@@ -2290,24 +2055,14 @@
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
     },
     total=False,
 )
 
-DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
-    {
-        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
-        "sortCriteria": BucketSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeBucketsRequestRequestTypeDef = TypedDict(
     "DescribeBucketsRequestRequestTypeDef",
     {
         "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
         "maxResults": int,
         "nextToken": str,
         "sortCriteria": BucketSortCriteriaTypeDef,
@@ -2322,36 +2077,28 @@
         "notClassified": SensitivityAggregationsTypeDef,
         "notSensitive": SensitivityAggregationsTypeDef,
         "sensitive": SensitivityAggregationsTypeDef,
     },
     total=False,
 )
 
-ClassificationExportConfigurationOutputTypeDef = TypedDict(
-    "ClassificationExportConfigurationOutputTypeDef",
-    {
-        "s3Destination": S3DestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 ClassificationExportConfigurationTypeDef = TypedDict(
     "ClassificationExportConfigurationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
 
 ListClassificationScopesResponseTypeDef = TypedDict(
     "ListClassificationScopesResponseTypeDef",
     {
         "classificationScopes": List[ClassificationScopeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDataIdentifierRequestRequestTypeDef",
     {
         "name": str,
@@ -2374,35 +2121,54 @@
 
 class CreateCustomDataIdentifierRequestRequestTypeDef(
     _RequiredCreateCustomDataIdentifierRequestRequestTypeDef,
     _OptionalCreateCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
+GetCustomDataIdentifierResponseTypeDef = TypedDict(
+    "GetCustomDataIdentifierResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deleted": bool,
+        "description": str,
+        "id": str,
+        "ignoreWords": List[str],
+        "keywords": List[str],
+        "maximumMatchDistance": int,
+        "name": str,
+        "regex": str,
+        "severityLevels": List[SeverityLevelTypeDef],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateInvitationsResponseTypeDef = TypedDict(
     "CreateInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingCriteriaOutputTypeDef = TypedDict(
     "FindingCriteriaOutputTypeDef",
     {
         "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
@@ -2419,104 +2185,222 @@
 )
 
 ListCustomDataIdentifiersResponseTypeDef = TypedDict(
     "ListCustomDataIdentifiersResponseTypeDef",
     {
         "items": List[CustomDataIdentifierSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    {
+        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
+        "sortCriteria": BucketSortCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    {
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
+    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "resourceArn": str,
+        },
+    )
+)
+_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
+    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+):
+    pass
+
+ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 GetSensitiveDataOccurrencesResponseTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesResponseTypeDef",
     {
         "error": str,
         "sensitiveDataOccurrences": Dict[str, List[DetectedDataDetailsTypeDef]],
         "status": RevealRequestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceProfileDetectionsResponseTypeDef = TypedDict(
     "ListResourceProfileDetectionsResponseTypeDef",
     {
         "detections": List[DetectionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsFiltersResponseTypeDef = TypedDict(
     "ListFindingsFiltersResponseTypeDef",
     {
         "findingsFilterListItems": List[FindingsFilterListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "administrator": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "master": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "invitations": List[InvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCustomDataIdentifierResponseTypeDef = TypedDict(
-    "GetCustomDataIdentifierResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "deleted": bool,
-        "description": str,
-        "id": str,
-        "ignoreWords": List[str],
-        "keywords": List[str],
-        "maximumMatchDistance": int,
-        "name": str,
-        "regex": str,
-        "severityLevels": List[SeverityLevelOutputTypeDef],
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingStatisticsResponseTypeDef = TypedDict(
     "GetFindingStatisticsResponseTypeDef",
     {
         "countsByGroup": List[GroupCountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsPublicationConfigurationResponseTypeDef = TypedDict(
     "GetFindingsPublicationConfigurationResponseTypeDef",
     {
-        "securityHubConfiguration": SecurityHubConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "findingIds": Sequence[str],
     },
@@ -2537,31 +2421,38 @@
 GetResourceProfileResponseTypeDef = TypedDict(
     "GetResourceProfileResponseTypeDef",
     {
         "profileUpdatedAt": datetime,
         "sensitivityScore": int,
         "sensitivityScoreOverridden": bool,
         "statistics": ResourceStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRevealConfigurationResponseTypeDef = TypedDict(
     "GetRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": RevealConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateRevealConfigurationRequestRequestTypeDef",
+    {
+        "configuration": RevealConfigurationTypeDef,
     },
 )
 
 UpdateRevealConfigurationResponseTypeDef = TypedDict(
     "UpdateRevealConfigurationResponseTypeDef",
     {
-        "configuration": RevealConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": RevealConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef = TypedDict(
     "_RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     {
         "findingId": str,
@@ -2585,25 +2476,25 @@
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
         "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
         "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "GetUsageStatisticsRequestRequestTypeDef",
     {
@@ -2617,15 +2508,15 @@
 )
 
 GetUsageTotalsResponseTypeDef = TypedDict(
     "GetUsageTotalsResponseTypeDef",
     {
         "timeRange": TimeRangeType,
         "usageTotals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IpAddressDetailsTypeDef = TypedDict(
     "IpAddressDetailsTypeDef",
     {
         "ipAddressV4": str,
@@ -2637,16 +2528,16 @@
     total=False,
 )
 
 JobScheduleFrequencyOutputTypeDef = TypedDict(
     "JobScheduleFrequencyOutputTypeDef",
     {
         "dailySchedule": Dict[str, Any],
-        "monthlySchedule": MonthlyScheduleOutputTypeDef,
-        "weeklySchedule": WeeklyScheduleOutputTypeDef,
+        "monthlySchedule": MonthlyScheduleTypeDef,
+        "weeklySchedule": WeeklyScheduleTypeDef,
     },
     total=False,
 )
 
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
@@ -2667,71 +2558,55 @@
 )
 
 ListManagedDataIdentifiersResponseTypeDef = TypedDict(
     "ListManagedDataIdentifiersResponseTypeDef",
     {
         "items": List[ManagedDataIdentifierSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceProfileArtifactsResponseTypeDef = TypedDict(
     "ListResourceProfileArtifactsResponseTypeDef",
     {
         "artifacts": List[ResourceProfileArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSensitivityInspectionTemplatesResponseTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "sensitivityInspectionTemplates": List[SensitivityInspectionTemplatesEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "lineRange": RangeTypeDef,
         "offsetRange": RangeTypeDef,
         "pageNumber": int,
     },
     total=False,
 )
 
-PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutFindingsPublicationConfigurationRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "securityHubConfiguration": SecurityHubConfigurationTypeDef,
-    },
-    total=False,
-)
-
-UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateRevealConfigurationRequestRequestTypeDef",
-    {
-        "configuration": RevealConfigurationTypeDef,
-    },
-)
-
 S3ObjectTypeDef = TypedDict(
     "S3ObjectTypeDef",
     {
         "bucketArn": str,
         "eTag": str,
         "extension": str,
         "key": str,
@@ -2832,15 +2707,15 @@
 ):
     pass
 
 TagCriterionForJobOutputTypeDef = TypedDict(
     "TagCriterionForJobOutputTypeDef",
     {
         "comparator": JobComparatorType,
-        "tagValues": List[TagCriterionPairForJobOutputTypeDef],
+        "tagValues": List[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
@@ -2851,15 +2726,15 @@
 )
 
 TagScopeTermOutputTypeDef = TypedDict(
     "TagScopeTermOutputTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
-        "tagValues": List[TagValuePairOutputTypeDef],
+        "tagValues": List[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
     },
     total=False,
 )
 
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
@@ -2868,30 +2743,14 @@
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
     },
     total=False,
 )
 
-GetAllowListResponseTypeDef = TypedDict(
-    "GetAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": AllowListCriteriaOutputTypeDef,
-        "description": str,
-        "id": str,
-        "name": str,
-        "status": AllowListStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAllowListRequestRequestTypeDef",
     {
         "clientToken": str,
         "criteria": AllowListCriteriaTypeDef,
         "name": str,
     },
@@ -2906,14 +2765,30 @@
 )
 
 class CreateAllowListRequestRequestTypeDef(
     _RequiredCreateAllowListRequestRequestTypeDef, _OptionalCreateAllowListRequestRequestTypeDef
 ):
     pass
 
+GetAllowListResponseTypeDef = TypedDict(
+    "GetAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": AllowListCriteriaTypeDef,
+        "description": str,
+        "id": str,
+        "name": str,
+        "status": AllowListStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAllowListRequestRequestTypeDef",
     {
         "criteria": AllowListCriteriaTypeDef,
         "id": str,
         "name": str,
     },
@@ -2963,53 +2838,53 @@
         "classifiableSizeInBytes": int,
         "lastUpdated": datetime,
         "objectCount": int,
         "sizeInBytes": int,
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClassificationExportConfigurationResponseTypeDef = TypedDict(
     "GetClassificationExportConfigurationResponseTypeDef",
     {
-        "configuration": ClassificationExportConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": ClassificationExportConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutClassificationExportConfigurationResponseTypeDef = TypedDict(
-    "PutClassificationExportConfigurationResponseTypeDef",
+PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
+    "PutClassificationExportConfigurationRequestRequestTypeDef",
     {
-        "configuration": ClassificationExportConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": ClassificationExportConfigurationTypeDef,
     },
 )
 
-PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
-    "PutClassificationExportConfigurationRequestRequestTypeDef",
+PutClassificationExportConfigurationResponseTypeDef = TypedDict(
+    "PutClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsFilterResponseTypeDef = TypedDict(
     "GetFindingsFilterResponseTypeDef",
     {
         "action": FindingsFilterActionType,
         "arn": str,
         "description": str,
         "findingCriteria": FindingCriteriaOutputTypeDef,
         "id": str,
         "name": str,
         "position": int,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
         "action": FindingsFilterActionType,
@@ -3057,15 +2932,15 @@
     pass
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -3103,15 +2978,15 @@
     pass
 
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListClassificationJobsRequestRequestTypeDef",
     {
@@ -3137,15 +3012,15 @@
 
 GetClassificationScopeResponseTypeDef = TypedDict(
     "GetClassificationScopeResponseTypeDef",
     {
         "id": str,
         "name": str,
         "s3": S3ClassificationScopeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateClassificationScopeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClassificationScopeRequestRequestTypeDef",
     {
         "id": str,
@@ -3255,15 +3130,15 @@
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "matchingResources": List[MatchingResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDetectionTypeDef = TypedDict(
     "CustomDetectionTypeDef",
     {
         "arn": str,
@@ -3294,15 +3169,15 @@
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "nextToken": str,
         "records": List[UsageRecordTypeDef],
         "timeRange": TimeRangeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "assumedRole": AssumedRoleTypeDef,
@@ -3471,15 +3346,15 @@
 )
 
 DescribeBucketsResponseTypeDef = TypedDict(
     "DescribeBucketsResponseTypeDef",
     {
         "buckets": List[BucketMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourcesAffectedTypeDef = TypedDict(
     "ResourcesAffectedTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
@@ -3513,15 +3388,15 @@
 )
 
 SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     {
         "bucketCriteria": SearchResourcesBucketCriteriaTypeDef,
         "sortCriteria": SearchResourcesSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 PolicyDetailsTypeDef = TypedDict(
     "PolicyDetailsTypeDef",
     {
@@ -3580,15 +3455,15 @@
 )
 
 ListClassificationJobsResponseTypeDef = TypedDict(
     "ListClassificationJobsResponseTypeDef",
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClassificationJobResponseTypeDef = TypedDict(
     "DescribeClassificationJobResponseTypeDef",
     {
         "allowListIds": List[str],
@@ -3608,15 +3483,15 @@
         "name": str,
         "s3JobDefinition": S3JobDefinitionOutputTypeDef,
         "samplingPercentage": int,
         "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
         "statistics": StatisticsTypeDef,
         "tags": Dict[str, str],
         "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -3672,10 +3547,10 @@
     total=False,
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.py` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2/waiter.pyi` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/PKG-INFO` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-macie2
-Version: 1.28.12
-Summary: Type annotations for boto3.Macie2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Macie2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-macie2.svg?color=blue)](https://pypi.org/project/mypy-boto3-macie2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-macie2)](https://pepy.tech/project/mypy-boto3-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Macie2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[boto3.Macie2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-macie2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -467,23 +467,23 @@
 ```python
 from mypy_boto3_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
     AdminAccountTypeDef,
-    S3WordsListOutputTypeDef,
     S3WordsListTypeDef,
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
     BatchGetCustomDataIdentifiersRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BucketCountByEffectivePermissionTypeDef,
     BucketCountByEncryptionTypeTypeDef,
     BucketCountBySharedAccessTypeTypeDef,
     BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef,
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketPolicyTypeDef,
     BucketServerSideEncryptionTypeDef,
@@ -491,197 +491,188 @@
     KeyValuePairTypeDef,
     ObjectCountByEncryptionTypeTypeDef,
     ObjectLevelStatisticsTypeDef,
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
-    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
-    CreateAllowListResponseTypeDef,
-    CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
-    CreateCustomDataIdentifierResponseTypeDef,
-    CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
-    CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
     CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMemberRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClassificationJobRequestRequestTypeDef,
     LastRunErrorStatusTypeDef,
     StatisticsTypeDef,
     UserPausedDetailsTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DetectedDataDetailsTypeDef,
     DetectionTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DomainDetailsTypeDef,
     EnableMacieRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     SeverityTypeDef,
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
-    GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
-    SeverityLevelOutputTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
-    SecurityHubConfigurationOutputTypeDef,
+    SecurityHubConfigurationTypeDef,
     SortCriteriaTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
-    GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
-    RevealConfigurationOutputTypeDef,
+    RevealConfigurationTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
-    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
     SensitivityInspectionTemplateExcludesOutputTypeDef,
     SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
-    MonthlyScheduleOutputTypeDef,
-    WeeklyScheduleOutputTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
     SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
     S3BucketDefinitionForJobOutputTypeDef,
-    ListAllowListsRequestListAllowListsPaginateTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
-    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
-    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
-    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
     ListFindingsFiltersRequestRequestTypeDef,
-    ListFindingsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListJobsFilterTermTypeDef,
-    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
     ListManagedDataIdentifiersRequestRequestTypeDef,
     ManagedDataIdentifierSummaryTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
     ListResourceProfileArtifactsRequestRequestTypeDef,
     ResourceProfileArtifactTypeDef,
-    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
     ListResourceProfileDetectionsRequestRequestTypeDef,
-    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
-    SecurityHubConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    RevealConfigurationTypeDef,
     S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
     SensitivityInspectionTemplateExcludesTypeDef,
     SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
-    TagCriterionPairForJobOutputTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagValuePairOutputTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
-    TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
-    UpdateFindingsFilterResponseTypeDef,
     UpdateMacieSessionRequestRequestTypeDef,
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    AllowListCriteriaOutputTypeDef,
     AllowListCriteriaTypeDef,
-    ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
+    CreateAllowListResponseTypeDef,
+    CreateClassificationJobResponseTypeDef,
+    CreateCustomDataIdentifierResponseTypeDef,
+    CreateFindingsFilterResponseTypeDef,
+    CreateMemberResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    GetAutomatedDiscoveryConfigurationResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetMacieSessionResponseTypeDef,
+    GetMemberResponseTypeDef,
+    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
+    ListAllowListsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TestCustomDataIdentifierResponseTypeDef,
+    UpdateAllowListResponseTypeDef,
+    UpdateFindingsFilterResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
-    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
-    ClassificationExportConfigurationOutputTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
+    GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
+    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
+    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
+    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
+    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
-    GetCustomDataIdentifierResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
     GetFindingsPublicationConfigurationResponseTypeDef,
+    PutFindingsPublicationConfigurationRequestRequestTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
+    UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
@@ -689,37 +680,35 @@
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
-    PutFindingsPublicationConfigurationRequestRequestTypeDef,
-    UpdateRevealConfigurationRequestRequestTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
     UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
     TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
     TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
-    GetAllowListResponseTypeDef,
     CreateAllowListRequestRequestTypeDef,
+    GetAllowListResponseTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
-    PutClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
+    PutClassificationExportConfigurationResponseTypeDef,
     GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
```

### Comparing `mypy-boto3-macie2-1.28.12/mypy_boto3_macie2.egg-info/SOURCES.txt` & `mypy-boto3-macie2-1.28.15/mypy_boto3_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-macie2-1.28.12/setup.py` & `mypy-boto3-macie2-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-macie2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Macie2 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Macie2 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

