# Comparing `tmp/flake8-6.0.0.tar.gz` & `tmp/flake8-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-6.0.0.tar", last modified: Wed Nov 23 19:27:42 2022, max compression
+gzip compressed data, was "flake8-6.1.0.tar", last modified: Sat Jul 29 19:04:44 2023, max compression
```

## Comparing `flake8-6.0.0.tar` & `flake8-6.1.0.tar`

### file list

```diff
@@ -1,211 +1,53 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.662058 flake8-6.0.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)      122 2022-10-30 18:55:43.000000 flake8-6.0.0/CONTRIBUTING.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      473 2022-10-30 18:55:43.000000 flake8-6.0.0/CONTRIBUTORS.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1172 2022-10-30 18:55:43.000000 flake8-6.0.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)      217 2022-10-30 18:55:43.000000 flake8-6.0.0/MANIFEST.in
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3628 2022-11-23 19:27:42.662058 flake8-6.0.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2602 2022-10-30 18:55:43.000000 flake8-6.0.0/README.rst
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.642058 flake8-6.0.0/docs/
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.642058 flake8-6.0.0/docs/source/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9801 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/conf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2078 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/faq.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2198 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/glossary.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3060 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/index.rst
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.646058 flake8-6.0.0/docs/source/internal/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2228 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/checker.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      841 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/cli.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6517 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/contributing.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1549 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/formatters.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      792 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/index.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7768 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/option_handling.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1255 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/plugin_handling.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2735 2022-11-23 19:03:06.000000 flake8-6.0.0/docs/source/internal/releases.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4174 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/start-to-finish.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2379 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/utils.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6441 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/writing-code.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5220 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/internal/writing-documentation.rst
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.646058 flake8-6.0.0/docs/source/plugin-development/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1816 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/plugin-development/formatters.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1952 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/plugin-development/index.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6942 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/plugin-development/plugin-parameters.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4769 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/plugin-development/registering-plugins.rst
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/docs/source/release-notes/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/0.6.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      194 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/0.7.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)       92 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/0.8.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      116 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/0.9.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      155 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.0.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      266 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.1.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.2.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)       83 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.3.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)       70 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.3.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      103 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.4.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      280 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.5.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      667 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.6.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      237 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.6.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      105 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.6.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      250 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/1.7.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      630 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.0.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      459 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.1.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      551 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.2.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      157 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.2.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      130 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.2.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)       85 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.2.3.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      484 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.2.4.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      138 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.2.5.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      220 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.3.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      781 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.4.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      304 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.4.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      596 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.5.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      317 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.5.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      198 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.5.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.5.3.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      103 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.5.4.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      195 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.5.5.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      459 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.6.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      217 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.6.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/2.6.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2656 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.0.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      394 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.0.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      320 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.0.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1222 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.0.3.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      328 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.0.4.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2121 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.1.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      465 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.1.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      268 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.2.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      615 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.2.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1219 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.3.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      797 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.4.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      332 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.4.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      812 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.5.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1834 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.6.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1299 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      313 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      514 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      586 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.3.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      328 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.4.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      319 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.5.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      393 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.6.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      331 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.7.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      615 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.8.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      357 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.7.9.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4341 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.8.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      300 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.8.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      656 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.8.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      394 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.8.3.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      433 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.8.4.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      700 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.9.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      313 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.9.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      448 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/3.9.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1553 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/4.0.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      309 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/4.0.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2698 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/5.0.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      314 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/5.0.1.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      379 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/5.0.2.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      326 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/5.0.3.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      332 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/release-notes/5.0.4.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1257 2022-11-23 19:21:58.000000 flake8-6.0.0/docs/source/release-notes/6.0.0.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1308 2022-11-23 19:02:44.000000 flake8-6.0.0/docs/source/release-notes/index.rst
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/docs/source/user/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9150 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/configuration.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8786 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/error-codes.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)      617 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/index.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2259 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/invocation.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)    24083 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/options.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3532 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/python-api.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1377 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/using-hooks.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2141 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/using-plugins.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9564 2022-10-30 18:55:43.000000 flake8-6.0.0/docs/source/user/violations.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)       93 2022-10-30 18:55:43.000000 flake8-6.0.0/pytest.ini
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1896 2022-11-23 19:27:42.662058 flake8-6.0.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)      198 2022-10-30 18:55:43.000000 flake8-6.0.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.642058 flake8-6.0.0/src/
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/src/flake8/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1943 2022-11-23 19:02:16.000000 flake8-6.0.0/src/flake8/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      178 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/__main__.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/src/flake8/api/
--rw-r--r--   0 asottile  (1000) asottile  (1000)      241 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/api/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6898 2022-10-30 19:08:28.000000 flake8-6.0.0/src/flake8/api/legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    22524 2022-10-31 00:13:11.000000 flake8-6.0.0/src/flake8/checker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1209 2022-11-15 18:06:17.000000 flake8-6.0.0/src/flake8/defaults.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2581 2022-10-30 19:08:28.000000 flake8-6.0.0/src/flake8/discover_files.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2393 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/exceptions.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/src/flake8/formatting/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       97 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/formatting/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2022 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/formatting/_windows_color.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7356 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/formatting/base.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3057 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/formatting/default.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/src/flake8/main/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       98 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/main/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7949 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/main/application.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      599 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/main/cli.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/main/debug.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    10783 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/main/options.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.658058 flake8-6.0.0/src/flake8/options/
--rw-r--r--   0 asottile  (1000) asottile  (1000)      496 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/options/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1963 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/options/aggregator.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4572 2022-11-15 18:06:17.000000 flake8-6.0.0/src/flake8/options/config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11525 2022-11-16 00:10:45.000000 flake8-6.0.0/src/flake8/options/manager.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2162 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/options/parse_args.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.658058 flake8-6.0.0/src/flake8/plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       92 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11154 2022-11-23 18:28:14.000000 flake8-6.0.0/src/flake8/plugins/finder.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6036 2022-11-23 18:46:49.000000 flake8-6.0.0/src/flake8/plugins/pycodestyle.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6446 2022-11-23 19:00:20.000000 flake8-6.0.0/src/flake8/plugins/pyflakes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1241 2022-11-15 18:06:17.000000 flake8-6.0.0/src/flake8/plugins/reporter.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    16374 2022-11-15 18:06:17.000000 flake8-6.0.0/src/flake8/processor.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4358 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/statistics.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14445 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/style_guide.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8168 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/utils.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2039 2022-10-30 18:55:43.000000 flake8-6.0.0/src/flake8/violation.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.654058 flake8-6.0.0/src/flake8.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3628 2022-11-23 19:27:42.000000 flake8-6.0.0/src/flake8.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6153 2022-11-23 19:27:42.000000 flake8-6.0.0/src/flake8.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-11-23 19:27:42.000000 flake8-6.0.0/src/flake8.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      422 2022-11-23 19:27:42.000000 flake8-6.0.0/src/flake8.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       72 2022-11-23 19:27:42.000000 flake8-6.0.0/src/flake8.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        7 2022-11-23 19:27:42.000000 flake8-6.0.0/src/flake8.egg-info/top_level.txt
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.658058 flake8-6.0.0/tests/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       95 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      176 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/conftest.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.658058 flake8-6.0.0/tests/integration/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/integration/__init__.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.658058 flake8-6.0.0/tests/integration/subdir/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/integration/subdir/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      326 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/integration/subdir/aplugin.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2068 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/integration/test_aggregator.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      469 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/integration/test_api_legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11257 2022-11-23 18:28:14.000000 flake8-6.0.0/tests/integration/test_checker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11868 2022-11-23 18:28:14.000000 flake8-6.0.0/tests/integration/test_main.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4944 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/integration/test_plugins.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.662058 flake8-6.0.0/tests/unit/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      669 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/conftest.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-23 19:27:42.662058 flake8-6.0.0/tests/unit/plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    23537 2022-11-23 19:00:20.000000 flake8-6.0.0/tests/unit/plugins/finder_test.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      979 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/plugins/pycodestyle_test.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2202 2022-11-23 18:28:14.000000 flake8-6.0.0/tests/unit/plugins/reporter_test.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1189 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_application.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6454 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_base_formatter.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2520 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_checker_manager.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1269 2022-11-23 18:28:14.000000 flake8-6.0.0/tests/unit/test_debug.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8063 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_decision_engine.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      556 2022-11-15 18:06:17.000000 flake8-6.0.0/tests/unit/test_defaults.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4846 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_discover_files.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1051 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_exceptions.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1883 2022-11-23 18:28:14.000000 flake8-6.0.0/tests/unit/test_file_checker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12612 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_file_processor.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1325 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_filenameonly_formatter.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3510 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_legacy_api.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      576 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_main_options.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      884 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_nothing_formatter.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1713 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_option.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6839 2022-11-16 00:10:45.000000 flake8-6.0.0/tests/unit/test_option_manager.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8223 2022-11-15 18:06:17.000000 flake8-6.0.0/tests/unit/test_options_config.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1007 2022-11-23 19:00:20.000000 flake8-6.0.0/tests/unit/test_pyflakes_codes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4480 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_statistics.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5032 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_style_guide.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6386 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_utils.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2151 2022-10-30 18:55:43.000000 flake8-6.0.0/tests/unit/test_violation.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2355 2022-11-23 18:28:14.000000 flake8-6.0.0/tox.ini
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.827286 flake8-6.1.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1172 2022-10-30 18:55:43.000000 flake8-6.1.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3690 2023-07-29 19:04:44.827286 flake8-6.1.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2664 2023-06-13 01:47:27.000000 flake8-6.1.0/README.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1897 2023-07-29 19:04:44.827286 flake8-6.1.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      198 2022-10-30 18:55:43.000000 flake8-6.1.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.819286 flake8-6.1.0/src/
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.823286 flake8-6.1.0/src/flake8/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1943 2023-07-29 18:53:45.000000 flake8-6.1.0/src/flake8/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      178 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      283 2023-07-29 18:40:02.000000 flake8-6.1.0/src/flake8/_compat.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.823286 flake8-6.1.0/src/flake8/api/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      241 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/api/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6898 2022-10-30 19:08:28.000000 flake8-6.1.0/src/flake8/api/legacy.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    22581 2023-07-29 18:40:02.000000 flake8-6.1.0/src/flake8/checker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1109 2023-06-13 01:47:27.000000 flake8-6.1.0/src/flake8/defaults.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2581 2022-10-30 19:08:28.000000 flake8-6.1.0/src/flake8/discover_files.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2393 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/exceptions.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.823286 flake8-6.1.0/src/flake8/formatting/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       97 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/formatting/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2022 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/formatting/_windows_color.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7356 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/formatting/base.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3057 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/formatting/default.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.823286 flake8-6.1.0/src/flake8/main/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       98 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/main/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7949 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/main/application.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      599 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/main/cli.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      911 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/main/debug.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11008 2022-12-14 17:58:37.000000 flake8-6.1.0/src/flake8/main/options.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.827286 flake8-6.1.0/src/flake8/options/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      496 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/options/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1963 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/options/aggregator.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4572 2022-11-15 18:06:17.000000 flake8-6.1.0/src/flake8/options/config.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11525 2022-11-16 00:10:45.000000 flake8-6.1.0/src/flake8/options/manager.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2162 2022-12-21 17:38:20.000000 flake8-6.1.0/src/flake8/options/parse_args.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.827286 flake8-6.1.0/src/flake8/plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       92 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11154 2022-12-14 18:12:49.000000 flake8-6.1.0/src/flake8/plugins/finder.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5680 2023-07-29 17:28:33.000000 flake8-6.1.0/src/flake8/plugins/pycodestyle.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6717 2023-07-29 17:08:07.000000 flake8-6.1.0/src/flake8/plugins/pyflakes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1241 2022-11-15 18:06:17.000000 flake8-6.1.0/src/flake8/plugins/reporter.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    16599 2023-07-29 18:40:02.000000 flake8-6.1.0/src/flake8/processor.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4358 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/statistics.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14432 2022-12-14 17:58:37.000000 flake8-6.1.0/src/flake8/style_guide.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8168 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/utils.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2039 2022-10-30 18:55:43.000000 flake8-6.1.0/src/flake8/violation.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 19:04:44.823286 flake8-6.1.0/src/flake8.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3690 2023-07-29 19:04:44.000000 flake8-6.1.0/src/flake8.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1164 2023-07-29 19:04:44.000000 flake8-6.1.0/src/flake8.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-29 19:04:44.000000 flake8-6.1.0/src/flake8.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      422 2023-07-29 19:04:44.000000 flake8-6.1.0/src/flake8.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       72 2023-07-29 19:04:44.000000 flake8-6.1.0/src/flake8.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        7 2023-07-29 19:04:44.000000 flake8-6.1.0/src/flake8.egg-info/top_level.txt
```

### Comparing `flake8-6.0.0/LICENSE` & `flake8-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/PKG-INFO` & `flake8-6.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8
-Version: 6.0.0
+Version: 6.1.0
 Summary: the modular source code checker: pep8 pyflakes and co
 Home-page: https://github.com/pycqa/flake8
 Author: Tarek Ziade
 Author-email: tarek@ziade.org
 Maintainer: Ian Stapleton Cordasco
 Maintainer-email: graffatcolmingov@gmail.com
 License: MIT
