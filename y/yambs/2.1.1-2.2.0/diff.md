# Comparing `tmp/yambs-2.1.1.tar.gz` & `tmp/yambs-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-2.1.1.tar", last modified: Sat Jul 22 21:25:12 2023, max compression
+gzip compressed data, was "yambs-2.2.0.tar", last modified: Sat Jul 29 06:53:33 2023, max compression
```

## Comparing `yambs-2.1.1.tar` & `yambs-2.2.0.tar`

### file list

```diff
@@ -1,96 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-22 21:24:06.000000 yambs-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-22 21:25:12.719061 yambs-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-22 21:24:06.000000 yambs-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-22 21:24:06.000000 yambs-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 21:25:12.719061 yambs-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-22 21:24:06.000000 yambs-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.711061 yambs-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-22 21:24:06.000000 yambs-2.1.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-22 21:24:06.000000 yambs-2.1.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/generate/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.719061 yambs-2.1.1/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-22 21:24:06.000000 yambs-2.1.1/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:25:12.715061 yambs-2.1.1/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-22 21:25:12.000000 yambs-2.1.1/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-22 21:25:12.000000 yambs-2.1.1/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:25:12.000000 yambs-2.1.1/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-22 21:25:12.000000 yambs-2.1.1/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-22 21:25:12.000000 yambs-2.1.1/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 21:25:12.000000 yambs-2.1.1/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 06:52:19.000000 yambs-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-29 06:53:33.786966 yambs-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-29 06:52:19.000000 yambs-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-29 06:52:19.000000 yambs-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 06:53:33.786966 yambs-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-29 06:52:19.000000 yambs-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.778967 yambs-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 06:52:19.000000 yambs-2.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-29 06:52:19.000000 yambs-2.2.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.778967 yambs-2.2.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/handlers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/handlers/yambs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-2.1.1/LICENSE` & `yambs-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/PKG-INFO` & `yambs-2.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.1.1
+Version: 2.2.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=f95824d927cb8814a559ce41e03ebd38
+    hash=9fd78d02f6bd1c0baddfb2fa7ba65d51
     =====================================
 -->
 
-# yambs ([2.1.1](https://pypi.org/project/yambs/))
+# yambs ([2.2.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -42,17 +39,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/yambs.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
-* [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
```

### Comparing `yambs-2.1.1/README.md` & `yambs-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=f95824d927cb8814a559ce41e03ebd38
+    hash=9fd78d02f6bd1c0baddfb2fa7ba65d51
     =====================================
 -->
 
-# yambs ([2.1.1](https://pypi.org/project/yambs/))
+# yambs ([2.2.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -19,17 +19,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/yambs.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
-* [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
```

### Comparing `yambs-2.1.1/pyproject.toml` & `yambs-2.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "2.1.1"
+version = "2.2.0"
 description = "Yet another meta build-system."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
@@ -34,12 +31,13 @@
   "flake8",
   "black",
   "ruff",
   "mypy",
   "isort",
   "yamllint",
   "setuptools-wrapper",
-  "types-setuptools"
+  "types-setuptools",
+  "types-requests"
 ]
 
 [project.scripts]
 mbs = "yambs.entry:main"
```

### Comparing `yambs-2.1.1/setup.py` & `yambs-2.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=7cd5513daf171d1a95f64dc81343a73b
+# hash=f3af34a4b5815c617489419b194b30b5
 # =====================================
 
 """
 yambs - Package definition for distribution.
 """
 
 # third-party
@@ -24,17 +24,14 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.8",
-        "3.9",
-        "3.10",
         "3.11",
     ],
 }
 setup(
     pkg_info,
     author_info,
 )
