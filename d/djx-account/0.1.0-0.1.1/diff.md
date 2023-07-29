# Comparing `tmp/djx_account-0.1.0.tar.gz` & `tmp/djx_account-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djx_account-0.1.0.tar", max compression
+gzip compressed data, was "djx_account-0.1.1.tar", max compression
```

## Comparing `djx_account-0.1.0.tar` & `djx_account-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0       36 2023-07-05 21:20:56.666798 djx_account-0.1.0/djx_account/.git
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.687287 djx_account-0.1.0/djx_account/__init__.py
--rw-r--r--   0        0        0      438 2023-07-05 21:20:56.688287 djx_account-0.1.0/djx_account/admin.py
--rw-r--r--   0        0        0      226 2023-07-05 21:20:56.688287 djx_account-0.1.0/djx_account/apps.py
--rw-r--r--   0        0        0     1831 2023-07-05 21:20:56.689288 djx_account-0.1.0/djx_account/email_constructor.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.689288 djx_account-0.1.0/djx_account/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.690287 djx_account-0.1.0/djx_account/management/commands/__init__.py
--rw-r--r--   0        0        0      630 2023-07-05 21:20:56.691287 djx_account-0.1.0/djx_account/management/commands/create_admin.py
--rw-r--r--   0        0        0     1360 2023-07-05 21:20:56.691287 djx_account-0.1.0/djx_account/managers.py
--rw-r--r--   0        0        0     5103 2023-07-05 21:20:56.692287 djx_account-0.1.0/djx_account/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.692287 djx_account-0.1.0/djx_account/migrations/__init__.py
--rw-r--r--   0        0        0     1499 2023-07-05 21:20:56.693288 djx_account-0.1.0/djx_account/models.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.693288 djx_account-0.1.0/djx_account/serializers/__init__.py
--rw-r--r--   0        0        0     4947 2023-07-05 21:20:56.694288 djx_account-0.1.0/djx_account/serializers/base_oauth_serializers.py
--rw-r--r--   0        0        0     6005 2023-07-05 21:20:56.695286 djx_account-0.1.0/djx_account/serializers/login_serializers.py
--rw-r--r--   0        0        0      326 2023-07-05 21:20:56.695286 djx_account-0.1.0/djx_account/serializers/oauth_credentials_serializers.py
--rw-r--r--   0        0        0     1772 2023-07-05 21:20:56.696286 djx_account-0.1.0/djx_account/serializers/registration_serializers.py
--rw-r--r--   0        0        0     3458 2023-07-05 21:20:56.696286 djx_account-0.1.0/djx_account/serializers/reset_password_serializers.py
--rw-r--r--   0        0        0      256 2023-07-05 21:20:56.697289 djx_account-0.1.0/djx_account/serializers/user_claims_serializer.py
--rw-r--r--   0        0        0     2977 2023-07-05 21:20:56.697289 djx_account-0.1.0/djx_account/serializers/user_confirmation_serializers.py
--rw-r--r--   0        0        0     1428 2023-07-05 21:20:56.698290 djx_account-0.1.0/djx_account/serializers/user_serializers.py
--rw-r--r--   0        0        0     1012 2023-07-05 21:20:56.698290 djx_account-0.1.0/djx_account/serializers/user_token_serializers.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.699290 djx_account-0.1.0/djx_account/services/__init__.py
--rw-r--r--   0        0        0     3128 2023-07-05 21:20:56.699290 djx_account-0.1.0/djx_account/services/discord_service.py
--rw-r--r--   0        0        0     1209 2023-07-05 21:20:56.700288 djx_account-0.1.0/djx_account/services/facebook_service.py
--rw-r--r--   0        0        0     2057 2023-07-05 21:20:56.701288 djx_account-0.1.0/djx_account/services/google_service.py
--rw-r--r--   0        0        0     1603 2023-07-05 21:20:56.701288 djx_account-0.1.0/djx_account/services/microsoft_service.py
--rw-r--r--   0        0        0      181 2023-07-05 21:20:56.702293 djx_account-0.1.0/djx_account/services/oauth_service_interface.py
--rw-r--r--   0        0        0     1432 2023-07-05 21:20:56.702293 djx_account-0.1.0/djx_account/services/twitter_service.py
--rw-r--r--   0        0        0     1340 2023-07-05 21:20:56.703287 djx_account-0.1.0/djx_account/settings.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.703287 djx_account-0.1.0/djx_account/signals/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.704287 djx_account-0.1.0/djx_account/signals/receivers.py
--rw-r--r--   0        0        0      274 2023-07-05 21:20:56.704287 djx_account-0.1.0/djx_account/signals/senders.py
--rw-r--r--   0        0        0      377 2023-07-05 21:20:56.705289 djx_account-0.1.0/djx_account/templates/header/mail.html
--rw-r--r--   0        0        0      500 2023-07-05 21:20:56.706292 djx_account-0.1.0/djx_account/templates/password_reset/mail.html
--rw-r--r--   0        0        0      500 2023-07-05 21:20:56.706292 djx_account-0.1.0/djx_account/templates/registration_welcome/mail.html
--rw-r--r--   0        0        0      500 2023-07-05 21:20:56.707289 djx_account-0.1.0/djx_account/templates/user_confirmation/mail.html
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.708289 djx_account-0.1.0/djx_account/tests/__init__.py
--rw-r--r--   0        0        0     1945 2023-07-05 21:20:56.708289 djx_account-0.1.0/djx_account/tests/tests_login_serializer.py
--rw-r--r--   0        0        0     1181 2023-07-05 21:20:56.709288 djx_account-0.1.0/djx_account/tests/tests_login_view.py
--rw-r--r--   0        0        0     1876 2023-07-05 21:20:56.710288 djx_account-0.1.0/djx_account/tests/tests_registation_serializer.py
--rw-r--r--   0        0        0     1437 2023-07-05 21:20:56.710288 djx_account-0.1.0/djx_account/tests/tests_registration_view.py
--rw-r--r--   0        0        0     2783 2023-07-05 21:20:56.711288 djx_account-0.1.0/djx_account/tests/tests_reset_password_serializer.py
--rw-r--r--   0        0        0     1540 2023-07-05 21:20:56.711288 djx_account-0.1.0/djx_account/tests/tests_reset_password_view.py
--rw-r--r--   0        0        0     1701 2023-07-05 21:20:56.712288 djx_account-0.1.0/djx_account/tests/tests_user_confirmation_serializer.py
--rw-r--r--   0        0        0     1036 2023-07-05 21:20:56.712288 djx_account-0.1.0/djx_account/tests/tests_user_confirmation_view.py
--rw-r--r--   0        0        0     1478 2023-07-05 21:20:56.713288 djx_account-0.1.0/djx_account/tests/tests_user_serializer.py
--rw-r--r--   0        0        0     2091 2023-07-05 21:20:56.713288 djx_account-0.1.0/djx_account/tests/tests_user_views.py
--rw-r--r--   0        0        0      886 2023-07-05 21:20:56.714294 djx_account-0.1.0/djx_account/urls.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.714294 djx_account-0.1.0/djx_account/utils/__init__.py
--rw-r--r--   0        0        0      362 2023-07-05 21:20:56.715288 djx_account-0.1.0/djx_account/utils/custom_tests.py
--rw-r--r--   0        0        0      466 2023-07-05 21:20:56.715288 djx_account-0.1.0/djx_account/utils/error_messages.py
--rw-r--r--   0        0        0      205 2023-07-05 21:20:56.716291 djx_account-0.1.0/djx_account/utils/exceptions.py
--rw-r--r--   0        0        0      429 2023-07-05 21:20:56.717288 djx_account-0.1.0/djx_account/utils/format_with_jinja.py
--rw-r--r--   0        0        0      623 2023-07-05 21:20:56.717288 djx_account-0.1.0/djx_account/utils/mail_api.py
--rw-r--r--   0        0        0      375 2023-07-05 21:20:56.718290 djx_account-0.1.0/djx_account/utils/others.py
--rw-r--r--   0        0        0      371 2023-07-05 21:20:56.718290 djx_account-0.1.0/djx_account/utils/token_generator.py
--rw-r--r--   0        0        0        0 2023-07-05 21:20:56.719288 djx_account-0.1.0/djx_account/views/__init__.py
--rw-r--r--   0        0        0     3981 2023-07-05 21:20:56.719288 djx_account-0.1.0/djx_account/views/login_views.py
--rw-r--r--   0        0        0      515 2023-07-05 21:20:56.720288 djx_account-0.1.0/djx_account/views/registration_views.py
--rw-r--r--   0        0        0     1588 2023-07-05 21:20:56.720288 djx_account-0.1.0/djx_account/views/reset_password_views.py
--rw-r--r--   0        0        0     1194 2023-07-05 21:20:56.721289 djx_account-0.1.0/djx_account/views/user_confirmation_views.py
--rw-r--r--   0        0        0     1729 2023-07-05 21:20:56.722291 djx_account-0.1.0/djx_account/views/user_views.py
--rw-r--r--   0        0        0      516 2023-07-05 21:26:44.756503 djx_account-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 21:17:59.365119 djx_account-0.1.0/README.md
--rw-r--r--   0        0        0     1248 1970-01-01 00:00:00.000000 djx_account-0.1.0/setup.py
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 djx_account-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-07-05 21:20:56.666798 djx_account-0.1.1/djx_account/.git
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.687287 djx_account-0.1.1/djx_account/__init__.py
+-rw-r--r--   0        0        0      438 2023-07-05 21:20:56.688287 djx_account-0.1.1/djx_account/admin.py
+-rw-r--r--   0        0        0      226 2023-07-05 21:20:56.688287 djx_account-0.1.1/djx_account/apps.py
+-rw-r--r--   0        0        0     1831 2023-07-05 21:20:56.689288 djx_account-0.1.1/djx_account/email_constructor.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.689288 djx_account-0.1.1/djx_account/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.690287 djx_account-0.1.1/djx_account/management/commands/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-05 21:20:56.691287 djx_account-0.1.1/djx_account/management/commands/create_admin.py
+-rw-r--r--   0        0        0     1360 2023-07-05 21:20:56.691287 djx_account-0.1.1/djx_account/managers.py
+-rw-r--r--   0        0        0     5103 2023-07-05 21:20:56.692287 djx_account-0.1.1/djx_account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      583 2023-07-29 15:36:46.926840 djx_account-0.1.1/djx_account/migrations/0002_alter_oauthcredentials_access_token_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.692287 djx_account-0.1.1/djx_account/migrations/__init__.py
+-rw-r--r--   0        0        0     1469 2023-07-29 15:36:46.927839 djx_account-0.1.1/djx_account/models.py
+-rw-r--r--   0        0        0      618 2023-07-29 15:36:46.928840 djx_account-0.1.1/djx_account/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.693288 djx_account-0.1.1/djx_account/serializers/__init__.py
+-rw-r--r--   0        0        0     5129 2023-07-29 15:36:46.929839 djx_account-0.1.1/djx_account/serializers/base_oauth_serializers.py
+-rw-r--r--   0        0        0     6005 2023-07-05 21:20:56.695286 djx_account-0.1.1/djx_account/serializers/login_serializers.py
+-rw-r--r--   0        0        0      326 2023-07-05 21:20:56.695286 djx_account-0.1.1/djx_account/serializers/oauth_credentials_serializers.py
+-rw-r--r--   0        0        0     1772 2023-07-05 21:20:56.696286 djx_account-0.1.1/djx_account/serializers/registration_serializers.py
+-rw-r--r--   0        0        0     3458 2023-07-05 21:20:56.696286 djx_account-0.1.1/djx_account/serializers/reset_password_serializers.py
+-rw-r--r--   0        0        0      256 2023-07-05 21:20:56.697289 djx_account-0.1.1/djx_account/serializers/user_claims_serializer.py
+-rw-r--r--   0        0        0     2977 2023-07-05 21:20:56.697289 djx_account-0.1.1/djx_account/serializers/user_confirmation_serializers.py
+-rw-r--r--   0        0        0     1428 2023-07-05 21:20:56.698290 djx_account-0.1.1/djx_account/serializers/user_serializers.py
+-rw-r--r--   0        0        0     1012 2023-07-05 21:20:56.698290 djx_account-0.1.1/djx_account/serializers/user_token_serializers.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.699290 djx_account-0.1.1/djx_account/services/__init__.py
+-rw-r--r--   0        0        0     3128 2023-07-05 21:20:56.699290 djx_account-0.1.1/djx_account/services/discord_service.py
+-rw-r--r--   0        0        0     1209 2023-07-05 21:20:56.700288 djx_account-0.1.1/djx_account/services/facebook_service.py
+-rw-r--r--   0        0        0     2127 2023-07-29 15:36:46.930840 djx_account-0.1.1/djx_account/services/google_service.py
+-rw-r--r--   0        0        0     1603 2023-07-05 21:20:56.701288 djx_account-0.1.1/djx_account/services/microsoft_service.py
+-rw-r--r--   0        0        0      181 2023-07-05 21:20:56.702293 djx_account-0.1.1/djx_account/services/oauth_service_interface.py
+-rw-r--r--   0        0        0     1432 2023-07-05 21:20:56.702293 djx_account-0.1.1/djx_account/services/twitter_service.py
+-rw-r--r--   0        0        0     1436 2023-07-29 15:36:46.931840 djx_account-0.1.1/djx_account/settings.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.703287 djx_account-0.1.1/djx_account/signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.704287 djx_account-0.1.1/djx_account/signals/receivers.py
+-rw-r--r--   0        0        0      274 2023-07-05 21:20:56.704287 djx_account-0.1.1/djx_account/signals/senders.py
+-rw-r--r--   0        0        0      377 2023-07-05 21:20:56.705289 djx_account-0.1.1/djx_account/templates/header/mail.html
+-rw-r--r--   0        0        0      500 2023-07-05 21:20:56.706292 djx_account-0.1.1/djx_account/templates/password_reset/mail.html
+-rw-r--r--   0        0        0      500 2023-07-05 21:20:56.706292 djx_account-0.1.1/djx_account/templates/registration_welcome/mail.html
+-rw-r--r--   0        0        0      500 2023-07-05 21:20:56.707289 djx_account-0.1.1/djx_account/templates/user_confirmation/mail.html
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.708289 djx_account-0.1.1/djx_account/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2023-07-05 21:20:56.708289 djx_account-0.1.1/djx_account/tests/tests_login_serializer.py
+-rw-r--r--   0        0        0     1181 2023-07-05 21:20:56.709288 djx_account-0.1.1/djx_account/tests/tests_login_view.py
+-rw-r--r--   0        0        0     1876 2023-07-05 21:20:56.710288 djx_account-0.1.1/djx_account/tests/tests_registation_serializer.py
+-rw-r--r--   0        0        0     1437 2023-07-05 21:20:56.710288 djx_account-0.1.1/djx_account/tests/tests_registration_view.py
+-rw-r--r--   0        0        0     2783 2023-07-05 21:20:56.711288 djx_account-0.1.1/djx_account/tests/tests_reset_password_serializer.py
+-rw-r--r--   0        0        0     1540 2023-07-05 21:20:56.711288 djx_account-0.1.1/djx_account/tests/tests_reset_password_view.py
+-rw-r--r--   0        0        0     1701 2023-07-05 21:20:56.712288 djx_account-0.1.1/djx_account/tests/tests_user_confirmation_serializer.py
+-rw-r--r--   0        0        0     1036 2023-07-05 21:20:56.712288 djx_account-0.1.1/djx_account/tests/tests_user_confirmation_view.py
+-rw-r--r--   0        0        0     1478 2023-07-05 21:20:56.713288 djx_account-0.1.1/djx_account/tests/tests_user_serializer.py
+-rw-r--r--   0        0        0     2091 2023-07-05 21:20:56.713288 djx_account-0.1.1/djx_account/tests/tests_user_views.py
+-rw-r--r--   0        0        0      886 2023-07-05 21:20:56.714294 djx_account-0.1.1/djx_account/urls.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.714294 djx_account-0.1.1/djx_account/utils/__init__.py
+-rw-r--r--   0        0        0      362 2023-07-05 21:20:56.715288 djx_account-0.1.1/djx_account/utils/custom_tests.py
+-rw-r--r--   0        0        0      466 2023-07-05 21:20:56.715288 djx_account-0.1.1/djx_account/utils/error_messages.py
+-rw-r--r--   0        0        0      205 2023-07-05 21:20:56.716291 djx_account-0.1.1/djx_account/utils/exceptions.py
+-rw-r--r--   0        0        0      429 2023-07-05 21:20:56.717288 djx_account-0.1.1/djx_account/utils/format_with_jinja.py
+-rw-r--r--   0        0        0      623 2023-07-05 21:20:56.717288 djx_account-0.1.1/djx_account/utils/mail_api.py
+-rw-r--r--   0        0        0      375 2023-07-05 21:20:56.718290 djx_account-0.1.1/djx_account/utils/others.py
+-rw-r--r--   0        0        0      371 2023-07-05 21:20:56.718290 djx_account-0.1.1/djx_account/utils/token_generator.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:20:56.719288 djx_account-0.1.1/djx_account/views/__init__.py
+-rw-r--r--   0        0        0     3981 2023-07-05 21:20:56.719288 djx_account-0.1.1/djx_account/views/login_views.py
+-rw-r--r--   0        0        0      515 2023-07-05 21:20:56.720288 djx_account-0.1.1/djx_account/views/registration_views.py
+-rw-r--r--   0        0        0     1588 2023-07-05 21:20:56.720288 djx_account-0.1.1/djx_account/views/reset_password_views.py
+-rw-r--r--   0        0        0     1194 2023-07-05 21:20:56.721289 djx_account-0.1.1/djx_account/views/user_confirmation_views.py
+-rw-r--r--   0        0        0     1729 2023-07-05 21:20:56.722291 djx_account-0.1.1/djx_account/views/user_views.py
+-rw-r--r--   0        0        0      516 2023-07-29 15:37:12.560975 djx_account-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:59.365119 djx_account-0.1.1/README.md
+-rw-r--r--   0        0        0     1248 1970-01-01 00:00:00.000000 djx_account-0.1.1/setup.py
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 djx_account-0.1.1/PKG-INFO
```

### Comparing `djx_account-0.1.0/djx_account/email_constructor.py` & `djx_account-0.1.1/djx_account/email_constructor.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/management/commands/create_admin.py` & `djx_account-0.1.1/djx_account/management/commands/create_admin.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/managers.py` & `djx_account-0.1.1/djx_account/managers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/migrations/0001_initial.py` & `djx_account-0.1.1/djx_account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/models.py` & `djx_account-0.1.1/djx_account/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     class Meta:
         unique_together = (('user', 'email'),)
 
 
 class OauthCredentials(models.Model):
     user = models.ForeignKey(UserModel, on_delete=models.CASCADE)
     oauth_category = models.CharField(max_length=10)
