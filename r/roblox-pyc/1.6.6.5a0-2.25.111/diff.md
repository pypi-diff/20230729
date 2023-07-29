# Comparing `tmp/roblox-pyc-1.6.6.5a0.tar.gz` & `tmp/roblox-pyc-2.25.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-1.6.6.5a0.tar", last modified: Sun Jul  9 20:03:59 2023, max compression
+gzip compressed data, was "roblox-pyc-2.25.111.tar", last modified: Sat Jul 29 20:02:13 2023, max compression
```

## Comparing `roblox-pyc-1.6.6.5a0.tar` & `roblox-pyc-2.25.111.tar`

### file list

```diff
@@ -1,35 +1,129 @@
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 20:03:59.818242 roblox-pyc-1.6.6.5a0/
--rw-r--r--   0 aaravs     (501) staff       (20)    34525 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/LICENSE
--rw-r--r--   0 aaravs     (501) staff       (20)     3010 2023-07-09 20:03:59.818469 roblox-pyc-1.6.6.5a0/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)     2784 2023-07-09 17:36:20.000000 roblox-pyc-1.6.6.5a0/README.md
--rw-r--r--   0 aaravs     (501) staff       (20)       89 2023-07-09 01:34:29.000000 roblox-pyc-1.6.6.5a0/pyproject.toml
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 20:03:59.798189 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/
--rw-r--r--   0 aaravs     (501) staff       (20)     3010 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 aaravs     (501) staff       (20)      606 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        1 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      102 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 aaravs     (501) staff       (20)       43 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 aaravs     (501) staff       (20)        4 2023-07-09 20:03:59.000000 roblox-pyc-1.6.6.5a0/roblox_pyc.egg-info/top_level.txt
--rw-r--r--   0 aaravs     (501) staff       (20)      243 2023-07-09 20:03:59.819423 roblox-pyc-1.6.6.5a0/setup.cfg
--rw-r--r--   0 aaravs     (501) staff       (20)      440 2023-07-09 15:41:08.000000 roblox-pyc-1.6.6.5a0/setup.py
-drwxr-xr-x   0 aaravs     (501) staff       (20)        0 2023-07-09 20:03:59.817083 roblox-pyc-1.6.6.5a0/src/
--rw-r--r--   0 aaravs     (501) staff       (20)       38 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/__init__.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1464 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/binopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      382 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/boolopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)      450 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/cmpopdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1848 2023-07-09 20:00:46.000000 roblox-pyc-1.6.6.5a0/src/cnodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)      800 2023-07-09 03:44:33.000000 roblox-pyc-1.6.6.5a0/src/colortext.py
--rw-r--r--   0 aaravs     (501) staff       (20)      790 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/config.py
--rw-r--r--   0 aaravs     (501) staff       (20)     1050 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/context.py
--rw-r--r--   0 aaravs     (501) staff       (20)      447 2023-07-09 15:13:23.000000 roblox-pyc-1.6.6.5a0/src/cpAST.py
--rw-r--r--   0 aaravs     (501) staff       (20)      404 2023-07-09 20:02:43.000000 roblox-pyc-1.6.6.5a0/src/ctranslator.py
--rw-r--r--   0 aaravs     (501) staff       (20)      482 2023-07-09 17:33:56.000000 roblox-pyc-1.6.6.5a0/src/header.py
--rw-r--r--   0 aaravs     (501) staff       (20)      282 2023-07-09 01:58:37.000000 roblox-pyc-1.6.6.5a0/src/loopcounter.py
--rw-r--r--   0 aaravs     (501) staff       (20)    21165 2023-07-09 17:23:29.000000 roblox-pyc-1.6.6.5a0/src/luainit.py
--rw-r--r--   0 aaravs     (501) staff       (20)      181 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/nameconstdesc.py
--rw-r--r--   0 aaravs     (501) staff       (20)    27684 2023-07-09 01:59:38.000000 roblox-pyc-1.6.6.5a0/src/nodevisitor.py
--rw-r--r--   0 aaravs     (501) staff       (20)     2153 2023-07-09 17:33:27.000000 roblox-pyc-1.6.6.5a0/src/pytranslator.py
--rw-r--r--   0 aaravs     (501) staff       (20)     7632 2023-07-09 18:40:50.000000 roblox-pyc-1.6.6.5a0/src/robloxpy.py
--rw-r--r--   0 aaravs     (501) staff       (20)      642 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/symbolsstack.py
--rw-r--r--   0 aaravs     (501) staff       (20)      157 2023-07-07 21:26:51.000000 roblox-pyc-1.6.6.5a0/src/tokenendmode.py
--rw-r--r--   0 aaravs     (501) staff       (20)      567 2023-07-08 14:04:57.000000 roblox-pyc-1.6.6.5a0/src/unaryopdesc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.736924 roblox-pyc-2.25.111/
+-rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-29 20:02:13.736924 roblox-pyc-2.25.111/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.724924 roblox-pyc-2.25.111/roblox_pyc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-29 20:02:13.000000 roblox-pyc-2.25.111/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-29 20:02:13.000000 roblox-pyc-2.25.111/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 20:02:13.000000 roblox-pyc-2.25.111/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-29 20:02:13.000000 roblox-pyc-2.25.111/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 20:02:13.000000 roblox-pyc-2.25.111/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 20:02:13.000000 roblox-pyc-2.25.111/roblox_pyc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.728924 roblox-pyc-2.25.111/robloxpyc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.728924 roblox-pyc-2.25.111/robloxpyc/LuauAST/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/bundle.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.728924 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/List.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/create.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/enums.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/globals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/strings.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/impl/typeGuards.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.728924 roblox-pyc-2.25.111/robloxpyc/LuauAST/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/types/mapping.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/types/nodes.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/types/operators.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.728924 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/assert.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/getKindName.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/isMetamethod.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/isReservedClassField.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/isReservedIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/isValidIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauAST/util/isValidNumberLiteral.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.728924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/RenderState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.720924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.732924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.732924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderCallExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderComputedIndexExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderMethodCallExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderParenthesizedExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderPropertyAccessExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderTemporaryIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderArray.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderBinaryExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderMap.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderMixedTable.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderNumberLiteral.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderSet.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.732924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/fields/renderMapField.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.732924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderBreakStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderCallStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderContinueStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderDoStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderRepeatStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderReturnStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/nodes/statements/renderWhileStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/render.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/solveTempIds.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.736924 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/getEnding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/getOrSetDefault.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/getSafeBracketEquals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/identity.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/needsParentheses.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/renderArguments.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/renderParameters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/renderStatements.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/LuauRenderer/util/visit.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:13.736924 roblox-pyc-2.25.111/robloxpyc/__communication__/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/__communication__/cfg.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/basecompilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/binopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/boolopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/climaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/cmpopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/cnodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/colortext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/configmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/cpAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/ctranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/errormanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/installationmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/loopcounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/luainit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/luainitlua.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    49380 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/nameconstdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/nodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62675 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/pytranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/robloxpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/symbolsstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/textcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/tokenendmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/unaryopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/wally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/robloxpyc/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-29 20:02:13.736924 roblox-pyc-2.25.111/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-29 20:02:04.000000 roblox-pyc-2.25.111/setup.py
```

### Comparing `roblox-pyc-1.6.6.5a0/LICENSE` & `roblox-pyc-2.25.111/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5a0/src/config.py` & `roblox-pyc-2.25.111/robloxpyc/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5a0/src/luainit.py` & `roblox-pyc-2.25.111/robloxpyc/luainitlua.lua`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,312 @@
-initcode = """
+--// AsynchronousAI @Dev98799 \\--
+----------------------------------------------------------------------------------------
+-- stdlib used to hold built in functions wrappers and libraries                      --
+----------------------------------------------------------------------------------------
+
+-- stdlib Version 2.5.9 --
+
+local module = { }
+
+-- Language used for gamewrapper (from Highlighter by boatbomber)
+local language = {
+	-- Luau Functions
+	["assert"] = "function",
+	["error"] = "function",
+	["getfenv"] = "function",
+	["getmetatable"] = "function",
+	["ipairs"] = "function",
+	["loadstring"] = "function",
+	["newproxy"] = "function",
+	["next"] = "function",
+	["pairs"] = "function",
+	["pcall"] = "function",
+	["print"] = "function",
+	["rawequal"] = "function",
+	["rawget"] = "function",
+	["rawlen"] = "function",
+	["rawset"] = "function",
+	["select"] = "function",
+	["setfenv"] = "function",
+	["setmetatable"] = "function",
+	["tonumber"] = "function",
+	["tostring"] = "function",
+	["unpack"] = "function",
+	["xpcall"] = "function",
+
+	-- Luau Functions (Deprecated)
+	["collectgarbage"] = "function",
+
+	-- Luau Variables
+	["_G"] = "table",
+	["_VERSION"] = "string",
+
+	-- Luau Tables
+	["bit32"] = "table",
+	["coroutine"] = "table",
+	["debug"] = "table",
+	["math"] = "table",
+	["os"] = "table",
+	["string"] = "table",
+	["table"] = "table",
+	["utf8"] = "table",
+
+	-- Roblox Functions
+	["DebuggerManager"] = "function",
+	["delay"] = "function",
+	["gcinfo"] = "function",
+	["PluginManager"] = "function",
+	["require"] = "function",
+	["settings"] = "function",
+	["spawn"] = "function",
+	["tick"] = "function",
+	["time"] = "function",
+	["UserSettings"] = "function",
+	["wait"] = "function",
+	["warn"] = "function",
+
+	-- Roblox Functions (Deprecated)
+	["Delay"] = "function",
+	["ElapsedTime"] = "function",
+	["elapsedTime"] = "function",
+	["printidentity"] = "function",
+	["Spawn"] = "function",
+	["Stats"] = "function",
+	["stats"] = "function",
+	["Version"] = "function",
+	["version"] = "function",
+	["Wait"] = "function",
+	["ypcall"] = "function",
+
+	-- Roblox Variables
+	["game"] = "Instance",
+	["plugin"] = "Instance",
+	["script"] = "Instance",
+	["shared"] = "Instance",
+	["workspace"] = "Instance",
+
+	-- Roblox Variables (Deprecated)
+	["Game"] = "Instance",
+	["Workspace"] = "Instance",
+
+	-- Roblox Tables
+	["Axes"] = "table",
+	["BrickColor"] = "table",
+	["CatalogSearchParams"] = "table",
+	["CFrame"] = "table",
+	["Color3"] = "table",
+	["ColorSequence"] = "table",
+	["ColorSequenceKeypoint"] = "table",
+	["DateTime"] = "table",
+	["DockWidgetPluginGuiInfo"] = "table",
+	["Enum"] = "table",
+	["Faces"] = "table",
+	["FloatCurveKey"] = "table",
+	["Font"] = "table",
+	["Instance"] = "table",
+	["NumberRange"] = "table",
+	["NumberSequence"] = "table",
+	["NumberSequenceKeypoint"] = "table",
+	["OverlapParams"] = "table",
+	["PathWaypoint"] = "table",
+	["PhysicalProperties"] = "table",
+	["Random"] = "table",
+	["Ray"] = "table",
+	["RaycastParams"] = "table",
+	["Rect"] = "table",
+	["Region3"] = "table",
+	["Region3int16"] = "table",
+	["RotationCurveKey"] = "table",
+	["SharedTable"] = "table",
+	["task"] = "table",
+	["TweenInfo"] = "table",
+	["UDim"] = "table",
+	["UDim2"] = "table",
+	["Vector2"] = "table",
+	["Vector2int16"] = "table",
+	["Vector3"] = "table",
+	["Vector3int16"] = "table",
+}
+function backwordreplace(s, old, new, occurrence) -- Lua implementation of the python function in robloxpy.py line ~600
+	local li = {}
+	local i = 1
+	while true do
+		local j = string.find(s, old, i, true)
+		if not j then
+			break
+		end
+		table.insert(li, string.sub(s, i, j - 1))
+		i = j + #old
+		if #li == occurrence then
+			break
+		end
+	end
+	table.insert(li, string.sub(s, i))
+	return table.concat(li, new)
+end
+local function parse_path(path, start_obj)
+	local obj = start_obj or game
+	local parts = string.split(path, "/")
+	for i, part in ipairs(parts) do
+		if part == "" then
+			obj = game
+		elseif part == "~" then
+			obj = game
+		elseif part == ".." then
+			obj = obj.Parent
+		else
+			if not obj:FindFirstChild(part) then
+				error("Object not found: " .. part .." in "..obj.Name.."\n\n\tDo not add .json, .txt, etc. to the end of file names, this version doesnt support them.")
+				return nil
+			end
+			obj = obj:FindFirstChild(part)
+		end
+	end
+	return obj
+end
 
-							--// AsynchronousAI @Dev98799 \\--
-				-------------------------------------------------------------------------------
-				-- this script was added by roblox-pyc plugin to give you the full experience.-- 
-				-- below you will find lua equivelents of built in python functions, it is   --         
-				-- free to use for your personal needs and feel free to edit it, if needed to--
-				-- reset it or update it simply delete it and use the plugin again to do so  --
-				-------------------------------------------------------------------------------
-
-									-- Version 1.0.0 --
-
-local module = {}
-local string_meta = {}
-local slicefun = function (sequence, start, stop, step) -- slice
+local slicefun = function (seq, start, stop, step)
 	local sliced = {}
-	local len = #sequence
-
-	-- Set default values for start, stop, and step
+	local len = #seq
 	start = start or 1
 	stop = stop or len
 	step = step or 1
-
-	-- Handle negative indices
 	if start < 0 then
 		start = len + start + 1
 	end
 	if stop < 0 then
 		stop = len + stop + 1
 	end
-
-	-- Adjust start and stop values if they are out of bounds
-	if start < 1 then
-		start = 1
-	elseif start > len then
-		start = len + 1
-	end
-	if stop < 1 then
-		stop = 1
-	elseif stop > len then
-		stop = len + 1
-	end
-
-	-- Build the sliced table
 	for i = start, stop - 1, step do
-		table.insert(sliced, sequence[i])
+		table.insert(sliced, seq[i])
 	end
-
-	-- Return the sliced table as a string if the input was a string
-	if typeof(sequence) == "string" then
-		return table.concat(sliced)
+	return sliced
+end
+function endswith(s, suffix) -- like string.endswith in python
+	return string.sub(s, -string.len(suffix)) == suffix
+end
+local wrappercache = setmetatable({}, {__mode = "k"})
+local wrap, unwrap
+unwrap = function(wrapped)
+	if type(wrapped) == "table" then
+		local real = {}
+		for k,v in next,wrapped do
+			real[k] = unwrap(v)
+		end
+		return real
+	else
+		local real = wrappercache[wrapped]
+		if real == nil then
+			return wrapped
+		end
+		return real
+	end
+end
+wrap = function(real, functions) 
+	functions = functions or {}
+	for w,r in next,wrappercache do
+		if r == real then
+			return w
+		end
 	end
 
-	return sliced
+	if type(real) == "userdata" then
+		local fake = newproxy(true)
+		local meta = getmetatable(fake)
+
+		meta.__index = function(s,k)
+
+			if table.find(functions, k) then
+				return functions[k]
+			end
+			if real[k] then
+				if typeof(real[k]) == "RBXScriptSignal" then
+					local newSignal = {}
+					setmetatable(newSignal, {
+						__call = function(func)
+							real:Connect(func)
+						end,
+						__index = function(index) return real[index] end
+					})
+					return newSignal
+				elseif type(real[k]) == "function" then
+					return function(...)
+						local returnval
+						local items = unpack(table.pack(...))
+						local s, e = pcall(function()
+							returnval = wrap(real[k](items))
+						end)
+						if (not s) then 
+							local rawcall = real[k](real, items)
+							returnval = wrap(rawcall)
+						elseif not s then
+							error(e)
+						end
+						return returnval
+					end
+				end
+				return wrap(real[k], functions)
+			end
+		end
+
+		meta.__newindex = function(s,k,v)
+			real[k] = v
+		end
+
+		meta.__tostring = function(s)
+			return tostring(real)
+		end
+
+		wrappercache[fake] = real
+		return fake
+
+	elseif type(real) == "function" then
+		return function(special, ...)
+			if special == selfcval then
+				return wrap(real(real, ...))
+			end
+			return wrap(real(special, ...))
+		end
+
+	elseif type(real) == "table" then
+		local fake = {}
+		for k,v in next,real do
+			fake[k] = wrap(v)
+		end
+		return fake
+
+	else
+		return real
+	end
 end
 
+local function set_metatable(var, mt)
+	local var_type = typeof(var)
+	if var_type == "Instance" then
+		var:SetAttribute("__metatable", mt)
+	elseif var_type == "table" then
+		setmetatable(var, mt)
+	end
+	return var
+end
+local function set_fun_meta(f, rmt)
+	return function()
+		local returnval = f()
+		if returnval == nil then return end
+		if type(returnval) == "function" then
+			return set_fun_meta(returnval, rmt)
+		else
+			set_metatable(rmt)
+		end
+	end
+end
 local gtype 
 if not typeof then
 	gtype = function(obj)
-		local type = typeof(obj)
+		local type = type(obj)
 		if type == "table" then
 			if obj._is_list then
 				return "list"
 			end
 			if obj._is_dict then
 				return "dict"
 			end
@@ -71,318 +316,280 @@
 else 
 	gtype = typeof
 end
 local typeof = gtype
 
 
 
-setmetatable(string_meta, {
-	__add = function(v1, v2)
-		if typeof(v1) == "string" and typeof(v2) == "string" then
-			return v1 .. v2
-		end
-		return v1 + v2
-	end,
-	__index = function(self, index)
-		if typeof(index) == "string" then
-			-- if it start with SLICE! then it is a slice, get the start, stop, and step values. sometimes the 3rd value is not there, so we need to check for that
-			if string.sub(index, 1, 6) == "SLICE!" then
-				local start, stop, step = string.match(index, "SLICE!%((%d+), (%d+), (%d+)%)")
-				if not step then
-					start, stop = string.match(index, "SLICE!%((%d+), (%d+)%)")
-					step = 1
-				end
-				return slicefun(self, tonumber(start), tonumber(stop), tonumber(step))
-			end
-		end
-	end,
-
-})
-local list = {}
-setmetatable(list, {
-	__call = function(_, t)
-		local result = {}
+function list(t)
+	local result = {}
 
-		result._is_list = true
+	result._is_list = true
 
-		result._data = {}
-		for _, v in ipairs(t) do
-			table.insert(result._data, v)
-		end
+	result._data = {}
+	for _, v in ipairs(t) do
+		table.insert(result._data, v)
+	end
 
-		local methods = {}
+	local methods = {}
 
-		methods.append = function(value)
-			table.insert(result._data, value)
-		end
+	methods.append = function(value)
+		table.insert(result._data, value)
+	end
 
-		methods.extend = function(iterable)
-			for value in iterable do
-				table.insert(result._data, value)
-			end
+	methods.extend = function(iterable)
+		for value in iterable do
+			table.insert(result._data, value)
 		end
+	end
 
-		methods.insert = function(index, value)
-			table.insert(result._data, index, value)
-		end
+	methods.insert = function(index, value)
+		table.insert(result._data, index, value)
+	end
 
-		methods.remove = function(value)
-			for i, v in ipairs(result._data) do
-				if value == v then
-					table.remove(result._data, i)
-					break
-				end
+	methods.remove = function(value)
+		for i, v in ipairs(result._data) do
+			if value == v then
+				table.remove(result._data, i)
+				break
 			end
 		end
+	end
 
-		methods.pop = function(index)
-			index = index or #result._data
-			local value = result._data[index]
-			table.remove(result._data, index)
-			return value
-		end
+	methods.pop = function(index)
+		index = index or #result._data
+		local value = result._data[index]
+		table.remove(result._data, index)
+		return value
+	end
 
-		methods.clear = function()
-			result._data = {}
-		end
+	methods.clear = function()
+		result._data = {}
+	end
 
-		methods.index = function(value, start, end_)
-			start = start or 1
-			end_ = end_ or #result._data
+	methods.index = function(value, start, end_)
+		start = start or 1
+		end_ = end_ or #result._data
 
-			for i = start, end_, 1 do
-				if result._data[i] == value then
-					return i
-				end
+		for i = start, end_, 1 do
+			if result._data[i] == value then
+				return i
 			end
-
-			return nil
 		end
 
-		methods.count = function(value)
-			local cnt = 0
-			for _, v in ipairs(result._data) do
-				if v == value then
-					cnt = cnt + 1
-				end
-			end
+		return nil
+	end
 
-			return cnt
+	methods.count = function(value)
+		local cnt = 0
+		for _, v in ipairs(result._data) do
+			if v == value then
+				cnt = cnt + 1
+			end
 		end
 
-		methods.sort = function(key, reverse)
-			key = key or nil
-			reverse = reverse or false
-
-			table.sort(result._data, function(a, b)
-				if reverse then
-					return a < b
-				end
+		return cnt
+	end
 
-				return a > b
-			end)
-		end
+	methods.sort = function(key, reverse)
+		key = key or nil
+		reverse = reverse or false
 
-		methods.reverse = function()
-			local new_data = {}
-			for i = #result._data, 1, -1 do
-				table.insert(new_data, result._data[i])
+		table.sort(result._data, function(a, b)
+			if reverse then
+				return a < b
 			end
 
-			result._data = new_data
-		end
+			return a > b
+		end)
+	end
 
-		methods.copy = function()
-			return list(result._data)
+	methods.reverse = function()
+		local new_data = {}
+		for i = #result._data, 1, -1 do
+			table.insert(new_data, result._data[i])
 		end
 
-		local iterator_index = nil
+		result._data = new_data
+	end
 
-		setmetatable(result, {
-			__index = function(self, index)
-				if typeof(index) == "number" then
-					if index < 0 then
-						index = #result._data + index
-					end
-					return rawget(result._data, index + 1)
-				end
-				if typeof(index) == "string" then
-					-- If it starts with SLICE! then it is a slice, get the start, stop, and step values. Sometimes the 3rd value is not there, so we need to check for that
-					if string.sub(index, 1, 6) == "SLICE!" then
-						local start, stop, step = string.match(index, "SLICE!%((%d+), (%d+), (%d+)%)")
-						if not step then
-							start, stop = string.match(index, "SLICE!%((%d+), (%d+)%)")
-							step = 1
-						end
-						return slicefun(self, tonumber(start), tonumber(stop), tonumber(step))
-					end
+	methods.copy = function()
+		return list(result._data)
+	end
+
+	local iterator_index = nil
+
+	setmetatable(result, {
+		__index = function(self, index)
+			if typeof(index) == "number" then
+				if index < 0 then
+					index = #result._data + index
 				end
+				return rawget(result._data, index + 1)
+			end
+			return methods[index]
+		end,
+		__newindex = function(self, index, value)
+			result._data[index] = value
+		end,
+		__call = function(self, _, idx)
+			if idx == nil and iterator_index ~= nil then
+				iterator_index = nil
+			end
 
-				return methods[index]
-			end,
-			__newindex = function(self, index, value)
-				result._data[index] = value
-			end,
-			__call = function(self, _, idx)
-				if idx == nil and iterator_index ~= nil then
-					iterator_index = nil
-				end
-
-				local v = nil
-				iterator_index, v = next(result._data, iterator_index)
-
-				return v
-			end,
-		})
-
-		return result
-	end,
-})
-
-local dict = {}
-setmetatable(dict, {
-	__call = function(_, t)
-		local result = {}
+			local v = nil
+			iterator_index, v = next(result._data, iterator_index)
 
-		result._is_dict = true
+			return v
+		end,
+	})
 
-		result._data = {}
-		for k, v in pairs(t) do
-			result._data[k] = v
-		end
+	return result
+end
+function dict(t)
+	local result = {}
 
-		local methods = {}
+	result._is_dict = true
 
-		local key_index = nil
+	result._data = {}
+	for k, v in pairs(t) do
+		result._data[k] = v
+	end
 
-		methods.clear = function()
-			result._data = {}
-		end
+	local methods = {}
 
-		methods.copy = function()
-			return dict(result._data)
-		end
+	local key_index = nil
 
-		methods.get = function(key, default)
-			default = default or nil
-			if result._data[key] == nil then
-				return default
-			end
+	methods.clear = function()
+		result._data = {}
+	end
 
-			return result._data[key]
-		end
+	methods.copy = function()
+		return dict(result._data)
+	end
 
-		methods.items = function()
-			return pairs(result._data)
+	methods.get = function(key, default)
+		default = default or nil
+		if result._data[key] == nil then
+			return default
 		end
 
-		methods.keys = function()
-			return function(self, idx, _) 
-				if idx == nil and key_index ~= nil then
-					key_index = nil
-				end
+		return result._data[key]
+	end
 
-				key_index, _ = next(result._data, key_index)
-				return key_index
-			end
-		end
+	methods.items = function()
+		return pairs(result._data)
+	end
 
-		methods.pop = function(key, default)
-			default = default or nil
-			if result._data[key] ~= nil then
-				local value = result._data[key]
-				result._data[key] = nil 
-				return key, value
+	methods.keys = function()
+		return function(self, idx, _) 
+			if idx == nil and key_index ~= nil then
+				key_index = nil
 			end
 
-			return key, default
+			key_index, _ = next(result._data, key_index)
+			return key_index
 		end
+	end
 
-		methods.popitem = function()
-			local key, value = next(result._data)
-			if key ~= nil then
-				result._data[key] = nil
-			end
-
+	methods.pop = function(key, default)
+		default = default or nil
+		if result._data[key] ~= nil then
+			local value = result._data[key]
+			result._data[key] = nil 
 			return key, value
 		end
 
-		methods.setdefault = function(key, default)
-			if result._data[key] == nil then
-				result._data[key] = default
-			end
+		return key, default
+	end
 
-			return result._data[key]
+	methods.popitem = function()
+		local key, value = next(result._data)
+		if key ~= nil then
+			result._data[key] = nil
 		end
 
-		methods.update = function(t)
-			assert(t._is_dict)
+		return key, value
+	end
 
-			for k, v in t.items() do
-				result._data[k] = v
-			end
+	methods.setdefault = function(key, default)
+		if result._data[key] == nil then
+			result._data[key] = default
 		end
 
-		methods.values = function()
-			return function(self, idx, _) 
-				if idx == nil and key_index ~= nil then
-					key_index = nil
-				end
+		return result._data[key]
+	end
 
-				key_index, value = next(result._data, key_index)
-				return value
+	methods.update = function(t)
+		assert(t._is_dict)
+
+		for k, v in t.items() do
+			result._data[k] = v
+		end
+	end
+
+	methods.values = function()
+		return function(self, idx, _) 
+			if idx == nil and key_index ~= nil then
+				key_index = nil
 			end
+
+			key_index, value = next(result._data, key_index)
+			return value
 		end
+	end
 
-		setmetatable(result, {
-			__index = function(self, index)
-				if typeof(index) == "string" then
-					-- If it starts with SLICE! then it is a slice, get the start, stop, and step values. Sometimes the 3rd value is not there, so we need to check for that
-					if string.sub(index, 1, 6) == "SLICE!" then
-						local start, stop, step = string.match(index, "SLICE!%((%d+), (%d+), (%d+)%)")
-						if not step then
-							start, stop = string.match(index, "SLICE!%((%d+), (%d+)%)")
-							step = 1
-						end
-						return slicefun(self, tonumber(start), tonumber(stop), tonumber(step))
+	setmetatable(result, {
+		__index = function(self, index)
+			if typeof(index) == "string" then
+				-- If it starts with SLICE! then it is a slice, get the start, stop, and step values. Sometimes the 3rd value is not there, so we need to check for that
+				if string.sub(index, 1, 6) == "SLICE!" then
+					local start, stop, step = string.match(index, "SLICE!%((%d+), (%d+), (%d+)%)")
+					if (not stop) and (not step) and start then -- 1 value
+						start = string.match(index, "SLICE!%((%d+), (%d+)%)")
+						step = 1
+						stop = -1
+					elseif not step then -- 2 values
+						start, stop = string.match(index, "SLICE!%((%d+), (%d+)%)")
+						step = 1
 					end
+					return slicefun(self, tonumber(start), tonumber(stop), tonumber(step))
 				end
-				if result._data[index] ~= nil then
-					return result._data[index]
-				end
-				return methods[index]
-			end,
-			__newindex = function(self, index, value)
-				result._data[index] = value
-			end,
-			__call = function(self, _, idx)
-				if idx == nil and key_index ~= nil then
-					key_index = nil
-				end
-
-				key_index, _ = next(result._data, key_index)
-
-				return key_index            
-			end,
-		})
+			end
+			if result._data[index] ~= nil then
+				return result._data[index]
+			end
+			return methods[index]
+		end,
+		__newindex = function(self, index, value)
+			result._data[index] = value
+		end,
+		__call = function(self, _, idx)
+			if idx == nil and key_index ~= nil then
+				key_index = nil
+			end
 
-		return result
-	end,
-})
+			key_index, _ = next(result._data, key_index)
 
+			return key_index            
+		end,
+	})
 
-local module = function(self)
-	return { 
-	py = {
-		{ -- python library
+	return result
+end
+--{SOURCECODEGOESHERE}--
 
-		},
-		{ -- built in
-		string_meta = string_meta, list = list, dict = dict, -- class meta
-		
+local libraries = {
+	["example"] = function() print("Example library!") end,
+	--{ITEMSGOHERE}--
+}
+local dependenciesfolder = script.Parent
+local pythonBuiltIn = function(inScript) -- python built in
+	local items = {
+		list = list, dict = dict, -- class meta
 		staticmethod = function(old_fun) -- staticmethod
 			local wrapper = function(first, ...)
 				return old_fun(...)
 			end
 
 			return wrapper
 		end,
@@ -443,15 +650,15 @@
 			if not e then a=1 else a=s end
 			if not e then b=s else b=e end
 			for i = a, b do
 				tb[#tb+1] = i
 			end
 			return tb
 		end,
-		__name__ = self.Name:sub(1,#self.Name-3), -- __name__ 
+		__name__ = if inScript:IsA("BaseScript") then "__main__" else inScript.Name , 
 		len = function(x) return #x end, -- len()
 		abs = math.abs, -- abs()
 		str = tostring, -- str()
 		int = tonumber, -- int()
 
 		sum = function(tbl) --sum()
 			local total = 0
@@ -522,15 +729,17 @@
 		chr = string.char, -- chr
 
 		callable = function(fun) -- callable()
 			if rawget(fun) ~= fun then warn("At the momement Roblox.py's function callable() does not fully support metatables.") end
 			return typeof(rawget(fun))	== "function"
 		end,
 		float = tonumber, -- float()
-		
+		super = function()
+			error("roblox-pyc does not has a Lua implementation of the function `super`. Use `self` instead")
+		end,
 		format = function(format, ...) -- format
 			local args = {...}
 			local num_args = select("#", ...)
 
 			local formatted_string = string.gsub(format, "{(%d+)}", function(index)
 				index = tonumber(index)
 				if index >= 1 and index <= num_args then
@@ -538,19 +747,19 @@
 				else
 					return "{" .. index .. "}"
 				end
 			end)
 
 			return formatted_string
 		end,
-		
+
 		hex = function (value) -- hex
 			return string.format("%x", value)
 		end,
-		
+
 		id = function (obj) -- id
 			return print(tostring({obj}):gsub("table: ", ""):split(" ")[1])
 		end,
 		map = function (func, ...) --map
 			local args = {...}
 			local result = {}
 			local num_args = select("#", ...)
@@ -575,21 +784,21 @@
 
 			return result
 		end,
 		bool = function(x) -- bool
 			if x == false or x == nil or x == 0 then
 				return false
 			end
-		
+
 			if typeof(x) == "table" then
 				if x._is_list or x._is_dict then
 					return next(x._data) ~= nil
 				end
 			end
-		
+
 			return true
 		end,
 		divmod = function(a, b) -- divmod
 			local res = { math.floor(a / b), math.fmod(a, b) }
 			return unpack(res)
 		end,
 		slice = slicefun,	
@@ -599,15 +808,15 @@
 					if v == item then
 						return true
 					end
 				end
 			elseif type(items) == "string" and type(item) == "string" then
 				return string.find(items, item, 1, true) ~= nil
 			end
-		
+
 			return false
 		end,
 		asynchronousfunction = function(func) -- asynchronousfunction
 			return function(...)
 				local all = {...}
 				coroutine.wrap(function()
 					func(unpack(all))
@@ -617,15 +826,15 @@
 		match = function(value, values) -- match
 			if values[value] then
 				return values[value]()
 			elseif values["default"] then
 				return values["default"]() 
 			end
 		end,
-		
+
 		anext = function (iterator) -- anext
 			local status, value = pcall(iterator)
 			if status then
 				return value
 			end
 		end,
 
@@ -681,23 +890,38 @@
 		end,
 		-- oct()
 		oct = function (num) --oct
 			return string.format("%o", num)
 		end,
 
 		-- open()
-		open = function (filename, mode) --open
-			if not io then error("io is not enabled") end
-			return io.open(filename, mode)
+		open = function (path, mode)
+			local obj = parse_path(path, inScript)
+			if obj:IsA("ModuleScript") then
+				local source = fromFileImport(obj)
+				if mode == "r" then
+					return source.Contents or error("File is not in correct roblox-pyc format, cannot be read.")
+				elseif mode == "w" then
+					return {
+						write = function(self, data)
+							obj:SetSource(data)
+						end,
+						close = function(self)
+							--obj:SaveSource()
+							return -- do nothing
+						end
+					}
+				else
+					error("Invalid mode, at the moment only r and w are supported: " .. mode)
+				end
+			else
+				error("Object is not a LuaSourceContainer: " .. path)
+			end
 		end,
 
-		-- ord()
-		ord = function (c) --ord
-			return string.byte(c)
-		end,
 
 		-- pow()
 		pow = function (base, exponent, modulo) --pow
 			if modulo ~= nil then
 				return math.pow(base, exponent) % modulo
 			else
 				return base ^ exponent
@@ -706,17 +930,15 @@
 
 		-- eval()
 		eval = function (expr, env)
 			return loadstring(expr)()
 		end,
 
 		-- exec()
-		exec = function (code, env)
-			return loadstring(expr)()
-		end,
+		exec = loadstring,
 
 		-- filter()
 		filter = function (predicate, iterable)
 			local result = {}
 			for _, value in ipairs(iterable) do
 				if predicate(value) then
 					table.insert(result, value)
@@ -734,171 +956,285 @@
 			end
 			return frozenSet
 		end,
 		-- aiter()
 		aiter = function (iterable) -- aiter
 			return pairs(iterable)
 		end,
-		
+
 		-- bin()
-		bin = function (number) -- bin
-			return string.format("%b", number)
+		bin = function(num: number)
+			local bits = {}
+			repeat
+				table.insert(bits, 1, num % 2)
+				num = math.floor(num / 2)
+			until num == 0
+			return "0b" .. table.concat(bits)
 		end,
 		-- complex() 
 		complex = function (real, imag) -- complex
 			return { real = real, imag = imag }
 		end,
-		
+
 		-- delattr()
 		deltaattr = function (object, attribute) -- delattr
 			object[attribute] = nil
 		end,	
 
 		-- enumerate()
 		enumerate = function (iterable) -- enumerate
 			local i = 0
 			return function()
-			i = i + 1
-			local value = iterable[i]
-			if value ~= nil then
-				return i, value
-			end
+				i = i + 1
+				local value = iterable[i]
+				if value ~= nil then
+					return i, value
+				end
 			end
 		end,
 
 		-- breakpoint()
 		breakpoint = function () -- breakpoint
-			-- This function can be left empty or you can add a debug hook to pause execution.
-			-- Here's an example using the debug library to pause execution:
-			debug.sethook(function()
-			print("Breakpoint hit!")
-			--io.read() -- Wait for user input to continue
-			end, "c")
+			debug.traceback("Breakpoint hit!")
+
 		end,
-		
+
 		-- bytearray()
 		bytearray = function (arg) -- bytearray
 			if type(arg) == "string" then
-			local bytes = {}
-			for i = 1, #arg do
-				table.insert(bytes, string.byte(arg, i))
-			end
-			return bytes
+				local bytes = {}
+				for i = 1, #arg do
+					table.insert(bytes, string.byte(arg, i))
+				end
+				return bytes
 			elseif type(arg) == "number" then
-			local bytes = {}
-			while arg > 0 do
-				table.insert(bytes, 1, arg % 256)
-				arg = math.floor(arg / 256)
-			end
-			return bytes
+				local bytes = {}
+				while arg > 0 do
+					table.insert(bytes, 1, arg % 256)
+					arg = math.floor(arg / 256)
+				end
+				return bytes
 			elseif type(arg) == "table" then
-			return arg -- Assuming it's already a bytearray table
+				return arg -- Assuming it's already a bytearray table
 			else
-			error("Invalid argument type for bytearray()")
+				error("Invalid argument type for bytearray()")
 			end
 		end,
-		
+
 		-- bytes()
 		bytes = function (arg) -- bytes
 			if type(arg) == "string" then
-			local bytes = {}
-			for i = 1, #arg do
-				table.insert(bytes, string.byte(arg, i))
-			end
-			return bytes
+				local bytes = {}
+				for i = 1, #arg do
+					table.insert(bytes, string.byte(arg, i))
+				end
+				return bytes
 			elseif type(arg) == "table" then
-			return arg -- Assuming it's already a bytes table
+				return arg -- Assuming it's already a bytes table
 			else
-			error("Invalid argument type for bytes()")
+				error("Invalid argument type for bytes()")
 			end
 		end,
-		
+
 		-- compile()
-		compile = function (source, filename, mode) -- compile
-			-- This is a placeholder implementation and might not cover all possible use cases.
-			-- You would need to provide your own implementation based on your specific requirements.
-			-- Here's an example of a simple compilation to execute Lua code directly:
-			local compiledFunction = loadstring(source, filename)
-			return compiledFunction
-		end,
+		compile = loadstring,
+
 
-		
 		-- help()
 		help = function (object) -- help
 			-- This is a placeholder implementation and might not cover all possible use cases.
 			-- You would need to provide your own implementation based on your specific requirements.
 			-- Here's an example of displaying a help message for an object:
 			print("Help for object:", object)
 			print("Type:", type(object))
-			-- Add more information or documentation here
+			print("Learn more in the official roblox documentation!")
 		end,
-		
+
 		-- memoryview()
 		memoryview = function (object) -- memoryview
 			-- This is a placeholder implementation and might not cover all possible use cases.
 			-- You would need to provide your own implementation based on your specific requirements.
 			-- Here's an example of creating a memory view object:
 			if type(object) == "table" then
-			local buffer = table.concat(object)
-			return { buffer = buffer, itemsize = 1 }
+				local buffer = table.concat(object)
+				return { buffer = buffer, itemsize = 1 }
 			else
-			error("Invalid argument type for memoryview()")
+				error("Invalid argument type for memoryview()")
 			end
 		end,
 		-- repr()
 		repr = function (object) -- repr
 			-- This is a placeholder implementation and might not cover all possible use cases.
 			-- You would need to provide your own implementation based on your specific requirements.
 			-- Here's an example of generating a representation of an object:
 			return tostring(object)
 		end,
-		
+
 		-- sorted()
 		sorted = function (iterable, cmp, key, reverse) -- sorted
 			-- This is a placeholder implementation and might not cover all possible use cases.
 			-- You would need to provide your own implementation based on your specific requirements.
 			-- Here's an example of sorting an iterable table:
 			local sortedTable = {}
 			for key, value in pairs(iterable) do
-			table.insert(sortedTable, { key = key, value = value })
+				table.insert(sortedTable, { key = key, value = value })
 			end
 			table.sort(sortedTable, function(a, b)
-			-- Compare logic based on cmp, key, reverse parameters
-			return a.key < b.key
+				-- Compare logic based on cmp, key, reverse parameters
+				return a.key < b.key
 			end)
 			local i = 0
 			return function()
-			i = i + 1
-			local entry = sortedTable[i]
-			if entry then
-				return entry.key, entry.value
-			end
+				i = i + 1
+				local entry = sortedTable[i]
+				if entry then
+					return entry.key, entry.value
+				end
 			end
 		end,
-		
+
 		-- vars()
 		vars = function (object) -- vars
 			-- This is a placeholder implementation and might not cover all possible use cases.
 			-- You would need to provide your own implementation based on your specific requirements.
 			-- Here's an example of getting the attributes of an object:
 			local attributes = {}
 			for key, value in pairs(object) do
-			attributes[key] = value
+				attributes[key] = value
 			end
 			return attributes
 		end,
-		
+
 		__import__ = require,
+
+		formatmod = function (left, right)
+			if type(left) == "string" then
+				return string.format(left, right)
+			elseif type(left) == "table" then
+				local result = {}
+				for i, v in ipairs(left) do
+					result[i] = string.format(v, right)
+				end
+				return result
+			elseif type(left) == "number" then
+				return math.fmod(left, right)
+			else
+				error("Invalid argument type for %")
+			end
+		end,
+
+		safeadd = function(left, right)
+			if type(left) ~= type(right) then
+				error("Cannot add values of different types")
+			end
+			local chosentype = type(left)
+			if chosentype == "string" then
+				return left .. right
+			elseif chosentype == "number" then
+				return left + right
+			elseif chosentype == "table" then
+				local result = {}
+				for i, v in ipairs(left) do
+					table.insert(result, v)
+				end
+				for i, v in ipairs(right) do
+					table.insert(result, v)
+				end
+				return result
+			elseif chosentype == "function" then
+				return function(...)
+					left(...)
+					right(...)
+				end
+			else
+				error("Invalid argument type for +")
+			end
+		end
 	}
-		
-	}
-	}
+	
+	for i, v in items do
+		items[i] = wrap(v)
+	end
+	for i, v in language do
+		items[i] = wrap(getfenv()[i])
+	end
+	return items
+end
+function fromFileImport(scriptin)
+	if scriptin == nil then error("Cannot import from nil.") end
+	if scriptin:IsA("ModuleScript") then
+		return require(scriptin)
+	else
+		return _G.pyc.data[scriptin] or error("Cannot import from script, it is not a module script and is not registered in _G")
+	end
+end
+local import = function(inscript) return function(index, sub) -- import
+	-- IMPORT METHODS:
+	-- Local libraries table - Added
+	-- _G.pyc.data[script], will return all of its return values, for non modulescripts  - Added in fromFileImport
+	-- require(script), for modulescripts  - Added in fromFileImport
+	-- (require/_G.pyc.data).Contents, for open, dont worry about this one  - Added in open
+	-- Index is .<filename>, look for the script/module script from inscript's parent - Added
+	-- Index is /<filename>, look inside of inscript  - Added
+	-- Index is . look for sub inside of inscripts parent - Added
+	-- Index is / look for sub inside of inscript - Added
+	-- Search in dependencies folder, dependencies folder should have a script called "content" use fromFileImport and that will have all of the dependencies - Added
+
+
+	if index == "." then
+		if sub then
+			return fromFileImport(inscript.Parent:FindFirstChild(sub))
+		end
+	elseif index == "/" then
+		if sub then
+			return fromFileImport(inscript:FindFirstChild(sub))
+		end
+	elseif index:sub(1,1) == "." then
+		if sub then
+			return fromFileImport(inscript.Parent:FindFirstChild(index:sub(2)))[sub]
+		end
+	elseif index:sub(1,1) == "/" then
+		if sub then
+			return fromFileImport(inscript:FindFirstChild(index:sub(2)))[sub]
+		end
+	elseif libraries[index] then -- Local libraries table
+		if sub then
+			return libraries[index][sub]
+		end
+		return libraries[index]
+	else
+		local dependencies = fromFileImport(dependenciesfolder:FindFirstChild("content")).Contents -- works just like open
+		if dependencies[index] then
+			if sub then
+				return dependencies[index][sub]
+			end
+			return dependencies[index]
+		end
+	end
+end end
+local include = function()
+	error("C and C++ are not complete yet")
 end
 
+local module = function(scriptname)
+	return { 
+		py = {
+			import(scriptname),
+			pythonBuiltIn(scriptname)
+		},
+		lunar = {
+			import(scriptname),
+			{-- lunar built in: NOTHING
+			},
+		},
+		c = {
+			include,
+			{-- c and c++ built in
+			}
+		}
+	}
+end
 
 
-return module
-"""
-
-allfunctions = "stringmeta, list, dict, staticmethod, classsmethod, class, range, __name__, len, abs, str, int, sum, max, min, reversed, split, round, all, any, ord, char, callable, zip, float, format, hex, id, map, bool, divmod, slice, operator_in, asynchronousfunction, match, anext, ascii, dir, getattr, globals, hasattr, input, isinstance, issubclass, iter, locals, oct, open, ord, pow, eval, exec, filter, frozenset, aiter, bin, complex, delattr, enumerate, breakpoint, bytearray, bytes, compile, help, memoryview, repr, sorted, vars, __import__"
 
-allfunctions = allfunctions.split(", ")
+_G.pyc = module
+_G.pyc.libs = {}
```

