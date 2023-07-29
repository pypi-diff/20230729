# Comparing `tmp/pmvcs-1.0.1.tar.gz` & `tmp/pmvcs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmvcs-1.0.1.tar", last modified: Wed Jul 26 15:09:07 2023, max compression
+gzip compressed data, was "pmvcs-1.0.2.tar", last modified: Sat Jul 29 21:29:43 2023, max compression
```

## Comparing `pmvcs-1.0.1.tar` & `pmvcs-1.0.2.tar`

### file list

```diff
@@ -1,136 +1,176 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/
--rw-rw-rw-   0        0        0      589 2023-07-26 15:00:48.000000 pmvcs-1.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    35823 2023-07-10 09:52:19.000000 pmvcs-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      894 2023-07-26 15:02:59.000000 pmvcs-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7460 2023-07-26 15:09:07.860775 pmvcs-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7424 2023-07-26 14:57:22.000000 pmvcs-1.0.1/README.ES.md
--rw-rw-rw-   0        0        0     6740 2023-07-26 14:57:46.000000 pmvcs-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/__init__.py
--rw-rw-rw-   0        0        0      134 2023-07-10 10:34:58.000000 pmvcs-1.0.1/pmvcs/__main__.py
--rw-rw-rw-   0        0        0      129 2023-07-26 15:01:51.000000 pmvcs-1.0.1/pmvcs/__version__.py
--rw-rw-rw-   0        0        0     1595 2023-07-26 00:50:16.000000 pmvcs-1.0.1/pmvcs/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs/core/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs/core/controllers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/controllers/__init__.py
--rw-rw-rw-   0        0        0     3292 2023-07-24 03:47:22.000000 pmvcs-1.0.1/pmvcs/core/controllers/base_controller.py
--rw-rw-rw-   0        0        0     3271 2023-07-24 03:36:42.000000 pmvcs-1.0.1/pmvcs/core/controllers/menus.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.800813 pmvcs-1.0.1/pmvcs/core/decorators/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/decorators/__init__.py
--rw-rw-rw-   0        0        0      920 2023-07-26 14:00:32.000000 pmvcs-1.0.1/pmvcs/core/decorators/decorators_views.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.800813 pmvcs-1.0.1/pmvcs/core/helpers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/helpers/__init__.py
--rw-rw-rw-   0        0        0     1107 2023-07-24 03:29:48.000000 pmvcs-1.0.1/pmvcs/core/helpers/base_helper.py
--rw-rw-rw-   0        0        0     1440 2023-07-24 03:16:46.000000 pmvcs-1.0.1/pmvcs/core/helpers/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.810935 pmvcs-1.0.1/pmvcs/core/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/interfaces/__init__.py
--rw-rw-rw-   0        0        0      730 2023-07-24 02:56:34.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_controller.py
--rw-rw-rw-   0        0        0      197 2023-07-13 14:26:55.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_helper.py
--rw-rw-rw-   0        0        0     1746 2023-07-24 03:21:41.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_model.py
--rw-rw-rw-   0        0        0     1764 2023-07-24 03:04:12.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_view.py
--rw-rw-rw-   0        0        0      941 2023-07-24 02:59:42.000000 pmvcs-1.0.1/pmvcs/core/interfaces/menus.py
--rw-rw-rw-   0        0        0     2025 2023-07-24 03:05:25.000000 pmvcs-1.0.1/pmvcs/core/interfaces/router.py
--rw-rw-rw-   0        0        0      933 2023-07-24 00:28:53.000000 pmvcs-1.0.1/pmvcs/core/interfaces/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.810935 pmvcs-1.0.1/pmvcs/core/models/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/models/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:04.000000 pmvcs-1.0.1/pmvcs/core/models/about.py
--rw-rw-rw-   0        0        0     1977 2023-07-24 03:18:08.000000 pmvcs-1.0.1/pmvcs/core/models/base_model.py
--rw-rw-rw-   0        0        0      688 2023-07-12 06:21:03.000000 pmvcs-1.0.1/pmvcs/core/models/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.810935 pmvcs-1.0.1/pmvcs/core/models/entities/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/models/entities/__init__.py
--rw-rw-rw-   0        0        0     2312 2023-07-24 03:44:22.000000 pmvcs-1.0.1/pmvcs/core/models/language.py
--rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:41.000000 pmvcs-1.0.1/pmvcs/core/models/menus.py
--rw-rw-rw-   0        0        0     3239 2023-07-24 02:38:28.000000 pmvcs-1.0.1/pmvcs/core/models/parser.py
--rw-rw-rw-   0        0        0     5082 2023-07-24 05:01:16.000000 pmvcs-1.0.1/pmvcs/core/router.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.820867 pmvcs-1.0.1/pmvcs/core/setup/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.820867 pmvcs-1.0.1/pmvcs/core/setup/languages/
--rw-rw-rw-   0        0        0     2113 2023-07-23 19:31:08.000000 pmvcs-1.0.1/pmvcs/core/setup/languages/en.setup.ini
--rw-rw-rw-   0        0        0     2409 2023-07-23 21:29:37.000000 pmvcs-1.0.1/pmvcs/core/setup/languages/es.setup.ini
--rw-rw-rw-   0        0        0     3251 2023-07-24 03:46:11.000000 pmvcs-1.0.1/pmvcs/core/setup/setup.py
--rw-rw-rw-   0        0        0     3419 2023-07-24 02:35:12.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_config_file.py
--rw-rw-rw-   0        0        0      718 2023-07-23 23:48:39.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_defaults.py
--rw-rw-rw-   0        0        0     1035 2023-07-23 23:59:48.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_example.py
--rw-rw-rw-   0        0        0     1541 2023-07-23 22:57:42.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_extras.py
--rw-rw-rw-   0        0        0     4361 2023-07-24 04:48:12.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_files.py
--rw-rw-rw-   0        0        0     4878 2023-07-24 03:46:58.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_install.py
--rw-rw-rw-   0        0        0     3128 2023-07-24 04:06:23.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_menus.py
--rw-rw-rw-   0        0        0     3734 2023-07-24 05:13:48.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_multiple.py
--rw-rw-rw-   0        0        0      957 2023-07-23 22:57:43.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_parser.py
--rw-rw-rw-   0        0        0     1952 2023-07-23 23:56:31.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_unique.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/core/views/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/views/__init__.py
--rw-rw-rw-   0        0        0     2813 2023-07-24 03:04:20.000000 pmvcs-1.0.1/pmvcs/core/views/base_view.py
--rw-rw-rw-   0        0        0     5226 2023-07-24 04:56:15.000000 pmvcs-1.0.1/pmvcs/core/views/sample.py
--rw-rw-rw-   0        0        0      803 2023-07-24 05:10:48.000000 pmvcs-1.0.1/pmvcs/pmvcs.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/__init__.py
--rw-rw-rw-   0        0        0      169 2023-07-12 07:38:03.000000 pmvcs-1.0.1/pmvcs/setup/app.py
--rw-rw-rw-   0        0        0      683 2023-07-13 21:01:35.000000 pmvcs-1.0.1/pmvcs/setup/config.ini
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/controllers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/controllers/__init__.py
--rw-rw-rw-   0        0        0      874 2023-07-23 22:57:44.000000 pmvcs-1.0.1/pmvcs/setup/defaults/controllers/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/decorators/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/helpers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/__init__.py
--rw-rw-rw-   0        0        0      266 2023-07-23 23:45:10.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/base_controller.py
--rw-rw-rw-   0        0        0      161 2023-07-12 21:12:21.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/base_model.py
--rw-rw-rw-   0        0        0      142 2023-07-12 21:10:40.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/base_view.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/languages/
--rw-rw-rw-   0        0        0      547 2023-07-13 20:50:52.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.about.ini
--rw-rw-rw-   0        0        0      427 2023-07-13 20:59:38.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.ini
--rw-rw-rw-   0        0        0        7 2023-07-23 17:22:52.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.menus.ini
--rw-rw-rw-   0        0        0      590 2023-07-13 20:50:43.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.about.ini
--rw-rw-rw-   0        0        0      467 2023-07-26 14:23:27.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.ini
--rw-rw-rw-   0        0        0        7 2023-07-23 17:22:57.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.menus.ini
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/models/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/models/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-12 21:12:40.000000 pmvcs-1.0.1/pmvcs/setup/defaults/models/base_model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/models/entities/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/defaults/views/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/views/__init__.py
--rw-rw-rw-   0        0        0      499 2023-07-12 21:13:12.000000 pmvcs-1.0.1/pmvcs/setup/defaults/views/base_view.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.770691 pmvcs-1.0.1/pmvcs/setup/example/
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/example/controllers/
--rw-rw-rw-   0        0        0     1462 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/example/controllers/base_controller.py
--rw-rw-rw-   0        0        0     1212 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/example/controllers/example_one.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/example/languages/
--rw-rw-rw-   0        0        0      622 2023-07-13 20:19:29.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/en.ini
--rw-rw-rw-   0        0        0      142 2023-07-10 11:18:47.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/en.menus.ini
--rw-rw-rw-   0        0        0     1280 2023-07-13 19:46:27.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/en.sample.ini
--rw-rw-rw-   0        0        0      669 2023-07-26 14:21:30.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/es.ini
--rw-rw-rw-   0        0        0      142 2023-07-10 11:18:26.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/es.menus.ini
--rw-rw-rw-   0        0        0     1408 2023-07-13 19:46:48.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/es.sample.ini
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/example/models/
--rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.1/pmvcs/setup/example/models/example_one.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/example/views/
--rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.1/pmvcs/setup/example/views/example_one.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.770691 pmvcs-1.0.1/pmvcs/setup/module_unique/
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/module_unique/controllers/
--rw-rw-rw-   0        0        0      852 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/module_unique/controllers/unique.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.770691 pmvcs-1.0.1/pmvcs/setup/modules_base/
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/modules_base/controllers/
--rw-rw-rw-   0        0        0      958 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/modules_base/controllers/controller.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/modules_base/models/
--rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.1/pmvcs/setup/modules_base/models/model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/modules_base/views/
--rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.1/pmvcs/setup/modules_base/views/view.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 22:50:30.000000 pmvcs-1.0.1/pmvcs/tests/__init__.py
--rw-rw-rw-   0        0        0      736 2023-07-24 00:03:55.000000 pmvcs-1.0.1/pmvcs/tests/test_default.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs.egg-info/
--rw-rw-rw-   0        0        0     7460 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3319 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1525 2023-07-26 15:01:55.000000 pmvcs-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-07-25 21:31:09.000000 pmvcs-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 15:09:07.860775 pmvcs-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.113293 pmvcs-1.0.2/
+-rw-rw-rw-   0        0        0      634 2023-07-29 21:28:01.000000 pmvcs-1.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35823 2023-07-10 09:52:19.000000 pmvcs-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      894 2023-07-26 15:02:59.000000 pmvcs-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8299 2023-07-29 21:29:43.113293 pmvcs-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8281 2023-07-29 21:23:20.000000 pmvcs-1.0.2/README.ES.md
+-rw-rw-rw-   0        0        0     7579 2023-07-29 21:23:25.000000 pmvcs-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.371251 pmvcs-1.0.2/examples/
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.449875 pmvcs-1.0.2/examples/codebreaker/
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.449875 pmvcs-1.0.2/examples/codebreaker/app/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.513016 pmvcs-1.0.2/examples/codebreaker/app/controllers/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/controllers/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-07-26 19:42:56.000000 pmvcs-1.0.2/examples/codebreaker/app/controllers/base_controller.py
+-rw-rw-rw-   0        0        0     3192 2023-07-26 19:25:48.000000 pmvcs-1.0.2/examples/codebreaker/app/controllers/codebreaker_easy.py
+-rw-rw-rw-   0        0        0     3296 2023-07-26 19:25:48.000000 pmvcs-1.0.2/examples/codebreaker/app/controllers/codebreaker_hard.py
+-rw-rw-rw-   0        0        0     3215 2023-07-26 19:25:49.000000 pmvcs-1.0.2/examples/codebreaker/app/controllers/codebreaker_normal.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.513016 pmvcs-1.0.2/examples/codebreaker/app/decorators/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.513016 pmvcs-1.0.2/examples/codebreaker/app/helpers/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.513016 pmvcs-1.0.2/examples/codebreaker/app/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/interfaces/base_controller.py
+-rw-rw-rw-   0        0        0      161 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/interfaces/base_model.py
+-rw-rw-rw-   0        0        0      142 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/interfaces/base_view.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.575504 pmvcs-1.0.2/examples/codebreaker/app/models/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/models/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/models/base_model.py
+-rw-rw-rw-   0        0        0     3627 2023-07-26 19:42:04.000000 pmvcs-1.0.2/examples/codebreaker/app/models/codebreaker.py
+-rw-rw-rw-   0        0        0      186 2023-07-26 11:29:34.000000 pmvcs-1.0.2/examples/codebreaker/app/models/codebreaker_easy.py
+-rw-rw-rw-   0        0        0      186 2023-07-26 11:29:45.000000 pmvcs-1.0.2/examples/codebreaker/app/models/codebreaker_hard.py
+-rw-rw-rw-   0        0        0      192 2023-07-26 11:28:50.000000 pmvcs-1.0.2/examples/codebreaker/app/models/codebreaker_normal.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.575504 pmvcs-1.0.2/examples/codebreaker/app/models/entities/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 13:23:51.000000 pmvcs-1.0.2/examples/codebreaker/app/models/errors.py
+-rw-rw-rw-   0        0        0     2563 2023-07-26 19:35:15.000000 pmvcs-1.0.2/examples/codebreaker/app/models/validations.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.575504 pmvcs-1.0.2/examples/codebreaker/app/views/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/views/__init__.py
+-rw-rw-rw-   0        0        0     2263 2023-07-26 19:35:55.000000 pmvcs-1.0.2/examples/codebreaker/app/views/base_view.py
+-rw-rw-rw-   0        0        0      180 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/views/codebreaker_easy.py
+-rw-rw-rw-   0        0        0      180 2023-07-26 11:26:44.000000 pmvcs-1.0.2/examples/codebreaker/app/views/codebreaker_hard.py
+-rw-rw-rw-   0        0        0      186 2023-07-26 11:27:58.000000 pmvcs-1.0.2/examples/codebreaker/app/views/codebreaker_normal.py
+-rw-rw-rw-   0        0        0      169 2023-07-26 11:25:29.000000 pmvcs-1.0.2/examples/codebreaker/app.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.622455 pmvcs-1.0.2/examples/codebreaker/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-25 08:29:17.000000 pmvcs-1.0.2/examples/codebreaker/tests/__init__.py
+-rw-rw-rw-   0        0        0     2337 2023-07-26 19:40:17.000000 pmvcs-1.0.2/examples/codebreaker/tests/test_codebreaker.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.653697 pmvcs-1.0.2/pmvcs/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/__init__.py
+-rw-rw-rw-   0        0        0      134 2023-07-10 10:34:58.000000 pmvcs-1.0.2/pmvcs/__main__.py
+-rw-rw-rw-   0        0        0      129 2023-07-29 20:57:17.000000 pmvcs-1.0.2/pmvcs/__version__.py
+-rw-rw-rw-   0        0        0     1595 2023-07-26 00:50:16.000000 pmvcs-1.0.2/pmvcs/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.653697 pmvcs-1.0.2/pmvcs/core/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.669233 pmvcs-1.0.2/pmvcs/core/controllers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/controllers/__init__.py
+-rw-rw-rw-   0        0        0     3292 2023-07-24 03:47:22.000000 pmvcs-1.0.2/pmvcs/core/controllers/base_controller.py
+-rw-rw-rw-   0        0        0     3271 2023-07-24 03:36:42.000000 pmvcs-1.0.2/pmvcs/core/controllers/menus.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.684853 pmvcs-1.0.2/pmvcs/core/decorators/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/decorators/__init__.py
+-rw-rw-rw-   0        0        0      920 2023-07-26 14:00:32.000000 pmvcs-1.0.2/pmvcs/core/decorators/decorators_views.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.684853 pmvcs-1.0.2/pmvcs/core/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1151 2023-07-29 20:55:30.000000 pmvcs-1.0.2/pmvcs/core/helpers/base_helper.py
+-rw-rw-rw-   0        0        0     1440 2023-07-24 03:16:46.000000 pmvcs-1.0.2/pmvcs/core/helpers/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.716573 pmvcs-1.0.2/pmvcs/core/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      730 2023-07-24 02:56:34.000000 pmvcs-1.0.2/pmvcs/core/interfaces/base_controller.py
+-rw-rw-rw-   0        0        0      197 2023-07-13 14:26:55.000000 pmvcs-1.0.2/pmvcs/core/interfaces/base_helper.py
+-rw-rw-rw-   0        0        0     1746 2023-07-24 03:21:41.000000 pmvcs-1.0.2/pmvcs/core/interfaces/base_model.py
+-rw-rw-rw-   0        0        0     1764 2023-07-24 03:04:12.000000 pmvcs-1.0.2/pmvcs/core/interfaces/base_view.py
+-rw-rw-rw-   0        0        0      941 2023-07-24 02:59:42.000000 pmvcs-1.0.2/pmvcs/core/interfaces/menus.py
+-rw-rw-rw-   0        0        0     2025 2023-07-24 03:05:25.000000 pmvcs-1.0.2/pmvcs/core/interfaces/router.py
+-rw-rw-rw-   0        0        0      933 2023-07-24 00:28:53.000000 pmvcs-1.0.2/pmvcs/core/interfaces/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.747818 pmvcs-1.0.2/pmvcs/core/models/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/models/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:04.000000 pmvcs-1.0.2/pmvcs/core/models/about.py
+-rw-rw-rw-   0        0        0     1977 2023-07-24 03:18:08.000000 pmvcs-1.0.2/pmvcs/core/models/base_model.py
+-rw-rw-rw-   0        0        0      688 2023-07-12 06:21:03.000000 pmvcs-1.0.2/pmvcs/core/models/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.747818 pmvcs-1.0.2/pmvcs/core/models/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/models/entities/__init__.py
+-rw-rw-rw-   0        0        0     2312 2023-07-24 03:44:22.000000 pmvcs-1.0.2/pmvcs/core/models/language.py
+-rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:41.000000 pmvcs-1.0.2/pmvcs/core/models/menus.py
+-rw-rw-rw-   0        0        0     3239 2023-07-24 02:38:28.000000 pmvcs-1.0.2/pmvcs/core/models/parser.py
+-rw-rw-rw-   0        0        0     5082 2023-07-29 20:55:47.000000 pmvcs-1.0.2/pmvcs/core/router.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.826659 pmvcs-1.0.2/pmvcs/core/setup/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.857906 pmvcs-1.0.2/pmvcs/core/setup/languages/
+-rw-rw-rw-   0        0        0     2113 2023-07-23 19:31:08.000000 pmvcs-1.0.2/pmvcs/core/setup/languages/en.setup.ini
+-rw-rw-rw-   0        0        0     2409 2023-07-23 21:29:37.000000 pmvcs-1.0.2/pmvcs/core/setup/languages/es.setup.ini
+-rw-rw-rw-   0        0        0     3251 2023-07-24 03:46:11.000000 pmvcs-1.0.2/pmvcs/core/setup/setup.py
+-rw-rw-rw-   0        0        0     3419 2023-07-24 02:35:12.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_config_file.py
+-rw-rw-rw-   0        0        0      718 2023-07-23 23:48:39.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_defaults.py
+-rw-rw-rw-   0        0        0     1035 2023-07-23 23:59:48.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_example.py
+-rw-rw-rw-   0        0        0     1541 2023-07-23 22:57:42.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_extras.py
+-rw-rw-rw-   0        0        0     4361 2023-07-24 04:48:12.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_files.py
+-rw-rw-rw-   0        0        0     4878 2023-07-24 03:46:58.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_install.py
+-rw-rw-rw-   0        0        0     3128 2023-07-24 04:06:23.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_menus.py
+-rw-rw-rw-   0        0        0     3734 2023-07-24 05:13:48.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_multiple.py
+-rw-rw-rw-   0        0        0      957 2023-07-23 22:57:43.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_parser.py
+-rw-rw-rw-   0        0        0     1952 2023-07-23 23:56:31.000000 pmvcs-1.0.2/pmvcs/core/setup/setup_unique.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.889063 pmvcs-1.0.2/pmvcs/core/views/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/core/views/__init__.py
+-rw-rw-rw-   0        0        0     2813 2023-07-24 03:04:20.000000 pmvcs-1.0.2/pmvcs/core/views/base_view.py
+-rw-rw-rw-   0        0        0     5226 2023-07-24 04:56:15.000000 pmvcs-1.0.2/pmvcs/core/views/sample.py
+-rw-rw-rw-   0        0        0      803 2023-07-24 05:10:48.000000 pmvcs-1.0.2/pmvcs/pmvcs.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.907360 pmvcs-1.0.2/pmvcs/setup/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/__init__.py
+-rw-rw-rw-   0        0        0      169 2023-07-12 07:38:03.000000 pmvcs-1.0.2/pmvcs/setup/app.py
+-rw-rw-rw-   0        0        0      683 2023-07-13 21:01:35.000000 pmvcs-1.0.2/pmvcs/setup/config.ini
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.907360 pmvcs-1.0.2/pmvcs/setup/defaults/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.907360 pmvcs-1.0.2/pmvcs/setup/defaults/controllers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/controllers/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-07-23 22:57:44.000000 pmvcs-1.0.2/pmvcs/setup/defaults/controllers/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.907360 pmvcs-1.0.2/pmvcs/setup/defaults/decorators/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.907360 pmvcs-1.0.2/pmvcs/setup/defaults/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.907360 pmvcs-1.0.2/pmvcs/setup/defaults/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-07-23 23:45:10.000000 pmvcs-1.0.2/pmvcs/setup/defaults/interfaces/base_controller.py
+-rw-rw-rw-   0        0        0      161 2023-07-12 21:12:21.000000 pmvcs-1.0.2/pmvcs/setup/defaults/interfaces/base_model.py
+-rw-rw-rw-   0        0        0      142 2023-07-12 21:10:40.000000 pmvcs-1.0.2/pmvcs/setup/defaults/interfaces/base_view.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.936523 pmvcs-1.0.2/pmvcs/setup/defaults/languages/
+-rw-rw-rw-   0        0        0      547 2023-07-13 20:50:52.000000 pmvcs-1.0.2/pmvcs/setup/defaults/languages/en.about.ini
+-rw-rw-rw-   0        0        0      427 2023-07-13 20:59:38.000000 pmvcs-1.0.2/pmvcs/setup/defaults/languages/en.ini
+-rw-rw-rw-   0        0        0        7 2023-07-23 17:22:52.000000 pmvcs-1.0.2/pmvcs/setup/defaults/languages/en.menus.ini
+-rw-rw-rw-   0        0        0      590 2023-07-13 20:50:43.000000 pmvcs-1.0.2/pmvcs/setup/defaults/languages/es.about.ini
+-rw-rw-rw-   0        0        0      467 2023-07-26 14:23:27.000000 pmvcs-1.0.2/pmvcs/setup/defaults/languages/es.ini
+-rw-rw-rw-   0        0        0        7 2023-07-23 17:22:57.000000 pmvcs-1.0.2/pmvcs/setup/defaults/languages/es.menus.ini
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.952144 pmvcs-1.0.2/pmvcs/setup/defaults/models/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/models/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-12 21:12:40.000000 pmvcs-1.0.2/pmvcs/setup/defaults/models/base_model.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.952144 pmvcs-1.0.2/pmvcs/setup/defaults/models/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.952144 pmvcs-1.0.2/pmvcs/setup/defaults/views/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.2/pmvcs/setup/defaults/views/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-07-12 21:13:12.000000 pmvcs-1.0.2/pmvcs/setup/defaults/views/base_view.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.386873 pmvcs-1.0.2/pmvcs/setup/example/
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.983387 pmvcs-1.0.2/pmvcs/setup/example/controllers/
+-rw-rw-rw-   0        0        0     1462 2023-07-23 22:57:46.000000 pmvcs-1.0.2/pmvcs/setup/example/controllers/base_controller.py
+-rw-rw-rw-   0        0        0     1212 2023-07-23 22:57:46.000000 pmvcs-1.0.2/pmvcs/setup/example/controllers/example_one.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.034746 pmvcs-1.0.2/pmvcs/setup/example/languages/
+-rw-rw-rw-   0        0        0      622 2023-07-13 20:19:29.000000 pmvcs-1.0.2/pmvcs/setup/example/languages/en.ini
+-rw-rw-rw-   0        0        0      142 2023-07-10 11:18:47.000000 pmvcs-1.0.2/pmvcs/setup/example/languages/en.menus.ini
+-rw-rw-rw-   0        0        0     1280 2023-07-13 19:46:27.000000 pmvcs-1.0.2/pmvcs/setup/example/languages/en.sample.ini
+-rw-rw-rw-   0        0        0      669 2023-07-26 14:21:30.000000 pmvcs-1.0.2/pmvcs/setup/example/languages/es.ini
+-rw-rw-rw-   0        0        0      142 2023-07-10 11:18:26.000000 pmvcs-1.0.2/pmvcs/setup/example/languages/es.menus.ini
+-rw-rw-rw-   0        0        0     1408 2023-07-13 19:46:48.000000 pmvcs-1.0.2/pmvcs/setup/example/languages/es.sample.ini
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.034746 pmvcs-1.0.2/pmvcs/setup/example/models/
+-rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.2/pmvcs/setup/example/models/example_one.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.034746 pmvcs-1.0.2/pmvcs/setup/example/views/
+-rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.2/pmvcs/setup/example/views/example_one.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.386873 pmvcs-1.0.2/pmvcs/setup/module_unique/
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.081610 pmvcs-1.0.2/pmvcs/setup/module_unique/controllers/
+-rw-rw-rw-   0        0        0      852 2023-07-23 22:57:46.000000 pmvcs-1.0.2/pmvcs/setup/module_unique/controllers/unique.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.386873 pmvcs-1.0.2/pmvcs/setup/modules_base/
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.097271 pmvcs-1.0.2/pmvcs/setup/modules_base/controllers/
+-rw-rw-rw-   0        0        0      958 2023-07-23 22:57:46.000000 pmvcs-1.0.2/pmvcs/setup/modules_base/controllers/controller.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.097271 pmvcs-1.0.2/pmvcs/setup/modules_base/models/
+-rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.2/pmvcs/setup/modules_base/models/model.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.097271 pmvcs-1.0.2/pmvcs/setup/modules_base/views/
+-rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.2/pmvcs/setup/modules_base/views/view.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:43.113293 pmvcs-1.0.2/pmvcs/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 22:50:30.000000 pmvcs-1.0.2/pmvcs/tests/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-07-24 00:03:55.000000 pmvcs-1.0.2/pmvcs/tests/test_default.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:29:42.653697 pmvcs-1.0.2/pmvcs.egg-info/
+-rw-rw-rw-   0        0        0     8299 2023-07-29 21:29:42.000000 pmvcs-1.0.2/pmvcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4722 2023-07-29 21:29:42.000000 pmvcs-1.0.2/pmvcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 21:29:42.000000 pmvcs-1.0.2/pmvcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-29 21:29:42.000000 pmvcs-1.0.2/pmvcs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 21:29:42.000000 pmvcs-1.0.2/pmvcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1525 2023-07-29 20:57:05.000000 pmvcs-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-25 21:31:09.000000 pmvcs-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 21:29:43.113293 pmvcs-1.0.2/setup.cfg
```

### Comparing `pmvcs-1.0.1/CHANGELOG.md` & `pmvcs-1.0.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 ^ -> Change
 - -> Removed
 ! -> Note
 ```
 
 
 ```
