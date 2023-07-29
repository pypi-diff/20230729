# Comparing `tmp/uptrain-0.3.4.tar.gz` & `tmp/uptrain-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.3.4.tar", last modified: Fri Jul  7 09:32:53 2023, max compression
+gzip compressed data, was "uptrain-0.3.6.tar", last modified: Sat Jul 29 04:21:40 2023, max compression
```

## Comparing `uptrain-0.3.4.tar` & `uptrain-0.3.6.tar`

### file list

```diff
@@ -1,207 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.894305 uptrain-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 09:32:44.000000 uptrain-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 09:32:53.894305 uptrain-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-07 09:32:44.000000 uptrain-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 09:32:44.000000 uptrain-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:32:53.894305 uptrain-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-07-07 09:32:44.000000 uptrain-0.3.4/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/st_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/st_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/code/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/drift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/embs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/io/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/language/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/model_grade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.866305 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/completion_fns/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/elsuite/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/openai_evals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/sql_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/sqlglot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/v0/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/v0/core/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/popularity_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/distances/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/abstract_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/cosine_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/distance_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/hamming_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/l2_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/norm_ratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/annotation_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/dataset_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/model_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/io/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/io/runtime_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/log_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/log_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/new_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/st_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.882305 uptrain-0.3.4/uptrain/v0/core/classes/managers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/managers/check_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.882305 uptrain-0.3.4/uptrain/v0/core/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/abstract_measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/input_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/output_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/edge_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/model_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/output_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/signals/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/signals/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/abstract_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/norm_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/old_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/abstract_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/encoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/model_signal_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/ee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/ee/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.890305 uptrain-0.3.4/uptrain/v0/ee/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/classes/measurables/llm_measurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.890305 uptrain-0.3.4/uptrain/v0/ee/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/ops_agg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.890305 uptrain-0.3.4/uptrain/v0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_a-b_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_concept_drift_custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_data_integrity_zscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_edge_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.894305 uptrain-0.3.4/uptrain/v0/tests/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/get_data_from_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/pushup_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_adwin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_ddm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_recommender_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_visuals_dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_visuals_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_visuals_shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.894305 uptrain-0.3.4/uptrain/validation_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/validation_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/validation_wrapper/validation_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.696524 uptrain-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 04:21:27.000000 uptrain-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-07-29 04:21:40.696524 uptrain-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-07-29 04:21:27.000000 uptrain-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 04:21:27.000000 uptrain-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 04:21:40.696524 uptrain-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.676524 uptrain-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-29 04:21:27.000000 uptrain-0.3.6/tests/test_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-07-29 04:21:27.000000 uptrain-0.3.6/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.676524 uptrain-0.3.6/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.680524 uptrain-0.3.6/uptrain/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/dashboard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/dashboard/st_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/dashboard/st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/dashboard/st_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.680524 uptrain-0.3.6/uptrain/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/framework/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/framework/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/framework/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.680524 uptrain-0.3.6/uptrain/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.680524 uptrain-0.3.6/uptrain/operators/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/code/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/embs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.680524 uptrain-0.3.6/uptrain/operators/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/io/bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/io/duck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/io/excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/operators/language/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/model_grade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.672524 uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/completion_fns/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/elsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/openai_evals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/language/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/operators/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/utilities/sql_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/utilities/sqlglot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/classes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/algorithms/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/algorithms/popularity_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/classes/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/abstract_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/cosine_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/distance_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/hamming_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/l2_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/distances/norm_ratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/classes/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/finetuning/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/classes/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/helpers/annotation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/helpers/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/helpers/dataset_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/helpers/model_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.684524 uptrain-0.3.6/uptrain/v0/core/classes/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/io/runtime_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.688524 uptrain-0.3.6/uptrain/v0/core/classes/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/log_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/log_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/new_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/new_st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/new_st_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/logging/st_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.688524 uptrain-0.3.6/uptrain/v0/core/classes/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/managers/check_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.688524 uptrain-0.3.6/uptrain/v0/core/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/abstract_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/feature_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/input_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/measurable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/output_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.688524 uptrain-0.3.6/uptrain/v0/core/classes/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/abstract_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/abstract_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/edge_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/feature_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/model_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/monitors/output_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/core/classes/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/signals/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/core/classes/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/abstract_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/norm_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/statistics/old_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/core/classes/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/visuals/abstract_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/visuals/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/visuals/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/classes/visuals/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/core/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/encoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/lib/datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/lib/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/core/lib/model_signal_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/ee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/ee/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/ee/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/classes/measurables/llm_measurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.692524 uptrain-0.3.6/uptrain/v0/ee/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/ee/lib/ops_agg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.696524 uptrain-0.3.6/uptrain/v0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_a-b_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_concept_drift_custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_data_integrity_zscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_edge_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.696524 uptrain-0.3.6/uptrain/v0/tests/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/get_data_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/model_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/model_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_helpers/pushup_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_monitors_concept_drift_adwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_monitors_concept_drift_ddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_recommender_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_visuals_dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_visuals_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/v0/tests/test_visuals_shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.696524 uptrain-0.3.6/uptrain/validation_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/validation_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-29 04:21:27.000000 uptrain-0.3.6/uptrain/validation_wrapper/validation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 04:21:40.676524 uptrain-0.3.6/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-07-29 04:21:40.000000 uptrain-0.3.6/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-29 04:21:40.000000 uptrain-0.3.6/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 04:21:40.000000 uptrain-0.3.6/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 04:21:40.000000 uptrain-0.3.6/uptrain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-29 04:21:40.000000 uptrain-0.3.6/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-29 04:21:40.000000 uptrain-0.3.6/uptrain.egg-info/top_level.txt
```

### Comparing `uptrain-0.3.4/LICENSE` & `uptrain-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/PKG-INFO` & `uptrain-0.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.3.4
+Version: 0.3.6
 Summary: UpTrain - ML Observability and Retraining Framework
 Maintainer-email: UpTrain AI Team <uptrain.ai@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain
 Keywords: uptrain,ai,retraining,ML,observability
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
 <h2>
   <p align="center">
-    <p align="center">An open-source framework to evaluate, test and monitor LLM applications</p>
+    <p align="center">An open-source framework to evaluate and monitor LLM applications</p>
   </p>
 </h2>
 
 <p align="center">
 <a href="https://docs.uptrain.ai/docs/" rel="nofollow"><strong>Docs</strong></a>
 <!-- -
 <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a> -->
@@ -74,32 +74,30 @@
 <kbd>[<img title="French" alt="French language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/fr.svg" width="22">](/i18n/README.fr.md)</kbd>
 <kbd>[<img title="Japanese" alt="Japanese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/jp.svg" width="22">](/i18n/README.ja.md)</kbd>
 <kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd> -->
 
 
 **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM applications are performing reliably by allowing users to check aspects such as correctness, structural integrity, bias, hallucination, etc. UpTrain can be used to:
 
-1) Validate model's response and safeguard your users against hallucinations, bias, incorrect output formats, etc.
-2) Experiment across multiple model providers, prompt templates, and quantify model's performance.
-3) Monitor your model's performance in production and protect yourself against unwanted drifts
+## Experimentation
 
+UpTrain framework can be used to experiment across multiple prompts, model providers, chain configurations, etc. and get quantitative scores to compare them. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
 
-# Key Features 💡
+<img width="600" src="https://github.com/uptrain-ai/uptrain/assets/108270398/f6d1802a-079a-4bf0-8eb8-de879c2aa465" alt="uptrain experimentation">
 
 
-- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
-- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
-- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
-- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
-- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
-- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
-- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
-- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
-- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
-- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
+## Validation
+
+You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
+
+<img width="600" src="https://github.com/uptrain-ai/uptrain/assets/108270398/a34af650-a8ea-466c-9b5d-83e7f31eb8e2" alt="uptrain validation">
+
+## Monitoring
+
+You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
 
 # Get started 🙌
 
 <!-- You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). -->
 
 To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
@@ -109,69 +107,70 @@
 ```
 
 Note: Uptrain uses commonly used python libraries like openai-evals and sentence-transformers. To make sure, all the functionalities work, use the `uptrain-add` command to install the full version of the package.
 ```bash
 uptrain-add --feature full
 ```
 
-### How to define checks:
-Say we want to check whether our model's responses contain any grammatical mistakes or not.
+### How to use UpTrain in 4 simple steps:
+Say we want to plot a line chart showing whether our model's responses contain any grammatical mistakes or not.
 
 ```python
-# Define your checkset - list of simple checks, dataset file, 
-# and api_keys
+# Step 1: Choose and create the appropriate operator from UpTrain
+grammar_score = GrammarScore(
+  col_in_text = "model_response",       # input column name (from dataset)
+  col_out = "grammar_score"             # desired output column name
+)
+
+# Step 2: Create a check with the operators and the required plots as arguments 
+grammar_check = Check(
+  operators = [grammar_score],
+  plots = LineChart(y = "grammar_score")
+)
 
+# Step 3: Create a CheckSet with the checks and data source as arguments
 checkset = CheckSet(
-    checks = Check(
-        name = "grammar_score",
-        operators = [
-            GrammarScore(
-                col_in_text = "model_response",
-                col_out = "grammar_score"
-            ),
-        ],
-        plots = PlotlyChart.Table(title="Grammar scores"),
-    ),
+    checks = [grammar_check]
     source = JsonReader(fpath = '...')
 )
-settings = Settings(openai_api_key = '...')
 
-checkset.setup(settings)
-checkset.run()
+# Step 4: Set up and run the CheckSet
+checkset.setup(Settings(openai_api_key = '...'))
+checkset.run(dataset)
 ```
 
 <!-- For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial). -->
 
 <h4> </h4>
 
+# Key Features 💡
+
+
+- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
+- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
+- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
+- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
+- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
+- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
+- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
+- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
+- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
+- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
+
+
 # Integrations
 
 | Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | 
 | ------------- | ------------- | ------------- | ------------- | 
 | OpenAI Evals ✅ | GPT-3.5-turbo ✅ | Langchain 🔜 | HuggingFace 🔜 |
 | EleutherAI LM Eval 🔜 | GPT-4 ✅  | Llama Index 🔜 |  Replicate 🔜 |
 | BIG-Bench 🔜 | Claude 🔜 | AutoGPT 🔜 |
 | | Cohere 🔜 | 
 
 
-# UpTrain in Action
-
-## Experimentation
-
-You can use the UpTrain framework to run and compare LLM responses for different prompts, models, LLM chains, etc. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
-
-## Validation
-
-You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
-
-## Monitoring
-
-You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
-
-
 # Why UpTrain 🤔?
 
 Large language models are trained over billions of data points and perform really well over a wide variety of tasks. But one thing these models are not good at is being deterministic. Even with the most well-crafted prompts, the model can misbehave for certain inputs, be it hallucinations, wrong output structure, toxic or biased response, irrelevant response, and error modes can be immense. 
 
 To ensure your LLM applications work reliably and correctly, UpTrain makes it easy for developers to evaluate the responses of their applications on multiple criteria. UpTrain's evaluation framework can be used to:
 
 1) Validate (and correct) the response of the model before showing it to the user
```

#### html2text {}

