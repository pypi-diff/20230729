# Comparing `tmp/mia-accounting-1.5.6.tar.gz` & `tmp/mia-accounting-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.5.6.tar", last modified: Tue May 23 01:08:21 2023, max compression
+gzip compressed data, was "mia-accounting-1.5.7.tar", last modified: Sat Jul 29 05:25:09 2023, max compression
```

## Comparing `mia-accounting-1.5.6.tar` & `mia-accounting-1.5.7.tar`

### file list

```diff
@@ -1,305 +1,306 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.6/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.6/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.6/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.6/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.6/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.6/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.6/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     8529 2023-05-23 01:07:11.000000 mia-accounting-1.5.6/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.6/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.6/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.6/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.6/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.6/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.6/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.6/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-23 01:08:21.610039 mia-accounting-1.5.6/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-05-23 01:07:41.000000 mia-accounting-1.5.6/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.6/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.6/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.6/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.6/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.6/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.6/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.6/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.6/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.6/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.6/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.6/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.6/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.586039 mia-accounting-1.5.6/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.6/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.6/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.6/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.6/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unmatched_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.586039 mia-accounting-1.5.6/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.6/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.6/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.6/src/accounting/report/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.6/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/report/utils/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.6/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.6/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.586039 mia-accounting-1.5.6/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.6/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.6/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.6/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.6/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1025 2023-05-23 01:03:30.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-05-23 01:03:29.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1140 2023-05-23 01:03:30.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14561 2023-05-22 10:32:23.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4231 2023-05-22 09:36:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1125 2023-05-23 01:03:29.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1118 2023-05-23 01:03:55.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4345 2023-05-22 09:36:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5630 2023-05-17 13:41:20.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied.html
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     6959 2023-05-23 00:59:42.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.6/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.6/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.602039 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.602039 mia-accounting-1.5.6/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.6/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.6/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.6/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     3749 2023-05-23 00:59:42.000000 mia-accounting-1.5.6/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.6/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.6/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.602039 mia-accounting-1.5.6/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)      107 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.6/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.6/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32948 2023-05-22 23:22:24.000000 mia-accounting-1.5.6/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23998 2023-05-22 23:24:38.000000 mia-accounting-1.5.6/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    16282 2023-05-22 23:26:32.000000 mia-accounting-1.5.6/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   105500 2023-05-23 00:40:17.000000 mia-accounting-1.5.6/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    42546 2023-05-23 00:01:57.000000 mia-accounting-1.5.6/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    16950 2023-05-23 00:10:42.000000 mia-accounting-1.5.6/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4649 2023-05-23 00:59:42.000000 mia-accounting-1.5.6/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13324 2023-05-23 00:02:48.000000 mia-accounting-1.5.6/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3367 2023-05-17 11:57:23.000000 mia-accounting-1.5.6/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.6/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6656 2023-05-23 00:22:47.000000 mia-accounting-1.5.6/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.6/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.6/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.6/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.6/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.6/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    28011 2023-05-23 00:12:12.000000 mia-accounting-1.5.6/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15328 2023-05-23 00:16:21.000000 mia-accounting-1.5.6/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5470 2023-05-22 23:23:54.000000 mia-accounting-1.5.6/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16955 2023-05-22 23:52:24.000000 mia-accounting-1.5.6/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.7/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.7/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.7/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.801157 mia-accounting-1.5.7/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.7/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.7/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.801157 mia-accounting-1.5.7/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.801157 mia-accounting-1.5.7/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.7/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.801157 mia-accounting-1.5.7/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.7/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-07-29 02:00:53.000000 mia-accounting-1.5.7/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2577 2023-07-29 05:07:08.000000 mia-accounting-1.5.7/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     9098 2023-07-29 05:24:52.000000 mia-accounting-1.5.7/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.7/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.7/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.7/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.7/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.7/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.7/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.7/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.805157 mia-accounting-1.5.7/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3105 2023-07-29 05:12:12.000000 mia-accounting-1.5.7/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.805157 mia-accounting-1.5.7/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.7/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.7/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.7/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7222 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.7/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.7/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.805157 mia-accounting-1.5.7/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.7/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1863 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.7/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.7/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.7/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3453 2023-07-29 05:11:43.000000 mia-accounting-1.5.7/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.805157 mia-accounting-1.5.7/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.7/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.7/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.7/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.7/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.7/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.805157 mia-accounting-1.5.7/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.7/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.7/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3210 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.805157 mia-accounting-1.5.7/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.7/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.809157 mia-accounting-1.5.7/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.7/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.7/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24539 2023-07-29 02:03:46.000000 mia-accounting-1.5.7/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3360 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.7/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.809157 mia-accounting-1.5.7/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.7/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.7/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13072 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.7/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3861 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32627 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.809157 mia-accounting-1.5.7/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.7/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.7/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.7/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.809157 mia-accounting-1.5.7/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.7/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.7/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.809157 mia-accounting-1.5.7/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.7/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4523 2023-06-05 14:43:35.000000 mia-accounting-1.5.7/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.813157 mia-accounting-1.5.7/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.7/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17973 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18791 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11738 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8122 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8845 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5185 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5166 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.7/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.813157 mia-accounting-1.5.7/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.7/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.7/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.7/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.7/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.7/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.7/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.7/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.7/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.7/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.813157 mia-accounting-1.5.7/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.7/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.7/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.7/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.7/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.7/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.7/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.7/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.7/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1025 2023-05-23 01:32:48.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1575 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-05-23 01:32:48.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-07-26 12:27:46.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1140 2023-05-23 01:32:48.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.817156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14561 2023-05-22 10:32:23.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3236 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4231 2023-05-22 09:36:19.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3785 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1125 2023-05-23 01:32:48.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1118 2023-05-23 01:32:48.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.821156 mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4345 2023-05-22 09:36:19.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.825156 mia-accounting-1.5.7/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-07-26 12:27:46.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.825156 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1690 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1275 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1754 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5624 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4829 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4594 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4190 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4934 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4032 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3704 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3031 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3831 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3028 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6947 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.825156 mia-accounting-1.5.7/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-07-29 00:55:31.000000 mia-accounting-1.5.7/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.7/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.825156 mia-accounting-1.5.7/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-07-29 00:56:45.000000 mia-accounting-1.5.7/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-07-29 00:56:45.000000 mia-accounting-1.5.7/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.825156 mia-accounting-1.5.7/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-07-29 00:56:45.000000 mia-accounting-1.5.7/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-07-29 05:07:08.000000 mia-accounting-1.5.7/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.829156 mia-accounting-1.5.7/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.7/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.7/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.7/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.7/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3920 2023-07-29 02:03:45.000000 mia-accounting-1.5.7/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7077 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11777 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.7/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.7/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.7/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2063 2023-07-29 02:11:47.000000 mia-accounting-1.5.7/src/accounting/utils/title_case.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5022 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.829156 mia-accounting-1.5.7/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-07-29 05:25:09.000000 mia-accounting-1.5.7/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11469 2023-07-29 05:25:09.000000 mia-accounting-1.5.7/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-07-29 05:25:09.000000 mia-accounting-1.5.7/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)      107 2023-07-29 05:25:09.000000 mia-accounting-1.5.7/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-07-29 05:25:09.000000 mia-accounting-1.5.7/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.829156 mia-accounting-1.5.7/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4447 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4403 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    33845 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9725 2023-07-29 05:07:21.000000 mia-accounting-1.5.7/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24729 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16527 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   107441 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    43835 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17427 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18160 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.829156 mia-accounting-1.5.7/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4589 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.7/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14076 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3409 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13090 2023-07-29 02:11:44.000000 mia-accounting-1.5.7/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.7/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6689 2023-06-03 03:11:45.000000 mia-accounting-1.5.7/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1247 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.7/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.7/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.7/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2685 2023-06-10 02:42:19.000000 mia-accounting-1.5.7/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2237 2023-06-10 02:43:08.000000 mia-accounting-1.5.7/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3467 2023-06-10 02:43:08.000000 mia-accounting-1.5.7/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.797157 mia-accounting-1.5.7/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-07-29 05:25:09.833156 mia-accounting-1.5.7/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2237 2023-06-10 02:43:08.000000 mia-accounting-1.5.7/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3467 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    29015 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15723 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5421 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16945 2023-07-29 02:11:45.000000 mia-accounting-1.5.7/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.5.6/LICENSE` & `mia-accounting-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/MANIFEST.in` & `mia-accounting-1.5.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/PKG-INFO` & `mia-accounting-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.6
+Version: 1.5.7
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.6/README.rst` & `mia-accounting-1.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/Makefile` & `mia-accounting-1.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/make.bat` & `mia-accounting-1.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.account.rst` & `mia-accounting-1.5.7/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.base_account.rst` & `mia-accounting-1.5.7/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.currency.rst` & `mia-accounting-1.5.7/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.5.7/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.5.7/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.5.7/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.option.rst` & `mia-accounting-1.5.7/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.report.period.rst` & `mia-accounting-1.5.7/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.report.reports.rst` & `mia-accounting-1.5.7/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.report.rst` & `mia-accounting-1.5.7/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.report.utils.rst` & `mia-accounting-1.5.7/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.rst` & `mia-accounting-1.5.7/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/accounting.utils.rst` & `mia-accounting-1.5.7/docs/source/accounting.utils.rst`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,22 @@
 -----------------------------------
 
 .. automodule:: accounting.utils.strip_text
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.utils.title\_case module
+-----------------------------------
+
+.. automodule:: accounting.utils.title_case
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.utils.user module
 ----------------------------
 
 .. automodule:: accounting.utils.user
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.5.6/docs/source/changelog.rst` & `mia-accounting-1.5.7/docs/source/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 Change Log
 ==========
 
 
+Version 1.5.7
+-------------
+
+Released 2023/7/29
+
+Revised account title capitalization to capitalize account titles
+upon initialization of base accounts, rather than when displaying
+the accounts.  This prevents the system from incorrectly
+capitalizing titles of user-added accounts.
+
+For existing installation, run the ``accounting-titleize`` console
+command to capitalize the existing account titles that were already
+initialized.
+
+Other fixes:
+
+* Added missing documentation to the global variables, class
+  properties, and object properties.
+* Various minor fixes.
+
+
 Version 1.5.6
 -------------
 
 Released 2023/5/23
 
 Bug fixes.
```

### Comparing `mia-accounting-1.5.6/docs/source/conf.py` & `mia-accounting-1.5.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/examples.rst` & `mia-accounting-1.5.7/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/history.rst` & `mia-accounting-1.5.7/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/index.rst` & `mia-accounting-1.5.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/docs/source/intro.rst` & `mia-accounting-1.5.7/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/pyproject.toml` & `mia-accounting-1.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/__init__.py` & `mia-accounting-1.5.7/src/accounting/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 from flask import Flask, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 
 from accounting.utils.user import UserUtilityInterface
 
-VERSION: str = "1.5.6"
+VERSION: str = "1.5.7"
 """The package version."""
 db: SQLAlchemy = SQLAlchemy()
 """The database instance."""
 data_dir: Path = Path(__file__).parent / "data"
 """The data directory."""
 
 
@@ -59,16 +59,17 @@
 
     from .template_globals import currency_options, default_currency_code
     bp.add_app_template_global(currency_options,
                                "accounting_currency_options")
     bp.add_app_template_global(default_currency_code,
                                "accounting_default_currency_code")
 
-    from .commands import init_db_command
+    from .commands import init_db_command, titleize_command
     app.cli.add_command(init_db_command)
+    app.cli.add_command(titleize_command)
 
     from . import locale
     locale.init_app(app, bp)
 
     from .utils import permission
     permission.init_app(bp, user_utils)
```

### Comparing `mia-accounting-1.5.6/src/accounting/account/__init__.py` & `mia-accounting-1.5.7/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/account/commands.py` & `mia-accounting-1.5.7/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/account/converters.py` & `mia-accounting-1.5.7/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/account/forms.py` & `mia-accounting-1.5.7/src/accounting/account/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,17 @@
 
     def __init__(self, base: BaseAccount):
         """Constructs the form to reorder the accounts under a base account.
 
         :param base: The base account.
         """
         self.base: BaseAccount = base
+        """The base account."""
         self.is_modified: bool = False
+        """Whether the order is modified."""
 
     def save_order(self) -> None:
         """Saves the order of the account.
 
         :return:
         """
         accounts: list[Account] = self.base.accounts
```

### Comparing `mia-accounting-1.5.6/src/accounting/account/queries.py` & `mia-accounting-1.5.7/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/account/views.py` & `mia-accounting-1.5.7/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/base_account/__init__.py` & `mia-accounting-1.5.7/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/base_account/commands.py` & `mia-accounting-1.5.7/src/accounting/base_account/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 import csv
 
 import sqlalchemy as sa
 
 from accounting import data_dir
 from accounting import db
 from accounting.models import BaseAccount, BaseAccountL10n
+from accounting.utils.title_case import title_case
 
 
 def init_base_accounts_command() -> None:
     """Initializes the base accounts."""
     if BaseAccount.query.first() is not None:
         return
 
     with open(data_dir / "base_accounts.csv") as fp:
         data: list[dict[str, str]] = [x for x in csv.DictReader(fp)]
     account_data: list[dict[str, str]] = [{"code": x["code"],
-                                           "title_l10n": x["title"]}
+                                           "title_l10n": title_case(x["title"])}
                                           for x in data]
     locales: list[str] = [x[5:] for x in data[0] if x.startswith("l10n-")]
     l10n_data: list[dict[str, str]] = [{"account_code": x["code"],
                                         "locale": y,
                                         "title": x[f"l10n-{y}"]}
                                        for x in data for y in locales]
     db.session.execute(sa.insert(BaseAccount), account_data)
```

### Comparing `mia-accounting-1.5.6/src/accounting/base_account/converters.py` & `mia-accounting-1.5.7/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/base_account/queries.py` & `mia-accounting-1.5.7/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/base_account/views.py` & `mia-accounting-1.5.7/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/currency/__init__.py` & `mia-accounting-1.5.7/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/currency/commands.py` & `mia-accounting-1.5.7/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/currency/converters.py` & `mia-accounting-1.5.7/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/currency/forms.py` & `mia-accounting-1.5.7/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/currency/queries.py` & `mia-accounting-1.5.7/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/currency/views.py` & `mia-accounting-1.5.7/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/data/base_accounts.csv` & `mia-accounting-1.5.7/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/forms.py` & `mia-accounting-1.5.7/src/accounting/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
     def __init__(self, message: str | LazyString):
         """Constructs the validator.
 
         :param message: The error message.
         """
         self.__message: str | LazyString = message
+        """The error message."""
 
     def __call__(self, form: FlaskForm, field: StringField) -> None:
         if field.data is None:
             return
         if re.match(r"^(?:[1235689]|7[5678])", field.data) \
                 and not field.data.startswith("3351-") \
                 and not field.data.startswith("3353-"):
@@ -81,14 +82,15 @@
 
     def __init__(self, message: str | LazyString):
         """Constructs the validator.
 
         :param message: The error message.
         """
         self.__message: str | LazyString = message
+        """The error message."""
 
     def __call__(self, form: FlaskForm, field: StringField) -> None:
         if field.data is None:
             return
         if re.match(r"^(?:[123489]|7[1234])", field.data) \
                 and not field.data.startswith("3351-") \
                 and not field.data.startswith("3353-"):
```

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/converters.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
 
         :param obj: The journal entry object.
         :return: None.
         """
         is_new: bool = obj.id is None
         if is_new:
             obj.id = new_id(JournalEntry)
-        self.date: DateField
         self.__set_date(obj, self.date.data)
         obj.note = self.note.data
 
         collector_cls: Type[LineItemCollector] = self.collector
         collector: collector_cls = collector_cls(self, obj)
         collector.collect()
```

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/forms/reorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 
     def __init__(self, date: dt.date):
         """Constructs the form to reorder the journal entries in a day.
 
         :param date: The date.
         """
         self.date: dt.date = date
+        """The date."""
         self.is_modified: bool = False
+        """Whether the order is modified."""
 
     def save_order(self) -> None:
         """Saves the order of the account.
 
         :return:
         """
         journal_entries: list[JournalEntry] = JournalEntry.query\
```

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/utils/description_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,19 @@
         """Constructs a recurring transaction.
 
         :param name: The name.
         :param description_template: The description template.
         :param account: The account.
         """
         self.name: str = name
+        """The name."""
         self.account: DescriptionAccount = DescriptionAccount(account, 0)
+        """The account."""
         self.description_template: str = description_template
+        """The description template."""
 
     @property
     def account_codes(self) -> list[str]:
         """Returns the account codes by the order of their frequencies.
 
         :return: The account codes by the order of their frequencies.
         """
```

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/journal_entry/views.py` & `mia-accounting-1.5.7/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/locale.py` & `mia-accounting-1.5.7/src/accounting/locale.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 from pathlib import Path
 
 from flask import Flask, Response, Blueprint
 from flask_babel import LazyString, Domain
 from flask_babel_js import JAVASCRIPT, c2js
 
 translation_dir: Path = Path(__file__).parent / "translations"
+"""The directory of the translation files."""
 domain: Domain = Domain(translation_directories=[translation_dir],
                         domain="accounting")
+"""The message domain."""
 
 
 def gettext(string, **variables) -> str:
     """A replacement of the Babel gettext() function..
 
     :param string: The message to translate.
     :param variables: The variable substitution.
@@ -116,10 +118,9 @@
 def init_app(app: Flask, bp: Blueprint) -> None:
     """Initializes the application.
 
     :param app: The Flask application.
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
-    bp.add_url_rule("/_jstrans.js", "babel_catalog",
-                    __babel_js_catalog_view)
+    bp.add_url_rule("/_jstrans.js", "babel_catalog", __babel_js_catalog_view)
     app.jinja_env.globals["A_"] = domain.gettext
```

### Comparing `mia-accounting-1.5.6/src/accounting/models.py` & `mia-accounting-1.5.7/src/accounting/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 
 
 class BaseAccount(db.Model):
     """A base account."""
     __tablename__ = "accounting_base_accounts"
     """The table name."""
     code: Mapped[str] = mapped_column(primary_key=True)
-    """The code."""
+    """The account code."""
     title_l10n: Mapped[str] = mapped_column("title")
     """The title."""
     l10n: Mapped[list[BaseAccountL10n]] \
         = db.relationship(back_populates="account", lazy=False)
     """The localized titles."""
     accounts: Mapped[list[Account]] = db.relationship(back_populates="base")
     """The descendant accounts under the base account."""
 
     def __str__(self) -> str:
         """Returns the string representation of the base account.
 
         :return: The string representation of the base account.
         """
-        return f"{self.code} {self.title.title()}"
+        return f"{self.code} {self.title}"
 
     @property
     def title(self) -> str:
         """Returns the title in the current locale.
 
         :return: The title in the current locale.
         """
@@ -83,15 +83,15 @@
     """A localized base account title."""
     __tablename__ = "accounting_base_accounts_l10n"
     """The table name."""
     account_code: Mapped[str] \
         = mapped_column(db.ForeignKey(BaseAccount.code, onupdate="CASCADE",
                                       ondelete="CASCADE"),
                         primary_key=True)
-    """The code of the account."""
+    """The account code."""
     account: Mapped[BaseAccount] = db.relationship(back_populates="l10n")
     """The account."""
     locale: Mapped[str] = mapped_column(primary_key=True)
     """The locale."""
     title: Mapped[str]
     """The localized title."""
 
@@ -147,15 +147,15 @@
     """The code of the net-change account,"""
 
     def __str__(self) -> str:
         """Returns the string representation of this account.
 
         :return: The string representation of this account.
         """
-        return f"{self.base_code}-{self.no:03d} {self.title.title()}"
+        return f"{self.base_code}-{self.no:03d} {self.title}"
 
     @property
     def code(self) -> str:
         """Returns the code.
 
         :return: The code.
         """
@@ -365,17 +365,17 @@
 
 
 class Currency(db.Model):
     """A currency."""
     __tablename__ = "accounting_currencies"
     """The table name."""
     code: Mapped[str] = mapped_column(primary_key=True)
-    """The code."""
+    """The currency code."""
     name_l10n: Mapped[str] = mapped_column("name")
-    """The name."""
+    """The currency name."""
     created_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
     """The date and time when this record was created."""
     created_by_id: Mapped[int] \
         = mapped_column(db.ForeignKey(user_pk_column, onupdate="CASCADE"))
     """The ID of the user who created the record."""
@@ -540,15 +540,15 @@
     __tablename__ = "accounting_journal_entries"
     """The table name."""
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=False)
     """The journal entry ID."""
     date: Mapped[dt.date]
     """The date."""
     no: Mapped[int] = mapped_column(default=text("1"))
-    """The account number under the date."""
+    """The journal entry number under the date."""
     note: Mapped[str | None]
     """The note."""
     created_at: Mapped[dt.datetime] \
         = mapped_column(db.DateTime(timezone=True),
                         server_default=db.func.now())
     """The date and time when this record was created."""
     created_by_id: Mapped[int] \
```

### Comparing `mia-accounting-1.5.6/src/accounting/option/__init__.py` & `mia-accounting-1.5.7/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/option/forms.py` & `mia-accounting-1.5.7/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/option/views.py` & `mia-accounting-1.5.7/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/__init__.py` & `mia-accounting-1.5.7/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/converters.py` & `mia-accounting-1.5.7/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/__init__.py` & `mia-accounting-1.5.7/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/chooser.py` & `mia-accounting-1.5.7/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/description.py` & `mia-accounting-1.5.7/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/month_end.py` & `mia-accounting-1.5.7/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/parser.py` & `mia-accounting-1.5.7/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/period.py` & `mia-accounting-1.5.7/src/accounting/report/period/period.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         :param end: The end date, or None till no end.
         """
         self.start: dt.date | None = start
         """The start of the period."""
         self.end: dt.date | None = end
         """The end of the period."""
         self.is_default: bool = False
-        """Whether the is the default period."""
+        """Whether this is the default period."""
         self.is_this_month: bool = False
         """Whether the period is this month."""
         self.is_last_month: bool = False
         """Whether the period is last month."""
         self.is_since_last_month: bool = False
         """Whether the period is since last month."""
         self.is_this_year: bool = False
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.5.7/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/period/specification.py` & `mia-accounting-1.5.7/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/__init__.py` & `mia-accounting-1.5.7/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.5.7/src/accounting/report/reports/balance_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,23 +141,25 @@
             .order_by(Account.base_code, Account.no)
         account_balances: list[sa.Row] \
             = db.session.execute(select_balance).all()
         self.__all_accounts: list[Account] = Account.query\
             .filter(sa.or_(Account.id.in_({x.id for x in account_balances}),
                            Account.base_code == "3351",
                            Account.base_code == "3353")).all()
+        """The accounts."""
         account_by_id: dict[int, Account] \
             = {x.id: x for x in self.__all_accounts}
         self.accounts: list[ReportAccount] \
             = [ReportAccount(account=account_by_id[x.id],
                              amount=x.balance,
                              url=ledger_url(self.__currency,
                                             account_by_id[x.id],
                                             self.__period))
                for x in account_balances]
+        """The accounts on the balance sheet."""
         self.__add_accumulated()
         self.__add_current_period()
         self.accounts.sort(key=lambda x: (x.account.base_code, x.account.no))
         for balance in self.accounts:
             if not balance.account.base_code.startswith("1"):
                 balance.amount = -balance.amount
         return self.accounts
@@ -448,19 +450,19 @@
     def __section_csv_rows(section: Section) -> list[CSVHalfRow]:
         """Gathers the CSV rows for a section.
 
         :param section: The section.
         :return: The CSV rows for the section.
         """
         rows: list[CSVHalfRow] \
-            = [CSVHalfRow(section.title.title.title(), None)]
+            = [CSVHalfRow(section.title.title, None)]
         for subsection in section.subsections:
-            rows.append(CSVHalfRow(f" {subsection.title.title.title()}", None))
+            rows.append(CSVHalfRow(f" {subsection.title.title}", None))
             for account in subsection.accounts:
-                rows.append(CSVHalfRow(f"  {str(account.account).title()}",
+                rows.append(CSVHalfRow(f"  {str(account.account)}",
                                        account.amount))
         return rows
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
 
         :return: The report as HTML.
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.5.7/src/accounting/report/reports/income_expenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,21 +403,21 @@
         """
         rows: list[CSVRow] = [CSVRow(gettext("Date"), gettext("Account"),
                                      gettext("Description"), gettext("Income"),
                                      gettext("Expense"), gettext("Balance"),
                                      gettext("Note"))]
         if self.__brought_forward is not None:
             rows.append(CSVRow(self.__brought_forward.date,
-                               str(self.__brought_forward.account).title(),
+                               str(self.__brought_forward.account),
                                self.__brought_forward.description,
                                self.__brought_forward.income,
                                self.__brought_forward.expense,
                                self.__brought_forward.balance,
                                None))
