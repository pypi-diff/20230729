# Comparing `tmp/mypy-boto3-ssm-contacts-1.28.15.tar.gz` & `tmp/mypy-boto3-ssm-contacts-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.15.tar", last modified: Fri Jul 28 20:43:48 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
```

## Comparing `mypy-boto3-ssm-contacts-1.28.15.tar` & `mypy-boto3-ssm-contacts-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.313927 mypy-boto3-ssm-contacts-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-28 20:43:48.301927 mypy-boto3-ssm-contacts-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.301927 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40555 2023-07-28 20:40:04.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-28 20:40:04.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.301927 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:48.313927 mypy-boto3-ssm-contacts-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.013419 mypy-boto3-ssm-contacts-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-29 10:04:16.005419 mypy-boto3-ssm-contacts-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.997419 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32497 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32440 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-29 10:00:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-29 10:00:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40555 2023-07-29 10:00:16.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-29 10:00:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.005419 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:04:15.000000 mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.013419 mypy-boto3-ssm-contacts-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 10:00:14.000000 mypy-boto3-ssm-contacts-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/LICENSE` & `mypy-boto3-ssm-contacts-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.15
-Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/README.md` & `mypy-boto3-ssm-contacts-1.28.15.post1/README.md`

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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.pyi` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__main__.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMContacts 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.SSMContacts 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,18 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
     PreviewOverrideTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -156,15 +158,15 @@
         """
 
     def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: PlanTypeDef,
+        Plan: Union[PlanTypeDef, PlanOutputTypeDef],
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
@@ -194,15 +196,15 @@
 
     def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         StartTime: Union[datetime, str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
@@ -426,15 +428,15 @@
 
     def list_preview_rotation_shifts(
         self,
         *,
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
@@ -551,15 +553,19 @@
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#untag_resource)
         """
 
     def update_contact(
-        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanTypeDef = ...
+        self,
+        *,
+        ContactId: str,
+        DisplayName: str = ...,
+        Plan: Union[PlanTypeDef, PlanOutputTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact)
         """
@@ -578,15 +584,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact_channel)
         """
 
     def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         ContactIds: Sequence[str] = ...,
         StartTime: Union[datetime, str] = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.pyi` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,18 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
     PreviewOverrideTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -147,15 +149,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#close)
         """
     def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: PlanTypeDef,
+        Plan: Union[PlanTypeDef, PlanOutputTypeDef],
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
@@ -183,15 +185,15 @@
         """
     def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         StartTime: Union[datetime, str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
@@ -393,15 +395,15 @@
         """
     def list_preview_rotation_shifts(
         self,
         *,
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
@@ -507,15 +509,19 @@
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#untag_resource)
         """
     def update_contact(
-        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanTypeDef = ...
+        self,
+        *,
+        ContactId: str,
+        DisplayName: str = ...,
+        Plan: Union[PlanTypeDef, PlanOutputTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact)
         """
@@ -532,15 +538,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/client/#update_contact_channel)
         """
     def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         ContactIds: Sequence[str] = ...,
         StartTime: Union[datetime, str] = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.pyi` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     TimeRangeTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
@@ -209,15 +210,15 @@
 
     def paginate(
         self,
         *,
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.pyi` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     TimeRangeTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
@@ -199,15 +200,15 @@
 
     def paginate(
         self,
         *,
         EndTime: Union[datetime, str],
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef],
         RotationStartTime: Union[datetime, str] = ...,
         StartTime: Union[datetime, str] = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.pyi` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.15
-Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt` & `mypy-boto3-ssm-contacts-1.28.15.post1/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.15/setup.py` & `mypy-boto3-ssm-contacts-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-contacts",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder"
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

