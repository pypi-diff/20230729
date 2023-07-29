# Comparing `tmp/aleksis_app_paweljong-2.0.dev2.tar.gz` & `tmp/aleksis_app_paweljong-3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_paweljong-2.0.dev2.tar", max compression
+gzip compressed data, was "aleksis_app_paweljong-3.0.dev1.tar", max compression
```

## Comparing `aleksis_app_paweljong-2.0.dev2.tar` & `aleksis_app_paweljong-3.0.dev1.tar`

### file list

```diff
@@ -1,108 +1,109 @@
--rw-r--r--   0        0        0     3513 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev2/LICENCE.rst
--rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev2/README.rst
--rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/__init__.py
--rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/apps.py
--rw-r--r--   0        0        0     1253 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/data_checks.py
--rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/filters.py
--rw-r--r--   0        0        0    16277 2023-06-07 12:34:32.225375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/forms.py
--rw-r--r--   0        0        0    12923 2023-07-03 20:57:19.659645 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/frontend/index.js
--rw-r--r--   0        0        0      563 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47795 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    31014 2023-07-02 21:38:39.358049 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    64927 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47711 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-02 21:38:39.358049 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-02 21:38:39.362049 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8628 2023-07-02 21:37:58.185924 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0001_initial.py
--rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0002_event_website.py
--rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
--rw-r--r--   0        0        0      893 2023-07-02 21:37:58.185924 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
--rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
--rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
--rw-r--r--   0        0        0     2493 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0007_terms.py
--rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
--rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
--rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
--rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
--rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0012_event_slug.py
--rw-r--r--   0        0        0     2429 2022-03-01 20:42:19.678476 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0013_info_mailings.py
--rw-r--r--   0        0        0     2855 2022-03-03 20:52:23.956034 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
--rw-r--r--   0        0        0     1268 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0015_registrationstate.py
--rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
--rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
--rw-r--r--   0        0        0     1781 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
--rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0019_retractions.py
--rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0020_check_in.py
--rw-r--r--   0        0        0     2217 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0021_checkpoint.py
--rw-r--r--   0        0        0      681 2022-07-08 20:57:59.622407 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py
--rw-r--r--   0        0        0      452 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0023_eventregistration_cost.py
--rw-r--r--   0        0        0      430 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0024_add_cost_to_registration.py
--rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/__init__.py
--rw-r--r--   0        0        0    16558 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/models.py
--rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/predicates.py
--rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/preferences.py
--rw-r--r--   0        0        0     9079 2022-06-30 15:18:35.332204 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/rules.py
--rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/settings.py
--rw-r--r--   0        0        0     1076 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/static/css/paweljong.css
--rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
--rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
--rw-r--r--   0        0        0     4445 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/tables.py
--rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/tasks.py
--rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
--rw-r--r--   0        0        0      560 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html
--rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/create.html
--rw-r--r--   0        0        0     3557 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/detail.html
--rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/edit.html
--rw-r--r--   0        0        0     2480 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/full.html
--rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/list.html
--rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/manage.html
--rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
--rw-r--r--   0        0        0     5118 2023-06-07 12:34:32.229375 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
--rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
--rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
--rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/registered.html
--rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/terms.html
--rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
--rw-r--r--   0        0        0    13116 2022-06-28 20:06:29.947789 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
--rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
--rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
--rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
--rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
--rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
--rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/corona.html
--rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
--rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
--rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
--rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/manage.html
--rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
--rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/register.html
--rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/register_start.html
--rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
--rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
--rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
--rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
--rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/term/create.html
--rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/term/edit.html
--rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/term/list.html
--rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
--rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
--rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
--rw-r--r--   0        0        0     2272 2023-07-02 13:19:00.183869 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/account_registered.email
--rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/event_created.email
--rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/event_notification.email
--rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/event_registered.email
--rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
--rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templatetags/coerce.py
--rw-r--r--   0        0        0     5596 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/urls.py
--rw-r--r--   0        0        0    40215 2023-07-02 15:36:07.119560 aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/views.py
--rw-r--r--   0        0        0     1523 2023-07-03 20:57:22.319659 aleksis_app_paweljong-2.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev2/setup.py
--rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 aleksis_app_paweljong-2.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     3513 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-11-30 15:14:06.498459 aleksis_app_paweljong-3.0.dev1/LICENCE.rst
+-rw-r--r--   0        0        0     1173 2022-02-21 18:12:43.394342 aleksis_app_paweljong-3.0.dev1/README.rst
+-rw-r--r--   0        0        0      155 2021-11-30 15:50:47.629248 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/__init__.py
+-rw-r--r--   0        0        0      530 2022-02-21 18:12:43.394342 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/apps.py
+-rw-r--r--   0        0        0     1253 2023-06-07 12:34:32.225375 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/data_checks.py
+-rw-r--r--   0        0        0     1726 2022-06-24 14:54:41.596452 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/filters.py
+-rw-r--r--   0        0        0    16267 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/forms.py
+-rw-r--r--   0        0        0     3500 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/frontend/components/event/Checkpoint.vue
+-rw-r--r--   0        0        0    12790 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/frontend/index.js
+-rw-r--r--   0        0        0      563 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-07-02 21:38:39.362049 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47795 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    31014 2023-07-02 21:38:39.358049 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    64927 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-02 21:38:39.362049 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47711 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-02 21:38:39.358049 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-02 21:38:39.362049 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-02 21:38:39.362049 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47665 2023-07-02 15:36:07.119560 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8580 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0001_initial.py
+-rw-r--r--   0        0        0      457 2021-11-30 15:50:20.745263 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0002_event_website.py
+-rw-r--r--   0        0        0      493 2022-02-21 09:18:10.132166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0003_alter_event_feedback_aspects.py
+-rw-r--r--   0        0        0      893 2023-07-02 21:37:58.185924 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py
+-rw-r--r--   0        0        0      479 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0005_eventregistration_medical_information.py
+-rw-r--r--   0        0        0      860 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0006_unique_constraints.py
+-rw-r--r--   0        0        0     2477 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0007_terms.py
+-rw-r--r--   0        0        0      582 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py
+-rw-r--r--   0        0        0      609 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0009_remove_feedback.py
+-rw-r--r--   0        0        0      461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0010_term_confirmation_text.py
+-rw-r--r--   0        0        0      484 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0011_registration_accepted_terms.py
+-rw-r--r--   0        0        0      463 2022-02-21 20:54:12.455591 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0012_event_slug.py
+-rw-r--r--   0        0        0     2413 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0013_info_mailings.py
+-rw-r--r--   0        0        0     2839 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py
+-rw-r--r--   0        0        0     1252 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0015_registrationstate.py
+-rw-r--r--   0        0        0      475 2022-03-08 14:40:05.708390 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0016_eventregistration_states.py
+-rw-r--r--   0        0        0      419 2022-03-13 13:23:46.984225 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0017_fix_voucher_max_length.py
+-rw-r--r--   0        0        0     1724 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py
+-rw-r--r--   0        0        0      637 2022-06-19 20:01:59.822897 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0019_retractions.py
+-rw-r--r--   0        0        0      638 2022-06-24 14:54:41.596452 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0020_check_in.py
+-rw-r--r--   0        0        0     2201 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0021_checkpoint.py
+-rw-r--r--   0        0        0      681 2022-07-08 20:57:59.622407 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py
+-rw-r--r--   0        0        0      452 2023-07-02 13:19:00.183869 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0023_eventregistration_cost.py
+-rw-r--r--   0        0        0      430 2023-07-02 13:19:00.183869 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0024_add_cost_to_registration.py
+-rw-r--r--   0        0        0     2525 2023-07-29 20:46:19.646976 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0025_add_managed_by_label.py
+-rw-r--r--   0        0        0        0 2021-11-30 15:14:06.498459 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/__init__.py
+-rw-r--r--   0        0        0    16558 2023-07-02 13:19:00.183869 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/models.py
+-rw-r--r--   0        0        0     1333 2022-06-19 21:06:49.061623 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/predicates.py
+-rw-r--r--   0        0        0      732 2022-03-06 19:51:43.057119 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/preferences.py
+-rw-r--r--   0        0        0     9079 2022-06-30 15:18:35.332204 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/rules.py
+-rw-r--r--   0        0        0     1975 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/schema.py
+-rw-r--r--   0        0        0       51 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/settings.py
+-rw-r--r--   0        0        0     1076 2023-06-07 12:34:32.229375 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/static/css/paweljong.css
+-rw-r--r--   0        0        0      481 2022-06-27 10:59:54.101694 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/static/js/paweljong/checkpoint.js
+-rw-r--r--   0        0        0      597 2022-06-27 10:59:54.101694 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js
+-rw-r--r--   0        0        0     4445 2023-06-07 12:34:32.229375 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/tables.py
+-rw-r--r--   0        0        0      266 2022-03-01 20:03:12.342378 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/tasks.py
+-rw-r--r--   0        0        0     1316 2022-02-22 22:51:08.579836 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/account_wizard.html
+-rw-r--r--   0        0        0      592 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/create.html
+-rw-r--r--   0        0        0     3556 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/detail.html
+-rw-r--r--   0        0        0      585 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/edit.html
+-rw-r--r--   0        0        0     2480 2023-06-07 12:34:32.229375 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/full.html
+-rw-r--r--   0        0        0      568 2021-11-30 15:38:18.987000 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/list.html
+-rw-r--r--   0        0        0      915 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/manage.html
+-rw-r--r--   0        0        0      576 2022-06-27 10:59:54.101694 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html
+-rw-r--r--   0        0        0     5118 2023-06-07 12:34:32.229375 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_start.html
+-rw-r--r--   0        0        0     1640 2022-02-21 20:56:23.799158 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html
+-rw-r--r--   0        0        0     1876 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html
+-rw-r--r--   0        0        0      312 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/registered.html
+-rw-r--r--   0        0        0      535 2022-06-19 21:06:49.061623 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/terms.html
+-rw-r--r--   0        0        0      599 2022-03-08 14:40:05.708390 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html
+-rw-r--r--   0        0        0    13116 2022-06-28 20:06:29.947789 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html
+-rw-r--r--   0        0        0      514 2022-03-06 19:55:13.296748 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html
+-rw-r--r--   0        0        0      513 2022-03-01 20:03:12.342378 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html
+-rw-r--r--   0        0        0      508 2022-03-01 20:03:12.342378 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/edit.html
+-rw-r--r--   0        0        0      483 2022-03-01 20:03:12.342378 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/list.html
+-rw-r--r--   0        0        0     6730 2022-03-13 13:23:46.984225 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html
+-rw-r--r--   0        0        0     1461 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/corona.html
+-rw-r--r--   0        0        0     3192 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html
+-rw-r--r--   0        0        0     1947 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html
+-rw-r--r--   0        0        0     1081 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html
+-rw-r--r--   0        0        0      494 2021-11-30 15:38:18.987000 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/manage.html
+-rw-r--r--   0        0        0     1025 2022-06-21 19:40:35.903740 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/voucher.html
+-rw-r--r--   0        0        0      505 2021-11-30 15:38:18.987000 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/register.html
+-rw-r--r--   0        0        0     2434 2022-02-22 22:51:08.583835 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/register_start.html
+-rw-r--r--   0        0        0      506 2022-03-08 14:40:05.708390 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/chip.html
+-rw-r--r--   0        0        0      525 2022-03-08 14:40:05.708390 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html
+-rw-r--r--   0        0        0      520 2022-03-08 14:40:05.708390 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html
+-rw-r--r--   0        0        0      507 2022-03-08 14:40:05.708390 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/list.html
+-rw-r--r--   0        0        0      497 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/term/create.html
+-rw-r--r--   0        0        0      492 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/term/edit.html
+-rw-r--r--   0        0        0      451 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/term/list.html
+-rw-r--r--   0        0        0      594 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/create.html
+-rw-r--r--   0        0        0      590 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html
+-rw-r--r--   0        0        0      939 2022-06-21 19:41:29.939654 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/list.html
+-rw-r--r--   0        0        0     2272 2023-07-02 13:19:00.183869 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/account_registered.email
+-rw-r--r--   0        0        0     2365 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_created.email
+-rw-r--r--   0        0        0       94 2022-03-06 19:55:13.296748 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_notification.email
+-rw-r--r--   0        0        0     3879 2022-03-13 13:23:46.984225 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_registered.email
+-rw-r--r--   0        0        0       94 2022-03-01 20:03:12.342378 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/info_mailing.email
+-rw-r--r--   0        0        0      235 2022-02-21 09:18:10.136166 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templatetags/coerce.py
+-rw-r--r--   0        0        0     5452 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/urls.py
+-rw-r--r--   0        0        0    38484 2023-07-29 20:46:15.310966 aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/views.py
+-rw-r--r--   0        0        0     1601 2023-07-29 20:46:25.746991 aleksis_app_paweljong-3.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 aleksis_app_paweljong-3.0.dev1/PKG-INFO
```

### Comparing `aleksis_app_paweljong-2.0.dev2/CHANGELOG.rst` & `aleksis_app_paweljong-3.0.dev1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/LICENCE.rst` & `aleksis_app_paweljong-3.0.dev1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/README.rst` & `aleksis_app_paweljong-3.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/apps.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/data_checks.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/filters.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/forms.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,29 +379,29 @@
 
         for field in event.terms.all():
             field_instance = forms.BooleanField(
                 required=True,
                 label=field.confirmation_text,
             )
             self.fields[f"consent_{field.pk}"] = field_instance
