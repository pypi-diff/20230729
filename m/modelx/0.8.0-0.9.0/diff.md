# Comparing `tmp/modelx-0.8.0.tar.gz` & `tmp/modelx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\modelx-0.8.0.tar", last modified: Mon Jul  6 16:34:28 2020, max compression
+gzip compressed data, was "dist\modelx-0.9.0.tar", last modified: Sat Aug  8 16:47:49 2020, max compression
```

## Comparing `modelx-0.8.0.tar` & `modelx-0.9.0.tar`

### file list

```diff
@@ -1,203 +1,207 @@
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/
--rw-rw-rw-   0        0        0     7652 2017-10-21 14:59:00.000000 modelx-0.8.0/LICENSE.LESSER.txt
--rw-rw-rw-   0        0        0    35147 2017-09-09 01:33:52.000000 modelx-0.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      273 2018-02-08 14:53:53.000000 modelx-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8896 2020-07-06 16:34:28.000000 modelx-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     6253 2020-05-31 13:20:29.000000 modelx-0.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/
--rw-rw-rw-   0        0        0     1106 2020-07-06 16:24:56.000000 modelx-0.8.0/modelx/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/core/
--rw-rw-rw-   0        0        0      708 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/core/__init__.py
--rw-rw-rw-   0        0        0    20761 2020-07-06 16:06:35.000000 modelx-0.8.0/modelx/core/api.py
--rw-rw-rw-   0        0        0    32236 2020-07-05 05:28:30.000000 modelx-0.8.0/modelx/core/base.py
--rw-rw-rw-   0        0        0    21952 2020-07-05 06:24:56.000000 modelx-0.8.0/modelx/core/cells.py
--rw-rw-rw-   0        0        0     4954 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/core/chainmap.py
--rw-rw-rw-   0        0        0        0 2017-02-27 20:25:34.000000 modelx-0.8.0/modelx/core/config.py
--rw-rw-rw-   0        0        0     1512 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/core/errors.py
--rw-rw-rw-   0        0        0    15151 2020-06-04 05:00:30.000000 modelx-0.8.0/modelx/core/formula.py
--rw-rw-rw-   0        0        0    46491 2020-07-05 05:28:30.000000 modelx-0.8.0/modelx/core/model.py
--rw-rw-rw-   0        0        0     6650 2020-05-16 02:40:28.000000 modelx-0.8.0/modelx/core/node.py
--rw-rw-rw-   0        0        0     4483 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/core/reference.py
--rw-rw-rw-   0        0        0    60684 2020-07-05 06:24:56.000000 modelx-0.8.0/modelx/core/space.py
--rw-rw-rw-   0        0        0    19616 2020-07-03 15:52:44.000000 modelx-0.8.0/modelx/core/spacecontainer.py
--rw-rw-rw-   0        0        0    19547 2020-05-16 02:40:28.000000 modelx-0.8.0/modelx/core/system.py
--rw-rw-rw-   0        0        0     7944 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/core/util.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/io/
--rw-rw-rw-   0        0        0        0 2017-04-02 04:06:38.000000 modelx-0.8.0/modelx/io/__init__.py
--rw-rw-rw-   0        0        0    16553 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/io/excel.py
--rw-rw-rw-   0        0        0    11948 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/io/pandas.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/qtgui/
--rw-rw-rw-   0        0        0      344 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/qtgui/__init__.py
--rw-rw-rw-   0        0        0     2955 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/qtgui/api.py
--rw-rw-rw-   0        0        0    14097 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/qtgui/modeltree.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/serialize/
--rw-rw-rw-   0        0        0     3484 2020-07-02 10:14:05.000000 modelx-0.8.0/modelx/serialize/__init__.py
--rw-rw-rw-   0        0        0      713 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/serialize/jsonvalues.py
--rw-rw-rw-   0        0        0    22020 2020-06-22 15:26:35.000000 modelx-0.8.0/modelx/serialize/serializer_1.py
--rw-rw-rw-   0        0        0    42331 2020-07-03 14:03:32.000000 modelx-0.8.0/modelx/serialize/serializer_2.py
--rw-rw-rw-   0        0        0     8514 2020-07-03 13:44:22.000000 modelx-0.8.0/modelx/serialize/serializer_3.py
--rw-rw-rw-   0        0        0     9096 2020-06-23 13:39:25.000000 modelx-0.8.0/modelx/serialize/ziputil.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/testing/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/testing/__init__.py
--rw-rw-rw-   0        0        0     1788 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/testing/testutil.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/
--rw-rw-rw-   0        0        0        0 2017-03-30 04:15:52.000000 modelx-0.8.0/modelx/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/api/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/api/__init__.py
--rw-rw-rw-   0        0        0     4523 2020-05-12 15:00:48.000000 modelx-0.8.0/modelx/tests/core/api/test_api.py
--rw-rw-rw-   0        0        0      842 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/api/test_cur_model.py
--rw-rw-rw-   0        0        0      687 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/api/test_defcells.py
--rw-rw-rw-   0        0        0     1167 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/api/test_stacktrace.py
--rw-rw-rw-   0        0        0     6208 2020-05-08 12:40:39.000000 modelx-0.8.0/modelx/tests/core/api/test_traceback.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/base/
--rw-rw-rw-   0        0        0        0 2019-01-10 12:26:11.000000 modelx-0.8.0/modelx/tests/core/base/__init__.py
--rw-rw-rw-   0        0        0      749 2020-06-06 08:34:21.000000 modelx-0.8.0/modelx/tests/core/base/test_impl.py
--rw-rw-rw-   0        0        0      933 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/base/test_interface.py
--rw-rw-rw-   0        0        0     1984 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/base/test_lazyeval.py
--rw-rw-rw-   0        0        0     1572 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/base/test_repr.py
--rw-rw-rw-   0        0        0      784 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/base/test_view.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/cells/
--rw-rw-rw-   0        0        0        0 2017-10-09 07:02:10.000000 modelx-0.8.0/modelx/tests/core/cells/__init__.py
--rw-rw-rw-   0        0        0     1131 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/conftest.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/cells/node/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/node/__init__.py
--rw-rw-rw-   0        0        0      752 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/node/test_itemproxy.py
--rw-rw-rw-   0        0        0     1827 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/node/test_node_repr.py
--rw-rw-rw-   0        0        0     3277 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells.py
--rw-rw-rw-   0        0        0     2491 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells_clear.py
--rw-rw-rw-   0        0        0      543 2019-10-04 03:36:10.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells_inheritance.py
--rw-rw-rw-   0        0        0      470 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells_mutual.py
--rw-rw-rw-   0        0        0     1600 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells_property.py
--rw-rw-rw-   0        0        0     1644 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells_repr.py
--rw-rw-rw-   0        0        0     2527 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_cells_setitem.py
--rw-rw-rw-   0        0        0      741 2020-06-06 04:55:21.000000 modelx-0.8.0/modelx/tests/core/cells/test_copy.py
--rw-rw-rw-   0        0        0     2557 2020-05-08 12:40:39.000000 modelx-0.8.0/modelx/tests/core/cells/test_error.py
--rw-rw-rw-   0        0        0      938 2019-08-07 15:32:38.000000 modelx-0.8.0/modelx/tests/core/cells/test_formula.py
--rw-rw-rw-   0        0        0     2617 2020-05-15 12:27:39.000000 modelx-0.8.0/modelx/tests/core/cells/test_signature.py
--rw-rw-rw-   0        0        0     1943 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/cells/test_valuecells.py
--rw-rw-rw-   0        0        0     1607 2019-07-29 14:17:33.000000 modelx-0.8.0/modelx/tests/core/conftest.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/formula/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/formula/__init__.py
--rw-rw-rw-   0        0        0     1423 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/formula/test_formula.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/model/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/model/__init__.py
--rw-rw-rw-   0        0        0     4263 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/model/test_model.py
--rw-rw-rw-   0        0        0     2744 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/model/test_model_pickle.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/reference/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/__init__.py
--rw-rw-rw-   0        0        0     1829 2020-05-05 13:11:17.000000 modelx-0.8.0/modelx/tests/core/reference/test_attrref.py
--rw-rw-rw-   0        0        0     1666 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/test_clear_itemspaces.py
--rw-rw-rw-   0        0        0     1338 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/test_recalc.py
--rw-rw-rw-   0        0        0      935 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/test_recalc_dynamic_cells.py
--rw-rw-rw-   0        0        0      770 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/test_recalc_inherit.py
--rw-rw-rw-   0        0        0     1039 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/test_ref_order.py
--rw-rw-rw-   0        0        0      346 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/reference/test_refproxy.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/space/
--rw-rw-rw-   0        0        0        0 2019-07-29 13:01:22.000000 modelx-0.8.0/modelx/tests/core/space/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/__init__.py
--rw-rw-rw-   0        0        0     1450 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_base_ref_change.py
--rw-rw-rw-   0        0        0     2739 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_dynamic_spaces.py
--rw-rw-rw-   0        0        0     1165 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_param_formula.py
--rw-rw-rw-   0        0        0      369 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_space_dynamic.py
--rw-rw-rw-   0        0        0     1510 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_space_parameters.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/space/element/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/element/__init__.py
--rw-rw-rw-   0        0        0      861 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/element/test_element.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/__init__.py
--rw-rw-rw-   0        0        0     1309 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/test_add_bases.py
--rw-rw-rw-   0        0        0     9148 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/test_bases_change.py
--rw-rw-rw-   0        0        0      331 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/test_cyclic_inheritance.py
--rw-rw-rw-   0        0        0     1077 2020-05-17 11:03:58.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/test_del_base.py
--rw-rw-rw-   0        0        0     1712 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/test_space_derived.py
--rw-rw-rw-   0        0        0     4800 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/inheritance/test_space_inheritance.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/space/itemspaceparent/
--rw-rw-rw-   0        0        0        0 2020-05-16 05:41:49.000000 modelx-0.8.0/modelx/tests/core/space/itemspaceparent/__init__.py
--rw-rw-rw-   0        0        0      534 2020-05-16 07:41:36.000000 modelx-0.8.0/modelx/tests/core/space/itemspaceparent/conftest.py
--rw-rw-rw-   0        0        0      655 2020-05-22 13:44:39.000000 modelx-0.8.0/modelx/tests/core/space/itemspaceparent/test_formula.py
--rw-rw-rw-   0        0        0      941 2020-05-16 07:43:30.000000 modelx-0.8.0/modelx/tests/core/space/itemspaceparent/test_itemspaces.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/space/properties/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/properties/__init__.py
--rw-rw-rw-   0        0        0      836 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/properties/test_spaces.py
--rw-rw-rw-   0        0        0     2150 2020-07-05 06:26:17.000000 modelx-0.8.0/modelx/tests/core/space/test_copy.py
--rw-rw-rw-   0        0        0      323 2020-05-17 14:46:37.000000 modelx-0.8.0/modelx/tests/core/space/test_del_cells.py
--rw-rw-rw-   0        0        0      905 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_delattr.py
--rw-rw-rw-   0        0        0     2243 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_new_cells_from_csv.py
--rw-rw-rw-   0        0        0     4525 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_new_cells_from_excel.py
--rw-rw-rw-   0        0        0     3189 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_new_cells_from_pandas.py
--rw-rw-rw-   0        0        0     3577 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_new_space_from_csv.py
--rw-rw-rw-   0        0        0     2827 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_new_space_from_excel.py
--rw-rw-rw-   0        0        0     2402 2019-07-23 12:18:30.000000 modelx-0.8.0/modelx/tests/core/space/test_new_space_from_pandas.py
--rw-rw-rw-   0        0        0      471 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/space/test_set_formula.py
--rw-rw-rw-   0        0        0     4388 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_space.py
--rw-rw-rw-   0        0        0     2362 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/space/test_space_container.py
--rw-rw-rw-   0        0        0     1144 2020-06-23 14:58:32.000000 modelx-0.8.0/modelx/tests/core/space/test_space_reload.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/core/system/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/core/system/__init__.py
--rw-rw-rw-   0        0        0     3376 2020-05-08 12:40:39.000000 modelx-0.8.0/modelx/tests/core/system/test_system.py
--rw-rw-rw-   0        0        0      837 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/system/test_thread.py
--rw-rw-rw-   0        0        0     2229 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/core/test_util.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/io/
--rw-rw-rw-   0        0        0        0 2017-08-10 04:25:06.000000 modelx-0.8.0/modelx/tests/io/__init__.py
--rw-rw-rw-   0        0        0     3022 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/io/test_excel.py
--rw-rw-rw-   0        0        0     5560 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/io/test_pandas.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/lifelib/
--rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.8.0/modelx/tests/lifelib/__init__.py
--rw-rw-rw-   0        0        0     2646 2020-06-23 14:15:03.000000 modelx-0.8.0/modelx/tests/lifelib/test_serialize.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/performance/
--rw-rw-rw-   0        0        0        0 2020-05-15 15:50:48.000000 modelx-0.8.0/modelx/tests/performance/__init__.py
--rw-rw-rw-   0        0        0      693 2020-05-15 16:19:40.000000 modelx-0.8.0/modelx/tests/performance/test_performance.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/serialize/
--rw-rw-rw-   0        0        0       25 2020-06-23 12:26:50.000000 modelx-0.8.0/modelx/tests/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/
--rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/__init__.py
--rw-rw-rw-   0        0        0     2194 2020-06-23 09:05:43.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_cells_from_csv.py
--rw-rw-rw-   0        0        0     7390 2020-06-23 08:57:03.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_cells_from_excel.py
--rw-rw-rw-   0        0        0      927 2020-06-23 08:47:16.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_cells_from_pandas.py
--rw-rw-rw-   0        0        0     2291 2020-06-23 08:45:52.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_space_from_csv.py
--rw-rw-rw-   0        0        0     2830 2020-06-23 08:03:32.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_space_from_excel.py
--rw-rw-rw-   0        0        0     1012 2020-06-23 02:27:45.000000 modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_space_from_pandas.py
--rw-rw-rw-   0        0        0     2814 2020-06-23 09:23:52.000000 modelx-0.8.0/modelx/tests/serialize/test_dynamic.py
--rw-rw-rw-   0        0        0     1132 2020-07-04 03:06:59.000000 modelx-0.8.0/modelx/tests/serialize/test_log_input.py
--rw-rw-rw-   0        0        0     4538 2020-07-03 14:39:28.000000 modelx-0.8.0/modelx/tests/serialize/test_serialize.py
--rw-rw-rw-   0        0        0     4981 2020-06-20 13:43:10.000000 modelx-0.8.0/modelx/tests/serialize/test_ziputil.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/testdata/
--rw-rw-rw-   0        0        0      377 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/__init__.py
--rw-rw-rw-   0        0        0      240 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/reloadtest_after.py
--rw-rw-rw-   0        0        0      177 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/reloadtest_before.py
--rw-rw-rw-   0        0        0      420 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/testmodule.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/testdata/testpkg/
--rw-rw-rw-   0        0        0      160 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/testpkg/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx/tests/testdata/testpkg/nestedpkg/
--rw-rw-rw-   0        0        0      129 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/testpkg/nestedpkg/__init__.py
--rw-rw-rw-   0        0        0      120 2020-04-26 15:12:26.000000 modelx-0.8.0/modelx/tests/testdata/testpkg/testmod.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/modelx.egg-info/
--rw-rw-rw-   0        0        0     8896 2020-07-06 16:34:27.000000 modelx-0.8.0/modelx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6435 2020-07-06 16:34:27.000000 modelx-0.8.0/modelx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-06 16:34:27.000000 modelx-0.8.0/modelx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2020-07-06 16:34:27.000000 modelx-0.8.0/modelx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-07-06 16:34:27.000000 modelx-0.8.0/modelx.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/samples/
--rw-rw-rw-   0        0        0      116 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/samples/actuarial_projection/
--rw-rw-rw-   0        0        0        0 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/actuarial_projection/__init__.py
--rw-rw-rw-   0        0        0        0 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/actuarial_projection/projection.py
--rw-rw-rw-   0        0        0      649 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/dynamic_reference.py
-drwxrwxrwx   0        0        0        0 2020-07-06 16:34:28.000000 modelx-0.8.0/samples/netprem/
--rw-rw-rw-   0        0        0      116 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/netprem/__init__.py
--rw-rw-rw-   0        0        0      786 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/netprem/commutation_funcs.py
--rw-rw-rw-   0        0        0      422 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/netprem/lifetable.py
--rw-rw-rw-   0        0        0     1532 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/netprem/model.py
--rw-rw-rw-   0        0        0      272 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/netprem/policy.py
--rw-rw-rw-   0        0        0      656 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/sample_actuarialmodel.py
--rw-rw-rw-   0        0        0      225 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/sample_all.py
--rw-rw-rw-   0        0        0     1149 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/sample_firststep.py
--rw-rw-rw-   0        0        0      324 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/sample_lifetable_decorator.py
--rw-rw-rw-   0        0        0     1575 2019-10-13 15:26:22.000000 modelx-0.8.0/samples/sample_loan.py
--rw-rw-rw-   0        0        0     1695 2019-07-29 02:41:56.000000 modelx-0.8.0/samples/sample_model.py
--rw-rw-rw-   0        0        0      593 2019-08-07 11:52:59.000000 modelx-0.8.0/samples/sample_zero_bond.py
--rw-rw-rw-   0        0        0       59 2020-07-06 16:34:28.000000 modelx-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     5682 2020-04-26 15:12:26.000000 modelx-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/
+-rw-rw-rw-   0        0        0     7652 2017-10-21 14:59:00.000000 modelx-0.9.0/LICENSE.LESSER.txt
+-rw-rw-rw-   0        0        0    35147 2017-09-09 01:33:52.000000 modelx-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      273 2018-02-08 14:53:53.000000 modelx-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8896 2020-08-08 16:47:49.000000 modelx-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6253 2020-07-10 14:35:51.000000 modelx-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/
+-rw-rw-rw-   0        0        0     1106 2020-08-08 16:43:01.000000 modelx-0.9.0/modelx/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/core/
+-rw-rw-rw-   0        0        0      708 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/core/__init__.py
+-rw-rw-rw-   0        0        0    22170 2020-08-08 15:16:05.000000 modelx-0.9.0/modelx/core/api.py
+-rw-rw-rw-   0        0        0    32334 2020-08-06 14:46:57.000000 modelx-0.9.0/modelx/core/base.py
+-rw-rw-rw-   0        0        0    21952 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/core/cells.py
+-rw-rw-rw-   0        0        0     4954 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/core/chainmap.py
+-rw-rw-rw-   0        0        0        0 2017-02-27 20:25:34.000000 modelx-0.9.0/modelx/core/config.py
+-rw-rw-rw-   0        0        0     1512 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/core/errors.py
+-rw-rw-rw-   0        0        0    15151 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/core/formula.py
+-rw-rw-rw-   0        0        0    49839 2020-08-08 15:16:05.000000 modelx-0.9.0/modelx/core/model.py
+-rw-rw-rw-   0        0        0     6650 2020-05-16 02:40:28.000000 modelx-0.9.0/modelx/core/node.py
+-rw-rw-rw-   0        0        0     5031 2020-08-05 14:46:31.000000 modelx-0.9.0/modelx/core/reference.py
+-rw-rw-rw-   0        0        0    60574 2020-08-06 15:04:46.000000 modelx-0.9.0/modelx/core/space.py
+-rw-rw-rw-   0        0        0    26667 2020-08-07 13:56:57.000000 modelx-0.9.0/modelx/core/spacecontainer.py
+-rw-rw-rw-   0        0        0    21071 2020-08-07 02:47:19.000000 modelx-0.9.0/modelx/core/system.py
+-rw-rw-rw-   0        0        0     7944 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/core/util.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/io/
+-rw-rw-rw-   0        0        0        0 2017-04-02 04:06:38.000000 modelx-0.9.0/modelx/io/__init__.py
+-rw-rw-rw-   0        0        0     5640 2020-08-07 12:44:24.000000 modelx-0.9.0/modelx/io/baseio.py
+-rw-rw-rw-   0        0        0    11815 2020-08-02 05:08:23.000000 modelx-0.9.0/modelx/io/excel_legacy.py
+-rw-rw-rw-   0        0        0    18092 2020-08-07 12:41:59.000000 modelx-0.9.0/modelx/io/excelio.py
+-rw-rw-rw-   0        0        0    11948 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/io/pandas.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/qtgui/
+-rw-rw-rw-   0        0        0      344 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/qtgui/__init__.py
+-rw-rw-rw-   0        0        0     2955 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/qtgui/api.py
+-rw-rw-rw-   0        0        0    14097 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/qtgui/modeltree.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/serialize/
+-rw-rw-rw-   0        0        0     3862 2020-08-08 04:38:07.000000 modelx-0.9.0/modelx/serialize/__init__.py
+-rw-rw-rw-   0        0        0      713 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/serialize/jsonvalues.py
+-rw-rw-rw-   0        0        0    22020 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/serialize/serializer_1.py
+-rw-rw-rw-   0        0        0    42465 2020-08-08 04:38:07.000000 modelx-0.9.0/modelx/serialize/serializer_2.py
+-rw-rw-rw-   0        0        0     8559 2020-07-24 09:49:32.000000 modelx-0.9.0/modelx/serialize/serializer_3.py
+-rw-rw-rw-   0        0        0    49545 2020-08-08 06:50:28.000000 modelx-0.9.0/modelx/serialize/serializer_4.py
+-rw-rw-rw-   0        0        0    11609 2020-08-08 14:57:18.000000 modelx-0.9.0/modelx/serialize/ziputil.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/testing/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/testing/__init__.py
+-rw-rw-rw-   0        0        0     1788 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/testing/testutil.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/
+-rw-rw-rw-   0        0        0        0 2017-03-30 04:15:52.000000 modelx-0.9.0/modelx/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/api/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/api/__init__.py
+-rw-rw-rw-   0        0        0     4523 2020-05-12 15:00:48.000000 modelx-0.9.0/modelx/tests/core/api/test_api.py
+-rw-rw-rw-   0        0        0      842 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/api/test_cur_model.py
+-rw-rw-rw-   0        0        0      687 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/api/test_defcells.py
+-rw-rw-rw-   0        0        0     1167 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/api/test_stacktrace.py
+-rw-rw-rw-   0        0        0     6208 2020-05-08 12:40:39.000000 modelx-0.9.0/modelx/tests/core/api/test_traceback.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/base/
+-rw-rw-rw-   0        0        0        0 2019-01-10 12:26:11.000000 modelx-0.9.0/modelx/tests/core/base/__init__.py
+-rw-rw-rw-   0        0        0      749 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/core/base/test_impl.py
+-rw-rw-rw-   0        0        0      933 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/base/test_interface.py
+-rw-rw-rw-   0        0        0     1984 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/base/test_lazyeval.py
+-rw-rw-rw-   0        0        0     1572 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/base/test_repr.py
+-rw-rw-rw-   0        0        0      784 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/base/test_view.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/cells/
+-rw-rw-rw-   0        0        0        0 2017-10-09 07:02:10.000000 modelx-0.9.0/modelx/tests/core/cells/__init__.py
+-rw-rw-rw-   0        0        0     1131 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/conftest.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/cells/node/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/node/__init__.py
+-rw-rw-rw-   0        0        0      752 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/node/test_itemproxy.py
+-rw-rw-rw-   0        0        0     1827 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/node/test_node_repr.py
+-rw-rw-rw-   0        0        0     3277 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells.py
+-rw-rw-rw-   0        0        0     2491 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells_clear.py
+-rw-rw-rw-   0        0        0      543 2019-10-04 03:36:10.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells_inheritance.py
+-rw-rw-rw-   0        0        0      470 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells_mutual.py
+-rw-rw-rw-   0        0        0     1600 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells_property.py
+-rw-rw-rw-   0        0        0     1644 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells_repr.py
+-rw-rw-rw-   0        0        0     2527 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_cells_setitem.py
+-rw-rw-rw-   0        0        0      772 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/core/cells/test_copy.py
+-rw-rw-rw-   0        0        0     2557 2020-05-08 12:40:39.000000 modelx-0.9.0/modelx/tests/core/cells/test_error.py
+-rw-rw-rw-   0        0        0      938 2019-08-07 15:32:38.000000 modelx-0.9.0/modelx/tests/core/cells/test_formula.py
+-rw-rw-rw-   0        0        0     2617 2020-05-15 12:27:39.000000 modelx-0.9.0/modelx/tests/core/cells/test_signature.py
+-rw-rw-rw-   0        0        0     1943 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/cells/test_valuecells.py
+-rw-rw-rw-   0        0        0     1607 2019-07-29 14:17:33.000000 modelx-0.9.0/modelx/tests/core/conftest.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/formula/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/formula/__init__.py
+-rw-rw-rw-   0        0        0     1423 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/formula/test_formula.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/model/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/model/__init__.py
+-rw-rw-rw-   0        0        0     4263 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/model/test_model.py
+-rw-rw-rw-   0        0        0     2886 2020-08-06 15:04:45.000000 modelx-0.9.0/modelx/tests/core/model/test_model_pickle.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/reference/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/__init__.py
+-rw-rw-rw-   0        0        0     1829 2020-05-05 13:11:17.000000 modelx-0.9.0/modelx/tests/core/reference/test_attrref.py
+-rw-rw-rw-   0        0        0     1666 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/test_clear_itemspaces.py
+-rw-rw-rw-   0        0        0     1338 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/test_recalc.py
+-rw-rw-rw-   0        0        0      935 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/test_recalc_dynamic_cells.py
+-rw-rw-rw-   0        0        0      770 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/test_recalc_inherit.py
+-rw-rw-rw-   0        0        0     1039 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/test_ref_order.py
+-rw-rw-rw-   0        0        0      346 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/reference/test_refproxy.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/space/
+-rw-rw-rw-   0        0        0        0 2019-07-29 13:01:22.000000 modelx-0.9.0/modelx/tests/core/space/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/__init__.py
+-rw-rw-rw-   0        0        0     1450 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_base_ref_change.py
+-rw-rw-rw-   0        0        0     2739 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_dynamic_spaces.py
+-rw-rw-rw-   0        0        0     1165 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_param_formula.py
+-rw-rw-rw-   0        0        0      369 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_space_dynamic.py
+-rw-rw-rw-   0        0        0     1510 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_space_parameters.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/space/element/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/element/__init__.py
+-rw-rw-rw-   0        0        0      861 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/element/test_element.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/__init__.py
+-rw-rw-rw-   0        0        0     1309 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/test_add_bases.py
+-rw-rw-rw-   0        0        0     9148 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/test_bases_change.py
+-rw-rw-rw-   0        0        0      331 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/test_cyclic_inheritance.py
+-rw-rw-rw-   0        0        0     1077 2020-05-17 11:03:58.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/test_del_base.py
+-rw-rw-rw-   0        0        0     1712 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/test_space_derived.py
+-rw-rw-rw-   0        0        0     4800 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/inheritance/test_space_inheritance.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/space/itemspaceparent/
+-rw-rw-rw-   0        0        0        0 2020-05-16 05:41:49.000000 modelx-0.9.0/modelx/tests/core/space/itemspaceparent/__init__.py
+-rw-rw-rw-   0        0        0      534 2020-05-16 07:41:36.000000 modelx-0.9.0/modelx/tests/core/space/itemspaceparent/conftest.py
+-rw-rw-rw-   0        0        0      655 2020-05-22 13:44:39.000000 modelx-0.9.0/modelx/tests/core/space/itemspaceparent/test_formula.py
+-rw-rw-rw-   0        0        0      941 2020-05-16 07:43:30.000000 modelx-0.9.0/modelx/tests/core/space/itemspaceparent/test_itemspaces.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/space/properties/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/properties/__init__.py
+-rw-rw-rw-   0        0        0      836 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/properties/test_spaces.py
+-rw-rw-rw-   0        0        0     2150 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/core/space/test_copy.py
+-rw-rw-rw-   0        0        0      323 2020-05-17 14:46:37.000000 modelx-0.9.0/modelx/tests/core/space/test_del_cells.py
+-rw-rw-rw-   0        0        0      905 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_delattr.py
+-rw-rw-rw-   0        0        0     2243 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_new_cells_from_csv.py
+-rw-rw-rw-   0        0        0     4525 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_new_cells_from_excel.py
+-rw-rw-rw-   0        0        0     3189 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_new_cells_from_pandas.py
+-rw-rw-rw-   0        0        0     3577 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_new_space_from_csv.py
+-rw-rw-rw-   0        0        0     2827 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_new_space_from_excel.py
+-rw-rw-rw-   0        0        0     2402 2019-07-23 12:18:30.000000 modelx-0.9.0/modelx/tests/core/space/test_new_space_from_pandas.py
+-rw-rw-rw-   0        0        0      471 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/space/test_set_formula.py
+-rw-rw-rw-   0        0        0     4388 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_space.py
+-rw-rw-rw-   0        0        0     2362 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/space/test_space_container.py
+-rw-rw-rw-   0        0        0     1144 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/core/space/test_space_reload.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/core/system/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/core/system/__init__.py
+-rw-rw-rw-   0        0        0     3376 2020-05-08 12:40:39.000000 modelx-0.9.0/modelx/tests/core/system/test_system.py
+-rw-rw-rw-   0        0        0      837 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/system/test_thread.py
+-rw-rw-rw-   0        0        0     2229 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/core/test_util.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/io/
+-rw-rw-rw-   0        0        0        0 2017-08-10 04:25:06.000000 modelx-0.9.0/modelx/tests/io/__init__.py
+-rw-rw-rw-   0        0        0     3029 2020-07-24 09:53:05.000000 modelx-0.9.0/modelx/tests/io/test_excel.py
+-rw-rw-rw-   0        0        0    10318 2020-08-08 07:44:54.000000 modelx-0.9.0/modelx/tests/io/test_excelio.py
+-rw-rw-rw-   0        0        0     5560 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/io/test_pandas.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/lifelib/
+-rw-rw-rw-   0        0        0        0 2019-06-27 12:34:26.000000 modelx-0.9.0/modelx/tests/lifelib/__init__.py
+-rw-rw-rw-   0        0        0     2974 2020-07-12 05:43:22.000000 modelx-0.9.0/modelx/tests/lifelib/test_serialize.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/performance/
+-rw-rw-rw-   0        0        0        0 2020-05-15 15:50:48.000000 modelx-0.9.0/modelx/tests/performance/__init__.py
+-rw-rw-rw-   0        0        0      693 2020-05-15 16:19:40.000000 modelx-0.9.0/modelx/tests/performance/test_performance.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/serialize/
+-rw-rw-rw-   0        0        0        0 2020-07-11 10:49:13.000000 modelx-0.9.0/modelx/tests/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/
+-rw-rw-rw-   0        0        0        0 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/__init__.py
+-rw-rw-rw-   0        0        0     2196 2020-07-11 16:40:44.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_cells_from_csv.py
+-rw-rw-rw-   0        0        0     7390 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_cells_from_excel.py
+-rw-rw-rw-   0        0        0      927 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_cells_from_pandas.py
+-rw-rw-rw-   0        0        0     2291 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_space_from_csv.py
+-rw-rw-rw-   0        0        0     2830 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_space_from_excel.py
+-rw-rw-rw-   0        0        0     1012 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_space_from_pandas.py
+-rw-rw-rw-   0        0        0     2814 2020-07-10 14:35:51.000000 modelx-0.9.0/modelx/tests/serialize/test_dynamic.py
+-rw-rw-rw-   0        0        0     1148 2020-08-08 06:48:19.000000 modelx-0.9.0/modelx/tests/serialize/test_log_input.py
+-rw-rw-rw-   0        0        0     5648 2020-08-08 08:00:30.000000 modelx-0.9.0/modelx/tests/serialize/test_serialize.py
+-rw-rw-rw-   0        0        0     5937 2020-08-08 06:53:32.000000 modelx-0.9.0/modelx/tests/serialize/test_ziputil.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/testdata/
+-rw-rw-rw-   0        0        0      377 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/__init__.py
+-rw-rw-rw-   0        0        0      240 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/reloadtest_after.py
+-rw-rw-rw-   0        0        0      177 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/reloadtest_before.py
+-rw-rw-rw-   0        0        0      420 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/testmodule.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/testdata/testpkg/
+-rw-rw-rw-   0        0        0      160 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/testpkg/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx/tests/testdata/testpkg/nestedpkg/
+-rw-rw-rw-   0        0        0      129 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/testpkg/nestedpkg/__init__.py
+-rw-rw-rw-   0        0        0      120 2020-04-26 15:12:26.000000 modelx-0.9.0/modelx/tests/testdata/testpkg/testmod.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/modelx.egg-info/
+-rw-rw-rw-   0        0        0     8896 2020-08-08 16:47:48.000000 modelx-0.9.0/modelx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6548 2020-08-08 16:47:48.000000 modelx-0.9.0/modelx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-08-08 16:47:48.000000 modelx-0.9.0/modelx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2020-08-08 16:47:48.000000 modelx-0.9.0/modelx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2020-08-08 16:47:48.000000 modelx-0.9.0/modelx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/samples/
+-rw-rw-rw-   0        0        0      116 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/samples/actuarial_projection/
+-rw-rw-rw-   0        0        0        0 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/actuarial_projection/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/actuarial_projection/projection.py
+-rw-rw-rw-   0        0        0      649 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/dynamic_reference.py
+drwxrwxrwx   0        0        0        0 2020-08-08 16:47:49.000000 modelx-0.9.0/samples/netprem/
+-rw-rw-rw-   0        0        0      116 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/netprem/__init__.py
+-rw-rw-rw-   0        0        0      786 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/netprem/commutation_funcs.py
+-rw-rw-rw-   0        0        0      422 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/netprem/lifetable.py
+-rw-rw-rw-   0        0        0     1532 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/netprem/model.py
+-rw-rw-rw-   0        0        0      272 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/netprem/policy.py
+-rw-rw-rw-   0        0        0      656 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/sample_actuarialmodel.py
+-rw-rw-rw-   0        0        0      225 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/sample_all.py
+-rw-rw-rw-   0        0        0     1149 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/sample_firststep.py
+-rw-rw-rw-   0        0        0      324 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/sample_lifetable_decorator.py
+-rw-rw-rw-   0        0        0     1575 2019-10-13 15:26:22.000000 modelx-0.9.0/samples/sample_loan.py
+-rw-rw-rw-   0        0        0     1695 2019-07-29 02:41:56.000000 modelx-0.9.0/samples/sample_model.py
+-rw-rw-rw-   0        0        0      593 2019-08-07 11:52:59.000000 modelx-0.9.0/samples/sample_zero_bond.py
+-rw-rw-rw-   0        0        0       59 2020-08-08 16:47:49.000000 modelx-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     5682 2020-04-26 15:12:26.000000 modelx-0.9.0/setup.py
```

### Comparing `modelx-0.8.0/LICENSE.LESSER.txt` & `modelx-0.9.0/LICENSE.LESSER.txt`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/LICENSE.txt` & `modelx-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/PKG-INFO` & `modelx-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: modelx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Build and run complex models composed of formulas and data
 Home-page: https://github.com/fumitoh/modelx
 Author: Fumito Hamamura
 Author-email: fumito.ham@gmail.com
 License: LGPLv3
 Description: modelx
         ======
```

