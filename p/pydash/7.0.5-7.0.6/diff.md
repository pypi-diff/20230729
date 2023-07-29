# Comparing `tmp/pydash-7.0.5.tar.gz` & `tmp/pydash-7.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-7.0.5.tar", last modified: Thu Jul  6 13:57:26 2023, max compression
+gzip compressed data, was "pydash-7.0.6.tar", last modified: Sat Jul 29 19:57:35 2023, max compression
```

## Comparing `pydash-7.0.5.tar` & `pydash-7.0.6.tar`

### file list

```diff
@@ -1,630 +1,630 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.260303 pydash-7.0.5/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205446 pydash-7.0.5/.tox/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.189874 pydash-7.0.5/.tox/.package/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.189941 pydash-7.0.5/.tox/.package/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.189989 pydash-7.0.5/.tox/.package/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190038 pydash-7.0.5/.tox/.package/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212134 pydash-7.0.5/.tox/.package/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.5/.tox/.package/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190170 pydash-7.0.5/.tox/.pkg/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190218 pydash-7.0.5/.tox/.pkg/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190273 pydash-7.0.5/.tox/.pkg/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190324 pydash-7.0.5/.tox/.pkg/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212401 pydash-7.0.5/.tox/.pkg/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.5/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190448 pydash-7.0.5/.tox/3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190500 pydash-7.0.5/.tox/3.11/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.190557 pydash-7.0.5/.tox/3.11/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193353 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212635 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212726 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212819 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.212915 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213173 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213260 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213361 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213458 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213556 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213669 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.213774 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214124 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214239 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214347 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214451 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214552 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.191785 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214656 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.214939 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215028 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215117 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215432 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215541 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215799 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.215902 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216156 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216259 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216514 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216774 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216864 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.216958 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217042 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217127 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217216 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217490 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217581 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217667 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217750 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217843 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.217937 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218028 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.5/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193481 pydash-7.0.5/.tox/py310/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193529 pydash-7.0.5/.tox/py310/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.193576 pydash-7.0.5/.tox/py310/lib/python3.10/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196082 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218130 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218242 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218344 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218433 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218700 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218784 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218874 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.218959 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219049 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219133 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219216 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219462 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219564 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219663 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219752 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219855 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.219951 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.194594 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220039 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220288 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220399 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220508 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220734 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.220826 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221074 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221180 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221422 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221508 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221705 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.221935 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222030 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222130 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222233 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222338 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222443 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222667 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222760 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222844 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.222939 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223028 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223281 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223372 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223474 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.5/.tox/py310/lib/python3.10/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196187 pydash-7.0.5/.tox/py311/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196227 pydash-7.0.5/.tox/py311/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.196273 pydash-7.0.5/.tox/py311/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199110 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223572 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223669 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223775 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.223881 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224120 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224206 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224302 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224390 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224474 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224568 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224675 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.224943 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225033 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225124 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225222 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225318 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.197430 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225410 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225639 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225726 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.225812 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226080 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226174 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226417 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226507 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226744 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.226829 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227068 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227288 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227387 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227484 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227588 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227688 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.227791 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228035 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228135 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228222 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228309 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228397 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228487 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228590 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.5/.tox/py311/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199244 pydash-7.0.5/.tox/py37/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199304 pydash-7.0.5/.tox/py37/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.199366 pydash-7.0.5/.tox/py37/lib/python3.7/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202250 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228693 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228790 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228887 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.228990 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229236 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229327 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229413 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229506 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229596 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229691 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.229963 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230055 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230149 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230247 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230340 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230425 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.200646 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230512 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230778 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.230887 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231002 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231268 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231359 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231593 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231683 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231890 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.231976 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232192 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232437 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232543 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232663 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.201620 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232781 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/py/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.232893 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233007 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233128 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233417 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233537 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233664 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233786 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.233907 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234202 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234379 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.5/.tox/py37/lib/python3.7/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202360 pydash-7.0.5/.tox/py38/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202411 pydash-7.0.5/.tox/py38/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.202465 pydash-7.0.5/.tox/py38/lib/python3.8/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205355 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234517 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234648 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234766 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.234877 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235143 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235265 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235386 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235505 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235624 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235745 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.235871 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236152 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236268 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236389 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236504 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236658 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_resources/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236777 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.236905 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.203711 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237031 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237341 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237457 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237570 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237865 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.237973 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238230 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238348 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238602 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238712 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.238963 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239220 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239339 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239452 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239566 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239669 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.239788 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240069 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240176 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240283 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240402 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240516 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240789 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.240901 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241014 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.5/.tox/py38/lib/python3.8/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205505 pydash-7.0.5/.tox/py39/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205558 pydash-7.0.5/.tox/py39/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.205613 pydash-7.0.5/.tox/py39/lib/python3.9/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.208903 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241132 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241254 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241371 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241485 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241757 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241871 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.241983 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242093 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242210 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242327 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242448 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242726 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242841 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.242953 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243070 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243246 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243365 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.207067 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243482 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243746 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243850 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.243955 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244220 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244320 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244526 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244625 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244860 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.244957 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245205 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245420 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245522 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245629 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245753 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245863 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.245979 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246245 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246348 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246450 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246561 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246662 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.246930 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.247023 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.247122 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.5/.tox/py39/lib/python3.9/site-packages/twine/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-7.0.5/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    40894 2023-07-06 13:44:03.000000 pydash-7.0.5/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.5/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.5/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.5/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)    44369 2023-07-06 13:57:26.260416 pydash-7.0.5/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.5/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.249857 pydash-7.0.5/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.249987 pydash-7.0.5/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.5/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.5/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.5/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5356 2023-06-24 16:30:19.000000 pydash-7.0.5/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.5/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.5/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.5/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.5/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.5/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.5/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.5/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.5/pylintrc
--rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.5/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.5/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     2524 2023-07-06 13:57:26.260824 pydash-7.0.5/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.209270 pydash-7.0.5/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.253259 pydash-7.0.5/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-07-06 13:44:11.000000 pydash-7.0.5/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    69930 2023-07-06 13:41:49.000000 pydash-7.0.5/src/pydash/arrays.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.254793 pydash-7.0.5/src/pydash/chaining/
--rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.5/src/pydash/chaining/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.5/src/pydash/chaining/all_funcs.py
--rw-r--r--   0 dgilland   (501) staff       (20)   123464 2023-07-06 13:41:49.000000 pydash-7.0.5/src/pydash/chaining/all_funcs.pyi
--rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.5/src/pydash/chaining/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.5/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.5/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.5/src/pydash/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.5/src/pydash/types.py
--rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.5/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.254120 pydash-7.0.5/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)    44369 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)    16254 2023-07-06 13:57:26.000000 pydash-7.0.5/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      289 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-07-06 13:57:24.000000 pydash-7.0.5/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.5/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.257845 pydash-7.0.5/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.5/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.209558 pydash-7.0.5/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.258019 pydash-7.0.5/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.5/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.5/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.5/tests/helpers.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-06 13:57:26.260157 pydash-7.0.5/tests/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/pytest_mypy_testing/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    17085 2023-07-06 13:41:49.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.5/tests/pytest_mypy_testing/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.5/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.5/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.5/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.5/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.5/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.5/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.5/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.5/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.5/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.589389 pydash-7.0.6/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.533189 pydash-7.0.6/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517382 pydash-7.0.6/.tox/.package/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517434 pydash-7.0.6/.tox/.package/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517485 pydash-7.0.6/.tox/.package/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517530 pydash-7.0.6/.tox/.package/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.540357 pydash-7.0.6/.tox/.package/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.6/.tox/.package/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517641 pydash-7.0.6/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517683 pydash-7.0.6/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517726 pydash-7.0.6/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517769 pydash-7.0.6/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.540614 pydash-7.0.6/.tox/.pkg/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.6/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517904 pydash-7.0.6/.tox/3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.517963 pydash-7.0.6/.tox/3.11/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.518015 pydash-7.0.6/.tox/3.11/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.520702 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.540879 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.540994 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541105 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541214 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541507 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541618 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541725 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541818 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.541913 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542011 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542101 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542401 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542496 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542586 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542680 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542785 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.519164 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.542896 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.543196 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.543317 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.543425 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.543720 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.543814 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.544023 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.544113 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.544365 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.544469 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.544715 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.544946 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545044 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545153 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545243 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545329 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545415 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545676 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545760 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545852 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.545950 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546035 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546119 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546204 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.6/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.520829 pydash-7.0.6/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.520877 pydash-7.0.6/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.520924 pydash-7.0.6/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.523820 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546294 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546387 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546485 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546581 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546838 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.546923 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547011 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547097 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547187 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547270 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547366 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547610 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547696 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547790 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547884 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.547984 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548078 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.522130 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548165 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548432 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548539 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548644 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548871 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.548958 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.549198 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.549292 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.549517 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.549605 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.549809 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550026 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550116 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550204 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550295 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550377 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550467 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550696 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550782 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550867 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.550961 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551052 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551298 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551392 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551494 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.6/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.523949 pydash-7.0.6/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.524003 pydash-7.0.6/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.524057 pydash-7.0.6/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.527035 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551593 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551682 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551779 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.551880 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552140 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552232 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552329 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552413 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552498 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552596 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552698 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.552952 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553036 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553123 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553214 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553302 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.525272 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553403 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553663 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553766 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.553856 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.554127 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.554213 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.554458 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.554547 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.554793 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.554880 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555107 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555310 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555399 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555487 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555576 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555666 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555757 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.555998 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556096 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556186 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556270 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556367 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556462 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556551 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.6/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.527160 pydash-7.0.6/.tox/py37/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.527217 pydash-7.0.6/.tox/py37/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.527271 pydash-7.0.6/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.530170 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556647 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556756 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556867 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.556972 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.557278 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.557400 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.557523 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.557636 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.557754 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.557879 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558177 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558285 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558382 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558467 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558562 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558660 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.528424 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.558764 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559014 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559116 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559226 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559494 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559589 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559837 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.559935 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.560148 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.560238 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.560488 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.560739 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.560830 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.560918 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.529519 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561008 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561103 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561204 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561290 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561564 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561679 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561787 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.561903 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562024 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562291 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562398 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.6/.tox/py37/lib/python3.7/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.530284 pydash-7.0.6/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.530325 pydash-7.0.6/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.530366 pydash-7.0.6/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.533101 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562514 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562630 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562739 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.562861 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.563124 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.563243 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.563467 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.563615 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.563756 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.563879 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564002 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564317 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564450 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564581 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564710 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564843 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.564976 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.565093 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.531588 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.565214 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.565509 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.565647 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.565772 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.566060 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.566186 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.566451 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.566565 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.566816 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.566937 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.567321 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.567581 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.567702 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.567826 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.567953 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.568076 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.568204 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.568548 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.568690 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.568810 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.568939 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569069 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569377 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569499 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569620 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.6/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.533248 pydash-7.0.6/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.533309 pydash-7.0.6/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.533372 pydash-7.0.6/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.536973 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569744 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569862 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.569976 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570093 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570385 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570496 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570602 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570694 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570801 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.570901 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571009 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571277 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571390 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571499 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571607 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571703 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571789 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.534931 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.571888 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.572134 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.572221 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.572302 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.572554 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.572661 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.572897 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.573005 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.573275 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.573387 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.573631 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.573851 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.573941 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574029 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574130 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574216 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574308 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574576 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574675 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574759 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574860 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.574969 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.575230 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.575327 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.575429 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.6/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1396 2023-06-02 13:53:01.000000 pydash-7.0.6/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    41047 2023-07-29 19:24:08.000000 pydash-7.0.6/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.6/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.6/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)    44522 2023-07-29 19:57:35.589527 pydash-7.0.6/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.6/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.578343 pydash-7.0.6/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.578480 pydash-7.0.6/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.6/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.6/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.6/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5356 2023-06-24 16:30:19.000000 pydash-7.0.6/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.6/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.6/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.6/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.6/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.6/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.6/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.6/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.6/pylintrc
+-rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.6/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.6/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     2524 2023-07-29 19:57:35.589940 pydash-7.0.6/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.537346 pydash-7.0.6/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.582023 pydash-7.0.6/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-07-29 19:23:05.000000 pydash-7.0.6/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    69930 2023-07-06 13:41:49.000000 pydash-7.0.6/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.583776 pydash-7.0.6/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.6/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.6/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   126275 2023-07-29 19:21:21.000000 pydash-7.0.6/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.6/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.6/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.6/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.6/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.6/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.6/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.582665 pydash-7.0.6/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)    44522 2023-07-29 19:57:33.000000 pydash-7.0.6/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    16254 2023-07-29 19:57:35.000000 pydash-7.0.6/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-07-29 19:57:33.000000 pydash-7.0.6/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      289 2023-07-29 19:57:33.000000 pydash-7.0.6/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-07-29 19:57:33.000000 pydash-7.0.6/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.6/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.586749 pydash-7.0.6/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.6/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.537638 pydash-7.0.6/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.586935 pydash-7.0.6/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.6/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.6/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.6/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-07-29 19:57:35.589246 pydash-7.0.6/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.6/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    17085 2023-07-06 13:41:49.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.6/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.6/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.6/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.6/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.6/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.6/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.6/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.6/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.6/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.6/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.6/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.6/tox.ini
```

### Comparing `pydash-7.0.5/AUTHORS.rst` & `pydash-7.0.6/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/CHANGELOG.rst` & `pydash-7.0.6/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.6 (2023-07-29)
+-------------------
+
+- Fix typing for chaining interface for methods that use varargs. Thanks DeviousStoat_!
+
+
 v7.0.5 (2023-07-06)
 -------------------
 
-- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values.
+- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values. Thanks DeviousStoat_!
 
 
 v7.0.4 (2023-06-02)
 -------------------
 
 - Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
```

### Comparing `pydash-7.0.5/CONTRIBUTING.rst` & `pydash-7.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/LICENSE.rst` & `pydash-7.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/PKG-INFO` & `pydash-7.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.5
+Version: 7.0.6
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,18 +61,24 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.6 (2023-07-29)
+-------------------
+
+- Fix typing for chaining interface for methods that use varargs. Thanks DeviousStoat_!
+
+
 v7.0.5 (2023-07-06)
 -------------------
 
-- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values.
+- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values. Thanks DeviousStoat_!
 
 
 v7.0.4 (2023-06-02)
 -------------------
 
 - Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
```

### Comparing `pydash-7.0.5/README.rst` & `pydash-7.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/Makefile` & `pydash-7.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/api.rst` & `pydash-7.0.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/callbacks.rst` & `pydash-7.0.6/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/chaining.rst` & `pydash-7.0.6/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/conf.py` & `pydash-7.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/deeppath.rst` & `pydash-7.0.6/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/differences.rst` & `pydash-7.0.6/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/index.rst` & `pydash-7.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/quickstart.rst` & `pydash-7.0.6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/templating.rst` & `pydash-7.0.6/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/docs/upgrading.rst` & `pydash-7.0.6/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/pylintrc` & `pydash-7.0.6/pylintrc`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/setup.cfg` & `pydash-7.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/__init__.py` & `pydash-7.0.6/src/pydash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python port of Lo-Dash."""
 
-__version__ = "7.0.5"
+__version__ = "7.0.6"
 
 from .arrays import (
     chunk,
     compact,
     concat,
     difference,
     difference_by,
```

