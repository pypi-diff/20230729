# Comparing `tmp/tendril-interests-0.3.3.tar.gz` & `tmp/tendril-interests-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-interests-0.3.3.tar", last modified: Sat Jul 29 13:33:41 2023, max compression
+gzip compressed data, was "tendril-interests-0.3.4.tar", last modified: Sat Jul 29 15:02:45 2023, max compression
```

## Comparing `tendril-interests-0.3.3.tar` & `tendril-interests-0.3.4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.971650 tendril-interests-0.3.3/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-29 13:33:41.971650 tendril-interests-0.3.3/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.3/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-29 13:33:41.971650 tendril-interests-0.3.3/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3288 2023-07-29 05:48:32.000000 tendril-interests-0.3.3/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.3/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.3/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.3/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.3/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.3/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.3.3/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    21379 2023-07-25 18:59:57.000000 tendril-interests-0.3.3/src/tendril/apiserver/templates/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.3/src/tendril/apiserver/templates/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.963651 tendril-interests-0.3.3/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.3/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/authz/approvals/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.3/src/tendril/authz/approvals/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.3/src/tendril/authz/approvals/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.3/src/tendril/authz/approvals/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.3/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.3/src/tendril/authz/roles/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.3/src/tendril/authz/roles/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.3/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.3/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.3/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.3/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.3/src/tendril/common/interests/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.3/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.3/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.3/src/tendril/common/interests/representations.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.3/src/tendril/common/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.3/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.3/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.3/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.3/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.3/src/tendril/db/controllers/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.3/src/tendril/db/controllers/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/db/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.3/src/tendril/db/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.3/src/tendril/db/mixins/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.3/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.3/src/tendril/db/models/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.3/src/tendril/db/models/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.3/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    19016 2023-07-26 02:49:51.000000 tendril-interests-0.3.3/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.3/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.3/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17517 2023-07-29 04:40:45.000000 tendril-interests-0.3.3/src/tendril/interests/mixins/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      284 2023-07-29 03:58:12.000000 tendril-interests-0.3.3/src/tendril/interests/mixins/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6292 2023-07-29 13:33:21.000000 tendril-interests-0.3.3/src/tendril/interests/mixins/monitors.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.3/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.3/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.3/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.3/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.3/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.3/src/tendril/libraries/mixins/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.967651 tendril-interests-0.3.3/src/tendril/monitors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.3.3/src/tendril/monitors/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1062 2023-07-29 12:20:20.000000 tendril-interests-0.3.3/src/tendril/monitors/spec.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.971650 tendril-interests-0.3.3/src/tendril_interests.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-29 13:33:41.000000 tendril-interests-0.3.3/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2557 2023-07-29 13:33:41.000000 tendril-interests-0.3.3/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-29 13:33:41.000000 tendril-interests-0.3.3/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      586 2023-07-29 13:33:41.000000 tendril-interests-0.3.3/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-29 13:33:41.000000 tendril-interests-0.3.3/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:33:41.971650 tendril-interests-0.3.3/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.3/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-29 15:02:45.623826 tendril-interests-0.3.4/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.4/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-29 15:02:45.623826 tendril-interests-0.3.4/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3288 2023-07-29 05:48:32.000000 tendril-interests-0.3.4/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.611827 tendril-interests-0.3.4/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.4/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.4/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.4/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.4/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.4/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.3.4/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21379 2023-07-25 18:59:57.000000 tendril-interests-0.3.4/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.4/src/tendril/apiserver/templates/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.4/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.4/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.4/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.4/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.4/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.4/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.4/src/tendril/authz/roles/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.615826 tendril-interests-0.3.4/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.4/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.4/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.4/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.4/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.4/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.4/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.4/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.4/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.4/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.4/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.4/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.4/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.4/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.4/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.4/src/tendril/db/controllers/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.4/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.4/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.4/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.4/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.4/src/tendril/db/models/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.4/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    19016 2023-07-26 02:49:51.000000 tendril-interests-0.3.4/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.4/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.4/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17517 2023-07-29 04:40:45.000000 tendril-interests-0.3.4/src/tendril/interests/mixins/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      284 2023-07-29 03:58:12.000000 tendril-interests-0.3.4/src/tendril/interests/mixins/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6240 2023-07-29 13:52:16.000000 tendril-interests-0.3.4/src/tendril/interests/mixins/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.4/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.4/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.4/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.4/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.4/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.4/src/tendril/libraries/mixins/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril/monitors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.3.4/src/tendril/monitors/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1062 2023-07-29 12:20:20.000000 tendril-interests-0.3.4/src/tendril/monitors/spec.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/src/tendril_interests.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-29 15:02:45.000000 tendril-interests-0.3.4/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2557 2023-07-29 15:02:45.000000 tendril-interests-0.3.4/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-29 15:02:45.000000 tendril-interests-0.3.4/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      586 2023-07-29 15:02:45.000000 tendril-interests-0.3.4/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-29 15:02:45.000000 tendril-interests-0.3.4/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 15:02:45.619826 tendril-interests-0.3.4/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.4/tox.ini
```

### Comparing `tendril-interests-0.3.3/.gitignore` & `tendril-interests-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/.readthedocs.yml` & `tendril-interests-0.3.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/.travis.yml` & `tendril-interests-0.3.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/LICENSE` & `tendril-interests-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/PKG-INFO` & `tendril-interests-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.3.3
+Version: 0.3.4
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.3.3/README.rst` & `tendril-interests-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/Makefile` & `tendril-interests-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/_static/custom.css` & `tendril-interests-0.3.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/_static/favicon.ico` & `tendril-interests-0.3.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/_static/logo.png` & `tendril-interests-0.3.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/_static/logo_packed.png` & `tendril-interests-0.3.4/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/_templates/about.html` & `tendril-interests-0.3.4/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/conf.py` & `tendril-interests-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/index.rst` & `tendril-interests-0.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/docs/installation.rst` & `tendril-interests-0.3.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/setup.py` & `tendril-interests-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/apiserver/routers/interests.py` & `tendril-interests-0.3.4/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/apiserver/templates/interests.py` & `tendril-interests-0.3.4/src/tendril/apiserver/templates/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/apiserver/templates/interests_approvals.py` & `tendril-interests-0.3.4/src/tendril/apiserver/templates/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/authz/approvals/interests.py` & `tendril-interests-0.3.4/src/tendril/authz/approvals/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/authz/approvals/manager.py` & `tendril-interests-0.3.4/src/tendril/authz/approvals/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/authz/roles/interests.py` & `tendril-interests-0.3.4/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/authz/roles/interests_approvals.py` & `tendril-interests-0.3.4/src/tendril/authz/roles/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/common/interests/approvals.py` & `tendril-interests-0.3.4/src/tendril/common/interests/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/common/interests/exceptions.py` & `tendril-interests-0.3.4/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/common/interests/memberships.py` & `tendril-interests-0.3.4/src/tendril/common/interests/memberships.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/config/__init__.py` & `tendril-interests-0.3.4/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/config/interests.py` & `tendril-interests-0.3.4/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/db/controllers/interests.py` & `tendril-interests-0.3.4/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/db/controllers/interests_approvals.py` & `tendril-interests-0.3.4/src/tendril/db/controllers/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/db/models/interests.py` & `tendril-interests-0.3.4/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/db/models/interests_approvals.py` & `tendril-interests-0.3.4/src/tendril/db/models/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/interests/base.py` & `tendril-interests-0.3.4/src/tendril/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/interests/manager.py` & `tendril-interests-0.3.4/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/interests/mixins/approvals.py` & `tendril-interests-0.3.4/src/tendril/interests/mixins/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/interests/mixins/monitors.py` & `tendril-interests-0.3.4/src/tendril/interests/mixins/monitors.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
         kwargs = self._monitor_get_cache_loc(spec)
         kwargs.update({
             'deser': spec.deserializer or json.loads
         })
         value = transit.read(**kwargs)
         if spec.default is not None and not value:
             value = spec.default
-        print(f"GET {spec.publish_name()} {value}")
         return value
 
     def _monitors_at_export_level(self, export_level):
         return [x for x in self.monitors_spec if x.export_level <= export_level]
 
     def export(self, session=None, auth_user=None, **kwargs):
         rv = {}
```

### Comparing `tendril-interests-0.3.3/src/tendril/libraries/interests/base.py` & `tendril-interests-0.3.4/src/tendril/libraries/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/libraries/interests/manager.py` & `tendril-interests-0.3.4/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril/monitors/spec.py` & `tendril-interests-0.3.4/src/tendril/monitors/spec.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril_interests.egg-info/PKG-INFO` & `tendril-interests-0.3.4/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.3.3
+Version: 0.3.4
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.3.3/src/tendril_interests.egg-info/SOURCES.txt` & `tendril-interests-0.3.4/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/src/tendril_interests.egg-info/requires.txt` & `tendril-interests-0.3.4/src/tendril_interests.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/tests/coveralls.py` & `tendril-interests-0.3.4/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.3/tox.ini` & `tendril-interests-0.3.4/tox.ini`

 * *Files identical despite different names*