-        rows.extend([CSVRow(x.date, str(x.account).title(), x.description,
+        rows.extend([CSVRow(x.date, str(x.account), x.description,
                             x.income, x.expense, x.balance, x.note)
                      for x in self.__line_items])
         if self.__total is not None:
             rows.append(CSVRow(gettext("Total"), None, None,
                                self.__total.income, self.__total.expense,
                                self.__total.balance, None))
         return rows
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.5.7/src/accounting/report/reports/income_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         """
         self.title: BaseAccount = title
         """The title account."""
         self.subsections: list[Subsection] = []
         """The subsections in the section."""
         self.accumulated: AccumulatedTotal \
             = AccumulatedTotal(accumulated_title)
+        """The accumulated total."""
 
     @property
     def total(self) -> Decimal:
         """Returns the total of the section.
 
         :return: The total of the section.
         """
@@ -221,20 +222,20 @@
         titles: list[BaseAccount] = BaseAccount.query\
             .filter(BaseAccount.code.in_({"4", "5", "6", "7", "8", "9"})).all()
         subtitles: list[BaseAccount] = BaseAccount.query\
             .filter(BaseAccount.code.in_({x.account.base_code[:2]
                                           for x in balances})).all()
 
         total_titles: dict[str, str] \
-            = {"4": gettext("total operating revenue"),
-               "5": gettext("gross income"),
-               "6": gettext("operating income"),
-               "7": gettext("before tax income"),
-               "8": gettext("after tax income"),
-               "9": gettext("net income or loss for current period")}
+            = {"4": gettext("Total Operating Revenue"),
+               "5": gettext("Gross Income"),
+               "6": gettext("Operating Income"),
+               "7": gettext("Before Tax Income"),
+               "8": gettext("After Tax Income"),
+               "9": gettext("Net Income or Loss for Current Period")}
 
         sections: dict[str, Section] \
             = {x.code: Section(x, total_titles[x.code]) for x in titles}
         subsections: dict[str, Subsection] \
             = {x.code: Subsection(x) for x in subtitles}
         for subsection in subsections.values():
             sections[subsection.title.code[0]].subsections.append(subsection)
@@ -296,22 +297,22 @@
         """Composes and returns the CSV rows.
 
         :return: The CSV rows.
         """
         total_str: str = gettext("Total")
         rows: list[CSVRow] = [CSVRow(None, gettext("Amount"))]
         for section in self.__sections:
-            rows.append(CSVRow(str(section.title).title(), None))
+            rows.append(CSVRow(str(section.title), None))
             for subsection in section.subsections:
-                rows.append(CSVRow(f" {str(subsection.title).title()}", None))
+                rows.append(CSVRow(f" {str(subsection.title)}", None))
                 for account in subsection.accounts:
-                    rows.append(CSVRow(f"  {str(account.account).title()}",
+                    rows.append(CSVRow(f"  {str(account.account)}",
                                        account.amount))
                 rows.append(CSVRow(f" {total_str}", subsection.total))
-            rows.append(CSVRow(section.accumulated.title.title(),
+            rows.append(CSVRow(section.accumulated.title,
                                section.accumulated.amount))
             rows.append(CSVRow(None, None))
         rows = rows[:-1]
         return rows
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/journal.py` & `mia-accounting-1.5.7/src/accounting/report/reports/journal.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     :return: The CSV rows.
     """
     rows: list[CSVRow] = [CSVRow(gettext("Date"), gettext("Currency"),
                                  gettext("Account"), gettext("Description"),
                                  gettext("Debit"), gettext("Credit"),
                                  gettext("Note"))]
     rows.extend([CSVRow(x.journal_entry.date, x.currency.code,
-                        str(x.account).title(), x.description,
+                        str(x.account), x.description,
                         x.debit, x.credit, x.journal_entry.note)
                  for x in line_items])
     return rows
 
 
 class Journal(BaseReport):
     """The journal."""
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/ledger.py` & `mia-accounting-1.5.7/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/search.py` & `mia-accounting-1.5.7/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.5.7/src/accounting/report/reports/trial_balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     def __get_csv_rows(self) -> list[CSVRow]:
         """Composes and returns the CSV rows.
 
         :return: The CSV rows.
         """
         rows: list[CSVRow] = [CSVRow(gettext("Account"), gettext("Debit"),
                                      gettext("Credit"))]
-        rows.extend([CSVRow(str(x.account).title(), x.debit, x.credit)
+        rows.extend([CSVRow(str(x.account), x.debit, x.credit)
                      for x in self.__accounts])
         rows.append(CSVRow(gettext("Total"), self.__total.debit,
                            self.__total.credit))
         return rows
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.5.7/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.5.7/src/accounting/report/reports/unapplied_accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,16 +116,15 @@
 def get_csv_rows(accounts: list[Account]) -> list[CSVRow]:
     """Composes and returns the CSV rows from the line items.
 
     :param accounts: The accounts.
     :return: The CSV rows.
     """
     rows: list[CSVRow] = [CSVRow(gettext("Account"), gettext("Count"))]
-    rows.extend([CSVRow(str(x).title(), x.count)
-                 for x in accounts])
+    rows.extend([CSVRow(str(x), x.count) for x in accounts])
     return rows
 
 
 class AccountsWithUnappliedOriginalLineItems(BaseReport):
     """The accounts with unapplied original line items."""
 
     def __init__(self, currency: Currency):
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/unmatched.py` & `mia-accounting-1.5.7/src/accounting/report/reports/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/reports/unmatched_accounts.py` & `mia-accounting-1.5.7/src/accounting/report/reports/unmatched_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,15 @@
 def get_csv_rows(accounts: list[Account]) -> list[CSVRow]:
     """Composes and returns the CSV rows from the line items.
 
     :param accounts: The accounts.
     :return: The CSV rows.
     """
     rows: list[CSVRow] = [CSVRow(gettext("Account"), gettext("Count"))]
-    rows.extend([CSVRow(str(x).title(), x.count)
-                 for x in accounts])
+    rows.extend([CSVRow(str(x), x.count) for x in accounts])
     return rows
 
 
 class AccountsWithUnmatchedOffsets(BaseReport):
     """The accounts with unmatched offsets."""
 
     def __init__(self, currency: Currency):
```

### Comparing `mia-accounting-1.5.6/src/accounting/report/template_filters.py` & `mia-accounting-1.5.7/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/__init__.py` & `mia-accounting-1.5.7/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.5.7/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/base_report.py` & `mia-accounting-1.5.7/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.5.7/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/offset_matcher.py` & `mia-accounting-1.5.7/src/accounting/report/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/option_link.py` & `mia-accounting-1.5.7/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.5.7/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/report_type.py` & `mia-accounting-1.5.7/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.5.7/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/unmatched.py` & `mia-accounting-1.5.7/src/accounting/report/utils/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/utils/urls.py` & `mia-accounting-1.5.7/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/report/views.py` & `mia-accounting-1.5.7/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/css/style.css` & `mia-accounting-1.5.7/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/account-form.js` & `mia-accounting-1.5.7/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/account-order.js` & `mia-accounting-1.5.7/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/currency-form.js` & `mia-accounting-1.5.7/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/description-editor.js` & `mia-accounting-1.5.7/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.5.7/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.5.7/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.5.7/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.5.7/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.5.7/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.5.7/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/option-form.js` & `mia-accounting-1.5.7/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.5.7/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.5.7/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/template_filters.py` & `mia-accounting-1.5.7/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/template_globals.py` & `mia-accounting-1.5.7/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/account/detail.html`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         </div>
       </div>
     </div>
   </form>
 {% endif %}
 
 <div class="accounting-card col-sm-6">
-  <div class="accounting-card-title">{{ obj.title|title }}</div>
+  <div class="accounting-card-title">{{ obj.title }}</div>
   <div class="accounting-card-code">{{ obj.code }}</div>
   {% if obj.is_need_offset %}
     <div>
       <span class="badge rounded-pill bg-info">{{ A_("Needs Offset") }}</span>
     </div>
   {% endif %}
   <div class="small text-secondary fst-italic">
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/base-account/detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   <a class="btn btn-primary" role="button" href="{{ url_for("accounting.account.list")|accounting_or_next }}">
     <i class="fa-solid fa-circle-chevron-left"></i>
     <span class="d-none d-md-inline">{{ A_("Back") }}</span>
   </a>
 </div>
 
 <div class="accounting-card col-sm-6">
-  <div class="accounting-card-title">{{ obj.title|title }}</div>
+  <div class="accounting-card-title">{{ obj.title }}</div>
   <div class="accounting-card-code">{{ obj.code }}</div>
   {% if obj.accounts %}
     <div>
     {% for account in obj.accounts %}
       <a class="btn btn-primary" role="button" href="{{ url_for("accounting.account.detail", account=account)|accounting_append_next }}">
         {{ account }}
       </a>
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/base.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {# <ul> For SonarQube not to complain about incorrect HTML #}
 {% for line_item in line_items %}
   <li class="list-group-item accounting-journal-entry-line-item">
     <div class="d-flex justify-content-between">
       <div>
         <div class="small">
           <span class="d-none d-md-inline">{{ line_item.account.code }}</span>
-          {{ line_item.account.title|title }}
+          {{ line_item.account.title }}
         </div>
         {% if line_item.description is not none %}
           <div>{{ line_item.description }}</div>
         {% endif %}
         {% if line_item.original_line_item %}
           <div class="fst-italic small accounting-original-line-item">
             <a href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.original_line_item.journal_entry)|accounting_append_next }}">
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
 limitations under the License. Author: imacat@mail.imacat.idv.tw (imacat) First
 written: 2023/3/14 #} {#
     * For SonarQube not to complain about incorrect HTML #} {% for line_item in
       line_items %}
-    * {{ line_item.account.code }} {{ line_item.account.title|title }}
+    * {{ line_item.account.code }} {{ line_item.account.title }}
       {% if line_item.description is not none %}
       {{ line_item.description }}
       {% endif %} {% if line_item.original_line_item %}
       journal-entry.detail",
       journal_entry=line_item.original_line_item.journal_entry)|accounting_append_next
       }}"> {{ A_("Offset %(item)s", item=line_item.original_line_item) }}
 {% endif %} {% if line_item.is_need_offset %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         <ul id="accounting-original-line-item-selector-option-list" class="list-group accounting-selector-list">
           {% for line_item in form.original_line_item_options %}
             <li id="accounting-original-line-item-selector-option-{{ line_item.id }}" class="list-group-item d-flex justify-content-between accounting-clickable accounting-original-line-item-selector-option" data-id="{{ line_item.id }}" data-date="{{ line_item.journal_entry.date }}" data-debit-credit="{{ "debit" if line_item.is_debit else "credit" }}" data-currency-code="{{ line_item.currency.code }}" data-account-code="{{ line_item.account_code }}" data-account-title="{{ line_item.account.title }}" data-account-text="{{ line_item.account }}" data-description="{{ line_item.description|accounting_default }}" data-net-balance="{{ line_item.net_balance|accounting_journal_entry_format_amount_input }}" data-text="{{ line_item }}" data-query-values="{{ line_item.query_values|tojson|forceescape }}" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">
               <div>
                 <div class="small">
                   {{ line_item.journal_entry.date|accounting_format_date }}
                   <span class="d-none d-md-inline">{{ line_item.account.code }}</span>
-                  {{ line_item.account.title|title }}
+                  {{ line_item.account.title }}
                 </div>
                 {{ line_item.description|accounting_default }}
               </div>
               <div>
                 <span class="badge bg-primary rounded-pill">
                   <span id="accounting-original-line-item-selector-option-{{ line_item.id }}-net-balance">{{ line_item.net_balance|accounting_format_amount }}</span>
                   / {{ line_item.amount|accounting_format_amount }}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,28 @@
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/3/8
 #}
 <div class="accounting-report-table-row accounting-balance-sheet-section">
-  <div>{{ section.title.title|title }}</div>
+  <div>{{ section.title.title }}</div>
 </div>
 <div class="accounting-report-table-body">
   {% for subsection in section.subsections %}
     <div class="accounting-report-table-row accounting-balance-sheet-subsection">
       <div>
         <span class="d-none d-md-inline">{{ subsection.title.code }}</span>
-        {{ subsection.title.title|title }}
+        {{ subsection.title.title }}
       </div>
     </div>
     {% for account in subsection.accounts %}
       <a class="d-flex justify-content-between accounting-report-table-row accounting-balance-sheet-account" href="{{ account.url }}">
         <div>
           <span class="d-none d-md-inline">{{ account.account.code }}</span>
-          {{ account.account.title|title }}
+          {{ account.account.title }}
         </div>
         <div class="accounting-amount {% if account.amount < 0 %} text-danger {% endif %}">{{ account.amount|accounting_report_format_amount }}</div>
       </a>
     {% endfor %}
   {% endfor %}
 </div>
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files 0% similar despite different names*

```diff
@@ -16,12 +16,12 @@
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/3/8
 #}
 <div>{{ line_item.date|accounting_format_date }}</div>
-<div>{{ line_item.account.title|title }}</div>
+<div>{{ line_item.account.title }}</div>
 <div>{{ line_item.description|accounting_default }}</div>
 <div class="accounting-amount">{{ line_item.income|accounting_format_amount|accounting_default }}</div>
 <div class="accounting-amount">{{ line_item.expense|accounting_format_amount|accounting_default }}</div>
 <div class="accounting-amount {% if line_item.balance < 0 %} text-danger {% endif %}">{{ line_item.balance|accounting_report_format_amount }}</div>
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 <div>
   {% if line_item.date or line_item.account %}
     <div class="text-muted small">
       {% if line_item.date %}
         {{ line_item.date|accounting_format_date }}
       {% endif %}
       {% if line_item.account %}
-        {{ line_item.account.title|title }}
+        {{ line_item.account.title }}
       {% endif %}
     </div>
   {% endif %}
   {% if line_item.description %}
     <div>{{ line_item.description }}</div>
   {% endif %}
 </div>
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
       <i class="fa-solid fa-clipboard"></i>
       <span class="d-none d-md-inline">{{ A_("Account") }}</span>
     </button>
     <ul class="dropdown-menu accounting-toolbar-accounts" aria-labelledby="accounting-choose-account">
       {% for account in report.account_options %}
         <li>
           <a class="dropdown-item {% if account.is_active %} active {% endif %}" href="{{ account.url }}">
-            {{ account.title|title }}
+            {{ account.title }}
           </a>
         </li>
       {% endfor %}
     </ul>
   </div>
 {% endif %}
 {% if use_period_chooser %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Income and Expenses Log of %(account)s %(period)s", account=report.account.title|title, period=report.period.desc|title) }}{% else %}{{ A_("Income and Expenses Log of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Income and Expenses Log of %(account)s %(period)s", account=report.account.title, period=report.period.desc|title) }}{% else %}{{ A_("Income and Expenses Log of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true,
           use_period_chooser = true %}
```

#### html2text {}

```diff
@@ -8,19 +8,19 @@
 the License for the specific language governing permissions and limitations
 under the License. Author: imacat@mail.imacat.idv.tw (imacat) First written:
 2023/3/5 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
 {% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
 accounting_default_currency_code() %}{{ A_("Income and Expenses Log of %
-(account)s %(period)s", account=report.account.title|title,
+(account)s %(period)s", account=report.account.title,
 period=report.period.desc|title) }}{% else %}{{ A_("Income and Expenses Log of
 %(account)s in %(currency)s %(period)s", currency=report.currency.name|title,
-account=report.account.title|title, period=report.period.desc|title) }}{% endif
-%}{% endblock %}{% endblock %} {% block content %}
+account=report.account.title, period=report.period.desc|title) }}{% endif %}{%
+endblock %}{% endblock %} {% block content %}
 {% with use_currency_chooser = true, use_account_chooser = true,
 use_period_chooser = true %} {% include "accounting/report/include/toolbar-
 buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
 "accounting/report/include/search-modal.html" %} {% if report.has_data %} {%
 with pagination = report.pagination %} {% include "accounting/include/
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/income-statement.html`

 * *Files 3% similar despite different names*

```diff
@@ -62,40 +62,40 @@
         </div>
       </div>
       <div class="accounting-report-table-body">
         {% for section in report.sections %}
           <div class="accounting-report-table-row accounting-income-statement-section">
             <div>
               <span class="d-none d-md-inline">{{ section.title.code }}</span>
-              {{ section.title.title|title }}
+              {{ section.title.title }}
             </div>
           </div>
           {% for subsection in section.subsections %}
             <div class="accounting-report-table-row accounting-income-statement-subsection">
               <div>
                 <span class="d-none d-md-inline">{{ subsection.title.code }}</span>
-                {{ subsection.title.title|title }}
+                {{ subsection.title.title }}
               </div>
             </div>
             {% for account in subsection.accounts %}
               <a class="accounting-report-table-row accounting-income-statement-account" href="{{ account.url }}">
                 <div>
                   <span class="d-none d-md-inline">{{ account.account.code }}</span>
-                  {{ account.account.title|title }}
+                  {{ account.account.title }}
                 </div>
                 <div class="accounting-amount {% if account.amount < 0 %} text-danger {% endif %}">{{ account.amount|accounting_report_format_amount }}</div>
               </a>
             {% endfor %}
             <div class="accounting-report-table-row accounting-income-statement-subtotal">
               <div>{{ A_("Total") }}</div>
               <div class="accounting-amount {% if subsection.total < 0 %} text-danger {% endif %}">{{ subsection.total|accounting_report_format_amount }}</div>
             </div>
           {% endfor %}
           <div class="accounting-report-table-row accounting-income-statement-total">
-            <div>{{ section.accumulated.title|title }}</div>
+            <div>{{ section.accumulated.title }}</div>
             <div class="accounting-amount {% if section.accumulated.amount < 0 %} text-danger {% endif %}">{{ section.accumulated.amount|accounting_report_format_amount }}</div>
           </div>
         {% endfor %}
       </div>
     </div>
   </div>
 {% else %}
```

#### html2text {}

```diff
@@ -24,23 +24,23 @@
 ***** {% if report.currency.code == accounting_default_currency_code() %} {{ A_
 ("Income Statement %(period)s", period=report.period.desc|title) }} {% else %}
 {{ A_("Income Statement of %(currency)s %(period)s",
 currency=report.currency.name|title, period=report.period.desc|title) }} {%
 endif %} *****
 {{ A_("Amount") }}
 {% for section in report.sections %}
-{{ section.title.code }} {{ section.title.title|title }}
+{{ section.title.code }} {{ section.title.title }}
 {% for subsection in section.subsections %}
-{{ subsection.title.code }} {{ subsection.title.title|title }}
+{{ subsection.title.code }} {{ subsection.title.title }}
 {% for account in subsection.accounts %}
-{{_account.account.code_}}_{{_account.account.title|title_}}
+{{_account.account.code_}}_{{_account.account.title_}}
 {{_account.amount|accounting_report_format_amount_}}
  {% endfor %}
 {{ A_("Total") }}
 {{ subsection.total|accounting_report_format_amount }}
 {% endfor %}
-{{ section.accumulated.title|title }}
+{{ section.accumulated.title }}
 {{ section.accumulated.amount|accounting_report_format_amount }}
 {% endfor %}
 {% else %}
 {{ A_("There is no data.") }}
 {% endif %} {% endblock %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/journal.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     <div class="accounting-report-table-body">
       {% for line_item in report.line_items %}
         <a class="accounting-report-table-row" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
           <div>{{ line_item.journal_entry.date|accounting_format_date }}</div>
           <div>{{ line_item.currency.name }}</div>
           <div>
             <span class="d-none d-md-inline">{{ line_item.account.code }}</span>
-            {{ line_item.account.title|title }}
+            {{ line_item.account.title }}
           </div>
           <div>{{ line_item.description|accounting_default }}</div>
           <div class="accounting-amount">{{ line_item.debit|accounting_format_amount|accounting_default }}</div>
           <div class="accounting-amount">{{ line_item.credit|accounting_format_amount|accounting_default }}</div>
         </a>
       {% endfor %}
     </div>
@@ -78,15 +78,15 @@
   <div class="list-group d-md-none">
   {% for line_item in report.line_items %}
     <a class="list-group-item list-group-item-action" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
       <div class="d-flex justify-content-between">
         <div {% if not line_item.is_debit %} class="accounting-mobile-journal-credit" {% endif %}>
           <div class="text-muted small">
             {{ line_item.journal_entry.date|accounting_format_date }}
-            {{ line_item.account.title|title }}
+            {{ line_item.account.title }}
             {% if line_item.currency.code != accounting_default_currency_code() %}
               <span class="badge rounded-pill bg-info">{{ line_item.currency.code }}</span>
             {% endif %}
           </div>
           {% if line_item.description is not none %}
             <div>{{ line_item.description }}</div>
           {% endif %}
```

#### html2text {}

```diff
@@ -27,26 +27,26 @@
 {{ A_("Debit") }}
 {{ A_("Credit") }}
 {% for line_item in report.line_items %}
 journal-entry.detail",
 journal_entry=line_item.journal_entry)|accounting_append_next }}">
 {{ line_item.journal_entry.date|accounting_format_date }}
 {{ line_item.currency.name }}
-{{ line_item.account.code }} {{ line_item.account.title|title }}
+{{ line_item.account.code }} {{ line_item.account.title }}
 {{ line_item.description|accounting_default }}
 {{ line_item.debit|accounting_format_amount|accounting_default }}
 {{ line_item.credit|accounting_format_amount|accounting_default }}
  {% endfor %}
 {% for line_item in report.line_items %}
 journal-entry.detail",
 journal_entry=line_item.journal_entry)|accounting_append_next }}">
 % if not line_item.is_debit %} class="accounting-mobile-journal-credit" {%
 endif %}>
 {{ line_item.journal_entry.date|accounting_format_date }} {
-{ line_item.account.title|title }} {% if line_item.currency.code !=
+{ line_item.account.title }} {% if line_item.currency.code !=
 accounting_default_currency_code() %} {{ line_item.currency.code }} {% endif %}
 {% if line_item.description is not none %}
 {{ line_item.description }}
 {% endif %}
 {{ line_item.amount|accounting_format_amount }}
  {% endfor %}
 {% else %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/ledger.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Ledger of %(account)s %(period)s", account=report.account.title|title, period=report.period.desc|title) }}{% else %}{{ A_("Ledger of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Ledger of %(account)s %(period)s", account=report.account.title, period=report.period.desc|title) }}{% else %}{{ A_("Ledger of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true,
           use_period_chooser = true %}
```

#### html2text {}

```diff
@@ -8,17 +8,17 @@
 governing permissions and limitations under the License. Author:
 imacat@mail.imacat.idv.tw (imacat) First written: 2023/3/5 #} {% extends
 "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
 {% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
 accounting_default_currency_code() %}{{ A_("Ledger of %(account)s %(period)s",
-account=report.account.title|title, period=report.period.desc|title) }}{% else
-%}{{ A_("Ledger of %(account)s in %(currency)s %(period)s",
-currency=report.currency.name|title, account=report.account.title|title,
+account=report.account.title, period=report.period.desc|title) }}{% else %}{
+{ A_("Ledger of %(account)s in %(currency)s %(period)s",
+currency=report.currency.name|title, account=report.account.title,
 period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %} {%
 block content %}
 {% with use_currency_chooser = true, use_account_chooser = true,
 use_period_chooser = true %} {% include "accounting/report/include/toolbar-
 buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     <div class="accounting-report-table-body">
       {% for line_item in report.line_items %}
         <a class="accounting-report-table-row" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
           <div>{{ line_item.journal_entry.date|accounting_format_date }}</div>
           <div>{{ line_item.currency.name }}</div>
           <div>
             <span class="d-none d-md-inline">{{ line_item.account.code }}</span>
-            {{ line_item.account.title|title }}
+            {{ line_item.account.title }}
           </div>
           <div>{{ line_item.description|accounting_default }}</div>
           <div class="accounting-amount">{{ line_item.debit|accounting_format_amount|accounting_default }}</div>
           <div class="accounting-amount">{{ line_item.credit|accounting_format_amount|accounting_default }}</div>
         </a>
       {% endfor %}
     </div>
@@ -75,15 +75,15 @@
   <div class="list-group d-md-none">
   {% for line_item in report.line_items %}
     <a class="list-group-item list-group-item-action" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
       <div class="d-flex justify-content-between">
         <div {% if not line_item.is_debit %} class="accounting-mobile-journal-credit" {% endif %}>
           <div class="text-muted small">
             {{ line_item.journal_entry.date|accounting_format_date }}
-            {{ line_item.account.title|title }}
+            {{ line_item.account.title }}
             {% if line_item.currency.code != accounting_default_currency_code() %}
               <span class="badge rounded-pill bg-info">{{ line_item.currency.code }}</span>
             {% endif %}
           </div>
           {% if line_item.description is not none %}
             <div>{{ line_item.description }}</div>
           {% endif %}
```

#### html2text {}

```diff
@@ -25,26 +25,26 @@
 {{ A_("Debit") }}
 {{ A_("Credit") }}
 {% for line_item in report.line_items %}
 journal-entry.detail",
 journal_entry=line_item.journal_entry)|accounting_append_next }}">
 {{ line_item.journal_entry.date|accounting_format_date }}
 {{ line_item.currency.name }}
-{{ line_item.account.code }} {{ line_item.account.title|title }}
+{{ line_item.account.code }} {{ line_item.account.title }}
 {{ line_item.description|accounting_default }}
 {{ line_item.debit|accounting_format_amount|accounting_default }}
 {{ line_item.credit|accounting_format_amount|accounting_default }}
  {% endfor %}
 {% for line_item in report.line_items %}
 journal-entry.detail",
 journal_entry=line_item.journal_entry)|accounting_append_next }}">
 % if not line_item.is_debit %} class="accounting-mobile-journal-credit" {%
 endif %}>
 {{ line_item.journal_entry.date|accounting_format_date }} {
-{ line_item.account.title|title }} {% if line_item.currency.code !=
+{ line_item.account.title }} {% if line_item.currency.code !=
 accounting_default_currency_code() %} {{ line_item.currency.code }} {% endif %}
 {% if line_item.description is not none %}
 {{ line_item.description }}
 {% endif %}
 {{ line_item.amount|accounting_format_amount }}
  {% endfor %}
 {% else %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         </div>
       </div>
       <div class="accounting-report-table-body">
         {% for account in report.accounts %}
           <a class="accounting-report-table-row" href="{{ account.url }}">
             <div>
               <span class="d-none d-md-inline">{{ account.account.code }}</span>
-              {{ account.account.title|title }}
+              {{ account.account.title }}
             </div>
             <div class="accounting-amount">{{ account.debit|accounting_format_amount|accounting_default }}</div>
             <div class="accounting-amount">{{ account.credit|accounting_format_amount|accounting_default }}</div>
           </a>
         {% endfor %}
       </div>
       <div class="accounting-report-table-footer">
```

#### html2text {}

```diff
@@ -26,15 +26,15 @@
 { A_("Trial Balance of %(currency)s %(period)s",
 currency=report.currency.name|title, period=report.period.desc|title) }} {%
 endif %} *****
 {{ A_("Account") }}
 {{ A_("Debit") }}
 {{ A_("Credit") }}
 {% for account in report.accounts %}
