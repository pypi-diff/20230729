# Comparing `tmp/django-import-export-celery-1.5.tar.gz` & `tmp/django-import-export-celery-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-import-export-celery-1.5.tar", last modified: Thu May 25 13:59:34 2023, max compression
+gzip compressed data, was "django-import-export-celery-1.6.tar", last modified: Sat Jul 29 10:17:31 2023, max compression
```

## Comparing `django-import-export-celery-1.5.tar` & `django-import-export-celery-1.6.tar`

### file list

```diff
@@ -1,35 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:34.374446 django-import-export-celery-1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-05-25 13:59:34.374446 django-import-export-celery-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:34.370446 django-import-export-celery-1.5/django_import_export_celery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-05-25 13:59:34.000000 django-import-export-celery-1.5/django_import_export_celery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-25 13:59:34.000000 django-import-export-celery-1.5/django_import_export_celery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:59:34.000000 django-import-export-celery-1.5/django_import_export_celery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:59:34.000000 django-import-export-celery-1.5/django_import_export_celery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 13:59:34.000000 django-import-export-celery-1.5/django_import_export_celery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 13:59:34.000000 django-import-export-celery-1.5/django_import_export_celery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:34.370446 django-import-export-celery-1.5/import_export_celery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/admin_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:34.374446 django-import-export-celery-1.5/import_export_celery/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0002_auto_20190923_1132.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0003_exportjob.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0004_exportjob_email_on_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0005_exportjob_site_of_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0006_auto_20191125_1236.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0007_auto_20210210_1831.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:59:34.374446 django-import-export-celery-1.5/import_export_celery/models/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/models/exportjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/models/importjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/import_export_celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-25 13:59:34.374446 django-import-export-celery-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 13:59:22.000000 django-import-export-celery-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/django_import_export_celery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:17:31.000000 django-import-export-celery-1.6/django_import_export_celery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/admin_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/locale/pt/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/import_export_celery/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0002_auto_20190923_1132.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0003_exportjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0004_exportjob_email_on_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0005_exportjob_site_of_origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0006_auto_20191125_1236.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0007_auto_20210210_1831.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/import_export_celery/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/models/exportjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/models/importjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.579264 django-import-export-celery-1.6/import_export_celery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/import_export_celery/templates/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/templates/email/export_job_completion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/import_export_celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-29 10:17:31.583263 django-import-export-celery-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-29 10:17:21.000000 django-import-export-celery-1.6/setup.py
```

### Comparing `django-import-export-celery-1.5/LICENSE` & `django-import-export-celery-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/PKG-INFO` & `django-import-export-celery-1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export-celery
-Version: 1.5
+Version: 1.6
 Summary: Process long running django imports and exports in celery
 Home-page: https://github.com/auto-mat/django-import-export-celery
 Download-URL: http://pypi.python.org/pypi/django-import-export-celery/
 Author: Timothy Hobbs
 Author-email: timothy.hobbs@auto-mat.cz
 License: License :: OSI Approved :: GNU Lesser General Public License v3.0 or later (LGPLv3.0+)
 Classifier: Topic :: Utilities
@@ -175,14 +175,33 @@
 4. Save the model
 
 5. You will receive an email when the export is done, click on the link in the email
 
 6. Click on the link near the bottom of the page titled `Exported file`.
 
 
+Excluding export file formats in the admin site
+-----------------------------------------------
+
+All available file formats to export are taken from the `Tablib project <https://pypi.org/project/tablib/>`__.
+
+To exclude or disable file formats from the admin site, configure `IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS` django settings variable. This variable is a list of format strings written in lower case.
+
+    ::
+
+        IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS = ["csv", "xls"]
+
+Customizing File Storage Backend
+--------------------------------
+
+Define a custom storage backend by adding the `IMPORT_EXPORT_CELERY_STORAGE` to your Django settings. For instance:
+
+    ::
+
+        IMPORT_EXPORT_CELERY_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
 
 Customizing email template for export job completion email
 ----------------------------------------------------------
 
 By default this is the subject and template used to send the email
 
 
@@ -203,15 +222,15 @@
         EXPORT_JOB_COMPLETION_MAIL_TEMPLATE="path_to_folder/your_custom_template.html"
 
 
 The email template will get some context variables that you can use to customize your template.
 
 
     ::
-        
+
         {
             export_job: The current instance of ExportJob model
             app_label: export_job.app_label
             model: export_job.model
             link: A link to go to the export_job instance on django admin
         }
 
