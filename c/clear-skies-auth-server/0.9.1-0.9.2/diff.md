# Comparing `tmp/clear_skies_auth_server-0.9.1.tar.gz` & `tmp/clear_skies_auth_server-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_auth_server-0.9.1.tar", max compression
+gzip compressed data, was "clear_skies_auth_server-0.9.2.tar", max compression
```

## Comparing `clear_skies_auth_server-0.9.1.tar` & `clear_skies_auth_server-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0     1065 2023-07-12 20:39:38.591088 clear_skies_auth_server-0.9.1/LICENSE
--rw-r--r--   0        0        0     1901 2023-07-12 20:39:38.591088 clear_skies_auth_server-0.9.1/README.md
--rw-r--r--   0        0        0     1110 2023-07-14 10:48:26.525736 clear_skies_auth_server-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-14 10:45:01.313322 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/__init__.py
--rw-r--r--   0        0        0       64 2023-07-12 20:39:38.591088 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/applications/__init__.py
--rw-r--r--   0        0        0     2024 2023-07-14 10:49:56.121890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/applications/key_manager.py
--rw-r--r--   0        0        0      224 2023-07-14 10:49:56.081890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/column_types/__init__.py
--rw-r--r--   0        0        0     4566 2023-07-14 10:49:56.153890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/column_types/password.py
--rw-r--r--   0        0        0      528 2023-07-14 10:49:56.081890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/__init__.py
--rw-r--r--   0        0        0     1493 2023-07-14 10:49:56.117890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/create_key.py
--rw-r--r--   0        0        0     1166 2023-07-14 10:49:56.101890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/delete_key.py
--rw-r--r--   0        0        0     1090 2023-07-14 10:49:56.101890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/delete_oldest_key.py
--rw-r--r--   0        0        0      568 2023-07-14 10:49:56.089890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/jwks.py
--rw-r--r--   0        0        0     4826 2023-07-14 10:49:56.173890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/key_base.py
--rw-r--r--   0        0        0      683 2023-07-14 10:49:56.093890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/list_keys.py
--rw-r--r--   0        0        0        0 2023-07-12 20:39:38.591088 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_less_email_request_login.py
--rw-r--r--   0        0        0        0 2023-07-12 20:39:38.591088 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_less_validate_login.py
--rw-r--r--   0        0        0    16683 2023-07-14 10:49:56.261890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_login.py
--rw-r--r--   0        0        0     7925 2023-07-14 10:49:56.217890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_reset.py
--rw-r--r--   0        0        0     7932 2023-07-14 10:49:56.217890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_reset_request.py
--rw-r--r--   0        0        0      730 2023-07-14 10:49:56.117890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/__init__.py
--rw-r--r--   0        0        0      604 2023-07-14 10:49:56.121890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/letters_digits.py
--rw-r--r--   0        0        0     1066 2023-07-14 10:49:56.133890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py
--rw-r--r--   0        0        0      944 2023-07-14 10:49:56.145890 clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/password_validation.py
--rw-r--r--   0        0        0     2932 1970-01-01 00:00:00.000000 clear_skies_auth_server-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-03 23:13:07.715639 clear_skies_auth_server-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1901 2023-04-05 23:17:34.389853 clear_skies_auth_server-0.9.2/README.md
+-rw-r--r--   0        0        0     1110 2023-07-29 19:49:02.889586 clear_skies_auth_server-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-07-28 10:30:32.385807 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-11 11:04:47.143650 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/applications/__init__.py
+-rw-r--r--   0        0        0     2024 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/applications/key_manager.py
+-rw-r--r--   0        0        0      264 2023-07-23 12:00:28.807356 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/authentication/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-29 19:48:46.333491 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/authentication/jwks_direct.py
+-rw-r--r--   0        0        0      379 2023-07-20 20:45:09.680453 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/column_types/__init__.py
+-rw-r--r--   0        0        0    12265 2023-07-20 01:48:22.054909 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/column_types/multi_tenant_configuration.py
+-rw-r--r--   0        0        0     5011 2023-07-22 14:20:33.055474 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/column_types/password.py
+-rw-r--r--   0        0        0     1904 2023-07-22 15:02:01.773222 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/column_types/tenant_id.py
+-rw-r--r--   0        0        0      780 2023-07-28 21:35:59.261167 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/__init__.py
+-rw-r--r--   0        0        0     1493 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/create_key.py
+-rw-r--r--   0        0        0     1166 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/delete_key.py
+-rw-r--r--   0        0        0     1090 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/delete_oldest_key.py
+-rw-r--r--   0        0        0      577 2023-07-28 10:30:32.385807 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/jwks.py
+-rw-r--r--   0        0        0     4828 2023-07-22 14:58:59.065986 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/key_base.py
+-rw-r--r--   0        0        0      683 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/list_keys.py
+-rw-r--r--   0        0        0        0 2023-04-04 23:17:41.819609 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_less_email_request_login.py
+-rw-r--r--   0        0        0        0 2023-04-04 23:17:51.235652 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_less_validate_login.py
+-rw-r--r--   0        0        0    18530 2023-07-29 19:45:03.023805 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_login.py
+-rw-r--r--   0        0        0     5990 2023-07-29 19:48:46.457492 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_reset.py
+-rw-r--r--   0        0        0     8585 2023-07-29 19:48:46.533492 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_reset_request.py
+-rw-r--r--   0        0        0     1415 2023-07-28 17:15:08.379602 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/profile.py
+-rw-r--r--   0        0        0    12718 2023-07-29 19:48:46.641493 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/switch_tenant.py
+-rw-r--r--   0        0        0      793 2023-07-28 11:08:13.445657 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-18 11:19:05.147085 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/letters_digits.py
+-rw-r--r--   0        0        0     1066 2023-07-18 11:19:05.147085 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py
+-rw-r--r--   0        0        0     1654 2023-07-29 19:48:46.485492 clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/password_validation.py
+-rw-r--r--   0        0        0     2932 1970-01-01 00:00:00.000000 clear_skies_auth_server-0.9.2/PKG-INFO
```

### Comparing `clear_skies_auth_server-0.9.1/LICENSE` & `clear_skies_auth_server-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/README.md` & `clear_skies_auth_server-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/pyproject.toml` & `clear_skies_auth_server-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-auth-server"
-version = "0.9.1"
+version = "0.9.2"
 description = "clearskies bindings for managing an authentication server that issues JWTs"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-auth-server"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/applications/key_manager.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/applications/key_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/column_types/password.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/column_types/password.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from clearskies.column_types import string, String