-{{_account.account.code_}}_{{_account.account.title|title_}}
+{{_account.account.code_}}_{{_account.account.title_}}
 {{_account.debit|accounting_format_amount|accounting_default_}}
 {{_account.credit|accounting_format_amount|accounting_default_}}
  {% endfor %}
 {{ A_("Total") }}
 {{ report.total.debit|accounting_format_amount }}
 {{ report.total.credit|accounting_format_amount }}
 {% else %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Accounts with Unapplied Items") }}{% else %}{{ A_("Accounts with Unapplied Items in %(currency)s", currency=report.currency.name|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Accounts With Unapplied Items") }}{% else %}{{ A_("Accounts With Unapplied Items in %(currency)s", currency=report.currency.name|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
@@ -42,17 +42,17 @@
 {% include "accounting/report/include/search-modal.html" %}
 
 {% if report.has_data %}
   <div class="accounting-sheet">
     <div class="d-none d-sm-flex justify-content-center mb-3">
       <h2 class="text-center">
         {% if report.currency.code == accounting_default_currency_code() %}
-          {{ A_("Accounts with Unapplied Items") }}
+          {{ A_("Accounts With Unapplied Items") }}
         {% else %}
-          {{ A_("Accounts with Unapplied Items in %(currency)s", currency=report.currency.name|title) }}
+          {{ A_("Accounts With Unapplied Items in %(currency)s", currency=report.currency.name|title) }}
         {% endif %}
       </h2>
     </div>
 
     <div class="accounting-report-table accounting-unapplied-account-table">
         <div class="accounting-report-table-header">
           <div class="accounting-report-table-row">
@@ -60,15 +60,15 @@
           </div>
         </div>
       <div class="accounting-report-table-body">
         {% for account in report.accounts %}
           <a class="accounting-report-table-row" href="{{ url_for("accounting-report.unapplied", currency=report.currency, account=account, period=report.period) }}">
             <div>
               <span class="d-none d-md-inline">{{ account.code }}</span>
-              {{ account.title|title }}
+              {{ account.title }}
             </div>
             <div class="accounting-amount">{{ account.count }}</div>
           </a>
         {% endfor %}
       </div>
     </div>
   </div>
```

#### html2text {}

```diff
@@ -8,30 +8,30 @@
 implied. See the License for the specific language governing permissions and
 limitations under the License. Author: imacat@mail.imacat.idv.tw (imacat) First
 written: 2023/4/8 #} {% extends "accounting/base.html" %} {% block
 accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
 {% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
-accounting_default_currency_code() %}{{ A_("Accounts with Unapplied Items") }}
-{% else %}{{ A_("Accounts with Unapplied Items in %(currency)s",
+accounting_default_currency_code() %}{{ A_("Accounts With Unapplied Items") }}
+{% else %}{{ A_("Accounts With Unapplied Items in %(currency)s",
 currency=report.currency.name|title) }}{% endif %}{% endblock %}{% endblock %}
 {% block content %}
 {% with use_currency_chooser = true, use_account_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/search-modal.html" %} {% if
 report.has_data %}
 ***** {% if report.currency.code == accounting_default_currency_code() %} {{ A_
-("Accounts with Unapplied Items") }} {% else %} {{ A_("Accounts with Unapplied
+("Accounts With Unapplied Items") }} {% else %} {{ A_("Accounts With Unapplied
 Items in %(currency)s", currency=report.currency.name|title) }} {% endif %}
 *****
 {{ A_("Count") }}
 {% for account in report.accounts %}
 unapplied", currency=report.currency, account=account, period=report.period)
 }}">
-{{ account.code }} {{ account.title|title }}
+{{ account.code }} {{ account.title }}
 {{ account.count }}
  {% endfor %}
 {% else %}
 {{ A_("There is no data.") }}
 {% endif %} {% endblock %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/unapplied.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Unapplied Items of %(account)s", account=report.account.title|title) }}{% else %}{{ A_("Unapplied Items of %(account)s in %(currency)s", currency=report.currency.name|title, account=report.account.title|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Unapplied Items of %(account)s", account=report.account.title) }}{% else %}{{ A_("Unapplied Items of %(account)s in %(currency)s", currency=report.currency.name|title, account=report.account.title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
```

#### html2text {}

```diff
@@ -8,18 +8,18 @@
 the License for the specific language governing permissions and limitations
 under the License. Author: imacat@mail.imacat.idv.tw (imacat) First written:
 2023/4/7 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
 {% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
 accounting_default_currency_code() %}{{ A_("Unapplied Items of %(account)s",
-account=report.account.title|title) }}{% else %}{{ A_("Unapplied Items of %
-(account)s in %(currency)s", currency=report.currency.name|title,
-account=report.account.title|title) }}{% endif %}{% endblock %}{% endblock %}
-{% block content %}
+account=report.account.title) }}{% else %}{{ A_("Unapplied Items of %(account)s
+in %(currency)s", currency=report.currency.name|title,
+account=report.account.title) }}{% endif %}{% endblock %}{% endblock %} {%
+block content %}
 {% with use_currency_chooser = true, use_account_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/search-modal.html" %} {% if
 report.has_data %} {% with pagination = report.pagination %} {% include
 "accounting/include/pagination.html" %} {% endwith %}
 {{ A_("Date") }}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched-accounts.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/unmatched-accounts.html`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Accounts with Unmatched Offsets") }}{% else %}{{ A_("Accounts with Unmatched Offsets in %(currency)s", currency=report.currency.name|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Accounts With Unmatched Offsets") }}{% else %}{{ A_("Accounts With Unmatched Offsets in %(currency)s", currency=report.currency.name|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
@@ -42,17 +42,17 @@
 {% include "accounting/report/include/search-modal.html" %}
 
 {% if report.has_data %}
   <div class="accounting-sheet">
     <div class="d-none d-sm-flex justify-content-center mb-3">
       <h2 class="text-center">
         {% if report.currency.code == accounting_default_currency_code() %}
-          {{ A_("Accounts with Unmatched Offsets") }}
+          {{ A_("Accounts With Unmatched Offsets") }}
         {% else %}
-          {{ A_("Accounts with Unmatched Offsets in %(currency)s", currency=report.currency.name|title) }}
+          {{ A_("Accounts With Unmatched Offsets in %(currency)s", currency=report.currency.name|title) }}
         {% endif %}
       </h2>
     </div>
 
     <div class="accounting-report-table accounting-unapplied-account-table">
         <div class="accounting-report-table-header">
           <div class="accounting-report-table-row">
@@ -60,15 +60,15 @@
           </div>
         </div>
       <div class="accounting-report-table-body">
         {% for account in report.accounts %}
           <a class="accounting-report-table-row" href="{{ url_for("accounting-report.unmatched", currency=report.currency, account=account, period=report.period) }}">
             <div>
               <span class="d-none d-md-inline">{{ account.code }}</span>
-              {{ account.title|title }}
+              {{ account.title }}
             </div>
             <div class="accounting-amount">{{ account.count }}</div>
           </a>
         {% endfor %}
       </div>
     </div>
   </div>
```

#### html2text {}

```diff
@@ -8,30 +8,30 @@
 implied. See the License for the specific language governing permissions and
 limitations under the License. Author: imacat@mail.imacat.idv.tw (imacat) First
 written: 2023/4/17 #} {% extends "accounting/base.html" %} {% block
 accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
 {% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
-accounting_default_currency_code() %}{{ A_("Accounts with Unmatched Offsets")
-}}{% else %}{{ A_("Accounts with Unmatched Offsets in %(currency)s",
+accounting_default_currency_code() %}{{ A_("Accounts With Unmatched Offsets")
+}}{% else %}{{ A_("Accounts With Unmatched Offsets in %(currency)s",
 currency=report.currency.name|title) }}{% endif %}{% endblock %}{% endblock %}
 {% block content %}
 {% with use_currency_chooser = true, use_account_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/search-modal.html" %} {% if
 report.has_data %}
 ***** {% if report.currency.code == accounting_default_currency_code() %} {{ A_
-("Accounts with Unmatched Offsets") }} {% else %} {{ A_("Accounts with
+("Accounts With Unmatched Offsets") }} {% else %} {{ A_("Accounts With
 Unmatched Offsets in %(currency)s", currency=report.currency.name|title) }} {%
 endif %} *****
 {{ A_("Count") }}
 {% for account in report.accounts %}
 unmatched", currency=report.currency, account=account, period=report.period)
 }}">
-{{ account.code }} {{ account.title|title }}
+{{ account.code }} {{ account.title }}
 {{ account.count }}
  {% endfor %}
 {% else %}
 {{ A_("There is no data.") }}
 {% endif %} {% endblock %}
```

### Comparing `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched.html` & `mia-accounting-1.5.7/src/accounting/templates/accounting/report/unmatched.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Unmatched Offsets of %(account)s", account=report.account.title|title) }}{% else %}{{ A_("Unmatched Offsets of %(account)s in %(currency)s", currency=report.currency.name|title, account=report.account.title|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Unmatched Offsets of %(account)s", account=report.account.title) }}{% else %}{{ A_("Unmatched Offsets of %(account)s in %(currency)s", currency=report.currency.name|title, account=report.account.title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
```

#### html2text {}

```diff
@@ -8,18 +8,18 @@
 License for the specific language governing permissions and limitations under
 the License. Author: imacat@mail.imacat.idv.tw (imacat) First written: 2023/4/
 17 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
 {% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
 accounting_default_currency_code() %}{{ A_("Unmatched Offsets of %(account)s",
-account=report.account.title|title) }}{% else %}{{ A_("Unmatched Offsets of %
+account=report.account.title) }}{% else %}{{ A_("Unmatched Offsets of %
 (account)s in %(currency)s", currency=report.currency.name|title,
-account=report.account.title|title) }}{% endif %}{% endblock %}{% endblock %}
-{% block content %}
+account=report.account.title) }}{% endif %}{% endblock %}{% endblock %} {%
+block content %}
 {% with use_currency_chooser = true, use_account_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/search-modal.html" %} {% if
 report.matched_pairs %}   {{ A_("Match") }}
 match-offsets", currency=report.currency, account=report.account) }}"
 method="post">
```

### Comparing `mia-accounting-1.5.6/src/accounting/translations/accounting.pot` & `mia-accounting-1.5.7/src/accounting/translations/accounting.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,55 +4,55 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-18 09:32+0800\n"
+"POT-Creation-Date: 2023-07-29 08:55+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: src/accounting/forms.py:33
 #: src/accounting/static/js/journal-entry-form.js:1080
-#: src/accounting/static/js/journal-entry-line-item-editor.js:411
+#: src/accounting/static/js/journal-entry-line-item-editor.js:415
 #: src/accounting/static/js/option-form.js:537
 #: src/accounting/static/js/option-form.js:803
 msgid "Please select the account."
 msgstr ""
 
 #: src/accounting/forms.py:44
 msgid "The currency does not exist."
 msgstr ""
 
 #: src/accounting/forms.py:55 src/accounting/option/forms.py:42
 msgid "The account does not exist."
 msgstr ""
 
-#: src/accounting/models.py:581
+#: src/accounting/models.py:578
 #, python-format
 msgid "Cash Disbursement Journal Entry#%(id)s"
 msgstr ""
 
-#: src/accounting/models.py:584
+#: src/accounting/models.py:581
 #, python-format
 msgid "Cash Receipt Journal Entry#%(id)s"
 msgstr ""
 
-#: src/accounting/models.py:585
+#: src/accounting/models.py:582
 #, python-format
 msgid "Transfer Journal Entry#%(id)s"
 msgstr ""
 
-#: src/accounting/models.py:714
+#: src/accounting/models.py:706
 #, python-format
 msgid "%(date)s %(description)s %(amount)s"
 msgstr ""
 
 #: src/accounting/report/period/shortcuts.py:121
 #: src/accounting/template_filters.py:52
 #: src/accounting/templates/accounting/report/include/period-chooser.html:99
@@ -95,15 +95,15 @@
 msgstr ""
 
 #: src/accounting/account/forms.py:81
 msgid "Please fill in the title"
 msgstr ""
 
 #: src/accounting/account/queries.py:50
-#: src/accounting/report/reports/search.py:101
+#: src/accounting/report/reports/search.py:100
 #: src/accounting/templates/accounting/account/detail.html:97
 #: src/accounting/templates/accounting/account/list.html:62
 msgid "Needs Offset"
 msgstr ""
 
 #: src/accounting/account/views.py:90
 msgid "The account is added successfully"
@@ -199,32 +199,32 @@
 msgid "The journal entry cannot be deleted."
 msgstr ""
 
 #: src/accounting/journal_entry/views.py:184
 msgid "The journal entry is deleted successfully."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:39
+#: src/accounting/journal_entry/forms/currency.py:38
 msgid "Please select the currency."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:62
+#: src/accounting/journal_entry/forms/currency.py:61
 msgid "The currency must be the same as the original line item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:89
+#: src/accounting/journal_entry/forms/currency.py:88
 msgid "The currency must not be changed when there is offset."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:98
+#: src/accounting/journal_entry/forms/currency.py:97
 #: src/accounting/static/js/journal-entry-form.js:773
 msgid "Please add some line items."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/currency.py:111
+#: src/accounting/journal_entry/forms/currency.py:110
 #: src/accounting/static/js/journal-entry-form.js:522
 msgid "The totals of the debit and credit amounts do not match."
 msgstr ""
 
 #: src/accounting/journal_entry/forms/journal_entry.py:48
 #: src/accounting/static/js/journal-entry-form.js:264
 #: src/accounting/static/js/period-chooser.js:265
@@ -245,70 +245,70 @@
 msgid "Please add some currencies."
 msgstr ""
 
 #: src/accounting/journal_entry/forms/journal_entry.py:104
 msgid "Line items with offset cannot be deleted."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:49
+#: src/accounting/journal_entry/forms/line_item.py:48
 msgid "The original line item does not exist."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:70
+#: src/accounting/journal_entry/forms/line_item.py:69
 msgid "The original line item is on the same debit or credit."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:85
+#: src/accounting/journal_entry/forms/line_item.py:84
 msgid "The original line item does not need offset."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:101
+#: src/accounting/journal_entry/forms/line_item.py:100
 msgid "The original line item cannot be an offset item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:119
+#: src/accounting/journal_entry/forms/line_item.py:118
 msgid "The account must be the same as the original line item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:135
+#: src/accounting/journal_entry/forms/line_item.py:134
 msgid "The account must not be changed when there is offset."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:151
+#: src/accounting/journal_entry/forms/line_item.py:150
 msgid "A payable line item cannot start from debit."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:167
+#: src/accounting/journal_entry/forms/line_item.py:166
 msgid "A receivable line item cannot start from credit."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:178
-#: src/accounting/static/js/journal-entry-line-item-editor.js:436
+#: src/accounting/journal_entry/forms/line_item.py:177
+#: src/accounting/static/js/journal-entry-line-item-editor.js:440
 msgid "Please fill in a positive amount."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:220
-#: src/accounting/static/js/journal-entry-line-item-editor.js:442
+#: src/accounting/journal_entry/forms/line_item.py:219
+#: src/accounting/static/js/journal-entry-line-item-editor.js:446
 #, python-format
 msgid ""
 "The amount must not exceed the net balance %(balance)s of the original "
 "line item."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:241
-#: src/accounting/static/js/journal-entry-line-item-editor.js:450
+#: src/accounting/journal_entry/forms/line_item.py:239
+#: src/accounting/static/js/journal-entry-line-item-editor.js:454
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:426
+#: src/accounting/journal_entry/forms/line_item.py:424
 msgid "This account is not for debit line items."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:478
+#: src/accounting/journal_entry/forms/line_item.py:476
 msgid "This account is not for credit line items."
 msgstr ""
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr ""
 
@@ -411,23 +411,23 @@
 msgstr ""
 
 #: src/accounting/report/period/shortcuts.py:146
 #: src/accounting/templates/accounting/report/include/period-chooser.html:122
 msgid "All"
 msgstr ""
 
-#: src/accounting/report/reports/balance_sheet.py:423
-#: src/accounting/report/reports/balance_sheet.py:427
-#: src/accounting/report/reports/balance_sheet.py:439
+#: src/accounting/report/reports/balance_sheet.py:425
+#: src/accounting/report/reports/balance_sheet.py:429
 #: src/accounting/report/reports/balance_sheet.py:441
-#: src/accounting/report/reports/income_expenses.py:189
-#: src/accounting/report/reports/income_expenses.py:423
-#: src/accounting/report/reports/income_statement.py:300
-#: src/accounting/report/reports/ledger.py:171
-#: src/accounting/report/reports/ledger.py:380
+#: src/accounting/report/reports/balance_sheet.py:443
+#: src/accounting/report/reports/income_expenses.py:187
+#: src/accounting/report/reports/income_expenses.py:420
+#: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/ledger.py:168
+#: src/accounting/report/reports/ledger.py:376
 #: src/accounting/report/reports/trial_balance.py:229
 #: src/accounting/templates/accounting/journal-entry/disbursement/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html:38
 #: src/accounting/templates/accounting/journal-entry/receipt/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:39
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:55
 #: src/accounting/templates/accounting/report/balance-sheet.html:65
@@ -439,120 +439,120 @@
 #: src/accounting/templates/accounting/report/income-expenses.html:81
 #: src/accounting/templates/accounting/report/income-statement.html:89
 #: src/accounting/templates/accounting/report/ledger.html:82
 #: src/accounting/templates/accounting/report/trial-balance.html:80
 msgid "Total"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:136
-#: src/accounting/report/reports/ledger.py:132
+#: src/accounting/report/reports/income_expenses.py:134
+#: src/accounting/report/reports/ledger.py:129
 msgid "Brought forward"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:407
+#: src/accounting/report/reports/income_expenses.py:404
 #: src/accounting/report/reports/journal.py:158
-#: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/ledger.py:362
 #: src/accounting/report/reports/unapplied.py:148
 #: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
 #: src/accounting/templates/accounting/report/unapplied.html:52
 #: src/accounting/templates/accounting/report/unmatched.html:93
 msgid "Date"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:407
+#: src/accounting/report/reports/income_expenses.py:404
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/report/reports/unapplied_accounts.py:122
 #: src/accounting/report/reports/unmatched_accounts.py:122
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:58
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:40
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
 #: src/accounting/templates/accounting/report/trial-balance.html:61
 msgid "Account"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:408
+#: src/accounting/report/reports/income_expenses.py:405
 #: src/accounting/report/reports/journal.py:159
-#: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/ledger.py:362
 #: src/accounting/report/reports/unapplied.py:149
 #: src/accounting/report/reports/unmatched.py:159
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:29
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:50
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
 #: src/accounting/templates/accounting/report/unapplied.html:53
 #: src/accounting/templates/accounting/report/unmatched.html:94
 msgid "Description"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:408
+#: src/accounting/report/reports/income_expenses.py:405
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:409
+#: src/accounting/report/reports/income_expenses.py:406
 #: src/accounting/templates/accounting/report/income-expenses.html:59
 msgid "Expense"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:409
-#: src/accounting/report/reports/ledger.py:368
+#: src/accounting/report/reports/income_expenses.py:406
+#: src/accounting/report/reports/ledger.py:364
 #: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
 #: src/accounting/templates/accounting/report/unmatched.html:97
 msgid "Balance"
 msgstr ""
 
-#: src/accounting/report/reports/income_expenses.py:410
+#: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:161
-#: src/accounting/report/reports/ledger.py:368
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
+#: src/accounting/report/reports/ledger.py:364
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:179
 #: src/accounting/templates/accounting/journal-entry/include/form.html:73
 msgid "Note"
 msgstr ""
 
-#: src/accounting/report/reports/income_statement.py:228
-msgid "total operating revenue"
-msgstr ""
-
 #: src/accounting/report/reports/income_statement.py:229
-msgid "gross income"
+msgid "Total Operating Revenue"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:230
-msgid "operating income"
+msgid "Gross Income"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:231
-msgid "before tax income"
+msgid "Operating Income"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:232
-msgid "after tax income"
+msgid "Before Tax Income"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:233
-msgid "net income or loss for current period"
+msgid "After Tax Income"
 msgstr ""
 
-#: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/income_statement.py:234
+msgid "Net Income or Loss for Current Period"
+msgstr ""
+
+#: src/accounting/report/reports/income_statement.py:302
 #: src/accounting/report/reports/unapplied.py:149
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:66
 #: src/accounting/templates/accounting/report/income-statement.html:61
 #: src/accounting/templates/accounting/report/unapplied.html:54
 msgid "Amount"
 msgstr ""
 
 #: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/unapplied.py:148
@@ -561,29 +561,29 @@
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
 msgid "Currency"
 msgstr ""
 
 #: src/accounting/report/reports/journal.py:160
-#: src/accounting/report/reports/ledger.py:367
+#: src/accounting/report/reports/ledger.py:363
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
 #: src/accounting/templates/accounting/report/trial-balance.html:62
 #: src/accounting/templates/accounting/report/unmatched.html:95
 msgid "Debit"
 msgstr ""
 
 #: src/accounting/report/reports/journal.py:160
-#: src/accounting/report/reports/ledger.py:367
+#: src/accounting/report/reports/ledger.py:363
 #: src/accounting/report/reports/trial_balance.py:226
 #: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
@@ -608,24 +608,24 @@
 #: src/accounting/report/reports/unapplied_accounts.py:122
 #: src/accounting/report/reports/unmatched_accounts.py:122
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:59
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:59
 msgid "Count"
 msgstr ""
 
-#: src/accounting/report/utils/offset_matcher.py:163
+#: src/accounting/report/utils/offset_matcher.py:161
 msgid "There is no unmatched offset."
 msgstr ""
 
-#: src/accounting/report/utils/offset_matcher.py:167
+#: src/accounting/report/utils/offset_matcher.py:165
 #, python-format
 msgid "%(total)s unmatched offsets without original items."
 msgstr ""
 
-#: src/accounting/report/utils/offset_matcher.py:172
+#: src/accounting/report/utils/offset_matcher.py:170
 #, python-format
 msgid ""
 "%(matches)s unmatched offsets out of %(total)s can match with their "
 "original items."
 msgstr ""
 
 #: src/accounting/report/utils/report_chooser.py:86
@@ -746,15 +746,15 @@
 msgstr ""
 
 #: src/accounting/static/js/description-editor.js:1195
 msgid "December"
 msgstr ""
 
 #: src/accounting/static/js/journal-entry-form.js:1085
-#: src/accounting/static/js/journal-entry-line-item-editor.js:430
+#: src/accounting/static/js/journal-entry-line-item-editor.js:434
 msgid "Please fill in the amount."
 msgstr ""
 
 #: src/accounting/static/js/journal-entry-form.js:1107
 #: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:37
 #: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:41
 #, python-format
@@ -827,39 +827,39 @@
 msgid "Confirm Delete Account"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:77
 #: src/accounting/templates/accounting/account/include/form.html:91
 #: src/accounting/templates/accounting/currency/detail.html:73
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:27
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:30
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:31
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:29
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:29
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
 #: src/accounting/templates/accounting/report/unmatched.html:58
 msgid "Close"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:83
 #: src/accounting/templates/accounting/account/include/form.html:112
 #: src/accounting/templates/accounting/currency/detail.html:79
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:195
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:71
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:66
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
 #: src/accounting/templates/accounting/report/unmatched.html:74
 msgid "Cancel"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
@@ -936,20 +936,20 @@
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/include/form.html:75
 #: src/accounting/templates/accounting/account/order.html:62
 #: src/accounting/templates/accounting/currency/include/form.html:57
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:195
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:196
 #: src/accounting/templates/accounting/journal-entry/include/form.html:80
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:71
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:72
 #: src/accounting/templates/accounting/journal-entry/order.html:61
 #: src/accounting/templates/accounting/option/form.html:80
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:66
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:67
 msgid "Save"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/include/form.html:45
 msgid "Base account"
 msgstr ""
 
@@ -1002,15 +1002,15 @@
 msgstr ""
 
 #: src/accounting/templates/accounting/currency/include/form.html:44
 msgid "Code"
 msgstr ""
 
 #: src/accounting/templates/accounting/currency/include/form.html:50
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:33
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:34
 msgid "Name"
 msgstr ""
 
 #: src/accounting/templates/accounting/include/nav.html:27
 msgid "Accounting"
 msgstr ""
 
@@ -1071,61 +1071,61 @@
 msgid "Select Account"
 msgstr ""
 
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:44
 msgid "More…"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:36
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:37
 msgid "Offset..."
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:44
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:45
 msgid "General"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:49
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:50
 msgid "Travel"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:54
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:55
 msgid "Bus"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:59
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:60
 msgid "Recurring"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:64
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:65
 msgid "Annotation"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:73
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:90
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:125
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:74
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:91
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:126
 msgid "Tag"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:105
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:146
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:106
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:147
 #: src/accounting/templates/accounting/report/include/period-chooser.html:129
 msgid "From"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:114
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:151
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:115
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:152
 #: src/accounting/templates/accounting/report/include/period-chooser.html:135
 msgid "To"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:130
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:131
 msgid "Route"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:172
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:173
 msgid "The Number of Items"
 msgstr ""
 
 #: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:45
 #: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:46
 msgid "Offsets"
 msgstr ""
@@ -1149,19 +1149,19 @@
 msgid "Confirm Delete Journal Entry"
 msgstr ""
 
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:81
 msgid "Do you really want to delete this journal entry?"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:27
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 msgid "Line Item Content"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:34
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:35
 msgid "Original Line Item"
 msgstr ""
 
 #: src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html:25
 #: src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html:26
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:31
 msgid "Cash Disbursement"
@@ -1209,51 +1209,51 @@
 
 #: src/accounting/templates/accounting/option/detail.html:70
 #: src/accounting/templates/accounting/option/form.html:72
 #: src/accounting/templates/accounting/option/form.html:96
 msgid "Recurring Income"
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:47
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:48
 msgid "Description Template"
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:52
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:53
 msgid "Available template variables:"
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:54
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:55
 msgid "This month, as a number."
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:55
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:56
 msgid "This month, in its name."
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:56
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:57
 msgid "Last month, as a number."
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:57
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:58
 msgid "Last month, in its name."
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:58
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:59
 msgid "The previous bimonthly period, as numbers."
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:59
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:60
 msgid "The previous bimonthly period, as their names."
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:62
 msgid "Example:"
 msgstr ""
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:62
 msgid "Water bill for {last_bimonthly_name}"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/balance-sheet.html:29
 #: src/accounting/templates/accounting/report/balance-sheet.html:51
 #, python-format
 msgid "Balance Sheet %(period)s"
@@ -1312,42 +1312,42 @@
 #: src/accounting/templates/accounting/report/trial-balance.html:53
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:29
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:49
-msgid "Accounts with Unapplied Items"
+msgid "Accounts With Unapplied Items"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:29
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:51
 #, python-format
-msgid "Accounts with Unapplied Items in %(currency)s"
+msgid "Accounts With Unapplied Items in %(currency)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unapplied.html:29
 #, python-format
 msgid "Unapplied Items of %(account)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unapplied.html:29
 #, python-format
 msgid "Unapplied Items of %(account)s in %(currency)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:29
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:49
-msgid "Accounts with Unmatched Offsets"
+msgid "Accounts With Unmatched Offsets"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:29
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:51
 #, python-format
-msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgid "Accounts With Unmatched Offsets in %(currency)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/unmatched.html:29
 #, python-format
 msgid "Unmatched Offsets of %(account)s"
 msgstr ""
 
@@ -1409,17 +1409,17 @@
 msgid "Download"
 msgstr ""
 
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr ""
 
-#: src/accounting/utils/pagination.py:206
+#: src/accounting/utils/pagination.py:207
 msgctxt "Pagination|"
 msgid "Previous"
 msgstr ""
 
-#: src/accounting/utils/pagination.py:255
+#: src/accounting/utils/pagination.py:256
 msgctxt "Pagination|"
 msgid "Next"
 msgstr ""
```

### Comparing `mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.7/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-18 09:32+0800\n"
-"PO-Revision-Date: 2023-04-18 09:32+0800\n"
+"POT-Creation-Date: 2023-07-29 08:55+0800\n"
+"PO-Revision-Date: 2023-07-29 08:56+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -50,24 +50,24 @@
 
 msgid "Accounting"
 msgstr "记帐"
 
 msgid "Accounts"
 msgstr "科目"
 
-msgid "Accounts with Unapplied Items"
+msgid "Accounts With Unapplied Items"
 msgstr "含未抵销项目的科目"
 
-msgid "Accounts with Unapplied Items in %(currency)s"
+msgid "Accounts With Unapplied Items in %(currency)s"
 msgstr "%(currency)s含未抵销项目的科目"
 
-msgid "Accounts with Unmatched Offsets"
+msgid "Accounts With Unmatched Offsets"
 msgstr "含遗漏抵销项目的科目"
 
-msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgid "Accounts With Unmatched Offsets in %(currency)s"
 msgstr "%(currency)s含遗漏抵销项目的科目"
 
 msgid "Add a New Account"
 msgstr "添加科目"
 
 msgid "Add a New Cash Disbursement Journal Entry"
 msgstr "添加现金支出传票"
@@ -77,14 +77,17 @@
 
 msgid "Add a New Currency"
 msgstr "添加货币"
 
 msgid "Add a New Transfer Journal Entry"
 msgstr "添加转帐传票"
 
+msgid "After Tax Income"
+msgstr "税后净利"
+
 msgid "All"
 msgstr "全部"
 
 msgid "Amount"
 msgstr "金额"
 
 msgid "Annotation"
@@ -122,14 +125,17 @@
 
 msgid "Base Accounts"
 msgstr "基本科目"
 
 msgid "Base account"
 msgstr "基本科目"
 
+msgid "Before Tax Income"
+msgstr "税前净利"
+
 msgid "Brought forward"
 msgstr "前期转入"
 
 msgid "Bus"
 msgstr "公车"
 
 msgid "Can match %(item)s"
@@ -271,14 +277,17 @@
 
 msgid "Fully offset"
 msgstr "全部抵销"
 
 msgid "General"
 msgstr "一般"
 
+msgid "Gross Income"
+msgstr "营业毛利"
+
 msgid "Income"
 msgstr "收入"
 
 msgid "Income Statement"
 msgstr "损益表"
 
 msgid "Income Statement %(period)s"
@@ -364,14 +373,17 @@
 
 msgid "Needs Offset"
 msgstr "需抵销"
 
 msgid "Net Balance"
 msgstr "净额"
 
+msgid "Net Income or Loss for Current Period"
+msgstr "本期损益"
+
 msgid "Net balance"
 msgstr "净额"
 
 msgid "New"
 msgstr "添加"
 
 msgctxt "Pagination|"
@@ -395,14 +407,17 @@
 
 msgid "Offset..."
 msgstr "抵销…"
 
 msgid "Offsets"
 msgstr "抵销"
 
+msgid "Operating Income"
+msgstr "营业净利"
+
 msgid "Order"
 msgstr "次序"
 
 msgid "Original Line Item"
 msgstr "原始分录"
 
 msgid "Page navigation"
@@ -719,14 +734,17 @@
 
 msgid "Tomorrow"
 msgstr "明天"
 
 msgid "Total"
 msgstr "合计"
 
+msgid "Total Operating Revenue"
+msgstr "营业收入总额"
+
 msgid "Transfer"
 msgstr "转帐"
 
 msgid "Transfer Journal Entry#%(id)s"
 msgstr "转帐传票#%(id)s"
 
 msgid "Travel"
@@ -776,42 +794,24 @@
 
 msgid "You cannot select a payable account as expense."
 msgstr "支出不能选应付科目。"
 
 msgid "You cannot select a receivable account as income."
 msgstr "收入不能选应收科目。"
 
-msgid "after tax income"
-msgstr "税后净利"
-
-msgid "before tax income"
-msgstr "税前净利"
-
 msgid "current assets and liabilities"
 msgstr "流动资产与负债"
 
 msgid "for all time"
 msgstr "全部"
 
-msgid "gross income"
-msgstr "营业毛利"
-
 msgid "in %(period)s"
 msgstr "%(period)s"
 
 msgid "in %(start)s-%(end)s"
 msgstr "%(start)s-%(end)s"
 
-msgid "net income or loss for current period"
-msgstr "本期损益"
-
-msgid "operating income"
-msgstr "营业净利"
-
 msgid "since %(start)s"
 msgstr "%(start)s至今"
 
-msgid "total operating revenue"
-msgstr "营业收入总额"
-
 msgid "until %(end)s"
 msgstr "%(end)s前"
```

### Comparing `mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.7/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-18 09:32+0800\n"
-"PO-Revision-Date: 2023-04-18 09:32+0800\n"
+"POT-Creation-Date: 2023-07-29 08:55+0800\n"
+"PO-Revision-Date: 2023-07-29 08:56+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: src/accounting/forms.py:33
 #: src/accounting/static/js/journal-entry-form.js:1080
-#: src/accounting/static/js/journal-entry-line-item-editor.js:411
+#: src/accounting/static/js/journal-entry-line-item-editor.js:415
 #: src/accounting/static/js/option-form.js:537
 #: src/accounting/static/js/option-form.js:803
 msgid "Please select the account."
 msgstr "请选择科目。"
 
 #: src/accounting/forms.py:44
 msgid "The currency does not exist."
 msgstr "没有这个货币。"
 
 #: src/accounting/forms.py:55 src/accounting/option/forms.py:42
 msgid "The account does not exist."
 msgstr "没有这个科目。"
 
-#: src/accounting/models.py:581
+#: src/accounting/models.py:578
 #, python-format
 msgid "Cash Disbursement Journal Entry#%(id)s"
 msgstr "现金支出传票#%(id)s"
 
-#: src/accounting/models.py:584
+#: src/accounting/models.py:581
 #, python-format
 msgid "Cash Receipt Journal Entry#%(id)s"
 msgstr "现金收入传票#%(id)s"
 
-#: src/accounting/models.py:585
+#: src/accounting/models.py:582
 #, python-format
 msgid "Transfer Journal Entry#%(id)s"
 msgstr "转帐传票#%(id)s"
 
-#: src/accounting/models.py:714
+#: src/accounting/models.py:706
 #, python-format
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
 #: src/accounting/report/period/shortcuts.py:121
 #: src/accounting/template_filters.py:52
 #: src/accounting/templates/accounting/report/include/period-chooser.html:99
@@ -97,15 +97,15 @@
 msgstr "请选择基本科目。"
 
 #: src/accounting/account/forms.py:81
 msgid "Please fill in the title"
 msgstr "请填上标题。"
 
 #: src/accounting/account/queries.py:50
-#: src/accounting/report/reports/search.py:101
+#: src/accounting/report/reports/search.py:100
 #: src/accounting/templates/accounting/account/detail.html:97
 #: src/accounting/templates/accounting/account/list.html:62
 msgid "Needs Offset"
 msgstr "需抵销"
 
 #: src/accounting/account/views.py:90
 msgid "The account is added successfully"
@@ -201,32 +201,32 @@
 msgid "The journal entry cannot be deleted."
 msgstr "传票不可删除。"
 
 #: src/accounting/journal_entry/views.py:184
 msgid "The journal entry is deleted successfully."
 msgstr "传票删掉了"
 
-#: src/accounting/journal_entry/forms/currency.py:39
+#: src/accounting/journal_entry/forms/currency.py:38
 msgid "Please select the currency."
 msgstr "请选择货币。"
 
-#: src/accounting/journal_entry/forms/currency.py:62
+#: src/accounting/journal_entry/forms/currency.py:61
 msgid "The currency must be the same as the original line item."
 msgstr "货币需和原始分录相同。"
 
-#: src/accounting/journal_entry/forms/currency.py:89
+#: src/accounting/journal_entry/forms/currency.py:88
 msgid "The currency must not be changed when there is offset."
 msgstr "抵销过不可变更货币。"
 
-#: src/accounting/journal_entry/forms/currency.py:98
+#: src/accounting/journal_entry/forms/currency.py:97
 #: src/accounting/static/js/journal-entry-form.js:773
 msgid "Please add some line items."
 msgstr "请加上分录。"
 
-#: src/accounting/journal_entry/forms/currency.py:111
+#: src/accounting/journal_entry/forms/currency.py:110
 #: src/accounting/static/js/journal-entry-form.js:522
 msgid "The totals of the debit and credit amounts do not match."
 msgstr "借方贷方合计不符。 "
 
 #: src/accounting/journal_entry/forms/journal_entry.py:48
 #: src/accounting/static/js/journal-entry-form.js:264
 #: src/accounting/static/js/period-chooser.js:265
@@ -247,70 +247,70 @@
 msgid "Please add some currencies."
 msgstr "请加上货币。"
 
 #: src/accounting/journal_entry/forms/journal_entry.py:104
 msgid "Line items with offset cannot be deleted."
 msgstr "无法删除抵销过的分录。"
 
-#: src/accounting/journal_entry/forms/line_item.py:49
+#: src/accounting/journal_entry/forms/line_item.py:48
 msgid "The original line item does not exist."
 msgstr "没有这笔原始分录。"
 
-#: src/accounting/journal_entry/forms/line_item.py:70
+#: src/accounting/journal_entry/forms/line_item.py:69
 msgid "The original line item is on the same debit or credit."
 msgstr "原始分录在借贷同一边。"
 
-#: src/accounting/journal_entry/forms/line_item.py:85
+#: src/accounting/journal_entry/forms/line_item.py:84
 msgid "The original line item does not need offset."
 msgstr "这笔原始分录不需抵销。"
 
-#: src/accounting/journal_entry/forms/line_item.py:101
+#: src/accounting/journal_entry/forms/line_item.py:100
 msgid "The original line item cannot be an offset item."
 msgstr "原始分录不可以是抵销分录。"
 
-#: src/accounting/journal_entry/forms/line_item.py:119
+#: src/accounting/journal_entry/forms/line_item.py:118
 msgid "The account must be the same as the original line item."
 msgstr "科目需和原始分录相同。"
 
-#: src/accounting/journal_entry/forms/line_item.py:135
+#: src/accounting/journal_entry/forms/line_item.py:134
 msgid "The account must not be changed when there is offset."
 msgstr "抵销过不可变更科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:151
+#: src/accounting/journal_entry/forms/line_item.py:150
 msgid "A payable line item cannot start from debit."
 msgstr "不可由借方新建应付款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:167
+#: src/accounting/journal_entry/forms/line_item.py:166
 msgid "A receivable line item cannot start from credit."
 msgstr "不可由贷方新建应收款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:178
-#: src/accounting/static/js/journal-entry-line-item-editor.js:436
+#: src/accounting/journal_entry/forms/line_item.py:177
+#: src/accounting/static/js/journal-entry-line-item-editor.js:440
 msgid "Please fill in a positive amount."
 msgstr "金额请填正数。"
 
-#: src/accounting/journal_entry/forms/line_item.py:220
-#: src/accounting/static/js/journal-entry-line-item-editor.js:442
+#: src/accounting/journal_entry/forms/line_item.py:219
+#: src/accounting/static/js/journal-entry-line-item-editor.js:446
 #, python-format
 msgid ""
 "The amount must not exceed the net balance %(balance)s of the original "
 "line item."
 msgstr "金额不可超过原始分录净额 %(balance)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:241
-#: src/accounting/static/js/journal-entry-line-item-editor.js:450
+#: src/accounting/journal_entry/forms/line_item.py:239
+#: src/accounting/static/js/journal-entry-line-item-editor.js:454
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr "金额不可低于抵销总额 %(total)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:426
+#: src/accounting/journal_entry/forms/line_item.py:424
 msgid "This account is not for debit line items."
 msgstr "科目不是借方科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:478
+#: src/accounting/journal_entry/forms/line_item.py:476
 msgid "This account is not for credit line items."
 msgstr "科目不是贷方科目。"
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr "这不是流动科目。"
 
@@ -413,23 +413,23 @@
 msgstr "去年"
 
 #: src/accounting/report/period/shortcuts.py:146
 #: src/accounting/templates/accounting/report/include/period-chooser.html:122
 msgid "All"
 msgstr "全部"
 
-#: src/accounting/report/reports/balance_sheet.py:423
-#: src/accounting/report/reports/balance_sheet.py:427
-#: src/accounting/report/reports/balance_sheet.py:439
+#: src/accounting/report/reports/balance_sheet.py:425
+#: src/accounting/report/reports/balance_sheet.py:429
 #: src/accounting/report/reports/balance_sheet.py:441
-#: src/accounting/report/reports/income_expenses.py:189
-#: src/accounting/report/reports/income_expenses.py:423
-#: src/accounting/report/reports/income_statement.py:300
-#: src/accounting/report/reports/ledger.py:171
-#: src/accounting/report/reports/ledger.py:380
+#: src/accounting/report/reports/balance_sheet.py:443
+#: src/accounting/report/reports/income_expenses.py:187
+#: src/accounting/report/reports/income_expenses.py:420
+#: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/ledger.py:168
+#: src/accounting/report/reports/ledger.py:376
 #: src/accounting/report/reports/trial_balance.py:229
 #: src/accounting/templates/accounting/journal-entry/disbursement/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html:38
 #: src/accounting/templates/accounting/journal-entry/receipt/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:39
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:55
 #: src/accounting/templates/accounting/report/balance-sheet.html:65
@@ -441,120 +441,120 @@
 #: src/accounting/templates/accounting/report/income-expenses.html:81
 #: src/accounting/templates/accounting/report/income-statement.html:89
 #: src/accounting/templates/accounting/report/ledger.html:82
 #: src/accounting/templates/accounting/report/trial-balance.html:80
 msgid "Total"
 msgstr "合计"
 
-#: src/accounting/report/reports/income_expenses.py:136
-#: src/accounting/report/reports/ledger.py:132
+#: src/accounting/report/reports/income_expenses.py:134
+#: src/accounting/report/reports/ledger.py:129
 msgid "Brought forward"
 msgstr "前期转入"
 
-#: src/accounting/report/reports/income_expenses.py:407
+#: src/accounting/report/reports/income_expenses.py:404
 #: src/accounting/report/reports/journal.py:158
-#: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/ledger.py:362
 #: src/accounting/report/reports/unapplied.py:148
 #: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
 #: src/accounting/templates/accounting/report/unapplied.html:52
 #: src/accounting/templates/accounting/report/unmatched.html:93
 msgid "Date"
 msgstr "日期"
 
-#: src/accounting/report/reports/income_expenses.py:407
+#: src/accounting/report/reports/income_expenses.py:404
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/report/reports/unapplied_accounts.py:122
 #: src/accounting/report/reports/unmatched_accounts.py:122
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:58
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:40
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
 #: src/accounting/templates/accounting/report/trial-balance.html:61
 msgid "Account"
 msgstr "科目"
 
-#: src/accounting/report/reports/income_expenses.py:408
+#: src/accounting/report/reports/income_expenses.py:405
 #: src/accounting/report/reports/journal.py:159
-#: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/ledger.py:362
 #: src/accounting/report/reports/unapplied.py:149
 #: src/accounting/report/reports/unmatched.py:159
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:29
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:50
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
 #: src/accounting/templates/accounting/report/unapplied.html:53
 #: src/accounting/templates/accounting/report/unmatched.html:94
 msgid "Description"
 msgstr "摘要"
 
-#: src/accounting/report/reports/income_expenses.py:408
+#: src/accounting/report/reports/income_expenses.py:405
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr "收入"
 
-#: src/accounting/report/reports/income_expenses.py:409
+#: src/accounting/report/reports/income_expenses.py:406
 #: src/accounting/templates/accounting/report/income-expenses.html:59
 msgid "Expense"
 msgstr "支出"
 
-#: src/accounting/report/reports/income_expenses.py:409
-#: src/accounting/report/reports/ledger.py:368
+#: src/accounting/report/reports/income_expenses.py:406
+#: src/accounting/report/reports/ledger.py:364
 #: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
 #: src/accounting/templates/accounting/report/unmatched.html:97
 msgid "Balance"
 msgstr "余额"
 
-#: src/accounting/report/reports/income_expenses.py:410
+#: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:161
-#: src/accounting/report/reports/ledger.py:368
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
+#: src/accounting/report/reports/ledger.py:364
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:179
 #: src/accounting/templates/accounting/journal-entry/include/form.html:73
 msgid "Note"
 msgstr "备注"
 
-#: src/accounting/report/reports/income_statement.py:228
-msgid "total operating revenue"
+#: src/accounting/report/reports/income_statement.py:229
+msgid "Total Operating Revenue"
 msgstr "营业收入总额"
 
-#: src/accounting/report/reports/income_statement.py:229
-msgid "gross income"
+#: src/accounting/report/reports/income_statement.py:230
+msgid "Gross Income"
 msgstr "营业毛利"
 
-#: src/accounting/report/reports/income_statement.py:230
-msgid "operating income"
+#: src/accounting/report/reports/income_statement.py:231
+msgid "Operating Income"
 msgstr "营业净利"
 
-#: src/accounting/report/reports/income_statement.py:231
-msgid "before tax income"
+#: src/accounting/report/reports/income_statement.py:232
+msgid "Before Tax Income"
 msgstr "税前净利"
 
-#: src/accounting/report/reports/income_statement.py:232
-msgid "after tax income"
+#: src/accounting/report/reports/income_statement.py:233
+msgid "After Tax Income"
 msgstr "税后净利"
 
-#: src/accounting/report/reports/income_statement.py:233
-msgid "net income or loss for current period"
+#: src/accounting/report/reports/income_statement.py:234
+msgid "Net Income or Loss for Current Period"
 msgstr "本期损益"
 
-#: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/income_statement.py:302
 #: src/accounting/report/reports/unapplied.py:149
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:66
 #: src/accounting/templates/accounting/report/income-statement.html:61
 #: src/accounting/templates/accounting/report/unapplied.html:54
 msgid "Amount"
 msgstr "金额"
 
 #: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/unapplied.py:148
@@ -563,29 +563,29 @@
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
 msgid "Currency"
 msgstr "货币"
 
 #: src/accounting/report/reports/journal.py:160
-#: src/accounting/report/reports/ledger.py:367
+#: src/accounting/report/reports/ledger.py:363
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
 #: src/accounting/templates/accounting/report/trial-balance.html:62
 #: src/accounting/templates/accounting/report/unmatched.html:95
 msgid "Debit"
 msgstr "借方"
 
 #: src/accounting/report/reports/journal.py:160
-#: src/accounting/report/reports/ledger.py:367
+#: src/accounting/report/reports/ledger.py:363
 #: src/accounting/report/reports/trial_balance.py:226
 #: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
@@ -610,24 +610,24 @@
 #: src/accounting/report/reports/unapplied_accounts.py:122
 #: src/accounting/report/reports/unmatched_accounts.py:122
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:59
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:59
 msgid "Count"
 msgstr "数量"
 
-#: src/accounting/report/utils/offset_matcher.py:163
+#: src/accounting/report/utils/offset_matcher.py:161
 msgid "There is no unmatched offset."
 msgstr "没有遗漏的抵销分录"
 
-#: src/accounting/report/utils/offset_matcher.py:167
+#: src/accounting/report/utils/offset_matcher.py:165
 #, python-format
 msgid "%(total)s unmatched offsets without original items."
 msgstr "%(total)s 笔遗漏的抵销分录无法自动抵销。"
 
-#: src/accounting/report/utils/offset_matcher.py:172
+#: src/accounting/report/utils/offset_matcher.py:170
 #, python-format
 msgid ""
 "%(matches)s unmatched offsets out of %(total)s can match with their "
 "original items."
 msgstr "%(total)s 笔遗漏的抵销分录中，可配对抵销掉 %(matches)s 笔。"
 
 #: src/accounting/report/utils/report_chooser.py:86
@@ -748,15 +748,15 @@
 msgstr "十一月"
 
 #: src/accounting/static/js/description-editor.js:1195
 msgid "December"
 msgstr "十二月"
 
 #: src/accounting/static/js/journal-entry-form.js:1085
-#: src/accounting/static/js/journal-entry-line-item-editor.js:430
+#: src/accounting/static/js/journal-entry-line-item-editor.js:434
 msgid "Please fill in the amount."
 msgstr "请填上金额。"
 
 #: src/accounting/static/js/journal-entry-form.js:1107
 #: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:37
 #: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:41
 #, python-format
@@ -829,39 +829,39 @@
 msgid "Confirm Delete Account"
 msgstr "确认删除科目"
 
 #: src/accounting/templates/accounting/account/detail.html:77
 #: src/accounting/templates/accounting/account/include/form.html:91
 #: src/accounting/templates/accounting/currency/detail.html:73
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:27
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:30
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:31
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:29
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:29
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
 #: src/accounting/templates/accounting/report/unmatched.html:58
 msgid "Close"
 msgstr "关闭"
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr "你确定要删掉这个科目吗？"
 
 #: src/accounting/templates/accounting/account/detail.html:83
 #: src/accounting/templates/accounting/account/include/form.html:112
 #: src/accounting/templates/accounting/currency/detail.html:79
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:195
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:71
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:66
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
 #: src/accounting/templates/accounting/report/unmatched.html:74
 msgid "Cancel"
 msgstr "取消"
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
@@ -938,20 +938,20 @@
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr "%(base)s下的科目"
 
 #: src/accounting/templates/accounting/account/include/form.html:75
 #: src/accounting/templates/accounting/account/order.html:62
 #: src/accounting/templates/accounting/currency/include/form.html:57
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:195
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:196
 #: src/accounting/templates/accounting/journal-entry/include/form.html:80
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:71
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:72
 #: src/accounting/templates/accounting/journal-entry/order.html:61
 #: src/accounting/templates/accounting/option/form.html:80
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:66
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:67
 msgid "Save"
 msgstr "保存"
 
 #: src/accounting/templates/accounting/account/include/form.html:45
 msgid "Base account"
 msgstr "基本科目"
 
@@ -1004,15 +1004,15 @@
 msgstr "货币管理"
 
 #: src/accounting/templates/accounting/currency/include/form.html:44
 msgid "Code"
 msgstr "代码"
 
 #: src/accounting/templates/accounting/currency/include/form.html:50
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:33
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:34
 msgid "Name"
 msgstr "名称"
 
 #: src/accounting/templates/accounting/include/nav.html:27
 msgid "Accounting"
 msgstr "记帐"
 
@@ -1073,61 +1073,61 @@
 msgid "Select Account"
 msgstr "选择科目"
 
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:44
 msgid "More…"
 msgstr "更多…"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:36
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:37
 msgid "Offset..."
 msgstr "抵销…"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:44
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:45
 msgid "General"
 msgstr "一般"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:49
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:50
 msgid "Travel"
 msgstr "差旅"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:54
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:55
 msgid "Bus"
 msgstr "公车"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:59
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:60
 msgid "Recurring"
 msgstr "常用"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:64
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:65
 msgid "Annotation"
 msgstr "注记"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:73
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:90
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:125
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:74
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:91
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:126
 msgid "Tag"
 msgstr "标签"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:105
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:146
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:106
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:147
 #: src/accounting/templates/accounting/report/include/period-chooser.html:129
 msgid "From"
 msgstr "从"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:114
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:151
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:115
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:152
 #: src/accounting/templates/accounting/report/include/period-chooser.html:135
 msgid "To"
 msgstr "至"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:130
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:131
 msgid "Route"
 msgstr "路线"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:172
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:173
 msgid "The Number of Items"
 msgstr "数量"
 
 #: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:45
 #: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:46
 msgid "Offsets"
 msgstr "抵销"
@@ -1151,19 +1151,19 @@
 msgid "Confirm Delete Journal Entry"
 msgstr "确认删除传票"
 
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:81
 msgid "Do you really want to delete this journal entry?"
 msgstr "你确定要删掉这张传票吗？"
 
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:27
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 msgid "Line Item Content"
 msgstr "分录内容"
 
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:34
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:35
 msgid "Original Line Item"
 msgstr "原始分录"
 
 #: src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html:25
 #: src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html:26
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:31
 msgid "Cash Disbursement"
@@ -1211,51 +1211,51 @@
 
 #: src/accounting/templates/accounting/option/detail.html:70
 #: src/accounting/templates/accounting/option/form.html:72
 #: src/accounting/templates/accounting/option/form.html:96
 msgid "Recurring Income"
 msgstr "常用收入"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:47
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:48
 msgid "Description Template"
 msgstr "摘要范本"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:52
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:53
 msgid "Available template variables:"
 msgstr "范本变量说明："
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:54
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:55
 msgid "This month, as a number."
 msgstr "这个月的数字。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:55
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:56
 msgid "This month, in its name."
 msgstr "这个月的名称。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:56
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:57
 msgid "Last month, as a number."
 msgstr "上个月的数字。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:57
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:58
 msgid "Last month, in its name."
 msgstr "上个月的名称。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:58
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:59
 msgid "The previous bimonthly period, as numbers."
 msgstr "前个双月期的数字。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:59
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:60
 msgid "The previous bimonthly period, as their names."
 msgstr "前个双月期的名称。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:62
 msgid "Example:"
 msgstr "范例："
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:62
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水费{last_bimonthly_number}月"
 
 #: src/accounting/templates/accounting/report/balance-sheet.html:29
 #: src/accounting/templates/accounting/report/balance-sheet.html:51
 #, python-format
 msgid "Balance Sheet %(period)s"
@@ -1314,42 +1314,42 @@
 #: src/accounting/templates/accounting/report/trial-balance.html:53
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s试算表"
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:29
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:49
-msgid "Accounts with Unapplied Items"
+msgid "Accounts With Unapplied Items"
 msgstr "含未抵销项目的科目"
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:29
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:51
 #, python-format
-msgid "Accounts with Unapplied Items in %(currency)s"
+msgid "Accounts With Unapplied Items in %(currency)s"
 msgstr "%(currency)s含未抵销项目的科目"
 
 #: src/accounting/templates/accounting/report/unapplied.html:29
 #, python-format
 msgid "Unapplied Items of %(account)s"
 msgstr "%(account)s未抵销项目"
 
 #: src/accounting/templates/accounting/report/unapplied.html:29
 #, python-format
 msgid "Unapplied Items of %(account)s in %(currency)s"
 msgstr "%(currency)s%(account)s未抵销项目"
 
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:29
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:49
-msgid "Accounts with Unmatched Offsets"
+msgid "Accounts With Unmatched Offsets"
 msgstr "含遗漏抵销项目的科目"
 
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:29
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:51
 #, python-format
-msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgid "Accounts With Unmatched Offsets in %(currency)s"
 msgstr "%(currency)s含遗漏抵销项目的科目"
 
 #: src/accounting/templates/accounting/report/unmatched.html:29
 #, python-format
 msgid "Unmatched Offsets of %(account)s"
 msgstr "%(account)s遗漏的抵销项目"
 
@@ -1411,17 +1411,17 @@
 msgid "Download"
 msgstr "下载"
 
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流动资产与负债"
 
-#: src/accounting/utils/pagination.py:206
+#: src/accounting/utils/pagination.py:207
 msgctxt "Pagination|"
 msgid "Previous"
 msgstr "上一页"
 
-#: src/accounting/utils/pagination.py:255
+#: src/accounting/utils/pagination.py:256
 msgctxt "Pagination|"
 msgid "Next"
 msgstr "下一页"
```

### Comparing `mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.7/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-18 09:32+0800\n"
-"PO-Revision-Date: 2023-04-18 09:32+0800\n"
+"POT-Creation-Date: 2023-07-29 08:55+0800\n"
+"PO-Revision-Date: 2023-07-29 08:56+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -50,24 +50,24 @@
 
 msgid "Accounting"
 msgstr "記帳"
 
 msgid "Accounts"
 msgstr "科目"
 
-msgid "Accounts with Unapplied Items"
+msgid "Accounts With Unapplied Items"
 msgstr "含未抵銷項目的科目"
 
-msgid "Accounts with Unapplied Items in %(currency)s"
+msgid "Accounts With Unapplied Items in %(currency)s"
 msgstr "%(currency)s含未抵銷項目的科目"
 
-msgid "Accounts with Unmatched Offsets"
+msgid "Accounts With Unmatched Offsets"
 msgstr "含遺漏抵銷項目的科目"
 
-msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgid "Accounts With Unmatched Offsets in %(currency)s"
 msgstr "%(currency)s含遺漏抵銷項目的科目"
 
 msgid "Add a New Account"
 msgstr "新增科目"
 
 msgid "Add a New Cash Disbursement Journal Entry"
 msgstr "新增現金支出傳票"
@@ -77,14 +77,17 @@
 
 msgid "Add a New Currency"
 msgstr "新增貨幣"
 
 msgid "Add a New Transfer Journal Entry"
 msgstr "新增轉帳傳票"
 
+msgid "After Tax Income"
+msgstr "稅後淨利"
+
 msgid "All"
 msgstr "全部"
 
 msgid "Amount"
 msgstr "金額"
 
 msgid "Annotation"
@@ -122,14 +125,17 @@
 
 msgid "Base Accounts"
 msgstr "基本科目"
 
 msgid "Base account"
 msgstr "基本科目"
 
+msgid "Before Tax Income"
+msgstr "稅前淨利"
+
 msgid "Brought forward"
 msgstr "前期轉入"
 
 msgid "Bus"
 msgstr "公車"
 
 msgid "Can match %(item)s"
@@ -271,14 +277,17 @@
 
 msgid "Fully offset"
 msgstr "全部抵銷"
 
 msgid "General"
 msgstr "一般"
 
+msgid "Gross Income"
+msgstr "營業毛利"
+
 msgid "Income"
 msgstr "收入"
 
 msgid "Income Statement"
 msgstr "損益表"
 
 msgid "Income Statement %(period)s"
@@ -364,14 +373,17 @@
 
 msgid "Needs Offset"
 msgstr "需抵銷"
 
 msgid "Net Balance"
 msgstr "淨額"
 
+msgid "Net Income or Loss for Current Period"
+msgstr "本期損益"
+
 msgid "Net balance"
 msgstr "淨額"
 
 msgid "New"
 msgstr "新增"
 
 msgctxt "Pagination|"
@@ -395,14 +407,17 @@
 
 msgid "Offset..."
 msgstr "抵銷…"
 
 msgid "Offsets"
 msgstr "抵銷"
 
+msgid "Operating Income"
+msgstr "營業淨利"
+
 msgid "Order"
 msgstr "次序"
 
 msgid "Original Line Item"
 msgstr "原始分錄"
 
 msgid "Page navigation"
@@ -719,14 +734,17 @@
 
 msgid "Tomorrow"
 msgstr "明天"
 
 msgid "Total"
 msgstr "合計"
 
+msgid "Total Operating Revenue"
+msgstr "營業收入總額"
+
 msgid "Transfer"
 msgstr "轉帳"
 
 msgid "Transfer Journal Entry#%(id)s"
 msgstr "轉帳傳票#%(id)s"
 
 msgid "Travel"
@@ -776,42 +794,24 @@
 
 msgid "You cannot select a payable account as expense."
 msgstr "支出不能選應付科目。"
 
 msgid "You cannot select a receivable account as income."
 msgstr "收入不能選應收科目。"
 
-msgid "after tax income"
-msgstr "稅後淨利"
-
-msgid "before tax income"
-msgstr "稅前淨利"
-
 msgid "current assets and liabilities"
 msgstr "流動資產與負債"
 
 msgid "for all time"
 msgstr "全部"
 
-msgid "gross income"
-msgstr "營業毛利"
-
 msgid "in %(period)s"
 msgstr "%(period)s"
 
 msgid "in %(start)s-%(end)s"
 msgstr "%(start)s-%(end)s"
 
-msgid "net income or loss for current period"
-msgstr "本期損益"
-
-msgid "operating income"
-msgstr "營業淨利"
-
 msgid "since %(start)s"
 msgstr "%(start)s至今"
 
-msgid "total operating revenue"
-msgstr "營業收入總額"
-
 msgid "until %(end)s"
 msgstr "%(end)s前"
```

### Comparing `mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.7/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-18 09:32+0800\n"
-"PO-Revision-Date: 2023-04-18 09:32+0800\n"
+"POT-Creation-Date: 2023-07-29 08:55+0800\n"
+"PO-Revision-Date: 2023-07-29 08:56+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: src/accounting/forms.py:33
 #: src/accounting/static/js/journal-entry-form.js:1080
-#: src/accounting/static/js/journal-entry-line-item-editor.js:411
+#: src/accounting/static/js/journal-entry-line-item-editor.js:415
 #: src/accounting/static/js/option-form.js:537
 #: src/accounting/static/js/option-form.js:803
 msgid "Please select the account."
 msgstr "請選擇科目。"
 
 #: src/accounting/forms.py:44
 msgid "The currency does not exist."
 msgstr "沒有這個貨幣。"
 
 #: src/accounting/forms.py:55 src/accounting/option/forms.py:42
 msgid "The account does not exist."
 msgstr "沒有這個科目。"
 
-#: src/accounting/models.py:581
+#: src/accounting/models.py:578
 #, python-format
 msgid "Cash Disbursement Journal Entry#%(id)s"
 msgstr "現金支出傳票#%(id)s"
 
-#: src/accounting/models.py:584
+#: src/accounting/models.py:581
 #, python-format
 msgid "Cash Receipt Journal Entry#%(id)s"
 msgstr "現金收入傳票#%(id)s"
 
-#: src/accounting/models.py:585
+#: src/accounting/models.py:582
 #, python-format
 msgid "Transfer Journal Entry#%(id)s"
 msgstr "轉帳傳票#%(id)s"
 
-#: src/accounting/models.py:714
+#: src/accounting/models.py:706
 #, python-format
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
 #: src/accounting/report/period/shortcuts.py:121
 #: src/accounting/template_filters.py:52
 #: src/accounting/templates/accounting/report/include/period-chooser.html:99
@@ -97,15 +97,15 @@
 msgstr "請選擇基本科目。"
 
 #: src/accounting/account/forms.py:81
 msgid "Please fill in the title"
 msgstr "請填上標題。"
 
 #: src/accounting/account/queries.py:50
-#: src/accounting/report/reports/search.py:101
+#: src/accounting/report/reports/search.py:100
 #: src/accounting/templates/accounting/account/detail.html:97
 #: src/accounting/templates/accounting/account/list.html:62
 msgid "Needs Offset"
 msgstr "需抵銷"
 
 #: src/accounting/account/views.py:90
 msgid "The account is added successfully"
@@ -201,32 +201,32 @@
 msgid "The journal entry cannot be deleted."
 msgstr "傳票不可刪除。"
 
 #: src/accounting/journal_entry/views.py:184
 msgid "The journal entry is deleted successfully."
 msgstr "傳票刪掉了"
 
-#: src/accounting/journal_entry/forms/currency.py:39
+#: src/accounting/journal_entry/forms/currency.py:38
 msgid "Please select the currency."
 msgstr "請選擇貨幣。"
 
-#: src/accounting/journal_entry/forms/currency.py:62
+#: src/accounting/journal_entry/forms/currency.py:61
 msgid "The currency must be the same as the original line item."
 msgstr "貨幣需和原始分錄相同。"
 
-#: src/accounting/journal_entry/forms/currency.py:89
+#: src/accounting/journal_entry/forms/currency.py:88
 msgid "The currency must not be changed when there is offset."
 msgstr "抵銷過不可變更貨幣。"
 
-#: src/accounting/journal_entry/forms/currency.py:98
+#: src/accounting/journal_entry/forms/currency.py:97
 #: src/accounting/static/js/journal-entry-form.js:773
 msgid "Please add some line items."
 msgstr "請加上分錄。"
 
-#: src/accounting/journal_entry/forms/currency.py:111
+#: src/accounting/journal_entry/forms/currency.py:110
 #: src/accounting/static/js/journal-entry-form.js:522
 msgid "The totals of the debit and credit amounts do not match."
 msgstr "借方貸方合計不符。 "
 
 #: src/accounting/journal_entry/forms/journal_entry.py:48
 #: src/accounting/static/js/journal-entry-form.js:264
 #: src/accounting/static/js/period-chooser.js:265
@@ -247,70 +247,70 @@
 msgid "Please add some currencies."
 msgstr "請加上貨幣。"
 
 #: src/accounting/journal_entry/forms/journal_entry.py:104
 msgid "Line items with offset cannot be deleted."
 msgstr "無法刪除抵銷過的分錄。"
 
-#: src/accounting/journal_entry/forms/line_item.py:49
+#: src/accounting/journal_entry/forms/line_item.py:48
 msgid "The original line item does not exist."
 msgstr "沒有這筆原始分錄。"
 
-#: src/accounting/journal_entry/forms/line_item.py:70
+#: src/accounting/journal_entry/forms/line_item.py:69
 msgid "The original line item is on the same debit or credit."
 msgstr "原始分錄在借貸同一邊。"
 
-#: src/accounting/journal_entry/forms/line_item.py:85
+#: src/accounting/journal_entry/forms/line_item.py:84
 msgid "The original line item does not need offset."
 msgstr "這筆原始分錄不需抵銷。"
 
-#: src/accounting/journal_entry/forms/line_item.py:101
+#: src/accounting/journal_entry/forms/line_item.py:100
 msgid "The original line item cannot be an offset item."
 msgstr "原始分錄不可以是抵銷分錄。"
 
-#: src/accounting/journal_entry/forms/line_item.py:119
+#: src/accounting/journal_entry/forms/line_item.py:118
 msgid "The account must be the same as the original line item."
 msgstr "科目需和原始分錄相同。"
 
-#: src/accounting/journal_entry/forms/line_item.py:135
+#: src/accounting/journal_entry/forms/line_item.py:134
 msgid "The account must not be changed when there is offset."
 msgstr "抵銷過不可變更科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:151
+#: src/accounting/journal_entry/forms/line_item.py:150
 msgid "A payable line item cannot start from debit."
 msgstr "不可由借方新建應付款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:167
+#: src/accounting/journal_entry/forms/line_item.py:166
 msgid "A receivable line item cannot start from credit."
 msgstr "不可由貸方新建應收款。"
 
-#: src/accounting/journal_entry/forms/line_item.py:178
-#: src/accounting/static/js/journal-entry-line-item-editor.js:436
+#: src/accounting/journal_entry/forms/line_item.py:177
+#: src/accounting/static/js/journal-entry-line-item-editor.js:440
 msgid "Please fill in a positive amount."
 msgstr "金額請填正數。"
 
-#: src/accounting/journal_entry/forms/line_item.py:220
-#: src/accounting/static/js/journal-entry-line-item-editor.js:442
+#: src/accounting/journal_entry/forms/line_item.py:219
+#: src/accounting/static/js/journal-entry-line-item-editor.js:446
 #, python-format
 msgid ""
 "The amount must not exceed the net balance %(balance)s of the original "
 "line item."
 msgstr "金額不可超過原始分錄凈額 %(balance)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:241
-#: src/accounting/static/js/journal-entry-line-item-editor.js:450
+#: src/accounting/journal_entry/forms/line_item.py:239
+#: src/accounting/static/js/journal-entry-line-item-editor.js:454
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr "金額不可低於抵銷總額 %(total)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:426
+#: src/accounting/journal_entry/forms/line_item.py:424
 msgid "This account is not for debit line items."
 msgstr "科目不是借方科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:478
+#: src/accounting/journal_entry/forms/line_item.py:476
 msgid "This account is not for credit line items."
 msgstr "科目不是貸方科目。"
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr "這不是流動科目。"
 
@@ -413,23 +413,23 @@
 msgstr "去年"
 
 #: src/accounting/report/period/shortcuts.py:146
 #: src/accounting/templates/accounting/report/include/period-chooser.html:122
 msgid "All"
 msgstr "全部"
 
-#: src/accounting/report/reports/balance_sheet.py:423
-#: src/accounting/report/reports/balance_sheet.py:427
-#: src/accounting/report/reports/balance_sheet.py:439
+#: src/accounting/report/reports/balance_sheet.py:425
+#: src/accounting/report/reports/balance_sheet.py:429
 #: src/accounting/report/reports/balance_sheet.py:441
-#: src/accounting/report/reports/income_expenses.py:189
-#: src/accounting/report/reports/income_expenses.py:423
-#: src/accounting/report/reports/income_statement.py:300
-#: src/accounting/report/reports/ledger.py:171
-#: src/accounting/report/reports/ledger.py:380
+#: src/accounting/report/reports/balance_sheet.py:443
+#: src/accounting/report/reports/income_expenses.py:187
+#: src/accounting/report/reports/income_expenses.py:420
+#: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/ledger.py:168
+#: src/accounting/report/reports/ledger.py:376
 #: src/accounting/report/reports/trial_balance.py:229
 #: src/accounting/templates/accounting/journal-entry/disbursement/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html:38
 #: src/accounting/templates/accounting/journal-entry/receipt/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:39
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:55
 #: src/accounting/templates/accounting/report/balance-sheet.html:65
@@ -441,120 +441,120 @@
 #: src/accounting/templates/accounting/report/income-expenses.html:81
 #: src/accounting/templates/accounting/report/income-statement.html:89
 #: src/accounting/templates/accounting/report/ledger.html:82
 #: src/accounting/templates/accounting/report/trial-balance.html:80
 msgid "Total"
 msgstr "合計"
 
-#: src/accounting/report/reports/income_expenses.py:136
-#: src/accounting/report/reports/ledger.py:132
+#: src/accounting/report/reports/income_expenses.py:134
+#: src/accounting/report/reports/ledger.py:129
 msgid "Brought forward"
 msgstr "前期轉入"
 
-#: src/accounting/report/reports/income_expenses.py:407
+#: src/accounting/report/reports/income_expenses.py:404
 #: src/accounting/report/reports/journal.py:158
-#: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/ledger.py:362
 #: src/accounting/report/reports/unapplied.py:148
 #: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
 #: src/accounting/templates/accounting/report/unapplied.html:52
 #: src/accounting/templates/accounting/report/unmatched.html:93
 msgid "Date"
 msgstr "日期"
 
-#: src/accounting/report/reports/income_expenses.py:407
+#: src/accounting/report/reports/income_expenses.py:404
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/report/reports/unapplied_accounts.py:122
 #: src/accounting/report/reports/unmatched_accounts.py:122
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:58
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:40
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
 #: src/accounting/templates/accounting/report/trial-balance.html:61
 msgid "Account"
 msgstr "科目"
 
-#: src/accounting/report/reports/income_expenses.py:408
+#: src/accounting/report/reports/income_expenses.py:405
 #: src/accounting/report/reports/journal.py:159
-#: src/accounting/report/reports/ledger.py:366
+#: src/accounting/report/reports/ledger.py:362
 #: src/accounting/report/reports/unapplied.py:149
 #: src/accounting/report/reports/unmatched.py:159
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:29
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:50
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
 #: src/accounting/templates/accounting/report/unapplied.html:53
 #: src/accounting/templates/accounting/report/unmatched.html:94
 msgid "Description"
 msgstr "摘要"
 
-#: src/accounting/report/reports/income_expenses.py:408
+#: src/accounting/report/reports/income_expenses.py:405
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr "收入"
 
-#: src/accounting/report/reports/income_expenses.py:409
+#: src/accounting/report/reports/income_expenses.py:406
 #: src/accounting/templates/accounting/report/income-expenses.html:59
 msgid "Expense"
 msgstr "支出"
 
-#: src/accounting/report/reports/income_expenses.py:409
-#: src/accounting/report/reports/ledger.py:368
+#: src/accounting/report/reports/income_expenses.py:406
+#: src/accounting/report/reports/ledger.py:364
 #: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
 #: src/accounting/templates/accounting/report/unmatched.html:97
 msgid "Balance"
 msgstr "餘額"
 
-#: src/accounting/report/reports/income_expenses.py:410
+#: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:161
-#: src/accounting/report/reports/ledger.py:368
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
+#: src/accounting/report/reports/ledger.py:364
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:179
 #: src/accounting/templates/accounting/journal-entry/include/form.html:73
 msgid "Note"
 msgstr "備註"
 
-#: src/accounting/report/reports/income_statement.py:228
-msgid "total operating revenue"
+#: src/accounting/report/reports/income_statement.py:229
+msgid "Total Operating Revenue"
 msgstr "營業收入總額"
 
-#: src/accounting/report/reports/income_statement.py:229
-msgid "gross income"
+#: src/accounting/report/reports/income_statement.py:230
+msgid "Gross Income"
 msgstr "營業毛利"
 
-#: src/accounting/report/reports/income_statement.py:230
-msgid "operating income"
+#: src/accounting/report/reports/income_statement.py:231
+msgid "Operating Income"
 msgstr "營業淨利"
 
-#: src/accounting/report/reports/income_statement.py:231
-msgid "before tax income"
+#: src/accounting/report/reports/income_statement.py:232
+msgid "Before Tax Income"
 msgstr "稅前淨利"
 
-#: src/accounting/report/reports/income_statement.py:232
-msgid "after tax income"
+#: src/accounting/report/reports/income_statement.py:233
+msgid "After Tax Income"
 msgstr "稅後淨利"
 
-#: src/accounting/report/reports/income_statement.py:233
-msgid "net income or loss for current period"
+#: src/accounting/report/reports/income_statement.py:234
+msgid "Net Income or Loss for Current Period"
 msgstr "本期損益"
 
-#: src/accounting/report/reports/income_statement.py:301
+#: src/accounting/report/reports/income_statement.py:302
 #: src/accounting/report/reports/unapplied.py:149
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:66
 #: src/accounting/templates/accounting/report/income-statement.html:61
 #: src/accounting/templates/accounting/report/unapplied.html:54
 msgid "Amount"
 msgstr "金額"
 
 #: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/unapplied.py:148
@@ -563,29 +563,29 @@
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
 msgid "Currency"
 msgstr "貨幣"
 
 #: src/accounting/report/reports/journal.py:160
-#: src/accounting/report/reports/ledger.py:367
+#: src/accounting/report/reports/ledger.py:363
 #: src/accounting/report/reports/trial_balance.py:225
 #: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
 #: src/accounting/templates/accounting/report/trial-balance.html:62
 #: src/accounting/templates/accounting/report/unmatched.html:95
 msgid "Debit"
 msgstr "借方"
 
 #: src/accounting/report/reports/journal.py:160
-#: src/accounting/report/reports/ledger.py:367
+#: src/accounting/report/reports/ledger.py:363
 #: src/accounting/report/reports/trial_balance.py:226
 #: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
@@ -610,24 +610,24 @@
 #: src/accounting/report/reports/unapplied_accounts.py:122
 #: src/accounting/report/reports/unmatched_accounts.py:122
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:59
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:59
 msgid "Count"
 msgstr "數量"
 
-#: src/accounting/report/utils/offset_matcher.py:163
+#: src/accounting/report/utils/offset_matcher.py:161
 msgid "There is no unmatched offset."
 msgstr "沒有遺漏的抵銷分錄"
 
-#: src/accounting/report/utils/offset_matcher.py:167
+#: src/accounting/report/utils/offset_matcher.py:165
 #, python-format
 msgid "%(total)s unmatched offsets without original items."
 msgstr "%(total)s 筆遺漏的抵銷分錄無法自動抵銷。"
 
-#: src/accounting/report/utils/offset_matcher.py:172
+#: src/accounting/report/utils/offset_matcher.py:170
 #, python-format
 msgid ""
 "%(matches)s unmatched offsets out of %(total)s can match with their "
 "original items."
 msgstr "%(total)s 筆遺漏的抵銷分錄中，可配對抵銷掉 %(matches)s 筆。"
 
 #: src/accounting/report/utils/report_chooser.py:86
@@ -748,15 +748,15 @@
 msgstr "十一月"
 
 #: src/accounting/static/js/description-editor.js:1195
 msgid "December"
 msgstr "十二月"
 
 #: src/accounting/static/js/journal-entry-form.js:1085
-#: src/accounting/static/js/journal-entry-line-item-editor.js:430
+#: src/accounting/static/js/journal-entry-line-item-editor.js:434
 msgid "Please fill in the amount."
 msgstr "請填上金額。"
 
 #: src/accounting/static/js/journal-entry-form.js:1107
 #: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:37
 #: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:41
 #, python-format
@@ -829,39 +829,39 @@
 msgid "Confirm Delete Account"
 msgstr "確認刪除科目"
 
 #: src/accounting/templates/accounting/account/detail.html:77
 #: src/accounting/templates/accounting/account/include/form.html:91
 #: src/accounting/templates/accounting/currency/detail.html:73
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:27
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:30
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:31
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:29
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:29
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
 #: src/accounting/templates/accounting/report/unmatched.html:58
 msgid "Close"
 msgstr "關閉"
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr "你確定要刪掉這個科目嗎？"
 
 #: src/accounting/templates/accounting/account/detail.html:83
 #: src/accounting/templates/accounting/account/include/form.html:112
 #: src/accounting/templates/accounting/currency/detail.html:79
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:195
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:71
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:66
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
 #: src/accounting/templates/accounting/report/unmatched.html:74
 msgid "Cancel"
 msgstr "取消"
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
@@ -938,20 +938,20 @@
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr "%(base)s下的科目"
 
 #: src/accounting/templates/accounting/account/include/form.html:75
 #: src/accounting/templates/accounting/account/order.html:62
 #: src/accounting/templates/accounting/currency/include/form.html:57
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:195
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:196
 #: src/accounting/templates/accounting/journal-entry/include/form.html:80
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:71
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:72
 #: src/accounting/templates/accounting/journal-entry/order.html:61
 #: src/accounting/templates/accounting/option/form.html:80
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:66
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:67
 msgid "Save"
 msgstr "儲存"
 
 #: src/accounting/templates/accounting/account/include/form.html:45
 msgid "Base account"
 msgstr "基本科目"
 
@@ -1004,15 +1004,15 @@
 msgstr "貨幣管理"
 
 #: src/accounting/templates/accounting/currency/include/form.html:44
 msgid "Code"
 msgstr "代碼"
 
 #: src/accounting/templates/accounting/currency/include/form.html:50
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:33
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:34
 msgid "Name"
 msgstr "名稱"
 
 #: src/accounting/templates/accounting/include/nav.html:27
 msgid "Accounting"
 msgstr "記帳"
 
@@ -1073,61 +1073,61 @@
 msgid "Select Account"
 msgstr "選擇科目"
 
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:44
 msgid "More…"
 msgstr "更多…"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:36
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:37
 msgid "Offset..."
 msgstr "抵銷…"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:44
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:45
 msgid "General"
 msgstr "一般"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:49
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:50
 msgid "Travel"
 msgstr "差旅"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:54
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:55
 msgid "Bus"
 msgstr "公車"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:59
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:60
 msgid "Recurring"
 msgstr "常用"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:64
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:65
 msgid "Annotation"
 msgstr "註記"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:73
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:90
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:125
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:74
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:91
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:126
 msgid "Tag"
 msgstr "標籤"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:105
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:146
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:106
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:147
 #: src/accounting/templates/accounting/report/include/period-chooser.html:129
 msgid "From"
 msgstr "從"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:114
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:151
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:115
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:152
 #: src/accounting/templates/accounting/report/include/period-chooser.html:135
 msgid "To"
 msgstr "至"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:130
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:131
 msgid "Route"
 msgstr "路線"
 
-#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:172
+#: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:173
 msgid "The Number of Items"
 msgstr "數量"
 
 #: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:45
 #: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:46
 msgid "Offsets"
 msgstr "抵銷"
@@ -1151,19 +1151,19 @@
 msgid "Confirm Delete Journal Entry"
 msgstr "確認刪除傳票"
 
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:81
 msgid "Do you really want to delete this journal entry?"
 msgstr "你確定要刪掉這張傳票嗎？"
 
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:27
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 msgid "Line Item Content"
 msgstr "分錄內容"
 
-#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:34
+#: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:35
 msgid "Original Line Item"
 msgstr "原始分錄"
 
 #: src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html:25
 #: src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html:26
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:31
 msgid "Cash Disbursement"
@@ -1211,51 +1211,51 @@
 
 #: src/accounting/templates/accounting/option/detail.html:70
 #: src/accounting/templates/accounting/option/form.html:72
 #: src/accounting/templates/accounting/option/form.html:96
 msgid "Recurring Income"
 msgstr "常用收入"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:47
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:48
 msgid "Description Template"
 msgstr "摘要範本"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:52
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:53
 msgid "Available template variables:"
 msgstr "範本變數說明："
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:54
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:55
 msgid "This month, as a number."
 msgstr "這個月的數字。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:55
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:56
 msgid "This month, in its name."
 msgstr "這個月的名稱。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:56
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:57
 msgid "Last month, as a number."
 msgstr "上個月的數字。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:57
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:58
 msgid "Last month, in its name."
 msgstr "上個月的名稱。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:58
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:59
 msgid "The previous bimonthly period, as numbers."
 msgstr "前個雙月期的數字。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:59
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:60
 msgid "The previous bimonthly period, as their names."
 msgstr "前個雙月期的名稱。"
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:62
 msgid "Example:"
 msgstr "範例："
 
-#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
+#: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:62
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水費{last_bimonthly_number}月"
 
 #: src/accounting/templates/accounting/report/balance-sheet.html:29
 #: src/accounting/templates/accounting/report/balance-sheet.html:51
 #, python-format
 msgid "Balance Sheet %(period)s"
@@ -1314,42 +1314,42 @@
 #: src/accounting/templates/accounting/report/trial-balance.html:53
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s試算表"
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:29
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:49
-msgid "Accounts with Unapplied Items"
+msgid "Accounts With Unapplied Items"
 msgstr "含未抵銷項目的科目"
 
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:29
 #: src/accounting/templates/accounting/report/unapplied-accounts.html:51
 #, python-format
-msgid "Accounts with Unapplied Items in %(currency)s"
+msgid "Accounts With Unapplied Items in %(currency)s"
 msgstr "%(currency)s含未抵銷項目的科目"
 
 #: src/accounting/templates/accounting/report/unapplied.html:29
 #, python-format
 msgid "Unapplied Items of %(account)s"
 msgstr "%(account)s未抵銷項目"
 
 #: src/accounting/templates/accounting/report/unapplied.html:29
 #, python-format
 msgid "Unapplied Items of %(account)s in %(currency)s"
 msgstr "%(currency)s%(account)s未抵銷項目"
 
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:29
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:49
-msgid "Accounts with Unmatched Offsets"
+msgid "Accounts With Unmatched Offsets"
 msgstr "含遺漏抵銷項目的科目"
 
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:29
 #: src/accounting/templates/accounting/report/unmatched-accounts.html:51
 #, python-format
-msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgid "Accounts With Unmatched Offsets in %(currency)s"
 msgstr "%(currency)s含遺漏抵銷項目的科目"
 
 #: src/accounting/templates/accounting/report/unmatched.html:29
 #, python-format
 msgid "Unmatched Offsets of %(account)s"
 msgstr "%(account)s遺漏的抵銷項目"
 
@@ -1411,17 +1411,17 @@
 msgid "Download"
 msgstr "下載"
 
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流動資產與負債"
 
-#: src/accounting/utils/pagination.py:206
+#: src/accounting/utils/pagination.py:207
 msgctxt "Pagination|"
 msgid "Previous"
 msgstr "上一頁"
 
-#: src/accounting/utils/pagination.py:255
+#: src/accounting/utils/pagination.py:256
 msgctxt "Pagination|"
 msgid "Next"
 msgstr "下一頁"
```

### Comparing `mia-accounting-1.5.6/src/accounting/utils/__init__.py` & `mia-accounting-1.5.7/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/cast.py` & `mia-accounting-1.5.7/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/current_account.py` & `mia-accounting-1.5.7/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/flash_errors.py` & `mia-accounting-1.5.7/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.5.7/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/next_uri.py` & `mia-accounting-1.5.7/src/accounting/utils/next_uri.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,15 @@
     :return: The valid next URI.
     """
     next_uri: str | None = request.form.get("next") \
         if request.method == "POST" else request.args.get("next")
     if next_uri is None:
         return None
     try:
-        return URLSafeSerializer(current_app.config["SECRET_KEY"])\
-            .loads(next_uri, "next")
+        return decode_next(next_uri)
     except BadData:
         return None
 
 
 def __set_next(uri: str, next_uri: str) -> str:
     """Sets the next URI to the query arguments.
 
@@ -103,14 +102,24 @@
     :param uri: The next URI.
     :return: The encoded next URI.
     """
     return URLSafeSerializer(current_app.config["SECRET_KEY"])\
         .dumps(uri, "next")
 
 
+def decode_next(uri: str) -> str:
+    """Decodes the encoded next URI.
+
+    :param uri: The encoded next URI.
+    :return: The next URI.
+    """
+    return URLSafeSerializer(current_app.config["SECRET_KEY"])\
+        .loads(uri, "next")
+
+
 def init_app(bp: Blueprint) -> None:
     """Initializes the application.
 
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
     bp.add_app_template_global(__as_next, "accounting_as_next")
```

### Comparing `mia-accounting-1.5.6/src/accounting/utils/offset_alias.py` & `mia-accounting-1.5.7/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/options.py` & `mia-accounting-1.5.7/src/accounting/utils/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,19 @@
         """Constructs the recurring item.
 
         :param name: The name.
         :param account_code: The account code.
         :param description_template: The description template.
         """
         self.name: str = name
+        """The name."""
         self.account_code: str = account_code
+        """The account code."""
         self.description_template: str = description_template
+        """The description template."""
 
     @property
     def account_text(self) -> str:
         """Returns the account text.
 
         :return: The account text.
         """
@@ -57,16 +60,18 @@
     def __init__(self, data: dict[str, list[tuple[str, str, str]]]):
         """Constructs the recurring item.
 
         :param data: The data.
         """
         self.expenses: list[RecurringItem] \
             = [RecurringItem(x[0], x[1], x[2]) for x in data["expense"]]
+        """The recurring expenses."""
         self.incomes: list[RecurringItem] \
             = [RecurringItem(x[0], x[1], x[2]) for x in data["income"]]
+        """The recurring incomes."""
 
     @property
     def codes(self) -> set[str]:
         """Returns all the account codes.
 
         :return: All the account codes.
         """
```

### Comparing `mia-accounting-1.5.6/src/accounting/utils/pagination.py` & `mia-accounting-1.5.7/src/accounting/utils/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     """The HTTP code."""
 
 
 DEFAULT_PAGE_SIZE: int = 10
 """The default page size."""
 
 T = TypeVar("T")
+"""The pagination item type."""
 
 
 class Pagination(Generic[T]):
     """The pagination utility."""
 
     def __init__(self, items: list[T], is_reversed: bool = False):
         """Constructs the pagination.
```

### Comparing `mia-accounting-1.5.6/src/accounting/utils/permission.py` & `mia-accounting-1.5.7/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/query.py` & `mia-accounting-1.5.7/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/random_id.py` & `mia-accounting-1.5.7/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/strip_text.py` & `mia-accounting-1.5.7/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/src/accounting/utils/user.py` & `mia-accounting-1.5.7/src/accounting/utils/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from typing import TypeVar, Generic, Type
 
 import sqlalchemy as sa
 from flask import g, Response
 from flask_sqlalchemy.model import Model
 
 T = TypeVar("T", bound=Model)
+"""The user data model data type."""
 
 
 class UserUtilityInterface(Generic[T], ABC):
     """The interface for the user utilities."""
 
     @abstractmethod
     def can_view(self) -> bool:
```

### Comparing `mia-accounting-1.5.6/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.5.7/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.6
+Version: 1.5.7
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.6/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.5.7/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 src/accounting/utils/offset_alias.py
 src/accounting/utils/options.py
 src/accounting/utils/pagination.py
 src/accounting/utils/permission.py
 src/accounting/utils/query.py
 src/accounting/utils/random_id.py
 src/accounting/utils/strip_text.py
+src/accounting/utils/title_case.py
 src/accounting/utils/user.py
 src/mia_accounting.egg-info/PKG-INFO
 src/mia_accounting.egg-info/SOURCES.txt
 src/mia_accounting.egg-info/dependency_links.txt
 src/mia_accounting.egg-info/requires.txt
 src/mia_accounting.egg-info/top_level.txt
 tests/babel-utils-test-site.py
```

### Comparing `mia-accounting-1.5.6/tests/babel-utils-test-site.py` & `mia-accounting-1.5.7/tests/babel-utils-test-site.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 from time import strftime
 
 import click
 from babel.messages.frontend import CommandLineInterface
 from opencc import OpenCC
 
 root_dir: Path = Path(__file__).parent.parent
+"""The project root directory."""
 translation_dir: Path = root_dir / "tests" / "test_site" / "translations"
+"""The directory of the translation files."""
 domain: str = "messages"
+"""The message domain."""
 
 
 @click.group()
 def main() -> None:
     """Manages the message translation."""
```

### Comparing `mia-accounting-1.5.6/tests/babel-utils.py` & `mia-accounting-1.5.7/tests/babel-utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 from time import strftime
 
 import click
 from babel.messages.frontend import CommandLineInterface
 from opencc import OpenCC
 
 root_dir: Path = Path(__file__).parent.parent
+"""The project root directory."""
 translation_dir: Path = root_dir / "src" / "accounting" / "translations"
+"""The directory of the translation files."""
 domain: str = "accounting"
+"""The message domain."""
 
 
 @click.group()
 def main() -> None:
     """Manages the message translation."""
```

### Comparing `mia-accounting-1.5.6/tests/test_account.py` & `mia-accounting-1.5.7/tests/test_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 import unittest
 
 import httpx
 from flask import Flask
 
 from accounting.utils.next_uri import encode_next
 from test_site import db
-from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
-    add_journal_entry
+from testlib import NEXT_URI, create_test_app, get_client, get_csrf_token, \
+    set_locale, add_journal_entry
 
 
 class AccountData:
     """The account data."""
 
     def __init__(self, base_code: str, no: int, title: str):
         """Constructs the account data.
@@ -68,49 +68,55 @@
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import Account, AccountL10n
             AccountL10n.query.delete()
             Account.query.delete()
             db.session.commit()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
         response: httpx.Response
 
-        response = self.client.post(f"{PREFIX}/store",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": CASH.base_code,
-                                          "title": CASH.title})
+        response = self.__client.post(f"{PREFIX}/store",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": CASH.base_code,
+                                            "title": CASH.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{CASH.code}")
 
-        response = self.client.post(f"{PREFIX}/store",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": BANK.base_code,
-                                          "title": BANK.title})
+        response = self.__client.post(f"{PREFIX}/store",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": BANK.base_code,
+                                            "title": BANK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{BANK.code}")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
         from accounting.models import Account
-        client, csrf_token = get_client(self.app, "nobody")
+        client: httpx.Client = get_client(self.__app, "nobody")
+        csrf_token: str = get_csrf_token(client)
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/{CASH.code}")
         self.assertEqual(response.status_code, 403)
@@ -136,30 +142,31 @@
         response = client.post(f"{PREFIX}/{BANK.code}/delete",
                                data={"csrf_token": csrf_token})
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/bases/{CASH.base_code}")
         self.assertEqual(response.status_code, 403)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             cash_id: int = Account.find_by_code(CASH.code).id
 
         response = client.post(f"{PREFIX}/bases/{CASH.base_code}",
                                data={"csrf_token": csrf_token,
-                                     "next": self.encoded_next_uri,
+                                     "next": self.__encoded_next_uri,
                                      f"{cash_id}-no": "5"})
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
         from accounting.models import Account
-        client, csrf_token = get_client(self.app, "viewer")
+        client: httpx.Client = get_client(self.__app, "viewer")
+        csrf_token: str = get_csrf_token(client)
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
         response = client.get(f"{PREFIX}/{CASH.code}")
         self.assertEqual(response.status_code, 200)
@@ -185,177 +192,178 @@
         response = client.post(f"{PREFIX}/{BANK.code}/delete",
                                data={"csrf_token": csrf_token})
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/bases/{CASH.base_code}")
         self.assertEqual(response.status_code, 200)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             cash_id: int = Account.find_by_code(CASH.code).id
 
         response = client.post(f"{PREFIX}/bases/{CASH.base_code}",
                                data={"csrf_token": csrf_token,
-                                     "next": self.encoded_next_uri,
+                                     "next": self.__encoded_next_uri,
                                      f"{cash_id}-no": "5"})
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
         from accounting.models import Account
         response: httpx.Response
 
-        response = self.client.get(PREFIX)
+        response = self.__client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/{CASH.code}")
+        response = self.__client.get(f"{PREFIX}/{CASH.code}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/create")
+        response = self.__client.get(f"{PREFIX}/create")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/store",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": STOCK.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(f"{PREFIX}/store",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": STOCK.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{STOCK.code}")
 
-        response = self.client.get(f"{PREFIX}/{CASH.code}/edit")
+        response = self.__client.get(f"{PREFIX}/{CASH.code}/edit")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/{CASH.code}/update",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": CASH.base_code,
-                                          "title": f"{CASH.title}-2"})
+        response = self.__client.post(f"{PREFIX}/{CASH.code}/update",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": CASH.base_code,
+                                            "title": f"{CASH.title}-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], f"{PREFIX}/{CASH.code}")
 
-        response = self.client.post(f"{PREFIX}/{BANK.code}/delete",
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(f"{PREFIX}/{BANK.code}/delete",
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], PREFIX)
 
-        response = self.client.get(f"{PREFIX}/bases/{CASH.base_code}")
+        response = self.__client.get(f"{PREFIX}/bases/{CASH.base_code}")
         self.assertEqual(response.status_code, 200)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             cash_id: int = Account.find_by_code(CASH.code).id
 
-        response = self.client.post(f"{PREFIX}/bases/{CASH.base_code}",
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri,
-                                          f"{cash_id}-no": "5"})
+        response = self.__client.post(f"{PREFIX}/bases/{CASH.base_code}",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri,
+                                            f"{cash_id}-no": "5"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_add(self) -> None:
         """Tests to add the currencies.
 
         :return: None.
         """
         from accounting.models import Account
         create_uri: str = f"{PREFIX}/create"
         store_uri: str = f"{PREFIX}/store"
         detail_uri: str = f"{PREFIX}/{STOCK.code}"
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual({x.code for x in Account.query.all()},
                              {CASH.code, BANK.code})
 
         # Missing CSRF token
-        response = self.client.post(store_uri,
-                                    data={"base_code": STOCK.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"base_code": STOCK.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 400)
 
         # CSRF token mismatch
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": f"{self.csrf_token}-2",
-                                          "base_code": STOCK.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token":
+                                            f"{self.__csrf_token}-2",
+                                            "base_code": STOCK.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 400)
 
         # Empty base account code
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": " ",
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": " ",
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing base account
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "9999",
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "9999",
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Unavailable base account
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "1",
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "1",
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Empty name
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": STOCK.base_code,
-                                          "title": " "})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": STOCK.base_code,
+                                            "title": " "})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # A nominal account that needs offset
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "6172",
-                                          "title": STOCK.title,
-                                          "is_need_offset": "yes"})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "6172",
+                                            "title": STOCK.title,
+                                            "is_need_offset": "yes"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Success, with spaces to be stripped
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": f" {STOCK.base_code} ",
-                                          "title": f" {STOCK.title} "})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": f" {STOCK.base_code} ",
+                                            "title": f" {STOCK.title} "})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         # Success under the same base
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": STOCK.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": STOCK.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{STOCK.base_code}-002")
 
         # Success under the same base, with order in a mess.