### Comparing `modelx-0.8.0/README.rst` & `modelx-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/__init__.py` & `modelx-0.9.0/modelx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Attributes:
     models (dict): Alias for :func:`get_models`.
         Available for Python 3.7 or newer
 
 """
 
-VERSION = (0, 8, 0)
+VERSION = (0, 9, 0)
 __version__ = ".".join([str(x) for x in VERSION])
 from modelx.core.api import *  # must come after __version__ assignment.
 try:
     from modelx.core.api import __getattr__, __dir__
 except ImportError:
     pass
 from modelx.qtgui.api import *
```

### Comparing `modelx-0.8.0/modelx/core/__init__.py` & `modelx-0.9.0/modelx/core/__init__.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/core/api.py` & `modelx-0.9.0/modelx/core/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     from modelx import *
 
 """
 import sys as _sys
 import ast as _ast
 import warnings
 from types import FunctionType as _FunctionType
+import zipfile
 
 from modelx.core import mxsys as _system
 from modelx.core.cells import CellsMaker as _CellsMaker
 from modelx.core.space import BaseSpace as _Space
 from modelx.core.model import Model as _Model
 from modelx.core.base import get_interfaces as _get_interfaces
 from modelx.core.util import is_valid_name as _is_valid_name
@@ -302,15 +303,15 @@
             _system.currentmodel.currentspace = _system.currentmodel.spaces[
                 space
             ]
 
         return cur_space()
 
 
