# Comparing `tmp/cmdix-2.0.2.tar.gz` & `tmp/cmdix-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdix-2.0.2.tar", last modified: Mon Jun 19 21:50:37 2023, max compression
+gzip compressed data, was "cmdix-3.0.0.tar", last modified: Sat Jul 29 17:44:13 2023, max compression
```

## Comparing `cmdix-2.0.2.tar` & `cmdix-3.0.0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-19 21:50:18.000000 cmdix-2.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-19 21:50:18.000000 cmdix-2.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-19 21:50:18.000000 cmdix-2.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-19 21:50:18.000000 cmdix-2.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-19 21:50:18.000000 cmdix-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 21:50:18.000000 cmdix-2.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 21:50:18.000000 cmdix-2.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-19 21:50:18.000000 cmdix-2.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-19 21:50:18.000000 cmdix-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-19 21:50:37.731521 cmdix-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-19 21:50:18.000000 cmdix-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/cmdix/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4795 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/cmdix/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/basename.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/bunzip2.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/bzip2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/cal.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/chown.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/chroot.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/crond.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/dirname.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/gunzip.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/httpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/ln.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/md5sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mkdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mktemp.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/rmdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sendmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sh.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha1sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha224sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha256sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha384sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha512sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/shred.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/shuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/touch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/uname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/wc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/wget.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/yes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/cmdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 21:50:18.000000 cmdix-2.0.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-19 21:50:18.000000 cmdix-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-19 21:50:18.000000 cmdix-2.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 21:50:18.000000 cmdix-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 21:50:18.000000 cmdix-2.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-19 21:50:18.000000 cmdix-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-19 21:50:18.000000 cmdix-2.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-19 21:50:37.731521 cmdix-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_cp.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_md5sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_onlyunix.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_pycoreutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_pycoreutils_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-19 21:50:18.000000 cmdix-2.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.749660 cmdix-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-29 17:43:53.000000 cmdix-3.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-29 17:43:53.000000 cmdix-3.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.729660 cmdix-3.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-29 17:43:53.000000 cmdix-3.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.729660 cmdix-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-29 17:43:53.000000 cmdix-3.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-29 17:43:53.000000 cmdix-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 17:43:53.000000 cmdix-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-29 17:43:53.000000 cmdix-3.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-29 17:43:53.000000 cmdix-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-29 17:43:53.000000 cmdix-3.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-29 17:44:13.749660 cmdix-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-29 17:43:53.000000 cmdix-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.733660 cmdix-3.0.0/cmdix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4752 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.745660 cmdix-3.0.0/cmdix/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/bunzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/chown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/crond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/dirname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/gunzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/httpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/rmdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sendmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sha1sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sha224sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sha256sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sha384sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sha512sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/shred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/shuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/touch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/uname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/wget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/yes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/command/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.745660 cmdix-3.0.0/cmdix/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-29 17:43:53.000000 cmdix-3.0.0/cmdix/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.733660 cmdix-3.0.0/cmdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-29 17:44:13.000000 cmdix-3.0.0/cmdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-29 17:44:13.000000 cmdix-3.0.0/cmdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:44:13.000000 cmdix-3.0.0/cmdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-29 17:44:13.000000 cmdix-3.0.0/cmdix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-29 17:44:13.000000 cmdix-3.0.0/cmdix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 17:44:13.000000 cmdix-3.0.0/cmdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-29 17:43:53.000000 cmdix-3.0.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.749660 cmdix-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-29 17:43:53.000000 cmdix-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 17:43:53.000000 cmdix-3.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-29 17:43:53.000000 cmdix-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-29 17:43:53.000000 cmdix-3.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 17:43:53.000000 cmdix-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-29 17:43:53.000000 cmdix-3.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-29 17:44:13.753660 cmdix-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:44:13.749660 cmdix-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_onlyunix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_pycoreutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_pycoreutils_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-29 17:43:53.000000 cmdix-3.0.0/tests/test_uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 17:43:53.000000 cmdix-3.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-29 17:43:53.000000 cmdix-3.0.0/tox.ini
```

### Comparing `cmdix-2.0.2/.github/workflows/main.yml` & `cmdix-3.0.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -38,68 +38,63 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        # tests hang on Python < 3.9
-        #- python: "3.8"
-        #  platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         # disabled for #11
         #- python: pypy3.9
         #  platform: ubuntu-latest
         
         # tests hang on Python < 3.9
         exclude:
-        - python: "3.7"
+        - python: "3.8"
           platform: macos-latest
-        - python: "3.7"
+        - python: "3.8"
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -122,16 +117,16 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `cmdix-2.0.2/Dockerfile` & `cmdix-3.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/LICENSE` & `cmdix-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/PKG-INFO` & `cmdix-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 2.0.2
+Version: 3.0.0
 Summary: Unix commands in Pure Python
 Home-page: https://github.com/jaraco/cmdix
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
    :target: https://pypi.org/project/cmdix
```

### Comparing `cmdix-2.0.2/README.rst` & `cmdix-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/__init__.py` & `cmdix-3.0.0/cmdix/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 import argparse
 import os
 import shlex
 import platform
+from importlib import metadata
 
-import importlib_metadata as metadata
 import importlib_resources as resources
 
 from . import command
 from .exception import CommandNotFoundException
 
 
 __version__ = metadata.version(__name__)
@@ -41,15 +41,15 @@
         return not (needs_unix and is_windows)
     except CommandNotFoundException:
         return False
 
 
 def _get_command(name):
     # Try to import the command module
-    importstring = 'cmdix.command.{0}'.format(name)
+    importstring = f'cmdix.command.{name}'
     try:
         return __import__(importstring, fromlist=1).parseargs
     except ImportError:
         raise CommandNotFoundException(name)
 
 
 def getcommand(commandname):
@@ -71,15 +71,15 @@
     all = (path.stem for path in paths if not path.name.startswith('_'))
     return filter(_is_available, all)
 
 
 def _gen_script_definitions():
     print('console_scripts =')
     for cmd in listcommands():
