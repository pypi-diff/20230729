# Comparing `tmp/mypy-boto3-devops-guru-1.28.15.tar.gz` & `tmp/mypy-boto3-devops-guru-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devops-guru-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
+gzip compressed data, was "mypy-boto3-devops-guru-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
```

## Comparing `mypy-boto3-devops-guru-1.28.15.tar` & `mypy-boto3-devops-guru-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.976961 mypy-boto3-devops-guru-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-07-28 20:42:37.972960 mypy-boto3-devops-guru-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.968960 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-28 20:22:53.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-28 20:22:52.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64825 2023-07-28 20:22:55.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64758 2023-07-28 20:22:54.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.972960 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23366 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:37.000000 mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.976961 mypy-boto3-devops-guru-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-28 20:22:51.000000 mypy-boto3-devops-guru-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.885101 mypy-boto3-devops-guru-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23372 2023-07-29 10:02:55.877101 mypy-boto3-devops-guru-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.877101 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31416 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31364 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64825 2023-07-29 09:42:22.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64758 2023-07-29 09:42:21.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:20.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.877101 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23372 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:02:55.000000 mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.885101 mypy-boto3-devops-guru-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-29 09:42:18.000000 mypy-boto3-devops-guru-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-devops-guru-1.28.15/LICENSE` & `mypy-boto3-devops-guru-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/PKG-INFO` & `mypy-boto3-devops-guru-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.15
-Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devops-guru-1.28.15/README.md` & `mypy-boto3-devops-guru-1.28.15.post1/README.md`

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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.py` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/__init__.pyi` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.py` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
@@ -68,14 +69,15 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
     UpdateResourceCollectionFilterTypeDef,
@@ -124,15 +126,17 @@
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#exceptions)
         """
 
     def add_notification_channel(
-        self, *, Config: NotificationChannelConfigTypeDef
+        self,
+        *,
+        Config: Union[NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef]
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#add_notification_channel)
         """
@@ -477,15 +481,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#search_organization_insights)
         """
 
     def start_cost_estimation(
         self,
         *,
-        ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
+        ResourceCollection: Union[
+            CostEstimationResourceCollectionFilterTypeDef,
+            CostEstimationResourceCollectionFilterOutputTypeDef,
+        ],
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/client.pyi` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
@@ -68,14 +69,15 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
     UpdateResourceCollectionFilterTypeDef,
@@ -119,15 +121,17 @@
         """
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#exceptions)
         """
     def add_notification_channel(
-        self, *, Config: NotificationChannelConfigTypeDef
+        self,
+        *,
+        Config: Union[NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef]
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#add_notification_channel)
         """
@@ -442,15 +446,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/client/#search_organization_insights)
         """
     def start_cost_estimation(
         self,
         *,
-        ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
+        ResourceCollection: Union[
+            CostEstimationResourceCollectionFilterTypeDef,
+            CostEstimationResourceCollectionFilterOutputTypeDef,
+        ],
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.py` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/literals.pyi` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.py` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/paginator.pyi` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.py` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru/type_defs.pyi` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/PKG-INFO` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.28.15
-Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
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
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devops-guru-1.28.15/mypy_boto3_devops_guru.egg-info/SOURCES.txt` & `mypy-boto3-devops-guru-1.28.15.post1/mypy_boto3_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.28.15/setup.py` & `mypy-boto3-devops-guru-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devops-guru",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DevOpsGuru 1.28.15 service generated with mypy-boto3-builder"
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

