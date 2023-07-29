# Comparing `tmp/ihatemoney-6.0.1.tar.gz` & `tmp/ihatemoney-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ihatemoney-6.0.1.tar", last modified: Sat Jul 22 18:02:18 2023, max compression
+gzip compressed data, was "ihatemoney-6.1.0.tar", last modified: Sat Jul 29 13:09:02 2023, max compression
```

## Comparing `ihatemoney-6.0.1.tar` & `ihatemoney-6.1.0.tar`

### file list

```diff
@@ -1,319 +1,320 @@
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      945 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/CONTRIBUTORS
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1781 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/LICENSE
--rw-r--r--   0 zorun     (1000) zorun     (1000)      205 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/MANIFEST.in
--rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/PKG-INFO
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2183 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/README.md
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/__init__.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/api/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6122 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/common.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/api/v1/
--rw-r--r--   0 zorun     (1000) zorun     (1000)       53 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/v1/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1115 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/v1/resources.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)       97 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/babel.cfg
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/conf-templates/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      641 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/apache-vhost.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      192 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/gunicorn.conf.py.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2277 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/ihatemoney.cfg.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      752 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/nginx.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      186 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/supervisord.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1844 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/currency_convertor.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      868 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/default_settings.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      544 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/emails.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15859 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/forms.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6041 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/history.py
--rwxr-xr-x   0 zorun     (1000) zorun     (1000)     2406 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/manage.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/migrations/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      790 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/alembic.ini
--rwxr-xr-x   0 zorun     (1000) zorun     (1000)     3014 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/env.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/migrations/versions/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      614 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/26d6a218c329_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8427 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      627 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/6c6fb2b7f229_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2002 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      963 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      625 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1085 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/b9a10d5d63ce_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1629 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      977 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26923 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/models.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3498 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/monkeypath_continuum.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8632 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/run.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/static/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/static/css/
--rw-r--r--   0 zorun     (1000) zorun     (1000)   155758 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/bootstrap.min.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14225 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/datatables.min.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/download_mobile_app.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9387 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/main.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2185 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/tagsinput.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6742 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/favicon.ico
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/static/fonts/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4582 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/OFL.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)    40370 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.eot
--rw-r--r--   0 zorun     (1000) zorun     (1000)    81869 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20920 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.woff
--rw-r--r--   0 zorun     (1000) zorun     (1000)      777 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/fontfaces.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    63744 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.eot
--rw-r--r--   0 zorun     (1000) zorun     (1000)    77893 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    33380 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.woff
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/images/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      155 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/add.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)    12353 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/app-store.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5634 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/bill.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      518 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/book.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      890 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/cog.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/delete.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      143 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/deleter.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      167 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/edit.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6681 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/f-droid.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      557 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/file-alt.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1272 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/file-csv-solid.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      692 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/git.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1458 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/globe.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    69751 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/google-play.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5814 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/indicate.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1304 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/legal.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      356 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/mobile-alt.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      293 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/paper-plane.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      319 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/plus.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      183 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/reactivate.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3505 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/read.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     7325 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/share.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      259 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/show.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      158 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_asc.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      146 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_asc_disabled.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      199 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_both.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      157 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_desc.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_desc_disabled.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      291 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/x.svg
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/js/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    58072 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/bootstrap.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    84649 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/datatables.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)      326 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/ihatemoney.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    89501 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21004 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/popper.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    10060 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/tagsinput.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24989 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/tether.min.js
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/photoswipe/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11607 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)      547 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1554 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      866 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/preloader.gif
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9878 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4137 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31904 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.min.js
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/showcase/
--rw-r--r--   0 zorun     (1000) zorun     (1000)   110452 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/1.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    80684 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/2.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    79206 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/3.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    74018 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/4.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    85550 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/5.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)   116502 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/6.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    91376 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/7.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    93966 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/8.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)   132986 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/9.webp
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/templates/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      508 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/404.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      381 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/add_bill.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      266 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/add_member.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      340 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/admin.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      456 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/authenticate.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      195 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/create_project.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2047 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/dashboard.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      253 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/display_errors.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1274 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/download_mobile_app.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      384 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/edit_member.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3183 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/edit_project.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8800 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/forms.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      819 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/helpers.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14207 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/history.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3242 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/home.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      628 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      663 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9363 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/layout.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8094 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/list_bills.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      308 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      189 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      296 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder_sent.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      240 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/recent_projects.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      458 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/reminder_mail.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      462 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/reminder_mail.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      278 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/reset_password.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2132 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/send_invites.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      649 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/settle_bills.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3333 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/showcase.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/sidebar_table_layout.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1323 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/statistics.html
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/tests/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31635 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/api_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    62720 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/budget_test.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/tests/common/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/common/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      455 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/common/help_functions.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3642 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/common/ihatemoney_testcase.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24612 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/history_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      247 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/ihatemoney.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      243 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/ihatemoney_envvar.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23512 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/import_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15296 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/main_test.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/bn/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3626 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18252 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2105 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19243 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/ca/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20292 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26010 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/cs/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3806 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19876 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/de/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21148 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    27611 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/el/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11152 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26286 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/eo/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14668 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24947 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/es/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8803 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21878 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/es_419/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20099 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    27588 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/fa/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4871 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19283 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/fr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24032 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    34440 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/he/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    13498 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21847 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/hi/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21207 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    35887 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/hu/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6025 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18680 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/id/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18123 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26079 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/it/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14297 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26112 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ja/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14961 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26614 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/kn/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6873 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21364 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ms/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1711 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17896 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    12943 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    30034 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/nl/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    12418 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24311 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/pl/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19768 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    27083 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/pt/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19649 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26437 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19135 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26311 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ru/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24769 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    33304 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/sr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3599 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19114 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/sv/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18537 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25233 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ta/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6917 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24755 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/te/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9177 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24405 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/th/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3702 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19037 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/tr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19795 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    27394 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/uk/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5936 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22133 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ur/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1190 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16608 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/vi/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      411 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16154 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16680 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24563 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14648 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/utils.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3596 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/versioning.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    30734 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/web.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)       66 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/wsgi.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney.egg-info/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/PKG-INFO
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9525 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/SOURCES.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/dependency_links.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)      229 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/entry_points.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/not-zip-safe
--rw-r--r--   0 zorun     (1000) zorun     (1000)      708 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/requires.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)       11 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/top_level.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2038 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/setup.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)       38 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/setup.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      958 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/CONTRIBUTORS
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1781 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/LICENSE
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      211 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/MANIFEST.in
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/PKG-INFO
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2183 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/README.md
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/__init__.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/api/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/api/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6122 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/api/common.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/api/v1/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       53 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/api/v1/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1115 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/api/v1/resources.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       97 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/babel.cfg
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/conf-templates/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      641 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/conf-templates/apache-vhost.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      192 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/conf-templates/gunicorn.conf.py.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2277 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/conf-templates/ihatemoney.cfg.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      752 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/conf-templates/nginx.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      186 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/conf-templates/supervisord.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1844 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/currency_convertor.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      868 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/default_settings.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      544 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/emails.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16484 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/forms.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6041 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/history.py
+-rwxr-xr-x   0 zorun     (1000) zorun     (1000)     2406 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/manage.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/migrations/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      790 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/alembic.ini
+-rwxr-xr-x   0 zorun     (1000) zorun     (1000)     3014 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/env.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/migrations/versions/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      614 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/26d6a218c329_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8427 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      627 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2002 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      963 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      625 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1085 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1629 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      977 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27120 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/models.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3498 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/monkeypath_continuum.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8632 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/run.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/static/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/static/css/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   155758 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/css/bootstrap.min.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14225 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/css/datatables.min.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/css/download_mobile_app.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9387 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/css/main.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2185 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/css/tagsinput.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6742 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/favicon.ico
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.251746 ihatemoney-6.1.0/ihatemoney/static/fonts/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4582 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/OFL.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    40370 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    81869 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20920 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      777 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/fontfaces.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    63744 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/lobster-webfont.eot
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    77893 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/lobster-webfont.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    33380 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/fonts/lobster-webfont.woff
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.255746 ihatemoney-6.1.0/ihatemoney/static/images/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      155 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/add.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12353 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/app-store.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5634 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/bill.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      518 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/book.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      890 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/cog.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/delete.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      143 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/deleter.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      167 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/edit.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6681 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/f-droid.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      557 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/file-alt.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1272 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/file-csv-solid.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      692 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/git.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1458 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/globe.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    69751 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/google-play.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5814 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/indicate.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1304 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/legal.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      356 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/mobile-alt.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      293 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/paper-plane.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      319 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/plus.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      183 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/reactivate.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3505 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/read.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     7325 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/share.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      259 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/show.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      158 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/sort_asc.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      146 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/sort_asc_disabled.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      199 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/sort_both.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      157 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/sort_desc.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/sort_desc_disabled.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      291 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/images/x.svg
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.255746 ihatemoney-6.1.0/ihatemoney/static/js/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    58072 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/bootstrap.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    84649 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/datatables.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      326 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/ihatemoney.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    89501 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21004 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/popper.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    10060 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/tagsinput.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24989 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/js/tether.min.js
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.255746 ihatemoney-6.1.0/ihatemoney/static/photoswipe/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.255746 ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11607 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/default-skin.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      547 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/default-skin.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1554 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      866 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/preloader.gif
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9878 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4137 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/photoswipe.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31904 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/photoswipe/photoswipe.min.js
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.255746 ihatemoney-6.1.0/ihatemoney/static/showcase/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   110452 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/1.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    80684 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/2.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    79206 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/3.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    74018 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/4.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    85550 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/5.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   116502 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/6.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    91376 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/7.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    93966 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/8.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   132986 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/static/showcase/9.webp
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/templates/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      508 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/404.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      381 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/add_bill.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      266 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/add_member.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      340 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/admin.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      456 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/authenticate.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      195 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/create_project.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2047 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/dashboard.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      253 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/display_errors.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1274 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/download_mobile_app.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      384 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/edit_member.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3183 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/edit_project.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8839 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/forms.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      819 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/helpers.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14207 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/history.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3242 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/home.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      628 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/invitation_mail.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      663 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/invitation_mail.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9566 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/layout.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8291 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/list_bills.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/password_reminder.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      308 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/password_reminder.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      189 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/password_reminder.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      296 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/password_reminder_sent.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1257 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/project_feed.xml
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      240 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/recent_projects.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      458 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/reminder_mail.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      462 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/reminder_mail.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      278 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/reset_password.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2734 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/send_invites.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      649 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/settle_bills.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3333 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/showcase.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/sidebar_table_layout.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1323 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/templates/statistics.html
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/tests/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    33522 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/api_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    77899 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/budget_test.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/tests/common/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/common/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      455 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/common/help_functions.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3724 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/common/ihatemoney_testcase.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24834 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/history_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      247 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/ihatemoney.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      243 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/ihatemoney_envvar.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23512 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/import_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    15306 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/tests/main_test.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.243746 ihatemoney-6.1.0/ihatemoney/translations/bn/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/bn/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3626 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/bn/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19963 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/bn/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.243746 ihatemoney-6.1.0/ihatemoney/translations/bn_BD/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2105 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20941 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.243746 ihatemoney-6.1.0/ihatemoney/translations/ca/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20292 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27189 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.243746 ihatemoney-6.1.0/ihatemoney/translations/cs/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3806 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21538 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/de/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21148 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    28759 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/el/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/el/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11152 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    28028 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/eo/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14668 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26107 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/es/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8803 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23540 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/es_419/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20099 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    28782 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/fa/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4871 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20946 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/fr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25571 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    36577 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/he/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/he/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14086 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/he/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23738 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/he/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/hi/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21207 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    37099 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/hu/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6025 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20330 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/id/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/id/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18123 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27261 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/id/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/it/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/it/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14297 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27289 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/ja/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14961 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27778 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/kn/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/kn/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6873 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23040 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/ms/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/ms/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1711 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19551 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/nb_NO/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12943 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31180 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/nl/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12418 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25472 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/pl/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.259746 ihatemoney-6.1.0/ihatemoney/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19768 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    28262 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/pt/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19649 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27624 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/pt_BR/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19135 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27495 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/ru/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24769 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    34538 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/sr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/sr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3599 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20720 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/sv/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18537 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26406 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/ta/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/ta/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6917 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26471 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/te/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/te/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9177 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/te/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26119 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/te/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/th/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/th/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3702 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20643 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/th/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/tr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19795 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    28572 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/uk/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5936 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23818 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/ur/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/ur/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1190 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ur/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18214 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/ur/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/vi/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/vi/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      411 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/vi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17760 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/vi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney/translations/zh_Hans/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16680 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25718 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14648 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/utils.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3596 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/versioning.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    32442 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/web.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       66 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/ihatemoney/wsgi.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-29 13:09:02.247746 ihatemoney-6.1.0/ihatemoney.egg-info/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/PKG-INFO
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9563 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      229 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/entry_points.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/not-zip-safe
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      734 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/requires.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       11 2023-07-29 13:09:02.000000 ihatemoney-6.1.0/ihatemoney.egg-info/top_level.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2065 2023-07-29 13:09:02.263746 ihatemoney-6.1.0/setup.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       38 2023-07-29 13:09:01.000000 ihatemoney-6.1.0/setup.py
```

### Comparing `ihatemoney-6.0.1/CONTRIBUTORS` & `ihatemoney-6.1.0/CONTRIBUTORS`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Carey Metcalfe
 cbrosnan
 Daniel Schreiber
 DavidRThrashJr
 donkers
 Edwin Smulders
 Elizabeth Sherrock
+Éloi Rivard
 eMerzh
 Erwan Lacoudre
 Feth AREZKI
 Frédéric Sureau
 Gianluca De Cola
 Glandos
 Heimen Stoffels
```

### Comparing `ihatemoney-6.0.1/LICENSE` & `ihatemoney-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/PKG-INFO` & `ihatemoney-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihatemoney
-Version: 6.0.1
+Version: 6.1.0
 Summary: A simple shared budget manager web application.
 Home-page: https://github.com/spiral-project/ihatemoney
 Author: Alexis Métaireau & contributors
 Author-email: alexis@notmyidea.org
 License: Custom BSD Beerware
 Description: UNKNOWN
 Keywords: web,budget
```

### Comparing `ihatemoney-6.0.1/README.md` & `ihatemoney-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/api/common.py` & `ihatemoney-6.1.0/ihatemoney/api/common.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/api/v1/resources.py` & `ihatemoney-6.1.0/ihatemoney/api/v1/resources.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/conf-templates/apache-vhost.conf.j2` & `ihatemoney-6.1.0/ihatemoney/conf-templates/apache-vhost.conf.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/conf-templates/ihatemoney.cfg.j2` & `ihatemoney-6.1.0/ihatemoney/conf-templates/ihatemoney.cfg.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/conf-templates/nginx.conf.j2` & `ihatemoney-6.1.0/ihatemoney/conf-templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/currency_convertor.py` & `ihatemoney-6.1.0/ihatemoney/currency_convertor.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/default_settings.py` & `ihatemoney-6.1.0/ihatemoney/default_settings.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/emails.py` & `ihatemoney-6.1.0/ihatemoney/emails.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/forms.py` & `ihatemoney-6.1.0/ihatemoney/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,19 @@
             valuelist[0] = str(eval_arithmetic_expression(value))
 
         return super(CalculatorStringField, self).process_formdata(valuelist)
 
 
 class EditProjectForm(FlaskForm):
     name = StringField(_("Project name"), validators=[DataRequired()])
+    current_password = PasswordField(
+        _("Current private code"),
+        description=_("Enter existing private code to edit project"),
+        validators=[DataRequired()],
+    )
     # If empty -> don't change the password
     password = PasswordField(
         _("New private code"),
         description=_("Enter a new code if you want to change it"),
     )
     contact_email = StringField(_("Email"), validators=[DataRequired(), Email()])
     project_history = BooleanField(_("Enable project history"))
@@ -150,14 +155,21 @@
             self.id = SimpleNamespace(data=kwargs.pop("id", ""))
         super().__init__(*args, **kwargs)
         self.default_currency.choices = [
             (currency_name, render_localized_currency(currency_name, detailed=True))
             for currency_name in self.currency_helper.get_currencies()
         ]
 
+    def validate_current_password(self, field):
+        project = Project.query.get(self.id.data)
+        if project is None:
+            raise ValidationError(_("Unknown error"))
+        if not check_password_hash(project.password, self.current_password.data):
+            raise ValidationError(_("Invalid private code."))
+
     @property
     def logging_preference(self):
         """Get the LoggingMode object corresponding to current form data."""
         if not self.project_history.data:
             return LoggingMode.DISABLED
         else:
             if self.ip_recording.data:
@@ -208,15 +220,17 @@
         ],
         description=_("Compatible with Cospend"),
     )
 
 
 class ProjectForm(EditProjectForm):
     id = StringField(_("Project identifier"), validators=[DataRequired()])
-    # This field overrides the one from EditProjectForm
+    # Remove this field that is inherited from EditProjectForm
+    current_password = None
+    # This field overrides the one from EditProjectForm (to make it mandatory)
     password = PasswordField(_("Private code"), validators=[DataRequired()])
     submit = SubmitField(_("Create the project"))
 
     def save(self):
         """Create a new project with the information given by this form.
 
         Returns the created instance
```

### Comparing `ihatemoney-6.0.1/ihatemoney/history.py` & `ihatemoney-6.1.0/ihatemoney/history.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/manage.py` & `ihatemoney-6.1.0/ihatemoney/manage.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/alembic.ini` & `ihatemoney-6.1.0/ihatemoney/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/env.py` & `ihatemoney-6.1.0/ihatemoney/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/26d6a218c329_.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/26d6a218c329_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/6c6fb2b7f229_.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/b9a10d5d63ce_.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py` & `ihatemoney-6.1.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/models.py` & `ihatemoney-6.1.0/ihatemoney/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,15 +449,16 @@
         purge_history(self)
         db.session.commit()
 
     def generate_token(self, token_type="auth"):
         """Generate a timed and serialized JsonWebToken
 
         :param token_type: Either "auth" for authentication (invalidated when project code changed),
-                        or "reset" for password reset (invalidated after expiration)
+                        or "reset" for password reset (invalidated after expiration),
+                        or "feed" for project feeds (invalidated when project code changed)
         """
 
         if token_type == "reset":
             serializer = URLSafeTimedSerializer(
                 current_app.config["SECRET_KEY"], salt=token_type
             )
             token = serializer.dumps([self.id])
@@ -472,17 +473,18 @@
     @staticmethod
     def verify_token(token, token_type="auth", project_id=None, max_age=3600):
         """Return the project id associated to the provided token,
         None if the provided token is expired or not valid.
 
         :param token: Serialized TimedJsonWebToken
         :param token_type: Either "auth" for authentication (invalidated when project code changed),