@@ -107,9 +107,10 @@
 * `Getting Started Contributing
   <https://flake8.pycqa.org/en/latest/internal/contributing.html>`_
 
 
 Maintenance
 ===========
 
-Flake8 was created by Tarek Ziadé and is currently maintained by `Ian Cordasco
+Flake8 was created by Tarek Ziadé and is currently maintained by `anthony sottile
+<https://github.com/sponsors/asottile>`_ and `Ian Cordasco
 <https://www.coglib.com/~icordasc/>`_
```

### Comparing `flake8-6.0.0/README.rst` & `flake8-6.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -81,9 +81,10 @@
 * `Getting Started Contributing
   <https://flake8.pycqa.org/en/latest/internal/contributing.html>`_
 
 
 Maintenance
 ===========
 
-Flake8 was created by Tarek Ziadé and is currently maintained by `Ian Cordasco
+Flake8 was created by Tarek Ziadé and is currently maintained by `anthony sottile
+<https://github.com/sponsors/asottile>`_ and `Ian Cordasco
 <https://www.coglib.com/~icordasc/>`_
```

### Comparing `flake8-6.0.0/setup.cfg` & `flake8-6.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description_content_type = text/x-rst
 url = https://github.com/pycqa/flake8
 author = Tarek Ziade
 author_email = tarek@ziade.org
 maintainer = Ian Stapleton Cordasco
 maintainer_email = graffatcolmingov@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Framework :: Flake8
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
@@ -23,21 +23,21 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Software Development :: Quality Assurance
 
 [options]
 packages = find:
