# Comparing `tmp/xiaobaisaf-2.3.7.tar.gz` & `tmp/xiaobaisaf-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobaisaf-2.3.7.tar", last modified: Sat Jul 29 14:10:06 2023, max compression
+gzip compressed data, was "xiaobaisaf-2.3.8.tar", last modified: Sat Jul 29 16:24:15 2023, max compression
```

## Comparing `xiaobaisaf-2.3.7.tar` & `xiaobaisaf-2.3.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.486052 xiaobaisaf-2.3.7/
--rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.7/LICENSE
--rw-rw-rw-   0        0        0    12938 2023-07-29 14:10:06.486052 xiaobaisaf-2.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    12267 2023-07-29 14:08:28.000000 xiaobaisaf-2.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.438126 xiaobaisaf-2.3.7/saf/
--rw-rw-rw-   0        0        0     1527 2023-07-29 13:56:45.000000 xiaobaisaf-2.3.7/saf/__init__.py
--rw-rw-rw-   0        0        0      152 2023-07-29 14:00:20.000000 xiaobaisaf-2.3.7/saf/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.441088 xiaobaisaf-2.3.7/saf/data/
--rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.7/saf/data/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/data/config.py
--rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/data/favicon.ico
--rw-rw-rw-   0        0        0     1201 2023-06-26 08:03:27.000000 xiaobaisaf-2.3.7/saf/data/software_check.sh
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.442085 xiaobaisaf-2.3.7/saf/example/
--rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.444080 xiaobaisaf-2.3.7/saf/example/api/
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.446074 xiaobaisaf-2.3.7/saf/example/api/Config/
--rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Config/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Config/config.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.447072 xiaobaisaf-2.3.7/saf/example/api/TestCases/
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/TestCases/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/TestCases/test_one_html_case_template.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.452087 xiaobaisaf-2.3.7/saf/example/api/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/api_client.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/logger.py
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/run.py
--rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/send_email_script.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.452087 xiaobaisaf-2.3.7/saf/example/web/
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.458126 xiaobaisaf-2.3.7/saf/example/web/Cases/
--rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/__init__.py
--rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/conftest.py
--rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_allure.py
--rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_submitBug.py
--rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v1.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v2.py
--rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v3.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.462115 xiaobaisaf-2.3.7/saf/example/web/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/logger.py
--rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.463113 xiaobaisaf-2.3.7/saf/example/web/pageObject/
--rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/pageObject/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/pageObject/register_page_element.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.480067 xiaobaisaf-2.3.7/saf/utils/
--rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/BugUtils.py
--rw-rw-rw-   0        0        0     2651 2023-07-29 14:10:05.000000 xiaobaisaf-2.3.7/saf/utils/CaptchaUtils.py
--rw-rw-rw-   0        0        0     4132 2023-07-26 17:29:54.000000 xiaobaisaf-2.3.7/saf/utils/Demo.py
--rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/ElementUtils.py
--rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidDeviceGUI.py
--rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageCLI.py
--rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageGUI.py
--rw-rw-rw-   0        0        0    10701 2023-07-22 18:26:01.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackagePower.py
--rw-rw-rw-   0        0        0     1583 2023-07-21 15:26:19.000000 xiaobaisaf-2.3.7/saf/utils/MonitorCANBus.py
--rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/utils/MonitorDBs.py
--rw-rw-rw-   0        0        0    11552 2023-07-21 15:48:01.000000 xiaobaisaf-2.3.7/saf/utils/Selenium2POM.py
--rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/SendMsgUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/utils/YamlUtils.py
--rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.7/saf/utils/__init__.py
--rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/utils/downloadUtils.py
--rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/networkSpeedUtils.py
--rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.7/saf/utils/osEnvUtils.py
--rw-rw-rw-   0        0        0     2549 2023-07-29 13:43:39.000000 xiaobaisaf-2.3.7/saf/utils/xiaobaicmd.py
--rw-rw-rw-   0        0        0       42 2023-07-29 14:10:06.487048 xiaobaisaf-2.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2514 2023-07-06 16:41:30.000000 xiaobaisaf-2.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.485054 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/
--rw-rw-rw-   0        0        0    12938 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      154 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.516886 xiaobaisaf-2.3.8/
+-rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.8/LICENSE
+-rw-rw-rw-   0        0        0    13239 2023-07-29 16:24:15.516886 xiaobaisaf-2.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12568 2023-07-29 16:23:12.000000 xiaobaisaf-2.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.474000 xiaobaisaf-2.3.8/saf/
+-rw-rw-rw-   0        0        0     1527 2023-07-29 14:13:17.000000 xiaobaisaf-2.3.8/saf/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-07-29 14:51:28.000000 xiaobaisaf-2.3.8/saf/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.476992 xiaobaisaf-2.3.8/saf/data/
+-rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.8/saf/data/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.8/saf/data/config.py
+-rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.8/saf/data/favicon.ico
+-rw-rw-rw-   0        0        0     1201 2023-06-26 08:03:27.000000 xiaobaisaf-2.3.8/saf/data/software_check.sh
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.477990 xiaobaisaf-2.3.8/saf/example/
+-rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.480982 xiaobaisaf-2.3.8/saf/example/api/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.481979 xiaobaisaf-2.3.8/saf/example/api/Config/
+-rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/Config/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/Config/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.483974 xiaobaisaf-2.3.8/saf/example/api/TestCases/
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/TestCases/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/TestCases/test_one_html_case_template.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.486966 xiaobaisaf-2.3.8/saf/example/api/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/api/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/Utils/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/api/Utils/api_client.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/api/Utils/logger.py
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/run.py
+-rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/api/send_email_script.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.487963 xiaobaisaf-2.3.8/saf/example/web/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.492950 xiaobaisaf-2.3.8/saf/example/web/Cases/
+-rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/conftest.py
+-rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_allure.py
+-rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_submitBug.py
+-rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_v1.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_v2.py
+-rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_v3.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.495941 xiaobaisaf-2.3.8/saf/example/web/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/web/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/web/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/web/Utils/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.8/saf/example/web/Utils/logger.py
+-rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.497936 xiaobaisaf-2.3.8/saf/example/web/pageObject/
+-rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/pageObject/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/example/web/pageObject/register_page_element.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.510902 xiaobaisaf-2.3.8/saf/utils/
+-rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.8/saf/utils/BugUtils.py
+-rw-rw-rw-   0        0        0     3849 2023-07-29 16:18:29.000000 xiaobaisaf-2.3.8/saf/utils/CaptchaUtils.py
+-rw-rw-rw-   0        0        0      128 2023-07-29 16:11:56.000000 xiaobaisaf-2.3.8/saf/utils/Demo.py
+-rw-rw-rw-   0        0        0     1271 2023-07-29 14:13:17.000000 xiaobaisaf-2.3.8/saf/utils/ElementUtils.py
+-rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.8/saf/utils/MonitorAndroidDeviceGUI.py
+-rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.8/saf/utils/MonitorAndroidPackageCLI.py
+-rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.8/saf/utils/MonitorAndroidPackageGUI.py
+-rw-rw-rw-   0        0        0    10705 2023-07-29 14:13:17.000000 xiaobaisaf-2.3.8/saf/utils/MonitorAndroidPackagePower.py
+-rw-rw-rw-   0        0        0     1583 2023-07-21 15:26:19.000000 xiaobaisaf-2.3.8/saf/utils/MonitorCANBus.py
+-rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.8/saf/utils/MonitorDBs.py
+-rw-rw-rw-   0        0        0    11999 2023-07-29 14:13:17.000000 xiaobaisaf-2.3.8/saf/utils/Selenium2POM.py
+-rw-rw-rw-   0        0        0     2694 2023-07-29 14:13:17.000000 xiaobaisaf-2.3.8/saf/utils/SendMsgUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.8/saf/utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.8/saf/utils/__init__.py
+-rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.8/saf/utils/downloadUtils.py
+-rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.8/saf/utils/networkSpeedUtils.py
+-rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.8/saf/utils/osEnvUtils.py
+-rw-rw-rw-   0        0        0     2549 2023-07-29 14:13:17.000000 xiaobaisaf-2.3.8/saf/utils/xiaobaicmd.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:24:15.516886 xiaobaisaf-2.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2514 2023-07-06 16:41:30.000000 xiaobaisaf-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:24:15.515888 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/
+-rw-rw-rw-   0        0        0    13239 2023-07-29 16:24:15.000000 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2023-07-29 16:24:15.000000 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:24:15.000000 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-29 16:24:15.000000 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      154 2023-07-29 16:24:15.000000 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-29 16:24:15.000000 xiaobaisaf-2.3.8/xiaobaisaf.egg-info/top_level.txt
```

### Comparing `xiaobaisaf-2.3.7/LICENSE` & `xiaobaisaf-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/PKG-INFO` & `xiaobaisaf-2.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.7
+Version: 2.3.8
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -23,16 +23,16 @@
 
 ### 版本注意
     尽量使用Python 3.9.* 版本
     防止某些库出现不兼容问题，导致功能不可使用
 
 ### 安装教程
 ```commandline
-pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple    注：将pip源修改为国内源
-pip install saf
+pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple   注：将pip源修改为国内源
+pip install xiaobaisaf
 ```
 
 ### 使用说明
 - 优先修改saf/data/config.py中飞书/钉钉的webhook
 ```python
 # filename=config.py
 
@@ -46,15 +46,15 @@
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
 
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
-from saf.utils.SendMsgUtils import robotSendMessage
+from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item):
     """
     :param item:
     """
@@ -286,37 +286,41 @@
 
 ### saf>2.2   基础adb实现Android设备的电量监控功能
 ```cmd
 xiaobaicmd -m power   # 界面监控设备的电量与内存使用率的实时界面
 xiaobaicmd -m memory   # 界面监控设备的电量与内存使用率的实时界面
 ```
 
-### saf>2.3.5   新增实时监控Android当前APP的CPU使用率及FPS数据
+### saf>2.3.5 新增实时监控Android当前APP的CPU使用率及FPS数据
 ```cmd