-        print('\t{cmd} = cmdix:run'.format(**locals()))
+        print(f'\t{cmd} = cmdix:run')
 
 
 def get_parser(commandname):
     parser = argparse.ArgumentParser(
         add_help=False,
         description="Coreutils in Pure Python.",
         prog=commandname,
@@ -154,15 +154,15 @@
 def run_subcommand(commandname, argv):
     """
     Run the subcommand
     """
     try:
         cmd = getcommand(commandname)
     except CommandNotFoundException:
-        print("Command `{0}` not found.".format(commandname), file=sys.stderr)
+        print(f"Command `{commandname}` not found.", file=sys.stderr)
         return
     p = cmd(argparse.ArgumentParser(prog=commandname))
     args = p.parse_args(argv)
     args.func(args)
 
 
 def runcommandline(commandline):
```

### Comparing `cmdix-2.0.2/cmdix/command/base64.py` & `cmdix-3.0.0/cmdix/command/base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/basename.py` & `cmdix-3.0.0/cmdix/command/basename.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/cal.py` & `cmdix-3.0.0/cmdix/command/cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/cat.py` & `cmdix-3.0.0/cmdix/command/cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/chmod.py` & `cmdix-3.0.0/cmdix/command/chmod.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/chown.py` & `cmdix-3.0.0/cmdix/command/chown.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,12 @@
 
 
 def func(args):
     if not args.owner:
         try:
             user = pwd.getpwnam(args.owner)
         except KeyError:
-            raise StdErrException(
-                "{0}: invalid user: '{1}'".format(args.prog, args.owner)
-            )
+            raise StdErrException(f"{args.prog}: invalid user: '{args.owner}'")
         uid = user.pw_uid
 
     for arg in args.FILE:
         os.chown(arg, int(uid), -1)
```

### Comparing `cmdix-2.0.2/cmdix/command/chroot.py` & `cmdix-3.0.0/cmdix/command/chroot.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/cp.py` & `cmdix-3.0.0/cmdix/command/cp.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 def handle_direct(_copy, args, dest, src):
     name = os.path.basename(src)
     dstfile = os.path.join(dest, name) if os.path.isdir(dest) else dest
     _copy(src, dstfile)
     if args.verbose:
-        print("'{0}' -> '{1}'".format(src, dstfile))
+        print(f"'{src}' -> '{dstfile}'")
 
 
 def walk(_copy, args, dest, src):
     # Walk the source directory
     for root, dirnames, filenames in os.walk(src):
         if root == dest:
             continue
@@ -83,24 +83,24 @@
 
         # Create subdirectories in destination directory
         for subdir in dirnames:
             dstdir = os.path.join(dest, dstmid, subdir)
             if not os.path.exists(dest):
                 os.mkdir(dstdir)
             if args.verbose:
-                print("'{0}' -> '{1}'".format(root, dstdir))
+                print(f"'{root}' -> '{dstdir}'")
 
         # Copy file
         for filename in filenames:
             dstfile = os.path.join(dest, dstmid, filename)
             srcfile = os.path.join(root, filename)
             if args.interactive and os.path.exists(dstfile):
                 q = input(
-                    "{0}: {1} already ".format(args.prog, dstfile)
+                    f"{args.prog}: {dstfile} already "
                     + "exists; do you wish to overwrite (y or n)?"
                 )
                 if q.upper() != 'Y':
                     exception.StdOutException("not overwritten", 2)
                     continue
             _copy(srcfile, dstfile)
             if args.verbose:
-                print("'{0}' -> '{1}'".format(srcfile, dstfile))
+                print(f"'{srcfile}' -> '{dstfile}'")
```

### Comparing `cmdix-2.0.2/cmdix/command/crond.py` & `cmdix-3.0.0/cmdix/command/crond.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,31 +73,31 @@
             and job.hour in ['*', now.tm_hour]
             and job.mday in ['*', now.tm_mday]
             and job.mon in ['*', now.tm_mon]
             and job.wday in ['*', now.tm_wday]
         ):
             cmd = job.cmd
             if args.verbose:
-                logger.info("Running job {0}".format(cmd))
+                logger.info(f"Running job {cmd}")
 
             if args.dryrun:
                 break
 
             # Run the command
             stdout, stderr = subprocess.Popen(
                 cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True
             ).communicate()
             if args.verbose:
                 if stdout:
-                    logger.info("{0}: {1}".format(cmd, stdout.strip()))
+                    logger.info(f"{cmd}: {stdout.strip()}")
                 if stderr:
-                    logger.error("{0}: {1}".format(cmd, stderr.strip()))
+                    logger.error(f"{cmd}: {stderr.strip()}")
         else:
             if args.verbose:
-                logger.info("Skipping job {0}".format(job))
+                logger.info(f"Skipping job {job}")
 
 
 def read_and_load(Job, args, joblist):
     # Read crontab and load jobs
     for line in lib.parsefilelist(args.FILE):
         # Strip comments and split the string
         split = line.strip().partition('#')[0].split(None, 6)
@@ -109,10 +109,10 @@
                 mon=split[3],
                 wday=split[4],
                 user=split[5],
                 cmd=split[6],
             )
             joblist.append(job)
             if args.verbose:
-                print('Read {0}'.format(job))
+                print(f'Read {job}')
         elif split:
-            print('Ignoring invalid line {0}'.format(line))
+            print(f'Ignoring invalid line {line}')
```

### Comparing `cmdix-2.0.2/cmdix/command/diff.py` & `cmdix-3.0.0/cmdix/command/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,24 +47,24 @@
 def func(args):
     # Get modification times
     fromdate = time.ctime(os.stat(args.FILE1).st_mtime)
     todate = time.ctime(os.stat(args.FILE2).st_mtime)
 
     # Open fromfile
     try:
-        with open(args.FILE1, 'U') as fd:
+        with open(args.FILE1) as fd:
             fromlines = fd.readlines()
-    except IOError:
+    except OSError:
         print("Error opening file " + args.FILE1, file=sys.stderr)
 
     # Open tofile
     try:
-        with open(args.FILE2, 'U') as fd:
+        with open(args.FILE2) as fd:
             tolines = fd.readlines()