-                        or "reset" for password reset (invalidated after expiration)
-        :param project_id: Project ID. Used for token_type "auth" to use the password as serializer
-                        secret key.
+                        or "reset" for password reset (invalidated after expiration),
+                        or "feed" for project feeds (invalidated when project code changed)
+        :param project_id: Project ID. Used for token_type "auth" and "feed" to use the password
+                        as serializer secret key.
         :param max_age: Token expiration time (in seconds). Only used with token_type "reset"
         """
         loads_kwargs = {}
         if token_type == "reset":
             serializer = URLSafeTimedSerializer(
                 current_app.config["SECRET_KEY"], salt=token_type
             )
```

### Comparing `ihatemoney-6.0.1/ihatemoney/monkeypath_continuum.py` & `ihatemoney-6.1.0/ihatemoney/monkeypath_continuum.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/run.py` & `ihatemoney-6.1.0/ihatemoney/run.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/css/bootstrap.min.css` & `ihatemoney-6.1.0/ihatemoney/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/css/datatables.min.css` & `ihatemoney-6.1.0/ihatemoney/static/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/css/main.css` & `ihatemoney-6.1.0/ihatemoney/static/css/main.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/css/tagsinput.css` & `ihatemoney-6.1.0/ihatemoney/static/css/tagsinput.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/favicon.ico` & `ihatemoney-6.1.0/ihatemoney/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/OFL.txt` & `ihatemoney-6.1.0/ihatemoney/static/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.eot` & `ihatemoney-6.1.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.svg` & `ihatemoney-6.1.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.woff` & `ihatemoney-6.1.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/fontfaces.css` & `ihatemoney-6.1.0/ihatemoney/static/fonts/fontfaces.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.eot` & `ihatemoney-6.1.0/ihatemoney/static/fonts/lobster-webfont.eot`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.svg` & `ihatemoney-6.1.0/ihatemoney/static/fonts/lobster-webfont.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.woff` & `ihatemoney-6.1.0/ihatemoney/static/fonts/lobster-webfont.woff`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/app-store.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/app-store.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/bill.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/bill.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/book.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/book.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/cog.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/cog.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/f-droid.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/f-droid.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/file-alt.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/file-alt.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/file-csv-solid.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/file-csv-solid.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/git.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/git.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/globe.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/globe.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/google-play.png` & `ihatemoney-6.1.0/ihatemoney/static/images/google-play.png`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/indicate.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/indicate.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/legal.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/legal.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/read.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/read.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/images/share.svg` & `ihatemoney-6.1.0/ihatemoney/static/images/share.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/js/bootstrap.min.js` & `ihatemoney-6.1.0/ihatemoney/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/js/datatables.min.js` & `ihatemoney-6.1.0/ihatemoney/static/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/js/jquery-3.6.0.min.js` & `ihatemoney-6.1.0/ihatemoney/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/js/popper.min.js` & `ihatemoney-6.1.0/ihatemoney/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/js/tagsinput.js` & `ihatemoney-6.1.0/ihatemoney/static/js/tagsinput.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/js/tether.min.js` & `ihatemoney-6.1.0/ihatemoney/static/js/tether.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.css` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/default-skin.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.png` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/default-skin.png`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.svg` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/preloader.gif` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/default-skin/preloader.gif`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.css` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/photoswipe.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.min.js` & `ihatemoney-6.1.0/ihatemoney/static/photoswipe/photoswipe.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/1.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/1.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/2.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/2.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/3.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/3.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/4.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/4.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/5.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/5.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/6.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/6.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/7.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/7.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/8.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/8.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/static/showcase/9.webp` & `ihatemoney-6.1.0/ihatemoney/static/showcase/9.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/dashboard.html` & `ihatemoney-6.1.0/ihatemoney/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/download_mobile_app.html` & `ihatemoney-6.1.0/ihatemoney/templates/download_mobile_app.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/edit_project.html` & `ihatemoney-6.1.0/ihatemoney/templates/edit_project.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/forms.html` & `ihatemoney-6.1.0/ihatemoney/templates/forms.html`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         <div id="privacy_checkboxes" class="card card-body bg-light">
         {{ checkbox(form.project_history) }}
         {{ checkbox(form.ip_recording) }}
         </div>
     </div>
 
     {{ input(form.default_currency) }}
+    {{ input(form.current_password) }}
     <div class="actions">
         <button class="btn btn-primary">{{ _("Save changes") }}</button>
     </div>
 
 {% endmacro %}
 
 {% macro delete_project(form) %}
```

#### html2text {}

```diff
@@ -26,15 +26,15 @@
 ['ENABLE_CAPTCHA'] %} {{ input(form.captcha) }} {% endif %} {% if not home %} {
 { submit(form.submit, home=True) }} {% endif %} {% endmacro %} {% macro
 edit_project(form) %} {% include "display_errors.html" %} {{ form.hidden_tag()
 }} {{ input(form.name) }} {{ input(form.password) }} {{ input
 (form.contact_email) }}
 {{ _("Privacy Settings") }}
 {{ checkbox(form.project_history) }} {{ checkbox(form.ip_recording) }}
-{{ input(form.default_currency) }}
+{{ input(form.default_currency) }} {{ input(form.current_password) }}
 {{ _("Save changes") }}
 {% endmacro %} {% macro delete_project(form) %} {% include
 "display_errors.html" %}
 {{ _("This will remove all bills and participants in this project!") }}
 {{ form.hidden_tag() }} {{ input(form.password) }}
 {{ _("Delete project") }}
 {% endmacro %} {% macro import_project(form) %} {% include
```

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/helpers.js` & `ihatemoney-6.1.0/ihatemoney/templates/helpers.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/history.html` & `ihatemoney-6.1.0/ihatemoney/templates/history.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/home.html` & `ihatemoney-6.1.0/ihatemoney/templates/home.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.en.j2` & `ihatemoney-6.1.0/ihatemoney/templates/invitation_mail.en.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.fr.j2` & `ihatemoney-6.1.0/ihatemoney/templates/invitation_mail.fr.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/layout.html` & `ihatemoney-6.1.0/ihatemoney/templates/layout.html`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 <i class="icon before-text">{{ static_include("images/plus.svg") | safe }}</i>
                 {{ _("Start a new project") }}
               </a>
             </li>
             {% if g.project %}
             <li><a class="dropdown-item" href="{{ url_for("main.history") }}">{{ _("History") }}</a></li>
             <li><a class="dropdown-item" href="{{ url_for("main.edit_project") }}">{{ _("Settings") }}</a></li>
+            <li><a class="dropdown-item" href="{{ url_for("main.feed", token=g.project.generate_token("feed")) }}">{{ _("RSS Feed") }}</a></li>
             {% endif %}
 
             {% if session['projects'] and not ((session['projects'] | length) == 1 and g.project and g.project.id in session['projects']) %}
             <li class="dropdown-divider"></li>
             <li class="dropdown-header">{{ _('Other projects :') }}</li>
               {% for id, name in session['projects'].items() %}
                 {% if not g.project or id != g.project.id %}
@@ -114,20 +115,22 @@
                 {% endif %}
               {% endfor %}
             {% endif %}
             <li class="dropdown-divider"></li>
             {% if session['is_admin'] %}
             <li><a class="dropdown-item" href="{{ url_for("main.dashboard") }}">{{ _("Dashboard") }}</a></li>
             {% endif %}
+            {% if g.logout_form %}
             <li>
               <form action="{{ url_for("main.exit") }}" method="post">
                 {{ g.logout_form.hidden_tag() }}
                 {{ g.logout_form.submit(class="dropdown-item") }}
               </form>
             </li>
+            {% endif %}
           </ul>
         </li>
       {% endif %}
       </ul>
     </div>
   </nav>
```

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/list_bills.html` & `ihatemoney-6.1.0/ihatemoney/templates/list_bills.html`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     $('#bill_table tbody tr').hover(highlight_owers, unhighlight_owers);
 
     {% include "helpers.js" %}
     confirm_action(".delete-bill", { exclude_classes: "action delete", add_classes: "btn btn-sm" });
 
 {% endblock %}
 
+{% block head %}
+    <link href="{{ url_for(".feed", token=g.project.generate_token("feed")) }}" type="application/rss+xml" rel="alternate" title="{{ g.project.name }}" />
+{% endblock %}
 
 {% block sidebar %}
     <div class="sidebar_content">
         <form id="add-member-form" action="{{ url_for(".add_member") }}" method="post" class="py-3">
             {{ forms.add_member(member_form) }}
         </form>
 
@@ -157,20 +160,21 @@
         <div class="py-3 d-flex justify-content-center empty-bill">
         <div class="card d-inline-flex p-2">
             <div class="card-body text-center text-muted">
                 <i class="icon icon-white billimg">{{ static_include("images/bill.svg") | safe }}</i>
                 <h3>{{ _('No bills')}}</h3>
                 <p>
                     {{ _("Nothing to list yet.")}}<br />
-                    {{ _("You probably want to") }}
-                    {%- if g.project.members %} <a href="{{ url_for('.add_bill') }}" data-toggle="modal" data-target="#bill-form">
-                            {{- _("add a bill") -}}
-                        </a> ?
-                    {% else %} <a href="{{ url_for('.add_member') }}">
-                            {{- _('add participants') -}}
-                        </a> ?
+                    {%- if g.project.members %}
+                        <a href="{{ url_for('.add_bill') }}" data-toggle="modal" data-target="#bill-form">
+                            {{- _("Add your first bill") -}}
+                        </a>
+                    {% else %}
+                        <a href="{{ url_for('.add_member') }}">
+                            {{- _("Add the first participant") -}}
+                        </a>
                     {%- endif -%}
                 </p>
             </div>
         </div></div>
     {% endif %}
 {% endblock %}
```

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/settle_bills.html` & `ihatemoney-6.1.0/ihatemoney/templates/settle_bills.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/showcase.html` & `ihatemoney-6.1.0/ihatemoney/templates/showcase.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/sidebar_table_layout.html` & `ihatemoney-6.1.0/ihatemoney/templates/sidebar_table_layout.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/templates/statistics.html` & `ihatemoney-6.1.0/ihatemoney/templates/statistics.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/tests/api_test.py` & `ihatemoney-6.1.0/ihatemoney/tests/api_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,64 +90,93 @@
                 "id": "raclette",
                 "password": "raclette",
                 "contact_email": "not-an-email",
                 "default_currency": "XXX",
             },
         )
 
-        self.assertTrue(400, resp.status_code)
+        self.assertEqual(400, resp.status_code)
         self.assertEqual(
             '{"contact_email": ["Invalid email address."]}\n', resp.data.decode("utf-8")
         )
 
         # create it
         with self.app.mail.record_messages() as outbox:
             resp = self.api_create("raclette")
-            self.assertTrue(201, resp.status_code)
+            self.assertEqual(201, resp.status_code)
 
             # Check that email messages have been sent.
             self.assertEqual(len(outbox), 1)
             self.assertEqual(outbox[0].recipients, ["raclette@notmyidea.org"])
 
         # create it twice should return a 400
         resp = self.api_create("raclette")
 
-        self.assertTrue(400, resp.status_code)
+        self.assertEqual(400, resp.status_code)
         self.assertIn("id", json.loads(resp.data.decode("utf-8")))
 
         # get information about it
         resp = self.client.get(
             "/api/projects/raclette", headers=self.get_auth("raclette")
         )
 
-        self.assertTrue(200, resp.status_code)
+        self.assertEqual(200, resp.status_code)
         expected = {
             "members": [],
             "name": "raclette",
             "contact_email": "raclette@notmyidea.org",
             "default_currency": "XXX",
             "id": "raclette",
             "logging_preference": 1,
         }
         decoded_resp = json.loads(resp.data.decode("utf-8"))
         self.assertDictEqual(decoded_resp, expected)
 
-        # edit should work
+        # edit should fail if we don't provide the current private code
         resp = self.client.put(
             "/api/projects/raclette",
             data={
                 "contact_email": "yeah@notmyidea.org",
                 "default_currency": "XXX",
                 "password": "raclette",
                 "name": "The raclette party",
                 "project_history": "y",
             },
             headers=self.get_auth("raclette"),
         )
+        self.assertEqual(400, resp.status_code)
 
+        # edit should fail if we provide the wrong private code
+        resp = self.client.put(
+            "/api/projects/raclette",
+            data={
+                "contact_email": "yeah@notmyidea.org",
+                "default_currency": "XXX",
+                "current_password": "fromage aux patates",
+                "password": "raclette",
+                "name": "The raclette party",
+                "project_history": "y",
+            },
+            headers=self.get_auth("raclette"),
+        )
+        self.assertEqual(400, resp.status_code)
+
+        # edit with the correct private code should work
+        resp = self.client.put(
+            "/api/projects/raclette",
+            data={
+                "contact_email": "yeah@notmyidea.org",
+                "default_currency": "XXX",
+                "current_password": "raclette",
+                "password": "raclette",
+                "name": "The raclette party",
+                "project_history": "y",
+            },
+            headers=self.get_auth("raclette"),
+        )
         self.assertEqual(200, resp.status_code)
 
         resp = self.client.get(
             "/api/projects/raclette", headers=self.get_auth("raclette")
         )
 
         self.assertEqual(200, resp.status_code)
@@ -164,14 +193,15 @@
 
         # password change is possible via API
         resp = self.client.put(
             "/api/projects/raclette",
             data={
                 "contact_email": "yeah@notmyidea.org",
                 "default_currency": "XXX",
+                "current_password": "raclette",
                 "password": "tartiflette",
                 "name": "The raclette party",
             },
             headers=self.get_auth("raclette"),
         )
 
         self.assertEqual(200, resp.status_code)
@@ -193,15 +223,15 @@
         self.assertEqual(401, resp.status_code)
 
     def test_token_creation(self):
         """Test that token of project is generated"""
 
         # Create project
         resp = self.api_create("raclette")
-        self.assertTrue(201, resp.status_code)
+        self.assertEqual(201, resp.status_code)
 
         # Get token
         resp = self.client.get(
             "/api/projects/raclette/token", headers=self.get_auth("raclette")
         )
 
         self.assertEqual(200, resp.status_code)
@@ -209,17 +239,31 @@
         decoded_resp = json.loads(resp.data.decode("utf-8"))
 
         # Access with token
         resp = self.client.get(
             "/api/projects/raclette/token",
             headers={"Authorization": f"Basic {decoded_resp['token']}"},
         )
-
         self.assertEqual(200, resp.status_code)
 
+        # We shouldn't be able to edit project without private code
+        resp = self.client.put(
+            "/api/projects/raclette",
+            data={
+                "contact_email": "yeah@notmyidea.org",
+                "default_currency": "XXX",
+                "password": "tartiflette",
+                "name": "The raclette party",
+            },
+            headers={"Authorization": f"Basic {decoded_resp['token']}"},
+        )
+        self.assertEqual(400, resp.status_code)
+        expected_resp = {"current_password": ["This field is required."]}
+        self.assertEqual(expected_resp, json.loads(resp.data.decode("utf-8")))
+
     def test_token_login(self):
         resp = self.api_create("raclette")
         # Get token
         resp = self.client.get(
             "/api/projects/raclette/token", headers=self.get_auth("raclette")
         )
         decoded_resp = json.loads(resp.data.decode("utf-8"))
@@ -573,27 +617,27 @@
                 headers=self.get_auth("raclette"),
             )
             self.assertStatus(400, req)
 
     def test_currencies(self):
         # check /currencies for list of supported currencies
         resp = self.client.get("/api/currencies")
-        self.assertTrue(201, resp.status_code)
+        self.assertEqual(200, resp.status_code)
         self.assertIn("XXX", json.loads(resp.data.decode("utf-8")))
 
         # create project with a default currency
         resp = self.api_create("raclette", default_currency="EUR")
-        self.assertTrue(201, resp.status_code)
+        self.assertEqual(201, resp.status_code)
 
         # get information about it
         resp = self.client.get(
             "/api/projects/raclette", headers=self.get_auth("raclette")
         )
 
-        self.assertTrue(200, resp.status_code)
+        self.assertEqual(200, resp.status_code)
         expected = {
             "members": [],
             "name": "raclette",
             "contact_email": "raclette@notmyidea.org",
             "default_currency": "EUR",
             "id": "raclette",
             "logging_preference": 1,
@@ -715,14 +759,15 @@
 
         # Try to remove default project currency, it should fail
         req = self.client.put(
             "/api/projects/raclette",
             data={
                 "contact_email": "yeah@notmyidea.org",
                 "default_currency": "XXX",
+                "current_password": "raclette",
                 "password": "raclette",
                 "name": "The raclette party",
             },
             headers=self.get_auth("raclette"),
         )
         self.assertStatus(400, req)
         self.assertIn("This project cannot be set", req.data.decode("utf-8"))
```

### Comparing `ihatemoney-6.0.1/ihatemoney/tests/budget_test.py` & `ihatemoney-6.1.0/ihatemoney/tests/budget_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from collections import defaultdict
 import datetime
 import re
 import unittest
 from urllib.parse import urlparse, urlunparse
 
 from flask import session, url_for
+from libfaketime import fake_time
 import pytest
 from werkzeug.security import check_password_hash, generate_password_hash
 
 from ihatemoney import models
 from ihatemoney.currency_convertor import CurrencyConverter
 from ihatemoney.tests.common.help_functions import extract_link
 from ihatemoney.tests.common.ihatemoney_testcase import IhatemoneyTestCase
 from ihatemoney.versioning import LoggingMode
+from ihatemoney.web import build_etag
 
 
 class BudgetTestCase(IhatemoneyTestCase):
     def test_notifications(self):
         """Test that the notifications are sent, and that email addresses
         are checked properly.
         """
@@ -94,15 +96,15 @@
             url_start = outbox[0].body.find("You can log in using this link: ") + 32
             url_end = outbox[0].body.find(".\n", url_start)
             url = outbox[0].body[url_start:url_end]
         self.client.post("/exit")
         # Test that we got a valid token
         resp = self.client.get(url, follow_redirects=True)
         self.assertIn(
-            'You probably want to <a href="/raclette/members/add"',
+            '<a href="/raclette/members/add">Add the first participant',
             resp.data.decode("utf-8"),
         )
         # Test empty and invalid tokens
         self.client.post("/exit")
         # Use another project_id
         parsed_url = urlparse(url)
         resp = self.client.get(
@@ -146,33 +148,44 @@
         self.assertIn('href="/raclette/"', data)
 
         # Second join shouldn't add a double link
         self.client.get(invite_link)
         data = self.client.get("/tartiflette/").data.decode("utf-8")
         self.assertEqual(data.count('href="/raclette/"'), 1)
 
+    def test_invalid_invite_link_with_feed_token(self):
+        """Test that a 'feed' token is not valid to join a project"""
+        self.post_project("raclette")
+        project = self.get_project("raclette")
+        invite_link = url_for(
+            ".join_project", project_id="raclette", token=project.generate_token("feed")
+        )
+        response = self.client.get(invite_link, follow_redirects=True)
+        assert "Provided token is invalid" in response.data.decode()
+
     def test_invite_code_invalidation(self):
         """Test that invitation link expire after code change"""
         self.login("raclette")
         self.post_project("raclette")
         response = self.client.get("/raclette/invite").data.decode("utf-8")
-        link = extract_link(response, "share the following link")
+        link = extract_link(response, "give them the following invitation link")
 
         self.client.post("/exit")
         response = self.client.get(link)
         # Link is valid
         self.assertEqual(response.status_code, 302)
 
         # Change password to invalidate token
         # Other data are required, but useless for the test
         response = self.client.post(
             "/raclette/edit",
             data={
                 "name": "raclette",
                 "contact_email": "zorglub@notmyidea.org",
+                "current_password": "raclette",
                 "password": "didoudida",
                 "default_currency": "XXX",
             },
             follow_redirects=True,
         )
         self.assertEqual(response.status_code, 200)
         self.assertNotIn("alert-danger", response.data.decode("utf-8"))
@@ -360,26 +373,25 @@
         self.post_project("raclette")
         self.login("raclette")
 
         result = self.client.get("/raclette/")
 
         # Empty bill list and no participant, should now propose to add participants first
         self.assertIn(
-            'You probably want to <a href="/raclette/members/add"',
+            '<a href="/raclette/members/add">Add the first participant',
             result.data.decode("utf-8"),
         )
 
         result = self.client.post("/raclette/members/add", data={"name": "zorglub"})
 
         result = self.client.get("/raclette/")
 
         # Empty bill with member, list should now propose to add bills
-        self.assertIn(
-            'You probably want to <a href="/raclette/add"', result.data.decode("utf-8")
-        )
+        self.assertIn('<a href="/raclette/add"', result.data.decode("utf-8"))
+        self.assertIn("Add your first bill", result.data.decode("utf-8"))
 
     def test_membership(self):
         self.post_project("raclette")
         self.login("raclette")
 
         # adds a member to this project
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
@@ -907,27 +919,47 @@
             "name": "Super raclette party!",
             "contact_email": "zorglub@notmyidea.org",
             "password": "didoudida",
             "logging_preference": LoggingMode.ENABLED.value,
             "default_currency": "USD",
         }
 
-        resp = self.client.post("/raclette/edit", data=new_data, follow_redirects=True)
-        self.assertEqual(resp.status_code, 200)
+        # It should fail if we don't provide the current password
+        resp = self.client.post("/raclette/edit", data=new_data, follow_redirects=False)
+        self.assertIn("This field is required", resp.data.decode("utf-8"))
+        project = self.get_project("raclette")
+        self.assertNotEqual(project.name, new_data["name"])
+        self.assertNotEqual(project.contact_email, new_data["contact_email"])
+        self.assertNotEqual(project.default_currency, new_data["default_currency"])
+        self.assertFalse(check_password_hash(project.password, new_data["password"]))
+
+        # It should fail if we provide the wrong current password
+        new_data["current_password"] = "patates au fromage"
+        resp = self.client.post("/raclette/edit", data=new_data, follow_redirects=False)
+        self.assertIn("Invalid private code", resp.data.decode("utf-8"))
+        project = self.get_project("raclette")
+        self.assertNotEqual(project.name, new_data["name"])
+        self.assertNotEqual(project.contact_email, new_data["contact_email"])
+        self.assertNotEqual(project.default_currency, new_data["default_currency"])
+        self.assertFalse(check_password_hash(project.password, new_data["password"]))
+
+        # It should work if we give the current private code
+        new_data["current_password"] = "raclette"
+        resp = self.client.post("/raclette/edit", data=new_data)
+        self.assertEqual(resp.status_code, 302)
         project = self.get_project("raclette")
-
         self.assertEqual(project.name, new_data["name"])
         self.assertEqual(project.contact_email, new_data["contact_email"])
         self.assertEqual(project.default_currency, new_data["default_currency"])
         self.assertTrue(check_password_hash(project.password, new_data["password"]))
 
         # Editing a project with a wrong email address should fail
         new_data["contact_email"] = "wrong_email"
 
-        resp = self.client.post("/raclette/edit", data=new_data, follow_redirects=True)
+        resp = self.client.post("/raclette/edit", data=new_data)
         self.assertIn("Invalid email address", resp.data.decode("utf-8"))
 
     def test_dashboard(self):
         # test that the dashboard is deactivated by default
         resp = self.client.post(
             "/admin?goto=%2Fdashboard",
             data={"admin_password": "adminpass"},
@@ -1681,10 +1713,363 @@
             with c.session_transaction() as sess:
                 sess["projects"] = [("raclette", "raclette")]
             # It should convert entry to dict
             c.get("/")
             self.assertIsInstance(session["projects"], dict)
             self.assertIn("raclette", session["projects"])
 
+    def test_rss_feed(self):
+        """
+        Tests that the RSS feed output content is expected.
+        """
+        with fake_time("2023-07-25 12:00:00"):
+            self.post_project("raclette")
+            self.client.post("/raclette/members/add", data={"name": "george"})
+            self.client.post("/raclette/members/add", data={"name": "peter"})
+            self.client.post("/raclette/members/add", data={"name": "steven"})
+
+            self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-31",
+                    "what": "fromage à raclette",
+                    "payer": 1,
+                    "payed_for": [1, 2, 3],
+                    "amount": "12",
+                    "original_currency": "EUR",
+                },
+            )
+            self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-30",
+                    "what": "charcuterie",
+                    "payer": 2,
+                    "payed_for": [1, 2],
+                    "amount": "15",
+                    "original_currency": "EUR",
+                },
+            )
+            self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-29",
+                    "what": "vin blanc",
+                    "payer": 2,
+                    "payed_for": [1, 2],
+                    "amount": "10",
+                    "original_currency": "EUR",
+                },
+            )
+
+        project = self.get_project("raclette")
+        token = project.generate_token("feed")
+        resp = self.client.get(f"/raclette/feed/{token}.xml")
+
+        expected_rss_content = f"""<?xml version="1.0" encoding="utf-8"?>
+<rss version="2.0"
+    xmlns:dc="http://purl.org/dc/elements/1.1/"
+    xmlns:atom="http://www.w3.org/2005/Atom"
+    >
+    <channel>
+        <title>I Hate Money — raclette</title>
+        <description>Latest bills from raclette</description>
+        <atom:link href="http://localhost/raclette/feed/{token}.xml" rel="self" type="application/rss+xml" />
+        <link>http://localhost/raclette/</link>
+        <item>
+            <title>fromage à raclette - €12.00</title>
+            <guid isPermaLink="false">1</guid>
+            <dc:creator>george</dc:creator>
+            <description>December 31, 2016 - george, peter, steven : €4.00</description>
+            <pubDate>Tue, 25 Jul 2023 00:00:00 +0000</pubDate>
+        </item>
+        <item>
+            <title>charcuterie - €15.00</title>
+            <guid isPermaLink="false">2</guid>
+            <dc:creator>peter</dc:creator>
+            <description>December 30, 2016 - george, peter : €7.50</description>
+            <pubDate>Tue, 25 Jul 2023 00:00:00 +0000</pubDate>
+        </item>
+        <item>
+            <title>vin blanc - €10.00</title>
+            <guid isPermaLink="false">3</guid>
+            <dc:creator>peter</dc:creator>
+            <description>December 29, 2016 - george, peter : €5.00</description>
+            <pubDate>Tue, 25 Jul 2023 00:00:00 +0000</pubDate>
+        </item>
+        </channel>
+</rss>"""  # noqa: E501
+        assert resp.data.decode() == expected_rss_content
+
+    def test_rss_feed_history_disabled(self):
+        """
+        Tests that RSS feeds is correctly rendered even if the project
+        history is disabled.
+        """
+        with fake_time("2023-07-25 12:00:00"):
+            self.post_project("raclette", project_history=False)
+            self.client.post("/raclette/members/add", data={"name": "george"})
+            self.client.post("/raclette/members/add", data={"name": "peter"})
+            self.client.post("/raclette/members/add", data={"name": "steven"})
+
+            self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-31",
+                    "what": "fromage à raclette",
+                    "payer": 1,
+                    "payed_for": [1, 2, 3],
+                    "amount": "12",
+                    "original_currency": "EUR",
+                },
+            )
+            self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-30",
+                    "what": "charcuterie",
+                    "payer": 2,
+                    "payed_for": [1, 2],
+                    "amount": "15",
+                    "original_currency": "EUR",
+                },
+            )
+            self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-29",
+                    "what": "vin blanc",
+                    "payer": 2,
+                    "payed_for": [1, 2],
+                    "amount": "10",
+                    "original_currency": "EUR",
+                },
+            )
+
+        project = self.get_project("raclette")
+        token = project.generate_token("feed")
+        resp = self.client.get(f"/raclette/feed/{token}.xml")
+
+        expected_rss_content = f"""<?xml version="1.0" encoding="utf-8"?>
+<rss version="2.0"
+    xmlns:dc="http://purl.org/dc/elements/1.1/"
+    xmlns:atom="http://www.w3.org/2005/Atom"
+    >
+    <channel>
+        <title>I Hate Money — raclette</title>
+        <description>Latest bills from raclette</description>
+        <atom:link href="http://localhost/raclette/feed/{token}.xml" rel="self" type="application/rss+xml" />
+        <link>http://localhost/raclette/</link>
+        <item>
+            <title>fromage à raclette - €12.00</title>
+            <guid isPermaLink="false">1</guid>
+            <dc:creator>george</dc:creator>
+            <description>December 31, 2016 - george, peter, steven : €4.00</description>
+            <pubDate>Tue, 25 Jul 2023 00:00:00 +0000</pubDate>
+        </item>
+        <item>
+            <title>charcuterie - €15.00</title>
+            <guid isPermaLink="false">2</guid>
+            <dc:creator>peter</dc:creator>
+            <description>December 30, 2016 - george, peter : €7.50</description>
+            <pubDate>Tue, 25 Jul 2023 00:00:00 +0000</pubDate>
+        </item>
+        <item>
+            <title>vin blanc - €10.00</title>
+            <guid isPermaLink="false">3</guid>
+            <dc:creator>peter</dc:creator>
+            <description>December 29, 2016 - george, peter : €5.00</description>
+            <pubDate>Tue, 25 Jul 2023 00:00:00 +0000</pubDate>
+        </item>
+        </channel>
+</rss>"""  # noqa: E501
+        assert resp.data.decode() == expected_rss_content
+
+    def test_rss_if_modified_since_header(self):
+        # Project creation
+        with fake_time("2023-07-26 13:00:00"):
+            self.post_project("raclette")
+            self.client.post("/raclette/members/add", data={"name": "george"})
+            project = self.get_project("raclette")
+            token = project.generate_token("feed")
+
+            resp = self.client.get(f"/raclette/feed/{token}.xml")
+            assert resp.status_code == 200
+            assert resp.headers.get("Last-Modified") == "Wed, 26 Jul 2023 13:00:00 UTC"
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={"If-Modified-Since": "Tue, 26 Jul 2023 12:00:00 UTC"},
+        )
+        assert resp.status_code == 200
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={"If-Modified-Since": "Tue, 26 Jul 2023 14:00:00 UTC"},
+        )
+        assert resp.status_code == 304
+
+        # Add bill
+        with fake_time("2023-07-27 13:00:00"):
+            self.login("raclette")
+            resp = self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-31",
+                    "what": "fromage à raclette",
+                    "payer": 1,
+                    "payed_for": [1],
+                    "amount": "12",
+                    "original_currency": "EUR",
+                },
+                follow_redirects=True,
+            )
+            assert resp.status_code == 200
+            assert "The bill has been added" in resp.data.decode()
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={"If-Modified-Since": "Tue, 27 Jul 2023 12:00:00 UTC"},
+        )
+        assert resp.headers.get("Last-Modified") == "Thu, 27 Jul 2023 13:00:00 UTC"
+        assert resp.status_code == 200
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={"If-Modified-Since": "Tue, 27 Jul 2023 14:00:00 UTC"},
+        )
+        assert resp.status_code == 304
+
+    def test_rss_etag_headers(self):
+        # Project creation
+        with fake_time("2023-07-26 13:00:00"):
+            self.post_project("raclette")
+            self.client.post("/raclette/members/add", data={"name": "george"})
+            project = self.get_project("raclette")
+            token = project.generate_token("feed")
+
+            resp = self.client.get(f"/raclette/feed/{token}.xml")
+            assert resp.headers.get("ETag") == build_etag(
+                project.id, "2023-07-26T13:00:00"
+            )
+            assert resp.status_code == 200
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={
+                "If-None-Match": build_etag(project.id, "2023-07-26T12:00:00"),
+            },
+        )
+        assert resp.status_code == 200
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={
+                "If-None-Match": build_etag(project.id, "2023-07-26T13:00:00"),
+            },
+        )
+        assert resp.status_code == 304
+
+        # Add bill
+        with fake_time("2023-07-27 13:00:00"):
+            self.login("raclette")
+            resp = self.client.post(
+                "/raclette/add",
+                data={
+                    "date": "2016-12-31",
+                    "what": "fromage à raclette",
+                    "payer": 1,
+                    "payed_for": [1],
+                    "amount": "12",
+                    "original_currency": "EUR",
+                },
+                follow_redirects=True,
+            )
+            assert resp.status_code == 200
+            assert "The bill has been added" in resp.data.decode()
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={
+                "If-None-Match": build_etag(project.id, "2023-07-27T12:00:00"),
+            },
+        )
+        assert resp.headers.get("ETag") == build_etag(project.id, "2023-07-27T13:00:00")
+        assert resp.status_code == 200
+
+        resp = self.client.get(
+            f"/raclette/feed/{token}.xml",
+            headers={
+                "If-None-Match": build_etag(project.id, "2023-07-27T13:00:00"),
+            },
+        )
+        assert resp.status_code == 304
+
+    def test_rss_feed_bad_token(self):
+        self.post_project("raclette")
+        project = self.get_project("raclette")
+        token = project.generate_token("feed")
+
+        resp = self.client.get(f"/raclette/feed/{token}.xml")
+        self.assertEqual(resp.status_code, 200)
+        resp = self.client.get("/raclette/feed/invalid-token.xml")
+        self.assertEqual(resp.status_code, 404)
+
+    def test_rss_feed_different_project_with_same_password(
+        self,
+    ):
+        """
+        Test that a 'feed' token is not valid to access the feed of
+        another project with the same password.
+        """
+        self.post_project("raclette", password="password")
+        self.post_project("reblochon", password="password")
+        project = self.get_project("raclette")
+        token = project.generate_token("feed")
+
+        resp = self.client.get(f"/reblochon/feed/{token}.xml")
+        self.assertEqual(resp.status_code, 404)
+
+    def test_rss_feed_different_project_with_different_password(
+        self,
+    ):
+        """
+        Test that a 'feed' token is not valid to access the feed of
+        another project with a different password.
+        """
+        self.post_project("raclette", password="password")
+        self.post_project("reblochon", password="another-password")
+        project = self.get_project("raclette")
+        token = project.generate_token("feed")
+
+        resp = self.client.get(f"/reblochon/feed/{token}.xml")
+        self.assertEqual(resp.status_code, 404)
+
+    def test_rss_feed_invalidated_token(self):
+        """
+        Tests that a feed URL becames invalid when the project password changes.
+        """
+        self.post_project("raclette")
+        project = self.get_project("raclette")
+        token = project.generate_token("feed")
+
+        resp = self.client.get(f"/raclette/feed/{token}.xml")
+        self.assertEqual(resp.status_code, 200)
+
+        self.client.post(
+            "/raclette/edit",
+            data={
+                "name": "raclette",
+                "contact_email": "zorglub@notmyidea.org",
+                "current_password": "raclette",
+                "password": "didoudida",
+                "default_currency": "XXX",
+            },
+            follow_redirects=True,
+        )
+
+        resp = self.client.get(f"/raclette/feed/{token}.xml")
+        self.assertEqual(resp.status_code, 404)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ihatemoney-6.0.1/ihatemoney/tests/common/ihatemoney_testcase.py` & `ihatemoney-6.1.0/ihatemoney/tests/common/ihatemoney_testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,27 +52,29 @@
     def post_project(
         self,
         id,
         follow_redirects=True,
         default_currency="XXX",
         name=None,
         password=None,
+        project_history=True,
     ):
         """Create a fake project"""
         name = name or id
         password = password or id
         # create the project
         return self.client.post(
             "/create",
             data={
                 "name": name,
                 "id": id,
                 "password": password,
                 "contact_email": f"{id}@notmyidea.org",
                 "default_currency": default_currency,
+                "project_history": project_history,
             },
             follow_redirects=follow_redirects,
         )
 
     def import_project(self, id, data, success=True):
         resp = self.client.post(
             f"/{id}/import",
```

### Comparing `ihatemoney-6.0.1/ihatemoney/tests/history_test.py` & `ihatemoney-6.1.0/ihatemoney/tests/history_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,20 @@
     def test_simple_create_logentry_no_ip(self):
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn(f"Project {em_surround('demo')} added", resp.data.decode("utf-8"))
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 1)
         self.assertNotIn("127.0.0.1", resp.data.decode("utf-8"))
 
-    def change_privacy_to(self, logging_preference):
+    def change_privacy_to(self, current_password, logging_preference):
         # Change only logging_preferences
         new_data = {
             "name": "demo",
             "contact_email": "demo@notmyidea.org",
+            "current_password": current_password,
             "password": "demo",
             "default_currency": "XXX",
         }
 
         if logging_preference != LoggingMode.DISABLED:
             new_data["project_history"] = "y"
             if logging_preference == LoggingMode.RECORD_IP:
@@ -72,14 +73,15 @@
             f"Project {em_surround('demo')} added", resp.data.decode("utf-8")
         )
 
     def test_project_edit(self):
         new_data = {
             "name": "demo2",
             "contact_email": "demo2@notmyidea.org",
+            "current_password": "demo",
             "password": "123456",
             "project_history": "y",
             "default_currency": "USD",  # Currency changed from default
         }
 
         resp = self.client.post("/demo/edit", data=new_data, follow_redirects=True)
         self.assertEqual(resp.status_code, 200)
@@ -110,71 +112,72 @@
         resp = self.client.get("/demo/edit")
         self.assertEqual(resp.status_code, 200)
         self.assertIn(
             '<input checked id="project_history" name="project_history" type="checkbox" value="y">',
             resp.data.decode("utf-8"),
         )
 
-        self.change_privacy_to(LoggingMode.DISABLED)
+        self.change_privacy_to("demo", LoggingMode.DISABLED)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn("Disabled Project History\n", resp.data.decode("utf-8"))
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 2)
         self.assertNotIn("127.0.0.1", resp.data.decode("utf-8"))
 
-        self.change_privacy_to(LoggingMode.RECORD_IP)
+        self.change_privacy_to("demo", LoggingMode.RECORD_IP)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn(
             "Enabled Project History & IP Address Recording", resp.data.decode("utf-8")
         )
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 2)
         self.assertEqual(resp.data.decode("utf-8").count("127.0.0.1"), 1)
 
-        self.change_privacy_to(LoggingMode.ENABLED)
+        self.change_privacy_to("demo", LoggingMode.ENABLED)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn("Disabled IP Address Recording\n", resp.data.decode("utf-8"))
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 2)
         self.assertEqual(resp.data.decode("utf-8").count("127.0.0.1"), 2)
 
     def test_project_privacy_edit2(self):
-        self.change_privacy_to(LoggingMode.RECORD_IP)
+        self.change_privacy_to("demo", LoggingMode.RECORD_IP)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn("Enabled IP Address Recording\n", resp.data.decode("utf-8"))
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 1)
         self.assertEqual(resp.data.decode("utf-8").count("127.0.0.1"), 1)
 
-        self.change_privacy_to(LoggingMode.DISABLED)
+        self.change_privacy_to("demo", LoggingMode.DISABLED)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn(
             "Disabled Project History & IP Address Recording", resp.data.decode("utf-8")
         )
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 1)
         self.assertEqual(resp.data.decode("utf-8").count("127.0.0.1"), 2)
 
-        self.change_privacy_to(LoggingMode.ENABLED)
+        self.change_privacy_to("demo", LoggingMode.ENABLED)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn("Enabled Project History\n", resp.data.decode("utf-8"))
         self.assertEqual(resp.data.decode("utf-8").count("<td> -- </td>"), 2)
         self.assertEqual(resp.data.decode("utf-8").count("127.0.0.1"), 2)
 
     def do_misc_database_operations(self, logging_mode):
         new_data = {
             "name": "demo2",
             "contact_email": "demo2@notmyidea.org",
+            "current_password": "demo",
             "password": "123456",
             "default_currency": "USD",
         }
 
         # Keep privacy settings where they were
         if logging_mode != LoggingMode.DISABLED:
             new_data["project_history"] = "y"
@@ -229,15 +232,15 @@
         resp = self.client.post(
             f"/demo/members/{user_id}/delete", follow_redirects=True
         )
         self.assertEqual(resp.status_code, 200)
 
     def test_disable_clear_no_new_records(self):
         # Disable logging
-        self.change_privacy_to(LoggingMode.DISABLED)
+        self.change_privacy_to("demo", LoggingMode.DISABLED)
 
         # Ensure we can't clear history with a GET or with a password-less POST
         resp = self.client.get("/demo/erase_history")
         self.assertEqual(resp.status_code, 405)
         resp = self.client.post("/demo/erase_history", follow_redirects=True)
         self.assertIn(
             "Error deleting project history",
@@ -272,21 +275,21 @@
         # Do lots of database operations & check that there's still no history
         self.do_misc_database_operations(LoggingMode.DISABLED)
 
         self.assert_empty_history_logging_disabled()
 
     def test_clear_ip_records(self):
         # Enable IP Recording
-        self.change_privacy_to(LoggingMode.RECORD_IP)
+        self.change_privacy_to("demo", LoggingMode.RECORD_IP)
 
         # Do lots of database operations to generate IP address entries
         self.do_misc_database_operations(LoggingMode.RECORD_IP)
 
         # Disable IP Recording
-        self.change_privacy_to(LoggingMode.ENABLED)
+        self.change_privacy_to("123456", LoggingMode.ENABLED)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertNotIn(
             "This project has history disabled. New actions won't appear below.",
             resp.data.decode("utf-8"),
         )
```

### Comparing `ihatemoney-6.0.1/ihatemoney/tests/import_test.py` & `ihatemoney-6.1.0/ihatemoney/tests/import_test.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/tests/main_test.py` & `ihatemoney-6.1.0/ihatemoney/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,30 +235,30 @@
         # Check that an error message is displayed
         self.assertIn(
             "We tried to send you an reminder email, but there was an error",
             resp.data.decode("utf-8"),
         )
         # Check that we were redirected to the home page anyway
         self.assertIn(
-            'You probably want to <a href="/raclette/members/add"',
+            '<a href="/raclette/members/add">Add the first participant',
             resp.data.decode("utf-8"),
         )
 
     def test_creation_email_failure_socket(self):
         self.login("raclette")
         with patch.object(self.app.mail, "send", MagicMock(side_effect=socket.error)):
             resp = self.post_project("raclette")
         # Check that an error message is displayed
         self.assertIn(
             "We tried to send you an reminder email, but there was an error",
             resp.data.decode("utf-8"),
         )
         # Check that we were redirected to the home page anyway
         self.assertIn(
-            'You probably want to <a href="/raclette/members/add"',
+            '<a href="/raclette/members/add">Add the first participant',
             resp.data.decode("utf-8"),
         )
 
     def test_password_reset_email_failure(self):
         self.create_project("raclette")
         for exception in (smtplib.SMTPException, socket.error):
             with patch.object(self.app.mail, "send", MagicMock(side_effect=exception)):
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/bn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/bn/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-04-14 21:10+0000\n"
 "Last-Translator: Hasidul Islam <ihasidul@gmail.com>\n"
 "Language: bn\n"
 "Language-Team: Bengali <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/bn/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
@@ -23,14 +23,21 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr "প্রজেক্টের নাম"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "নতুন ব্যক্তিগত কোড"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "নতুন ব্যক্তিগত কোড"
 
 msgid "Enter a new code if you want to change it"
 msgstr "আপনি যদি এটি পরিবর্তন করতে চান তবে একটি নতুন কোড লিখুন"
 
 msgid "Email"
@@ -44,14 +51,20 @@
 
 msgid "Default Currency"
 msgstr "ডিফল্ট মুদ্রা"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "অজানা ত্রুটি"
+
+msgid "Invalid private code."
+msgstr "অবৈধ ব্যক্তিগত কোড."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "এই প্রজেক্টটি 'নো কারেন্সি' সেট করা যাবে না কারণ এতে একাধিক মুদ্রার বিল "
 "রয়েছে৷"
 
@@ -83,20 +96,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "অনুগ্রহ করে, এগিয়ে যেতে ক্যাপচা যাচাই করুন।"
 
 msgid "Enter private code to confirm deletion"
 msgstr "মুছে ফেলা নিশ্চিত করতে ব্যক্তিগত কোড লিখুন"
 
-msgid "Unknown error"
-msgstr "অজানা ত্রুটি"
-
-msgid "Invalid private code."
-msgstr "অবৈধ ব্যক্তিগত কোড."
-
 msgid "Get in"
 msgstr "প্রবেশ করুন"
 
 msgid "Admin password"
 msgstr "অ্যাডমিন পাসওয়ার্ড"
 
 msgid "Send me the code by email"
@@ -252,14 +259,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -743,14 +753,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -819,21 +832,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -848,45 +858,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "ব্যক্তিগত কোড"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -985,7 +1007,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2020-08-01 10:41+0000\n"
 "Last-Translator: Oymate <dhruboadittya96@gmail.com>\n"
 "Language: bn_BD\n"
 "Language-Team: Bengali (Bangladesh) "
 "<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/bn_BD/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -26,14 +26,21 @@
 "কোন বৈধ পরিমাণ বা অভিব্যক্তি নয়। শুধুমাত্র সংখ্যা এবং + - * / অপারেটর "
 "গ্রহণ করা হয়।"
 
 msgid "Project name"
 msgstr "প্রকল্পের নাম"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "ব্যক্তিগত কোড"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "ব্যক্তিগত কোড"
 
 msgid "Enter a new code if you want to change it"
 msgstr "আপনি যদি এটি পরিবর্তন করতে চান তবে একটি নতুন কোড লিখুন"
 
 msgid "Email"
@@ -47,14 +54,21 @@
 
 msgid "Default Currency"
 msgstr "ডিফল্ট মুদ্রা"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "অজানা ত্রুট"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "ব্যক্তিগত কোড"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -82,21 +96,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr "মুছে ফেলার জন্য ব্যক্তিগত কোড লিখুন"
 
-msgid "Unknown error"
-msgstr "অজানা ত্রুট"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "ব্যক্তিগত কোড"
-
 msgid "Get in"
 msgstr "ভিতরে আস"
 
 msgid "Admin password"
 msgstr "অ্যাডমিন পাসওয়ার্ড"
 
 msgid "Send me the code by email"
@@ -252,14 +259,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -746,14 +756,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -822,21 +835,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -851,45 +861,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "ব্যক্তিগত কোড"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1090,7 +1112,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/ca/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-09-12 15:25+0000\n"
 "Last-Translator: Maite Guix <maite.guix@gmail.com>\n"
 "Language: ca\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/ca/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "No és un import o expressió vàlida. Només s'accepten números i els "
 "operadors + - * /."
 
 msgid "Project name"
 msgstr "Nom del projecte"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Codi privat nou"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Codi privat nou"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Introdueix un codi nou si vols el canviar"
 
 msgid "Email"
@@ -48,14 +55,20 @@
 msgstr "Moneda per defecte"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "L'establiment d'una moneda predeterminada permet la conversió de moneda "
 "entre factures"
 
+msgid "Unknown error"
+msgstr "Error desconegut"
+
+msgid "Invalid private code."
+msgstr "Codi privat no vàlid."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Aquest projecte no es pot definir com a «cap moneda» perquè conté "
 "factures en diverses monedes."
 
@@ -87,20 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Si us plau, valida el captcha per a continuar."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Introdueix el codi privat per a confirmar la supressió"
 
-msgid "Unknown error"
-msgstr "Error desconegut"
-
-msgid "Invalid private code."
-msgstr "Codi privat no vàlid."
-
 msgid "Get in"
 msgstr "Entrar-hi"
 
 msgid "Admin password"
 msgstr "Contrasenya d'administració"
 
 msgid "Send me the code by email"
@@ -269,14 +276,17 @@
 
 msgid "Unknown project"
 msgstr "Projecte desconegut"
 
 msgid "Password successfully reset."
 msgstr "La contrasenya s'ha restablert correctament."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -787,14 +797,17 @@
 
 msgid "History"
 msgstr "Historial"
 
 msgid "Settings"
 msgstr "Configuració"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Altres projectes:"
 
 msgid "switch to"
 msgstr "commutar a"
 
 msgid "Dashboard"
@@ -863,22 +876,21 @@
 
 msgid "No bills"
 msgstr "Sense factures"
 
 msgid "Nothing to list yet."
 msgstr "Res a enumerar encara."
 
-msgid "You probably want to"
-msgstr "Probablement vulguis"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "afegir una factura"
 
-msgid "add participants"
-msgstr "afegir participants"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Editar aquest participant"
 
 msgid "Password reminder"
 msgstr "Recordatori de contrasenya"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -894,55 +906,64 @@
 
 msgid "Reset your password"
 msgstr "Restablir la contrasenya"
 
 msgid "Invite people to join this project"
 msgstr "Convidar a persones a unir-se a aquest projecte"
 
-msgid "Share Identifier & code"
-msgstr "Compartir l'identificador i el codi"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Pots compartir l'identificador del projecte i el codi privat per "
-"qualsevol mitjà de comunicació."
 
-msgid "Identifier:"
-msgstr "Identificador:"
-
-msgid "Share the Link"
-msgstr "Compartir l'enllaç"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Pots compartir directament l'enllaç següent a través del teu mitjà "
-"preferit"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Enviar per correu electrònic"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Especifica una llista (separada per comes) dels correus electrònic als "
 "que vols notificar la\n"
 "                creació d'aquest projecte de gestió pressupostària i els "
 "hi enviarem un correu electrònic."
 
+msgid "Share Identifier & code"
+msgstr "Compartir l'identificador i el codi"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificador:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Codi privat"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Qui ha de pagar?"
 
 msgid "To whom?"
 msgstr "A qui?"
 
 msgid "Who?"
@@ -1035,7 +1056,30 @@
 
 #~ msgid " show"
 #~ msgstr "mostrar"
 
 #~ msgid "Edit the project"
 #~ msgstr "Editar el projecte"
 
+#~ msgid "You probably want to"
+#~ msgstr "Probablement vulguis"
+
+#~ msgid "add participants"
+#~ msgstr "afegir participants"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Pots compartir l'identificador del projecte"
+#~ " i el codi privat per qualsevol "
+#~ "mitjà de comunicació."
+
+#~ msgid "Share the Link"
+#~ msgstr "Compartir l'enllaç"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Pots compartir directament l'enllaç següent"
+#~ " a través del teu mitjà preferit"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-11-07 10:07+0000\n"
 "Last-Translator: Moshi Moshi <ifeeltiredboss@gmail.com>\n"
 "Language: cs\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/cs/>\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
@@ -23,14 +23,21 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "Neplatná částka nebo výraz. Pouze čísla a operátory + - * / jsou přípustná"
 
 msgid "Project name"
 msgstr "Název projektu"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Nový soukromý kód"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Nový soukromý kód"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Pokud chcete provést změnu vložte nový kód"
 
 msgid "Email"
@@ -44,14 +51,20 @@
 
 msgid "Default Currency"
 msgstr "Výchozí měna"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "Neznámá chyba"
+
+msgid "Invalid private code."
+msgstr "Neplatný soukromý přístupový kód."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Tento projekt nemůže být nastaven na 'bez měny' protože obsahuje účty v "
 "různých měnáh."
 
@@ -83,20 +96,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr "Potvrďte smazání vložením soukromého kódu"
 
-msgid "Unknown error"
-msgstr "Neznámá chyba"
-
-msgid "Invalid private code."
-msgstr "Neplatný soukromý přístupový kód."
-
 msgid "Get in"
 msgstr "Vstoupit"
 
 msgid "Admin password"
 msgstr "Administrátorské heslo"
 
 msgid "Send me the code by email"
@@ -263,14 +270,17 @@
 
 msgid "Unknown project"
 msgstr "Neznámý projekt"
 
 msgid "Password successfully reset."
 msgstr "Heslo bylo úspěšné obnoveno."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -759,14 +769,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -835,21 +848,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -864,45 +874,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Přístupový kód"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1105,7 +1127,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/de/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-07-16 14:04+0000\n"
 "Last-Translator: Luke <luke@luporr.de>\n"
-"Language-Team: German <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/de/>\n"
 "Language: de\n"
+"Language-Team: German <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/de/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr ""
 "Du hast gerade das Projekt '%(project)s' erstellt, um deine Ausgaben zu "
 "teilen"
@@ -27,14 +27,21 @@
 msgstr ""
 "Kein gültiger Betrag oder Ausdruck. Es werden nur Zahlen und die "
 "Operatoren + - * / akzeptiert."
 
 msgid "Project name"
 msgstr "Projektname"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Neuer privater Code"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Neuer privater Code"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Gib einen neuen Code ein, falls du ihn ändern möchtest"
 
 msgid "Email"
@@ -50,14 +57,20 @@
 msgstr "Standardwährung"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Das Festlegen einer Standardwährung ermöglicht die Währungsumrechnung "
 "zwischen Rechnungen"
 
+msgid "Unknown error"
+msgstr "Unbekannter Fehler"
+
+msgid "Invalid private code."
+msgstr "ungültiger privater Code."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Dieses Projekt kann nicht auf \"ohne Währung\" eingestellt werden, weil "
 "es Rechnungen unterschiedlicher Währungen enthält."
 
@@ -89,20 +102,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Bitte bestätige das Captcha, um fortzufahren."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Geben Sie Ihren privaten Code ein, um die Löschung zu bestätigen"
 
-msgid "Unknown error"
-msgstr "Unbekannter Fehler"
-
-msgid "Invalid private code."
-msgstr "ungültiger privater Code."
-
 msgid "Get in"
 msgstr "Eintreten"
 
 msgid "Admin password"
 msgstr "Admin-Passwort"
 
 msgid "Send me the code by email"
@@ -274,14 +281,17 @@
 
 msgid "Unknown project"
 msgstr "Unbekanntes Projekt"
 
 msgid "Password successfully reset."
 msgstr "Passwort erfolgreich zurückgesetzt."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -789,14 +799,17 @@
 
 msgid "History"
 msgstr "Verlauf"
 
 msgid "Settings"
 msgstr "Einstellungen"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Andere Projekte:"
 
 msgid "switch to"
 msgstr "wechseln zu"
 
 msgid "Dashboard"
@@ -865,22 +878,21 @@
 
 msgid "No bills"
 msgstr "Keine Ausgaben"
 
 msgid "Nothing to list yet."
 msgstr "Noch nichts aufzulisten."
 
-msgid "You probably want to"
-msgstr "Du willst wahrscheinlich"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "eine Ausgabe hinzufügen"
 
-msgid "add participants"
-msgstr "Teilnehmer hinzufügen"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Diesen Benutzer bearbeiten"
 
 msgid "Password reminder"
 msgstr "Passwort-Erinnerung"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -896,53 +908,64 @@
 
 msgid "Reset your password"
 msgstr "Setze dein Passwort zurück"
 
 msgid "Invite people to join this project"
 msgstr "Lade Leute ein, diesem Projekt beizutreten"
 
-msgid "Share Identifier & code"
-msgstr "Teile die ID & den Code"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Du kannst die Projekt-ID und den privaten Code auf jedem "
-"Kommunikationsweg weitergeben."
-
-msgid "Identifier:"
-msgstr "ID:"
-
-msgid "Share the Link"
-msgstr "Link teilen"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Du kannst den folgenden Link direkt über dein bevorzugtes Medium teilen"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Per E-Mail versenden"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Gib eine (durch Kommas getrennte) Liste von E-Mail-Adressen an, die du "
 "über die\n"
 "\t\t\tErstellung dieses Projekts informieren möchtest, und wir senden "
 "ihnen eine E-Mail."
 
+msgid "Share Identifier & code"
+msgstr "Teile die ID & den Code"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Privater Code"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Wer zahlt?"
 
 msgid "To whom?"
 msgstr "An wen?"
 
 msgid "Who?"
@@ -1139,7 +1162,29 @@
 #~ msgstr "Einladungen senden"
 
 #~ msgid " show"
 #~ msgstr "Zeigen"
 
 #~ msgid "Edit the project"
 #~ msgstr "Projekt bearbeiten"
+
+#~ msgid "You probably want to"
+#~ msgstr "Du willst wahrscheinlich"
+
+#~ msgid "add participants"
+#~ msgstr "Teilnehmer hinzufügen"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Du kannst die Projekt-ID und den"
+#~ " privaten Code auf jedem Kommunikationsweg"
+#~ " weitergeben."
+
+#~ msgid "Share the Link"
+#~ msgstr "Link teilen"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "Du kannst den folgenden Link direkt über dein bevorzugtes Medium teilen"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/el/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-08-01 08:34+0000\n"
 "Last-Translator: Eugenia Russell <eugenia.russell2019@gmail.com>\n"
 "Language: el\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/el/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -24,14 +24,21 @@
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr "Τίτλος εργασίας"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "Ιδιωτικός κωδικός"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "Ιδιωτικός κωδικός"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Εισαγάγετε έναν νέο κωδικό εάν θέλετε να τον αλλάξετε"
 
 msgid "Email"
@@ -45,14 +52,22 @@
 
 msgid "Default Currency"
 msgstr "Προεπιλεγμένο Νόμισμα"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+#, fuzzy
+msgid "Unknown error"
+msgstr "Άγνωστο πρότζεκτ"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "Ιδιωτικός κωδικός"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Αυτό το έργο δεν μπορεί να οριστεί σε \"χωρίς νόμισμα\" επειδή περιέχει "
 "λογαριασμούς σε πολλαπλά νομίσματα."
 
@@ -85,22 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr "Εισαγάγετε ιδιωτικό κωδικό για επιβεβαίωση της διαγραφής"
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "Άγνωστο πρότζεκτ"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "Ιδιωτικός κωδικός"
-
 msgid "Get in"
 msgstr "Συνδεθείτε"
 
 msgid "Admin password"
 msgstr "Κωδικός πρόσβασης διαχειριστή"
 
 msgid "Send me the code by email"
@@ -265,14 +272,17 @@
 
 msgid "Unknown project"
 msgstr "Άγνωστο πρότζεκτ"
 
 msgid "Password successfully reset."
 msgstr "Επαναφορά του κωδικού επιτυχώς."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -772,14 +782,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -849,22 +862,20 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
-msgstr ""
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Προσθήκη συμμετέχοντος"
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -878,45 +889,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Ιδιωτικός κωδικός"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1093,7 +1116,47 @@
 
 #~ msgid " show"
 #~ msgstr "εμφάνιση"
 
 #~ msgid "Edit the project"
 #~ msgstr "Επεξεργαστείτε το έργο"
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-10-01 20:35+0000\n"
 "Last-Translator: phlostically <phlostically@mailinator.com>\n"
 "Language: eo\n"
 "Language-Team: Esperanto <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/eo/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Ne valida kvanto aŭ esprimo. Nur nombroj kaj la operatoroj + - * / estas "
 "akceptataj."
 
 msgid "Project name"
 msgstr "Nomo de projekto"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Nova privata kodo"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Nova privata kodo"
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -46,14 +53,20 @@
 
 msgid "Default Currency"
 msgstr "Implicita valuto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "Nekonata eraro"
+
+msgid "Invalid private code."
+msgstr "Nevalida privata kodo."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Ĉi tiu projekto ne povas esti agordita al «neniu valuto», ĉar ĝi enhavas "
 "fakturojn en pluraj valutoj."
 
@@ -86,20 +99,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-msgid "Unknown error"
-msgstr "Nekonata eraro"
-
-msgid "Invalid private code."
-msgstr "Nevalida privata kodo."
-
 msgid "Get in"
 msgstr "Eniri"
 
 msgid "Admin password"
 msgstr "Administra pasvorto"
 
 msgid "Send me the code by email"
@@ -266,14 +273,17 @@
 
 msgid "Unknown project"
 msgstr "Nekonata projekto"
 
 msgid "Password successfully reset."
 msgstr "Pasvorto sukcese restarigita."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -782,14 +792,17 @@
 
 msgid "History"
 msgstr "Historio"
 
 msgid "Settings"
 msgstr "Agordoj"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Aliaj projektoj:"
 
 msgid "switch to"
 msgstr "salti al"
 
 msgid "Dashboard"
@@ -859,22 +872,21 @@
 
 msgid "No bills"
 msgstr "Neniu fakturo"
 
 msgid "Nothing to list yet."
 msgstr "Nenio listigebla ankoraŭ."
 
-msgid "You probably want to"
-msgstr "Vi probable volas"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "aldoni fakturon"
 
-msgid "add participants"
-msgstr "aldoni partoprenantojn"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Aldono partoprenanton"
 
 msgid "Password reminder"
 msgstr "Rememorigilo pri pasvorto"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -890,51 +902,64 @@
 
 msgid "Reset your password"
 msgstr "Restarigi vian pasvorton"
 
 msgid "Invite people to join this project"
 msgstr "Inviti homojn aliĝi al ĉi tiu projekto"
 
-msgid "Share Identifier & code"
-msgstr "Konigi identigilon kaj kodon"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
-msgstr "Vi povas iel ajn konigi la projektan identigilon kaj la privatan kodon."
-
-msgid "Identifier:"
-msgstr "Identigilo:"
-
-msgid "Share the Link"
-msgstr "Sendi la ligon"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Vi povas rekte sendi la jenan hiperligon per via preferata komunikilo"
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
+msgstr ""
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Sendi retpoŝte"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Specifu (kome apartigitan) liston de tiuj retpoŝtaj adresoj, kiujn vi "
 "volas sciigi pri la\n"
 "                kreado de ĉi tiu buĝet-administra projekto, kaj ni sendos"
 " al ili retpoŝtajn mesaĝojn por vi."
 
+msgid "Share Identifier & code"
+msgstr "Konigi identigilon kaj kodon"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identigilo:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Privata kodo"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Kiu pagas?"
 
 msgid "To whom?"
 msgstr "Al kiu?"
 
 msgid "Who?"
@@ -1092,7 +1117,25 @@
 
 #~ msgid " show"
 #~ msgstr "montri"
 
 #~ msgid "Edit the project"
 #~ msgstr "Redakti la projekton"
 
+#~ msgid "You probably want to"
+#~ msgstr "Vi probable volas"
+
+#~ msgid "add participants"
+#~ msgstr "aldoni partoprenantojn"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr "Vi povas iel ajn konigi la projektan identigilon kaj la privatan kodon."
+
+#~ msgid "Share the Link"
+#~ msgstr "Sendi la ligon"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "Vi povas rekte sendi la jenan hiperligon per via preferata komunikilo"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/es/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-11-14 05:48+0000\n"
 "Last-Translator: Sabtag3 <dioni1984@yahoo.com>\n"
 "Language: es\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/es/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Cantidad o expresión no válida. Solo se aceptan números y los operadores "
 "+ - * /."
 
 msgid "Project name"
 msgstr "Nombre del proyecto"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Nuevo código privado"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Nuevo código privado"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Ingrese un nuevo código si desea cambiarlo"
 
 msgid "Email"
@@ -48,14 +55,20 @@
 msgstr "Moneda por defecto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Establecer una moneda predeterminada permite la conversión de moneda "
 "entre facturas"
 
+msgid "Unknown error"
+msgstr "Error desconocido"
+
+msgid "Invalid private code."
+msgstr "Código privado no válido."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Este proyecto no se puede configurar como \"sin moneda\" porque contiene "
 "facturas en varias monedas."
 
@@ -87,20 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Por favor, valide el captcha para proceder."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Ingrese el código privado para confirmar la eliminación"
 
-msgid "Unknown error"
-msgstr "Error desconocido"
-
-msgid "Invalid private code."
-msgstr "Código privado no válido."
-
 msgid "Get in"
 msgstr "Entra"
 
 msgid "Admin password"
 msgstr "Contraseña de administrador"
 
 msgid "Send me the code by email"
@@ -271,14 +278,17 @@
 
 msgid "Unknown project"
 msgstr "Proyecto desconocido"
 
 msgid "Password successfully reset."
 msgstr "La contraseña se restableció correctamente."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -778,14 +788,17 @@
 
 msgid "History"
 msgstr "Historia"
 
 msgid "Settings"
 msgstr "Ajustes"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Otros proyectos :"
 
 msgid "switch to"
 msgstr "cambiar a"
 
 msgid "Dashboard"
@@ -854,22 +867,21 @@
 
 msgid "No bills"
 msgstr "Sin facturas"
 
 msgid "Nothing to list yet."
 msgstr "No hay nada que mostrar todavía."
 
-msgid "You probably want to"
-msgstr "Probablemente quieras"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "añadir una factura"
 
-msgid "add participants"
-msgstr "añadir participantes"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Añadir participante"
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -883,45 +895,57 @@
 
 msgid "Reset your password"
 msgstr "Reestablecer tu contraseña"
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
-msgstr "Compartir identificador i código"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
 
-msgid "Identifier:"
-msgstr "Identificador:"
-
-msgid "Share the Link"
-msgstr "Compartir el enlace"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
+msgstr ""
+
+msgid "Share Identifier & code"
+msgstr "Compartir identificador i código"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificador:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Código privado"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr "¿Para quién?"
@@ -1103,7 +1127,44 @@
 
 #~ msgid " show"
 #~ msgstr "mostrar"
 
 #~ msgid "Edit the project"
 #~ msgstr "Editar el proyecto"
 
+#~ msgid "You probably want to"
+#~ msgstr "Probablemente quieras"
+
+#~ msgid "add participants"
+#~ msgstr "añadir participantes"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr "Compartir el enlace"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-04-11 17:12+0000\n"
 "Last-Translator: Santiago José Gutiérrez Llanos "
 "<gutierrezapata17@gmail.com>\n"
 "Language: es_419\n"
 "Language-Team: Spanish (Latin America) "
 "<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/es_419/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
@@ -26,14 +26,21 @@
 msgstr ""
 "No es una cantidad o expresión válida. Solo se aceptan números y los "
 "operadores + - * /."
 
 msgid "Project name"
 msgstr "Nombre del Proyecto"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Nuevo código privado"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Nuevo código privado"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Entra un nuevo código si tu quieres cambiarlo"
 
 msgid "Email"
@@ -49,14 +56,20 @@
 msgstr "Moneda por defecto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Establecer una moneda predeterminada permite la conversión de divisas "
 "entre facturas"
 
+msgid "Unknown error"
+msgstr "Error desconocido"
+
+msgid "Invalid private code."
+msgstr "Código privado inválido."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Este proyecto no se puede establecer en 'ninguna moneda' porque contiene "
 "facturas en varias monedas."
 
@@ -88,20 +101,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Por favor, completa el captcha para seguir."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Introduzca el código privado para confirmar la eliminación"
 
-msgid "Unknown error"
-msgstr "Error desconocido"
-
-msgid "Invalid private code."
-msgstr "Código privado inválido."
-
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
 msgstr "Contraseña de Administrador"
 
 msgid "Send me the code by email"
@@ -272,14 +279,17 @@
 
 msgid "Unknown project"
 msgstr "Proyecto desconocido"
 
 msgid "Password successfully reset."
 msgstr "Contraseña restablecida con éxito."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -786,14 +796,17 @@
 
 msgid "History"
 msgstr "Historial"
 
 msgid "Settings"
 msgstr "Configuración"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Otros proyectos :"
 
 msgid "switch to"
 msgstr "cambiar a"
 
 msgid "Dashboard"
@@ -862,22 +875,21 @@
 
 msgid "No bills"
 msgstr "Sin facturas"
 
 msgid "Nothing to list yet."
 msgstr "Aún no hay nada que listar."
 
-msgid "You probably want to"
-msgstr "Probablemente quieras"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "agregar una factura"
 
-msgid "add participants"
-msgstr "agregar participantes"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Editar este participante"
 
 msgid "Password reminder"
 msgstr "Recordar contraseña"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -893,55 +905,64 @@
 
 msgid "Reset your password"
 msgstr "Restablecer su contraseña"
 
 msgid "Invite people to join this project"
 msgstr "Invita a personas a unirse a este proyecto"
 
-msgid "Share Identifier & code"
-msgstr "Compartir identificador y código"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Puede compartir el identificador del proyecto y el código privado por "
-"cualquier medio de comunicación."
 
-msgid "Identifier:"
-msgstr "Identificador:"
-
-msgid "Share the Link"
-msgstr "Comparte el enlace"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Puedes compartir directamente el siguiente enlace a través de tu medio "
-"preferido"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Enviar por correo electrónico"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Especifique una lista (separada por comas) de las direcciones de correo "
 "electrónico a las que desea notificar acerca de la\n"
 "creación de este proyecto de gestión presupuestaria y les enviaremos un "
 "correo electrónico para usted."
 
+msgid "Share Identifier & code"
+msgstr "Compartir identificador y código"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificador:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Código privado"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "¿Quién paga?"
 
 msgid "To whom?"
 msgstr "¿A quién?"
 
 msgid "Who?"
@@ -1122,7 +1143,31 @@
 
 #~ msgid " show"
 #~ msgstr "enseñar"
 
 #~ msgid "Edit the project"
 #~ msgstr "Editar el proyecto"
 
+#~ msgid "You probably want to"
+#~ msgstr "Probablemente quieras"
+
+#~ msgid "add participants"
+#~ msgstr "agregar participantes"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Puede compartir el identificador del "
+#~ "proyecto y el código privado por "
+#~ "cualquier medio de comunicación."
+
+#~ msgid "Share the Link"
+#~ msgstr "Comparte el enlace"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Puedes compartir directamente el siguiente "
+#~ "enlace a través de tu medio "
+#~ "preferido"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-03-19 21:40+0000\n"
 "Last-Translator: Sai Mohammad-Hossein Emami <emami@outlook.com>\n"
 "Language: fa\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/fa/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
@@ -23,14 +23,21 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "مقدار یا عبارت نامعتبر. فقط اعداد و عملیات‌های + - * / مجاز هستند."
 
 msgid "Project name"
 msgstr "نام پروژه"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "کد خصوصی جدید"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "کد خصوصی جدید"
 
 msgid "Enter a new code if you want to change it"
 msgstr "اگر مایل به تغییر هستید یه کد جدید وارد کنید"
 
 msgid "Email"
@@ -44,14 +51,20 @@
 
 msgid "Default Currency"
 msgstr "واحد پولی پیش فرض"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "تنظیم واحد پولی پیش فرض امکان تبدیل ارز بین قبض‌ها رو فراهم می‌کنه"
 
+msgid "Unknown error"
+msgstr "خطای ناشناخته"
+
+msgid "Invalid private code."
+msgstr "کد خصوصی نامعتبر."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "این پروژه نمی‌تونه به صورت «بدون واحد پولی» تنظیم بشه چون شامل قبوض با "
 "ارزهای مختلفه."
 
@@ -83,20 +96,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "لطفا برای ادامه کپچا رو تایید کن."
 
 msgid "Enter private code to confirm deletion"
 msgstr "کد خصوصی رو برای تایید حذف وارد کن"
 
-msgid "Unknown error"
-msgstr "خطای ناشناخته"
-
-msgid "Invalid private code."
-msgstr "کد خصوصی نامعتبر."
-
 msgid "Get in"
 msgstr "بیا تو"
 
 msgid "Admin password"
 msgstr "گذرواژه‌ی مدیر"
 
 msgid "Send me the code by email"
@@ -252,14 +259,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -743,14 +753,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -819,21 +832,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -848,45 +858,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "کد خصوصی"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1027,7 +1049,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -64,14 +64,20 @@
 
 msgid "Add a new bill"
 msgstr "Nouvelle facture"
 
 msgid "Add participant"
 msgstr "Ajouter un⋅e participant⋅e"
 
+msgid "Add the first participant"
+msgstr "Ajouter le premier participant ou la première participante"
+
+msgid "Add your first bill"
+msgstr "Ajouter votre première facture"
+
 msgid "Added on %(date)s"
 msgstr "Ajouté le %(date)s"
 
 msgid "Admin password"
 msgstr "Mot de passe administrateur⋅ice"
 
 msgid "Administation Dashboard"
@@ -188,14 +194,17 @@
 
 msgid "Create the project"
 msgstr "Créer le projet"
 
 msgid "Currency"
 msgstr "Devise"
 
+msgid "Current private code"
+msgstr "Code d’accès actuel"
+
 msgid "Dashboard"
 msgstr "Tableau de bord"
 
 msgid "Date"
 msgstr "Date"
 
 msgid "Default Currency"
@@ -277,14 +286,17 @@
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr "Activer l'historique du projet et l’enregistrement des adresses IP"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Entrez un nouveau code si vous souhaitez le changer"
 
+msgid "Enter existing private code to edit project"
+msgstr "Entrez le code d'accès existant pour éditer le projet"
+
 msgid "Enter private code to confirm deletion"
 msgstr "Entrez le code d'accès pour confirmer la suppression"
 
 msgid "Error activating participant"
 msgstr "Erreur lors de l'activation de ce⋅tte participant⋅e"
 
 msgid "Error deleting bill"
@@ -545,14 +557,17 @@
 
 msgid "Privacy Settings"
 msgstr "Vie privée"
 
 msgid "Private code"
 msgstr "Code d’accès"
 
+msgid "Private code:"
+msgstr "Code d’accès :"
+
 msgid "Project"
 msgstr "Projet"
 
 msgid "Project %(name)s added"
 msgstr "Projet %(name)s ajouté"
 
 msgid "Project %(name)s changed in an unknown way"
@@ -572,14 +587,17 @@
 
 msgid "Project private code changed"
 msgstr "Le mot de passe du projet a été modifié"
 
 msgid "Project renamed to %(new_project_name)s"
 msgstr "Projet renommé en %(new_project_name)s"
 
+msgid "Project settings have been changed successfully."
+msgstr "Les paramètres du projet ont bien été enregistrés."
+
 msgid "Project settings modified"
 msgstr "Les paramètres du projet ont été modifiés"
 
 msgid "Project successfully deleted"
 msgstr "Projet supprimé"
 
 msgid "Project successfully uploaded"
@@ -587,14 +605,17 @@
 
 msgid "Projects"
 msgstr "Projets"
 
 msgid "Provided token is invalid"
 msgstr "Ce jeton est invalide"
 
+msgid "RSS Feed"
+msgstr "Flux RSS"
+
 msgid "Reset password"
 msgstr "Réinitialiser le mot de passe"
 
 msgid "Reset your password"
 msgstr "Changez votre code d'accès"
 
 msgid "Return to home page"
@@ -628,16 +649,16 @@
 
 msgid "Settle plans"
 msgstr "Remboursements"
 
 msgid "Share Identifier & code"
 msgstr "Partager l'identifiant et le code"
 
-msgid "Share the Link"
-msgstr "Partagez le lien"
+msgid "Share an invitation link"
+msgstr "Partager un lien d'invitation"
 
 msgid "Simple operations are allowed, e.g. (18+36.2)/3"
 msgstr "Les opérations simples sont possibles, par exemple (18+36.2)/3"
 
 msgid "Simply sharing money with others?"
 msgstr "Ça vous arrive de partager de l’argent avec d’autres ?"
 
@@ -662,21 +683,21 @@
 msgstr ""
 "Désolé, une erreur s’est produite lors de l’envoi du courriel d’invitation."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Désolé, nous ne trouvons pas la page demandée."
 
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify about "
-"the\n"
-"                creation of this budget management project and we will send "
-"them an email for you."
-msgstr ""
-"Entrez les emails des personnes avec qui vous souhaitez partager ce projet, "
-"nous leur enverrons un lien d'invitation."
+"Specify a list of email adresses (separated by comma) of people you want to "
+"notify about the creation of this project. We will send them an email with "
+"the invitation link."
+msgstr ""
+"Entrez les emails des personnes avec qui vous souhaitez partager ce projet "
+"(en séparant les adresses emails avec des virgules). Nous leur enverrons un "
+"mail avec le lien d'invitation."
 
 msgid "Spent"
 msgstr "A dépensé"
 
 msgid "Start a new project"
 msgstr "Nouveau projet"
 
@@ -700,14 +721,26 @@
 
 msgid "The bill has been deleted"
 msgstr "La facture a été supprimée"
 
 msgid "The bill has been modified"
 msgstr "La facture a été modifiée"
 
+msgid ""
+"The easiest way to invite people is to give them the following invitation "
+"link.<br />They will be able to access the project, manage participants, add/"
+"edit/delete bills. However, they will not have access to important settings "
+"such as changing the private code or deleting the whole project."
+msgstr ""
+"Pour inviter des personnes dans ce projet, vous pouvez leur donner le lien "
+"d'invitation ci-dessous.<br />Elles pourront ainsi accéder au projet, gérer "
+"les participants, ajouter/modifier/supprimer des factures. En revanche, "
+"elles ne pourront pas modifier des paramètres importants tels que le code "
+"d'accès ou supprimer le projet."
+
 msgid "The email %(email)s is not valid"
 msgstr "L’email %(email)s est invalide"
 
 msgid "The participant name is invalid"
 msgstr "Le nom du participant est incorrect"
 
 msgid "The project you are trying to access do not exist, do you want to"
@@ -811,54 +844,46 @@
 
 msgid "Who?"
 msgstr "Qui ?"
 
 msgid "You can clear the project history to remove them."
 msgstr "Vous pouvez supprimer l'historique du projet pour les enlever."
 
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Vous pouvez directement partager le lien suivant"
-
 msgid "You can enable history on the settings page."
 msgstr "Vous pouvez activer l'historique dans les paramètres."
 
 msgid ""
 "You can share the project identifier and the private code by any "
-"communication means."
-msgstr ""
-"Vous pouvez partager l'identifiant de ce projet et le code d'accès par "
-"d'autres moyens."
+"communication means.<br />Anyone with the private code will have access to "
+"the full project, including changing settings such as the private code or "
+"project email address, or even deleting the whole project."
+msgstr ""
+"Vous pouvez partager l'identifiant de ce projet et le code d'accès par tout "
+"moyen de votre choix.<br />Une personne possédant le code d'accès aura un "
+"accès complet au projet, y compris pour changer le code d'accès ou l'adresse "
+"email associée au projet, voire même supprimer complètement le projet."
 
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Vous avez été invité⋅e à partager vos dépenses pour %(project)s"
 
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "Vous venez de créer « %(project)s » pour partager vos dépenses"
 
-msgid "You probably want to"
-msgstr "Vous souhaitez sûrement"
-
 msgid "You should start by adding participants"
 msgstr "Vous devriez commencer par ajouter des participant⋅es"
 
 msgid "You're sharing a house?"
 msgstr "Vous êtes en colocation ?"
 
 msgid "Your invitations have been sent"
 msgstr "Vos invitations ont bien été envoyées"
 
 msgid "Your projects"
 msgstr "Vos projets"
 
-msgid "add a bill"
-msgstr "ajouter une facture"
-
-msgid "add participants"
-msgstr "ajouter des participant⋅es"
-
 msgid "can't remember your password?"
 msgstr "Code d’accès oublié ?"
 
 msgid "create it"
 msgstr "le créer"
 
 msgid "deactivate"
@@ -881,14 +906,17 @@
 
 msgid "show"
 msgstr "voir"
 
 msgid "switch to"
 msgstr "aller à"
 
+msgid "the private code was defined when you created the project"
+msgstr "le code d'accès a été défini lorsque vous avez créé le projet"
+
 msgid "you can contribute and improve it!"
 msgstr "vous pouvez y contribuer et l’améliorer !"
 
 msgid "you sure?"
 msgstr "vous confirmez ?"
 
 msgid "{dual_object_0} and {dual_object_1}"
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is distributed under the same license as the PROJECT project.
 # Alexis Métaireau <alexis@notmyidea.org>, 2011.
 # Adrien CLERC, 2018.
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
-"PO-Revision-Date: 2023-07-15 08:51+0000\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
+"PO-Revision-Date: 2023-07-29 13:07+0000\n"
 "Last-Translator: Baptiste <weblate@bitsofnetworks.org>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -30,14 +30,20 @@
 msgstr ""
 "Ceci n'est pas un montant ou une expression valide. Seuls les nombres et "
 "les opérateurs + - * / sont acceptés."
 
 msgid "Project name"
 msgstr "Nom de projet"
 
+msgid "Current private code"
+msgstr "Code d’accès actuel"
+
+msgid "Enter existing private code to edit project"
+msgstr "Entrez le code d'accès existant pour éditer le projet"
+
 msgid "New private code"
 msgstr "Nouveau code d’accès"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Entrez un nouveau code si vous souhaitez le changer"
 
 msgid "Email"
@@ -53,14 +59,20 @@
 msgstr "Devise par défaut"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Choisir une devise par défaut permet d'activer la conversion de devises "
 "entre les factures"
 
+msgid "Unknown error"
+msgstr "Erreur inconnue"
+
+msgid "Invalid private code."
+msgstr "Code d’accès invalide."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Ce projet ne peut pas être sans devise car il contient des factures "
 "utilisant des devises différentes."
 
@@ -92,20 +104,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Merci de valider le captcha avant de continuer."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Entrez le code d'accès pour confirmer la suppression"
 
-msgid "Unknown error"
-msgstr "Erreur inconnue"
-
-msgid "Invalid private code."
-msgstr "Code d’accès invalide."
-
 msgid "Get in"
 msgstr "Entrer"
 
 msgid "Admin password"
 msgstr "Mot de passe administrateur⋅ice"
 
 msgid "Send me the code by email"
@@ -270,14 +276,17 @@
 
 msgid "Unknown project"
 msgstr "Projet inconnu"
 
 msgid "Password successfully reset."
 msgstr "Le mot de passe a été changé avec succès."
 
+msgid "Project settings have been changed successfully."
+msgstr "Les paramètres du projet ont bien été enregistrés."
+
 msgid "Unable to parse CSV"
 msgstr "Erreur lors de la lecture du fichier CSV"
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr "Attribut manquant : %(attribute)s"
 
@@ -786,14 +795,17 @@
 
 msgid "History"
 msgstr "Historique"
 
 msgid "Settings"
 msgstr "Options"
 
+msgid "RSS Feed"
+msgstr "Flux RSS"
+
 msgid "Other projects :"
 msgstr "Autres projets :"
 
 msgid "switch to"
 msgstr "aller à"
 
 msgid "Dashboard"
@@ -862,22 +874,19 @@
 
 msgid "No bills"
 msgstr "Pas encore de factures"
 
 msgid "Nothing to list yet."
 msgstr "Rien à lister pour le moment."
 
-msgid "You probably want to"
-msgstr "Vous souhaitez sûrement"
-
-msgid "add a bill"
-msgstr "ajouter une facture"
+msgid "Add your first bill"
+msgstr "Ajouter votre première facture"
 
-msgid "add participants"
-msgstr "ajouter des participant⋅es"
+msgid "Add the first participant"
+msgstr "Ajouter le premier participant ou la première participante"
 
 msgid "Password reminder"
 msgstr "Rappel du code d’accès"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -893,50 +902,70 @@
 
 msgid "Reset your password"
 msgstr "Changez votre code d'accès"
 
 msgid "Invite people to join this project"
 msgstr "Invitez des personnes à rejoindre ce projet"
 
-msgid "Share Identifier & code"
-msgstr "Partager l'identifiant et le code"
+msgid "Share an invitation link"
+msgstr "Partager un lien d'invitation"
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
-msgstr ""
-"Vous pouvez partager l'identifiant de ce projet et le code d'accès par "
-"d'autres moyens."
-
-msgid "Identifier:"
-msgstr "Identifiant :"
-
-msgid "Share the Link"
-msgstr "Partagez le lien"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Vous pouvez directement partager le lien suivant"
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
+msgstr ""
+"Pour inviter des personnes dans ce projet, vous pouvez leur donner le "
+"lien d'invitation ci-dessous.<br />Elles pourront ainsi accéder au "
+"projet, gérer les participants, ajouter/modifier/supprimer des factures. "
+"En revanche, elles ne pourront pas modifier des paramètres importants "
+"tels que le code d'accès ou supprimer le projet."
 
 msgid "Scan QR code"
 msgstr "Scannez le QR code"
 
 msgid "Use a mobile device with a compatible app."
 msgstr "Utilisez un appareil mobile avec une application compatible."
 
 msgid "Send via Emails"
 msgstr "Envoyer par email(s)"
 
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
+msgstr ""
+"Entrez les emails des personnes avec qui vous souhaitez partager ce projet ("
+"en séparant les adresses emails avec des virgules). Nous leur enverrons un "
+"mail avec le lien d'invitation."
+
+msgid "Share Identifier & code"
+msgstr "Partager l'identifiant et le code"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
-"Entrez les emails des personnes avec qui vous souhaitez partager ce "
-"projet, nous leur enverrons un lien d'invitation."
+"Vous pouvez partager l'identifiant de ce projet et le code d'accès par "
+"tout moyen de votre choix.<br />Une personne possédant le code d'accès "
+"aura un accès complet au projet, y compris pour changer le code d'accès "
+"ou l'adresse email associée au projet, voire même supprimer complètement "
+"le projet."
+
+msgid "Identifier:"
+msgstr "Identifiant :"
+
+msgid "Private code:"
+msgstr "Code d’accès :"
+
+msgid "the private code was defined when you created the project"
+msgstr "le code d'accès a été défini lorsque vous avez créé le projet"
 
 msgid "Who pays?"
 msgstr "Qui doit payer ?"
 
 msgid "To whom?"
 msgstr "Pour qui ?"
 
@@ -1334,7 +1363,28 @@
 #~ msgstr "Envoyer les invitations"
 
 #~ msgid " show"
 #~ msgstr "voir"
 
 #~ msgid "Edit the project"
 #~ msgstr "Éditer le projet"
+
+#~ msgid "You probably want to"
+#~ msgstr "Vous souhaitez sûrement"
+
+#~ msgid "add participants"
+#~ msgstr "ajouter des participant⋅es"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Vous pouvez partager l'identifiant de ce"
+#~ " projet et le code d'accès par "
+#~ "d'autres moyens."
+
+#~ msgid "Share the Link"
+#~ msgstr "Partagez le lien"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "Vous pouvez directement partager le lien suivant"
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/he/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -46,17 +46,23 @@
 
 msgid "Actions"
 msgstr "פעולות"
 
 msgid "Add"
 msgstr "הוסף"
 
+msgid "Add a bill"
+msgstr "הוסף חשבון"
+
 msgid "Add a new bill"
 msgstr "הוסף הוצאה חדשה"
 
+msgid "Add participant"
+msgstr "הוסף משתתפים"
+
 msgid "Added on %(date)s"
 msgstr "נוסף בתאריך %(date)s"
 
 msgid "Admin password"
 msgstr "סיסמת מנהל"
 
 msgid "Administration tasks are currently disabled."
@@ -101,20 +107,32 @@
 
 msgid "Delete project"
 msgstr "מחק פרויקט"
 
 msgid "Deleted project history."
 msgstr "הסטוריית הפרויקט נמחקה."
 
+msgid "Disabled Project History"
+msgstr "היסטורית פרויקט מושבתת"
+
 msgid "Documentation"
 msgstr "דוקומנטציה"
 
+msgid "Download"
+msgstr "הורד"
+
 msgid "Download Mobile Application"
 msgstr "הורד אפליקציית מובייל"
 
+msgid "Edit this bill"
+msgstr "ערוך את החשבון"
+
+msgid "Edit this participant"
+msgstr "ערוך את המשתתף"
+
 msgid "Email"
 msgstr "דוא\"ל"
 
 msgid "Enable project history"
 msgstr "אפשר היסטוריית פרויקט"
 
 msgid "Enter a new code if you want to change it"
@@ -131,14 +149,17 @@
 
 msgid "Error deleting project history"
 msgstr "שגיאה במחיקת הסטוריית הפרויקט"
 
 msgid "Event"
 msgstr "אירוע"
 
+msgid "Everyone"
+msgstr "כולם"
+
 msgid "Expenses by Month"
 msgstr "הוצאות לפי חודש"
 
 msgid "External link"
 msgstr "קישור חיצוני"
 
 msgid "For what?"
@@ -197,14 +218,17 @@
 
 msgid "Missing attribute: %(attribute)s"
 msgstr "תכונה חסרה:%(attribute)s"
 
 msgid "Mobile Application"
 msgstr "יישום לנייד"
 
+msgid "More options"
+msgstr "יותר אפשרויות"
+
 msgid "Name"
 msgstr "שם"
 
 msgid "New private code"
 msgstr "קוד פרטי חדש"
 
 msgid "Newest bill"
@@ -212,14 +236,17 @@
 
 msgid "No Currency"
 msgstr "ללא מטבע"
 
 msgid "No bills"
 msgstr "אין הוצאות"
 
+msgid "No one"
+msgstr "אף אחד"
+
 msgid "No token provided"
 msgstr "טוקן לא הוזן"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "כמות או ביטוי לא תקין. יש להזין רק מספרים וסימני הפעולה + - * /."
@@ -482,14 +509,17 @@
 
 msgid "edit"
 msgstr "ערוך"
 
 msgid "euro"
 msgstr "אירו"
 
+msgid "john.doe@example.com, mary.moe@site.com"
+msgstr "john.doe@example.com, mary.moe@site.com"
+
 msgid "switch to"
 msgstr "שנה ל"
 
 msgid "you can contribute and improve it!"
 msgstr "אתה יכול לתרום ולשפר אותו!"
 
 msgid "you sure?"
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/he/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
-"PO-Revision-Date: 2023-07-22 14:03+0000\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
+"PO-Revision-Date: 2023-07-24 07:07+0000\n"
 "Last-Translator: Nati Lintzer <nlintzer@gmail.com>\n"
-"Language-Team: Hebrew <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/he/>\n"
 "Language: he\n"
+"Language-Team: Hebrew <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/he/>\n"
+"Plural-Forms: nplurals=4; plural=(n == 1) ? 0 : ((n == 2) ? 1 : ((n > 10 "
+"&& n % 10 == 0) ? 2 : 3))\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1) ? 0 : ((n == 2) ? 1 : ((n > 10 && "
-"n % 10 == 0) ? 2 : 3));\n"
-"X-Generator: Weblate 5.0-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "יצרת את פרויקט '%(project)s' כדי לחלוק את הוצאותיך"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "כמות או ביטוי לא תקין. יש להזין רק מספרים וסימני הפעולה + - * /."
 
 msgid "Project name"
 msgstr "שם הפרויקט"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "קוד פרטי חדש"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "קוד פרטי חדש"
 
 msgid "Enter a new code if you want to change it"
 msgstr "הזן.י קוד חדש אם תרצה.י לשנות את הקוד"
 
 msgid "Email"
@@ -45,14 +52,20 @@
 
 msgid "Default Currency"
 msgstr "מטבע ברירת המחדל"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "בחירת מטבע ברירת מחדל מאפשרת המרת מטבע בין חשבונות"
 
+msgid "Unknown error"
+msgstr "שגיאה לא ידועה"
+
+msgid "Invalid private code."
+msgstr "קוד פרטי לא תקין."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "בפרויקט זה לא ניתן להגדיר 'ללא מטבע' מכיוון שהוא כולל חשבונות במספר "
 "מטבעות."
 
@@ -82,20 +95,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "אנא אמת את ה-Captcha כדי להמשיך."
 
 msgid "Enter private code to confirm deletion"
 msgstr "הזן את הקוד הפרטי כדי לאשר מחיקה"
 
-msgid "Unknown error"
-msgstr "שגיאה לא ידועה"
-
-msgid "Invalid private code."
-msgstr "קוד פרטי לא תקין."
-
 msgid "Get in"
 msgstr "היכנס"
 
 msgid "Admin password"
 msgstr "סיסמת מנהל"
 
 msgid "Send me the code by email"
@@ -185,16 +192,16 @@
 msgstr ""
 
 #, python-format
 msgid ""
 "Please check the email configuration of the server or contact the "
 "administrator: %(admin_email)s"
 msgstr ""
-"מצטערים, אך אירעה שגיאה בעת ששלחנו לכם את המייל עם הוראות איפוס הסיסמה. אנא "
-"בדקו את הגדרות המייל בשרת או פנו למנהל השרת:%(admin_email)s"
+"מצטערים, אך אירעה שגיאה בעת ששלחנו לכם את המייל עם הוראות איפוס הסיסמה. "
+"אנא בדקו את הגדרות המייל בשרת או פנו למנהל השרת:%(admin_email)s"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} ו- {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
@@ -258,14 +265,17 @@
 
 msgid "Unknown project"
 msgstr "פרויקט לא ידוע"
 
 msgid "Password successfully reset."
 msgstr "הסיסמה אופסה בהצלחה."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr "תכונה חסרה:%(attribute)s"
 
@@ -455,45 +465,45 @@
 msgid "Import previously exported project"
 msgstr "ייבא פרוייקט קודם מיוצא"
 
 msgid "Choose file"
 msgstr "בחר קובץ"
 
 msgid "Edit this bill"
-msgstr ""
+msgstr "ערוך את החשבון"
 
 msgid "Add a bill"
-msgstr ""
+msgstr "הוסף חשבון"
 
 msgid "Simple operations are allowed, e.g. (18+36.2)/3"
 msgstr ""
 
 msgid "Everyone"
-msgstr ""
+msgstr "כולם"
 
 msgid "No one"
-msgstr ""
+msgstr "אף אחד"
 
 msgid "More options"
-msgstr ""
+msgstr "יותר אפשרויות"
 
 msgid "Add participant"
-msgstr ""
+msgstr "הוסף משתתפים"
 
 msgid "Edit this participant"
-msgstr ""
+msgstr "ערוך את המשתתף"
 
 msgid "john.doe@example.com, mary.moe@site.com"
-msgstr ""
+msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "Download"
-msgstr ""
+msgstr "הורד"
 
 msgid "Disabled Project History"
-msgstr ""
+msgstr "היסטורית פרויקט מושבתת"
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr ""
 
 msgid "Enabled Project History"
 msgstr ""
 
@@ -749,14 +759,17 @@
 
 msgid "History"
 msgstr "הסטוריה"
 
 msgid "Settings"
 msgstr "הגדרות"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "פרויקטים אחרים:"
 
 msgid "switch to"
 msgstr "שנה ל"
 
 msgid "Dashboard"
@@ -825,22 +838,20 @@
 
 msgid "No bills"
 msgstr "אין הוצאות"
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr "אתה כנראה רוצה"
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
-msgstr "הוסף משתמשים"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "ערוך את המשתתף"
 
 msgid "Password reminder"
 msgstr "תזכורת סיסמה"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -854,45 +865,57 @@
 
 msgid "Reset your password"
 msgstr "אפס את סיסמתך"
 
 msgid "Invite people to join this project"
 msgstr "הזמן אנשים להצטרף לפרויקט"
 
-msgid "Share Identifier & code"
-msgstr "שתף מזהה וקוד"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
-msgstr "אתה יכול לשתף את מזהה הפרויקט והקוד הפרטי באמצעות כל אמצעי תקשורת."
-
-msgid "Identifier:"
-msgstr "מזהה:"
-
-msgid "Share the Link"
-msgstr "שתף את הלינק"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "אתה יכול לשתף ישירות את הלינק באמצעי המועדף עליך"
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
+msgstr ""
 
 msgid "Scan QR code"
 msgstr "סרוק את הברקוד"
 
 msgid "Use a mobile device with a compatible app."
 msgstr "השתמש במכשיר נייד עם יישום תואם."
 
 msgid "Send via Emails"
 msgstr "שלח באמצעות דוא\"ל"
 
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
+msgstr ""
+
+msgid "Share Identifier & code"
+msgstr "שתף מזהה וקוד"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "מזהה:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "קוד פרטי"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr "מי משלם?"
 
 msgid "To whom?"
 msgstr "למי?"
@@ -976,7 +999,48 @@
 #~ msgstr "שלח הזמנות"
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
+
+#~ msgid "You probably want to"
+#~ msgstr "אתה כנראה רוצה"
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr "הוסף משתמשים"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr "אתה יכול לשתף את מזהה הפרויקט והקוד הפרטי באמצעות כל אמצעי תקשורת."
+
+#~ msgid "Share the Link"
+#~ msgstr "שתף את הלינק"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "אתה יכול לשתף ישירות את הלינק באמצעי המועדף עליך"
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2020-06-14 14:41+0000\n"
 "Last-Translator: raghupalash <singhpalash0@gmail.com>\n"
 "Language: hi\n"
 "Language-Team: Hindi <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/hi/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
@@ -26,14 +26,21 @@
 "वैध राशि या चिह्न नहीं। केवल संख्या और + - * / ऑपरेटरों को स्वीकार किया "
 "जाता है।"
 
 msgid "Project name"
 msgstr "परियोजना का नाम"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "निजी कोड"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "निजी कोड"
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -47,14 +54,22 @@
 
 msgid "Default Currency"
 msgstr "डिफ़ॉल्ट मुद्रा"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+#, fuzzy
+msgid "Unknown error"
+msgstr "अज्ञात परियोजना"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "निजी कोड"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -85,22 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "अज्ञात परियोजना"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "निजी कोड"
-
 msgid "Get in"
 msgstr "अंदर जाइये"
 
 msgid "Admin password"
 msgstr "व्यवस्थापक पासवर्ड"
 
 msgid "Send me the code by email"
@@ -267,14 +274,17 @@
 
 msgid "Unknown project"
 msgstr "अज्ञात परियोजना"
 
 msgid "Password successfully reset."
 msgstr "पासवर्ड सफलतापूर्वक रीसेट हो गया है।"
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -790,14 +800,17 @@
 
 msgid "History"
 msgstr "इतिहास"
 
 msgid "Settings"
 msgstr "सेटिंग्स"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "अन्य परियोजनाएँ :"
 
 msgid "switch to"
 msgstr "पर स्विच करें"
 
 msgid "Dashboard"
@@ -867,22 +880,21 @@
 
 msgid "No bills"
 msgstr "कोई बिल नहीं"
 
 msgid "Nothing to list yet."
 msgstr "सूचि बनाने के लिए कुछ नहीं।"
 
-msgid "You probably want to"
-msgstr "आप शायद यह करना चाहते हैं"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "बिल जोड़ें"
 
-msgid "add participants"
-msgstr "प्रतिभागियों को जोड़ें"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "प्रतिभागी जोड़ें"
 
 msgid "Password reminder"
 msgstr "पासवर्ड अनुस्मारक"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -898,53 +910,64 @@
 
 msgid "Reset your password"
 msgstr "अपना पासवर्ड रीसेट करें"
 
 msgid "Invite people to join this project"
 msgstr "इस परियोजना से जुड़ने के लिए लोगों को आमंत्रित करें"
 
-msgid "Share Identifier & code"
-msgstr "पहचानकर्ता और कोड साझा करें"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"आप किसी भी संचार माध्यम से परियोजना पहचानकर्ता और निजी कोड साझा कर सकते "
-"हैं।"
-
-msgid "Identifier:"
-msgstr "पहचानकर्ता:"
-
-msgid "Share the Link"
-msgstr "लिंक साझा करें"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "आप नीचे दिए गए लिंक को सीधे अपने पसंदीदा माध्यम से साझा कर सकते हैं"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "ईमेल के माध्यम से भेजें"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "उन ईमेल पतों की एक (अल्पविराम से अलग की गयी) सूची निर्दिष्ट करें जिन्हे "
 "आप इस \n"
 "\t\t   बजट प्रबंधन परियोजना के निर्माण के बारे में सूचित करना चाहते हैं "
 "और हम उन्हें आपके लिए एक ईमेल भेजेंगे।"
 
+msgid "Share Identifier & code"
+msgstr "पहचानकर्ता और कोड साझा करें"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "पहचानकर्ता:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "निजी कोड"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "किसे भुगतान करना है?"
 
 msgid "To whom?"
 msgstr "किसको?"
 
 msgid "Who?"
@@ -1106,7 +1129,28 @@
 
 #~ msgid " show"
 #~ msgstr "प्रदर्शन"
 
 #~ msgid "Edit the project"
 #~ msgstr "प्रोजेक्ट संपादित करें"
 
+#~ msgid "You probably want to"
+#~ msgstr "आप शायद यह करना चाहते हैं"
+
+#~ msgid "add participants"
+#~ msgstr "प्रतिभागियों को जोड़ें"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "आप किसी भी संचार माध्यम से "
+#~ "परियोजना पहचानकर्ता और निजी कोड साझा "
+#~ "कर सकते हैं।"
+
+#~ msgid "Share the Link"
+#~ msgstr "लिंक साझा करें"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "आप नीचे दिए गए लिंक को सीधे अपने पसंदीदा माध्यम से साझा कर सकते हैं"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/hu/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-04-19 11:51+0000\n"
 "Last-Translator: Gergely Kocsis <koger23@gmail.com>\n"
 "Language: hu\n"
 "Language-Team: Hungarian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/hu/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Érvénytelen mennyiség vagy kifejezés. Csak számok és műveleti jelek ( + -"
 " * /) megengedettek."
 
 msgid "Project name"
 msgstr "A projekt neve"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Új titkos kód"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Új titkos kód"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Adj meg egy új kódot, ha meg akarod változtatni"
 
 msgid "Email"
@@ -48,14 +55,20 @@
 msgstr "Alapértelmezett Pénznem"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Alapértelmezett pénznem beállítása lehetővé teszi a számlák közötti "
 "pénzváltást"
 
+msgid "Unknown error"
+msgstr "Ismeretlen hiba"
+
+msgid "Invalid private code."
+msgstr "Érvénytelen titkos kód."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "A projekt nem állítható pénznem nélkülire, mert számlákat és több "
 "pénznemet is tartalmaz."
 
@@ -87,20 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Kérlek validáld a captcha-t a folytatáshoz."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Add meg a titkos kódot a törlés megerősítéséhez"
 
-msgid "Unknown error"
-msgstr "Ismeretlen hiba"
-
-msgid "Invalid private code."
-msgstr "Érvénytelen titkos kód."
-
 #, fuzzy
 msgid "Get in"
 msgstr "Szállj be"
 
 msgid "Admin password"
 msgstr "Adminisztrátori jelszó"
 
@@ -260,14 +267,17 @@
 
 msgid "Unknown project"
 msgstr "Ismeretlen projekt"
 
 msgid "Password successfully reset."
 msgstr "Jelszó sikeresen visszaállítva."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -752,14 +762,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -828,21 +841,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -857,45 +867,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Titkos kód"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -988,7 +1010,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/id/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-04-11 17:12+0000\n"
 "Last-Translator: Santiago José Gutiérrez Llanos "
 "<gutierrezapata17@gmail.com>\n"
 "Language: id\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/id/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -26,14 +26,21 @@
 msgstr ""
 "Bukan jumlah atau operator yang valid. Hanya angka dan operator + -* / "
 "yang diterima."
 
 msgid "Project name"
 msgstr "Nama proyek"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Kode pribadi baru"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Kode pribadi baru"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Masukkan sebuah kode baru jika Anda ingin menggantinya"
 
 msgid "Email"
@@ -47,14 +54,20 @@
 
 msgid "Default Currency"
 msgstr "Mata Uang Standar"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "Menetapkan mata uang default memungkinkan konversi mata uang antar tagihan"
 
+msgid "Unknown error"
+msgstr "Kesalahan tidak diketahui"
+
+msgid "Invalid private code."
+msgstr "Kode pribadi tidak valid."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Proyek ini tidak dapat disetel ke 'tanpa mata uang' karena berisi tagihan"
 " dalam berbagai mata uang."
 
@@ -86,20 +99,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Mohon, silahkan validasi captcha untuk melanjutkan."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Masukkan kode pribadi untuk mengkonfirmasi penghapusan"
 
-msgid "Unknown error"
-msgstr "Kesalahan tidak diketahui"
-
-msgid "Invalid private code."
-msgstr "Kode pribadi tidak valid."
-
 msgid "Get in"
 msgstr "Masuk"
 
 msgid "Admin password"
 msgstr "Kata sandi admin"
 
 msgid "Send me the code by email"
@@ -264,14 +271,17 @@
 
 msgid "Unknown project"
 msgstr "Proyek tidak diketahui"
 
 msgid "Password successfully reset."
 msgstr "Kata sandi berhasil diatur ulang."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -773,14 +783,17 @@
 
 msgid "History"
 msgstr "Riwayat"
 
 msgid "Settings"
 msgstr "Pengaturan"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Proyek lainnya:"
 
 msgid "switch to"
 msgstr "ganti ke"
 
 msgid "Dashboard"
@@ -849,22 +862,21 @@
 
 msgid "No bills"
 msgstr "Tidak ada tagihan"
 
 msgid "Nothing to list yet."
 msgstr "Belum ada untuk didaftarkan."
 
-msgid "You probably want to"
-msgstr "Anda mungkin menginginkan"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "tambah tagihan"
 
-msgid "add participants"
-msgstr "tambah partisipan"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Sunting anggota ini"
 
 msgid "Password reminder"
 msgstr "Pengingat kata sandi"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -880,55 +892,64 @@
 
 msgid "Reset your password"
 msgstr "Atur ulang kata sandi Anda"
 
 msgid "Invite people to join this project"
 msgstr "Undang orang untuk bergabung dalam proyek ini"
 
-msgid "Share Identifier & code"
-msgstr "Bagikan ID & kode"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Anda bisa membagikan ID proyek dan kode pribadi dengan cara komunikasi "
-"apapun."
 
-msgid "Identifier:"
-msgstr "ID:"
-
-msgid "Share the Link"
-msgstr "Bagikan tautan"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Anda bisa membagikan tautan secara langsung melalui media yang Anda "
-"inginkan"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Kirim melalui surel"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Spesifikkan daftar alamat surel (dipisah dengan koma) yang akan Anda "
 "kirim pemberitahuan tentang\n"
 "                pembuatan dari manajemen anggaran proyek ini dan kami "
 "akan memngirim mereka sebuah surel."
 
+msgid "Share Identifier & code"
+msgstr "Bagikan ID & kode"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "ID:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Kode pribadi"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Siapa membayar?"
 
 msgid "To whom?"
 msgstr "Kepada siapa?"
 
 msgid "Who?"
@@ -1117,7 +1138,31 @@
 
 #~ msgid " show"
 #~ msgstr "tampilkan"
 
 #~ msgid "Edit the project"
 #~ msgstr "Ubah proyek"
 
+#~ msgid "You probably want to"
+#~ msgstr "Anda mungkin menginginkan"
+
+#~ msgid "add participants"
+#~ msgstr "tambah partisipan"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Anda bisa membagikan ID proyek dan "
+#~ "kode pribadi dengan cara komunikasi "
+#~ "apapun."
+
+#~ msgid "Share the Link"
+#~ msgstr "Bagikan tautan"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Anda bisa membagikan tautan secara "
+#~ "langsung melalui media yang Anda "
+#~ "inginkan"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/it/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-07-12 15:18+0000\n"
 "Last-Translator: Matteo Piotto <piotto@gmail.com>\n"
 "Language: it\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/it/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -26,14 +26,21 @@
 "Quantità o espressione non valida. Solo numeri e operatori + - * / "
 "accettati."
 
 msgid "Project name"
 msgstr "Nome del progetto"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "Codice privato"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "Codice privato"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Inserisci un nuovo codice se lo vuoi modificare"
 
 msgid "Email"
@@ -49,14 +56,22 @@
 msgstr "Valuta predefinita"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Impostando una valuta predefinita abilita la conversione della valuta tra"
 " le fatture"
 
+#, fuzzy
+msgid "Unknown error"
+msgstr "Progetto non conosciuto"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "Codice privato non valido."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Questo progetto non può essere impostato come 'nessuna valuta' perché "
 "contiene fatture in più valute."
 
@@ -89,22 +104,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Si prega di validare il captcha per procedere."
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "Progetto non conosciuto"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "Codice privato non valido."
-
 msgid "Get in"
 msgstr "Entra"
 
 msgid "Admin password"
 msgstr "Password dell'amministratore"
 
 msgid "Send me the code by email"
@@ -275,14 +282,17 @@
 
 msgid "Unknown project"
 msgstr "Progetto non conosciuto"
 
 msgid "Password successfully reset."
 msgstr "Reset della password effettuato."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -805,14 +815,17 @@
 
 msgid "History"
 msgstr "Cronologia"
 
 msgid "Settings"
 msgstr "Impostazioni"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Altri progetti:"
 
 msgid "switch to"
 msgstr "passa a"
 
 msgid "Dashboard"
@@ -882,22 +895,21 @@
 
 msgid "No bills"
 msgstr "Nessun addebito"
 
 msgid "Nothing to list yet."
 msgstr "Ancora niente da mostrare."
 
-msgid "You probably want to"
-msgstr "Probabilmente vuoi"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "aggiungi una spesa"
 
-msgid "add participants"
-msgstr "aggiunti partecipanti"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Aggiungi partecipante"
 
 msgid "Password reminder"
 msgstr "Promemoria password"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -913,55 +925,64 @@
 
 msgid "Reset your password"
 msgstr "Reset della tua password"
 
 msgid "Invite people to join this project"
 msgstr "Invita persone a collaborare a questo progetto"
 
-msgid "Share Identifier & code"
-msgstr "Condividi Identificatore & codice"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"È possibile condividere l'identificativo del progetto e il codice privato"
-" con qualsiasi mezzo di comunicazione."
-
-msgid "Identifier:"
-msgstr "Identificatore:"
 
-msgid "Share the Link"
-msgstr "Condividi il Link"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Puoi condividere direttamente il seguente link attraverso il tuo canale "
-"preferito"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Inviare via Email"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Specifica un elenco di indirizzi email (separati da virgola) a cui vuoi "
 "notificare la\n"
 "                creazione di questo progetto di gestione budget e "
 "manderemo a ciascuno di loro un messaggio per te."
 
+msgid "Share Identifier & code"
+msgstr "Condividi Identificatore & codice"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificatore:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Codice privato"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Chi paga?"
 
 msgid "To whom?"
 msgstr "A chi?"
 
 msgid "Who?"
@@ -1142,7 +1163,30 @@
 
 #~ msgid " show"
 #~ msgstr "visualizza"
 
 #~ msgid "Edit the project"
 #~ msgstr "Modifica il progetto"
 
+#~ msgid "You probably want to"
+#~ msgstr "Probabilmente vuoi"
+
+#~ msgid "add participants"
+#~ msgstr "aggiunti partecipanti"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "È possibile condividere l'identificativo del"
+#~ " progetto e il codice privato con "
+#~ "qualsiasi mezzo di comunicazione."
+
+#~ msgid "Share the Link"
+#~ msgstr "Condividi il Link"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Puoi condividere direttamente il seguente "
+#~ "link attraverso il tuo canale preferito"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2020-11-11 16:28+0000\n"
 "Last-Translator: Jwen921 <yangjingwen0921@gmail.com>\n"
 "Language: ja\n"
 "Language-Team: Japanese <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/ja/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
@@ -24,14 +24,21 @@
 "accepted."
 msgstr "無効な入力です。数字と「+ - * / 」の演算子しか入力できません。"
 
 msgid "Project name"
 msgstr "プロジェクトの名前"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "暗証コード"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "暗証コード"
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -45,14 +52,22 @@
 
 msgid "Default Currency"
 msgstr "初期設定にする通貨"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+#, fuzzy
+msgid "Unknown error"
+msgstr "未知のプロジェクト"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "暗証コード"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -81,22 +96,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "未知のプロジェクト"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "暗証コード"
-
 msgid "Get in"
 msgstr "入る"
 
 msgid "Admin password"
 msgstr "管理者パスワード"
 
 msgid "Send me the code by email"
@@ -256,14 +263,17 @@
 
 msgid "Unknown project"
 msgstr "未知のプロジェクト"
 
 msgid "Password successfully reset."
 msgstr "パスワードを再設定できました。"
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -763,14 +773,17 @@
 
 msgid "History"
 msgstr "歴史"
 
 msgid "Settings"
 msgstr "設定"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "他のプロジェクト："
 
 msgid "switch to"
 msgstr "…に切り替える"
 
 msgid "Dashboard"
@@ -840,21 +853,20 @@
 
 msgid "No bills"
 msgstr "明細なし"
 
 msgid "Nothing to list yet."
 msgstr "表示できるものはありません。"
 
-msgid "You probably want to"
-msgstr "…したいかもしれない"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "明細を追加する"
 
-msgid "add participants"
+#, fuzzy
+msgid "Add the first participant"
 msgstr "参加者を追加する"
 
 msgid "Password reminder"
 msgstr "パスワードを思いさせる"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -869,49 +881,62 @@
 
 msgid "Reset your password"
 msgstr "パスワードを再設定する"
 
 msgid "Invite people to join this project"
 msgstr "他人をこのプロジェクトに招待する"
 
-msgid "Share Identifier & code"
-msgstr "名前とコードを共有する"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
-msgstr "プロジェクト名と私用コードは何の方法でも共有できます。"
-
-msgid "Identifier:"
-msgstr "名前："
-
-msgid "Share the Link"
-msgstr "リンクを共有する"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "好きの手段で以下のリンクを直接に共有できる"
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
+msgstr ""
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "メールで送る"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "…を知らせたいメールアドレスのリストを特定する（カンマ区切り）\n"
 "彼らにこの予算管理プロジェクトの作成をメールでお知らせします。"
 
+msgid "Share Identifier & code"
+msgstr "名前とコードを共有する"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "名前："
+
+#, fuzzy
+msgid "Private code:"
+msgstr "暗証コード"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "誰が支払った？"
 
 msgid "To whom?"
 msgstr "誰まで？"
 
 msgid "Who?"
@@ -1063,7 +1088,25 @@
 
 #~ msgid " show"
 #~ msgstr "表示"
 
 #~ msgid "Edit the project"
 #~ msgstr "プロジェクトを編集する"
 
+#~ msgid "You probably want to"
+#~ msgstr "…したいかもしれない"
+
+#~ msgid "add participants"
+#~ msgstr "参加者を追加する"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr "プロジェクト名と私用コードは何の方法でも共有できます。"
+
+#~ msgid "Share the Link"
+#~ msgstr "リンクを共有する"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "好きの手段で以下のリンクを直接に共有できる"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-10-17 04:56+0000\n"
 "Last-Translator: a-g-rao <athrigrao@gmail.com>\n"
 "Language: kn\n"
 "Language-Team: Kannada <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/kn/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
@@ -27,14 +27,21 @@
 msgstr ""
 "ಮೊತ್ತ ಅಥವಾ ಪದಕಂತೆ ಸರಿಯಿಲ್ಲ. ಸಂಖ್ಯೆ ಮತ್ತು +-*/ ಎಣಿಕೆಬಳಕಗಳನ್ನು ಮಾತ್ರ "
 "ಸ್ವೀಕರಿಸಲಾಗುವುದು."
 
 msgid "Project name"
 msgstr "ಯೋಜನೆಯ ಹೆಸರು"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "ಹೊಸ ಸಂಕೇತಪದ"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "ಹೊಸ ಸಂಕೇತಪದ"
 
 msgid "Enter a new code if you want to change it"
 msgstr "ಸಂಕೇತಪದ ಬದಲಾಯಿಸಬೇಕೆಂದರೆ ನಮೂದಿಸಿ."
 
 msgid "Email"
@@ -48,14 +55,20 @@
 
 msgid "Default Currency"
 msgstr ""
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "ಅಜ್ಞಾತ ದೋಷ"
+
+msgid "Invalid private code."
+msgstr "ನಮೂದಿಸಿರುವ ಸಂಕೇತಪದ ಅಮಾನ್ಯವಾಗಿದೆ."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -83,20 +96,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr "ತೆಗೆದುಹಾಕಲು ನಿಮ್ಮ ಸಂಕೇತಪದವನ್ನು ನಮೂದಿಸಿ"
 
-msgid "Unknown error"
-msgstr "ಅಜ್ಞಾತ ದೋಷ"
-
-msgid "Invalid private code."
-msgstr "ನಮೂದಿಸಿರುವ ಸಂಕೇತಪದ ಅಮಾನ್ಯವಾಗಿದೆ."
-
 msgid "Get in"
 msgstr "ಒಳಹೊಗು"
 
 msgid "Admin password"
 msgstr "ಆಡಳಿತ ನಿರ್ವಾಹಕ ಪ್ರವೇಶ ಪದ"
 
 msgid "Send me the code by email"
@@ -255,14 +262,17 @@
 
 msgid "Unknown project"
 msgstr "ಗೊತ್ತಿಲ್ಲದ ಯೋಜನೆ"
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -748,14 +758,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -824,21 +837,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -853,45 +863,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "ಸಂಕೇತಪದ"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1023,7 +1045,47 @@
 
 #~ msgid " show"
 #~ msgstr "ತೋರಿಸಿ"
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-07-18 12:32+0000\n"
 "Last-Translator: Kemystra <izzmin97@gmail.com>\n"
 "Language: ms\n"
 "Language-Team: Malay <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/ms/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
@@ -23,14 +23,21 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "Nilai atau ungkapan yang sah. Hanya nombor dan operasi + - * / diterima."
 
 msgid "Project name"
 msgstr "Nama projek"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Kod peribadi baharu"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Kod peribadi baharu"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Masukkan kod baharu jika kamu mahu mengubahnya"
 
 msgid "Email"
@@ -48,14 +55,21 @@
 msgid "Default Currency"
 msgstr "Mata wang asal"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
 #, fuzzy
+msgid "Unknown error"
+msgstr "Ralat yang tidak dikenalpasti"
+
+msgid "Invalid private code."
+msgstr "Kod peribadi tidak sah."
+
+#, fuzzy
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Projek ini tidak boleh disetkan kepada 'tiada mata wang' kerana projek "
 "ini mempunyai wang dalam beberapa bentuk mata wang"
 
@@ -85,21 +99,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr "Masukkan kod peribadi untuk mengesahkan penghapusan"
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "Ralat yang tidak dikenalpasti"
-
-msgid "Invalid private code."
-msgstr "Kod peribadi tidak sah."
-
 msgid "Get in"
 msgstr "Masuk"
 
 msgid "Admin password"
 msgstr "Kata laluan pentadbir"
 
 msgid "Send me the code by email"
@@ -262,14 +269,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -754,14 +764,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -830,21 +843,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -859,45 +869,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Kod peribadi"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1029,7 +1051,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-02-13 16:54+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language: nb_NO\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/i"
 "-hate-money/i-hate-money/nb_NO/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Ikke et gyldig beløp eller uttrykk. Kun nummer og operatorene + - * / "
 "godtas."
 
 msgid "Project name"
 msgstr "Prosjektnavn"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Ny privat kode"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Ny privat kode"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Skriv inn en ny kode hvis du ønsker å endre den"
 
 msgid "Email"
@@ -46,14 +53,20 @@
 
 msgid "Default Currency"
 msgstr "Forvalgt valuta"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "En forvalg valutainnstilling skrur på konvertering mellom regninger"
 
+msgid "Unknown error"
+msgstr "Ukjent feil"
+
+msgid "Invalid private code."
+msgstr "Ugyldig privat kode"
+
 #, fuzzy
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Dette prosjektet kan ikke settes til «Ingen valuta» fordi det inneholder "
 "regninger i flere valutaer."
@@ -87,20 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Bekreft CAPTCHA-en for å fortsette."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Skriv inn privat kode for å bekrefte sletting"
 
-msgid "Unknown error"
-msgstr "Ukjent feil"
-
-msgid "Invalid private code."
-msgstr "Ugyldig privat kode"
-
 #, fuzzy
 msgid "Get in"
 msgstr "Til prosjektet"
 
 msgid "Admin password"
 msgstr "Administratorpassord"
 
@@ -271,14 +278,17 @@
 msgid "Unknown project"
 msgstr "Ukjent prosjekt"
 
 #, fuzzy
 msgid "Password successfully reset."
 msgstr "Passord tilbakestilt."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -815,14 +825,17 @@
 
 msgid "History"
 msgstr "Historikk"
 
 msgid "Settings"
 msgstr "Innstillinger"
 
+msgid "RSS Feed"
+msgstr ""
+
 #, fuzzy
 msgid "Other projects :"
 msgstr "Andre prosjekter:"
 
 msgid "switch to"
 msgstr "bytt til"
 
@@ -895,22 +908,21 @@
 msgid "No bills"
 msgstr "Ingen regninger"
 
 #, fuzzy
 msgid "Nothing to list yet."
 msgstr "Ingenting å liste opp enda."
 
-msgid "You probably want to"
-msgstr "Du ønsker antagelig å"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "legge til en regning"
 
-msgid "add participants"
-msgstr "legge til deltagere"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Legg til deltager"
 
 msgid "Password reminder"
 msgstr "Passordpåminner"
 
 #, fuzzy
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -926,56 +938,65 @@
 
 msgid "Reset your password"
 msgstr "Tilbakestill passordet ditt"
 
 msgid "Invite people to join this project"
 msgstr "Inviter folk til å ta del i dette prosjektet"
 
-#, fuzzy
-msgid "Share Identifier & code"
-msgstr "Del identifikator og kode"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Du kan dele prosjektidentifikatoren og den private koden slik det måtte "
-"passe deg."
-
-msgid "Identifier:"
-msgstr "Identifikator:"
-
-#, fuzzy
-msgid "Share the Link"
-msgstr "Del lenken"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Du kan dele denne lenken slik du ønsker"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 #, fuzzy
 msgid "Send via Emails"
 msgstr "Send via e-poster"
 
 #, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Angi en (kommainndelt) liste over e-postadresser du ønsker å varsle om\n"
 "opprettelsen av dette budsjetthåndteringsprosjektet, og de vil få en "
 "e-post om det."
 
+#, fuzzy
+msgid "Share Identifier & code"
+msgstr "Del identifikator og kode"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identifikator:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Privat kode"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Hvem betaler?"
 
 msgid "To whom?"
 msgstr "Til hvem?"
 
 msgid "Who?"
@@ -1293,7 +1314,28 @@
 
 #~ msgid " show"
 #~ msgstr "vis"
 
 #~ msgid "Edit the project"
 #~ msgstr "Rediger prosjektet"
 
+#~ msgid "You probably want to"
+#~ msgstr "Du ønsker antagelig å"
+
+#~ msgid "add participants"
+#~ msgstr "legge til deltagere"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Du kan dele prosjektidentifikatoren og "
+#~ "den private koden slik det måtte "
+#~ "passe deg."
+
+#~ msgid "Share the Link"
+#~ msgstr "Del lenken"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "Du kan dele denne lenken slik du ønsker"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version:  \n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-02-17 02:50+0000\n"
 "Last-Translator: Sander Kooijmans <weblate@gogognome.nl>\n"
 "Language: nl\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/nl/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -28,14 +28,21 @@
 "Geen geldig bedrag of expressie. Gebruik alleen getallen en + - * / "
 "operatoren."
 
 msgid "Project name"
 msgstr "Projectnaam"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "Privécode"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "Privécode"
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -49,14 +56,22 @@
 
 msgid "Default Currency"
 msgstr "Standaard munteenheid"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+#, fuzzy
+msgid "Unknown error"
+msgstr "Onbekend project"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "Privécode"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -85,22 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "Onbekend project"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "Privécode"
-
 msgid "Get in"
 msgstr "Inloggen"
 
 msgid "Admin password"
 msgstr "Admin-wachtwoord"
 
 msgid "Send me the code by email"
@@ -268,14 +275,17 @@
 
 msgid "Unknown project"
 msgstr "Onbekend project"
 
 msgid "Password successfully reset."
 msgstr "Wachtwoord is hersteld."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -787,14 +797,17 @@
 
 msgid "History"
 msgstr "Geschiedenis"
 
 msgid "Settings"
 msgstr "Instellingen"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Overige projecten:"
 
 msgid "switch to"
 msgstr "overschakelen naar"
 
 msgid "Dashboard"
@@ -864,22 +877,21 @@
 
 msgid "No bills"
 msgstr "Geen rekeningen"
 
 msgid "Nothing to list yet."
 msgstr "Nog niks."
 
-msgid "You probably want to"
-msgstr "Waarschijnlijk wil je"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "een rekening toevoegen"
 
-msgid "add participants"
-msgstr "deelnemers toevoegen"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Deelnemer toevoegen"
 
 msgid "Password reminder"
 msgstr "Wachtwoordhint"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -895,53 +907,64 @@
 
 msgid "Reset your password"
 msgstr "Wachtwoord herstellen"
 
 msgid "Invite people to join this project"
 msgstr "Nodig mensen uit voor dit project"
 
-msgid "Share Identifier & code"
-msgstr "Identificatie en code delen"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Je kunt de projectidentificatie en privécode delen via welk "
-"communicatieplatform dan ook."
-
-msgid "Identifier:"
-msgstr "Identificatie:"
-
-msgid "Share the Link"
-msgstr "Link delen"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Je kunt de volgende link direct delen"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Versturen via e-mail"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Stel een (kommagescheiden) lijst op met e-mailadressen van personen die "
 "je op de\n"
 "                hoogte wilt stellen van dit project - wij sturen hen een "
 "e-mail."
 
+msgid "Share Identifier & code"
+msgstr "Identificatie en code delen"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificatie:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Privécode"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Wie betaalt?"
 
 msgid "To whom?"
 msgstr "Aan wie?"
 
 msgid "Who?"
@@ -1116,7 +1139,28 @@
 
 #~ msgid " show"
 #~ msgstr "tonen"
 
 #~ msgid "Edit the project"
 #~ msgstr "Project bewerken"
 
+#~ msgid "You probably want to"
+#~ msgstr "Waarschijnlijk wil je"
+
+#~ msgid "add participants"
+#~ msgstr "deelnemers toevoegen"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Je kunt de projectidentificatie en "
+#~ "privécode delen via welk communicatieplatform"
+#~ " dan ook."
+
+#~ msgid "Share the Link"
+#~ msgstr "Link delen"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "Je kunt de volgende link direct delen"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-09-27 14:19+0000\n"
 "Last-Translator: Andrzej Ochodek <andrzej.ochodek@gmail.com>\n"
 "Language: pl\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/pl/>\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && "
 "(n%100<10 || n%100>=20) ? 1 : 2\n"
@@ -26,14 +26,21 @@
 msgstr ""
 "Niepoprawna kwota lub wyrażenie. Akceptowane są tylko liczby i operatory "
 "+ - * /."
 
 msgid "Project name"
 msgstr "Nazwa projektu"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Nowy kod prywatny"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Nowy kod prywatny"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Wprowadź nowy kod jeżeli chcesz go zmienić"
 
 msgid "Email"
@@ -49,14 +56,20 @@
 msgstr "Domyślna waluta"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Wybranie domyślnej waluty pozwala na konwersję walutową pomiędzy "
 "rachunkami"
 
+msgid "Unknown error"
+msgstr "Nieznany błąd"
+
+msgid "Invalid private code."
+msgstr "Nieprawidłowy kod prywatny."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Ten projekt nie może zostać oznaczony jako 'bez waluty', ponieważ zawiera"
 " on rachunki w różnych walutach."
 
@@ -88,20 +101,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Rozwiąż captcha, by kontynuować."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Wprowadź kod prywatny w celu potwierdzenia usunięcia"
 
-msgid "Unknown error"
-msgstr "Nieznany błąd"
-
-msgid "Invalid private code."
-msgstr "Nieprawidłowy kod prywatny."
-
 msgid "Get in"
 msgstr "Wejdź"
 
 msgid "Admin password"
 msgstr "Hasło administratora"
 
 msgid "Send me the code by email"
@@ -267,14 +274,17 @@
 
 msgid "Unknown project"
 msgstr "Nieznany projekt"
 
 msgid "Password successfully reset."
 msgstr "Hasło zostało pomyślnie zresetowane."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -781,14 +791,17 @@
 
 msgid "History"
 msgstr "Historia"
 
 msgid "Settings"
 msgstr "Ustawienia"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Inne projekty:"
 
 msgid "switch to"
 msgstr "przełącz na"
 
 msgid "Dashboard"
@@ -857,22 +870,21 @@
 
 msgid "No bills"
 msgstr "Brak rachunków"
 
 msgid "Nothing to list yet."
 msgstr "Nie ma jeszcze żadnej listy."
 
-msgid "You probably want to"
-msgstr "Prawdopodobnie chcesz"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "dodać rachunek"
 
-msgid "add participants"
-msgstr "dodać członków"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Edytuj tego uczestnika"
 
 msgid "Password reminder"
 msgstr "Przypomnienie hasła"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -888,55 +900,64 @@
 
 msgid "Reset your password"
 msgstr "Zresetuj swoje hasło"
 
 msgid "Invite people to join this project"
 msgstr "Zaproś ludzi do dołączenia do tego projektu"
 
-msgid "Share Identifier & code"
-msgstr "Udostępnij identyfikator i kod"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Identyfikator projektu i kod prywatny można udostępniać dowolnymi "
-"środkami komunikacji."
 
-msgid "Identifier:"
-msgstr "Identyfikator:"
-
-msgid "Share the Link"
-msgstr "Udostępnij link"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Możesz bezpośrednio udostępnić poniższy link za pośrednictwem "
-"preferowanego medium"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Wyślij przez maile"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Podaj (adresy rozdzielone przecinkami) adresy email, które chcesz "
 "powiadomić o \n"
 "                utworzeniu tego projektu zarządzania budżetem, a my "
 "wyślemy Ci wiadomość email."
 
+msgid "Share Identifier & code"
+msgstr "Udostępnij identyfikator i kod"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identyfikator:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Kod prywatny"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Kto płaci?"
 
 msgid "To whom?"
 msgstr "Komu?"
 
 msgid "Who?"
@@ -1113,7 +1134,30 @@
 
 #~ msgid " show"
 #~ msgstr "pokaż"
 
 #~ msgid "Edit the project"
 #~ msgstr "Edytuj projekt"
 
+#~ msgid "You probably want to"
+#~ msgstr "Prawdopodobnie chcesz"
+
+#~ msgid "add participants"
+#~ msgstr "dodać członków"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Identyfikator projektu i kod prywatny "
+#~ "można udostępniać dowolnymi środkami "
+#~ "komunikacji."
+
+#~ msgid "Share the Link"
+#~ msgstr "Udostępnij link"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Możesz bezpośrednio udostępnić poniższy link"
+#~ " za pośrednictwem preferowanego medium"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-05-05 00:47+0000\n"
 "Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
 "Language: pt\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/pt/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
 "aceites."
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Código privado novo"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Código privado novo"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Digite um novo código se quiser alterá-lo"
 
 msgid "Email"
@@ -46,14 +53,20 @@
 
 msgid "Default Currency"
 msgstr "Moeda predefinida"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "Definir uma moeda padrão permite a conversão de moeda entre faturas"
 
+msgid "Unknown error"
+msgstr "Erro desconhecido"
+
+msgid "Invalid private code."
+msgstr "Código privado inválido."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Este projeto não pode ser definido como 'sem moeda' porque contém faturas"
 " em várias moedas."
 
@@ -85,20 +98,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Por favor, valide o captcha para prosseguir."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Digite o código privado para confirmar a exclusão"
 
-msgid "Unknown error"
-msgstr "Erro desconhecido"
-
-msgid "Invalid private code."
-msgstr "Código privado inválido."
-
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
 msgstr "Palavra-passe do administrador"
 
 msgid "Send me the code by email"
@@ -267,14 +274,17 @@
 
 msgid "Unknown project"
 msgstr "Projeto desconhecido"
 
 msgid "Password successfully reset."
 msgstr "Palavra-passe redefinida corretamente."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -781,14 +791,17 @@
 
 msgid "History"
 msgstr "Histórico"
 
 msgid "Settings"
 msgstr "Configurações"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Outros projetos:"
 
 msgid "switch to"
 msgstr "mudar para"
 
 msgid "Dashboard"
@@ -857,22 +870,21 @@
 
 msgid "No bills"
 msgstr "Sem faturas"
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
-msgid "You probably want to"
-msgstr "Provavelmente gostaria de"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "adicionar uma fatura"
 
-msgid "add participants"
-msgstr "adicionar participantes"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Editar este participante"
 
 msgid "Password reminder"
 msgstr "Lembrete de palavra-passe"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -888,55 +900,64 @@
 
 msgid "Reset your password"
 msgstr "Redefinir sua palavra-passe"
 
 msgid "Invite people to join this project"
 msgstr "Convide pessoas para participar deste projeto"
 
-msgid "Share Identifier & code"
-msgstr "Compartilhar Identificador & código"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Pode compartilhar o identificador do projeto e o código privado por "
-"qualquer meio de comunicação."
 
-msgid "Identifier:"
-msgstr "Identificador:"
-
-msgid "Share the Link"
-msgstr "Compartilhar a ligação"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Pode compartilhar diretamente o seguinte ligação através do seu meio "
-"preferido"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Enviar via E-mails"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Especifique uma lista (separada por vírgulas) de endereços de e-mail que "
 "deseja notificar sobre a\n"
 "                criação deste projeto de gestão orçamental e enviaremos "
 "um e-mail para si."
 
+msgid "Share Identifier & code"
+msgstr "Compartilhar Identificador & código"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificador:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Código privado"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Quem paga?"
 
 msgid "To whom?"
 msgstr "A quem?"
 
 msgid "Who?"
@@ -1093,7 +1114,30 @@
 
 #~ msgid " show"
 #~ msgstr "exibir"
 
 #~ msgid "Edit the project"
 #~ msgstr "Editar o projeto"
 
+#~ msgid "You probably want to"
+#~ msgstr "Provavelmente gostaria de"
+
+#~ msgid "add participants"
+#~ msgstr "adicionar participantes"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Pode compartilhar o identificador do "
+#~ "projeto e o código privado por "
+#~ "qualquer meio de comunicação."
+
+#~ msgid "Share the Link"
+#~ msgstr "Compartilhar a ligação"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Pode compartilhar diretamente o seguinte "
+#~ "ligação através do seu meio preferido"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-05-05 00:47+0000\n"
 "Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/i"
 "-hate-money/i-hate-money/pt_BR/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
 "aceitos."
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Código privado novo"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Código privado novo"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Insira um novo código se quiser alterá-lo"
 
 msgid "Email"
@@ -46,14 +53,20 @@
 
 msgid "Default Currency"
 msgstr "Moeda Padrão"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "Definir uma moeda padrão permite a conversão de moeda entre contas"
 
+msgid "Unknown error"
+msgstr "Erro desconhecido"
+
+msgid "Invalid private code."
+msgstr "Código privado inválido."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "O projeto não pode ser definido como 'sem moeda' porque contém contas em "
 "várias moedas."
 
@@ -85,20 +98,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Por favor, valide o captcha para prosseguir."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Digite o código privado para confirmar a exclusão"
 
-msgid "Unknown error"
-msgstr "Erro desconhecido"
-
-msgid "Invalid private code."
-msgstr "Código privado inválido."
-
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
 msgstr "Senha do administrador"
 
 msgid "Send me the code by email"
@@ -266,14 +273,17 @@
 
 msgid "Unknown project"
 msgstr "Projeto desconhecido"
 
 msgid "Password successfully reset."
 msgstr "Senha redefinida corretamente."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -779,14 +789,17 @@
 
 msgid "History"
 msgstr "Histórico"
 
 msgid "Settings"
 msgstr "Configurações"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Outros projetos:"
 
 msgid "switch to"
 msgstr "mudar para"
 
 msgid "Dashboard"
@@ -855,22 +868,21 @@
 
 msgid "No bills"
 msgstr "Sem contas"
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
-msgid "You probably want to"
-msgstr "Você provavelmente gostaria de"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "adicionar uma conta"
 
-msgid "add participants"
-msgstr "adicionar participantes"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Editar usuário"
 
 msgid "Password reminder"
 msgstr "Lembrete de senha"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -886,55 +898,64 @@
 
 msgid "Reset your password"
 msgstr "Redefinir sua senha"
 
 msgid "Invite people to join this project"
 msgstr "Convide pessoas para participar deste projeto"
 
-msgid "Share Identifier & code"
-msgstr "Compartilhar Identificador & código"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Você pode compartilhar o identificador do projeto e o código privado por "
-"qualquer meio de comunicação."
 
-msgid "Identifier:"
-msgstr "Identificador:"
-
-msgid "Share the Link"
-msgstr "Compartilhar o Link"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Você pode compartilhar diretamente o seguinte link através do seu meio "
-"preferido"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Enviar via E-mails"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Especifica uma lista de endereços de email (separados por vírgula) que "
 "você quer notificar acerca da\n"
 "                criação deste projeto de gestão de saldo e nós iremos "
 "enviar um email por si."
 
+msgid "Share Identifier & code"
+msgstr "Compartilhar Identificador & código"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identificador:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Código privado"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Quem paga?"
 
 msgid "To whom?"
 msgstr "Para quem?"
 
 msgid "Who?"
@@ -1092,7 +1113,31 @@
 
 #~ msgid " show"
 #~ msgstr "exibir"
 
 #~ msgid "Edit the project"
 #~ msgstr "Editar o projeto"
 
+#~ msgid "You probably want to"
+#~ msgstr "Você provavelmente gostaria de"
+
+#~ msgid "add participants"
+#~ msgstr "adicionar participantes"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Você pode compartilhar o identificador "
+#~ "do projeto e o código privado por"
+#~ " qualquer meio de comunicação."
+
+#~ msgid "Share the Link"
+#~ msgstr "Compartilhar o Link"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Você pode compartilhar diretamente o "
+#~ "seguinte link através do seu meio "
+#~ "preferido"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-05-07 23:52+0000\n"
 "Last-Translator: Egor Dubenetskiy <egor@banka.space>\n"
 "Language: ru\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/ru/>\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
@@ -26,14 +26,21 @@
 msgstr ""
 "Недопустимая сумма выражения. Принимаются только цифры и операторы + - * "
 "/ ."
 
 msgid "Project name"
 msgstr "Имя проекта"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Новый приватный код"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Новый приватный код"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Введите новый код, если хотите его изменить"
 
 msgid "Email"
@@ -49,14 +56,20 @@
 msgstr "Валюта по умолчанию"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Установка валюты по умолчанию позволяет конвертировать валюту между "
 "счетами"
 
+msgid "Unknown error"
+msgstr "Неизвестная ошибка"
+
+msgid "Invalid private code."
+msgstr "Неверный приватный код."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Для этого проекта нельзя установить режим «без валюты», так как он "
 "содержит счета в нескольких валютах."
 
@@ -88,20 +101,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Пожалуйста, подтвердите капчу, чтобы продолжить."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Введите приватный код, чтобы подтвердить удаление"
 
-msgid "Unknown error"
-msgstr "Неизвестная ошибка"
-
-msgid "Invalid private code."
-msgstr "Неверный приватный код."
-
 msgid "Get in"
 msgstr "Войти"
 
 msgid "Admin password"
 msgstr "Пароль администратора"
 
 msgid "Send me the code by email"
@@ -268,14 +275,17 @@
 
 msgid "Unknown project"
 msgstr "Неизвестный проект"
 
 msgid "Password successfully reset."
 msgstr "Пароль успешно восстановлен."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -788,14 +798,17 @@
 
 msgid "History"
 msgstr "История"
 
 msgid "Settings"
 msgstr "Настройки"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Остальные проекты :"
 
 msgid "switch to"
 msgstr "сменён на"
 
 msgid "Dashboard"
@@ -864,22 +877,21 @@
 
 msgid "No bills"
 msgstr "Нет счетов"
 
 msgid "Nothing to list yet."
 msgstr "Нечего перечислять еще."
 
-msgid "You probably want to"
-msgstr "Возможно вы хотите"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "добавить счёт"
 
-msgid "add participants"
-msgstr "добавить пользователя"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Редактировать участника"
 
 msgid "Password reminder"
 msgstr "Напоминание пароля"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -893,53 +905,64 @@
 
 msgid "Reset your password"
 msgstr "Восстановить пароль"
 
 msgid "Invite people to join this project"
 msgstr "Пригласите людей присоединиться к этому проекту"
 
-msgid "Share Identifier & code"
-msgstr "Поделиться идентификатором и кодом"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Вы можете поделиться идентификатором проекта и личным кодом любым "
-"способом связи."
-
-msgid "Identifier:"
-msgstr "Идентификатор:"
-
-msgid "Share the Link"
-msgstr "Поделиться ссылкой"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Вы можете напрямую поделиться следующей ссылкой через любой способ связи"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Отправить по почте"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Укажите (разделенный запятыми) список адресов электронной почты, которые "
 "вы хотите уведомить о\n"
 "                создание этого проекта управления бюджетом, и мы вышлем "
 "им письмо."
 
+msgid "Share Identifier & code"
+msgstr "Поделиться идентификатором и кодом"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Идентификатор:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Приватный код"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Кто платит?"
 
 msgid "To whom?"
 msgstr "Кому?"
 
 msgid "Who?"
@@ -1118,7 +1141,29 @@
 
 #~ msgid " show"
 #~ msgstr "показать"
 
 #~ msgid "Edit the project"
 #~ msgstr "Изменить проект"
 
+#~ msgid "You probably want to"
+#~ msgstr "Возможно вы хотите"
+
+#~ msgid "add participants"
+#~ msgstr "добавить пользователя"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Вы можете поделиться идентификатором проекта"
+#~ " и личным кодом любым способом связи."
+
+#~ msgid "Share the Link"
+#~ msgstr "Поделиться ссылкой"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Вы можете напрямую поделиться следующей "
+#~ "ссылкой через любой способ связи"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-04-09 13:26+0000\n"
 "Last-Translator: Rastko Sarcevic <ralesarcevic@gmail.com>\n"
 "Language: sr\n"
 "Language-Team: Serbian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/sr/>\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
@@ -24,14 +24,20 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr ""
 
+msgid "Current private code"
+msgstr ""
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr ""
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -45,14 +51,20 @@
 
 msgid "Default Currency"
 msgstr "Podrazumevana Valuta"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr ""
+
+msgid "Invalid private code."
+msgstr ""
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -81,20 +93,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-msgid "Unknown error"
-msgstr ""
-
-msgid "Invalid private code."
-msgstr ""
-
 msgid "Get in"
 msgstr ""
 
 msgid "Admin password"
 msgstr "Administratorska lozinka"
 
 msgid "Send me the code by email"
@@ -251,14 +257,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr "Lozinka uspešno resetovana."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -745,14 +754,17 @@
 
 msgid "History"
 msgstr "Istorija"
 
 msgid "Settings"
 msgstr "Podešavanja"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -821,21 +833,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -850,45 +859,56 @@
 
 msgid "Reset your password"
 msgstr "Resetuj lozinku"
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
-msgstr "Podelite link"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "Scan QR code"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Send via Emails"
+msgid "Share Identifier & code"
 msgstr ""
 
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr ""
+
+msgid "Private code:"
+msgstr ""
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr "Ko plaća?"
 
 msgid "To whom?"
 msgstr "Kome?"
@@ -1089,7 +1109,47 @@
 
 #~ msgid " show"
 #~ msgstr "prikaži"
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr "Podelite link"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2023-02-07 21:51+0000\n"
 "Last-Translator: Kristoffer Grundström "
 "<swedishsailfishosuser@tutanota.com>\n"
 "Language: sv\n"
 "Language-Team: Swedish <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/sv/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
@@ -26,14 +26,21 @@
 msgstr ""
 "Inte en giltig summa eller uttryck. Endast nummer och +-* /-operatörer "
 "accepteras."
 
 msgid "Project name"
 msgstr "Namn på projektet"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Ny privat kod"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Ny privat kod"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Ange en ny kod om du vill ändra den"
 
 msgid "Email"
@@ -47,14 +54,20 @@
 
 msgid "Default Currency"
 msgstr "Standardvaluta"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "Okänt fel"
+
+msgid "Invalid private code."
+msgstr "Ogiltig privat kod."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Det här projektet kan inte ställas in till 'ingen valuta' eftersom att "
 "det innehåller sedlar i flera olika valutor."
 
@@ -86,20 +99,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Snälla, bekräfta captcha för att fortsätta."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Ange privat kod för att bekräfta borttagning"
 
-msgid "Unknown error"
-msgstr "Okänt fel"
-
-msgid "Invalid private code."
-msgstr "Ogiltig privat kod."
-
 msgid "Get in"
 msgstr ""
 
 msgid "Admin password"
 msgstr "Lösenord för admin"
 
 msgid "Send me the code by email"
@@ -267,14 +274,17 @@
 
 msgid "Unknown project"
 msgstr "Okänt projekt"
 
 msgid "Password successfully reset."
 msgstr "Återställningen av lösenordet lyckades."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -776,14 +786,17 @@
 
 msgid "History"
 msgstr "Historik"
 
 msgid "Settings"
 msgstr "Inställningar"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Andra projekt :"
 
 msgid "switch to"
 msgstr "byt till"
 
 msgid "Dashboard"
@@ -852,22 +865,21 @@
 
 msgid "No bills"
 msgstr "Inga räkningar"
 
 msgid "Nothing to list yet."
 msgstr "Ingenting att lista än."
 
-msgid "You probably want to"
-msgstr "Du kanske vill"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "lägg till en räkning"
 
-msgid "add participants"
-msgstr "lägg till deltagare"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Redigera den här deltagaren"
 
 msgid "Password reminder"
 msgstr "Lösenordspåminnare"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -883,53 +895,64 @@
 
 msgid "Reset your password"
 msgstr "Återställ ditt lösenord"
 
 msgid "Invite people to join this project"
 msgstr "Bjud in personer att ansluta till det här projektet"
 
-msgid "Share Identifier & code"
-msgstr "Dela ut identifierare & kod"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Du kan dela projektets identifierare och den privata koden så som det "
-"passar dig."
-
-msgid "Identifier:"
-msgstr "Identifierare:"
-
-msgid "Share the Link"
-msgstr "Dela ut länken"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "Du kan direkt dela ut följande länk via föredraget media"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "Skicka via e-post"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Ange en (delat med ett kommatecken)  lista över e-postadresser som du "
 "vill underrätta om\n"
 "                skapandet av det här budgethanteringsprojektet gör att de"
 " kommer att få ett e-postmeddelande om det."
 
+msgid "Share Identifier & code"
+msgstr "Dela ut identifierare & kod"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Identifierare:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Privat kod"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Vem betalar?"
 
 msgid "To whom?"
 msgstr "Till vem?"
 
 msgid "Who?"
@@ -1078,7 +1101,28 @@
 
 #~ msgid " show"
 #~ msgstr "visa"
 
 #~ msgid "Edit the project"
 #~ msgstr "Redigera projektet"
 
+#~ msgid "You probably want to"
+#~ msgstr "Du kanske vill"
+
+#~ msgid "add participants"
+#~ msgstr "lägg till deltagare"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Du kan dela projektets identifierare och"
+#~ " den privata koden så som det "
+#~ "passar dig."
+
+#~ msgid "Share the Link"
+#~ msgstr "Dela ut länken"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "Du kan direkt dela ut följande länk via föredraget media"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2020-07-01 18:41+0000\n"
 "Last-Translator: rohitn01 <rohitmen01@gmail.com>\n"
 "Language: ta\n"
 "Language-Team: Tamil <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/ta/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -28,14 +28,21 @@
 "சரியான அளவு அல்லது வெளிப்பாடு அல்ல. எண்கள் மற்றும் + - * / ஆபரேட்டர்கள் "
 "ஏற்றுக்கொள்ளப்படுகிறார்கள்."
 
 msgid "Project name"
 msgstr "திட்டத்தின் பெயர்"
 
 #, fuzzy
+msgid "Current private code"
+msgstr "தனியார் குறியீடு"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
+#, fuzzy
 msgid "New private code"
 msgstr "தனியார் குறியீடு"
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -49,14 +56,22 @@
 
 msgid "Default Currency"
 msgstr "இயல்புநிலை நாணயம்"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+#, fuzzy
+msgid "Unknown error"
+msgstr "தெரியாத திட்டம்"
+
+#, fuzzy
+msgid "Invalid private code."
+msgstr "தனியார் குறியீடு"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -86,22 +101,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-#, fuzzy
-msgid "Unknown error"
-msgstr "தெரியாத திட்டம்"
-
-#, fuzzy
-msgid "Invalid private code."
-msgstr "தனியார் குறியீடு"
-
 msgid "Get in"
 msgstr "உள்ளே வா"
 
 msgid "Admin password"
 msgstr "நிர்வாகி கடவுச்சொல்"
 
 msgid "Send me the code by email"
@@ -270,14 +277,17 @@
 
 msgid "Unknown project"
 msgstr "தெரியாத திட்டம்"
 
 msgid "Password successfully reset."
 msgstr "கடவுச்சொல் வெற்றிகரமாக மீட்டமைக்கப்படுகிறது."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -770,14 +780,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -846,21 +859,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add a bill"
-msgstr ""
-
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -875,45 +885,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "Share the Link"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Scan QR code"
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid "Send via Emails"
+msgid "Identifier:"
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+#, fuzzy
+msgid "Private code:"
+msgstr "தனியார் குறியீடு"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1094,7 +1116,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/te/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/te/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-10-04 14:19+0000\n"
 "Last-Translator: Sharan J <sharanjs1999@gmail.com>\n"
 "Language: te\n"
 "Language-Team: Telugu <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/te/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -26,14 +26,21 @@
 msgstr ""
 "మీరు ఇచ్చిన లెక్కింపు సరైనది కాదు . సంఖ్యలు మరియు + - * / మాత్రమే "
 "అంగీకరించబడతాయి."
 
 msgid "Project name"
 msgstr "ప్రాజెక్ట్ పేరు"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "కొత్త ప్రైవేట్ కోడ్"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "కొత్త ప్రైవేట్ కోడ్"
 
 msgid "Enter a new code if you want to change it"
 msgstr "మీరు ముందు కోడ్ ని మార్చాలి అంటే కొత్త కోడ్ ఇవ్వండి"
 
 msgid "Email"
@@ -50,14 +57,20 @@
 msgstr "డిఫాల్ట్ కరెన్సీ"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "డిఫాల్ట్ కరెన్సీని సెట్ చేయడం వలన బిల్లుల మధ్య కరెన్సీ మార్పిడిని "
 "కుదురుతుంది"
 
+msgid "Unknown error"
+msgstr "గుర్తించలేని ఎర్రర్"
+
+msgid "Invalid private code."
+msgstr "ప్రైవేట్ కోడ్ తప్పు."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "ఈ ప్రాజెక్ట్ బహుళ కరెన్సీలలో బిల్లులను కలిగి ఉన్నందున 'నో కరెన్సీ'కి సెట్"
 " చెయ్యడం కుదరదు."
 
@@ -91,20 +104,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "ముందుకు సాగడం కొరకు క్యాప్చాను వాలిడేట్ చేయండి."
 
 msgid "Enter private code to confirm deletion"
 msgstr "తొలగింపును ధృవీకరించడం కొరకు ప్రయివేట్ కోడ్‌ను నమోదు చేయండి"
 
-msgid "Unknown error"
-msgstr "గుర్తించలేని ఎర్రర్"
-
-msgid "Invalid private code."
-msgstr "ప్రైవేట్ కోడ్ తప్పు."
-
 msgid "Get in"
 msgstr "లోపలి వేళ్ళు"
 
 #, fuzzy
 msgid "Admin password"
 msgstr "అడ్మిన్ పాస్ వర్డ్"
 
@@ -278,14 +285,17 @@
 
 msgid "Unknown project"
 msgstr "తెలియని ప్రాజెక్ట్"
 
 msgid "Password successfully reset."
 msgstr "పాస్ వర్డ్ విజయవంతంగా రీసెట్ చేయబడింది."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -778,14 +788,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -854,21 +867,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -883,45 +893,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "ప్రైవేట్ కోడ్"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -998,7 +1020,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/th/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2021-09-16 14:36+0000\n"
 "Last-Translator: PPNplus <ppnplus@protonmail.com>\n"
 "Language: th\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/th/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
@@ -23,14 +23,20 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr "ชื่อโครงการ"
 
+msgid "Current private code"
+msgstr ""
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr ""
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -44,14 +50,20 @@
 
 msgid "Default Currency"
 msgstr "สกุลเงินค่าเริ่มต้น"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "ข้อผิดพลาดที่ไม่รู้จัก"
+
+msgid "Invalid private code."
+msgstr ""
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -79,20 +91,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-msgid "Unknown error"
-msgstr "ข้อผิดพลาดที่ไม่รู้จัก"
-
-msgid "Invalid private code."
-msgstr ""
-
 msgid "Get in"
 msgstr "เข้าด้านใน"
 
 msgid "Admin password"
 msgstr "รหัสผ่านผู้ดูแล"
 
 msgid "Send me the code by email"
@@ -249,14 +255,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -740,14 +749,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -816,21 +828,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -845,45 +854,56 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+msgid "Private code:"
+msgstr ""
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr "ให้ใคร?"
@@ -1018,7 +1038,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-11-07 10:07+0000\n"
 "Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
 "Language: tr\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/tr/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -25,14 +25,21 @@
 msgstr ""
 "Geçerli bir miktar veya ifade değil. Yalnızca rakamlar ve + - * / "
 "operatörleri kabul edilir."
 
 msgid "Project name"
 msgstr "Proje adı"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Yeni özel kod"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Yeni özel kod"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Kodu değiştirmek istiyorsanız yenisini girin"
 
 msgid "Email"
@@ -48,14 +55,20 @@
 msgstr "Öntanımlı Para Birimi"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 "Öntanımlı para biriminin ayarlanması, faturalar arasında para birimi "
 "dönüştürmeyi etkinleştirir"
 
+msgid "Unknown error"
+msgstr "Bilinmeyen hata"
+
+msgid "Invalid private code."
+msgstr "Geçersiz özel kod."
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Bu proje, birden fazla para biriminde faturalar içerdiğinden 'para birimi"
 " yok' olarak ayarlanamaz."
 
@@ -87,20 +100,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Lütfen, devam etmek için captcha'yı doğrulayın."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Silme işlemini onaylamak için özel kodu girin"
 
-msgid "Unknown error"
-msgstr "Bilinmeyen hata"
-
-msgid "Invalid private code."
-msgstr "Geçersiz özel kod."
-
 msgid "Get in"
 msgstr "Alın"
 
 msgid "Admin password"
 msgstr "Yönetici parolası"
 
 msgid "Send me the code by email"
@@ -268,14 +275,17 @@
 
 msgid "Unknown project"
 msgstr "Bilinmeyen proje"
 
 msgid "Password successfully reset."
 msgstr "Parola başarıyla sıfırlandı."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -784,14 +794,17 @@
 
 msgid "History"
 msgstr "Geçmiş"
 
 msgid "Settings"
 msgstr "Ayarlar"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "Diğer projeler:"
 
 msgid "switch to"
 msgstr "geçiş yap"
 
 msgid "Dashboard"
@@ -860,22 +873,21 @@
 
 msgid "No bills"
 msgstr "Fatura yok"
 
 msgid "Nothing to list yet."
 msgstr "Henüz listelenecek bir şey yok."
 
-msgid "You probably want to"
-msgstr "Muhtemelen istediğiniz"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "bir fatura ekle"
 
-msgid "add participants"
-msgstr "katılımcılar ekle"
+#, fuzzy
+msgid "Add the first participant"
+msgstr "Bu katılımcıyı düzenle"
 
 msgid "Password reminder"
 msgstr "Parola hatırlatıcı"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
@@ -891,55 +903,64 @@
 
 msgid "Reset your password"
 msgstr "Parolanızı sıfırlayın"
 
 msgid "Invite people to join this project"
 msgstr "İnsanları bu projeye katılmaya davet et"
 
-msgid "Share Identifier & code"
-msgstr "Tanımlayıcıyı ve Kodu Paylaş"
-
-msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+msgid "Share an invitation link"
 msgstr ""
-"Proje tanımlayıcısını ve özel kodu herhangi bir iletişim aracıyla "
-"paylaşabilirsiniz."
 
-msgid "Identifier:"
-msgstr "Tanımlayıcı:"
-
-msgid "Share the Link"
-msgstr "Bağlantıyı Paylaş"
-
-msgid "You can directly share the following link via your prefered medium"
+msgid ""
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
-"Aşağıdaki bağlantıyı tercih ettiğiniz ortam aracılığıyla doğrudan "
-"paylaşabilirsiniz"
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "E-posta ile Gönder"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "Bu bütçe yönetimi projesinin oluşturulması hakkında bildirimde bulunmak "
 "istediğiniz e-posta \n"
 "                adreslerinin (virgülle ayrılmış) bir listesini belirtin, "
 "biz de sizin için onlara bir e-posta gönderelim."
 
+msgid "Share Identifier & code"
+msgstr "Tanımlayıcıyı ve Kodu Paylaş"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "Tanımlayıcı:"
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Özel kod"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "Kim ödüyor?"
 
 msgid "To whom?"
 msgstr "Kime?"
 
 msgid "Who?"
@@ -1129,7 +1150,30 @@
 
 #~ msgid " show"
 #~ msgstr "göster"
 
 #~ msgid "Edit the project"
 #~ msgstr "Projeyi düzenle"
 
+#~ msgid "You probably want to"
+#~ msgstr "Muhtemelen istediğiniz"
+
+#~ msgid "add participants"
+#~ msgstr "katılımcılar ekle"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+#~ "Proje tanımlayıcısını ve özel kodu "
+#~ "herhangi bir iletişim aracıyla "
+#~ "paylaşabilirsiniz."
+
+#~ msgid "Share the Link"
+#~ msgstr "Bağlantıyı Paylaş"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+#~ "Aşağıdaki bağlantıyı tercih ettiğiniz ortam"
+#~ " aracılığıyla doğrudan paylaşabilirsiniz"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-09-17 10:24+0000\n"
 "Last-Translator: Dmytro Onopa <dmytro.onopa@gmail.com>\n"
 "Language: uk\n"
 "Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/uk/>\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
@@ -24,14 +24,21 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "Не вірна сума чи вираз. Приймаються тільки числа та оператори + - * /."
 
 msgid "Project name"
 msgstr "Назва проєкту"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "Новий приватний код"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "Новий приватний код"
 
 msgid "Enter a new code if you want to change it"
 msgstr "Введіть новий код якщо бажаєте його змінити"
 
 msgid "Email"
@@ -45,14 +52,20 @@
 
 msgid "Default Currency"
 msgstr "Валюта по замовчуванню"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "Встановлення типової валюти уможливлює конвертацію валюти між векселями"
 
+msgid "Unknown error"
+msgstr "Невідома помилка"
+
+msgid "Invalid private code."
+msgstr "Помилковий приватний ключ"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Цей проект не може бути встановлено у значення \"Без валюти\", оскільки "
 "він містить декілько валют в рахунках."
 
@@ -84,20 +97,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Будь ласка, заповніть капчу для продовження."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Введіть приватний ключ для підтвердження видалення."
 
-msgid "Unknown error"
-msgstr "Невідома помилка"
-
-msgid "Invalid private code."
-msgstr "Помилковий приватний ключ"
-
 msgid "Get in"
 msgstr "Отримати в"
 
 msgid "Admin password"
 msgstr "Пароль адміністратора"
 
 msgid "Send me the code by email"
@@ -256,14 +263,17 @@
 
 msgid "Unknown project"
 msgstr "Невідомий проєкт"
 
 msgid "Password successfully reset."
 msgstr "Пароль з успіхом відновлено."
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -752,14 +762,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -828,21 +841,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -857,45 +867,57 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+#, fuzzy
+msgid "Private code:"
+msgstr "Приватний код"
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -1103,7 +1125,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/ur/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/ur/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-07-03 10:18+0000\n"
 "Last-Translator: Shafiq Azeez <fubukishirouk@gmail.com>\n"
 "Language: ur\n"
 "Language-Team: Urdu <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/ur/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -23,14 +23,20 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr "منصوبےکانام"
 
+msgid "Current private code"
+msgstr ""
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr ""
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -44,14 +50,20 @@
 
 msgid "Default Currency"
 msgstr ""
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr "نامعلوم خرابی"
+
+msgid "Invalid private code."
+msgstr ""
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -79,20 +91,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-msgid "Unknown error"
-msgstr "نامعلوم خرابی"
-
-msgid "Invalid private code."
-msgstr ""
-
 msgid "Get in"
 msgstr ""
 
 msgid "Admin password"
 msgstr ""
 
 msgid "Send me the code by email"
@@ -248,14 +254,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -738,14 +747,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -814,21 +826,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -843,45 +852,56 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+msgid "Private code:"
+msgstr ""
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -980,7 +1000,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/vi/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language: vi\n"
 "Language-Team: none\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -22,14 +22,20 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr ""
 
+msgid "Current private code"
+msgstr ""
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr ""
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
@@ -43,14 +49,20 @@
 
 msgid "Default Currency"
 msgstr ""
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+msgid "Unknown error"
+msgstr ""
+
+msgid "Invalid private code."
+msgstr ""
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -78,20 +90,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
-msgid "Unknown error"
-msgstr ""
-
-msgid "Invalid private code."
-msgstr ""
-
 msgid "Get in"
 msgstr ""
 
 msgid "Admin password"
 msgstr ""
 
 msgid "Send me the code by email"
@@ -247,14 +253,17 @@
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -737,14 +746,17 @@
 
 msgid "History"
 msgstr ""
 
 msgid "Settings"
 msgstr ""
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
@@ -813,21 +825,18 @@
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
-msgid "You probably want to"
-msgstr ""
-
-msgid "add a bill"
+msgid "Add your first bill"
 msgstr ""
 
-msgid "add participants"
+msgid "Add the first participant"
 msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -842,45 +851,56 @@
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
-msgid "Share Identifier & code"
+msgid "Share an invitation link"
 msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
 msgstr ""
 
-msgid "Identifier:"
+msgid "Scan QR code"
 msgstr ""
 
-msgid "Share the Link"
+msgid "Use a mobile device with a compatible app."
 msgstr ""
 
-msgid "You can directly share the following link via your prefered medium"
+msgid "Send via Emails"
 msgstr ""
 
-msgid "Scan QR code"
+msgid ""
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 
-msgid "Use a mobile device with a compatible app."
+msgid "Share Identifier & code"
 msgstr ""
 
-msgid "Send via Emails"
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
 msgstr ""
 
-msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+msgid "Identifier:"
+msgstr ""
+
+msgid "Private code:"
+msgstr ""
+
+msgid "the private code was defined when you created the project"
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
 msgstr ""
@@ -979,7 +999,47 @@
 
 #~ msgid " show"
 #~ msgstr ""
 
 #~ msgid "Edit the project"
 #~ msgstr ""
 
+#~ msgid "You probably want to"
+#~ msgstr ""
+
+#~ msgid "add a bill"
+#~ msgstr ""
+
+#~ msgid "add participants"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr ""
+
+#~ msgid "Share the Link"
+#~ msgstr ""
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email for you."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Specify a (comma separated) list of "
+#~ "email adresses you want to notify "
+#~ "about the\n"
+#~ "                creation of this budget "
+#~ "management project and we will send "
+#~ "them an email with the invitation "
+#~ "link."
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo` & `ihatemoney-6.1.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po` & `ihatemoney-6.1.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"POT-Creation-Date: 2023-07-29 14:24+0200\n"
 "PO-Revision-Date: 2022-07-21 05:15+0000\n"
 "Last-Translator: z.liu <zwliu07@live.com>\n"
 "Language: zh_Hans\n"
 "Language-Team: Chinese (Simplified) "
 "<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/zh_Hans/>"
 "\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -24,14 +24,21 @@
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "金额或符号无效。仅限数字与+-*/符号。"
 
 msgid "Project name"
 msgstr "账目名称"
 
+#, fuzzy
+msgid "Current private code"
+msgstr "新的私人代码"
+
+msgid "Enter existing private code to edit project"
+msgstr ""
+
 msgid "New private code"
 msgstr "新的私人代码"
 
 msgid "Enter a new code if you want to change it"
 msgstr "如要更改，请输入新代码"
 
 msgid "Email"
@@ -45,14 +52,20 @@
 
 msgid "Default Currency"
 msgstr "默认货币"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "设置默认货币可实现账单之间的货币转换"
 
+msgid "Unknown error"
+msgstr "未知错误"
+
+msgid "Invalid private code."
+msgstr "无效的私人代码。"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr "此项目不能设置为“无货币”，因为它包含多种货币的账单。"
 
 msgid "Compatible with Cospend"
 msgstr ""
@@ -80,20 +93,14 @@
 
 msgid "Please, validate the captcha to proceed."
 msgstr "请输入验证码以继续。"
 
 msgid "Enter private code to confirm deletion"
 msgstr "请输入专用代码以确认删除"
 
-msgid "Unknown error"
-msgstr "未知错误"
-
-msgid "Invalid private code."
-msgstr "无效的私人代码。"
-
 msgid "Get in"
 msgstr "进入"
 
 msgid "Admin password"
 msgstr "管理密码"
 
 msgid "Send me the code by email"
@@ -253,14 +260,17 @@
 
 msgid "Unknown project"
 msgstr "未知项目"
 
 msgid "Password successfully reset."
 msgstr "密码重置成功。"
 
+msgid "Project settings have been changed successfully."
+msgstr ""
+
 msgid "Unable to parse CSV"
 msgstr ""
 
 #, python-format
 msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
@@ -755,14 +765,17 @@
 
 msgid "History"
 msgstr "历史"
 
 msgid "Settings"
 msgstr "设置"
 
+msgid "RSS Feed"
+msgstr ""
+
 msgid "Other projects :"
 msgstr "其他项目："
 
 msgid "switch to"
 msgstr "切换到"
 
 msgid "Dashboard"
@@ -832,21 +845,20 @@
 
 msgid "No bills"
 msgstr "没有账单"
 
 msgid "Nothing to list yet."
 msgstr "没有列表。"
 
-msgid "You probably want to"
-msgstr "你想要"
-
-msgid "add a bill"
+#, fuzzy
+msgid "Add your first bill"
 msgstr "添加账单"
 
-msgid "add participants"
+#, fuzzy
+msgid "Add the first participant"
 msgstr "添加参与人"
 
 msgid "Password reminder"
 msgstr "密码提醒"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
@@ -861,49 +873,62 @@
 
 msgid "Reset your password"
 msgstr "重设密码"
 
 msgid "Invite people to join this project"
 msgstr "邀请其他人加入项目"
 
-msgid "Share Identifier & code"
-msgstr "分享标识符与码"
+msgid "Share an invitation link"
+msgstr ""
 
 msgid ""
-"You can share the project identifier and the private code by any "
-"communication means."
-msgstr "你可以通过任何通信手段分享项目标识符与专用码。"
-
-msgid "Identifier:"
-msgstr "标识符："
-
-msgid "Share the Link"
-msgstr "分享链接"
-
-msgid "You can directly share the following link via your prefered medium"
-msgstr "你可以直接通过你喜欢的媒体分享链接"
+"The easiest way to invite people is to give them the following invitation"
+" link.<br />They will be able to access the project, manage participants,"
+" add/edit/delete bills. However, they will not have access to important "
+"settings such as changing the private code or deleting the whole project."
+msgstr ""
 
 msgid "Scan QR code"
 msgstr ""
 
 msgid "Use a mobile device with a compatible app."
 msgstr ""
 
 msgid "Send via Emails"
 msgstr "邮件发送"
 
+#, fuzzy
 msgid ""
-"Specify a (comma separated) list of email adresses you want to notify "
-"about the\n"
-"                creation of this budget management project and we will "
-"send them an email for you."
+"Specify a list of email adresses (separated by comma) of people you want "
+"to notify about the creation of this project. We will send them an email "
+"with the invitation link."
 msgstr ""
 "请指定一个邮箱接收通知。\n"
 "我们会创建预算管理项目，并把它通过邮件发送给你。"
 
+msgid "Share Identifier & code"
+msgstr "分享标识符与码"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means.<br />Anyone with the private code will have access "
+"to the full project, including changing settings such as the private code"
+" or project email address, or even deleting the whole project."
+msgstr ""
+
+msgid "Identifier:"
+msgstr "标识符："
+
+#, fuzzy
+msgid "Private code:"
+msgstr "共享密钥"
+
+msgid "the private code was defined when you created the project"
+msgstr ""
+
 msgid "Who pays?"
 msgstr "谁付款？"
 
 msgid "To whom?"
 msgstr "给谁？"
 
 msgid "Who?"
@@ -1085,7 +1110,25 @@
 
 #~ msgid " show"
 #~ msgstr "显示"
 
 #~ msgid "Edit the project"
 #~ msgstr "编辑项目"
 
+#~ msgid "You probably want to"
+#~ msgstr "你想要"
+
+#~ msgid "add participants"
+#~ msgstr "添加参与人"
+
+#~ msgid ""
+#~ "You can share the project identifier "
+#~ "and the private code by any "
+#~ "communication means."
+#~ msgstr "你可以通过任何通信手段分享项目标识符与专用码。"
+
+#~ msgid "Share the Link"
+#~ msgstr "分享链接"
+
+#~ msgid "You can directly share the following link via your prefered medium"
+#~ msgstr "你可以直接通过你喜欢的媒体分享链接"
+
```

### Comparing `ihatemoney-6.0.1/ihatemoney/utils.py` & `ihatemoney-6.1.0/ihatemoney/utils.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/versioning.py` & `ihatemoney-6.1.0/ihatemoney/versioning.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.1/ihatemoney/web.py` & `ihatemoney-6.1.0/ihatemoney/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 are directly handled in the forms module.
 
 Basically, this blueprint takes care of the authentication and provides
 some shortcuts to make your life better when coding (see `pull_project`
 and `add_project_id` for a quick overview)
 """
 from functools import wraps