-xiaobaicmd -m gui   
+xiaobaicmd -m gui
 ```
 
-### saf>2.3.6   新增识别滑块验证码破解
+### saf>2.3.7 新增识别滑块验证码破解
 ```python
 from saf.utils.CaptchaUtils import checkSlider
 from saf import selenium_webdriver, By
 
 driver = selenium_webdriver.Chrome()
 
 driver.get("https://www.xiaobaisoftware.com")
 
 # 其它操作...
 
+# 定位目标图（小图）
 target_element = driver.find_element(By.XPATH, value='')
 
+# 定位背景图（大图）
 background_element = driver.find_element(By.XPATH, value='')
 
+# 定位滑块按钮
 button_element = driver.find_element(By.XPATH, value='')
 
-checkSlider(driver, target_element, background_element, button_element)
+# 参数：浏览器驱动、目标元素、背景元素、滑块元素、失败重试（非必须，默认：False）、重试次数（非必须，默认：3）
+checkSlider(driver, target_element, background_element, button_element, True, 5)
 ```
 
 ### 环境检测[还未实现]
 ```bat
 xiaobaicmd  --init
 
 检测内容: 
@@ -344,29 +348,30 @@
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
 | version | info                            |
-|---------|---------------------------------|
-| 1.0     | 基本实现web自动化模板功能                  |
-| 1.1     | fix上个版本的BUG                     |
-| 1.2     | 新增allure报告库及封装禅道提单接口            |
-| 1.3     | 新增jira提单接口                      |
-| 1.4     | 新增pytest参数化样例                   |
-| 1.5     | 优化pytest样例内容                    |
-| 1.6     | 优化                              |
-| 1.7     | 新增基础环境检测功能                      |
-| 1.8     | 新增API自动化模板                      |
-| 1.9     | 新增xiaobaicmd -u命令               |
-| 2.0     | 新增xiaobaicmd -m命令               |
-| 2.1     | 新增xiaobaicmd --device命令         |
-| 2.2     | 优化xiaobaicmd --device命令         |
-| 2.3     | 新增实时监控Android设备耗电量              |
-| 2.3.1   | fix                             |
-| 2.3.2   | fix                             |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
-| 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
-| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
-| 2.3.6   | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
-| 2.3.7   | 新增识别滑块验证码破解                     |
+|--------|---------------------------------|
+| 1.0    | 基本实现web自动化模板功能                  |
+| 1.1    | fix上个版本的BUG                     |
+| 1.2    | 新增allure报告库及封装禅道提单接口            |
+| 1.3    | 新增jira提单接口                      |
+| 1.4    | 新增pytest参数化样例                   |
+| 1.5    | 优化pytest样例内容                    |
+| 1.6    | 优化                              |
+| 1.7    | 新增基础环境检测功能                      |
+| 1.8    | 新增API自动化模板                      |
+| 1.9    | 新增xiaobaicmd -u命令               |
+| 2.0    | 新增xiaobaicmd -m命令               |
+| 2.1    | 新增xiaobaicmd --device命令         |
+| 2.2    | 优化xiaobaicmd --device命令         |
+| 2.3    | 新增实时监控Android设备耗电量              |
+| 2.3.1  | fix                             |
+| 2.3.2  | fix                             |
+| 2.3.3  | 新增实时监控Android当前APP的内存使用率        |
+| 2.3.4  | 优化xiaobaicmd -m gui效果展示         |
+| 2.3.5  | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.6  | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
+| 2.3.7  | 新增识别滑块验证码破解                     |
+| 2.3.8  | 优化识别滑块验证码破解                     |
```

### Comparing `xiaobaisaf-2.3.7/README.md` & `xiaobaisaf-2.3.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 ### 版本注意
     尽量使用Python 3.9.* 版本
     防止某些库出现不兼容问题，导致功能不可使用
 
 ### 安装教程
 ```commandline
-pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple    注：将pip源修改为国内源
-pip install saf
+pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple   注：将pip源修改为国内源
+pip install xiaobaisaf
 ```
 
 ### 使用说明
 - 优先修改saf/data/config.py中飞书/钉钉的webhook
 ```python
 # filename=config.py
 
@@ -34,15 +34,15 @@
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
 
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
-from saf.utils.SendMsgUtils import robotSendMessage
+from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item):
     """
     :param item:
     """
@@ -274,37 +274,41 @@
 
 ### saf>2.2   基础adb实现Android设备的电量监控功能
 ```cmd
 xiaobaicmd -m power   # 界面监控设备的电量与内存使用率的实时界面
 xiaobaicmd -m memory   # 界面监控设备的电量与内存使用率的实时界面
 ```
 
-### saf>2.3.5   新增实时监控Android当前APP的CPU使用率及FPS数据
+### saf>2.3.5 新增实时监控Android当前APP的CPU使用率及FPS数据
 ```cmd