-package_dir = 
-	=src
 install_requires = 
 	mccabe>=0.7.0,<0.8.0
-	pycodestyle>=2.10.0,<2.11.0
-	pyflakes>=3.0.0,<3.1.0
+	pycodestyle>=2.11.0,<2.12.0
+	pyflakes>=3.1.0,<3.2.0
 python_requires = >=3.8.1
+package_dir = 
+	=src
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	flake8 = flake8.main.cli:main
```

### Comparing `flake8-6.0.0/src/flake8/__init__.py` & `flake8-6.1.0/src/flake8/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import logging
 import sys
 
 LOG = logging.getLogger(__name__)
 LOG.addHandler(logging.NullHandler())
 
-__version__ = "6.0.0"
+__version__ = "6.1.0"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
 
 _VERBOSITY_TO_LOG_LEVEL = {
     # output more than warnings but not debugging info
     1: logging.INFO,  # INFO is a numerical level of 20
     # output debugging information
     2: logging.DEBUG,  # DEBUG is a numerical level of 10
```

### Comparing `flake8-6.0.0/src/flake8/api/legacy.py` & `flake8-6.1.0/src/flake8/api/legacy.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/checker.py` & `flake8-6.1.0/src/flake8/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Sequence
 from typing import Tuple
 
 from flake8 import defaults
 from flake8 import exceptions
 from flake8 import processor
 from flake8 import utils
+from flake8._compat import FSTRING_START
 from flake8.discover_files import expand_paths
 from flake8.options.parse_args import parse_args
 from flake8.plugins.finder import Checkers
 from flake8.plugins.finder import LoadedPlugin
 from flake8.style_guide import StyleGuideManager
 
 Results = List[Tuple[str, int, int, str, Optional[str]]]
@@ -156,15 +157,15 @@
         # Otherwise, we know jobs should be an integer and we can just convert
         # it to an integer
         return jobs.n_jobs
 
     def _handle_results(self, filename: str, results: Results) -> int:
         style_guide = self.style_guide
         reported_results_count = 0
-        for (error_code, line_number, column, text, physical_line) in results:
+        for error_code, line_number, column, text, physical_line in results:
             reported_results_count += style_guide.handle_error(
                 code=error_code,
                 filename=filename,
                 line_number=line_number,
                 column_number=column,
                 text=text,
                 physical_line=physical_line,
@@ -419,15 +420,15 @@
             checker = self.run_check(plugin, tree=ast)
             # If the plugin uses a class, call the run method of it, otherwise
             # the call should return something iterable itself
             try:
                 runner = checker.run()
             except AttributeError:
                 runner = checker
-            for (line_number, offset, text, _) in runner:
+            for line_number, offset, text, _ in runner:
                 self.report(
                     error_code=None,
                     line_number=line_number,
                     column=offset,
                     text=text,
                 )
 
@@ -547,39 +548,39 @@
             self.run_logical_checks()
 
     def check_physical_eol(
         self, token: tokenize.TokenInfo, prev_physical: str
     ) -> None:
         """Run physical checks if and only if it is at the end of the line."""
         assert self.processor is not None
+        if token.type == FSTRING_START:  # pragma: >=3.12 cover
+            self.processor.fstring_start(token.start[0])
         # a newline token ends a single physical line.
-        if processor.is_eol_token(token):
+        elif processor.is_eol_token(token):
             # if the file does not end with a newline, the NEWLINE
             # token is inserted by the parser, but it does not contain
             # the previous physical line in `token[4]`
-            if token[4] == "":
+            if token.line == "":
                 self.run_physical_checks(prev_physical)
             else:
-                self.run_physical_checks(token[4])
+                self.run_physical_checks(token.line)
         elif processor.is_multiline_string(token):
             # Less obviously, a string that contains newlines is a
             # multiline string, either triple-quoted or with internal
             # newlines backslash-escaped. Check every physical line in the
             # string *except* for the last one: its newline is outside of
             # the multiline string, so we consider it a regular physical
             # line, and will check it like any other physical line.
             #
             # Subtleties:
             # - have to wind self.line_number back because initially it
             #   points to the last line of the string, and we want
             #   check_physical() to give accurate feedback
-            line_no = token[2][0]
-            with self.processor.inside_multiline(line_number=line_no):
-                for line in self.processor.split_line(token):
-                    self.run_physical_checks(line)
+            for line in self.processor.multiline_string(token):
+                self.run_physical_checks(line)
 
 
 def _try_initialize_processpool(
     job_count: int,
     argv: Sequence[str],
 ) -> multiprocessing.pool.Pool | None:
     """Return a new process pool instance if we are able to create one."""
```

### Comparing `flake8-6.0.0/src/flake8/defaults.py` & `flake8-6.1.0/src/flake8/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     "__pycache__",
     ".tox",
     ".nox",
     ".eggs",
     "*.egg",
 )
 IGNORE = ("E121", "E123", "E126", "E226", "E24", "E704", "W503", "W504")
-SELECT = ("E", "F", "W", "C90")
 MAX_LINE_LENGTH = 79
 INDENT_SIZE = 4
 
 # Other constants
 WHITESPACE = frozenset(" \t")
 
 STATISTIC_NAMES = ("logical lines", "physical lines", "tokens")
@@ -33,15 +32,14 @@
     # ``# noqa:E123,W451,F921``
     # ``# NoQA: E123,W451,F921``
     # ``# NOQA: E123,W451,F921``
     # ``# NOQA:E123,W451,F921``
     # We do not want to capture the ``: `` that follows ``noqa``
     # We do not care about the casing of ``noqa``
     # We want a comma-separated list of errors
-    # https://regex101.com/r/4XUuax/2 full explanation of the regex
     r"# noqa(?::[\s]?(?P<codes>([A-Z]+[0-9]+(?:[,\s]+)?)+))?",
     re.IGNORECASE,
 )
 
 NOQA_FILE = re.compile(r"\s*# flake8[:=]\s*noqa", re.I)
 
 VALID_CODE_PREFIX = re.compile("^[A-Z]{1,3}[0-9]{0,3}$", re.ASCII)