-    except IOError:
+    except OSError:
         print("Error opening file " + args.FILE2, file=sys.stderr)
 
     # Create diff
     if args.unified:
         diff = difflib.unified_diff(
             fromlines, tolines, args.FILE1, args.FILE2, fromdate, todate, n=args.lines
         )
```

### Comparing `cmdix-2.0.2/cmdix/command/dirname.py` & `cmdix-3.0.0/cmdix/command/dirname.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/env.py` & `cmdix-3.0.0/cmdix/command/env.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/expand.py` & `cmdix-3.0.0/cmdix/command/expand.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/httpd.py` & `cmdix-3.0.0/cmdix/command/httpd.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,22 @@
                 if self.userdict[username] == password:
                     return self.app(environ, start_response)
 
         return wsgierror(
             start_response,
             401,
             "Authentication required",
-            [(b'WWW-Authenticate', b'Basic realm={0}'.format(self.realm))],
+            [(b'WWW-Authenticate', b'Basic realm={}'.format(self.realm))],
         )
 
 
 def wsgierror(start_response, code, text, headers=[]):
     h = [(b'Content-Type', b'text/html')]
     h.extend(headers)
-    start_response(b'{0} '.format(code), h)
+    start_response(b'{} '.format(code), h)
     return [
         b'''<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN"><html><head>
                 <title>{code} {text}</title></head><body><h1>{code} {text}</h1>
                 </body></html>'''.format(
             code=code, text=text
         )
     ]