+from clearskies.column_types import String
 from clearskies.input_requirements import required
 from passlib.context import CryptContext
 
 
 class Password(String):
     _crypt_context = None
 
@@ -46,15 +46,20 @@
                 f"Error for column '{self.name}' in model '{self.model_class.__name__}': "
                 + "repeat_password_column_name should be a string, but instead I received a "
                 + str(type(repeat_password_column_name))
             )
 
     def _finalize_configuration(self, configuration):
         configuration = super()._finalize_configuration(
-            {"repeat_password_column_name": "repeat_password", **configuration}
+            {
+                "require_repeat_password": True,
+                "repeat_password_column_name": "repeat_password",
+                "for_login": False,
+                **configuration,
+            }
         )
         found = False
         for config_name in self.crypt_config_names:
             if config_name in configuration:
                 found = True
                 break
         if not found:
@@ -85,14 +90,16 @@
 
     def pre_save(self, data, model):
         # if the password is being set to a non-value, then unset it
         if self.name in data and not data[self.name]:
             del data[self.name]
         elif data.get(self.name):
             data[self.name] = self._crypt_context.hash(data[self.name])
+        if self.config("require_repeat_password") and not self.config("for_login") and "repeat_password" in data:
+            del data["repeat_password"]
         return data
 
     def validate_password(self, user, password):
         hashed_password = user.get(self.name)
         if not hashed_password:
             return False
 
@@ -109,9 +116,11 @@
 
     def additional_write_columns(self, is_create=False):
         if self.config("for_login"):
             return {}
 
         extra_columns = super().additional_write_columns(is_create=is_create)
         if self.config("require_repeat_password"):
-            extra_columns.update([string("repeat_password", is_temporary=True)])
+            repeat_password_column = self.di.build(String, cache=False)
+            repeat_password_column.configure("repeat_password", {"is_temporary": True}, self.model_class)
+            extra_columns["repeat_password"] = repeat_password_column
         return extra_columns
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/__init__.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from .create_key import CreateKey
 from .delete_key import DeleteKey
 from .delete_oldest_key import DeleteOldestKey