### Comparing `roblox-pyc-1.6.6.5a0/src/nodevisitor.py` & `roblox-pyc-2.25.111/robloxpyc/nodevisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 """Node visitor"""
-import ast
-
-from .binopdesc import BinaryOperationDesc
-from .boolopdesc import BooleanOperationDesc
-from .cmpopdesc import CompareOperationDesc
-from .nameconstdesc import NameConstantDesc
-from .unaryopdesc import UnaryOperationDesc
-
-from .context import Context
-from .loopcounter import LoopCounter
-from .tokenendmode import TokenEndMode
+import ast, sys
 
+import os 
+if not (os.path.dirname(os.path.abspath(__file__)).startswith(sys.path[-1])):
+    from binopdesc import BinaryOperationDesc
+    from boolopdesc import BooleanOperationDesc
+    from cmpopdesc import CompareOperationDesc
+    from nameconstdesc import NameConstantDesc
+    from unaryopdesc import UnaryOperationDesc
+
+    from context import Context
+    from loopcounter import LoopCounter
+    from tokenendmode import TokenEndMode
+    from colortext import *
+else:
+    from .binopdesc import BinaryOperationDesc
+    from .boolopdesc import BooleanOperationDesc
+    from .cmpopdesc import CompareOperationDesc
+    from .nameconstdesc import NameConstantDesc
+    from .unaryopdesc import UnaryOperationDesc
+
+    from .context import Context
+    from .loopcounter import LoopCounter
+    from .tokenendmode import TokenEndMode
+    from .colortext import *
 
 class NodeVisitor(ast.NodeVisitor):
     LUACODE = "[[lua]]"
 
     """Node visitor"""
     def __init__(self, context=None, config=None):
         self.context = context if context is not None else Context()