### Comparing `pydash-7.0.5/src/pydash/arrays.py` & `pydash-7.0.6/src/pydash/arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/chaining/all_funcs.py` & `pydash-7.0.6/src/pydash/chaining/all_funcs.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/chaining/all_funcs.pyi` & `pydash-7.0.6/src/pydash/chaining/all_funcs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,18 @@
     CurryRightFour,
     CurryRightOne,
     CurryRightThree,
     CurryRightTwo,
     CurryThree,
     CurryTwo,
     Debounce,
+    Disjoin,
     Flow,
     Iterated,
+    Juxtapose,
     Negate,
     Once,
     Partial,
     Rearg,
     Spread,
     Throttle,
 )
@@ -62,14 +64,16 @@
 P = ParamSpec("P")
 
 class AllFuncs:
     def chunk(self: "Chain[t.Sequence[T]]", size: int = 1) -> "Chain[t.List[t.Sequence[T]]]":
         return self._wrap(pyd.chunk)(size)
     def compact(self: "Chain[t.Iterable[t.Union[T, None]]]") -> "Chain[t.List[T]]":
         return self._wrap(pyd.compact)()
+    def concat(self: "Chain[t.Iterable[T]]", *arrays: t.Iterable[T]) -> "Chain[t.List[T]]":
+        return self._wrap(pyd.concat)(*arrays)
     def difference(self: "Chain[t.Iterable[T]]", *others: t.Iterable[T]) -> "Chain[t.List[T]]":
         return self._wrap(pyd.difference)(*others)
     @t.overload
     def difference_by(
         self: "Chain[t.Iterable[T]]",
         *others: t.Iterable[T],
         iteratee: t.Union[IterateeObjT, t.Callable[[T], t.Any], None]
@@ -210,14 +214,16 @@
     ) -> "Chain[t.List[t.Union[T, T2]]]": ...
     @t.overload
     def intercalate(
         self: "Chain[t.Iterable[T]]", separator: T2
     ) -> "Chain[t.List[t.Union[T, T2]]]": ...
     def intercalate(self, separator):
         return self._wrap(pyd.intercalate)(separator)