-from .list_keys import ListKeys
-from .key_base import KeyBase
 from .jwks import Jwks
+from .key_base import KeyBase
+from .list_keys import ListKeys
+from .password_login import PasswordLogin
+from .password_reset import PasswordReset
+from .password_reset_request import PasswordResetRequest
+from .profile import Profile
+from .switch_tenant import SwitchTenant
 
 # from .password_less_email_request_login import PasswordLessEmailRequestLogin
 # from .password_less_validate_login import PasswordLessValidateLogin
-from .password_login import PasswordLogin
 
 __all__ = [
     "CreateKey",
     "DeleteKey",
     "DeleteOldestKey",
     "ListKeys",
     "KeyBase",
     "Jwks",
     "PasswordLogin",
+    "PasswordReset",
+    "PasswordResetRequest",
+    "Profile",
+    "SwitchTenant",
 ]
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/create_key.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/create_key.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/delete_key.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/delete_key.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/delete_oldest_key.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/delete_oldest_key.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/key_base.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/key_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         key_type = configuration.get("key_type")
         if key_type and key_type != "RSA":
             raise ValueError("Currently only RSA keys are supported.")
 
     def fetch_and_check_keys(self, path, use_cache=True):
         if use_cache and path in self._key_cache:
             cache_valid_time = self._datetime.datetime.now() - self._datetime.timedelta(
-                seconds=self.configuration("cache_valid_time")
+                seconds=self.configuration("key_cache_duration")
             )
             if self._key_cache[path]["cache_time"] > cache_valid_time:
                 return self._key_cache[path]["key_data"]
 
         raw_data = self._secrets.get(path, silent_if_not_found=True)
         if not raw_data:
             return {}
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/list_keys.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/list_keys.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_login.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 class PasswordLogin(KeyBase):
     _configuration_defaults = {
         "user_model_class": "",
         "username_column_name": "email",
         "password_column_name": "password",
+        "tenant_id_column_name": None,
+        "tenant_id_source": None,
+        "tenant_id_source_key_name": None,
         "jwt_lifetime_seconds": 86400,
         "issuer": "",
         "audience": "",
         "path_to_private_keys": "",
         "path_to_public_keys": "",
         "key_cache_duration": 7200,
         "claims_callable": None,
@@ -43,15 +46,15 @@
 
     def __init__(self, di, secrets, datetime):
         super().__init__(di, secrets, datetime)
         self._columns = None
 
     def _check_configuration(self, configuration):
         super()._check_configuration(configuration)
-        error_prefix = "Invalid configuation for handler " + self.__class__.__name__ + ":"
+        error_prefix = "Invalid configuration for handler " + self.__class__.__name__ + ":"
         for key in self._required_configurations:
             if not configuration.get(key):
                 raise ValueError(f"{error_prefix} missing required configuration '{key}'")
         if "claims_callable" in configuration and not callable(configuration.get("claims_callable")):
             raise ValueError(f"{error_prefix} the provided 'claims_callable' configuration is not actually callable.")
         if "input_error_callable" in configuration and not callable(configuration.get("input_error_callable")):
             raise ValueError(
@@ -155,41 +158,67 @@
                 )
             for index, login_check_callable in enumerate(login_check_callables):
                 if not callable(login_check_callable):
                     raise ValueError(
                         f"{error_prefix} each entry in 'login_check_callables' should be a callable, but entry #{index} is not callable."
                     )
 
+        if configuration.get("tenant_id_column_name"):
+            tenant_id_column_name = configuration.get("tenant_id_column_name")
+            if tenant_id_column_name not in self._columns:
+                raise ValueError(
+                    f"{error_prefix} 'tenant_id_column_name' is '{tenant_id_column_name}' but this column does not exist in the user model class, '{user_model_class.__name__}'"
+                )
+            for config_name in ["tenant_id_source", "tenant_id_source_key_name"]:
+                if not configuration.get(config_name):
+                    raise ValueError(
+                        f"{error_prefix} 'tenant_id_column_name' is specified, which enables multi-tenant login. However, this also requires you to define '{config_name}', which is not defined."
+                    )
+            if configuration.get("tenant_id_source") not in ["routing_data"]:
+                raise ValueError(
+                    f"{error_prefix} 'tenant_id_source must be set to 'routing_data', but is something else."
+                )
+
     def _get_audit_column(self, columns):
         audit_column = None
         for column in columns.values():
             if not isinstance(column, Audit):
                 continue
             return column
         return None
 
-    def apply_default_configuation(self, configuration):
+    def apply_default_configuration(self, configuration):
         if not configuration.get("audit_column_name") and ("audit" not in configuration or configuration["audit"]):
             configuration["audit_column_name"] = self._get_audit_column(self._columns).name
-        return super().apply_default_configuation(configuration)
+        return super().apply_default_configuration(configuration)
 
     @property
     def users(self):
         return self._di.build(self.configuration("user_model_class"), cache=True)
 
     def handle(self, input_output):
         request_data = self.request_data(input_output)
         input_errors = self._find_input_errors(self.users, request_data, input_output)
         if input_errors:
             raise InputError(input_errors)
 
         username_column_name = self.configuration("username_column_name")
         password_column_name = self.configuration("password_column_name")
         password_column = self._columns[password_column_name]
-        user = self.users.find(f"{username_column_name}=" + request_data[username_column_name])
+        tenant_id_value = None
+        users = self.users
+        if self.configuration("tenant_id_column_name"):
+            tenant_id_column_name = self.configuration("tenant_id_column_name")
+            tenant_id_source_key_name = self.configuration("tenant_id_source_key_name")
+            if self.configuration("tenant_id_source") == "routing_data":
+                tenant_id_value = input_output.routing_data().get(tenant_id_source_key_name)
+            if not tenant_id_value:
+                return self.error(input_output, "Invalid username/password combination", 404)
+            users = users.where(f"{tenant_id_column_name}={tenant_id_value}")
+        user = users.find(f"{username_column_name}=" + request_data[username_column_name])
 
         # no user found
         if not user.exists:
             return self.error(input_output, "Invalid username/password combination", 404)
 
         # account lockout
         if self.account_locked(user):
@@ -250,15 +279,15 @@
                         },
                     )
                     return self.error(input_output, response, 404)
 
         self.audit(user, self.configuration("audit_action_name_successful_login"))
         signing_key = self.get_youngest_private_key(self.configuration("path_to_private_keys"), as_json=False)
         jwt_claims = self.get_jwt_claims(user)
