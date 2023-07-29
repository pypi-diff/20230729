# Comparing `tmp/xiaobaisaf-2.3.5.tar.gz` & `tmp/xiaobaisaf-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobaisaf-2.3.5.tar", last modified: Fri Jul 21 15:48:02 2023, max compression
+gzip compressed data, was "xiaobaisaf-2.3.7.tar", last modified: Sat Jul 29 14:10:06 2023, max compression
```

## Comparing `xiaobaisaf-2.3.5.tar` & `xiaobaisaf-2.3.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.533143 xiaobaisaf-2.3.5/
--rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.5/LICENSE
--rw-rw-rw-   0        0        0    12129 2023-07-21 15:48:02.533143 xiaobaisaf-2.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    11458 2023-07-21 15:37:05.000000 xiaobaisaf-2.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.505217 xiaobaisaf-2.3.5/saf/
--rw-rw-rw-   0        0        0     1436 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.5/saf/__init__.py
--rw-rw-rw-   0        0        0      152 2023-07-21 15:34:18.000000 xiaobaisaf-2.3.5/saf/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.507212 xiaobaisaf-2.3.5/saf/data/
--rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.5/saf/data/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/data/config.py
--rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/data/favicon.ico
--rw-rw-rw-   0        0        0     1201 2023-06-26 08:03:27.000000 xiaobaisaf-2.3.5/saf/data/software_check.sh
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.508210 xiaobaisaf-2.3.5/saf/example/
--rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.509207 xiaobaisaf-2.3.5/saf/example/api/
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.510205 xiaobaisaf-2.3.5/saf/example/api/Config/
--rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Config/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Config/config.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.511202 xiaobaisaf-2.3.5/saf/example/api/TestCases/
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/TestCases/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/TestCases/test_one_html_case_template.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.514194 xiaobaisaf-2.3.5/saf/example/api/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/api_client.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/api/Utils/logger.py
--rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/run.py
--rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/api/send_email_script.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.514194 xiaobaisaf-2.3.5/saf/example/web/
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.518183 xiaobaisaf-2.3.5/saf/example/web/Cases/
--rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/__init__.py
--rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/conftest.py
--rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_allure.py
--rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_submitBug.py
--rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v1.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v2.py
--rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v3.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.519179 xiaobaisaf-2.3.5/saf/example/web/Utils/
--rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.5/saf/example/web/Utils/logger.py
--rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.520177 xiaobaisaf-2.3.5/saf/example/web/pageObject/
--rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/pageObject/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/example/web/pageObject/register_page_element.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.529154 xiaobaisaf-2.3.5/saf/utils/
--rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/BugUtils.py
--rw-rw-rw-   0        0        0      130 2023-07-05 15:07:02.000000 xiaobaisaf-2.3.5/saf/utils/Demo.py
--rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidDeviceGUI.py
--rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageCLI.py
--rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageGUI.py
--rw-rw-rw-   0        0        0     7790 2023-06-30 17:18:46.000000 xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackagePower.py
--rw-rw-rw-   0        0        0     1583 2023-07-21 15:26:19.000000 xiaobaisaf-2.3.5/saf/utils/MonitorCANBus.py
--rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/utils/MonitorDBs.py
--rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.5/saf/utils/YamlUtils.py
--rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.5/saf/utils/__init__.py
--rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.5/saf/utils/downloadUtils.py
--rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/elementUtils.py
--rw-rw-rw-   0        0        0      660 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/imageUtils.py
--rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/networkSpeedUtils.py
--rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.5/saf/utils/osEnvUtils.py
--rw-rw-rw-   0        0        0    11552 2023-07-21 15:48:01.000000 xiaobaisaf-2.3.5/saf/utils/selenium2POM.py
--rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.5/saf/utils/sendMsgUtils.py
--rw-rw-rw-   0        0        0     2549 2023-06-30 17:16:51.000000 xiaobaisaf-2.3.5/saf/utils/xiaobaicmd.py
--rw-rw-rw-   0        0        0       42 2023-07-21 15:48:02.534140 xiaobaisaf-2.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2514 2023-07-06 16:41:30.000000 xiaobaisaf-2.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 15:48:02.532146 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/
--rw-rw-rw-   0        0        0    12129 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1865 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      154 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-21 15:48:02.000000 xiaobaisaf-2.3.5/xiaobaisaf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.486052 xiaobaisaf-2.3.7/
+-rw-rw-rw-   0        0        0    35181 2023-06-27 16:34:34.000000 xiaobaisaf-2.3.7/LICENSE
+-rw-rw-rw-   0        0        0    12938 2023-07-29 14:10:06.486052 xiaobaisaf-2.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    12267 2023-07-29 14:08:28.000000 xiaobaisaf-2.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.438126 xiaobaisaf-2.3.7/saf/
+-rw-rw-rw-   0        0        0     1527 2023-07-29 13:56:45.000000 xiaobaisaf-2.3.7/saf/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-07-29 14:00:20.000000 xiaobaisaf-2.3.7/saf/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.441088 xiaobaisaf-2.3.7/saf/data/
+-rw-rw-rw-   0        0        0      225 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.7/saf/data/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/data/config.py
+-rw-rw-rw-   0        0        0     4286 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/data/favicon.ico
+-rw-rw-rw-   0        0        0     1201 2023-06-26 08:03:27.000000 xiaobaisaf-2.3.7/saf/data/software_check.sh
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.442085 xiaobaisaf-2.3.7/saf/example/
+-rw-rw-rw-   0        0        0      100 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.444080 xiaobaisaf-2.3.7/saf/example/api/
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.446074 xiaobaisaf-2.3.7/saf/example/api/Config/
+-rw-rw-rw-   0        0        0      131 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Config/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Config/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.447072 xiaobaisaf-2.3.7/saf/example/api/TestCases/
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/TestCases/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/TestCases/test_one_html_case_template.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.452087 xiaobaisaf-2.3.7/saf/example/api/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/api_client.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/api/Utils/logger.py
+-rw-rw-rw-   0        0        0      129 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/run.py
+-rw-rw-rw-   0        0        0      549 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/api/send_email_script.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.452087 xiaobaisaf-2.3.7/saf/example/web/
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.458126 xiaobaisaf-2.3.7/saf/example/web/Cases/
+-rw-rw-rw-   0        0        0      140 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/conftest.py
+-rw-rw-rw-   0        0        0      930 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_allure.py
+-rw-rw-rw-   0        0        0      962 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_submitBug.py
+-rw-rw-rw-   0        0        0      320 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v1.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v2.py
+-rw-rw-rw-   0        0        0      228 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v3.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.462115 xiaobaisaf-2.3.7/saf/example/web/Utils/
+-rw-rw-rw-   0        0        0     1389 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-06-28 15:26:03.000000 xiaobaisaf-2.3.7/saf/example/web/Utils/logger.py
+-rw-rw-rw-   0        0        0      435 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.463113 xiaobaisaf-2.3.7/saf/example/web/pageObject/
+-rw-rw-rw-   0        0        0      166 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/pageObject/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/example/web/pageObject/register_page_element.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.480067 xiaobaisaf-2.3.7/saf/utils/
+-rw-rw-rw-   0        0        0     8132 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/BugUtils.py
+-rw-rw-rw-   0        0        0     2651 2023-07-29 14:10:05.000000 xiaobaisaf-2.3.7/saf/utils/CaptchaUtils.py
+-rw-rw-rw-   0        0        0     4132 2023-07-26 17:29:54.000000 xiaobaisaf-2.3.7/saf/utils/Demo.py
+-rw-rw-rw-   0        0        0     1271 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/ElementUtils.py
+-rw-rw-rw-   0        0        0     2076 2023-06-27 16:40:34.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidDeviceGUI.py
+-rw-rw-rw-   0        0        0     8917 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageCLI.py
+-rw-rw-rw-   0        0        0    14196 2023-07-05 15:45:45.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageGUI.py
+-rw-rw-rw-   0        0        0    10701 2023-07-22 18:26:01.000000 xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackagePower.py
+-rw-rw-rw-   0        0        0     1583 2023-07-21 15:26:19.000000 xiaobaisaf-2.3.7/saf/utils/MonitorCANBus.py
+-rw-rw-rw-   0        0        0     5933 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/utils/MonitorDBs.py
+-rw-rw-rw-   0        0        0    11552 2023-07-21 15:48:01.000000 xiaobaisaf-2.3.7/saf/utils/Selenium2POM.py
+-rw-rw-rw-   0        0        0     2694 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/SendMsgUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-27 16:34:37.000000 xiaobaisaf-2.3.7/saf/utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      201 2023-06-27 16:34:35.000000 xiaobaisaf-2.3.7/saf/utils/__init__.py
+-rw-rw-rw-   0        0        0     3061 2023-06-27 16:34:38.000000 xiaobaisaf-2.3.7/saf/utils/downloadUtils.py
+-rw-rw-rw-   0        0        0     1369 2023-06-27 16:34:36.000000 xiaobaisaf-2.3.7/saf/utils/networkSpeedUtils.py
+-rw-rw-rw-   0        0        0      132 2023-06-27 16:40:21.000000 xiaobaisaf-2.3.7/saf/utils/osEnvUtils.py
+-rw-rw-rw-   0        0        0     2549 2023-07-29 13:43:39.000000 xiaobaisaf-2.3.7/saf/utils/xiaobaicmd.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 14:10:06.487048 xiaobaisaf-2.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2514 2023-07-06 16:41:30.000000 xiaobaisaf-2.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:10:06.485054 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/
+-rw-rw-rw-   0        0        0    12938 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      154 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-29 14:10:06.000000 xiaobaisaf-2.3.7/xiaobaisaf.egg-info/top_level.txt
```

### Comparing `xiaobaisaf-2.3.5/LICENSE` & `xiaobaisaf-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/PKG-INFO` & `xiaobaisaf-2.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.5
+Version: 2.3.7
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -23,36 +23,38 @@
 
 ### 版本注意
     尽量使用Python 3.9.* 版本
     防止某些库出现不兼容问题，导致功能不可使用
 
 ### 安装教程
 ```commandline
-pip config set global.index-url https://pypi.douban.com/simple    注：将pip源修改为国内源
+pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple    注：将pip源修改为国内源
 pip install saf
 ```
 
 ### 使用说明
 - 优先修改saf/data/config.py中飞书/钉钉的webhook
 ```python
+# filename=config.py
+
 class feishu(object):
     @staticmethod
     def webhook():
         return 'https://open.feishu.cn/open-apis/bot/v2/hook/xxxx'
 
 class dingding(object):
     @staticmethod
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
 
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
-from saf.utils.sendMsgUtils import robotSendMessage
+from saf.utils.SendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item):
     """
     :param item:
     """
@@ -63,15 +65,15 @@
         robotSendMessage(robot_name='feishu', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='feishu,dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
 ```
 
 - 用例文件
 ```python
-# fielname = test_xiaobai_auto_script.py
+# fielname = test_xiaobai_testcase.py
 
 def setup_module():
     ''' 用例脚本执行之前需要准备的信息 '''
     ...
 
 def teardown_module():
     ''' 用例脚本执行之后需要清除的信息 '''
@@ -98,15 +100,15 @@
             1、UI测试就是定位需要操作的界面节点然后执行操作
             2、API测试就是执行相关接口实现接口的功能
         需要针对每次的结果添加断言进行判断处理
     '''
 ```
 
 ```python
-# filename = test_xiaobai_shop_allure.py
+# filename = test_xiaobai_allure.py
 # JDK与Allure已安装且配置好环境变量（若不知道可以查看公众号：小白科技之窗）
 import pytest
 import allure
 
 @allure.feature('下单')
 class Test_order():
     @allure.story('登录')
@@ -124,15 +126,15 @@
         ''' 搜索商品 '''
         with allure.step('搜索框输入：苹果'):
             assert True
         with allure.step('点击搜索按钮'):
             assert False
 '''
 # 执行脚本
-pytest test_xiaobai_shop_allure.py --alluredir=../data
+pytest test_xiaobai_allure.py --alluredir=../data
 
 # 打开报告
 allure serve ../data
 或者
 allure generate -c -o ../report ../data
 allure open ../report
 '''
@@ -140,25 +142,26 @@
 
 ### saf>1.1 使用禅道API，测试失败自动提单
 - 需要在禅道后台>>二次开发>>应用>>添加应用>>创建开启免密的应用 
 - 需要将上一步所生成数据【代号】与【密钥】写入到`saf/data/config.py`中zenTao相关的参数位置
 
 ```python
 # filename = saf/data/config.py