-xiaobaicmd -m gui   
+xiaobaicmd -m gui
 ```
 
-### saf>2.3.6   新增识别滑块验证码破解
+### saf>2.3.7 新增识别滑块验证码破解
 ```python
 from saf.utils.CaptchaUtils import checkSlider
 from saf import selenium_webdriver, By
 
 driver = selenium_webdriver.Chrome()
 
 driver.get("https://www.xiaobaisoftware.com")
 
 # 其它操作...
 
+# 定位目标图（小图）
 target_element = driver.find_element(By.XPATH, value='')
 
+# 定位背景图（大图）
 background_element = driver.find_element(By.XPATH, value='')
 
+# 定位滑块按钮
 button_element = driver.find_element(By.XPATH, value='')
 
-checkSlider(driver, target_element, background_element, button_element)
+# 参数：浏览器驱动、目标元素、背景元素、滑块元素、失败重试（非必须，默认：False）、重试次数（非必须，默认：3）
+checkSlider(driver, target_element, background_element, button_element, True, 5)
 ```
 
 ### 环境检测[还未实现]
 ```bat
 xiaobaicmd  --init
 
 检测内容: 
@@ -332,29 +336,30 @@
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
 | version | info                            |
-|---------|---------------------------------|
-| 1.0     | 基本实现web自动化模板功能                  |
-| 1.1     | fix上个版本的BUG                     |
-| 1.2     | 新增allure报告库及封装禅道提单接口            |
-| 1.3     | 新增jira提单接口                      |
-| 1.4     | 新增pytest参数化样例                   |
-| 1.5     | 优化pytest样例内容                    |
-| 1.6     | 优化                              |
-| 1.7     | 新增基础环境检测功能                      |
-| 1.8     | 新增API自动化模板                      |
-| 1.9     | 新增xiaobaicmd -u命令               |
-| 2.0     | 新增xiaobaicmd -m命令               |
-| 2.1     | 新增xiaobaicmd --device命令         |
-| 2.2     | 优化xiaobaicmd --device命令         |
-| 2.3     | 新增实时监控Android设备耗电量              |
-| 2.3.1   | fix                             |
-| 2.3.2   | fix                             |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
-| 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
-| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
-| 2.3.6   | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
-| 2.3.7   | 新增识别滑块验证码破解                     |
+|--------|---------------------------------|
+| 1.0    | 基本实现web自动化模板功能                  |
+| 1.1    | fix上个版本的BUG                     |
+| 1.2    | 新增allure报告库及封装禅道提单接口            |
+| 1.3    | 新增jira提单接口                      |
+| 1.4    | 新增pytest参数化样例                   |
+| 1.5    | 优化pytest样例内容                    |
+| 1.6    | 优化                              |
+| 1.7    | 新增基础环境检测功能                      |
+| 1.8    | 新增API自动化模板                      |
+| 1.9    | 新增xiaobaicmd -u命令               |
+| 2.0    | 新增xiaobaicmd -m命令               |
+| 2.1    | 新增xiaobaicmd --device命令         |
+| 2.2    | 优化xiaobaicmd --device命令         |
+| 2.3    | 新增实时监控Android设备耗电量              |
+| 2.3.1  | fix                             |
+| 2.3.2  | fix                             |
+| 2.3.3  | 新增实时监控Android当前APP的内存使用率        |
+| 2.3.4  | 优化xiaobaicmd -m gui效果展示         |
+| 2.3.5  | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.6  | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
+| 2.3.7  | 新增识别滑块验证码破解                     |
+| 2.3.8  | 优化识别滑块验证码破解                     |
```

### Comparing `xiaobaisaf-2.3.7/saf/__init__.py` & `xiaobaisaf-2.3.8/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/data/config.py` & `xiaobaisaf-2.3.8/saf/data/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/data/favicon.ico` & `xiaobaisaf-2.3.8/saf/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/data/software_check.sh` & `xiaobaisaf-2.3.8/saf/data/software_check.sh`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/Config/config.py` & `xiaobaisaf-2.3.8/saf/example/api/Config/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/TestCases/test_one_html_case_template.py` & `xiaobaisaf-2.3.8/saf/example/api/TestCases/test_one_html_case_template.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.8/saf/example/api/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/Utils/YamlUtils.py` & `xiaobaisaf-2.3.8/saf/example/api/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/Utils/api_client.py` & `xiaobaisaf-2.3.8/saf/example/api/Utils/api_client.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/run.py` & `xiaobaisaf-2.3.8/saf/example/api/run.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/api/send_email_script.py` & `xiaobaisaf-2.3.8/saf/example/api/send_email_script.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/web/Cases/conftest.py` & `xiaobaisaf-2.3.8/saf/example/web/Cases/conftest.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_allure.py` & `xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_allure.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_submitBug.py` & `xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_submitBug.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v2.py` & `xiaobaisaf-2.3.8/saf/example/web/Cases/test_xiaobai_case_v2.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/web/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.8/saf/example/web/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/example/web/Utils/YamlUtils.py` & `xiaobaisaf-2.3.8/saf/example/web/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/BugUtils.py` & `xiaobaisaf-2.3.8/saf/utils/BugUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/ElementUtils.py` & `xiaobaisaf-2.3.8/saf/utils/ElementUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidDeviceGUI.py` & `xiaobaisaf-2.3.8/saf/utils/MonitorAndroidDeviceGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageCLI.py` & `xiaobaisaf-2.3.8/saf/utils/MonitorAndroidPackageCLI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageGUI.py` & `xiaobaisaf-2.3.8/saf/utils/MonitorAndroidPackageGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackagePower.py` & `xiaobaisaf-2.3.8/saf/utils/MonitorAndroidPackagePower.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,9 +213,9 @@
             self.label_fps_rate.config(text=f'FPS刷新率[红线]：{current_fps_rate}/s')
 
 def power():
     root = tk.Tk()
     app = App(root)
     root.mainloop()
 
-if __name__ == '__main__':
-    power()
+# if __name__ == '__main__':
+#     power()
```

