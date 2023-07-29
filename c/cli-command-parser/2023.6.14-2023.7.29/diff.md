# Comparing `tmp/cli_command_parser-2023.6.14.tar.gz` & `tmp/cli_command_parser-2023.7.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.6.14.tar", last modified: Wed Jun 14 11:33:24 2023, max compression
+gzip compressed data, was "cli_command_parser-2023.7.29.tar", last modified: Sat Jul 29 13:18:34 2023, max compression
```

## Comparing `cli_command_parser-2023.6.14.tar` & `cli_command_parser-2023.7.29.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.916368 cli_command_parser-2023.6.14/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/MANIFEST.in
--rw-rw-rw-   0        0        0     5611 2023-06-14 11:33:24.916368 cli_command_parser-2023.6.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.777369 cli_command_parser-2023.6.14/lib/
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.840368 cli_command_parser-2023.6.14/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1158 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-06-14 11:33:14.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0     2430 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19228 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12619 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    18449 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    18586 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.866369 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8297 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.879368 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     9618 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    20740 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5445 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.901370 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6582 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8897 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0     7601 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/patterns.py
--rw-rw-rw-   0        0        0    22732 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    13618 2023-05-20 18:50:11.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.915368 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    16944 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/actions.py
--rw-rw-rw-   0        0        0    22558 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    16514 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10656 2023-05-13 19:45:03.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     8242 2023-05-21 20:53:58.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    24296 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4422 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    16701 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    12301 2023-06-14 11:32:55.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1882 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     5216 2023-05-29 16:32:28.000000 cli_command_parser-2023.6.14/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:33:24.850368 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     5611 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 11:33:24.000000 cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.6.14/pyproject.toml
--rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.6.14/readme.rst
--rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.6.14/requirements-dev.txt
--rw-rw-rw-   0        0        0     1293 2023-06-14 11:33:24.917369 cli_command_parser-2023.6.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.900525 cli_command_parser-2023.7.29/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/MANIFEST.in
+-rw-rw-rw-   0        0        0     5611 2023-07-29 13:18:34.901523 cli_command_parser-2023.7.29/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.694523 cli_command_parser-2023.7.29/lib/
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.778522 cli_command_parser-2023.7.29/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1158 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2023-07-29 13:18:24.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0     2430 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19228 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    12838 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    18449 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    19091 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.816522 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8297 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.830522 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     9604 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    20856 2023-07-29 13:17:30.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5445 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.863523 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6582 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     8897 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0     7601 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/patterns.py
+-rw-rw-rw-   0        0        0    22732 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    13618 2023-05-20 18:50:11.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.900525 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    16944 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/actions.py
+-rw-rw-rw-   0        0        0    22558 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    16514 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    10656 2023-05-13 19:45:03.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     8242 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    24296 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4422 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    16701 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    12301 2023-06-14 11:32:55.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1882 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     5216 2023-05-29 16:32:28.000000 cli_command_parser-2023.7.29/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:18:34.790524 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     5611 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-29 13:18:34.000000 cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.29/pyproject.toml
+-rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.7.29/readme.rst
+-rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.7.29/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1293 2023-07-29 13:18:34.904523 cli_command_parser-2023.7.29/setup.cfg
```

### Comparing `cli_command_parser-2023.6.14/LICENSE` & `cli_command_parser-2023.7.29/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/PKG-INFO` & `cli_command_parser-2023.7.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.6.14
+Version: 2023.7.29
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/__init__.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/annotations.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/annotations.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/command_parameters.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/commands.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,14 +162,16 @@
         Validates the number of ActionFlags that were specified, and calls all of the specified
         :func:`~.options.before_main` / :obj:`~.options.action_flag` actions such as ``--help`` that were
         defined with ``before_main=True`` and ``always_available=True`` in their configured order.
 
         :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
         :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
+        # TODO: --help should take precedence over input validation - right now, if a Path input expecting a
+        #  non-existent file receives a file that exists, that error is reported instead of showing help text
         ctx = self.__ctx
         n_flags = ctx.action_flag_count
         if n_flags and not ctx.config.multiple_action_flags and n_flags > 1:
             raise ParamConflict(ctx.all_action_flags, 'combining multiple action flags is disabled')
 
         if before := ctx.categorized_action_flags[ActionPhase.BEFORE_MAIN]:
             action = get_params(self).action