-1.0.2-dev ---> 	None yet.
-
+1.0.2 ---> 	+ Added kwargs to by pass variables into the helpers
+```
+```
 1.0.1 ---> 	^ Modified core decorators' views to by pass args and kwargs
 			# Translated one spanish constant in es.ini (ERROR: Unknown format)
 			+ Added how to use configuration/language/view functions in documentation.
 			+ Added changelog in markdown format.
 ```
-
 ```
 1.0.0 ---> 	Initial release
 ```
```

### Comparing `pmvcs-1.0.1/LICENSE` & `pmvcs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/MANIFEST.in` & `pmvcs-1.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/PKG-INFO` & `pmvcs-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pmvcs
-Version: 1.0.1
-Summary: Python MVC Shell Framework Package is a tiny framework for shell projects in Python.
-Author-email: Gonzalo Mahserdjian <gsmx64@outlook.com>
-License: GNU/GPL version 3
-Project-URL: Homepage, https://github.com/gsmx64/pmvcs
-Project-URL: Bug Tracker, https://github.com/gsmx64/pmvcs/issues
-Keywords: pmvcs,python shell,python mvc,python shell framework,python mvc,python mvc shell framework
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python MVC Shell Framework Package
 
 ## About the package
 
 Python MVC Shell Framework Package (PMVCS) is a tiny framework for shell projects making in Python.
 
 ![PMVCS intro language selection](/docs/images/pmvcs-intro-language.png)