### Comparing `xiaobaisaf-2.3.7/saf/utils/MonitorCANBus.py` & `xiaobaisaf-2.3.8/saf/utils/MonitorCANBus.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/MonitorDBs.py` & `xiaobaisaf-2.3.8/saf/utils/MonitorDBs.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/Selenium2POM.py` & `xiaobaisaf-2.3.8/saf/utils/Selenium2POM.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 from selenium.common.exceptions import NoSuchWindowException
 
 
 class PageListener:
     def __init__(self, start_url: str = 'https://www.baidu.com', dirname: str = '.', rewrite: bool = True):
         '''
         基于Selenium基础操作过程中将每页内容转为POM
-        :param to_str       : True将结果转为字符串返回 ,False将结果写入到脚本，自动输出到Pages包中
+        :param start_url   : 首页地址
+        :param dirname     : 目录
+        :param rewrite     : 是否覆盖目录
+        :return
         '''
         self.PY_FILE_NAME_LIST = []
         if rewrite and path.exists(f'{dirname}/Pages'):
             try:
                 remove(f'{dirname}/Pages')
             except PermissionError as e:
                 pass
@@ -99,14 +102,20 @@
                     self.PageHandles = self.driver.window_handles
             except KeyboardInterrupt as e:
                 exit(-1)
             except NoSuchWindowException as e:
                 exit(-2)
 
     def code2file(self, code: str, filename: str = None):