```diff
@@ -1,100 +1,100 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.3.4 Summary: UpTrain - ML
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.6 Summary: UpTrain - ML
 Observability and Retraining Framework Maintainer-email: UpTrain AI Team
 ai@gmail.com> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
 uptrain,ai,retraining,ML,observability Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown Provides-Extra: test License-File:
 LICENSE
                                *** [uptrain] ***
-***** An open-source framework to evaluate, test and monitor LLM applications
-*****
+***** An open-source framework to evaluate and monitor LLM applications *****
             Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
                   Welcome] [Docs] [Community] [Website]  ***
   **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
 applications are performing reliably by allowing users to check aspects such as
 correctness, structural integrity, bias, hallucination, etc. UpTrain can be
-used to: 1) Validate model's response and safeguard your users against
-hallucinations, bias, incorrect output formats, etc. 2) Experiment across
-multiple model providers, prompt templates, and quantify model's performance.
-3) Monitor your model's performance in production and protect yourself against
-unwanted drifts # Key Features ð¡ - **[ChatGPT Grading](https://uptrain-
-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to
-grade your model outputs. - **[Custom Grading Checks](https://uptrain-
-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom
-grading prompts. - **[Embeddings Similarity Check](https://uptrain-
-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity
-between prompt and response embeddings - **[Output Validation](https://
-github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** -
-Safeguard your users against inappropriate responses - **[Prompt A/B Testing]
+used to: ## Experimentation UpTrain framework can be used to experiment across
+multiple prompts, model providers, chain configurations, etc. and get
+quantitative scores to compare them. Check out the [experimentation tutorial]
 (https://github.com/uptrain-ai/uptrain/blob/main/examples/
-prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and
-compare them quantatively. - **[UMAP Visualization and Clustering](https://
-uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding
-space using tools like UMAP and t-SNE. - **[Hallucination Checks]()** - Use
-metrics like custom grading, text similarity, and embedding similarity to check
-for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
-outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
-Built-in pivoting functionalities for data dice and slice to pinpoint low-
-performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
-performance in realtime. # Get started ð  To run it on your machine,
-checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
-quickstart): ### Install the package through pip: ```bash pip install uptrain
-``` Note: Uptrain uses commonly used python libraries like openai-evals and
-sentence-transformers. To make sure, all the functionalities work, use the
-`uptrain-add` command to install the full version of the package. ```bash
-uptrain-add --feature full ``` ### How to define checks: Say we want to check
-whether our model's responses contain any grammatical mistakes or not.
-```python # Define your checkset - list of simple checks, dataset file, # and
-api_keys checkset = CheckSet( checks = Check( name = "grammar_score", operators
-= [ GrammarScore( col_in_text = "model_response", col_out = "grammar_score" ),
-], plots = PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader
-(fpath = '...') ) settings = Settings(openai_api_key = '...') checkset.setup
-(settings) checkset.run() ```
-# Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
-frameworks | | ------------- | ------------- | ------------- | ------------- |
-| OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
-EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
-BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
-Action ## Experimentation You can use the UpTrain framework to run and compare
-LLM responses for different prompts, models, LLM chains, etc. Check out the
-[experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/
-examples/prompt_experiments_tutorial.ipynb) to learn more. ## Validation You
-can use the UpTrain Validation Manager to define checks, retry logic and
-validate your LLM responses before showing it to your users. Check out the
-[tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-validation_tutorial.ipynb). ## Monitoring You can use the UpTrain framework to
-continuously monitor your model's performance and get real-time insights on how
-well it is doing on a variety of evaluation metrics. Check out the monitoring
-tutorial to learn more. # Why UpTrain ð¤? Large language models are trained
-over billions of data points and perform really well over a wide variety of
-tasks. But one thing these models are not good at is being deterministic. Even
-with the most well-crafted prompts, the model can misbehave for certain inputs,
-be it hallucinations, wrong output structure, toxic or biased response,
-irrelevant response, and error modes can be immense. To ensure your LLM
-applications work reliably and correctly, UpTrain makes it easy for developers
-to evaluate the responses of their applications on multiple criteria. UpTrain's
-evaluation framework can be used to: 1) Validate (and correct) the response of
-the model before showing it to the user 2) Get quantitative measures to
-experiment across multiple prompts, model providers, etc. 3) Do unit testing to
-ensure no buggy prompt or code gets pushed into your production 4) Monitor your
-LLM applications in real time and understand when they are going wrong in order
-to fix them before users complain. We are constantly working to make UpTrain
-better. Want a new feature or need any integrations? Feel free to [create an
-issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://
-github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the
-repository. # License ð» This repo is published under Apache 2.0 license. We
-are also working towards adding a hosted offering to make setting off eval runs
-easier - please fill **[this form](https://docs.google.com/forms/d/e/
+prompt_experiments_tutorial.ipynb) to learn more. [uptrain experimentation] ##
+Validation You can use the UpTrain Validation Manager to define checks, retry
+logic and validate your LLM responses before showing it to your users. Check
+out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/
+examples/validation_tutorial.ipynb). [uptrain validation] ## Monitoring You can
+use the UpTrain framework to continuously monitor your model's performance and
+get real-time insights on how well it is doing on a variety of evaluation
+metrics. Check out the monitoring tutorial to learn more. # Get started ð
+To run it on your machine, checkout the [Quickstart tutorial](https://
+docs.uptrain.ai/getting-started/quickstart): ### Install the package through
+pip: ```bash pip install uptrain ``` Note: Uptrain uses commonly used python
+libraries like openai-evals and sentence-transformers. To make sure, all the
+functionalities work, use the `uptrain-add` command to install the full version
+of the package. ```bash uptrain-add --feature full ``` ### How to use UpTrain
+in 4 simple steps: Say we want to plot a line chart showing whether our model's
+responses contain any grammatical mistakes or not. ```python # Step 1: Choose
+and create the appropriate operator from UpTrain grammar_score = GrammarScore
+( col_in_text = "model_response", # input column name (from dataset) col_out =
+"grammar_score" # desired output column name ) # Step 2: Create a check with
+the operators and the required plots as arguments grammar_check = Check
+( operators = [grammar_score], plots = LineChart(y = "grammar_score") ) # Step
+3: Create a CheckSet with the checks and data source as arguments checkset =
+CheckSet( checks = [grammar_check] source = JsonReader(fpath = '...') ) # Step
+4: Set up and run the CheckSet checkset.setup(Settings(openai_api_key = '...'))
+checkset.run(dataset) ```
+# Key Features ð¡ - **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/
+operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model
+outputs. - **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/
+operators/language/ModelGradeScore/)** - Write your custom grading prompts. -
+**[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/
+CosineSimilarity/)** - Compute cosine similarity between prompt and response
+embeddings - **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/
+main/examples/validation_tutorial.ipynb)** - Safeguard your users against
+inappropriate responses - **[Prompt A/B Testing](https://github.com/uptrain-ai/
+uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment
+across multiple prompts and compare them quantatively. - **[UMAP Visualization
+and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** -
+Visualize your embedding space using tools like UMAP and t-SNE. - **
+[Hallucination Checks]()** - Use metrics like custom grading, text similarity,
+and embedding similarity to check for hallucinations. - **[Toxic Keywords
+Checks]()** - Make sure your model outputs are not biased or contain toxic
+keywords. - **[Feature Slicing]()** - Built-in pivoting functionalities for
+data dice and slice to pinpoint low-performing cohorts. - **[Realtime
+Dashboards]()** - Monitor your model's performance in realtime. # Integrations
+| Eval Frameworks | LLM Providers | LLM Packages | Serving frameworks | | -----
+-------- | ------------- | ------------- | ------------- | | OpenAI Evals â |
+GPT-3.5-turbo â | Langchain ð | HuggingFace ð | | EleutherAI LM Eval
+ð | GPT-4 â | Llama Index ð | Replicate ð | | BIG-Bench ð |
+Claude ð | AutoGPT ð | | | Cohere ð | # Why UpTrain ð¤? Large
+language models are trained over billions of data points and perform really
+well over a wide variety of tasks. But one thing these models are not good at
+is being deterministic. Even with the most well-crafted prompts, the model can
+misbehave for certain inputs, be it hallucinations, wrong output structure,
+toxic or biased response, irrelevant response, and error modes can be immense.
+To ensure your LLM applications work reliably and correctly, UpTrain makes it
+easy for developers to evaluate the responses of their applications on multiple
+criteria. UpTrain's evaluation framework can be used to: 1) Validate (and
+correct) the response of the model before showing it to the user 2) Get
+quantitative measures to experiment across multiple prompts, model providers,
+etc. 3) Do unit testing to ensure no buggy prompt or code gets pushed into your
+production 4) Monitor your LLM applications in real time and understand when
+they are going wrong in order to fix them before users complain. We are
+constantly working to make UpTrain better. Want a new feature or need any
+integrations? Feel free to [create an issue](https://github.com/uptrain-ai/
+uptrain/issues) or [contribute](https://github.com/uptrain-ai/uptrain/blob/
+main/CONTRIBUTING.md) directly to the repository. # License ð» This repo is
+published under Apache 2.0 license. We are also working towards adding a hosted
+offering to make setting off eval runs easier - please fill **[this form]
+(https://docs.google.com/forms/d/e/
 1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/
 viewform?usp=sf_link)** to get a waitlist slot. # Stay Updated âï¸ We are
 continuously adding tons of features and use cases. Please support us by giving
 the project a star â­! # Provide feedback (Harsher the better ð) We are
 building UpTrain in public. Help us improve by giving your feedback **[here]
 (https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-
 jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**. # Contributors ð¥ï¸ We
```

### Comparing `uptrain-0.3.4/README.md` & `uptrain-0.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
 <h2>
   <p align="center">
-    <p align="center">An open-source framework to evaluate, test and monitor LLM applications</p>
+    <p align="center">An open-source framework to evaluate and monitor LLM applications</p>
   </p>
 </h2>
 
 <p align="center">
 <a href="https://docs.uptrain.ai/docs/" rel="nofollow"><strong>Docs</strong></a>
 <!-- -
 <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a> -->
@@ -53,32 +53,30 @@
 <kbd>[<img title="French" alt="French language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/fr.svg" width="22">](/i18n/README.fr.md)</kbd>
 <kbd>[<img title="Japanese" alt="Japanese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/jp.svg" width="22">](/i18n/README.ja.md)</kbd>
 <kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd> -->
 
 
 **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM applications are performing reliably by allowing users to check aspects such as correctness, structural integrity, bias, hallucination, etc. UpTrain can be used to:
 
-1) Validate model's response and safeguard your users against hallucinations, bias, incorrect output formats, etc.
-2) Experiment across multiple model providers, prompt templates, and quantify model's performance.
-3) Monitor your model's performance in production and protect yourself against unwanted drifts
+## Experimentation
 
+UpTrain framework can be used to experiment across multiple prompts, model providers, chain configurations, etc. and get quantitative scores to compare them. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
 
-# Key Features 💡
+<img width="600" src="https://github.com/uptrain-ai/uptrain/assets/108270398/f6d1802a-079a-4bf0-8eb8-de879c2aa465" alt="uptrain experimentation">
 
 
-- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
-- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
-- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
-- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
-- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
-- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
-- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
-- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
-- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
-- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
+## Validation
+
+You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
+
+<img width="600" src="https://github.com/uptrain-ai/uptrain/assets/108270398/a34af650-a8ea-466c-9b5d-83e7f31eb8e2" alt="uptrain validation">
+
+## Monitoring
+
+You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
 
 # Get started 🙌
 
 <!-- You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). -->
 
 To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
@@ -88,69 +86,70 @@
 ```
 
 Note: Uptrain uses commonly used python libraries like openai-evals and sentence-transformers. To make sure, all the functionalities work, use the `uptrain-add` command to install the full version of the package.
 ```bash
 uptrain-add --feature full
 ```
 
-### How to define checks:
-Say we want to check whether our model's responses contain any grammatical mistakes or not.
+### How to use UpTrain in 4 simple steps:
+Say we want to plot a line chart showing whether our model's responses contain any grammatical mistakes or not.
 
 ```python
-# Define your checkset - list of simple checks, dataset file, 
-# and api_keys
+# Step 1: Choose and create the appropriate operator from UpTrain
+grammar_score = GrammarScore(
+  col_in_text = "model_response",       # input column name (from dataset)
+  col_out = "grammar_score"             # desired output column name
+)
+
+# Step 2: Create a check with the operators and the required plots as arguments 
+grammar_check = Check(
+  operators = [grammar_score],
+  plots = LineChart(y = "grammar_score")
+)
 
+# Step 3: Create a CheckSet with the checks and data source as arguments
 checkset = CheckSet(
-    checks = Check(
-        name = "grammar_score",
-        operators = [
-            GrammarScore(
-                col_in_text = "model_response",
-                col_out = "grammar_score"
-            ),
-        ],
-        plots = PlotlyChart.Table(title="Grammar scores"),
-    ),
+    checks = [grammar_check]
     source = JsonReader(fpath = '...')
 )
-settings = Settings(openai_api_key = '...')
 
-checkset.setup(settings)
-checkset.run()
+# Step 4: Set up and run the CheckSet
+checkset.setup(Settings(openai_api_key = '...'))
+checkset.run(dataset)
 ```
 
 <!-- For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial). -->
 
 <h4> </h4>
 
+# Key Features 💡
+
+
+- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
+- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
+- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
+- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
+- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
+- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
+- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
+- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
+- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
+- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
+
+
 # Integrations
 
 | Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | 
 | ------------- | ------------- | ------------- | ------------- | 
 | OpenAI Evals ✅ | GPT-3.5-turbo ✅ | Langchain 🔜 | HuggingFace 🔜 |
 | EleutherAI LM Eval 🔜 | GPT-4 ✅  | Llama Index 🔜 |  Replicate 🔜 |
 | BIG-Bench 🔜 | Claude 🔜 | AutoGPT 🔜 |
 | | Cohere 🔜 | 
 
 
-# UpTrain in Action
-
-## Experimentation
-
-You can use the UpTrain framework to run and compare LLM responses for different prompts, models, LLM chains, etc. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
-
-## Validation
-
-You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
-
-## Monitoring
-
-You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
-
-
 # Why UpTrain 🤔?
 
 Large language models are trained over billions of data points and perform really well over a wide variety of tasks. But one thing these models are not good at is being deterministic. Even with the most well-crafted prompts, the model can misbehave for certain inputs, be it hallucinations, wrong output structure, toxic or biased response, irrelevant response, and error modes can be immense. 
 
 To ensure your LLM applications work reliably and correctly, UpTrain makes it easy for developers to evaluate the responses of their applications on multiple criteria. UpTrain's evaluation framework can be used to:
 
 1) Validate (and correct) the response of the model before showing it to the user
```