+
 import hashlib
 import time
 class zenTao(object):
     '''
     参考禅道接口文档：
     https://www.zentao.net/book/zentaopmshelp/integration-287.html
     '''
     @staticmethod
     def baseURL():
         ''' 禅道的根路径 '''
-        return 'http://192.168.254.133/zentao'
+        return 'http://192.168.0.240/zentao'
  
     @staticmethod
     def account():
         ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
         return '开启密钥的账户名称，例如管理员：admin'
  
     @staticmethod
@@ -182,14 +185,15 @@
         _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
         return _md5.hexdigest()
 ```
 
 - 用例同目录下创建`conftest.py`pytest的配置文件
 ```python
 # filename = conftest.py
+
 from saf.utils.BugUtils import addZenTaoBUG
 import pytest
   
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item, call):
   """
   :param item:
@@ -203,15 +207,14 @@
                         steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
     
  ```
 - 用例文件正常编写，正常运行即可
 
 ### saf>1.0 拷贝web自动化模板到D:\autoProject目录下
 ```bat
-
 xiaobaicmd -t web -d D:\autoProject
 xiaobaicmd --template web --dirname D:\autoProject
 xiaobaicmd -t api -d D:\autoProject
 xiaobaicmd --template api --dirname D:\autoProject
 xiaobaicmd -t app -d D:\autoProject[暂时不支持]
 ```
 
@@ -283,14 +286,39 @@
 
 ### saf>2.2   基础adb实现Android设备的电量监控功能
 ```cmd
 xiaobaicmd -m power   # 界面监控设备的电量与内存使用率的实时界面
 xiaobaicmd -m memory   # 界面监控设备的电量与内存使用率的实时界面
 ```
 
+### saf>2.3.5   新增实时监控Android当前APP的CPU使用率及FPS数据
+```cmd
+xiaobaicmd -m gui   
+```
+
+### saf>2.3.6   新增识别滑块验证码破解
+```python
+from saf.utils.CaptchaUtils import checkSlider
+from saf import selenium_webdriver, By
+
+driver = selenium_webdriver.Chrome()
+
+driver.get("https://www.xiaobaisoftware.com")
+
+# 其它操作...
+
+target_element = driver.find_element(By.XPATH, value='')
+
+background_element = driver.find_element(By.XPATH, value='')
+
+button_element = driver.find_element(By.XPATH, value='')
+
+checkSlider(driver, target_element, background_element, button_element)
+```
+
 ### 环境检测[还未实现]
 ```bat
 xiaobaicmd  --init
 
 检测内容: 
 1、python版本及第三方库
 2、第三方工具及环境
@@ -336,7 +364,9 @@
 | 2.2     | 优化xiaobaicmd --device命令         |
 | 2.3     | 新增实时监控Android设备耗电量              |
 | 2.3.1   | fix                             |
 | 2.3.2   | fix                             |
 | 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
 | 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
 | 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.6   | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
+| 2.3.7   | 新增识别滑块验证码破解                     |
```

### Comparing `xiaobaisaf-2.3.5/README.md` & `xiaobaisaf-2.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,36 +11,38 @@
 
 ### 版本注意
     尽量使用Python 3.9.* 版本
     防止某些库出现不兼容问题，导致功能不可使用
 
 ### 安装教程
 ```commandline
-pip config set global.index-url https://pypi.douban.com/simple    注：将pip源修改为国内源
+pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple    注：将pip源修改为国内源
 pip install saf
 ```
 
 ### 使用说明
 - 优先修改saf/data/config.py中飞书/钉钉的webhook
 ```python
+# filename=config.py
+
 class feishu(object):
     @staticmethod
     def webhook():
         return 'https://open.feishu.cn/open-apis/bot/v2/hook/xxxx'
 
 class dingding(object):
     @staticmethod
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
 
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
-from saf.utils.sendMsgUtils import robotSendMessage
+from saf.utils.SendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item):
     """
     :param item:
     """
@@ -51,15 +53,15 @@
         robotSendMessage(robot_name='feishu', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='feishu,dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
 ```
 
 - 用例文件
 ```python
-# fielname = test_xiaobai_auto_script.py
+# fielname = test_xiaobai_testcase.py
 
 def setup_module():
     ''' 用例脚本执行之前需要准备的信息 '''
     ...
 
 def teardown_module():
     ''' 用例脚本执行之后需要清除的信息 '''
@@ -86,15 +88,15 @@
             1、UI测试就是定位需要操作的界面节点然后执行操作
             2、API测试就是执行相关接口实现接口的功能
         需要针对每次的结果添加断言进行判断处理
     '''
 ```
 
 ```python
-# filename = test_xiaobai_shop_allure.py
+# filename = test_xiaobai_allure.py
 # JDK与Allure已安装且配置好环境变量（若不知道可以查看公众号：小白科技之窗）
 import pytest
 import allure
 
 @allure.feature('下单')
 class Test_order():
     @allure.story('登录')
@@ -112,15 +114,15 @@
         ''' 搜索商品 '''
         with allure.step('搜索框输入：苹果'):
             assert True
         with allure.step('点击搜索按钮'):
             assert False
 '''
 # 执行脚本
-pytest test_xiaobai_shop_allure.py --alluredir=../data
+pytest test_xiaobai_allure.py --alluredir=../data
 
 # 打开报告
 allure serve ../data
 或者
 allure generate -c -o ../report ../data
 allure open ../report
 '''
@@ -128,25 +130,26 @@
 
 ### saf>1.1 使用禅道API，测试失败自动提单
 - 需要在禅道后台>>二次开发>>应用>>添加应用>>创建开启免密的应用 
 - 需要将上一步所生成数据【代号】与【密钥】写入到`saf/data/config.py`中zenTao相关的参数位置
 
 ```python
 # filename = saf/data/config.py
+
 import hashlib
 import time
 class zenTao(object):
     '''
     参考禅道接口文档：
     https://www.zentao.net/book/zentaopmshelp/integration-287.html
     '''
     @staticmethod
     def baseURL():
         ''' 禅道的根路径 '''
-        return 'http://192.168.254.133/zentao'
+        return 'http://192.168.0.240/zentao'
  
     @staticmethod
     def account():
         ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
         return '开启密钥的账户名称，例如管理员：admin'
  
     @staticmethod
@@ -170,14 +173,15 @@
         _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
         return _md5.hexdigest()
 ```
 
 - 用例同目录下创建`conftest.py`pytest的配置文件
 ```python
 # filename = conftest.py
+
 from saf.utils.BugUtils import addZenTaoBUG
 import pytest
   
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item, call):
   """
   :param item:
@@ -191,15 +195,14 @@
                         steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
     
  ```
 - 用例文件正常编写，正常运行即可
 
 ### saf>1.0 拷贝web自动化模板到D:\autoProject目录下
 ```bat
-
 xiaobaicmd -t web -d D:\autoProject
 xiaobaicmd --template web --dirname D:\autoProject
 xiaobaicmd -t api -d D:\autoProject
 xiaobaicmd --template api --dirname D:\autoProject
 xiaobaicmd -t app -d D:\autoProject[暂时不支持]
 ```
 
@@ -271,14 +274,39 @@
 
 ### saf>2.2   基础adb实现Android设备的电量监控功能
 ```cmd
 xiaobaicmd -m power   # 界面监控设备的电量与内存使用率的实时界面
 xiaobaicmd -m memory   # 界面监控设备的电量与内存使用率的实时界面
 ```
 
+### saf>2.3.5   新增实时监控Android当前APP的CPU使用率及FPS数据
+```cmd
+xiaobaicmd -m gui   
+```
+
+### saf>2.3.6   新增识别滑块验证码破解
+```python
+from saf.utils.CaptchaUtils import checkSlider
+from saf import selenium_webdriver, By
+
+driver = selenium_webdriver.Chrome()
+
+driver.get("https://www.xiaobaisoftware.com")
+
+# 其它操作...
+
+target_element = driver.find_element(By.XPATH, value='')
+
+background_element = driver.find_element(By.XPATH, value='')
+
+button_element = driver.find_element(By.XPATH, value='')
+
+checkSlider(driver, target_element, background_element, button_element)
+```
+
 ### 环境检测[还未实现]
 ```bat
 xiaobaicmd  --init
 
 检测内容: 
 1、python版本及第三方库
 2、第三方工具及环境