```

### Comparing `yambs-2.1.1/tests/test_entry.py` & `yambs-2.2.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/aggregation/__init__.py` & `yambs-2.2.0/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/app.py` & `yambs-2.2.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/commands/all.py` & `yambs-2.2.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/commands/common.py` & `yambs-2.2.0/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/commands/dist.py` & `yambs-2.2.0/yambs/commands/dist.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/commands/gen.py` & `yambs-2.2.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/commands/native.py` & `yambs-2.2.0/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/commands/uf2conv.py` & `yambs-2.2.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/config/__init__.py` & `yambs-2.2.0/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/config/board.py` & `yambs-2.2.0/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/config/common.py` & `yambs-2.2.0/yambs/config/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 A module for common configuration interfaces.
 """
 
 # built-in
 from pathlib import Path
-from typing import Any, Dict, NamedTuple, Optional, Type, TypeVar
+from typing import Any, Dict, NamedTuple, Optional, Set, Type, TypeVar
 
 # third-party
 from vcorelib.dict import merge
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io import DEFAULT_INCLUDES_KEY
-from vcorelib.io.types import JsonObject as _JsonObject
+from vcorelib.io import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike, find_file, normalize
 
 # internal
 from yambs import PKG_NAME
+from yambs.dependency.config import Dependency
 from yambs.schemas import YambsDictCodec as _YambsDictCodec
 
 T = TypeVar("T", bound="CommonConfig")
 DEFAULT_CONFIG = f"{PKG_NAME}.yaml"
 
 
 class Project(NamedTuple):
@@ -69,14 +70,15 @@
     data: Dict[str, Any]
 
     root: Path
     src_root: Path
     build_root: Path
     ninja_root: Path
     dist_root: Path
+    third_party_root: Path
 
     file: Optional[Path]
 
     def directory(self, name: str, mkdir: bool = True) -> Path:
         """Get a configurable directory."""
 
         name_root = Path(str(self.data[name]))
@@ -94,19 +96,27 @@
         self.data = data
         self.root = Path()
 
         self.src_root = self.directory("src_root")
         self.build_root = self.directory("build_root")
         self.ninja_root = self.directory("ninja_out")
         self.dist_root = self.directory("dist_out")
+        self.third_party_root = self.directory("third_party_root")
 
         self.file = None
 
         self.project = Project.create(data["project"])  # type: ignore
 
+        # Collect project dependency data.
+        self.dependencies: Set[Dependency] = set()
+        for dep in data.get("dependencies", []):  # type: ignore
+            new_dep = Dependency(data=dep, verify=False)  # type: ignore
+            new_dep.github.setdefault("owner", self.project.owner)
+            self.dependencies.add(new_dep)
+
     @classmethod
     def load(
         cls: Type[T],
         path: Pathlike = DEFAULT_CONFIG,
         package_config: str = DEFAULT_CONFIG,
         root: Pathlike = None,
     ) -> T:
```

### Comparing `yambs-2.1.1/yambs/data/includes/chips.yaml` & `yambs-2.2.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/includes/infineon.yaml` & `yambs-2.2.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/includes/microchip.yaml` & `yambs-2.2.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/native.yaml` & `yambs-2.2.0/yambs/data/native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/schemas/Chip.yaml` & `yambs-2.2.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/schemas/Config.yaml` & `yambs-2.2.0/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/schemas/Native.yaml` & `yambs-2.2.0/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/templates/native_rules.ninja.j2` & `yambs-2.2.0/yambs/data/templates/native_rules.ninja.j2`

 * *Files 20% similar despite different names*

```diff
@@ -12,13 +12,20 @@
 {% if common_ldflags %}
 
 ldflags ={% for flag in common_ldflags %} {{flag}}{% endfor %}
 
 {% endif %}
 
 rule link
-  command = $ld $cflags $ldflags -Wl,-Map=$out.map $in -o $out
+  command = $ld $cflags -Wl,-Map=$out.map $in $ldflags -o $out
 
 rule ar
   command = ar rcs $out $in
 
 build_dir = {{build_root}}/$variant
+
+rule script
+  command = /bin/bash $in $out
+
+build $build_dir/third_party.txt: script $third_party_dir/third_party.sh
+
+build ${variant}_third_party: phony $build_dir/third_party.txt
```

### Comparing `yambs-2.1.1/yambs/data/templates/rules.ninja.j2` & `yambs-2.2.0/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/data/uf2families.json` & `yambs-2.2.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/dist/__init__.py` & `yambs-2.2.0/yambs/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/entry.py` & `yambs-2.2.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/environment/__init__.py` & `yambs-2.2.0/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/environment/native.py` & `yambs-2.2.0/yambs/environment/native.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # third-party
 from vcorelib.io import ARBITER
 from vcorelib.logging import LoggerMixin
 
 # internal
 from yambs.aggregation import collect_files, populate_sources, sources_headers
 from yambs.config.native import Native
+from yambs.dependency.manager import DependencyManager
 from yambs.generate.common import get_jinja, render_template
 from yambs.generate.ninja import write_continuation
 from yambs.generate.ninja.format import render_format
 from yambs.generate.variants import generate as generate_variants
 from yambs.translation import BUILD_DIR_PATH, get_translator
 
 
@@ -32,14 +33,18 @@
     def __init__(self, config: Native) -> None:
         """Initialize this instance."""
 
         super().__init__()
 
         self.config = config
 
+        self.dependency_manager = DependencyManager(
+            self.config.third_party_root
+        )
+
         # Collect sources.
         self.sources = collect_files(config.src_root)
         self.apps: Set[Path] = set()
         self.regular: Set[Path] = set()
         populate_sources(
             self.sources, config.src_root, self.apps, self.regular
         )
@@ -109,14 +114,18 @@
 
             stream.write(line + str(out))
 
             for file in outputs:
                 write_continuation(stream, offset)
                 stream.write(str(file))
 
+            # Executables can't be linked until third-party dependencies are
+            # actually built.
+            stream.write(" | ${variant}_third_party")
+
             stream.write(linesep + linesep)
 
         line = "build ${variant}_apps: phony "
         offset = " " * len(line)
 
         elfs_list = list(elfs.values())
 
@@ -170,14 +179,29 @@
                 },
             )
 
     def generate(self, sources_only: bool = False) -> None:
         """Generate ninja files."""
 
         if not sources_only:
+            # Audit dependencies.
+            for dep in self.config.dependencies:
+                self.dependency_manager.audit(dep)
+
+            # Create build script.
+            self.dependency_manager.save(logger=self.logger)
+
+            # Handle compile and link flags generated by the third-party pass.
+            self.config.data["common_cflags"].extend(
+                self.dependency_manager.compile_flags
+            )
+            self.config.data["common_ldflags"].extend(
+                self.dependency_manager.link_flags
+            )
+
             # Render templates.
             generate_variants(
                 self.jinja, self.config, self.config.data["cflag_groups"]
             )
             self.render(self.config.root, "build.ninja")
             for template in ["all", "rules"]:
                 self.render(self.config.ninja_root, f"{template}.ninja")
```

### Comparing `yambs-2.1.1/yambs/generate/__init__.py` & `yambs-2.2.0/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/architectures.py` & `yambs-2.2.0/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/boards.py` & `yambs-2.2.0/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/chips.py` & `yambs-2.2.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/common.py` & `yambs-2.2.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/ninja/__init__.py` & `yambs-2.2.0/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/ninja/format.py` & `yambs-2.2.0/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/toolchains.py` & `yambs-2.2.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/generate/variants.py` & `yambs-2.2.0/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/schemas.py` & `yambs-2.2.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/translation/__init__.py` & `yambs-2.2.0/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs/uf2/__init__.py` & `yambs-2.2.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.1.1/yambs.egg-info/PKG-INFO` & `yambs-2.2.0/yambs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.1.1
+Version: 2.2.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=f95824d927cb8814a559ce41e03ebd38
+    hash=9fd78d02f6bd1c0baddfb2fa7ba65d51
     =====================================
 -->
 
-# yambs ([2.1.1](https://pypi.org/project/yambs/))
+# yambs ([2.2.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -42,17 +39,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/yambs.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.8`](https://docs.python.org/3.8/)
-* [`python3.9`](https://docs.python.org/3.9/)
-* [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
```

### Comparing `yambs-2.1.1/yambs.egg-info/SOURCES.txt` & `yambs-2.2.0/yambs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,18 @@
 yambs/data/includes/infineon.yaml
 yambs/data/includes/microchip.yaml
 yambs/data/schemas/Architecture.yaml
 yambs/data/schemas/Board.yaml
 yambs/data/schemas/Chip.yaml
 yambs/data/schemas/CommonConfig.yaml
 yambs/data/schemas/Config.yaml
+yambs/data/schemas/Dependency.yaml
+yambs/data/schemas/Github.yaml
 yambs/data/schemas/Native.yaml
+yambs/data/schemas/Project.yaml
 yambs/data/schemas/Toolchain.yaml
 yambs/data/schemas/Variant.yaml
 yambs/data/schemas/config_common.yaml
 yambs/data/schemas/entry_common.yaml
 yambs/data/schemas/toolchain_common.yaml
 yambs/data/templates/all.ninja.j2
 yambs/data/templates/architecture.ninja.j2
@@ -57,21 +60,30 @@
 yambs/data/templates/compile_commands.ninja.j2
 yambs/data/templates/native_all.ninja.j2
 yambs/data/templates/native_build.ninja.j2
 yambs/data/templates/native_rules.ninja.j2
 yambs/data/templates/rules.ninja.j2
 yambs/data/templates/toolchain.ninja.j2
 yambs/data/templates/variant.ninja.j2
+yambs/dependency/__init__.py
+yambs/dependency/config.py
+yambs/dependency/github.py
+yambs/dependency/manager.py
+yambs/dependency/state.py
+yambs/dependency/handlers/__init__.py
+yambs/dependency/handlers/types.py
+yambs/dependency/handlers/yambs.py
 yambs/dist/__init__.py
 yambs/environment/__init__.py
 yambs/environment/native.py
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
 yambs/generate/toolchains.py
 yambs/generate/variants.py
 yambs/generate/ninja/__init__.py
 yambs/generate/ninja/format.py
+yambs/github/__init__.py
 yambs/translation/__init__.py
 yambs/uf2/__init__.py
```