-def restore_model(path, name=None):
+def restore_model(path, name=None, datapath=None):
     """Restore a model and return it.
 
     Restore a model saved by the :meth:`~modelx.core.model.Model.backup` method
     from ``path``.
 
     Args:
         path (:obj:`str`): Path to the file to restore the model from.
@@ -319,32 +320,32 @@
     Returns:
         A new model created from the file.
 
     See Also:
         :py:meth:`~modelx.core.model.Model.backup`
 
     """
-    return _system.restore_model(path, name)
+    return _system.restore_model(path, name, datapath)
 
 
-def open_model(path, name=None):
+def open_model(path, name=None, datapath=None):
     """Load a model saved from a file and return it.
 
     Args:
         path (:obj:`str`): Path to the file to load the model from.
         name (optional): If specified, the model is renamed to this name.
 
     Returns:
         A new model created from the file.
 
     .. deprecated:: 0.5.0 Use :func:`restore_model` instead.
     """
     warnings.warn(
         "'open_model' function is deprecated. Use 'restore_model' instead.")
-    return _system.restore_model(path, name)
+    return _system.restore_model(path, name, datapath)
 
 
 def start_stacktrace(maxlen=10000):
     """Activate stack tracing.
 
     Start tracing the call stack of formula calculations held internally
     in modelx.
@@ -498,39 +499,67 @@
 
     """
     return _serialize.write_model(
         _system, model, model_path, is_zip=False,
         backup=backup, log_input=log_input, version=version)
 
 