@@ -221,16 +240,16 @@
 
 You can enter a preconfigured dev environment by first running `make` and then launching `./develop.sh` to get into a docker compose environment packed with **redis**, **celery**, **postgres** and everything you need to run and test django-import-export-celery.
 
 Before submitting a PR please run `flake8` and (in the examples directory) `python3 manange.py test`.
 
 Please note, that you need to restart celery for changes to propogate to the workers. Do this with `docker-compose down celery`, `docker-compose up celery`.
 
-Comercial support
------------------
+Commercial support
+------------------
 
-Comercial support is provided by `gradesta s.r.o <https://gradesta.com/support/>`_.
+Commercial support is provided by `gradesta s.r.o <https://gradesta.com/support/>`_.
 
 Credits
 -------
 
 `django-import-export-celery` was developed by the Czech non-profit `auto*mat z.s. <https://auto-mat.cz>`_.
```

### Comparing `django-import-export-celery-1.5/README.rst` & `django-import-export-celery-1.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -154,14 +154,33 @@
 4. Save the model
 
 5. You will receive an email when the export is done, click on the link in the email
 
 6. Click on the link near the bottom of the page titled `Exported file`.
 
 
+Excluding export file formats in the admin site
+-----------------------------------------------
+
+All available file formats to export are taken from the `Tablib project <https://pypi.org/project/tablib/>`__.
+
+To exclude or disable file formats from the admin site, configure `IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS` django settings variable. This variable is a list of format strings written in lower case.
+
+    ::
+
+        IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS = ["csv", "xls"]
+
+Customizing File Storage Backend
+--------------------------------
+
+Define a custom storage backend by adding the `IMPORT_EXPORT_CELERY_STORAGE` to your Django settings. For instance:
+
+    ::
+
+        IMPORT_EXPORT_CELERY_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
 
 Customizing email template for export job completion email
 ----------------------------------------------------------
 
 By default this is the subject and template used to send the email
 
 
@@ -182,15 +201,15 @@
         EXPORT_JOB_COMPLETION_MAIL_TEMPLATE="path_to_folder/your_custom_template.html"
 
 
 The email template will get some context variables that you can use to customize your template.
 
 
     ::
-        
+
         {
             export_job: The current instance of ExportJob model
             app_label: export_job.app_label
             model: export_job.model
             link: A link to go to the export_job instance on django admin
         }
 
@@ -200,16 +219,16 @@
 
 You can enter a preconfigured dev environment by first running `make` and then launching `./develop.sh` to get into a docker compose environment packed with **redis**, **celery**, **postgres** and everything you need to run and test django-import-export-celery.
 
 Before submitting a PR please run `flake8` and (in the examples directory) `python3 manange.py test`.
 
 Please note, that you need to restart celery for changes to propogate to the workers. Do this with `docker-compose down celery`, `docker-compose up celery`.
 
-Comercial support
------------------
+Commercial support
+------------------
 
-Comercial support is provided by `gradesta s.r.o <https://gradesta.com/support/>`_.
+Commercial support is provided by `gradesta s.r.o <https://gradesta.com/support/>`_.
 
 Credits
 -------
 
 `django-import-export-celery` was developed by the Czech non-profit `auto*mat z.s. <https://auto-mat.cz>`_.
```

### Comparing `django-import-export-celery-1.5/django_import_export_celery.egg-info/PKG-INFO` & `django-import-export-celery-1.6/django_import_export_celery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export-celery
-Version: 1.5
+Version: 1.6
 Summary: Process long running django imports and exports in celery
 Home-page: https://github.com/auto-mat/django-import-export-celery
 Download-URL: http://pypi.python.org/pypi/django-import-export-celery/
 Author: Timothy Hobbs
 Author-email: timothy.hobbs@auto-mat.cz
 License: License :: OSI Approved :: GNU Lesser General Public License v3.0 or later (LGPLv3.0+)
 Classifier: Topic :: Utilities
@@ -175,14 +175,33 @@
 4. Save the model
 
 5. You will receive an email when the export is done, click on the link in the email
 
 6. Click on the link near the bottom of the page titled `Exported file`.
 
 
