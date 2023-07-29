# Comparing `tmp/infrahouse-toolkit-2.0.7.tar.gz` & `tmp/infrahouse-toolkit-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahouse-toolkit-2.0.7.tar", last modified: Sat Jul 29 16:17:13 2023, max compression
+gzip compressed data, was "infrahouse-toolkit-2.0.8.tar", last modified: Sat Jul 29 17:04:09 2023, max compression
```

## Comparing `infrahouse-toolkit-2.0.7.tar` & `infrahouse-toolkit-2.0.8.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.backends.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.tests.status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_download/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.916593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_publish/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.916593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.916593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_upload/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.916593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.916593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/tests/test_get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.916593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/s3backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/s3backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/githubpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/test_parse_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/test_parse_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:17:13.912593 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-29 16:17:13.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-29 16:17:13.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:17:13.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-29 16:17:13.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:16:58.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-29 16:17:13.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 16:17:13.000000 infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-29 16:17:13.920593 infrahouse-toolkit-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-29 16:16:30.000000 infrahouse-toolkit-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.288392 infrahouse-toolkit-2.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_plan.cmd_download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_plan.cmd_min_permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_plan.cmd_publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_plan.cmd_remove.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_plan.cmd_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.backends.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.tests.github_pr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.tests.status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.288392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.296392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.300392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/tests/test_get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.300392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.300392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/s3backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.300392 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/s3backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/s3backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/s3backend/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/s3backend/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/test_get_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/githubpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/test_parse_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/test_parse_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:04:09.292392 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-29 17:04:09.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-29 17:04:09.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:04:09.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-29 17:04:09.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:03:54.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-29 17:04:09.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 17:04:09.000000 infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-29 17:04:09.304391 infrahouse-toolkit-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-29 17:03:26.000000 infrahouse-toolkit-2.0.8/setup.py
```

### Comparing `infrahouse-toolkit-2.0.7/CONTRIBUTING.rst` & `infrahouse-toolkit-2.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/LICENSE` & `infrahouse-toolkit-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/PKG-INFO` & `infrahouse-toolkit-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 2.0.7
+Version: 2.0.8
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-2.0.7/README.rst` & `infrahouse-toolkit-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/Makefile` & `infrahouse-toolkit-2.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/conf.py` & `infrahouse-toolkit-2.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.ih_s3_reprepro.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.cli.tests.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.cli.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.backends.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.backends.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.backends.tests.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.backends.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.backends.tests.s3backend.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.tests.github_pr.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.tests.github_pr.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.tests.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.tests.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/infrahouse_toolkit.terraform.tests.status.rst` & `infrahouse-toolkit-2.0.8/docs/infrahouse_toolkit.terraform.tests.status.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/installation.rst` & `infrahouse-toolkit-2.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/docs/usage.rst` & `infrahouse-toolkit-2.0.8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_download/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_min_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_publish/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_remove/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_plan/cmd_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/aws.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 .. topic:: ``aws.py``
 
     AWS helper functions.
 """
+from os import environ
 
 import boto3
 import requests
 from botocore.exceptions import ClientError
 
 from infrahouse_toolkit import LOG
 
@@ -81,11 +82,31 @@
     """
     Another way to get AWS credentials is from EC2 instance metadata.
 
     :return: A dictionary with AWS_* variables.
     """
     url = "http://169.254.169.254/latest/meta-data/iam/security-credentials/"
     profile_name = requests.get(url, timeout=10).text
+    LOG.debug("Profile name %s", profile_name)
     profile_data = requests.get(f"{url}/{profile_name}", timeout=10).json()
     profile_data["SessionToken"] = profile_data["Token"]
 
     return {var: profile_data.get(key) for var, key in VALUE_MAP.items()}
+
+
+def get_credentials_from_environ():
+    """Yet another way to get credentials.
+
+    If environment is already configured for AWS access, simply get the credential from the environment.
+    This is a situation when a user configures AWS_* in their env.
+    Or when a role has been assumed and AWS_* are configured.
+
+    :return: A dictionary with AWS_* variables.
+    """
+    return {
+        "AWS_ACCESS_KEY_ID": environ.get("AWS_ACCESS_KEY_ID"),
+        "AWS_SECRET_ACCESS_KEY": environ.get("AWS_SECRET_ACCESS_KEY"),
+        "AWS_SESSION_TOKEN": environ.get("AWS_SESSION_TOKEN"),
+        "AWSACCESSKEYID": environ.get("AWS_ACCESS_KEY_ID"),
+        "AWSSECRETACCESSKEY": environ.get("AWS_SECRET_ACCESS_KEY"),
+        "AWSSESSIONTOKEN": environ.get("AWS_SESSION_TOKEN"),
+    }
```

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_check.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_checkpool.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_deleteunreferenced.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_dumpunreferenced.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_get_secret_value.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_includedeb.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_list.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_remove.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/cmd_set_secret_value.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/gpg.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/ih_s3_reprepro/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 .. topic:: ``utils.py``
 
     Various helper functions.
 """
 import json