#### html2text {}

```diff
@@ -1,88 +1,88 @@
                                *** [uptrain] ***
-***** An open-source framework to evaluate, test and monitor LLM applications
-*****
+***** An open-source framework to evaluate and monitor LLM applications *****
             Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
                   Welcome] [Docs] [Community] [Website]  ***
   **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
 applications are performing reliably by allowing users to check aspects such as
 correctness, structural integrity, bias, hallucination, etc. UpTrain can be
-used to: 1) Validate model's response and safeguard your users against
-hallucinations, bias, incorrect output formats, etc. 2) Experiment across
-multiple model providers, prompt templates, and quantify model's performance.
-3) Monitor your model's performance in production and protect yourself against
-unwanted drifts # Key Features ð¡ - **[ChatGPT Grading](https://uptrain-
-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to
-grade your model outputs. - **[Custom Grading Checks](https://uptrain-
-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom
-grading prompts. - **[Embeddings Similarity Check](https://uptrain-
-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity
-between prompt and response embeddings - **[Output Validation](https://
-github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** -
-Safeguard your users against inappropriate responses - **[Prompt A/B Testing]
+used to: ## Experimentation UpTrain framework can be used to experiment across
+multiple prompts, model providers, chain configurations, etc. and get
+quantitative scores to compare them. Check out the [experimentation tutorial]
 (https://github.com/uptrain-ai/uptrain/blob/main/examples/
-prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and
-compare them quantatively. - **[UMAP Visualization and Clustering](https://
-uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding
-space using tools like UMAP and t-SNE. - **[Hallucination Checks]()** - Use
-metrics like custom grading, text similarity, and embedding similarity to check
-for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
-outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
-Built-in pivoting functionalities for data dice and slice to pinpoint low-
-performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
-performance in realtime. # Get started ð  To run it on your machine,
-checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
-quickstart): ### Install the package through pip: ```bash pip install uptrain
-``` Note: Uptrain uses commonly used python libraries like openai-evals and
-sentence-transformers. To make sure, all the functionalities work, use the
-`uptrain-add` command to install the full version of the package. ```bash
-uptrain-add --feature full ``` ### How to define checks: Say we want to check
-whether our model's responses contain any grammatical mistakes or not.
-```python # Define your checkset - list of simple checks, dataset file, # and
-api_keys checkset = CheckSet( checks = Check( name = "grammar_score", operators
-= [ GrammarScore( col_in_text = "model_response", col_out = "grammar_score" ),
-], plots = PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader
-(fpath = '...') ) settings = Settings(openai_api_key = '...') checkset.setup
-(settings) checkset.run() ```
-# Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
-frameworks | | ------------- | ------------- | ------------- | ------------- |
-| OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
-EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
-BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
-Action ## Experimentation You can use the UpTrain framework to run and compare
-LLM responses for different prompts, models, LLM chains, etc. Check out the
-[experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/
-examples/prompt_experiments_tutorial.ipynb) to learn more. ## Validation You
-can use the UpTrain Validation Manager to define checks, retry logic and
-validate your LLM responses before showing it to your users. Check out the
-[tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-validation_tutorial.ipynb). ## Monitoring You can use the UpTrain framework to
-continuously monitor your model's performance and get real-time insights on how
-well it is doing on a variety of evaluation metrics. Check out the monitoring
-tutorial to learn more. # Why UpTrain ð¤? Large language models are trained
-over billions of data points and perform really well over a wide variety of
-tasks. But one thing these models are not good at is being deterministic. Even
-with the most well-crafted prompts, the model can misbehave for certain inputs,
-be it hallucinations, wrong output structure, toxic or biased response,
-irrelevant response, and error modes can be immense. To ensure your LLM
-applications work reliably and correctly, UpTrain makes it easy for developers
-to evaluate the responses of their applications on multiple criteria. UpTrain's
-evaluation framework can be used to: 1) Validate (and correct) the response of
-the model before showing it to the user 2) Get quantitative measures to
-experiment across multiple prompts, model providers, etc. 3) Do unit testing to
-ensure no buggy prompt or code gets pushed into your production 4) Monitor your
-LLM applications in real time and understand when they are going wrong in order
-to fix them before users complain. We are constantly working to make UpTrain
-better. Want a new feature or need any integrations? Feel free to [create an
-issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://
-github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the
-repository. # License ð» This repo is published under Apache 2.0 license. We
-are also working towards adding a hosted offering to make setting off eval runs
-easier - please fill **[this form](https://docs.google.com/forms/d/e/
+prompt_experiments_tutorial.ipynb) to learn more. [uptrain experimentation] ##
+Validation You can use the UpTrain Validation Manager to define checks, retry
+logic and validate your LLM responses before showing it to your users. Check
+out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/
+examples/validation_tutorial.ipynb). [uptrain validation] ## Monitoring You can
+use the UpTrain framework to continuously monitor your model's performance and
+get real-time insights on how well it is doing on a variety of evaluation
+metrics. Check out the monitoring tutorial to learn more. # Get started ð
+To run it on your machine, checkout the [Quickstart tutorial](https://
+docs.uptrain.ai/getting-started/quickstart): ### Install the package through
+pip: ```bash pip install uptrain ``` Note: Uptrain uses commonly used python
+libraries like openai-evals and sentence-transformers. To make sure, all the
+functionalities work, use the `uptrain-add` command to install the full version
+of the package. ```bash uptrain-add --feature full ``` ### How to use UpTrain
+in 4 simple steps: Say we want to plot a line chart showing whether our model's
+responses contain any grammatical mistakes or not. ```python # Step 1: Choose
+and create the appropriate operator from UpTrain grammar_score = GrammarScore
+( col_in_text = "model_response", # input column name (from dataset) col_out =
+"grammar_score" # desired output column name ) # Step 2: Create a check with
+the operators and the required plots as arguments grammar_check = Check
+( operators = [grammar_score], plots = LineChart(y = "grammar_score") ) # Step
+3: Create a CheckSet with the checks and data source as arguments checkset =
+CheckSet( checks = [grammar_check] source = JsonReader(fpath = '...') ) # Step
+4: Set up and run the CheckSet checkset.setup(Settings(openai_api_key = '...'))
+checkset.run(dataset) ```
+# Key Features ð¡ - **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/
+operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model
+outputs. - **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/
+operators/language/ModelGradeScore/)** - Write your custom grading prompts. -
+**[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/
+CosineSimilarity/)** - Compute cosine similarity between prompt and response
+embeddings - **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/
+main/examples/validation_tutorial.ipynb)** - Safeguard your users against
+inappropriate responses - **[Prompt A/B Testing](https://github.com/uptrain-ai/
+uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment
+across multiple prompts and compare them quantatively. - **[UMAP Visualization
+and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** -
+Visualize your embedding space using tools like UMAP and t-SNE. - **
+[Hallucination Checks]()** - Use metrics like custom grading, text similarity,
+and embedding similarity to check for hallucinations. - **[Toxic Keywords
+Checks]()** - Make sure your model outputs are not biased or contain toxic
+keywords. - **[Feature Slicing]()** - Built-in pivoting functionalities for
+data dice and slice to pinpoint low-performing cohorts. - **[Realtime
+Dashboards]()** - Monitor your model's performance in realtime. # Integrations
+| Eval Frameworks | LLM Providers | LLM Packages | Serving frameworks | | -----
+-------- | ------------- | ------------- | ------------- | | OpenAI Evals â |
+GPT-3.5-turbo â | Langchain ð | HuggingFace ð | | EleutherAI LM Eval
+ð | GPT-4 â | Llama Index ð | Replicate ð | | BIG-Bench ð |
+Claude ð | AutoGPT ð | | | Cohere ð | # Why UpTrain ð¤? Large
+language models are trained over billions of data points and perform really
+well over a wide variety of tasks. But one thing these models are not good at
+is being deterministic. Even with the most well-crafted prompts, the model can
+misbehave for certain inputs, be it hallucinations, wrong output structure,
+toxic or biased response, irrelevant response, and error modes can be immense.
+To ensure your LLM applications work reliably and correctly, UpTrain makes it
+easy for developers to evaluate the responses of their applications on multiple
+criteria. UpTrain's evaluation framework can be used to: 1) Validate (and
+correct) the response of the model before showing it to the user 2) Get
+quantitative measures to experiment across multiple prompts, model providers,
+etc. 3) Do unit testing to ensure no buggy prompt or code gets pushed into your
+production 4) Monitor your LLM applications in real time and understand when
+they are going wrong in order to fix them before users complain. We are
+constantly working to make UpTrain better. Want a new feature or need any
+integrations? Feel free to [create an issue](https://github.com/uptrain-ai/
+uptrain/issues) or [contribute](https://github.com/uptrain-ai/uptrain/blob/
+main/CONTRIBUTING.md) directly to the repository. # License ð» This repo is
+published under Apache 2.0 license. We are also working towards adding a hosted
+offering to make setting off eval runs easier - please fill **[this form]
+(https://docs.google.com/forms/d/e/
 1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/
 viewform?usp=sf_link)** to get a waitlist slot. # Stay Updated âï¸ We are
 continuously adding tons of features and use cases. Please support us by giving
 the project a star â­! # Provide feedback (Harsher the better ð) We are
 building UpTrain in public. Help us improve by giving your feedback **[here]
 (https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-
 jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**. # Contributors ð¥ï¸ We
```

### Comparing `uptrain-0.3.4/pyproject.toml` & `uptrain-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "uptrain"
-version = "0.3.4"
+version = "0.3.6"
 description = "UpTrain - ML Observability and Retraining Framework"
 readme = "README.md"
 maintainers = [{ name = "UpTrain AI Team", email = "uptrain.ai@gmail.com" }]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `uptrain-0.3.4/tests/test_operators.py` & `uptrain-0.3.6/tests/test_operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -189,63 +189,58 @@
     # Return the input DataFrame as it is
     output_df = expand_op.run(df)["output"]
 
     # Print the output DataFrame
     print(output_df)
 
 
-# uptrain.operators.vis
-def test_vis_plot_operators():
+# uptrain.operators.chart
+def test_chart_operators():
     import polars as pl
-    from uptrain.operators import PlotlyChart
+    from uptrain.operators import LineChart, ScatterPlot, BarChart, Histogram, MultiPlot, CustomPlotlyChart
 
     # Create a DataFrame
     df = pl.DataFrame({"x": [1, 2, 3, 4, 5], "y": [10, 20, 15, 25, 30]})
 
-    # LINE CHART
-    # Create a line chart using the PlotlyChart class
-    line_chart = PlotlyChart.Line(props={"x": "x", "y": "y"}, title="Line Chart")
-
-    # Generate the line chart
-    line_chart = line_chart.run(df)["extra"]["chart"]
-
-    # Show the chart
-    # line_chart.show()
-
-    # SCATTER CHART
-    # Create a scatter chart using the PlotlyChart class
-    scatter_chart = PlotlyChart.Scatter(
-        props={"x": "x", "y": "y"}, title="Scatter Chart"
+    multiplot = MultiPlot(
+        charts=[
+            LineChart(
+                x="x",
+                y="y",
+                title="Line Chart"
+            ),
+            ScatterPlot(
+                x="x",
+                y="y",
+                title="Scatter Plot"
+            ),
+            BarChart(
+                x="x",
+                y="y",
+                title="Bar Chart"
+            ),
+            Histogram(
+                x="x",
+                title="Histogram"
+            ),
+            CustomPlotlyChart(
+                kind="funnel",
+                x="x",
+                y="y",
+                title="Funnel Chart"
+            )
+        ],
+        title="MultiPlot",
     )
 
-    # Generate the scatter chart
-    scatter_chart = scatter_chart.run(df)["extra"]["chart"]
-
-    # Show the chart
-    # scatter_chart.show()
-
-    # BAR CHART
-    # Create a bar chart using the PlotlyChart class
-    bar_chart = PlotlyChart.Bar(props={"x": "x", "y": "y"}, title="Bar Chart")
-
-    # Generate the bar chart
-    bar_chart = bar_chart.run(df)["extra"]["chart"]
-
-    # Show the chart
-    # bar_chart.show()
-
-    # HISTOGRAM
-    # Create a histogram using the PlotlyChart class
-    histogram = PlotlyChart.Histogram(props={"x": "x"}, title="Histogram")
-
-    # Generate the histogram
-    histogram = histogram.run(df)["extra"]["chart"]
+    # Generate the multiplot
+    chart = multiplot.run(df)["extra"]["chart"]
 
     # Show the chart
-    # histogram.show()
+    chart.show()
 
 
 # uptrain.operators.language.rouge
 def test_rouge_operator():
     import polars as pl
     from uptrain.operators import RougeScore
 
@@ -340,14 +335,14 @@
         }
     )
 
     # Set the reference text for comparison
     ref_text = "This is a sample text."
 
     # Create an instance of the TextComparison class
-    comp_op = TextComparison(reference_text=ref_text, col_in_text="text")
+    comp_op = TextComparison(reference_texts=ref_text, col_in_text="text")
 
     # Compare each text entry with the reference text
     comparison = comp_op.run(df)["output"]
 
     # Print the comparison results
     print(comparison)
```

### Comparing `uptrain-0.3.4/uptrain/cli.py` & `uptrain-0.3.6/uptrain/cli.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/dashboard/st_helpers.py` & `uptrain-0.3.6/uptrain/dashboard/st_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,36 @@
 
 import streamlit as st
 import polars as pl
 import pandas as pd
 import plotly.express as px
 
 from uptrain.framework import CheckSet, Check, Settings
+from uptrain.operators import Table
 
 
 # -----------------------------------------------------------
 # Utility functions
 # NOTE: functions with prefix `st_` create streamlit elements
 # -----------------------------------------------------------
 
+CONSOLIDATED_CHECK = Check(
+    name="Consolidated Results",
+    operators=[],
+    plots=[Table(title="Consolidated Results")],
+)
 
-def st_setup_layout():
+
+def st_setup_layout(title: str = "UpTrain Dashboard"):
     st.set_page_config(
         page_title="UpTrain Dashboard",
         layout="wide",
         page_icon="https://github.com/uptrain-ai/uptrain/raw/dashboard/uptrain/core/classes/logging/uptrain_logo_icon.png",
     )  # TODO: find another source for the icon
-    st.title("UpTrain Live Dashboard")
+    st.title(title)
     st_style = """<style> footer {visibility: hidden;} </style>"""
     st.markdown(st_style, unsafe_allow_html=True)
 
 
 def read_checkset(logs_folder: str):
     """read the uptrain configuration for this run"""
     config_path = os.path.join(logs_folder, "config.json")
@@ -37,38 +44,25 @@
     config_path = os.path.join(logs_folder, "settings.json")
     return Settings.deserialize(config_path)
 
 
 def st_make_check_selector(checkset: "CheckSet"):
     """Make a selector for a checkset"""
     # Pick a check from the checkset to view
-    checks = checkset.checks + [checkset._consolidated_check]
+    checks = checkset.checks + [CONSOLIDATED_CHECK]
     with st.sidebar:
         select_check_index = st.sidebar.selectbox(
             "Select a check to view",
             options=list(range(len(checks))),
             format_func=lambda x: checks[x].name,
         )  # streamlit is being weird with classes, so iterate over their indices
     check = checks[select_check_index]  # type: ignore
     return check
 
 
-def load_data_for_check_local(settings: "Settings", check: "Check"):
-    from uptrain.operators import DeltaWriter, JsonWriter
-
-    sink = CheckSet._get_sink_for_check(settings, check)
-    if isinstance(sink, (DeltaWriter, JsonWriter)):
-        source = sink.to_reader()
-        source.setup(settings)
-    else:
-        raise NotImplementedError(f"{type(sink)} is not supported for now.")
-    output = source.run()
-    return output["output"]
-
-
 def st_filter_template(df, attribute, default_all=False):
     container = st.container()
     all = st.checkbox(f"Select all {attribute}", value=default_all)
     values = list(df[attribute].unique().sort())
 
     if all:
         selected_options = container.multiselect(
```

### Comparing `uptrain-0.3.4/uptrain/dashboard/st_setup.py` & `uptrain-0.3.6/uptrain/dashboard/st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/framework/base.py` & `uptrain-0.3.6/uptrain/framework/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,28 @@
     "OperatorDAG",
     "Settings",
 ]
 
 
 class Settings(BaseSettings):
     # uptrain stores logs in this folder
-    logs_folder: str = "/tmp/uptrain_logs"
+    logs_folder: str = "/tmp/uptrain-logs"
 
     # external api related
     openai_api_key: str = Field(None, env="OPENAI_API_KEY")
     openai_rpm_limit: int = 100
 
     # uptrain managed service related
     uptrain_access_token: str = Field(None, env="UPTRAIN_ACCESS_TOKEN")
     uptrain_server_url: str = Field(None, env="UPTRAIN_SERVER_URL")
 
+    # allow additional fields as needed by different operators
+    class Config:
+        extra = "allow"
+
     def check_and_get(self, key: str) -> t.Any:
         """Check if a value is present in the settings and return it."""
         value = getattr(self, key)
         if value is None:
             raise ValueError(f"Expected value for {key} to be present in the settings.")
         return value
```

### Comparing `uptrain-0.3.4/uptrain/framework/checks.py` & `uptrain-0.3.6/uptrain/framework/checks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 """Implements `Check` objects used for LLM evaluation purposes.
 """
 from __future__ import annotations
 from dataclasses import dataclass
 import os
 import typing as t
 
+from loguru import logger
 import polars as pl
+from pydantic import BaseModel
 
 from uptrain.operators.base import *
 from uptrain.utilities import jsonload, jsondump, to_py_types, clear_directory
 from uptrain.framework.base import OperatorDAG, Settings
-from uptrain.operators import PlotlyChart
+from uptrain.operators import Table, PromptGenerator, TextCompletion, OutputParser
 
-if t.TYPE_CHECKING:
-    from uptrain.operators import PromptGenerator
+__all__ = ["Check", "CheckSet", "ExperimentArgs"]
 
-__all__ = [
-    "Check",
-    "CheckSet",
-]
 
-
-@register_op
-class Check(Operator):
+class Check:
     """A simple check that runs the given list of table operators in sequence.
 
     Attributes:
         name (str): Name of the check.
         operators (list[TableOp]): A list of operators to run in sequence on the input data. The output of each
             operator is passed as input to the next operator.
         plots (list[Operator]): How to plot the output of the check.
-
     """
 
     name: str
     operators: list[Operator]
     plots: list[Operator]
 
     def __init__(
@@ -108,20 +102,14 @@
 
     def __init__(
         self,
         source: Operator,
         checks: list[t.Any],
         preprocessors: list[TransformOp] | None = None,
     ):
-        self._consolidated_check = Check(
-            name="Consolidated Results",
-            operators=[],
-            plots=[PlotlyChart.Table(title="Consolidated Results")],
-        )
-
         self.source = source
         self.checks = checks
         self.preprocessors = preprocessors if preprocessors is not None else []
 
         # verify all checks have different names
         check_names = [check.name for check in checks]
         assert len(set(check_names)) == len(check_names), "Duplicate check names"
@@ -135,97 +123,149 @@
         self._settings = settings
         logs_dir = self._settings.logs_folder
         if not os.path.exists(logs_dir):
             os.makedirs(logs_dir)
         else:
             clear_directory(logs_dir)
 
+        logger.info(f"Uptrain Logs directory: {logs_dir}")
+
         # persist the check-set as well as the corresponding settings
         self.serialize(os.path.join(logs_dir, "config.json"))
         self._settings.serialize(os.path.join(logs_dir, "settings.json"))
 
         self.source.setup(self._settings)
         for preprocessor in self.preprocessors:
             preprocessor.setup(self._settings)
         for check in self.checks:
             check.setup(self._settings)
-        self._consolidated_check.setup(self._settings)
         return self
 
     def run(self):
         """Run all checks in this set."""
-        from uptrain.operators.io.writers import JsonWriter
+        from uptrain.operators import JsonWriter
 
         source_output = self.source.run()["output"]
-        assert source_output is not None, "Output of source is None"
+        if source_output is None:
+            raise RuntimeError("Dataset read from the source is: None")
+        if len(source_output) == 0:
+            raise RuntimeError("Dataset read from the source is: empty")
 
         if len(self.preprocessors) > 0:
             for preprocessor in self.preprocessors:
                 source_output = preprocessor.run(source_output)["output"]
                 assert source_output is not None, "Output of preprocessor is None"
 
             # persist the preprocessed input for debugging
             JsonWriter(
                 fpath=os.path.join(
                     self._settings.logs_folder, "preprocessed_input.jsonl"
                 )
             ).setup(self._settings).run(source_output)
 
-        consolidated_outputs = source_output
         for check in self.checks:
             check_output = check.run(source_output)
             assert check_output is not None, f"Output of check {check.name} is None"
             self._get_sink_for_check(self._settings, check).run(check_output)
 
-            if all(isinstance(operator, ColumnOp) for operator in check.operators):
-                consolidated_outputs = consolidated_outputs.with_columns(
-                    [
-                        check_output[col_name]
-                        for col_name in list(
-                            set(check_output.columns)
-                            - set(consolidated_outputs.columns)
-                        )
-                    ]
-                )
-
-        self._get_sink_for_check(self._settings, self._consolidated_check).run(
-            self._consolidated_check.run(consolidated_outputs)
-        )
-
     @staticmethod
     def _get_sink_for_check(settings: Settings, check: Check):
         """Get the sink operator for this check."""
-        from uptrain.operators.io.writers import JsonWriter
+        from uptrain.operators import JsonWriter
 
-        return JsonWriter(
-            fpath=os.path.join(settings.logs_folder, f"{check.name}.jsonl")
-        )
+        fname = check.name.replace(" ", "_") + ".jsonl"
+        return JsonWriter(fpath=os.path.join(settings.logs_folder, fname))
 
     @classmethod
     def from_dict(cls, data: dict) -> "CheckSet":
+        checks = [Check.from_dict(check) for check in data.get("checks", [])]
         return cls(
             source=deserialize_operator(data["source"]),
             preprocessors=[
                 deserialize_operator(op) for op in data.get("preprocessors", [])
             ],  # type: ignore
-            checks=[deserialize_operator(check) for check in data.get("checks", [])],
+            checks=checks,
         )
 
     def dict(self) -> dict:
         return {
             "source": to_py_types(self.source),
             "preprocessors": [to_py_types(op) for op in self.preprocessors],
-            "checks": [to_py_types(check) for check in self.checks],
+            "checks": [check.dict() for check in self.checks],
         }
 
     @classmethod
     def deserialize(cls, fpath: str) -> "CheckSet":
         with open(fpath, "r") as f:
             return cls.from_dict(jsonload(f))
 
     def serialize(self, fpath: t.Optional[str] = None):
         """Serialize this check set along with the run settings to a JSON file."""
         if fpath is None:
             fpath = os.path.join(self._settings.logs_folder, "config.json")
 
         with open(fpath, "w") as f:
             jsondump(self.dict(), f)
+
+
+class ExperimentArgs(BaseModel):
+    """Container for arguments to run a LLM experiment. This is the entrypoint to run prompt/model tests with Uptrain for users.
+    This generates multiple prompts, generate LLM responses for them and parses the response to add multiple columns.
+
+    Attributes:
+        prompt_template (str): Prompt template to generate multiple prompts to experiment with.
+        prompt_params (dict(str, str)): Dictionary of prompt variables with experiment with.
+        models (str or list[str]): Either a single model or list of models to experiment with.
+        context_vars (dict or list): List of dataset variables with mapping between variable name in prompt and variable name in dataset
+        temperature (float): Temperature for the LLM response generation.
+        col_out_response (str): LLM output will be saved under this column name
+        col_out_mapping (dict): Mapping used to parse LLM response
+    """
+
+    prompt_template: str
+    prompt_params: dict = {}
+    models: t.Union[str, list[str]]
+    context_vars: t.Union[dict, list]
+    temperature: float = 1.0
+    col_out_response: str = "response"
+    col_out_mapping: t.Optional[dict] = None
+
+    def _get_preprocessors(self):
+        "Convert experiment args into checkset preprocessors for execution"
+        if isinstance(self.context_vars, list):
+            self.context_vars = dict(zip(self.context_vars, self.context_vars))
+
+        preprocessors = [
+            PromptGenerator(
+                prompt_template=self.prompt_template,
+                prompt_params=self.prompt_params,
+                models=[self.models] if isinstance(self.models, str) else self.models,
+                context_vars=self.context_vars,
+            ),
+            TextCompletion(
+                col_in_prompt="exp_prompt",
+                col_in_model="exp_model",
+                col_out_completion=self.col_out_response,
+                temperature=self.temperature,
+            ),
+        ]
+
+        if self.col_out_mapping is not None:
+            preprocessors.append(
+                OutputParser(
+                    col_in_response=self.col_out_response,
+                    col_out_mapping=self.col_out_mapping,
+                )
+            )
+
+        return preprocessors
+
+    def _modify_checks(self, checks):
+        "Modify checks to add experiment variables into plots"
+        for check in checks:
+            if check.plots is not None:
+                for plot in check.plots:
+                    if plot.kind in ["histogram", "bar", "line"]:
+                        if "barmode" not in plot.props:
+                            plot.props.update({"barmode": "group"})
+                        plot.props["color"] = "exp_experiment_id"
+        return checks
```

### Comparing `uptrain-0.3.4/uptrain/framework/signal.py` & `uptrain-0.3.6/uptrain/framework/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/base.py` & `uptrain-0.3.6/uptrain/operators/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Operators for the uptrain.core module. 
 """
 
 from __future__ import annotations
 import importlib
+import types
 import typing as t
 import typing_extensions as te
 
 from loguru import logger
 from pydantic import BaseModel, Field, root_validator
 import polars as pl
 
@@ -29,14 +30,28 @@
 ]
 
 # -----------------------------------------------------------
 # Base classes for operators
 # -----------------------------------------------------------
 
 
+def make_module_for_custom_ops():
+    """Creates a module to hold custom operators. `inspect.getsource` is
+    giving me a lot of grief.
+    """
+    mod = types.ModuleType("_uptrain_custom_ops")
+    preamble = [
+        "from uptrain.operators import ColumnOp, TransformOp, register_custom_op",
+        "import polars as pl",
+    ]
+    for line in preamble:
+        exec(line, mod.__dict__)
+    return mod
+
+
 class TYPE_TABLE_OUTPUT(te.TypedDict):
     output: pl.DataFrame | None
     extra: te.NotRequired[dict]
 
 
 class Operator(t.Protocol):
     """
@@ -58,40 +73,36 @@
     """
 
     def dict(self) -> dict:
         """
         Serialize this operator to a json dictionary. The objective is to be able to
         recreate the operator from this dict.
 
-        NOTE: If your operator is a pydantic model, pydantic handles this. Though if you
-        have fields with custom non-python types, you MUST override and implement both a
-        `dict` and a`from_dict` method.
+        NOTE: If your operator is a pydantic model, the `to_py_types` method in
+        `uptrain.utilities` handles this. Though if you have fields with custom
+        non-python types, you MUST override and implement both a `dict` and a`from_dict`
+        method.
+        TODO: With pydantic v2, nested models work with custom (de)serializers. Use that
+        when moving.
         """
         ...
 
     def setup(self, settings: "Settings") -> "Operator":
         """Setup the operator. This must be called before the operator is run."""
         ...
 
     run: t.Callable[..., TYPE_TABLE_OUTPUT]  # runs the operator
 
 
 class OpBaseModel(BaseModel):
     """
     Base class you can use if constructing an operator using a pydantic
     model, to get around some of the sharp edges.
-
-    Attributes:
-        _state (dict): A dict you can use to store state values between multiple
-            calls to the `run` method.
-
     """
 
-    _state: dict = Field(default_factory=dict)
-
     class Config:
         extra = "allow"
         smart_union = True
         underscore_attrs_are_private = True
 
 
 class ColumnOp(OpBaseModel):
@@ -147,35 +158,61 @@
         cls, "run"
     ), "All Uptrain operators must define a `setup` and a `run` method."
     op_name = f"{cls.__module__}:{cls.__name__}"
     cls._uptrain_op_name = op_name  # type: ignore
     return cls
 
 
+def register_custom_op(cls: T) -> T:
+    """Decorator that marks the class as a custom Uptrain operator, that is not
+    part of the core uptrain package. These are serialized by storing the entire
+    source code of the class, and deserialized by exec-ing the source code.
+
+    NOTE: This introduces some restrictions on the operator.
+    - This operator is dserialised in an empty namespace, so all imports must
+    be done inside the class definition.
+    - For typing, use string annotations.
+    - Custom operators must be defined in a separate .py file and not in the
+    interpreter (like a jupyter notebook).
+    """
+    cls._uptrain_op_custom = True  # type: ignore
+    return register_op(cls)
+
+
+CUSTOM_OP_MODULE = make_module_for_custom_ops()
+
+
 def deserialize_operator(data: dict) -> Operator:
     """Deserialize an operator from the serialized dict."""
     op_name = data["op_name"]
+    params = data["params"]
     mod_name, cls_name = op_name.split(":")
     try:
-        mod = importlib.import_module(mod_name)
-        op = getattr(mod, cls_name)
+        # Check if it is a custom operator, that'd need exec-ing
+        if "source" in data:
+            exec(data["source"], CUSTOM_OP_MODULE.__dict__)
+            klass = getattr(CUSTOM_OP_MODULE, cls_name)
+            # to get around serialisation round-trip woes
+            klass._uptrain_op_custom_source = data["source"]
+            return klass(**params)  # type: ignore
+        else:
+            mod = importlib.import_module(mod_name)
+            op = getattr(mod, cls_name)
+            # Is it a class implemented by uptrain or a regular pydantic model?
+            if hasattr(op, "from_dict"):
+                return op.from_dict(params)  # type: ignore
+            else:
+                return op(**params)  # type: ignore
+
     except (ModuleNotFoundError, AttributeError) as exc:
         logger.error(
             f"Error when trying to fetch the operator: \n{exc}\n Creating a placeholder op for {op_name}."
         )
         return PlaceholderOp(op_name=op_name, params=data["params"])
 
-    params = data["params"]
-    if hasattr(op, "from_dict"):
-        # not a pydantic model, so a class implemented by uptrain
-        return op.from_dict(params)  # type: ignore
-    else:
-        # likely a pydantic model
-        return op(**params)  # type: ignore
-
 
 # -----------------------------------------------------------
 # Utility routines for operators
 # -----------------------------------------------------------
 
 
 def get_output_col_name_at(index: int) -> str:
```

### Comparing `uptrain-0.3.4/uptrain/operators/code/sql.py` & `uptrain-0.3.6/uptrain/operators/code/sql.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/drift.py` & `uptrain-0.3.6/uptrain/operators/drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         ```
 
     Output:
         ```
         INFO     | uptrain.operators.drift:run:181 - Drift detected using DDM!
         Counter: 129466
         ```
-
     """
 
     algorithm: t.Literal["DDM", "ADWIN"]
     params: t.Union[ParamsDDM, ParamsADWIN]
     col_in_measure: str = "metric"
 
     @root_validator
```

### Comparing `uptrain-0.3.4/uptrain/operators/embs.py` & `uptrain-0.3.6/uptrain/operators/embs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/io/readers.py` & `uptrain-0.3.6/uptrain/operators/io/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+"""Basic IO operators for reading and writing data from Uptrain."""
+
 from __future__ import annotations
 import typing as t
 
 import polars as pl
 import deltalake as dl
 
 if t.TYPE_CHECKING:
     from uptrain.framework import Settings
 from uptrain.operators.base import *
 
 # -----------------------------------------------------------
-# Read from text file formats - csv and json
+# Read from text file formats - csv, json
 # -----------------------------------------------------------
 
 
 @register_op
 class CsvReader(TransformOp):
     """Reads data from a csv file.
 
@@ -126,21 +128,48 @@
 
         if data is not None:
             assert isinstance(data, pl.DataFrame)
         return {"output": data}
 
 
 # -----------------------------------------------------------
-# Read from Uptrain's object storage
+# Writer objects
 # -----------------------------------------------------------
 
 
-class UptrainReader(TransformOp):
-    dataset_id: str
+@register_op
+class DeltaWriter(OpBaseModel):
+    fpath: str
+    columns: t.Optional[list[str]] = None
 
     def setup(self, settings: Settings):
         return self
 
-    def run(self) -> TYPE_TABLE_OUTPUT:
-        raise NotImplementedError(
-            "UptrainReader is not implemented yet in the library."
-        )
+    def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
+        if self.columns is None:
+            self.columns = list(data.columns)
+        assert set(self.columns) == set(data.columns)
+        data.write_delta(self.fpath, mode="append")
+        return {"output": None}
+
+    def to_reader(self):
+        return DeltaReader(fpath=self.fpath)  # type: ignore
+
+
+@register_op
+class JsonWriter(OpBaseModel):
+    fpath: str
+    columns: t.Optional[list[str]] = None
+
+    def setup(self, settings: Settings):
+        return self
+
+    def to_reader(self):
+        return JsonReader(fpath=self.fpath)  # type: ignore
+
+    def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
+        if self.columns is None:
+            self.columns = list(data.columns)
+        assert set(self.columns) == set(data.columns)
+        with open(self.fpath, "a") as f:
+            f.write(data.write_ndjson())
+        return {"output": None}
```

### Comparing `uptrain-0.3.4/uptrain/operators/language/embedding.py` & `uptrain-0.3.6/uptrain/operators/language/embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/language/generation.py` & `uptrain-0.3.6/uptrain/operators/language/generation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Implement operators to generate text. 
 """
 
 from __future__ import annotations
 import itertools
 import typing as t
+import json
 
 from loguru import logger
 import polars as pl
 from uptrain.framework import Settings
 
 if t.TYPE_CHECKING:
     from uptrain.framework import Settings
@@ -44,22 +45,23 @@
             self.context_vars = dict(zip(self.context_vars, self.context_vars))
         return self
 
     """Construct all the prompt variations and generate completions for each."""
 
     def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
         list_params = []
-        for combo in itertools.product(*self.prompt_params.values(), self.models):
+        for experiment_id, combo in enumerate(itertools.product(*self.prompt_params.values(), self.models)):
             prompt_params, model = combo[:-1], combo[-1]
             variables = dict(zip(self.prompt_params.keys(), prompt_params))
             list_params.append(
                 {
                     "template": self.prompt_template,
                     self.col_out_prefix + "model": model,
                     **{self.col_out_prefix + k: v for k, v in variables.items()},
+                    self.col_out_prefix + "experiment_id": experiment_id
                 }
             )
         params_dataset = pl.DataFrame(list_params)
 
         # Do a cross join of the input with the params dataset to get all the
         # inputs for the completion step
         input_dataset = data.join(params_dataset, on=None, how="cross")
@@ -68,15 +70,22 @@
         # formatting the prompt template with the row values
         prompts = []
         for row in input_dataset.iter_rows(named=True):
             fill = {k: row[v] for k, v in self.context_vars.items()}
             fill.update(
                 {k: row[self.col_out_prefix + k] for k in self.prompt_params.keys()}
             )
-            prompt = row["template"].format(**fill)
+
+            #TODO: Temp Fix for handling json in prompts. Permanent fix is to integrate langchain?
+            try:
+                prompt = row["template"].format(**fill)
+            except:
+                prompt = row['template']
+                for k, v in fill.items():
+                    prompt = prompt.replace("{{" + k + "}}", v)
             prompts.append(prompt)
 
         input_w_prompts = input_dataset.with_columns(
             [pl.Series(self.col_out_prefix + "prompt", prompts)]
         )
         return {"output": input_w_prompts}
 
@@ -96,34 +105,37 @@
     """
     Takes a table of prompts and LLM model to use, generates output text.
 
     Attributes:
         col_in_prompt (str): The name of the column containing the prompt template.
         col_in_model (str): The name of the column containing the model name.
         col_out_completion (str): The name of the column containing the generated text.
+        temperature (float): Temperature for the LLM to generate responses.
 
     Returns:
         TYPE_TABLE_OUTPUT: A dictionary containing the dataset with the output text.
     """
 
     col_in_prompt: str = "prompt"
     col_in_model: str = "model"
     col_out_completion: str = "generated"
+    temperature: float = 1.0
     _api_client: LLMMulticlient
 
     def setup(self, settings: Settings):
         self._api_client = LLMMulticlient(settings=settings)
         return self
 
     def _make_payload(self, id: t.Any, text: str, model: str) -> Payload:
         return Payload(
             endpoint="chat.completions",
             data={
                 "model": model,
                 "messages": [{"role": "user", "content": text}],
+                "temperature": self.temperature,
             },
             metadata={"index": id},
         )
 
     def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
         prompt_ser = data.get_column(self.col_in_prompt)
         model_ser = data.get_column(self.col_in_model)
@@ -150,7 +162,34 @@
 
         output_text = pl.Series(
             values=[val for _, val in sorted(results, key=lambda x: x[0])]
         )
         return {
             "output": data.with_columns([output_text.alias(self.col_out_completion)])
         }
+
+
+@register_op
+class OutputParser(ColumnOp):
+    """
+    Takes a table of LLM respones and parses them into individual columns
+    
+    Attributes:
+        col_in_response (str): The name of the column containing the raw model response.
+        col_out_mapping (str): A dictionary containing the mapping of keys in response to their output column names.
+
+    Returns:
+        TYPE_TABLE_OUTPUT: A dictionary containing the dataset with the output text.
+    """
+
+    col_in_response: str 
+    col_out_mapping: dict
+
+    def setup(self, settings: "Settings"):
+        return self
+
+    """Parse the LLM responses"""
+
+    def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
+        responses = data[self.col_in_response]
+        parsed_responses = pl.DataFrame([json.loads(x) for x in responses])
+        return {"output": data.with_columns([parsed_responses[k].alias(v) for k,v in self.col_out_mapping.items()])}
```

### Comparing `uptrain-0.3.4/uptrain/operators/language/grammar.py` & `uptrain-0.3.6/uptrain/operators/language/grammar.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/language/llm.py` & `uptrain-0.3.6/uptrain/operators/language/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Implement checks to test language quality. 
 """
 
 from __future__ import annotations
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
+import random
 import typing as t
 
 import aiolimiter
 from loguru import logger
 from tqdm.asyncio import tqdm_asyncio
 from pydantic import BaseModel, Field
 
@@ -40,52 +41,57 @@
     error: t.Optional[str] = None
 
 
 async def async_process_payload(
     payload: Payload, limiter: aiolimiter.AsyncLimiter, max_retries: int
 ) -> Payload:
     async with limiter:
-        for _ in range(max_retries):  # failed requests don't count towards rate limit
+        for count in range(
+            max_retries
+        ):  # failed requests don't count towards rate limit
             try:
                 if payload.endpoint == "chat.completions":
                     payload.response = await openai.ChatCompletion.acreate(
-                        **payload.data, request_timeout=5
+                        **payload.data, request_timeout=10
                     )
                     break
                 else:
                     raise ValueError(f"Unknown endpoint: {payload.endpoint}")
             except Exception as exc:
-                payload.error = str(exc)
                 logger.error(
                     f"Error when sending request to openai API: {payload.error}"
                 )
-                if isinstance(
-                    exc,
-                    (
-                        openai.error.RateLimitError,
-                        openai.error.ServiceUnavailableError,
-                        openai.error.APIError,
-                        openai.error.APIConnectionError,
-                        openai.error.Timeout,
-                    ),
+                if (
+                    isinstance(
+                        exc,
+                        (
+                            openai.error.RateLimitError,
+                            openai.error.ServiceUnavailableError,
+                            openai.error.APIError,
+                            openai.error.APIConnectionError,
+                            openai.error.Timeout,
+                        ),
+                    )
+                    and count < max_retries - 1
                 ):
-                    await asyncio.sleep(3)
+                    await asyncio.sleep(random.uniform(0.5, 1.5) * count + 1)
                 else:
+                    payload.error = str(exc)
                     break
 
         return payload
 
 
 class LLMMulticlient:
     """
     Use multiple threads to send requests to the OpenAI API concurrently.
     """
 
     def __init__(self, settings: t.Optional[Settings] = None):
-        self._max_tries = 3
+        self._max_tries = 4
         self._rpm_limit = 20
         if settings is not None:
             openai.api_key = settings.check_and_get("openai_api_key")  # type: ignore
             self._rpm_limit = settings.check_and_get("openai_rpm_limit")
 
     def fetch_responses(self, input_payloads: list[Payload]) -> list[Payload]:
         try:
```

### Comparing `uptrain-0.3.4/uptrain/operators/language/model_grade.py` & `uptrain-0.3.6/uptrain/operators/language/model_grade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Implement checks to test if a piece of text has been taken from a source.
 
 """
 
 from __future__ import annotations
 import typing as t
-import yaml
 import os
 
 from loguru import logger
 import polars as pl
 from uptrain.framework import Settings
 
 if t.TYPE_CHECKING:
@@ -90,26 +89,26 @@
             columns in the input dataset.
 
     """
 
     grading_prompt_template: str
     eval_type: t.Literal["cot_classify", "classify", "classify_cot"] = "cot_classify"
     choice_strings: list[str]
-    choice_scores: dict[str, float]
+    choice_scores: t.Union[dict[str, float], dict[str, list[float]]]
     context_vars: dict[str, str]
-    col_out: str = "model_grade_score"
+    col_out: t.Union[str, list[str]] = "model_grade_score"
 
     def setup(self, settings: Settings):
         self._api_client = LLMMulticlient(settings=settings)
         return self
 
     def _make_payload(self, id: t.Any, messages: list[dict]) -> Payload:
         return Payload(
             endpoint="chat.completions",
-            data={"model": "gpt-3.5-turbo", "messages": messages},
+            data={"model": "gpt-3.5-turbo", "messages": messages, "temperature": 0.2},
             metadata={"index": id},
         )
 
     def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
         prompts = []
         for row in data.rows(named=True):
             subs = {k: row[v] for k, v in self.context_vars.items()}
@@ -128,33 +127,45 @@
             self._make_payload(idx, prompt_msgs)
             for idx, prompt_msgs in enumerate(prompts)
         ]
         output_payloads = self._api_client.fetch_responses(input_payloads)
 
         results = []
         for res in output_payloads:
-            assert (
-                res is not None
-            ), "Response should not be None, we should've handled exceptions beforehand."
             idx = res.metadata["index"]
             if res.error is not None:
                 logger.error(
                     f"Error when processing payload at index {idx}: {res.error}"
                 )
                 results.append((idx, None))
             else:
-                resp_text = res.response["choices"][0]["message"]["content"]
-                choice = get_choice(
-                    text=resp_text,
-                    eval_type=self.eval_type,
-                    match_fn="starts_or_endswith",
-                    choice_strings=self.choice_strings,
-                )
-                score = get_choice_score(
-                    choice, self.choice_strings, self.choice_scores
-                )
-                results.append((idx, score))
-
-        result_scores = pl.Series(
-            [val for _, val in sorted(results, key=lambda x: x[0])]
-        )
-        return {"output": data.with_columns([result_scores.alias(self.col_out)])}
+                try:
+                    resp_text = res.response["choices"][0]["message"]["content"]
+                    choice = get_choice(
+                        text=resp_text,
+                        eval_type=self.eval_type,
+                        match_fn="starts_or_endswith",
+                        choice_strings=self.choice_strings,
+                    )
+                    score = get_choice_score(
+                        choice, self.choice_strings, self.choice_scores
+                    )
+                    results.append((idx, score))
+                except Exception as e:
+                    logger.error(
+                        f"Error when processing payload at index {idx}, not an API error: {e}"
+                    )
+                    results.append((idx, None))
+
+        if isinstance(self.col_out, list):
+            sorted(results, key=lambda x: x[0])
+            result_scores = [
+                pl.Series(
+                    [val[idx] if val is not None else None for _, val in results]
+                ).alias(self.col_out[idx])
+                for idx in range(len(self.col_out))
+            ]
+        else:
+            result_scores = pl.Series(
+                [val for _, val in sorted(results, key=lambda x: x[0])]
+            ).alias(self.col_out)
+        return {"output": data.with_columns(result_scores)}
```

### Comparing `uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py` & `uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py` & `uptrain-0.3.6/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/language/openai_evals.py` & `uptrain-0.3.6/uptrain/operators/language/openai_evals.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/language/rouge.py` & `uptrain-0.3.6/uptrain/operators/language/rouge.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/language/text.py` & `uptrain-0.3.6/uptrain/operators/language/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,70 @@
             return None
 
         results = data.get_column(self.col_in_text).apply(fetch_version)
         return {"output": data.with_columns([results.alias(self.col_out)])}
 
 
 @register_op
+class WordCount(ColumnOp):
+    """
+    Operator to calculate the number of words in each text entry in a column.
+
+    Attributes:
+        col_in_text (str): The name of the input column containing the text data.
+        col_out (str): The name of the output column containing the number of words.
+
+    Returns:
+        dict: A dictionary containing the calculated number of words.
+
+    Example:
+        ```
+        import polars as pl
+        from uptrain.operators import WordCount
+
+        # Create a DataFrame
+        df = pl.DataFrame({
+            "text": ["This is a sample text.", "Another example sentence.", "Yet another sentence."]
+        })
+
+        # Create an instance of the WordCount class
+        word_count_op = WordCount(col_in_text="text")
+
+        # Calculate the number of words in each text entry
+        word_counts = word_count_op.run(df)["output"]
+
+        # Print the word counts
+        print(word_counts)
+        ```
+
+    Output:
+        ```
+        shape: (3,)
+        Series: '_col_0' [i64]
+        [
+                5
+                3
+                3
+        ]
+        ```
+
+    """
+
+    col_in_text: str
+    col_out: str = "word_count"
+
+    def setup(self, settings: Settings):
+        return self
+
+    def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
+        results = data.get_column(self.col_in_text).apply(lambda x: len(x.split(" ")))
+        return {"output": data.with_columns([results.alias(self.col_out)])}
+
+
+@register_op
 class TextLength(ColumnOp):
     """
     Operator to calculate the length of each text entry in a column.
 
     Attributes:
         col_in_text (str): The name of the input column containing the text data.
         col_out (str): The name of the output column containing the text lengths.
@@ -141,18 +197,18 @@
         results = data.get_column(self.col_in_text).apply(len)
         return {"output": data.with_columns([results.alias(self.col_out)])}
 
 
 @register_op
 class TextComparison(ColumnOp):
     """
-    Operator to compare each text entry in a column with a reference text.
+    Operator to compare each text entry in a column with a list of reference texts.
 
     Attributes:
-        reference_text (str): The reference text for comparison.
+        reference_texts (Union[list[str], str]): List of reference text for comparison.
         col_in_text (str): The name of the input column containing the text data.
         col_out (str): The name of the output column containing the comparison results.
 
     Returns:
         dict: A dictionary containing the comparison results (1 if equal, 0 otherwise).
 
     Example:
@@ -162,18 +218,18 @@
 
         # Create a DataFrame
         df = pl.DataFrame({
             "text": ["This is a sample text.", "Another example sentence.", "Yet another sentence."]
         })
 
         # Set the reference text for comparison
-        ref_text = "This is a sample text."
+        ref_text = ["This is a sample text.", "Yet another sentence."]
 
         # Create an instance of the TextComparison class
-        comp_op = TextComparison(reference_text=ref_text, col_in_text="text")
+        comp_op = TextComparison(reference_texts=ref_text, col_in_text="text")
 
         # Compare each text entry with the reference text
         comparison = comp_op.run(df)["output"]
 
         # Print the comparison results
         print(comparison)
         ```
@@ -181,30 +237,32 @@
     Output:
         ```
         shape: (3,)
         Series: '_col_0' [i64]
         [
                 1
                 0
-                0
+                1
         ]
         ```
 
     """
 
-    reference_text: str
+    reference_texts: t.Union[list[str], str]
     col_in_text: str
     col_out: str = "text_comparison"
 
     def setup(self, settings: Settings):
+        if isinstance(self.reference_texts, str):
+            self.reference_texts = [self.reference_texts]
         return self
 
     def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
         results = data.get_column(self.col_in_text).apply(
-            lambda x: int(x == self.reference_text)
+            lambda x: int(sum([x == y for y in self.reference_texts]))
         )
         return {"output": data.with_columns([results.alias(self.col_out)])}
 
 
 # Check if a Keyword exists in input text
 @register_op
 class KeywordDetector(ColumnOp):
```

### Comparing `uptrain-0.3.4/uptrain/operators/metrics.py` & `uptrain-0.3.6/uptrain/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/operators/similarity.py` & `uptrain-0.3.6/uptrain/operators/similarity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/utilities/__init__.py` & `uptrain-0.3.6/uptrain/utilities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,39 @@
 # -----------------------------------------------------------
 # utility routines for JSON serialization - parts picked off
 # from the openai-evals codebase
 # -----------------------------------------------------------
 
 
 def to_py_types(obj: t.Any) -> t.Any:
+    import inspect
+
     # for nested dataclasses/pydantic models/operators
     if isinstance(obj, dict):
         return {k: to_py_types(v) for k, v in obj.items()}
     elif isinstance(obj, list):
         return [to_py_types(v) for v in obj]
     elif dataclasses.is_dataclass(obj):
         return to_py_types(dataclasses.asdict(obj))
     elif hasattr(obj, "_uptrain_op_name"):
-        return {"op_name": getattr(obj, "_uptrain_op_name"), "params": obj.dict()}
+        if hasattr(obj, "_uptrain_op_custom"):
+            if hasattr(obj, "_uptrain_op_custom_source"):
+                source = obj._uptrain_op_custom_source
+            else:
+                source = inspect.getsource(obj.__class__)
+            return {
+                "op_name": getattr(obj, "_uptrain_op_name"),
+                "params": obj.dict(include=set(obj.__fields__)),
+                "source": source,
+            }
+        else:
+            return {
+                "op_name": getattr(obj, "_uptrain_op_name"),
+                "params": obj.dict(include=set(obj.__fields__)),
+            }
     elif isinstance(obj, pydantic.BaseModel):
         return obj.dict()
 
     # for numpy types
     if isinstance(obj, np.integer):
         return int(obj)
     elif isinstance(obj, np.floating):
```

### Comparing `uptrain-0.3.4/uptrain/utilities/sql_utils.py` & `uptrain-0.3.6/uptrain/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/utilities/sql_utils_test.py` & `uptrain-0.3.6/uptrain/utilities/sql_utils_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/utilities/sqlglot_test.py` & `uptrain-0.3.6/uptrain/utilities/sqlglot_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/constants.py` & `uptrain-0.3.6/uptrain/v0/constants.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/algorithms/clustering.py` & `uptrain-0.3.6/uptrain/v0/core/classes/algorithms/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/algorithms/popularity_bias.py` & `uptrain-0.3.6/uptrain/v0/core/classes/algorithms/popularity_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/distances/cosine_distance.py` & `uptrain-0.3.6/uptrain/v0/core/classes/distances/cosine_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/distances/distance_resolver.py` & `uptrain-0.3.6/uptrain/v0/core/classes/distances/distance_resolver.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/distances/hamming_distance.py` & `uptrain-0.3.6/uptrain/v0/core/classes/distances/hamming_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/distances/l2_distance.py` & `uptrain-0.3.6/uptrain/v0/core/classes/distances/l2_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/distances/norm_ratio.py` & `uptrain-0.3.6/uptrain/v0/core/classes/distances/norm_ratio.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/finetuning/finetuning.py` & `uptrain-0.3.6/uptrain/v0/core/classes/finetuning/finetuning.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/framework.py` & `uptrain-0.3.6/uptrain/v0/core/classes/framework.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/helpers/annotation_helper.py` & `uptrain-0.3.6/uptrain/v0/core/classes/helpers/annotation_helper.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/helpers/config_handler.py` & `uptrain-0.3.6/uptrain/v0/core/classes/helpers/config_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/helpers/dataset_handler.py` & `uptrain-0.3.6/uptrain/v0/core/classes/helpers/dataset_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/helpers/model_handler.py` & `uptrain-0.3.6/uptrain/v0/core/classes/helpers/model_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/io/runtime_manager.py` & `uptrain-0.3.6/uptrain/v0/core/classes/io/runtime_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/log_handler.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/log_postgres.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/log_postgres.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/log_streamlit.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/log_streamlit.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/new_log_handler.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/new_log_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_run.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/new_st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_setup.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/new_st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/logging/st_run.py` & `uptrain-0.3.6/uptrain/v0/core/classes/logging/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/managers/check_manager.py` & `uptrain-0.3.6/uptrain/v0/core/classes/managers/check_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/__init__.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/abstract_measurable.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/abstract_measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/accuracy.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/condition.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/condition.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/custom.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/custom.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/distance.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature_concat.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/feature_concat.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/input_feature.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/input_feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable_resolver.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/measurable_resolver.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/output_feature.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/output_feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/measurables/scalar_from_embedding.py` & `uptrain-0.3.6/uptrain/v0/core/classes/measurables/scalar_from_embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_check.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/abstract_check.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_monitor.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/abstract_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/accuracy.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/concept_drift.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/concept_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/custom_monitor.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/custom_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_drift.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/data_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_integrity.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/data_integrity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/edge_case.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/edge_case.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/feature_drift.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/feature_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/model_bias.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/model_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/monitors/output_comparison.py` & `uptrain-0.3.6/uptrain/v0/core/classes/monitors/output_comparison.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/signals/signal.py` & `uptrain-0.3.6/uptrain/v0/core/classes/signals/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/signals/signal_manager.py` & `uptrain-0.3.6/uptrain/v0/core/classes/signals/signal_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/statistics/convergence.py` & `uptrain-0.3.6/uptrain/v0/core/classes/statistics/convergence.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/statistics/distance.py` & `uptrain-0.3.6/uptrain/v0/core/classes/statistics/distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/statistics/distribution.py` & `uptrain-0.3.6/uptrain/v0/core/classes/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/statistics/norm_embedding.py` & `uptrain-0.3.6/uptrain/v0/core/classes/statistics/norm_embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/statistics/old_distribution.py` & `uptrain-0.3.6/uptrain/v0/core/classes/statistics/old_distribution.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/visuals/clustering.py` & `uptrain-0.3.6/uptrain/v0/core/classes/visuals/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/visuals/dimensionality_reduction.py` & `uptrain-0.3.6/uptrain/v0/core/classes/visuals/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/visuals/plot.py` & `uptrain-0.3.6/uptrain/v0/core/classes/visuals/plot.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/classes/visuals/shap.py` & `uptrain-0.3.6/uptrain/v0/core/classes/visuals/shap.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/encoders/__init__.py` & `uptrain-0.3.6/uptrain/v0/core/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/lib/algorithms.py` & `uptrain-0.3.6/uptrain/v0/core/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/lib/cache.py` & `uptrain-0.3.6/uptrain/v0/core/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/lib/datastores.py` & `uptrain-0.3.6/uptrain/v0/core/lib/datastores.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/lib/helper_funcs.py` & `uptrain-0.3.6/uptrain/v0/core/lib/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/core/lib/model_signal_funcs.py` & `uptrain-0.3.6/uptrain/v0/core/lib/model_signal_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/ee/classes/measurables/llm_measurables.py` & `uptrain-0.3.6/uptrain/v0/ee/classes/measurables/llm_measurables.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/ee/lib/algorithms.py` & `uptrain-0.3.6/uptrain/v0/ee/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/ee/lib/cache.py` & `uptrain-0.3.6/uptrain/v0/ee/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/ee/lib/ops_agg.py` & `uptrain-0.3.6/uptrain/v0/ee/lib/ops_agg.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_a-b_testing.py` & `uptrain-0.3.6/uptrain/v0/tests/test_a-b_testing.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_concept_drift_custom_monitor.py` & `uptrain-0.3.6/uptrain/v0/tests/test_concept_drift_custom_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_dashboard.py` & `uptrain-0.3.6/uptrain/v0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_data_drift.py` & `uptrain-0.3.6/uptrain/v0/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_data_integrity.py` & `uptrain-0.3.6/uptrain/v0/tests/test_data_integrity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_data_integrity_zscore.py` & `uptrain-0.3.6/uptrain/v0/tests/test_data_integrity_zscore.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_datastores.py` & `uptrain-0.3.6/uptrain/v0/tests/test_datastores.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_edge_cases.py` & `uptrain-0.3.6/uptrain/v0/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_helpers/dataset.py` & `uptrain-0.3.6/uptrain/v0/tests/test_helpers/dataset.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_helpers/get_data_from_remote.py` & `uptrain-0.3.6/uptrain/v0/tests/test_helpers/get_data_from_remote.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_helpers/helper_funcs.py` & `uptrain-0.3.6/uptrain/v0/tests/test_helpers/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_tensorflow.py` & `uptrain-0.3.6/uptrain/v0/tests/test_helpers/model_tensorflow.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_torch.py` & `uptrain-0.3.6/uptrain/v0/tests/test_helpers/model_torch.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_helpers/pushup_signal.py` & `uptrain-0.3.6/uptrain/v0/tests/test_helpers/pushup_signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_adwin.py` & `uptrain-0.3.6/uptrain/v0/tests/test_monitors_concept_drift_adwin.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_ddm.py` & `uptrain-0.3.6/uptrain/v0/tests/test_monitors_concept_drift_ddm.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_recommender_bias.py` & `uptrain-0.3.6/uptrain/v0/tests/test_recommender_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_visuals_dimensionality_reduction.py` & `uptrain-0.3.6/uptrain/v0/tests/test_visuals_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_visuals_plot.py` & `uptrain-0.3.6/uptrain/v0/tests/test_visuals_plot.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/v0/tests/test_visuals_shap.py` & `uptrain-0.3.6/uptrain/v0/tests/test_visuals_shap.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.4/uptrain/validation_wrapper/validation_manager.py` & `uptrain-0.3.6/uptrain/validation_wrapper/validation_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,34 +6,48 @@
 from uptrain.framework.signal import Signal
 from uptrain.framework.checks import Check, Settings
 
 
 class ValidationManager(BaseModel):
     check: t.Any
     completion_function: t.Any
+    retry_logic: list[dict]
     pass_condition: t.Any
     max_retries: int = 3
 
     def setup(self):
         self.check.setup(Settings())
 
     def run(self, inputs):
         for key in inputs.keys():
             inputs[key] = [inputs[key]]
         response_is_valid = False
         num_tries = 0
+        completion_function = self.completion_function
+        response_history = {}
         while not response_is_valid:
+            response = completion_function(inputs)
+            response_history.update({'attempt_' + str(num_tries): response})
             num_tries += 1
-            response = self.completion_function(inputs)
             inputs["response"] = [response]
             data = pl.from_dict(inputs)
             data = self.check.run(data)
             response_is_valid = self.pass_condition.run(data)[0]
 
             if response_is_valid:
                 logger.success(f"Validation check PASSED after {num_tries} attempt(s)")                
             elif num_tries < self.max_retries:
-                logger.warning(f"RETRYING validation check {num_tries} of {self.max_retries}")
+                completion_function = self.completion_function
+                selected_retry_function = "default"
+                for retry_condition in list(self.retry_logic):
+                    if retry_condition['signal'].run(data)[0] == True:
+                        completion_function = retry_condition['completion_function']
+                        selected_retry_function = retry_condition['name']
+                        break
+                logger.warning(f"RETRYING validation check {num_tries} of {self.max_retries} with logic: {selected_retry_function}")
             else:
                 response_is_valid = True
                 logger.warning(f"Validation check FAILED after {self.max_retries} attempt(s)")
+        if num_tries > 1:
+            logger.info(f"Response History: {response_history}")
+
         return response
```

### Comparing `uptrain-0.3.4/uptrain.egg-info/PKG-INFO` & `uptrain-0.3.6/uptrain.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.3.4
+Version: 0.3.6
 Summary: UpTrain - ML Observability and Retraining Framework
 Maintainer-email: UpTrain AI Team <uptrain.ai@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain
 Keywords: uptrain,ai,retraining,ML,observability
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
 <h2>
   <p align="center">
-    <p align="center">An open-source framework to evaluate, test and monitor LLM applications</p>
+    <p align="center">An open-source framework to evaluate and monitor LLM applications</p>
   </p>
 </h2>
 
 <p align="center">
 <a href="https://docs.uptrain.ai/docs/" rel="nofollow"><strong>Docs</strong></a>
 <!-- -
 <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a> -->
@@ -74,32 +74,30 @@
 <kbd>[<img title="French" alt="French language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/fr.svg" width="22">](/i18n/README.fr.md)</kbd>
 <kbd>[<img title="Japanese" alt="Japanese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/jp.svg" width="22">](/i18n/README.ja.md)</kbd>
 <kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd> -->
 
 
 **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM applications are performing reliably by allowing users to check aspects such as correctness, structural integrity, bias, hallucination, etc. UpTrain can be used to:
 
-1) Validate model's response and safeguard your users against hallucinations, bias, incorrect output formats, etc.
-2) Experiment across multiple model providers, prompt templates, and quantify model's performance.
-3) Monitor your model's performance in production and protect yourself against unwanted drifts
+## Experimentation
 