@@ -185,14 +169,49 @@
         """
         Returns a float or int value
         """
         pass
 ```
 
 
+### Custom Helpers: Pass variables:
+
+In __init__ it should have:
+
+```
+def __init__(self, **kwargs) -> None:
+	self.pmvcs_helper = kwargs['pmvcs_helper']
+	self.kwargs = { 'pmvcs_cfg': kwargs['pmvcs_cfg'],
+					'pmvcs_lang': kwargs['pmvcs_lang'],
+					'pmvcs_helper': kwargs['pmvcs_helper']}
+						
+```
+
+And in the function that calls the helper:
+
+```
+def to_string_table(self, data: dict) -> str:
+	kwargs2 = { 'data': data,
+				'file_name': 'temp_file'}
+	kwargs2.update(self.kwargs)
+	table_helper = self.pmvcs_helper.load_helper('table', **kwargs2)
+	table_helper.record_file()
+```
+
+Finally in the helper we retrieve the values as:
+
+```
+def __init__(self, **kwargs) -> None:
+	super().__init__(**kwargs)
+	
+	self._data = kwargs['data']
+	self._file_name = f"{kwargs['file_name']}.{self._file_extension}"
+```
+
+
 ### Get configuration constants from config.ini:
 
 Get a configuration constant in string type from "OPTIONS":
 ```
 Code: >>> self.cfg.get("EXAMPLE_CONSTANT", "OPTIONS")
 Returns: This is an example value from config file
 Value Type: <class 'str'>