+        '''
+        将代码写入文件
+        :param code:
+        :param filename:
+        :return:
+        '''
         with open(filename, 'w', encoding='UTF-8') as f:
             f.write(code)
             f.close()
             del f
 
     def identify_inputs_and_buttons(self, url, html):
         '''
@@ -138,14 +147,19 @@
             button_list.append({'tag': button_tag, 'name': button_name, 'xpath': button_xpath})
         title = '_'.join(lazy_pinyin(soup.select("title")[0].text)).upper()
         title = ''.join(re.findall('[0-9a-zA-Z_]+', title))
         return self.converter(page_name=title, url=url,
                               input_list=input_list, button_list=button_list)
 
     def get_xpath(self, element):
+        '''
+        获取xpath表达式
+        :param element:
+        :return:
+        '''
         components = []
         child = element
         while child is not None:
             siblings = child.find_previous_siblings()
             index = len(siblings) + 1
             if child.name == 'html':
                 components.insert(0, '/html')
@@ -169,14 +183,22 @@
             components.insert(0, f'/{child.name}[{index}]')
             child = child.parent
         xpath = ''.join(components)
         xpath = xpath if xpath.startswith('/html') else '/' + xpath
         return xpath
 
     def converter(self, page_name: str, url: str, input_list: list, button_list: list):
+        '''
+        将输入框与按钮等转为POM代码
+        :param page_name:
+        :param url:
+        :param input_list:
+        :param button_list:
+        :return:
+        '''
         function_strings = []
         function_names = []
         function_strings.append('#! /usr/bin/env python')
         function_strings.append(f'')
         function_strings.append('#********************************#')
         function_strings.append('#    欢迎使用自动生成POM代码工具      #')
         function_strings.append('#      Auther:xiaobaiTser        #')
@@ -217,9 +239,9 @@
             button_item['tag'] = str(button_item['tag']).replace('\n', '\n\t\t')
             function_strings.append(f"\t\t{button_item['tag']}")
             function_strings.append("\t\t'''")
             function_strings.append(f'\t\tself.driver.find_element(By.XPATH, \'{xpath}\').click()')
             function_strings.append(f'')
         return '\n'.join(function_strings)
 