+UpTrain framework can be used to experiment across multiple prompts, model providers, chain configurations, etc. and get quantitative scores to compare them. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
 
-# Key Features 💡
+<img width="600" src="https://github.com/uptrain-ai/uptrain/assets/108270398/f6d1802a-079a-4bf0-8eb8-de879c2aa465" alt="uptrain experimentation">
 
 
-- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
-- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
-- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
-- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
-- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
-- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
-- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
-- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
-- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
-- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
+## Validation
+
+You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
+
+<img width="600" src="https://github.com/uptrain-ai/uptrain/assets/108270398/a34af650-a8ea-466c-9b5d-83e7f31eb8e2" alt="uptrain validation">
+
+## Monitoring
+
+You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
 
 # Get started 🙌
 
 <!-- You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). -->
 
 To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
@@ -109,69 +107,70 @@
 ```
 
 Note: Uptrain uses commonly used python libraries like openai-evals and sentence-transformers. To make sure, all the functionalities work, use the `uptrain-add` command to install the full version of the package.
 ```bash
 uptrain-add --feature full
 ```
 
-### How to define checks:
-Say we want to check whether our model's responses contain any grammatical mistakes or not.
+### How to use UpTrain in 4 simple steps:
+Say we want to plot a line chart showing whether our model's responses contain any grammatical mistakes or not.
 
 ```python