-def zip_model(model, model_path, backup=True, log_input=False, version=None):
+def zip_model(model, model_path, backup=True, log_input=False,
+              compression=zipfile.ZIP_DEFLATED, compresslevel=None,
+              version=None):
     """Archive model to a zip file
 
     Write ``model`` to a single zip file. The contents are the
     same as the directory tree output by the :func:`write_model` function.
 
+    .. versionchanged:: 0.9.0
+        ``compression`` and ``compresslevel`` parameters are added.
+
     .. versionadded:: 0.8.0
 
     Args:
         model: Model object to archive.
         model_path(str): Path to the zip file.
         backup(bool, optional): Whether to backup an existing file with
             the same name if it already exists. Defaults to ``True``.
         log_input(bool, optional): If ``True``, input values in Cells are
             output to *_input_log.txt* under ``model_path``. Defaults
             to ``False``.
+        compression(optional): Identifier of the ZIP compression method
+            to use. This method uses `zipfile.ZipFile`_ class internally
+            and ``compression`` and ``compresslevel`` arguments are
+            passed to `zipfile.ZipFile`_ constructor.
+            See `zipfile.ZipFile`_ manual page for available identifiers.
+            Defaults to `zipfile.ZIP_DEFLATED`_.
+        compresslevel(optional):
+            Integer identifier to indicate the compression level to use.
+            If not specified, the default compression level is used.
+            See `zipfile.ZipFile`_ explanation on the Python Standard
+            Library site for available integer identifiers for
+            each compression method.
+            For Python 3.6, this parameter is ignored.
+
         version(int, optional): Format version to write model.
             Defaults to the most recent version.
+            This parameter should be left unspecified in normal cases.
+
+    .. _zipfile.ZipFile:
+       https://docs.python.org/3/library/zipfile.html#zipfile.ZipFile
+
+    .. _zipfile.ZIP_DEFLATED:
+       https://docs.python.org/3/library/zipfile.html#zipfile.ZIP_DEFLATED
 
     See Also:
         :func:`write_model`
     """
     return _serialize.write_model(
         _system, model, model_path, is_zip=True,
-        backup=backup, log_input=log_input, version=version)
+        backup=backup, log_input=log_input,
+        compression=compression, compresslevel=compresslevel,
+        version=version)
 
 
 def read_model(model_path, name=None):
     """Read model from files.
 
     Read model form a folder(directory) tree or a zip file ``model_path``.
     The model must be saved either by :py:func:`~write_model`,
```

### Comparing `modelx-0.8.0/modelx/core/base.py` & `modelx-0.9.0/modelx/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     The rationales for splitting implementation from its interface are twofold,
     one is to hide from users attributes used only within the package,
     and the other is to free referring objects from getting affected by
     special methods that are meant for changing the behaviour of operations
     for users."""
 
     __cls_stateattrs = [
+        "system",
         "interface",
         "parent",
         "name",
         "model",
         "allow_none",
         "lazy_evals",
         "_doc"]
@@ -255,18 +256,14 @@
     def evalrepr(self):
         """Evaluable repr"""
         if self.is_model():
             return self.get_fullname()
         else:
             return self.parent.evalrepr + "." + self.name
 
-    def restore_state(self, system):
-        """Called after unpickling to restore some attributes manually."""
-        self.system = system
-
     def is_model(self):
         return self.parent is None
 
     def has_ascendant(self, other):
 
         if self.is_model():
             return False
@@ -277,14 +274,17 @@
 
     def has_descendant(self, other):
         return other.has_ascendant(self)
 
     def has_linealrel(self, other):
         return self.has_ascendant(other) or self.has_descendant(other)
 
+    def on_delete(self):
+        raise NotImplementedError
+
     # ----------------------------------------------------------------------
     # repr methods
 
     @property
     def doc(self):
         return self._doc
 
@@ -500,14 +500,16 @@
     def __reduce__(self):
         if self._impl.system.serializing:
 
             if self._impl.system.serializing.version == 2:
                 return self._reduce_serialize_2()
             elif self._impl.system.serializing.version == 3:
                 return self._reduce_serialize_3()
+            elif self._impl.system.serializing.version == 4:
+                return self._reduce_serialize_4()
             else:
                 raise ValueError("invalid serializer version")
         else:
             return object.__reduce__(self)
 
     def _reduce_serialize_2(self):
 
@@ -528,14 +530,16 @@
             # Replace model name with empty string
             tupleid = ("",) + self._tupleid[1:]
         else:
             tupleid = self._tupleid
 
         return _get_object_from_tupleid, (tupleid,)
 
+    _reduce_serialize_4 = _reduce_serialize_3
+
     def set_property(self, name: str, value):
         """Set property ``name``
 
         Set ``value`` to property ``name`` of an interface.
         Equivalent to ``x.name = value``,
         where x is a Model/Space/Cells object.
         """
```

### Comparing `modelx-0.8.0/modelx/core/cells.py` & `modelx-0.9.0/modelx/core/cells.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/core/chainmap.py` & `modelx-0.9.0/modelx/core/chainmap.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/core/errors.py` & `modelx-0.9.0/modelx/core/errors.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/core/formula.py` & `modelx-0.9.0/modelx/core/formula.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/core/model.py` & `modelx-0.9.0/modelx/core/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,27 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
 import builtins
 import itertools