+import hashlib
 import json
 import os
 from urllib.parse import urlparse, urlunparse
 
 from flask import (
     Blueprint,
+    Response,
     abort,
     current_app,
     flash,
     g,
     make_response,
     redirect,
     render_template,
@@ -150,15 +152,16 @@
         project_id = entered_project_id.lower()
         project = Project.query.get(project_id)
         if not project:
             raise Redirect303(url_for(".create_project", project_id=project_id))
 
         is_admin = session.get("is_admin")
         is_invitation = endpoint == "main.join_project"
-        if session.get(project.id) or is_admin or is_invitation:
+        is_feed = endpoint == "main.feed"
+        if session.get(project.id) or is_admin or is_invitation or is_feed:
             # add project into kwargs and call the original function
             g.project = project
         else:
             # redirect to authentication page
             raise Redirect303(url_for(".authenticate", project_id=project_id))
 
 
@@ -422,15 +425,16 @@
     # Edit form
     if edit_form.validate_on_submit():
         project = edit_form.update(g.project)
 
         db.session.add(project)
         db.session.commit()
 
-        return redirect(url_for("main.list_bills"))
+        flash(_("Project settings have been changed successfully."))
+        return redirect(url_for("main.edit_project"))
     else:
         edit_form.name.data = g.project.name
 
         if g.project.logging_preference != LoggingMode.DISABLED:
             edit_form.project_history.data = True
             if g.project.logging_preference == LoggingMode.RECORD_IP:
                 edit_form.ip_recording.data = True
@@ -894,14 +898,61 @@
         members_stats=g.project.members_stats,
         monthly_stats=g.project.monthly_stats,
         months=months,
         current_view="statistics",
     )
 
 