@@ -323,8 +351,10 @@
 | 2.1     | 新增xiaobaicmd --device命令         |
 | 2.2     | 优化xiaobaicmd --device命令         |
 | 2.3     | 新增实时监控Android设备耗电量              |
 | 2.3.1   | fix                             |
 | 2.3.2   | fix                             |
 | 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
 | 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
-| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.6   | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
+| 2.3.7   | 新增识别滑块验证码破解                     |
```

### Comparing `xiaobaisaf-2.3.5/saf/__init__.py` & `xiaobaisaf-2.3.7/saf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 @Author: xiaobaiTser
 @Time  : 2022/8/20 22:22
 @File  : __init__.py
 '''
 from typing import Union
 import datetime
 
-# 将pip更新源设置为：https://pypi.douban.com/simple
-# pip config set global.index-url https://pypi.douban.com/simple
+# 将pip更新源设置为：https://pypi.tuna.tsinghua.edu.cn/simple
+# pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
 
 from selenium import webdriver as selenium_webdriver
+from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys     # 键盘事件
 from selenium.webdriver.common.action_chains import ActionChains  # 鼠标事件
 from webdriver_manager.chrome import ChromeDriverManager
 from loguru import logger
 # 运行日志
@@ -26,13 +27,13 @@
 from yaml import full_load
 
 # 当前版本的httpx，只有在异步请求时才略优于requests，此处可使用到发送消息使用
 # from httpx import request
 try:
     from ddddocr import DdddOcr
 except ImportError as e:
-    import os; os.system('pip install ddddocr -i https://pypi.douban.com/simple')
+    import os; os.system('pip install ddddocr -i https://pypi.tuna.tsinghua.edu.cn/simple')
     # 如果运行ddddocr运行报错更新opencv库：
     os.system('pip uninstall opencv-python')
     os.system('pip uninstall opencv-contrib-python')
     os.system('pip install opencv-contrib-python')
     os.system('pip install opencv-python')
```

### Comparing `xiaobaisaf-2.3.5/saf/data/config.py` & `xiaobaisaf-2.3.7/saf/data/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/data/favicon.ico` & `xiaobaisaf-2.3.7/saf/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/data/software_check.sh` & `xiaobaisaf-2.3.7/saf/data/software_check.sh`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/Config/config.py` & `xiaobaisaf-2.3.7/saf/example/api/Config/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/TestCases/test_one_html_case_template.py` & `xiaobaisaf-2.3.7/saf/example/api/TestCases/test_one_html_case_template.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.7/saf/example/api/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/Utils/YamlUtils.py` & `xiaobaisaf-2.3.7/saf/example/api/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/Utils/api_client.py` & `xiaobaisaf-2.3.7/saf/example/api/Utils/api_client.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/run.py` & `xiaobaisaf-2.3.7/saf/example/api/run.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/api/send_email_script.py` & `xiaobaisaf-2.3.7/saf/example/api/send_email_script.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/web/Cases/conftest.py` & `xiaobaisaf-2.3.7/saf/example/web/Cases/conftest.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_allure.py` & `xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_allure.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_submitBug.py` & `xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_submitBug.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/web/Cases/test_xiaobai_case_v2.py` & `xiaobaisaf-2.3.7/saf/example/web/Cases/test_xiaobai_case_v2.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/web/Utils/ExcelUtils.py` & `xiaobaisaf-2.3.7/saf/example/web/Utils/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/example/web/Utils/YamlUtils.py` & `xiaobaisaf-2.3.7/saf/example/web/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/BugUtils.py` & `xiaobaisaf-2.3.7/saf/utils/BugUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidDeviceGUI.py` & `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidDeviceGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageCLI.py` & `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageCLI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackageGUI.py` & `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackageGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/MonitorAndroidPackagePower.py` & `xiaobaisaf-2.3.7/saf/utils/MonitorAndroidPackagePower.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 '''
 @Author: xiaobaiTser
 @email : 807447312@qq.com
 @Time  : 2023/6/28 20:41
 @File  : MonitorAndroidPackagePowser.py
 '''
 import os
+import re
 import tkinter as tk
 import subprocess
 import threading
 import time
 from tkinter import filedialog, messagebox
 
 import matplotlib.pyplot as plt
@@ -37,18 +38,24 @@
         self.stop_button.pack(side='left', padx=10, pady=10)
 
         self.export_button = tk.Button(master, text='导出', command=self.export)
         self.export_button.pack(side='left', padx=10, pady=10)
 
         # 创建tkinter标签，用于显示最新的电量数据
         self.label_power = tk.Label(master, text='设备当前电量：')
-        self.label_power.pack(side='bottom', padx=10, pady=10)
-        # 创建tkinter标签，用于显示最新的电量数据
-        self.label_memory_rate = tk.Label(master, text='APP内存使用率：')
-        self.label_memory_rate.pack(side='bottom', padx=10, pady=10)
+        self.label_power.pack(side='bottom', padx=2, pady=2)
+        # 创建tkinter标签，用于显示最新的内存数据
+        self.label_memory_rate = tk.Label(master, text='内存使用率：')
+        self.label_memory_rate.pack(side='bottom', padx=2, pady=2)
+        # 创建tkinter标签，用于显示最新的CPU数据
+        self.label_cpu_rate = tk.Label(master, text='CPU使用率：')
+        self.label_cpu_rate.pack(side='bottom', padx=2, pady=2)
+        # 创建tkinter标签，用于显示最新的FPS数据
+        self.label_fps_rate = tk.Label(master, text='FPS刷新率：')
+        self.label_fps_rate.pack(side='bottom', padx=2, pady=2)
 
         # 创建matplotlib图形区域
         self.fig = plt.figure(figsize=(6, 4))
         self.ax = self.fig.add_subplot(111)
         self.ax.set_xlabel('Time(s)')
         self.ax.set_ylabel('Rate(%)')
         self.ax.set_xlim(0, 30)
@@ -64,81 +71,113 @@
             self.is_running = True
             self.device_id = subprocess.check_output(['adb', 'devices']).decode('utf-8').split('\n')[1].split('\t')[0]
             self.total_memory = \
                 subprocess.check_output(['adb', 'shell', 'cat', '/proc/meminfo', '|', 'grep', '"MemTotal"']).decode(
                     'utf-8').split()[1]
             self.power_data = []
             self.app_memory_data = []
+            self.app_cpu_data = []
+            self.app_fps_data = []
 
-            # 在后台启动一个线程来获取电量数据
+            # 在后台启动一个线程来获取数据
             self.power_thread = threading.Thread(target=self.get_data)
             self.power_thread.start()
 
     def stop(self):
         self.is_running = False
 
     def export(self):
         # 弹出文件对话框，获取用户选择的文件名和存储位置
         file_path = filedialog.asksaveasfilename(defaultextension='.csv', filetypes=(("CSV文件", "*.csv"),))
         if file_path:
             try:
                 # 合并数据
-                merged_list = [(a[0], a[1], b[0], b[1]) for a, b in zip(self.power_data, self.app_memory_data)]
+                merged_list = [(a[0], a[1], b[0], b[1], c, d) for a, b, c, d in zip(self.power_data,
+                                                                                 self.app_memory_data,
+                                                                                 self.app_cpu_data,
+                                                                                 self.app_fps_data)]
                 # 导出电量数据到CSV文件
                 with open(file_path, 'w', newline='') as f:
                     writer = csv.writer(f)
-                    writer.writerows([('运行时间（秒）', '电量（%）', '包名', '内存使用率（%）')])
+                    writer.writerows([('运行时间（秒）', '设备电量（%）', '应用程序包名', '内存使用率（%）', 'CPU使用率（%）',
+                                       'FPS（帧/秒）')])
                     writer.writerows(merged_list)
                 messagebox.showinfo("小白提醒：", "数据已经保存完成！")
             except PermissionError:
                 messagebox.showerror("小白提示：", "文件无法访问！文件是否打开？请先关闭后重新尝试！")
 
     def get_data(self):
-
         while self.is_running:
             # 电量
-            power_output = subprocess.check_output(['adb', '-s', self.device_id, 'shell', 'dumpsys', 'battery', '|', 'grep', 'level']).decode('utf-8').strip()
+            power_output = subprocess.check_output(['adb', '-s', self.device_id, 'shell', 'dumpsys', 'battery', '|',
+                                                    'grep', 'level']).decode('utf-8').strip()
             power_level = int(power_output.split(':')[1])
             self.power_data.append((int(time.time()-self.start_time), power_level))
 
-            # 内存
             package_name = \
                 subprocess.check_output(['adb', 'shell', 'dumpsys', 'window', '|', 'grep', 'mCurrentFocus']).decode(
                     'utf-8')
             if 'mCurrentFocus=null' in package_name:
                 status = messagebox.askyesno("小白提示：", "存在熄屏或者切换APP的行为！获取数据期间尽量不要切换或者熄屏！")
                 if status:
                     try:
-                        subprocess.check_output(['adb', 'shell', 'settings', 'put', 'system', 'screen_off_timeout',  '-1'])
+                        subprocess.check_output(['adb', 'shell', 'settings', 'put', 'system', 'screen_off_timeout',
+                                                 '-1'])
                     except Exception:
                         messagebox.showerror('小白错误提示：', '设置失败！')
                 else:
 
                     exit(0)
             else:
                 package_name = package_name.split()[2].split('/')[0]
                 package_pid = subprocess.check_output(['adb', 'shell', 'ps', '|', 'grep', package_name]).decode(
                         'utf-8')
                 app_package_pid = ''
                 for pid in package_pid.split('\r\n'):
                     if package_name in pid.split():
                         app_package_pid = pid.split()[1]
                         break
-                result = subprocess.run(['adb', 'shell', 'dumpsys', 'meminfo', app_package_pid], capture_output=True, text=True)
+
+                # 内存
+                result = subprocess.run(['adb', 'shell', 'dumpsys', 'meminfo', app_package_pid], capture_output=True,
+                                        text=True)
                 memory_output = result.stdout
                 # 解析输出，获取当前打开的APP的内存使用情况
-                app_memory_usage = ''
                 lines = memory_output.split('\n')
                 for line in lines:
                     if 'TOTAL' in line:
                         app_memory_usage = line.split()[1]
                         self.app_memory_data.append(
                             (package_name, round(int(app_memory_usage) * 100 / int(self.total_memory), 1)))
                         break
 
+                # CPU
+                output = subprocess.check_output(["adb", "shell", "top", "-n", "1", "-d", "1", "-p",
+                                                  app_package_pid]).decode("utf-8")
+                lines = output.strip().split("\n")
+                if len(lines) >= 2:
+                    # 提取CPU使用率数据
+                    cpu_line = lines[-1]
+                    try:
+                        self.app_cpu_data.append(float(cpu_line.split()[8]))
+                    except Exception as e:
+                        self.app_cpu_data.append(0.0)
+
+                # 获取FPS数据
+                output = subprocess.check_output(
+                    ["adb", "shell", "dumpsys", "gfxinfo", package_name, "framestats"]).decode("utf-8")
+                lines = output.strip().split("\r\n")
+                janky_frames_line = [x for x in lines if 'Janky frames:' in x][0] \
+                    if len([x for x in lines if 'Janky frames:' in x]) > 0 \
+                    else '(0.0%)'
+                janky_frames = float(re.findall('\((.*?)%\)', janky_frames_line)[0])
+                self.app_fps_data.append(int(60 * (1 - janky_frames / 100)))
+
+                # 其他数据...
+
                 self.update_data()
                 time.sleep(1)
 
     def update_data(self):
         # 更新图表数据和电量标签
         if self.power_data:
             self.ax.clear()
@@ -151,23 +190,31 @@
             self.ax.set_ylim(0, 100)
 
             if len(self.ax.lines) > 0:
                 self.ax.lines.pop(0)
             if self.power_data[-1][0] > 30:
                 self.ax.plot([t for t, _ in self.power_data[-30:]], [p for _, p in self.power_data[-30:]])
                 self.ax.plot([t for t, _ in self.power_data[-30:]], [p for _, p in self.app_memory_data[-30:]])
+                self.ax.plot([t for t, _ in self.power_data[-30:]], [p for p in self.app_cpu_data[-30:]])
+                self.ax.plot([t for t, _ in self.power_data[-30:]], [p for p in self.app_fps_data[-30:]])
             else:
                 self.ax.plot([t for t, _ in self.power_data], [p for _, p in self.power_data])
                 self.ax.plot([t for t, _ in self.power_data], [p for _, p in self.app_memory_data])
+                self.ax.plot([t for t, _ in self.power_data], [p for p in self.app_cpu_data])
+                self.ax.plot([t for t, _ in self.power_data], [p for p in self.app_fps_data])
             self.canvas.draw()
             # 更新电量标签
             current_power = self.power_data[-1][1]
             current_memory_rate = self.app_memory_data[-1][1]
+            current_cpu_rate = self.app_cpu_data[-1]
+            current_fps_rate = self.app_fps_data[-1]
             self.label_power.config(text=f'设备当前电量[蓝线]：{current_power}%')
-            self.label_memory_rate.config(text=f'APP内存使用率[红线]：{current_memory_rate}%')
+            self.label_memory_rate.config(text=f'内存使用率[橙线]：{current_memory_rate}%')
+            self.label_cpu_rate.config(text=f'CPU使用率[绿线]：{current_cpu_rate}%')
+            self.label_fps_rate.config(text=f'FPS刷新率[红线]：{current_fps_rate}/s')
 
 def power():
     root = tk.Tk()
     app = App(root)
     root.mainloop()
 
 if __name__ == '__main__':
```

### Comparing `xiaobaisaf-2.3.5/saf/utils/MonitorCANBus.py` & `xiaobaisaf-2.3.7/saf/utils/MonitorCANBus.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/MonitorDBs.py` & `xiaobaisaf-2.3.7/saf/utils/MonitorDBs.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/YamlUtils.py` & `xiaobaisaf-2.3.7/saf/utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/downloadUtils.py` & `xiaobaisaf-2.3.7/saf/utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/elementUtils.py` & `xiaobaisaf-2.3.7/saf/utils/ElementUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/networkSpeedUtils.py` & `xiaobaisaf-2.3.7/saf/utils/networkSpeedUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/selenium2POM.py` & `xiaobaisaf-2.3.7/saf/utils/Selenium2POM.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/sendMsgUtils.py` & `xiaobaisaf-2.3.7/saf/utils/SendMsgUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/saf/utils/xiaobaicmd.py` & `xiaobaisaf-2.3.7/saf/utils/xiaobaicmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 @Author: xiaobaiTser
 @Time  : 2022/8/24 2:26
 @File  : xiaobaicmd.py
 '''
 import os.path
 from shutil import copytree
 import click