-        token = jwt.JWT(header={"alg": "RS256", "typ": "JWT"}, claims=jwt_claims)
+        token = jwt.JWT(header={"alg": "RS256", "typ": "JWT", "kid": signing_key["kid"]}, claims=jwt_claims)
         token.make_signed_token(signing_key)
 
         return input_output.respond(
             {
                 "token": token.serialize(),
                 "expires_at": jwt_claims["exp"],
             },
@@ -327,15 +356,15 @@
             input_errors = {
                 **input_errors,
                 **more_input_errors,
             }
         return input_errors
 
     def get_jwt_claims(self, user):
-        if self.configuration("input_error_callable"):
+        if self.configuration("claims_callable"):
             claims = self._di.call_function(user=user)
         else:
             claims = {
                 claim_column: user.get(claim_column) for claim_column in self.configuration("claims_column_names")
             }
 
         now = self._datetime.datetime.now(self._datetime.timezone.utc)
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/handlers/password_reset.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/handlers/password_reset_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import secrets
 import inspect
 from clearskies.handlers.exceptions import InputError
 from clearskies.handlers.base import Base
 from clearskies.column_types import Audit
 
 
-class PasswordReset(Base):
+class PasswordResetRequest(Base):
     _configuration_defaults = {
         "user_model_class": "",
         "username_column_name": "email",
         "email_column_name": "email",
         "reset_key_lifetime_seconds": 86400,
         "reset_key_column_name": "reset_key",
         "reset_expiration_column_name": "reset_key_expiration",
+        "where": None,
         "input_error_callable": None,
         "audit": True,
         "audit_column_name": None,
         "audit_action_name": "request_password_reset",
         "users": None,
     }
 
@@ -27,15 +28,15 @@
     def __init__(self, di, datetime):
         super().__init__(di)
         self._columns = None
         self._datetime = datetime
 
     def _check_configuration(self, configuration):
         super()._check_configuration(configuration)
-        error_prefix = "Invalid configuation for handler " + self.__class__.__name__ + ":"
+        error_prefix = "Invalid configuration for handler " + self.__class__.__name__ + ":"
         for key in self._required_configurations:
             if not configuration.get(key):
                 raise ValueError(f"{error_prefix} missing required configuration '{key}'")
 
         user_model_class = configuration.get("user_model_class")
         if not inspect.isclass(user_model_class):
             raise ValueError(
@@ -60,15 +61,15 @@
         ]
         for config_name in columns_to_check:
             is_default = config_name not in configuration
             column_name = configuration.get(config_name, self._configuration_defaults.get(config_name))
             if column_name not in self._columns:
                 if is_default:
                     raise ValueError(
-                        f"{error_prefix} the configuration setting, '{config_name}' is not set and the deafult column name, '{column_name}', does not exist in the user model '{user_model_class.__name__}'"
+                        f"{error_prefix} the configuration setting, '{config_name}' is not set and the default column name, '{column_name}', does not exist in the user model '{user_model_class.__name__}'"
                     )
                 else:
                     raise ValueError(
                         f"{error_prefix} the provided column name for {config_name}, '{column_name}', does not exist in the user model '{user_model_class.__name__}'"
                     )
         lifetime = configuration.get("reset_key_lifetime_seconds")
         if lifetime and not isinstance(lifetime, int):
@@ -81,38 +82,52 @@
                     f"{error_prefix} 'audit_column_name' is '{audit_column_name}' but this column does not exist in the user model class, '{user_model_class.__name__}'"
                 )
             if not isinstance(self._columns[audit_column_name], Audit):
                 raise ValueError(
                     f"{error_prefix} 'audit_column_name' is '{audit_column_name}' but this column is not an audit column for the user model class, '{user_model_class.__name__}'"
                 )
 