+    def interleave(self: "Chain[t.Iterable[T]]", *arrays: t.Iterable[T]) -> "Chain[t.List[T]]":
+        return self._wrap(pyd.interleave)(*arrays)
     def intersection(
         self: "Chain[t.Sequence[T]]", *others: t.Iterable[t.Any]
     ) -> "Chain[t.List[T]]":
         return self._wrap(pyd.intersection)(*others)
     @t.overload
     def intersection_by(
         self: "Chain[t.Sequence[T]]",
@@ -531,14 +537,18 @@
     ) -> "Chain[t.List[T]]": ...
     @t.overload
     def xor_with(
         self: "Chain[t.Sequence[T]]", *lists: t.Union[t.Iterable[T2], t.Callable[[T, T2], t.Any]]
     ) -> "Chain[t.List[T]]": ...
     def xor_with(self, *lists, **kwargs):
         return self._wrap(pyd.xor_with)(*lists, **kwargs)
+    def zip_(self: "Chain[t.Iterable[T]]", *arrays: t.Iterable[T]) -> "Chain[t.List[t.List[T]]]":
+        return self._wrap(pyd.zip_)(*arrays)
+    zip = zip_
+
     @t.overload
     def zip_object(
         self: "Chain[t.Iterable[t.Tuple[T, T2]]]", values: None = None
     ) -> "Chain[t.Dict[T, T2]]": ...
     @t.overload
     def zip_object(
         self: "Chain[t.Iterable[t.List[t.Union[T, T2]]]]", values: None = None
@@ -547,14 +557,42 @@
     def zip_object(self: "Chain[t.Iterable[T]]", values: t.List[T2]) -> "Chain[t.Dict[T, T2]]": ...
     def zip_object(self, values=None):
         return self._wrap(pyd.zip_object)(values)
     def zip_object_deep(
         self: "Chain[t.Iterable[t.Any]]", values: t.Union[t.List[t.Any], None] = None
     ) -> "Chain[t.Dict]":
         return self._wrap(pyd.zip_object_deep)(values)
+    @t.overload
+    def zip_with(
+        self: "Chain[t.Iterable[T]]",
+        *arrays: t.Iterable[T],
+        iteratee: t.Union[
+            t.Callable[[T, T, int, t.List[T]], T2],
+            t.Callable[[T, T, int], T2],
+            t.Callable[[T, T], T2],
+            t.Callable[[T], T2],
+        ]
+    ) -> "Chain[t.List[T2]]": ...
+    @t.overload
+    def zip_with(
+        self: "Chain[t.Iterable[T]]", *arrays: t.Iterable[T]
+    ) -> "Chain[t.List[t.List[T]]]": ...
+    @t.overload
+    def zip_with(
+        self: "Chain[t.Union[t.Iterable[T], t.Callable[[T, T, int, t.List[T]], T2], t.Callable[[T, T, int], T2], t.Callable[[T, T], T2], t.Callable[[T], T2]]]",
+        *arrays: t.Union[
+            t.Iterable[T],
+            t.Callable[[T, T, int, t.List[T]], T2],
+            t.Callable[[T, T, int], T2],
+            t.Callable[[T, T], T2],
+            t.Callable[[T], T2],
+        ]
+    ) -> "Chain[t.List[t.Union[t.List[T], T2]]]": ...
+    def zip_with(self, *arrays, **kwargs):
+        return self._wrap(pyd.zip_with)(*arrays, **kwargs)
     def tap(self: "Chain[T]", interceptor: t.Callable[[T], t.Any]) -> "Chain[T]":
         return self._wrap(pyd.tap)(interceptor)
     def thru(self: "Chain[T]", interceptor: t.Callable[[T], T2]) -> "Chain[T2]":
         return self._wrap(pyd.thru)(interceptor)
     @t.overload
     def at(self: "Chain[t.Mapping[T, T2]]", *paths: T) -> "Chain[t.List[t.Union[T2, None]]]": ...
     @t.overload
@@ -1360,14 +1398,18 @@
         return self._wrap(pyd.sort_by)(iteratee, reverse)
     def after(self: "Chain[t.Callable[P, T]]", n: t.SupportsInt) -> "Chain[After[P, T]]":
         return self._wrap(pyd.after)(n)
     def ary(self: "Chain[t.Callable[..., T]]", n: t.Union[t.SupportsInt, None]) -> "Chain[Ary[T]]":
         return self._wrap(pyd.ary)(n)
     def before(self: "Chain[t.Callable[P, T]]", n: t.SupportsInt) -> "Chain[Before[P, T]]":
         return self._wrap(pyd.before)(n)
+    def conjoin(
+        self: "Chain[t.Callable[[T], t.Any]]", *funcs: t.Callable[[T], t.Any]
+    ) -> "Chain[t.Callable[[t.Iterable[T]], bool]]":
+        return self._wrap(pyd.conjoin)(*funcs)
     @t.overload
     def curry(
         self: "Chain[t.Callable[[T1], T]]", arity: t.Union[int, None] = None
     ) -> "Chain[CurryOne[T1, T]]": ...
     @t.overload
     def curry(
         self: "Chain[t.Callable[[T1, T2], T]]", arity: t.Union[int, None] = None
@@ -1412,14 +1454,18 @@
         self: "Chain[t.Callable[P, T]]", wait: int, max_wait: t.Union[int, Literal[False]] = False
     ) -> "Chain[Debounce[P, T]]":
         return self._wrap(pyd.debounce)(wait, max_wait)
     def delay(
         self: "Chain[t.Callable[P, T]]", wait: int, *args: "P.args", **kwargs: "P.kwargs"
     ) -> "Chain[T]":
         return self._wrap(pyd.delay)(wait, *args, **kwargs)
+    def disjoin(
+        self: "Chain[t.Callable[[T], t.Any]]", *funcs: t.Callable[[T], t.Any]
+    ) -> "Chain[Disjoin[T]]":
+        return self._wrap(pyd.disjoin)(*funcs)
     @t.overload
     def flip(
         self: "Chain[t.Callable[[T1, T2, T3, T4, T5], T]]",
     ) -> "Chain[t.Callable[[T5, T4, T3, T2, T1], T]]": ...
     @t.overload
     def flip(
         self: "Chain[t.Callable[[T1, T2, T3, T4], T]]",
@@ -1455,14 +1501,16 @@
     ) -> "Chain[Flow[P, T]]": ...
     @t.overload
     def flow(
         self: "Chain[t.Callable[P, T2]]", func2: t.Callable[[T2], T]
     ) -> "Chain[Flow[P, T]]": ...
     @t.overload
     def flow(self: "Chain[t.Callable[P, T]]") -> "Chain[Flow[P, T]]": ...
+    def flow(self, *funcs):
+        return self._wrap(pyd.flow)(*funcs)
     @t.overload
     def flow_right(
         self: "Chain[t.Callable[[T4], T]]",
         func4: t.Callable[[T3], T4],
         func3: t.Callable[[T2], T3],
         func2: t.Callable[[T1], T2],
         func1: t.Callable[P, T1],
@@ -1480,16 +1528,22 @@
     ) -> "Chain[Flow[P, T]]": ...
     @t.overload
     def flow_right(
         self: "Chain[t.Callable[[T1], T]]", func1: t.Callable[P, T1]
     ) -> "Chain[Flow[P, T]]": ...
     @t.overload
     def flow_right(self: "Chain[t.Callable[P, T]]") -> "Chain[Flow[P, T]]": ...
+    def flow_right(self, *funcs):
+        return self._wrap(pyd.flow_right)(*funcs)
     def iterated(self: "Chain[t.Callable[[T], T]]") -> "Chain[Iterated[T]]":
         return self._wrap(pyd.iterated)()
+    def juxtapose(
+        self: "Chain[t.Callable[P, T]]", *funcs: t.Callable[P, T]
+    ) -> "Chain[Juxtapose[P, T]]":
+        return self._wrap(pyd.juxtapose)(*funcs)
     def negate(self: "Chain[t.Callable[P, t.Any]]") -> "Chain[Negate[P]]":
         return self._wrap(pyd.negate)()
     def once(self: "Chain[t.Callable[P, T]]") -> "Chain[Once[P, T]]":
         return self._wrap(pyd.once)()
     @t.overload
     def over_args(
         self: "Chain[t.Callable[[T1, T2, T3, T4, T5], T]]",
@@ -2828,14 +2882,16 @@
         return self._wrap(pyd.unescape)()
     def upper_case(self: "Chain[t.Any]") -> "Chain[str]":
         return self._wrap(pyd.upper_case)()
     def upper_first(self: "Chain[str]") -> "Chain[str]":
         return self._wrap(pyd.upper_first)()
     def unquote(self: "Chain[t.Any]", quote_char: t.Any = '"') -> "Chain[str]":
         return self._wrap(pyd.unquote)(quote_char)
+    def url(self: "Chain[t.Any]", *paths: t.Any, **params: t.Any) -> "Chain[str]":
+        return self._wrap(pyd.url)(*paths, **params)
     def words(self: "Chain[t.Any]", pattern: t.Union[str, None] = None) -> "Chain[t.List[str]]":
         return self._wrap(pyd.words)(pattern)
     def attempt(
         self: "Chain[t.Callable[P, T]]", *args: "P.args", **kwargs: "P.kwargs"
     ) -> "Chain[t.Union[T, Exception]]":
         return self._wrap(pyd.attempt)(*args, **kwargs)
     @t.overload
@@ -2936,24 +2992,28 @@
         self: "Chain[PathT]", *args: t.Any, **kwargs: t.Any
     ) -> "Chain[t.Callable[..., t.Any]]":
         return self._wrap(pyd.method)(*args, **kwargs)
     def method_of(
         self: "Chain[t.Any]", *args: t.Any, **kwargs: t.Any
     ) -> "Chain[t.Callable[..., t.Any]]":
         return self._wrap(pyd.method_of)(*args, **kwargs)
+    def noop(self: "Chain[t.Any]", *args: t.Any, **kwargs: t.Any) -> "Chain[None]":
+        return self._wrap(pyd.noop)(*args, **kwargs)
     def over(self: "Chain[t.Iterable[t.Callable[P, T]]]") -> "Chain[t.Callable[P, t.List[T]]]":
         return self._wrap(pyd.over)()
     def over_every(self: "Chain[t.Iterable[t.Callable[P, t.Any]]]") -> "Chain[t.Callable[P, bool]]":
         return self._wrap(pyd.over_every)()
     def over_some(self: "Chain[t.Iterable[t.Callable[P, t.Any]]]") -> "Chain[t.Callable[P, bool]]":
         return self._wrap(pyd.over_some)()
     def property_(self: "Chain[PathT]") -> "Chain[t.Callable[[t.Any], t.Any]]":
         return self._wrap(pyd.property_)()
     property = property_
 
+    def properties(self: "Chain[t.Any]", *paths: t.Any) -> "Chain[t.Callable[[t.Any], t.Any]]":
+        return self._wrap(pyd.properties)(*paths)
     def property_of(self: "Chain[t.Any]") -> "Chain[t.Callable[[PathT], t.Any]]":
         return self._wrap(pyd.property_of)()
     @t.overload
     def random(
         self: "Chain[int]", stop: int = 1, *, floating: Literal[False] = False
     ) -> "Chain[int]": ...
     @t.overload
@@ -2973,20 +3033,26 @@
         return self._wrap(pyd.random)(stop, floating)
     @t.overload
     def range_(self: "Chain[int]") -> "Chain[t.Generator[int, None, None]]": ...
     @t.overload
     def range_(
         self: "Chain[int]", stop: int, step: int = 1
     ) -> "Chain[t.Generator[int, None, None]]": ...
+    def range_(self, *args):
+        return self._wrap(pyd.range_)(*args)
+    range = range_
+
     @t.overload
     def range_right(self: "Chain[int]") -> "Chain[t.Generator[int, None, None]]": ...
     @t.overload
     def range_right(
         self: "Chain[int]", stop: int, step: int = 1
     ) -> "Chain[t.Generator[int, None, None]]": ...
+    def range_right(self, *args):
+        return self._wrap(pyd.range_right)(*args)
     @t.overload
     def result(self: "Chain[None]", key: t.Any, default: None = None) -> "Chain[None]": ...
     @t.overload
     def result(self: "Chain[None]", key: t.Any, default: T) -> "Chain[T]": ...
     @t.overload
     def result(self: "Chain[t.Any]", key: t.Any, default: t.Any = None) -> "Chain[t.Any]": ...
     def result(self, key, default=None):
```

### Comparing `pydash-7.0.5/src/pydash/chaining/chaining.py` & `pydash-7.0.6/src/pydash/chaining/chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/collections.py` & `pydash-7.0.6/src/pydash/collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/functions.py` & `pydash-7.0.6/src/pydash/functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/helpers.py` & `pydash-7.0.6/src/pydash/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/numerical.py` & `pydash-7.0.6/src/pydash/numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/objects.py` & `pydash-7.0.6/src/pydash/objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/predicates.py` & `pydash-7.0.6/src/pydash/predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/strings.py` & `pydash-7.0.6/src/pydash/strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/types.py` & `pydash-7.0.6/src/pydash/types.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash/utilities.py` & `pydash-7.0.6/src/pydash/utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/src/pydash.egg-info/PKG-INFO` & `pydash-7.0.6/src/pydash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.5
+Version: 7.0.6
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,18 +61,24 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.6 (2023-07-29)
+-------------------
+
+- Fix typing for chaining interface for methods that use varargs. Thanks DeviousStoat_!
+
+
 v7.0.5 (2023-07-06)
 -------------------
 
-- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values.
+- Fix typing for ``find_index`` and ``find_last_index`` by allowing ``predicate`` argument to be callback shorthand values. Thanks DeviousStoat_!
 
 
 v7.0.4 (2023-06-02)
 -------------------
 
 - Exclude incompatible ``typing-extensions`` version ``4.6.0`` from install requirements. Incompatibility was fixed in ``4.6.1``.
```

### Comparing `pydash-7.0.5/src/pydash.egg-info/SOURCES.txt` & `pydash-7.0.6/src/pydash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tasks.py` & `pydash-7.0.6/tasks.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/build/testresults/junit.xml` & `pydash-7.0.6/tests/build/testresults/junit.xml`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/helpers.py` & `pydash-7.0.6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_arrays.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_chaining.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_collections.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_functions.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_numerical.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_objects.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_predicates.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_strings.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/pytest_mypy_testing/test_utilities.py` & `pydash-7.0.6/tests/pytest_mypy_testing/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_arrays.py` & `pydash-7.0.6/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_chaining.py` & `pydash-7.0.6/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_collections.py` & `pydash-7.0.6/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_functions.py` & `pydash-7.0.6/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_numerical.py` & `pydash-7.0.6/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_objects.py` & `pydash-7.0.6/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_predicates.py` & `pydash-7.0.6/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_strings.py` & `pydash-7.0.6/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.5/tests/test_utilities.py` & `pydash-7.0.6/tests/test_utilities.py`

 * *Files identical despite different names*