-from saf.utils.selenium2POM import PageListener
+from saf.utils.Selenium2POM import PageListener
 from saf.utils.MonitorAndroidPackageGUI import gui
 from saf.utils.MonitorAndroidPackageCLI import cli
 from saf.utils.MonitorAndroidDeviceGUI import MonitorDevice
 from saf.utils.MonitorAndroidPackagePower import power
 
 @click.command()
 @click.option('--template', '-t', type=click.Choice(['web', 'api', 'app']), nargs=1, help='创建自动化项目模板')
```

### Comparing `xiaobaisaf-2.3.5/setup.py` & `xiaobaisaf-2.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.3.5/xiaobaisaf.egg-info/PKG-INFO` & `xiaobaisaf-2.3.7/xiaobaisaf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.3.5
+Version: 2.3.7
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
@@ -23,36 +23,38 @@
 
 ### 版本注意
     尽量使用Python 3.9.* 版本
     防止某些库出现不兼容问题，导致功能不可使用
 
 ### 安装教程
 ```commandline
-pip config set global.index-url https://pypi.douban.com/simple    注：将pip源修改为国内源
+pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple    注：将pip源修改为国内源
 pip install saf
 ```
 
 ### 使用说明
 - 优先修改saf/data/config.py中飞书/钉钉的webhook
 ```python
+# filename=config.py
+
 class feishu(object):
     @staticmethod
     def webhook():
         return 'https://open.feishu.cn/open-apis/bot/v2/hook/xxxx'
 
 class dingding(object):
     @staticmethod
     def webhook():
         return 'https://oapi.dingtalk.com/robot/send?access_token=xxxxxxxx'
 ```
 
 - conftest.py（保持此文件与用例文件在同目录下）
 ```python
 # filename = conftest.py
-from saf.utils.sendMsgUtils import robotSendMessage
+from saf.utils.SendMsgUtils import robotSendMessage
 import pytest
 
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item):
     """
     :param item:
     """
@@ -63,15 +65,15 @@
         robotSendMessage(robot_name='feishu', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
         # robotSendMessage(robot_name='feishu,dingding', msg=f'测试脚本：{report.nodeid.split("::")[0]}\n测试用例：{report.nodeid.split("::")[1]}\n测试结果：{report.outcome}')
 ```
 
 - 用例文件
 ```python
-# fielname = test_xiaobai_auto_script.py
+# fielname = test_xiaobai_testcase.py
 
 def setup_module():
     ''' 用例脚本执行之前需要准备的信息 '''
     ...
 
 def teardown_module():
     ''' 用例脚本执行之后需要清除的信息 '''
@@ -98,15 +100,15 @@
             1、UI测试就是定位需要操作的界面节点然后执行操作
             2、API测试就是执行相关接口实现接口的功能
         需要针对每次的结果添加断言进行判断处理
     '''
 ```
 
 ```python
-# filename = test_xiaobai_shop_allure.py
+# filename = test_xiaobai_allure.py
 # JDK与Allure已安装且配置好环境变量（若不知道可以查看公众号：小白科技之窗）
 import pytest
 import allure
 
 @allure.feature('下单')
 class Test_order():
     @allure.story('登录')
@@ -124,15 +126,15 @@
         ''' 搜索商品 '''
         with allure.step('搜索框输入：苹果'):
             assert True
         with allure.step('点击搜索按钮'):
             assert False
 '''
 # 执行脚本
-pytest test_xiaobai_shop_allure.py --alluredir=../data
+pytest test_xiaobai_allure.py --alluredir=../data
 
 # 打开报告
 allure serve ../data
 或者
 allure generate -c -o ../report ../data
 allure open ../report
 '''
@@ -140,25 +142,26 @@
 
 ### saf>1.1 使用禅道API，测试失败自动提单
 - 需要在禅道后台>>二次开发>>应用>>添加应用>>创建开启免密的应用 
 - 需要将上一步所生成数据【代号】与【密钥】写入到`saf/data/config.py`中zenTao相关的参数位置
 
 ```python
 # filename = saf/data/config.py