-            node = Row(f"consent_{field.pk}")
+            node = f"consent_{field.pk}"
             self.add_node_to_layout(node)
 
         if event.date_retraction:
             field_instance = forms.BooleanField(
                 required=True,
                 label=_(
                     "I confirm that the retraction of the registration is not possible anymore "
                     "after {}"
                 ).format(
                     dateformat.format(event.date_retraction, formats.get_format("DATE_FORMAT"))
                 ),
             )
             self.fields["retraction_deadline"] = field_instance
-            node = Row("retraction_deadline")
+            node = "retraction_deadline"
             self.add_node_to_layout(node)
 
 
 class EditEventRegistrationForm(forms.ModelForm):
 
     layout = Layout(
         Row("event", "person"),
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/frontend/index.js` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/frontend/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -51,19 +51,16 @@
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "paweljong.eventDetailByName",
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
         path: "event/:slug/checkpoint/",
-        component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
+        component: () => import("./components/event/Checkpoint.vue"),
         name: "paweljong.eventByNameCheckpoint",
-        props: {
-            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-        },
     }, {
         path: "event/:slug/start/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "paweljong.registerEventBySlugStart",
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/frontend/messages/en.json` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0001_initial.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by Django 3.2.9 on 2021-11-30 15:23
 
-import django.contrib.sites.managers
+import aleksis.core.managers
 from django.db import migrations, models
 import django.db.models.deletion
 import localflavor.generic.models
 
 
 class Migration(migrations.Migration):
 
@@ -31,15 +31,15 @@
                 ('cost', models.IntegerField(verbose_name='Cost in €')),
                 ('max_participants', models.PositiveSmallIntegerField(verbose_name='Maximum participants')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.CreateModel(
             name='Voucher',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('extended_data', models.JSONField(default=dict, editable=False)),
@@ -53,30 +53,30 @@
                 ('used_person_uid', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, related_name='used_vouchers', to='core.person', verbose_name='Used by')),
             ],
             options={
                 'verbose_name': 'Vouchers',
                 'verbose_name_plural': 'Vouchers',
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.CreateModel(
             name='FeedbackAspect',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('extended_data', models.JSONField(default=dict, editable=False)),
                 ('aspect', models.CharField(max_length=100)),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.CreateModel(
             name='EventRegistration',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('extended_data', models.JSONField(default=dict, editable=False)),
@@ -95,15 +95,15 @@
                 ('voucher', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, to='paweljong.voucher', verbose_name='Voucher')),
             ],
             options={
                 'verbose_name': 'Registration',
                 'verbose_name_plural': 'Registrations',
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.CreateModel(
             name='EventFeedback',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('extended_data', models.JSONField(default=dict, editable=False)),
@@ -117,15 +117,15 @@
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'verbose_name': 'Event feedback',
                 'verbose_name_plural': 'Event feedbacks',
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.AddField(
             model_name='event',
             name='feedback_aspects',
             field=models.ManyToManyField(related_name='event', to='paweljong.FeedbackAspect', verbose_name='Feedback aspects'),
         ),
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0004_richtext_field_information.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0006_unique_constraints.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0006_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0007_terms.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0007_terms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.2.12 on 2022-02-20 15:24
 
 import ckeditor.fields
-import django.contrib.sites.managers
+import aleksis.core.managers
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
@@ -50,15 +50,15 @@
                 ('term', ckeditor.fields.RichTextField(verbose_name='Term')),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.AddField(
             model_name='event',
             name='terms',
             field=models.ManyToManyField(blank=True, related_name='event', to='paweljong.Terms', verbose_name='Terms'),
         ),
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0008_remove_terms_from_event.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0009_remove_feedback.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0009_remove_feedback.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0013_info_mailings.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0013_info_mailings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.2.12 on 2022-03-01 15:19
 
 import ckeditor.fields
-import django.contrib.sites.managers
+import aleksis.core.managers
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
@@ -35,15 +35,15 @@
                 ('sent_to', models.ManyToManyField(blank=True, editable=False, related_name='received_info_mailings', to='core.Person', verbose_name='Sent to persons')),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.AddField(
             model_name='event',
             name='info_mailings',
             field=models.ManyToManyField(blank=True, related_name='events', to='paweljong.InfoMailing', verbose_name='Info mailings'),
         ),
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0014_move_sent_to_to_through.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by Django 3.2.12 on 2022-03-02 19:50
 
-import django.contrib.sites.managers
+import aleksis.core.managers
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 def migrate_to_new_through(apps, schema_editor):
     Event = apps.get_model("paweljong", "Event")
     EventRegistration = apps.get_model("paweljong", "EventRegistration")
@@ -41,15 +41,15 @@
                 ('sent_to', models.ManyToManyField(blank=True, editable=False, related_name='received_info_mailings', to='core.Person', verbose_name='Sent to persons')),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
         migrations.AddField(
             model_name='event',
             name='info_mailings_new',
             field=models.ManyToManyField(blank=True, related_name='events', through='paweljong.EventInfoMailingThrough', to='paweljong.InfoMailing', verbose_name='Info mailings'),
         ),
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0015_registrationstate.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0015_registrationstate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.2.12 on 2022-03-06 20:09
 
 import colorfield.fields
-import django.contrib.sites.managers
+import aleksis.core.managers
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
@@ -23,11 +23,11 @@
                 ('colour', colorfield.fields.ColorField(blank=True, default='', image_field=None, max_length=18, samples=None, verbose_name='Colour')),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
     ]
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0018_payment_with_tezor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Generated by Django 3.2.12 on 2022-03-11 23:23
 
 from django.db import migrations, models
 
 from payments import PaymentStatus
 
 def create_invoices(apps, schema_editor):
-    db_alias = schema_editor.connection.alias
-
     Person = apps.get_model("core", "Person")
     EventRegistration = apps.get_model("paweljong", "EventRegistration")
     SEPAMandate = apps.get_model("djp_sepa", "SEPAMandate")
 
     from aleksis.apps.paweljong.models import EventRegistration as RealEventRegistration
 
     EventRegistration.get_invoice = RealEventRegistration.get_invoice
     EventRegistration._get_total_amount = RealEventRegistration._get_total_amount
     EventRegistration.get_purchased_items = RealEventRegistration.get_purchased_items
     Person.addressing_name = property(lambda p: p.first_name + " " + p.last_name)
 
-    for registration in EventRegistration.objects.using(db_alias).all():
+    for registration in EventRegistration._base_manager.all():
         invoice = registration.get_invoice()
         invoice.status = PaymentStatus.PREAUTH
         if registration.accept_sepa:
             invoice.variant = "sdd"
             SEPAMandate.objects.create(payment_id=invoice.pk, account_holder=f"{registration.person.addressing_name}", iban=registration.iban, bic="XXXXXXXXXXX", date=registration.date_registered)
         else:
             invoice.variant = "pledge"
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0019_retractions.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0019_retractions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0020_check_in.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0020_check_in.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0021_checkpoint.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0021_checkpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by Django 3.2.13 on 2022-06-24 18:31
 
-import django.contrib.sites.managers
+import aleksis.core.managers
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
@@ -33,11 +33,11 @@
                 ('checked_by', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='event_checkpoints_created', to='core.person', verbose_name='Checked by person')),
                 ('site', models.ForeignKey(default=1, editable=False, on_delete=django.db.models.deletion.CASCADE, to='sites.site')),
             ],
             options={
                 'abstract': False,
             },
             managers=[
-                ('objects', django.contrib.sites.managers.CurrentSiteManager()),
+                ('objects', aleksis.core.managers.AlekSISBaseManager()),
             ],
         ),
     ]
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/migrations/0022_send_to_retracted_or_not_checked_in.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/models.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/predicates.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/preferences.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/rules.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/static/css/paweljong.css` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/static/css/paweljong.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/static/js/paweljong/qrscanner.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/tables.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/account_wizard.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/account_wizard.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/checkpoint.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/create.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 {% extends "core/base.html" %}
 {% load material_form i18n any_js %}
 
-{% block page_title %}{% blocktrans %}Checkpoint{% endblocktrans %}{% endblock %}
-{% block browser_title %}{% blocktrans %}Checkpoint{% endblocktrans %}{% endblock %}
+{% block page_title %}{% blocktrans %}Create event{% endblocktrans %}{% endblock %}
+{% block browser_title %}{% blocktrans %}Create event{% endblocktrans %}{% endblock %}
 
 {% block extra_head %}
     {{ form.media.css }}
+    {% include_css "select2-materialize" %}
 {% endblock %}
 
 {% block content %}
 
   <form method="post">
     {% csrf_token %}
-    {% form form=form %}{% form %}
+    {% form form=form %}{% endform %}
     {% include "core/partials/save_button.html" %}
   </form>
-
-  <div id="qr-reader" data-target-input="username"></div>
-
+  {% include_js "select2-materialize" %}
   {{ form.media.js }}
 
 {% endblock %}
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/create.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/create.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 {% extends "core/base.html" %}
 {% load material_form i18n any_js %}
 
-{% block page_title %}{% blocktrans %}Create event{% endblocktrans %}{% endblock %}
-{% block browser_title %}{% blocktrans %}Create event{% endblocktrans %}{% endblock %}
+{% block page_title %}{% blocktrans %}Create voucher{% endblocktrans %}{% endblock %}
+{% block browser_title %}{% blocktrans %}Create voucher{% endblocktrans %}{% endblock %}
 
 {% block extra_head %}
     {{ form.media.css }}
     {% include_css "select2-materialize" %}
 {% endblock %}
 
 {% block content %}
-
   <form method="post">
     {% csrf_token %}
     {% form form=form %}{% endform %}
     {% include "core/partials/save_button.html" %}
   </form>
-  {% include_js "select2-materialize" %}
   {{ form.media.js }}
-
+  {% include_js "select2-materialize" %}
 {% endblock %}
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/detail.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/detail.html`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
      {% if can_change_event_rule %}
       <a href="{% url 'edit_event_by_slug' event.slug %}" class="btn waves-effect waves-light">
         <i class="material-icons left iconify" data-icon="mdi:edit"></i>
         {% trans "Edit" %}
       </a>
      {% endif %}
      {% if can_checkpoint_rule %}