+import os
 import sys
 from contextlib import contextmanager
 from os import getgid, getuid
 from os import path as osp
 from subprocess import CalledProcessError, Popen, check_call
 from tempfile import TemporaryDirectory
 from time import sleep, time
 
 import boto3
 
 from infrahouse_toolkit import DEFAULT_OPEN_ENCODING, LOG
 from infrahouse_toolkit.cli.ih_s3_reprepro.aws import (
     assume_role,
+    get_credentials_from_environ,
     get_credentials_from_profile,
 )
 from infrahouse_toolkit.cli.ih_s3_reprepro.gpg import gpg
 
 DEPENDENCIES = ["reprepro", "gpg", "s3fs"]
 
 
@@ -64,14 +66,16 @@
             aws_access_key_id=env["AWS_ACCESS_KEY_ID"],
             aws_secret_access_key=env["AWS_SECRET_ACCESS_KEY"],
             aws_session_token=env["AWS_SESSION_TOKEN"],
             region_name=region,
         )
         response = sts.get_caller_identity()
         LOG.debug("Assumed role: %s", response)
+    elif "AWS_ACCESS_KEY_ID" in os.environ:
+        env = get_credentials_from_environ()
     else:
         env = get_credentials_from_profile()
 
     LOG.debug("To reproduce environment: \n%s", "\n".join([f'export {key}="{value}"' for key, value in env.items()]))
     LOG.debug("Command to debug: mkdir -p %s; %s -o dbglevel=info -f -o curldbg", path, " ".join(cmd))
     execute(cmd, env=env)
 
@@ -82,15 +86,15 @@
 
     :param path: Local filesystem path name where the S3 bucket is mounted at.
     :type path: str
     """
     try:
         check_call(["umount", path])
     except CalledProcessError as err:
-        LOG.error(err)
+        LOG.exception(err)
         sys.exit(1)
 
 
 @contextmanager
 def local_s3(bucket, role_arn=None, retry_timeout=60, region=None) -> str:
     """
     Mount an S3 bucket locally and return a mount point.
@@ -114,14 +118,17 @@
                 if osp.exists(osp.join(mnt_dir, "conf/distributions")):
                     break
                 LOG.warning("Waiting until s3://%s is mounted at %s", bucket, mnt_dir)
                 sleep(1)
                 if time() > timeout:
                     raise RuntimeError(f"s3://{bucket} is not mounted after {retry_timeout} seconds")
             yield mnt_dir
+        except Exception as err:
+            LOG.critical(err)
+            raise
 
         finally:
             umount_s3(mnt_dir)
 
 
 def execute(cmd: list, env: dict = None):
     """
```

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/lib.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/lib.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/cli/tests/conftest.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/logging.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/__init__.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/s3backend.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/s3backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tests/s3backend/test_region.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/backends/tfbackend.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/backends/tfbackend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/githubpr.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/githubpr.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/status.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/status.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/test_find_comment_by_backend.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/github_pr/test_publish_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_eq.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_eq.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_metadata.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_metadata.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_summary_counts.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/status/test_summary_resources.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/test_parse_comment.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/test_parse_comment.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit/terraform/tests/test_parse_plan.py` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit/terraform/tests/test_parse_plan.py`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/PKG-INFO` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahouse-toolkit
-Version: 2.0.7
+Version: 2.0.8
 Summary: A collection of tools for building infrastructure.
 Home-page: https://github.com/infrahouse/infrahouse-toolkit
 Author: Oleksandr Kuzminskyi
 Author-email: aleks@infrahouse.com
 License: Apache Software License 2.0
 Keywords: infrahouse-toolkit
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `infrahouse-toolkit-2.0.7/infrahouse_toolkit.egg-info/SOURCES.txt` & `infrahouse-toolkit-2.0.8/infrahouse_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infrahouse-toolkit-2.0.7/setup.cfg` & `infrahouse-toolkit-2.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.0.7
+current_version = 2.0.8
 commit = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
 
 [bumpversion:file(pycode):infrahouse_toolkit/__init__.py]
```

### Comparing `infrahouse-toolkit-2.0.7/setup.py` & `infrahouse-toolkit-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     include_package_data=True,
     keywords="infrahouse-toolkit",
     name="infrahouse-toolkit",
     packages=find_packages(include=["infrahouse_toolkit", "infrahouse_toolkit.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/infrahouse/infrahouse-toolkit",
-    version="2.0.7",
+    version="2.0.8",
     zip_safe=False,
 )
```