@@ -140,16 +140,16 @@
         sys.stderr = sys.__stderr__
         stdoutio.seek(0)
         stderrio.seek(0)
         stdoutstr = ''.join(stdoutio.readlines())
         stderrstr = ''.join(stderrio.readlines())
         start_response(b'200 ', [(b'Content-Type', b'text/html')])
         return [
-            str("<div class='stdout'>{0}</div>").format(stdoutstr),
-            str("<div class='stderr'>{0}</div>").format(stderrstr),
+            "<div class='stdout'>{}</div>".format(stdoutstr),
+            "<div class='stderr'>{}</div>".format(stderrstr),
         ]
     else:
         html = template.format(
             title='Cmdix Console',
             css=css,
             banner=cmdix.showbanner(),
             javascript=javascript,
@@ -199,23 +199,23 @@
         else:
             filelist.append(file)
 
     dirlist.sort()
     filelist.sort()
 
     res = '<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">\n'
-    res += '<html><head><title>{0}</title></head><body>\n'.format(path)
+    res += f'<html><head><title>{path}</title></head><body>\n'
     res += '<big><strong>Listing %s</strong></big><br>\n' % (path)
     if path != '/':
         item = '..'
-        res += 'D <a href=%s>%s</a><br/>\n' % (urljoin(path, item), item)
+        res += 'D <a href={}>{}</a><br/>\n'.format(urljoin(path, item), item)
     for item in dirlist:
-        res += 'D <a href=%s>%s</a><br/>\n' % (urljoin(path, item), item)
+        res += 'D <a href={}>{}</a><br/>\n'.format(urljoin(path, item), item)
     for item in filelist:
-        res += 'F <a href=%s>%s</a><br/>\n' % (urljoin(path, item), item)
+        res += 'F <a href={}>{}</a><br/>\n'.format(urljoin(path, item), item)
     res += '</body></html>'
     return str(res)
 
 
 def parseargs(p):
     """
     Add arguments and `func` to `p`.
```

### Comparing `cmdix-2.0.2/cmdix/command/id.py` & `cmdix-3.0.0/cmdix/command/id.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,8 +82,8 @@
         return uid
 
     if args.name:
         exception.StdErrException(
             "id: cannot print only names " + "or real IDs in default format"
         )
 
-    print("uid={0}({1}) gid={2}({3})".format(uid, username, gid, username))
+    print(f"uid={uid}({username}) gid={gid}({username})")
```

### Comparing `cmdix-2.0.2/cmdix/command/init.py` & `cmdix-3.0.0/cmdix/command/init.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/kill.py` & `cmdix-3.0.0/cmdix/command/kill.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,44 +46,42 @@
     if list(signals.values()).count(sig):
         sigint = sig
     elif sig in signals:
         sigint = signals[sig]
     elif sig.lstrip('SIG') in signals:
         sigint = signals[sig.lstrip('SIG')]
     else:
-        raise exception.StdErrException(
-            "kill: {0}: invalid signal specification".format(sig)
-        )
+        raise exception.StdErrException(f"kill: {sig}: invalid signal specification")
 
     for pid in args.pid:
         try:
             pid = int(pid)
         except ValueError:
             raise exception.StdErrException(
-                "kill: {0}: arguments must be process or job IDs".format(pid)
+                f"kill: {pid}: arguments must be process or job IDs"
             )
 
         os.kill(pid, sigint)
 
 
 def add_arguments(p, signals):
     # Add a string option for each signal
     for name, sigint in list(signals.items()):
         signame = 'SIG' + name.upper()
         p.add_argument(
             "--" + signame,
             action="store_const",
             dest="signal",
             const=sigint,
-            help="send signal {0}".format(signame),
+            help=f"send signal {signame}",
         )
 
     # Add an integer option for each signal
     for sigint in set(signals.values()):
         if sigint < 10:
             p.add_argument(
                 "-%i" % sigint,
                 action="store_const",
                 dest="signal",
                 const=sigint,
-                help="send signal {0}".format(sigint),
+                help=f"send signal {sigint}",
             )
```

### Comparing `cmdix-2.0.2/cmdix/command/ln.py` & `cmdix-3.0.0/cmdix/command/ln.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/logger.py` & `cmdix-3.0.0/cmdix/command/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         port = args.port or 514
         address = (host, port)
     else:
         address = '/dev/log'
 
     handler = logging.handlers.SysLogHandler(address, facility)
     if facility not in handler.facility_names:
-        err = "Unknown facility {0}. ".format(facility) + "Valid facilities are: "
+        err = f"Unknown facility {facility}. " + "Valid facilities are: "
         facilitylist = list(handler.facility_names.keys())
         facilitylist.sort()
         for f in facilitylist:
             err += f + ", "
 
         raise StdErrException(err)
```

### Comparing `cmdix-2.0.2/cmdix/command/ls.py` & `cmdix-3.0.0/cmdix/command/ls.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,42 +18,55 @@
         + "directory by default). Sort entries "
         + "alphabetically if none of -cftuvSUX nor --sort."
     )
     p.add_argument('FILE', nargs="*")
     p.add_argument(
         "-l", "--longlist", action="store_true", help="use a long listing format"
     )
+    p.add_argument(
+        "-a",
+        "--all",
+        dest="filter",
+        default=hide_dot,
+        action="store_const",
+        const=None,
+        help="show all files",
+    )
     return p
 
 
+def hide_dot(filename):
+    return not filename.startswith('.')
+
+
 def func(args):
     filelist = args.FILE
     if not args.FILE:
         filelist = ['.']
 
     for arg in filelist:
         dirlist = os.listdir(arg)
         dirlist.sort()
         ell = []
         sizelen = 0  # Length of the largest filesize integer
         nlinklen = 0  # Length of the largest nlink integer
-        for f in dirlist:
+        for f in filter(args.filter, dirlist):
             path = os.path.join(arg, f)
             if not args.longlist:
                 print(f)
             else:
                 st = os.lstat(path)
                 mode = lib.mode2string(st.st_mode)
                 nlink = st.st_nlink
                 uid = st.st_uid
                 gid = st.st_gid
                 size = st.st_size
                 mtime = time.localtime(st.st_mtime)
                 if stat.S_ISLNK(st.st_mode):
-                    f += " -> {0}".format(os.readlink(path))
+                    f += f" -> {os.readlink(path)}"
                 ell.append((mode, nlink, uid, gid, size, mtime, f))
 
                 # Update sizelen
                 _sizelen = len(str(size))
                 if _sizelen > sizelen:
                     sizelen = _sizelen
```

### Comparing `cmdix-2.0.2/cmdix/command/mkdir.py` & `cmdix-3.0.0/cmdix/command/mkdir.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,12 +48,12 @@
                 pathlist.insert(0, path)
                 path, tail = os.path.split(path)
 
             # Create all directories in pathlist
             for path in pathlist:
                 os.mkdir(path, int(args.mode))
                 if args.verbose:
-                    print("mkdir: created directory '{0}'".format(path))
+                    print(f"mkdir: created directory '{path}'")
         else:
             os.mkdir(arg, int(args.mode))
             if args.verbose:
-                print("mkdir: created directory '{0}'".format(arg))
+                print(f"mkdir: created directory '{arg}'")
```

### Comparing `cmdix-2.0.2/cmdix/command/mktemp.py` & `cmdix-3.0.0/cmdix/command/mktemp.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/more.py` & `cmdix-3.0.0/cmdix/command/more.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/mount.py` & `cmdix-3.0.0/cmdix/command/mount.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if args.SOURCE and args.DEST:
         mount_c(args.SOURCE, args.DEST, args.types, args.verbose)
     elif args.SOURCE or args.all:
         # Read fstab
         try:
             with open('/etc/fstab') as fd:
                 lines = fd.readlines()
-        except IOError:
+        except OSError:
             print("Error: Couldn't read /etc/ftab", file=sys.stderr)
             return
 
         # Mount filesystem
         mounted_something = False
         for line in lines:
             line = line.partition('#')[0]  # Remove comments
@@ -65,38 +65,36 @@
                 mounted_something = True
         if not mounted_something:
             print(args.SOURCE + " not found in /etc/fstab", file=sys.stderr)
     else:
         # Display currently mounted filesystems
         try:
             print(open('/etc/mtab').read().strip())
-        except IOError:
+        except OSError:
             print("Error: Couldn't read /etc/mtab", file=sys.stderr)
 
 
 def mount_c(source, dest, fstype, options=0, data='', verbose=False):
     """
     Frontend to libc mount
     """
     if verbose:
-        print("Trying to mount {0} on {1} as type {2}".format(source, dest, fstype))
+        print(f"Trying to mount {source} on {dest} as type {fstype}")
     libc = ctypes.CDLL(ctypes.util.find_library('c'))
     res = libc.mount(str(source), str(dest), str(fstype), options, str(data))
     if res < 0:
-        print(
-            "Error: Mounting {0} on {1} failed!".format(source, dest), file=sys.stderr
-        )
+        print(f"Error: Mounting {source} on {dest} failed!", file=sys.stderr)
 
 
 def get_available_filesystems():
     ell = []
     try:
         with open('/proc/filesystems') as fd:
             for line in fd.readlines():
                 ell.append(line.split()[-1])
-    except IOError:
+    except OSError:
         print(
             "Error reading supported filesystems from /proc/filesystems",
             file=sys.stderr,
         )
         return ell
     return ell
```

### Comparing `cmdix-2.0.2/cmdix/command/mv.py` & `cmdix-3.0.0/cmdix/command/mv.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,10 +25,10 @@
     )
     return p
 
 
 def func(args):
     for src in args.SOURCE:
         if args.verbose:
-            print("'{0}' -> '{1}'".format(src, args.DEST))
+            print(f"'{src}' -> '{args.DEST}'")
 
         shutil.move(src, args.DEST)
```

### Comparing `cmdix-2.0.2/cmdix/command/nl.py` & `cmdix-3.0.0/cmdix/command/nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/pwd.py` & `cmdix-3.0.0/cmdix/command/pwd.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/rm.py` & `cmdix-3.0.0/cmdix/command/rm.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,22 +50,22 @@
     if args.recursive and os.path.isdir(arg):
         # Remove directory recursively
         for root, dirs, files in os.walk(arg, topdown=False, onerror=_raise):
             for name in files:
                 path = os.path.join(root, name)
                 os.remove(path)
                 if args.verbose:
-                    print("Removed file '{0}'\n".format(path))
+                    print(f"Removed file '{path}'\n")
             for name in dirs:
                 path = os.path.join(root, name)
                 os.rmdir(path)
                 if args.verbose:
-                    print("Removed directory '{0}'\n".format(path))
+                    print(f"Removed directory '{path}'\n")
         os.rmdir(arg)
     else:
         # Remove single file
         try:
             os.remove(arg)
             if args.verbose:
-                print("Removed '{0}'\n".format(arg))
+                print(f"Removed '{arg}'\n")
         except OSError as err:
             _raise(err)
```

### Comparing `cmdix-2.0.2/cmdix/command/rmdir.py` & `cmdix-3.0.0/cmdix/command/rmdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/sendmail.py` & `cmdix-3.0.0/cmdix/command/sendmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         help="certificate file to use. implies '-s'",
     )
     p.add_argument(
         "-f",
         "-r",
         "--sender",
         dest="sender",
-        default="{0}@{1}".format(lib.getcurrentusername(), platform.node()),
+        default=f"{lib.getcurrentusername()}@{platform.node()}",
         help="set the envelope sender address",
     )
     p.add_argument(
         "-k", "--keyfile", dest="keyfile", help="key file to use. implies '-s'"
     )
     p.add_argument(
         "-m",
```

### Comparing `cmdix-2.0.2/cmdix/command/seq.py` & `cmdix-3.0.0/cmdix/command/seq.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/sh.py` & `cmdix-3.0.0/cmdix/command/sh.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def do_shell(self, line):
         """
         Run when them command is '!' or 'shell'.
         Execute the line using the Python interpreter.
         i.e. "!dir()"
         """
         try:
-            exec("r = {0}".format(line))
+            exec(f"r = {line}")
         except Exception as err:
             return pprint.pformat(err) + '\n'
         else:
             return pprint.pformat(line) + '\n'
 
     def emptyline(self):
         """
```

### Comparing `cmdix-2.0.2/cmdix/command/shred.py` & `cmdix-3.0.0/cmdix/command/shred.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/shuf.py` & `cmdix-3.0.0/cmdix/command/shuf.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,16 +84,14 @@
         lines = lines[0 : int(args.headcount)]
     for line in lines:
         outfd.write(line + '\n')
 
 
 def echo(args, outfd):
     if args.inputrange:
-        exception.StdErrException(
-            "{0}: cannot combine -e and -i options".format(args.prog)
-        )
+        exception.StdErrException(f"{args.prog}: cannot combine -e and -i options")
     lines = args.file
     random.shuffle(lines)
     if args.headcount:
         lines = lines[0 : int(args.headcount)]
     for line in lines:
         outfd.write(line + '\n')
```

### Comparing `cmdix-2.0.2/cmdix/command/sleep.py` & `cmdix-3.0.0/cmdix/command/sleep.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/sort.py` & `cmdix-3.0.0/cmdix/command/sort.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/tail.py` & `cmdix-3.0.0/cmdix/command/tail.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                     print(line, end='')
     else:
         for fd in fds:
             pos, lines = args.lines + 1, []
             while len(lines) <= args.lines:
                 try:
                     fd.seek(-pos, 2)
-                except IOError:
+                except OSError:
                     fd.seek(0)
                     break
                 finally:
                     lines = list(fd)
                 pos *= 2
             for line in lines[-args.lines :]:
                 print(line, end='')
```

### Comparing `cmdix-2.0.2/cmdix/command/tar.py` & `cmdix-3.0.0/cmdix/command/tar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from ..exception import StdErrException
 import sys
 import tarfile
+import contextlib
+
+from ..exception import StdErrException
 
 
 def parseargs(p):
     """
     Add arguments and `func` to `p`.
 
     :param p: ArgumentParser
@@ -24,96 +26,87 @@
         "Files that end with '.bz2' or '.gz' are decompressed " + "automatically."
     )
     p.add_argument('FILE', nargs="*")
     p.add_argument(
         "-c",
         "--create",
         action="store_true",
-        dest="create",
         help="create zipfile from source.",
     )
     p.add_argument(
         "-t", "--list", action="store_true", dest="list", help="list files in zipfile."
     )
     p.add_argument(
         "-x",
         "--extract",
         action="store_true",
-        dest="extract",
         help="extract tarfile into current directory.",
     )
     p.add_argument(
         "-j",
         "--bzip2",
         action="store_true",
-        dest="bzip2",
         help="(de)compress using bzip2",
     )
     p.add_argument(
         "-f", "--file", dest="archive", help="use archive file or device ARCHIVE"
     )
-    p.add_argument(
-        "-z", "--gzip", action="store_true", dest="gzip", help="(de)compress using gzip"
-    )
+    p.add_argument("-z", "--gzip", action="store_true", help="(de)compress using gzip")
     return p
 
 
+@contextlib.contextmanager
+def _open_fallback(filename, fallback=sys.stdin, mode='r'):
+    if not filename:
+        yield fallback
+        return
+
+    with open(filename, mode=mode) as fd:
+        yield fd
+
+
 def func(args):
     if bool(args.list) + bool(args.create) + bool(args.extract) > 1:
         print("You may not specify more than one of '-ctx'", file=sys.stderr)
         sys.exit(2)
 
     if args.extract or args.list:
-        if args.archive:
-            infile = open(args.archive, 'rb')
-        else:
-            infile = sys.stdin
-        try:
-            tar = tarfile.open(fileobj=infile)
-        except tarfile.TarError:
-            raise StdErrException(
-                "Could not parse file {0}. Are you sure it is a tar-archive?".format(
-                    infile.name
+        with _open_fallback(args.archive, mode='rb') as infile:
+            try:
+                with tarfile.open(fileobj=infile) as tar:
+                    if args.extract:
+                        tar.extractall()
+
+                    elif args.list:
+                        list_(tar)
+
+            except tarfile.TarError:
+                raise StdErrException(
+                    "Could not parse file {}. Are you sure it is a tar-archive?".format(
+                        infile.name
+                    )
                 )
-            )
-
-    if args.extract:
-        tar.extractall()
-        tar.close()
-
-    elif args.list:
-        list_(tar)
 
     elif args.create:
         create(args)
     else:
         print("Either '-c', '-t' or '-x' should be specified", file=sys.stderr)
 
 
 def list_(tar):
     for tarinfo in tar:
-        name = tarinfo.name
-        if tarinfo.isdir():
-            name += '/'
-        print(name)
-    tar.close()
+        print(tarinfo.name + '/' * tarinfo.isdir())
 
 
 def create(args):
-    # Set outfile
-    if args.archive:
-        outfile = open(args.archive, 'wb')
-    else:
-        outfile = sys.stout
-    # Set mode
-    if args.gzip:
-        mode = 'w:gz'
-    elif args.bzip2:
-        mode = 'w:bz2'
-    else:
-        mode = 'w'
-    tar = tarfile.open(fileobj=outfile, mode=mode)
-    for arg in args.FILE:
-        tar.add(arg)
-    tar.close()
-    if args.archive:
-        outfile.close()
+    with _open_fallback(args.archive, mode='wb', fallback=sys.stdout) as outfile:
+        # Set mode
+        if args.gzip:
+            mode = 'w:gz'
+        elif args.bzip2:
+            mode = 'w:bz2'
+        else:
+            mode = 'w'
+
+        with tarfile.open(fileobj=outfile, mode=mode) as tar:
+            for arg in args.FILE:
+                tar.add(arg)
```

### Comparing `cmdix-2.0.2/cmdix/command/tee.py` & `cmdix-3.0.0/cmdix/command/tee.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/touch.py` & `cmdix-3.0.0/cmdix/command/touch.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/uname.py` & `cmdix-3.0.0/cmdix/command/uname.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import platform
 import subprocess
-import io
 import re
 import contextlib
 
 
 def parseargs(p):
     """
     Add arguments and `func` to `p`.
@@ -89,15 +88,15 @@
     )
     return p
 
 
 def processor_from_cpu_info():
     pattern = re.compile(r'model name\s+: (.*)')
     try:
-        with io.open('/proc/cpuinfo') as lines:
+        with open('/proc/cpuinfo') as lines:
             matched = next(filter(pattern.match, lines))
             return pattern.match(matched).group(1)
     except Exception:
         pass
 
 
 def get_processor():
@@ -108,15 +107,15 @@
     the info another way.
     """
     if platform.system() == 'Windows':
         return platform.processor()
 
     if platform.system() == 'Darwin':
         cmd = 'sysctl -n machdep.cpu.brand_string'.split()
-        return subprocess.check_output(cmd, universal_newlines=True).strip()
+        return subprocess.check_output(cmd, text=True).strip()
 
     return processor_from_cpu_info() or 'unknown'
 
 
 @contextlib.contextmanager
 def patch_syscmd_uname():
     """
```

### Comparing `cmdix-2.0.2/cmdix/command/uptime.py` & `cmdix-3.0.0/cmdix/command/uptime.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,11 +27,11 @@
         uptime = str(datetime.timedelta(seconds=uptimeseconds))[:-10]
 
     with open('/proc/loadavg') as f:
         load5, load10, load15, proc, unknown = f.readline().split()[:5]
         totproc, avgproc = proc.split('/')
 
     print(
-        " {0:%H:%M:%S} up ".format(datetime.datetime.today())
-        + " {0},  {1} users,  ".format(uptime, 'TODO')
-        + "load average: {0}, {1}, {2}".format(load5, load10, load15)
+        f" {datetime.datetime.today():%H:%M:%S} up "
+        + " {},  {} users,  ".format(uptime, 'TODO')
+        + f"load average: {load5}, {load10}, {load15}"
     )