-        with self.app.app_context():
+        with self.__app.app_context():
             stock_2: Account = Account.find_by_code(f"{STOCK.base_code}-002")
             stock_2.no = 66
             db.session.commit()
 
-        response = self.client.post(store_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": STOCK.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(store_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": STOCK.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{STOCK.base_code}-003")
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual({x.code for x in Account.query.all()},
                              {CASH.code, BANK.code, STOCK.code,
                               f"{STOCK.base_code}-002",
                               f"{STOCK.base_code}-003"})
 
             account: Account = Account.find_by_code(STOCK.code)
             self.assertEqual(account.base_code, STOCK.base_code)
@@ -370,146 +378,147 @@
         detail_uri: str = f"{PREFIX}/{CASH.code}"
         edit_uri: str = f"{PREFIX}/{CASH.code}/edit"
         update_uri: str = f"{PREFIX}/{CASH.code}/update"
         detail_c_uri: str = f"{PREFIX}/{STOCK.code}"
         response: httpx.Response
 
         # Success, with spaces to be stripped
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": f" {CASH.base_code} ",
-                                          "title": f" {CASH.title}-1 "})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": f" {CASH.base_code} ",
+                                            "title": f" {CASH.title}-1 "})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account: Account = Account.find_by_code(CASH.code)
             self.assertEqual(account.base_code, CASH.base_code)
             self.assertEqual(account.title_l10n, f"{CASH.title}-1")
 
         # Empty base account code
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": " ",
-                                          "title": STOCK.title})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": " ",
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing base account
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "9999",
-                                          "title": STOCK.title})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "9999",
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Unavailable base account
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "1",
-                                          "title": STOCK.title})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "1",
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Empty name
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": STOCK.base_code,
-                                          "title": " "})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": STOCK.base_code,
+                                            "title": " "})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # A nominal account that needs offset
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "6172",
-                                          "title": STOCK.title,
-                                          "is_need_offset": "yes"})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "6172",
+                                            "title": STOCK.title,
+                                            "is_need_offset": "yes"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Change the base account
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": STOCK.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": STOCK.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_c_uri)
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
 