-       <a href="{% url 'event_by_name_checkpoint' event.slug %}" class="btn waves-effect waves-light">
+     <a href="/app/paweljong/event/{{ event.slug }}/checkpoint" class="btn waves-effect waves-light">
          <i class="material-icons left iconify" data-icon="mdi:access-point-check"></i>
          {% trans "Checkpoint" %}
        </a>
      {% endif %}
     </p>
 
     <div class="card">
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/edit.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/full.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/list.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/manage.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/manage.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/persons_group.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/register_start.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_start.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/register_wizard_consent.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event/terms.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event/terms.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/event_registration/notification.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/info_mailing/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/invoice_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/corona.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/corona.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_attendance.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_participants.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/list_sign.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/print/voucher.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/print/voucher.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/register_start.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/register_start.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/registration_state/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/voucher/create.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/edit.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "core/base.html" %}
 {% load material_form i18n any_js %}
 
-{% block page_title %}{% blocktrans %}Create voucher{% endblocktrans %}{% endblock %}
-{% block browser_title %}{% blocktrans %}Create voucher{% endblocktrans %}{% endblock %}
+{% block page_title %}{% blocktrans %}Edit voucher{% endblocktrans %}{% endblock %}
+{% block browser_title %}{% blocktrans %}Edit voucher{% endblocktrans %}{% endblock %}
 
 {% block extra_head %}
     {{ form.media.css }}
     {% include_css "select2-materialize" %}
 {% endblock %}
 
 {% block content %}
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/paweljong/voucher/list.html` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/paweljong/voucher/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/account_registered.email` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/account_registered.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/event_created.email` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_created.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/templates/templated_email/event_registered.email` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/templates/templated_email/event_registered.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/urls.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,14 @@
         "group_persons/<int:pk>/add/",
         views.PersonGroupView.as_view(),
         name="add_persons_to_group",
     ),
     path("event/<slug:slug>/", views.EventFullView.as_view(), name="event_by_name"),
     path("event/<slug:slug>/detail/", views.EventDetailView.as_view(), name="event_detail_by_name"),
     path(
-        "event/<slug:slug>/checkpoint/",
-        views.EventCheckpointView.as_view(),
-        name="event_by_name_checkpoint",
-    ),
-    path(
         "event/<slug:slug>/start/",
         views.RegisterEventStart.as_view(),
         name="register_event_by_slug_start",
     ),
     path("misc/set_email_needed/<slug:slug>/", views.set_email_needed, name="set_email_needed"),
     path("misc/set_email_needed/", views.set_email_needed, name="set_email_needed_no_slug"),
     path(
```

### Comparing `aleksis_app_paweljong-2.0.dev2/aleksis/apps/paweljong/views.py` & `aleksis_app_paweljong-3.0.dev1/aleksis/apps/paweljong/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1008,63 +1008,14 @@
 
         return super().form_valid(self)
 
     def get_success_url(self):
         return reverse("add_persons_to_group", kwargs={"pk": self.kwargs["pk"]})
 
 
-class EventCheckpointView(PermissionRequiredMixin, FormView):
-
-    template_name = "paweljong/event/checkpoint.html"
-    permission_required = "paweljong.event_checkpoint_rule"
-    form_class = EventCheckpointForm
-
-    def get_object(self):
-        return Event.objects.get(slug=self.kwargs["slug"])
-
-    def get_initial(self):
-        initial = super().get_initial() or {}
-        if "comment" in self.request.GET:
-            initial["comment"] = self.request.GET.get("comment")
-        return initial
-
-    def form_valid(self, form):
-        checkpoint = Checkpoint()
-
-        checkpoint.event = get_object_or_404(Event, slug=self.kwargs["slug"])
-        try:
-            checkpoint.person = Person.objects.get(user__username=form.cleaned_data["username"])
-        except Person.DoesNotExist:
-            messages.error(self.request, _("The provided username is not linked to a person."))
-        checkpoint.checked_by = self.request.user.person
-
-        checkpoint.comment = form.cleaned_data["comment"]
-        checkpoint.timestamp = timezone.now()
-        if form.cleaned_data["use_latlon"]:
-            checkpoint.lat = form.cleaned_data["lat"]
-            checkpoint.lon = form.cleaned_data["lon"]
-
-        checkpoint.save()
-        messages.success(
-            self.request,
-            _("{} successfully checked for {}.").format(
-                str(checkpoint.person), str(checkpoint.comment)
-            ),
-        )
-        self._comment = checkpoint.comment
-        return super().form_valid(self)
-
-    def get_success_url(self):
-        return (
-            reverse("event_by_name_checkpoint", kwargs={"slug": self.kwargs["slug"]})
-            + "?"
-            + urlencode({"comment": self._comment})
-        )
-
-
 class ViewTerms(PermissionRequiredMixin, DetailView):
 
     context_object_name = "event"
     template_name = "paweljong/event/terms.html"
     permission_required = "paweljong.can_view_terms_rule"
     model = Event
     slug_field = "slug"
```

### Comparing `aleksis_app_paweljong-2.0.dev2/pyproject.toml` & `aleksis_app_paweljong-3.0.dev1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Paweljong"
-version = "2.0.dev2"
+version = "3.0.dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "AlekSIS (School Information System) — App Paweljong (Camp/Event management)"
@@ -21,20 +21,21 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0b0"
+aleksis-core = "^4.0.0.dev0"
 django-localflavor = "^3.0"
-django-formtools = "2.3"
+django-formtools = "2.2"
 django-starfield = "^1.0"
-aleksis-app-postbuero = { version = "2.0.1.dev0" , allow-prereleases = true }
-aleksis-app-tezor = {version = "2.0dev1", allow-prereleases = true }
+aleksis-app-postbuero = { version = "^3.0.dev0", allow-prereleases = true }
+aleksis-app-tezor = { version = "^2.0.dev0", allow-prereleases = true }
+aleksis-app-kort = { version = "^1.0.dev0" , allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 paweljong = "aleksis.apps.paweljong.apps:DefaultConfig"
```

### Comparing `aleksis_app_paweljong-2.0.dev2/PKG-INFO` & `aleksis_app_paweljong-3.0.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: aleksis-app-paweljong
-Version: 2.0.dev2
+Version: 3.0.dev1
 Summary: AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 Home-page: https://hacknfun.camp
 License: EUPL-1.2-or-later
 Author: Tom Teichler
 Author-email: tom.teichler@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-app-postbuero (==2.0.1.dev0)
-Requires-Dist: aleksis-app-tezor (==2.0dev1)
-Requires-Dist: aleksis-core (>=3.0b0,<4.0)
-Requires-Dist: django-formtools (==2.3)
+Requires-Dist: aleksis-app-kort (==1.*)
+Requires-Dist: aleksis-app-postbuero (==3.*)
+Requires-Dist: aleksis-app-tezor (==2.*)
+Requires-Dist: aleksis-core (==4.*)
+Requires-Dist: django-formtools (==2.2)
 Requires-Dist: django-localflavor (>=3.0,<4.0)
 Requires-Dist: django-starfield (>=1.0,<2.0)
 Project-URL: Repository, https://edugit.org/Teckids/hacknfun/AlekSIS-App-Paweljong
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Paweljong (Camp/Event management)
 ==================================================================================================
```

