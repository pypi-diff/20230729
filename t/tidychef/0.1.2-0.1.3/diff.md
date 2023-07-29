# Comparing `tmp/tidychef-0.1.2.tar.gz` & `tmp/tidychef-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidychef-0.1.2.tar", max compression
+gzip compressed data, was "tidychef-0.1.3.tar", max compression
```

## Comparing `tidychef-0.1.2.tar` & `tidychef-0.1.3.tar`

### file list

```diff
@@ -1,88 +1,95 @@
--rw-r--r--   0        0        0     1980 2023-07-25 09:34:32.797397 tidychef-0.1.2/README.md
--rw-r--r--   0        0        0     1223 2023-07-25 09:34:44.616988 tidychef-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      245 2023-07-25 07:54:18.333658 tidychef-0.1.2/tidychef/__init__.py
--rw-r--r--   0        0        0      110 2023-07-05 08:30:04.083380 tidychef-0.1.2/tidychef/acquire/__init__.py
--rw-r--r--   0        0        0      520 2023-07-24 18:04:58.226769 tidychef-0.1.2/tidychef/acquire/base.py
--rw-r--r--   0        0        0      133 2023-06-28 13:56:49.387210 tidychef-0.1.2/tidychef/acquire/csv/__init__.py
--rw-r--r--   0        0        0     3402 2023-07-25 07:42:58.792065 tidychef-0.1.2/tidychef/acquire/csv/http_implemented.py
--rw-r--r--   0        0        0     3036 2023-07-25 07:43:33.075028 tidychef-0.1.2/tidychef/acquire/csv/local_implemented.py
--rw-r--r--   0        0        0     2455 2023-07-25 07:45:41.458935 tidychef-0.1.2/tidychef/acquire/main.py
--rw-r--r--   0        0        0      163 2023-07-23 15:42:10.265499 tidychef-0.1.2/tidychef/acquire/python/__init__.py
--rw-r--r--   0        0        0     2467 2023-07-25 07:43:28.624238 tidychef-0.1.2/tidychef/acquire/python/listoflists_implemented.py
--rw-r--r--   0        0        0     2851 2023-07-25 07:44:03.424136 tidychef-0.1.2/tidychef/acquire/python/pipetable_implemented.py
--rw-r--r--   0        0        0      133 2023-06-28 14:19:41.973466 tidychef-0.1.2/tidychef/acquire/xls/__init__.py
--rw-r--r--   0        0        0     4258 2023-07-25 07:44:26.721737 tidychef-0.1.2/tidychef/acquire/xls/http_implemented.py
--rw-r--r--   0        0        0     3345 2023-07-25 07:44:39.053004 tidychef-0.1.2/tidychef/acquire/xls/local_implemented.py
--rw-r--r--   0        0        0      134 2023-06-28 13:56:49.375947 tidychef-0.1.2/tidychef/acquire/xlsx/__init__.py
--rw-r--r--   0        0        0     4372 2023-07-25 07:44:56.396637 tidychef-0.1.2/tidychef/acquire/xlsx/http_implemented.py
--rw-r--r--   0        0        0     3662 2023-07-25 07:45:08.699028 tidychef-0.1.2/tidychef/acquire/xlsx/local_implemented.py
--rw-r--r--   0        0        0      149 2023-07-23 17:11:06.781553 tidychef-0.1.2/tidychef/against/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 20:08:08.429121 tidychef-0.1.2/tidychef/against/implementations/__init__.py
--rw-r--r--   0        0        0      638 2023-07-25 07:23:52.963306 tidychef-0.1.2/tidychef/against/implementations/base.py
--rw-r--r--   0        0        0     1163 2023-07-25 07:25:47.995142 tidychef-0.1.2/tidychef/against/implementations/items.py
--rw-r--r--   0        0        0     2401 2023-07-25 07:25:53.424611 tidychef-0.1.2/tidychef/against/implementations/length.py
--rw-r--r--   0        0        0     3572 2023-07-25 07:25:36.472780 tidychef-0.1.2/tidychef/against/implementations/numeric.py
--rw-r--r--   0        0        0     1120 2023-07-25 07:26:23.342013 tidychef-0.1.2/tidychef/against/implementations/regex.py
--rw-r--r--   0        0        0     1766 2023-07-25 07:47:12.734570 tidychef-0.1.2/tidychef/against/wrapper.py
--rw-r--r--   0        0        0       48 2023-05-28 22:18:13.690464 tidychef-0.1.2/tidychef/column/__init__.py
--rw-r--r--   0        0        0     2970 2023-07-25 07:46:59.116780 tidychef-0.1.2/tidychef/column/base.py
--rw-r--r--   0        0        0     4995 2023-07-25 07:47:30.656866 tidychef-0.1.2/tidychef/column/column.py
--rw-r--r--   0        0        0      527 2023-06-27 16:25:09.098617 tidychef-0.1.2/tidychef/datafuncs/README.md
--rw-r--r--   0        0        0     1075 2023-07-23 17:11:06.809528 tidychef-0.1.2/tidychef/datafuncs/__init__.py
--rw-r--r--   0        0        0     8878 2023-07-24 18:03:57.415174 tidychef-0.1.2/tidychef/datafuncs/common.py
--rw-r--r--   0        0        0     5639 2023-07-24 18:03:55.736608 tidychef-0.1.2/tidychef/datafuncs/excel.py
--rw-r--r--   0        0        0     6119 2023-07-24 18:03:54.264597 tidychef-0.1.2/tidychef/datafuncs/ordering.py
--rw-r--r--   0        0        0      453 2023-05-24 09:26:45.996492 tidychef-0.1.2/tidychef/direction/README.md
--rw-r--r--   0        0        0       60 2023-07-12 10:33:30.217649 tidychef-0.1.2/tidychef/direction/__init__.py
--rw-r--r--   0        0        0     4803 2023-07-24 18:03:49.931406 tidychef-0.1.2/tidychef/direction/directions.py
--rw-r--r--   0        0        0      885 2023-07-23 17:11:06.805910 tidychef-0.1.2/tidychef/exceptions/__init__.py
--rw-r--r--   0        0        0     2150 2023-07-23 13:37:16.866495 tidychef-0.1.2/tidychef/exceptions/badparams.py
--rw-r--r--   0        0        0      777 2023-07-23 17:10:30.841539 tidychef-0.1.2/tidychef/exceptions/cells.py
--rw-r--r--   0        0        0     3408 2023-07-23 17:10:20.538378 tidychef-0.1.2/tidychef/exceptions/common.py
--rw-r--r--   0        0        0      652 2023-07-12 12:23:20.039435 tidychef-0.1.2/tidychef/exceptions/lookups.py
--rw-r--r--   0        0        0        0 2023-07-12 13:26:57.378906 tidychef-0.1.2/tidychef/lookup/__init__.py
--rw-r--r--   0        0        0      447 2023-07-24 18:03:47.784091 tidychef-0.1.2/tidychef/lookup/base.py
--rw-r--r--   0        0        0        0 2023-05-26 13:52:55.388417 tidychef-0.1.2/tidychef/lookup/engines/README.md
--rw-r--r--   0        0        0        0 2023-06-14 15:18:13.870543 tidychef-0.1.2/tidychef/lookup/engines/__init__.py
--rw-r--r--   0        0        0    13681 2023-07-25 07:48:25.203597 tidychef-0.1.2/tidychef/lookup/engines/closest.py
--rw-r--r--   0        0        0      957 2023-07-24 18:03:44.342917 tidychef-0.1.2/tidychef/lookup/engines/constant.py
--rw-r--r--   0        0        0     6129 2023-07-25 07:48:38.777076 tidychef-0.1.2/tidychef/lookup/engines/direct.py
--rw-r--r--   0        0        0     4049 2023-07-25 07:48:47.404609 tidychef-0.1.2/tidychef/lookup/engines/horizontal_condition.py
--rw-r--r--   0        0        0    10700 2023-07-25 07:49:00.642629 tidychef-0.1.2/tidychef/lookup/engines/within.py
--rw-r--r--   0        0        0       21 2023-05-24 09:26:45.998537 tidychef-0.1.2/tidychef/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 09:26:46.000263 tidychef-0.1.2/tidychef/models/source/__init__.py
--rw-r--r--   0        0        0     6999 2023-07-25 07:49:30.892006 tidychef-0.1.2/tidychef/models/source/cell.py
--rw-r--r--   0        0        0       77 2023-05-24 09:26:46.000543 tidychef-0.1.2/tidychef/models/source/cellformat.py
--rw-r--r--   0        0        0     7762 2023-07-25 07:49:40.728144 tidychef-0.1.2/tidychef/models/source/table.py
--rw-r--r--   0        0        0       39 2023-06-20 17:35:02.406176 tidychef-0.1.2/tidychef/notebook/__init__.py
--rw-r--r--   0        0        0      465 2023-07-16 10:09:55.515709 tidychef-0.1.2/tidychef/notebook/ipython.py
--rw-r--r--   0        0        0        0 2023-06-17 11:41:28.459219 tidychef-0.1.2/tidychef/notebook/preview/__init__.py
--rw-r--r--   0        0        0     3778 2023-07-25 07:51:24.701683 tidychef-0.1.2/tidychef/notebook/preview/boundary.py
--rw-r--r--   0        0        0     2910 2023-07-25 07:50:26.281679 tidychef-0.1.2/tidychef/notebook/preview/html/components.py
--rw-r--r--   0        0        0      651 2023-07-14 22:09:11.515526 tidychef-0.1.2/tidychef/notebook/preview/html/constants.py
--rw-r--r--   0        0        0     2616 2023-07-25 07:50:37.866855 tidychef-0.1.2/tidychef/notebook/preview/html/main.py
--rw-r--r--   0        0        0     4869 2023-07-25 07:50:58.627598 tidychef-0.1.2/tidychef/notebook/preview/html/table.py
--rw-r--r--   0        0        0      926 2023-07-16 14:00:02.838338 tidychef-0.1.2/tidychef/notebook/preview/html/tidy_data.py
--rw-r--r--   0        0        0       59 2023-07-12 10:33:30.001045 tidychef-0.1.2/tidychef/output/__init__.py
--rw-r--r--   0        0        0      561 2023-06-16 19:33:30.841073 tidychef-0.1.2/tidychef/output/base.py
--rw-r--r--   0        0        0    14254 2023-07-25 07:52:00.465984 tidychef-0.1.2/tidychef/output/tidydata.py
--rw-r--r--   0        0        0      459 2023-06-27 16:24:57.036542 tidychef-0.1.2/tidychef/selection/README.md
--rw-r--r--   0        0        0      143 2023-07-12 10:33:30.114915 tidychef-0.1.2/tidychef/selection/__init__.py
--rw-r--r--   0        0        0      153 2023-07-24 18:06:08.468256 tidychef-0.1.2/tidychef/selection/csv/csv.py
--rw-r--r--   0        0        0     2022 2023-06-27 16:25:30.891041 tidychef-0.1.2/tidychef/selection/filters/README.md
--rw-r--r--   0        0        0      196 2023-07-17 15:19:20.512477 tidychef-0.1.2/tidychef/selection/filters/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-24 18:06:42.658006 tidychef-0.1.2/tidychef/selection/filters/common.py
--rw-r--r--   0        0        0    28752 2023-07-25 07:58:50.258318 tidychef-0.1.2/tidychef/selection/selectable.py
--rw-r--r--   0        0        0      132 2023-06-28 16:12:18.376303 tidychef-0.1.2/tidychef/selection/xls/xls.py
--rw-r--r--   0        0        0      134 2023-06-28 16:11:52.808553 tidychef-0.1.2/tidychef/selection/xlsx/xlsx.py
--rw-r--r--   0        0        0       41 2023-06-28 13:17:51.552905 tidychef-0.1.2/tidychef/utils/__init__.py
--rw-r--r--   0        0        0       72 2023-05-24 09:26:46.004839 tidychef-0.1.2/tidychef/utils/cellutils/__init__.py
--rw-r--r--   0        0        0     1556 2023-05-24 09:26:46.005013 tidychef-0.1.2/tidychef/utils/cellutils/excel.py
--rw-r--r--   0        0        0       76 2023-05-24 09:26:46.005163 tidychef-0.1.2/tidychef/utils/decorators/README.md
--rw-r--r--   0        0        0       94 2023-07-18 07:19:23.361670 tidychef-0.1.2/tidychef/utils/decorators/__init__.py
--rw-r--r--   0        0        0      572 2023-05-28 22:18:13.736328 tidychef-0.1.2/tidychef/utils/decorators/dontmutate.py
--rw-r--r--   0        0        0       40 2023-06-16 20:07:44.113463 tidychef-0.1.2/tidychef/utils/fileutils/__init__.py
--rw-r--r--   0        0        0      809 2023-07-24 18:06:46.898985 tidychef-0.1.2/tidychef/utils/fileutils/paths.py
--rw-r--r--   0        0        0      494 2023-06-28 13:56:51.241240 tidychef-0.1.2/tidychef/utils/http/caching.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 tidychef-0.1.2/setup.py
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 tidychef-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2157 2023-07-29 13:07:21.242264 tidychef-0.1.3/README.md
+-rw-r--r--   0        0        0     1256 2023-07-29 18:35:46.983867 tidychef-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-07-25 10:48:21.442542 tidychef-0.1.3/tidychef/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-29 13:46:10.145828 tidychef-0.1.3/tidychef/acquire/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-25 10:48:21.442841 tidychef-0.1.3/tidychef/acquire/base.py
+-rw-r--r--   0        0        0      133 2023-07-25 10:48:21.443013 tidychef-0.1.3/tidychef/acquire/csv/__init__.py
+-rw-r--r--   0        0        0     3402 2023-07-25 10:48:21.443203 tidychef-0.1.3/tidychef/acquire/csv/http_implemented.py
+-rw-r--r--   0        0        0     3036 2023-07-25 10:48:21.443371 tidychef-0.1.3/tidychef/acquire/csv/local_implemented.py
+-rw-r--r--   0        0        0    10615 2023-07-29 15:41:13.756802 tidychef-0.1.3/tidychef/acquire/excel_time.py
+-rw-r--r--   0        0        0     2455 2023-07-25 10:48:21.443507 tidychef-0.1.3/tidychef/acquire/main.py
+-rw-r--r--   0        0        0      133 2023-07-27 14:17:58.059556 tidychef-0.1.3/tidychef/acquire/ods/__init__.py
+-rw-r--r--   0        0        0     4498 2023-07-29 13:46:12.233315 tidychef-0.1.3/tidychef/acquire/ods/http_implemented.py
+-rw-r--r--   0        0        0     3167 2023-07-29 13:46:12.167301 tidychef-0.1.3/tidychef/acquire/ods/local_implemented.py
+-rw-r--r--   0        0        0      163 2023-07-25 10:48:21.443684 tidychef-0.1.3/tidychef/acquire/python/__init__.py
+-rw-r--r--   0        0        0     2467 2023-07-25 10:48:21.443839 tidychef-0.1.3/tidychef/acquire/python/listoflists_implemented.py
+-rw-r--r--   0        0        0     2851 2023-07-25 10:48:21.443953 tidychef-0.1.3/tidychef/acquire/python/pipetable_implemented.py
+-rw-r--r--   0        0        0      133 2023-07-25 10:48:21.444117 tidychef-0.1.3/tidychef/acquire/xls/__init__.py
+-rw-r--r--   0        0        0     3995 2023-07-29 16:49:19.165261 tidychef-0.1.3/tidychef/acquire/xls/http_implemented.py
+-rw-r--r--   0        0        0     3059 2023-07-29 16:49:27.105585 tidychef-0.1.3/tidychef/acquire/xls/local_implemented.py
+-rw-r--r--   0        0        0     3852 2023-07-29 17:59:31.503924 tidychef-0.1.3/tidychef/acquire/xls/shared.py
+-rw-r--r--   0        0        0      134 2023-07-25 10:48:21.444533 tidychef-0.1.3/tidychef/acquire/xlsx/__init__.py
+-rw-r--r--   0        0        0     4117 2023-07-29 17:31:33.932274 tidychef-0.1.3/tidychef/acquire/xlsx/http_implemented.py
+-rw-r--r--   0        0        0     3407 2023-07-29 17:52:20.445039 tidychef-0.1.3/tidychef/acquire/xlsx/local_implemented.py
+-rw-r--r--   0        0        0     3224 2023-07-29 18:02:58.610886 tidychef-0.1.3/tidychef/acquire/xlsx/shared.py
+-rw-r--r--   0        0        0      149 2023-07-29 13:46:12.103603 tidychef-0.1.3/tidychef/against/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:21.445014 tidychef-0.1.3/tidychef/against/implementations/__init__.py
+-rw-r--r--   0        0        0      638 2023-07-25 10:48:21.445135 tidychef-0.1.3/tidychef/against/implementations/base.py
+-rw-r--r--   0        0        0     1163 2023-07-25 10:48:21.445268 tidychef-0.1.3/tidychef/against/implementations/items.py
+-rw-r--r--   0        0        0     2401 2023-07-25 10:48:21.445394 tidychef-0.1.3/tidychef/against/implementations/length.py
+-rw-r--r--   0        0        0     3537 2023-07-29 13:42:59.323155 tidychef-0.1.3/tidychef/against/implementations/numeric.py
+-rw-r--r--   0        0        0     1120 2023-07-29 13:46:12.174321 tidychef-0.1.3/tidychef/against/implementations/regex.py
+-rw-r--r--   0        0        0     1766 2023-07-29 13:46:12.202258 tidychef-0.1.3/tidychef/against/wrapper.py
+-rw-r--r--   0        0        0       48 2023-07-25 10:48:21.445902 tidychef-0.1.3/tidychef/column/__init__.py
+-rw-r--r--   0        0        0     2970 2023-07-25 10:48:21.446019 tidychef-0.1.3/tidychef/column/base.py
+-rw-r--r--   0        0        0     5047 2023-07-29 13:46:12.396381 tidychef-0.1.3/tidychef/column/column.py
+-rw-r--r--   0        0        0      527 2023-07-25 10:48:21.446305 tidychef-0.1.3/tidychef/datafuncs/README.md
+-rw-r--r--   0        0        0     1075 2023-07-29 13:46:12.195861 tidychef-0.1.3/tidychef/datafuncs/__init__.py
+-rw-r--r--   0        0        0     8878 2023-07-25 10:48:21.446544 tidychef-0.1.3/tidychef/datafuncs/common.py
+-rw-r--r--   0        0        0     5639 2023-07-25 10:48:21.446692 tidychef-0.1.3/tidychef/datafuncs/excel.py
+-rw-r--r--   0        0        0     6119 2023-07-25 10:48:21.446806 tidychef-0.1.3/tidychef/datafuncs/ordering.py
+-rw-r--r--   0        0        0      453 2023-07-25 10:48:21.446970 tidychef-0.1.3/tidychef/direction/README.md
+-rw-r--r--   0        0        0       60 2023-07-25 10:48:21.447080 tidychef-0.1.3/tidychef/direction/__init__.py
+-rw-r--r--   0        0        0     4803 2023-07-25 10:48:21.447203 tidychef-0.1.3/tidychef/direction/directions.py
+-rw-r--r--   0        0        0      885 2023-07-29 15:42:07.757131 tidychef-0.1.3/tidychef/exceptions/__init__.py
+-rw-r--r--   0        0        0     2150 2023-07-25 10:48:21.447473 tidychef-0.1.3/tidychef/exceptions/badparams.py
+-rw-r--r--   0        0        0      777 2023-07-25 10:48:21.447575 tidychef-0.1.3/tidychef/exceptions/cells.py
+-rw-r--r--   0        0        0     3408 2023-07-29 15:42:02.778914 tidychef-0.1.3/tidychef/exceptions/common.py
+-rw-r--r--   0        0        0      652 2023-07-25 10:48:21.447808 tidychef-0.1.3/tidychef/exceptions/lookups.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:21.447916 tidychef-0.1.3/tidychef/lookup/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-25 10:48:21.448016 tidychef-0.1.3/tidychef/lookup/base.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:21.448111 tidychef-0.1.3/tidychef/lookup/engines/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:21.448165 tidychef-0.1.3/tidychef/lookup/engines/__init__.py
+-rw-r--r--   0        0        0    13669 2023-07-29 13:43:34.445104 tidychef-0.1.3/tidychef/lookup/engines/closest.py
+-rw-r--r--   0        0        0      957 2023-07-25 10:48:21.448424 tidychef-0.1.3/tidychef/lookup/engines/constant.py
+-rw-r--r--   0        0        0     6129 2023-07-29 13:46:12.622462 tidychef-0.1.3/tidychef/lookup/engines/direct.py
+-rw-r--r--   0        0        0     4049 2023-07-29 13:46:12.359708 tidychef-0.1.3/tidychef/lookup/engines/horizontal_condition.py
+-rw-r--r--   0        0        0    10700 2023-07-29 13:46:12.833989 tidychef-0.1.3/tidychef/lookup/engines/within.py
+-rw-r--r--   0        0        0       21 2023-07-25 10:48:21.448979 tidychef-0.1.3/tidychef/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:21.449075 tidychef-0.1.3/tidychef/models/source/__init__.py
+-rw-r--r--   0        0        0     7195 2023-07-29 13:46:12.658244 tidychef-0.1.3/tidychef/models/source/cell.py
+-rw-r--r--   0        0        0       77 2023-07-25 10:48:21.449294 tidychef-0.1.3/tidychef/models/source/cellformat.py
+-rw-r--r--   0        0        0     7762 2023-07-25 10:48:21.449417 tidychef-0.1.3/tidychef/models/source/table.py
+-rw-r--r--   0        0        0       39 2023-07-25 10:48:21.449558 tidychef-0.1.3/tidychef/notebook/__init__.py
+-rw-r--r--   0        0        0      465 2023-07-25 10:48:21.449658 tidychef-0.1.3/tidychef/notebook/ipython.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:48:21.449769 tidychef-0.1.3/tidychef/notebook/preview/__init__.py
+-rw-r--r--   0        0        0     3762 2023-07-29 13:44:56.305958 tidychef-0.1.3/tidychef/notebook/preview/boundary.py
+-rw-r--r--   0        0        0     2910 2023-07-25 10:48:21.450103 tidychef-0.1.3/tidychef/notebook/preview/html/components.py
+-rw-r--r--   0        0        0      651 2023-07-25 10:48:21.450202 tidychef-0.1.3/tidychef/notebook/preview/html/constants.py
+-rw-r--r--   0        0        0     2616 2023-07-25 10:48:21.450308 tidychef-0.1.3/tidychef/notebook/preview/html/main.py
+-rw-r--r--   0        0        0     4869 2023-07-29 13:46:12.739005 tidychef-0.1.3/tidychef/notebook/preview/html/table.py
+-rw-r--r--   0        0        0      926 2023-07-25 10:48:21.450516 tidychef-0.1.3/tidychef/notebook/preview/html/tidy_data.py
+-rw-r--r--   0        0        0       59 2023-07-25 10:48:21.450652 tidychef-0.1.3/tidychef/output/__init__.py
+-rw-r--r--   0        0        0      561 2023-07-25 10:48:21.450760 tidychef-0.1.3/tidychef/output/base.py
+-rw-r--r--   0        0        0    15600 2023-07-29 13:46:12.972057 tidychef-0.1.3/tidychef/output/tidydata.py
+-rw-r--r--   0        0        0      459 2023-07-25 10:48:21.451052 tidychef-0.1.3/tidychef/selection/README.md
+-rw-r--r--   0        0        0      178 2023-07-29 13:46:10.108793 tidychef-0.1.3/tidychef/selection/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-25 10:48:21.451291 tidychef-0.1.3/tidychef/selection/csv/csv.py
+-rw-r--r--   0        0        0     2022 2023-07-25 10:48:21.451444 tidychef-0.1.3/tidychef/selection/filters/README.md
+-rw-r--r--   0        0        0      196 2023-07-25 10:48:21.451541 tidychef-0.1.3/tidychef/selection/filters/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-25 10:48:21.451635 tidychef-0.1.3/tidychef/selection/filters/common.py
+-rw-r--r--   0        0        0      132 2023-07-26 16:45:28.267730 tidychef-0.1.3/tidychef/selection/ods/ods.py
+-rw-r--r--   0        0        0    28828 2023-07-29 13:46:13.296801 tidychef-0.1.3/tidychef/selection/selectable.py
+-rw-r--r--   0        0        0      132 2023-07-25 10:48:21.452056 tidychef-0.1.3/tidychef/selection/xls/xls.py
+-rw-r--r--   0        0        0      134 2023-07-25 10:48:21.452191 tidychef-0.1.3/tidychef/selection/xlsx/xlsx.py
+-rw-r--r--   0        0        0       41 2023-07-25 10:48:21.452328 tidychef-0.1.3/tidychef/utils/__init__.py
+-rw-r--r--   0        0        0       72 2023-07-25 10:48:21.452460 tidychef-0.1.3/tidychef/utils/cellutils/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-25 10:48:21.452590 tidychef-0.1.3/tidychef/utils/cellutils/excel.py
+-rw-r--r--   0        0        0       76 2023-07-25 10:48:21.452737 tidychef-0.1.3/tidychef/utils/decorators/README.md
+-rw-r--r--   0        0        0       94 2023-07-25 10:48:21.452842 tidychef-0.1.3/tidychef/utils/decorators/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-25 10:48:21.452950 tidychef-0.1.3/tidychef/utils/decorators/dontmutate.py
+-rw-r--r--   0        0        0       40 2023-07-25 10:48:21.453093 tidychef-0.1.3/tidychef/utils/fileutils/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-25 10:48:21.453191 tidychef-0.1.3/tidychef/utils/fileutils/paths.py
+-rw-r--r--   0        0        0      494 2023-07-25 10:48:21.453334 tidychef-0.1.3/tidychef/utils/http/caching.py
+-rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 tidychef-0.1.3/setup.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 tidychef-0.1.3/PKG-INFO
```

### Comparing `tidychef-0.1.2/README.md` & `tidychef-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 ![](https://mikeadamss.github.io/tidychef/_images/bands-before.png)
 
 into something that looks like this:
 
 ![](https://mikeadamss.github.io/tidychef/_images/bands-after.png)
 _Note: image cropped for reasons of practicality._
 
+Currently supported input formats are `xls`, `xlsx`, `ods` and `csv`. Though users can add additional formats relatively easily and without a codebase change being necessary.
+
 Tidychef is **designed to allow even novice python users or analysts to quickly become productive** but also has an advanced feature set and is designed to be readily and easily extended (adding new source of tabulated data, your own use case specific methods and filters and domain specific validation etc are all possible and documented in detail).
 
 In depth training material, examples and technical documentation [can be found here](https://mikeadamss.github.io/tidychef/intro.html#).
 
 ## Installation
 
 ```
 pip install tidychef
 ```
 
-## Acknowlagements
+## Acknowledgements
 
 Tidychef is directly inspired by the python package [databaker](https://github.com/sensiblecodeio/databaker) created by [The Sensible Code Company](https://sensiblecode.io/) in partnership with the United Kingdoms [Office For National Statistics](https://www.ons.gov.uk/).
 
 While I liked [databaker](https://github.com/sensiblecodeio/databaker) and successfully worked with it on multiple ETL projects over the course of almost a decade, this software should be considered the culmination of that work and the lessons learned from that time.
```

### Comparing `tidychef-0.1.2/pyproject.toml` & `tidychef-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidychef"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python framework for transforming tabulated data with visual relationships into tidy data"
 authors = ["mikeAdamss <mikelovesbooks@gmail.com>"]
 packages = [
   {include = "tidychef"},
 ]
 license = "Apache 2.0"
 readme = "README.md"
@@ -16,14 +16,16 @@
 requests = "^2.31.0"
 validators = "^0.20.0"
 openpyxl = "^3.1.2"
 cachecontrol = "^0.13.1"
 filelock = "^3.12.2"
 xlrd = "^2.0.1"
 jupyter = "^1.0.0"
+ezodf = "^0.3.2"
+lxml = "^4.9.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 isort = "^5.10.1"
 pytest-cov = "^3.0.0"
 jupyter-book = "^0.15.1"
```

### Comparing `tidychef-0.1.2/tidychef/acquire/base.py` & `tidychef-0.1.3/tidychef/acquire/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/acquire/csv/http_implemented.py` & `tidychef-0.1.3/tidychef/acquire/csv/http_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/acquire/csv/local_implemented.py` & `tidychef-0.1.3/tidychef/acquire/csv/local_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/acquire/main.py` & `tidychef-0.1.3/tidychef/acquire/main.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/acquire/python/listoflists_implemented.py` & `tidychef-0.1.3/tidychef/acquire/python/listoflists_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/acquire/python/pipetable_implemented.py` & `tidychef-0.1.3/tidychef/acquire/python/pipetable_implemented.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/acquire/xls/http_implemented.py` & `tidychef-0.1.3/tidychef/acquire/xls/http_implemented.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 from typing import Callable, List, Optional, Union
 
 import requests
 import validators
 import xlrd
 
 from tidychef.acquire.base import BaseReader
-from tidychef.models.source.cell import Cell
-from tidychef.models.source.table import Table
 from tidychef.selection.selectable import Selectable
 from tidychef.selection.xls.xls import XlsSelectable
 from tidychef.utils.http.caching import get_cached_session
 
 from ..base import BaseReader
 from ..main import acquirer
+from .shared import sheets_from_workbook
 
 
 def http(
     source: Union[str, Path],
     selectable: Selectable = XlsSelectable,
     pre_hook: Optional[Callable] = None,
     post_hook: Optional[Callable] = None,
@@ -107,28 +106,22 @@
                 """
             )
 
         bio = io.BytesIO()
         bio.write(response.content)
         bio.seek(0)
 
-        workbook: xlrd.Book = xlrd.open_workbook(file_contents=bio.read(), **kwargs)
-        assert isinstance(workbook, xlrd.Book)
+        custom_time_formats = kwargs.get("custom_time_formats", {})
+        kwargs.pop("custom_time_formats", None)
 
-        tidychef_selectables = []
-        worksheet_names = workbook.sheet_names()
-        for worksheet_name in worksheet_names:
-
-            worksheet = workbook.sheet_by_name(worksheet_name, **kwargs)
-
-            table = Table()
-            num_rows = worksheet.nrows
-            for y in range(0, num_rows):
-                for x, cell in enumerate(worksheet.row(y)):
-                    table.add_cell(
-                        Cell(x=x, y=y, value=str(cell.value) if cell.value else "")
-                    )
-
-            tidychef_selectables.append(
-                selectable(table, source=source, name=worksheet_name)
-            )
-        return tidychef_selectables
+        workbook: xlrd.Book = xlrd.open_workbook(
+            file_contents=bio.read(), formatting_info=True, **kwargs
+        )
+
+        sheets = sheets_from_workbook(source, selectable, workbook, custom_time_formats, self.tables, **kwargs)
+        # In this instance we've filtered the tables at the point of reading, so
+        # remove the post load table name regex.
+        self.tables = None 
+
+        if len(sheets) == 1:
+            return sheets[0]
+        return sheets
```

### Comparing `tidychef-0.1.2/tidychef/acquire/xls/local_implemented.py` & `tidychef-0.1.3/tidychef/acquire/xls/local_implemented.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 
 from pathlib import Path
 from typing import Callable, List, Optional, Union
 
 import xlrd
 
 from tidychef.acquire.base import BaseReader
-from tidychef.models.source.cell import Cell
-from tidychef.models.source.table import Table
 from tidychef.selection.selectable import Selectable
 from tidychef.selection.xls.xls import XlsSelectable
 
 from ..base import BaseReader
 from ..main import acquirer
+from .shared import sheets_from_workbook
 
 
 def local(
     source: Union[str, Path],
     selectable: Selectable = XlsSelectable,
     pre_hook: Optional[Callable] = None,
     post_hook: Optional[Callable] = None,
@@ -78,28 +77,21 @@
         Additional **kwargs are propagated to xlrd.open_workbook()
 
         :param source: A Path or str representing a path indicating a local file
         :param selectable: The selectable type to be returned.
         :return: A list of type as specified by param selectable.
         """
 
-        workbook: xlrd.Book = xlrd.open_workbook(source)
-        assert isinstance(workbook, xlrd.Book)
+        custom_time_formats = kwargs.get("custom_time_formats", {})
+        kwargs.pop("custom_time_formats", None)
 
-        tidychef_selectables = []
-        worksheet_names = workbook.sheet_names()
-        for worksheet_name in worksheet_names:
-
-            worksheet = workbook.sheet_by_name(worksheet_name, **kwargs)
-
-            table = Table()
-            num_rows = worksheet.nrows
-            for y in range(0, num_rows):
-                for x, cell in enumerate(worksheet.row(y)):
-                    table.add_cell(
-                        Cell(x=x, y=y, value=str(cell.value) if cell.value else "")
-                    )
-
-            tidychef_selectables.append(
-                selectable(table, source=source, name=worksheet_name)
-            )
-        return tidychef_selectables
+        workbook: xlrd.Book = xlrd.open_workbook(source, formatting_info=True)
+        
+        sheets = sheets_from_workbook(source, selectable, workbook, custom_time_formats, self.tables, **kwargs)
+
+        # In this instance we've filtered the tables at the point of reading, so
+        # remove the post load filter.
+        self.tables = None 
+
+        if len(sheets) == 1:
+            return sheets[0]
+        return sheets
```

### Comparing `tidychef-0.1.2/tidychef/acquire/xlsx/http_implemented.py` & `tidychef-0.1.3/tidychef/acquire/ods/http_implemented.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,135 +1,139 @@
 """
 Holds the code that defines the local xlsx reader.
 """
 
-import io
 from pathlib import Path
+from tempfile import NamedTemporaryFile
 from typing import Callable, List, Optional, Union
 
-import openpyxl
+import ezodf
 import requests
 import validators
+from ezodf.document import PackagedDocument
 
 from tidychef.acquire.base import BaseReader
 from tidychef.models.source.cell import Cell
 from tidychef.models.source.table import Table
+from tidychef.selection.ods.ods import OdsSelectable
 from tidychef.selection.selectable import Selectable
-from tidychef.selection.xlsx.xlsx import XlsxSelectable
 from tidychef.utils.http.caching import get_cached_session
 
 from ..base import BaseReader
 from ..main import acquirer
 
 
 def http(
     source: Union[str, Path],
-    selectable: Selectable = XlsxSelectable,
+    selectable: Selectable = OdsSelectable,
     pre_hook: Optional[Callable] = None,
     post_hook: Optional[Callable] = None,
     session: requests.Session = None,
     cache: bool = True,
     tables: str = None,
     **kwargs,
-) -> Union[XlsxSelectable, List[XlsxSelectable]]:
+) -> Union[OdsSelectable, List[OdsSelectable]]:
     """
     Read data from a Path (or string representing a path)
     present on the same machine where tidychef is running.
 
-    This local xlsx reader uses openpyxl:
-    https://openpyxl.readthedocs.io/en/stable/index.html
-
-    Any kwargs passed to this function are propagated to
-    the openpyxl.load_workbook() method.
-
     :param source: A url.
-    :param selectable: A class that implements tidychef.selection.selectable.Selectable of an inheritor of. Default is XlsxSelectable
+    :param selectable: A class that implements tidychef.selection.selectable.Selectable of an inheritor of. Default is OdsSelectable.
     :param pre_hook: A callable that can take source as an argument
-    :param post_hook: A callable that can take the output of XlsxSelectable.parse() as an argument.
+    :param post_hook: A callable that can take the output of HttpOdsReader.parse() as an argument.
     :param session: An optional requests.Session object.
     :param cache: Boolean flag for whether or not to cache get requests.
     :return: A single populated Selectable of type as specified by selectable param.
     """
 
     assert validators.url(source), f"'{source}' is not a valid http/https url."
 
     return acquirer(
         source,
-        HttpXlsxReader(tables),
+        HttpOdsReader(tables),
         selectable,
         pre_hook=pre_hook,
         post_hook=post_hook,
         session=session,
         cache=cache,
         **kwargs,
     )
 
 
-class HttpXlsxReader(BaseReader):
+class HttpOdsReader(BaseReader):
     """
     A reader to lead in a source where that source is a locally
     held xlsx file.
     """
 
     def parse(
         self,
         source: str,
-        selectable: Selectable = XlsxSelectable,
-        data_only=True,
+        selectable: Selectable = OdsSelectable,
         session: requests.Session = None,
         cache: bool = True,
         **kwargs,
-    ) -> List[XlsxSelectable]:
+    ) -> List[OdsSelectable]:
         """
         Parse the provided source into a list of Selectables. Unless overridden the
-        selectable is of type XlsxSelectable.
+        selectable is of type XlsSelectable.
 
-        Additional **kwargs are propagated to openpyxl.load_workbook()
+        Additional **kwargs are propagated to xlrd.open_workbook()
 
-        :param source: A url.
+        :param source: A url
         :param selectable: The selectable type to be returned.
-        :data_only: An openpyxl.load_workbook() option to disable acquisition of non data elements from the tabulated source (macros etc)
+        :param session: An optional requests.Session object.
         :param session: An optional requests.Session object.
         :param cache: Boolean flag for whether or not to cache get requests.
         :return: A list of type as specified by param selectable.
         """
 
         if not session:
             if cache:
                 session = get_cached_session()
             else:
                 session = requests.session()
 
-        response: requests.Response = session.get(source, **kwargs)
+        response: requests.Response = session.get(source)
         if not response.ok:
             raise requests.exceptions.HTTPError(
                 f"""
                 Unable to get url: {source}
                 {response}
                 """
             )
 
-        bio = io.BytesIO()
-        bio.write(response.content)
-        bio.seek(0)
-
-        workbook: openpyxl.Workbook = openpyxl.load_workbook(
-            bio, data_only=data_only, **kwargs
-        )
+        # TODO: faster!
+        # So ezodf doesn't want to take a fileobject but instead needs a
+        # solid file. For now we're writing to a temp (self deleting) file
+        # and passing it in.
+        # This works but there's whole file write and re-read more in here
+        # that their needs to be.
+
+        temp_file = NamedTemporaryFile()
+        temp_file.write(response.content)
+        temp_file.seek(0)
 
+        spreadsheet: PackagedDocument = ezodf.opendoc(temp_file.name)
         tidychef_selectables = []
-        worksheet_names = workbook.get_sheet_names()
-        for worksheet_name in worksheet_names:
 
-            worksheet = workbook.get_sheet_by_name(worksheet_name)
+        for worksheet in spreadsheet.sheets:
 
             table = Table()
-            for y, row in enumerate(worksheet.iter_rows()):
+            for y, row in enumerate(worksheet.rows()):
                 for x, cell in enumerate(row):
                     table.add_cell(
-                        Cell(x=x, y=y, value=str(cell.value) if cell.value else "")
+                        Cell(
+                            x=int(x),
+                            y=int(y),
+                            value=str(cell.plaintext())
+                            if cell.value is not None
+                            else "",
+                        )
                     )
 
             tidychef_selectables.append(
-                selectable(table, source=source, name=worksheet_name)
+                selectable(table, source=source, name=worksheet.name)
             )
+
+        temp_file.close()
         return tidychef_selectables
```

### Comparing `tidychef-0.1.2/tidychef/acquire/xlsx/local_implemented.py` & `tidychef-0.1.3/tidychef/acquire/xlsx/local_implemented.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 from pathlib import Path
 from typing import Callable, List, Optional, Union
 
 import openpyxl
 
 from tidychef.acquire.base import BaseReader
-from tidychef.models.source.cell import Cell
-from tidychef.models.source.table import Table
 from tidychef.selection.selectable import Selectable
 from tidychef.selection.xlsx.xlsx import XlsxSelectable
 from tidychef.utils import fileutils
 
 from ..base import BaseReader
 from ..main import acquirer
+from .shared import sheets_from_workbook
 
 
 def local(
     source: Union[str, Path],
     selectable: Selectable = XlsxSelectable,
     pre_hook: Optional[Callable] = None,
     post_hook: Optional[Callable] = None,
@@ -81,30 +80,25 @@
 
         :param source: A Path or str representing a path indicating a local file
         :param selectable: The selectable type to be returned.
         :data_only: An openpyxl.load_workbook() option to disable acquisition of non data elements from the tabulated source (macros etc)
         :return: A list of type as specified by param selectable.
         """
 
-        source: Path = fileutils.ensure_existing_path(source, **kwargs)
+        source: Path = fileutils.ensure_existing_path(source)
+
+        custom_time_formats = kwargs.get("custom_time_formats", {})
+        kwargs.pop("custom_time_formats", None)
 
         workbook: openpyxl.Workbook = openpyxl.load_workbook(
             source, data_only=data_only, **kwargs
         )
 
-        tidychef_selectables = []
-        worksheet_names = workbook.get_sheet_names()
-        for worksheet_name in worksheet_names:
-
-            worksheet = workbook.get_sheet_by_name(worksheet_name)
-
-            table = Table()
-            for y, row in enumerate(worksheet.iter_rows()):
-                for x, cell in enumerate(row):
-                    table.add_cell(
-                        Cell(x=x, y=y, value=str(cell.value) if cell.value else "")
-                    )
-
-            tidychef_selectables.append(
-                selectable(table, source=source, name=worksheet_name)
-            )
-        return tidychef_selectables
+        sheets = sheets_from_workbook(source, selectable, workbook, custom_time_formats, self.tables)
+
+        # In this instance we've filtered the tables at the point of reading, so
+        # remove the post load filter.
+        self.tables = None 
+
+        if len(sheets) == 1:
+            return sheets[0]
+        return sheets
```

### Comparing `tidychef-0.1.2/tidychef/against/implementations/base.py` & `tidychef-0.1.3/tidychef/against/implementations/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/against/implementations/items.py` & `tidychef-0.1.3/tidychef/against/implementations/items.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/against/implementations/length.py` & `tidychef-0.1.3/tidychef/against/implementations/length.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/against/implementations/numeric.py` & `tidychef-0.1.3/tidychef/against/implementations/numeric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from dataclasses import dataclass
-
 from tidychef.against.implementations.base import BaseValidator
 from tidychef.models.source.cell import Cell
 
 
 class IsNumericOrFloatValidator(BaseValidator):
     """
     A class to return bool (valid or not) when
```

### Comparing `tidychef-0.1.2/tidychef/against/implementations/regex.py` & `tidychef-0.1.3/tidychef/against/implementations/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         Does the value property of the Cell
         match the provided pattern.
 
         :param cell: A single tidychef Cell object.
         :return: bool, is it valid or not
         """
         if self._compiled is None:
-            self._compiled = re.compile(r'' + self.pattern)
+            self._compiled = re.compile(r"" + self.pattern)
         if self._compiled.match(cell.value):
             return True
         return False
 
     def msg(self, cell: Cell) -> str:
         """
         Provide a contextually meaningful
```

### Comparing `tidychef-0.1.2/tidychef/against/wrapper.py` & `tidychef-0.1.3/tidychef/against/wrapper.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/column/base.py` & `tidychef-0.1.3/tidychef/column/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/column/column.py` & `tidychef-0.1.3/tidychef/column/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import copy
-from typing import Callable, List, Dict, Optional
+from typing import Callable, Dict, List, Optional
 
 from tidychef.column.base import BaseColumn
 from tidychef.exceptions import CellValidationError
 from tidychef.lookup.base import BaseLookupEngine
 from tidychef.lookup.engines.constant import Constant
 from tidychef.lookup.engines.horizontal_condition import HorizontalCondition
 from tidychef.models.source.cell import Cell
@@ -34,15 +34,17 @@
         """
         Returns table name where table name is known,
         else "Unnamed Table"
         """
         return self._table
 
     @staticmethod
-    def horizontal_condition(column_label: str, resolver: Callable, priority=0) -> Column:
+    def horizontal_condition(
+        column_label: str, resolver: Callable, priority=0
+    ) -> Column:
         """
         Creates a column that populates based on the
         values resolved for one or more other columns.
 
         :param column_label: The label we wish to give to the column.
         :param resolver: A callable to resolve the horizontal condition logic.
         :priority: controls order of resolution for all present HorizontalCondition objects,
@@ -126,15 +128,17 @@
         # isn't, so only check its valid once.
         if self.validation is not None and cell not in self._validated_cells:
             self._validated_cells.append(cell)
             if not self.validation(cell):
                 if hasattr(self.validation, "msg"):
                     msg = f"Message is: {self.validation.msg(cell)}"
                 else:
-                    msg = ''
-                raise CellValidationError(f'''
+                    msg = ""
+                raise CellValidationError(
+                    f"""
                         Column {self.label} has a cell that is not valid,
                         Invalid cell {cell}.
                         {msg}                      
-                        ''')
+                        """
+                )
 
         return cell
```

### Comparing `tidychef-0.1.2/tidychef/datafuncs/README.md` & `tidychef-0.1.3/tidychef/datafuncs/README.md`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/datafuncs/__init__.py` & `tidychef-0.1.3/tidychef/datafuncs/__init__.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/datafuncs/common.py` & `tidychef-0.1.3/tidychef/datafuncs/common.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/datafuncs/excel.py` & `tidychef-0.1.3/tidychef/datafuncs/excel.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/datafuncs/ordering.py` & `tidychef-0.1.3/tidychef/datafuncs/ordering.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/direction/directions.py` & `tidychef-0.1.3/tidychef/direction/directions.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/exceptions/__init__.py` & `tidychef-0.1.3/tidychef/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/exceptions/badparams.py` & `tidychef-0.1.3/tidychef/exceptions/badparams.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/exceptions/cells.py` & `tidychef-0.1.3/tidychef/exceptions/cells.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/exceptions/common.py` & `tidychef-0.1.3/tidychef/exceptions/common.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/exceptions/lookups.py` & `tidychef-0.1.3/tidychef/exceptions/lookups.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/lookup/engines/closest.py` & `tidychef-0.1.3/tidychef/lookup/engines/closest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from tidychef.direction.directions import Direction
 from tidychef.exceptions import AmbiguousLookupError, ImpossibleLookupError
 from tidychef.models.source.cell import Cell
 from tidychef.models.source.table import LiveTable
```

### Comparing `tidychef-0.1.2/tidychef/lookup/engines/constant.py` & `tidychef-0.1.3/tidychef/lookup/engines/constant.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/lookup/engines/direct.py` & `tidychef-0.1.3/tidychef/lookup/engines/direct.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/lookup/engines/horizontal_condition.py` & `tidychef-0.1.3/tidychef/lookup/engines/horizontal_condition.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/lookup/engines/within.py` & `tidychef-0.1.3/tidychef/lookup/engines/within.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/models/source/cell.py` & `tidychef-0.1.3/tidychef/models/source/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,14 +190,21 @@
     x: int
     y: int
 
     # Optional as some tabulated formats (eg csv) do not have
     # cell formatting.
     cellformat: Optional[CellFormatting] = None
 
+    def __post_init__(self):
+        """
+        We'll store the original value of the cell
+        for where a cell value has been changed.
+        """
+        self._original_value = self.value
+
     def is_blank(self, disregard_whitespace: bool = True):
         """
         Can the contents of the cell be regarded as blank
 
         :param disregard_whitespace: Flag so we can choose to treat
         cells with just whitespace as populated.
         """
```

### Comparing `tidychef-0.1.2/tidychef/models/source/table.py` & `tidychef-0.1.3/tidychef/models/source/table.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/notebook/preview/boundary.py` & `tidychef-0.1.3/tidychef/notebook/preview/boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional
+from typing import List
 
 from tidychef import datafuncs as dfc
 from tidychef.models.source.cell import Cell
 from tidychef.models.source.table import LiveTable
 
 
 class Boundary:
```

### Comparing `tidychef-0.1.2/tidychef/notebook/preview/html/components.py` & `tidychef-0.1.3/tidychef/notebook/preview/html/components.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/notebook/preview/html/constants.py` & `tidychef-0.1.3/tidychef/notebook/preview/html/constants.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/notebook/preview/html/main.py` & `tidychef-0.1.3/tidychef/notebook/preview/html/main.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/notebook/preview/html/table.py` & `tidychef-0.1.3/tidychef/notebook/preview/html/table.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/notebook/preview/html/tidy_data.py` & `tidychef-0.1.3/tidychef/notebook/preview/html/tidy_data.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/output/base.py` & `tidychef-0.1.3/tidychef/output/base.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/output/tidydata.py` & `tidychef-0.1.3/tidychef/output/tidydata.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 import tabulate
 from IPython.core.display import HTML, display
 
 from tidychef.column.base import BaseColumn
 from tidychef.exceptions import DroppingNonColumnError, MisalignedHeadersError
 from tidychef.lookup.engines.horizontal_condition import HorizontalCondition
+from tidychef.models.source.cell import VirtualCell
 from tidychef.models.source.table import LiveTable
 from tidychef.notebook.ipython import in_notebook
 from tidychef.notebook.preview.html.tidy_data import tidy_data_as_html_table_string
 from tidychef.output.base import BaseOutput
 from tidychef.utils.decorators import dontmutate
 
 
-
 class TidyData(BaseOutput):
     def __init__(
         self,
         observations: LiveTable,
         *columns,
         obs_apply: Callable = None,
         drop: Optional[List[str]] = None,
@@ -61,20 +61,21 @@
     def __get_representation(self):  # pragma: no cover
         """
         Representation logic shared by __str__ and __repr__
         """
         if not self._data:
             self._transform()
 
-        header_row = self._data[0]
-        data_rows = self._data[1:]
+        table_as_strings = self._data_as_table_of_strings()
+        header_row = table_as_strings[0]
+        data_rows = table_as_strings[1:]
 
         # If we're in a notebook, create a nice html display
         if in_notebook():
-            display(HTML(tidy_data_as_html_table_string(self._data)))
+            display(HTML(tidy_data_as_html_table_string(table_as_strings)))
             return ""
 
         # Else return something that'll make sense in a terminal
         return tabulate.tabulate(data_rows, headers=header_row)
 
     def __repr__(self):  # pragma: no cover
         return self.__get_representation()
@@ -82,14 +83,39 @@
     def __str__(self):  # pragma: no cover
         return self.__get_representation()
 
     def __len__(self):
         self._transform()
         return len(self._data)
 
+    def _data_as_table_of_strings(self) -> List[List[str]]:
+        """
+        Generates a table of strings from a table of Cells.
+
+        So turns something like this:
+
+        [
+         [ Cell(x=1, y=2, value="Ray"), Cell(x=41, y=2, value="Egon") ],
+         [ Cell(x=9, y=5, value="Peter"), Cell(x=0, y=12, value="Winston") ]
+        ]
+
+        Into something like this:
+
+        [
+         [ "Ray", "Egon" ],
+         [ "Peter", "Winston" ]
+        ]
+        """
+        string_table = []
+        self._transform()
+        for row in self._data:
+            string_row = [x.value for x in row]
+            string_table.append(string_row)
+        return string_table
+
     def to_dict(self) -> dict:
         """
         Outputs the TidyData as a pandas style dictionary, i.e
 
         {
             column1: [column1value1, column1value2, column1value3],
             column2: [column2value1, column2value2, column2value3],
@@ -98,22 +124,22 @@
         """
         self._transform()
         output_dict: Dict[str, List[str]] = {}
 
         count = 0
         translater: Dict[i, str] = {}
 
-        for column_name in self._data[0]:
-            output_dict[column_name] = []
-            translater[count] = column_name
+        for column_header_cell in self._data[0]:
+            output_dict[column_header_cell.value] = []
+            translater[count] = column_header_cell.value
             count += 1
 
         for row in self._data[1:]:
             for i, item in enumerate(row):
-                output_dict[translater[i]].append(item)
+                output_dict[translater[i]].append(item.value)
 
         return output_dict
 
     @staticmethod
     def from_tidy(*tidy_data_objects: TidyData) -> TidyData:
         """
         Creates a class:TidyData object from multiple class:TidyData objects
@@ -205,61 +231,72 @@
         Once this method has been ran, this internal
         representation can be accessed via "._data".
 
         This result is cached so future calls to transform
         will not repopulate this attribute and will be
         ignored.
         """
+
+        # Dev note:
+        # The key point here is we're assembling a table
+        # of Cell and VirtualCell objects, not a table
+        # of the strings that each represent.
+        # This is so we maintain provenance information
+        # regarding how and from where each value was
+        # acquired.
+
         if not self._data:
             grid = []
             drop_count = 0
 
             # Observations always has the table name so
             # spread it around to cover those columns that
             # are created via static methods.
             for column in self.columns:
                 column._table == self.observations._name
 
             # We need to carefully construct our lists of lists
             # such that the HorizontalCondition columns are created last
             # Ordering will be restored at the end via this list.
-            ordered_column_headers = [self.observations.label] + [
-                x.label for x in self.columns
-            ]
+            ordered_column_header_cells = [
+                VirtualCell(value=self.observations.label)
+            ] + [VirtualCell(value=x.label) for x in self.columns]
 
             # Obs label
             if self.observations.label in self.drop:
-                unordered_header_row = []
+                unordered_header_row_cells = []
                 drop_count += 1
             else:
-                unordered_header_row = [self.observations.label]
+                unordered_header_row_cells = [
+                    VirtualCell(value=self.observations.label)
+                ]
 
             # Standard Column labels
             for column in [
                 x for x in self.columns if not isinstance(x.engine, HorizontalCondition)
             ]:
                 if column.label not in self.drop:
-                    unordered_header_row.append(column.label)
+                    unordered_header_row_cells.append(VirtualCell(value=column.label))
                 else:
                     drop_count += 1
 
             # Horizontal Condition
             for column in [
                 x for x in self.columns if isinstance(x.engine, HorizontalCondition)
             ]:
                 if column.label not in self.drop:
-                    unordered_header_row.append(column.label)
+                    unordered_header_row_cells.append(VirtualCell(value=column.label))
                 else:
                     drop_count += 1
 
             # Conditional column labels
             header_row = []
-            for col in ordered_column_headers:
-                if col in unordered_header_row:
-                    header_row.append(col)
+            for column_header_cell in ordered_column_header_cells:
+                if column_header_cell in unordered_header_row_cells:
+                    header_row.append(column_header_cell)
 
             grid.append(header_row)
 
             # If user has opted to drop a column that does
             # not exist, we need to tell them.
             if drop_count != len(self.drop):
                 raise DroppingNonColumnError(
@@ -278,57 +315,53 @@
 
                 # note we ALWAYS want values in the column_value_dict
                 # regardless of whether we're dropping the column
                 column_value_dict: Dict[str, str] = {}
                 column_value_dict[self.observations.label] = observation.value
 
                 if self.observations.label not in self.drop:
-                    row_as_dict[self.observations.label] = (
-                        observation.value
-                        if not self.obs_apply
-                        else self.obs_apply(observation.value)
-                    )
+                    if self.obs_apply is not None:
+                        observation.value = self.obs_apply(observation.value)
+                    row_as_dict[self.observations.label] = observation
 
                 # Resolve the standard columns first
                 standard_columns = [
                     x
                     for x in self.columns
                     if not isinstance(x.engine, HorizontalCondition)
                 ]
                 for column in standard_columns:
-                    col_value = column.resolve_column_cell_from_obs_cell(
-                        observation
-                    ).value
-                    column_value_dict[column.label] = col_value
+                    column_cell = column.resolve_column_cell_from_obs_cell(observation)
+                    column_value_dict[column.label] = column_cell.value
                     if column.label not in self.drop:
-                        row_as_dict[column.label] = col_value
+                        row_as_dict[column.label] = column_cell
 
                 # Now we know the standard column values, resolve the
                 # horizontal conditions
                 condition_columns = [
                     x for x in self.columns if isinstance(x.engine, HorizontalCondition)
                 ]
                 priorities = set([x.engine.priority for x in condition_columns])
                 for i in priorities:
                     for column in condition_columns:
                         if column.engine.priority == i:
-                            col_value = column.resolve_column_cell_from_obs_cell(
+                            column_cell = column.resolve_column_cell_from_obs_cell(
                                 observation, column_value_dict
-                            ).value
+                            )
 
-                            column_value_dict[column.label] = col_value
+                            column_value_dict[column.label] = column_cell.value
                             if column.label not in self.drop:
-                                row_as_dict[column.label] = col_value
+                                row_as_dict[column.label] = column_cell
 
                 # Order for output
                 line = []
-                for col in ordered_column_headers:
-                    value_to_output = row_as_dict.get(col, None)
-                    if value_to_output is not None:
-                        line.append(value_to_output)
+                for column_cell in ordered_column_header_cells:
+                    cell_wanted = row_as_dict.get(column_cell.value, None)
+                    if cell_wanted is not None:
+                        line.append(cell_wanted)
 
                 grid.append(line)
 
             self._data = grid
 
     def to_csv(
         self,
@@ -348,16 +381,15 @@
         :param path: The location we want to output the
         csv to.
         :param write_headers: Whether or not to include the
         headers when writing to csv.
         :param write_mode: The mode with which to open
         the python file object. Defaults to "w".
         """
-        if not self._data:
-            self._transform()
+        self._transform()
 
         if not isinstance(path, (Path, str)):
             raise ValueError(
                 "To output to a file you must provide a pathlib.Path object or a str"
             )
 
         if isinstance(path, str):
@@ -366,15 +398,15 @@
         if not path.parent.exists():
             raise FileNotFoundError(
                 f'The specified output directory "{path.parent.absolute()}" for the file "{path.name}" does not exist.'
             )
 
         with open(path, write_mode) as csvfile:
             tidywriter = csv.writer(csvfile, **kwargs)
-            for i, row in enumerate(self._data):
+            for i, row in enumerate(self._data_as_table_of_strings()):
                 if i == 0 and not write_headers:
                     continue
                 tidywriter.writerow(row)
 
     def drop_duplicates(
         self,
         print_duplicates: bool = False,
@@ -398,17 +430,17 @@
         ]
 
         for row in self._data:
             if row not in unique:
                 unique.append(row)
             else:
                 if print_duplicates:  # pragma: no cover
-                    lines.append(",".join(row))
+                    lines.append(",".join([x.value for x in row]))
                 if csv_duplicate_path:
-                    non_unique.append(row)
+                    non_unique.append([x.value for x in row])
 
         if print_duplicates:  # pragma: no cover
             for line in lines:
                 print(line)
 
         if csv_duplicate_path:
             if not isinstance(csv_duplicate_path, Path):
```

### Comparing `tidychef-0.1.2/tidychef/selection/filters/README.md` & `tidychef-0.1.3/tidychef/selection/filters/README.md`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/selection/filters/common.py` & `tidychef-0.1.3/tidychef/selection/filters/common.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/selection/selectable.py` & `tidychef-0.1.3/tidychef/selection/selectable.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,28 +492,32 @@
         invalid value message.
         """
 
         validation_errors = []
         for cell in self.cells:
             if not validator(cell):
                 if raise_first_error:
-                    raise CellValidationError(f'''
+                    raise CellValidationError(
+                        f"""
 When making selections from table: {self.name} the
 following validation error was encountered:
 {validator.msg(cell)}
-                ''')
+                """
+                    )
                 else:
                     validation_errors.append(validator.msg(cell))
 
         if len(validation_errors) > 0:
-            raise CellValidationError(f'''
+            raise CellValidationError(
+                f"""
 When making selections from table: {self.name} the
 following validation errors were encountered:
 {linesep.join(validation_errors)}
-                ''')
+                """
+            )
 
         return self
 
     @dontmutate
     def filter(self, check: Callable):
         """
         Selects just the cells that match the provided check
@@ -534,15 +538,15 @@
     def re(self, pattern: str):
         """
         Filter the current selection of cells to only include
         cells whose value matches the provided regular expression
         pattern.
         """
 
-        matcher = re.compile(r'' + pattern)
+        matcher = re.compile(r"" + pattern)
         self.cells = [x for x in self.cells if matcher.match(x.value) is not None]
         _explain(self, f"Regex, pattern {pattern}")
         return self
 
     @dontmutate
     def waffle(self, direction: Direction, additional_selection: Selectable):
         """
```

### Comparing `tidychef-0.1.2/tidychef/utils/cellutils/excel.py` & `tidychef-0.1.3/tidychef/utils/cellutils/excel.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/utils/decorators/dontmutate.py` & `tidychef-0.1.3/tidychef/utils/decorators/dontmutate.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/tidychef/utils/fileutils/paths.py` & `tidychef-0.1.3/tidychef/utils/fileutils/paths.py`

 * *Files identical despite different names*

### Comparing `tidychef-0.1.2/setup.py` & `tidychef-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['tidychef',
  'tidychef.acquire',
  'tidychef.acquire.csv',
+ 'tidychef.acquire.ods',
  'tidychef.acquire.python',
  'tidychef.acquire.xls',
  'tidychef.acquire.xlsx',
  'tidychef.against',
  'tidychef.against.implementations',
  'tidychef.column',
  'tidychef.datafuncs',
@@ -21,40 +22,43 @@
  'tidychef.notebook',
  'tidychef.notebook.preview',
  'tidychef.notebook.preview.html',
  'tidychef.output',
  'tidychef.selection',
  'tidychef.selection.csv',
  'tidychef.selection.filters',
+ 'tidychef.selection.ods',
  'tidychef.selection.xls',
  'tidychef.selection.xlsx',
  'tidychef.utils',
  'tidychef.utils.cellutils',
  'tidychef.utils.decorators',
  'tidychef.utils.fileutils',
  'tidychef.utils.http']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cachecontrol>=0.13.1,<0.14.0',
+ 'ezodf>=0.3.2,<0.4.0',
  'filelock>=3.12.2,<4.0.0',
  'jupyter>=1.0.0,<2.0.0',
+ 'lxml>=4.9.3,<5.0.0',
  'openpyxl>=3.1.2,<4.0.0',
  'requests>=2.31.0,<3.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'validators>=0.20.0,<0.21.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'tidychef',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python framework for transforming tabulated data with visual relationships into tidy data',
-    'long_description': '# Tidychef\n\n![Tests](https://github.com/mikeAdamss/tidychef/actions/workflows/tests.yml/badge.svg)\n![100% Test Coverage](./jupyterbook/images/coverage-100.svg)\n![Static Badge](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)\n\nTidychef is a python framework to enable “data extraction for humans” via simple python beginner friendly "recipes". It aims at allowing users to easily transform tabulated data sources that use visual relationships (human readable only data) into simple machine readable "tidy data" in a repeatable way.\n\ni.e: it allows you to reliably turn something that looks like this: \n\n![](https://mikeadamss.github.io/tidychef/_images/bands-before.png)\n\ninto something that looks like this:\n\n![](https://mikeadamss.github.io/tidychef/_images/bands-after.png)\n_Note: image cropped for reasons of practicality._\n\nTidychef is **designed to allow even novice python users or analysts to quickly become productive** but also has an advanced feature set and is designed to be readily and easily extended (adding new source of tabulated data, your own use case specific methods and filters and domain specific validation etc are all possible and documented in detail).\n\nIn depth training material, examples and technical documentation [can be found here](https://mikeadamss.github.io/tidychef/intro.html#).\n\n## Installation\n\n```\npip install tidychef\n```\n\n## Acknowlagements\n\nTidychef is directly inspired by the python package [databaker](https://github.com/sensiblecodeio/databaker) created by [The Sensible Code Company](https://sensiblecode.io/) in partnership with the United Kingdoms [Office For National Statistics](https://www.ons.gov.uk/).\n\nWhile I liked [databaker](https://github.com/sensiblecodeio/databaker) and successfully worked with it on multiple ETL projects over the course of almost a decade, this software should be considered the culmination of that work and the lessons learned from that time.',
+    'long_description': '# Tidychef\n\n![Tests](https://github.com/mikeAdamss/tidychef/actions/workflows/tests.yml/badge.svg)\n![100% Test Coverage](./jupyterbook/images/coverage-100.svg)\n![Static Badge](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)\n\nTidychef is a python framework to enable “data extraction for humans” via simple python beginner friendly "recipes". It aims at allowing users to easily transform tabulated data sources that use visual relationships (human readable only data) into simple machine readable "tidy data" in a repeatable way.\n\ni.e: it allows you to reliably turn something that looks like this: \n\n![](https://mikeadamss.github.io/tidychef/_images/bands-before.png)\n\ninto something that looks like this:\n\n![](https://mikeadamss.github.io/tidychef/_images/bands-after.png)\n_Note: image cropped for reasons of practicality._\n\nCurrently supported input formats are `xls`, `xlsx`, `ods` and `csv`. Though users can add additional formats relatively easily and without a codebase change being necessary.\n\nTidychef is **designed to allow even novice python users or analysts to quickly become productive** but also has an advanced feature set and is designed to be readily and easily extended (adding new source of tabulated data, your own use case specific methods and filters and domain specific validation etc are all possible and documented in detail).\n\nIn depth training material, examples and technical documentation [can be found here](https://mikeadamss.github.io/tidychef/intro.html#).\n\n## Installation\n\n```\npip install tidychef\n```\n\n## Acknowledgements\n\nTidychef is directly inspired by the python package [databaker](https://github.com/sensiblecodeio/databaker) created by [The Sensible Code Company](https://sensiblecode.io/) in partnership with the United Kingdoms [Office For National Statistics](https://www.ons.gov.uk/).\n\nWhile I liked [databaker](https://github.com/sensiblecodeio/databaker) and successfully worked with it on multiple ETL projects over the course of almost a decade, this software should be considered the culmination of that work and the lessons learned from that time.',
     'author': 'mikeAdamss',
     'author_email': 'mikelovesbooks@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mikeAdamss/tidychef',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tidychef-0.1.2/PKG-INFO` & `tidychef-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: tidychef
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python framework for transforming tabulated data with visual relationships into tidy data
 Home-page: https://github.com/mikeAdamss/tidychef
 License: Apache 2.0
 Author: mikeAdamss
 Author-email: mikelovesbooks@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachecontrol (>=0.13.1,<0.14.0)
+Requires-Dist: ezodf (>=0.3.2,<0.4.0)
 Requires-Dist: filelock (>=3.12.2,<4.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/mikeAdamss/tidychef
 Description-Content-Type: text/markdown
@@ -38,22 +40,24 @@
 ![](https://mikeadamss.github.io/tidychef/_images/bands-before.png)
 
 into something that looks like this:
 
 ![](https://mikeadamss.github.io/tidychef/_images/bands-after.png)
 _Note: image cropped for reasons of practicality._
 
+Currently supported input formats are `xls`, `xlsx`, `ods` and `csv`. Though users can add additional formats relatively easily and without a codebase change being necessary.
+
 Tidychef is **designed to allow even novice python users or analysts to quickly become productive** but also has an advanced feature set and is designed to be readily and easily extended (adding new source of tabulated data, your own use case specific methods and filters and domain specific validation etc are all possible and documented in detail).
 
 In depth training material, examples and technical documentation [can be found here](https://mikeadamss.github.io/tidychef/intro.html#).
 
 ## Installation
 
 ```
 pip install tidychef
 ```
 
-## Acknowlagements
+## Acknowledgements
 
 Tidychef is directly inspired by the python package [databaker](https://github.com/sensiblecodeio/databaker) created by [The Sensible Code Company](https://sensiblecode.io/) in partnership with the United Kingdoms [Office For National Statistics](https://www.ons.gov.uk/).
 
 While I liked [databaker](https://github.com/sensiblecodeio/databaker) and successfully worked with it on multiple ETL projects over the course of almost a decade, this software should be considered the culmination of that work and the lessons learned from that time.
```