```

### Comparing `flake8-6.0.0/src/flake8/discover_files.py` & `flake8-6.1.0/src/flake8/discover_files.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/exceptions.py` & `flake8-6.1.0/src/flake8/exceptions.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/formatting/_windows_color.py` & `flake8-6.1.0/src/flake8/formatting/_windows_color.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/formatting/base.py` & `flake8-6.1.0/src/flake8/formatting/base.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/formatting/default.py` & `flake8-6.1.0/src/flake8/formatting/default.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/main/application.py` & `flake8-6.1.0/src/flake8/main/application.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/main/cli.py` & `flake8-6.1.0/src/flake8/main/cli.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/main/debug.py` & `flake8-6.1.0/src/flake8/main/debug.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/main/options.py` & `flake8-6.1.0/src/flake8/main/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -293,28 +293,32 @@
 
     add_option(
         "--select",
         metavar="errors",
         parse_from_config=True,
         comma_separated_list=True,
         help=(
-            f"Comma-separated list of error codes to enable. "
-            f"For example, ``--select=E4,E51,W234``. "
-            f"(Default: {','.join(defaults.SELECT)})"
+            "Limit the reported error codes to codes prefix-matched by this "
+            "list.  "
+            "You usually do not need to specify this option as the default "
+            "includes all installed plugin codes.  "
+            "For example, ``--select=E4,E51,W234``."
         ),
     )
 
     add_option(
         "--extend-select",
         metavar="errors",
         parse_from_config=True,
         comma_separated_list=True,
         help=(
-            "Comma-separated list of error codes to add to the list "
-            "of selected ones. For example, ``--extend-select=E4,E51,W234``."
+            "Add additional error codes to the default ``--select``.  "
+            "You usually do not need to specify this option as the default "
+            "includes all installed plugin codes.  "
+            "For example, ``--extend-select=E4,E51,W234``."
         ),
     )
 
     add_option(
         "--disable-noqa",
         default=False,
         parse_from_config=True,
```

### Comparing `flake8-6.0.0/src/flake8/options/aggregator.py` & `flake8-6.1.0/src/flake8/options/aggregator.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/options/config.py` & `flake8-6.1.0/src/flake8/options/config.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/options/manager.py` & `flake8-6.1.0/src/flake8/options/manager.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/options/parse_args.py` & `flake8-6.1.0/src/flake8/options/parse_args.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/plugins/finder.py` & `flake8-6.1.0/src/flake8/plugins/finder.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/plugins/pycodestyle.py` & `flake8-6.1.0/src/flake8/plugins/pycodestyle.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 from pycodestyle import extraneous_whitespace as _extraneous_whitespace
 from pycodestyle import imports_on_separate_lines as _imports_on_separate_lines
 from pycodestyle import indentation as _indentation
 from pycodestyle import maximum_doc_length as _maximum_doc_length
 from pycodestyle import maximum_line_length as _maximum_line_length
 from pycodestyle import missing_whitespace as _missing_whitespace
 from pycodestyle import missing_whitespace_after_keyword as _missing_whitespace_after_keyword  # noqa: E501
-from pycodestyle import missing_whitespace_around_operator as _missing_whitespace_around_operator  # noqa: E501
 from pycodestyle import module_imports_on_top_of_file as _module_imports_on_top_of_file  # noqa: E501
-from pycodestyle import python_3000_async_await_keywords as _python_3000_async_await_keywords  # noqa: E501
 from pycodestyle import python_3000_invalid_escape_sequence as _python_3000_invalid_escape_sequence  # noqa: E501
 from pycodestyle import tabs_obsolete as _tabs_obsolete
 from pycodestyle import tabs_or_spaces as _tabs_or_spaces
 from pycodestyle import trailing_blank_lines as _trailing_blank_lines
 from pycodestyle import trailing_whitespace as _trailing_whitespace
 from pycodestyle import whitespace_around_comma as _whitespace_around_comma
 from pycodestyle import whitespace_around_keywords as _whitespace_around_keywords  # noqa: E501
@@ -70,19 +68,17 @@
     yield from _compound_statements(logical_line)
     yield from _continued_indentation(logical_line, tokens, indent_level, hang_closing, indent_char, indent_size, noqa, verbose)  # noqa: E501
     yield from _explicit_line_join(logical_line, tokens)
     yield from _extraneous_whitespace(logical_line)
     yield from _imports_on_separate_lines(logical_line)
     yield from _indentation(logical_line, previous_logical, indent_char, indent_level, previous_indent_level, indent_size)  # noqa: E501
     yield from _maximum_doc_length(logical_line, max_doc_length, noqa, tokens)
-    yield from _missing_whitespace(logical_line)
+    yield from _missing_whitespace(logical_line, tokens)
     yield from _missing_whitespace_after_keyword(logical_line, tokens)
-    yield from _missing_whitespace_around_operator(logical_line, tokens)
     yield from _module_imports_on_top_of_file(logical_line, indent_level, checker_state, noqa)  # noqa: E501
-    yield from _python_3000_async_await_keywords(logical_line, tokens)
     yield from _python_3000_invalid_escape_sequence(logical_line, tokens, noqa)
     yield from _whitespace_around_comma(logical_line)
     yield from _whitespace_around_keywords(logical_line)
     yield from _whitespace_around_named_parameter_equals(logical_line, tokens)
     yield from _whitespace_around_operator(logical_line)
     yield from _whitespace_before_comment(logical_line, tokens)
     yield from _whitespace_before_parameters(logical_line, tokens)
```

### Comparing `flake8-6.0.0/src/flake8/plugins/pyflakes.py` & `flake8-6.1.0/src/flake8/plugins/pyflakes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Plugin built-in to Flake8 to treat pyflakes as a plugin."""
 from __future__ import annotations
 
 import argparse
 import ast
+import logging
 import os
 from typing import Any
 from typing import Generator
 
 import pyflakes.checker
 
 from flake8 import utils
 from flake8.options.manager import OptionManager
 
+LOG = logging.getLogger(__name__)
+
 FLAKE8_PYFLAKES_CODES = {
     "UnusedImport": "F401",
     "ImportShadowedByLoopVar": "F402",
     "ImportStarUsed": "F403",
     "LateFutureImport": "F404",
     "ImportStarUsage": "F405",
     "ImportStarNotPermitted": "F406",
@@ -41,15 +44,14 @@
     "TwoStarredExpressions": "F622",
     "AssertTuple": "F631",
     "IsLiteral": "F632",
     "InvalidPrintSyntax": "F633",
     "IfTuple": "F634",
     "BreakOutsideLoop": "F701",
     "ContinueOutsideLoop": "F702",
-    "ContinueInFinally": "F703",
     "YieldOutsideFunction": "F704",
     "ReturnOutsideFunction": "F706",
     "DefaultExceptNotLast": "F707",
     "DoctestSyntaxError": "F721",
     "ForwardAnnotationSyntaxError": "F722",
     "RedefinedWhileUnused": "F811",
     "UndefinedName": "F821",
@@ -133,14 +135,20 @@
     @classmethod
     def parse_options(cls, options: argparse.Namespace) -> None:
         """Parse option values from Flake8's OptionManager."""
         if options.builtins:
             cls.builtIns = cls.builtIns.union(options.builtins)
         cls.with_doctest = options.doctests
 
+        if options.include_in_doctest or options.exclude_from_doctest:
+            LOG.warning(
+                "--include-in-doctest / --exclude-from-doctest will be "
+                "removed in a future version.  see PyCQA/flake8#1747"
+            )
+
         included_files = []
         for included_file in options.include_in_doctest:
             if included_file == "":
                 continue
             if not included_file.startswith((os.sep, "./", "~/")):
                 included_files.append(f"./{included_file}")
             else:
```

### Comparing `flake8-6.0.0/src/flake8/plugins/reporter.py` & `flake8-6.1.0/src/flake8/plugins/reporter.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/processor.py` & `flake8-6.1.0/src/flake8/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Module containing our file processor that tokenizes a file for checks."""
 from __future__ import annotations
 
 import argparse
 import ast
-import contextlib
 import logging
 import tokenize
 from typing import Any
 from typing import Generator
 from typing import List
 from typing import Tuple
 
 from flake8 import defaults
 from flake8 import utils
+from flake8._compat import FSTRING_END
+from flake8._compat import FSTRING_MIDDLE
 from flake8.plugins.finder import LoadedPlugin
 
 LOG = logging.getLogger(__name__)
 NEWLINE = frozenset([tokenize.NL, tokenize.NEWLINE])
 
 SKIP_TOKENS = frozenset(
     [tokenize.NL, tokenize.NEWLINE, tokenize.INDENT, tokenize.DEDENT]
@@ -112,34 +113,47 @@
         #: Verbosity level of Flake8
         self.verbose = options.verbose
         #: Statistics dictionary
         self.statistics = {"logical lines": 0}
         self._file_tokens: list[tokenize.TokenInfo] | None = None
         # map from line number to the line we'll search for `noqa` in
         self._noqa_line_mapping: dict[int, str] | None = None
+        self._fstring_start = -1
 
     @property
     def file_tokens(self) -> list[tokenize.TokenInfo]:
         """Return the complete set of tokens for a file."""
         if self._file_tokens is None:
             line_iter = iter(self.lines)
             self._file_tokens = list(
                 tokenize.generate_tokens(lambda: next(line_iter))
             )
 
         return self._file_tokens
 
-    @contextlib.contextmanager
-    def inside_multiline(
-        self, line_number: int
-    ) -> Generator[None, None, None]:
-        """Context-manager to toggle the multiline attribute."""
-        self.line_number = line_number
+    def fstring_start(self, lineno: int) -> None:
+        """Signal the beginning of an fstring."""
+        self._fstring_start = lineno
+
+    def multiline_string(
+        self, token: tokenize.TokenInfo
+    ) -> Generator[str, None, None]:
+        """Iterate through the lines of a multiline string."""
+        if token.type == FSTRING_END:
+            start = self._fstring_start
+        else:
+            start = token.start[0]
+
         self.multiline = True
-        yield
+        self.line_number = start
+        # intentionally don't include the last line, that line will be
+        # terminated later by a future end-of-line
+        for _ in range(start, token.end[0]):
+            yield self.lines[self.line_number - 1]
+            self.line_number += 1
         self.multiline = False
 
     def reset_blank_before(self) -> None:
         """Reset the blank_before attribute to zero."""
         self.blank_before = 0
 
     def delete_first_token(self) -> None:
@@ -174,15 +188,15 @@
             self.previous_indent_level = self.indent_level
             self.previous_logical = self.logical_line
             if not self.indent_level:
                 self.previous_unindented_logical_line = self.logical_line
         self.blank_lines = 0
         self.tokens = []
 
-    def build_logical_line_tokens(self) -> _Logical:
+    def build_logical_line_tokens(self) -> _Logical:  # noqa: C901
         """Build the mapping, comments, and logical line lists."""
         logical = []
         comments = []
         mapping: _LogicalMapping = []
         length = 0
         previous_row = previous_column = None
         for token_type, text, start, end, line in self.tokens:
@@ -191,14 +205,16 @@
             if not mapping:
                 mapping = [(0, start)]
             if token_type == tokenize.COMMENT:
                 comments.append(text)
                 continue
             if token_type == tokenize.STRING:
                 text = mutate_string(text)
+            elif token_type == FSTRING_MIDDLE:
+                text = "x" * len(text)
             if previous_row:
                 (start_row, start_column) = start
                 if previous_row != start_row:
                     row_index = previous_row - 1
                     column_index = previous_column - 1
                     previous_text = self.lines[row_index][column_index]
                     if previous_text == "," or (
@@ -221,27 +237,14 @@
         """Build a logical line from the current tokens list."""
         comments, logical, mapping_list = self.build_logical_line_tokens()
         joined_comments = "".join(comments)
         self.logical_line = "".join(logical)
         self.statistics["logical lines"] += 1
         return joined_comments, self.logical_line, mapping_list
 
-    def split_line(
-        self, token: tokenize.TokenInfo
-    ) -> Generator[str, None, None]:
-        """Split a physical line's line based on new-lines.
-
-        This also auto-increments the line number for the caller.
-        """
-        # intentionally don't include the last line, that line will be
-        # terminated later by a future end-of-line
-        for line_no in range(token.start[0], token.end[0]):
-            yield self.lines[line_no - 1]
-            self.line_number += 1
-
     def keyword_arguments_for(
         self,
         parameters: dict[str, bool],
         arguments: dict[str, Any],
     ) -> dict[str, Any]:
         """Generate the keyword arguments for a list of parameters."""
         ret = {}
@@ -388,15 +391,17 @@
 def is_eol_token(token: tokenize.TokenInfo) -> bool:
     """Check if the token is an end-of-line token."""
     return token[0] in NEWLINE or token[4][token[3][1] :].lstrip() == "\\\n"
 
 
 def is_multiline_string(token: tokenize.TokenInfo) -> bool:
     """Check if this is a multiline string."""
-    return token[0] == tokenize.STRING and "\n" in token[1]
+    return token.type == FSTRING_END or (
+        token.type == tokenize.STRING and "\n" in token.string
+    )
 
 
 def token_is_newline(token: tokenize.TokenInfo) -> bool:
     """Check if the token type is a newline token type."""
     return token[0] in NEWLINE
```

### Comparing `flake8-6.0.0/src/flake8/statistics.py` & `flake8-6.1.0/src/flake8/statistics.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/style_guide.py` & `flake8-6.1.0/src/flake8/style_guide.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self.ignored_explicitly = _explicitly_chosen(
             option=options.ignore,
             extend=options.extend_ignore,
         )
 
         self.selected = _select_ignore(
             option=options.select,
-            default=defaults.SELECT,
+            default=(),
             extended_default=options.extended_default_select,
             extend=options.extend_select,
         )
         self.ignored = _select_ignore(
             option=options.ignore,
             default=defaults.IGNORE,
             extended_default=options.extended_default_ignore,
```

### Comparing `flake8-6.0.0/src/flake8/utils.py` & `flake8-6.1.0/src/flake8/utils.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8/violation.py` & `flake8-6.1.0/src/flake8/violation.py`

 * *Files identical despite different names*

### Comparing `flake8-6.0.0/src/flake8.egg-info/PKG-INFO` & `flake8-6.1.0/src/flake8.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8
-Version: 6.0.0
+Version: 6.1.0
 Summary: the modular source code checker: pep8 pyflakes and co
 Home-page: https://github.com/pycqa/flake8
 Author: Tarek Ziade
 Author-email: tarek@ziade.org
 Maintainer: Ian Stapleton Cordasco
 Maintainer-email: graffatcolmingov@gmail.com
 License: MIT
@@ -107,9 +107,10 @@
 * `Getting Started Contributing
   <https://flake8.pycqa.org/en/latest/internal/contributing.html>`_
 
 
 Maintenance
 ===========
 
-Flake8 was created by Tarek Ziadé and is currently maintained by `Ian Cordasco
+Flake8 was created by Tarek Ziadé and is currently maintained by `anthony sottile
+<https://github.com/sponsors/asottile>`_ and `Ian Cordasco
 <https://www.coglib.com/~icordasc/>`_
```