-    access_token = models.CharField(max_length=100)
-    refresh_token = models.CharField(max_length=100, null=True, blank=True)
+    access_token = models.TextField()
+    refresh_token = models.TextField(null=True, blank=True)
     expires_at = models.DateTimeField(null=True, blank=True)
```

### Comparing `djx_account-0.1.0/djx_account/serializers/base_oauth_serializers.py` & `djx_account-0.1.1/djx_account/serializers/base_oauth_serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.urls import reverse as reverse_url
 from rest_framework import serializers
 
 from djx_account import settings
 from djx_account.models import OauthCredentials, UserModel
 from djx_account.serializers.oauth_credentials_serializers import OauthCredentialSerializer
 from djx_account.serializers.user_token_serializers import UserTokenSerializer
+from djx_account.signals.senders import registration_completed
 from djx_account.utils.error_messages import ErrorMessage
 from djx_account.utils.exceptions import BadRequestException
 
 
 class OauthBaseSerializer(serializers.Serializer):
     oauth_category = None
     service = None
@@ -32,34 +33,34 @@
                 "oauth_category": self.oauth_category
             }
         )
         serializer.is_valid(raise_exception=True)
         serializer.save()
 
     def create(self, validated_data):
-        code = validated_data.get('code')
-        redirect_to = validated_data.get('redirect_to', None)
+        # code = validated_data.get('code')
+        # redirect_to = validated_data.get('redirect_to', None)
         response = self.service.check_token(**validated_data)
 
         user_data = response['user']
         user_credentials = response['credentials']