-        response = self.client.get(detail_c_uri)
+        response = self.__client.get(detail_c_uri)
         self.assertEqual(response.status_code, 200)
 
     def test_update_not_modified(self) -> None:
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import Account
         detail_uri: str = f"{PREFIX}/{CASH.code}"
         update_uri: str = f"{PREFIX}/{CASH.code}/update"
         account: Account
         response: httpx.Response
 
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": f" {CASH.base_code} ",
-                                          "title": f" {CASH.title} "})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": f" {CASH.base_code} ",
+                                            "title": f" {CASH.title} "})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertIsNotNone(account)
             account.created_at \
                 = account.created_at - dt.timedelta(seconds=5)
             account.updated_at = account.created_at
             db.session.commit()
 
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": CASH.base_code,
-                                          "title": STOCK.title})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": CASH.base_code,
+                                            "title": STOCK.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertIsNotNone(account)
             self.assertLess(account.created_at,
                             account.updated_at)
 
     def test_created_updated_by(self) -> None:
         """Tests the created-by and updated-by record.
 
         :return: None.
         """
         from accounting.models import Account
         editor_username, admin_username = "editor", "admin"
-        client, csrf_token = get_client(self.app, admin_username)
+        client: httpx.Client = get_client(self.__app, admin_username)
+        csrf_token: str = get_csrf_token(client)
         detail_uri: str = f"{PREFIX}/{CASH.code}"
         update_uri: str = f"{PREFIX}/{CASH.code}/update"
         account: Account
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.created_by.username, editor_username)
             self.assertEqual(account.updated_by.username, editor_username)
 
         response = client.post(update_uri,
                                data={"csrf_token": csrf_token,
                                      "base_code": CASH.base_code,
                                      "title": f"{CASH.title}-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.created_by.username,
                              editor_username)
             self.assertEqual(account.updated_by.username,
                              admin_username)
 
     def test_l10n(self) -> None:
@@ -519,59 +528,59 @@
         """
         from accounting.models import Account
         detail_uri: str = f"{PREFIX}/{CASH.code}"
         update_uri: str = f"{PREFIX}/{CASH.code}/update"
         account: Account
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, CASH.title)
             self.assertEqual(account.l10n, [])
 
-        set_locale(self.app, self.client, self.csrf_token, "zh_Hant")
+        set_locale(self.__app, self.__client, self.__csrf_token, "zh_Hant")
 
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": CASH.base_code,
-                                          "title": f"{CASH.title}-zh_Hant"})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": CASH.base_code,
+                                            "title": f"{CASH.title}-zh_Hant"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, CASH.title)
             self.assertEqual({(x.locale, x.title) for x in account.l10n},
                              {("zh_Hant", f"{CASH.title}-zh_Hant")})
 
-        set_locale(self.app, self.client, self.csrf_token, "en")
+        set_locale(self.__app, self.__client, self.__csrf_token, "en")
 
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": CASH.base_code,
-                                          "title": f"{CASH.title}-2"})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": CASH.base_code,
+                                            "title": f"{CASH.title}-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, f"{CASH.title}-2")
             self.assertEqual({(x.locale, x.title) for x in account.l10n},
                              {("zh_Hant", f"{CASH.title}-zh_Hant")})
 
-        set_locale(self.app, self.client, self.csrf_token, "zh_Hant")
+        set_locale(self.__app, self.__client, self.__csrf_token, "zh_Hant")
 
-        response = self.client.post(update_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": CASH.base_code,
-                                          "title": f"{CASH.title}-zh_Hant-2"})
+        response = self.__client.post(update_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": CASH.base_code,
+                                            "title": f"{CASH.title}-zh_Hant-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, f"{CASH.title}-2")
             self.assertEqual({(x.locale, x.title) for x in account.l10n},
                              {("zh_Hant", f"{CASH.title}-zh_Hant-2")})
 
     def test_delete(self) -> None:
         """Tests to delete a currency.
@@ -580,81 +589,81 @@
         """
         from accounting.models import Account
         detail_uri: str = f"{PREFIX}/{PETTY.code}"
         delete_uri: str = f"{PREFIX}/{PETTY.code}/delete"
         list_uri: str = PREFIX
         response: httpx.Response
 
-        response = self.client.post(f"{PREFIX}/store",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": PETTY.base_code,
-                                          "title": PETTY.title})
+        response = self.__client.post(f"{PREFIX}/store",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": PETTY.base_code,
+                                            "title": PETTY.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        add_journal_entry(self.client,
-                          form={"csrf_token": self.csrf_token,
-                                "next": self.encoded_next_uri,
+        add_journal_entry(self.__client,
+                          form={"csrf_token": self.__csrf_token,
+                                "next": self.__encoded_next_uri,
                                 "date": dt.date.today().isoformat(),
                                 "currency-1-code": "USD",
                                 "currency-1-credit-1-account_code": BANK.code,
                                 "currency-1-credit-1-amount": "20"})
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual({x.code for x in Account.query.all()},
                              {CASH.code, PETTY.code, BANK.code})
 
         # Cannot delete the cash account
-        response = self.client.post(f"{PREFIX}/{CASH.code}/delete",
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(f"{PREFIX}/{CASH.code}/delete",
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], f"{PREFIX}/{CASH.code}")
 
         # Cannot delete the account that is in use
-        response = self.client.post(f"{PREFIX}/{BANK.code}/delete",
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(f"{PREFIX}/{BANK.code}/delete",
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], f"{PREFIX}/{BANK.code}")
 
         # Success
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], list_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual({x.code for x in Account.query.all()},
                              {CASH.code, BANK.code})
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 404)
 
     def test_change_base_code(self) -> None:
         """Tests to change the base code of an account.
 
         :return: None.
         """
         from accounting.models import Account
         response: httpx.Response
 
         for i in range(2, 6):
-            response = self.client.post(f"{PREFIX}/store",
-                                        data={"csrf_token": self.csrf_token,
-                                              "base_code": "1111",
-                                              "title": "Title"})
+            response = self.__client.post(f"{PREFIX}/store",
+                                          data={"csrf_token": self.__csrf_token,
+                                                "base_code": "1111",
+                                                "title": "Title"})
             self.assertEqual(response.status_code, 302)
             self.assertEqual(response.headers["Location"],
                              f"{PREFIX}/1111-00{i}")
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account_1: Account = Account.find_by_code("1111-001")
             id_1: int = account_1.id
             account_2: Account = Account.find_by_code("1111-002")
             id_2: int = account_2.id
             account_3: Account = Account.find_by_code("1111-003")
             id_3: int = account_3.id
             account_4: Account = Account.find_by_code("1111-004")
@@ -666,22 +675,22 @@
             account_3.no = 8
             account_4.base_code = "1112"
             account_4.no = 2
             account_5.base_code = "1112"
             account_5.no = 6
             db.session.commit()
 
-        response = self.client.post(f"{PREFIX}/1111-005/update",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "1112",
-                                          "title": "Title"})
+        response = self.__client.post(f"{PREFIX}/1111-005/update",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "base_code": "1112",
+                                            "title": "Title"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], f"{PREFIX}/1112-003")
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(db.session.get(Account, id_1).no, 1)
             self.assertEqual(db.session.get(Account, id_2).no, 3)
             self.assertEqual(db.session.get(Account, id_3).no, 2)
             self.assertEqual(db.session.get(Account, id_4).no, 1)
             self.assertEqual(db.session.get(Account, id_5).no, 2)
 
     def test_reorder(self) -> None:
@@ -689,65 +698,65 @@
 
         :return: None.
         """
         from accounting.models import Account
         response: httpx.Response
 
         for i in range(2, 6):
-            response = self.client.post(f"{PREFIX}/store",
-                                        data={"csrf_token": self.csrf_token,
-                                              "base_code": "1111",
-                                              "title": "Title"})
+            response = self.__client.post(f"{PREFIX}/store",
+                                          data={"csrf_token": self.__csrf_token,
+                                                "base_code": "1111",
+                                                "title": "Title"})
             self.assertEqual(response.status_code, 302)
             self.assertEqual(response.headers["Location"],
                              f"{PREFIX}/1111-00{i}")
 
         # Normal reorder
-        with self.app.app_context():
+        with self.__app.app_context():
             id_1: int = Account.find_by_code("1111-001").id
             id_2: int = Account.find_by_code("1111-002").id
             id_3: int = Account.find_by_code("1111-003").id
             id_4: int = Account.find_by_code("1111-004").id
             id_5: int = Account.find_by_code("1111-005").id
 
-        response = self.client.post(f"{PREFIX}/bases/1111",
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri,
-                                          f"{id_1}-no": "4",
-                                          f"{id_2}-no": "1",
-                                          f"{id_3}-no": "5",
-                                          f"{id_4}-no": "2",
-                                          f"{id_5}-no": "3"})
+        response = self.__client.post(f"{PREFIX}/bases/1111",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri,
+                                            f"{id_1}-no": "4",
+                                            f"{id_2}-no": "1",
+                                            f"{id_3}-no": "5",
+                                            f"{id_4}-no": "2",
+                                            f"{id_5}-no": "3"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(db.session.get(Account, id_1).code, "1111-004")
             self.assertEqual(db.session.get(Account, id_2).code, "1111-001")
             self.assertEqual(db.session.get(Account, id_3).code, "1111-005")
             self.assertEqual(db.session.get(Account, id_4).code, "1111-002")
             self.assertEqual(db.session.get(Account, id_5).code, "1111-003")
 
         # Malformed orders
-        with self.app.app_context():
+        with self.__app.app_context():
             db.session.get(Account, id_1).no = 3
             db.session.get(Account, id_2).no = 4
             db.session.get(Account, id_3).no = 6
             db.session.get(Account, id_4).no = 8
             db.session.get(Account, id_5).no = 9
             db.session.commit()
 
-        response = self.client.post(f"{PREFIX}/bases/1111",
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri,
-                                          f"{id_2}-no": "3a",
-                                          f"{id_3}-no": "5",
-                                          f"{id_4}-no": "2"})
+        response = self.__client.post(f"{PREFIX}/bases/1111",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri,
+                                            f"{id_2}-no": "3a",
+                                            f"{id_3}-no": "5",
+                                            f"{id_4}-no": "2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(db.session.get(Account, id_1).code, "1111-003")
             self.assertEqual(db.session.get(Account, id_2).code, "1111-004")
             self.assertEqual(db.session.get(Account, id_3).code, "1111-002")
             self.assertEqual(db.session.get(Account, id_4).code, "1111-001")
             self.assertEqual(db.session.get(Account, id_5).code, "1111-005")
```

### Comparing `mia-accounting-1.5.6/tests/test_base_account.py` & `mia-accounting-1.5.7/tests/test_base_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,50 +35,51 @@
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
+        client: httpx.Client = get_client(self.__app, "nobody")
         response: httpx.Response
 
         response = client.get(LIST_URI)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(DETAIL_URI)
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
+        client: httpx.Client = get_client(self.__app, "viewer")
         response: httpx.Response
 
         response = client.get(LIST_URI)
         self.assertEqual(response.status_code, 200)
 
         response = client.get(DETAIL_URI)
         self.assertEqual(response.status_code, 200)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "editor")
+        client: httpx.Client = get_client(self.__app, "editor")
         response: httpx.Response
 
         response = client.get(LIST_URI)
         self.assertEqual(response.status_code, 200)
 
         response = client.get(DETAIL_URI)
         self.assertEqual(response.status_code, 200)
```

### Comparing `mia-accounting-1.5.6/tests/test_commands.py` & `mia-accounting-1.5.7/tests/test_commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the console commands.
 
 """
 import csv
+import datetime as dt
+import re
 import unittest
 from typing import Any
 
 import sqlalchemy as sa
 from click.testing import Result
 from flask import Flask
 from flask.testing import FlaskCliRunner
@@ -36,37 +38,38 @@
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
-            # Drop every accounting table, to see if accounting-init recreates
-            # them correctly.
+    def test_init_db(self) -> None:
+        """Tests the "accounting-init-db" console command.
+
+        :return: None.
+        """
+        with self.__app.app_context():
+            # Drop every accounting table, to see if accounting-init-db
+            # recreates them correctly.
             tables: list[sa.Table] \
                 = [db.metadata.tables[x] for x in db.metadata.tables
                    if x.startswith("accounting_")]
             for table in tables:
                 db.session.execute(DropTable(table))
             db.session.commit()
             inspector: sa.Inspector = sa.inspect(db.session.connection())
             self.assertEqual(len({x for x in inspector.get_table_names()
                                   if x.startswith("accounting_")}),
                              0)
 
-    def test_init(self) -> None:
-        """Tests the "accounting-init" console command.
-
-        :return: None.
-        """
-        runner: FlaskCliRunner = self.app.test_cli_runner()
-        with self.app.app_context():
+        runner: FlaskCliRunner = self.__app.test_cli_runner()
+        with self.__app.app_context():
             result: Result = runner.invoke(
                 args=["accounting-init-db", "-u", "editor"])
         self.assertEqual(result.exit_code, 0,
                          result.output + str(result.exception))
         self.__test_base_account_data()
         self.__test_account_data()
         self.__test_currency_data()
@@ -76,43 +79,63 @@
 
         :return: None.
         """
         from accounting import data_dir
         from accounting.models import BaseAccount
 
         with open(data_dir / "base_accounts.csv") as fp:
-            data: dict[dict[str, Any]] \
-                = {x["code"]: {"code": x["code"],
-                               "title": x["title"],
-                               "l10n": {y[5:]: x[y]
-                                        for y in x if y.startswith("l10n-")}}
-                   for x in csv.DictReader(fp)}
+            rows: list[dict[str, str]] = list(csv.DictReader(fp))
+        data: dict[dict[str, Any]] \
+            = {x["code"]: {"code": x["code"],
+                           "title": x["title"],
+                           "l10n": {y[5:]: x[y]
+                                    for y in x if y.startswith("l10n-")}}
+               for x in rows}
 
-        with self.app.app_context():
+        with self.__app.app_context():
             accounts: list[BaseAccount] = BaseAccount.query.all()
 
         self.assertEqual(len(accounts), len(data))
         for account in accounts:
             self.assertIn(account.code, data)
-            self.assertEqual(account.title_l10n, data[account.code]["title"])
+            self.assertEqual(account.title_l10n.lower(),
+                             data[account.code]["title"].lower())
+            self.__test_title_case(account.title_l10n)
             l10n: dict[str, str] = {x.locale: x.title for x in account.l10n}
             self.assertEqual(len(l10n), len(data[account.code]["l10n"]))
             for locale in l10n:
                 self.assertIn(locale, data[account.code]["l10n"])
                 self.assertEqual(l10n[locale],
                                  data[account.code]["l10n"][locale])
 
+    def __test_title_case(self, s: str) -> None:
+        """Tests the case of a base account title.
+
+        :param s: The base account title.
+        :return: None.
+        """
+        from accounting.utils.title_case import MINOR_WORDS
+
+        self.assertTrue(s[0].isupper(), s)
+        for word in re.findall(r"\w+", s):
+            if len(word) >= 4:
+                self.assertTrue(word.istitle(), s)
+            elif word in MINOR_WORDS:
+                self.assertTrue(word.islower(), s)
+            else:
+                self.assertTrue(word.istitle(), s)
+
     def __test_account_data(self) -> None:
         """Tests the account data.
 
         :return: None.
         """
         from accounting.models import BaseAccount, Account, AccountL10n
 
-        with self.app.app_context():
+        with self.__app.app_context():
             bases: list[BaseAccount] = BaseAccount.query\
                 .filter(sa.func.char_length(BaseAccount.code) == 4).all()
             accounts: list[Account] = Account.query.all()
             l10n: list[AccountL10n] = AccountL10n.query.all()
 
         self.assertEqual({x.code for x in bases},
                          {x.base_code for x in accounts})
@@ -138,20 +161,86 @@
             data: dict[dict[str, Any]] \
                 = {x["code"]: {"code": x["code"],
                                "name": x["name"],
                                "l10n": {y[5:]: x[y]
                                         for y in x if y.startswith("l10n-")}}
                    for x in csv.DictReader(fp)}
 
-        with self.app.app_context():
+        with self.__app.app_context():
             currencies: list[Currency] = Currency.query.all()
 
         self.assertEqual(len(currencies), len(data))
         for currency in currencies:
             self.assertIn(currency.code, data)
             self.assertEqual(currency.name_l10n, data[currency.code]["name"])
             l10n: dict[str, str] = {x.locale: x.name for x in currency.l10n}
             self.assertEqual(len(l10n), len(data[currency.code]["l10n"]))
             for locale in l10n:
                 self.assertIn(locale, data[currency.code]["l10n"])
                 self.assertEqual(l10n[locale],
                                  data[currency.code]["l10n"][locale])
+
+    def test_titleize(self) -> None:
+        """Tests the "accounting-titleize" console command.
+
+        :return: None.
+        """
+        from accounting.models import BaseAccount, Account
+        from accounting.utils.random_id import new_id
+        from accounting.utils.user import get_user_pk
+        runner: FlaskCliRunner = self.__app.test_cli_runner()
+
+        with self.__app.app_context():
+            # Resets the accounts.
+            tables: list[sa.Table] \
+                = [db.metadata.tables[x] for x in db.metadata.tables
+                   if x.startswith("accounting_")]
+            for table in tables:
+                db.session.execute(DropTable(table))
+            db.session.commit()
+            inspector: sa.Inspector = sa.inspect(db.session.connection())
+            self.assertEqual(len({x for x in inspector.get_table_names()
+                                  if x.startswith("accounting_")}),
+                             0)
+            result: Result = runner.invoke(
+                args=["accounting-init-db", "-u", "editor"])
+            self.assertEqual(result.exit_code, 0,
+                             result.output + str(result.exception))
+
+            # Turns the titles into lowercase.
+            for base in BaseAccount.query:
+                base.title_l10n = base.title_l10n.lower()
+            for account in Account.query:
+                account.title_l10n = account.title_l10n.lower()
+                account.created_at \
+                    = account.created_at - dt.timedelta(seconds=5)
+                account.updated_at = account.created_at
+
+            # Adds a custom account.
+            custom_title = "MBK Bank"
+            creator_pk: int = get_user_pk("editor")
+            new_account: Account = Account(
+                id=new_id(Account),
+                base_code="1112",
+                no="2",
+                title_l10n=custom_title,
+                is_need_offset=False,
+                created_by_id=creator_pk,
+                updated_by_id=creator_pk)
+            db.session.add(new_account)
+            db.session.commit()
+
+            result: Result = runner.invoke(
+                args=["accounting-titleize", "-u", "editor"])
+            self.assertEqual(result.exit_code, 0,
+                             result.output + str(result.exception))
+            for base in BaseAccount.query:
+                self.__test_title_case(base.title_l10n)
+            for account in Account.query:
+                if account.id != new_account.id:
+                    self.__test_title_case(account.title_l10n)
+                    self.assertNotEqual(account.created_at, account.updated_at)
+                else:
+                    self.assertEqual(account.title_l10n, custom_title)
+
+            db.session.delete(new_account)
+            db.session.commit()
```

### Comparing `mia-accounting-1.5.6/tests/test_description_editor.py` & `mia-accounting-1.5.7/tests/test_description_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,50 +16,56 @@
 #  limitations under the License.
 """The test for the description editor.
 
 """
 import datetime as dt
 import unittest
 
+import httpx
 from flask import Flask
 
 from accounting.utils.next_uri import encode_next
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
-    add_journal_entry
+    get_csrf_token, add_journal_entry
 
 
 class DescriptionEditorTestCase(unittest.TestCase):
     """The description editor test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_description_editor(self) -> None:
         """Test the description editor.
 
         :return: None.
         """
         from accounting.journal_entry.utils.description_editor import \
             DescriptionEditor
-        for form in get_form_data(self.csrf_token, self.encoded_next_uri):
-            add_journal_entry(self.client, form)
-        with self.app.app_context():
+        for form in get_form_data(self.__csrf_token, self.__encoded_next_uri):
+            add_journal_entry(self.__client, form)
+        with self.__app.app_context():
             editor: DescriptionEditor = DescriptionEditor()
 
         # Debit-General
         self.assertEqual(len(editor.debit.general.tags), 2)
         self.assertEqual(editor.debit.general.tags[0].name, "Lunch")
         self.assertEqual(len(editor.debit.general.tags[0].accounts), 2)
         self.assertEqual(editor.debit.general.tags[0].accounts[0].code,
```

### Comparing `mia-accounting-1.5.6/tests/test_journal_entry.py` & `mia-accounting-1.5.7/tests/test_journal_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import httpx
 from flask import Flask
 
 from accounting.utils.next_uri import encode_next
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
-    add_journal_entry, match_journal_entry_detail
+    get_csrf_token, add_journal_entry, match_journal_entry_detail
 from testlib_journal_entry import NON_EMPTY_NOTE, EMPTY_NOTE, \
     get_add_form, get_unchanged_update_form, get_update_form, \
     set_negative_amount, remove_debit_in_a_currency, \
     remove_credit_in_a_currency
 
 PREFIX: str = "/accounting/journal-entries"
 """The URL prefix for the journal entry management."""
@@ -44,31 +44,37 @@
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
-        journal_entry_id: int = add_journal_entry(self.client,
+        client: httpx.Client = get_client(self.__app, "nobody")
+        csrf_token: str = get_csrf_token(client)
+        journal_entry_id: int = add_journal_entry(self.__client,
                                                   self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         add_form["csrf_token"] = csrf_token
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         update_form["csrf_token"] = csrf_token
         response: httpx.Response
 
@@ -93,16 +99,17 @@
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
-        journal_entry_id: int = add_journal_entry(self.client,
+        client: httpx.Client = get_client(self.__app, "viewer")
+        csrf_token: str = get_csrf_token(client)
+        journal_entry_id: int = add_journal_entry(self.__client,
                                                   self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         add_form["csrf_token"] = csrf_token
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         update_form["csrf_token"] = csrf_token
         response: httpx.Response
 
@@ -127,130 +134,130 @@
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        journal_entry_id: int = add_journal_entry(self.client,
+        journal_entry_id: int = add_journal_entry(self.__client,
                                                   self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         response: httpx.Response
 
-        response = self.client.get(f"{PREFIX}/{journal_entry_id}")
+        response = self.__client.get(f"{PREFIX}/{journal_entry_id}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/create/receipt")
+        response = self.__client.get(f"{PREFIX}/create/receipt")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/store/receipt",
-                                    data=add_form)
+        response = self.__client.post(f"{PREFIX}/store/receipt",
+                                      data=add_form)
         self.assertEqual(response.status_code, 302)
         match_journal_entry_detail(response.headers["Location"])
 
-        response = self.client.get(f"{PREFIX}/{journal_entry_id}/edit")
+        response = self.__client.get(f"{PREFIX}/{journal_entry_id}/edit")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/{journal_entry_id}/update",
-                                    data=update_form)
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id}/update",
+                                      data=update_form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_id}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
-        response = self.client.post(f"{PREFIX}/{journal_entry_id}/delete",
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id}/delete",
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], RETURN_TO_URI)
 
     def test_add(self) -> None:
         """Tests to add the journal entries.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         create_uri: str = (f"{PREFIX}/create/receipt?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/receipt"
         response: httpx.Response
         form: dict[str, str]
         journal_entry: JournalEntry | None
 
         # No currency content
         form = self.__get_add_form()
         form = {x: form[x] for x in form if not x.startswith("currency-")}
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Missing currency
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = ""
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing currency
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = "ZZZ"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # No credit content in a currency
         form = self.__get_add_form()
         remove_credit_in_a_currency(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing account
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-account_code")][0]
         form[key] = "9999-999"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-credit account
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.OFFICE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # A receivable line item cannot start from credit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.RECEIVABLE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Negative amount
         form = self.__get_add_form()
         set_negative_amount(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Success
-        response = self.client.post(store_uri,
-                                    data=self.__get_add_form())
+        response = self.__client.post(store_uri,
+                                      data=self.__get_add_form())
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies), 3)
 
             self.assertEqual(currencies[0].code, "JPY")
             self.assertEqual(len(currencies[0].debit), 1)
@@ -304,116 +311,116 @@
                              Accounts.DONATION)
 
             self.assertEqual(journal_entry.note, NON_EMPTY_NOTE)
 
         # Success, with empty note
         form = self.__get_add_form()
         form["note"] = EMPTY_NOTE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             self.assertIsNone(journal_entry.note)
 
     def test_basic_update(self) -> None:
         """Tests the basic rules to update a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         edit_uri: str = (f"{PREFIX}/{journal_entry_id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
             old_id: set[int] = set()
             for currency in currencies0:
                 old_id.update({x.id for x in currency.debit})
 
         # No currency content
         form = form_0.copy()
         form = {x: form[x] for x in form if not x.startswith("currency-")}
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Missing currency
         form = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = ""
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing currency
         form = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = "ZZZ"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # No credit content in a currency
         form = form_0.copy()
         remove_credit_in_a_currency(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-account_code")][0]
         form[key] = "9999-999"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-credit account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.OFFICE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # A receivable line item cannot start from credit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.RECEIVABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Negative amount
         form: dict[str, str] = form_0.copy()
         set_negative_amount(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        response = self.client.post(update_uri, data=form_0)
+        response = self.__client.post(update_uri, data=form_0)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies1: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies1), 3)
 
             self.assertEqual(currencies1[0].code, "AUD")
             self.assertEqual(len(currencies1[0].debit), 1)
@@ -486,206 +493,214 @@
     def test_update_not_modified(self) -> None:
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
-        response = self.client.post(
+        response = self.__client.post(
             update_uri,
             data=self.__get_unchanged_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             journal_entry.created_at \
                 = journal_entry.created_at - dt.timedelta(seconds=5)
             journal_entry.updated_at = journal_entry.created_at
             db.session.commit()
 
-        response = self.client.post(
+        response = self.__client.post(
             update_uri, data=self.__get_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             self.assertLess(journal_entry.created_at, journal_entry.updated_at)
 
     def test_created_updated_by(self) -> None:
         """Tests the created-by and updated-by record.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         editor_username, admin_username = "editor", "admin"
-        client, csrf_token = get_client(self.app, admin_username)
+        client: httpx.Client = get_client(self.__app, admin_username)
+        csrf_token: str = get_csrf_token(client)
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
                              editor_username)
             self.assertEqual(journal_entry.updated_by.username,
                              editor_username)
 
         form: dict[str, str] = self.__get_update_form(journal_entry_id)
         form["csrf_token"] = csrf_token
         response = client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
                              editor_username)
             self.assertEqual(journal_entry.updated_by.username,
                              admin_username)
 
     def test_delete(self) -> None:
         """Tests to delete a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryLineItem
         journal_entry_id_1: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id_1}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         delete_uri: str = f"{PREFIX}/{journal_entry_id_1}/delete"
         response: httpx.Response
 
         form: dict[str, str] = self.__get_add_form()
         key: str = [x for x in form if x.endswith("-account_code")][0]
         form[key] = Accounts.PAYABLE
-        journal_entry_id_2: int = add_journal_entry(self.client, form)
-        with self.app.app_context():
+        journal_entry_id_2: int = add_journal_entry(self.__client, form)
+        with self.__app.app_context():
             journal_entry: JournalEntry | None \
                 = db.session.get(JournalEntry, journal_entry_id_2)
             self.assertIsNotNone(journal_entry)
             line_item: JournalEntryLineItem \
                 = [x for x in journal_entry.line_items
                    if x.account_code == Accounts.PAYABLE][0]
         add_journal_entry(
-            self.client,
-            form={"csrf_token": self.csrf_token,
-                  "next": self.encoded_next_uri,
+            self.__client,
+            form={"csrf_token": self.__csrf_token,
+                  "next": self.__encoded_next_uri,
                   "date": dt.date.today().isoformat(),
                   "currency-1-code": line_item.currency_code,
                   "currency-1-debit-1-original_line_item_id": line_item.id,
                   "currency-1-debit-1-account_code": line_item.account_code,
                   "currency-1-debit-1-amount": "1"})
 
         # Cannot delete the journal entry that is in use
-        response = self.client.post(f"{PREFIX}/{journal_entry_id_2}/delete",
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id_2}/delete",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_id_2}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
         # Success
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 404)
 
     def __get_add_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token,
-                                            self.encoded_next_uri)
+        form: dict[str, str] = get_add_form(self.__csrf_token,
+                                            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
     def __get_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             not changed.
         """
         form: dict[str, str] = get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
     def __get_update_form(self, journal_entry_id: int) -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             changed.
         """
         form: dict[str, str] = get_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri,
-            False)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri, False)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
 
 class CashDisbursementJournalEntryTestCase(unittest.TestCase):
     """The cash disbursement journal entry test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
+        client: httpx.Client = get_client(self.__app, "nobody")
+        csrf_token: str = get_csrf_token(client)
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         add_form["csrf_token"] = csrf_token
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         update_form["csrf_token"] = csrf_token
         response: httpx.Response
 
         response = client.get(f"{PREFIX}/{journal_entry_id}")
@@ -709,17 +724,18 @@
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
+        client: httpx.Client = get_client(self.__app, "viewer")
+        csrf_token: str = get_csrf_token(client)
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         add_form["csrf_token"] = csrf_token
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         update_form["csrf_token"] = csrf_token
         response: httpx.Response
 
         response = client.get(f"{PREFIX}/{journal_entry_id}")
@@ -744,129 +760,129 @@
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         response: httpx.Response
 
-        response = self.client.get(f"{PREFIX}/{journal_entry_id}")
+        response = self.__client.get(f"{PREFIX}/{journal_entry_id}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/create/disbursement")
+        response = self.__client.get(f"{PREFIX}/create/disbursement")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/store/disbursement",
-                                    data=add_form)
+        response = self.__client.post(f"{PREFIX}/store/disbursement",
+                                      data=add_form)
         self.assertEqual(response.status_code, 302)
         match_journal_entry_detail(response.headers["Location"])
 