```

### Comparing `pmvcs-1.0.1/README.ES.md` & `pmvcs-1.0.2/README.ES.md`

 * *Files 14% similar despite different names*

```diff
@@ -169,14 +169,49 @@
         """
         Returns a float or int value
         """
         pass
 ```
 
 
+### Ayudantes Personalizados: Pasar variables:
+
+En el __init__ debería tener:
+
+```
+def __init__(self, **kwargs) -> None:
+	self.pmvcs_helper = kwargs['pmvcs_helper']
+	self.kwargs = { 'pmvcs_cfg': kwargs['pmvcs_cfg'],
+					'pmvcs_lang': kwargs['pmvcs_lang'],
+					'pmvcs_helper': kwargs['pmvcs_helper']}
+						
+```
+
+Y en la función que llama al ayudante:
+
+```
+def to_string_table(self, data: dict) -> str:
+	kwargs2 = { 'data': data,
+				'file_name': 'temp_file'}
+	kwargs2.update(self.kwargs)
+	table_helper = self.pmvcs_helper.load_helper('table', **kwargs2)
+	table_helper.record_file()
+```
+
+Finalmente en el ayudante recuperamos los valores como:
+
+```
+def __init__(self, **kwargs) -> None:
+	super().__init__(**kwargs)
+	
+	self._data = kwargs['data']
+	self._file_name = f"{kwargs['file_name']}.{self._file_extension}"
+```
+
+
 ### Obtener constantes de configuration de config.ini:
 
 Obtiene una constante de configuración en tipo cadena desde "OPTIONS":
 ```
 Código: >>> self.cfg.get("EXAMPLE_CONSTANT", "OPTIONS")
 Retorna: This is an example value from config file
 Tipo de Valor: <class 'str'>