```

### Comparing `cmdix-2.0.2/cmdix/command/uuidgen.py` & `cmdix-3.0.0/cmdix/command/uuidgen.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/watch.py` & `cmdix-3.0.0/cmdix/command/watch.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,14 +49,14 @@
             text = addsts(args.seconds, cmd, text, sts)
     finally:
         curses.endwin()
 
 
 def addsts(interval, cmd, text, sts):
     now = time.strftime("%H:%M:%S")
-    text = "%s, every %g sec: %s\n%s" % (now, interval, cmd, text)
+    text = "{}, every {:g} sec: {}\n{}".format(now, interval, cmd, text)
     if sts:
         msg = "Exit status: %d; signal: %d" % (sts >> 8, sts & 0xFF)
         if text and not text.endswith("\n"):
             msg = "\n" + msg
         text += msg
     return text
```

### Comparing `cmdix-2.0.2/cmdix/command/wc.py` & `cmdix-3.0.0/cmdix/command/wc.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/cmdix/command/wget.py` & `cmdix-3.0.0/cmdix/command/wget.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,14 @@
     opener = build_opener()
     opener.addheaders = [('User-agent', useragent)]
 
     for url in args.url:
         try:
             fdin = opener.open(url)
         except HTTPError as e:
-            exception.StdErrException("HTTP error opening {0}: {1}".format(url, e))
+            exception.StdErrException(f"HTTP error opening {url}: {e}")
 
         length = int(fdin.headers['content-length'])
-        print("Getting {0} bytes from {1}...".format(length, url))
+        print(f"Getting {length} bytes from {url}...")
 
         shutil.copyfileobj(fdin, fdout)
         print("Done")
```

### Comparing `cmdix-2.0.2/cmdix/command/zip.py` & `cmdix-3.0.0/cmdix/command/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def addToZip(zf, path, zippath):
         if os.path.isfile(path):
             zf.write(path, zippath, zipfile.ZIP_DEFLATED)
         elif os.path.isdir(path):
             for nm in os.listdir(path):
                 addToZip(zf, os.path.join(path, nm), os.path.join(zippath, nm))
         else:
-            exception.StdErrException("Can't store {0}".format(path))
+            exception.StdErrException(f"Can't store {path}")
 
     zf = zipfile.ZipFile(args[0], 'w', allowZip64=True)
     for src in args[1:]:
         addToZip(zf, src, os.path.basename(src))
     zf.close()
 
 