-import pickle
-import copy
+import zipfile
 
 import networkx as nx
 
 from modelx.core.base import (
     add_stateattrs,
     Interface,
     Impl,
     get_interfaces,
-    ImplDict,
     ReferenceManager,
     ImplChainMap,
     BaseView,
-    Derivable,
-    NullImpl
+    Derivable
 )
 from modelx.core.reference import ReferenceImpl
 from modelx.core.cells import CellsImpl, UserCellsImpl
 from modelx.core.node import OBJ, KEY, get_node, node_has_key
 from modelx.core.spacecontainer import (
     BaseSpaceContainerImpl,
     EditableSpaceContainerImpl,
@@ -42,14 +39,15 @@
 from modelx.core.space import (
     UserSpaceImpl,
     SpaceDict,
     SpaceView,
     SharedRefDict
 )
 from modelx.core.util import is_valid_name, AutoNamer
+from modelx.io.baseio import DataClientReferenceManager
 
 _nxver = tuple(int(n) for n in nx.__version__.split(".")[:2])
 
 
 class TraceGraph(nx.DiGraph):
     """Directed Graph of ObjectArgs"""
 
@@ -133,43 +131,47 @@
     __slots__ = ()
 
     def rename(self, name, rename_old=False):
         """Rename the model itself"""
         self._impl.system.rename_model(
             new_name=name, old_name=self.name, rename_old=rename_old)
 
-    def save(self, filepath):
+    def save(self, filepath, datapath=None):
         """Back up the model to a file.
 
+        .. deprecated:: 0.9.0 Use :meth:`backup` instead.
+
         Alias for :meth:`backup`. See :meth:`backup` for details.
         """
-        self._impl.save(filepath)
+        self._impl.system.backup_model(self, filepath, datapath)
 
-    def backup(self, filepath):
+    def backup(self, filepath, datapath=None):
         """Back up the model to a file.
 
         Backup the model to a single binary file. This method internally
         utilizes Python's standard library,
         `pickle <https://docs.python.org/3/library/pickle.html>`_.
         This method should only be used for saving the model temporarily,
         as the saved model may not be restored by different
         versions of modelx, or when the Python environment changes,
         for example, due to package upgrade.
         Saving the model by :meth:`write` method is more robust.
 
+        .. versionchanged:: 0.9.0 ``datapath`` parameter is added.
         .. versionadded:: 0.7.0
 
         Args:
             filepath(str): file path
+            datapath(optional): Path to a folder to store internal files.
 
         See Also:
             :meth:`write`
             :func:`~modelx.restore_model`
         """
-        self._impl.save(filepath)
+        self._impl.system.backup_model(self, filepath, datapath)
 
     def close(self):
         """Close the model."""
         self._impl.close()
 
     @Interface.doc.setter
     def doc(self, value):
@@ -182,33 +184,68 @@
         on self. See :py:func:`~modelx.write_model` section for the details.
 
         .. versionchanged:: 0.8.0
         .. versionadded:: 0.0.22
 
         Args:
             model_path(str): Folder(directory) path where the model is saved.
+            backup(bool, optional): Whether to backup an existing file with
+                the same name if it already exists. Defaults to ``True``.
+            log_input(bool, optional): If ``True``, input values in Cells are
+                output to *_input_log.txt* under ``model_path``. Defaults
+                to ``False``.
         """
         from modelx.serialize import write_model
         write_model(self._impl.system, self, model_path, is_zip=False,
                     backup=backup, log_input=log_input)
 
-    def zip(self, model_path, backup=True, log_input=False):
+    def zip(self, model_path, backup=True, log_input=False,
+            compression=zipfile.ZIP_DEFLATED, compresslevel=None):
         """Archive model to a zip file.
 
         This method performs the :py:func:`~modelx.zip_model`
         on self. See :py:func:`~modelx.zip_model` section for the details.
 
+        .. versionchanged:: 0.9.0
+            ``compression`` and ``compresslevel`` parameters are added.
+
         .. versionadded:: 0.8.0
 
         Args:
             model_path(str): Folder(directory) path where the model is saved.
+            backup(bool, optional): Whether to backup an existing file with
+                the same name if it already exists. Defaults to ``True``.
+            log_input(bool, optional): If ``True``, input values in Cells are
+                output to *_input_log.txt* under ``model_path``. Defaults
+                to ``False``.
+            compression(optional): Identifier of the ZIP compression method
+                to use. This method uses `zipfile.ZipFile`_ class internally
+                and ``compression`` and ``compresslevel`` arguments are
+                passed to `zipfile.ZipFile`_ constructor.
+                See `zipfile.ZipFile`_ manual page for available identifiers.
+                Defaults to `zipfile.ZIP_DEFLATED`_.
+            compresslevel(optional):
+                Integer identifier to indicate the compression level to use.
+                If not specified, the default compression level is used.
+                See `zipfile.ZipFile`_ explanation on the Python Standard
+                Library site for available integer identifiers for
+                each compression method.
+                For Python 3.6, this parameter is ignored.
+
+        .. _zipfile.ZipFile:
+           https://docs.python.org/3/library/zipfile.html#zipfile.ZipFile
+
+        .. _zipfile.ZIP_DEFLATED:
+           https://docs.python.org/3/library/zipfile.html#zipfile.ZIP_DEFLATED
+
         """
         from modelx.serialize import write_model
         write_model(self._impl.system, self, model_path, is_zip=True,
-                    backup=backup, log_input=log_input)
+                    backup=backup, log_input=log_input,
+                    compression=compression, compresslevel=compresslevel)
 
     # ----------------------------------------------------------------------
     # Getting and setting attributes
 
     def __getattr__(self, name):
         return self._impl.get_attr(name)
 
@@ -221,14 +258,38 @@
     def __delattr__(self, name):
         self._impl.del_attr(name)
 
     def __dir__(self):
         return self._impl.namespace.interfaces
 
     @property
+    def dataclients(self):
+        """List of :class:`~modelx.io.baseio.BaseDataClient` objects
+
+        Returns a list of objects of BaseDataClient sub-classes
+        that are associated to this Model.
+
+        :class:`~modelx.io.excelio.ExcelRange`
+        is a sub class of :class:`~modelx.io.baseio.BaseDataClient`, and
+        :class:`~modelx.io.excelio.ExcelRange`
+        objects created by
+        :meth:`Model.new_excel_range<modelx.core.model.Model.new_excel_range>`
+        or
+        :meth:`UserSpace.new_excel_range<modelx.core.space.UserSpace.new_excel_range>`
+        methods of this Model
+        are included in the returned list.
+
+        See Also:
+
+            :meth:`UserSpace.new_excel_range<modelx.core.space.UserSpace.new_excel_range>`
+            :meth:`Model.new_excel_range<modelx.core.model.Model.new_excel_range>`
+        """
+        return list(self._impl.datarefmgr.clients)
+
+    @property
     def tracegraph(self):
         """A directed graph of cells."""
         return self._impl.tracegraph
 
     @property
     def refs(self):
         """Return a mapping of global references."""
@@ -283,15 +344,16 @@
     __cls_stateattrs = [
             "_namespace",
             "_global_refs",
             "_dynamic_bases",
             "_dynamic_bases_inverse",
             "_dynamic_base_namer",
             "spacemgr",
-            "currentspace"
+            "currentspace",
+            "datarefmgr"
     ]
 
     def __init__(self, *, system, name):
 
         if not name:
             name = system._modelnamer.get_next(system.models)
         elif not is_valid_name(name):
@@ -314,14 +376,15 @@
         self._dynamic_bases_inverse = {}
         self._dynamic_base_namer = AutoNamer("__Space")
         self._namespace = ImplChainMap(
             self, BaseView, [self._named_spaces, self._global_refs]
         )
         self.allow_none = False
         self.lazy_evals = self._namespace
+        self.datarefmgr = DataClientReferenceManager()
 
     def rename(self, name):
         """Rename self. Must be called only by its system."""
         if is_valid_name(name):
             if name not in self.system.models:
                 self.name = name
                 return True  # Rename success
@@ -347,19 +410,14 @@
     @property
     def namespace(self):
         return self._namespace.fresh
 
     def close(self):
         self.system.close_model(self)
 
-    def save(self, filepath):
-        self.update_lazyevals()
-        with open(filepath, "wb") as file:
-            pickle.dump(self.interface, file, protocol=4)
-
     def get_impl_from_name(self, name):
         """Retrieve an object by a dotted name relative to the model."""
         parts = name.split(".")
         space = self.spaces[parts.pop(0)]
         if parts:
             return space.get_impl_from_name(".".join(parts))
         else:
@@ -393,18 +451,22 @@
             state[gname] = nx.relabel_nodes(graph, mapping)
 
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
-    def restore_state(self, system):
+    def restore_state(self, datapath=None):
         """Called after unpickling to restore some attributes manually."""
-        Impl.restore_state(self, system)
-        BaseSpaceContainerImpl.restore_state(self, system)
+        BaseSpaceContainerImpl.restore_state(self)
+
+        for client in self.datarefmgr.clients:
+            self.system.iomanager.register_client(
+                client, model=self.interface, datapath=datapath)
+
         mapping = {}
         for node in self.tracegraph:
             if isinstance(node, tuple):
                 name, key = node
             else:
                 name, key = node, None
             cells = self.get_impl_from_name(name)
@@ -415,14 +477,15 @@
     def del_space(self, name):
         space = self.spaces[name]
         self.spacemgr.del_defined_space(self, name)
         if space is self.currentspace:
             self.currentspace = None
 
     def del_ref(self, name):
+        self.global_refs[name].on_delete()
         self.global_refs.del_item(name)
 
     def change_ref(self, name, value):
         ref = self.global_refs[name]
         ref.change_value(value, False)
         self.model.clear_attr_referrers(ref)
```

### Comparing `modelx-0.8.0/modelx/core/node.py` & `modelx-0.9.0/modelx/core/node.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/core/reference.py` & `modelx-0.9.0/modelx/core/reference.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 import builtins
 import importlib
 from types import ModuleType, FunctionType
 import functools
 
 from modelx.core.base import add_stateattrs, Derivable, Impl, Interface
+from modelx.io.excelio import BaseDataClient
 
 
 # For backward compatibility with -v0.0.23
 class _DummyBuiltins:
     pass
 
 
@@ -76,25 +77,36 @@
             self,
             system=parent.system,
             parent=parent,
             name=name,
             interface=value)
         Derivable.__init__(self, is_derived)
 
+        if isinstance(value, BaseDataClient):
+            self.model.datarefmgr.add_reference(self, value)
+
         self.container = container
         container.set_item(name, self)
 
     def change_value(self, value, is_derived):
         if not is_derived:
             self.set_defined()
+        if isinstance(self.interface, BaseDataClient):
+            self.model.datarefmgr.del_reference(self, self.interface)
+        if isinstance(value, BaseDataClient):
+            self.model.datarefmgr.add_reference(self, value)
         self.interface = value
         self.container.set_update()
         for sc in self.container.scopes:
             sc.clear_referrers(self.name)
 
+    def on_delete(self):
+        if isinstance(self.interface, BaseDataClient):
+            self.model.datarefmgr.del_reference(self, self.interface)
+
     def __getstate__(self):
         state = {
             key: value
             for key, value in self.__dict__.items()
             if key in self.stateattrs
         }
         value = state["interface"]
```

### Comparing `modelx-0.8.0/modelx/core/space.py` & `modelx-0.9.0/modelx/core/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1201,21 +1201,17 @@
             if key in self.stateattrs
         }
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
-    def restore_state(self, system):
+    def restore_state(self):
         """Called after unpickling to restore some attributes manually."""
-        Impl.restore_state(self, system)
-        BaseSpaceContainerImpl.restore_state(self, system)
-
-        for cells in self._cells.values():
-            cells.restore_state(system)
+        BaseSpaceContainerImpl.restore_state(self)
 
     # ----------------------------------------------------------------------
     # Pandas, Module, Excel I/O
 
     def to_frame(self, args):
         return _to_frame_inner(self.cells, args)
 
@@ -1381,15 +1377,15 @@
             param_order: a sequence of integers representing
                 the order of params and extra_params.
             transpose: in which direction 'vertical' or 'horizontal'
             names_col: a string or a list of names of the extra params.
             param_rows: integer or string expression, or a sequence of them
                 indicating row (or column) to be interpreted as parameters.
         """
-        import modelx.io.excel as xl
+        import modelx.io.excel_legacy as xl
 
         cellstable = xl.CellsTable(
             book,
             range_,
             sheet,
             names_row,
             param_cols,
@@ -1655,14 +1651,15 @@
 
     def on_create_ref(self, name, value, is_derived):
         return ReferenceImpl(self, name, value,
                       container=self._self_refs,
                       is_derived=is_derived)
 
     def on_del_ref(self, name):
+        self.self_refs[name].on_delete()
         self.self_refs.del_item(name)
 
 
 class DynamicSpace(BaseSpace):
     """Dynamically created space.
 
     Dynamic spaces of a parametric space
@@ -1829,17 +1826,17 @@
         return refs
 
     def _bind_args(self, args):
         self.boundargs = self.parent.formula.signature.bind(**args)
         self.argvalues = tuple(self.boundargs.arguments.values())
         self.argvalues_if = tuple(get_interfaces(self.argvalues))
 
-    def restore_state(self, system):
+    def restore_state(self):
 
-        super().restore_state(system)
+        super().restore_state()
 
         # From Python 3.5, signature is pickable,
         # pickling logic involving signature may be simplified.
         self._bind_args(self._arguments)
 
     @property
     def _baseattrs(self):
```

### Comparing `modelx-0.8.0/modelx/core/system.py` & `modelx-0.9.0/modelx/core/system.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 import sys
 import time
 import os.path
 import warnings
 import pickle
 import threading
 import traceback
+import pathlib
 from collections import deque
 import modelx   # https://bugs.python.org/issue18145
 from modelx.core.node import get_node_repr
 from modelx.core.model import ModelImpl
 from modelx.core.util import AutoNamer, is_valid_name
 from modelx.core.errors import DeepReferenceError, FormulaError
 from modelx.core.node import OBJ, KEY, Element
+from modelx.io.baseio import IOManager, BaseSharedData
 
 
 class Executor:
 
     def __init__(self, system, maxdepth=None):
 
         # Use thread to increase stack size and deepen callstack
@@ -343,14 +345,51 @@
     try:
         __IPYTHON__
         return True
     except NameError:
         return False
 
 
+class SystemPickler(pickle.Pickler):
+
+    def __init__(self, file, datapath=None, **kwargs):
+        super().__init__(file, **kwargs)
+        self.datapath = pathlib.Path(datapath) if datapath else None
+
+    def persistent_id(self, obj):
+
+        if isinstance(obj, System):
+            return "System", None
+        elif isinstance(obj, IOManager):
+            return "IOManager", None
+        elif isinstance(obj, BaseSharedData):
+            obj.save(self.datapath)
+            return "BaseSharedData", None
+        else:
+            return None
+
+
+class SystemUnpickler(pickle.Unpickler):
+
+    def __init__(self, file, system):
+        super().__init__(file)
+        self.system = system
+
+    def persistent_load(self, pid):
+
+        if pid[0] == "System":
+            return self.system
+        elif pid[0] == "IOManager":
+            return self.system.iomanager
+        elif pid[0] == "BaseSharedData":
+            return None
+        else:
+            raise pickle.UnpicklingError("unsupported persistent object")
+
+
 class System:
 
     orig_settings = {
         "sys.recursionlimit": sys.getrecursionlimit(),
         "showwarning": warnings.showwarning
     }
 
@@ -374,14 +413,16 @@
                 self.setup_ipython()
             else:
                 self.shell = None
                 self.is_ipysetup = False
         else:
             self.is_ipysetup = False
 
+        self.iomanager = IOManager(self)
+
     def setup_ipython(self):
         """Monkey patch shell's error handler.
 
         This method is to monkey-patch the showtraceback method of
         IPython's InteractiveShell to
 
         __IPYTHON__ is not detected when starting an IPython kernel,
@@ -492,19 +533,24 @@
             if self.currentmodel:
                 m = self.currentmodel
             else:
                 m = self.new_model()    # self.new_model sets current_model
             m.currentspace = m.spacemgr.new_space(m)
             return m.currentspace
 
-    def restore_model(self, path, name):
+    def backup_model(self, model, filepath, datapath):
+        model._impl.update_lazyevals()
+        with open(filepath, "wb") as file:
+            SystemPickler(file, datapath, protocol=4).dump(model)
+
+    def restore_model(self, path, name, datapath):
         with open(path, "rb") as file:
-            model = pickle.load(file)
+            model = SystemUnpickler(file, self).load()
 
-        model._impl.restore_state(self)
+        model._impl.restore_state(datapath)
 
         if name is not None:
             if not is_valid_name(name):
                 raise ValueError("Invalid name '%s'." % name)
 
         newname = name or model.name
 
@@ -520,14 +566,15 @@
 
         return model
 
     def close_model(self, model):
         del self.models[model.name]
         if self.currentmodel is model:
             self.currentmodel = None
+        model.datarefmgr.del_all()
 
     def get_object(self, name, as_proxy=False):
         """Retrieve an object by its absolute name."""
 
         parts = name.split(".")
         try:
             model = self.models[parts.pop(0)].interface
@@ -600,14 +647,17 @@
 
     def clear_stacktrace(self):
         if self._is_stacktrace_active():
             self.callstack.tracestack.clear()
         else:
             raise RuntimeError("call stack trace not active")
 
+    def _check_sanity(self):
+        self.iomanager._check_sanity()
+
 
 mxsys = System()
 
 
 # --------------------------------------------------------------------------
 # Monkey patch functions for custom error messages
```

### Comparing `modelx-0.8.0/modelx/core/util.py` & `modelx-0.9.0/modelx/core/util.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/io/excel.py` & `modelx-0.9.0/modelx/io/excel_legacy.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,103 +8,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
-import re
-import string
+
 import itertools
 from collections import namedtuple
-
 import openpyxl as opxl
-
-
-def _get_col_index(name):
-    """Convert column name to index."""
-
-    index = string.ascii_uppercase.index
-    col = 0
-    for c in name.upper():
-        col = col * 26 + index(c) + 1
-    return col
-
-
-def _is_range_address(range_addr):
-
-    # RANGE_EXPR modified from openpyxl.utils.cells
-    # see https://bitbucket.org/openpyxl/openpyxl
-
-    RANGE_EXPR = """
-    (?P<cells>
-    [$]?(?P<min_col>[A-Za-z]{1,3})?
-    [$]?(?P<min_row>\d+)?
-    (:[$]?(?P<max_col>[A-Za-z]{1,3})?
-    [$]?(?P<max_row>\d+)?)?
-    )$
-    """
-    RANGE_EXPR_RE = re.compile(RANGE_EXPR, re.VERBOSE)
-
-    match = RANGE_EXPR_RE.match(range_addr)
-
-    if not match:
-        return False
-    else:
-        cells = match.group("cells")
-
-    if not cells:
-        return False
-    else:
-        min_col = _get_col_index(match.group("min_col"))
-        min_row = int(match.group("min_row"))
-
-        # if range_addr is for a single cell,
-        # max_col and max_row are None.
-        max_col = match.group("max_col")
-        max_col = max_col and _get_col_index(max_col)
-
-        max_row = match.group("max_row")
-        max_row = max_row and int(max_row)
-
-        if max_col and max_row:
-            return (
-                (min_col <= max_col)
-                and (min_row <= max_row)
-                and (max_col <= 16384)
-                and (max_row <= 1048576)
-            )
-        else:
-            return (min_col <= 16384) and (min_row <= 1048576)
-
-
-def _get_range(book, range_, sheet):
-    """Return a range as nested dict of openpyxl cells."""
-
-    filename = None
-    if isinstance(book, str):
-        filename = book
-        book = opxl.load_workbook(book, data_only=True)
-    elif isinstance(book, opxl.Workbook):
-        pass
-    else:
-        raise TypeError
-
-    if _is_range_address(range_):
-        sheet_names = [name.upper() for name in book.sheetnames]
-        index = sheet_names.index(sheet.upper())
-        data = book.worksheets[index][range_]
-    else:
-        data = _get_namedrange(book, range_, sheet)
-        if data is None:
-            raise ValueError(
-                "Named range '%s' not found in %s" % (range_, filename or book)
-            )
-
-    return data
+from .excelio import _is_range_address, _get_namedrange, _get_range
 
 
 def read_range(filepath, range_expr, sheet=None, dict_generator=None):
     """Read values from an Excel range into a dictionary.
 
     `range_expr` ie either a range address string, such as "A1", "$C$3:$E$5",
     or a defined name string for a range, such as "NamedRange1".
@@ -154,95 +70,14 @@
     if dict_generator is None:
         dict_generator = default_generator
 
     gen = dict_generator(cells)
     return {keyval[0]: keyval[1] for keyval in gen}
 
 
-def _get_namedrange(book, rangename, sheetname=None):
-    """Get range from a workbook.
-
-    A workbook can contain multiple definitions for a single name,
-    as a name can be defined for the entire book or for
-    a particular sheet.
-
-    If sheet is None, the book-wide def is searched,
-    otherwise sheet-local def is looked up.
-
-    Args:
-        book: An openpyxl workbook object.
-        rangename (str): Range expression, such as "A1", "$G4:$K10",
-            named range "NamedRange1".
-        sheetname (str, optional): None for book-wide name def,
-            sheet name for sheet-local named range.
-
-    Returns:
-        Range object specified by the name.
-
-    """
-
-    def cond(namedef):
-
-        if namedef.type.upper() == "RANGE":
-            if namedef.name.upper() == rangename.upper():
-
-                if sheetname is None:
-                    if not namedef.localSheetId:
-                        return True
-
-                else:  # sheet local name
-                    sheet_id = [sht.upper() for sht in book.sheetnames].index(
-                        sheetname.upper()
-                    )
-
-                    if namedef.localSheetId == sheet_id:
-                        return True
-
-        return False
-
-    def get_destinations(name_def):
-        """Workaround for the bug in DefinedName.destinations"""
-
-        from openpyxl.formula import Tokenizer
-        from openpyxl.utils.cell import SHEETRANGE_RE
-
-        if name_def.type == "RANGE":
-            tok = Tokenizer("=" + name_def.value)
-            for part in tok.items:
-                if part.subtype == "RANGE":
-                    m = SHEETRANGE_RE.match(part.value)
-                    if m.group("quoted"):
-                        sheet_name = m.group("quoted")
-                    else:
-                        sheet_name = m.group("notquoted")
-
-                    yield sheet_name, m.group("cells")
-
-    namedef = next(
-        (item for item in book.defined_names.definedName if cond(item)), None
-    )
-
-    if namedef is None:
-        return None
-
-    dests = get_destinations(namedef)
-    xlranges = []
-
-    sheetnames_upper = [name.upper() for name in book.sheetnames]
-
-    for sht, addr in dests:
-        if sheetname:
-            sht = sheetname
-        index = sheetnames_upper.index(sht.upper())
-        xlranges.append(book.worksheets[index][addr])
-
-    if len(xlranges) == 1:
-        return xlranges[0]
-    else:
-        return xlranges
 
 
 _IndexRange = namedtuple("_IndexRange", ["begin", "len", "skip"])
 
 
 class _CellsOrientation:
     ROW = 1
```

### Comparing `modelx-0.8.0/modelx/io/pandas.py` & `modelx-0.9.0/modelx/io/pandas.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/qtgui/api.py` & `modelx-0.9.0/modelx/qtgui/api.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/qtgui/modeltree.py` & `modelx-0.9.0/modelx/qtgui/modeltree.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/serialize/__init__.py` & `modelx-0.9.0/modelx/serialize/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pathlib
 import importlib
 import shutil
 import json
+import zipfile
 from . import ziputil
 
 
 _MX_TO_FORMAT = {
     (0, 0, 25): 1,
     (0, 1, 0): 2,
-    (0, 2, 0): 3
+    (0, 2, 0): 3,
+    (0, 9, 0): 4
 }
 
 HIGHEST_VERSION = list(_MX_TO_FORMAT.values())[-1]
 DEFAULT_MAX_BACKUPS = 3
 
 
 def _get_serializer(version):
@@ -84,28 +86,35 @@
     except KeyError:
         return _get_serializer(1)
 
     return _get_serializer(params["serializer_version"])
 
 
 def write_model(system, model, model_path,
-                is_zip, backup=True, log_input=False, version=None):
+                is_zip, backup=True, log_input=False,
+                compression=zipfile.ZIP_DEFLATED,
+                compresslevel=None,
+                version=None):
 
     version = version or HIGHEST_VERSION
     max_backups = DEFAULT_MAX_BACKUPS if backup else 0
 
     root = pathlib.Path(model_path)
     _increment_backups(model, root, max_backups)
 
-    ziputil.make_root(root, is_zip)
+    ziputil.make_root(root, is_zip, compression, compresslevel)
     ziputil.write_str(json.dumps({"serializer_version": version}),
-                      root / "_system.json")
+                      root / "_system.json",
+                      compression=compression,
+                      compresslevel=compresslevel)
 
     serializer = _get_serializer(version)
-    serializer.ModelWriter(system, model, root, log_input=log_input
+    serializer.ModelWriter(system, model, root, log_input=log_input,
+                           compression=compression,
+                           compresslevel=compresslevel
                            ).write_model()
 
     return model
 
 
 def read_model(system, model_path, name=None):
     kwargs = {"name": name} if name else {}
```

### Comparing `modelx-0.8.0/modelx/serialize/jsonvalues.py` & `modelx-0.9.0/modelx/serialize/jsonvalues.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/serialize/serializer_1.py` & `modelx-0.9.0/modelx/serialize/serializer_1.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/serialize/serializer_2.py` & `modelx-0.9.0/modelx/serialize/serializer_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,17 @@
 class ModelWriter:
 
     version = 2
     model_encoder = None
     space_encoder = None
 
     def __init__(self, system, model: Model, path: pathlib.Path,
-                 log_input: bool):
+                 log_input: bool,
+                 compression=None, compresslevel=None
+                 ):
 
         self.system = system
         self.model = model
         self.root = path
         self.call_ids = []
         self.pickledata = {}
         self.method_encoders = []
@@ -248,26 +250,26 @@
                 self.root / "_model.py",
                 self.root / "data")
 
             self._write_recursive(encoder)
             self.write_pickledata()
 
             if self.log_input:
-                ziputil.write_str(
+                ziputil.write_str_utf8(
                     "\n".join(self.input_log),
                     self.root / "_input_log.txt"
                 )
 
         finally:
             self.system.serializing = None
             self.call_ids.clear()
 
     def _write_recursive(self, encoder):
 
-        ziputil.write_str(encoder.encode(), encoder.srcpath)
+        ziputil.write_str_utf8(encoder.encode(), encoder.srcpath)
 
         for space in encoder.target.spaces.values():
 
             if not MethodCallEncoder.from_method(space):
                 if isinstance(encoder.target, Model):
                     srcpath = encoder.srcpath.parent / (space.name + ".py")
                 else:
@@ -282,15 +284,15 @@
                 self._write_recursive(e)
 
         encoder.instruct().execute()
 
     def write_pickledata(self):
         if self.pickledata:
             file = self.root / "data/data.pickle"
-            ziputil.write_file(
+            ziputil.write_file_utf8(
                 lambda f: pickle.dump(self.pickledata, f), file, mode="b")
 
 
 class BaseEncoder:
 
     def __init__(self, writer, target,
                  parent=None, name=None, srcpath=None, datapath=None):
@@ -598,15 +600,15 @@
 
         if cellsdata:   # Save IDs
 
             def write_dataid(f):
                 for keyid, valid in cellsdata:
                     f.write("(%s, %s)\n" % (keyid, valid))
 
-            ziputil.write_file(write_dataid, self.datapath, "t")
+            ziputil.write_file_utf8(write_dataid, self.datapath, "t")
 
     def instruct(self):
         return Instruction(self.pickle_value)
 
 
 class MethodCallEncoder(BaseEncoder):
 
@@ -772,15 +774,15 @@
 
     @classmethod
     def condition(cls, target):
         return True  # default encoder
 
     def pickle_value(self, path: pathlib.Path, value):
         key = id(value)
-        ziputil.write_str(str(key), path)
+        ziputil.write_str_utf8(str(key), path)
         if key not in self.writer.pickledata:
             self.writer.pickledata[key] = value
 
     def encode(self):
         data = self.datapath.relative_to(self.srcpath.parent).as_posix()
         return "(\"Pickle\", \"%s\")" % data
 
@@ -898,15 +900,15 @@
         return target
 
     def _parse_dynamic_inputs(self, path_):
         pass
 
     def parse_source(self, path_, obj: Interface):
 
-        src = ziputil.read_str(path_)
+        src = ziputil.read_str_utf8(path_)
         srcstructure = SourceStructure(src)
         atok = asttokens.ASTTokens(src, parse=True)
 
         for i, stmt in enumerate(atok.tree.body):
             sec = srcstructure.get_section(stmt.lineno)
             parser = self.parser_selector_class.select(stmt, sec, atok)(
                 stmt, atok, self, sec, obj, srcpath=path_
@@ -916,15 +918,15 @@
                 ist.execute()
             else:
                 self.instructions.append(ist)
 
     def read_pickledata(self):
         file = self.path / "data/data.pickle"
         if ziputil.exists(file):
-            self.pickledata = ziputil.read_file(pickle.load, file, "b")
+            self.pickledata = ziputil.read_file_utf8(pickle.load, file, "b")
 
 
 class BaseNodeParser:
     AST_NODE = None
     default_priority = PriorityID.NORMAL
 
     def __init__(self, node, atok, reader, section, obj, srcpath, **kwargs):
@@ -1230,15 +1232,15 @@
         cells = self.impl.cells[self.cellsname]
         for key, val in data.items():
             cells.set_value(key, val)
 
     def load_pickledata(self):
         if ziputil.exists(self.datapath):
             data = {}
-            lines = ziputil.read_file(lambda f: f.readlines(),
+            lines = ziputil.read_file_utf8(lambda f: f.readlines(),
                                       self.datapath,
                                       "t")
             for line in lines:
                 keyid, valid = ast.literal_eval(line)
                 key = self.reader.pickledata[keyid]
                 val = self.reader.pickledata[valid]
                 data[key] = val
@@ -1394,15 +1396,16 @@
 class PickleDecoder(TupleDecoder):
     DECTYPE = "Pickle"
 
     def decode(self):
         return self.srcpath.parent / self.elm(1)
 
     def restore(self):
-        key = ziputil.read_file(lambda f: int(f.read()), self.decode(), "t")
+        key = ziputil.read_file_utf8(
+            lambda f: int(f.read()), self.decode(), "t")
 
         return self.reader.pickledata[key]
 
 
 class LiteralDecoder(ValueDecoder):
 
     @classmethod
```

### Comparing `modelx-0.8.0/modelx/serialize/serializer_3.py` & `modelx-0.9.0/modelx/serialize/serializer_3.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         if self.space._named_itemspaces:
 
             def callback(f):
                 for s in self.space._named_itemspaces.values():
                     self._pickle_dynamic_space(f, s)
 
-            ziputil.write_file(callback, datafile, "t")
+            ziputil.write_file_utf8(callback, datafile, "t")
 
     def _pickle_dynamic_space(self, file, space):
 
         for cells in space.cells.values():
             for key in cells._impl.input_keys:
                 value = cells._impl.data[key]
                 keyid = id(key)
@@ -219,20 +219,21 @@
 
 # --------------------------------------------------------------------------
 # Model Reading
 
 
 class ModelReader(ModelReader2):
 
+    version = ModelWriter.version
     def _parse_dynamic_inputs(self, path_):
 
         file = path_ / "data/_dynamic_inputs"
         if ziputil.exists(file):
 
-            lines = ziputil.read_file(
+            lines = ziputil.read_file_utf8(
                 lambda f: f.readlines(),
                 file,
                 "t"
             )
 
             instructuions = []
             for line in lines:
```

### Comparing `modelx-0.8.0/modelx/serialize/ziputil.py` & `modelx-0.9.0/modelx/serialize/ziputil.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library.  If not, see <http://www.gnu.org/licenses/>.
 
+import sys
 import pathlib
 import zipfile
 import tempfile
 import io
 import shutil
 import locale
 import os
@@ -28,17 +29,33 @@
 
 def make_parent_dir(path: pathlib.Path):
 
     if not path.parent.exists():
         path.parent.mkdir(parents=True, exist_ok=True)
 
 
-def make_root(root: pathlib.Path, is_zip: bool):
+def _compress_kwargs(compression, compresslevel):
+
+    kwargs = dict(
+        compression=compression,
+        compresslevel=compresslevel)
+
+    if sys.version_info[:2] <= (3, 6):
+        kwargs.pop("compresslevel")
+
+    return kwargs
+
+
+def make_root(root: pathlib.Path, is_zip: bool,
+              compression=None,
+              compresslevel=None):
     if is_zip:
-        with zipfile.ZipFile(root, "w"):
+
+        with zipfile.ZipFile(root, "w",
+                             **_compress_kwargs(compression, compresslevel)):
             pass
     else:
         root.mkdir(parents=True, exist_ok=True)
 
 
 def find_zip_parent(path: pathlib.Path):
     """Return path to parent zip file.
@@ -130,48 +147,64 @@
         if name.split("/") == archive.split("/")[-1]:
             return False
 
     return True
 
 
 def write_str(string: str, path: pathlib.Path,
-                 encoding=None, newline=None):
+              encoding=None, newline=None,
+              compression=None,
+              compresslevel=None):
     """Write string into a file under a directory or in a zip file."""
 
     write_file(lambda f: f.write(string), path, mode="t",
-                 encoding=encoding, newline=newline)
+                encoding=encoding, newline=newline,
+                **_compress_kwargs(compression, compresslevel))
+
 