-# Define your checkset - list of simple checks, dataset file, 
-# and api_keys
+# Step 1: Choose and create the appropriate operator from UpTrain
+grammar_score = GrammarScore(
+  col_in_text = "model_response",       # input column name (from dataset)
+  col_out = "grammar_score"             # desired output column name
+)
+
+# Step 2: Create a check with the operators and the required plots as arguments 
+grammar_check = Check(
+  operators = [grammar_score],
+  plots = LineChart(y = "grammar_score")
+)
 
+# Step 3: Create a CheckSet with the checks and data source as arguments
 checkset = CheckSet(
-    checks = Check(
-        name = "grammar_score",
-        operators = [
-            GrammarScore(
-                col_in_text = "model_response",
-                col_out = "grammar_score"
-            ),
-        ],
-        plots = PlotlyChart.Table(title="Grammar scores"),
-    ),
+    checks = [grammar_check]
     source = JsonReader(fpath = '...')
 )
-settings = Settings(openai_api_key = '...')
 
-checkset.setup(settings)
-checkset.run()
+# Step 4: Set up and run the CheckSet
+checkset.setup(Settings(openai_api_key = '...'))
+checkset.run(dataset)
 ```
 
 <!-- For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial). -->
 
 <h4> </h4>
 
+# Key Features 💡
+
+
+- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
+- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
+- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
+- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
+- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
+- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
+- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
+- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
+- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
+- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
+
+
 # Integrations
 
 | Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | 
 | ------------- | ------------- | ------------- | ------------- | 
 | OpenAI Evals ✅ | GPT-3.5-turbo ✅ | Langchain 🔜 | HuggingFace 🔜 |
 | EleutherAI LM Eval 🔜 | GPT-4 ✅  | Llama Index 🔜 |  Replicate 🔜 |
 | BIG-Bench 🔜 | Claude 🔜 | AutoGPT 🔜 |
 | | Cohere 🔜 | 
 
 
-# UpTrain in Action
-
-## Experimentation
-
-You can use the UpTrain framework to run and compare LLM responses for different prompts, models, LLM chains, etc. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
-
-## Validation
-
-You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
-
-## Monitoring
-
-You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
-
-
 # Why UpTrain 🤔?
 
 Large language models are trained over billions of data points and perform really well over a wide variety of tasks. But one thing these models are not good at is being deterministic. Even with the most well-crafted prompts, the model can misbehave for certain inputs, be it hallucinations, wrong output structure, toxic or biased response, irrelevant response, and error modes can be immense. 
 
 To ensure your LLM applications work reliably and correctly, UpTrain makes it easy for developers to evaluate the responses of their applications on multiple criteria. UpTrain's evaluation framework can be used to:
 
 1) Validate (and correct) the response of the model before showing it to the user
```