+
 import hashlib
 import time
 class zenTao(object):
     '''
     参考禅道接口文档：
     https://www.zentao.net/book/zentaopmshelp/integration-287.html
     '''
     @staticmethod
     def baseURL():
         ''' 禅道的根路径 '''
-        return 'http://192.168.254.133/zentao'
+        return 'http://192.168.0.240/zentao'
  
     @staticmethod
     def account():
         ''' 后台-》二次开发-》应用-》免密登录的账户名 '''
         return '开启密钥的账户名称，例如管理员：admin'
  
     @staticmethod
@@ -182,14 +185,15 @@
         _md5 = hashlib.md5(f'{zenTao.getCode()}{zenTao.getKey()}{zenTao.getTime()}'.encode('utf-8'))
         return _md5.hexdigest()
 ```
 
 - 用例同目录下创建`conftest.py`pytest的配置文件
 ```python
 # filename = conftest.py
+
 from saf.utils.BugUtils import addZenTaoBUG
 import pytest
   
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item, call):
   """
   :param item:
@@ -203,15 +207,14 @@
                         steps=f'{doc}预期结果：passed<br>测试结果：{report.outcome}')
     
  ```
 - 用例文件正常编写，正常运行即可
 
 ### saf>1.0 拷贝web自动化模板到D:\autoProject目录下
 ```bat
-
 xiaobaicmd -t web -d D:\autoProject
 xiaobaicmd --template web --dirname D:\autoProject
 xiaobaicmd -t api -d D:\autoProject
 xiaobaicmd --template api --dirname D:\autoProject
 xiaobaicmd -t app -d D:\autoProject[暂时不支持]
 ```
 
@@ -283,14 +286,39 @@
 
 ### saf>2.2   基础adb实现Android设备的电量监控功能
 ```cmd
 xiaobaicmd -m power   # 界面监控设备的电量与内存使用率的实时界面
 xiaobaicmd -m memory   # 界面监控设备的电量与内存使用率的实时界面
 ```
 
+### saf>2.3.5   新增实时监控Android当前APP的CPU使用率及FPS数据
+```cmd
+xiaobaicmd -m gui   
+```
+
+### saf>2.3.6   新增识别滑块验证码破解
+```python
+from saf.utils.CaptchaUtils import checkSlider
+from saf import selenium_webdriver, By
+
+driver = selenium_webdriver.Chrome()
+
+driver.get("https://www.xiaobaisoftware.com")
+
+# 其它操作...
+
+target_element = driver.find_element(By.XPATH, value='')
+
+background_element = driver.find_element(By.XPATH, value='')
+
+button_element = driver.find_element(By.XPATH, value='')
+
+checkSlider(driver, target_element, background_element, button_element)
+```
+
 ### 环境检测[还未实现]
 ```bat
 xiaobaicmd  --init
 
 检测内容: 
 1、python版本及第三方库
 2、第三方工具及环境
@@ -336,7 +364,9 @@
 | 2.2     | 优化xiaobaicmd --device命令         |
 | 2.3     | 新增实时监控Android设备耗电量              |
 | 2.3.1   | fix                             |
 | 2.3.2   | fix                             |
 | 2.3.3   | 新增实时监控Android当前APP的内存使用率        |
 | 2.3.4   | 优化xiaobaicmd -m gui效果展示         |
 | 2.3.5   | 优化xiaobaicmd -u 转PO代码时xpath的表达式 |
+| 2.3.6   | 新增实时监控Android当前APP的CPU使用率及FPS数据 |
+| 2.3.7   | 新增识别滑块验证码破解                     |
```

### Comparing `xiaobaisaf-2.3.5/xiaobaisaf.egg-info/SOURCES.txt` & `xiaobaisaf-2.3.7/xiaobaisaf.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,30 +31,30 @@
 saf/example/web/Utils/ExcelUtils.py
 saf/example/web/Utils/YamlUtils.py
 saf/example/web/Utils/__init__.py
 saf/example/web/Utils/logger.py
 saf/example/web/pageObject/__init__.py
 saf/example/web/pageObject/register_page_element.py
 saf/utils/BugUtils.py
+saf/utils/CaptchaUtils.py
 saf/utils/Demo.py
+saf/utils/ElementUtils.py
 saf/utils/MonitorAndroidDeviceGUI.py
 saf/utils/MonitorAndroidPackageCLI.py
 saf/utils/MonitorAndroidPackageGUI.py
 saf/utils/MonitorAndroidPackagePower.py
 saf/utils/MonitorCANBus.py
 saf/utils/MonitorDBs.py
+saf/utils/Selenium2POM.py
+saf/utils/SendMsgUtils.py
 saf/utils/YamlUtils.py
 saf/utils/__init__.py
 saf/utils/downloadUtils.py
-saf/utils/elementUtils.py
-saf/utils/imageUtils.py
 saf/utils/networkSpeedUtils.py
 saf/utils/osEnvUtils.py
-saf/utils/selenium2POM.py
-saf/utils/sendMsgUtils.py
 saf/utils/xiaobaicmd.py
 xiaobaisaf.egg-info/PKG-INFO
 xiaobaisaf.egg-info/SOURCES.txt
 xiaobaisaf.egg-info/dependency_links.txt
 xiaobaisaf.egg-info/entry_points.txt
 xiaobaisaf.egg-info/requires.txt
 xiaobaisaf.egg-info/top_level.txt
```