```

### Comparing `pmvcs-1.0.1/README.md` & `pmvcs-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pmvcs
+Version: 1.0.2
+Summary: Python MVC Shell Framework Package is a tiny framework for shell projects in Python.
+Author-email: Gonzalo Mahserdjian <gsmx64@outlook.com>
+License: GNU/GPL version 3
+Project-URL: Homepage, https://github.com/gsmx64/pmvcs
+Project-URL: Bug Tracker, https://github.com/gsmx64/pmvcs/issues
+Keywords: pmvcs,python shell,python mvc,python shell framework,python mvc,python mvc shell framework
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Python MVC Shell Framework Package
 
 ## About the package
 
 Python MVC Shell Framework Package (PMVCS) is a tiny framework for shell projects making in Python.
 
 ![PMVCS intro language selection](/docs/images/pmvcs-intro-language.png)
@@ -169,14 +185,49 @@
         """
         Returns a float or int value
         """
         pass
 ```
 
 
+### Custom Helpers: Pass variables:
+
+In __init__ it should have:
+
+```
+def __init__(self, **kwargs) -> None:
+	self.pmvcs_helper = kwargs['pmvcs_helper']
+	self.kwargs = { 'pmvcs_cfg': kwargs['pmvcs_cfg'],
+					'pmvcs_lang': kwargs['pmvcs_lang'],
+					'pmvcs_helper': kwargs['pmvcs_helper']}
+						
+```
+
+And in the function that calls the helper:
+
+```
+def to_string_table(self, data: dict) -> str:
+	kwargs2 = { 'data': data,
+				'file_name': 'temp_file'}
+	kwargs2.update(self.kwargs)
+	table_helper = self.pmvcs_helper.load_helper('table', **kwargs2)
+	table_helper.record_file()
+```
+
+Finally in the helper we retrieve the values as:
+
+```
+def __init__(self, **kwargs) -> None:
+	super().__init__(**kwargs)
+	
+	self._data = kwargs['data']
+	self._file_name = f"{kwargs['file_name']}.{self._file_extension}"
+```
+
+
 ### Get configuration constants from config.ini:
 
 Get a configuration constant in string type from "OPTIONS":
 ```
 Code: >>> self.cfg.get("EXAMPLE_CONSTANT", "OPTIONS")
 Returns: This is an example value from config file
 Value Type: <class 'str'>