#### html2text {}

```diff
@@ -1,100 +1,100 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.3.4 Summary: UpTrain - ML
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.6 Summary: UpTrain - ML
 Observability and Retraining Framework Maintainer-email: UpTrain AI Team
 ai@gmail.com> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
 uptrain,ai,retraining,ML,observability Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown Provides-Extra: test License-File:
 LICENSE
                                *** [uptrain] ***
-***** An open-source framework to evaluate, test and monitor LLM applications
-*****
+***** An open-source framework to evaluate and monitor LLM applications *****
             Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
                   Welcome] [Docs] [Community] [Website]  ***
   **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
 applications are performing reliably by allowing users to check aspects such as
 correctness, structural integrity, bias, hallucination, etc. UpTrain can be
-used to: 1) Validate model's response and safeguard your users against
-hallucinations, bias, incorrect output formats, etc. 2) Experiment across
-multiple model providers, prompt templates, and quantify model's performance.
-3) Monitor your model's performance in production and protect yourself against
-unwanted drifts # Key Features ð¡ - **[ChatGPT Grading](https://uptrain-
-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to
-grade your model outputs. - **[Custom Grading Checks](https://uptrain-
-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom
-grading prompts. - **[Embeddings Similarity Check](https://uptrain-
-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity
-between prompt and response embeddings - **[Output Validation](https://
-github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** -
-Safeguard your users against inappropriate responses - **[Prompt A/B Testing]
+used to: ## Experimentation UpTrain framework can be used to experiment across
+multiple prompts, model providers, chain configurations, etc. and get
+quantitative scores to compare them. Check out the [experimentation tutorial]
 (https://github.com/uptrain-ai/uptrain/blob/main/examples/
-prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and
-compare them quantatively. - **[UMAP Visualization and Clustering](https://
-uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding
-space using tools like UMAP and t-SNE. - **[Hallucination Checks]()** - Use
-metrics like custom grading, text similarity, and embedding similarity to check
-for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
-outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
-Built-in pivoting functionalities for data dice and slice to pinpoint low-
-performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
-performance in realtime. # Get started ð  To run it on your machine,
-checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
-quickstart): ### Install the package through pip: ```bash pip install uptrain
-``` Note: Uptrain uses commonly used python libraries like openai-evals and
-sentence-transformers. To make sure, all the functionalities work, use the
-`uptrain-add` command to install the full version of the package. ```bash
-uptrain-add --feature full ``` ### How to define checks: Say we want to check
-whether our model's responses contain any grammatical mistakes or not.
-```python # Define your checkset - list of simple checks, dataset file, # and
-api_keys checkset = CheckSet( checks = Check( name = "grammar_score", operators
-= [ GrammarScore( col_in_text = "model_response", col_out = "grammar_score" ),
-], plots = PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader
-(fpath = '...') ) settings = Settings(openai_api_key = '...') checkset.setup
-(settings) checkset.run() ```
-# Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
-frameworks | | ------------- | ------------- | ------------- | ------------- |
-| OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
-EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
-BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
-Action ## Experimentation You can use the UpTrain framework to run and compare
-LLM responses for different prompts, models, LLM chains, etc. Check out the
-[experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/
-examples/prompt_experiments_tutorial.ipynb) to learn more. ## Validation You
-can use the UpTrain Validation Manager to define checks, retry logic and
-validate your LLM responses before showing it to your users. Check out the
-[tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-validation_tutorial.ipynb). ## Monitoring You can use the UpTrain framework to
-continuously monitor your model's performance and get real-time insights on how
-well it is doing on a variety of evaluation metrics. Check out the monitoring
-tutorial to learn more. # Why UpTrain ð¤? Large language models are trained
-over billions of data points and perform really well over a wide variety of
-tasks. But one thing these models are not good at is being deterministic. Even
-with the most well-crafted prompts, the model can misbehave for certain inputs,
-be it hallucinations, wrong output structure, toxic or biased response,
-irrelevant response, and error modes can be immense. To ensure your LLM
-applications work reliably and correctly, UpTrain makes it easy for developers
-to evaluate the responses of their applications on multiple criteria. UpTrain's
-evaluation framework can be used to: 1) Validate (and correct) the response of
-the model before showing it to the user 2) Get quantitative measures to
-experiment across multiple prompts, model providers, etc. 3) Do unit testing to
-ensure no buggy prompt or code gets pushed into your production 4) Monitor your
-LLM applications in real time and understand when they are going wrong in order
-to fix them before users complain. We are constantly working to make UpTrain
-better. Want a new feature or need any integrations? Feel free to [create an
-issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://
-github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the
-repository. # License ð» This repo is published under Apache 2.0 license. We
-are also working towards adding a hosted offering to make setting off eval runs
-easier - please fill **[this form](https://docs.google.com/forms/d/e/
+prompt_experiments_tutorial.ipynb) to learn more. [uptrain experimentation] ##
+Validation You can use the UpTrain Validation Manager to define checks, retry
+logic and validate your LLM responses before showing it to your users. Check
+out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/
+examples/validation_tutorial.ipynb). [uptrain validation] ## Monitoring You can
+use the UpTrain framework to continuously monitor your model's performance and
+get real-time insights on how well it is doing on a variety of evaluation
+metrics. Check out the monitoring tutorial to learn more. # Get started ð
+To run it on your machine, checkout the [Quickstart tutorial](https://
+docs.uptrain.ai/getting-started/quickstart): ### Install the package through
+pip: ```bash pip install uptrain ``` Note: Uptrain uses commonly used python
+libraries like openai-evals and sentence-transformers. To make sure, all the
+functionalities work, use the `uptrain-add` command to install the full version
+of the package. ```bash uptrain-add --feature full ``` ### How to use UpTrain
+in 4 simple steps: Say we want to plot a line chart showing whether our model's
+responses contain any grammatical mistakes or not. ```python # Step 1: Choose
+and create the appropriate operator from UpTrain grammar_score = GrammarScore
+( col_in_text = "model_response", # input column name (from dataset) col_out =
+"grammar_score" # desired output column name ) # Step 2: Create a check with
+the operators and the required plots as arguments grammar_check = Check
+( operators = [grammar_score], plots = LineChart(y = "grammar_score") ) # Step
+3: Create a CheckSet with the checks and data source as arguments checkset =
+CheckSet( checks = [grammar_check] source = JsonReader(fpath = '...') ) # Step
+4: Set up and run the CheckSet checkset.setup(Settings(openai_api_key = '...'))
+checkset.run(dataset) ```
+# Key Features ð¡ - **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/
+operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model
+outputs. - **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/
+operators/language/ModelGradeScore/)** - Write your custom grading prompts. -
+**[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/
+CosineSimilarity/)** - Compute cosine similarity between prompt and response
+embeddings - **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/
+main/examples/validation_tutorial.ipynb)** - Safeguard your users against
+inappropriate responses - **[Prompt A/B Testing](https://github.com/uptrain-ai/
+uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment
+across multiple prompts and compare them quantatively. - **[UMAP Visualization
+and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** -
+Visualize your embedding space using tools like UMAP and t-SNE. - **
+[Hallucination Checks]()** - Use metrics like custom grading, text similarity,
+and embedding similarity to check for hallucinations. - **[Toxic Keywords
+Checks]()** - Make sure your model outputs are not biased or contain toxic
+keywords. - **[Feature Slicing]()** - Built-in pivoting functionalities for
+data dice and slice to pinpoint low-performing cohorts. - **[Realtime
+Dashboards]()** - Monitor your model's performance in realtime. # Integrations
+| Eval Frameworks | LLM Providers | LLM Packages | Serving frameworks | | -----
+-------- | ------------- | ------------- | ------------- | | OpenAI Evals â |
+GPT-3.5-turbo â | Langchain ð | HuggingFace ð | | EleutherAI LM Eval
+ð | GPT-4 â | Llama Index ð | Replicate ð | | BIG-Bench ð |
+Claude ð | AutoGPT ð | | | Cohere ð | # Why UpTrain ð¤? Large
+language models are trained over billions of data points and perform really
+well over a wide variety of tasks. But one thing these models are not good at
+is being deterministic. Even with the most well-crafted prompts, the model can
+misbehave for certain inputs, be it hallucinations, wrong output structure,
+toxic or biased response, irrelevant response, and error modes can be immense.
+To ensure your LLM applications work reliably and correctly, UpTrain makes it
+easy for developers to evaluate the responses of their applications on multiple
+criteria. UpTrain's evaluation framework can be used to: 1) Validate (and
+correct) the response of the model before showing it to the user 2) Get
+quantitative measures to experiment across multiple prompts, model providers,
+etc. 3) Do unit testing to ensure no buggy prompt or code gets pushed into your
+production 4) Monitor your LLM applications in real time and understand when
+they are going wrong in order to fix them before users complain. We are
+constantly working to make UpTrain better. Want a new feature or need any
+integrations? Feel free to [create an issue](https://github.com/uptrain-ai/
+uptrain/issues) or [contribute](https://github.com/uptrain-ai/uptrain/blob/
+main/CONTRIBUTING.md) directly to the repository. # License ð» This repo is
+published under Apache 2.0 license. We are also working towards adding a hosted
+offering to make setting off eval runs easier - please fill **[this form]
+(https://docs.google.com/forms/d/e/
 1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/
 viewform?usp=sf_link)** to get a waitlist slot. # Stay Updated âï¸ We are
 continuously adding tons of features and use cases. Please support us by giving
 the project a star â­! # Provide feedback (Harsher the better ð) We are
 building UpTrain in public. Help us improve by giving your feedback **[here]
 (https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-
 jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**. # Contributors ð¥ï¸ We
```

### Comparing `uptrain-0.3.4/uptrain.egg-info/SOURCES.txt` & `uptrain-0.3.6/uptrain.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+tests/test_custom_ops.py
 tests/test_operators.py
 uptrain/__init__.py
 uptrain/cli.py
 uptrain.egg-info/PKG-INFO
 uptrain.egg-info/SOURCES.txt
 uptrain.egg-info/dependency_links.txt
 uptrain.egg-info/entry_points.txt
@@ -20,25 +21,27 @@
 uptrain/framework/base.py
 uptrain/framework/checks.py
 uptrain/framework/remote.py
 uptrain/framework/signal.py
 uptrain/operators/__init__.py
 uptrain/operators/__init__.pyi
 uptrain/operators/base.py
+uptrain/operators/chart.py
 uptrain/operators/drift.py
 uptrain/operators/embs.py
 uptrain/operators/metrics.py
 uptrain/operators/similarity.py
 uptrain/operators/table.py
-uptrain/operators/vis.py
 uptrain/operators/code/__init__.py
 uptrain/operators/code/sql.py
 uptrain/operators/io/__init__.py
-uptrain/operators/io/readers.py
-uptrain/operators/io/writers.py
+uptrain/operators/io/base.py
+uptrain/operators/io/bq.py
+uptrain/operators/io/duck.py
+uptrain/operators/io/excel.py
 uptrain/operators/language/__init__.py
 uptrain/operators/language/embedding.py
 uptrain/operators/language/generation.py
 uptrain/operators/language/grammar.py
 uptrain/operators/language/llm.py
 uptrain/operators/language/model_grade.py
 uptrain/operators/language/openai_evals.py
```