-if __name__ == '__main__':
-    PageListener(start_url='https://www.zhiguanpo.com/#/')
+# if __name__ == '__main__':
+#     PageListener(start_url='http://192.168.0.240:9800/login')
```

### Comparing `xiaobaisaf-2.3.7/saf/utils/SendMsgUtils.py` & `xiaobaisaf-2.3.8/saf/utils/SendMsgUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/YamlUtils.py` & `xiaobaisaf-2.3.8/saf/utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/downloadUtils.py` & `xiaobaisaf-2.3.8/saf/utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/networkSpeedUtils.py` & `xiaobaisaf-2.3.8/saf/utils/networkSpeedUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/saf/utils/xiaobaicmd.py` & `xiaobaisaf-2.3.8/saf/utils/xiaobaicmd.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/setup.py` & `xiaobaisaf-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.7/xiaobaisaf.egg-info/PKG-INFO` & `xiaobaisaf-2.3.8/xiaobaisaf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.7
+Version: 2.3.8
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -23,16 +23,16 @@
 
 ### 版本注意
     尽量使用Python 3.9.* 版本
     防止某些库出现不兼容问题，导致功能不可使用
 
 ### 安装教程
 ```commandline
-pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple    注：将pip源修改为国内源
-pip install saf
+pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple   注：将pip源修改为国内源
+pip install xiaobaisaf
 ```
 
 ### 使用说明
 - 优先修改saf/data/config.py中飞书/钉钉的webhook
 ```python
 # filename=config.py
 
@@ -46,15 +46,15 @@
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
 
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
-from saf.utils.SendMsgUtils import robotSendMessage
+from saf.utils.sendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item):
     """
     :param item:
     """
@@ -286,37 +286,41 @@
 
 ### saf>2.2   基础adb实现Android设备的电量监控功能
 ```cmd
 xiaobaicmd -m power   # 界面监控设备的电量与内存使用率的实时界面
 xiaobaicmd -m memory   # 界面监控设备的电量与内存使用率的实时界面
 ```
 
-### saf>2.3.5   新增实时监控Android当前APP的CPU使用率及FPS数据
+### saf>2.3.5 新增实时监控Android当前APP的CPU使用率及FPS数据
 ```cmd