```

### Comparing `pmvcs-1.0.1/pmvcs/cli.py` & `pmvcs-1.0.2/pmvcs/cli.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/controllers/base_controller.py` & `pmvcs-1.0.2/pmvcs/core/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/controllers/menus.py` & `pmvcs-1.0.2/pmvcs/core/controllers/menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/decorators/decorators_views.py` & `pmvcs-1.0.2/pmvcs/core/decorators/decorators_views.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/helpers/base_helper.py` & `pmvcs-1.0.2/pmvcs/core/helpers/base_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,24 @@
         self.pmvcs_lang = kwargs['pmvcs_lang']
 
         if self.__class__.__name__ == 'BaseHelper':
             self.pmvcs_router = kwargs['pmvcs_router']
         else:
             kwargs['pmvcs_router'] = None
 
-    def load_helper(self, helper_name: str, is_pmvcs=False) -> object:
+    def load_helper(self, helper_name: str, is_pmvcs=False, **kwargs) -> object:
         """
         Loads a helper
         """
-        kwargs = {'pmvcs_cfg': self.pmvcs_cfg,
+        kwargs2 = {'pmvcs_cfg': self.pmvcs_cfg,
                   'pmvcs_lang': self.pmvcs_lang,
                   'pmvcs_helper': self}
+        kwargs2.update(kwargs)
         return self.pmvcs_router.import_module(
-            helper_name, 'Helper', is_pmvcs, **kwargs)
+            helper_name, 'Helper', is_pmvcs, **kwargs2)
 
     @staticmethod
     def test() -> str:
         """
         Testing function
         """
         return 'Hello from PMVCS Base Helper!'