+        for callable_name in ["where", "input_error_callable"]:
+            config = configuration.get(callable_name)
+            if config and not callable(config):
+                raise ValueError(f"{error_prefix} '{callable_name}' must be a callable but it is a " + type(config))
+
     def _get_audit_column(self, columns):
         audit_column = None
         for column in columns.values():
             if not isinstance(column, Audit):
                 continue
             return column
         return None
 
-    def apply_default_configuation(self, configuration):
+    def apply_default_configuration(self, configuration):
         if not configuration.get("audit_column_name") and ("audit" not in configuration or configuration["audit"]):
             configuration["audit_column_name"] = self._get_audit_column(self._columns).name
-        return super().apply_default_configuation(configuration)
+        return super().apply_default_configuration(configuration)
 
     @property
     def users(self):
         return self._di.build(self.configuration("user_model_class"), cache=True)
 
     def handle(self, input_output):
         request_data = self.request_data(input_output)
         input_errors = self._find_input_errors(self.users, request_data, input_output)
         if input_errors:
             raise InputError(input_errors)
 
         username_column_name = self.configuration("username_column_name")
+        users = self.users
+        if self.configuration("where"):
+            users = self._di.call_function(
+                self.configuration("where"),
+                users=users,
+                input_output=input_output,
+                request_data=request_data,
+                routing_data=input_output.routing_data(),
+            )
         user = self.users.find(f"{username_column_name}=" + request_data[username_column_name])
 
         # no user found.  Don't return data since that gives away if the user exists in the system.
         if not user.exists:
             return self.success(input_output, {})
 
         self.audit(user, self.configuration("audit_action_name"))
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/__init__.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     return BindingConfig(LettersDigits)
 
 
 def letters_digits_special_characters(special_characters="!@#$%^&*()<>,.?~`"):
     return BindingConfig(LettersDigitsSpecialCharacters, special_characters=special_characters)
 
 
-def password_validation():
-    return BindingConfig(PasswordValidation)
+def password_validation(password_column_name):
+    return BindingConfig(PasswordValidation, password_column_name=password_column_name)
 
 
 __all__ = [
     "letters_digits",
     "letters_digits_special_characters",
     "LettersDigits",
     "LettersDigitsSpecialCharacters",
```

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/letters_digits.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/letters_digits.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py` & `clear_skies_auth_server-0.9.2/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.1/PKG-INFO` & `clear_skies_auth_server-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-auth-server
-Version: 0.9.1
+Version: 0.9.2
 Summary: clearskies bindings for managing an authentication server that issues JWTs
 Home-page: https://github.com/cmancone/clearskies-auth-server
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