-        additional_data = response['additional_data']
+        # additional_data = response['additional_data']
         if settings.CREATE_USER_ON_LOGIN:
             user, _ = UserModel.objects.get_or_create(
                 email=user_data['email'],
                 defaults=user_data
             )
         else:
             try:
                 user = UserModel.objects.get(
                     email=user_data['email']
                 )
             except UserModel.DoesNotExist:
                 raise BadRequestException(ErrorMessage.user_not_found)
-        self.save_oauth_credentials(user, user_credentials)
+        # self.save_oauth_credentials(user, user_credentials)
         return user
 
     def get_default_redirect_to_value(self, value):
         if value is None:
             req = self.context['request']
             url = reverse_url(self.default_redirect_url)
             value = req.build_absolute_uri(url)
@@ -95,18 +96,20 @@
         redirect_to = validated_data.get('redirect_to', None)
         redirect_to = self.get_default_redirect_to_value(redirect_to)
         response = self.service.check_token(redirect_uri=redirect_to, **validated_data)
         user_data = response['user']
         user_credentials = response['credentials'] if "credentials" in response else None
 
         if settings.CREATE_USER_ON_LOGIN:
-            user, _ = UserModel.objects.get_or_create(
+            user, created = UserModel.objects.get_or_create(
                 email=user_data['email'],
                 defaults=user_data
             )
+            if created:
+                registration_completed.send(sender=self.__class__, user=user)
         else:
             try:
                 user = UserModel.objects.get(
                     email=user_data['email']
                 )
             except UserModel.DoesNotExist:
                 raise BadRequestException(ErrorMessage.user_not_found)
```

### Comparing `djx_account-0.1.0/djx_account/serializers/login_serializers.py` & `djx_account-0.1.1/djx_account/serializers/login_serializers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/serializers/registration_serializers.py` & `djx_account-0.1.1/djx_account/serializers/registration_serializers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/serializers/reset_password_serializers.py` & `djx_account-0.1.1/djx_account/serializers/reset_password_serializers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/serializers/user_confirmation_serializers.py` & `djx_account-0.1.1/djx_account/serializers/user_confirmation_serializers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/serializers/user_serializers.py` & `djx_account-0.1.1/djx_account/serializers/user_serializers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/serializers/user_token_serializers.py` & `djx_account-0.1.1/djx_account/serializers/user_token_serializers.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/services/discord_service.py` & `djx_account-0.1.1/djx_account/services/discord_service.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/services/facebook_service.py` & `djx_account-0.1.1/djx_account/services/facebook_service.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/services/google_service.py` & `djx_account-0.1.1/djx_account/services/google_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,45 +14,46 @@
 from djx_account.utils.error_messages import ErrorMessage
 from djx_account.utils.exceptions import BadRequestException
 
 
 class GoogleService:
 
     @staticmethod
-    def get_url(redirect_uri):
+    def get_url(redirect_uri, **kwargs):
         client_id = settings.GOOGLE_CLIENT_ID
         base_url = "https://accounts.google.com/o/oauth2/auth"
         req = requests.PreparedRequest()
         req.prepare_url(base_url,
                         {"client_id": client_id,
                          "redirect_uri": redirect_uri,
                          "scope": "email",
                          "response_type": "code"})
         return req.url
 
     @staticmethod
-    def check_token(code, redirect_uri):
+    def check_token(code, redirect_uri, **kwargs):
         response = requests.post(
             url="https://oauth2.googleapis.com/token",
             data={"code": code, "client_id": settings.GOOGLE_CLIENT_ID,
                   "redirect_uri": redirect_uri,
                   "client_secret": settings.GOOGLE_CLIENT_SECRET,
                   "grant_type": "authorization_code"},
         )
         if response.status_code != 200:
             raise BadRequestException(ErrorMessage.invalid_code)
 
         data = response.json()
         token = data['id_token']
-        token_data = id_token.verify_oauth2_token(token, google_request.Request(), clock_skew_in_seconds=0)
-        expires_in = token['expires_in']
+        token_data = id_token.verify_oauth2_token(token, google_request.Request(), clock_skew_in_seconds=10)
+        expires_in = data['expires_in']
         expires_at = now() + datetime.timedelta(seconds=expires_in)
         return {
             "user": {
                 "email": token_data["email"],
+                "username": token_data["email"],
             },
             "credentials": {
                 "access_token": data['access_token'],
                 "expires_at": expires_at,
             },
             "additional_data": {
                 "email_verified": token_data["email_verified"]
```

### Comparing `djx_account-0.1.0/djx_account/services/microsoft_service.py` & `djx_account-0.1.1/djx_account/services/microsoft_service.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/services/twitter_service.py` & `djx_account-0.1.1/djx_account/services/twitter_service.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/settings.py` & `djx_account-0.1.1/djx_account/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.conf import settings
 
 DJX_ACCOUNT = settings.DJX_ACCOUNT
 
 USER_CONFIRMATION_TOKEN_TTL = DJX_ACCOUNT['USER_CONFIRMATION_TOKEN_TTL']
 USER_PASSWORD_RESET_TOKEN_TTL = DJX_ACCOUNT['USER_PASSWORD_RESET_TOKEN_TTL']
 
-CLIENT_USER_CONFIRMATION_TOKEN_URL = "http://Localhost:8000"
-CLIENT_USER_PASSWORD_RESET_TOKEN_URL = "http://localhost:8000"
+CLIENT_USER_CONFIRMATION_TOKEN_URL = DJX_ACCOUNT["CLIENT_USER_CONFIRMATION_TOKEN_URL"]
+CLIENT_USER_PASSWORD_RESET_TOKEN_URL = DJX_ACCOUNT["CLIENT_USER_PASSWORD_RESET_TOKEN_URL"]
 
 GOOGLE_CLIENT_SECRET = DJX_ACCOUNT['GOOGLE']['CLIENT_SECRET']
 GOOGLE_CLIENT_ID = DJX_ACCOUNT['GOOGLE']['CLIENT_ID']
 
 FACEBOOK_CLIENT_ID = DJX_ACCOUNT['FACEBOOK']['CLIENT_ID']
 FACEBOOK_SECRET = DJX_ACCOUNT['FACEBOOK']['CLIENT_SECRET']
 
@@ -27,8 +27,8 @@
 DISCORD_CLIENT_SECRET = DJX_ACCOUNT['DISCORD']['CLIENT_SECRET']
 DISCORD_USERNAME_KEY = 'email'
 
 DEFAULT_ADMIN_USERNAME = DJX_ACCOUNT["DEFAULT_ADMIN_USERNAME"]
 DEFAULT_ADMIN_EMAIL = DJX_ACCOUNT["DEFAULT_ADMIN_EMAIL"]
 DEFAULT_ADMIN_PASSWORD = DJX_ACCOUNT["DEFAULT_ADMIN_PASSWORD"]
 
-CREATE_USER_ON_LOGIN = True
+CREATE_USER_ON_LOGIN = DJX_ACCOUNT.get("CREATE_USER_ON_LOGIN", False)
```

### Comparing `djx_account-0.1.0/djx_account/tests/tests_login_serializer.py` & `djx_account-0.1.1/djx_account/tests/tests_login_serializer.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_login_view.py` & `djx_account-0.1.1/djx_account/tests/tests_login_view.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_registation_serializer.py` & `djx_account-0.1.1/djx_account/tests/tests_registation_serializer.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_registration_view.py` & `djx_account-0.1.1/djx_account/tests/tests_registration_view.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_reset_password_serializer.py` & `djx_account-0.1.1/djx_account/tests/tests_reset_password_serializer.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_reset_password_view.py` & `djx_account-0.1.1/djx_account/tests/tests_reset_password_view.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_user_confirmation_serializer.py` & `djx_account-0.1.1/djx_account/tests/tests_user_confirmation_serializer.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_user_confirmation_view.py` & `djx_account-0.1.1/djx_account/tests/tests_user_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_user_serializer.py` & `djx_account-0.1.1/djx_account/tests/tests_user_serializer.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/tests/tests_user_views.py` & `djx_account-0.1.1/djx_account/tests/tests_user_views.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/urls.py` & `djx_account-0.1.1/djx_account/urls.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/utils/mail_api.py` & `djx_account-0.1.1/djx_account/utils/mail_api.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/views/login_views.py` & `djx_account-0.1.1/djx_account/views/login_views.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/views/registration_views.py` & `djx_account-0.1.1/djx_account/views/registration_views.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/views/reset_password_views.py` & `djx_account-0.1.1/djx_account/views/reset_password_views.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/views/user_confirmation_views.py` & `djx_account-0.1.1/djx_account/views/user_confirmation_views.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/djx_account/views/user_views.py` & `djx_account-0.1.1/djx_account/views/user_views.py`

 * *Files identical despite different names*

### Comparing `djx_account-0.1.0/pyproject.toml` & `djx_account-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djx-account"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["nope"]
 readme = "README.md"
 packages = [{include = "djx_account"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `djx_account-0.1.0/setup.py` & `djx_account-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'jinja2>=3.1.2,<4.0.0',
  'msal>=1.20.0,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'tweepy>=4.12.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'djx-account',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
     'author': 'nope',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `djx_account-0.1.0/PKG-INFO` & `djx_account-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djx-account
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: nope
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.1.4,<5.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
```

