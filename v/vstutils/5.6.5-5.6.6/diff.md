# Comparing `tmp/vstutils-5.6.5.tar.gz` & `tmp/vstutils-5.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.6.5.tar", last modified: Fri Jul 28 22:03:56 2023, max compression
+gzip compressed data, was "vstutils-5.6.6.tar", last modified: Fri Jul 28 22:39:13 2023, max compression
```

## Comparing `vstutils-5.6.5.tar` & `vstutils-5.6.6.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.560984 vstutils-5.6.5/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.6.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.6.5/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.6.5/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4427 2023-07-28 22:03:56.560984 vstutils-5.6.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.6.5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-30 04:31:13.000000 vstutils-5.6.5/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.6.5/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.6.5/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-30 04:31:13.000000 vstutils-5.6.5/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 04:31:13.000000 vstutils-5.6.5/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 03:44:06.000000 vstutils-5.6.5/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.6.5/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-20 19:01:25.000000 vstutils-5.6.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-28 22:03:56.560984 vstutils-5.6.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.496984 vstutils-5.6.5/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-28 21:53:56.000000 vstutils-5.6.5/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.504984 vstutils-5.6.5/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.6.5/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.6.5/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-17 22:32:27.000000 vstutils-5.6.5/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.6.5/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    29456 2023-07-20 20:14:05.000000 vstutils-5.6.5/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.6.5/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.6.5/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.6.5/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.6.5/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    13849 2023-07-20 08:09:36.000000 vstutils-5.6.5/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.6.5/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:54.000000 vstutils-5.6.5/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.508984 vstutils-5.6.5/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.6.5/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-14 07:52:42.000000 vstutils-5.6.5/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.6.5/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.508984 vstutils-5.6.5/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-08 04:27:47.000000 vstutils-5.6.5/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    24783 2023-07-20 19:01:25.000000 vstutils-5.6.5/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-20 19:01:25.000000 vstutils-5.6.5/vstutils/api/schema/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)    11717 2023-07-20 19:01:25.000000 vstutils-5.6.5/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.6.5/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.6.5/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:54.000000 vstutils-5.6.5/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3554 2023-06-30 04:31:13.000000 vstutils-5.6.5/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-06-28 03:44:06.000000 vstutils-5.6.5/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-07-20 20:14:05.000000 vstutils-5.6.5/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.480984 vstutils-5.6.5/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.508984 vstutils-5.6.5/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.512984 vstutils-5.6.5/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.6.5/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.512984 vstutils-5.6.5/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.6.5/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.512984 vstutils-5.6.5/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.516984 vstutils-5.6.5/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.6.5/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     3661 2023-07-08 04:27:47.000000 vstutils-5.6.5/vstutils/management/commands/rpc_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 22:32:27.000000 vstutils-5.6.5/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.6.5/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.6.5/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10594 2023-06-30 04:31:13.000000 vstutils-5.6.5/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.516984 vstutils-5.6.5/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.6.5/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25952 2023-07-14 05:18:37.000000 vstutils-5.6.5/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-07-20 08:09:36.000000 vstutils-5.6.5/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.6.5/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.6.5/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.6.5/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55943 2023-07-28 21:53:56.000000 vstutils-5.6.5/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.6.5/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.484984 vstutils-5.6.5/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.528984 vstutils-5.6.5/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126391 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      170 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1099741 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/505.js
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/505.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38355 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    73740 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536116 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    87131 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355745 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)   113317 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/app_loader.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   317669 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      750 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3621 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   513410 2023-07-28 22:03:55.000000 vstutils-5.6.5/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.528984 vstutils-5.6.5/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.532984 vstutils-5.6.5/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5592 2023-07-20 08:09:36.000000 vstutils-5.6.5/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.532984 vstutils-5.6.5/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.6.5/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.6.5/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.6.5/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.6.5/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.536984 vstutils-5.6.5/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.6.5/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.6.5/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.536984 vstutils-5.6.5/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.536984 vstutils-5.6.5/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.6.5/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.540984 vstutils-5.6.5/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.544984 vstutils-5.6.5/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.548984 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.548984 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.552984 vstutils-5.6.5/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.552984 vstutils-5.6.5/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.6.5/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.556984 vstutils-5.6.5/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.6.5/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.556984 vstutils-5.6.5/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.556984 vstutils-5.6.5/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.556984 vstutils-5.6.5/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.560984 vstutils-5.6.5/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.6.5/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.6.5/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18312 2023-07-08 04:27:47.000000 vstutils-5.6.5/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.560984 vstutils-5.6.5/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16335 2023-07-14 02:01:10.000000 vstutils-5.6.5/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    24130 2023-07-14 02:01:10.000000 vstutils-5.6.5/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    19158 2023-07-14 02:01:10.000000 vstutils-5.6.5/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.6.5/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    47150 2023-07-20 08:09:36.000000 vstutils-5.6.5/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.6.5/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.6.5/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:03:56.496984 vstutils-5.6.5/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4427 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7789 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1835 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 22:03:56.000000 vstutils-5.6.5/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.898118 vstutils-5.6.6/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.6.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.6.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.6.6/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-07-28 22:39:13.898118 vstutils-5.6.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.6.6/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-30 04:31:13.000000 vstutils-5.6.6/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.6.6/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.6.6/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-30 04:31:13.000000 vstutils-5.6.6/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 04:31:13.000000 vstutils-5.6.6/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 03:44:06.000000 vstutils-5.6.6/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.6.6/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-20 19:01:25.000000 vstutils-5.6.6/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-28 22:39:13.902118 vstutils-5.6.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.6.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.842117 vstutils-5.6.6/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-28 22:32:10.000000 vstutils-5.6.6/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.850117 vstutils-5.6.6/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.6.6/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.6.6/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-17 22:32:27.000000 vstutils-5.6.6/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.6.6/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29456 2023-07-20 20:14:05.000000 vstutils-5.6.6/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.6.6/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.6.6/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.6.6/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.6.6/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13849 2023-07-20 08:09:36.000000 vstutils-5.6.6/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.6.6/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:54.000000 vstutils-5.6.6/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.854117 vstutils-5.6.6/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.6.6/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-14 07:52:42.000000 vstutils-5.6.6/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9387 2023-07-28 22:32:10.000000 vstutils-5.6.6/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.6.6/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.854117 vstutils-5.6.6/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-08 04:27:47.000000 vstutils-5.6.6/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    24783 2023-07-20 19:01:25.000000 vstutils-5.6.6/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-20 19:01:25.000000 vstutils-5.6.6/vstutils/api/schema/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)    11717 2023-07-20 19:01:25.000000 vstutils-5.6.6/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.6.6/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.6.6/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:54.000000 vstutils-5.6.6/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3554 2023-06-30 04:31:13.000000 vstutils-5.6.6/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-06-28 03:44:06.000000 vstutils-5.6.6/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-07-20 20:14:05.000000 vstutils-5.6.6/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.830117 vstutils-5.6.6/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.854117 vstutils-5.6.6/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.858117 vstutils-5.6.6/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.6.6/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.858117 vstutils-5.6.6/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.6.6/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.858117 vstutils-5.6.6/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.858117 vstutils-5.6.6/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.6.6/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     3661 2023-07-08 04:27:47.000000 vstutils-5.6.6/vstutils/management/commands/rpc_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 22:32:27.000000 vstutils-5.6.6/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.6.6/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.6.6/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10594 2023-06-30 04:31:13.000000 vstutils-5.6.6/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.862117 vstutils-5.6.6/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.6.6/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25952 2023-07-14 05:18:37.000000 vstutils-5.6.6/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-07-20 08:09:36.000000 vstutils-5.6.6/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.6.6/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.6.6/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.6.6/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55943 2023-07-28 21:53:56.000000 vstutils-5.6.6/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.6.6/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.830117 vstutils-5.6.6/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.870118 vstutils-5.6.6/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126391 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1099741 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/505.js
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/505.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38355 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    73740 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536116 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    87131 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355745 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)   113317 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/app_loader.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   317669 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      750 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   513410 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.874117 vstutils-5.6.6/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.874117 vstutils-5.6.6/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-07-20 08:09:36.000000 vstutils-5.6.6/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.874117 vstutils-5.6.6/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.6.6/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.6.6/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.6.6/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.6.6/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.878117 vstutils-5.6.6/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.6.6/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.6.6/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.878117 vstutils-5.6.6/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.878117 vstutils-5.6.6/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.6.6/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.878117 vstutils-5.6.6/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.886118 vstutils-5.6.6/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.886118 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.886118 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.890118 vstutils-5.6.6/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.890118 vstutils-5.6.6/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.6.6/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.894118 vstutils-5.6.6/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.6.6/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.894118 vstutils-5.6.6/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.894118 vstutils-5.6.6/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.898118 vstutils-5.6.6/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.898118 vstutils-5.6.6/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.6.6/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.6.6/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18312 2023-07-08 04:27:47.000000 vstutils-5.6.6/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.898118 vstutils-5.6.6/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16335 2023-07-14 02:01:10.000000 vstutils-5.6.6/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    24130 2023-07-14 02:01:10.000000 vstutils-5.6.6/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    19158 2023-07-14 02:01:10.000000 vstutils-5.6.6/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.6.6/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47150 2023-07-20 08:09:36.000000 vstutils-5.6.6/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.6.6/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.6.6/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:39:13.842117 vstutils-5.6.6/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7789 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 22:39:13.000000 vstutils-5.6.6/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.6.5/LICENSE` & `vstutils-5.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/MANIFEST.in` & `vstutils-5.6.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/NOTICE` & `vstutils-5.6.6/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/PKG-INFO` & `vstutils-5.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.6.5
+Version: 5.6.6
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.6.5/README.rst` & `vstutils-5.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/setup.cfg` & `vstutils-5.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/setup.py` & `vstutils-5.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/actions.py` & `vstutils-5.6.6/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/admin.py` & `vstutils-5.6.6/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/auth.py` & `vstutils-5.6.6/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/base.py` & `vstutils-5.6.6/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/decorators.py` & `vstutils-5.6.6/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/decorators.pyi` & `vstutils-5.6.6/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/doc_generator.py` & `vstutils-5.6.6/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/endpoint.py` & `vstutils-5.6.6/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/fields.py` & `vstutils-5.6.6/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/filter_backends.py` & `vstutils-5.6.6/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/filters.py` & `vstutils-5.6.6/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/health.py` & `vstutils-5.6.6/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/meta.py` & `vstutils-5.6.6/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/metrics.py` & `vstutils-5.6.6/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/migrations/0001_initial.py` & `vstutils-5.6.6/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.6.6/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.6.6/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.6.6/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.6.6/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.6.6/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/models.py` & `vstutils-5.6.6/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/pagination.py` & `vstutils-5.6.6/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/parsers.py` & `vstutils-5.6.6/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/permissions.py` & `vstutils-5.6.6/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/renderers.py` & `vstutils-5.6.6/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/responses.py` & `vstutils-5.6.6/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/responses.pyi` & `vstutils-5.6.6/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/routers.py` & `vstutils-5.6.6/vstutils/api/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 class _AbstractRouter(routers.DefaultRouter):
 
     def __init__(self, *args, **kwargs):
         self.custom_urls = []
         self.permission_classes = kwargs.pop("perms", None)
         super().__init__(*args, **kwargs)
 