```

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/compat.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/compat.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/config.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/config.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/context.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,38 +135,46 @@
     def terminal_width(self) -> int:
         """Returns the current terminal width as the number of characters that fit on a single line."""
         if (width := self._terminal_width) is not None:
             return width
         return _TERMINAL.width
 
     def get_parsed(
-        self, exclude: Collection[Parameter] = (), recursive: Bool = True, default: Any = None
+        self,
+        exclude: Collection[Parameter] = (),
+        recursive: Bool = True,
+        default: Any = None,
+        include_defaults: Bool = True,
     ) -> Dict[str, Any]:
         """
         Returns all of the parsed arguments as a dictionary.
 
         The :ref:`get_parsed() <advanced:Parsed Args as a Dictionary>` helper function provides an easier way to access
         this functionality.
 
         :param exclude: Parameter objects that should be excluded from the returned results
         :param recursive: Whether parsed arguments should be recursively gathered from parent Commands
         :param default: The default value to use for parameters that raise :class:`.MissingArgument` when attempting to
           obtain their result values.
+        :param include_defaults: Whether default values should be included in the returned results.  If False, only
+          user-provided values will be included.
         :return: A dictionary containing all of the arguments that were parsed.  The keys in the returned dict match
           the names assigned to the Parameters in the Command associated with this Context.
         """
         with self:
             if recursive and (parent := self.parent):
-                parsed = parent.get_parsed(exclude, recursive)
+                parsed = parent.get_parsed(exclude, recursive, default, include_defaults)
             else:
                 parsed = {}
 
+            # TODO: Add way to get a nested dict with ParamGroup names as the keys of the nested sections?
             if params := self.params:
                 for param in params.iter_params(exclude):
-                    parsed[param.name] = param.result_value(default)
+                    if include_defaults or param in self._parsed:
+                        parsed[param.name] = param.result_value(default)
 
         return parsed
 
     @cached_property
     def params(self) -> Optional[CommandParameters]:
         """
         The :class:`.CommandParameters` object that contains the categorized Parameters from the Command associated
@@ -434,15 +442,17 @@
     """
     try:
         return command._Command__ctx  # noqa
     except AttributeError as e:
         raise TypeError('get_context only supports Command objects') from e
 
 
-def get_parsed(command: Command, to_call: Callable = None, default: Any = None) -> Dict[str, Any]:
+def get_parsed(
+    command: Command, to_call: Callable = None, default: Any = None, include_defaults: Bool = True
+) -> Dict[str, Any]:
     """
     Provides a way to obtain all of the arguments that were parsed for the given Command as a dictionary.
 
     If the parsed arguments are intended to be used to call a particular function/method, or to initialize a particular
     class, then that callable can be provided as the ``to_call`` parameter to filter the parsed arguments to only the
     ones that would be accepted by it.  It will not be called by this function.
 
@@ -458,15 +468,15 @@
       be used to filter the parsed arguments.  If provided, then only the keys that match the callable's signature will
       be included in the returned dictionary of parsed arguments.
     :param default: The default value to use for parameters that raise :class:`.MissingArgument` when attempting to
       obtain their result values.
     :return: A dictionary containing all of the (optionally filtered) arguments that were parsed.  The keys in the
       returned dict match the names assigned to the Parameters in the given Command.
     """
-    parsed = get_context(command).get_parsed(default=default)
+    parsed = get_context(command).get_parsed(default=default, include_defaults=include_defaults)
     if to_call is not None:
         sig = Signature.from_callable(to_call)
         keys = {k for k, p in sig.parameters.items() if p.kind != _Parameter.VAR_KEYWORD}
         parsed = {k: v for k, v in parsed.items() if k in keys}
 
     return parsed
```

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/command_builder.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/conversion/visitor.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/core.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/core.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/documentation.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/documentation.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,41 +31,44 @@
 
 
 class CommandHelpFormatter:
     def __init__(self, command: CommandType, params: CommandParameters):
         self.command = command
         self.params = params
         self.pos_group = ParamGroup(description='Positional arguments')
+        self.req_group = ParamGroup(description='Required arguments')
         self.opt_group = ParamGroup(description='Optional arguments')
-        self.groups = [self.pos_group, self.opt_group]
+        self.groups = [self.pos_group, self.req_group, self.opt_group]
 
     @cached_property
     def _meta(self) -> ProgramMetadata:
         return get_metadata(self.command)
 
     def maybe_add_groups(self, groups: Iterable[ParamGroup]):
         for group in groups:
             if group.group:  # prevent duplicates
                 continue
             if group.contains_positional:
                 self.pos_group.add(group)
             else:
                 self.groups.append(group)
 
-    def maybe_add_option(self, param: Optional[Parameter]):
-        if param is not None and not param.group:
-            self.opt_group.add(param)
-
     def maybe_add_positionals(self, params: Iterable[BasePositional]):
         self.pos_group.extend(param for param in params if not param.group)
 