+def write_str_utf8(string: str, path: pathlib.Path, newline=None,
+                   compression=None,
+                   compresslevel=None):
 
-def write_str_utf8(string: str, path: pathlib.Path):
-    write_str(string, path, encoding="utf-8", newline="\n")
+    write_str(string, path, encoding="utf-8", newline=newline,
+              **_compress_kwargs(compression, compresslevel)
+              )
 
 
-def pandas_to_pickle(obj, path: pathlib.Path):
+def pandas_to_pickle(obj, path: pathlib.Path,
+                     compression=None,
+                     compresslevel=None):
 
     root = find_zip_parent(path)
 
     if root:
         with tempfile.TemporaryDirectory() as dirname:
             filepath = str(pathlib.Path(dirname).joinpath("temp"))
             obj.to_pickle(filepath)
             archive = get_archive_path(path, root)
-            with zipfile.ZipFile(root, mode="a") as f:
+            with zipfile.ZipFile(
+                    root,
+                    mode="a",
+                    **_compress_kwargs(compression, compresslevel)
+                    ) as f:
                 if not _archive_exists(archive, f):
                     if is_valid_archive_path(archive, f):
                         f.write(filepath, archive)
                     else:
                         raise ValueError("invalid archive '%s'" % archive)
 
     else:
         make_parent_dir(path)
         obj.to_pickle(str(path))
 
 
 def write_file(callback, path: pathlib.Path, mode,
-                 encoding=None, newline=None):
+               encoding=None, newline=None,
+               compression=None,
+               compresslevel=None):
 
     if mode == "b":
         def encode(b): return b
     elif mode == "t":
         encoding = encoding or locale.getpreferredencoding()
         def encode(s): return s.encode(encoding)
     else:
@@ -190,41 +223,55 @@
             return path.open("wt", encoding=encoding, newline=newline)
 
     root = find_zip_parent(path)
 
     if root:
         archive = get_archive_path(path, root)
         with get_io(mode) as buff:
-            with zipfile.ZipFile(root, mode="a") as f:
+            with zipfile.ZipFile(
+                    root, mode="a",
+                    **_compress_kwargs(compression, compresslevel)
+            ) as f:
                 if not _archive_exists(archive, f):
                     if is_valid_archive_path(archive, f):
                         callback(buff)
                         buff.seek(0)
                         f.writestr(archive, encode(buff.read()))
                     else:
                         raise ValueError("invalid archive '%s'" % archive)
 
     else:
         make_parent_dir(path)
         with open_path(mode) as f:
             callback(f)
 
 
-def copy_file(src, dst):
+def write_file_utf8(callback, path: pathlib.Path, mode, newline=None,
+                    compression=None,
+                    compresslevel=None):
+    return write_file(callback, path, mode, encoding="utf-8", newline=newline,
+                      **_compress_kwargs(compression, compresslevel))
+
+
+def copy_file(src: pathlib.Path, dst: pathlib.Path,
+              compression=None, compresslevel=None):
 
     root_src = find_zip_parent(src)
     root_dst = find_zip_parent(dst)
 
     if root_src and root_dst:
 
         arc_src = get_archive_path(src, root_src)
         arc_dst = get_archive_path(dst, root_dst)
         with zipfile.ZipFile(root_src, mode="r") as zip_src:
             with zip_src.open(arc_src, mode="r") as f_src:
-                with zipfile.ZipFile(root_dst, mode="a") as zip_dst:
+                with zipfile.ZipFile(
+                        root_dst, mode="a",
+                        **_compress_kwargs(compression, compresslevel)
+                        ) as zip_dst:
                     if not _archive_exists(arc_dst, zip_dst):
                         if is_valid_archive_path(arc_dst, zip_dst):
                             zip_dst.writestr(arc_dst, f_src.read())
                         else:
                             raise ValueError("invalid archive '%s'" % arc_dst)
 
     elif root_src and not root_dst:
@@ -238,36 +285,56 @@
                     str(pathlib.Path(dirname) / arc_src),
                     str(pathlib.Path(dst))
                 )
 
     elif not root_src and root_dst:
 
         arc_dst = get_archive_path(dst, root_dst)
-        with zipfile.ZipFile(root_dst, mode="a") as zip_dst:
+        with zipfile.ZipFile(root_dst, mode="a",
+                             **_compress_kwargs(compression, compresslevel)
+                             ) as zip_dst:
             if not _archive_exists(arc_dst, zip_dst):
                 if is_valid_archive_path(arc_dst, zip_dst):
                     zip_dst.write(src, arc_dst)
                 else:
                     raise ValueError("invalid archive '%s'" % arc_dst)
 
     elif not root_src and not root_dst:
         shutil.copyfile(str(src), str(dst))
 
     else:
         raise RuntimeError("must not happen")
 
 
+def copy_dir_to_zip(src: pathlib.Path, dest: pathlib.Path,
+                    compression, compresslevel):
+    """Copy directory tree into a zip file
+
+    Arg:
+        src: path-like object pointing to a directory
+        dest: path pointing to a zip file
+    """
+    src = src.resolve()
+    for d, _, files in os.walk(src):
+        for f in files:
+            srcfile = pathlib.Path(os.path.join(d, f))
+            rel = srcfile.relative_to(src)
+            destfile = dest.joinpath(rel)
+            copy_file(srcfile, destfile,
+                      **_compress_kwargs(compression, compresslevel))
+
+
 def read_str(path: pathlib.Path, encoding=None, newline=None):
 
     return read_file(
         lambda f: f.read(), path, "t", encoding=encoding, newline=newline)
 
 
-def read_str_utf8(path: pathlib.Path):
-    return read_str(path, encoding="utf-8", newline="\n")
+def read_str_utf8(path: pathlib.Path, newline=None):
+    return read_str(path, encoding="utf-8", newline=newline)
 
 
 def read_file(callback, path: pathlib.Path, mode,
                 encoding=None, newline=None):
 
     root = find_zip_parent(path)
 
@@ -290,7 +357,10 @@
                     f = f_zipext
 
                 return callback(f)
     else:
         with open_path(mode) as f:
             return callback(f)
 
+
+def read_file_utf8(callback, path: pathlib.Path, mode, newline=None):
+    return read_file(callback, path, mode, encoding="utf-8", newline=newline)
```

### Comparing `modelx-0.8.0/modelx/testing/testutil.py` & `modelx-0.9.0/modelx/testing/testutil.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/api/test_api.py` & `modelx-0.9.0/modelx/tests/core/api/test_api.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/api/test_cur_model.py` & `modelx-0.9.0/modelx/tests/core/api/test_cur_model.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/api/test_defcells.py` & `modelx-0.9.0/modelx/tests/core/api/test_defcells.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/api/test_stacktrace.py` & `modelx-0.9.0/modelx/tests/core/api/test_stacktrace.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/api/test_traceback.py` & `modelx-0.9.0/modelx/tests/core/api/test_traceback.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/base/test_impl.py` & `modelx-0.9.0/modelx/tests/core/base/test_impl.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/base/test_interface.py` & `modelx-0.9.0/modelx/tests/core/base/test_interface.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/base/test_lazyeval.py` & `modelx-0.9.0/modelx/tests/core/base/test_lazyeval.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/base/test_repr.py` & `modelx-0.9.0/modelx/tests/core/base/test_repr.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/base/test_view.py` & `modelx-0.9.0/modelx/tests/core/base/test_view.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/conftest.py` & `modelx-0.9.0/modelx/tests/core/cells/conftest.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/node/test_itemproxy.py` & `modelx-0.9.0/modelx/tests/core/cells/node/test_itemproxy.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/node/test_node_repr.py` & `modelx-0.9.0/modelx/tests/core/cells/node/test_node_repr.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_cells.py` & `modelx-0.9.0/modelx/tests/core/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_cells_clear.py` & `modelx-0.9.0/modelx/tests/core/cells/test_cells_clear.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_cells_inheritance.py` & `modelx-0.9.0/modelx/tests/core/cells/test_cells_inheritance.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_cells_property.py` & `modelx-0.9.0/modelx/tests/core/cells/test_cells_property.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_cells_repr.py` & `modelx-0.9.0/modelx/tests/core/cells/test_cells_repr.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_cells_setitem.py` & `modelx-0.9.0/modelx/tests/core/cells/test_cells_setitem.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_copy.py` & `modelx-0.9.0/modelx/tests/core/cells/test_copy.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import modelx as mx
-import pytest
-import itertools
-
-
-@pytest.fixture(params=["foo", "bar"])
-def samplecells(request):
-
-    m, s = mx.new_model(), mx.new_space("Source")
-
-    @mx.defcells
-    def foo(x):
-        return x
-
-    foo[0] = 1
-    s.new_cells("bar", lambda x: 2 * x)
-    s.bar[0] = 1
-    return s.cells[request.param]
-
-
-@pytest.mark.parametrize(
-    "to_another_model, name",
-    list(itertools.product([False, True], [None, "baz"])))
-def test_copy(samplecells, to_another_model, name):
-
-    src = samplecells
-    m = mx.new_model() if to_another_model else samplecells.model
-    s2 = m.new_space()
-    samplecells.copy(s2, name=name)
-
-    assert s2.cells[name or src.name](0) == 1
+import modelx as mx
+import pytest
+import itertools
+
+
+@pytest.fixture(params=["foo", "bar"])
+def samplecells(request):
+
+    m, s = mx.new_model(), mx.new_space("Source")
+
+    @mx.defcells
+    def foo(x):
+        return x
+
+    foo[0] = 1
+    s.new_cells("bar", lambda x: 2 * x)
+    s.bar[0] = 1
+    return s.cells[request.param]
+
+
+@pytest.mark.parametrize(
+    "to_another_model, name",
+    list(itertools.product([False, True], [None, "baz"])))
+def test_copy(samplecells, to_another_model, name):
+
+    src = samplecells
+    m = mx.new_model() if to_another_model else samplecells.model
+    s2 = m.new_space()
+    samplecells.copy(s2, name=name)
+
+    assert s2.cells[name or src.name](0) == 1
     assert s2.cells[name or src.name](1) == src[1]
```

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_error.py` & `modelx-0.9.0/modelx/tests/core/cells/test_error.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_formula.py` & `modelx-0.9.0/modelx/tests/core/cells/test_formula.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_signature.py` & `modelx-0.9.0/modelx/tests/core/cells/test_signature.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/cells/test_valuecells.py` & `modelx-0.9.0/modelx/tests/core/cells/test_valuecells.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/conftest.py` & `modelx-0.9.0/modelx/tests/core/conftest.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/formula/test_formula.py` & `modelx-0.9.0/modelx/tests/core/formula/test_formula.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/model/test_model.py` & `modelx-0.9.0/modelx/tests/core/model/test_model.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/model/test_model_pickle.py` & `modelx-0.9.0/modelx/tests/core/model/test_model_pickle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from textwrap import dedent
 import pytest
-import pickle
 import builtins
+import io
 
 from modelx.core.api import *
 from modelx.core import mxsys
-
+from modelx.core.system import SystemPickler, SystemUnpickler
 
 # ---- Test impl ----
 
 
 @pytest.fixture
 def pickletest():
 
@@ -31,16 +31,18 @@
     )
 
     func1 = space.new_cells(formula=func1)
     func2 = space.new_cells(formula=func2)
 
     func2(5)
 
-    byte_obj = pickle.dumps(model._impl)
-    unpickled = pickle.loads(byte_obj)
+    f = io.BytesIO()
+    SystemPickler(f).dump(model._impl)
+    f.seek(0)
+    unpickled = SystemUnpickler(f, mxsys).load()
 
     return [model._impl, unpickled]
 
 
 def test_unpickled_model(pickletest):
 
     model, unpickeld = pickletest
@@ -76,17 +78,19 @@
     )
 
     model, space = new_model(), new_space(name="Space1", formula=param)
     space.new_cells(formula=fibo)
 
     check = space[2].fibo(3)
 
-    byte_obj = pickle.dumps(model._impl)
-    unpickled = pickle.loads(byte_obj)
-    unpickled.restore_state(mxsys)
+    f = io.BytesIO()
+    SystemPickler(f).dump(model._impl)
+    f.seek(0)
+    unpickled = SystemUnpickler(f, mxsys).load()
+    unpickled.restore_state()
     model = unpickled.interface
 
     return (model, check)
 
 
 def test_pickle_dynamicspace(pickletest_dynamicspace):
```

