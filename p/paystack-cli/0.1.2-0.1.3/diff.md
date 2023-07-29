# Comparing `tmp/paystack_cli-0.1.2.tar.gz` & `tmp/paystack_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystack_cli-0.1.2.tar", max compression
+gzip compressed data, was "paystack_cli-0.1.3.tar", max compression
```

## Comparing `paystack_cli-0.1.2.tar` & `paystack_cli-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2023-07-24 20:00:11.419052 paystack_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0      919 2023-07-26 19:27:04.037005 paystack_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-19 21:04:35.944414 paystack_cli-0.1.2/paystack_cli/__init__.py
--rw-r--r--   0        0        0     1104 2023-07-24 16:58:10.490171 paystack_cli-0.1.2/paystack_cli/apple_pay.py
--rw-r--r--   0        0        0     3072 2023-07-24 17:35:10.884307 paystack_cli-0.1.2/paystack_cli/bulk_charges.py
--rw-r--r--   0        0        0     3586 2023-07-24 17:35:10.894307 paystack_cli-0.1.2/paystack_cli/charge.py
--rw-r--r--   0        0        0     3729 2023-07-24 17:35:10.924306 paystack_cli-0.1.2/paystack_cli/customers.py
--rw-r--r--   0        0        0     3746 2023-07-24 17:35:10.917640 paystack_cli-0.1.2/paystack_cli/dedicated_virtual_accounts.py
--rw-r--r--   0        0        0     3713 2023-07-24 17:40:00.337132 paystack_cli-0.1.2/paystack_cli/disputes.py
--rw-r--r--   0        0        0      710 2023-07-24 17:42:15.102544 paystack_cli-0.1.2/paystack_cli/integration.py
--rw-r--r--   0        0        0     7133 2023-07-26 19:05:49.756266 paystack_cli-0.1.2/paystack_cli/main.py
--rw-r--r--   0        0        0     1789 2023-07-26 19:05:04.664592 paystack_cli-0.1.2/paystack_cli/miscellaneous.py
--rw-r--r--   0        0        0     2795 2023-07-24 17:51:59.045863 paystack_cli-0.1.2/paystack_cli/payment_pages.py
--rw-r--r--   0        0        0     4479 2023-07-24 17:57:32.464325 paystack_cli-0.1.2/paystack_cli/payments_requests.py
--rw-r--r--   0        0        0     2093 2023-07-24 18:00:45.079200 paystack_cli-0.1.2/paystack_cli/plans.py
--rw-r--r--   0        0        0     1920 2023-07-24 18:04:03.576117 paystack_cli-0.1.2/paystack_cli/products.py
--rw-r--r--   0        0        0     1564 2023-07-24 18:06:12.699501 paystack_cli-0.1.2/paystack_cli/refunds.py
--rw-r--r--   0        0        0     1231 2023-07-24 18:09:03.792597 paystack_cli-0.1.2/paystack_cli/settlements.py
--rw-r--r--   0        0        0     3306 2023-07-24 18:12:46.875562 paystack_cli-0.1.2/paystack_cli/subaccounts.py
--rw-r--r--   0        0        0     2384 2023-07-24 18:16:37.889155 paystack_cli-0.1.2/paystack_cli/subscriptions.py
--rw-r--r--   0        0        0     2945 2023-07-24 18:28:41.008662 paystack_cli-0.1.2/paystack_cli/terminals.py
--rw-r--r--   0        0        0     5845 2023-07-24 18:32:52.056579 paystack_cli-0.1.2/paystack_cli/transactions.py
--rw-r--r--   0        0        0     2892 2023-07-24 18:36:11.984984 paystack_cli-0.1.2/paystack_cli/transactions_splits.py
--rw-r--r--   0        0        0     3150 2023-07-24 18:40:01.466531 paystack_cli-0.1.2/paystack_cli/transfer_recipients.py
--rw-r--r--   0        0        0     2447 2023-07-24 18:43:01.438487 paystack_cli-0.1.2/paystack_cli/transfers.py
--rw-r--r--   0        0        0     2044 2023-07-26 18:59:23.008137 paystack_cli-0.1.2/paystack_cli/transfers_control.py
--rw-r--r--   0        0        0     3426 2023-07-23 09:12:38.123328 paystack_cli-0.1.2/paystack_cli/utils.py
--rw-r--r--   0        0        0     1552 2023-07-24 18:51:27.954669 paystack_cli-0.1.2/paystack_cli/verification.py
--rw-r--r--   0        0        0      819 2023-07-26 18:38:21.191715 paystack_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 paystack_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-24 20:00:11.419052 paystack_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0      919 2023-07-29 17:11:02.663843 paystack_cli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 21:04:35.944414 paystack_cli-0.1.3/paystack_cli/__init__.py
+-rw-r--r--   0        0        0     1104 2023-07-27 09:42:56.394895 paystack_cli-0.1.3/paystack_cli/apple_pay.py
+-rw-r--r--   0        0        0     3072 2023-07-24 17:35:10.884307 paystack_cli-0.1.3/paystack_cli/bulk_charges.py
+-rw-r--r--   0        0        0     3586 2023-07-24 17:35:10.894307 paystack_cli-0.1.3/paystack_cli/charge.py
+-rw-r--r--   0        0        0     3729 2023-07-24 17:35:10.924306 paystack_cli-0.1.3/paystack_cli/customers.py
+-rw-r--r--   0        0        0     3746 2023-07-24 17:35:10.917640 paystack_cli-0.1.3/paystack_cli/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     3713 2023-07-24 17:40:00.337132 paystack_cli-0.1.3/paystack_cli/disputes.py
+-rw-r--r--   0        0        0      710 2023-07-24 17:42:15.102544 paystack_cli-0.1.3/paystack_cli/integration.py
+-rw-r--r--   0        0        0     7133 2023-07-29 16:51:13.413196 paystack_cli-0.1.3/paystack_cli/main.py
+-rw-r--r--   0        0        0     1789 2023-07-26 19:05:04.664592 paystack_cli-0.1.3/paystack_cli/miscellaneous.py
+-rw-r--r--   0        0        0     2795 2023-07-24 17:51:59.045863 paystack_cli-0.1.3/paystack_cli/payment_pages.py
+-rw-r--r--   0        0        0     4479 2023-07-24 17:57:32.464325 paystack_cli-0.1.3/paystack_cli/payments_requests.py
+-rw-r--r--   0        0        0     2093 2023-07-24 18:00:45.079200 paystack_cli-0.1.3/paystack_cli/plans.py
+-rw-r--r--   0        0        0     1920 2023-07-24 18:04:03.576117 paystack_cli-0.1.3/paystack_cli/products.py
+-rw-r--r--   0        0        0     1564 2023-07-24 18:06:12.699501 paystack_cli-0.1.3/paystack_cli/refunds.py
+-rw-r--r--   0        0        0     1231 2023-07-24 18:09:03.792597 paystack_cli-0.1.3/paystack_cli/settlements.py
+-rw-r--r--   0        0        0     3306 2023-07-24 18:12:46.875562 paystack_cli-0.1.3/paystack_cli/subaccounts.py
+-rw-r--r--   0        0        0     2384 2023-07-24 18:16:37.889155 paystack_cli-0.1.3/paystack_cli/subscriptions.py
+-rw-r--r--   0        0        0     2945 2023-07-24 18:28:41.008662 paystack_cli-0.1.3/paystack_cli/terminals.py
+-rw-r--r--   0        0        0     5845 2023-07-24 18:32:52.056579 paystack_cli-0.1.3/paystack_cli/transactions.py
+-rw-r--r--   0        0        0     2892 2023-07-24 18:36:11.984984 paystack_cli-0.1.3/paystack_cli/transactions_splits.py
+-rw-r--r--   0        0        0     3150 2023-07-24 18:40:01.466531 paystack_cli-0.1.3/paystack_cli/transfer_recipients.py
+-rw-r--r--   0        0        0     2447 2023-07-24 18:43:01.438487 paystack_cli-0.1.3/paystack_cli/transfers.py
+-rw-r--r--   0        0        0     2044 2023-07-26 18:59:23.008137 paystack_cli-0.1.3/paystack_cli/transfers_control.py
+-rw-r--r--   0        0        0     3426 2023-07-23 09:12:38.123328 paystack_cli-0.1.3/paystack_cli/utils.py
+-rw-r--r--   0        0        0     1552 2023-07-24 18:51:27.954669 paystack_cli-0.1.3/paystack_cli/verification.py
+-rw-r--r--   0        0        0      819 2023-07-29 16:51:13.429863 paystack_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 paystack_cli-0.1.3/PKG-INFO
```

### Comparing `paystack_cli-0.1.2/LICENSE` & `paystack_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/README.md` & `paystack_cli-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # paystack cli
 A command line app for interacting with [Paystack's](https://paystack.com/) API. Built with
 [Typer](https://typer.tiangolo.com/) and [Pypaystack2](https://gray-adeyi.github.io/pypaystack2/)
 
 ![utility in use](./paystack-cli.png)
 
 ## Installation
-Binaries of paystack cli be found [here](https://github.com/gray-adeyi/paystack-cli/releases/tag/0.1.2). Alternatively, Paystack cli can be installed from pypi
+Binaries of paystack cli be found [here](https://github.com/gray-adeyi/paystack-cli/releases/tag/0.1.3). Alternatively, Paystack cli can be installed from pypi
 with pip as shown below.
 ```bash
 pip install paystack-cli
 ```
 
 ## First time configurations
 You're required to add your paystack auth_key on first use as shown below
```

### Comparing `paystack_cli-0.1.2/paystack_cli/apple_pay.py` & `paystack_cli-0.1.3/paystack_cli/apple_pay.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/bulk_charges.py` & `paystack_cli-0.1.3/paystack_cli/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/charge.py` & `paystack_cli-0.1.3/paystack_cli/charge.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/customers.py` & `paystack_cli-0.1.3/paystack_cli/customers.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/dedicated_virtual_accounts.py` & `paystack_cli-0.1.3/paystack_cli/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/disputes.py` & `paystack_cli-0.1.3/paystack_cli/disputes.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/integration.py` & `paystack_cli-0.1.3/paystack_cli/integration.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/main.py` & `paystack_cli-0.1.3/paystack_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     reset_settings()
     rprint("auth key cleared! :boom:")
 
 
 @app.command()
 def version():
     """See CLI version"""
-    rprint("Paystack CLI Version 0.1.2")
+    rprint("Paystack CLI Version 0.1.3")
 
 
 def run():
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `paystack_cli-0.1.2/paystack_cli/miscellaneous.py` & `paystack_cli-0.1.3/paystack_cli/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/payment_pages.py` & `paystack_cli-0.1.3/paystack_cli/payment_pages.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/payments_requests.py` & `paystack_cli-0.1.3/paystack_cli/payments_requests.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/plans.py` & `paystack_cli-0.1.3/paystack_cli/plans.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/products.py` & `paystack_cli-0.1.3/paystack_cli/products.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/refunds.py` & `paystack_cli-0.1.3/paystack_cli/refunds.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/settlements.py` & `paystack_cli-0.1.3/paystack_cli/settlements.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/subaccounts.py` & `paystack_cli-0.1.3/paystack_cli/subaccounts.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/subscriptions.py` & `paystack_cli-0.1.3/paystack_cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/terminals.py` & `paystack_cli-0.1.3/paystack_cli/terminals.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/transactions.py` & `paystack_cli-0.1.3/paystack_cli/transactions.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/transactions_splits.py` & `paystack_cli-0.1.3/paystack_cli/transactions_splits.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/transfer_recipients.py` & `paystack_cli-0.1.3/paystack_cli/transfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/transfers.py` & `paystack_cli-0.1.3/paystack_cli/transfers.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/transfers_control.py` & `paystack_cli-0.1.3/paystack_cli/transfers_control.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/utils.py` & `paystack_cli-0.1.3/paystack_cli/utils.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/paystack_cli/verification.py` & `paystack_cli-0.1.3/paystack_cli/verification.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.2/pyproject.toml` & `paystack_cli-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paystack-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "A command line app for interacting with Paystack's API"
 authors = ["Gbenga Adeyi <adeyigbenga005@gmail.com>"]
 readme = "README.md"
 packages = [{include = "paystack_cli"}]
 keywords = ["paystack-python", "pypaystack", "paystack", "paystackapi"]
 license = "MIT"
 classifiers = [
```

### Comparing `paystack_cli-0.1.2/PKG-INFO` & `paystack_cli-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paystack-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A command line app for interacting with Paystack's API
 License: MIT
 Keywords: paystack-python,pypaystack,paystack,paystackapi
 Author: Gbenga Adeyi
 Author-email: adeyigbenga005@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 # paystack cli
 A command line app for interacting with [Paystack's](https://paystack.com/) API. Built with
 [Typer](https://typer.tiangolo.com/) and [Pypaystack2](https://gray-adeyi.github.io/pypaystack2/)
 
 ![utility in use](./paystack-cli.png)
 
 ## Installation
-Binaries of paystack cli be found [here](https://github.com/gray-adeyi/paystack-cli/releases/tag/0.1.2). Alternatively, Paystack cli can be installed from pypi
+Binaries of paystack cli be found [here](https://github.com/gray-adeyi/paystack-cli/releases/tag/0.1.3). Alternatively, Paystack cli can be installed from pypi
 with pip as shown below.
 ```bash
 pip install paystack-cli
 ```
 
 ## First time configurations
 You're required to add your paystack auth_key on first use as shown below
```