+def build_etag(project_id, last_modified):
+    return hashlib.md5(
+        (current_app.config["SECRET_KEY"] + project_id + last_modified).encode()
+    ).hexdigest()
+
+
+@main.route("/<project_id>/feed/<string:token>.xml")
+def feed(token):
+    verified_project_id = Project.verify_token(
+        token, token_type="feed", project_id=g.project.id
+    )
+    if verified_project_id != g.project.id:
+        abort(404)
+
+    weighted_bills = g.project.get_bill_weights_ordered().paginate(
+        per_page=100, error_out=True
+    )
+
+    # This computes the last modification datetime for the project or
+    # any of the 100 latest bills. This is done by reading the issued_at
+    # attribute generated by sqlalchemy-continuum.
+    bills_last_modified = [
+        bill.versions[0].transaction.issued_at for _, bill in weighted_bills.items
+    ]
+    project_last_modified = g.project.versions[0].transaction.issued_at
+    last_modified = max(bills_last_modified + [project_last_modified])
+    etag = build_etag(g.project.id, last_modified.isoformat())
+
+    if request.if_none_match and etag in request.if_none_match:
+        return "", 304
+
+    if (
+        request.if_modified_since
+        and request.if_modified_since.replace(tzinfo=None) >= last_modified
+    ):
+        return "", 304
+
+    return Response(
+        render_template("project_feed.xml", bills=weighted_bills),
+        mimetype="application/rss+xml",
+        headers={
+            "ETag": etag,
+            "Last-Modified": last_modified.strftime("%a, %d %b %Y %H:%M:%S UTC"),
+        },
+    )
+
+
 @main.route("/dashboard")
 @requires_admin()
 def dashboard():
     is_admin_dashboard_activated = current_app.config["ACTIVATE_ADMIN_DASHBOARD"]
     return render_template(
         "dashboard.html",
         projects=Project.query.all(),
```

### Comparing `ihatemoney-6.0.1/ihatemoney.egg-info/PKG-INFO` & `ihatemoney-6.1.0/ihatemoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihatemoney
-Version: 6.0.1
+Version: 6.1.0
 Summary: A simple shared budget manager web application.
 Home-page: https://github.com/spiral-project/ihatemoney
 Author: Alexis Métaireau & contributors
 Author-email: alexis@notmyidea.org
 License: Custom BSD Beerware
 Description: UNKNOWN
 Keywords: web,budget
```

### Comparing `ihatemoney-6.0.1/ihatemoney.egg-info/SOURCES.txt` & `ihatemoney-6.1.0/ihatemoney.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 ihatemoney/templates/invitation_mail.fr.j2
 ihatemoney/templates/layout.html
 ihatemoney/templates/list_bills.html
 ihatemoney/templates/password_reminder.en.j2
 ihatemoney/templates/password_reminder.fr.j2
 ihatemoney/templates/password_reminder.html
 ihatemoney/templates/password_reminder_sent.html
+ihatemoney/templates/project_feed.xml
 ihatemoney/templates/recent_projects.html
 ihatemoney/templates/reminder_mail.en.j2
 ihatemoney/templates/reminder_mail.fr.j2
 ihatemoney/templates/reset_password.html
 ihatemoney/templates/send_invites.html
 ihatemoney/templates/settle_bills.html
 ihatemoney/templates/showcase.html
```

### Comparing `ihatemoney-6.0.1/ihatemoney.egg-info/requires.txt` & `ihatemoney-6.1.0/ihatemoney.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 psycopg2-binary<3,>=2.9.2
 
 [dev]
 Flask-Testing>=0.8.1
 black==23.3.0
 flake8==5.0.4
 isort==5.11.5
+pytest-libfaketime>=0.1.2
 pytest>=6.2.5
 tox>=3.14.6
 vermin==1.5.2
 zest.releaser>=6.20.1
 
 [doc]
 Sphinx<8,>=7.0.1
```

### Comparing `ihatemoney-6.0.1/setup.cfg` & `ihatemoney-6.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ihatemoney
-version = 6.0.1
+version = 6.1.0
 url = https://github.com/spiral-project/ihatemoney
 description = A simple shared budget manager web application.
 long_description = file: README.rst, CHANGELOG.rst
 author = Alexis Métaireau & contributors
 author_email = alexis@notmyidea.org
 keywords = web, budget
 license = Custom BSD Beerware
@@ -55,14 +55,15 @@
 dev = 
 	black==23.3.0
 	flake8==5.0.4
 	isort==5.11.5
 	vermin==1.5.2
 	Flask-Testing>=0.8.1
 	pytest>=6.2.5
+	pytest-libfaketime>=0.1.2
 	tox>=3.14.6
 	zest.releaser>=6.20.1
 doc = 
 	Sphinx>=7.0.1,<8
 	docutils==0.20.1
 	myst-parser>=2,<3
```