-        response = self.client.get(f"{PREFIX}/{journal_entry_id}/edit")
+        response = self.__client.get(f"{PREFIX}/{journal_entry_id}/edit")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/{journal_entry_id}/update",
-                                    data=update_form)
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id}/update",
+                                      data=update_form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_id}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
-        response = self.client.post(f"{PREFIX}/{journal_entry_id}/delete",
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id}/delete",
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], RETURN_TO_URI)
 
     def test_add(self) -> None:
         """Tests to add the journal entries.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         create_uri: str = (f"{PREFIX}/create/disbursement?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/disbursement"
         response: httpx.Response
         form: dict[str, str]
         journal_entry: JournalEntry | None
 
         # No currency content
         form = self.__get_add_form()
         form = {x: form[x] for x in form if not x.startswith("currency-")}
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Missing currency
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = ""
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing currency
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = "ZZZ"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # No debit content in a currency
         form = self.__get_add_form()
         remove_debit_in_a_currency(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing account
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-account_code")][0]
         form[key] = "9999-999"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-debit account
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.SERVICE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # A payable line item cannot start from debit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.PAYABLE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Negative amount
         form = self.__get_add_form()
         set_negative_amount(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Success
-        response = self.client.post(store_uri,
-                                    data=self.__get_add_form())
+        response = self.__client.post(store_uri,
+                                      data=self.__get_add_form())
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies), 3)
 
             self.assertEqual(currencies[0].code, "JPY")
             self.assertEqual(len(currencies[0].debit), 2)
@@ -923,116 +939,116 @@
                              sum([x.amount for x in currencies[2].debit]))
 
             self.assertEqual(journal_entry.note, NON_EMPTY_NOTE)
 
         # Success, with empty note
         form = self.__get_add_form()
         form["note"] = EMPTY_NOTE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             self.assertIsNone(journal_entry.note)
 
     def test_basic_update(self) -> None:
         """Tests the basic rules to update a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         edit_uri: str = (f"{PREFIX}/{journal_entry_id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
             old_id: set[int] = set()
             for currency in currencies0:
                 old_id.update({x.id for x in currency.debit})
 
         # No currency content
         form = form_0.copy()
         form = {x: form[x] for x in form if not x.startswith("currency-")}
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Missing currency
         form = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = ""
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing currency
         form = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = "ZZZ"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # No debit content in a currency
         form = form_0.copy()
         remove_debit_in_a_currency(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-account_code")][0]
         form[key] = "9999-999"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-debit account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.SERVICE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # A payable line item cannot start from debit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.PAYABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Negative amount
         form: dict[str, str] = form_0.copy()
         set_negative_amount(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        response = self.client.post(update_uri, data=form_0)
+        response = self.__client.post(update_uri, data=form_0)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies1: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies1), 3)
 
             self.assertEqual(currencies1[0].code, "AUD")
             self.assertEqual(len(currencies1[0].debit), 2)
@@ -1109,175 +1125,183 @@
     def test_update_not_modified(self) -> None:
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
-        response = self.client.post(
+        response = self.__client.post(
             update_uri,
             data=self.__get_unchanged_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             journal_entry.created_at \
                 = journal_entry.created_at - dt.timedelta(seconds=5)
             journal_entry.updated_at = journal_entry.created_at
             db.session.commit()
 
-        response = self.client.post(
+        response = self.__client.post(
             update_uri, data=self.__get_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             self.assertLess(journal_entry.created_at, journal_entry.updated_at)
 
     def test_created_updated_by(self) -> None:
         """Tests the created-by and updated-by record.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         editor_username, admin_username = "editor", "admin"
-        client, csrf_token = get_client(self.app, admin_username)
+        client: httpx.Client = get_client(self.__app, admin_username)
+        csrf_token: str = get_csrf_token(client)
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
                              editor_username)
             self.assertEqual(journal_entry.updated_by.username,
                              editor_username)
 
         form: dict[str, str] = self.__get_update_form(journal_entry_id)
         form["csrf_token"] = csrf_token
         response = client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
                              editor_username)
             self.assertEqual(journal_entry.updated_by.username,
                              admin_username)
 
     def test_delete(self) -> None:
         """Tests to delete a journal entry.
 
         :return: None.
         """
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         delete_uri: str = f"{PREFIX}/{journal_entry_id}/delete"
         response: httpx.Response
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 404)
 
     def __get_add_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token,
-                                            self.encoded_next_uri)
+        form: dict[str, str] = get_add_form(self.__csrf_token,
+                                            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             not changed.
         """
         form: dict[str, str] = get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_update_form(self, journal_entry_id: int) -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             changed.
         """
         form: dict[str, str] = get_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri,
-            True)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri, True)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
 
 class TransferJournalEntryTestCase(unittest.TestCase):
     """The transfer journal entry test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, \
                 JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
+        client: httpx.Client = get_client(self.__app, "nobody")
+        csrf_token: str = get_csrf_token(client)
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         add_form["csrf_token"] = csrf_token
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         update_form["csrf_token"] = csrf_token
         response: httpx.Response
 
         response = client.get(f"{PREFIX}/{journal_entry_id}")
@@ -1301,17 +1325,18 @@
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
+        client: httpx.Client = get_client(self.__app, "viewer")
+        csrf_token: str = get_csrf_token(client)
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         add_form["csrf_token"] = csrf_token
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         update_form["csrf_token"] = csrf_token
         response: httpx.Response
 
         response = client.get(f"{PREFIX}/{journal_entry_id}")
@@ -1336,162 +1361,162 @@
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         add_form: dict[str, str] = self.__get_add_form()
         update_form: dict[str, str] = self.__get_update_form(journal_entry_id)
         response: httpx.Response
 
-        response = self.client.get(f"{PREFIX}/{journal_entry_id}")
+        response = self.__client.get(f"{PREFIX}/{journal_entry_id}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/create/transfer")
+        response = self.__client.get(f"{PREFIX}/create/transfer")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/store/transfer",
-                                    data=add_form)
+        response = self.__client.post(f"{PREFIX}/store/transfer",
+                                      data=add_form)
         self.assertEqual(response.status_code, 302)
         match_journal_entry_detail(response.headers["Location"])
 
-        response = self.client.get(f"{PREFIX}/{journal_entry_id}/edit")
+        response = self.__client.get(f"{PREFIX}/{journal_entry_id}/edit")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(f"{PREFIX}/{journal_entry_id}/update",
-                                    data=update_form)
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id}/update",
+                                      data=update_form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_id}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
-        response = self.client.post(f"{PREFIX}/{journal_entry_id}/delete",
-                                    data={"csrf_token": self.csrf_token})
+        response = self.__client.post(f"{PREFIX}/{journal_entry_id}/delete",
+                                      data={"csrf_token": self.__csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], RETURN_TO_URI)
 
     def test_add(self) -> None:
         """Tests to add the journal entries.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         create_uri: str = (f"{PREFIX}/create/transfer?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/transfer"
         response: httpx.Response
         form: dict[str, str]
         journal_entry: JournalEntry | None
 
         # No currency content
         form = self.__get_add_form()
         form = {x: form[x] for x in form if not x.startswith("currency-")}
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Missing currency
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = ""
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing currency
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = "ZZZ"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # No debit content in a currency
         form = self.__get_add_form()
         remove_debit_in_a_currency(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # No credit content in a currency
         form = self.__get_add_form()
         remove_credit_in_a_currency(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-existing account
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-account_code")][0]
         form[key] = "9999-999"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-debit account
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.SERVICE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Non-credit account
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.OFFICE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # A receivable line item cannot start from credit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.RECEIVABLE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # A payable line item cannot start from debit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.PAYABLE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Negative amount
         form = self.__get_add_form()
         set_negative_amount(form)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not balanced
         form = self.__get_add_form()
         key: str = [x for x in form.keys() if x.endswith("-amount")][0]
         form[key] = str(Decimal(form[key]) + 1000)
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Success
-        response = self.client.post(store_uri,
-                                    data=self.__get_add_form())
+        response = self.__client.post(store_uri,
+                                      data=self.__get_add_form())
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies), 3)
 
             self.assertEqual(currencies[0].code, "JPY")
             self.assertEqual(len(currencies[0].debit), 2)
@@ -1551,149 +1576,149 @@
                              Accounts.DONATION)
 
             self.assertEqual(journal_entry.note, NON_EMPTY_NOTE)
 
         # Success, with empty note
         form = self.__get_add_form()
         form["note"] = EMPTY_NOTE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             self.assertIsNone(journal_entry.note)
 
     def test_basic_update(self) -> None:
         """Tests the basic rules to update a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         edit_uri: str = (f"{PREFIX}/{journal_entry_id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
             old_id: set[int] = set()
             for currency in currencies0:
                 old_id.update({x.id for x in currency.debit})
 
         # No currency content
         form = form_0.copy()
         form = {x: form[x] for x in form if not x.startswith("currency-")}
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Missing currency
         form = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = ""
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing currency
         form = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-code")][0]
         form[key] = "ZZZ"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # No debit content in a currency
         form = form_0.copy()
         remove_debit_in_a_currency(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # No credit content in a currency
         form = form_0.copy()
         remove_credit_in_a_currency(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-account_code")][0]
         form[key] = "9999-999"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-debit account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.SERVICE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-credit account
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.OFFICE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # A receivable line item cannot start from credit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-credit-" in x][0]
         form[key] = Accounts.RECEIVABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # A payable line item cannot start from debit
         form = self.__get_add_form()
         key: str = [x for x in form.keys()
                     if x.endswith("-account_code") and "-debit-" in x][0]
         form[key] = Accounts.PAYABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Negative amount
         form: dict[str, str] = form_0.copy()
         set_negative_amount(form)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not balanced
         form: dict[str, str] = form_0.copy()
         key: str = [x for x in form.keys() if x.endswith("-amount")][0]
         form[key] = str(Decimal(form[key]) + 1000)
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        response = self.client.post(update_uri, data=form_0)
+        response = self.__client.post(update_uri, data=form_0)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies1: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies1), 3)
 
             self.assertEqual(currencies1[0].code, "AUD")
             self.assertEqual(len(currencies1[0].debit), 2)
@@ -1780,110 +1805,111 @@
     def test_update_not_modified(self) -> None:
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
-        response = self.client.post(
+        response = self.__client.post(
             update_uri,
             data=self.__get_unchanged_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             journal_entry.created_at \
                 = journal_entry.created_at - dt.timedelta(seconds=5)
             journal_entry.updated_at = journal_entry.created_at
             db.session.commit()
 
-        response = self.client.post(
+        response = self.__client.post(
             update_uri, data=self.__get_update_form(journal_entry_id))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             self.assertLess(journal_entry.created_at, journal_entry.updated_at)
 
     def test_created_updated_by(self) -> None:
         """Tests the created-by and updated-by record.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         editor_username, admin_username = "editor", "admin"
-        client, csrf_token = get_client(self.app, admin_username)
+        client: httpx.Client = get_client(self.__app, admin_username)
+        csrf_token: str = get_csrf_token(client)
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
                              editor_username)
             self.assertEqual(journal_entry.updated_by.username,
                              editor_username)
 
         form: dict[str, str] = self.__get_update_form(journal_entry_id)
         form["csrf_token"] = csrf_token
         response = client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
                              editor_username)
             self.assertEqual(journal_entry.updated_by.username,
                              admin_username)
 
     def test_save_as_receipt(self) -> None:
         """Tests to save a transfer journal entry as a cash receipt journal
         entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update?as=receipt"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
         form_0 = {x: form_0[x] for x in form_0 if "-debit-" not in x}
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
             old_id: set[int] = set()
             for currency in currencies0:
                 old_id.update({x.id for x in currency.debit})
 
         # Success
-        response = self.client.post(update_uri, data=form_0)
+        response = self.__client.post(update_uri, data=form_0)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies1: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies1), 3)
 
             self.assertEqual(currencies1[0].code, "AUD")
             self.assertEqual(len(currencies1[0].debit), 1)
@@ -1957,35 +1983,35 @@
         """Tests to save a transfer journal entry as a cash disbursement
         journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update?as=disbursement"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
         form_0 = {x: form_0[x] for x in form_0 if "-credit-" not in x}
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
             old_id: set[int] = set()
             for currency in currencies0:
                 old_id.update({x.id for x in currency.debit})
 
         # Success
-        response = self.client.post(update_uri, data=form_0)
+        response = self.__client.post(update_uri, data=form_0)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies1: list[JournalEntryCurrency] = journal_entry.currencies
             self.assertEqual(len(currencies1), 3)
 
             self.assertEqual(currencies1[0].code, "AUD")
             self.assertEqual(len(currencies1[0].debit), 2)
@@ -2061,106 +2087,112 @@
 
     def test_delete(self) -> None:
         """Tests to delete a journal entry.
 
         :return: None.
         """
         journal_entry_id: int \
-            = add_journal_entry(self.client, self.__get_add_form())
+            = add_journal_entry(self.__client, self.__get_add_form())
         detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         delete_uri: str = f"{PREFIX}/{journal_entry_id}/delete"
         response: httpx.Response
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
-        response = self.client.post(delete_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(delete_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 404)
 
     def __get_add_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        return get_add_form(self.csrf_token, self.encoded_next_uri)
+        return get_add_form(self.__csrf_token, self.__encoded_next_uri)
 
     def __get_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             not changed.
         """
         return get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri)
 
     def __get_update_form(self, journal_entry_id: int) -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             changed.
         """
         return get_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri,
-            None)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri, None)
 
 
 class JournalEntryReorderTestCase(unittest.TestCase):
     """The journal entry reorder test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_change_date(self) -> None:
         """Tests to change the date of a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         response: httpx.Response
 
-        id_1: int = add_journal_entry(self.client,
+        id_1: int = add_journal_entry(self.__client,
                                       self.__get_add_receipt_form())
-        id_2: int = add_journal_entry(self.client,
+        id_2: int = add_journal_entry(self.__client,
                                       self.__get_add_disbursement_form())
-        id_3: int = add_journal_entry(self.client,
+        id_3: int = add_journal_entry(self.__client,
                                       self.__get_add_transfer_form())
-        id_4: int = add_journal_entry(self.client,
+        id_4: int = add_journal_entry(self.__client,
                                       self.__get_add_receipt_form())
-        id_5: int = add_journal_entry(self.client,
+        id_5: int = add_journal_entry(self.__client,
                                       self.__get_add_disbursement_form())
 
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry_1: JournalEntry = db.session.get(JournalEntry, id_1)
             journal_entry_date_2: dt.date = journal_entry_1.date
             journal_entry_date_1: dt.date \
                 = journal_entry_date_2 - dt.timedelta(days=1)
             journal_entry_1.date = journal_entry_date_1
             journal_entry_1.no = 3
             journal_entry_2: JournalEntry = db.session.get(JournalEntry, id_2)
@@ -2174,126 +2206,127 @@
             journal_entry_5: JournalEntry = db.session.get(JournalEntry, id_5)
             journal_entry_5.no = 6
             db.session.commit()
 
         form: dict[str, str] \
             = self.__get_disbursement_unchanged_update_form(id_2)
         form["date"] = journal_entry_date_2.isoformat()
-        response = self.client.post(f"{PREFIX}/{id_2}/update", data=form)
+        response = self.__client.post(f"{PREFIX}/{id_2}/update", data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{id_2}?next={self.encoded_next_uri}")
+                         f"{PREFIX}/{id_2}?next={self.__encoded_next_uri}")
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 3)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 2)
             self.assertEqual(db.session.get(JournalEntry, id_4).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 2)
 
     def test_reorder(self) -> None:
         """Tests to reorder the journal entries in a same day.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         response: httpx.Response
 
-        id_1: int = add_journal_entry(self.client,
+        id_1: int = add_journal_entry(self.__client,
                                       self.__get_add_receipt_form())
-        id_2: int = add_journal_entry(self.client,
+        id_2: int = add_journal_entry(self.__client,
                                       self.__get_add_disbursement_form())
-        id_3: int = add_journal_entry(self.client,
+        id_3: int = add_journal_entry(self.__client,
                                       self.__get_add_transfer_form())
-        id_4: int = add_journal_entry(self.client,
+        id_4: int = add_journal_entry(self.__client,
                                       self.__get_add_receipt_form())
-        id_5: int = add_journal_entry(self.client,
+        id_5: int = add_journal_entry(self.__client,
                                       self.__get_add_disbursement_form())
 
-        with self.app.app_context():
+        with self.__app.app_context():
             date: dt.date = db.session.get(JournalEntry, id_1).date
 
-        response = self.client.post(
+        response = self.__client.post(
             f"{PREFIX}/dates/{date.isoformat()}",
-            data={"csrf_token": self.csrf_token,
-                  "next": self.encoded_next_uri,
+            data={"csrf_token": self.__csrf_token,
+                  "next": self.__encoded_next_uri,
                   f"{id_1}-no": "4",
                   f"{id_2}-no": "1",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2",
                   f"{id_5}-no": "3"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 4)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 5)
             self.assertEqual(db.session.get(JournalEntry, id_4).no, 2)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 3)
 
         # Malformed orders
-        with self.app.app_context():
+        with self.__app.app_context():
             db.session.get(JournalEntry, id_1).no = 3
             db.session.get(JournalEntry, id_2).no = 4
             db.session.get(JournalEntry, id_3).no = 6
             db.session.get(JournalEntry, id_4).no = 8
             db.session.get(JournalEntry, id_5).no = 9
             db.session.commit()
 
-        response = self.client.post(
+        response = self.__client.post(
             f"{PREFIX}/dates/{date.isoformat()}",
-            data={"csrf_token": self.csrf_token,
-                  "next": self.encoded_next_uri,
+            data={"csrf_token": self.__csrf_token,
+                  "next": self.__encoded_next_uri,
                   f"{id_2}-no": "3a",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 3)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 4)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 2)
             self.assertEqual(db.session.get(JournalEntry, id_4).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 5)
 
     def __get_add_receipt_form(self) -> dict[str, str]:
         """Returns the form data to add a new cash receipt journal entry.
 
         :return: The form data to add a new cash receipt journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token,
-                                            self.encoded_next_uri)
+        form: dict[str, str] = get_add_form(self.__csrf_token,
+                                            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
     def __get_add_disbursement_form(self) -> dict[str, str]:
         """Returns the form data to add a new cash disbursement journal entry.
 
         :return: The form data to add a new cash disbursement journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token,
-                                            self.encoded_next_uri)
+        form: dict[str, str] = get_add_form(self.__csrf_token,
+                                            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_disbursement_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a cash disbursement journal entry,
         where the data are not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the cash disbursement journal entry,
             where the data are not changed.
         """
         form: dict[str, str] = get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
+            journal_entry_id, self.__app, self.__csrf_token,
+            self.__encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_add_transfer_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        return get_add_form(self.csrf_token, self.encoded_next_uri)
+        return get_add_form(self.__csrf_token, self.__encoded_next_uri)
```

### Comparing `mia-accounting-1.5.6/tests/test_offset.py` & `mia-accounting-1.5.7/tests/test_offset.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,757 +26,763 @@
 from flask import Flask
 
 from accounting.utils.next_uri import encode_next
 from test_site import db
 from test_site.lib import JournalEntryLineItemData, JournalEntryCurrencyData, \
     JournalEntryData, BaseTestData
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
-    match_journal_entry_detail
+    get_csrf_token, match_journal_entry_detail
 
 PREFIX: str = "/accounting/journal-entries"
 """The URL prefix for the journal entry management."""
 
 
 class OffsetTestCase(unittest.TestCase):
     """The offset test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
-        self.data: OffsetTestData = OffsetTestData(self.app, "editor")
-        self.data.populate()
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
+        self.__data: OffsetTestData = OffsetTestData(self.__app, "editor")
+        """The offset test data."""
+        self.__data.populate()
 
     def test_add_receivable_offset(self) -> None:
         """Tests to add the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
         create_uri: str = (f"{PREFIX}/create/receipt?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/receipt"
         form: dict[str, str]
         old_amount: Decimal
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
-            self.data.l_r_or3d.journal_entry.days, [JournalEntryCurrencyData(
+            self.__data.l_r_or3d.journal_entry.days, [JournalEntryCurrencyData(
                 "USD",
                 [],
                 [JournalEntryLineItemData(
                     Accounts.RECEIVABLE,
-                    self.data.l_r_or1d.description, "300",
-                    original_line_item=self.data.l_r_or1d),
+                    self.__data.l_r_or1d.description, "300",
+                    original_line_item=self.__data.l_r_or1d),
                  JournalEntryLineItemData(
                      Accounts.RECEIVABLE,
-                     self.data.l_r_or1d.description, "100",
-                     original_line_item=self.data.l_r_or1d),
+                     self.__data.l_r_or1d.description, "100",
+                     original_line_item=self.__data.l_r_or1d),
                  JournalEntryLineItemData(
                      Accounts.RECEIVABLE,
-                     self.data.l_r_or3d.description, "100",
-                     original_line_item=self.data.l_r_or3d)])])
+                     self.__data.l_r_or3d.description, "100",
+                     original_line_item=self.__data.l_r_or3d)])])
 
         # Non-existing original line item ID
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
-            = str(self.data.l_p_or1c.id)
-        form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
+            = str(self.__data.l_p_or1c.id)
+        form["currency-1-credit-1-account_code"] = self.__data.l_p_or1c.account
         form["currency-1-credit-1-amount"] = "100"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = False
             db.session.commit()
-        response = self.client.post(
+        response = self.__client.post(
             store_uri,
-            data=journal_entry_data.new_form(self.csrf_token,
-                                             self.encoded_next_uri))
+            data=journal_entry_data.new_form(self.__csrf_token,
+                                             self.__encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
-            = str(self.data.l_p_of1d.id)
-        form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
-        response = self.client.post(store_uri, data=form)
+            = str(self.__data.l_p_of1d.id)
+        form["currency-1-credit-1-account_code"] = self.__data.l_p_of1d.account
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-code"] = "EUR"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same account
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_RECEIVABLE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not before the original line items
         old_days = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
-        response = self.client.post(store_uri, data=form)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
-        response = self.client.post(store_uri, data=form)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].credit:
                 self.assertIsNotNone(offset.original_line_item_id)
 
     def test_edit_receivable_offset(self) -> None:
         """Tests to edit the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account
-        journal_entry_data: JournalEntryData = self.data.j_r_of2
+        journal_entry_data: JournalEntryData = self.__data.j_r_of2
         edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.j_r_or2.days
+        journal_entry_data.days = self.__data.j_r_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("600")
 
         # Non-existing original line item ID
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
-            = str(self.data.l_p_or1c.id)
-        form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
+            = str(self.__data.l_p_or1c.id)
+        form["currency-1-credit-1-account_code"] = self.__data.l_p_or1c.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The original line item does not need offset
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = False
             db.session.commit()
-        response = self.client.post(
+        response = self.__client.post(
             update_uri,
-            data=journal_entry_data.update_form(self.csrf_token,
-                                                self.encoded_next_uri))
+            data=journal_entry_data.update_form(self.__csrf_token,
+                                                self.__encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
-            = str(self.data.l_p_of1d.id)
-        form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
-        response = self.client.post(update_uri, data=form)
+            = str(self.__data.l_p_of1d.id)
+        form["currency-1-credit-1-account_code"] = self.__data.l_p_of1d.account
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-code"] = "EUR"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_RECEIVABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_data.id}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
     def test_edit_receivable_original_line_item(self) -> None:
         """Tests to edit the receivable original line item.
 
         :return: None.
         """
         from accounting.models import JournalEntry
-        journal_entry_data: JournalEntryData = self.data.j_r_or1
+        journal_entry_data: JournalEntryData = self.__data.j_r_or1
         edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.j_r_of1.days
+        journal_entry_data.days = self.__data.j_r_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("3.4")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("3.4")
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-code"] = "EUR"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_RECEIVABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - partially offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   - Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   - Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - fully offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-2-amount"] \
             = str(journal_entry_data.currencies[0].debit[1].amount
                   - Decimal("0.01"))
         form["currency-1-credit-2-amount"] \
             = str(journal_entry_data.currencies[0].credit[1].amount
                   - Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not after the offset items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days - 1
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Not deleting matched original line items
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         del form["currency-1-debit-1-id"]
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_data.id}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
         # The original line item is always before the offset item, even when
         # they happen in the same day.
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry_or: JournalEntry | None = db.session.get(
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
             journal_entry_of: JournalEntry | None = db.session.get(
-                JournalEntry, self.data.j_r_of1.id)
+                JournalEntry, self.__data.j_r_of1.id)
             self.assertIsNotNone(journal_entry_of)
             self.assertEqual(journal_entry_or.date, journal_entry_of.date)
             self.assertLess(journal_entry_or.no, journal_entry_of.no)
 
     def test_add_payable_offset(self) -> None:
         """Tests to add the payable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
         create_uri: str = (f"{PREFIX}/create/disbursement?"
-                           f"next={self.encoded_next_uri}")
+                           f"next={self.__encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/disbursement"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
-            self.data.l_p_or3c.journal_entry.days, [JournalEntryCurrencyData(
+            self.__data.l_p_or3c.journal_entry.days, [JournalEntryCurrencyData(
                 "USD",
                 [JournalEntryLineItemData(
                     Accounts.PAYABLE,
-                    self.data.l_p_or1c.description, "500",
-                    original_line_item=self.data.l_p_or1c),
+                    self.__data.l_p_or1c.description, "500",
+                    original_line_item=self.__data.l_p_or1c),
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
-                     self.data.l_p_or1c.description, "300",
-                     original_line_item=self.data.l_p_or1c),
+                     self.__data.l_p_or1c.description, "300",
+                     original_line_item=self.__data.l_p_or1c),
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
-                     self.data.l_p_or3c.description, "120",
-                     original_line_item=self.data.l_p_or3c)],
+                     self.__data.l_p_or3c.description, "120",
+                     original_line_item=self.__data.l_p_or3c)],
                 [])])
 
         # Non-existing original line item ID
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
-            = str(self.data.l_r_or1d.id)
-        form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
+            = str(self.__data.l_r_or1d.id)
+        form["currency-1-debit-1-account_code"] = self.__data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = False
             db.session.commit()
-        response = self.client.post(
+        response = self.__client.post(
             store_uri,
-            data=journal_entry_data.new_form(self.csrf_token,
-                                             self.encoded_next_uri))
+            data=journal_entry_data.new_form(self.__csrf_token,
+                                             self.__encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
-            = str(self.data.l_r_of1c.id)
-        form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
-        response = self.client.post(store_uri, data=form)
+            = str(self.__data.l_r_of1c.id)
+        form["currency-1-debit-1-account_code"] = self.__data.l_r_of1c.account
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-code"] = "EUR"
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same account
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_PAYABLE
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
-        response = self.client.post(store_uri, data=form)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
-        response = self.client.post(store_uri, data=form)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.new_form(self.csrf_token,
-                                           self.encoded_next_uri)
-        response = self.client.post(store_uri, data=form)
+        form = journal_entry_data.new_form(self.__csrf_token,
+                                           self.__encoded_next_uri)
+        response = self.__client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].debit:
                 self.assertIsNotNone(offset.original_line_item_id)
 
     def test_edit_payable_offset(self) -> None:
         """Tests to edit the payable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
-        journal_entry_data: JournalEntryData = self.data.j_p_of2
+        journal_entry_data: JournalEntryData = self.__data.j_p_of2
         edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.j_p_or2.days
+        journal_entry_data.days = self.__data.j_p_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("900")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("900")
 
         # Non-existing original line item ID
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
-            = str(self.data.l_r_or1d.id)
-        form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
+            = str(self.__data.l_r_or1d.id)
+        form["currency-1-debit-1-account_code"] = self.__data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The original line item does not need offset
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = False
             db.session.commit()
-        response = self.client.post(
+        response = self.__client.post(
             update_uri,
-            data=journal_entry_data.update_form(self.csrf_token,
-                                                self.encoded_next_uri))
+            data=journal_entry_data.update_form(self.__csrf_token,
+                                                self.__encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
-            = str(self.data.l_r_of1c.id)
-        form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
-        response = self.client.post(update_uri, data=form)
+            = str(self.__data.l_r_of1c.id)
+        form["currency-1-debit-1-account_code"] = self.__data.l_r_of1c.account
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-code"] = "EUR"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_PAYABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].debit:
                 self.assertIsNotNone(offset.original_line_item_id)
 
     def test_edit_payable_original_line_item(self) -> None:
         """Tests to edit the payable original line item.
 
         :return: None.
         """
         from accounting.models import JournalEntry
-        journal_entry_data: JournalEntryData = self.data.j_p_or1
+        journal_entry_data: JournalEntryData = self.__data.j_p_or1
         edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
-        journal_entry_data.days = self.data.j_p_of1.days
+        journal_entry_data.days = self.__data.j_p_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("0.9")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("0.9")
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-code"] = "EUR"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_PAYABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - partially offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   - Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   - Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - fully offset
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         form["currency-1-debit-2-amount"] \
             = str(journal_entry_data.currencies[0].debit[1].amount
                   - Decimal("0.01"))
         form["currency-1-credit-2-amount"] \
             = str(journal_entry_data.currencies[0].credit[1].amount
                   - Decimal("0.01"))
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not after the offset items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days - 1
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Not deleting matched original line items
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
         del form["currency-1-credit-1-id"]
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token,
-                                              self.encoded_next_uri)
-        response = self.client.post(update_uri, data=form)
+        form = journal_entry_data.update_form(self.__csrf_token,
+                                              self.__encoded_next_uri)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_data.id}?"
-                         f"next={self.encoded_next_uri}")
+                         f"next={self.__encoded_next_uri}")
 
         # The original line item is always before the offset item, even when
         # they happen in the same day
-        with self.app.app_context():
+        with self.__app.app_context():
             journal_entry_or: JournalEntry | None = db.session.get(
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
             journal_entry_of: JournalEntry | None = db.session.get(
-                JournalEntry, self.data.j_p_of1.id)
+                JournalEntry, self.__data.j_p_of1.id)
             self.assertIsNotNone(journal_entry_of)
             self.assertEqual(journal_entry_or.date, journal_entry_of.date)
             self.assertLess(journal_entry_or.no, journal_entry_of.no)
 
 
 class OffsetTestData(BaseTestData):
     """The offset test data."""
@@ -803,26 +809,30 @@
             "Envelop", "0.9", Accounts.OFFICE, Accounts.PAYABLE)
 
         # Original journal entries
         self.j_r_or1: JournalEntryData = JournalEntryData(
             50, [JournalEntryCurrencyData(
                 "USD", [self.l_r_or1d, self.l_r_or4d],
                 [self.l_r_or1c, self.l_r_or4c])])
+        """The receivable original journal entry #1."""
         self.j_r_or2: JournalEntryData = JournalEntryData(
             30, [JournalEntryCurrencyData(
                 "USD", [self.l_r_or2d, self.l_r_or3d],
                 [self.l_r_or2c, self.l_r_or3c])])
+        """The receivable original journal entry #2."""
         self.j_p_or1: JournalEntryData = JournalEntryData(
             40, [JournalEntryCurrencyData(
                 "USD", [self.l_p_or1d, self.l_p_or4d],
                 [self.l_p_or1c, self.l_p_or4c])])
+        """The payable original journal entry #1."""
         self.j_p_or2: JournalEntryData = JournalEntryData(
             20, [JournalEntryCurrencyData(
                 "USD", [self.l_p_or2d, self.l_p_or3d],
                 [self.l_p_or2c, self.l_p_or3c])])
+        """The payable original journal entry #2."""
 
         self._add_journal_entry(self.j_r_or1)
         self._add_journal_entry(self.j_r_or2)
         self._add_journal_entry(self.j_p_or1)
         self._add_journal_entry(self.j_p_or2)
 
         # Receivable offset items
@@ -859,31 +869,37 @@
             "Envelop", "0.9", Accounts.PAYABLE, Accounts.CASH)
         self.l_p_of5d.original_line_item = self.l_p_or4c
 
         # Offset journal entries
         self.j_r_of1: JournalEntryData = JournalEntryData(
             25, [JournalEntryCurrencyData(
                 "USD", [self.l_r_of1d], [self.l_r_of1c])])
+        """The offset journal entry to the receivable #1."""
         self.j_r_of2: JournalEntryData = JournalEntryData(
             20, [JournalEntryCurrencyData(
                 "USD", [self.l_r_of2d, self.l_r_of3d, self.l_r_of4d],
                 [self.l_r_of2c, self.l_r_of3c, self.l_r_of4c])])
+        """The offset journal entry to the receivable #2."""
         self.j_r_of3: JournalEntryData = JournalEntryData(
             15, [JournalEntryCurrencyData(
                 "USD", [self.l_r_of5d], [self.l_r_of5c])])
+        """The offset journal entry to the receivable #3."""
         self.j_p_of1: JournalEntryData = JournalEntryData(
             15, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of1d], [self.l_p_of1c])])
+        """The offset journal entry to the payable #1."""
         self.j_p_of2: JournalEntryData = JournalEntryData(
             10, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
                 [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
+        """The offset journal entry to the payable #2."""
         self.j_p_of3: JournalEntryData = JournalEntryData(
             5, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of5d], [self.l_p_of5c])])
+        """The offset journal entry to the payable #3."""
 
         self._add_journal_entry(self.j_r_of1)
         self._add_journal_entry(self.j_r_of2)
         self._add_journal_entry(self.j_r_of3)
         self._add_journal_entry(self.j_p_of1)
         self._add_journal_entry(self.j_p_of2)
         self._add_journal_entry(self.j_p_of3)
```

### Comparing `mia-accounting-1.5.6/tests/test_option.py` & `mia-accounting-1.5.7/tests/test_option.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,46 +21,53 @@
 import unittest
 
 import httpx
 from flask import Flask
 
 from accounting.utils.next_uri import encode_next
 from test_site import db
-from testlib import NEXT_URI, Accounts, create_test_app, get_client
+from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
+    get_csrf_token
 
 PREFIX: str = "/accounting/options"
 """The URL prefix for the option management."""
 
 
 class OptionTestCase(unittest.TestCase):
     """The option test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import Option
             Option.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "admin")
+        self.__client: httpx.Client = get_client(self.__app, "admin")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
-        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        client: httpx.Client = get_client(self.__app, "nobody")
+        csrf_token: str = get_csrf_token(client)
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
         response = client.get(detail_uri)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(edit_uri)
@@ -70,17 +77,18 @@
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
-        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        client: httpx.Client = get_client(self.__app, "viewer")
+        csrf_token: str = get_csrf_token(client)
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
         response = client.get(detail_uri)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(edit_uri)
@@ -90,17 +98,18 @@
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "editor")
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
-        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        client: httpx.Client = get_client(self.__app, "editor")
+        csrf_token: str = get_csrf_token(client)
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
         response = client.get(detail_uri)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(edit_uri)
@@ -110,152 +119,152 @@
         self.assertEqual(response.status_code, 403)
 
     def test_admin(self) -> None:
         """Test the permission as administrator.
 
         :return: None.
         """
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
-        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
-        response = self.client.get(detail_uri)
+        response = self.__client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(edit_uri)
+        response = self.__client.get(edit_uri)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(update_uri, data=self.__get_form())
+        response = self.__client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
     def test_set(self) -> None:
         """Test to set the options.
 
         :return: None.
         """
         from accounting.utils.options import options
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
-        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         form: dict[str, str]
         response: httpx.Response
 
         # Empty currency code
         form = self.__get_form()
         form["default_currency_code"] = " "
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing currency code
         form = self.__get_form()
         form["default_currency_code"] = "ZZZ"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Empty current account
         form = self.__get_form()
         form["default_ie_account_code"] = " "
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing current account
         form = self.__get_form()
         form["default_ie_account_code"] = "9999-999"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not a current account
         form = self.__get_form()
         form["default_ie_account_code"] = Accounts.MEAL
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item name empty
         form = self.__get_form()
         key = [x for x in form if x.endswith("-name")][0]
         form[key] = " "
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item account empty
         form = self.__get_form()
         key = [x for x in form if x.endswith("-account_code")][0]
         form[key] = " "
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item non-expense account
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-expense-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.SERVICE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item non-income account
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-income-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.UTILITIES
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item payable expense
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-expense-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.PAYABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item receivable income
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-income-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.RECEIVABLE
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item description template empty
         form = self.__get_form()
         key = [x for x in form if x.endswith("-description_template")][0]
         form[key] = " "
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success, with malformed order
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(options.default_currency_code, "USD")
             self.assertEqual(options.default_ie_account_code, "1111-001")
             self.assertEqual(len(options.recurring.expenses), 0)
             self.assertEqual(len(options.recurring.incomes), 0)
 
-        response = self.client.post(update_uri, data=self.__get_form())
+        response = self.__client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(options.default_currency_code, "EUR")
             self.assertEqual(options.default_ie_account_code, "0000-000")
             self.assertEqual(len(options.recurring.expenses), 4)
             self.assertEqual(options.recurring.expenses[0].account_code,
                              Accounts.INSURANCE)
             self.assertEqual(options.recurring.expenses[1].account_code,
                              Accounts.POSTAGE)
@@ -268,125 +277,125 @@
                              Accounts.SERVICE)
             self.assertEqual(options.recurring.incomes[1].account_code,
                              Accounts.DONATION)
 
         # Success, with no recurring data
         form = self.__get_form()
         form = {x: form[x] for x in form if not x.startswith("recurring-")}
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             self.assertEqual(len(options.recurring.expenses), 0)
             self.assertEqual(len(options.recurring.incomes), 0)
 
     def test_update_not_modified(self) -> None:
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import Option
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         form: dict[str, str]
         option: Option | None
         resource: httpx.Response
 
-        response = self.client.post(update_uri, data=self.__get_form())
+        response = self.__client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             timestamp: dt.datetime \
                 = option.created_at - dt.timedelta(seconds=5)
             option.created_at = timestamp
             option.updated_at = timestamp
             db.session.commit()
 
         # The recurring setting was not modified
         form = self.__get_form()
         form["default_currency_code"] = "JPY"
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             self.assertEqual(option.created_at, timestamp)
             self.assertEqual(option.updated_at, timestamp)
 
         # The recurring setting was modified
         form = self.__get_form()
         key: str = [x for x in form
                     if x.startswith("recurring-expense-")
                     and x.endswith("-account_code")][0]
         form[key] = Accounts.MEAL
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             self.assertLess(option.created_at, option.updated_at)
 
     def test_created_updated_by(self) -> None:
         """Tests the created-by and updated-by record.
 
         :return: None.
         """
         from accounting.models import Option
         from accounting.utils.user import get_user_pk
         admin_username, editor_username = "admin", "editor"
-        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        detail_uri: str = f"{PREFIX}?next={self.__encoded_next_uri}"
         update_uri: str = f"{PREFIX}/update"
         option: Option | None
         response: httpx.Response
 
-        response = self.client.post(update_uri, data=self.__get_form())
+        response = self.__client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             editor_pk: int = get_user_pk(editor_username)
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             option.created_by_id = editor_pk
             option.updated_by_id = editor_pk
             db.session.commit()
 
         form: dict[str, str] = self.__get_form()
         key: str = [x for x in form
                     if x.startswith("recurring-expense-")
                     and x.endswith("-account_code")][0]
         form[key] = Accounts.MEAL
-        response = self.client.post(update_uri, data=form)
+        response = self.__client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             self.assertEqual(option.created_by.username, editor_username)
             self.assertEqual(option.updated_by.username, admin_username)
 
     def __get_form(self, csrf_token: str | None = None) -> dict[str, str]:
         """Returns the option form.
 
         :param csrf_token: The CSRF token.
         :return: The option form.
         """
         if csrf_token is None:
-            csrf_token = self.csrf_token
+            csrf_token = self.__csrf_token
         return {"csrf_token": csrf_token,
-                "next": self.encoded_next_uri,
+                "next": self.__encoded_next_uri,
                 "default_currency_code": "EUR",
                 "default_ie_account_code": "0000-000",
                 "recurring-expense-1-name": "Water bill",
                 "recurring-expense-1-account_code": Accounts.UTILITIES,
                 "recurring-expense-1-description_template":
                     "Water bill for {last_bimonthly_name}",
                 "recurring-expense-3-no": "16",
```

### Comparing `mia-accounting-1.5.6/tests/test_report.py` & `mia-accounting-1.5.7/tests/test_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import datetime as dt
 import unittest
 
 import httpx
 from flask import Flask
 
 from test_site.lib import BaseTestData
-from testlib import create_test_app, get_client, Accounts
+from testlib import create_test_app, get_client, get_csrf_token, Accounts
 
 PREFIX: str = "/accounting"
 """The URL prefix for the reports."""
 CSV_MIME: str = "text/csv; charset=utf-8"
 """The MIME type of the downloaded CSV files."""
 
 
@@ -37,30 +37,34 @@
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
-        ReportTestData(self.app, "editor").populate()
+        client: httpx.Client = get_client(self.__app, "nobody")
+        ReportTestData(self.__app, "editor").populate()
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 403)
@@ -142,16 +146,16 @@
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
-        ReportTestData(self.app, "editor").populate()
+        client: httpx.Client = get_client(self.__app, "viewer")
+        ReportTestData(self.__app, "editor").populate()
         response: httpx.Response
 
         response = client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
         response = client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 200)
@@ -244,204 +248,204 @@
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        ReportTestData(self.app, "editor").populate()
+        ReportTestData(self.__app, "editor").populate()
         response: httpx.Response
 
-        response = self.client.get(PREFIX)
+        response = self.__client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}?as=csv")
+        response = self.__client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/journal")
+        response = self.__client.get(f"{PREFIX}/journal")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/journal?as=csv")
+        response = self.__client.get(f"{PREFIX}/journal?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/ledger")
+        response = self.__client.get(f"{PREFIX}/ledger")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/ledger?as=csv")
+        response = self.__client.get(f"{PREFIX}/ledger?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/income-expenses")
+        response = self.__client.get(f"{PREFIX}/income-expenses")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/income-expenses?as=csv")
+        response = self.__client.get(f"{PREFIX}/income-expenses?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/trial-balance")
+        response = self.__client.get(f"{PREFIX}/trial-balance")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/trial-balance?as=csv")
+        response = self.__client.get(f"{PREFIX}/trial-balance?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/income-statement")
+        response = self.__client.get(f"{PREFIX}/income-statement")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/income-statement?as=csv")
+        response = self.__client.get(f"{PREFIX}/income-statement?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/balance-sheet")
+        response = self.__client.get(f"{PREFIX}/balance-sheet")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/balance-sheet?as=csv")
+        response = self.__client.get(f"{PREFIX}/balance-sheet?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/unapplied")
+        response = self.__client.get(f"{PREFIX}/unapplied")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/unapplied?as=csv")
+        response = self.__client.get(f"{PREFIX}/unapplied?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/unmatched")
+        response = self.__client.get(f"{PREFIX}/unmatched")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/unmatched?as=csv")
+        response = self.__client.get(f"{PREFIX}/unmatched?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/search?q=Salary")
+        response = self.__client.get(f"{PREFIX}/search?q=Salary")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/search?q=Salary&as=csv")
+        response = self.__client.get(f"{PREFIX}/search?q=Salary&as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/search?q=薪水")
+        response = self.__client.get(f"{PREFIX}/search?q=薪水")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/search?q=薪水&as=csv")
+        response = self.__client.get(f"{PREFIX}/search?q=薪水&as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
     def test_empty_db(self) -> None:
         """Tests the empty database.
 
         :return: None.
         """
         response: httpx.Response
 
-        response = self.client.get(PREFIX)
+        response = self.__client.get(PREFIX)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}?as=csv")
+        response = self.__client.get(f"{PREFIX}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/journal")
+        response = self.__client.get(f"{PREFIX}/journal")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/journal?as=csv")
+        response = self.__client.get(f"{PREFIX}/journal?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/ledger")
+        response = self.__client.get(f"{PREFIX}/ledger")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/ledger?as=csv")
+        response = self.__client.get(f"{PREFIX}/ledger?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/income-expenses")
+        response = self.__client.get(f"{PREFIX}/income-expenses")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/income-expenses?as=csv")
+        response = self.__client.get(f"{PREFIX}/income-expenses?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/trial-balance")
+        response = self.__client.get(f"{PREFIX}/trial-balance")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/trial-balance?as=csv")
+        response = self.__client.get(f"{PREFIX}/trial-balance?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/income-statement")
+        response = self.__client.get(f"{PREFIX}/income-statement")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/income-statement?as=csv")
+        response = self.__client.get(f"{PREFIX}/income-statement?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/balance-sheet")
+        response = self.__client.get(f"{PREFIX}/balance-sheet")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/balance-sheet?as=csv")
+        response = self.__client.get(f"{PREFIX}/balance-sheet?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/unapplied")
+        response = self.__client.get(f"{PREFIX}/unapplied")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/unapplied?as=csv")
+        response = self.__client.get(f"{PREFIX}/unapplied?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/unmatched")
+        response = self.__client.get(f"{PREFIX}/unmatched")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/unmatched?as=csv")
+        response = self.__client.get(f"{PREFIX}/unmatched?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(
+        response = self.__client.get(
             f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/search?q=Salary")
+        response = self.__client.get(f"{PREFIX}/search?q=Salary")
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(f"{PREFIX}/search?q=Salary&as=csv")
+        response = self.__client.get(f"{PREFIX}/search?q=Salary&as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
 
 class ReportTestData(BaseTestData):
     """The report test data."""
```

### Comparing `mia-accounting-1.5.6/tests/test_site/__init__.py` & `mia-accounting-1.5.7/tests/test_site/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,21 @@
 """
 import os
 from secrets import token_urlsafe
 from typing import Type
 
 from click.testing import Result
 from flask import Flask, Blueprint, render_template, redirect, Response, \
-    url_for, request
+    url_for
 from flask.testing import FlaskCliRunner
 from flask_babel_js import BabelJS
 from flask_sqlalchemy import SQLAlchemy
 from flask_wtf import CSRFProtect
 from sqlalchemy import Column
 
-from accounting.utils.next_uri import encode_next
-
 bp: Blueprint = Blueprint("home", __name__)
 """The global blueprint."""
 babel_js: BabelJS = BabelJS()
 """The Babel JavaScript instance."""
 csrf: CSRFProtect = CSRFProtect()
 """The CSRF protector."""
 db: SQLAlchemy = SQLAlchemy()
```

### Comparing `mia-accounting-1.5.6/tests/test_site/auth.py` & `mia-accounting-1.5.7/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/tests/test_site/lib.py` & `mia-accounting-1.5.7/tests/test_site/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,21 +53,28 @@
 
         :param account: The account code.
         :param description: The description.
         :param amount: The amount.
         :param original_line_item: The original journal entry line item.
         """
         self.journal_entry: JournalEntryData | None = None
+        """The journal entry data."""
         self.id: int = -1
+        """The journal entry line item ID."""
         self.no: int = -1
+        """The line item number under the journal entry and debit or credit."""
         self.original_line_item: JournalEntryLineItemData | None \
             = original_line_item
+        """The original journal entry line item."""
         self.account: str = account
+        """The account code."""
         self.description: str | None = description
+        """The description."""
         self.amount: Decimal = Decimal(amount)
+        """The amount."""
 
     def form(self, prefix: str, debit_credit: str, index: int,
              is_update: bool) -> dict[str, str]:
         """Returns the line item as form data.
 
         :param prefix: The prefix of the form fields.
         :param debit_credit: Either "debit" or "credit".
@@ -97,16 +104,19 @@
         """Constructs the journal entry currency data.
 
         :param currency: The currency code.
         :param debit: The debit line items.
         :param credit: The credit line items.
         """
         self.code: str = currency
+        """The currency code."""
         self.debit: list[JournalEntryLineItemData] = debit
+        """The debit line items."""
         self.credit: list[JournalEntryLineItemData] = credit
+        """The credit line items."""
 
     def form(self, index: int, is_update: bool) -> dict[str, str]:
         """Returns the currency as form data.
 
         :param index: The currency index.
         :param is_update: True for an update operation, or False otherwise
         :return: The form data.
@@ -127,17 +137,21 @@
     def __init__(self, days: int, currencies: list[JournalEntryCurrencyData]):
         """Constructs a journal entry.
 
         :param days: The number of days before today.
         :param currencies: The journal entry currency data.
         """
         self.id: int = -1
+        """The journal entry ID."""
         self.days: int = days
+        """The number of days before today."""
         self.currencies: list[JournalEntryCurrencyData] = currencies
+        """The journal entry currency data."""
         self.note: str | None = None
+        """The note."""
         for currency in self.currencies:
             for line_item in currency.debit:
                 line_item.journal_entry = self
             for line_item in currency.credit:
                 line_item.journal_entry = self
 
     def new_form(self, csrf_token: str, encoded_next_uri: str) \
@@ -186,21 +200,25 @@
     def __init__(self, app: Flask, username: str):
         """Constructs the test data.
 
         :param app: The Flask application.
         :param username: The username.
         """
         self._app: Flask = app
+        """The Flask application."""
         with self._app.app_context():
             current_user: User | None = User.query\
                 .filter(User.username == username).first()
             assert current_user is not None
             self.__current_user_id: int = current_user.id
+            """The current user ID."""
             self.__journal_entries: list[dict[str, Any]] = []
+            """The data of the journal entries."""
             self.__line_items: list[dict[str, Any]] = []
+            """The data of the journal entry line items."""
             self._init_data()
 
     @abstractmethod
     def _init_data(self) -> None:
         """Initializes the test data.
 
         :return: None
```

### Comparing `mia-accounting-1.5.6/tests/test_site/locale.py` & `mia-accounting-1.5.7/tests/test_site/locale.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     redirect, Flask
 from flask_babel import Babel
 from werkzeug.datastructures import LanguageAccept
 
 from accounting.utils.next_uri import or_next
 
 bp: Blueprint = Blueprint("locale", __name__, url_prefix="/")
+"""The blueprint for the localization."""
 
 
 def get_locale():
     """Returns the locale of the user
 
     :return: The locale of the user.
     """
```

### Comparing `mia-accounting-1.5.6/tests/test_site/reset.py` & `mia-accounting-1.5.7/tests/test_site/reset.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from . import db
 from .auth import admin_required
 from .lib import Accounts, JournalEntryLineItemData, JournalEntryData, \
     JournalEntryCurrencyData, BaseTestData
 
 bp: Blueprint = Blueprint("reset", __name__, url_prefix="/")
+"""The blueprint for the data reset."""
 
 
 @bp.get("reset", endpoint="reset-page")
 @admin_required
 def reset() -> str:
     """Resets the sample data.
```

### Comparing `mia-accounting-1.5.6/tests/test_site/static/favicon.svg` & `mia-accounting-1.5.7/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/tests/test_site/templates/base.html` & `mia-accounting-1.5.7/tests/test_site/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 
 <nav class="navbar navbar-expand-lg bg-body-tertiary bg-dark navbar-dark">
   <div class="container-fluid">
     <a class="navbar-brand" href="{{ url_for("home.home") }}">
       <i class="fa-solid fa-house"></i>
       {{ _("Home") }}
     </a>
-    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#collapsible-navbar" aria-controls="collapsible-navbar" aria-expanded="false" aria-label="Toggle navigation">
+    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#accounting-collapsible-navbar" aria-controls="accounting-collapsible-navbar" aria-expanded="false" aria-label="Toggle navigation">
       <span class="navbar-toggler-icon"></span>
     </button>
 
-    <div id="collapsible-navbar" class="collapse navbar-collapse">
+    <div id="accounting-collapsible-navbar" class="collapse navbar-collapse">
       <ul class="navbar-nav me-auto mb-2 mb-lg-0">
         {% include "accounting/include/nav.html" %}
       </ul>
 
       <!-- The right side -->
       <ul class="navbar-nav d-flex">
         {% if current_user() is not none %}
```

### Comparing `mia-accounting-1.5.6/tests/test_site/templates/home.html` & `mia-accounting-1.5.7/tests/test_site/templates/home.html`

 * *Files 10% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 #}
 {% extends "base.html" %}
 
 {% block header %}{% block title %}{{ _("Mia! Accounting Live Demonstration") }}{% endblock %}{% endblock %}
 
 {% block content %}
 
-<p>{{ _("This is the live demonstration of the Mia! Accounting project.  Please <a href=\"/login?next=%%2Faccounting\">log in</a> to continue.") }}</p>
+<p>{{ _("This is the live demonstration of the Mia! Accounting project.  Please <a href=\"%(url)s\">log in</a> to continue.", url=url_for("auth.login")) }}</p>
 
 <p>{{ _("You may also want to check the <a href=\"https://mia-accounting.readthedocs.io\">full documentation</a> and the <a href=\"https://github.com/imacat/mia-accounting\">Github repository</a>.") }}</p>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -7,11 +7,11 @@
 WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 License for the specific language governing permissions and limitations under
 the License. Author: imacat@mail.imacat.idv.tw (imacat) First written: 2023/1/
 27 #} {% extends "base.html" %} {% block header %}{% block title %}{{ _("Mia!
 Accounting Live Demonstration") }}{% endblock %}{% endblock %} {% block content
 %}
 {{ _("This is the live demonstration of the Mia! Accounting project. Please log
-in to continue.") }}
+in to continue.", url=url_for("auth.login")) }}
 {{ _("You may also want to check the full_documentation and the Github
 repository.") }}
 {% endblock %}
```

### Comparing `mia-accounting-1.5.6/tests/test_site/templates/login.html` & `mia-accounting-1.5.7/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/tests/test_site/templates/reset.html` & `mia-accounting-1.5.7/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.6/tests/test_site/translations/messages.pot` & `mia-accounting-1.5.7/tests/test_site/translations/messages.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-12 17:59+0800\n"
+"POT-Creation-Date: 2023-06-10 10:42+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: tests/test_site/reset.py:55
 msgid "The sample data are emptied and reset successfully."
 msgstr ""
 
-#: tests/test_site/reset.py:68
+#: tests/test_site/reset.py:69
 msgid "The database is emptied successfully."
 msgstr ""
 
 #: tests/test_site/templates/base.html:23
 msgid "en"
 msgstr ""
 
@@ -54,15 +54,15 @@
 msgid "Mia! Accounting Live Demonstration"
 msgstr ""
 
 #: tests/test_site/templates/home.html:28
 #, python-format
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a"
-" href=\"/login?next=%%2Faccounting\">log in</a> to continue."
+" href=\"%(url)s\">log in</a> to continue."
 msgstr ""
 
 #: tests/test_site/templates/home.html:30
 msgid ""
 "You may also want to check the <a href=\"https://mia-"
 "accounting.readthedocs.io\">full documentation</a> and the <a "
 "href=\"https://github.com/imacat/mia-accounting\">Github repository</a>."
```

### Comparing `mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.7/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-12 17:59+0800\n"
-"PO-Revision-Date: 2023-04-12 18:00+0800\n"
+"POT-Creation-Date: 2023-06-10 10:42+0800\n"
+"PO-Revision-Date: 2023-06-10 10:43+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -58,18 +58,16 @@
 msgstr "数据库已清空。"
 
 msgid "The sample data are emptied and reset successfully."
 msgstr "范例数据已清空重设。"
 
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a "
-"href=\"/login?next=%%2Faccounting\">log in</a> to continue."
-msgstr ""
-"这是 Mia! Accounting 项目的示范站。请先<a href=\"/login?next=%"
-"%2Faccounting\">登录</a>。"
+"href=\"%(url)s\">log in</a> to continue."
+msgstr "这是 Mia! Accounting 项目的示范站。请先<a href=\"%(url)s\">登录</a>。"
 
 msgid "Viewer"
 msgstr "读报表者"
 
 msgid ""
 "Warning: All the current accounting data will be deleted.  This cannot be "
 "undone.  Please backup your database first."
```

### Comparing `mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.5.7/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-12 17:59+0800\n"
-"PO-Revision-Date: 2023-04-12 18:00+0800\n"
+"POT-Creation-Date: 2023-06-10 10:42+0800\n"
+"PO-Revision-Date: 2023-06-10 10:43+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: tests/test_site/reset.py:55
 msgid "The sample data are emptied and reset successfully."
 msgstr "范例数据已清空重设。"
 
-#: tests/test_site/reset.py:68
+#: tests/test_site/reset.py:69
 msgid "The database is emptied successfully."
 msgstr "数据库已清空。"
 
 #: tests/test_site/templates/base.html:23
 msgid "en"
 msgstr "zh-Hans"
 
@@ -57,16 +57,16 @@
 msgid "Mia! Accounting Live Demonstration"
 msgstr "Mia! Accounting 示范站"
 
 #: tests/test_site/templates/home.html:28
 #, python-format
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a"
-" href=\"/login?next=%%2Faccounting\">log in</a> to continue."
-msgstr "这是 Mia! Accounting 项目的示范站。请先<a href=\"/login?next=%%2Faccounting\">登录</a>。"
+" href=\"%(url)s\">log in</a> to continue."
+msgstr "这是 Mia! Accounting 项目的示范站。请先<a href=\"%(url)s\">登录</a>。"
 
 #: tests/test_site/templates/home.html:30
 msgid ""
 "You may also want to check the <a href=\"https://mia-"
 "accounting.readthedocs.io\">full documentation</a> and the <a "
 "href=\"https://github.com/imacat/mia-accounting\">Github repository</a>."
 msgstr ""
```

### Comparing `mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.7/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-12 17:59+0800\n"
-"PO-Revision-Date: 2023-04-12 18:00+0800\n"
+"POT-Creation-Date: 2023-06-10 10:42+0800\n"
+"PO-Revision-Date: 2023-06-10 10:43+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -58,18 +58,16 @@
 msgstr "資料庫已清空。"
 
 msgid "The sample data are emptied and reset successfully."
 msgstr "範例資料已清空重設。"
 
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a "
-"href=\"/login?next=%%2Faccounting\">log in</a> to continue."
-msgstr ""
-"這是 Mia! Accounting 專案的示範站。請先<a href=\"/login?next=%"
-"%2Faccounting\">登入</a>。"
+"href=\"%(url)s\">log in</a> to continue."
+msgstr "這是 Mia! Accounting 專案的示範站。請先<a href=\"%(url)s\">登入</a>。"
 
 msgid "Viewer"
 msgstr "讀報表者"
 
 msgid ""
 "Warning: All the current accounting data will be deleted.  This cannot be "
 "undone.  Please backup your database first."
```

### Comparing `mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.5.7/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: mia-accounting-test-site 1.0.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-12 17:59+0800\n"
-"PO-Revision-Date: 2023-04-12 18:00+0800\n"
+"POT-Creation-Date: 2023-06-10 10:42+0800\n"
+"PO-Revision-Date: 2023-06-10 10:43+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: tests/test_site/reset.py:55
 msgid "The sample data are emptied and reset successfully."
 msgstr "範例資料已清空重設。"
 
-#: tests/test_site/reset.py:68
+#: tests/test_site/reset.py:69
 msgid "The database is emptied successfully."
 msgstr "資料庫已清空。"
 
 #: tests/test_site/templates/base.html:23
 msgid "en"
 msgstr "zh-Hant"
 
@@ -57,16 +57,16 @@
 msgid "Mia! Accounting Live Demonstration"
 msgstr "Mia! Accounting 示範站"
 
 #: tests/test_site/templates/home.html:28
 #, python-format
 msgid ""
 "This is the live demonstration of the Mia! Accounting project.  Please <a"
-" href=\"/login?next=%%2Faccounting\">log in</a> to continue."
-msgstr "這是 Mia! Accounting 專案的示範站。請先<a href=\"/login?next=%%2Faccounting\">登入</a>。"
+" href=\"%(url)s\">log in</a> to continue."
+msgstr "這是 Mia! Accounting 專案的示範站。請先<a href=\"%(url)s\">登入</a>。"
 
 #: tests/test_site/templates/home.html:30
 msgid ""
 "You may also want to check the <a href=\"https://mia-"
 "accounting.readthedocs.io\">full documentation</a> and the <a "
 "href=\"https://github.com/imacat/mia-accounting\">Github repository</a>."
 msgstr ""
```

### Comparing `mia-accounting-1.5.6/tests/test_unmatched_offset.py` & `mia-accounting-1.5.7/tests/test_unmatched_offset.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,117 +22,125 @@
 import httpx
 from flask import Flask
 
 from accounting.utils.next_uri import encode_next
 from test_site import db
 from test_site.lib import JournalEntryCurrencyData, JournalEntryData, \
     BaseTestData
-from testlib import NEXT_URI, create_test_app, get_client, Accounts
+from testlib import NEXT_URI, create_test_app, get_client, get_csrf_token, \
+    Accounts
 
 PREFIX: str = "/accounting/match-offsets/USD"
 """The URL prefix for the unmatched offset management."""
 
 
 class UnmatchedOffsetTestCase(unittest.TestCase):
     """The unmatched offset test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
-        with self.app.app_context():
+        with self.__app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
-            self.encoded_next_uri: str = encode_next(NEXT_URI)
+            self.__encoded_next_uri: str = encode_next(NEXT_URI)
+            """The encoded next URI."""
 
-        self.client, self.csrf_token = get_client(self.app, "editor")
+        self.__client: httpx.Client = get_client(self.__app, "editor")
+        """The user client."""
+        self.__csrf_token: str = get_csrf_token(self.__client)
+        """The CSRF token."""
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "nobody")
-        DifferentTestData(self.app, "nobody").populate()
+        client: httpx.Client = get_client(self.__app, "nobody")
+        csrf_token: str = get_csrf_token(client)
+        DifferentTestData(self.__app, "nobody").populate()
         response: httpx.Response
 
         response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
                                data={"csrf_token": csrf_token,
-                                     "next": self.encoded_next_uri})
+                                     "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
-        client, csrf_token = get_client(self.app, "viewer")
-        DifferentTestData(self.app, "viewer").populate()
+        client: httpx.Client = get_client(self.__app, "viewer")
+        csrf_token: str = get_csrf_token(client)
+        DifferentTestData(self.__app, "viewer").populate()
         response: httpx.Response
 
         response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
                                data={"csrf_token": csrf_token,
-                                     "next": self.encoded_next_uri})
+                                     "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
-        DifferentTestData(self.app, "editor").populate()
+        DifferentTestData(self.__app, "editor").populate()
         response: httpx.Response
 