+Excluding export file formats in the admin site
+-----------------------------------------------
+
+All available file formats to export are taken from the `Tablib project <https://pypi.org/project/tablib/>`__.
+
+To exclude or disable file formats from the admin site, configure `IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS` django settings variable. This variable is a list of format strings written in lower case.
+
+    ::
+
+        IMPORT_EXPORT_CELERY_EXCLUDED_FORMATS = ["csv", "xls"]
+
+Customizing File Storage Backend
+--------------------------------
+
+Define a custom storage backend by adding the `IMPORT_EXPORT_CELERY_STORAGE` to your Django settings. For instance:
+
+    ::
+
+        IMPORT_EXPORT_CELERY_STORAGE = "storages.backends.s3boto3.S3Boto3Storage"
 
 Customizing email template for export job completion email
 ----------------------------------------------------------
 
 By default this is the subject and template used to send the email
 
 
@@ -203,15 +222,15 @@
         EXPORT_JOB_COMPLETION_MAIL_TEMPLATE="path_to_folder/your_custom_template.html"
 
 
 The email template will get some context variables that you can use to customize your template.
 
 
     ::
-        
+
         {
             export_job: The current instance of ExportJob model
             app_label: export_job.app_label
             model: export_job.model
             link: A link to go to the export_job instance on django admin
         }
 
@@ -221,16 +240,16 @@
 
 You can enter a preconfigured dev environment by first running `make` and then launching `./develop.sh` to get into a docker compose environment packed with **redis**, **celery**, **postgres** and everything you need to run and test django-import-export-celery.
 
 Before submitting a PR please run `flake8` and (in the examples directory) `python3 manange.py test`.
 
 Please note, that you need to restart celery for changes to propogate to the workers. Do this with `docker-compose down celery`, `docker-compose up celery`.
 
-Comercial support
------------------
+Commercial support
+------------------
 
-Comercial support is provided by `gradesta s.r.o <https://gradesta.com/support/>`_.
+Commercial support is provided by `gradesta s.r.o <https://gradesta.com/support/>`_.
 
 Credits
 -------
 
 `django-import-export-celery` was developed by the Czech non-profit `auto*mat z.s. <https://auto-mat.cz>`_.
```

### Comparing `django-import-export-celery-1.5/django_import_export_celery.egg-info/SOURCES.txt` & `django-import-export-celery-1.6/django_import_export_celery.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 LICENSE
+MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 django_import_export_celery.egg-info/PKG-INFO
 django_import_export_celery.egg-info/SOURCES.txt
 django_import_export_celery.egg-info/dependency_links.txt
 django_import_export_celery.egg-info/not-zip-safe
 django_import_export_celery.egg-info/requires.txt
 django_import_export_celery.egg-info/top_level.txt
 import_export_celery/__init__.py
 import_export_celery/admin.py
 import_export_celery/admin_actions.py
 import_export_celery/apps.py
+import_export_celery/fields.py
 import_export_celery/model_config.py
 import_export_celery/tasks.py
 import_export_celery/utils.py
+import_export_celery/locale/pt/LC_MESSAGES/django.mo
 import_export_celery/migrations/0001_initial.py
 import_export_celery/migrations/0002_auto_20190923_1132.py
 import_export_celery/migrations/0003_exportjob.py
 import_export_celery/migrations/0004_exportjob_email_on_completion.py
 import_export_celery/migrations/0005_exportjob_site_of_origin.py
 import_export_celery/migrations/0006_auto_20191125_1236.py
 import_export_celery/migrations/0007_auto_20210210_1831.py
 import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py
+import_export_celery/migrations/0009_alter_exportjob_options_alter_importjob_options_and_more.py
 import_export_celery/migrations/__init__.py
 import_export_celery/models/__init__.py
 import_export_celery/models/exportjob.py
-import_export_celery/models/importjob.py
+import_export_celery/models/importjob.py
+import_export_celery/templates/email/export_job_completion.html
```

### Comparing `django-import-export-celery-1.5/import_export_celery/admin.py` & `django-import-export-celery-1.6/import_export_celery/admin.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/admin_actions.py` & `django-import-export-celery-1.6/import_export_celery/admin_actions.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/migrations/0001_initial.py` & `django-import-export-celery-1.6/import_export_celery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/migrations/0003_exportjob.py` & `django-import-export-celery-1.6/import_export_celery/migrations/0003_exportjob.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/migrations/0004_exportjob_email_on_completion.py` & `django-import-export-celery-1.6/import_export_celery/migrations/0004_exportjob_email_on_completion.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/migrations/0006_auto_20191125_1236.py` & `django-import-export-celery-1.6/import_export_celery/migrations/0006_auto_20191125_1236.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/migrations/0007_auto_20210210_1831.py` & `django-import-export-celery-1.6/import_export_celery/migrations/0007_auto_20210210_1831.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py` & `django-import-export-celery-1.6/import_export_celery/migrations/0008_alter_exportjob_id_alter_importjob_id.py`

 * *Files identical despite different names*

### Comparing `django-import-export-celery-1.5/import_export_celery/models/exportjob.py` & `django-import-export-celery-1.6/import_export_celery/models/exportjob.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from django.db import models
 from django.db import transaction
 from django.dispatch import receiver
 
 from django.db.models.signals import post_save
 from django.utils.translation import gettext_lazy as _
 