@@ -135,15 +148,15 @@
         if last_ctx["class_name"]:
             target = ".".join([last_ctx["class_name"], target])
 
         if "." not in target and not last_ctx["locals"].exists(target):
             local_keyword = "local "
             last_ctx["locals"].add_symbol(target)
 
-        self.emit("{local}{target}: {type} = {value}".format(local=local_keyword,
+        self.emit("{local}{target} = {value}".format(local=local_keyword,
                                                      target=target,
                                                      value=value,
                                                      type=self.visit_all(node.annotation, inline=True)))
         # example input:
         # a: int = 1
         # example output:
         # local a = 1
@@ -173,21 +186,25 @@
             "attr": node.attr,
         }
         self.emit(line.format(**values))
 
     def visit_BinOp(self, node):
         """Visit binary operation"""
         operation = BinaryOperationDesc.OPERATION[node.op.__class__]
-        line = "({})".format(operation["format"])
+        format = ""
+        if "format" in operation: 
+            format = operation["format"] 
+        else:
+            format = operation["function"](node.left, node.right)
+        line = "({})".format(format)
         values = {
             "left": self.visit_all(node.left, True),
             "right": self.visit_all(node.right, True),
             "operation": operation["value"],
         }
-
         self.emit(line.format(**values))
 
     def visit_BoolOp(self, node):
         """Visit boolean operation"""
         operation = BooleanOperationDesc.OPERATION[node.op.__class__]
         line = "({})".format(operation["format"])
         values = {
@@ -226,24 +243,17 @@
         self.emit("end)()")
 
     def visit_Await(self, node):
         """Visit await"""
         self.emit("coroutine.yield({})".format(self.visit_all(node.value, True)))
 
     def visit_Slice(self, node):
-        if node.step is None:
-            line = '"SLICE!({start}, {end})"'
-        else:
-            line = '"SLICE!({start}, {end}, {step})"'
-        values = {
-            "start": self.visit_all(node.lower, True),
-            "end": self.visit_all(node.upper, True),
-            "step": self.visit_all(node.step, True),
-        }
-        self.emit(line.format(**values))
+        """Visit slice"""
+        print(yellow("warning", ["bold"])+" syntax based slicing is not supported yet. Use slice(<sequence>, <start>, <end>, <step>) instead. This node will not be translated.")
+        
 
     def visit_JoinedStr(self, node):
         """Visit joined string"""
         values = [self.visit_all(value, True) for value in node.values]
         self.emit('.'.join(values))
     
     def visit_Bytes(self, node):
@@ -265,26 +275,29 @@
 
     def visit_ImportFrom(self, node):
         """Visit import from"""
         module = node.module
         if module is None:
             module = ""
         else:
-            module = module + "."
+            module = module
 
         for name in node.names:
             if name.asname is None:
-                self.emit("local {name} = require('{module}{name}')".format(
+                self.emit("local {name} = import(\"{module}\", \"{name}\")".format(
                     name=name.name,
                     module=module,
                 ))
             else:
-                self.emit("local {name} = require('{module}{name}')".format(
+                if name.name == "*":
+                    print("roblox-pyc: Importing all from a module is not supported yet. Issues will occur.")
+                self.emit("local {name} = import(\"{module}\", \"{realname}\")".format(
                     name=name.asname,
                     module=module,
+                    realname=name.name,
                 ))
 
     def visit_Assert(self, node):
         """Visit assert"""
         self.emit("assert({})".format(self.visit_all(node.test, True)))
 
     def visit_Nonlocal(self, node):
@@ -459,15 +472,15 @@
                 line += " and "
 
         self.emit("({})".format(line))
 
     def visit_Continue(self, node):
         """Visit continue"""
         last_ctx = self.context.last()
-        line = "{}".format(last_ctx["loop_label_name"])
+        line = "continue"
         self.emit(line)
 
     def visit_Delete(self, node):
         """Visit delete"""
         targets = [self.visit_all(target, inline=True) for target in node.targets]
         nils = ["nil" for _ in targets]
         line = "{targets} = {nils}".format(targets=", ".join(targets),
@@ -665,15 +678,15 @@
             "false_cond": self.visit_all(node.orelse, inline=True),
         }
 
         self.emit(line.format(**values))
 
     def visit_Import(self, node):
         """Visit import"""
-        line = 'local {asname} = require "{name}"'
+        line = 'local {asname} = import("{name}")'
         values = {"asname": "", "name": ""}
 
         if node.names[0].asname is None:
             values["name"] = node.names[0].name
             values["asname"] = values["name"]
             values["asname"] = values["asname"].split(".")[-1]
         else:
@@ -776,23 +789,26 @@
         value = node.s
         if value.startswith(NodeVisitor.LUACODE):
             value = value[len(NodeVisitor.LUACODE):]
             self.emit(value)
         elif self.context.last()["docstring"]:
             self.emit('--[[ {} ]]'.format(node.s))
         else:
-            self.emit('stringmeta "{}"'.format(node.s))
+            # Add to context
+            self.emit('"{}"'.format(node.s))
 
     def visit_Subscript(self, node):
         """Visit subscript"""
         line = "{name}[{index}]"
         values = {
             "name": self.visit_all(node.value, inline=True),
             "index": self.visit_all(node.slice, inline=True),
         }
+        # append to context
+        ##self.context.last()["subscript"] = node
 
         self.emit(line.format(**values))
 
     def visit_Tuple(self, node):
         """Visit tuple"""
         elements = [self.visit_all(item, inline=True) for item in node.elts]
         self.emit(", ".join(elements))
@@ -823,14 +839,50 @@
         self.visit_all(node.body)
         self.context.pop()
 
         #self.output[-1].append("::{}::".format(continue_label))
 
         self.emit("end")
 
+    def visit_Yield(self, node):
+        """Visit yield"""
+        self.emit("coroutine.yield({})".format(self.visit_all(node.value, True)))
+    def visit_GeneratorExp(self, node):
+        """Visit generator expression"""
+        self.emit("(function()")
+        self.emit("local result = list {}")
+
+        ends_count = 0
+
+        for comp in node.generators:
+            line = "for {target} in {iterator} do"
+            values = {
+                "target": self.visit_all(comp.target, inline=True),
+                "iterator": self.visit_all(comp.iter, inline=True),
+            }
+            line = line.format(**values)
+            self.emit(line)
+            ends_count += 1
+
+            for if_ in comp.ifs:
+                line = "if {} then".format(self.visit_all(if_, inline=True))
+                self.emit(line)
+                ends_count += 1
+
+        line = "result.append({})"
+        line = line.format(self.visit_all(node.elt, inline=True))
+        self.emit(line)
+
+        self.emit(" ".join(["end"] * ends_count))
+
+        self.emit("return result")
+        self.emit("end)()")
+    def visit_YieldFrom(self, node):
+        """Visit yield from"""
+        self.emit("coroutine.yield({})".format(self.visit_all(node.value, True)))
     def visit_With(self, node):
         """Visit with"""
         self.emit("do")
 
         self.visit_all(node.body)
 
         body = self.output[-1]
@@ -844,20 +896,49 @@
             line += self.visit_all(i.context_expr, inline=True)
             lines.append(line)
 
         for line in lines:
             body.insert(0, line)
 
         self.emit("end")
+    def visit_SetComp(self, node):
+        """Visit set comprehension"""
+        self.emit("(function()")
+        self.emit("local result = set {}")
+
+        ends_count = 0
+
+        for comp in node.generators:
+            line = "for {target} in {iterator} do"
+            values = {
+                "target": self.visit_all(comp.target, inline=True),
+                "iterator": self.visit_all(comp.iter, inline=True),
+            }
+            line = line.format(**values)
+            self.emit(line)
+            ends_count += 1
+
+            for if_ in comp.ifs:
+                line = "if {} then".format(self.visit_all(if_, inline=True))
+                self.emit(line)
+                ends_count += 1
+
+        line = "result.add({})"
+        line = line.format(self.visit_all(node.elt, inline=True))
+        self.emit(line)
 
+        self.emit(" ".join(["end"] * ends_count))
+
+        self.emit("return result")
+        self.emit("end)()")
     def generic_visit(self, node):
         """Unknown nodes handler"""
         if node is None:
             return
-        raise RuntimeError("Unknown node: {}".format(node))
+        raise RuntimeError("{} is unsupported".format(node))
 
     def visit_all(self, nodes, inline=False):
         """Visit all nodes in the given list"""
 
         if not inline:
             last_ctx = self.context.last()
             last_ctx["locals"].push()
```

### Comparing `roblox-pyc-1.6.6.5a0/src/pytranslator.py` & `roblox-pyc-2.25.111/robloxpyc/pytranslator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Python to lua translator class"""
 import ast
 import os
+import sys
+import os 
+if not (os.path.dirname(os.path.abspath(__file__)).startswith(sys.path[-1])):
+    from config import Config
+    from nodevisitor import NodeVisitor
+    from header import header, pyfooter
+    from luainit import initcode, allfunctions, generatewithlibraries, robloxfunctions
+else:
+    from .config import Config
+    from .nodevisitor import NodeVisitor
 
-from .config import Config
-from .nodevisitor import NodeVisitor
-
-from .header import header
-from .luainit import initcode, allfunctions
+    from .header import header, pyfooter
+    from .luainit import initcode, allfunctions, generatewithlibraries, robloxfunctions
 
 class Translator:
     """Python to lua main class translator"""
     def __init__(self, config=None, show_ast=False):
         self.config = config if config is not None else Config()
         self.show_ast = show_ast
 
@@ -18,34 +25,34 @@
 
     def translate(self, pycode):
         """Translate python code to lua code"""
         py_ast_tree = ast.parse(pycode)
 
         visitor = NodeVisitor(config=self.config)
 
-        if self.show_ast:
+        if self.show_ast: # 
             print(ast.dump(py_ast_tree))
 
         visitor.visit(py_ast_tree)
 
         self.output = visitor.output
         # check every single line for function calls
         functions = []
         for i in range(len(self.to_code().split("\n"))):
             # check if a function is being called, like print()
             
-            for function in allfunctions:
+            for function in (allfunctions+robloxfunctions):
                 if function in self.to_code().split("\n")[i] and function not in functions:
                     functions.append(function)
                     
                     
         # create header for function calls
         newheader = header(functions)
     
-        return newheader+self.to_code()
+        return newheader+self.to_code()+pyfooter
 
     def to_code(self, code=None, indent=0):
         """Create a lua code from the compiler output"""
         code = code if code is not None else self.output
 
         def add_indentation(line):
             """Add indentation to the given line"""
@@ -63,10 +70,9 @@
             elif isinstance(line, list):
                 sub_code = self.to_code(line, indent + 1)
                 lines.append(sub_code)
 
         return "\n".join(lines)
 
     @staticmethod
-    def get_luainit(filename="luainit.lua"):
-        
-        return initcode
+    def get_luainit(items):
+        return generatewithlibraries(items)
```

### Comparing `roblox-pyc-1.6.6.5a0/src/symbolsstack.py` & `roblox-pyc-2.25.111/robloxpyc/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-1.6.6.5a0/src/unaryopdesc.py` & `roblox-pyc-2.25.111/robloxpyc/unaryopdesc.py`

 * *Files identical despite different names*