@@ -111,18 +111,18 @@
 def test(args):
     if len(args) != 1:
         args.parser.print_usage(sys.stderr)
         sys.exit(1)
     zf = zipfile.ZipFile(args[0], 'r')
     badfile = zf.testzip()
     if badfile:
-        sys.stderr("Error on file {0}\n".format(badfile))
+        sys.stderr(f"Error on file {badfile}\n")
         sys.exit(1)
     else:
-        print("{0} tested ok".format(args[0]) + "\n")
+        print(f"{args[0]} tested ok" + "\n")
         sys.exit(0)
 
 
 def list_(args):
     if len(args) != 1:
         args.parser.print_usage(sys.stderr)
         sys.exit(1)
```

### Comparing `cmdix-2.0.2/cmdix/compressor.py` & `cmdix-3.0.0/cmdix/compressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     zippath = infile + suffix
     infile = open(infile, 'rb')
     if len(args.FILE) == 0 or args.stdout:
         outfile = sys.stdout
     else:
         if os.path.exists(zippath):
             q = input(
-                "{0}: {1} ".format(args.prog, zippath)
+                f"{args.prog}: {zippath} "
                 + "already exists; do you wish to overwrite (y or n)? "
             )
             if q.upper() != 'Y':
                 StdErrException("not overwritten", 2)
 
         outfile = compresstype(zippath, 'wb', compresslevel=args.compresslevel)
     return infile, outfile
@@ -148,15 +148,15 @@
     infile = compresstype(infile, 'rb', compresslevel=args.compresslevel)
     if len(args.FILE) == 0 or args.stdout:
         outfile = sys.stdout
     else:
         unzippath = infile.rstrip(suffix)
         if os.path.exists(unzippath):
             q = input(
-                "{0}: {1} ".format(args.prog, unzippath)
+                f"{args.prog}: {unzippath} "
                 + "already exists; do you wish to overwrite (y or n)? "
             )
             if q.upper() != 'Y':
                 StdOutException("not overwritten", 2)
 
         outfile = open(unzippath, 'wb')
     return infile, outfile
```

### Comparing `cmdix-2.0.2/cmdix/exception.py` & `cmdix-3.0.0/cmdix/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Raised when an unknown command is requested
     """
 
     def __init__(self, prog):
         self.prog = prog
 
     def __str__(self):
-        return "Command `{0}' not found.".format(self.prog)
+        return f"Command `{self.prog}' not found."
 
 
 class ExtraOperandException(StdErrException):
     """
     Raised when an argument is expected but not found
     """
```

### Comparing `cmdix-2.0.2/cmdix/hasher.py` & `cmdix-3.0.0/cmdix/hasher.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,13 +15,13 @@
             hasj = hashlib.new(algorithm)
             for data in iter(functools.partial(fd.read, 128), b''):
                 hasj.update(data)
             print(hasj.hexdigest() + '  ' + fd.name)
 
     p.set_defaults(func=myhash)
     p.description = (
-        "Print or check {0} ".format(algorithm.upper())
+        f"Print or check {algorithm.upper()} "
         + "checksums. With no FILE, or when FILE is -, read "
         + "standard input."
     )
     p.add_argument('FILE', nargs='*')
     return p
```

### Comparing `cmdix-2.0.2/cmdix/lib.py` & `cmdix-3.0.0/cmdix/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 try:
     from backports.hook_compressed import hook_compressed
 except ImportError:
     from fileinput import hook_compressed
 
 import cmdix
+from .compat import py39
 
 
 def filelist2fds(filelist, mode='r'):
     """
     Take a list of files and yield the file descriptor.
     Yield sys.stdin if the filename is `-`, or the filelist is empty.
     Unix-style patterns will be parsed.
@@ -40,15 +41,16 @@
     """
     filelist = filelist or ['-']
     for f in filelist:
         if f == '-':
             yield sys.stdin
         for filename in glob.iglob(f):
             if filename:
-                with open(filename, mode) as fd:
+                encoding = None if 'b' in mode else 'utf-8'
+                with open(filename, mode, encoding=encoding) as fd:
                     yield fd
             else:
                 print(f"Cannot access {filename}: No such file or directory")
 
 
 def getcurrentusername():
     """