-        response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(f"{PREFIX}/{Accounts.PAYABLE}",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_empty_db(self) -> None:
         """Test the empty database.
 
         :return: None.
         """
         response: httpx.Response
 
-        response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(f"{PREFIX}/{Accounts.PAYABLE}",
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_different(self) -> None:
         """Tests to match against different descriptions and amounts.
 
         :return: None.
         """
         from accounting.models import Currency, Account, JournalEntryLineItem
         from accounting.report.utils.offset_matcher import OffsetMatcher
         from accounting.template_globals import default_currency_code
-        data: DifferentTestData = DifferentTestData(self.app, "editor")
+        data: DifferentTestData = DifferentTestData(self.__app, "editor")
         data.populate()
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
         match_uri: str
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             currency: Currency | None \
                 = db.session.get(Currency, default_currency_code())
             assert currency is not None
 
         # The receivables
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or1d.id, data.l_r_or2d.id,
                               data.l_r_or3d.id, data.l_r_or4d.id})
             self.assertEqual({x.id for x in matcher.unmatched},
@@ -146,21 +154,21 @@
                                  data.l_r_of3c.id, data.l_r_of4c.id,
                                  data.l_r_of5c.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
         match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
-        response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(match_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or1d.id, data.l_r_or2d.id,
                               data.l_r_or3d.id})
             self.assertEqual({x.id for x in matcher.unmatched},
@@ -174,15 +182,15 @@
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of5c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or4d.id)
 
         # The payables
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or1c.id, data.l_p_or2c.id,
                               data.l_p_or3c.id, data.l_p_or4c.id})
             self.assertEqual({x.id for x in matcher.unmatched},
@@ -196,21 +204,21 @@
                                  data.l_p_of3d.id, data.l_p_of4d.id,
                                  data.l_p_of5d.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
         match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
-        response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(match_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or1c.id, data.l_p_or2c.id,
                               data.l_p_or3c.id})
             self.assertEqual({x.id for x in matcher.unmatched},
@@ -231,29 +239,29 @@
         """Tests to match against same descriptions and amounts.
 
         :return: None.
         """
         from accounting.models import Currency, Account, JournalEntryLineItem
         from accounting.report.utils.offset_matcher import OffsetMatcher
         from accounting.template_globals import default_currency_code
-        data: SameTestData = SameTestData(self.app, "editor")
+        data: SameTestData = SameTestData(self.__app, "editor")
         data.populate()
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
         match_uri: str
         response: httpx.Response
 
-        with self.app.app_context():
+        with self.__app.app_context():
             currency: Currency | None \
                 = db.session.get(Currency, default_currency_code())
             assert currency is not None
 
         # The receivables
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or1d.id, data.l_r_or3d.id,
                               data.l_r_or4d.id, data.l_r_or5d.id,
                               data.l_r_or6d.id})
@@ -274,21 +282,21 @@
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of3c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or2d.id)
 
         match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
-        response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(match_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or5d.id, data.l_r_or6d.id})
             self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_r_of1c.id, data.l_r_of5c.id})
@@ -311,15 +319,15 @@
             self.assertEqual(line_item.original_line_item_id, data.l_r_or3d.id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of6c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or4d.id)
 
         # The payables
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or1c.id, data.l_p_or3c.id,
                               data.l_p_or4c.id, data.l_p_or5c.id,
                               data.l_p_or6c.id})
@@ -340,21 +348,21 @@
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_p_of3d.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_p_or2c.id)
 
         match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
-        response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token,
-                                          "next": self.encoded_next_uri})
+        response = self.__client.post(match_uri,
+                                      data={"csrf_token": self.__csrf_token,
+                                            "next": self.__encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
-        with self.app.app_context():
+        with self.__app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or5c.id, data.l_p_or6c.id})
             self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_p_of1d.id, data.l_p_of5d.id})
@@ -406,26 +414,30 @@
             "Envelop", "0.9", Accounts.OFFICE, Accounts.PAYABLE)
 
         # Original journal entries
         self.j_r_or1: JournalEntryData = JournalEntryData(
             50, [JournalEntryCurrencyData(
                 "USD", [self.l_r_or1d, self.l_r_or4d],
                 [self.l_r_or1c, self.l_r_or4c])])
+        """The receivable original journal entry #1."""
         self.j_r_or2: JournalEntryData = JournalEntryData(
             30, [JournalEntryCurrencyData(
                 "USD", [self.l_r_or2d, self.l_r_or3d],
                 [self.l_r_or2c, self.l_r_or3c])])
+        """The receivable original journal entry #2"""
         self.j_p_or1: JournalEntryData = JournalEntryData(
             40, [JournalEntryCurrencyData(
                 "USD", [self.l_p_or1d, self.l_p_or4d],
                 [self.l_p_or1c, self.l_p_or4c])])
+        """The payable original journal entry #1."""
         self.j_p_or2: JournalEntryData = JournalEntryData(
             20, [JournalEntryCurrencyData(
                 "USD", [self.l_p_or2d, self.l_p_or3d],
                 [self.l_p_or2c, self.l_p_or3c])])
+        """The payable original journal entry #2."""
 
         self._add_journal_entry(self.j_r_or1)
         self._add_journal_entry(self.j_r_or2)
         self._add_journal_entry(self.j_p_or1)
         self._add_journal_entry(self.j_p_or2)
 
         # Receivable offset items
@@ -452,31 +464,37 @@
         self.l_p_of5d, self.l_p_of5c = self._couple(
             "Envelop", "0.9", Accounts.PAYABLE, Accounts.CASH)
 
         # Offset journal entries
         self.j_r_of1: JournalEntryData = JournalEntryData(
             25, [JournalEntryCurrencyData(
                 "USD", [self.l_r_of1d], [self.l_r_of1c])])
+        """The offset journal entry to the receivable #1."""
         self.j_r_of2: JournalEntryData = JournalEntryData(
             20, [JournalEntryCurrencyData(
                 "USD", [self.l_r_of2d, self.l_r_of3d, self.l_r_of4d],
                 [self.l_r_of2c, self.l_r_of3c, self.l_r_of4c])])
+        """The offset journal entry to the receivable #2."""
         self.j_r_of3: JournalEntryData = JournalEntryData(
             15, [JournalEntryCurrencyData(
                 "USD", [self.l_r_of5d], [self.l_r_of5c])])
+        """The offset journal entry to the receivable #3."""
         self.j_p_of1: JournalEntryData = JournalEntryData(
             15, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of1d], [self.l_p_of1c])])
+        """The offset journal entry to the payable #1."""
         self.j_p_of2: JournalEntryData = JournalEntryData(
             10, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of2d, self.l_p_of3d, self.l_p_of4d],
                 [self.l_p_of2c, self.l_p_of3c, self.l_p_of4c])])
+        """The offset journal entry to the payable #2."""
         self.j_p_of3: JournalEntryData = JournalEntryData(
             5, [JournalEntryCurrencyData(
                 "USD", [self.l_p_of5d], [self.l_p_of5c])])
+        """The offset journal entry to the payable #3."""
 
         self._add_journal_entry(self.j_r_of1)
         self._add_journal_entry(self.j_r_of2)
         self._add_journal_entry(self.j_r_of3)
         self._add_journal_entry(self.j_p_of1)
         self._add_journal_entry(self.j_p_of2)
         self._add_journal_entry(self.j_p_of3)
```

### Comparing `mia-accounting-1.5.6/tests/test_utils.py` & `mia-accounting-1.5.7/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 """
 import unittest
 from urllib.parse import quote_plus
 
 import httpx
 from flask import Flask, request
-from itsdangerous import URLSafeSerializer
 
-from accounting.utils.next_uri import append_next, inherit_next, or_next
+from accounting.utils.next_uri import append_next, inherit_next, or_next, \
+    encode_next, decode_next
 from accounting.utils.pagination import Pagination, DEFAULT_PAGE_SIZE
 from accounting.utils.query import parse_query_keywords
 from testlib import TEST_SERVER, create_test_app, get_csrf_token, NEXT_URI
 
 
 class NextUriTestCase(unittest.TestCase):
     """The test case for the next URI utilities."""
@@ -36,44 +36,49 @@
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
-        self.serializer: URLSafeSerializer \
-            = URLSafeSerializer(self.app.config["SECRET_KEY"])
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
 
     def test_next_uri(self) -> None:
         """Tests the next URI utilities with the next URI.
 
         :return: None.
         """
         def test_next_uri_view() -> str:
             """The test view with the next URI."""
             current_uri: str = request.full_path if request.query_string \
                 else request.path
+            with self.__app.app_context():
+                encoded_current: str = encode_next(current_uri)
             self.assertEqual(append_next(self.TARGET),
-                             f"{self.TARGET}?next={self.__encode(current_uri)}")
-            next_uri: str = request.form["next"] if request.method == "POST" \
-                else request.args["next"]
+                             f"{self.TARGET}?next={encoded_current}")
+            encoded_next_uri: str = request.form["next"] \
+                if request.method == "POST" else request.args["next"]
             self.assertEqual(inherit_next(self.TARGET),
-                             f"{self.TARGET}?next={next_uri}")
-            self.assertEqual(or_next(self.TARGET), self.__decode(next_uri))
+                             f"{self.TARGET}?next={encoded_next_uri}")
+            with self.__app.app_context():
+                next_uri: str = decode_next(encoded_next_uri)
+            self.assertEqual(or_next(self.TARGET), next_uri)
             return ""
 
-        self.app.add_url_rule("/test-next", view_func=test_next_uri_view,
-                              methods=["GET", "POST"])
-        client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
+        self.__app.add_url_rule("/test-next", view_func=test_next_uri_view,
+                                methods=["GET", "POST"])
+        client: httpx.Client = httpx.Client(app=self.__app,
+                                            base_url=TEST_SERVER)
         client.headers["Referer"] = TEST_SERVER
         csrf_token: str = get_csrf_token(client)
         response: httpx.Response
 
-        encoded_uri: str = self.__encode(NEXT_URI)
+        with self.__app.app_context():
+            encoded_uri: str = encode_next(NEXT_URI)
         response = client.get(f"/test-next?next={encoded_uri}&q=abc&page-no=4")
         self.assertEqual(response.status_code, 200)
         response = client.post("/test-next", data={"csrf_token": csrf_token,
                                                    "next": encoded_uri,
                                                    "name": "viewer"})
         self.assertEqual(response.status_code, 200)
 
@@ -84,17 +89,19 @@
         """
         def test_no_next_uri_view() -> str:
             """The test view without the next URI."""
             self.assertEqual(inherit_next(self.TARGET), self.TARGET)
             self.assertEqual(or_next(self.TARGET), self.TARGET)
             return ""
 
-        self.app.add_url_rule("/test-no-next", view_func=test_no_next_uri_view,
-                              methods=["GET", "POST"])
-        client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
+        self.__app.add_url_rule("/test-no-next",
+                                view_func=test_no_next_uri_view,
+                                methods=["GET", "POST"])
+        client: httpx.Client = httpx.Client(app=self.__app,
+                                            base_url=TEST_SERVER)
         client.headers["Referer"] = TEST_SERVER
         csrf_token: str = get_csrf_token(client)
         response: httpx.Response
 
         response = client.get("/test-no-next?q=abc&page-no=4")
         self.assertEqual(response.status_code, 200)
         response = client.post("/test-no-next", data={"csrf_token": csrf_token,
@@ -108,18 +115,19 @@
         """
         def test_invalid_next_uri_view() -> str:
             """The test view without the next URI."""
             self.assertEqual(inherit_next(self.TARGET), self.TARGET)
             self.assertEqual(or_next(self.TARGET), self.TARGET)
             return ""
 
-        self.app.add_url_rule("/test-invalid-next",
-                              view_func=test_invalid_next_uri_view,
-                              methods=["GET", "POST"])
-        client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
+        self.__app.add_url_rule("/test-invalid-next",
+                                view_func=test_invalid_next_uri_view,
+                                methods=["GET", "POST"])
+        client: httpx.Client = httpx.Client(app=self.__app,
+                                            base_url=TEST_SERVER)
         client.headers["Referer"] = TEST_SERVER
         csrf_token: str = get_csrf_token(client)
         next_uri: str
         expected1: str
         expected2: str
         response: httpx.Response
 
@@ -128,30 +136,14 @@
         response = client.get(f"/test-invalid-next?next={quote_plus(next_uri)}")
         self.assertEqual(response.status_code, 200)
         response = client.post("/test-invalid-next",
                                data={"csrf_token": csrf_token,
                                      "next": next_uri})
         self.assertEqual(response.status_code, 200)
 
-    def __encode(self, uri: str) -> str:
-        """Encodes the next URI.
-
-        :param uri: The next URI.
-        :return: The encoded next URI.
-        """
-        return self.serializer.dumps(uri, "next")
-
-    def __decode(self, uri: str) -> str:
-        """Decodes the next URI.
-
-        :param uri: The encoded next URI.
-        :return: The next URI.
-        """
-        return self.serializer.loads(uri, "next")
-
 
 class QueryKeywordParserTestCase(unittest.TestCase):
     """The test case for the query keyword parser."""
 
     def test_default(self) -> None:
         """Tests the query keyword parser.
 
@@ -186,54 +178,63 @@
         self.assertEqual(parse_query_keywords(""), [])
 
 
 class PaginationTestCase(unittest.TestCase):
     """The test case for pagination."""
 
     class Params:
-        """The testing parameters."""
+        """The testing pagination parameters."""
 
         def __init__(self, items: list[int], is_reversed: bool | None,
                      result: list[int], is_paged: bool):
             """Constructs the expected pagination.
 
             :param items: All the items in the list.
             :param is_reversed: Whether the default page is the last page.
             :param result: The expected items on the page.
             :param is_paged: Whether we need pagination.
             """
             self.items: list[int] = items
+            """All the items in the list."""
             self.is_reversed: bool | None = is_reversed
+            """Whether the default page is the last page."""
             self.result: list[int] = result
+            """The expected items on the page."""
             self.is_paged: bool = is_paged
+            """Whether we need pagination."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
-        self.app: Flask = create_test_app()
-        self.params = self.Params([], None, [], True)
+        self.__app: Flask = create_test_app()
+        """The Flask application."""
+        self.__params: PaginationTestCase.Params \
+            = self.Params([], None, [], True)
+        """The testing pagination parameters."""
 
-        @self.app.get("/test-pagination")
+        @self.__app.get("/test-pagination")
         def test_pagination_view() -> str:
             """The test view with the pagination."""
             pagination: Pagination
-            if self.params.is_reversed is not None:
+            if self.__params.is_reversed is not None:
                 pagination = Pagination[int](
-                    self.params.items, is_reversed=self.params.is_reversed)
+                    self.__params.items, is_reversed=self.__params.is_reversed)
             else:
-                pagination = Pagination[int](self.params.items)
-            self.assertEqual(pagination.is_paged, self.params.is_paged)
-            self.assertEqual(pagination.list, self.params.result)
+                pagination = Pagination[int](self.__params.items)
+            self.assertEqual(pagination.is_paged, self.__params.is_paged)
+            self.assertEqual(pagination.list, self.__params.result)
             return ""
 
-        self.client = httpx.Client(app=self.app, base_url=TEST_SERVER)
-        self.client.headers["Referer"] = TEST_SERVER
+        self.__client: httpx.Client = httpx.Client(app=self.__app,
+                                                   base_url=TEST_SERVER)
+        """The user client."""
+        self.__client.headers["Referer"] = TEST_SERVER
 
     def __test_success(self, query: str, items: range,
                        result: range, is_paged: bool = True,
                        is_reversed: bool | None = None) -> None:
         """Tests the pagination.
 
         :param query: The query string.
@@ -242,32 +243,32 @@
         :param is_paged: Whether we need pagination.
         :param is_reversed: Whether the list is reversed.
         :return: None.
         """
         target: str = "/test-pagination"
         if query != "":
             target = f"{target}?{query}"
-        self.params = self.Params(list(items), is_reversed,
-                                  list(result), is_paged)
-        response: httpx.Response = self.client.get(target)
+        self.__params = self.Params(list(items), is_reversed,
+                                    list(result), is_paged)
+        response: httpx.Response = self.__client.get(target)
         self.assertEqual(response.status_code, 200)
 
     def __test_malformed(self, query: str, items: range, redirect_to: str,
                          is_reversed: bool | None = None) -> None:
         """Tests the pagination.
 
         :param query: The query string.
         :param items: The original items.
         :param redirect_to: The expected target query of the redirection.
         :param is_reversed: Whether the list is reversed.
         :return: None.
         """
         target: str = "/test-pagination"
-        self.params = self.Params(list(items), is_reversed, [], True)
-        response: httpx.Response = self.client.get(f"{target}?{query}")
+        self.__params = self.Params(list(items), is_reversed, [], True)
+        response: httpx.Response = self.__client.get(f"{target}?{query}")
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{target}?{redirect_to}")
 
     def test_default(self) -> None:
         """Tests the default pagination.
```

### Comparing `mia-accounting-1.5.6/tests/testlib.py` & `mia-accounting-1.5.7/tests/testlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,33 +85,33 @@
 
     :param client: The httpx client.
     :return: The CSRF token.
     """
     return client.get("/.csrf-token").text
 
 
-def get_client(app: Flask, username: str) -> tuple[httpx.Client, str]:
+def get_client(app: Flask, username: str) -> httpx.Client:
     """Returns a user client.
 
     :param app: The Flask application.
     :param username: The username.
-    :return: A tuple of the client and the CSRF token.
+    :return: The user client.
     """
     client: httpx.Client = httpx.Client(app=app, base_url=TEST_SERVER)
     client.headers["Referer"] = TEST_SERVER
     csrf_token: str = get_csrf_token(client)
     with app.app_context():
         encoded_next_uri: str = encode_next(NEXT_URI)
     response: httpx.Response = client.post("/login",
                                            data={"csrf_token": csrf_token,
                                                  "next": encoded_next_uri,
                                                  "username": username})
     assert response.status_code == 302
     assert response.headers["Location"] == NEXT_URI
-    return client, csrf_token
+    return client
 
 
 def set_locale(app: Flask, client: httpx.Client, csrf_token: str,
                locale: Literal["en", "zh_Hant", "zh_Hans"]) -> None:
     """Sets the current locale.
 
     :param app: The Flask application.
```

### Comparing `mia-accounting-1.5.6/tests/testlib_journal_entry.py` & `mia-accounting-1.5.7/tests/testlib_journal_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import re
 from decimal import Decimal
 from secrets import randbelow
 
 from flask import Flask
 
 from test_site import db
-from testlib import NEXT_URI, Accounts
+from testlib import Accounts
 
 NON_EMPTY_NOTE: str = "  This is \n\na test."
 """The stripped content of an non-empty note."""
 EMPTY_NOTE: str = " \n\n  "
 """The empty note content."""
```