-from import_export.formats.base_formats import DEFAULT_FORMATS
-
+from ..fields import ImportExportFileField
 from ..tasks import run_export_job
+from ..utils import get_formats
 
 
 @with_author
 class ExportJob(models.Model):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._content_type = None
 
-    file = models.FileField(
+    file = ImportExportFileField(
         verbose_name=_("exported file"),
         upload_to="django-import-export-celery-export-jobs",
         blank=False,
         null=False,
         max_length=255,
     )
 
@@ -123,15 +123,15 @@
         ]
 
     @staticmethod
     def get_format_choices():
         """returns choices of available export formats"""
         return [
             (f.CONTENT_TYPE, f().get_title())
-            for f in DEFAULT_FORMATS
+            for f in get_formats()
             if f().can_export()
         ]
 
 
 @receiver(post_save, sender=ExportJob)
 def exportjob_post_save(sender, instance, **kwargs):
     if instance.resource and not instance.processing_initiated:
```

### Comparing `django-import-export-celery-1.5/import_export_celery/models/importjob.py` & `django-import-export-celery-1.6/import_export_celery/models/importjob.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from django.dispatch import receiver
 
 from django.db.models.signals import post_save
 from django.utils.translation import gettext_lazy as _
 
 from import_export.formats.base_formats import DEFAULT_FORMATS
 
+from ..fields import ImportExportFileField
 from ..tasks import run_import_job
 
 
 @with_author
 class ImportJob(models.Model):
-    file = models.FileField(
+    file = ImportExportFileField(
         verbose_name=_("File to be imported"),
         upload_to="django-import-export-celery-import-jobs",
         blank=False,
         null=False,
         max_length=255,
     )
 
@@ -41,15 +42,15 @@
     )
 
     format = models.CharField(
         verbose_name=_("Format of file to be imported"),
         max_length=255,
     )
 