+    def get_method_map(self, viewset, method_map):
+        # TODO: Remove it after 3.15 release with https://github.com/encode/django-rest-framework/pull/9057
+        bound_methods = {}
+        for method, action in method_map.items():
+            if getattr(viewset, action, None) is not None:
+                bound_methods[method] = action
+        return bound_methods
+
     def _get_api_root_dict(self):
         return {
             reg[0]: self.routes[0].name.format(basename=reg[2])
             for reg in self.registry
         }
 
     def _get_custom_lists(self):
```

### Comparing `vstutils-5.6.5/vstutils/api/routers.pyi` & `vstutils-5.6.6/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/schema/generators.py` & `vstutils-5.6.6/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/schema/info.py` & `vstutils-5.6.6/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/schema/inspectors.py` & `vstutils-5.6.6/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/schema/schema.py` & `vstutils-5.6.6/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/serializers.py` & `vstutils-5.6.6/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/throttling.py` & `vstutils-5.6.6/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/validators.py` & `vstutils-5.6.6/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/api/views.py` & `vstutils-5.6.6/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/asgi.py` & `vstutils-5.6.6/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/asgi_worker.py` & `vstutils-5.6.6/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/auth.py` & `vstutils-5.6.6/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/auth.pyi` & `vstutils-5.6.6/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/celery_beat_scheduler.py` & `vstutils-5.6.6/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.6.6/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/environment.py` & `vstutils-5.6.6/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/exceptions.py` & `vstutils-5.6.6/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/gui/context.py` & `vstutils-5.6.6/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/gui/forms.py` & `vstutils-5.6.6/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/gui/pwa_manifest.py` & `vstutils-5.6.6/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/gui/views.py` & `vstutils-5.6.6/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/ldap_utils.py` & `vstutils-5.6.6/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/_base.py` & `vstutils-5.6.6/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/celery_inspect.py` & `vstutils-5.6.6/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/dockerrun.py` & `vstutils-5.6.6/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/newproject.py` & `vstutils-5.6.6/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/rpc_worker.py` & `vstutils-5.6.6/vstutils/management/commands/rpc_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/run_task.py` & `vstutils-5.6.6/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/runrpc.py` & `vstutils-5.6.6/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/runserver.py` & `vstutils-5.6.6/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/management/commands/web.py` & `vstutils-5.6.6/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/middleware.py` & `vstutils-5.6.6/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/__init__.py` & `vstutils-5.6.6/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/base.py` & `vstutils-5.6.6/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/cent_notify.py` & `vstutils-5.6.6/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/custom_model.py` & `vstutils-5.6.6/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/custom_model.pyi` & `vstutils-5.6.6/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/decorators.py` & `vstutils-5.6.6/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/fields.py` & `vstutils-5.6.6/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/models/queryset.py` & `vstutils-5.6.6/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/settings.ini` & `vstutils-5.6.6/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/settings.py` & `vstutils-5.6.6/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/281.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/296.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/345.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/368.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/421.js` & `vstutils-5.6.6/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.6.6/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/505.js` & `vstutils-5.6.6/vstutils/static/bundle/505.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/505.js.LICENSE.txt` & `vstutils-5.6.6/vstutils/static/bundle/505.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/618.js` & `vstutils-5.6.6/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/683.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/686.js` & `vstutils-5.6.6/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/742.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.6.6/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/755.js` & `vstutils-5.6.6/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/826.chunk.js` & `vstutils-5.6.6/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.6.6/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/844.js` & `vstutils-5.6.6/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/app_loader.js` & `vstutils-5.6.6/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/base.js` & `vstutils-5.6.6/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.6.6/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.6.6/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/output.json` & `vstutils-5.6.6/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/spa.js` & `vstutils-5.6.6/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/bundle/vstutils.js` & `vstutils-5.6.6/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static/img/anonymous.png` & `vstutils-5.6.6/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/static_files.py` & `vstutils-5.6.6/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/tasks.py` & `vstutils-5.6.6/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/auth/base.html` & `vstutils-5.6.6/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/auth/language_selector.html` & `vstutils-5.6.6/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/auth/tfa.html` & `vstutils-5.6.6/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/base.html` & `vstutils-5.6.6/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/gui/base.html` & `vstutils-5.6.6/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/gui/offline.html` & `vstutils-5.6.6/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/gui/service-worker.js` & `vstutils-5.6.6/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.6.6/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.6.6/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/package.json.template` & `vstutils-5.6.6/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.6.6/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.6.6/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/setup.py.template` & `vstutils-5.6.6/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/test.py.template` & `vstutils-5.6.6/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.6.6/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.6.6/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.6.6/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/registration/confirm_email.html` & `vstutils-5.6.6/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.6.6/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.6.6/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/registration/user_registration.html` & `vstutils-5.6.6/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/rest_framework/admin.html` & `vstutils-5.6.6/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.6.6/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.6.6/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templatetags/request_static.py` & `vstutils-5.6.6/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templatetags/translation.py` & `vstutils-5.6.6/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.6.6/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.6.6/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/templatetags/vstconfigs.py` & `vstutils-5.6.6/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/tests.py` & `vstutils-5.6.6/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/tools.py` & `vstutils-5.6.6/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/translations/cn.py` & `vstutils-5.6.6/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/translations/ru.py` & `vstutils-5.6.6/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/translations/vi.py` & `vstutils-5.6.6/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/urls.py` & `vstutils-5.6.6/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/utils.py` & `vstutils-5.6.6/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/web.ini` & `vstutils-5.6.6/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils/wsgi.py` & `vstutils-5.6.6/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils.egg-info/PKG-INFO` & `vstutils-5.6.6/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.6.5
+Version: 5.6.6
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.6.5/vstutils.egg-info/SOURCES.txt` & `vstutils-5.6.6/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.6.5/vstutils.egg-info/requires.txt` & `vstutils-5.6.6/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