### Comparing `modelx-0.8.0/modelx/tests/core/reference/test_attrref.py` & `modelx-0.9.0/modelx/tests/core/reference/test_attrref.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/reference/test_clear_itemspaces.py` & `modelx-0.9.0/modelx/tests/core/reference/test_clear_itemspaces.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/reference/test_recalc.py` & `modelx-0.9.0/modelx/tests/core/reference/test_recalc.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/reference/test_recalc_dynamic_cells.py` & `modelx-0.9.0/modelx/tests/core/reference/test_recalc_dynamic_cells.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/reference/test_recalc_inherit.py` & `modelx-0.9.0/modelx/tests/core/reference/test_recalc_inherit.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/reference/test_ref_order.py` & `modelx-0.9.0/modelx/tests/core/reference/test_ref_order.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_base_ref_change.py` & `modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_base_ref_change.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_dynamic_spaces.py` & `modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_dynamic_spaces.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_param_formula.py` & `modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_param_formula.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/dynamic_spaces/test_space_parameters.py` & `modelx-0.9.0/modelx/tests/core/space/dynamic_spaces/test_space_parameters.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/element/test_element.py` & `modelx-0.9.0/modelx/tests/core/space/element/test_element.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/inheritance/test_add_bases.py` & `modelx-0.9.0/modelx/tests/core/space/inheritance/test_add_bases.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/inheritance/test_bases_change.py` & `modelx-0.9.0/modelx/tests/core/space/inheritance/test_bases_change.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/inheritance/test_del_base.py` & `modelx-0.9.0/modelx/tests/core/space/inheritance/test_del_base.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/inheritance/test_space_derived.py` & `modelx-0.9.0/modelx/tests/core/space/inheritance/test_space_derived.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/inheritance/test_space_inheritance.py` & `modelx-0.9.0/modelx/tests/core/space/inheritance/test_space_inheritance.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/itemspaceparent/conftest.py` & `modelx-0.9.0/modelx/tests/core/space/itemspaceparent/conftest.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/itemspaceparent/test_formula.py` & `modelx-0.9.0/modelx/tests/core/space/itemspaceparent/test_formula.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/itemspaceparent/test_itemspaces.py` & `modelx-0.9.0/modelx/tests/core/space/itemspaceparent/test_itemspaces.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/properties/test_spaces.py` & `modelx-0.9.0/modelx/tests/core/space/properties/test_spaces.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_copy.py` & `modelx-0.9.0/modelx/tests/core/space/test_copy.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_delattr.py` & `modelx-0.9.0/modelx/tests/core/space/test_delattr.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_new_cells_from_csv.py` & `modelx-0.9.0/modelx/tests/core/space/test_new_cells_from_csv.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_new_cells_from_excel.py` & `modelx-0.9.0/modelx/tests/core/space/test_new_cells_from_excel.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_new_cells_from_pandas.py` & `modelx-0.9.0/modelx/tests/core/space/test_new_cells_from_pandas.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_new_space_from_csv.py` & `modelx-0.9.0/modelx/tests/core/space/test_new_space_from_csv.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_new_space_from_excel.py` & `modelx-0.9.0/modelx/tests/core/space/test_new_space_from_excel.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_new_space_from_pandas.py` & `modelx-0.9.0/modelx/tests/core/space/test_new_space_from_pandas.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_space.py` & `modelx-0.9.0/modelx/tests/core/space/test_space.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_space_container.py` & `modelx-0.9.0/modelx/tests/core/space/test_space_container.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/space/test_space_reload.py` & `modelx-0.9.0/modelx/tests/core/space/test_space_reload.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/system/test_system.py` & `modelx-0.9.0/modelx/tests/core/system/test_system.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/system/test_thread.py` & `modelx-0.9.0/modelx/tests/core/system/test_thread.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/core/test_util.py` & `modelx-0.9.0/modelx/tests/core/test_util.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/io/test_excel.py` & `modelx-0.9.0/modelx/tests/io/test_excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-import modelx.io.excel as xl
+import modelx.io.excel_legacy as xl
 
 import pytest
 import openpyxl as opxl
 
 test_path = os.path.dirname(sys.modules[__name__].__file__)
 sample_book = test_path + "/test_xl_range.xlsx"
```

### Comparing `modelx-0.8.0/modelx/tests/io/test_pandas.py` & `modelx-0.9.0/modelx/tests/io/test_pandas.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/lifelib/test_serialize.py` & `modelx-0.9.0/modelx/tests/lifelib/test_serialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,28 +68,37 @@
 
 # @pytest.mark.skip()
 @pytest.mark.parametrize("project", _PROJECTS.keys())
 def test_with_lifelib(testpaths, project):
 
     build_path, write_path, zip_path = testpaths
 
-    from lifelib.commands import create
+    import lifelib
 
     testproj = project + "_test"
     projpath = build_path / testproj
 
-    create.main([
-        "--template",
-        project,
-        str(projpath)
-    ])
-
-    with SysPath(str(projpath.parent)):
-
-        module = importlib.import_module(testproj + "." + project)
+    if lifelib.VERSION > (0, 0, 14):
+        lifelib.create(project, projpath)
+        scriptpath = projpath / "scripts"
+    else:
+        from lifelib.commands import create
+        create.main([
+            "--template",
+            project,
+            str(projpath)
+        ])
+        scriptpath = projpath.parent
+
+    with SysPath(str(scriptpath)):
+
+        if lifelib.VERSION > (0, 0, 14):
+            module = importlib.import_module(project)
+        else:
+            module = importlib.import_module(testproj + "." + project)
 
         with SysPath(str(projpath)):
 
             m = module.build()
             m.hoge = "hoge"
             m.foo = 1
             m.bar = m.Input
```

### Comparing `modelx-0.8.0/modelx/tests/performance/test_performance.py` & `modelx-0.9.0/modelx/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_cells_from_csv.py` & `modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_cells_from_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         filepath=CSV_SINGLE_PARAM,
         cells=None,
         param=None,
         index_col=0
     )
     modelpath = tmp_path / "csv_single_param"
     getattr(mx, write_method)(m, modelpath)
-    assert ziputil.exists(modelpath.joinpath(CSV_SINGLE_PARAM.name))
+    assert ziputil.exists(modelpath / s.name / CSV_SINGLE_PARAM.name)
     m2 = mx.read_model(modelpath)
     # Write twice to check copy from renamed backup.
     getattr(mx, write_method)(m2, modelpath)
     m2 = mx.read_model(modelpath)
 
     # Compare components
     compare_model(m, m2)
@@ -50,15 +50,15 @@
         cells=None,
         param=None,
         index_col=[0, 1]
     )
 
     modelpath = tmp_path / "csv_mult_params"
     getattr(mx, write_method)(m, modelpath)
-    assert ziputil.exists(modelpath.joinpath(CSV_MULTI_PARAMS.name))
+    assert ziputil.exists(modelpath / s.name / CSV_MULTI_PARAMS.name)
     m2 = mx.read_model(modelpath)
 
     # Write twice to check copy from renamed backup.
     getattr(mx, write_method)(m2, modelpath)
     m2 = mx.read_model(modelpath)
 
     # Compare components
```

### Comparing `modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_cells_from_excel.py` & `modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_cells_from_excel.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_cells_from_pandas.py` & `modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_cells_from_pandas.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_space_from_csv.py` & `modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_space_from_csv.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_space_from_excel.py` & `modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_space_from_excel.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/construction_methods/test_new_space_from_pandas.py` & `modelx-0.9.0/modelx/tests/serialize/construction_methods/test_new_space_from_pandas.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/test_dynamic.py` & `modelx-0.9.0/modelx/tests/serialize/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/modelx/tests/serialize/test_log_input.py` & `modelx-0.9.0/modelx/tests/serialize/test_log_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import modelx as mx
 import pytest
 import itertools
+import zipfile
 from modelx.serialize import ziputil
 
 sample_log = """\
 SpaceA.SpaceB.foo(x=0)=Empty DataFrame
 Columns: []
 Index: []
 SpaceA.SpaceB.foo(x=2)=1
```

### Comparing `modelx-0.8.0/modelx/tests/serialize/test_serialize.py` & `modelx-0.9.0/modelx/tests/serialize/test_serialize.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+import zipfile
 import pytest
 from modelx import (
     write_model,
     read_model)
 from modelx.testing import testutil
 import modelx as mx
 
@@ -48,27 +49,32 @@
     return m
 
 
 @pytest.mark.parametrize(
     ["name", "version", "as_method", "write_method"],
     itertools.product(
         [None, "renamed"],
-        [2, 3],
+        [2, 3, 4],
         [True, False],
         ["write", "zip"]
     )
 )
 def test_read_write_model(testmodel, tmp_path, name, version, as_method,
                           write_method):
 
     path_ = tmp_path / "testdir"
     if as_method:
         getattr(testmodel, write_method)(path_)
     else:
-        getattr(mx, write_method + "_model")(testmodel, path_, version=version)
+        if as_method == "zip":
+            kwargs = dict(compression=zipfile.ZIP_STORED, version=version)
+        else:
+            kwargs = {}
+        getattr(mx, write_method + "_model")(
+            testmodel, path_, **kwargs)
     m = read_model(path_, name=name)
 
     assert m.name == (name if name else "TestModel")
     if name is None:
         testutil.compare_model(testmodel, m)
 
     # Check identities of modelx objects as refs
@@ -153,14 +159,41 @@
     assert m.SpaceA.u is m.SpaceB.ou[1]
 
     # Cells input data
     assert dict(m.SpaceA.foo) == {0: 0, 1: m}
     assert dict(m.SpaceA.lambdacells) == {0: "123", m.SpaceA: 3}
 
 
+@pytest.fixture(params=range(2))
+def combined_testmodel_fixture(testmodel, pickletest, request):
+    return [testmodel, pickletest][request.param]
+
+
+@pytest.mark.parametrize("meth_or_func, compression",
+                         itertools.product(["meth", "func"],
+                                           [zipfile.ZIP_DEFLATED,
+                                            zipfile.ZIP_STORED]))
+def test_zip_compression(
+        combined_testmodel_fixture, tmp_path, meth_or_func, compression):
+
+    model = combined_testmodel_fixture
+
+    if meth_or_func == "meth":
+        model.zip(tmp_path / "model.zip",
+                       compression=compression)
+    else:
+        mx.zip_model(model, tmp_path / "model.zip",
+                     compression=compression)
+
+    archive = zipfile.ZipFile(tmp_path / "model.zip")
+
+    for info in archive.infolist():
+        assert info.compress_type == compression
+
+
 @pytest.mark.parametrize("write_method", ["write_model", "zip_model"])
 def test_nested_space(tmp_path, write_method):
 
     m, s = mx.new_model(), mx.new_space()
     ns = s.new_space()
 
     @mx.defcells
```

### Comparing `modelx-0.8.0/modelx.egg-info/PKG-INFO` & `modelx-0.9.0/modelx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: modelx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Build and run complex models composed of formulas and data
 Home-page: https://github.com/fumitoh/modelx
 Author: Fumito Hamamura
 Author-email: fumito.ham@gmail.com
 License: LGPLv3
 Description: modelx
         ======
```

### Comparing `modelx-0.8.0/modelx.egg-info/SOURCES.txt` & `modelx-0.9.0/modelx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,27 @@
 modelx/core/node.py
 modelx/core/reference.py
 modelx/core/space.py
 modelx/core/spacecontainer.py
 modelx/core/system.py
 modelx/core/util.py
 modelx/io/__init__.py
-modelx/io/excel.py
+modelx/io/baseio.py
+modelx/io/excel_legacy.py
+modelx/io/excelio.py
 modelx/io/pandas.py
 modelx/qtgui/__init__.py
 modelx/qtgui/api.py
 modelx/qtgui/modeltree.py
 modelx/serialize/__init__.py
 modelx/serialize/jsonvalues.py
 modelx/serialize/serializer_1.py
 modelx/serialize/serializer_2.py
 modelx/serialize/serializer_3.py
+modelx/serialize/serializer_4.py
 modelx/serialize/ziputil.py
 modelx/testing/__init__.py
 modelx/testing/testutil.py
 modelx/tests/__init__.py
 modelx/tests/core/__init__.py
 modelx/tests/core/conftest.py
 modelx/tests/core/test_util.py
@@ -121,14 +124,15 @@
 modelx/tests/core/space/properties/__init__.py
 modelx/tests/core/space/properties/test_spaces.py
 modelx/tests/core/system/__init__.py
 modelx/tests/core/system/test_system.py
 modelx/tests/core/system/test_thread.py
 modelx/tests/io/__init__.py
 modelx/tests/io/test_excel.py
+modelx/tests/io/test_excelio.py
 modelx/tests/io/test_pandas.py
 modelx/tests/lifelib/__init__.py
 modelx/tests/lifelib/test_serialize.py
 modelx/tests/performance/__init__.py
 modelx/tests/performance/test_performance.py
 modelx/tests/serialize/__init__.py
 modelx/tests/serialize/test_dynamic.py
```

### Comparing `modelx-0.8.0/samples/dynamic_reference.py` & `modelx-0.9.0/samples/dynamic_reference.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/netprem/commutation_funcs.py` & `modelx-0.9.0/samples/netprem/commutation_funcs.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/netprem/model.py` & `modelx-0.9.0/samples/netprem/model.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/sample_actuarialmodel.py` & `modelx-0.9.0/samples/sample_actuarialmodel.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/sample_firststep.py` & `modelx-0.9.0/samples/sample_firststep.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/sample_loan.py` & `modelx-0.9.0/samples/sample_loan.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/sample_model.py` & `modelx-0.9.0/samples/sample_model.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/samples/sample_zero_bond.py` & `modelx-0.9.0/samples/sample_zero_bond.py`

 * *Files identical despite different names*

### Comparing `modelx-0.8.0/setup.py` & `modelx-0.9.0/setup.py`

 * *Files identical despite different names*

