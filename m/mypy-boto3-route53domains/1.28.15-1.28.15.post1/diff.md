# Comparing `tmp/mypy-boto3-route53domains-1.28.15.tar.gz` & `tmp/mypy-boto3-route53domains-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53domains-1.28.15.tar", last modified: Fri Jul 28 20:43:37 2023, max compression
+gzip compressed data, was "mypy-boto3-route53domains-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:03 2023, max compression
```

## Comparing `mypy-boto3-route53domains-1.28.15.tar` & `mypy-boto3-route53domains-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28505 2023-07-28 20:37:20.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28482 2023-07-28 20:37:20.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:03.149372 mypy-boto3-route53domains-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-29 10:04:03.141372 mypy-boto3-route53domains-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:03.129372 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29405 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29360 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28569 2023-07-29 09:57:25.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28546 2023-07-29 09:57:25.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:03.141372 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:03.149372 mypy-boto3-route53domains-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-route53domains-1.28.15/LICENSE` & `mypy-boto3-route53domains-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/PKG-INFO` & `mypy-boto3-route53domains-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.15
-Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53domains-1.28.15/README.md` & `mypy-boto3-route53domains-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.py` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.pyi` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.py` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
@@ -45,14 +46,15 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
+    NameserverOutputTypeDef,
     NameserverTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
@@ -368,17 +370,17 @@
         """
 
     def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
@@ -441,19 +443,19 @@
         """
 
     def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
         IdnLangCode: str = ...,
-        Nameservers: Sequence[NameserverTypeDef] = ...,
+        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
@@ -474,17 +476,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#transfer_domain_to_another_aws_account)
         """
 
     def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: ContactDetailTypeDef = ...,
-        RegistrantContact: ContactDetailTypeDef = ...,
-        TechContact: ContactDetailTypeDef = ...,
+        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
+        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
+        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact)
@@ -502,15 +504,19 @@
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact_privacy)
         """
 
     def update_domain_nameservers(
-        self, *, DomainName: str, Nameservers: Sequence[NameserverTypeDef], FIAuthKey: str = ...
+        self,
+        *,
+        DomainName: str,
+        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
+        FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_nameservers)
```

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.pyi` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
@@ -45,14 +46,15 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
+    NameserverOutputTypeDef,
     NameserverTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
@@ -339,17 +341,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#push_domain)
         """
     def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
@@ -406,19 +408,19 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#retrieve_domain_auth_code)
         """
     def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailTypeDef,
-        RegistrantContact: ContactDetailTypeDef,
-        TechContact: ContactDetailTypeDef,
+        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
         IdnLangCode: str = ...,
-        Nameservers: Sequence[NameserverTypeDef] = ...,
+        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
@@ -437,17 +439,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain_to_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#transfer_domain_to_another_aws_account)
         """
     def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: ContactDetailTypeDef = ...,
-        RegistrantContact: ContactDetailTypeDef = ...,
-        TechContact: ContactDetailTypeDef = ...,
+        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
+        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
+        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact)
@@ -463,15 +465,19 @@
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact_privacy)
         """
     def update_domain_nameservers(
-        self, *, DomainName: str, Nameservers: Sequence[NameserverTypeDef], FIAuthKey: str = ...
+        self,
+        *,
+        DomainName: str,
+        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
+        FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_nameservers)
```

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.py` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.pyi` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.py` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.pyi` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.py` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -959,15 +959,15 @@
     pass
 
 
 _RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
     },
 )
 _OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
         "FIAuthKey": str,
     },
@@ -1050,15 +1050,15 @@
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
```

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.pyi` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -944,15 +944,15 @@
 ):
     pass
 
 _RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
     },
 )
 _OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
         "FIAuthKey": str,
     },
@@ -1031,15 +1031,15 @@
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
```

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/PKG-INFO` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.15
-Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/SOURCES.txt` & `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15/setup.py` & `mypy-boto3-route53domains-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53domains",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Route53Domains 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