-    change_summary = models.FileField(
+    change_summary = ImportExportFileField(
         verbose_name=_("Summary of changes made by this import"),
         upload_to="django-import-export-celery-import-change-summaries",
         blank=True,
         null=True,
     )
 
     errors = models.TextField(
```

### Comparing `django-import-export-celery-1.5/import_export_celery/tasks.py` & `django-import-export-celery-1.6/import_export_celery/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from django.conf import settings
 from django.core.files.base import ContentFile
 from django.core.cache import cache
 
 from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 
-from import_export.formats.base_formats import DEFAULT_FORMATS
-
 from . import models
 from .model_config import ModelConfig
-from .utils import send_export_job_completion_mail
+from .utils import send_export_job_completion_mail, get_formats
 
 from celery.utils.log import get_task_logger
 import logging
 
 logger = logging.getLogger(__name__)
 
 log = get_task_logger(__name__)
@@ -35,15 +33,15 @@
         job_status = job_status
     cache.set(direction + "_job_status_%s" % job.pk, job_status)
     job.job_status = job_status
     job.save()
 
 
 def get_format(job):
-    for format in DEFAULT_FORMATS:
+    for format in get_formats():
         if job.format == format.CONTENT_TYPE:
             return format()
             break
 
 
 def _run_import_job(import_job, dry_run=True):
     change_job_status(import_job, "import", "1/5 Import started", dry_run)
@@ -54,26 +52,30 @@
     # Copied from https://github.com/django-import-export/django-import-export/blob/3c082f98afe7996e79f936418fced3094f141c26/import_export/admin.py#L260 sorry  # noqa
     try:
         data = import_job.file.read()
         if not import_format.is_binary():
             data = force_str(data, "utf8")
         dataset = import_format.create_dataset(data)
     except UnicodeDecodeError as e:
-        import_job.errors += _("Imported file has a wrong encoding: %s" % e) + "\n"
+        import_job.errors += (
+            _("Imported file has a wrong encoding: %s" % e) + "\n"
+        )
         change_job_status(
             import_job, "import", "Imported file has a wrong encoding", dry_run
         )
         import_job.save()
         return
     except Exception as e:
         import_job.errors += _("Error reading file: %s") % e + "\n"
         change_job_status(import_job, "import", "Error reading file", dry_run)
         import_job.save()
         return
-    change_job_status(import_job, "import", "2/5 Processing import data", dry_run)
+    change_job_status(
+        import_job, "import", "2/5 Processing import data", dry_run
+    )
 
     class Resource(model_config.resource):
         def __init__(self, import_job, *args, **kwargs):
             self.import_job = import_job
             super().__init__(*args, **kwargs)
 
         def before_import_row(self, row, **kwargs):
@@ -89,15 +91,17 @@
             return super().before_import_row(row, **kwargs)
 
     resource = Resource(import_job=import_job)
 
     skip_diff = resource._meta.skip_diff or resource._meta.skip_html_diff
 
     result = resource.import_data(dataset, dry_run=dry_run)
-    change_job_status(import_job, "import", "4/5 Generating import summary", dry_run)
+    change_job_status(
+        import_job, "import", "4/5 Generating import summary", dry_run
+    )
     for error in result.base_errors:
         import_job.errors += f"\n{error.error}\n{error.traceback}\n"
     for line, errors in result.row_errors():
         for error in errors:
             import_job.errors += _("Line: %s - %s\n\t%s\n%s") % (
                 line,
                 error.error,
@@ -107,15 +111,17 @@
 
     if dry_run:
         summary = "<html>"
         summary += "<head>"
         summary += '<meta charset="utf-8">'
         summary += "</head>"
         summary += "<body>"
-        summary += '<table  border="1">'  # TODO refactor the existing template so we can use it for this
+        summary += (  # TODO refactor the existing template so we can use it for this
+            '<table  border="1">'
+        )
         # https://github.com/django-import-export/django-import-export/blob/6575c3e1d89725701e918696fbc531aeb192a6f7/import_export/templates/admin/import_export/import.html
         if not result.invalid_rows and not skip_diff:
             cols = lambda row: "</td><td>".join([field for field in row.diff])
             summary += (
                 "<tr><td>change_type</td><td>"
                 + "</td><td>".join(
                     [f.column_name for f in resource.get_user_visible_fields()]
@@ -129,15 +135,17 @@
                         row.import_type + "</td><td>" + cols(row)
                         for row in result.valid_rows()
                     ]
                 )
                 + "</tr>"
             )
         else:
-            cols = lambda row: "</td><td>".join([str(field) for field in row.values])
+            cols = lambda row: "</td><td>".join(
+                [str(field) for field in row.values]
+            )
             cols_error = lambda row: "".join(
                 [
                     "<mark>"
                     + key
                     + "</mark>"
                     + "<br>"
                     + row.error.message_dict[key][0]
```

### Comparing `django-import-export-celery-1.5/setup.py` & `django-import-export-celery-1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,38 @@
 import datetime
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 requires = ["Django", "django-import-export", "django-author", "html2text"]
 
 try:
-    version = subprocess.check_output(
-        ["git", "describe", "--abbrev=0", "--tags"]
-    ).decode("utf-8").strip()
+    version = (
+        subprocess.check_output(["git", "describe", "--abbrev=0", "--tags"])
+        .decode("utf-8")
+        .strip()
+    )
 except subprocess.CalledProcessError:
     version = "0.dev" + datetime.datetime.now().strftime("%Y%m%d%H%M%S")
 
 setup(
     name="django-import-export-celery",
     version=version,
     author="Timothy Hobbs",
     author_email="timothy.hobbs@auto-mat.cz",
     url="https://github.com/auto-mat/django-import-export-celery",
     download_url="http://pypi.python.org/pypi/django-import-export-celery/",
     description="Process long running django imports and exports in celery",
-    long_description=codecs.open(os.path.join(here, "README.rst"), "r", "utf-8").read(),
+    long_description=codecs.open(
+        os.path.join(here, "README.rst"), "r", "utf-8"
+    ).read(),
     long_description_content_type="text/x-rst",
-    license="License :: OSI Approved :: GNU Lesser General Public License v3.0 or later (LGPLv3.0+)",
+    license=(
+        "License :: OSI Approved :: GNU Lesser General Public License v3.0 or"
+        " later (LGPLv3.0+)"
+    ),
     install_requires=requires,
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Topic :: Utilities",
         "Natural Language :: English",
```