```

### Comparing `pmvcs-1.0.1/pmvcs/core/helpers/filters.py` & `pmvcs-1.0.2/pmvcs/core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/interfaces/base_controller.py` & `pmvcs-1.0.2/pmvcs/core/interfaces/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/interfaces/base_model.py` & `pmvcs-1.0.2/pmvcs/core/interfaces/base_model.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/interfaces/base_view.py` & `pmvcs-1.0.2/pmvcs/core/interfaces/base_view.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/interfaces/menus.py` & `pmvcs-1.0.2/pmvcs/core/interfaces/menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/interfaces/router.py` & `pmvcs-1.0.2/pmvcs/core/interfaces/router.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/interfaces/sample.py` & `pmvcs-1.0.2/pmvcs/core/interfaces/sample.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/models/about.py` & `pmvcs-1.0.2/pmvcs/core/models/about.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/models/base_model.py` & `pmvcs-1.0.2/pmvcs/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/models/configuration.py` & `pmvcs-1.0.2/pmvcs/core/models/configuration.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/models/language.py` & `pmvcs-1.0.2/pmvcs/core/models/language.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/models/menus.py` & `pmvcs-1.0.2/pmvcs/core/models/menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/models/parser.py` & `pmvcs-1.0.2/pmvcs/core/models/parser.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/router.py` & `pmvcs-1.0.2/pmvcs/core/router.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/languages/en.setup.ini` & `pmvcs-1.0.2/pmvcs/core/setup/languages/en.setup.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/languages/es.setup.ini` & `pmvcs-1.0.2/pmvcs/core/setup/languages/es.setup.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_config_file.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_config_file.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_defaults.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_defaults.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_example.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_example.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_extras.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_extras.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_files.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_files.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_install.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_install.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_menus.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_multiple.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_multiple.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_parser.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_parser.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/setup/setup_unique.py` & `pmvcs-1.0.2/pmvcs/core/setup/setup_unique.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/views/base_view.py` & `pmvcs-1.0.2/pmvcs/core/views/base_view.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/core/views/sample.py` & `pmvcs-1.0.2/pmvcs/core/views/sample.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/pmvcs.py` & `pmvcs-1.0.2/pmvcs/pmvcs.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/config.ini` & `pmvcs-1.0.2/pmvcs/setup/config.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/defaults/controllers/base_controller.py` & `pmvcs-1.0.2/pmvcs/setup/defaults/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.about.ini` & `pmvcs-1.0.2/pmvcs/setup/defaults/languages/en.about.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.about.ini` & `pmvcs-1.0.2/pmvcs/setup/defaults/languages/es.about.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/defaults/models/base_model.py` & `pmvcs-1.0.2/examples/codebreaker/app/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/example/controllers/base_controller.py` & `pmvcs-1.0.2/pmvcs/setup/example/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/example/controllers/example_one.py` & `pmvcs-1.0.2/pmvcs/setup/example/controllers/example_one.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/example/languages/en.ini` & `pmvcs-1.0.2/pmvcs/setup/example/languages/en.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/example/languages/en.sample.ini` & `pmvcs-1.0.2/pmvcs/setup/example/languages/en.sample.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/example/languages/es.ini` & `pmvcs-1.0.2/pmvcs/setup/example/languages/es.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/example/languages/es.sample.ini` & `pmvcs-1.0.2/pmvcs/setup/example/languages/es.sample.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/module_unique/controllers/unique.py` & `pmvcs-1.0.2/pmvcs/setup/module_unique/controllers/unique.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/setup/modules_base/controllers/controller.py` & `pmvcs-1.0.2/pmvcs/setup/modules_base/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs/tests/test_default.py` & `pmvcs-1.0.2/pmvcs/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.1/pmvcs.egg-info/PKG-INFO` & `pmvcs-1.0.2/pmvcs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmvcs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python MVC Shell Framework Package is a tiny framework for shell projects in Python.
 Author-email: Gonzalo Mahserdjian <gsmx64@outlook.com>
 License: GNU/GPL version 3
 Project-URL: Homepage, https://github.com/gsmx64/pmvcs
 Project-URL: Bug Tracker, https://github.com/gsmx64/pmvcs/issues
 Keywords: pmvcs,python shell,python mvc,python shell framework,python mvc,python mvc shell framework
 Classifier: Programming Language :: Python :: 3
