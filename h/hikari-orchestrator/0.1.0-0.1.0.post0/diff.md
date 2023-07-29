# Comparing `tmp/hikari_orchestrator-0.1.0.tar.gz` & `tmp/hikari_orchestrator-0.1.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_orchestrator-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hikari_orchestrator-0.1.0.post0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hikari_orchestrator-0.1.0.tar` & `hikari_orchestrator-0.1.0.post0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0       14 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.gitattributes
--rw-r--r--   0        0        0       26 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      459 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1146 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0     1036 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1518 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/pr-docs.yml
--rw-r--r--   0        0        0      874 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      982 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1265 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/release-docs.yml
--rw-r--r--   0        0        0     1027 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      838 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1188 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1223 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1062 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0      856 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.github/workflows/verify-types.yml
--rw-r--r--   0        0        0     1748 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.gitignore
--rw-r--r--   0        0        0       85 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/.gitmodules
--rw-r--r--   0        0        0      501 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1515 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/LICENSE
--rw-r--r--   0        0        0      147 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/README.md
--rw-r--r--   0        0        0      115 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/dev-requirements/constraints.in
--rw-r--r--   0        0        0    51506 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/dev-requirements/constraints.txt
--rw-r--r--   0        0        0      141 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    71040 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0       17 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/docs/changelog.md
--rw-r--r--   0        0        0     3004 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/docs/index.md
--rw-r--r--   0        0        0       64 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/docs/reference.md
--rw-r--r--   0        0        0     7048 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/docs_src/LICENSE
--rw-r--r--   0        0        0      996 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/docs_src/index.py
--rw-r--r--   0        0        0     1941 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/hikari_orchestrator/__init__.py
--rw-r--r--   0        0        0     4017 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/hikari_orchestrator/__main__.py
--rw-r--r--   0        0        0    12623 2023-07-28 11:06:13.826758 hikari_orchestrator-0.1.0/hikari_orchestrator/_bot.py
--rw-r--r--   0        0        0    21207 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_client.py
--rw-r--r--   0        0        0     1684 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/__init__.py
--rw-r--r--   0        0        0     6393 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2.py
--rw-r--r--   0        0        0     8359 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2.pyi
--rw-r--r--   0        0        0    11416 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2_grpc.py
--rw-r--r--   0        0        0     4808 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2_grpc.pyi
--rw-r--r--   0        0        0    17603 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_service.py
--rw-r--r--   0        0        0     3155 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/_ssl.py
--rw-r--r--   0        0        0        0 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/hikari_orchestrator/py.typed
--rw-r--r--   0        0        0     1698 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1714 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/noxfile.py
--rw-r--r--   0        0        0       14 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.gitattributes
--rw-r--r--   0        0        0      458 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/dependabot.yml
--rw-r--r--   0        0        0     1240 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0      959 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/lint.yml
--rw-r--r--   0        0        0      976 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1032 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      832 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1182 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1217 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1114 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0     1751 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/.gitignore
--rw-r--r--   0        0        0     1520 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/LICENSE
--rw-r--r--   0        0        0      138 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/README.md
--rw-r--r--   0        0        0       50 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/bot/.env.example
--rw-r--r--   0        0        0      612 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/bot/Dockerfile
--rw-r--r--   0        0        0    30763 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/bot/main.py
--rw-r--r--   0        0        0       10 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/bot/requirements-extra.txt
--rw-r--r--   0        0        0      194 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/bot/requirements.in
--rw-r--r--   0        0        0    25212 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/bot/requirements.txt
--rw-r--r--   0        0        0      933 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/dev-requirements/flake8.in
--rw-r--r--   0        0        0    20370 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/dev-requirements/flake8.txt
--rw-r--r--   0        0        0       10 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/dev-requirements/type-checking-extra.txt
--rw-r--r--   0        0        0      112 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    34990 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0      250 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/docker-compose.yml
--rw-r--r--   0        0        0       26 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/FUNDING.yml
--rw-r--r--   0        0        0      764 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/clippy.yml
--rw-r--r--   0        0        0     1133 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/freeze-for-pr.yml
--rw-r--r--   0        0        0     1271 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/lint.yml
--rw-r--r--   0        0        0     1577 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/pr-docs.yml
--rw-r--r--   0        0        0      964 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/publish.yml
--rw-r--r--   0        0        0     2399 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/py-test.yml
--rw-r--r--   0        0        0     1013 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/reformat.yml
--rw-r--r--   0        0        0     1373 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/release-docs.yml
--rw-r--r--   0        0        0     1075 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/resync-piped.yml
--rw-r--r--   0        0        0     1223 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/rustfmt.yml
--rw-r--r--   0        0        0      869 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/type-check.yml
--rw-r--r--   0        0        0     1191 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/update-licence.yml
--rw-r--r--   0        0        0     1226 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/upgrade-locks.yml
--rw-r--r--   0        0        0     1130 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/verify-locks.yml
--rw-r--r--   0        0        0      887 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/actions/verify-types.yml
--rw-r--r--   0        0        0      550 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/dependabot.yml
--rw-r--r--   0        0        0      524 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/github/pull_request_template.md
--rw-r--r--   0        0        0     1713 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/noxfile.py
--rw-r--r--   0        0        0     4853 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/pyproject.toml
--rw-r--r--   0        0        0      115 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/python/base-requirements/docs.in
--rw-r--r--   0        0        0    31882 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/python/base-requirements/docs.txt
--rw-r--r--   0        0        0       90 2023-07-28 11:06:14.606778 hikari_orchestrator-0.1.0/piped/python/base-requirements/flake8.in
--rw-r--r--   0        0        0     1671 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/flake8.txt
--rw-r--r--   0        0        0       32 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/freeze-locks.in
--rw-r--r--   0        0        0    58539 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/freeze-locks.txt
--rw-r--r--   0        0        0     1070 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/library-flake8.in
--rw-r--r--   0        0        0    30104 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/library-flake8.txt
--rw-r--r--   0        0        0       58 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/lint.in
--rw-r--r--   0        0        0     5453 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/lint.txt
--rw-r--r--   0        0        0       60 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/nox.in
--rw-r--r--   0        0        0    16594 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/nox.txt
--rw-r--r--   0        0        0       12 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/publish.in
--rw-r--r--   0        0        0     8587 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/publish.txt
--rw-r--r--   0        0        0       78 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/reformat.in
--rw-r--r--   0        0        0    15634 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/reformat.txt
--rw-r--r--   0        0        0       64 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/tests.in
--rw-r--r--   0        0        0     8070 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/tests.txt
--rw-r--r--   0        0        0       29 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/type-checking.in
--rw-r--r--   0        0        0     3965 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/base-requirements/type-checking.txt
--rw-r--r--   0        0        0    24265 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/noxfile.py
--rw-r--r--   0        0        0     1714 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/noxfile.template.py
--rw-r--r--   0        0        0     4527 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/piped_shared/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/piped_shared/py.typed
--rw-r--r--   0        0        0      334 2023-07-28 11:06:14.610777 hikari_orchestrator-0.1.0/piped/python/pyproject.toml
--rw-r--r--   0        0        0     6969 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2604 2023-07-28 11:06:13.830758 hikari_orchestrator-0.1.0/schema.proto
--rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 hikari_orchestrator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.gitattributes
+-rw-r--r--   0        0        0       26 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      459 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1146 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1036 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1518 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/pr-docs.yml
+-rw-r--r--   0        0        0      874 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      982 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1265 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1027 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      838 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1188 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1223 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1062 2023-07-29 01:53:44.937924 hikari_orchestrator-0.1.0.post0/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0      856 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/.github/workflows/verify-types.yml
+-rw-r--r--   0        0        0     1748 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/.gitignore
+-rw-r--r--   0        0        0       85 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/.gitmodules
+-rw-r--r--   0        0        0      501 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/CHANGELOG.md
+-rw-r--r--   0        0        0     1515 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/LICENSE
+-rw-r--r--   0        0        0      147 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/README.md
+-rw-r--r--   0        0        0      115 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/constraints.in
+-rw-r--r--   0        0        0    51506 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/constraints.txt
+-rw-r--r--   0        0        0      141 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    71040 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0       17 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs/changelog.md
+-rw-r--r--   0        0        0     3004 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs/index.md
+-rw-r--r--   0        0        0       64 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs/reference.md
+-rw-r--r--   0        0        0     7048 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs_src/LICENSE
+-rw-r--r--   0        0        0      996 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/docs_src/index.py
+-rw-r--r--   0        0        0     1941 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__init__.py
+-rw-r--r--   0        0        0     4017 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__main__.py
+-rw-r--r--   0        0        0    12623 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_bot.py
+-rw-r--r--   0        0        0    21207 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_client.py
+-rw-r--r--   0        0        0     1684 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/__init__.py
+-rw-r--r--   0        0        0     6393 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.py
+-rw-r--r--   0        0        0     8359 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.pyi
+-rw-r--r--   0        0        0    11416 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     4808 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.pyi
+-rw-r--r--   0        0        0    17603 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_service.py
+-rw-r--r--   0        0        0     3155 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_ssl.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/hikari_orchestrator/py.typed
+-rw-r--r--   0        0        0     1698 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/mkdocs.yml
+-rw-r--r--   0        0        0     1714 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/noxfile.py
+-rw-r--r--   0        0        0       14 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.gitattributes
+-rw-r--r--   0        0        0      458 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/dependabot.yml
+-rw-r--r--   0        0        0     1240 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0      959 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      976 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1032 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      832 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1182 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1217 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1114 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0     1751 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/.gitignore
+-rw-r--r--   0        0        0     1520 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/LICENSE
+-rw-r--r--   0        0        0      138 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/README.md
+-rw-r--r--   0        0        0       50 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/.env.example
+-rw-r--r--   0        0        0      612 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/Dockerfile
+-rw-r--r--   0        0        0    30763 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/main.py
+-rw-r--r--   0        0        0       10 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/requirements-extra.txt
+-rw-r--r--   0        0        0      194 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/requirements.in
+-rw-r--r--   0        0        0    25212 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/bot/requirements.txt
+-rw-r--r--   0        0        0      933 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.in
+-rw-r--r--   0        0        0    20370 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0       10 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking-extra.txt
+-rw-r--r--   0        0        0      112 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    34990 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0      250 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/docker-compose.yml
+-rw-r--r--   0        0        0       26 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/FUNDING.yml
+-rw-r--r--   0        0        0      764 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/clippy.yml
+-rw-r--r--   0        0        0     1133 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1271 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/lint.yml
+-rw-r--r--   0        0        0     1577 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/pr-docs.yml
+-rw-r--r--   0        0        0      964 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/publish.yml
+-rw-r--r--   0        0        0     2399 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/py-test.yml
+-rw-r--r--   0        0        0     1013 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/reformat.yml
+-rw-r--r--   0        0        0     1373 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/release-docs.yml
+-rw-r--r--   0        0        0     1075 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/resync-piped.yml
+-rw-r--r--   0        0        0     1223 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/rustfmt.yml
+-rw-r--r--   0        0        0      869 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/type-check.yml
+-rw-r--r--   0        0        0     1191 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/update-licence.yml
+-rw-r--r--   0        0        0     1226 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/upgrade-locks.yml
+-rw-r--r--   0        0        0     1130 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-locks.yml
+-rw-r--r--   0        0        0      887 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-types.yml
+-rw-r--r--   0        0        0      550 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/dependabot.yml
+-rw-r--r--   0        0        0      524 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/github/pull_request_template.md
+-rw-r--r--   0        0        0     1713 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/noxfile.py
+-rw-r--r--   0        0        0     4853 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/docs.in
+-rw-r--r--   0        0        0    31882 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/docs.txt
+-rw-r--r--   0        0        0       90 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/flake8.in
+-rw-r--r--   0        0        0     1671 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/flake8.txt
+-rw-r--r--   0        0        0       32 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/freeze-locks.in
+-rw-r--r--   0        0        0    58539 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/freeze-locks.txt
+-rw-r--r--   0        0        0     1070 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.in
+-rw-r--r--   0        0        0    30104 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.txt
+-rw-r--r--   0        0        0       58 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/lint.in
+-rw-r--r--   0        0        0     5453 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/lint.txt
+-rw-r--r--   0        0        0       60 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/nox.in
+-rw-r--r--   0        0        0    16594 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/nox.txt
+-rw-r--r--   0        0        0       12 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/publish.in
+-rw-r--r--   0        0        0     8587 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/publish.txt
+-rw-r--r--   0        0        0       78 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/reformat.in
+-rw-r--r--   0        0        0    15634 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/reformat.txt
+-rw-r--r--   0        0        0       64 2023-07-29 01:53:45.637918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/tests.in
+-rw-r--r--   0        0        0     8070 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/tests.txt
+-rw-r--r--   0        0        0       29 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/type-checking.in
+-rw-r--r--   0        0        0     3965 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/type-checking.txt
+-rw-r--r--   0        0        0    24265 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/noxfile.py
+-rw-r--r--   0        0        0     1714 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/noxfile.template.py
+-rw-r--r--   0        0        0     4527 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/piped_shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/piped_shared/py.typed
+-rw-r--r--   0        0        0      334 2023-07-29 01:53:45.641918 hikari_orchestrator-0.1.0.post0/piped/python/pyproject.toml
+-rw-r--r--   0        0        0     6974 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/pyproject.toml
+-rw-r--r--   0        0        0     2604 2023-07-29 01:53:44.941924 hikari_orchestrator-0.1.0.post0/schema.proto
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 hikari_orchestrator-0.1.0.post0/PKG-INFO
```

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/freeze-for-pr.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/lint.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/pr-docs.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/pr-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/publish.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/reformat.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/release-docs.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/release-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/resync-piped.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/type-check.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/update-licence.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/upgrade-locks.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/verify-locks.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.github/workflows/verify-types.yml` & `hikari_orchestrator-0.1.0.post0/.github/workflows/verify-types.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/.gitignore` & `hikari_orchestrator-0.1.0.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/LICENSE` & `hikari_orchestrator-0.1.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/dev-requirements/constraints.txt` & `hikari_orchestrator-0.1.0.post0/dev-requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/dev-requirements/type-checking.txt` & `hikari_orchestrator-0.1.0.post0/dev-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/docs/index.md` & `hikari_orchestrator-0.1.0.post0/docs/index.md`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/docs_src/LICENSE` & `hikari_orchestrator-0.1.0.post0/docs_src/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/docs_src/index.py` & `hikari_orchestrator-0.1.0.post0/docs_src/index.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/__init__.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/__main__.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_bot.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_bot.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_client.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_client.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/__init__.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2.pyi` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2_grpc.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_protos/schema_pb2_grpc.pyi` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_protos/schema_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_service.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_service.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/hikari_orchestrator/_ssl.py` & `hikari_orchestrator-0.1.0.post0/hikari_orchestrator/_ssl.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/mkdocs.yml` & `hikari_orchestrator-0.1.0.post0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/noxfile.py` & `hikari_orchestrator-0.1.0.post0/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/freeze-for-pr.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/lint.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/reformat.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/resync-piped.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/type-check.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/update-licence.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/upgrade-locks.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.github/workflows/verify-locks.yml` & `hikari_orchestrator-0.1.0.post0/piped/.github/workflows/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/.gitignore` & `hikari_orchestrator-0.1.0.post0/piped/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/LICENSE` & `hikari_orchestrator-0.1.0.post0/piped/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/bot/Dockerfile` & `hikari_orchestrator-0.1.0.post0/piped/bot/Dockerfile`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/bot/main.py` & `hikari_orchestrator-0.1.0.post0/piped/bot/main.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/bot/requirements.txt` & `hikari_orchestrator-0.1.0.post0/piped/bot/requirements.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/dev-requirements/flake8.in` & `hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.in`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/dev-requirements/flake8.txt` & `hikari_orchestrator-0.1.0.post0/piped/dev-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/dev-requirements/type-checking.txt` & `hikari_orchestrator-0.1.0.post0/piped/dev-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/clippy.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/clippy.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/freeze-for-pr.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/lint.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/pr-docs.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/pr-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/publish.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/publish.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/py-test.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/py-test.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/reformat.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/release-docs.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/release-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/resync-piped.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/rustfmt.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/rustfmt.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/type-check.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/update-licence.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/upgrade-locks.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/verify-locks.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/actions/verify-types.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/actions/verify-types.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/dependabot.yml` & `hikari_orchestrator-0.1.0.post0/piped/github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/github/pull_request_template.md` & `hikari_orchestrator-0.1.0.post0/piped/github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/noxfile.py` & `hikari_orchestrator-0.1.0.post0/piped/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/pyproject.toml` & `hikari_orchestrator-0.1.0.post0/piped/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/docs.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/flake8.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/freeze-locks.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/freeze-locks.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/library-flake8.in` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.in`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/library-flake8.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/library-flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/lint.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/nox.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/nox.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/publish.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/reformat.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/reformat.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/tests.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/base-requirements/type-checking.txt` & `hikari_orchestrator-0.1.0.post0/piped/python/base-requirements/type-checking.txt`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/noxfile.py` & `hikari_orchestrator-0.1.0.post0/piped/python/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/noxfile.template.py` & `hikari_orchestrator-0.1.0.post0/piped/python/noxfile.template.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/piped/python/piped_shared/__init__.py` & `hikari_orchestrator-0.1.0.post0/piped/python/piped_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/pyproject.toml` & `hikari_orchestrator-0.1.0.post0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.3,<4,!=3.7"]
 build-backend = "flit_core.buildapi"
 
 [project]
-name = "hikari_orchestrator"
-version = "0.1.0"
+name = "hikari-orchestrator"
+version = "0.1.0.post"
 readme = "README.md"
 requires-python = ">=3.10.0,<3.12"
 license = {file = "LICENSE"}
 authors = [ {name = "Faster Speeding", email="lucina@lmbyrne.dev"} ]
 keywords = ["hikari"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `hikari_orchestrator-0.1.0/schema.proto` & `hikari_orchestrator-0.1.0.post0/schema.proto`

 * *Files identical despite different names*

### Comparing `hikari_orchestrator-0.1.0/PKG-INFO` & `hikari_orchestrator-0.1.0.post0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hikari_orchestrator
-Version: 0.1.0
+Name: hikari-orchestrator
+Version: 0.1.0.post0
 Summary: System for managing hikari shards across processes/systems.
 Keywords: hikari
 Author-email: Faster Speeding <lucina@lmbyrne.dev>
 Requires-Python: >=3.10.0,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -25,13 +25,13 @@
 Requires-Dist: hikari>=2.0.0.dev116, <3
 Requires-Dist: python-dotenv>=1, <2
 Project-URL: Changelog, https://h2o.cursed.solutions/changelog
 Project-URL: Documentation, https://h2o.cursed.solutions/
 Project-URL: Homepage, https://github.com/FasterSpeeding/hikari-orchestrator
 Project-URL: Repository, https://github.com/FasterSpeeding/hikari-orchestrator
 
-# hikari_orchestrator
+# Hikari Orchestrator
 
 A cute lil tool for orchestrating separate Hikari shard clusters.
 
 For more information see <https://h2o.cursed.solutions>.
```