-xiaobaicmd -m gui   
+xiaobaicmd -m gui
 ```
 
-### saf>2.3.6   新增识别滑块验证码破解
+### saf>2.3.7 新增识别滑块验证码破解
 ```python
 from saf.utils.CaptchaUtils import checkSlider
 from saf import selenium_webdriver, By
 
 driver = selenium_webdriver.Chrome()
 
 driver.get("https://www.xiaobaisoftware.com")
 
 # 其它操作...
 
+# 定位目标图（小图）
 target_element = driver.find_element(By.XPATH, value='')
 
+# 定位背景图（大图）
 background_element = driver.find_element(By.XPATH, value='')
 
+# 定位滑块按钮
 button_element = driver.find_element(By.XPATH, value='')
 
-checkSlider(driver, target_element, background_element, button_element)
+# 参数：浏览器驱动、目标元素、背景元素、滑块元素、失败重试（非必须，默认：False）、重试次数（非必须，默认：3）
+checkSlider(driver, target_element, background_element, button_element, True, 5)
 ```
 
 ### 环境检测[还未实现]
 ```bat
 xiaobaicmd  --init
 
 检测内容: 
@@ -344,29 +348,30 @@
 [163邮箱配置](http://help.163.com/09/1223/14/5R7P3QI100753VB8.html, "163邮箱配置")
 
 [QQ邮箱配置](https://service.mail.qq.com/cgi-bin/help?subtype=1&id=28&no=369, "QQ邮箱配置")
 
 ### 更新日志
 
 | version | info                            |
-|---------|---------------------------------|
-| 1.0     | 基本实现web自动化模板功能                  |
-| 1.1     | fix上个版本的BUG                     |
-| 1.2     | 新增allure报告库及封装禅道提单接口            |
-| 1.3     | 新增jira提单接口                      |
-| 1.4     | 新增pytest参数化样例                   |
-| 1.5     | 优化pytest样例内容                    |
-| 1.6     | 优化                              |
-| 1.7     | 新增基础环境检测功能                      |
-| 1.8     | 新增API自动化模板                      |
-| 1.9     | 新增xiaobaicmd -u命令               |
-| 2.0     | 新增xiaobaicmd -m命令               |
-| 2.1     | 新增xiaobaicmd --device命令         |
-| 2.2     | 优化xiaobaicmd --device命令         |
-| 2.3     | 新增实时监控Android设备耗电量              |
-| 2.3.1   | fix                             |
-| 2.3.2   | fix                             |
-| 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
-| 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
-| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
-| 2.3.6   | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
-| 2.3.7   | 新增识别滑块验证码破解                     |
+|--------|---------------------------------|
+| 1.0    | 基本实现web自动化模板功能                  |
+| 1.1    | fix上个版本的BUG                     |
+| 1.2    | 新增allure报告库及封装禅道提单接口            |
+| 1.3    | 新增jira提单接口                      |
+| 1.4    | 新增pytest参数化样例                   |
+| 1.5    | 优化pytest样例内容                    |
+| 1.6    | 优化                              |
+| 1.7    | 新增基础环境检测功能                      |
+| 1.8    | 新增API自动化模板                      |
+| 1.9    | 新增xiaobaicmd -u命令               |
+| 2.0    | 新增xiaobaicmd -m命令               |
+| 2.1    | 新增xiaobaicmd --device命令         |
+| 2.2    | 优化xiaobaicmd --device命令         |
+| 2.3    | 新增实时监控Android设备耗电量              |
+| 2.3.1  | fix                             |
+| 2.3.2  | fix                             |
+| 2.3.3  | 新增实时监控Android当前APP的内存使用率        |
+| 2.3.4  | 优化xiaobaicmd -m gui效果展示         |
+| 2.3.5  | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.6  | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
+| 2.3.7  | 新增识别滑块验证码破解                     |
+| 2.3.8  | 优化识别滑块验证码破解                     |
```

### Comparing `xiaobaisaf-2.3.7/xiaobaisaf.egg-info/SOURCES.txt` & `xiaobaisaf-2.3.8/xiaobaisaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