+    def maybe_add_option(self, param: Optional[Parameter]):
+        if param is not None and not param.group:
+            if param.required:
+                self.req_group.add(param)
+            else:
+                self.opt_group.add(param)
+
     def maybe_add_options(self, params: Iterable[BaseOption]):
-        # TODO: It would be good for required options' default group to indicate they are required, instead of the
-        #  default group saying "Optional"
-        self.opt_group.extend(param for param in params if not param.group)
+        for param in params:
+            self.maybe_add_option(param)
 
     def _iter_params(self) -> Iterator[Union[BasePositional, BaseOption, PassThru]]:
         params = self.params
         yield from params.all_positionals
         yield from params.options
         if (pass_thru := params.pass_thru) is not None:
             yield pass_thru
@@ -101,18 +104,15 @@
         return delim.join(parts)
 
     def format_help(self, allow_sys_argv: Bool = True) -> str:
         parts = [self.format_usage(allow_sys_argv=allow_sys_argv), '']
         if description := self._meta.description:
             parts += [description, '']
 
-        for group in self.groups:
-            if group.show_in_help:
-                parts.append(group.formatter.format_help())
-
+        parts.extend(group.formatter.format_help() for group in self.groups if group.show_in_help)
         if epilog := self._meta.format_epilog(ctx.config.extended_epilog, allow_sys_argv):
             parts.append(epilog)
 
         return '\n'.join(parts)
 
     # region RST Formatting
```

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # pylint: disable=W0613
 
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Type, Callable, Iterator, Iterable, Tuple, Dict
 
-from ..config import SubcommandAliasHelpMode
+from ..config import SubcommandAliasHelpMode, CmdAliasMode
 from ..context import ctx
 from ..core import get_config
 from ..parameters.base import BasePositional, BaseOption
 from ..parameters.choice_map import ChoiceMap, Choice
 from ..parameters import ParamGroup, PassThru, TriFlag
 from .restructured_text import RstTable
 from .utils import format_help_entry, _should_add_default
@@ -300,30 +300,32 @@
         return target_choice_map.values()
 
     def add(self, choice: Choice):
         self.choices.append(choice)
         if choice_str := choice.choice:
             self.choice_strs.append(choice_str)
 
-    def format(self, default_mode: SubcommandAliasHelpMode, tw_offset: int = 0, prefix: str = '') -> Iterator[str]:
+    def format(self, default_mode: CmdAliasMode, tw_offset: int = 0, prefix: str = '') -> Iterator[str]:
         """
-        :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured.
+        :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured,
+          or the format string to use for subcommand aliases.
         :param tw_offset: Terminal width offset for text width calculations.
         :param prefix: Prefix to add to every line (primarily intended for use with nested groups).
         :return: Generator that yields formatted help text entries (strings) for the Choices in this group.
         """
         for choice, usage, description in self.prepare(default_mode):
             yield format_help_entry((usage,), description, lpad=4, tw_offset=tw_offset, prefix=prefix)
 
-    def prepare(self, default_mode: SubcommandAliasHelpMode) -> Iterator[Tuple[Choice, OptStr, OptStr]]:
+    def prepare(self, default_mode: CmdAliasMode) -> Iterator[Tuple[Choice, OptStr, OptStr]]:
         """
         Prepares the choice values and descriptions to use for each Choice in this group based on the configured alias
         mode.
 
-        :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured.
+        :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured,
+          or the format string to use for subcommand aliases.
         :return: Generator that yields 3-tuples containing the :class:`.Choice` object, the choice string value, and
           the help text / description for that choice / alias.
         """
         first = self.choices[0]
         # If it's not a Command, get_config will return None.  If it is a Command, then it will use its config.  If the
         # alias mode is not set on that target Command, but it is set on its parent, then this will use that parent's
         # setting.
```

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/choices.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/files.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/numeric.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/patterns.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/patterns.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/time.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/metadata.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/metadata.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/nargs.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/nargs.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/actions.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/actions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/choice_map.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/option_strings.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/options.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parameters/positionals.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parse_tree.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/parser.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/testing.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/testing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/typing.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/typing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser/utils.py` & `cli_command_parser-2023.7.29/lib/cli_command_parser/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-command-parser
-Version: 2023.6.14
+Version: 2023.7.29
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.6.14/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2023.7.29/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/readme.rst` & `cli_command_parser-2023.7.29/readme.rst`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.6.14/setup.cfg` & `cli_command_parser-2023.7.29/setup.cfg`

 * *Files identical despite different names*