@@ -185,14 +185,49 @@
         """
         Returns a float or int value
         """
         pass
 ```
 
 
+### Custom Helpers: Pass variables:
+
+In __init__ it should have:
+
+```
+def __init__(self, **kwargs) -> None:
+	self.pmvcs_helper = kwargs['pmvcs_helper']
+	self.kwargs = { 'pmvcs_cfg': kwargs['pmvcs_cfg'],
+					'pmvcs_lang': kwargs['pmvcs_lang'],
+					'pmvcs_helper': kwargs['pmvcs_helper']}
+						
+```
+
+And in the function that calls the helper:
+
+```
+def to_string_table(self, data: dict) -> str:
+	kwargs2 = { 'data': data,
+				'file_name': 'temp_file'}
+	kwargs2.update(self.kwargs)
+	table_helper = self.pmvcs_helper.load_helper('table', **kwargs2)
+	table_helper.record_file()
+```
+
+Finally in the helper we retrieve the values as:
+
+```
+def __init__(self, **kwargs) -> None:
+	super().__init__(**kwargs)
+	
+	self._data = kwargs['data']
+	self._file_name = f"{kwargs['file_name']}.{self._file_extension}"
+```
+
+
 ### Get configuration constants from config.ini:
 
 Get a configuration constant in string type from "OPTIONS":
 ```
 Code: >>> self.cfg.get("EXAMPLE_CONSTANT", "OPTIONS")
 Returns: This is an example value from config file
 Value Type: <class 'str'>
```

### Comparing `pmvcs-1.0.1/pyproject.toml` & `pmvcs-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmvcs"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 authors = [
   { name="Gonzalo Mahserdjian", email="gsmx64@outlook.com" },
 ]
 description = "Python MVC Shell Framework Package is a tiny framework for shell projects in Python."
 requires-python = ">=3.7"
 license = {text = "GNU/GPL version 3"}
```