@@ -188,23 +190,23 @@
     """
     openhook = hook_compressed if decompress else None
 
     # Use stdin if filelist is empty
     filelist = filelist or '-'
 
     for filename in filelist:
-        yield fileinput.FileInput([filename], openhook=openhook)
+        yield fileinput.FileInput([filename], openhook=openhook, **py39.encoding)
 
 
 def showbanner(width=None):
     """
     Returns the command banner.
     The banner is centered if width is defined.
     """
-    subtext = "-= Cmdix version {0} =-".format(cmdix.__version__)
+    subtext = f"-= Cmdix version {cmdix.__version__} =-"
     banner = textwrap.dedent(
         r"""
           ___  __  __  ____  ____  _  _
          / __)(  \/  )(  _ \(_  _)( \/ )
         ( (__  )    (  )(_) )_)(_  )  (
          \___)(_/\/\_)(____/(____)(_/\_)
         """
```

### Comparing `cmdix-2.0.2/cmdix.egg-info/PKG-INFO` & `cmdix-3.0.0/cmdix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 2.0.2
+Version: 3.0.0
 Summary: Unix commands in Pure Python
 Home-page: https://github.com/jaraco/cmdix
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
    :target: https://pypi.org/project/cmdix
```

### Comparing `cmdix-2.0.2/cmdix.egg-info/SOURCES.txt` & `cmdix-3.0.0/cmdix.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 .coveragerc
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 Dockerfile
 LICENSE
+NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 cmdix/__init__.py
 cmdix/__main__.py
 cmdix/compressor.py
 cmdix/exception.py
@@ -48,15 +49,14 @@
 cmdix/command/gzip.py
 cmdix/command/httpd.py
 cmdix/command/id.py
 cmdix/command/init.py
 cmdix/command/kill.py
 cmdix/command/ln.py
 cmdix/command/logger.py
-cmdix/command/login.py
 cmdix/command/ls.py
 cmdix/command/md5sum.py
 cmdix/command/mkdir.py
 cmdix/command/mktemp.py
 cmdix/command/more.py
 cmdix/command/mount.py
 cmdix/command/mv.py
@@ -85,25 +85,26 @@
 cmdix/command/uuidgen.py
 cmdix/command/watch.py
 cmdix/command/wc.py
 cmdix/command/wget.py
 cmdix/command/whoami.py
 cmdix/command/yes.py
 cmdix/command/zip.py
+cmdix/compat/__init__.py
+cmdix/compat/py39.py
 docs/conf.py
 docs/history.rst
 docs/index.rst
 tests/__init__.py
 tests/test_base64.py
 tests/test_basename.py
 tests/test_cal.py
 tests/test_cat.py
 tests/test_cp.py
 tests/test_expand.py
-tests/test_login.py
 tests/test_ls.py
 tests/test_md5sum.py
 tests/test_nl.py
 tests/test_onlyunix.py
 tests/test_pycoreutils.py
 tests/test_pycoreutils_lib.py
 tests/test_tail.py
```

### Comparing `cmdix-2.0.2/cmdix.egg-info/entry_points.txt` & `cmdix-3.0.0/cmdix.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 gzip = cmdix:run
 httpd = cmdix:run
 id = cmdix:run
 init = cmdix:run
 kill = cmdix:run
 ln = cmdix:run
 logger = cmdix:run
-login = cmdix:run
 ls = cmdix:run
 md5sum = cmdix:run
 mkdir = cmdix:run
 mktemp = cmdix:run
 more = cmdix:run
 mount = cmdix:run
 mv = cmdix:run
```

### Comparing `cmdix-2.0.2/docs/conf.py` & `cmdix-3.0.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `cmdix-2.0.2/pytest.ini` & `cmdix-3.0.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/setup.cfg` & `cmdix-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 	Environment :: Console
 	Topic :: System :: Shells
 	Topic :: Utilities
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	importlib_metadata
 	importlib_resources
 	backports.hook_compressed; python_version < "3.10"
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
@@ -36,21 +35,21 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	types-backports
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 
 [options.entry_points]
 console_scripts = 
 	gunzip = cmdix:run
@@ -103,15 +102,14 @@
 	basename = cmdix:run
 	touch = cmdix:run
 	bunzip2 = cmdix:run
 	diff = cmdix:run
 	sleep = cmdix:run
 	mount = cmdix:run
 	watch = cmdix:run
-	login = cmdix:run
 	shred = cmdix:run
 	md5sum = cmdix:run
 	init = cmdix:run
 	uptime = cmdix:run
 	expand = cmdix:run
 	seq = cmdix:run
 	wget = cmdix:run
```

### Comparing `cmdix-2.0.2/tests/__init__.py` & `cmdix-3.0.0/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,25 @@
         assert filecmp.cmp(file1, file2)
 
     def createfile(self, filename, content=None, size=64 * 1024, fill='0'):
         """
         Create a temporary file containing `content`. If `content` is not
         defined, fill file with `size` times `fill`.
         """
-        pathlib.Path(self.workdir, filename).write_text(content or fill * size)
+        pathlib.Path(self.workdir, filename).write_text(
+            content or fill * size, encoding='utf-8'
+        )
 
     def createrandomfile(self, filename, size):
         """
         Create a temporary file containing random data
         """
-        pathlib.Path(self.workdir, filename).write_text(os.urandom(size))
+        pathlib.Path(self.workdir, filename).write_text(
+            os.urandom(size), encoding='utf-8'
+        )
 
     def runcommandline(self, commandline):
         """
         Run commandline as a subprocess.
 
         :param commandline: A string containing the commandline, i.e. 'ls -l X'
         :return:            A tuple containing the unicoded stdout and stderr
```

### Comparing `cmdix-2.0.2/tests/test_base64.py` & `cmdix-3.0.0/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/tests/test_cal.py` & `cmdix-3.0.0/tests/test_cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/tests/test_cat.py` & `cmdix-3.0.0/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/tests/test_cp.py` & `cmdix-3.0.0/tests/test_cp.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/tests/test_ls.py` & `cmdix-3.0.0/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/tests/test_nl.py` & `cmdix-3.0.0/tests/test_nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.2/tests/test_onlyunix.py` & `cmdix-3.0.0/tests/test_onlyunix.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 @pytest.mark.usefixtures('pretend_windows')
 class TestCase:
     unix_only_cmds = (
         'chmod',
         'chown',
         'id',
-        'login',
         'mount',
         'tee',
         'uptime',
         'whoami',
     )
 
     def test_onlyunix(self):
```

### Comparing `cmdix-2.0.2/tests/test_tar.py` & `cmdix-3.0.0/tests/test_tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,27 +32,28 @@
             'dir2/dir2-2/',
             'dir2/dir2-2/file2-2-1',
             'file1',
         ]
 
         for archive in ('foo.tar', 'foo.tar.bz2', 'foo.tar.gz'):
             # Create an archive
-            self.runcommandline('tar -cf {0} dir1 dir2 file1'.format(archive))
+            self.runcommandline(f'tar -cf {archive} dir1 dir2 file1')
             assert capsys.readouterr().out == ''
             list_ = []
-            for tarinfo in tarfile.open(archive):
-                name = tarinfo.name
-                if tarinfo.isdir():
-                    name += '/'
-                list_.append(name)
+            with tarfile.open(archive) as obj:
+                for tarinfo in obj:
+                    name = tarinfo.name
+                    if tarinfo.isdir():
+                        name += '/'
+                    list_.append(name)
             list_.sort()
             assert list_ == good
 
             # List the archive
-            self.runcommandline('tar -tf {0}'.format(archive))
+            self.runcommandline(f'tar -tf {archive}')
             x = capsys.readouterr().out.split()
             x.sort()
             assert x == good
 
             # Extract the archive
             """
             d = os.getcwd()
```

### Comparing `cmdix-2.0.2/tests/test_uuidgen.py` & `cmdix-3.0.0/tests/test_uuidgen.py`

 * *Files identical despite different names*

